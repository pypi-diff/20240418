# Comparing `tmp/BHBot-master-1.1.tar.gz` & `tmp/bhbot_master-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BHBot-master-1.1.tar", last modified: Tue Mar 19 19:49:08 2024, max compression
+gzip compressed data, was "bhbot_master-2.1.tar", last modified: Thu Apr 18 20:31:53 2024, max compression
```

## Comparing `BHBot-master-1.1.tar` & `bhbot_master-2.1.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:49:08.485429 BHBot-master-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:49:08.485429 BHBot-master-1.1/BHBot_master.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-03-19 19:49:08.000000 BHBot-master-1.1/BHBot_master.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-19 19:49:08.000000 BHBot-master-1.1/BHBot_master.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:49:08.000000 BHBot-master-1.1/BHBot_master.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:49:08.000000 BHBot-master-1.1/BHBot_master.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-19 19:49:04.000000 BHBot-master-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-03-19 19:49:08.485429 BHBot-master-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-19 19:49:04.000000 BHBot-master-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-19 19:49:04.000000 BHBot-master-1.1/abstract_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    20275 2024-03-19 19:49:04.000000 BHBot-master-1.1/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-03-19 19:49:04.000000 BHBot-master-1.1/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-19 19:49:04.000000 BHBot-master-1.1/client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-03-19 19:49:04.000000 BHBot-master-1.1/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-03-19 19:49:04.000000 BHBot-master-1.1/direct_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-19 19:49:04.000000 BHBot-master-1.1/font_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-03-19 19:49:04.000000 BHBot-master-1.1/levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-03-19 19:49:04.000000 BHBot-master-1.1/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 19:49:08.485429 BHBot-master-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-19 19:49:04.000000 BHBot-master-1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-03-19 19:49:04.000000 BHBot-master-1.1/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-03-19 19:49:04.000000 BHBot-master-1.1/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:53.240865 bhbot_master-2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:31:53.240865 bhbot_master-2.1/BHBot_master.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-18 20:31:53.000000 bhbot_master-2.1/BHBot_master.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 20:31:53.000000 bhbot_master-2.1/BHBot_master.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:31:53.000000 bhbot_master-2.1/BHBot_master.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:31:53.000000 bhbot_master-2.1/BHBot_master.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-18 20:31:49.000000 bhbot_master-2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-18 20:31:53.240865 bhbot_master-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-18 20:31:49.000000 bhbot_master-2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-18 20:31:49.000000 bhbot_master-2.1/abstract_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20821 2024-04-18 20:31:49.000000 bhbot_master-2.1/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-18 20:31:49.000000 bhbot_master-2.1/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 20:31:49.000000 bhbot_master-2.1/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-18 20:31:49.000000 bhbot_master-2.1/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-18 20:31:49.000000 bhbot_master-2.1/direct_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 20:31:49.000000 bhbot_master-2.1/font_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-04-18 20:31:49.000000 bhbot_master-2.1/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-18 20:31:49.000000 bhbot_master-2.1/levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-18 20:31:49.000000 bhbot_master-2.1/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 20:31:49.000000 bhbot_master-2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:31:53.240865 bhbot_master-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-18 20:31:49.000000 bhbot_master-2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 20:31:49.000000 bhbot_master-2.1/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-04-18 20:31:49.000000 bhbot_master-2.1/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-18 20:31:49.000000 bhbot_master-2.1/windows.py
```

### Comparing `BHBot-master-1.1/LICENSE` & `bhbot_master-2.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+Unlicense
 This is free and unencumbered software released into the public domain.
 
 Anyone is free to copy, modify, publish, use, compile, sell, or
 distribute this software, either in source code form or as a compiled
 binary, for any purpose, commercial or non-commercial, and by any
 means.
```

### Comparing `BHBot-master-1.1/abstract_mode.py` & `bhbot_master-2.1/abstract_mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,9 +22,11 @@
         pass
 
     @classmethod
     def get_name(cls):
         if isinstance(cls.name, str):
             return cls.name  # Shouldn't be used, here for backwards compatibility
         elif isinstance(cls.name, dict):
-            return cls.name.get(global_settings.language_name, cls.name.get('default', cls.__name__))
+            return cls.name.get(
+                global_settings.language_name, cls.name.get("default", cls.__name__)
+            )
         return cls.__name__
```

### Comparing `BHBot-master-1.1/bot.py` & `bhbot_master-2.1/bot.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,92 +72,108 @@
         if self.find_brawlhalla():
             self.brawlhalla.kill()
             sleep(5)
 
         try:
             steam = SteamClient()
         except SteamExeNotFound:
-            logger.error('no_steam_exe')
+            logger.error("no_steam_exe")
             return self.on_exit()
         count = 10000
         while not self.find_brawlhalla():
-            logger.debug('waiting_for_bh_window')
+            logger.debug("waiting_for_bh_window")
             self.process_queue()
             count += 1
             if count >= 10000:
                 steam.run_brawlhalla()
                 count = 0
 
         self.virtual_input = VirtualInput(self.brawlhalla, self.hotkeys)
         self.level_definer = LevelDefiner(self.brawlhalla)
 
-        logger.info('found_bh')
+        logger.info("found_bh")
         self.virtual_input.esc()  # idk why but it puts bh into windowed
         sleep(1)
         if self.brawlhalla.fullscreen:
-            logger.info('not_windowed_mode')
+            logger.info("not_windowed_mode")
             raise NotRespondingError
         self.brawlhalla.resize()
         self.get_states()
         if self.config.stealth:
-            logger.info('stealth_mode')
+            logger.info("stealth_mode")
             self.brawlhalla.hide()
             self.brawlhalla.set_low_priority()
 
     def initialize(self):
         self.ensure_brawlhalla()
         self.duration = 15
 
         self.go_to_menu(True)
         regenerate_layout()
-        self.current_menu_element = find_element('first_column').current_element
+        self.current_menu_element = find_element("first_column").current_element
         sleep(2)
 
         if self.config.mute:
             self.mute()
 
         if not self.characters:
             if self.mode.parse_character_levels:
                 self.characters = self.get_characters()
-                self.unlocked_characters = [character for character in self.characters if character.unlocked]
+                self.unlocked_characters = [
+                    character for character in self.characters if character.unlocked
+                ]
             else:
                 self.characters = [Character(name) for name in characters]
                 self.unlocked_characters = self.characters
 
         self.character = self.unlocked_characters[0]
-        logger.debug('initialized')
+        logger.debug("initialized")
 
     def on_exit(self):
         if self.virtual_input:
             self.virtual_input.release_keys()
         if self.config.stealth and self.brawlhalla:
             self.brawlhalla.kill()
-        text = global_settings.messages.get('initial_on_exit', 'initial_on_exit') % (format_time(time() - self.time_started), self.games_completed, self.crashes, self.total_xp)
+        text = global_settings.messages.get("initial_on_exit", "initial_on_exit") % (
+            format_time(time() - self.time_started),
+            self.games_completed,
+            self.crashes,
+            self.total_xp,
+        )
         if self.mode.parse_character_levels:
-            text += global_settings.messages.get('on_exit_has_rewards', 'on_exit_has_rewards') % (self.total_gold,)
+            text += global_settings.messages.get(
+                "on_exit_has_rewards", "on_exit_has_rewards"
+            ) % (self.total_gold,)
         else:
-            text += global_settings.messages.get('on_exit_no_rewards', 'on_exit_no_rewards') % (self.total_gold,)
+            text += global_settings.messages.get(
+                "on_exit_no_rewards", "on_exit_no_rewards"
+            ) % (self.total_gold,)
         box(text, endmargin=False)
         global_settings.update_stats(time=time() - self._time_started)
         stats = global_settings.get_stats()
-        total = global_settings.messages.get('total_stats', 'total_stats') % (stats.get('games', 0), stats.get('xp', 0), stats.get('gold', 0), format_time(stats.get('time', 0)))
+        total = global_settings.messages.get("total_stats", "total_stats") % (
+            stats.get("games", 0),
+            stats.get("xp", 0),
+            stats.get("gold", 0),
+            format_time(stats.get("time", 0)),
+        )
         box(total, endmargin=False)
         sys.exit()
 
     def process_queue(self, stop_delayed=False):
         put_back = []
         while not self.queue.empty():
             try:
                 msg = self.queue.get_nowait()
             except queue.Empty:
                 continue
             self.queue.task_done()
-            if msg == 'STOP':
+            if msg == "STOP":
                 raise KeyboardInterrupt
-            elif msg == 'DELAYED_STOP':
+            elif msg == "DELAYED_STOP":
                 if stop_delayed:
                     raise KeyboardInterrupt
                 put_back.append(msg)  # cycle it in queue waiting for delayed_stop check
         for item in put_back:
             self.queue.put_nowait(item)
 
     def check_stuff(self):
@@ -168,115 +184,114 @@
             raise NotRespondingError
 
     @property
     def state_conditions(self):
         conn_x = 1806 - ceil(98.5 * 2)  # 1609
         low_conn_x = conn_x - 26  # 1583
 
