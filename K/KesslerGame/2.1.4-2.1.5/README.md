# Comparing `tmp/KesslerGame-2.1.4.tar.gz` & `tmp/KesslerGame-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KesslerGame-2.1.4.tar", last modified: Wed Apr 17 03:45:27 2024, max compression
+gzip compressed data, was "KesslerGame-2.1.5.tar", last modified: Thu Apr 18 17:30:49 2024, max compression
```

## Comparing `KesslerGame-2.1.4.tar` & `KesslerGame-2.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 03:45:27.105560 KesslerGame-2.1.4/
--rw-rw-rw-   0        0        0    11565 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/LICENSE
--rw-rw-rw-   0        0        0       73 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3345 2024-04-17 03:45:27.105560 KesslerGame-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2677 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/README.md
--rw-rw-rw-   0        0        0      477 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       29 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/requirements.txt
--rw-rw-rw-   0        0        0      896 2024-04-17 03:45:27.105560 KesslerGame-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      747 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 03:45:27.089930 KesslerGame-2.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 03:45:27.089930 KesslerGame-2.1.4/src/KesslerGame.egg-info/
--rw-rw-rw-   0        0        0     3345 2024-04-17 03:45:26.000000 KesslerGame-2.1.4/src/KesslerGame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2024-04-17 03:45:27.000000 KesslerGame-2.1.4/src/KesslerGame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 03:45:26.000000 KesslerGame-2.1.4/src/KesslerGame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-17 03:45:26.000000 KesslerGame-2.1.4/src/KesslerGame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 03:45:26.000000 KesslerGame-2.1.4/src/KesslerGame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 03:45:26.000000 KesslerGame-2.1.4/src/KesslerGame.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2024-04-17 03:45:27.089930 KesslerGame-2.1.4/src/kesslergame/
--rw-rw-rw-   0        0        0      701 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/_version.py
--rw-rw-rw-   0        0        0     7086 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/asteroid.py
--rw-rw-rw-   0        0        0     1886 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/bullet.py
--rw-rw-rw-   0        0        0     1423 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/collisions.py
--rw-rw-rw-   0        0        0     1432 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/controller.py
--rw-rw-rw-   0        0        0     6110 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/controller_gamepad.py
-drwxrwxrwx   0        0        0        0 2024-04-17 03:45:27.105560 KesslerGame-2.1.4/src/kesslergame/graphics/
--rw-rw-rw-   0        0        0      380 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/__init__.py
--rw-rw-rw-   0        0        0     1054 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/graphics_base.py
--rw-rw-rw-   0        0        0     3034 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/graphics_handler.py
--rw-rw-rw-   0        0        0     5761 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/graphics_plt.py
--rw-rw-rw-   0        0        0    13877 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/graphics_tk.py
--rw-rw-rw-   0        0        0     3912 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/graphics_ue.py
-drwxrwxrwx   0        0        0        0 2024-04-17 03:45:27.105560 KesslerGame-2.1.4/src/kesslergame/graphics/images/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/images/__init__.py
--rw-rw-rw-   0        0        0     2708 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/images/playerShip1_green.png
--rw-rw-rw-   0        0        0     2578 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/images/playerShip1_orange.png
--rw-rw-rw-   0        0        0     3597 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/images/playerShip2_orange.png
--rw-rw-rw-   0        0        0     2725 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/graphics/images/playerShip3_orange.png
--rw-rw-rw-   0        0        0    17992 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/kessler_game.py
--rw-rw-rw-   0        0        0     2035 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/mines.py
--rw-rw-rw-   0        0        0     6571 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/scenario.py
--rw-rw-rw-   0        0        0     2488 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/score.py
--rw-rw-rw-   0        0        0    11185 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/ship.py
--rw-rw-rw-   0        0        0     1881 2024-04-17 03:44:53.000000 KesslerGame-2.1.4/src/kesslergame/team.py
+drwxrwxrwx   0        0        0        0 2024-04-18 17:30:49.946946 KesslerGame-2.1.5/
+-rw-rw-rw-   0        0        0    11565 2024-04-18 17:30:20.000000 KesslerGame-2.1.5/LICENSE
+-rw-rw-rw-   0        0        0       73 2024-04-18 17:30:20.000000 KesslerGame-2.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3345 2024-04-18 17:30:49.946946 KesslerGame-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2677 2024-04-18 17:30:20.000000 KesslerGame-2.1.5/README.md
+-rw-rw-rw-   0        0        0      477 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       29 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/requirements.txt
+-rw-rw-rw-   0        0        0      896 2024-04-18 17:30:49.946946 KesslerGame-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      747 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 17:30:49.930585 KesslerGame-2.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 17:30:49.930585 KesslerGame-2.1.5/src/KesslerGame.egg-info/
+-rw-rw-rw-   0        0        0     3345 2024-04-18 17:30:49.000000 KesslerGame-2.1.5/src/KesslerGame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1182 2024-04-18 17:30:49.000000 KesslerGame-2.1.5/src/KesslerGame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 17:30:49.000000 KesslerGame-2.1.5/src/KesslerGame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-18 17:30:49.000000 KesslerGame-2.1.5/src/KesslerGame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-18 17:30:49.000000 KesslerGame-2.1.5/src/KesslerGame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-18 17:30:49.000000 KesslerGame-2.1.5/src/KesslerGame.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-18 17:30:49.930585 KesslerGame-2.1.5/src/kesslergame/
+-rw-rw-rw-   0        0        0      701 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/_version.py
+-rw-rw-rw-   0        0        0     7086 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/asteroid.py
+-rw-rw-rw-   0        0        0     1886 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/bullet.py
+-rw-rw-rw-   0        0        0     1423 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/collisions.py
+-rw-rw-rw-   0        0        0     1432 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/controller.py
+-rw-rw-rw-   0        0        0     6110 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/controller_gamepad.py
+drwxrwxrwx   0        0        0        0 2024-04-18 17:30:49.930585 KesslerGame-2.1.5/src/kesslergame/graphics/
+-rw-rw-rw-   0        0        0      380 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/graphics_base.py
+-rw-rw-rw-   0        0        0     3034 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/graphics_handler.py
+-rw-rw-rw-   0        0        0     5761 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/graphics_plt.py
+-rw-rw-rw-   0        0        0    14069 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/graphics_tk.py
+-rw-rw-rw-   0        0        0     3912 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/graphics_ue.py
+drwxrwxrwx   0        0        0        0 2024-04-18 17:30:49.946946 KesslerGame-2.1.5/src/kesslergame/graphics/images/
+-rw-rw-rw-   0        0        0        0 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/images/__init__.py
+-rw-rw-rw-   0        0        0     2708 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/images/playerShip1_green.png
+-rw-rw-rw-   0        0        0     2578 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/images/playerShip1_orange.png
+-rw-rw-rw-   0        0        0     3597 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/images/playerShip2_orange.png
+-rw-rw-rw-   0        0        0     2725 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/graphics/images/playerShip3_orange.png
+-rw-rw-rw-   0        0        0    18348 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/kessler_game.py
+-rw-rw-rw-   0        0        0     2035 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/mines.py
+-rw-rw-rw-   0        0        0     6571 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/scenario.py
+-rw-rw-rw-   0        0        0     2578 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/score.py
+-rw-rw-rw-   0        0        0    11185 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/ship.py
+-rw-rw-rw-   0        0        0     1920 2024-04-18 17:30:21.000000 KesslerGame-2.1.5/src/kesslergame/team.py
```

### Comparing `KesslerGame-2.1.4/LICENSE` & `KesslerGame-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/PKG-INFO` & `KesslerGame-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KesslerGame
-Version: 2.1.4
+Version: 2.1.5
 Summary: Asteroids game simulation environment for ML and AI applications
 Home-page: https://github.com/ThalesGroup/kessler-game
 Author: Zachariah Phillips
 Author-email: zach.phillips@defense.us.thalesgroup.com
 Maintainer: Timothy Arnett
 Maintainer-email: tim.arnett@defense.us.thalesgroup.com
 License: Apache 2.0 License
