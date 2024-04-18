# Comparing `tmp/pyboy-2.0.1.tar.gz` & `tmp/pyboy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboy-2.0.1.tar", last modified: Thu Mar 21 07:55:49 2024, max compression
+gzip compressed data, was "pyboy-2.0.2.tar", last modified: Thu Apr 18 16:06:03 2024, max compression
```

## Comparing `pyboy-2.0.1.tar` & `pyboy-2.0.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 07:55:49.852482 pyboy-2.0.1/
--rw-r--r--   0 runner     (501) staff       (20)     7558 2024-03-21 07:53:09.000000 pyboy-2.0.1/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)       59 2024-03-21 07:53:09.000000 pyboy-2.0.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    16450 2024-03-21 07:55:49.851879 pyboy-2.0.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6581 2024-03-21 07:53:09.000000 pyboy-2.0.1/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 07:55:49.833680 pyboy-2.0.1/pyboy/
--rw-r--r--   0 runner     (501) staff       (20)      263 2024-03-21 07:53:09.000000 pyboy-2.0.1/pyboy/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5607 2024-03-21 07:53:09.000000 pyboy-2.0.1/pyboy/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 07:55:49.837671 pyboy-2.0.1/pyboy/api/
--rw-r--r--   0 runner     (501) staff       (20)      485 2024-03-21 07:53:09.000000 pyboy-2.0.1/pyboy/api/memory_scanner.pxd
--rw-r--r--   0 runner     (501) staff       (20)      712 2024-03-21 07:53:09.000000 pyboy-2.0.1/pyboy/api/screen.pxd
--rw-r--r--   0 runner     (501) staff       (20)      671 2024-03-21 07:53:09.000000 pyboy-2.0.1/pyboy/api/sprite.pxd
--rw-r--r--   0 runner     (501) staff       (20)      730 2024-03-21 07:53:09.000000 pyboy-2.0.1/pyboy/api/tile.pxd
--rw-r--r--   0 runner     (501) staff       (20)      659 2024-03-21 07:53:09.000000 pyboy-2.0.1/pyboy/api/tilemap.pxd
--rw-r--r--   0 runner     (501) staff       (20)     9927 2024-03-21 07:53:09.000000 pyboy-2.0.1/pyboy/conftest.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 07:55:49.841382 pyboy-2.0.1/pyboy/core/
--rw-r--r--   0 runner     (501) staff       (20)      293 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/bootrom.pxd
--rw-r--r--   0 runner     (501) staff       (20)      256 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/bootrom_cgb.bin
--rw-r--r--   0 runner     (501) staff       (20)      256 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/bootrom_dmg.bin
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 07:55:49.843776 pyboy-2.0.1/pyboy/core/cartridge/
--rw-r--r--   0 runner     (501) staff       (20)     1359 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/cartridge/base_mbc.pxd
--rw-r--r--   0 runner     (501) staff       (20)      597 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/cartridge/cartridge.pxd
--rw-r--r--   0 runner     (501) staff       (20)      387 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/cartridge/mbc1.pxd
--rw-r--r--   0 runner     (501) staff       (20)      309 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/cartridge/mbc2.pxd
--rw-r--r--   0 runner     (501) staff       (20)      309 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/cartridge/mbc3.pxd
--rw-r--r--   0 runner     (501) staff       (20)      309 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/cartridge/mbc5.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1067 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/cartridge/rtc.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1589 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/cpu.pxd
--rw-r--r--   0 runner     (501) staff       (20)      658 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/interaction.pxd
--rw-r--r--   0 runner     (501) staff       (20)     8070 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/lcd.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2822 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/mb.pxd
--rw-r--r--   0 runner     (501) staff       (20)    51233 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/opcodes.pxd
--rw-r--r--   0 runner     (501) staff       (20)      656 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/ram.pxd
--rw-r--r--   0 runner     (501) staff       (20)     7670 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/sound.pxd
--rw-r--r--   0 runner     (501) staff       (20)      774 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/core/timer.pxd
--rw-r--r--   0 runner     (501) staff       (20)    32768 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/default_rom.gb
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 07:55:49.844442 pyboy-2.0.1/pyboy/logging/
--rw-r--r--   0 runner     (501) staff       (20)      376 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/logging/logging.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2933 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/logging/logging.pyx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 07:55:49.850388 pyboy-2.0.1/pyboy/plugins/
--rw-r--r--   0 runner     (501) staff       (20)      242 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/auto_pause.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2101 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/base_plugin.pxd
--rw-r--r--   0 runner     (501) staff       (20)     4407 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/debug.pxd
--rw-r--r--   0 runner     (501) staff       (20)      297 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/debug_prompt.pxd
--rw-r--r--   0 runner     (501) staff       (20)      245 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/disable_input.pxd
--rw-r--r--   0 runner     (501) staff       (20)     6490 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/font.txt
--rw-r--r--   0 runner     (501) staff       (20)      449 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/game_wrapper_kirby_dream_land.pxd
--rw-r--r--   0 runner     (501) staff       (20)      311 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/game_wrapper_pokemon_gen1.pxd
--rw-r--r--   0 runner     (501) staff       (20)      706 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/game_wrapper_super_mario_land.pxd
--rw-r--r--   0 runner     (501) staff       (20)      634 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/game_wrapper_tetris.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2872 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/manager.pxd
--rw-r--r--   0 runner     (501) staff       (20)      271 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/record_replay.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1835 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/rewind.pxd
--rw-r--r--   0 runner     (501) staff       (20)      277 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/screen_recorder.pxd
--rw-r--r--   0 runner     (501) staff       (20)      249 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/screenshot_recorder.pxd
--rw-r--r--   0 runner     (501) staff       (20)      232 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/window_null.pxd
--rw-r--r--   0 runner     (501) staff       (20)      843 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/window_open_gl.pxd
--rw-r--r--   0 runner     (501) staff       (20)      740 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/plugins/window_sdl2.pxd
--rw-r--r--   0 runner     (501) staff       (20)     3044 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/pyboy.pxd
--rw-r--r--   0 runner     (501) staff       (20)    65325 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/pyboy.py
--rw-r--r--   0 runner     (501) staff       (20)     1881 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/utils.pxd
--rw-r--r--   0 runner     (501) staff       (20)     9482 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyboy/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-21 07:55:49.850740 pyboy-2.0.1/pyboy.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    16450 2024-03-21 07:55:49.000000 pyboy-2.0.1/pyboy.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1618 2024-03-21 07:55:49.000000 pyboy-2.0.1/pyboy.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-03-21 07:55:49.000000 pyboy-2.0.1/pyboy.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-03-21 07:55:49.000000 pyboy-2.0.1/pyboy.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-03-21 07:55:49.000000 pyboy-2.0.1/pyboy.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       59 2024-03-21 07:55:49.000000 pyboy-2.0.1/pyboy.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        7 2024-03-21 07:55:49.000000 pyboy-2.0.1/pyboy.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1924 2024-03-21 07:53:10.000000 pyboy-2.0.1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-03-21 07:55:49.852553 pyboy-2.0.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3728 2024-03-21 07:53:10.000000 pyboy-2.0.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-18 16:06:03.886065 pyboy-2.0.2/
+-rw-r--r--   0 runner     (501) staff       (20)     7558 2024-04-18 16:03:21.000000 pyboy-2.0.2/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)       59 2024-04-18 16:03:21.000000 pyboy-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    16861 2024-04-18 16:06:03.885433 pyboy-2.0.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6992 2024-04-18 16:03:21.000000 pyboy-2.0.2/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-18 16:06:03.866827 pyboy-2.0.2/pyboy/
+-rw-r--r--   0 runner     (501) staff       (20)      263 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5607 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-18 16:06:03.870681 pyboy-2.0.2/pyboy/api/
+-rw-r--r--   0 runner     (501) staff       (20)      485 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/api/memory_scanner.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      712 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/api/screen.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      671 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/api/sprite.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      730 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/api/tile.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      659 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/api/tilemap.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     9927 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/conftest.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-18 16:06:03.874479 pyboy-2.0.2/pyboy/core/
+-rw-r--r--   0 runner     (501) staff       (20)      293 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/bootrom.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      256 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/bootrom_cgb.bin
+-rw-r--r--   0 runner     (501) staff       (20)      256 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/bootrom_dmg.bin
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-18 16:06:03.876712 pyboy-2.0.2/pyboy/core/cartridge/
+-rw-r--r--   0 runner     (501) staff       (20)     1359 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/cartridge/base_mbc.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      597 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/cartridge/cartridge.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      387 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/cartridge/mbc1.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      309 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/cartridge/mbc2.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      309 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/cartridge/mbc3.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      309 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/cartridge/mbc5.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1067 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/cartridge/rtc.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/cpu.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      658 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/interaction.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     8070 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/lcd.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2859 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/mb.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    51233 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/opcodes.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      656 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/ram.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     7670 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/sound.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      774 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/core/timer.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    32768 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/default_rom.gb
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-18 16:06:03.877420 pyboy-2.0.2/pyboy/logging/
+-rw-r--r--   0 runner     (501) staff       (20)      376 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/logging/logging.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2933 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/logging/logging.pyx
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-18 16:06:03.883906 pyboy-2.0.2/pyboy/plugins/
+-rw-r--r--   0 runner     (501) staff       (20)      242 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/auto_pause.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2101 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/base_plugin.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     4407 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/debug.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      297 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/debug_prompt.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/disable_input.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     6490 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/font.txt
+-rw-r--r--   0 runner     (501) staff       (20)      449 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/game_wrapper_kirby_dream_land.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      311 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/game_wrapper_pokemon_gen1.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      706 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/game_wrapper_super_mario_land.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      634 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/game_wrapper_tetris.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2872 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/manager.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      271 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/record_replay.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1835 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/rewind.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      277 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/screen_recorder.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      249 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/screenshot_recorder.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      232 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/window_null.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      843 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/window_open_gl.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      740 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/plugins/window_sdl2.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     3044 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/pyboy.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    65456 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/pyboy.py
+-rw-r--r--   0 runner     (501) staff       (20)     1881 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/utils.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     9482 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyboy/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-18 16:06:03.884290 pyboy-2.0.2/pyboy.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    16861 2024-04-18 16:06:03.000000 pyboy-2.0.2/pyboy.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1618 2024-04-18 16:06:03.000000 pyboy-2.0.2/pyboy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-18 16:06:03.000000 pyboy-2.0.2/pyboy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-04-18 16:06:03.000000 pyboy-2.0.2/pyboy.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-18 16:06:03.000000 pyboy-2.0.2/pyboy.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       59 2024-04-18 16:06:03.000000 pyboy-2.0.2/pyboy.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        7 2024-04-18 16:06:03.000000 pyboy-2.0.2/pyboy.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1933 2024-04-18 16:03:21.000000 pyboy-2.0.2/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-18 16:06:03.886147 pyboy-2.0.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3774 2024-04-18 16:03:21.000000 pyboy-2.0.2/setup.py
```

### Comparing `pyboy-2.0.1/LICENSE.md` & `pyboy-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/PKG-INFO` & `pyboy-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Game Boy emulator written in Python
 Author-email: Mads Ynddal <mads@ynddal.dk>
 License: GNU Lesser General Public License
         =================================
         
         _Version 3, 29 June 2007_
         _Copyright © 2007 Free Software Foundation, Inc. &lt;<http://fsf.org/>&gt;_