-        _new_menu = {
-            'pixels': ((1890, 70),),
-            'colors': ((255, 255, 255),)
-        }
+        _new_menu = {"pixels": ((1890, 70),), "colors": ((255, 255, 255),)}
 
         res = {
-            'ingame': {
-                'pixels': ((conn_x, 58),),
-                'colors': (CONNECTION_LEVELS[0],),
-            },
-            'low_connection': {
-                'pixels': ((low_conn_x, 74),),
-                'colors': CONNECTION_LEVELS,
-            },
-            'menu': self.state_detection_pixels.get('menu') or _new_menu,
-            'loading': {
-                'pixels': ((899, 85),),
-                'colors': ((227, 248, 255),),
-            },
-            'bonus': {
-                'pixels': ((930, 320),),
-                'colors': ((109, 198, 211),),
-            },
-            'offline': {
-                'pixels': ((1674, 26),),
-                'colors': ((55, 66, 100), (57, 67, 101)),
-            },
-            'sorted_by_date': {
-                'pixels': ((331, 766),),
-                'colors': ((254, 254, 255),),
-            },
-            'lobby': {
-                'pixels': ((1325, 22),),
-                'colors': ((255, 255, 255),),
-            },
-            'game_in_progress': {
-                'pixels': ((960, 395),),
-                'colors': ((111, 200, 211),),
-            },
-            'settings_open': {
-                'pixels': ((1221, 106),),
-                'colors': ((220, 220, 222),),
-            },
-            'disconnected': {
-                'pixels': ((934, 623),),
-                'colors': ((247, 248, 249),),
-            },
-            'system_settings_selected': {
-                'pixels': ((1607, 195),),
-                'colors': ((39, 85, 136),),
-            },
-            'on_rewards_screen': {
-                'pixels': ((1035, 121),),
-                'colors': ((255, 255, 255),),
-            },
-            'level_up': {
-                'pixels': ((1363, 320),),
-                'colors': ((19, 133, 51),),
-            },
-            'popup': {
-                'pixels': ((940, 790),),
-                'colors': ((247, 248, 249),),
-            },
-            'in_mallhalla': {
-                'pixels': ((338, 972),),
-                'colors': ((100, 77, 255),),
-            },
-            'in_battle_pass': {
-                'pixels': ((171, 660),),
-                'colors': ((181, 201, 225),),
+            "ingame": {
+                "pixels": ((conn_x, 58),),
+                "colors": (CONNECTION_LEVELS[0],),
+            },
+            "low_connection": {
+                "pixels": ((low_conn_x, 74),),
+                "colors": CONNECTION_LEVELS,
+            },
+            "menu": self.state_detection_pixels.get("menu") or _new_menu,
+            "loading": {
+                "pixels": ((899, 85),),
+                "colors": ((227, 248, 255),),
+            },
+            "bonus": {
+                "pixels": ((930, 320),),
+                "colors": ((109, 198, 211),),
+            },
+            "offline": {
+                "pixels": ((1674, 26),),
+                "colors": ((55, 66, 100), (57, 67, 101)),
+            },
+            "sorted_by_date": {
+                "pixels": ((331, 766),),
+                "colors": ((254, 254, 255),),
+            },
+            "lobby": {
+                "pixels": ((1325, 22),),
+                "colors": ((255, 255, 255),),
+            },
+            "game_in_progress": {
+                "pixels": ((960, 395),),
+                "colors": ((111, 200, 211),),
+            },
+            "settings_open": {
+                "pixels": ((1221, 106),),
+                "colors": ((220, 220, 222),),
+            },
+            "disconnected": {
+                "pixels": ((934, 623),),
+                "colors": ((247, 248, 249),),
+            },
+            "system_settings_selected": {
+                "pixels": ((1607, 195),),
+                "colors": ((39, 85, 136),),
+            },
+            "on_rewards_screen": {
+                "pixels": ((1035, 121),),
+                "colors": ((255, 255, 255),),
+            },
+            "level_up": {
+                "pixels": ((1363, 320),),
+                "colors": ((19, 133, 51),),
+            },
+            "popup": {
+                "pixels": ((940, 790),),
+                "colors": ((247, 248, 249),),
+            },
+            "in_mallhalla": {
+                "pixels": ((338, 972),),
+                "colors": ((100, 77, 255),),
+            },
+            "in_battle_pass": {
+                "pixels": ((171, 660),),
+                "colors": ((181, 201, 225),),
             },
         }
 
         for key in res.keys():
-            if key != 'menu' and key in self.state_detection_pixels:
+            if key != "menu" and key in self.state_detection_pixels:
                 res[key] = self.state_detection_pixels[key]
 
         return res
 
     @property
     def duration_setting(self):
-        return [self.open_settings, 1] + \
-            [self.virtual_input.down] * 3 + \
-            (self.mode.next_duration - self.duration) * [self.virtual_input.right] + \
-            (self.duration - self.mode.next_duration) * [self.virtual_input.left] + \
-            [self.virtual_input.quick]
+        return (
+            [self.open_settings, 1]
+            + [self.virtual_input.down] * 3
+            + (self.mode.next_duration - self.duration) * [self.virtual_input.right]
+            + (self.duration - self.mode.next_duration) * [self.virtual_input.left]
+            + [self.virtual_input.quick]
+        )
 
     @property
     def danger_zone(self):
-        return {'in_mallhalla', 'in_battle_pass'}
+        return {"in_mallhalla", "in_battle_pass"}
 
     @property
     def safe_states(self):
-        return {'ingame', 'low_connection'}
+        return {"ingame", "low_connection"}
 
     @staticmethod
     def is_color(screenshot, pixels, colors):
-        tmp = [ screenshot.getpixel(pixel) for pixel in pixels ]
+        tmp = [screenshot.getpixel(pixel) for pixel in pixels]
         return any(screenshot.getpixel(pixel) in colors for pixel in pixels)
 
-    def execute_steps(self, *steps, delay=.2):
+    def execute_steps(self, *steps, delay=0.2):
         self.get_states()
         for step in steps:
             if isinstance(step, (int, float)):
                 sleep(step)
             elif isinstance(step, str):
                 if step in self.virtual_input.keys:
                     self.virtual_input.press_key(self.virtual_input.keys[step])
@@ -291,39 +306,42 @@
         try:
             self.initialize()
             self.initial_setup()
 
             while True:
                 self.execute_steps(self.before_fight, self.go_to_fight)
 
-                logger.info('started_fighting')
-                last, ig = True, True  # To avoid failing ingame detection on low connection bc of "Double kill" popup covering first connection column for 1 frame
+                logger.info("started_fighting")
+                last, ig = (
+                    True,
+                    True,
+                )  # To avoid failing ingame detection on low connection bc of "Double kill" popup covering first connection column for 1 frame
                 while last or ig:
                     self.get_states()
-                    last, ig = ig, self.has_state('ingame', 'low_connection')
+                    last, ig = ig, self.has_state("ingame", "low_connection")
                     self.virtual_input.fight()
 
-                self.execute_steps('ended_fighting', 5, self.after_fight)
+                self.execute_steps("ended_fighting", 5, self.after_fight)
 
         except NotRespondingError:
             self.crashes += 1
             sleep(5)
-            logger.info('reinitializing')
+            logger.info("reinitializing")
         except QueuedRecalculation:
             sleep(5)
-            logger.info('queued_recalc')
+            logger.info("queued_recalc")
         except ResizedError:
-            logger.warning('resized_warning')
+            logger.warning("resized_warning")
             sleep(5)
         except DangerZoneError:
-            logger.warning('danger_zone_warning')
+            logger.warning("danger_zone_warning")
             sleep(5)
         except InvalidStateError:
             self.crashes += 1
-            logger.warning('invalid_state_warning')
+            logger.warning("invalid_state_warning")
             sleep(5)
 
     def main_loop(self):
         while True:
             try:
                 self.main_sequence()
             except KeyboardInterrupt:
@@ -349,226 +367,257 @@
 
     def has_state(self, *states):
         return self.last_states & set(states)
 
     def go_to_menu(self, initial=False):
         iters = 0
         self.get_states()
-        while not self.has_state('menu'):
+        while not self.has_state("menu"):
             iters += 1
-            logger.debug('not_in_menu')
+            logger.debug("not_in_menu")
             self.virtual_input.esc()
             sleep(1)
-            if self.has_state('bonus'):
-                logger.info('collecting_bonus')
+            if self.has_state("bonus"):
+                logger.info("collecting_bonus")
                 self.virtual_input.quick()
-            if self.has_state('popup'):
-                logger.info('accepting_event_popup')
+            if self.has_state("popup"):
+                logger.info("accepting_event_popup")
                 self.virtual_input.quick()
-            if not initial and self.has_state('offline'):
-                logger.info('offline')
-                self.select_menu_item('custom_game_room')
+            if not initial and self.has_state("offline"):
+                logger.info("offline")
+                self.select_menu_item("custom_game_room")
                 self.go_to_lobby(100)
-                logger.info('reconnected')
+                logger.info("reconnected")
                 self.go_to_menu()
             if iters > 100:
                 raise NotRespondingError
             self.get_states()
 
     def select_item(self, item, *steps):
-        while not self.has_state(f'{item}_selected'):
-            logger.debug('item_not_selected', item)
-            self.execute_steps(*steps, delay=.05)
-            if self.has_state('game_in_progress'):
+        while not self.has_state(f"{item}_selected"):
+            logger.debug("item_not_selected", item)
+            self.execute_steps(*steps, delay=0.05)
+            if self.has_state("game_in_progress"):
                 self.virtual_input.dodge()
 
     def select_menu_item(self, name):
         target = find_element(name)
         keys = self.current_menu_element.move_to(target, self.virtual_input)
         self.current_menu_element = target
         self.execute_steps(*keys)
 
     def mute(self):
-        logger.info('muting')
-        self.select_menu_item('system_settings')
+        logger.info("muting")
+        self.select_menu_item("system_settings")
         self.get_states()
-        if not self.has_state('system_settings_selected'):
+        if not self.has_state("system_settings_selected"):
             raise InvalidStateError
-        self.execute_steps(self.virtual_input.quick, *([self.virtual_input.left] * 10), self.virtual_input.down, *([self.virtual_input.left] * 10), self.virtual_input.dodge)
+        self.execute_steps(
+            self.virtual_input.quick,
+            *([self.virtual_input.left] * 10),
+            self.virtual_input.down,
+            *([self.virtual_input.left] * 10),
+            self.virtual_input.dodge,
+        )
 
     def sort_by_date(self):
         counter = 0
-        while not self.has_state('sorted_by_date'):
-            logger.debug('sorting_by_date')
+        while not self.has_state("sorted_by_date"):
+            logger.debug("sorting_by_date")
             self.virtual_input.enter()
-            sleep(.5)
+            sleep(0.5)
             self.get_states()
             if counter > 10:
                 raise InvalidStateError
             counter += 1
 
     def get_characters(self):
         _characters = []
         rotation = get_rotation()
-        self.select_menu_item('meet_the_legends')
-        self.execute_steps(self.virtual_input.quick, .5, self.sort_by_date)
-        logger.info('collecting_character_data')
+        self.select_menu_item("meet_the_legends")
+        self.execute_steps(self.virtual_input.quick, 0.5, self.sort_by_date)
+        logger.info("collecting_character_data")
         for line in level_character_matrix:
             for character in line:
                 self.get_states()
                 level = self.level_definer.get_level()
                 xp = self.level_definer.get_xp(level)
                 unlocked = character in rotation or self.level_definer.get_unlocked()
                 _characters.append(Character(character, level, xp, unlocked))
                 logger.info(_characters[-1])
                 self.virtual_input.right()
-                sleep(.15)
-            #self.virtual_input.down()
-            sleep(.15)
-        unlocked_characters = [character.name for character in _characters if character.unlocked]
-        locked_characters = [character.name for character in _characters if not character.unlocked]
-        fixed_characters = unlocked_characters + ['random'] + locked_characters
+                sleep(0.15)
+            # self.virtual_input.down()
+            sleep(0.15)
+        unlocked_characters = [
+            character.name for character in _characters if character.unlocked
+        ]
+        locked_characters = [
+            character.name for character in _characters if not character.unlocked
+        ]
+        fixed_characters = unlocked_characters + ["random"] + locked_characters
         build_character_matrix(fixed_characters)
         self.go_to_menu()
         return _characters
 
     def go_to_lobby(self, max_iters=10):
         iters = 0
-        while not self.has_state('lobby'):
+        while not self.has_state("lobby"):
             self.virtual_input.quick()
             sleep(2)
             if iters > max_iters:
                 raise InvalidStateError
             self.get_states()
             iters += 1
 
     def validate_level(self):
         self.go_to_rewards_screen()
-        if self.duration < 3 or self.has_state('level_up'):
-            logger.debug('skip_lvl_valid')
+        if self.duration < 3 or self.has_state("level_up"):
+            logger.debug("skip_lvl_valid")
             return True
         xp = self.level_definer.get_xp(self.character.level, True)
         calculated_xp = get_duration_xp(self.duration)
-        logger.debug('calc_xp', calculated_xp)
-        logger.debug('pixel_xp', xp)
-        if (self.character.level < 40 and abs(xp - calculated_xp) > calculated_xp / 3):
-            logger.info('xp_discrep')
+        logger.debug("calc_xp", calculated_xp)
+        logger.debug("pixel_xp", xp)
+        if self.character.level < 40 and abs(xp - calculated_xp) > calculated_xp / 3:
+            logger.info("xp_discrep")
             return False
         return True
 
     def go_to_rewards_screen(self):
-        while not self.has_state('on_rewards_screen'):
+        while not self.has_state("on_rewards_screen"):
             self.virtual_input.quick()
             sleep(5)
             self.get_states()
 
     def open_settings(self):
-        while not self.has_state('settings_open'):
+        while not self.has_state("settings_open"):
             self.virtual_input.heavy()
             sleep(2)
             self.get_states()
 
     def wait_for_loading(self):
         iters = 0
-        while not self.has_state('loading'):
-            logger.debug('waiting_for_loading')
+        while not self.has_state("loading"):
+            logger.debug("waiting_for_loading")
             iters += 1
             self.virtual_input.quick()
             sleep(2)
             if iters > self.duration * 60:
                 raise NotRespondingError
             self.get_states()
 
     def wait_for_loaded(self):
         iters = 0
-        while self.has_state('loading'):
-            logger.debug('loading')
+        while self.has_state("loading"):
+            logger.debug("loading")
             iters += 1
             sleep(1)
             if iters > 100:
                 raise InvalidStateError
             self.get_states()
 
     def pick_character(self):
-        logger.info('pick_char', self.mode.next_character)
+        logger.info("pick_char", self.mode.next_character)
         if self.character != self.mode.next_character:
-            self.execute_steps(*self.character.get_path_to(self.mode.next_character.name))
+            self.execute_steps(
+                *self.character.get_path_to(self.mode.next_character.name)
+            )
             self.character = self.mode.next_character
 
     def set_duration(self):
-        logger.info('setting_dur', self.mode.next_duration)
+        logger.info("setting_dur", self.mode.next_duration)
         if self.duration != self.mode.next_duration:
             self.execute_steps(*self.duration_setting)
             self.duration = self.mode.next_duration
 
     def reset_xp(self):
-        self.execute_steps(self.virtual_input.dodge, self.virtual_input.dodge, self.go_to_menu)
+        self.execute_steps(
+            self.virtual_input.dodge, self.virtual_input.dodge, self.go_to_menu
+        )
         waiting_start = time()
-        logger.info('wait_for_xp_reset', self.config.auto_stop_duration)
+        logger.info("wait_for_xp_reset", self.config.auto_stop_duration)
         while time() - waiting_start < self.config.auto_stop_duration * 60:
-            logger.debug('wait_remaining', int(waiting_start + self.config.auto_stop_duration * 60 - time()))
+            logger.debug(
+                "wait_remaining",
+                int(waiting_start + self.config.auto_stop_duration * 60 - time()),
+            )
             self.check_stuff()
             sleep(1)
         self.last_pause = time()
         self.characters = []
         self.unlocked_characters = []
         raise QueuedRecalculation
 
     def setup_lobby(self):
         # noinspection PyTypeChecker
-        steps = [self.open_settings] + \
-                [self.virtual_input.right] * 10 + \
-                [self.virtual_input.down] * 3 + \
-                [self.virtual_input.left] * (2 - self.duration) + \
-                [self.virtual_input.right] * (self.duration - 2) + \
-                [self.virtual_input.down] * 2 + \
-                [self.virtual_input.left] * 6 + \
-                [self.virtual_input.down] * 2 + \
-                [self.virtual_input.right] + \
-                [self.virtual_input.rbr] + \
-                [self.virtual_input.down] * 3 + \
-                [self.virtual_input.left, self.virtual_input.down] * 3 + \
-                [self.virtual_input.left, self.virtual_input.quick]
+        steps = (
+            [self.open_settings]
+            + [self.virtual_input.right] * 8
+            + [self.virtual_input.down] * 3
+            + [self.virtual_input.left] * (2 - self.duration)
+            + [self.virtual_input.right] * (self.duration - 2)
+            + [self.virtual_input.down] * 2
+            + [self.virtual_input.left] * 6
+            + [self.virtual_input.down] * 2
+            + [self.virtual_input.right]
+            + [self.virtual_input.rbr]
+            + [self.virtual_input.down] * 3
+            + [self.virtual_input.left, self.virtual_input.down] * 3
+            + [self.virtual_input.left, self.virtual_input.quick]
+        )
         self.execute_steps(*steps)
 
     def add_bots(self):
-        steps = [self.virtual_input.throw, 1] + \
-                [self.virtual_input.down] * 3 + \
-                [self.virtual_input.quick] * 4 + \
-                [self.virtual_input.throw]
+        steps = (
+            [self.virtual_input.throw, 1]
+            + [self.virtual_input.down] * 3
+            + [self.virtual_input.quick] * 4
+            + [self.virtual_input.throw]
+        )
         self.execute_steps(*steps)
 
     def initial_setup(self):
-        self.execute_steps('creating_lobby', 1, 1)
-        self.select_menu_item('custom_game_room')
-        self.execute_steps(self.go_to_lobby, 'setting_lobby', self.setup_lobby, 4, self.add_bots)
+        self.execute_steps("creating_lobby", 1, 1)
+        self.select_menu_item("custom_game_room")
+        self.execute_steps(
+            self.go_to_lobby, "setting_lobby", self.setup_lobby, 4, self.add_bots
+        )
 
     def before_fight(self):
         self.execute_steps(2, self.pick_character, 1, self.set_duration, 1)
 
     def go_to_fight(self):
         self.process_queue(True)
-        self.execute_steps('starting_game', self.wait_for_loading, self.wait_for_loaded, 'loaded', 5)
+        self.execute_steps(
+            "starting_game", self.wait_for_loading, self.wait_for_loaded, "loaded", 5
+        )
 
     def after_fight(self):
         self.get_states()
-        if self.has_state('disconnected', 'game_in_progress', 'offline'):
-            logger.info('disconnected')
+        if self.has_state("disconnected", "game_in_progress", "offline"):
+            logger.info("disconnected")
             raise NotRespondingError
         self.games_completed += 1
         calc_xp = get_duration_xp(self.duration)
         time_to_sleep = self.config.auto_stop and (
-                (not self.config.auto_detect_auto_stop and time() - self.last_pause > self.config.auto_stop_frequency * 3600)
-                or (self.config.auto_detect_auto_stop and not self.validate_level()))
+            (
+                not self.config.auto_detect_auto_stop
+                and time() - self.last_pause > self.config.auto_stop_frequency * 3600
+            )
+            or (self.config.auto_detect_auto_stop and not self.validate_level())
+        )
         gold_for_level_up = self.character.add_xp(calc_xp)
         calc_gold = get_duration_gold(self.duration) + gold_for_level_up
         self.total_xp += calc_xp
         self.total_gold += calc_gold