```

### Comparing `KesslerGame-2.1.4/README.md` & `KesslerGame-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/setup.cfg` & `KesslerGame-2.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/setup.py` & `KesslerGame-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/KesslerGame.egg-info/PKG-INFO` & `KesslerGame-2.1.5/src/KesslerGame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KesslerGame
-Version: 2.1.4
+Version: 2.1.5
 Summary: Asteroids game simulation environment for ML and AI applications
 Home-page: https://github.com/ThalesGroup/kessler-game
 Author: Zachariah Phillips
 Author-email: zach.phillips@defense.us.thalesgroup.com
 Maintainer: Timothy Arnett
 Maintainer-email: tim.arnett@defense.us.thalesgroup.com
 License: Apache 2.0 License
```

### Comparing `KesslerGame-2.1.4/src/KesslerGame.egg-info/SOURCES.txt` & `KesslerGame-2.1.5/src/KesslerGame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/__init__.py` & `KesslerGame-2.1.5/src/kesslergame/__init__.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/asteroid.py` & `KesslerGame-2.1.5/src/kesslergame/asteroid.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/bullet.py` & `KesslerGame-2.1.5/src/kesslergame/bullet.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/collisions.py` & `KesslerGame-2.1.5/src/kesslergame/collisions.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/controller.py` & `KesslerGame-2.1.5/src/kesslergame/controller.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/controller_gamepad.py` & `KesslerGame-2.1.5/src/kesslergame/controller_gamepad.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/graphics/graphics_base.py` & `KesslerGame-2.1.5/src/kesslergame/graphics/graphics_base.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/graphics/graphics_handler.py` & `KesslerGame-2.1.5/src/kesslergame/graphics/graphics_handler.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/graphics/graphics_plt.py` & `KesslerGame-2.1.5/src/kesslergame/graphics/graphics_plt.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/graphics/graphics_tk.py` & `KesslerGame-2.1.5/src/kesslergame/graphics/graphics_tk.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         # default_ui = {'ships': True, 'lives_remaining': True, 'accuracy': True, 'asteroids_hit': True}
         UI_settings = {} if UI_settings is None else UI_settings
         self.show_ships = UI_settings.get('ships', True)
         self.show_lives = UI_settings.get('lives_remaining', True)
         self.show_accuracy = UI_settings.get('accuracy', True)
         self.show_asteroids_hit = UI_settings.get('asteroids_hit', True)
         self.show_shots_fired = UI_settings.get('shots_fired', False)
