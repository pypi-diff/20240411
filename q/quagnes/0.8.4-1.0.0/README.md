# Comparing `tmp/quagnes-0.8.4.tar.gz` & `tmp/quagnes-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quagnes-0.8.4.tar", last modified: Mon Apr  1 04:15:02 2024, max compression
+gzip compressed data, was "quagnes-1.0.0.tar", last modified: Thu Apr 11 05:16:29 2024, max compression
```

## Comparing `quagnes-0.8.4.tar` & `quagnes-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-01 04:15:02.186804 quagnes-0.8.4/
--rw-------   0 yar       (1000) yar       (1000)    35149 2024-03-02 00:03:19.000000 quagnes-0.8.4/LICENSE.txt
--rw-r--r--   0 yar       (1000) yar       (1000)    63635 2024-04-01 04:15:02.186804 quagnes-0.8.4/PKG-INFO
--rw-------   0 yar       (1000) yar       (1000)    22327 2024-04-01 04:13:09.000000 quagnes-0.8.4/README.md
--rw-------   0 yar       (1000) yar       (1000)      936 2024-04-01 04:08:50.000000 quagnes-0.8.4/pyproject.toml
--rw-r--r--   0 yar       (1000) yar       (1000)       38 2024-04-01 04:15:02.186804 quagnes-0.8.4/setup.cfg
-drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-01 04:15:02.150803 quagnes-0.8.4/src/
-drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-01 04:15:02.150803 quagnes-0.8.4/src/quagnes/
--rw-------   0 yar       (1000) yar       (1000)     3655 2024-04-01 04:09:04.000000 quagnes-0.8.4/src/quagnes/__init__.py
--rw-------   0 yar       (1000) yar       (1000)    54057 2024-03-29 02:24:20.000000 quagnes-0.8.4/src/quagnes/agnes.py
-drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-01 04:15:02.186804 quagnes-0.8.4/src/quagnes.egg-info/
--rw-r--r--   0 yar       (1000) yar       (1000)    63635 2024-04-01 04:15:02.000000 quagnes-0.8.4/src/quagnes.egg-info/PKG-INFO
--rw-------   0 yar       (1000) yar       (1000)      221 2024-04-01 04:15:02.000000 quagnes-0.8.4/src/quagnes.egg-info/SOURCES.txt
--rw-------   0 yar       (1000) yar       (1000)        1 2024-04-01 04:15:02.000000 quagnes-0.8.4/src/quagnes.egg-info/dependency_links.txt
--rw-------   0 yar       (1000) yar       (1000)        8 2024-04-01 04:15:02.000000 quagnes-0.8.4/src/quagnes.egg-info/top_level.txt
+drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-11 05:16:29.317278 quagnes-1.0.0/
+-r--------   0 yar       (1000) yar       (1000)    35149 2024-03-02 00:03:19.000000 quagnes-1.0.0/LICENSE.txt
+-rw-r--r--   0 yar       (1000) yar       (1000)    52358 2024-04-11 05:16:29.317278 quagnes-1.0.0/PKG-INFO
+-rwx------   0 yar       (1000) yar       (1000)    11050 2024-04-11 05:11:49.000000 quagnes-1.0.0/README.md
+-r--------   0 yar       (1000) yar       (1000)      936 2024-04-04 01:20:53.000000 quagnes-1.0.0/pyproject.toml
+-rw-r--r--   0 yar       (1000) yar       (1000)       38 2024-04-11 05:16:29.317278 quagnes-1.0.0/setup.cfg
+drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-11 05:16:29.313278 quagnes-1.0.0/src/
+drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-11 05:16:29.317278 quagnes-1.0.0/src/quagnes/
+-r-x------   0 yar       (1000) yar       (1000)     3655 2024-04-04 01:20:36.000000 quagnes-1.0.0/src/quagnes/__init__.py
+-rwx------   0 yar       (1000) yar       (1000)    77947 2024-04-10 14:43:47.000000 quagnes-1.0.0/src/quagnes/agnes.py
+drwxr-xr-x   0 yar       (1000) yar       (1000)        0 2024-04-11 05:16:29.317278 quagnes-1.0.0/src/quagnes.egg-info/
+-rw-r--r--   0 yar       (1000) yar       (1000)    52358 2024-04-11 05:16:29.000000 quagnes-1.0.0/src/quagnes.egg-info/PKG-INFO
+-rw-------   0 yar       (1000) yar       (1000)      221 2024-04-11 05:16:29.000000 quagnes-1.0.0/src/quagnes.egg-info/SOURCES.txt
+-rw-------   0 yar       (1000) yar       (1000)        1 2024-04-11 05:16:29.000000 quagnes-1.0.0/src/quagnes.egg-info/dependency_links.txt
+-rw-------   0 yar       (1000) yar       (1000)        8 2024-04-11 05:16:29.000000 quagnes-1.0.0/src/quagnes.egg-info/top_level.txt
```

### Comparing `quagnes-0.8.4/LICENSE.txt` & `quagnes-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `quagnes-0.8.4/PKG-INFO` & `quagnes-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quagnes
-Version: 0.8.4
+Version: 1.0.0
 Summary: This package solves Agnes (Agnes Sorel) solitaire card games. It can be used to solve games having the rules implemented in the GNOME AisleRiot package and the rules attributed to Dalton in 1909 and Parlett in 1979 among others and to calculate win rates.
 Author-email: Ray Griner <rgriner_fwd@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -714,389 +714,169 @@
     rc = new_game.play()
 
     # Write the return code and selected attributes from the game
     out_str = (str(rc) + ',' +
         ','.join([ str(getattr(new_game, attr)) for attr in attributes ]))
     print(out_str, flush=True)
 
-    # rc==1 are games that were won
-    if rc==1:
-        f = open(f'winners/win{rep}.txt', 'w', encoding='utf-8')
-        f.write(new_game.print_history())
-        f.close()
+    # rc==1 are games that were won, but probably best to only print a
+    # limited number for debugging or for rule variants when
+    # win rate is low
+
+    #if rc==1:
+    #    f = open(f'winners/win{rep}.txt', 'w', encoding='utf-8')
+    #    fwrite(new_game.print_history())
+    #    f.close()
 ```
 
 # Release Notes
-## Version 0.8.4
-- Copy editing of README.md and correct Wolter win rate to 45/1000000.
+## Version 1.0.0
+- Change name of `split_same_suit_runs` parameter to `split_runs` and make
+  parameter applicable regardless of the value of `move_same_suit`.
+- Add optimization for use when the losing state set is disabled.
+Track for each pile the last move depth, the number of cards
+moved, whether the pile was moved from or to, and whether the bottom card
+in the moved pile could be played to the foundation at the time of the move.
+Do not allow moves that: (a) reverse a previous tableau move without an
+intervening move to foundation or deal; (b) make the last deal after a
+tableau move where neither pile is dealt to and neither file had a card
+played to foundation; (c) play the bottom card of the moved pile to the
+foundation after the tableau move if it could have been played at the time
+of the move (and there has been no subsequent move to the pile or deal
+onto the pile).  These optimizations are only employed when the losing
+states set is
+disabled, as they use information not stored in the losing states set to
+determine whether a move can be played.
+- Add optimization when moves to empty piles allow zero or multiple cards
+to reduce the space of moves to consider when the stock is empty or near
+empty (without
+changing the win possibility or maximum score that can be attained). In
+these rules, we use the term 'top card' to describe the highest-rank card
+in the pile being moved and 'same-color top card' to be the card with equal
+rank in the same-color suit. The rules are: (a) when moving runs by suit,
+never split a run between same-suit cards when the stock is empty;
+(b) never split a run between same-suit cards when neither pile can be
+covered by a future deal and the same-color top card is in the foundation;
+(c) when the stock is empty, force a move onto a card of the same suit
+where possible when we know the target pile cannot be needed to move the
+same-color top card (ie, the same-color top card is already in the
+foundation or in same-suit sequence or the card one rank higher than the
+same-color top card is already exposed at the bottom of a pile); (d) when
+the stock is empty, force a move to the foundation if the card being
+moved cannot be needed as a target to be moved onto (ie, if the card in the
+same-color suit that is one rank lower is already in the foundation or in
+same-suit sequence).
+- Add new attributes created for these two optimizations in `_AgnesState` class (`in_suit_seq`, `last_in_pile`,
+  `_all_lmi`) and to output printed when state is printed.
+- Add `_AgnesState.hash_str` attribute to store the string representing
+  the hash of the object that will be stored in the losing states and
+  check loop set. Add `_Agnes_state.update_hash_str()` function called
+  after move is performed or undone to save the string in `hash_str`.
+  Previously, the `hash_str` was recalculated multiple times.
+- Fix bug in `Agnes.print_history` as only half the history was being
+  printed.
+- Use a single set to track whether loop has occured rather than a stack of
+  sets. Save result of check whether state is in the losing states set
+  so that we do not inefficiently (re-)insert the state into the losing
+  states set. Add attributes `is_loop` and `is_loser` to `_AgnesState`
+  class to support this logic.
+- Created for C++ implementation. Move detailed information
+  on the background, game rules, program methodology, and analysis of
+  win rates to that repository from this README. Add win rates
+  for rule variants where the empty rule is *AnyRun* or *HighRun*.
+
+# External Documentation
+A C++ implementation written by this package author also exists in a git
+repository.  Detailed information on the background, game rules, program
+methodology, and analysis of win rates are available [there](https://github.com/ghrgriner/quagnes-cpp/wiki/Rules,-Methodology,-and-Analysis-of-Win-Rates).
+
+# Using the Package
+Games are simulated by creating an `Agnes` object with the appropriate
+parameters, running `Agnes.play()`, and then using the return code and
+extracting desired statistics from `Agnes` class attributes.
+
+## Input Parameters
+The following are the parameters used to construct `Agnes` objects:
+
+|Parameter | Type | Description |
+|:-------- | :----- | :---------  |
+|`deck_filename` | `str` | Read deck from text file. If empty, a random deck will be used by calling `random.shuffle` and reversing the results. The text file should consist of 52 lines with each line formatted as `(rank, suit)`, where rank is in {0, 1, ..., 12} and suit is in {0, 1, 2, 3}. Suits are the same color if their value is equal modulus 2. The first card dealt is the base card.|
+|`move_to_empty_pile`| `str` | Rule for what can be moved to empty tableau piles. See following table for valid values.|
+|`move_same_suit`| `boolean` | If True, move runs by suit. If False (default), move runs by color.|
+|`split_runs` | `boolean` | If True, movable runs must be moved in their entirety. If False (default), a movable run can be split for a move).|
+|`face_up`| `boolean` |  If True, deal all cards face-up in the tableau. If False (default), only the last card in each column. |
+|`track_threshold`| `int` | If the number of cards left in the stock is greater than or equal to this value (default = 0), track losing states in a single set for the whole game. This set can consume a lot of memory if some of the other options are chosen that allow a large number of moves (eg, `move_to_empty_pile != 'none'`).|
+| `print_states` | `boolean` | Print detailed information about each state as moves are performed and undone. |
+| `maximize_score` | `boolean` | Maximize score. Disable optimization that inspects the layout of highest-ranked cards in the tableau to determine if game is unwinnable. |
+| `max_states` | `int` | Terminate game with return code 3 when number of states examined exceeds this threshold. 0 (default) means no threshold is used.|
+
+### Rule for Moving to Empty Piles
+|Value of `move_to_empty_pile` | Description |
+|:-------- | :---------  |
+|`'none'` | Empty piles can only be filled when dealing from stock (default). |
+|`'any run'` | Empty piles can be filled by any movable card or movable run. |
+|`'high run'` | Empty piles can be filled by any movable highest-rank card or movable run starting with a highest-rank card. |
+|`'any 1'` | Empty piles can be filled by any movable single card, but not by a movable run of more than one card. |
+|`'high 1'` | Empty piles can be filled by a single movable highest-rank card, but not by a movable run of more than one card. |
+
+## Output
+### `Agnes.play()` Return Code and `Agnes` Attributes
+The return code of the `Agnes.play()` function indicates whether the game is
+winnable (return code = 1), not winnable (return code = 2), or the
+simulation was terminated due to reaching the maximum number of states
+specified by the `max_states` parameter (return code = 3). The `Agnes`
+object has attributes with the same name and type as the input parameters
+that store the values of the parameters used during object construction.
+In addition, the following attributes of `Agnes` are updated when
+`Agnes.play()` is executed:
+
+| Attribute | Description |
+| :------------   | :---------  |
+| `n_states_checked` | Count number of states checked (including repeats). |
+| `n_deal` | Count number of deals performed (including those undone). |
+| `n_foundation` | Count number of moves to foundation performed (including those undone). |
+| `n_move_card_in_tableau` | Count number of moves in tableau performed (including those undone). |
+| `max_score` | Maximum score found during play. (If moving to empty piles is not allowed, this will not be the true maximum, unless `-z` was specified to disable the optimization that tries to detect unwinnable games from the location of the highest-rank cards in the tableau.) |
+| `max_depth` | Maximum depth of the search tree of moves. |
+| `current_depth` | Depth of the search tree when the game was terminated. This value is always 0 for losing games. |
+
+### Detailed Program Output
+When `print_states=True` for the `Agnes` object, `Agnes.play()` will print
+to standard output each state as moves are performed or undone.
 
-## Version 0.8.3
-- Copy editing of README.md
+```
+Move: Move 2 card(s) from pile 1 to pile 3
+
+piles:16#9-8-7##49-19-44##28-51-15-31##3-33-14-5-30-29##45-23-35##43-34-42-0-13-48-47-50##20-21-41-2-37#
+depth:11, n_stock_left:16, valid_moves:[DealMove(), TablMove(from_=3, n_cards=2, to_=2, expose=False, tabltype=2)]
+Foundations:[-1, -1, 1, 1]
+T0:[] | [(9, 0), (8, 0), (7, 0)]
+T1:[] | [(10, 3), (6, 1), (5, 3)]
+T2:[] | [(2, 2), (12, 3), (2, 1), (5, 2)]
+T3:[] | [(3, 0), (7, 2), (1, 1), (5, 0), (4, 2), (3, 2)]
+T4:[] | [(6, 3), (10, 1), (9, 2)]
+T5:[] | [(4, 3), (8, 2), (3, 3), (0, 0), (0, 1), (9, 3), (8, 3), (11, 3)]
+T6:[] | [(7, 1), (8, 1), (2, 3), (2, 0), (11, 2)]
+in_suit_seq:0011 0011 0000 0010 0010 0000 0000 1000 1001 0000 0000 0000 0000
+last_in_pile:0011 0011 0000 0010 0000 0011 0000 1000 0000 0010 0000 0011 0000
+
+Last move info:[10-2-T-T, 11-2-F-T, 0-0-F-T, 11-2-T-T, 10-2-F-T, 0-0-F-T, 9-1-F-T]
+```
 