-        logger.debug('update_total_stats')
-        global_settings.update_stats(games=1, time=time() - self._time_started, gold=calc_gold, xp=calc_xp)
+        logger.debug("update_total_stats")
+        global_settings.update_stats(
+            games=1, time=time() - self._time_started, gold=calc_gold, xp=calc_xp
+        )
         self._time_started = time()
-        logger.info('return_to_lobby')
+        logger.info("return_to_lobby")
         self.go_to_lobby()
         sleep(2)
         self.process_queue(True)
         if time_to_sleep:
             self.reset_xp()
```

### Comparing `BHBot-master-1.1/characters.py` & `bhbot_master-2.1/characters.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,109 @@
 from levels import *
 
-characters = ['bödvar', 'cassidy', 'orion', 'lord vraxx', 'gnash', 'queen nai', 'hattori', 'sir roland', 'scarlet', 'thatch', 'ada', 'sentinel', 'lucien', 
-              'teros', 'brynn', 'asuri', 'barraza', 'ember', 'azoth', 'koji', 'ulgrim', 'diana', 'jhala', 'kor', 'wu shang', 'val', 
-              'ragnir', 'cross', 'mirage', 'nix', 'mordex', 'yumiko', 'artemis', 'caspian', 'sidra', 'xull', 'kaya', 'isaiah', 'jiro', 
-              'lin fei', 'zariel', 'rayman', 'dusk', 'fait', 'thor', 'petra', 'vector', 'volkov', 'onyx', 'jaeyun', 'mako', 'magyar', 'reno', 'munin', 'arcadia', 'ezio', 'tezca',
-              'thea', 'red raptor', 'loki', 'seven']
+characters = [
+    "bödvar",
+    "cassidy",
+    "orion",
+    "lord vraxx",
+    "gnash",
+    "queen nai",
+    "hattori",
+    "sir roland",
+    "scarlet",
+    "thatch",
+    "ada",
+    "sentinel",
+    "lucien",
+    "teros",
+    "brynn",
+    "asuri",
+    "barraza",
+    "ember",
+    "azoth",
+    "koji",
+    "ulgrim",
+    "diana",
+    "jhala",
+    "kor",
+    "wu shang",
+    "val",
+    "ragnir",
+    "cross",
+    "mirage",
+    "nix",
+    "mordex",
+    "yumiko",
+    "artemis",
+    "caspian",
+    "sidra",
+    "xull",
+    "kaya",
+    "isaiah",
+    "jiro",
+    "lin fei",
+    "zariel",
+    "rayman",
+    "dusk",
+    "fait",
+    "thor",
+    "petra",
+    "vector",
+    "volkov",
+    "onyx",
+    "jaeyun",
+    "mako",
+    "magyar",
+    "reno",
+    "munin",
+    "arcadia",
+    "ezio",
+    "tezca",
+    "thea",
+    "red raptor",
+    "loki",
+    "seven",
+    "vivi",
+]
 
 level_character_matrix_width = 15
-level_character_matrix = list([characters[i:i + level_character_matrix_width] for i in range(0, len(characters), level_character_matrix_width)])
+level_character_matrix = list(
+    [
+        characters[i : i + level_character_matrix_width]
+        for i in range(0, len(characters), level_character_matrix_width)
+    ]
+)
 
 character_matrix_width = 13
 character_matrix = []
 
 
 def build_character_matrix(_characters):
     global character_matrix
-    character_matrix = list([_characters[i:i + character_matrix_width] for i in range(0, len(_characters), character_matrix_width)])
+    character_matrix = list(
+        [
+            _characters[i : i + character_matrix_width]
+            for i in range(0, len(_characters), character_matrix_width)
+        ]
+    )
 
 
-build_character_matrix(characters + ['random'])
+build_character_matrix(characters + ["random"])
 
 
 def find_char(name):
     for i, row in enumerate(character_matrix):
         try:
             return i + 1, row.index(name) + 1
         except ValueError:
             pass
 
 
 def map_to_char(row, col):
-    return ['down'] * (row - 1) + ['right'] * (col - 1)
+    return ["down"] * (row - 1) + ["right"] * (col - 1)
 
 
 def parse_pos(inp):
     try:
         pos = tuple(map(int, inp.split()))
     except ValueError:
         pos = find_char(inp.lower())
@@ -57,15 +126,17 @@
             self.xp -= levels_xp[self.level]
             self.level += 1
             if self.level in gold_levels:
                 gold += 120
         return gold
 
     def get_xp_to_level(self, level):
-        return max(sum((levels_xp[level]) for level in range(self.level, level)) - self.xp, 1)
+        return max(
+            sum((levels_xp[level]) for level in range(self.level, level)) - self.xp, 1
+        )
 
     @property
     def xp_to_next_level(self):
         return self.get_xp_to_level(self.level + 1)
 
     @property
     def total_xp(self):
@@ -82,16 +153,26 @@
     def xp_to_next_gold(self):
         return self.get_xp_to_level(self.next_gold_level)
 
     def get_path_to(self, name):
         orow, opos = find_char(self.name)
         trow, tpos = find_char(name)
         if orow == 4:
-            return (trow - orow) * ['down'] + (orow - trow) * ['up'] + (tpos - opos) * ['right'] + (opos - tpos) * ['left']
-        return (tpos - opos) * ['right'] + (opos - tpos) * ['left'] + (trow - orow) * ['down'] + (orow - trow) * ['up']
+            return (
+                (trow - orow) * ["down"]
+                + (orow - trow) * ["up"]
+                + (tpos - opos) * ["right"]
+                + (opos - tpos) * ["left"]
+            )
+        return (
+            (tpos - opos) * ["right"]
+            + (opos - tpos) * ["left"]
+            + (trow - orow) * ["down"]
+            + (orow - trow) * ["up"]
+        )
 
     @staticmethod
     def get_duration_for_xp(xp, maximum=15):
         return ceil(min((xp + 1) / 41, maximum))
 
     def get_duration_to_next_level(self, maximum=15):
         return self.get_duration_for_xp(self.xp_to_next_level, maximum)