-        self.show_bullets_remaining = UI_settings.get('bullets_remaining', False)
+        self.show_bullets_remaining = UI_settings.get('bullets_remaining', True)
+        self.show_mines_remaining = UI_settings.get('mines_remaining', True)
         self.show_controller_name = UI_settings.get('controller_name', True)
         self.script_dir = os.path.dirname(__file__)
         self.img_dir = os.path.join(self.script_dir, "images")
 
     def sort_list(self, order, list_to_order):
         i = len(order)
         sorted_list = [None] * (len(list_to_order) + (len(order)))
@@ -186,14 +187,16 @@
             team_info += "Accuracy: " + str(round(team.accuracy * 100, 1)) + "\n"
         if self.show_asteroids_hit:
             team_info += "Asteroids Hit: " + str(team.asteroids_hit) + "\n"
         if self.show_shots_fired:
             team_info += "Shots Fired: " + str(team.shots_fired) + "\n"
         if self.show_bullets_remaining:
             team_info += "Bullets Left: " + str(team.bullets_remaining) + "\n"
+        if self.show_mines_remaining:
+            team_info += "Mines Left: " + str(team.mines_remaining) + "\n"
 
         return team_info
 
     def plot_ships(self, ships: List[Ship]) -> None:
         """
         Plots each ship on the game screen using cached sprites and rotating them
         """
```

### Comparing `KesslerGame-2.1.4/src/kesslergame/graphics/graphics_ue.py` & `KesslerGame-2.1.5/src/kesslergame/graphics/graphics_ue.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/graphics/images/playerShip1_green.png` & `KesslerGame-2.1.5/src/kesslergame/graphics/images/playerShip1_green.png`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/graphics/images/playerShip1_orange.png` & `KesslerGame-2.1.5/src/kesslergame/graphics/images/playerShip1_orange.png`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/graphics/images/playerShip2_orange.png` & `KesslerGame-2.1.5/src/kesslergame/graphics/images/playerShip2_orange.png`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/graphics/images/playerShip3_orange.png` & `KesslerGame-2.1.5/src/kesslergame/graphics/images/playerShip3_orange.png`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/kessler_game.py` & `KesslerGame-2.1.5/src/kesslergame/kessler_game.py`

 * *Files 3% similar despite different names*

```diff
@@ -318,19 +318,22 @@
             # --- CHECK STOP CONDITIONS --------------------------------------------------------------------------------
             sim_time += self.time_step
             step += 1
 
             # No asteroids remain
             if not asteroids:
                 stop_reason = StopReason.no_asteroids