@@ -249,14 +249,22 @@
 ===============
 The instructions are simple:
 
 ```sh
 $ pip install pyboy
 ```
 
+> [!WARNING]
+> **If you're having issues on Windows, try this instead:** `pip install pyboy==2.0.0 pillow`
+>
+> PyPI (who maintains `pip install`) has stopped processing support tickets, and we've been unable to deploy
+> a fix for over a month now. Follow this thread for status: https://github.com/pypi/support/issues/3757
+>
+> If you're able to get in contact with PyPI, then please help us get this resolved!
+
 For details, see [installation instructions](https://github.com/Baekalfen/PyBoy/wiki/Installation).
 
 Now you're ready! Either use PyBoy directly from the terminal
 ```sh
 $ pyboy game_rom.gb
 ```
```

### Comparing `pyboy-2.0.1/README.md` & `pyboy-2.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,22 @@
 ===============
 The instructions are simple:
 
 ```sh
 $ pip install pyboy
 ```
 
+> [!WARNING]
+> **If you're having issues on Windows, try this instead:** `pip install pyboy==2.0.0 pillow`
+>
+> PyPI (who maintains `pip install`) has stopped processing support tickets, and we've been unable to deploy
+> a fix for over a month now. Follow this thread for status: https://github.com/pypi/support/issues/3757
+>
+> If you're able to get in contact with PyPI, then please help us get this resolved!
+
 For details, see [installation instructions](https://github.com/Baekalfen/PyBoy/wiki/Installation).
 
 Now you're ready! Either use PyBoy directly from the terminal
 ```sh
 $ pyboy game_rom.gb
 ```
```

#### html2text {}

```diff
@@ -4,21 +4,26 @@
 584149554132418570?style=for-the-badge&logo=Discord&label=PyBoy)](https://
 discord.gg/Zrf2nyH)
          _T_r_a_i_n_ _R_L_ _a_g_e_n_t_s_ _t_o_ _p_l_a_y_ _P_o_k_e_m_o_n_ _R_e_d            _R_e_w_i_n_d_ _a_n_y_ _g_a_m_e
                       _[_W_a_t_c_h_ _t_h_e_ _v_i_d_e_o_]            [extras/README/5.gif]
    Play the classics       _C_r_e_a_t_e_ _y_o_u_r_ _o_w_n_ _A_I   _B_e_a_t_ _w_o_r_l_d_ _r_e_c_o_r_d_s_ _w_i_t_h_ _A_I
 [extras/README/1.gif]    [extras/README/6.gif]     [extras/README/7.gif]
 Getting Started =============== The instructions are simple: ```sh $ pip
-install pyboy ``` For details, see [installation instructions](https://
-github.com/Baekalfen/PyBoy/wiki/Installation). Now you're ready! Either use
-PyBoy directly from the terminal ```sh $ pyboy game_rom.gb ``` Or use it in
-your Python scripts: ```python from pyboy import PyBoy pyboy = PyBoy
-('game_rom.gb') while pyboy.tick(): pass pyboy.stop() ``` The API ======= If
-you are looking to make a bot or AI, then these resources are a good place to
-start: * [PyBoy API Documentation](https://baekalfen.github.io/PyBoy/
+install pyboy ``` > [!WARNING] > **If you're having issues on Windows, try this
+instead:** `pip install pyboy==2.0.0 pillow` > > PyPI (who maintains `pip
+install`) has stopped processing support tickets, and we've been unable to
+deploy > a fix for over a month now. Follow this thread for status: https://
+github.com/pypi/support/issues/3757 > > If you're able to get in contact with
+PyPI, then please help us get this resolved! For details, see [installation
+instructions](https://github.com/Baekalfen/PyBoy/wiki/Installation). Now you're
+ready! Either use PyBoy directly from the terminal ```sh $ pyboy game_rom.gb
+``` Or use it in your Python scripts: ```python from pyboy import PyBoy pyboy =
+PyBoy('game_rom.gb') while pyboy.tick(): pass pyboy.stop() ``` The API =======
+If you are looking to make a bot or AI, then these resources are a good place
+to start: * [PyBoy API Documentation](https://baekalfen.github.io/PyBoy/
 index.html) * [Wiki Pages](https://github.com/Baekalfen/PyBoy/wiki/) * [Using
 PyBoy with Gym](https://github.com/Baekalfen/PyBoy/wiki/Using-PyBoy-with-Gym) *
 [Example: Kirby](https://github.com/Baekalfen/PyBoy/wiki/Example-Kirby) *
 [Example: Tetris](https://github.com/Baekalfen/PyBoy/wiki/Example-Tetris) *
 [Example: Super Mario Land](https://github.com/Baekalfen/PyBoy/wiki/Example-
 Super-Mario-Land) * [Code Examples](https://github.com/Baekalfen/PyBoy/tree/
 master/extras/examples) * [Discord](https://discord.gg/Zrf2nyH) When the
```

### Comparing `pyboy-2.0.1/pyboy/__main__.py` & `pyboy-2.0.2/pyboy/__main__.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/api/screen.pxd` & `pyboy-2.0.2/pyboy/api/screen.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/api/sprite.pxd` & `pyboy-2.0.2/pyboy/api/sprite.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/api/tile.pxd` & `pyboy-2.0.2/pyboy/api/tile.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/api/tilemap.pxd` & `pyboy-2.0.2/pyboy/api/tilemap.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/conftest.py` & `pyboy-2.0.2/pyboy/conftest.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/core/cartridge/base_mbc.pxd` & `pyboy-2.0.2/pyboy/core/cartridge/base_mbc.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/core/cartridge/cartridge.pxd` & `pyboy-2.0.2/pyboy/core/cartridge/cartridge.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/core/cartridge/rtc.pxd` & `pyboy-2.0.2/pyboy/core/cartridge/rtc.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/core/cpu.pxd` & `pyboy-2.0.2/pyboy/core/cpu.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/core/interaction.pxd` & `pyboy-2.0.2/pyboy/core/interaction.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/core/lcd.pxd` & `pyboy-2.0.2/pyboy/core/lcd.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/core/mb.pxd` & `pyboy-2.0.2/pyboy/core/mb.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,21 @@
 
     # CGB
     cdef HDMA hdma
     cdef uint8_t key1
     cdef bint double_speed
     cdef readonly bint cgb, cartridge_cgb
 
-    cdef list breakpoints_list
+    cdef dict breakpoints
     cdef bint breakpoint_singlestep
     cdef bint breakpoint_singlestep_latch
     cdef int64_t breakpoint_waiting
-    cdef int breakpoint_add(self, int64_t, int64_t) except -1 with gil
-    cdef void breakpoint_remove(self, int64_t) noexcept with gil
-    cdef inline int breakpoint_reached(self) noexcept with gil
+    cdef int64_t breakpoint_add(self, int64_t, int64_t) except -1 with gil
+    cdef void breakpoint_remove(self, int64_t, int64_t) noexcept with gil
+    cdef inline tuple[int64_t, int64_t, int64_t] breakpoint_reached(self) noexcept with gil
     cdef inline void breakpoint_reinject(self) noexcept nogil
 
     cdef inline bint processing_frame(self) noexcept nogil
 
     cdef void buttonevent(self, WindowEvent) noexcept
     cdef void stop(self, bint) noexcept
     @cython.locals(cycles=int64_t, mode0_cycles=int64_t, breakpoint_index=int64_t)
```

### Comparing `pyboy-2.0.1/pyboy/core/opcodes.pxd` & `pyboy-2.0.2/pyboy/core/opcodes.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/core/ram.pxd` & `pyboy-2.0.2/pyboy/core/ram.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/core/sound.pxd` & `pyboy-2.0.2/pyboy/core/sound.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/core/timer.pxd` & `pyboy-2.0.2/pyboy/core/timer.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/default_rom.gb` & `pyboy-2.0.2/pyboy/default_rom.gb`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/logging/logging.pyx` & `pyboy-2.0.2/pyboy/logging/logging.pyx`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/plugins/base_plugin.pxd` & `pyboy-2.0.2/pyboy/plugins/base_plugin.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/plugins/debug.pxd` & `pyboy-2.0.2/pyboy/plugins/debug.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/plugins/font.txt` & `pyboy-2.0.2/pyboy/plugins/font.txt`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/plugins/game_wrapper_super_mario_land.pxd` & `pyboy-2.0.2/pyboy/plugins/game_wrapper_super_mario_land.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/plugins/game_wrapper_tetris.pxd` & `pyboy-2.0.2/pyboy/plugins/game_wrapper_tetris.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/plugins/manager.pxd` & `pyboy-2.0.2/pyboy/plugins/manager.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/plugins/rewind.pxd` & `pyboy-2.0.2/pyboy/plugins/rewind.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/plugins/window_open_gl.pxd` & `pyboy-2.0.2/pyboy/plugins/window_open_gl.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/plugins/window_sdl2.pxd` & `pyboy-2.0.2/pyboy/plugins/window_sdl2.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/pyboy.pxd` & `pyboy-2.0.2/pyboy/pyboy.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/pyboy.py` & `pyboy-2.0.2/pyboy/pyboy.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,17 +344,18 @@
             # Reenter mb.tick until we eventually get a clean exit without breakpoints
             while self.mb.tick():
                 # Breakpoint reached
                 # NOTE: Potentially reinject breakpoint that we have now stepped passed
                 self.mb.breakpoint_reinject()
 
                 # NOTE: PC has not been incremented when hitting breakpoint!
-                breakpoint_index = self.mb.breakpoint_reached()
-                if breakpoint_index != -1:
-                    self.mb.breakpoint_remove(breakpoint_index)
+                breakpoint_meta = self.mb.breakpoint_reached()
+                if breakpoint_meta != (-1, -1, -1):
+                    bank, addr, _ = breakpoint_meta
+                    self.mb.breakpoint_remove(bank, addr)
                     self.mb.breakpoint_singlestep_latch = 0
 
                     if not self._handle_hooks():
                         self._plugin_manager.handle_breakpoint()
                 else:
                     if self.mb.breakpoint_singlestep_latch:
                         if not self._handle_hooks():
@@ -1089,14 +1090,15 @@
             bank, addr = self._lookup_symbol(addr)
 
         opcode = self.memory[bank, addr]
         if opcode == 0xDB:
             raise ValueError("Hook already registered for this bank and address.")
         self.mb.breakpoint_add(bank, addr)
         bank_addr_opcode = (bank & 0xFF) << 24 | (addr & 0xFFFF) << 8 | (opcode & 0xFF)
+        logger.debug("Adding hook for opcode %08x", bank_addr_opcode)
         self._hooks[bank_addr_opcode] = (callback, context)
 
     def hook_deregister(self, bank, addr):
         """
         Remove a previously registered hook from a specific bank and memory address.
 
         Example:
@@ -1121,20 +1123,20 @@
         Args:
             bank (int or None): ROM or RAM bank (None for symbol lookup)
             addr (int or str): Address in the Game Boy's address space (str for symbol lookup)
         """
         if bank is None and isinstance(addr, str):
             bank, addr = self._lookup_symbol(addr)
 
-        index = self.mb.breakpoint_find(bank, addr)
-        if index == -1:
+        breakpoint_meta = self.mb.breakpoint_find(bank, addr)
+        if not breakpoint_meta:
             raise ValueError("Breakpoint not found for bank and addr")
+        _, _, opcode = breakpoint_meta
 
-        _, _, opcode = self.mb.breakpoints_list[index]
-        self.mb.breakpoint_remove(index)
+        self.mb.breakpoint_remove(bank, addr)
         bank_addr_opcode = (bank & 0xFF) << 24 | (addr & 0xFFFF) << 8 | (opcode & 0xFF)
         self._hooks.pop(bank_addr_opcode)
 
     def _handle_hooks(self):
         if _handler := self._hooks.get(self.mb.breakpoint_waiting):
             (callback, context) = _handler
             callback(context)
```

### Comparing `pyboy-2.0.1/pyboy/utils.pxd` & `pyboy-2.0.2/pyboy/utils.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy/utils.py` & `pyboy-2.0.2/pyboy/utils.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyboy.egg-info/PKG-INFO` & `pyboy-2.0.2/pyboy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Game Boy emulator written in Python
 Author-email: Mads Ynddal <mads@ynddal.dk>
 License: GNU Lesser General Public License
         =================================
         
         _Version 3, 29 June 2007_
         _Copyright © 2007 Free Software Foundation, Inc. &lt;<http://fsf.org/>&gt;_
@@ -249,14 +249,22 @@
 ===============
 The instructions are simple:
 
 ```sh
 $ pip install pyboy
 ```
 
+> [!WARNING]
+> **If you're having issues on Windows, try this instead:** `pip install pyboy==2.0.0 pillow`
+>
+> PyPI (who maintains `pip install`) has stopped processing support tickets, and we've been unable to deploy
+> a fix for over a month now. Follow this thread for status: https://github.com/pypi/support/issues/3757
+>
+> If you're able to get in contact with PyPI, then please help us get this resolved!
+
 For details, see [installation instructions](https://github.com/Baekalfen/PyBoy/wiki/Installation).
 
 Now you're ready! Either use PyBoy directly from the terminal
 ```sh
 $ pyboy game_rom.gb
 ```
```

### Comparing `pyboy-2.0.1/pyboy.egg-info/SOURCES.txt` & `pyboy-2.0.2/pyboy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.1/pyproject.toml` & `pyboy-2.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyboy"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
     {name = "Mads Ynddal", email = "mads@ynddal.dk"}
 ]
 keywords = ["gameboy", "game boy", "emulator", "cython", "pypy"]
 description = "Game Boy emulator written in Python"
 readme = "README.md"
 license = {file = "LICENSE.md"}
@@ -40,15 +40,15 @@
 [project.scripts]
 pyboy = "pyboy.__main__:main"
 
 [build-system]
 requires = [
     "setuptools>=61.0.0",
     "wheel",
-    "cython>=3.0.6; platform_python_implementation == 'CPython'",
+    "cython>=3.0.6,!=3.0.10; platform_python_implementation == 'CPython'",
     "numpy",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 zip-safe = false
```

### Comparing `pyboy-2.0.1/setup.py` & `pyboy-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
         py_pxd_files = prep_pxd_py_files()
         cythonize_files = map(
             lambda src: Extension(
                 src.split(".")[0].replace(os.sep, "."),
                 [src],
                 extra_compile_args=cflags,
+                extra_link_args=["-s", "-w"],
                 include_dirs=[np.get_include()],
             ), list(py_pxd_files)
         )
         self.distribution.ext_modules = cythonize(
             [*cythonize_files],
             nthreads=thread_count,
             annotate=False,
```