@@ -104,11 +185,11 @@
         return self.get_duration_for_xp(self.xp_to_next_gold, maximum)
 
     @property
     def duration_to_next_gold(self):
         return self.get_duration_to_next_gold()
 
     def __str__(self):
-        return f'<{self.name.capitalize()} (lvl: {self.level}, xp: {self.xp}, unlocked: {self.unlocked})>'
+        return f"<{self.name.capitalize()} (lvl: {self.level}, xp: {self.xp}, unlocked: {self.unlocked})>"
 
     def __repr__(self):
         return str(self)
```

### Comparing `BHBot-master-1.1/config.py` & `bhbot_master-2.1/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,57 +3,67 @@
 from abstract_mode import Mode
 from characters import *
 from direct_input import *
 from utils import *
 
 
 def display_changelog():
-    changelog_path = Path(os.getenv('LOCALAPPDATA')) / 'BHBot' / 'changelog'
-    if global_settings.compiled and (not changelog_path.exists() or changelog_path.read_text('utf-8') != global_settings.APP_VERSION):
-        Sg.popup(*global_settings.APP_CHANGELOG, font=(global_settings.font, 13), title=global_settings.language.LAYOUT_MAPPING.get('changelog_popup_title', 'Changelog'), icon=global_settings.icon)
+    changelog_path = Path(os.getenv("LOCALAPPDATA")) / "BHBot" / "changelog"
+    if global_settings.compiled and (
+        not changelog_path.exists()
+        or changelog_path.read_text("utf-8") != global_settings.APP_VERSION
+    ):
+        Sg.popup(
+            *global_settings.APP_CHANGELOG,
+            font=(global_settings.font, 13),
+            title=global_settings.language.LAYOUT_MAPPING.get(
+                "changelog_popup_title", "Changelog"
+            ),
+            icon=global_settings.icon,
+        )
         changelog_path.parent.mkdir(parents=True, exist_ok=True)
-        changelog_path.write_text(global_settings.APP_VERSION, 'utf-8')
+        changelog_path.write_text(global_settings.APP_VERSION, "utf-8")
 
 
 class Config:
     def __init__(self, config):
-        self.character = config.get('character', 'Random')
-        self.duration = config.get('duration', 8)
-        self.auto_stop = config.get('auto_stop', True)
-        self.auto_detect_auto_stop = config.get('auto_detect_auto_stop', False)
-        self.auto_stop_frequency = config.get('auto_stop_frequency', 5)
-        self.auto_stop_duration = config.get('auto_stop_duration', 30)
+        self.character = config.get("character", "Random")
+        self.duration = config.get("duration", 8)
+        self.auto_stop = config.get("auto_stop", True)
+        self.auto_detect_auto_stop = config.get("auto_detect_auto_stop", False)
+        self.auto_stop_frequency = config.get("auto_stop_frequency", 5)
+        self.auto_stop_duration = config.get("auto_stop_duration", 30)
         # self.bots = config.get('bots', 2)
         self.bots = 2
-        self.mute = config.get('mute', False)
-        self.stealth = config.get('stealth', False)
+        self.mute = config.get("mute", False)
+        self.stealth = config.get("stealth", False)
         self.modes = self.get_modes()
         if not self.modes:
-            logger.error('no_modes')
+            logger.error("no_modes")
         else:
-            self.mode_name = config.get('mode_name', self.modes[0].get_name())
+            self.mode_name = config.get("mode_name", self.modes[0].get_name())
         self.version = global_settings.APP_VERSION
 
     @classmethod
     def load(cls):
         try:
-            res = json.load(global_settings.config_location.open('r'))
-            if res.get('version') != global_settings.APP_VERSION:
-                logger.warning('old_config')
+            res = json.load(global_settings.config_location.open("r"))
+            if res.get("version") != global_settings.APP_VERSION:
+                logger.warning("old_config")
             return cls(res)
         except FileNotFoundError:
             return cls({})
 
     # noinspection PyUnresolvedReferences
     @staticmethod
     def get_modes():
-        for mode in global_settings.modes_folder.glob('**/*.py'):
+        for mode in global_settings.modes_folder.glob("**/*.py"):
             if mode in global_settings.loaded_modes:
                 continue
-            spec = importlib.util.spec_from_file_location('module.name', mode)
+            spec = importlib.util.spec_from_file_location("module.name", mode)
             module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(module)
             global_settings.loaded_modes[mode] = module
         return Mode.__subclasses__()
 
     def get_mode(self, name):
         try:
@@ -63,87 +73,93 @@
 
     @property
     def mode(self):
         return self.get_mode(self.mode_name)
 
     @property
     def not_save(self):
-        return ['modes']
+        return ["modes"]
 
     def get_save_vars(self):
         return {k: v for k, v in vars(self).items() if k not in self.not_save}
 
     def save(self):
         try:
             global_settings.config_location.parent.mkdir(parents=True, exist_ok=True)
-            json.dump(self.get_save_vars(), global_settings.config_location.open('w+'))
+            json.dump(self.get_save_vars(), global_settings.config_location.open("w+"))
         except Exception as e:
-            logger.error('cant_save_config', e)
+            logger.error("cant_save_config", e)
 
     def __str__(self):
-        return global_settings.messages.get('config', 'Missing "config" entry in language').format(self)
+        return global_settings.messages.get(
+            "config", 'Missing "config" entry in language'
+        ).format(self)
 
 
 # noinspection PyUnresolvedReferences
 class GUIConfig:
     def __init__(self):
         self.config = Config.load()
         self.window = self.create_window()
 
     @property
     def characters(self):
         res = [character.capitalize() for character in sorted(characters)]
-        if hasattr(self, 'window') and not self.get_mode().parse_character_levels:
-            res.insert(0, 'Random')
+        if hasattr(self, "window") and not self.get_mode().parse_character_levels:
+            res.insert(0, "Random")
         return res
 
     @property
     def mode_names(self):
         return [mode.get_name() for mode in self.config.modes]
 
     @property
     def language_names(self):
         return [language.LANGUAGE for language in global_settings.languages]
 
     def get_mode(self):
-        return self.config.get_mode(self.window['mode_name'].get())
+        return self.config.get_mode(self.window["mode_name"].get())
 
     def update_layout(self):
-        if self.window['mode_name'].Values != self.mode_names:
-            self.window['mode_name'].Update(self.mode_names[0], values=self.mode_names)
-        if self.window['character'].Values != self.characters:
-            char = self.window['character'].get() if self.window['character'].get() in self.characters else self.characters[0]
-            self.window['character'].Update(char, values=self.characters)
+        if self.window["mode_name"].Values != self.mode_names:
+            self.window["mode_name"].Update(self.mode_names[0], values=self.mode_names)
+        if self.window["character"].Values != self.characters:
+            char = (
+                self.window["character"].get()
+                if self.window["character"].get() in self.characters
+                else self.characters[0]
+            )
+            self.window["character"].Update(char, values=self.characters)
         mode = self.get_mode()
         if mode.character_selection_enabled:
-            self.window['character'].update(disabled=False, readonly=True)
+            self.window["character"].update(disabled=False, readonly=True)
         else:
-            self.window['character'].update(disabled=True, readonly=True)
+            self.window["character"].update(disabled=True, readonly=True)
         if not mode.parse_character_levels:
-            self.window['auto_detect_auto_stop'].update(False, disabled=True)
+            self.window["auto_detect_auto_stop"].update(False, disabled=True)
         if mode.duration_selection_enabled:
-            self.window['duration'].update(disabled=False)
+            self.window["duration"].update(disabled=False)
         else:
-            self.window['duration'].update(disabled=True)
-        if self.window['auto_stop'].get():
-            self.window['auto_stop_duration'].update(disabled=False)
+            self.window["duration"].update(disabled=True)
+        if self.window["auto_stop"].get():
+            self.window["auto_stop_duration"].update(disabled=False)
             if mode.parse_character_levels:
-                self.window['auto_detect_auto_stop'].update(disabled=False)
-            if self.window['auto_detect_auto_stop'].get():
-                self.window['auto_stop_frequency'].update(disabled=True)
+                self.window["auto_detect_auto_stop"].update(disabled=False)
+            if self.window["auto_detect_auto_stop"].get():
+                self.window["auto_stop_frequency"].update(disabled=True)
             else:
-                self.window['auto_stop_frequency'].update(disabled=False)
+                self.window["auto_stop_frequency"].update(disabled=False)
         else:
-            self.window['auto_detect_auto_stop'].update(disabled=True)
-            self.window['auto_stop_frequency'].update(disabled=True)
-            self.window['auto_stop_duration'].update(disabled=True)
-        if self.window['stealth'].get():
-            self.window['mute'].update(True, disabled=True)
+            self.window["auto_detect_auto_stop"].update(disabled=True)
+            self.window["auto_stop_frequency"].update(disabled=True)
+            self.window["auto_stop_duration"].update(disabled=True)
+        if self.window["stealth"].get():
+            self.window["mute"].update(False, disabled=False)
         else:
-            self.window['mute'].update(disabled=False)
+            self.window["mute"].update(disabled=False)
 
     def save(self, values):
         for key in values:
             if isinstance(values[key], float) and values[key].is_integer():
                 values[key] = int(values[key])
         for k, v in values.items():
             if hasattr(self.config, k):
@@ -152,67 +168,178 @@
                 setattr(global_settings, k, v)
         self.config.save()
         global_settings.save()
 
     @staticmethod
     def row(key, input_element):
         input_element.Key = key
-        text = Sg.Text(' ', size=(1, 1), key=f'{key}_text', font=(global_settings.font, 12))
+        text = Sg.Text(
+            " ", size=(1, 1), key=f"{key}_text", font=(global_settings.font, 12)
+        )
         if isinstance(input_element, Sg.Slider):
             text.Pad = ((5, 0), (20, 0))