-## Version 0.8.2
-- Bug fix: add check for loops when `move_to_empty_pile != 'none'` in
-addition to the existing check when `split_same_suit_runs=True`.
-- Add Optimizations #6 and #7 listed below.
-- When printing a state, add a single line with a string that has the
-  same values stored in the set of losing states. This alllows the user
-  to easily search in the output for when the previous state occurred.
-  Note that a more compressed version of this string (one byte per
-  card) is stored in the set of losing states. A longer version is
-  printed that avoids characters that are special in regular expressions
-  to facilitate searching. 
-- Remove extensive description of the rules from the module docstring.
-
-# Background
-Agnes is a difficult solitaire card game under some rule variants. This
-package solves the game automatically.
-
-Users can simulate random games and calculate win rates under various
-permutations of rules, including moving sequences (runs) by same-suit or
-same-color, allowing or not same-suit runs to be split in the middle of the
-run for a move, dealing all tableau cards face-up at the start versus
-dealing only the final tableau card face-up, and whether and how empty
-columns can be filled in between deals (never, a single card of any rank, a
-single card of the highest rank, a run starting with a single card of any
-rank, or a run starting with a card of the highest rank). The package
-provides additional options for debugging and tuning of the search algorithm
-to be more memory-efficient at the expense of speed.
-
-In 1979 Parlett named the two main variants of Agnes as Agnes Sorel (the
-variant / set of variants described here) and Agnes Bernauer (a variant/set
-of variants that uses a reserve) [3]. This package only considers Agnes
-Sorel.
-
-Some analyses of win rates for Agnes Sorel has previously been conducted.
-Wolter published an experimental analysis of the win rates of this and
-other solitaires, reporting 45 winnable games in a million deals under 
-presumably the *Up-Suit-None* rules (defined below) [4]. Masten modified
-Wolter's solver and reported 900/100,000 (0.9%) games were winnable when
-empty columns could not be filled by any card, although it is unclear
-whether same-suit runs could be split during a move [5]. In this
-analysis, we conduct our own simulations to estimate win rates, assess
-agreement with Wolter and Masten and add win rates for other
-rule variants. As in the prior analyses, the win rates calculated here are
-under perfect play (i.e., the solver is allowed to undo losing moves).
-
-# Rules
-There is considerable heterogeneity in the rules that have been proposed
-for Agnes (see Wikipedia [1] and Keller [6] for some discussion of the 
-history). We describe first the rules according to Dalton [1-2] and
-variations that change only the handling of play on empty piles. The other
-main set of variants allow moving of same-color runs instead of
-same-suit runs. We describe the parameter settings to be used in our
-software when playing the different rule variants.
-
-Because our interest in the problem arose from playing the game in the GNOME
-AisleRiot package, the default parameters correspond to this variant.
-
-## Dalton (1909)
-The first description is of the game is attributed to Dalton in 1909 [1-2].
-We implement his rules, except most software we have seen have the tableau
-piles ascending in length from left to right, so we follow that convention,
-rather than the right to left described by Dalton. (It should be noted that
-symmetry cannot be used to claim the win rates are identical under this
-variation because only the first two piles are dealt to in the final deal.)
-The rules are the following:
-
-Deal seven piles as columns face-up in the tableau such that the first pile
-has one card and the last column has seven. Then, deal a single card and
-place it above the tableau in the foundation (base card). Foundations are
-built up by suit and the tableau is built down by color. Wrap from king to
-ace when necessary. Piles of cards in sequence in the same suit can be
-moved in the tableau. The top card in each tableau pile is exposed and can
-be moved to a different pile (if it has the appropriate color and rank) or
-to the foundation. If a movable run occurs by chance at the start of
-the game or after a deal, the run can also be moved. When a card or
-pile is moved, the card in the column above it becomes exposed and
-available for play. Empty tableau piles can be filled by any card or
-movable run, or they can be left empty. Dealing from the stock adds one
-card to the bottom of each tableau pile before play resumes, so a game will
-have three more deals of seven cards and a final deal of two cards. Cards
-cannot be played back from the foundation to the tableau.
-
-Note that while Dalton used the singular when saying 'Any exposed card may
-be moved into a vacant space [pile]', in the example game he plays, he moves
-a group of cards into an empty pile. We follow the latter interpretation.
-
-Dalton states that at the start the bottom card of each pile is exposed and
-doesn't explicitly state what is permitted if a movable run occurs by
-chance. However, in the sample game he plays, he does not distinguish
-between cards that appeared at the bottom of the column at the start versus
-those that did not, so we adopt the interpretation that runs may be
-moved even if they first occurred by chance. This is consistent with the
-software implementations we have seen.
-
-The game as described above can be played by specifying the parameters
-`move_same_suit=True`, `face_up=True`, and `move_to_empty_pile='any run'`.
-
-We denote the rules above as *Up-Suit-AnyRun*. The third part of
-each name is because many variants have evolved that alter what can be done
-with empty piles. We refer to these as:
-
-- *Up-Suit-None*: Empty piles can only be filled when dealing from stock.
-- *Up-Suit-Any1*: Empty piles can be filled by any single card, but not by
-  a movable run.
-- *Up-Suit-HighRun*: Empty piles can be filled a single highest rank card, or
-a run starting with the highest rank card (i.e., if the base card was a seven,
-an empty pile can be filled only with a six or run starting with a six).
-- *Up-Suit-High1*: Empty piles can be filled by a single highest rank card.
-
-The `move_to_empty_pile` parameter takes the values `'none'` (default), 
-`'any 1'`, `'high run'`, and `'high 1'`, respectively, for the above four
-variants.
-
-## Parlett (1979) and *NoSplit* variants
-Parlett gives rules like *Up-Suit-None* but also forbids splitting same
-suit runs (`split_same_suit_runs=False`) [3]. We denote this as 
-*Up-Suit-None-NoSplit*. We also allow other rules that move by suit to
-have this option and denote these by adding *-NoSplit* to the end of
-of the rule name.
-
-## *Down-Color* and *Up-Color* variants
-Among this group, the primary variant of interest is *Down-Color-None*,
-which corresponds to the game as played on AisleRiot, which is where we
-became interested in the game. We verified the rules on the current
-AisleRiot version 3.22.23.
-
-The first variation from the Dalton rules is that cards are dealt
-face down in the tableau except for the final card dealt in each pile.
-We start these variant names with *Down-* instead of *Up-*.
-The second variation is that runs may be moved if they are the
-same color instead of requiring they be the same suit. We use *-Color-*
-as the second part of the variant name to indicate this. The third
-part of the variant name is as described for the Dalton variants.
-
-Other variants of interest in this class are *Up-Color-AnyRun*. This and
-*Up-Color-None* match the rules described on the website poltaire.com,
-which offers solitaire play [7]. This site is of interest to us as it hosts
-an article by Wolter [4] that analyzes the winnability of the game as
-played on the site.
-
-# Methodology
-## Optimizations
-The following optimizations were used to improve the run-time over a naive
-depth-first search of all possible moves:
-
-1. When `move_to_empty_pile='none'`, if the highest rank card (e.g., a king
-if the base card is an ace) is placed in a tableau pile below a lower card
-of the same suit, the lower card can never be moved from the pile. This is
-detected as soon as the king is placed. Therefore, some games can be
-determined to be not winnable by examining only the starting layout. Note
-while this optimization improves run time, it is not possible to determine
-the maximum possible score if a branch is terminated for this reason. This
-concept can be extended by noting that if the king of clubs blocks the
-queen of hearts and the king of hearts blocks the queen of clubs, the game
-is also unwinnable. In general, we define after each deal a four vertex
-graph (one vertex for each suit), where an edge denotes which suits are
-blocked by the suit corresponding to the vertex. The state is not winnable
-if a cycle exists in the graph. This only needs to be checked after a deal.
-This optimization is disabled when `move_to_empty_pile != 'none'` or when
-`maximize_score=True`.
-
-2. A card is immediately placed on a foundation if its rank is no more than
-the rank of the top foundation card of the same color suit plus two. For
-example, if the base card is an ace, and we have already played up to the
-six of spades in the foundation, we immediately play the ace of clubs up
-to the eight of clubs (if possible) to the foundation. We would not
-immediately play the nine of clubs to the foundation as it might be
-needed in the tableau to move the eight of spades.
-
-3. We track states that we have already determined to be not winnable in
-a set. For example, suppose the initial state has two possible moves: M1)
-move a card from pile 1 to 2; M2) move a card from pile 4 to 5. Once we
-determine the sequence M1 → M2 is not winnable, there is no need to check
-the sequence M2 → M1, as they both result in the same state. This
-optimization can be tuned using the `track_threshold` parameter.
-
-4. To prevent infinite loops, we use a stack of sets that stores the state of
-the game (number of cards in the stock and arrangement of cards in the tableau)
-and check whether this has been repeated since the last deal or move to
-foundation.  If the state is a repeat, we consider no valid moves to be
-available at the repeated state. This second method is disabled if
-`split_same_suit_runs=False` and `move_to_empty_pile 'none'}`, as loops
-cannot occur under this combination of parameter settings.
-
-<!--- First, we track for each pile the last move number (i.e., the number of
-plays
-since the start of the game the pile was last involved in a move between
-tableau piles). This is set to zero at the start of the game and when a card
-is moved from the pile to the foundation or when the pile is dealt to. A move
-between two piles is not permitted if the last move numbers match and are
-greater than zero and the target pile is not empty (as this implies we have
-reversed a previously executed move). -->
-5. The simulation is implemented using two or three equal-length stacks
-where the nth item describes an aspect of the state of the game at the
-nth move.  These three stacks store: (1) the moves performed, (2) the valid
-moves not yet attempted, and (3) a set containing the arrangement of all
-tableau layouts that have occurred since the last deal or move to foundation.
-A single state object (`_AgnesState`) in the `Agnes` object initially
-stores information about the starting state, such as the cards in the
-foundation, the arrangement of cards in the tableau, and the number of
-cards left in the stock. When a move is performed or undone, the
-`_AgnesState` object is updated in-place based on the move information.
-Initial testing found this implementation to be about 5–7 times faster than
-using a stack of `_AgnesState` objects, although this hasn't been retested
-after the addition of some of the other optimizations.
-
-7. If there are multiple empty columns in the tableau that cannot be
-covered by a future deal, then it doesn't matter which column is played
-in, so the first is always chosen. Similarly, we do not consider a move
-that moves the entirety of one column to a different empty column when
-both columns cannot be covered by a future deal.
-
-8. We do not allow splitting same-suit runs when the stock is empty
-regardless of the value of the `split_same_suit_runs` parameter, unless
-`move_to_empty_pile = 'any 1'` or `'high 1'`.
-
-Lastly, note that if win rate is the only output statistic of interest
-and results are being calculated for multiple rule sets, users can exploit
-the fact that all wins under some rule set is sometimes a subset of wins
-under another rule set. For example, any game winnable when 
-`split_same_suit_runs=False` is also winnable when
-`split_same_suit_runs=True` when other parameter values are fixed.
-
-## Statistical Analysis
-Ten thousand decks were simulated using this package version 8.0.2.
-We calculated the win rates and the 95% confidence intervals (95% CI)
-using the score (Wilson) method for the following rules:
-*Down-Color-None*, *Up-Color-None*, *Up-Suit-None*,
-*Up-Suit-None-NoSplit*, *Up-Suit-HighRun*, *Up-Suit-HighRun-NoSplit*,
-*Up-Suit-AnyRun*, *Up-Suit-AnyRun-NoSplit*. If a set of simulations
-consumed too much memory, the simulation was run setting a maximum
-number of states examined to 50 million, and win rates were
-calculated assuming all incomplete simulations were losses and 
-then again assuming all were wins.
-
-For each set of rules, the mean (standard deviation) and maximum number
-of states examined were also reported. This statistic counts repeated
-states each time they are created.
-
-Lastly, we calculated separate p-values testing the equality of our
-estimate with those published by Masten [5] and Wolter \[4\] (the latter
-only when the rule for empty piles was *None*). A Chi-square test or Fisher
-exact test was used, as appropriate.
-
-All simulations were run using a C++ port of this package. The
-first thousand simulations for each rule variant were also run using this
-Python package version 0.8.2 on Python version 3.11.2, and the simulation
-result (win, loss, exceeded maximum states) and number of states examined
-were confirmed to match the C++ version. A laptop running 32-bit
-Debian GNU/Linux 12 was used for the simulations. Statistical analyses
-were conducted in R v4.2.2.
-
-# Results
-The results of the simulations are shown in the table below.
-
-| Rule Variant              | Completed Simulations, (n) | Wins, n (% [95% CI])    | P-value [a] | Mean (SD) States Examined (10^3) | Maximum States Examined (10^6) |
-| :------------------------ | :--------------: | :---------------------: | :---------: | :-------------------:     | :-----------------: |
-| *Down-Color-None*         | 10,000           | 99 (1.0% [0.8%, 1.2%])  | 0.40        | 89.0 (156.1)              | 63.7                |
-| *Up-Color-None*           |  9,996 [b]       | 113 (1.1% [0.9%, 1.4%], 1.2% [1.0%, 1.4%]) | 0.02, 0.01 |  72.6 (112.8) | 46.3       |
-| *Up-Suit-None*            | 10,000           | 42 (0.4% [0.3%, 0.6%]   | <.0001      | 10.2 (163.9)              |  8.5                |
-| *Up-Suit-None-NoSplit*    | 10,000           | 40 (0.4% [0.3%, 0.5%])  | <.0001      | 5.9 (94.1)            |  6.1                |
-| *Up-Suit-HighRun*         | 10,000           | 1454 (14.5% [13.9%, 15.2%]) | 0.92    | 207.3 (999.3)         | 31.9                |
-| *Up-Suit-HighRun-NoSplit* | 10,000           | 1411 (14.1% [13.4%, 14.8%]) | 0.30    | 112.9 (500.9)         | 22.6                |
-| *Up-Suit-AnyRun-NoSplit*  | 10,000           | 6384 (63.8% [62.9%, 64.8%]) | 0.69    | 59.2 (340.2)          | 16.1                |
-
-[a] P-value for comparison vs Masten results.
-
-[b] Simulations stopped after 50,000,000 states examined. Win rates and P-values are reported twice assuming all incomplete simulations are losses and wins. Mean and maximum states examined are reported for completed simulations.
-
-# Discussion
-We found 1.1% - 1.2% of games were winnable under the *Up-Color-None* rules
-and 1.0% of games were winnable under the *Down-Color-None* rules. For the
-former, the comparison to Masten's results gave a statistically significant
-difference at the 95% confidence level while the latter did not.  Our
-simulations for *Up-Suit-HighRun*, *Up-Suit-HighRun-NoSplit*, and
-*Up-Suit-AnyRun-NoSplit* were not statistically significantly different from
-those of Masten, although *Up-Suit-None* and *Up-Suit-None-NoSplit* were.
-
-A limitation of using Masten's results is he states win rates but isn't
-explicit about which rules are used, with the exception of how empty
-piles are filled. He refers readers to Keller's discussion [6] for more
-information, and this discussion suggests that Agnes rules follow 
-Whitehead rules (another solitaire) and require movable runs to be
-the same suit. That is, Keller indicates the rules are *Up-Suit-None*
-in our terminology [5,6]. However, Keller then goes on to note that all
-computer implementations he had seen allow moves by colored runs and not
-by same-suit runs, which would corresponds to the *Up-Color-None* rules in
-our terminology. 
-
-It was unexpected to find that when the rule for empty piles is *None*, our
-results for dealing face-down and moving by color matched Masten, while
-when the rule for empty piles is *HighRun* or *AnyRun*, our results for
-dealing face-up and moving by suit matched. It is unclear if Masten 
-reported results for different move rules, if the statistically significant
-differences we found were due to chance, or if consistent rules were used
-for a variant we have not yet tested (e.g., *Up-Color-None-NoSplit*,
-*Up-Color-HighRun-NoSplit*, and *Up-Color-AnyRun-NoSplit*).
-
-Despite these uncertainties about Masten's estimates, we add 95% CIs to
-his reported win rates and include them here. He reports the previously
-mentioned win rate (95% CI) of 0.9% (0.8%, 1.0%) when empty
-columns cannot be filled with moves from the tableau, 63.6% (63.3%, 63.9%)
-when the empty column can be filled by any movable run or single card
-(or perhaps disallowing runs — Masten is not explicit, but our results
-match filling with a run or single card), and 14.5% (14.3%, 14.7%) when
-empty columns can be filled only by a run starting with the highest rank
-card or single highest-rank card (or again, perhaps disallowing runs).
-
-All of our results were larger than the 45/1,000,000 reported by Wolter
-at significance level P<.0001. Given the large difference between our
-results and Wolter's results, we believe Wolter's results are incorrect
-and should not be cited.
-
-We have estimated win rates that to our knowledge have not been previously
-reported for Parlett's variant (*Up-Suit-None-NoSplit*) and
-*Down-Color-None*, with the former less than half of *Up-Suit-None* and the
-latter about 10% smaller.
-
-Much of the work for this project was originally completed in 2019
-assuming all cards were dealt face-up using Python 3.5. This 2024 update
-used Python 3.11.2. In 2019 we ported the Python code to C++ for
-performance testing and found a five-fold improvement in speed. When
-porting the code to Python 3.11, we found a two-fold decrease in run-time
-when switching the data structures used from tuples to dataclasses for the
-structures representing cards and moves.
-
-We have not all possible rule variants with this package. We considered
-including *Up-Suit-AnyRun*, but preliminary estimates indicated 
-high memory usage and a longer run time, and therefore we defer analysis
-of this variant to a later package version. The current package has some options
-to manage the memory (e.g., disabling the set that tracking losing states
-at various thresholds), but additional optimizations are possible
-once the set is disabled that are not yet implemented (e.g., 
-requiring cards to be placed to the foundation before moving a pile that we
-hope will improve run time). In addition, the package options allow
-disabling of splitting same-suit runs before a move, but this option will
-likely be generalized to disallow splitting of movable runs and then
-can be applied when moves are allowed by color.
+A line-by-line explanation of this output is provided in [the git repository of the C++ implementation](https://github.com/ghrgriner/quagnes-cpp/wiki/Program-Input-and-Output#explanation-of-detailed-output).
+However, note that this Python package does not write any messages to
+standard error.
 
 # References
 [1] Agnes (card game). Wikipedia.
     https://en.wikipedia.org/wiki/Agnes_(card_game). Retrieved
     March 15, 2024.
 
 [2] Dalton W (1909). "My favourite Patiences" in The Strand Magazine,
     Vol 38.
 
 [3] Parlett D (1979). The Penguin Book of Patience. London: Penguin.
 
-[4] Wolter J (2013). Experimental analysis of Agnes Sorel solitaire.
-    https://politaire.com/article/agnessorel.html. Retrieved
-    March 15, 2024.
-
-[5] Masten M (2021). Agnes Sorel.
-    https://solitairewinrates.com/AgnesSorel.html. Retrieved
-    March 17, 2024.
-
-[6] Keller M (2021). Whitehead and Agnes -- packing in color.
-    https://www.solitairelaboratory.com/whitehead.html. Retrieved
-    March 17, 2024.
-
-[7] Wolter J (2014). Rules for Agnes Sorel solitaire.
-    https://politaire.com/help/agnessorel. Retrieved March 17, 2024.
-
 # Disclosures
 We are not affiliated with any of the books, websites, or applications
 discussed in this documentation, except of course for this Python package
-which we wrote.
+and previously-mentioned C++ implementation which we wrote.
```

### Comparing `quagnes-0.8.4/pyproject.toml` & `quagnes-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quagnes"
-version = "0.8.4"
+version = "1.0.0"
 authors = [{name = "Ray Griner", email = "rgriner_fwd@outlook.com"}]
 description = "This package solves Agnes (Agnes Sorel) solitaire card games. It can be used to solve games having the rules implemented in the GNOME AisleRiot package and the rules attributed to Dalton in 1909 and Parlett in 1979 among others and to calculate win rates."
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `quagnes-0.8.4/src/quagnes/__init__.py` & `quagnes-1.0.0/src/quagnes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,11 +90,11 @@
 #------------------------------------------------------------------------------
 # File:    __init__.py
 # Date:    2024-03-14
 # Author:  Ray Griner
 # Changes:
 #------------------------------------------------------------------------------
 __author__ = 'Ray Griner'
-__version__ = '0.8.4'
+__version__ = '1.0.0'
 __all__ = ['Agnes']
 
 from .agnes import Agnes
```

### Comparing `quagnes-0.8.4/src/quagnes/agnes.py` & `quagnes-1.0.0/src/quagnes/agnes.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,14 +55,64 @@
 #  (6) Add uncompressed printing of table state to make it each to search for
 #     prior state when print_states=`True`. When printing compressed string
 #     to store in the set, change to use '#' and '-' since the character code
 #     for these are not in the range of codes that will be used by cards (which
 #     start at ASCII code 48).
 #  (7) Do not allow splitting of any run (same-suit or otherwise) once the
 #     stock is empty, unless EmptyRule is 'any 1' or 'high 1'.
+# [20240403RG] (1) Change `split_same_suit_runs` constructor parameter and
+#  `Agnes` attribute to `split_runs` and use the same logic to decide
+#  whether run must be moved in its entirety when `move_same_suit=false`.
+#  (2) Add new class attributes needed for run-time optimizations
+#  (2a) Create `_all_lmi` attribute on `Agnes` that stores a stack of
+#     newly defined LastMoveInfo objects.
+#  (2b) Add `tabltype` attribute to Move objects and enum for this to store
+#     whether a tableau move joined or split a same-suit sequence (considering
+#     only the top card of the pile). Similarly used for moves to foundation.
+#  (2c) Added `last_in_pile` and `in_suit_seq` attributes to `_AgnesState`
+#     objects to store whether a card is the final card in a tableau pile
+#     (or in the foundation) or in an exposed pile under a same-suit card that
+#     has one higher rank, respectively. These are both implemented as 13x4
+#     arrays and are updated / undone for each move using the new attribute
+#     from change (2b).
+#  (2d) Added _dont_deal_last function
+#  (3) Optimzations:
+#  (3a) When stock is 0 and empty_rule not in 'any 1' or 'high 1'... then
+#    never split a run between the same suit, regardless of whether moving
+#    by suit or color.
+#  (3b) When stock is 0 and empty_rule not in 'any 1' or 'high 1'... then
+#    force joins by suit sequence if the same-color top card of the pile being
+#    moved is (i) already in the foundation or (ii) `move_same_suit=false` and
+#    already under the next-highest card of the same suit (`in_suit_seq`) or
+#    (iii) `move_same_suit=false` and the card from the same-color suit is
+#    also available to be played on (`last_in_pile`).
+#  (3c) Do not move a card to the foundation unless one of the following is
+#    true:
+#     - track_threshold <= n_stock_left (ie, we are still using the
+#       losing_states set)
+#     - last_move_info[from_pile].depth == 0, ie, last operation on the pile
+#       wasn't a move within tableau to or from this pile
+#     - last_move_info[from_pile].can_move_to_found = true, ie, if the last
+#       operation was a move to this pile, we set can_move_to_found = true if
+#       it was NOT possible to perform the move to foundation when the tableau
+#       move was done.
+# (3d) If track_threshold > n_stock_left, do not allow reversing a move
+#   between two piles if no other operations have been done on those piles.
+#   Reversing a move means moving the same number of cards back that were
+#   originally moved.
+# (3e) When track_threshold is > 2, do not deal last deal if there there are
+#   two columns that will not be covered by the final deal where we just moved
+#   from one to the other with no other operations. (This restriction forces us
+#   to only consider the case when such moves are done after the last deal.)
+# (3f) Additional restriction on splitting same suit besides those implied by
+#   `split_runs` (which were implemented in set_n_movable). Only allow splits
+#   of same suit if source or target will be covered by future deal, or
+#   `split_empty_stock=True` or Card(src_card.rank, same_color_suit(src_card))
+#   is not in the foundation, where src_card is the highest-rank card in the
+#   part of the pile that is being moved.
 #------------------------------------------------------------------------------
 """A module for solving Agnes solitaire. """
 
 import random
 import copy
 from typing import Set, Optional, Union, NamedTuple
 from dataclasses import dataclass
@@ -83,23 +133,59 @@
 #Card = tuple[CardRank, CardSuit]
 #Card = collections.namedtuple('Card', 'rank suit')
 #
 #class Card(NamedTuple):
 #    rank: CardRank
 #    suit: CardSuit
 
+# TODO:
+@dataclass(frozen=True, slots=True)
+class LastMoveInfo:
+    """Information about the last tableau move performed on a pile.
+
+    Attributes
+    ----------
+    depth : int
+        Depth at which the last tableau move to or from this pile was
+        performed. Set to 0 if no prior such move or when a move to
+        foundation or deal on the pile occurs.
+    n_moved : int
+        Number of cards moved during the last tableau move to or from
+        this pile. Set to 0 if depth is set to 0.
+    moved_to : bool
+        True if depth is not 0 and this was the pile moved to.
+    can_move_to_found : bool
+        Set to false if depth is not 0 and the bottom card in the run
+        being moved could have been put into the foundation before the
+        move. This is set on the pile that was moved to. Otherwise, true.
+    """
+    depth: int = 0
+    n_moved: int = 0
+    moved_to: bool = False
+    can_move_to_found: bool = True
+
 #@dataclass(frozen=True)
 class SetNMovableOpts(NamedTuple):
+    """Options to pass to the `set_n_movable` function.
+    """
     move_same_suit: bool
-    split_same_suit_runs: bool
+    split_runs: bool
     split_empty_stock: bool
 
 @dataclass(frozen=True, slots=True)
 class Card:
-    """Dataclass representing a card in the deck."""
+    """Dataclass representing a card in the deck.
+
+    Attributes
+    ----------
+    rank : CardRank
+        Rank of the card
+    suit : CardSuit
+        Suit of the card. Suits that are equal modulus 2 are the same color.
+    """
     rank: CardRank
     suit: CardSuit
 
     def __repr__(self) -> str:
         return f'({self.rank}, {self.suit})'
 
     # Represent a card as a single byte string
@@ -110,15 +196,15 @@
         """
         return str(chr(48+13*self.suit+self.rank))
 
     # Represent a card as a readable string
     def struncomp(self) -> str:
         """An uncompressed representation.
 
-           Used when printing the state in a machine readable form.
+           Used when printing the state for humans to read.
         """
         return str(13*self.suit+self.rank)
 
     def twochar(self) -> str:
         """Return a two character string representing the card, eg, '3♦'."""
         if self.rank==0:
             rank_str = 'A'
@@ -166,46 +252,113 @@
 
 @dataclass(frozen=True)
 class DealMove:
     """Dataclass representing a deal from the stock."""
     def __str__(self) -> str:
         return 'Deal'
 
+class TablType(Enum):
+    """Indicates if a tableau move splits or joins a same-suit sequence.
+
+    Also used for moves to foundation (NONE and SPLIT only).
+    """
+    NONE = 0
+    SPLIT = 1
+    JOIN = 2
+
 @dataclass(frozen=True, slots=True)
 class MoveToFound:
-    """Dataclass representing a move of one card to the foundation."""
+    """Dataclass representing a move of one card to the foundation.
+
+    Attributes
+    ----------
+    from_ : int
+        Pile from which the card was taken.
+    suit : CardSuit
+        Suit of the card being moved.
+    expose : bool
+        Indicates whether a hidden card was exposed after the move.
+    tabltype : TablType
+        Indicates whether the card being moved was in sequence under
+        a card of the same suit (TablType.SPLIT) or not (TablType.NONE).
+    """
     from_: int
     suit: CardSuit
     expose: bool
+    tabltype: TablType
 
     def __str__(self) -> str:
         str2 = ''
         str1 = (f'Move bottom card from pile {self.from_} to foundation '
                 f'{self.suit}')
         if self.expose:
             str2 = ' (exposes a card)'
         return str1 + str2
 
+    def __repr__(self) -> str:
+        retlist: list[str] =['MoveToFound(from_=', str(self.from_),
+            ', suit=', str(self.suit)]
+        if self.expose:
+            retlist.append(', expose=True')
+        else:
+            retlist.append(', expose=False')
+        retlist.append(', tabltype=')
+        retlist.append(str(self.tabltype.value))
+        retlist.append(')')
+        return ''.join(retlist)
+
 @dataclass(frozen=True, slots=True)
 class TablMove:
-    """Dataclass representing a move in the tableau."""
+    """Dataclass representing a move in the tableau.
+
+    Attributes
+    ----------
+    from_ : int
+        Pile from which the run was moved.
+    n_cards : int
+        Number of cards in the run that was moved.
+    to_ : int
+        Pile to which the run was moved.
+    expose : bool
+        Indicates whether a hidden card was exposed after the move.
+    tabltype : TablType
+        Indicates whether the highest-rank card in the run being moved was
+        in sequence under a card of the same suit (TablType.SPLIT) or
+        will be in such sequence after the move (TablType.JOIN) or neither
+        (TablType.NONE).
+    """
     from_: int
     n_cards: int
     to_: int
     expose: bool
+    tabltype: TablType
 
     def __str__(self) -> str:
         str2 = ''
         str1 = (f'Move {self.n_cards} card(s) from pile {self.from_} to pile '
                f'{self.to_}')
         if self.expose:
             str2 = ' (exposes a card)'
         return str1 + str2
 
+    def __repr__(self) -> str:
+        retlist: list[str] =['TablMove(from_=', str(self.from_),
+            ', n_cards=', str(self.n_cards), ', to_=', str(self.to_)]
+        if self.expose:
+            retlist.append(', expose=True')
+        else:
+            retlist.append(', expose=False')
+        retlist.append(', tabltype=')
+        retlist.append(str(self.tabltype.value))
+        retlist.append(')')
+        return ''.join(retlist)
+
 class EmptyRule(Enum):
+    """Rule for what can be moved to an empty tableau pile.
+    """
     NONE = 0
     ANY1 = 1
     ANYRUN = 2
     HIGH1 = 3
     HIGHRUN = 4
 
 AgnesGraph = dict[CardSuit, set[CardSuit]]
@@ -242,14 +395,24 @@
         'none': False,
         'any 1': True,
         'any run': False,
         'high 1': True,
         'high run': False,
            }[emptyrule_str]
 
+def _dont_deal_last(last_move_info: list[LastMoveInfo]) -> bool:
+    anydup: set[int] = set()
+    for pile_index in range(2, 7):
+        if last_move_info[pile_index].depth > 0:
+            if last_move_info[pile_index].depth in anydup:
+                return True
+            else:
+                anydup.add(last_move_info[pile_index].depth)
+    return False
+
 #------------------------------------------------------------------------------
 # The largest trees hit a memory limit when writing to the losing_states set
 # so here we do some simple compression for the string representation rather
 # than using the form generated by __repr__ (which we keep for use in debugging
 # output).
 #------------------------------------------------------------------------------
 
@@ -308,15 +471,15 @@
         played in full.
     maximize_score : boolean
         Stores value of input parameter with the same name
     move_to_empty_pile : str
         Stores value of input parameter with the same name
     move_same_suit : boolean
         Stores value of input parameter with the same name
-    split_same_suit_runs : boolean
+    split_runs : boolean
         Stores value of input parameter with the same name
     face_up : boolean
         Stores value of input parameter with the same name
     maximize_score : boolean
         Stores value of input parameter with the same name
     track_threshold : boolean
         Stores value of input parameter with the same name
@@ -329,15 +492,15 @@
     max_states : boolean
         Stores value of input parameter with the same name
     """
 
     def __init__(self,
                  move_to_empty_pile: str = 'none',
                  move_same_suit: bool = False,
-                 split_same_suit_runs: bool = True,
+                 split_runs: bool = True,
                  face_up: bool = False,
                  maximize_score: bool = False,
                  track_threshold: int = 0,
                  print_states: bool = False,
                  test_deck: int = 0,
                  deck_filename: Optional[str] = None,
                  max_states: int = 0):
@@ -355,16 +518,17 @@
             'any run': Any movable run can be moved.
             'high run': Any movable run that is built down from a card of
                 highest rank.
         move_same_suit : boolean, optional (default = False)
             If True, only permit moving sequences of cards in the tableau
             that are the same suit. Otherwise, permit moving sequences of
             cards that are the same color.
-        split_same_suit_runs : boolean, optional (default = True)
-            If True, a sequence of the same suit can be split by a move.
+        split_runs: boolean, optional (default = True)
+            If True, allow a movable run to be split during a move. If
+            false, movable runs must be moved in their entirety.
         face_up : boolean, optional (default = False)
             Deal all cards face up in the tableau.
         track_threshold : int, optional (default = 0)
             If the number of cards left in the stock is greater than or
             equal to this value, track losing states in a single set for
             the whole game. This set can consume a lot of memory if some of
             the other options are chosen that allow a large number of moves
@@ -394,18 +558,19 @@
 
         # Initial deck, before standardizing so the base card has rank 0
         self._initial_deck: list[Card] = []
         # Deck after standardizing the base card
         self._deck: list[Card] = []
         # List to track the valid moves remaining for each state in the stack
         self._all_valid_moves: list[list[AgnesMove]] = []
+        self._all_lmi: list[list[LastMoveInfo]] = []
         # List of states we have been since the last deal or move-to-foundation
         # This is to check that we don't enter an infinite loop of moving
         # cards in the tableau.
-        self._check_loop_states: list[set[str]] = [set()]
+        self._check_loops: set[str] = set()
         # Moves performed to reach each state.
         self._moves: list[AgnesMove] = []
         self._curr_state: _AgnesState = _AgnesState()
         # States (as str) that we have already identified as losing
         self._losing_states: Set[str] = set()
         self.test_deck = test_deck
         self.n_states_checked = 1
@@ -415,22 +580,22 @@
         self.n_no_move_possible = 0
         self._max_states = max_states
         self.deck_filename = deck_filename
         self.move_to_empty_pile = move_to_empty_pile
         self.move_same_suit = move_same_suit
         self.print_states = print_states
         self.track_threshold = track_threshold
-        self.split_same_suit_runs = split_same_suit_runs
+        self.split_runs = split_runs
         self.max_depth = 0   # maximum depth of the search tree
         # Current depth of the search tree (i.e., number moves played to reach
         # the current state. Does not count moves played where search had to
         # backtrack.
         self.current_depth = 0
         self.face_up = face_up
-        self._check_for_loops = (split_same_suit_runs
+        self._check_for_loops = (split_runs
              or move_to_empty_pile != 'none')
         #self._face_up = True
         self.maximize_score = maximize_score
         self.max_score = 1   # maximum score found
         #self.move_from_same_suit = move_from_same_suit
         #move_from_same_suit : boolean, optional
         #    Allow moving a pile off of the same suit. For example,
@@ -474,27 +639,39 @@
         color, as are suits 1 and 3. The normalized cards are printed, ie,
         all cards have a number subtracted from their rank so that the base
         card has rank 0.
 
         Returns
         -------
         A string as described above.
+
+        Notes
+        -----
+        Because the `Agnes` object has to construct the states by undoing
+        moves, a deepcopy of the object is made before starting. This also 
+        (unnecessarily) copies the perhaps quite large `_losing_states`
+        attribute. Therefore, it is probably best to use this only for
+        debugging rather than printing the history for all winners.
         """
         states: list[_AgnesState] = []
         # inefficient, since losing_states set may be quite large, but we
         # expect to only do once for each winning game
         # a copy is needed because making/undoing moves changes the
         # current state stored in the `Agnes` object.
         copyself: Agnes = copy.deepcopy(self)
-        while copyself._moves:
-            states.append(copy.deepcopy(copyself._curr_state))
-            copyself._undo_move(no_print=True)
-            copyself._curr_state.set_valid_moves(self._enum_to_empty_pile)
+        # do not iterate over enumerate(...) since _moves is being modified
+        for move_index in range(0, len(copyself._moves)): # pylint: disable=protected-access
+            states.append(copy.deepcopy(copyself._curr_state)) #pylint: disable=protected-access
+            copyself._undo_move(no_print=True)                 #pylint: disable=protected-access
+            copyself._curr_state.set_valid_moves(self._enum_to_empty_pile, #pylint: disable=protected-access
+                self.move_same_suit, self.split_empty_stock,
+                self.track_threshold, self._all_lmi[-(move_index+1)])
+
         # Get the initial state also
-        states.append(copy.deepcopy(copyself._curr_state))
+        states.append(copy.deepcopy(copyself._curr_state)) # pylint: disable=protected-access
         return str(list(reversed(states)))
 
     # Print the deck used in a simple text format
     def export_deck(self, filename: str) -> None:
         """Export the deck to a text file.
 
         Write one card per line as (rank, suit) where suit is 0, 1, 2, or 3,
@@ -607,52 +784,61 @@
             1: Won
             2: Lost
             3: Terminated because number of states created exceeds
                max_states
         """
 
         first_state = self._curr_state
+        last_move_info: list[LastMoveInfo] = []
+        for i in range(0, 7):
+            last_move_info.append(LastMoveInfo())
 
         # Reset the indexing of all cards so base card has rank 0
         self._deck = []
         for i in range(0, 13*4):
             self._deck.append(Card(rank=(self._initial_deck[i].rank
                                 - self._initial_deck[0].rank) % 13,
                                    suit=self._initial_deck[i].suit))
         # Deal base card to foundation
         first_state.play_base_card(self._deck[0])
 
         snm_opts: SetNMovableOpts = SetNMovableOpts(
-            move_same_suit=self.move_same_suit,
-            split_same_suit_runs=self.split_same_suit_runs,
+            move_same_suit=self.move_same_suit, split_runs=self.split_runs,
             split_empty_stock=self.split_empty_stock)
 
         # Deal next cards to Tableau
         for i in range(0,7):
             for j in range(i,7):
                 first_state.deal_onto_pile(pile_index=j, deck=self._deck,
                     face_up=bool(self.face_up or j == i))
 
         for i in range(0,7):
             first_state.set_n_movable(i, snm_opts)
 
-        first_state.set_valid_moves(self._enum_to_empty_pile)
+        self._all_lmi.append(last_move_info)
+        first_state.set_valid_moves(self._enum_to_empty_pile,
+            self.move_same_suit, self.split_empty_stock,
+            self.track_threshold, self._all_lmi[-1])
 
         #print(first_state)
         self._all_valid_moves = [first_state.valid_moves]
         done = 0
-        if self.print_states: print(first_state)
+        if self.print_states:
+            print(first_state)
+            print(self._lmi_to_str())
         if (self._enum_to_empty_pile == EmptyRule.NONE
                 and not self.maximize_score
                 and first_state.any_pile_blocked()):
             return 2
         else:
             while done == 0:
                 done = self._perform_move()
-                if self.print_states: print(self._curr_state)
+                if self.print_states:
+                    print(self._curr_state)
+                    print(self._lmi_to_str())
             self.current_depth = self._curr_state.depth
             return done
 
     def _undo_move(self, no_print: bool) -> None:
         """Undo last move (last item in `_moves` stack).
 
         The three-step process when executing a move is described in the
@@ -674,24 +860,39 @@
         None
         """
 
         if self.print_states and not no_print: print('Undo move')
         new_state = self._curr_state
         curr_move = self._moves.pop()
         snm_opts: SetNMovableOpts = SetNMovableOpts(
-            move_same_suit=self.move_same_suit,
-            split_same_suit_runs=self.split_same_suit_runs,
+            move_same_suit=self.move_same_suit, split_runs=self.split_runs,
             split_empty_stock=self.split_empty_stock)
         self._all_valid_moves.pop()
-        if self._check_for_loops:
-            self._check_loop_states.pop()
+        self._all_lmi.pop()
+        if self._check_for_loops and not no_print:
+            if not new_state.is_loop:
+                self._check_loops.remove(new_state.hash_str)
         new_state.depth = new_state.depth - 1
+
+        new_state.is_loop = False
+        new_state.is_loser = False
+
         if curr_move is None:
             raise ValueError('_undo_move: curr_move should not be None')
         elif isinstance(curr_move, MoveToFound):
+            last_card: Card = Card(new_state.foundation[curr_move.suit],
+                                   curr_move.suit)
+            if curr_move.tabltype == TablType.NONE:
+                new_state.in_suit_seq[last_card.rank][last_card.suit] = False
+            if new_state.piles[curr_move.from_].exposed:
+                card_to_hide: Card = new_state.piles[
+                    curr_move.from_].exposed[-1]
+                new_state.last_in_pile[card_to_hide.rank][
+                    card_to_hide.suit] = False
+
             # if we exposed a card when we moved the card beneath it to the
             # foundation, turn it back over before moving the card back from
             # the foundation
             if curr_move.expose:
                 new_state.piles[curr_move.from_].hidden.append(
                     new_state.piles[curr_move.from_].exposed.pop())
             # now move the card back from the foundation
@@ -700,65 +901,82 @@
                      suit=curr_move.suit))
             new_state.foundation[curr_move.suit] -= 1
             new_state.set_n_movable(curr_move.from_, snm_opts)
         elif isinstance(curr_move, DealMove):
             # Deal from stock
             if new_state.n_stock_left == 0:
                 # Put two cards back on deck and remove them from the tableau
-                new_state.n_stock_left = 2
-                new_state.piles[0].exposed.pop()
-                new_state.piles[1].exposed.pop()
+                new_state.undo_deal_for_pile(0)
+                new_state.undo_deal_for_pile(1)
                 # set_n_movable depends on whether n_stock_left>0, so need
                 # to call it for all piles, not just the first two
                 for pile_index in range(0,7):
                     new_state.set_n_movable(pile_index, snm_opts)
             else:
-                new_state.n_stock_left = new_state.n_stock_left + 7
-                for pile in new_state.piles:
-                    pile.exposed.pop()
+                for pile_index, _ in enumerate(new_state.piles):
+                    new_state.undo_deal_for_pile(pile_index)
                 for i in range(0, 7):
                     new_state.set_n_movable(i, snm_opts)
         elif isinstance(curr_move, TablMove):
+            # since we are undoing the move here, the curr_move.to_ pile
+            #  is now the one we are moving the run from
+            from_pile = new_state.piles[curr_move.to_].exposed
+            to_pile = new_state.piles[curr_move.from_].exposed
+            top_card = from_pile[-curr_move.n_cards]
+            if curr_move.tabltype == TablType.JOIN:
+                new_state.in_suit_seq[top_card.rank][top_card.suit] = False
+            elif curr_move.tabltype == TablType.SPLIT:
+                new_state.in_suit_seq[top_card.rank][top_card.suit] = True
+
+            if len(from_pile) != curr_move.n_cards:
+                prev_card = from_pile[-1*(curr_move.n_cards + 1)]
+                new_state.last_in_pile[prev_card.rank][prev_card.suit] = True
+            if to_pile:
+                new_state.last_in_pile[to_pile[-1].rank][
+                    to_pile[-1].suit] = False
+
             # if we exposed a card when we moved the pile, turn it back over
             # before moving the pile back
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
 
+        new_state.update_hash_str()
+
         if self._moves:
             new_state.curr_move = self._moves[-1]
         else:
             new_state.curr_move = None
         # [20240315RG] bug fix for printing
         new_state.valid_moves = self._all_valid_moves[-1]
 
     def _perform_move(self) -> int:
         """Perform a move. Call _undo_move if no possible move.
 
         To make a move, update:
             (1) the appropriate attributes of `self._curr_state`
-                (`exposed`, `hidden`, `n_stock_left`, `foundation`)
+                (`exposed`, `hidden`, `n_stock_left`, `foundation`,
+                 `last_in_pile`, `in_suit_seq`)
             (2) any counters in `self` that count the various types of
                 moves made (`n_move_to_foundation`,`n_deal`,
                 `n_move_card_in_tableau`).
-            (3) append to the three stacks that track the evolution of the
-                game:` _moves`, `_all_valid_moves`, `_check_loop_states`.
-                While we could have used a single stack to manage these three
-                items, we intentionally do not maintain a stack of
-                _AgnesState objects. This would simplify the code (eg,
-                `_undo_move` could be replaced with popping the last state
-                from the stack), but increases the run-time 4.75-fold
-                for 1000 simulations (80m vs 381m).
+            (3) append to the stacks that track the evolution of the
+                game:` _moves`, `_all_valid_moves`, `_check_loop_states`,
+                `_all_lmi`.  While we could have used a single stack to
+                manage these three items, we intentionally do not maintain
+                a stack of _AgnesState objects. This would simplify the code
+                (eg, `_undo_move` could be replaced with popping the last
+                state) but increases the run-time.
 
         Arguments
         ---------
         None
 
         Returns
         -------
@@ -772,16 +990,15 @@
            3 if self.n_states_checked > self._max_states and
              self._max_states>0
 
         """
         self.n_states_checked += 1
 
         snm_opts: SetNMovableOpts = SetNMovableOpts(
-            move_same_suit=self.move_same_suit,
-            split_same_suit_runs=self.split_same_suit_runs,
+            move_same_suit=self.move_same_suit, split_runs=self.split_runs,
             split_empty_stock=self.split_empty_stock)
 
         if self._curr_state.depth > self.max_depth:
             self.max_depth = self._curr_state.depth
 
         if self._max_states > 0 and self.n_states_checked>self._max_states:
             #print(f'Terminated at {self.n_states_checked} moves', flush=True)
@@ -794,133 +1011,191 @@
 
         # Lost the game!
         if (self._curr_state.depth == 0 and not valid_moves):
             self.n_no_move_possible += 1
             return 2
         elif not valid_moves:
             # keep track of states that we know are losers
-            if self._curr_state.n_stock_left >= self.track_threshold:
-                self._losing_states.add(self._curr_state.strcompress())
+            if (self._curr_state.n_stock_left >= self.track_threshold
+                    and not self._curr_state.is_loser):
+                self._losing_states.add(self._curr_state.hash_str)
             self.n_no_move_possible += 1
             self._undo_move(no_print=False)
             return 0
         else:
             # Make a move
             curr_move = valid_moves.pop()
             new_state = self._curr_state
             new_state.curr_move = curr_move
+            self._all_lmi.append(copy.deepcopy(self._all_lmi[-1]))
+            last_move_info = self._all_lmi[-1]
             new_state.depth += 1
             if isinstance(curr_move, MoveToFound):
                 last_card = new_state.piles[curr_move.from_].exposed.pop()
                 if curr_move.expose:
                     new_state.piles[curr_move.from_].exposed.append(
                         new_state.piles[curr_move.from_].hidden.pop())
+                if new_state.piles[curr_move.from_].exposed:
+                    new_last = new_state.piles[curr_move.from_].exposed[-1]
+                    new_state.last_in_pile[new_last.rank][new_last.suit] = True
                 new_state.foundation[last_card.suit] += 1
-                if self._check_for_loops:
-                    check_loops: set[str] = set()
                 self.n_move_to_foundation += 1
                 # +4 here because -1 represents no card in pile
                 score = sum(new_state.foundation)+4
                 if score > self.max_score:
                     self.max_score = score
                 if score == 52: won_game = True
                 new_state.set_n_movable(curr_move.from_, snm_opts)
+                last_move_info[curr_move.from_] = LastMoveInfo(depth = 0,
+                    n_moved = 0, moved_to = False, can_move_to_found = True)
+                if curr_move.tabltype == TablType.NONE:
+                    new_state.in_suit_seq[last_card.rank][last_card.suit] = (
+                        True)
             elif isinstance(curr_move, DealMove):
                 # Deal from stock
                 if new_state.n_stock_left == 2:
                     new_state.deal_onto_pile(0, self._deck, True)
                     new_state.deal_onto_pile(1, self._deck, True)
                     # set_n_movable depends on whether n_stock_left>0, so need
                     # to call it for all piles, not just the first two
                     for pile_index in range(0,7):
                         new_state.set_n_movable(pile_index, snm_opts)
+                    last_move_info[0] = LastMoveInfo(depth = 0, n_moved = 0,
+                        moved_to = False, can_move_to_found = True)
+                    last_move_info[1] = LastMoveInfo(depth = 0, n_moved = 0,
+                        moved_to = False, can_move_to_found = True)
                 else:
                     for pile_index in range(0,7):
                         new_state.deal_onto_pile(pile_index, self._deck, True)
                     for pile_index in range(0,7):
                         new_state.set_n_movable(pile_index, snm_opts)
+                        last_move_info[pile_index] = LastMoveInfo(depth = 0,
+                            n_moved = 0, moved_to = False,
+                            can_move_to_found = True)
 
-                if self._check_for_loops:
-                    check_loops = set()
                 # If move_to_empty_pile == 'none', then our trick of speeding
                 # up run-time by seeing if any lower cards are blocked by
                 # the highest card won't work, because the highest card
                 # could be moved to an empty pile
                 if (self._enum_to_empty_pile == EmptyRule.NONE
                         and not self.maximize_score):
                     any_pile_blocked = new_state.any_pile_blocked()
                 self.n_deal += 1
             elif isinstance(curr_move, TablMove):
                 self.n_move_card_in_tableau += 1
+                from_pile = new_state.piles[curr_move.from_].exposed
+                to_pile = new_state.piles[curr_move.to_].exposed
+                if len(from_pile) != curr_move.n_cards:
+                    last_card = from_pile[-1 *(curr_move.n_cards+1)]
+                    new_state.last_in_pile[last_card.rank][last_card.suit] = (
+                        True)
+                if to_pile:
+                    new_state.last_in_pile[to_pile[-1].rank][
+                        to_pile[-1].suit] = False
+                top_card = from_pile[-1*curr_move.n_cards]
+                if curr_move.tabltype == TablType.JOIN:
+                    new_state.in_suit_seq[top_card.rank][top_card.suit] = True
+                elif curr_move.tabltype == TablType.SPLIT:
+                    new_state.in_suit_seq[top_card.rank][top_card.suit] = False
+
+                last_card = from_pile[-1]
+                last_move_info[curr_move.from_] = LastMoveInfo(
+                    depth = new_state.depth, n_moved = curr_move.n_cards,
+                    moved_to = False,
+                    can_move_to_found = True)
+                last_move_info[curr_move.to_] = LastMoveInfo(
+                    depth = new_state.depth, n_moved = curr_move.n_cards,
+                    moved_to = True,
+                    can_move_to_found = (
+                       not (new_state.foundation[last_card.suit]
+                            == (last_card.rank - 1))))
+
                 for n_to_pop in range(-1*curr_move.n_cards,0):
                     new_state.piles[curr_move.to_].exposed.append(
                         new_state.piles[curr_move.from_].exposed.pop(n_to_pop)
                         )
                 if curr_move.expose:
                     new_state.piles[curr_move.from_].exposed.append(
                         new_state.piles[curr_move.from_].hidden.pop())
                 new_state.set_n_movable(curr_move.from_, snm_opts)
                 new_state.set_n_movable(curr_move.to_, snm_opts)
-                if self._check_for_loops:
-                    check_loops = copy.copy(self._check_loop_states[-1])
             else:
                 raise TypeError(f'curr_move is {curr_move}')
+
+            new_state.update_hash_str()
+            new_state.is_loop = False
+            new_state.is_loser = False
+            if self._check_for_loops:
+                # Unlike other languages, Python doesn't give a return code
+                # indicating whether item was already in the set, but we can
+                # determine by getting the length before and after (O(1) time)
+                len_before = len(self._check_loops)
+                self._check_loops.add(new_state.hash_str)
+                if len_before == len(self._check_loops):
+                    new_state.is_loop = True
+
             #------------------------------------------------------------------
             # It's possible we've already evaluated that this state is losing.
             # Consider the case where there are two possible independent moves
             # (M1: Move 1 card from Pile 1 to 2, M2: move 1 card from pile 5
             # to 6). Once you check that M1->M2 doesn't win, no need to check
             # M2->M1
             #------------------------------------------------------------------
-            if (self._curr_state.n_stock_left >= self.track_threshold
-                and (new_state.strcompress() in self._losing_states)):
+            if new_state.is_loop:
+                if self.print_states:
+                    print('New state is a loop, '
+                          'so setting valid_moves to empty')
+                new_state.valid_moves = []
+            elif (self._curr_state.n_stock_left >= self.track_threshold
+                and (new_state.hash_str in self._losing_states)):
+                new_state.is_loser = True
                 new_state.valid_moves = []
                 if self.print_states:
                     print('Already checked the new state, '
                           'so setting valid_moves to empty')
             elif (self._enum_to_empty_pile == EmptyRule.NONE
                     and any_pile_blocked):
                 if self.print_states:
                     print('New state is a block, '
                           'so setting valid_moves to empty')
                 new_state.valid_moves = []
-            elif (self._check_for_loops and new_state.strcompress()
-                          in check_loops):
-                if self.print_states:
-                    print('New state is a loop, '
-                          'so setting valid_moves to empty')
-                new_state.valid_moves = []
             else:
-                new_state.set_valid_moves(self._enum_to_empty_pile)
-
-            if self._check_for_loops:
-                check_loops.add(new_state.strcompress())
+                new_state.set_valid_moves(self._enum_to_empty_pile,
+                    self.move_same_suit, self.split_empty_stock,
+                    self.track_threshold, self._all_lmi[-1])
 
             if won_game:
                 self._moves.append(curr_move)
-                # [RG20240316]
-                if self._check_for_loops:
-                    self._check_loop_states.append(set())
                 self._all_valid_moves.append([])
                 return 1
             elif not new_state.valid_moves:
-                if new_state.n_stock_left >= self.track_threshold:
-                    self._losing_states.add(new_state.strcompress())
                 self._all_valid_moves.append([])
-                if self._check_for_loops:
-                    self._check_loop_states.append(set())
                 self._moves.append(curr_move)
             else:
                 self._all_valid_moves.append(new_state.valid_moves)
-                if self._check_for_loops:
-                    self._check_loop_states.append(check_loops)
                 self._moves.append(curr_move)
 
             return 0
 
+    def _lmi_to_str(self) -> str:
+        lmi_top: list[LastMoveInfo] = self._all_lmi[-1]
+        retlist = []
+        for item in lmi_top:
+            if item.moved_to:
+                mt = 'T'
+            else:
+                mt = 'F'
+            if item.can_move_to_found:
+                t_or_f = 'T'
+            else:
+                t_or_f = 'F'
+            retlist.append(f'{item.depth}-{item.n_moved}-{mt}-{t_or_f}')
+        return f"Last move info:[{', '.join(retlist)}]"
+
+
 #------------------------------------------------------------------------------
 # AgnesState class - represents a state in the game.
 #------------------------------------------------------------------------------
 class _AgnesState:
     """Represent a state in the game.
 
     Attributes:
@@ -940,28 +1215,49 @@
         List of valid moves for this state. It is initialized when the state
         is created and then moves are popped off as they are tried.
     force_move : list[AgnesMove]
         List of move that will be forced. This will override the list of
         valid moves. For example, moving a card from the tableau to an
         empty foundation pile may be forced. See `set_valid_states`
         for details.
+    in_suit_seq : list[list[bool]]
+        True for a given card if the card is in an exposed pile in sequence
+        under a card of the same suit or is in the foundation. Access
+        as: in_suit_seq[card.rank][card.suit].
+    last_in_pile : list[list[bool]]
+        True for a given card if the card is the last card in an exposed
+        pile (ie, first available for play) or is in the foundation.
+        Access as: last_in_pile[card.rank][card.suit].
+    hash_str : str
+        Somewhat compressed representation of the cards left in the stock and
+        and tableau cards. This will be stored in the sets that check for
+        loops and previously losing states.
     """
     # default constructor
     def __init__(self) -> None:
         self.depth = 0
         self.n_stock_left = 52
         # Exposed and hidden cards in tableau.
         self.piles: tuple[AgnesPile, ...] = (AgnesPile([], [], []),
             AgnesPile([], [], []), AgnesPile([], [], []),
             AgnesPile([], [], []), AgnesPile([], [], []),
             AgnesPile([], [], []), AgnesPile([], [], []))
         self.foundation = [-1, -1, -1, -1]
         self.curr_move: Optional[AgnesMove] = None
         self.valid_moves: list[Optional[AgnesMove]] = []
-        self.force_move: list[Optional[AgnesMove]] = []
+        #self.force_move: list[Optional[AgnesMove]] = []
+        self.is_loop = False
+        self.is_loser = False
+        self.in_suit_seq: list[list[bool]] = []
+        self.last_in_pile: list[list[bool]] = []
+        self.hash_str: str = ''
+        for _ in range(0, 13):
+            self.in_suit_seq.append([False, False, False, False])
+            self.last_in_pile.append([False, False, False, False])
+
 
     # String representation of object (print() will use this)
     #def vertstr(self) -> str:
     #    str1 = (f'\nMove: {_describe_move(self.curr_move)}\n\n'
     #        f'depth:{self.depth}, n_stock_left:{self.n_stock_left}, '
     #        f'valid_moves:{self.valid_moves}\n')
     #
@@ -981,24 +1277,58 @@
             f'T0:{self.piles[0].hidden} | {self.piles[0].exposed}\n'
             f'T1:{self.piles[1].hidden} | {self.piles[1].exposed}\n'
             f'T2:{self.piles[2].hidden} | {self.piles[2].exposed}\n'
             f'T3:{self.piles[3].hidden} | {self.piles[3].exposed}\n'
             f'T4:{self.piles[4].hidden} | {self.piles[4].exposed}\n'
             f'T5:{self.piles[5].hidden} | {self.piles[5].exposed}\n'
             f'T6:{self.piles[6].hidden} | {self.piles[6].exposed}\n'
+            f'in_suit_seq:{self._print_in_suit_seq()}\n'
+            f'last_in_pile:{self._print_last_in_pile()}\n'
             )
 
-    def strcompress(self) -> str:
+    def _print_in_suit_seq(self) -> str:
+        '''Print in_suit_seq bool attribute as 0s and 1s.
+
+        Space is used to separate the nested lists.
+        '''
+        outlist = []
+        for suit_list in self.in_suit_seq:
+            suitlist = []
+            for suit in suit_list:
+                if suit:
+                    suitlist.append('1')
+                else:
+                    suitlist.append('0')
+            outlist.append(''.join(suitlist))
+        return ' '.join(outlist)
+
+    def _print_last_in_pile(self) -> str:
+        '''Print last_in_pile bool attribute as 0s and 1s.
+
+        Space is used to separate the nested lists.
+        '''
+        outlist = []
+        for suit_list in self.last_in_pile:
+            suitlist = []
+            for suit in suit_list:
+                if suit:
+                    suitlist.append('1')
+                else:
+                    suitlist.append('0')
+            outlist.append(''.join(suitlist))
+        return ' '.join(outlist)
+
+    def update_hash_str(self) -> None:
         """Compressed string representation of the state.
         """
         retlist = [str(chr(self.n_stock_left))]
         for pile in self.piles:
             retlist.append(_strpilecomp(pile.exposed))
             retlist.append(_strpilecomp(pile.hidden))
-        return '-'.join(retlist)
+        self.hash_str = '-'.join(retlist)
 
     def struncomp(self) -> str:
         """Uncompressed string representation of the state.
         """
         retlist = [str(self.n_stock_left)]
         for pile in self.piles:
             retlist.append(_strpileuncomp(pile.exposed))
@@ -1015,95 +1345,157 @@
     #        f'T0:{self.exposed[0]}\nT1:{self.exposed[1]}\n'
     #        f'T2:{self.exposed[2]}\nT3:{self.exposed[3]}\n'
     #        f'T4:{self.exposed[4]}\nT5:{self.exposed[5]}\n'
     #        f'T6:{self.exposed[6]}\n')
 
     def set_n_movable(self, pile_index: int,
                       snm_opts: SetNMovableOpts) -> None:
-        """Set n_movable for a given pile.
+        """Set self.piles[pile_index].n_movable.
 
         Note this just checks the number of cards from the bottom of the
         pile than can be moved according to the rules. It does not check
         whether there is somewhere the selected set of cards can be moved
         to. The latter is done in `set_valid_moves`.
 
+        The value of self.n_stock_left is used in addition to the
+        parameters passed in to determine if the stock is empty. Therefore,
+        this function must be called for all piles when the stock is
+        made empty (or such a move undone).
+
         Arguments
         ---------
         pile_index : int
             Index of the pile to check
         snm_opts : SetNMovableOpts
-            Tuple holding `Agnes` parameter values `move_same_suit` and
-            `split_same_suit_runs`, as well as `split_empty_stock`.
+            Tuple holding `Agnes` parameter values `move_same_suit`,
+            `split_runs`, and `split_empty_stock`.
 
         Returns
         -------
         List of integers with number of cards that can be moved from a
         pile.
-
-        Notes
-        -----
-        For now, this only uses information for a single pile, so this
-        could be a method of the `AgnesPile` class. However, future
-        optimizations will likely use other information from `self`.
         """
         pile = self.piles[pile_index].exposed
         self.piles[pile_index].n_movable.clear()
-        whole_suit_seq: bool = True
+        #whole_suit_seq: bool = True
         if pile:
             for card_index, card in enumerate(reversed(pile)):
                 try:
                     #above_card = pile[card_index + 1]
                     above_card = pile[-1 - card_index - 1]
                 except IndexError:
                     above_card = None
 
-                # Check rank & check suit is same color (convention is
-                # suits (0,2) and (1,3) are the same color)
+                # the next two if statements verify that the card starts a
+                # sequence of the same color
                 if not card.rank - card_index == pile[-1].rank:
-                    whole_suit_seq = False
+                    #whole_suit_seq = False
                     break
 
                 if not card.suit == pile[-1].suit:
-                    whole_suit_seq = False
+                    #whole_suit_seq = False
                     if (snm_opts.move_same_suit
                             or (card.suit % 2) != (pile[-1].suit % 2)):
                         break
 
-                if (snm_opts.split_same_suit_runs
-                        or above_card is None
-                        or not (above_card.rank == card.rank + 1
-                                and above_card.suit == card.suit)):
-                    if (whole_suit_seq and self.n_stock_left == 0
-                            and not snm_opts.split_empty_stock):
-                        self.piles[pile_index].n_movable.clear()
+                if above_card:
+                    is_split_same_suit = (above_card.rank == card.rank + 1
+                        and above_card.suit == card.suit)
+                    is_split_same_color = (above_card.rank == card.rank + 1
+                        and (above_card.suit - card.suit) % 2 == 0)
+                else:
+                    is_split_same_suit = False
+                    is_split_same_color = False
+
+                if (snm_opts.split_runs
+                        or (snm_opts.move_same_suit
+                            and not is_split_same_suit)
+                        or (not snm_opts.move_same_suit
+                            and not is_split_same_color)):
+                    if (self.n_stock_left == 0
+                            and not snm_opts.split_empty_stock
+                            and is_split_same_suit):
+                        continue
                     self.piles[pile_index].n_movable.append(card_index + 1)
 
+    def undo_deal_for_pile(self, pile_index: int) -> None:
+        """Undo deal of one card for pile identified by pile_index.
+
+        Set `in_suit_seq` and `last_in_pile` = False for the card being
+        undealt. If there is a card above this that will be now last,
+        set `last_in_pile` to True for that card. Pop the last card
+        from `piles[pile_index].exposed` and increase `n_stock_left` by 1.
+
+        Unlike deal_onto_pile, we don't need to handle face-down deals
+        because we never undo them.
+
+        Attributes
+        ----------
+        pile_index : int
+            Index of the pile for which the deal is undone
+        """
+        pile = self.piles[pile_index].exposed
+        last_card = pile[-1]
+        self.in_suit_seq[last_card.rank][last_card.suit] = False
+        self.last_in_pile[last_card.rank][last_card.suit] = False
+        pile.pop()
+        if pile:
+            new_last_card: Card = pile[-1]
+            self.last_in_pile[new_last_card.rank][new_last_card.suit] = True
+        self.n_stock_left += 1
+
   # Deal a single card from stock onto the pile identified by pile_index
     def deal_onto_pile(self, pile_index: int, deck: list[Card],
                        face_up: bool) -> None:
-        """Deal one card from the stock onto the pile identified by pile_index.
+        """Deal a card from the stock onto the pile with index pile_index.
+
+        Set `last_in_pile` = True for the card being dealt and set
+        `last_in_pile` = False for the card now covered by the deal (if
+        one exists). Set `in_suit_seq = True` for the dealt card if the card
+        happened to be dealt in sequence under a card of the same suit
+        in the exposed pile.  Card dealt is appended to the end of the
+        `exposed` pile if `face_up = True` and the `hidden` pile otherwise.
+        Decrease `n_stock_left` by 1.
+
+        Attributes
+        ----------
+        pile_index : int
+            Pile being dealt to.
+        deck : list[Card]
+            Deck from which we are dealing.
+        face_up : bool
+            Indicates whether card is dealt face-up (and put in the
+            self.piles[pile_index].exposed pile) or face-down (and put
+            in the .hidden pile).
         """
+        card: Card = deck[52 - self.n_stock_left]
         if face_up:
-            self.piles[pile_index].exposed.append(
-                deck[52 - self.n_stock_left])
+            if self.piles[pile_index].exposed:
+                last_card = self.piles[pile_index].exposed[-1]
+                if (card.rank + 1 == last_card.rank
+                        and card.suit == last_card.suit):
+                    self.in_suit_seq[card.rank][card.suit] = True
+                self.last_in_pile[last_card.rank][last_card.suit] = False
+            self.piles[pile_index].exposed.append(card)
+            self.last_in_pile[card.rank][card.suit] = True
         else:
-            self.piles[pile_index].hidden.append(
-                deck[52 - self.n_stock_left])
+            self.piles[pile_index].hidden.append(card)
         self.n_stock_left = self.n_stock_left - 1
 
     def any_pile_blocked(self) -> bool:
         """Check if game is unwinnable after a deal.
 
         This should only be called if `Agnes.move_to_empty_pile=='none'`.
         Otherwise, the game might be winnable even though suits are
         blocked because the 'kings' can be moved to an empty pile to
-        unblock the cards beneath them.
+        unblock the cards beneath them. (Here we use 'king' to refer to
+        the highest-rank card.)
 
         Creates a graph indicating whether a given 'king' is covering in
-        a pile a lower rank card of the same suit or a king of another
+        a pile a lower rank card of the same suit or a 'king' of another
         suit. If the graph has a cycle, the game cannot be won.
 
         Returns
         -------
         bool that is True if any pile or combination of piles blocks a win.
         """
         graph: AgnesGraph = {0: set(), 1: set(), 2: set(), 3: set()}
@@ -1119,76 +1511,144 @@
                         if (king_found[k]
                                     and (current_card.rank < 12
                                          or current_card.suit != k)):
                             graph[k].add(current_card.suit)
         return _cyclic(graph)
 
     # Set self.validmoves with the three types of moves
-    def set_valid_moves(self, enum_to_empty_pile: EmptyRule) -> None:
+    # TODO: update docstring description
+    def set_valid_moves(self, enum_to_empty_pile: EmptyRule,
+                        move_same_suit: bool, split_empty_stock: bool,
+                        track_threshold: int,
+                        last_move_info: list[LastMoveInfo]) -> None:
         """Set self.valid_moves to the valid moves available.
 
         Three types: DealMove()
-                     TablMove(from_=, to_=, n_cards=, expose=)
-                     MoveToFound(from_=, suit=, expose=)
+                     TablMove(from_=, to_=, n_cards=, expose=, tabltype=)
+                     MoveToFound(from_=, suit=, expose=, tabltype=)
 
-        If it is possible to put a card in the foundation, and that card
-        is less than or equal to two ranks higher than the highest card
-        in the foundation of the other suit, then moving the card to
-        the foundation is forced, ie, it is the only move stored in
-        `set.valid_moves`. (If multiple piles have a card meeting this
-        criteria, then the move from the last pile is forced.)
-
-        For example, suppose the base card is an Ace and the 6 of Spades
-        is the highest spade in the foundation. Then if there is a valid
-        move to put any club from Ace to 8 in the foundation, that move
-        will be forced (ie, the only valid move stored). If there is a
-        valid move to put the 9 of Clubs in the foundation, this would be
-        stored as a valid move, but would not be forced, because the 9
-        of clubs might be needed as a target to move the 8 of Spades under.
+        The `n_movable` attribute in a pile contains a list of the number
+        of cards in a pile that can be moved (based on the `move_same_suit`
+        and `split_runs` parameters when the `Agnes` object was created.
+        It also takes into account the optimization that there is no
+        benefit to splitting a sequence between two cards of the same
+        suit when the stock is empty, unless the empty rule is 'any 1' or
+        'high 1'.
+
+        This function creates a list of all valid moves that can be done
+        by seeing if a deal is available, which cards can be moved to which
+        target piles, and which cards can be moved to the foundation.
+
+        Various optimizations reduce the moves available. Forcing a move
+        means this is the only move that can be played. (If multiple moves
+        meet the forcing criteria, the last forced is used.)
+
+        (1) If n_stock_left == 2 and if track_threshold > 2, do not allow
+        the deal if there was a move between two piles that won't be covered
+        by the final deal. (Purpose is to reduce the search tree by forcing
+        these moves to occur after the final deal. This is only done when
+        track_threshold > 2 because otherwise we need to store the
+        information from LastMoveInfo in the `Agnes.losing_states` set.
+
+        (2) If there are multiple empty piles that won't be covered by
+        a future deal, only allow moves to the first pile.
+
+        (3) If we are not using the `losing_states` set (track_threshold >
+        `n_stock_left`), do not reverse a move (ie, move the same number
+        of cards from one pile to another).
+
+        (4) Force joins by suit sequence when the stock is empty and
+        `split_empty_stock is False` if the same-color top card of the
+        pile being moved satisfies (i) next lowest card is already in
+        the foundation or (ii) `move_same_suit = False` and already under
+        the next-highest card of the same suit or (iii)
+        `move_same_suit = False` and next-highest card is available to be
+        played on. For example, suppose we have a run starting with 4C
+        that we might put under 5C. This move is forced if (i) 3S in
+        foundation, (ii) `move_same_suit = False` and 4S already under 5S,
+        or (iii) `move_same_suit = False` and 5S is last in pile.
+
+        (5) Force move to foundation if (a) rank <= (highest rank in
+        foundation of same-color suit + 2) or (b) stock is empty and
+        `split_empty_stock = False` and next lowest rank of the same
+        color is already under in sequence under the same suit.
+
+        (6) Additional restriction on splitting same suit besides those
+        implied by `split_runs` (which were implemented in set_n_movable).
+        Only allow splits of same suit if source or target will be covered
+        by future deal, or split_empty_stock=true or Card(src_card.rank,
+        same_color_suit(src_card)) is not in the foundation, where src_card
+        is the highest-rank card in the part of the pile that is being
+        moved.
 
         Parameters
         ----------
         enum_to_empty_pile : EmptyRule
             `Agnes.move_to_empty_pile` parameter converted to enum.
+        move_same_suit : bool
+            `Agnes.move_same_suit` parameter
+        split_empty_stock : bool
+            `Agnes.split_empty_stock` attribute
+        track_threshold : int
+            `Agnes.track_threshold` attribute
+        last_move_info : list[LastMoveInfo]
+            The LastMoveInfo information for this state
 
         Returns
         -------
         None
         """
         self.valid_moves = []
-        self.force_move = []
+        force_move: Optional[AgnesMove] = None
 
         # Deal (DealMove dataclass)
-        if self.n_stock_left > 0:
+        if (self.n_stock_left > 2
+                or (self.n_stock_left == 2
+                    and (track_threshold <= 2
+                        or not _dont_deal_last(last_move_info)))):
             self.valid_moves.append(DealMove())
 
         for pile_index, pile in enumerate(self.piles):
             exp_pile = pile.exposed
+            tabltype: TablType = TablType.NONE
             # Moves in tableau (TablMove dataclass)
             #
             # Get a list of the number of cards that are movable
             # according to the input parameters. This does not yet consider
             # if there is a location the cards can be moved to.
             #n_movable = self.set_n_movable(pile_index, move_same_suit,
             #                                split_same_suit_runs)
 
             for n_to_move in pile.n_movable:
+                tabltype = TablType.NONE
                 # 'Source' card: the one we want to move
                 src_card = exp_pile[-n_to_move]
                 if n_to_move == len(exp_pile):
                     expose = bool(pile.hidden)
                 else:
                     expose = False
+                    card_above = exp_pile[-n_to_move - 1]
+                    if (src_card.rank + 1 == card_above.rank
+                            and src_card.suit == card_above.suit):
+                        tabltype = TablType.SPLIT
 
                 # 'target' pile is the pile we are trying to move to
                 found_empty_target = False
                 for target_index in range(0,7):
                     if (target_index == pile_index
                         or (not self.piles[target_index].exposed
-                            and found_empty_target)): continue
+                            and found_empty_target)
+                        or (track_threshold > self.n_stock_left
+                            and (last_move_info[pile_index].depth ==
+                                last_move_info[target_index].depth)
+                            and (last_move_info[pile_index].n_moved ==
+                                 n_to_move)
+                            and last_move_info[pile_index].moved_to
+                            and (last_move_info[pile_index].depth > 0))):
+                        continue
 
                     if self.piles[target_index].exposed:
                         target_card = self.piles[target_index].exposed[-1]
                     elif target_index >= self.n_stock_left:
                         found_empty_target = True
 
                     if not self.piles[target_index].exposed:
@@ -1199,48 +1659,95 @@
                             and
                                (((enum_to_empty_pile == EmptyRule.ANY1 or
                              (enum_to_empty_pile == EmptyRule.HIGH1
                               and src_card.rank == 12)) and n_to_move == 1) or
                              ((enum_to_empty_pile == EmptyRule.ANYRUN or
                              (enum_to_empty_pile == EmptyRule.HIGHRUN
                               and src_card.rank == 12))))):
-                            self.valid_moves.append(TablMove(
-                                from_=pile_index, n_cards=n_to_move,
-                                to_=target_index, expose=expose))
+                            if (pile_index < self.n_stock_left
+                                or target_index < self.n_stock_left
+                                or tabltype != TablType.SPLIT
+                                or split_empty_stock
+                                or self.foundation[
+                                   ((src_card.suit + 2) % 4)] < src_card.rank):
+                                self.valid_moves.append(TablMove(
+                                    from_=pile_index, n_cards=n_to_move,
+                                    to_=target_index, expose=expose,
+                                    tabltype=tabltype))
                     elif (self.piles[target_index].exposed
                             and src_card.rank == target_card.rank - 1
                             and ((src_card.suit
                                   - target_card.suit) % 2 == 0)):
-                        self.valid_moves.append(TablMove(
-                            from_=pile_index, n_cards=n_to_move,
-                            to_=target_index, expose=expose))
+                        if src_card.suit == target_card.suit:
+                            tabltype = TablType.JOIN
+
+                        if (pile_index < self.n_stock_left
+                            or target_index < self.n_stock_left
+                            or tabltype != TablType.SPLIT
+                            or split_empty_stock
+                            or self.foundation[
+                               ((src_card.suit + 2) % 4)] < src_card.rank):
+                            self.valid_moves.append(TablMove(
+                                from_=pile_index, n_cards=n_to_move,
+                                to_=target_index, expose=expose,
+                                tabltype=tabltype))
+                        if (not self.n_stock_left
+                            and not split_empty_stock
+                            and target_card.suit == src_card.suit
+                            and ((self.foundation[(src_card.suit+2)%4] + 1
+                                >= src_card.rank)
+                                or (not move_same_suit
+                                    and (self.in_suit_seq[src_card.rank][
+      (src_card.suit + 2) % 4]
+                                         or (src_card.rank < 12
+                                             and self.last_in_pile[
+      src_card.rank+1][(src_card.suit + 2) % 4]))))):
+                            force_move = TablMove(
+                                from_=pile_index, n_cards=n_to_move,
+                                to_=target_index, expose=expose,
+                                tabltype=tabltype)
 
             if exp_pile:
                 # Move card to foundation (MoveToFound dataclass)
                 last_card = exp_pile[-1]
                 expose = bool(len(exp_pile) == 1 and pile.hidden)
-                if last_card.rank - 1 == self.foundation[last_card.suit]:
+                if (last_card.rank - 1 == self.foundation[last_card.suit]
+                    and (track_threshold <= self.n_stock_left
+                        or not last_move_info[pile_index].depth
+                        or last_move_info[pile_index].can_move_to_found)):
+                    if self.in_suit_seq[last_card.rank][last_card.suit]:
+                        tabltype = TablType.SPLIT
+                    else:
+                        tabltype = TablType.NONE
                     self.valid_moves.append(MoveToFound(from_=pile_index,
-                            suit=last_card.suit, expose = expose))
+                            suit=last_card.suit, expose = expose,
+                            tabltype=tabltype))
                     same_color_suit = (last_card.suit + 2) % 4
 
                     # See discussion in docstring about forcing moves
-                    if last_card.rank <= self.foundation[same_color_suit] + 2:
-                        self.force_move = [MoveToFound(from_=pile_index,
-                                suit=last_card.suit, expose=expose)]
-
-        if self.force_move:
-            self.valid_moves = self.force_move
+                    if (last_card.rank <= self.foundation[same_color_suit] + 2
+                        or (self.n_stock_left == 0 and not split_empty_stock
+                            and self.in_suit_seq[last_card.rank - 1][
+                                same_color_suit])):
+                        force_move = MoveToFound(from_=pile_index,
+                                suit=last_card.suit, expose=expose,
+                                tabltype=tabltype)
+
+        if force_move:
+            self.valid_moves.clear()
+            self.valid_moves.append(force_move)
 
     def play_base_card(self, base_card: Card) -> None:
         """Play the base card into the foundation.
 
         Arguments
         ---------
         base_card : Card
 
         Returns
         -------
         None
         """
         self.foundation[base_card.suit] = 0
+        self.last_in_pile[0][base_card.suit] = True
+        self.in_suit_seq[0][base_card.suit] = True
         self.n_stock_left = self.n_stock_left - 1
```

### Comparing `quagnes-0.8.4/src/quagnes.egg-info/PKG-INFO` & `quagnes-1.0.0/src/quagnes.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quagnes
-Version: 0.8.4
+Version: 1.0.0
 Summary: This package solves Agnes (Agnes Sorel) solitaire card games. It can be used to solve games having the rules implemented in the GNOME AisleRiot package and the rules attributed to Dalton in 1909 and Parlett in 1979 among others and to calculate win rates.
 Author-email: Ray Griner <rgriner_fwd@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -714,389 +714,169 @@
     rc = new_game.play()
 
     # Write the return code and selected attributes from the game
     out_str = (str(rc) + ',' +
         ','.join([ str(getattr(new_game, attr)) for attr in attributes ]))
     print(out_str, flush=True)
 
-    # rc==1 are games that were won
-    if rc==1:
-        f = open(f'winners/win{rep}.txt', 'w', encoding='utf-8')
-        f.write(new_game.print_history())
-        f.close()
+    # rc==1 are games that were won, but probably best to only print a
+    # limited number for debugging or for rule variants when
+    # win rate is low
+
+    #if rc==1:
+    #    f = open(f'winners/win{rep}.txt', 'w', encoding='utf-8')
+    #    fwrite(new_game.print_history())
+    #    f.close()
 ```
 
 # Release Notes
-## Version 0.8.4
-- Copy editing of README.md and correct Wolter win rate to 45/1000000.
+## Version 1.0.0
+- Change name of `split_same_suit_runs` parameter to `split_runs` and make
+  parameter applicable regardless of the value of `move_same_suit`.
+- Add optimization for use when the losing state set is disabled.
+Track for each pile the last move depth, the number of cards
+moved, whether the pile was moved from or to, and whether the bottom card
+in the moved pile could be played to the foundation at the time of the move.
+Do not allow moves that: (a) reverse a previous tableau move without an
+intervening move to foundation or deal; (b) make the last deal after a
+tableau move where neither pile is dealt to and neither file had a card
+played to foundation; (c) play the bottom card of the moved pile to the
+foundation after the tableau move if it could have been played at the time
+of the move (and there has been no subsequent move to the pile or deal
+onto the pile).  These optimizations are only employed when the losing
+states set is
+disabled, as they use information not stored in the losing states set to
+determine whether a move can be played.
+- Add optimization when moves to empty piles allow zero or multiple cards
+to reduce the space of moves to consider when the stock is empty or near
+empty (without
+changing the win possibility or maximum score that can be attained). In
+these rules, we use the term 'top card' to describe the highest-rank card
+in the pile being moved and 'same-color top card' to be the card with equal
+rank in the same-color suit. The rules are: (a) when moving runs by suit,
+never split a run between same-suit cards when the stock is empty;
+(b) never split a run between same-suit cards when neither pile can be
+covered by a future deal and the same-color top card is in the foundation;
+(c) when the stock is empty, force a move onto a card of the same suit
+where possible when we know the target pile cannot be needed to move the
+same-color top card (ie, the same-color top card is already in the
+foundation or in same-suit sequence or the card one rank higher than the
+same-color top card is already exposed at the bottom of a pile); (d) when
+the stock is empty, force a move to the foundation if the card being
+moved cannot be needed as a target to be moved onto (ie, if the card in the
+same-color suit that is one rank lower is already in the foundation or in
+same-suit sequence).
+- Add new attributes created for these two optimizations in `_AgnesState` class (`in_suit_seq`, `last_in_pile`,
+  `_all_lmi`) and to output printed when state is printed.
+- Add `_AgnesState.hash_str` attribute to store the string representing
+  the hash of the object that will be stored in the losing states and
+  check loop set. Add `_Agnes_state.update_hash_str()` function called
+  after move is performed or undone to save the string in `hash_str`.
+  Previously, the `hash_str` was recalculated multiple times.
+- Fix bug in `Agnes.print_history` as only half the history was being
+  printed.
+- Use a single set to track whether loop has occured rather than a stack of
+  sets. Save result of check whether state is in the losing states set
+  so that we do not inefficiently (re-)insert the state into the losing
+  states set. Add attributes `is_loop` and `is_loser` to `_AgnesState`
+  class to support this logic.
+- Created for C++ implementation. Move detailed information
+  on the background, game rules, program methodology, and analysis of
+  win rates to that repository from this README. Add win rates
+  for rule variants where the empty rule is *AnyRun* or *HighRun*.
+
+# External Documentation
+A C++ implementation written by this package author also exists in a git
+repository.  Detailed information on the background, game rules, program
+methodology, and analysis of win rates are available [there](https://github.com/ghrgriner/quagnes-cpp/wiki/Rules,-Methodology,-and-Analysis-of-Win-Rates).
+
+# Using the Package
+Games are simulated by creating an `Agnes` object with the appropriate
+parameters, running `Agnes.play()`, and then using the return code and
+extracting desired statistics from `Agnes` class attributes.
+
+## Input Parameters
+The following are the parameters used to construct `Agnes` objects:
+
+|Parameter | Type | Description |
+|:-------- | :----- | :---------  |
+|`deck_filename` | `str` | Read deck from text file. If empty, a random deck will be used by calling `random.shuffle` and reversing the results. The text file should consist of 52 lines with each line formatted as `(rank, suit)`, where rank is in {0, 1, ..., 12} and suit is in {0, 1, 2, 3}. Suits are the same color if their value is equal modulus 2. The first card dealt is the base card.|
+|`move_to_empty_pile`| `str` | Rule for what can be moved to empty tableau piles. See following table for valid values.|
+|`move_same_suit`| `boolean` | If True, move runs by suit. If False (default), move runs by color.|
+|`split_runs` | `boolean` | If True, movable runs must be moved in their entirety. If False (default), a movable run can be split for a move).|
+|`face_up`| `boolean` |  If True, deal all cards face-up in the tableau. If False (default), only the last card in each column. |
+|`track_threshold`| `int` | If the number of cards left in the stock is greater than or equal to this value (default = 0), track losing states in a single set for the whole game. This set can consume a lot of memory if some of the other options are chosen that allow a large number of moves (eg, `move_to_empty_pile != 'none'`).|
+| `print_states` | `boolean` | Print detailed information about each state as moves are performed and undone. |
+| `maximize_score` | `boolean` | Maximize score. Disable optimization that inspects the layout of highest-ranked cards in the tableau to determine if game is unwinnable. |
+| `max_states` | `int` | Terminate game with return code 3 when number of states examined exceeds this threshold. 0 (default) means no threshold is used.|
+
+### Rule for Moving to Empty Piles
+|Value of `move_to_empty_pile` | Description |
+|:-------- | :---------  |
+|`'none'` | Empty piles can only be filled when dealing from stock (default). |
+|`'any run'` | Empty piles can be filled by any movable card or movable run. |
+|`'high run'` | Empty piles can be filled by any movable highest-rank card or movable run starting with a highest-rank card. |
+|`'any 1'` | Empty piles can be filled by any movable single card, but not by a movable run of more than one card. |
+|`'high 1'` | Empty piles can be filled by a single movable highest-rank card, but not by a movable run of more than one card. |
+
+## Output
+### `Agnes.play()` Return Code and `Agnes` Attributes
+The return code of the `Agnes.play()` function indicates whether the game is
+winnable (return code = 1), not winnable (return code = 2), or the
+simulation was terminated due to reaching the maximum number of states
+specified by the `max_states` parameter (return code = 3). The `Agnes`
+object has attributes with the same name and type as the input parameters
+that store the values of the parameters used during object construction.
+In addition, the following attributes of `Agnes` are updated when
+`Agnes.play()` is executed:
+
+| Attribute | Description |
+| :------------   | :---------  |
+| `n_states_checked` | Count number of states checked (including repeats). |
+| `n_deal` | Count number of deals performed (including those undone). |
+| `n_foundation` | Count number of moves to foundation performed (including those undone). |
+| `n_move_card_in_tableau` | Count number of moves in tableau performed (including those undone). |
+| `max_score` | Maximum score found during play. (If moving to empty piles is not allowed, this will not be the true maximum, unless `-z` was specified to disable the optimization that tries to detect unwinnable games from the location of the highest-rank cards in the tableau.) |
+| `max_depth` | Maximum depth of the search tree of moves. |
+| `current_depth` | Depth of the search tree when the game was terminated. This value is always 0 for losing games. |
+
+### Detailed Program Output
+When `print_states=True` for the `Agnes` object, `Agnes.play()` will print
+to standard output each state as moves are performed or undone.
 
-## Version 0.8.3
-- Copy editing of README.md
+```
+Move: Move 2 card(s) from pile 1 to pile 3
+
+piles:16#9-8-7##49-19-44##28-51-15-31##3-33-14-5-30-29##45-23-35##43-34-42-0-13-48-47-50##20-21-41-2-37#
+depth:11, n_stock_left:16, valid_moves:[DealMove(), TablMove(from_=3, n_cards=2, to_=2, expose=False, tabltype=2)]
+Foundations:[-1, -1, 1, 1]
+T0:[] | [(9, 0), (8, 0), (7, 0)]
+T1:[] | [(10, 3), (6, 1), (5, 3)]
+T2:[] | [(2, 2), (12, 3), (2, 1), (5, 2)]
+T3:[] | [(3, 0), (7, 2), (1, 1), (5, 0), (4, 2), (3, 2)]
+T4:[] | [(6, 3), (10, 1), (9, 2)]
+T5:[] | [(4, 3), (8, 2), (3, 3), (0, 0), (0, 1), (9, 3), (8, 3), (11, 3)]
+T6:[] | [(7, 1), (8, 1), (2, 3), (2, 0), (11, 2)]
+in_suit_seq:0011 0011 0000 0010 0010 0000 0000 1000 1001 0000 0000 0000 0000
+last_in_pile:0011 0011 0000 0010 0000 0011 0000 1000 0000 0010 0000 0011 0000
+
+Last move info:[10-2-T-T, 11-2-F-T, 0-0-F-T, 11-2-T-T, 10-2-F-T, 0-0-F-T, 9-1-F-T]
+```
 
-## Version 0.8.2
-- Bug fix: add check for loops when `move_to_empty_pile != 'none'` in
-addition to the existing check when `split_same_suit_runs=True`.
-- Add Optimizations #6 and #7 listed below.
-- When printing a state, add a single line with a string that has the
-  same values stored in the set of losing states. This alllows the user
-  to easily search in the output for when the previous state occurred.
-  Note that a more compressed version of this string (one byte per
-  card) is stored in the set of losing states. A longer version is
-  printed that avoids characters that are special in regular expressions
-  to facilitate searching. 
-- Remove extensive description of the rules from the module docstring.
-
-# Background
-Agnes is a difficult solitaire card game under some rule variants. This
-package solves the game automatically.
-
-Users can simulate random games and calculate win rates under various
-permutations of rules, including moving sequences (runs) by same-suit or
-same-color, allowing or not same-suit runs to be split in the middle of the
-run for a move, dealing all tableau cards face-up at the start versus
-dealing only the final tableau card face-up, and whether and how empty
-columns can be filled in between deals (never, a single card of any rank, a
-single card of the highest rank, a run starting with a single card of any
-rank, or a run starting with a card of the highest rank). The package
-provides additional options for debugging and tuning of the search algorithm
-to be more memory-efficient at the expense of speed.
-
-In 1979 Parlett named the two main variants of Agnes as Agnes Sorel (the
-variant / set of variants described here) and Agnes Bernauer (a variant/set
-of variants that uses a reserve) [3]. This package only considers Agnes
-Sorel.
-
-Some analyses of win rates for Agnes Sorel has previously been conducted.
-Wolter published an experimental analysis of the win rates of this and
-other solitaires, reporting 45 winnable games in a million deals under 
-presumably the *Up-Suit-None* rules (defined below) [4]. Masten modified
-Wolter's solver and reported 900/100,000 (0.9%) games were winnable when
-empty columns could not be filled by any card, although it is unclear
-whether same-suit runs could be split during a move [5]. In this
-analysis, we conduct our own simulations to estimate win rates, assess
-agreement with Wolter and Masten and add win rates for other
-rule variants. As in the prior analyses, the win rates calculated here are
-under perfect play (i.e., the solver is allowed to undo losing moves).
-
-# Rules
-There is considerable heterogeneity in the rules that have been proposed
-for Agnes (see Wikipedia [1] and Keller [6] for some discussion of the 
-history). We describe first the rules according to Dalton [1-2] and
-variations that change only the handling of play on empty piles. The other
-main set of variants allow moving of same-color runs instead of
-same-suit runs. We describe the parameter settings to be used in our
-software when playing the different rule variants.
-
-Because our interest in the problem arose from playing the game in the GNOME
-AisleRiot package, the default parameters correspond to this variant.
-
-## Dalton (1909)
-The first description is of the game is attributed to Dalton in 1909 [1-2].
-We implement his rules, except most software we have seen have the tableau
-piles ascending in length from left to right, so we follow that convention,
-rather than the right to left described by Dalton. (It should be noted that
-symmetry cannot be used to claim the win rates are identical under this
-variation because only the first two piles are dealt to in the final deal.)
-The rules are the following:
-
-Deal seven piles as columns face-up in the tableau such that the first pile
-has one card and the last column has seven. Then, deal a single card and
-place it above the tableau in the foundation (base card). Foundations are
-built up by suit and the tableau is built down by color. Wrap from king to
-ace when necessary. Piles of cards in sequence in the same suit can be
-moved in the tableau. The top card in each tableau pile is exposed and can
-be moved to a different pile (if it has the appropriate color and rank) or
-to the foundation. If a movable run occurs by chance at the start of
-the game or after a deal, the run can also be moved. When a card or
-pile is moved, the card in the column above it becomes exposed and
-available for play. Empty tableau piles can be filled by any card or
-movable run, or they can be left empty. Dealing from the stock adds one
-card to the bottom of each tableau pile before play resumes, so a game will
-have three more deals of seven cards and a final deal of two cards. Cards
-cannot be played back from the foundation to the tableau.
-
-Note that while Dalton used the singular when saying 'Any exposed card may
-be moved into a vacant space [pile]', in the example game he plays, he moves
-a group of cards into an empty pile. We follow the latter interpretation.
-
-Dalton states that at the start the bottom card of each pile is exposed and
-doesn't explicitly state what is permitted if a movable run occurs by
-chance. However, in the sample game he plays, he does not distinguish
-between cards that appeared at the bottom of the column at the start versus
-those that did not, so we adopt the interpretation that runs may be
-moved even if they first occurred by chance. This is consistent with the
-software implementations we have seen.
-
-The game as described above can be played by specifying the parameters
-`move_same_suit=True`, `face_up=True`, and `move_to_empty_pile='any run'`.
-
-We denote the rules above as *Up-Suit-AnyRun*. The third part of
-each name is because many variants have evolved that alter what can be done
-with empty piles. We refer to these as:
-
-- *Up-Suit-None*: Empty piles can only be filled when dealing from stock.
-- *Up-Suit-Any1*: Empty piles can be filled by any single card, but not by
-  a movable run.
-- *Up-Suit-HighRun*: Empty piles can be filled a single highest rank card, or
-a run starting with the highest rank card (i.e., if the base card was a seven,
-an empty pile can be filled only with a six or run starting with a six).
-- *Up-Suit-High1*: Empty piles can be filled by a single highest rank card.
-
-The `move_to_empty_pile` parameter takes the values `'none'` (default), 
-`'any 1'`, `'high run'`, and `'high 1'`, respectively, for the above four
-variants.
-
-## Parlett (1979) and *NoSplit* variants
-Parlett gives rules like *Up-Suit-None* but also forbids splitting same
-suit runs (`split_same_suit_runs=False`) [3]. We denote this as 
-*Up-Suit-None-NoSplit*. We also allow other rules that move by suit to
-have this option and denote these by adding *-NoSplit* to the end of
-of the rule name.
-
-## *Down-Color* and *Up-Color* variants
-Among this group, the primary variant of interest is *Down-Color-None*,
-which corresponds to the game as played on AisleRiot, which is where we
-became interested in the game. We verified the rules on the current
-AisleRiot version 3.22.23.
-
-The first variation from the Dalton rules is that cards are dealt
-face down in the tableau except for the final card dealt in each pile.
-We start these variant names with *Down-* instead of *Up-*.
-The second variation is that runs may be moved if they are the
-same color instead of requiring they be the same suit. We use *-Color-*
-as the second part of the variant name to indicate this. The third
-part of the variant name is as described for the Dalton variants.
-
-Other variants of interest in this class are *Up-Color-AnyRun*. This and
-*Up-Color-None* match the rules described on the website poltaire.com,
-which offers solitaire play [7]. This site is of interest to us as it hosts
-an article by Wolter [4] that analyzes the winnability of the game as
-played on the site.
-
-# Methodology
-## Optimizations
-The following optimizations were used to improve the run-time over a naive
-depth-first search of all possible moves:
-
-1. When `move_to_empty_pile='none'`, if the highest rank card (e.g., a king
-if the base card is an ace) is placed in a tableau pile below a lower card
-of the same suit, the lower card can never be moved from the pile. This is
-detected as soon as the king is placed. Therefore, some games can be
-determined to be not winnable by examining only the starting layout. Note
-while this optimization improves run time, it is not possible to determine
-the maximum possible score if a branch is terminated for this reason. This
-concept can be extended by noting that if the king of clubs blocks the
-queen of hearts and the king of hearts blocks the queen of clubs, the game
-is also unwinnable. In general, we define after each deal a four vertex
-graph (one vertex for each suit), where an edge denotes which suits are
-blocked by the suit corresponding to the vertex. The state is not winnable
-if a cycle exists in the graph. This only needs to be checked after a deal.
-This optimization is disabled when `move_to_empty_pile != 'none'` or when
-`maximize_score=True`.
-
-2. A card is immediately placed on a foundation if its rank is no more than
-the rank of the top foundation card of the same color suit plus two. For
-example, if the base card is an ace, and we have already played up to the
-six of spades in the foundation, we immediately play the ace of clubs up
-to the eight of clubs (if possible) to the foundation. We would not
-immediately play the nine of clubs to the foundation as it might be
-needed in the tableau to move the eight of spades.
-
-3. We track states that we have already determined to be not winnable in
-a set. For example, suppose the initial state has two possible moves: M1)
-move a card from pile 1 to 2; M2) move a card from pile 4 to 5. Once we
-determine the sequence M1 → M2 is not winnable, there is no need to check
-the sequence M2 → M1, as they both result in the same state. This
-optimization can be tuned using the `track_threshold` parameter.
-
-4. To prevent infinite loops, we use a stack of sets that stores the state of
-the game (number of cards in the stock and arrangement of cards in the tableau)
-and check whether this has been repeated since the last deal or move to
-foundation.  If the state is a repeat, we consider no valid moves to be
-available at the repeated state. This second method is disabled if
-`split_same_suit_runs=False` and `move_to_empty_pile 'none'}`, as loops
-cannot occur under this combination of parameter settings.
-
-<!--- First, we track for each pile the last move number (i.e., the number of
-plays
-since the start of the game the pile was last involved in a move between
-tableau piles). This is set to zero at the start of the game and when a card
-is moved from the pile to the foundation or when the pile is dealt to. A move
-between two piles is not permitted if the last move numbers match and are
-greater than zero and the target pile is not empty (as this implies we have
-reversed a previously executed move). -->
-5. The simulation is implemented using two or three equal-length stacks
-where the nth item describes an aspect of the state of the game at the
-nth move.  These three stacks store: (1) the moves performed, (2) the valid
-moves not yet attempted, and (3) a set containing the arrangement of all
-tableau layouts that have occurred since the last deal or move to foundation.
-A single state object (`_AgnesState`) in the `Agnes` object initially
-stores information about the starting state, such as the cards in the
-foundation, the arrangement of cards in the tableau, and the number of
-cards left in the stock. When a move is performed or undone, the
-`_AgnesState` object is updated in-place based on the move information.
-Initial testing found this implementation to be about 5–7 times faster than
-using a stack of `_AgnesState` objects, although this hasn't been retested
-after the addition of some of the other optimizations.
-
-7. If there are multiple empty columns in the tableau that cannot be
-covered by a future deal, then it doesn't matter which column is played
-in, so the first is always chosen. Similarly, we do not consider a move
-that moves the entirety of one column to a different empty column when
-both columns cannot be covered by a future deal.
-
-8. We do not allow splitting same-suit runs when the stock is empty
-regardless of the value of the `split_same_suit_runs` parameter, unless
-`move_to_empty_pile = 'any 1'` or `'high 1'`.
-
-Lastly, note that if win rate is the only output statistic of interest
-and results are being calculated for multiple rule sets, users can exploit
-the fact that all wins under some rule set is sometimes a subset of wins
-under another rule set. For example, any game winnable when 
-`split_same_suit_runs=False` is also winnable when
-`split_same_suit_runs=True` when other parameter values are fixed.
-
-## Statistical Analysis
-Ten thousand decks were simulated using this package version 8.0.2.
-We calculated the win rates and the 95% confidence intervals (95% CI)
-using the score (Wilson) method for the following rules:
-*Down-Color-None*, *Up-Color-None*, *Up-Suit-None*,
-*Up-Suit-None-NoSplit*, *Up-Suit-HighRun*, *Up-Suit-HighRun-NoSplit*,
-*Up-Suit-AnyRun*, *Up-Suit-AnyRun-NoSplit*. If a set of simulations
-consumed too much memory, the simulation was run setting a maximum
-number of states examined to 50 million, and win rates were
-calculated assuming all incomplete simulations were losses and 
-then again assuming all were wins.
-
-For each set of rules, the mean (standard deviation) and maximum number
-of states examined were also reported. This statistic counts repeated
-states each time they are created.
-
-Lastly, we calculated separate p-values testing the equality of our
-estimate with those published by Masten [5] and Wolter \[4\] (the latter
-only when the rule for empty piles was *None*). A Chi-square test or Fisher
-exact test was used, as appropriate.
-
-All simulations were run using a C++ port of this package. The
-first thousand simulations for each rule variant were also run using this
-Python package version 0.8.2 on Python version 3.11.2, and the simulation
-result (win, loss, exceeded maximum states) and number of states examined
-were confirmed to match the C++ version. A laptop running 32-bit
-Debian GNU/Linux 12 was used for the simulations. Statistical analyses
-were conducted in R v4.2.2.
-
-# Results
-The results of the simulations are shown in the table below.
-
-| Rule Variant              | Completed Simulations, (n) | Wins, n (% [95% CI])    | P-value [a] | Mean (SD) States Examined (10^3) | Maximum States Examined (10^6) |
-| :------------------------ | :--------------: | :---------------------: | :---------: | :-------------------:     | :-----------------: |
-| *Down-Color-None*         | 10,000           | 99 (1.0% [0.8%, 1.2%])  | 0.40        | 89.0 (156.1)              | 63.7                |
-| *Up-Color-None*           |  9,996 [b]       | 113 (1.1% [0.9%, 1.4%], 1.2% [1.0%, 1.4%]) | 0.02, 0.01 |  72.6 (112.8) | 46.3       |
-| *Up-Suit-None*            | 10,000           | 42 (0.4% [0.3%, 0.6%]   | <.0001      | 10.2 (163.9)              |  8.5                |
-| *Up-Suit-None-NoSplit*    | 10,000           | 40 (0.4% [0.3%, 0.5%])  | <.0001      | 5.9 (94.1)            |  6.1                |
-| *Up-Suit-HighRun*         | 10,000           | 1454 (14.5% [13.9%, 15.2%]) | 0.92    | 207.3 (999.3)         | 31.9                |
-| *Up-Suit-HighRun-NoSplit* | 10,000           | 1411 (14.1% [13.4%, 14.8%]) | 0.30    | 112.9 (500.9)         | 22.6                |
-| *Up-Suit-AnyRun-NoSplit*  | 10,000           | 6384 (63.8% [62.9%, 64.8%]) | 0.69    | 59.2 (340.2)          | 16.1                |
-
-[a] P-value for comparison vs Masten results.
-
-[b] Simulations stopped after 50,000,000 states examined. Win rates and P-values are reported twice assuming all incomplete simulations are losses and wins. Mean and maximum states examined are reported for completed simulations.
-
-# Discussion
-We found 1.1% - 1.2% of games were winnable under the *Up-Color-None* rules
-and 1.0% of games were winnable under the *Down-Color-None* rules. For the
-former, the comparison to Masten's results gave a statistically significant
-difference at the 95% confidence level while the latter did not.  Our
-simulations for *Up-Suit-HighRun*, *Up-Suit-HighRun-NoSplit*, and
-*Up-Suit-AnyRun-NoSplit* were not statistically significantly different from
-those of Masten, although *Up-Suit-None* and *Up-Suit-None-NoSplit* were.
-
-A limitation of using Masten's results is he states win rates but isn't
-explicit about which rules are used, with the exception of how empty
-piles are filled. He refers readers to Keller's discussion [6] for more
-information, and this discussion suggests that Agnes rules follow 
-Whitehead rules (another solitaire) and require movable runs to be
-the same suit. That is, Keller indicates the rules are *Up-Suit-None*
-in our terminology [5,6]. However, Keller then goes on to note that all
-computer implementations he had seen allow moves by colored runs and not
-by same-suit runs, which would corresponds to the *Up-Color-None* rules in
-our terminology. 
-
-It was unexpected to find that when the rule for empty piles is *None*, our
-results for dealing face-down and moving by color matched Masten, while
-when the rule for empty piles is *HighRun* or *AnyRun*, our results for
-dealing face-up and moving by suit matched. It is unclear if Masten 
-reported results for different move rules, if the statistically significant
-differences we found were due to chance, or if consistent rules were used
-for a variant we have not yet tested (e.g., *Up-Color-None-NoSplit*,
-*Up-Color-HighRun-NoSplit*, and *Up-Color-AnyRun-NoSplit*).
-
-Despite these uncertainties about Masten's estimates, we add 95% CIs to
-his reported win rates and include them here. He reports the previously
-mentioned win rate (95% CI) of 0.9% (0.8%, 1.0%) when empty
-columns cannot be filled with moves from the tableau, 63.6% (63.3%, 63.9%)
-when the empty column can be filled by any movable run or single card
-(or perhaps disallowing runs — Masten is not explicit, but our results
-match filling with a run or single card), and 14.5% (14.3%, 14.7%) when
-empty columns can be filled only by a run starting with the highest rank
-card or single highest-rank card (or again, perhaps disallowing runs).
-
-All of our results were larger than the 45/1,000,000 reported by Wolter
-at significance level P<.0001. Given the large difference between our
-results and Wolter's results, we believe Wolter's results are incorrect
-and should not be cited.
-
-We have estimated win rates that to our knowledge have not been previously
-reported for Parlett's variant (*Up-Suit-None-NoSplit*) and
-*Down-Color-None*, with the former less than half of *Up-Suit-None* and the
-latter about 10% smaller.
-
-Much of the work for this project was originally completed in 2019
-assuming all cards were dealt face-up using Python 3.5. This 2024 update
-used Python 3.11.2. In 2019 we ported the Python code to C++ for
-performance testing and found a five-fold improvement in speed. When
-porting the code to Python 3.11, we found a two-fold decrease in run-time
-when switching the data structures used from tuples to dataclasses for the
-structures representing cards and moves.
-
-We have not all possible rule variants with this package. We considered
-including *Up-Suit-AnyRun*, but preliminary estimates indicated 
-high memory usage and a longer run time, and therefore we defer analysis
-of this variant to a later package version. The current package has some options
-to manage the memory (e.g., disabling the set that tracking losing states
-at various thresholds), but additional optimizations are possible
-once the set is disabled that are not yet implemented (e.g., 
-requiring cards to be placed to the foundation before moving a pile that we
-hope will improve run time). In addition, the package options allow
-disabling of splitting same-suit runs before a move, but this option will
-likely be generalized to disallow splitting of movable runs and then
-can be applied when moves are allowed by color.
+A line-by-line explanation of this output is provided in [the git repository of the C++ implementation](https://github.com/ghrgriner/quagnes-cpp/wiki/Program-Input-and-Output#explanation-of-detailed-output).
+However, note that this Python package does not write any messages to
+standard error.
 
 # References
 [1] Agnes (card game). Wikipedia.
     https://en.wikipedia.org/wiki/Agnes_(card_game). Retrieved
     March 15, 2024.
 
 [2] Dalton W (1909). "My favourite Patiences" in The Strand Magazine,
     Vol 38.
 
 [3] Parlett D (1979). The Penguin Book of Patience. London: Penguin.
 
-[4] Wolter J (2013). Experimental analysis of Agnes Sorel solitaire.
-    https://politaire.com/article/agnessorel.html. Retrieved
-    March 15, 2024.
-
-[5] Masten M (2021). Agnes Sorel.
-    https://solitairewinrates.com/AgnesSorel.html. Retrieved
-    March 17, 2024.
-
-[6] Keller M (2021). Whitehead and Agnes -- packing in color.
-    https://www.solitairelaboratory.com/whitehead.html. Retrieved
-    March 17, 2024.
-
-[7] Wolter J (2014). Rules for Agnes Sorel solitaire.
-    https://politaire.com/help/agnessorel. Retrieved March 17, 2024.
-
 # Disclosures
 We are not affiliated with any of the books, websites, or applications
 discussed in this documentation, except of course for this Python package
-which we wrote.
+and previously-mentioned C++ implementation which we wrote.
```