-            # No ships are alive
-            elif not liveships:
+            # No ships are alive and no mines exist and no bullets exist
+            # Prevents unfairness where ship that dies before another gets score from its bullets as long as the other
+            # is alive but the one that lives longer doesn't get the same benefit from its bullets/mines persisting
+            # after it dies
+            elif not liveships and not len(mines) > 0 and not len(bullets) > 0:
                 stop_reason = StopReason.no_ships
             # All live ships are out of bullets and no bullets are on map
-            elif not sum([ship.bullets_remaining for ship in liveships]) and not len(bullets)>0 and scenario.stop_if_no_ammo:
+            elif not sum([ship.bullets_remaining for ship in liveships]) and not len(bullets) > 0 and scenario.stop_if_no_ammo:
                 stop_reason = StopReason.out_of_bullets
             # Out of time
             elif sim_time > time_limit:
                 stop_reason = StopReason.time_expired
 
             # --- FINISHING TIME STEP ----------------------------------------------------------------------------------
             # Get overall time step compute time
```

### Comparing `KesslerGame-2.1.4/src/kesslergame/mines.py` & `KesslerGame-2.1.5/src/kesslergame/mines.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/scenario.py` & `KesslerGame-2.1.5/src/kesslergame/scenario.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/score.py` & `KesslerGame-2.1.5/src/kesslergame/score.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,25 @@
             for ship in scenario.ships():
                 if team.team_id == ship.team:
                     team.total_bullets += scenario.bullet_limit
 
     def update(self, ships: List[Ship], sim_time: float, controller_perf: Optional[List[float]] = None) -> None:
         self.sim_time = sim_time
         for team in self.teams:
-            ast_hit, bul_hit, shots, bullets, deaths, lives = (0, 0, 0, 0, 0, 0)
+            ast_hit, bul_hit, shots, bullets, mines, deaths, lives = (0, 0, 0, 0, 0, 0, 0)
             for idx, ship in enumerate(ships):
                 if team.team_id == ship.team:
                     ast_hit += ship.asteroids_hit
                     bul_hit += ship.bullets_hit
                     shots += ship.bullets_shot
                     bullets += ship.bullets_remaining
+                    mines += ship.mines_remaining
                     deaths += ship.deaths
                     lives += ship.lives
                     if controller_perf is not None and controller_perf[idx] > 0:
                         team.eval_times.append(controller_perf[idx])
-            team.asteroids_hit, team.bullets_hit, team.shots_fired, team.bullets_remaining, team.deaths, team.lives_remaining = (ast_hit, bul_hit, shots, bullets, deaths, lives)
+            team.asteroids_hit, team.bullets_hit, team.shots_fired, team.bullets_remaining, team.mines_remaining, team.deaths, team.lives_remaining = (ast_hit, bul_hit, shots, bullets, mines, deaths, lives)
 
     def finalize(self, sim_time: float, stop_reason: 'StopReason', ships: List[Ship]) -> None:
         self.sim_time = sim_time
         self.stop_reason = stop_reason
         self.final_controllers = [ship.controller for ship in ships]
```

### Comparing `KesslerGame-2.1.4/src/kesslergame/ship.py` & `KesslerGame-2.1.5/src/kesslergame/ship.py`

 * *Files identical despite different names*

### Comparing `KesslerGame-2.1.4/src/kesslergame/team.py` & `KesslerGame-2.1.5/src/kesslergame/team.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         self.total_bullets: int = 0
         self.total_asteroids: int = 0
 
         self.asteroids_hit: int = 0
         self.bullets_hit: int = 0
         self.shots_fired: int = 0
         self.bullets_remaining: int = 0
+        self.mines_remaining: int = 0
         self.deaths: int = 0
         self.eval_times: list[float] = []
         self.lives_remaining: int = 0
 
     @property
     def accuracy(self) -> float:
         return self.bullets_hit / self.shots_fired if self.shots_fired else 0.0
```