-        layout = [
-            [text, input_element]
-        ]
-        return Sg.Column(layout, key=f'{key}_column', element_justification='left')
+        layout = [[text, input_element]]
+        return Sg.Column(layout, key=f"{key}_column", element_justification="left")
 
     def create_window(self):
         layout = [
-            [Sg.Text(' ', size=(1, 1), key='settings_title', font=(global_settings.font, 20))],
-            [Sg.Text(' ', size=(1, 1), key='settings_help', font=(global_settings.font, 16))],
-            [self.row('language_name', Sg.Combo(self.language_names, enable_events=True, readonly=True, default_value=global_settings.language_name, font=(global_settings.font, 12)))],
-            [self.row('font', Sg.Combo(global_settings.fonts, enable_events=True, readonly=True, default_value=global_settings.font, font=(global_settings.font, 12)))],
-            [self.row('autostart', Sg.Checkbox('', default=global_settings.autostart))],
-            [self.row('branch', Sg.Combo(['stable', 'beta'], readonly=True, default_value=global_settings.branch, font=(global_settings.font, 12)))],
-            [self.row('debug', Sg.Checkbox('', default=global_settings.debug))],
-            [self.row('mode_name', Sg.Combo(self.mode_names, readonly=True, default_value=self.config.mode_name, font=(global_settings.font, 12)))],
-            [self.row('character', Sg.Combo(self.characters, readonly=True, default_value=self.config.character, font=(global_settings.font, 12)))],
-            [self.row('duration', Sg.Slider(range=(1, 15), orientation='horizontal', default_value=self.config.duration, font=(global_settings.font, 12)))],
-            [self.row('auto_stop', Sg.Checkbox('', default=self.config.auto_stop))],
-            [self.row('auto_detect_auto_stop', Sg.Checkbox('', default=self.config.auto_detect_auto_stop))],
-            [self.row('auto_stop_frequency',
-                      Sg.Slider(range=(1, 20), resolution=.5, orientation='horizontal', default_value=self.config.auto_stop_frequency, font=(global_settings.font, 12)))],
-            [self.row('auto_stop_duration',
-                      Sg.Slider(range=(5, 240), resolution=5, orientation='horizontal', default_value=self.config.auto_stop_duration, font=(global_settings.font, 12)))],
+            [
+                Sg.Text(
+                    " ",
+                    size=(1, 1),
+                    key="settings_title",
+                    font=(global_settings.font, 20),
+                )
+            ],
+            [
+                Sg.Text(
+                    " ",
+                    size=(1, 1),
+                    key="settings_help",
+                    font=(global_settings.font, 16),
+                )
+            ],
+            [
+                self.row(
+                    "language_name",
+                    Sg.Combo(
+                        self.language_names,
+                        enable_events=True,
+                        readonly=True,
+                        default_value=global_settings.language_name,
+                        font=(global_settings.font, 12),
+                    ),
+                )
+            ],
+            [
+                self.row(
+                    "font",
+                    Sg.Combo(
+                        global_settings.fonts,
+                        enable_events=True,
+                        readonly=True,
+                        default_value=global_settings.font,
+                        font=(global_settings.font, 12),
+                    ),
+                )
+            ],
+            [self.row("autostart", Sg.Checkbox("", default=global_settings.autostart))],
+            [
+                self.row(
+                    "branch",
+                    Sg.Combo(
+                        ["stable", "beta"],
+                        readonly=True,
+                        default_value=global_settings.branch,
+                        font=(global_settings.font, 12),
+                    ),
+                )
+            ],
+            [self.row("debug", Sg.Checkbox("", default=global_settings.debug))],
+            [
+                self.row(
+                    "mode_name",
+                    Sg.Combo(
+                        self.mode_names,
+                        readonly=True,
+                        default_value=self.config.mode_name,
+                        font=(global_settings.font, 12),
+                    ),
+                )
+            ],
+            [
+                self.row(
+                    "character",
+                    Sg.Combo(
+                        self.characters,
+                        readonly=True,
+                        default_value=self.config.character,
+                        font=(global_settings.font, 12),
+                    ),
+                )
+            ],
+            [
+                self.row(
+                    "duration",
+                    Sg.Slider(
+                        range=(1, 15),
+                        orientation="horizontal",
+                        default_value=self.config.duration,
+                        font=(global_settings.font, 12),
+                    ),
+                )
+            ],
+            [self.row("auto_stop", Sg.Checkbox("", default=self.config.auto_stop))],
+            [
+                self.row(
+                    "auto_detect_auto_stop",
+                    Sg.Checkbox("", default=self.config.auto_detect_auto_stop),
+                )
+            ],
+            [
+                self.row(
+                    "auto_stop_frequency",
+                    Sg.Slider(
+                        range=(1, 20),
+                        resolution=0.5,
+                        orientation="horizontal",
+                        default_value=self.config.auto_stop_frequency,
+                        font=(global_settings.font, 12),
+                    ),
+                )
+            ],
+            [
+                self.row(
+                    "auto_stop_duration",
+                    Sg.Slider(
+                        range=(5, 240),
+                        resolution=5,
+                        orientation="horizontal",
+                        default_value=self.config.auto_stop_duration,
+                        font=(global_settings.font, 12),
+                    ),
+                )
+            ],
             # [self.row('bots', Sg.Combo(list(range(1, 8)), readonly=True, default_value=self.config.bots, font=(global_settings.font, 12)))],
-            [self.row('stealth', Sg.Checkbox('', default=self.config.stealth))],
-            [self.row('mute', Sg.Checkbox('', default=self.config.mute))],
-            [Sg.Button('', font=(global_settings.font, 12), key='hotkey_settings')],
-            [Sg.Button('', font=(global_settings.font, 12), key='save'), Sg.Button('', font=(global_settings.font, 12), key='back')]
+            [self.row("stealth", Sg.Checkbox("", default=self.config.stealth))],
+            [self.row("mute", Sg.Checkbox("", default=self.config.mute))],
+            [Sg.Button("", font=(global_settings.font, 12), key="hotkey_settings")],
+            [
+                Sg.Button("", font=(global_settings.font, 12), key="save"),
+                Sg.Button("", font=(global_settings.font, 12), key="back"),
+            ],
         ]
-        window = Sg.Window('', layout, size=(800, 800), keep_on_top=True, icon=global_settings.icon, metadata='settings_window_title').Finalize()
+        window = Sg.Window(
+            "",
+            layout,
+            size=(800, 800),
+            keep_on_top=True,
+            icon=global_settings.icon,
+            metadata="settings_window_title",
+        ).Finalize()
         global_settings.update_window(window)
         return window
 
     def start_loop(self):
         while True:
             event, values = self.window.read(timeout=50)
-            if event in (Sg.WINDOW_CLOSED, 'back'):
+            if event in (Sg.WINDOW_CLOSED, "back"):
                 break
-            elif event == 'save':
+            elif event == "save":
                 self.save(values)
                 break
-            elif event == 'hotkey_settings':
+            elif event == "hotkey_settings":
                 hotkeys = GUIHotkeys()
                 self.window.disable()
                 self.window.hide()
                 hotkeys.start_loop()
                 self.window.enable()
                 self.window.un_hide()
-            elif event == 'language_name':
-                global_settings.language_name = values['language_name']
+            elif event == "language_name":
+                global_settings.language_name = values["language_name"]
                 global_settings.save()
-            elif event == 'font':
-                global_settings.font = values['font']
+            elif event == "font":
+                global_settings.font = values["font"]
                 global_settings.save()
             self.update_layout()
             global_settings.update_window(self.window)
         self.window.close()
```

### Comparing `BHBot-master-1.1/direct_input.py` & `bhbot_master-2.1/direct_input.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 
     def PressKey(self, hexCode):
         win32gui.SendMessage(self.brawlhalla.window, win32con.WM_KEYDOWN, hexCode)
 
     def ReleaseKey(self, hexCode):
         win32gui.SendMessage(self.brawlhalla.window, win32con.WM_KEYUP, hexCode)
 
-    def press_key(self, *key_codes, delay=.05):
+    def press_key(self, *key_codes, delay=0.05):
         for key_code in key_codes:
             self.PressKey(key_code)
         sleep(delay)
         for key_code in key_codes:
             self.ReleaseKey(key_code)
 
     def release_keys(self):
         for key in self.keys:
             self.ReleaseKey(self.keys[key])
-            sleep(.05)
+            sleep(0.05)
 
     def up(self, *args, **kwargs):
         self.press_key(self.hotkeys.up, *args, **kwargs)
 
     def down(self, *args, **kwargs):
         self.press_key(self.hotkeys.down, *args, **kwargs)
 
@@ -70,47 +70,57 @@
     def esc(self, *args, **kwargs):
         self.press_key(self.hotkeys.esc, *args, **kwargs)
 
     def enter(self, *args, **kwargs):
         self.press_key(self.hotkeys.enter, *args, **kwargs)
 
     def fight(self):
-        move_keys = [self.hotkeys.left, self.hotkeys.up, self.hotkeys.down, self.hotkeys.right]
-        fight_keys = [self.hotkeys.throw, self.hotkeys.quick, self.hotkeys.heavy, self.hotkeys.dodge]
-        self.press_key(choice(move_keys), choice(fight_keys), delay=.2)
+        move_keys = [
+            self.hotkeys.left,
+            self.hotkeys.up,
+            self.hotkeys.down,
+            self.hotkeys.right,
+        ]
+        fight_keys = [
+            self.hotkeys.throw,
+            self.hotkeys.quick,
+            self.hotkeys.heavy,
+            self.hotkeys.dodge,
+        ]
+        self.press_key(choice(move_keys), choice(fight_keys), delay=0.2)
 
 
 class Hotkeys:
     def __init__(self, hotkeys):
-        self.up = hotkeys.get('up', win32con.VK_UP)
-        self.down = hotkeys.get('down', win32con.VK_DOWN)
-        self.left = hotkeys.get('left', win32con.VK_LEFT)
-        self.right = hotkeys.get('right', win32con.VK_RIGHT)
-        self.throw = hotkeys.get('throw', 0x48)
-        self.quick = hotkeys.get('quick', 0x4A)
-        self.heavy = hotkeys.get('heavy', 0x4B)
-        self.dodge = hotkeys.get('dodge', 0x4C)
+        self.up = hotkeys.get("up", win32con.VK_UP)
+        self.down = hotkeys.get("down", win32con.VK_DOWN)
+        self.left = hotkeys.get("left", win32con.VK_LEFT)
+        self.right = hotkeys.get("right", win32con.VK_RIGHT)
+        self.throw = hotkeys.get("throw", 0x48)
+        self.quick = hotkeys.get("quick", 0x4A)
+        self.heavy = hotkeys.get("heavy", 0x4B)
+        self.dodge = hotkeys.get("dodge", 0x4C)
         self.rbr = 0xDD
         self.esc = win32con.VK_ESCAPE
         self.enter = win32con.VK_RETURN
 
     @classmethod
     def load(cls):
         try:
-            res = json.load(global_settings.hotkeys_location.open('r'))
+            res = json.load(global_settings.hotkeys_location.open("r"))
             return cls(res)
         except FileNotFoundError:
             return cls({})
 
     def save(self):
         try:
             global_settings.hotkeys_location.parent.mkdir(parents=True, exist_ok=True)
-            json.dump(vars(self), global_settings.hotkeys_location.open('w+'))
+            json.dump(vars(self), global_settings.hotkeys_location.open("w+"))
         except Exception as e:
-            logger.error('cant_save_hotkeys', e)
+            logger.error("cant_save_hotkeys", e)
 
 
 class GUIHotkeys:
     def __init__(self):
         self.hotkeys = Hotkeys.load()
         self.window = self.create_window()
         self.hook = None
@@ -128,49 +138,87 @@
         if self.hook:
             keyboard.unhook(self.hook)
             self.hook = None
 
     @staticmethod
     def text_column(*keys):
         return Sg.Column(
-            [[Sg.Text(' ', size=(1, 1), key=f'{key}_text', font=(global_settings.font, 12))] for key in keys]
+            [
+                [
+                    Sg.Text(
+                        " ",
+                        size=(1, 1),
+                        key=f"{key}_text",
+                        font=(global_settings.font, 12),
+                    )
+                ]
+                for key in keys
+            ]
         )
 
     def input_column(self, *keys):
         return Sg.Column(
-            [[Sg.Input(size=(3, 1), key=key, enable_events=True, font=(global_settings.font, '12'), default_text=self.vk_to_char(vars(self.hotkeys)[key]))] for key in keys]
+            [
+                [
+                    Sg.Input(
+                        size=(3, 1),
+                        key=key,
+                        enable_events=True,
+                        font=(global_settings.font, "12"),
+                        default_text=self.vk_to_char(vars(self.hotkeys)[key]),
+                    )
+                ]
+                for key in keys
+            ]
         )
 
     def combined_column(self, *keys):
         return [self.text_column(*keys), self.input_column(*keys)]
 
     def create_window(self):
         layout = [
-            [Sg.Text(' ', size=(1, 1), key='hotkeys_title', font=(global_settings.font, 20))],
             [
-                *self.combined_column('up', 'left', 'throw', 'quick'),
-                *self.combined_column('down', 'right', 'dodge', 'heavy')
+                Sg.Text(
+                    " ",
+                    size=(1, 1),
+                    key="hotkeys_title",
+                    font=(global_settings.font, 20),
+                )
+            ],
+            [
+                *self.combined_column("up", "left", "throw", "quick"),
+                *self.combined_column("down", "right", "dodge", "heavy"),
+            ],
+            [
+                Sg.Button("", key="save", font=(global_settings.font, 12)),
+                Sg.Button("", key="back", font=(global_settings.font, 12)),
             ],
-            [Sg.Button('', key='save', font=(global_settings.font, 12)), Sg.Button('', key='back', font=(global_settings.font, 12))],
         ]
-        window = Sg.Window('', layout, size=(600, 350), keep_on_top=True, icon=global_settings.icon, metadata='hotkeys_window_title').Finalize()
+        window = Sg.Window(
+            "",
+            layout,
+            size=(600, 350),
+            keep_on_top=True,
+            icon=global_settings.icon,
+            metadata="hotkeys_window_title",
+        ).Finalize()
         global_settings.update_window(window)
         return window
 
     @staticmethod
     def vsc_to_vk(code):
         return win32api.MapVirtualKey(code, MAP_VSC_TO_VK)
 
     @staticmethod
     def vk_to_char(code):
         direct = {
-            win32con.VK_LEFT: '◁',
-            win32con.VK_UP: '△',
-            win32con.VK_RIGHT: '▷',
-            win32con.VK_DOWN: '▽',
+            win32con.VK_LEFT: "◁",
+            win32con.VK_UP: "△",
+            win32con.VK_RIGHT: "▷",
+            win32con.VK_DOWN: "▽",
         }
         if code in direct:
             return direct[code]
         return chr(win32api.MapVirtualKey(code, MAP_VK_TO_CHAR))
 
     def save(self):
         for key in self.converter:
@@ -178,19 +226,28 @@
         self.hotkeys.save()
 
     def start_loop(self):
         self.hook_keyboard()
         while True:
             event, values = self.window.read(timeout=50)
             if self.last_keyboard_event:
-                if event in ['up', 'down', 'left', 'right', 'quick', 'heavy', 'dodge', 'throw']:
+                if event in [
+                    "up",
+                    "down",
+                    "left",
+                    "right",
+                    "quick",
+                    "heavy",
+                    "dodge",
+                    "throw",
+                ]:
                     vk = self.vsc_to_vk(self.last_keyboard_event.scan_code)
                     self.window[event].Update(self.vk_to_char(vk))
                     self.converter[event] = vk
-            if event in (Sg.WINDOW_CLOSED, 'back'):
+            if event in (Sg.WINDOW_CLOSED, "back"):
                 break
-            elif event == 'save':
+            elif event == "save":
                 self.save()
                 break
             global_settings.update_window(self.window)
         self.unhook_keyboard()
         self.window.close()
```

### Comparing `BHBot-master-1.1/menu.py` & `bhbot_master-2.1/menu.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,60 +10,69 @@
     VERTICAL = auto()
 
 
 class MenuItem:
     def __init__(self, name: str):
         self.name = name
         self.position: Optional[int] = None  # assigned by parent
-        self.parent: Optional['Layout'] = None  # assigned by parent
+        self.parent: Optional["Layout"] = None  # assigned by parent
 
     def move_to_parent(self, vi: VirtualInput) -> list[Callable]:
         return []
 
-    def _move_to(self, target: 'MenuItem', vi: VirtualInput) -> list[Callable]:
+    def _move_to(self, target: "MenuItem", vi: VirtualInput) -> list[Callable]:
         if self.parent is None:
-            raise Exception('Trying to move from orphan')
+            raise Exception("Trying to move from orphan")
         if isinstance(target, ThirdColumn):
             # noinspection PyUnresolvedReferences
-            if find_element('first_column').current_position > 6:
+            if find_element("first_column").current_position > 6:
                 target.current_position = 2
             else:
                 target.current_position = 1
         if target == self.parent:
             return self.move_to_parent(vi)
         if target in self.parent.contents:
             if self.parent.direction == Direction.HORIZONTAL:
-                return (target.position - self.position) * [vi.right] + (self.position - target.position) * [vi.left]
-            return (target.position - self.position) * [vi.down] + (self.position - target.position) * [vi.up]
-        raise Exception('Trying to move to non-adjacent node')
+                return (target.position - self.position) * [vi.right] + (
+                    self.position - target.position
+                ) * [vi.left]
+            return (target.position - self.position) * [vi.down] + (
+                self.position - target.position
+            ) * [vi.up]
+        raise Exception("Trying to move to non-adjacent node")
 
-    def move_to(self, target: 'MenuItem', vi: VirtualInput) -> list[Callable]:
+    def move_to(self, target: "MenuItem", vi: VirtualInput) -> list[Callable]:
         path = path_between(self, target)
         steps = []
         for i in range(len(path) - 1):
             steps += path[i]._move_to(path[i + 1], vi)
         return steps
 
 
 class Layout(MenuItem):
-    def __init__(self, name: str, contents: list[MenuItem], base_position: int,
-                 direction: Direction):
+    def __init__(
+        self,
+        name: str,
+        contents: list[MenuItem],
+        base_position: int,
+        direction: Direction,
+    ):
         super().__init__(name)
         for pos, item in enumerate(contents):
             item.parent = self
             item.position = pos
         self.contents = contents
         self.current_position = base_position
         self.direction = direction
 
     @property
     def current_element(self):
         return self.contents[self.current_position]
 
-    def _move_to(self, target: 'MenuItem', vi: VirtualInput) -> list[Callable]:
+    def _move_to(self, target: "MenuItem", vi: VirtualInput) -> list[Callable]:
         if target in self.contents:
             steps = self.current_element._move_to(target, vi)
             self.current_position = target.position
             return steps
         return super()._move_to(target, vi)
 
 
@@ -122,70 +131,73 @@
         target = target.parent
 
     return steps + list(reversed(reverse_steps))
 
 
 def generate_layout():
     options_items = [
-        MenuItem(name) for name in [
-            'system_settings',
-            'controls',
-            'change_region',
-            'report_bug',
-            'image_render_tool',
-            'legal',
-            'exit_game',
+        MenuItem(name)
+        for name in [
+            "system_settings",
+            "controls",
+            "change_region",
+            "report_bug",
+            "image_render_tool",
+            "legal",
+            "exit_game",
         ]
     ]
-    options = Layout('options', options_items, 0, Direction.VERTICAL)
+    options = Layout("options", options_items, 0, Direction.VERTICAL)
 
     mini_menu_items = [
-        MenuItem(name) for name in [
-            'inventory',
-            'store',
-            'battle_pass',
-            'notifications',
-            'friends',
-            'clans',
-            'replays',
+        MenuItem(name)
+        for name in [
+            "inventory",
+            "store",
+            "battle_pass",
+            "notifications",
+            "friends",
+            "clans",
+            "replays",
         ]
     ]
     mini_menu_items.append(options)
-    mini_menu = MiniMenu('mini_menu', mini_menu_items, 0, Direction.HORIZONTAL)
+    mini_menu = MiniMenu("mini_menu", mini_menu_items, 0, Direction.HORIZONTAL)
 
     third_column_items = [
         mini_menu,
-        MenuItem('smol_ad'),
-        MenuItem('smoller_ad'),
+        MenuItem("smol_ad"),
+        MenuItem("smoller_ad"),
     ]
 
     second_column_items = [
-        MenuItem('big_ad'),
+        MenuItem("big_ad"),
     ]
 
     first_column_items = [
-        MenuItem(name) for name in [
-            'play',
-            'ranked',
-            'battle_pass',
-            'custom_game_room',
-            'brawl',
-            'offline',
-            'meet_the_legends',
-            'store',
+        MenuItem(name)
+        for name in [
+            "play",
+            "ranked",
+            "battle_pass",
+            "custom_game_room",
+            "brawl",
+            "offline",
+            "meet_the_legends",
+            "store",
         ]
     ]
-    first_column = Layout('first_column', first_column_items, 0, Direction.VERTICAL)
+    first_column = Layout("first_column", first_column_items, 0, Direction.VERTICAL)
 
     main_layout_items = [
         first_column,
-        Layout('second_column', second_column_items, 0, Direction.VERTICAL),
-        ThirdColumn('third_column', third_column_items, 1, Direction.VERTICAL),
+        Layout("second_column", second_column_items, 0, Direction.VERTICAL),
+        ThirdColumn("third_column", third_column_items, 1, Direction.VERTICAL),
     ]
-    main = Layout('main', main_layout_items, 0, Direction.HORIZONTAL)
+    main = Layout("main", main_layout_items, 0, Direction.HORIZONTAL)
     return main
 
 
 main_layout = generate_layout()
 
 
 def regenerate_layout():
```

### Comparing `BHBot-master-1.1/utils.py` & `bhbot_master-2.1/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from copy import copy
 from datetime import datetime, timedelta
 from math import floor, ceil
 from pathlib import Path
 
 import PySimpleGUI as Sg
 import requests
+
 # noinspection PyProtectedMember
 from pyupdater import rfh, log
 from pyupdater.client import Client
 
 from client_config import ClientConfig
 from font_loader import get_font_name, load_font
 
@@ -22,29 +23,31 @@
 
 
 def get_text(element):
     if isinstance(element, Sg.Text):
         return element.get()
     elif isinstance(element, Sg.Button):
         return element.get_text()
-    return f'Unsupported element type {type(element)}'
+    return f"Unsupported element type {type(element)}"
 
 
 def set_text(element, value):
     if isinstance(element, Sg.Text):
         element.set_size((len(value), 1))
         element.update(value)
     if isinstance(element, Sg.Button):
         element.update(value)
 
 
 def my_emit(superclass, record):
     record = copy(record)
-    if isinstance(record.msg, str) and record.msg.count('%s') < len(record.args):
-        record.msg += ' ' + ' '.join(['%s' for _ in range(len(record.args) - record.msg.count('%s'))])
+    if isinstance(record.msg, str) and record.msg.count("%s") < len(record.args):
+        record.msg += " " + " ".join(
+            ["%s" for _ in range(len(record.args) - record.msg.count("%s"))]
+        )
     superclass.emit(record)
 
 
 class MyStreamHandler(logging.StreamHandler):
     def emit(self, record):
         my_emit(super(), record)
 
@@ -55,23 +58,23 @@
 
 
 class MyFormatter(logging.Formatter):
     def format(self, record):
         # noinspection PyProtectedMember
         format_orig = self._style._fmt
         if record.levelno == logging.DEBUG:
-            self._style._fmt = '%(asctime)s %(levelname)s %(message)s'
+            self._style._fmt = "%(asctime)s %(levelname)s %(message)s"
         elif record.levelno == logging.INFO:
-            self._style._fmt = '%(message)s'
+            self._style._fmt = "%(message)s"
         result = super().format(record)
         self._style._fmt = format_orig
         return result
 
 
-logger = logging.getLogger('main_bot_logger')
+logger = logging.getLogger("main_bot_logger")
 logger.setLevel(logging.DEBUG)
 hdlr = MyStreamHandler()
 hdlr.setLevel(logging.DEBUG)
 hdlr.setFormatter(MyFormatter())
 logger.addHandler(hdlr)
 
 
@@ -81,123 +84,146 @@
 
 
 sys.excepthook = excepthook
 
 
 class Settings:
     installation_folder = Path.cwd()
-    logs_folder = Path(os.getenv('LOCALAPPDATA')) / 'BHBot' / 'logs'
-    installation_info_location = Path(os.getenv('LOCALAPPDATA')) / 'BHBot' / 'installation.data'
-    settings_location = Path(os.getenv('LOCALAPPDATA')) / 'BHBot' / 'settings.cfg'
-    config_location = Path(os.getenv('LOCALAPPDATA')) / 'BHBot' / 'bhbot.cfg'
-    hotkeys_location = Path(os.getenv('LOCALAPPDATA')) / 'BHBot' / 'hotkeys.cfg'
-    stats_location = Path(os.getenv('LOCALAPPDATA')) / 'BHBot' / 'stats.json'
+    logs_folder = Path(os.getenv("LOCALAPPDATA")) / "BHBot" / "logs"
+    installation_info_location = (
+        Path(os.getenv("LOCALAPPDATA")) / "BHBot" / "installation.data"
+    )
+    settings_location = Path(os.getenv("LOCALAPPDATA")) / "BHBot" / "settings.cfg"
+    config_location = Path(os.getenv("LOCALAPPDATA")) / "BHBot" / "bhbot.cfg"
+    hotkeys_location = Path(os.getenv("LOCALAPPDATA")) / "BHBot" / "hotkeys.cfg"
+    stats_location = Path(os.getenv("LOCALAPPDATA")) / "BHBot" / "stats.json"
 
     def __init__(self, settings):
-        self.APP_NAME = 'BHBot'
-        self.APP_VERSION = '3.5.23'
+        self.APP_NAME = "BHBot"
+        self.APP_VERSION = "3.5.23"
         self.APP_CHANGELOGS = {
-            'English': [
-                f'Updated to {self.APP_VERSION} \\o/',
+            "English": [
+                f"Updated to {self.APP_VERSION} \\o/",
                 'If it\'s your first time using the bot or seeing this message, please click "Instructions" and read them carefully',
-                '- Fixed ingame detection with low connection',
+                "- Fixed ingame detection with low connection",
             ],
-            'Русский': [
-                f'Обновился до {self.APP_VERSION} \\o/',
+            "Русский": [
+                f"Обновился до {self.APP_VERSION} \\o/",
                 'Если вы используете бота или видите это сообщение впервые, пожалуйста, нажмите на "Инструкции" и тщательно их прочтите',
-                '- Починил определение нахождения в бою при низком подключении',
-            ]
+                "- Починил определение нахождения в бою при низком подключении",
+            ],
         }
 
-        self.compiled = getattr(sys, 'frozen', False)
+        self.compiled = getattr(sys, "frozen", False)
 
         self.load_installation_info()
         self.clear_old_logs()
         self.add_file_handlers()
         self.load_fonts()
 
-        pyupdater_client = Client(ClientConfig(), refresh=True, progress_hooks=[self.print_update_status])
-
-        self.branch = settings.get('branch', 'stable')
-
-        self.new_version = pyupdater_client.update_check(self.APP_NAME, self.APP_VERSION, channel=self.branch, strict=self.branch != 'beta')
+        pyupdater_client = Client(
+            ClientConfig(), refresh=True, progress_hooks=[self.print_update_status]
+        )
+
+        self.branch = settings.get("branch", "stable")
+
+        self.new_version = pyupdater_client.update_check(
+            self.APP_NAME,
+            self.APP_VERSION,
+            channel=self.branch,
+            strict=self.branch != "beta",
+        )
 
         self.languages = self.get_languages()
         if not self.languages:
-            logger.error('No languages found. Program will not function with empty languages directory.')
-        self.language_name = settings.get('language_name', 'English')
-
-        self.APP_CHANGELOG = self.APP_CHANGELOGS.get(self.language_name, self.APP_CHANGELOGS.get('English'))
+            logger.error(
+                "No languages found. Program will not function with empty languages directory."
+            )
+        self.language_name = settings.get("language_name", "English")
+
+        self.APP_CHANGELOG = self.APP_CHANGELOGS.get(
+            self.language_name, self.APP_CHANGELOGS.get("English")
+        )
 
         self.fonts = self.get_fonts()
-        self.font = settings.get('font', 'Cousine Regular')
+        self.font = settings.get("font", "Cousine Regular")
 
-        self.autostart = settings.get('autostart', False)
+        self.autostart = settings.get("autostart", False)
 
-        self.icon = self.installation_folder / 'icon.ico'
+        self.icon = self.installation_folder / "icon.ico"
 
-        self.debug = settings.get('debug', False)
+        self.debug = settings.get("debug", False)
         self.gui_handler = None
         self.loaded_modes = {}
 
     @staticmethod
     def print_update_status(info):
-        if info['status'] == 'downloading':
-            logger.info('downloading', info["percent_complete"])
-        elif info['status'] == 'finished':
-            logger.info('downloaded', info["time"])
+        if info["status"] == "downloading":
+            logger.info("downloading", info["percent_complete"])
+        elif info["status"] == "finished":
+            logger.info("downloaded", info["time"])
 
     @classmethod
     def load(cls):
         try:
-            return cls(json.load(cls.settings_location.open('r')))
+            return cls(json.load(cls.settings_location.open("r")))
         except FileNotFoundError:
             return cls({})
 
     # noinspection PyUnresolvedReferences
     def get_languages(self):
         languages = []
-        for language in self.languages_folder.glob('*.py'):
-            spec = importlib.util.spec_from_file_location('module.name', language)
+        for language in self.languages_folder.glob("*.py"):
+            spec = importlib.util.spec_from_file_location("module.name", language)
             language_module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(language_module)
             languages.append(language_module)
         return languages
 
     def get_fonts(self):
-        fonts = ['Courier']
-        for font in self.fonts_folder.glob('**/*.ttf'):
-            fonts.append(get_font_name(font.open('rb')))
+        fonts = ["Courier"]
+        for font in self.fonts_folder.glob("**/*.ttf"):
+            fonts.append(get_font_name(font.open("rb")))
         return fonts
 
     def get_language(self, name):
         return next(filter(lambda x: x.LANGUAGE == name, self.languages))
 
     @property
     def language(self):
         return self.get_language(self.language_name)
 
     @property
     def not_save(self):
-        return ['fonts', 'languages', 'gui_handler', 'loaded_modes', 'new_version', 'compiled', 'APP_CHANGELOG', 'APP_CHANGELOGS', 'icon']
+        return [
+            "fonts",
+            "languages",
+            "gui_handler",
+            "loaded_modes",
+            "new_version",
+            "compiled",
+            "APP_CHANGELOG",
+            "APP_CHANGELOGS",
+            "icon",
+        ]
 
     def set_debug_state(self):
         if self.gui_handler:
             self.gui_handler.setLevel(logging.DEBUG if self.debug else logging.INFO)
 
     def get_save_vars(self):
         return {k: v for k, v in vars(self).items() if k not in self.not_save}
 
     def save(self):
         self.set_debug_state()
         try:
             self.settings_location.parent.mkdir(parents=True, exist_ok=True)
-            json.dump(self.get_save_vars(), self.settings_location.open('w+'))
+            json.dump(self.get_save_vars(), self.settings_location.open("w+"))
         except Exception as e:
-            logger.error(f'Could not save settings. Exception: {e}')
+            logger.error(f"Could not save settings. Exception: {e}")
 
     # noinspection PyUnresolvedReferences
     @property
     def messages(self):
         return self.language.MESSAGES
 
     # noinspection PyUnresolvedReferences
@@ -205,159 +231,188 @@
         for key in window.AllKeysDict:
             font = window[key].Font
             if font and font[0] != global_settings.font:
                 window[key].Font = (global_settings.font, font[1])
                 window[key].Widget.config(font=window[key].Font)
             if key in self.language.LAYOUT_MAPPING:
                 value = self.language.LAYOUT_MAPPING.get(key)
-                res_text = value[window[key].metadata].format(self) if window[key].metadata is not None else value.format(self)
+                res_text = (
+                    value[window[key].metadata].format(self)
+                    if window[key].metadata is not None
+                    else value.format(self)
+                )
                 if res_text != get_text(window[key]):
                     set_text(window[key], res_text)
             tooltip_text = None
-            if hasattr(self.language, 'TOOLTIPS') and key in self.language.TOOLTIPS:  # First condition is for backwards-compatibility
+            if (
+                hasattr(self.language, "TOOLTIPS") and key in self.language.TOOLTIPS
+            ):  # First condition is for backwards-compatibility
                 tooltip_value = self.language.TOOLTIPS.get(key)
-                tooltip_text = tooltip_value[window[key].metadata].format(self) if window[key].metadata is not None else tooltip_value.format(self)
+                tooltip_text = (
+                    tooltip_value[window[key].metadata].format(self)
+                    if window[key].metadata is not None
+                    else tooltip_value.format(self)
+                )
             if tooltip_text != window[key].Tooltip:
                 window[key].Tooltip = tooltip_text
                 window[key].set_tooltip(tooltip_text)
 
         if window.Title != self.language.LAYOUT_MAPPING.get(window.metadata):
             window.Title = self.language.LAYOUT_MAPPING.get(window.metadata)
             window.set_title(window.Title)
 
     def load_installation_info(self):
-        logger.debug('Loading installation info')
+        logger.debug("Loading installation info")
         if not self.compiled:
             return
-        if all(Path(folder).exists() for folder in ['fonts', 'languages', 'modes']):
-            logger.debug('Writing installation info')
+        if all(Path(folder).exists() for folder in ["fonts", "languages", "modes"]):
+            logger.debug("Writing installation info")
             return self.write_installation_info()
         if not self.installation_info_location.exists():
-            logger.error('Corrupted installation. Exiting.')
+            logger.error("Corrupted installation. Exiting.")
             sys.exit()
-        installation_info = json.load(self.installation_info_location.open('r'))
+        installation_info = json.load(self.installation_info_location.open("r"))
         for path in installation_info:
             setattr(type(self), path, Path(installation_info[path]))
 
     def write_installation_info(self):
-        logger.debug('Writing installation info')
+        logger.debug("Writing installation info")
         self.installation_info_location.parent.mkdir(parents=True, exist_ok=True)
         obj = {
-            'installation_folder': Path.cwd(),
-            'logs_folder': self.logs_folder,
-            'settings_location': self.settings_location,
-            'config_location': self.config_location,
-            'hotkeys_location': self.hotkeys_location,
-            'stats_location': self.stats_location,
+            "installation_folder": Path.cwd(),
+            "logs_folder": self.logs_folder,
+            "settings_location": self.settings_location,
+            "config_location": self.config_location,
+            "hotkeys_location": self.hotkeys_location,
+            "stats_location": self.stats_location,
         }
         obj = {k: str(v) for k, v in obj.items()}
-        json.dump(obj, self.installation_info_location.open('w+'))
+        json.dump(obj, self.installation_info_location.open("w+"))
 
     def clear_old_logs(self):
-        for log_file in self.logs_folder.glob('????????-??????.log'):
+        for log_file in self.logs_folder.glob("????????-??????.log"):
             dt = log_file.name[:-4]
-            dt = datetime.strptime(dt, '%Y%m%d-%H%M%S')
+            dt = datetime.strptime(dt, "%Y%m%d-%H%M%S")
             if datetime.now() - dt > timedelta(days=3):
                 log_file.unlink()
 
     def add_file_handlers(self):
         self.logs_folder.mkdir(parents=True, exist_ok=True)
-        file_hdlr = MyFileHandler(self.logs_folder / f'{datetime.now().strftime("%Y%m%d-%H%M%S")}.log', encoding='utf-8')
-        file_hdlr.setFormatter(logging.Formatter('[%(asctime)s] [%(threadName)s:THREAD%(thread)d] %(levelname)-8s %(message)s'))
+        file_hdlr = MyFileHandler(
+            self.logs_folder / f'{datetime.now().strftime("%Y%m%d-%H%M%S")}.log',
+            encoding="utf-8",
+        )
+        file_hdlr.setFormatter(
+            logging.Formatter(
+                "[%(asctime)s] [%(threadName)s:THREAD%(thread)d] %(levelname)-8s %(message)s"
+            )
+        )
         file_hdlr.setLevel(logging.DEBUG)
         logger.addHandler(file_hdlr)
-        error_hdlr = MyFileHandler(self.logs_folder / 'exceptions.log', encoding='utf-8')
-        error_hdlr.setFormatter(logging.Formatter('[%(asctime)s] [%(threadName)s:THREAD%(thread)d] %(levelname)-8s %(message)s'))
+        error_hdlr = MyFileHandler(
+            self.logs_folder / "exceptions.log", encoding="utf-8"
+        )
+        error_hdlr.setFormatter(
+            logging.Formatter(
+                "[%(asctime)s] [%(threadName)s:THREAD%(thread)d] %(levelname)-8s %(message)s"
+            )
+        )
         error_hdlr.setLevel(logging.WARNING)
         logger.addHandler(error_hdlr)
 
     @property
     def fonts_folder(self):
-        return self.installation_folder / 'fonts'
+        return self.installation_folder / "fonts"
 
     @property
     def languages_folder(self):
-        return self.installation_folder / 'languages'
+        return self.installation_folder / "languages"
 
     @property
     def modes_folder(self):
-        return self.installation_folder / 'modes'
+        return self.installation_folder / "modes"
 
     def load_fonts(self):
-        for font in self.fonts_folder.glob('**/*.ttf'):
+        for font in self.fonts_folder.glob("**/*.ttf"):
             load_font(str(font))
 
     def update_stats(self, **kwargs):
         current = self.get_stats()
         for key in kwargs:
             current[key] = current.get(key, 0) + kwargs[key]
-        json.dump(current, self.stats_location.open('w+'))
+        json.dump(current, self.stats_location.open("w+"))
 
     def get_stats(self):
         if not self.stats_location.exists():
             return {}
-        return json.load(self.stats_location.open('r'))
+        return json.load(self.stats_location.open("r"))
 
     def __str__(self):
-        return self.messages.get('settings', 'Missing "settings" entry in language').format(self)
+        return self.messages.get(
+            "settings", 'Missing "settings" entry in language'
+        ).format(self)
 
 
 global_settings = Settings.load()
 
 
 def box(text, startmargin=True, endmargin=True):
-    lines = text.split('\n')
+    lines = text.split("\n")
     longest_line = sorted(lines, key=lambda x: len(x), reverse=True)[0]
     length = len(longest_line) + 6
     if startmargin:
-        logger.info('\n\n')
-    logger.info('#' * length)
+        logger.info("\n\n")
+    logger.info("#" * length)
     for line in lines:
         spaces = (length - len(line) - 2) / 2
-        logger.info('#' + ' ' * ceil(spaces) + line + ' ' * floor(spaces) + '#')
-    logger.info('#' * length)
+        logger.info("#" + " " * ceil(spaces) + line + " " * floor(spaces) + "#")
+    logger.info("#" * length)
     if endmargin:
-        logger.info('\n\n')
+        logger.info("\n\n")
 
 
 def format_time(seconds):
     seconds = int(seconds)
     m, s = divmod(seconds, 60)
     h, m = divmod(m, 60)
-    return f'{h:d}:{m:02d}:{s:02d}'
+    return f"{h:d}:{m:02d}:{s:02d}"
 
 
 def get_rotation():
     try:
-        res = requests.get('https://sovamor.co/bhbot/rotation', timeout=5).json()
-        return [character.lower() for character in res.get('rotation')]
+        res = requests.get("https://sovamor.co/bhbot/rotation", timeout=5).json()
+        return [character.lower() for character in res.get("rotation")]
     except Exception as e:
-        logger.warning('rotation_error', e)
+        logger.warning("rotation_error", e)
         return []
 
 
 def get_menu_pixels():
     try:
-        res = requests.get('https://sovamor.co/bhbot/menu_pixels', timeout=5).json()
+        res = requests.get("https://sovamor.co/bhbot/menu_pixels", timeout=5).json()
         return {
             k: {
-                inner_k: tuple(x if not isinstance(x, list) else tuple(x) for x in inner_v) for inner_k, inner_v in v.items()
-            } for k, v in res.items()
+                inner_k: tuple(
+                    x if not isinstance(x, list) else tuple(x) for x in inner_v
+                )
+                for inner_k, inner_v in v.items()
+            }
+            for k, v in res.items()
         }
     except Exception as e:
-        logger.warning('menu_pixels_error', e)
+        logger.warning("menu_pixels_error", e)
         return {}
 
 
 def chunks(input_list, n):
     """
     Yield n number of sequential chunks from input_list.
     https://stackoverflow.com/a/54802737
     """
     d, r = divmod(len(input_list), n)
     for i in range(n):
         si = (d + 1) * (i if i < r else r) + d * (0 if i < r else i - r)
-        yield input_list[si:si + (d + 1 if i < r else d)]
+        yield input_list[si : si + (d + 1 if i < r else d)]
 
 
 def compare(fst, snd):
     return sum(fst[i] != snd[i] for i in range(min(len(fst), len(snd))))
```

### Comparing `BHBot-master-1.1/windows.py` & `bhbot_master-2.1/windows.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     res = []
     win32gui.EnumWindows(window_enumeration_handler, res)
     return res[0] if res else None
 
 
 class SteamClient:
     _WIN_REG_SHELL = (winreg.HKEY_CLASSES_ROOT, r"steam\Shell\Open\Command")
-    _PROCESS_NAME = 'steam.exe'
+    _PROCESS_NAME = "steam.exe"
 
     def __init__(self):
         self.path = self.find_exe()
         self.cmd = f'"{self.path}" -applaunch 291550 -noeac'
 
     # yoinked from battlenet extension for gog galaxy
     @staticmethod
@@ -68,15 +68,15 @@
                 return proc.exe()
 
     # yoinked from battlenet extension for gog galaxy
     def _find_exe_registry(self):
         shell_reg_value = self.__search_registry_for_run_cmd(*self._WIN_REG_SHELL)
         if shell_reg_value is None:
             return None
-        reg = re.compile("\"(.*?)\"")
+        reg = re.compile('"(.*?)"')
         return reg.search(shell_reg_value).groups()[0]
 
     def find_exe(self):
         res = self._find_exe_running() or self._find_exe_registry()
         if not res:
             raise SteamExeNotFound()
         return res
@@ -88,29 +88,31 @@
 class BrawlhallaProcess:
     def __init__(self, hwnd, proc):
         self.window = hwnd
         self.process = proc
 
     @classmethod
     def find(cls):
-        res = get_window('Brawlhalla.exe') or get_window('BrawlhallaGame.exe')  # support for beta
+        res = get_window("Brawlhalla.exe") or get_window(
+            "BrawlhallaGame.exe"
+        )  # support for beta
         if not res:
             return None
         return cls(*res)
 
     @property
     def responding(self):
         cmd = f'tasklist /FI "PID eq {self.process.pid}" /FI "STATUS eq running"'
         status = subprocess.check_output(cmd, creationflags=subprocess.DETACHED_PROCESS)
         return str(self.process.pid) in str(status)
 
     def kill(self):
         while self.process.is_running():
             self.process.kill()
-            sleep(.5)
+            sleep(0.5)
 
     def get_window_rect(self):
         return win32gui.GetWindowRect(self.window)
 
     def get_window_size(self):
         left, top, right, bot = self.get_window_rect()
         return right - left, bot - top
@@ -122,41 +124,67 @@
     @property
     def fullscreen(self):
         return self.get_client_size() == self.get_window_size()
 
     def resize(self):
         window_size = self.get_window_size()
         client_size = self.get_client_size()
-        logger.debug('resize', *window_size, *client_size, *Sg.Window.get_screen_size())
+        logger.debug("resize", *window_size, *client_size, *Sg.Window.get_screen_size())
         w_border = window_size[0] - client_size[0]
         h_border = window_size[1] - client_size[1]
-        while self.get_client_size() != (1920, 1080):  # getwindowsize or getclientsize or setwindowpos or something else is weird so it sometimes doesnt work first try
-            win32gui.SetWindowPos(self.window, 0, 0, 0, 1920 + w_border, 1080 + h_border, win32con.SWP_NOZORDER)
+        while self.get_client_size() != (
+            1920,
+            1080,
+        ):  # getwindowsize or getclientsize or setwindowpos or something else is weird so it sometimes doesnt work first try
+            win32gui.SetWindowPos(
+                self.window,
+                0,
+                0,
+                0,
+                1920 + w_border,
+                1080 + h_border,
+                win32con.SWP_NOZORDER,
+            )
 
     def move_off_screen(self):
-        logger.debug('move_offscreen')
+        logger.debug("move_offscreen")
         w, h = Sg.Window.get_screen_size()
-        win32gui.SetWindowPos(self.window, 0, w * 4, h * 4, 0, 0, win32con.SWP_NOSIZE | win32con.SWP_NOZORDER)
+        win32gui.SetWindowPos(
+            self.window,
+            0,
+            w * 4,
+            h * 4,
+            0,
+            0,
+            win32con.SWP_NOSIZE | win32con.SWP_NOZORDER,
+        )
 
     def make_transparent(self):
         style = win32gui.GetWindowLong(self.window, win32con.GWL_EXSTYLE)
         win32gui.ShowWindow(self.window, win32con.SW_HIDE)
-        style |= win32con.WS_EX_COMPOSITED | win32con.WS_EX_LAYERED | win32con.WS_EX_TRANSPARENT | win32con.WS_EX_TOOLWINDOW | win32con.WS_EX_NOACTIVATE
+        style |= (
+            win32con.WS_EX_COMPOSITED
+            | win32con.WS_EX_LAYERED
+            | win32con.WS_EX_TRANSPARENT
+            | win32con.WS_EX_TOOLWINDOW
+            | win32con.WS_EX_NOACTIVATE
+        )
         style &= ~win32con.WS_EX_APPWINDOW
         win32gui.SetWindowLong(self.window, win32con.GWL_EXSTYLE, style)
         sleep(1)
         win32gui.ShowWindow(self.window, win32con.SW_SHOW)
         winxpgui.SetLayeredWindowAttributes(self.window, 0, 0, win32con.LWA_ALPHA)
 
     def hide(self):
         self.move_off_screen()
         self.make_transparent()
 
     def make_screenshot(self):
         import win32ui
+
         w, h = self.get_client_size()
 
         window_dc = win32gui.GetWindowDC(self.window)
         mfc_dc = win32ui.CreateDCFromHandle(window_dc)
         save_dc = mfc_dc.CreateCompatibleDC()
 
         save_bit_map = win32ui.CreateBitmap()
@@ -165,31 +193,41 @@
         save_dc.SelectObject(save_bit_map)
 
         ctypes.windll.user32.PrintWindow(self.window, save_dc.GetSafeHdc(), 1)
 
         bmpinfo = save_bit_map.GetInfo()
         bmpstr = save_bit_map.GetBitmapBits(True)
 
-        im = Image.frombuffer('RGB', (bmpinfo['bmWidth'], bmpinfo['bmHeight']), bmpstr, 'raw', 'BGRX', 0, 1)
+        im = Image.frombuffer(
+            "RGB",
+            (bmpinfo["bmWidth"], bmpinfo["bmHeight"]),
+            bmpstr,
+            "raw",
+            "BGRX",
+            0,
+            1,
+        )
 
         win32gui.DeleteObject(save_bit_map.GetHandle())
         save_dc.DeleteDC()
         mfc_dc.DeleteDC()
         win32gui.ReleaseDC(self.window, window_dc)
         return im
 
     def set_low_priority(self):
-        handle = win32api.OpenProcess(win32con.PROCESS_SET_INFORMATION, True, self.process.pid)
+        handle = win32api.OpenProcess(
+            win32con.PROCESS_SET_INFORMATION, True, self.process.pid
+        )
         win32process.SetPriorityClass(handle, BELOW_NORMAL_PRIORITY_CLASS)
         win32api.CloseHandle(handle)
 
 
 class Singleton:
     def __init__(self):
-        res = get_window('BHBot.exe')
+        res = get_window("BHBot.exe")
         if res:
             window, _ = res
             self.set_focus(window)
             sys.exit()
 
     @staticmethod
     def set_focus(window):
```

