# Comparing `tmp/slint-1.6.0a5.tar.gz` & `tmp/slint-1.6.0a6.tar.gz`

## Comparing `slint-1.6.0a5.tar` & `slint-1.6.0a6.tar`

### file list

```diff
@@ -1,888 +1,888 @@
--rw-r--r--   0     1001      127      768 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/build/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/build/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127    15366 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/build/lib.rs
--rw-r--r--   0     1001      127     9884 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     1078 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/LICENSES/MIT.txt
--rw-r--r--   0     1001      127     1881 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/README.md
--rw-r--r--   0     1001      127     5140 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/android.rs
--rw-r--r--   0     1001      127      548 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/compile_fail_tests.rs
--rw-r--r--   0     1001      127     9447 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/building.md
--rw-r--r--   0     1001      127     7147 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/development.md
--rw-r--r--   0     1001      127     2881 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/install_qt.md
--rw-r--r--   0     1001      127        5 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/.gitignore
--rw-r--r--   0     1001      127     1013 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/README.md
--rw-r--r--   0     1001      127      261 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/book.toml
--rw-r--r--   0     1001      127      810 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt
--rw-r--r--   0     1001      127      515 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md
--rw-r--r--   0     1001      127      268 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/appwindow.slint
--rw-r--r--   0     1001      127     1216 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/conclusion.md
--rw-r--r--   0     1001      127     1337 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md
--rw-r--r--   0     1001      127     2039 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md
--rw-r--r--   0     1001      127     2483 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md
--rw-r--r--   0     1001      127     2126 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/getting_started.md
--rw-r--r--   0     1001      127      477 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/README.md
--rw-r--r--   0     1001      127     1122 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg
--rw-r--r--   0     1001      127     3210 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/at.png
--rw-r--r--   0     1001      127      971 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg
--rw-r--r--   0     1001      127     2265 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png
--rw-r--r--   0     1001      127     1577 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg
--rw-r--r--   0     1001      127     2613 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png
--rw-r--r--   0     1001      127      837 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg
--rw-r--r--   0     1001      127     1540 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png
--rw-r--r--   0     1001      127      485 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/cloud-solid.svg
--rw-r--r--   0     1001      127     1454 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png
--rw-r--r--   0     1001      127     2614 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg
--rw-r--r--   0     1001      127     2894 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png
--rw-r--r--   0     1001      127     1252 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg
--rw-r--r--   0     1001      127     2497 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png
--rw-r--r--   0     1001      127     6059 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png
--rw-r--r--   0     1001      127      467 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/video-solid.svg
--rw-r--r--   0     1001      127     1073 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/video.png
--rw-r--r--   0     1001      127     1060 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md
--rw-r--r--   0     1001      127      953 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/introduction.md
--rw-r--r--   0     1001      127     2800 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp
--rw-r--r--   0     1001      127      300 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/main_initial.cpp
--rw-r--r--   0     1001      127      877 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp
--rw-r--r--   0     1001      127     2620 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint
--rw-r--r--   0     1001      127     2130 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md
--rw-r--r--   0     1001      127      425 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/memory_tile.slint
--rw-r--r--   0     1001      127     2205 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint
--rw-r--r--   0     1001      127     2760 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md
--rw-r--r--   0     1001      127      262 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/book.toml
--rw-r--r--   0     1001      127      527 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/SUMMARY.md
--rw-r--r--   0     1001      127     1223 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/conclusion.md
--rw-r--r--   0     1001      127     1191 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md
--rw-r--r--   0     1001      127     2034 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md
--rw-r--r--   0     1001      127     2031 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md
--rw-r--r--   0     1001      127     1515 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/getting_started.md
--rw-r--r--   0     1001      127      477 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/README.md
--rw-r--r--   0     1001      127     1122 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg
--rw-r--r--   0     1001      127     3210 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/at.png
--rw-r--r--   0     1001      127      971 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg
--rw-r--r--   0     1001      127     2265 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png
--rw-r--r--   0     1001      127     1577 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg
--rw-r--r--   0     1001      127     2613 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png
--rw-r--r--   0     1001      127      837 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg
--rw-r--r--   0     1001      127     1540 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/bus.png
--rw-r--r--   0     1001      127      485 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/cloud-solid.svg
--rw-r--r--   0     1001      127     1454 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/cloud.png
--rw-r--r--   0     1001      127     2614 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg
--rw-r--r--   0     1001      127     2894 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/cogs.png
--rw-r--r--   0     1001      127     1252 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg
--rw-r--r--   0     1001      127     2497 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png
--rw-r--r--   0     1001      127     6059 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png
--rw-r--r--   0     1001      127      467 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/video-solid.svg
--rw-r--r--   0     1001      127     1073 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/video.png
--rw-r--r--   0     1001      127     1060 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md
--rw-r--r--   0     1001      127      960 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/introduction.md
--rw-r--r--   0     1001      127     1797 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/main_game_logic.js
--rw-r--r--   0     1001      127      275 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/main_initial.js
--rw-r--r--   0     1001      127      631 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js
--rw-r--r--   0     1001      127      265 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/memory.slint
--rw-r--r--   0     1001      127     2620 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint
--rw-r--r--   0     1001      127     2079 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/memory_tile.md
--rw-r--r--   0     1001      127      425 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/memory_tile.slint
--rw-r--r--   0     1001      127     2205 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint
--rw-r--r--   0     1001      127      202 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/package.json
--rw-r--r--   0     1001      127     2747 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md
--rw-r--r--   0     1001      127      262 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/rust/book.toml
--rw-r--r--   0     1001      127     3821 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/theme/head.hbs
--rw-r--r--   0     1001      127       84 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/theme/highlight.css
--rw-r--r--   0     1001      127      282 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/quickstart/theme/highlight.js
--rw-r--r--   0     1001      127      386 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/Pipfile
--rw-r--r--   0     1001      127      256 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/_static/theme_tweak.css
--rw-r--r--   0     1001      127      190 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/_templates/base.html
--rw-r--r--   0     1001      127     4339 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/conf.py
--rw-r--r--   0     1001      127      811 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/index.rst
--rw-r--r--   0     1001      127     7746 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md
--rw-r--r--   0     1001      127     1061 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/backend_qt.md
--rw-r--r--   0     1001      127     1692 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/backend_winit.md
--rw-r--r--   0     1001      127     7399 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md
--rw-r--r--   0     1001      127     6034 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md
--rw-r--r--   0     1001      127     3816 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/style.md
--rw-r--r--   0     1001      127     1095 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/introduction/index.md
--rw-r--r--   0     1001      127     2287 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/introduction/supported_platforms.md
--rw-r--r--   0     1001      127     1418 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/callbacks.md
--rw-r--r--   0     1001      127    40679 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/elements.md
--rw-r--r--   0     1001      127      975 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/functions.md
--rw-r--r--   0     1001      127     3227 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/globals.md
--rw-r--r--   0     1001      127      267 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/index.rst
--rw-r--r--   0     1001      127     3567 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/namespaces.md
--rw-r--r--   0     1001      127     1144 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/container.md
--rw-r--r--   0     1001      127     2165 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/file.md
--rw-r--r--   0     1001      127     1591 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/focus.md
--rw-r--r--   0     1001      127     1232 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/fonts.md
--rw-r--r--   0     1001      127      262 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/index.rst
--rw-r--r--   0     1001      127    13939 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/layouting.md
--rw-r--r--   0     1001      127     1787 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/purity.md
--rw-r--r--   0     1001      127     7822 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/translations.md
--rw-r--r--   0     1001      127     2235 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/index.rst
--rw-r--r--   0     1001      127     2270 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/animations.md
--rw-r--r--   0     1001      127     1627 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/callbacks.md
--rw-r--r--   0     1001      127      326 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/comments.md
--rw-r--r--   0     1001      127      492 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/conditions.md
--rw-r--r--   0     1001      127     1792 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/expressions.md
--rw-r--r--   0     1001      127     1821 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/functions.md
--rw-r--r--   0     1001      127     2776 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/globals.md
--rw-r--r--   0     1001      127      413 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/identifiers.md
--rw-r--r--   0     1001      127      402 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/index.rst
--rw-r--r--   0     1001      127      851 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md
--rw-r--r--   0     1001      127     3946 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/modules.md
--rw-r--r--   0     1001      127     5168 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/properties.md
--rw-r--r--   0     1001      127     1470 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/repetitions.md
--rw-r--r--   0     1001      127      658 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/statements.md
--rw-r--r--   0     1001      127     2210 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/states.md
--rw-r--r--   0     1001      127    17651 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/types.md
--rw-r--r--   0     1001      127      299 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/aboutslint.md
--rw-r--r--   0     1001      127     1469 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/button.md
--rw-r--r--   0     1001      127     1035 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/checkbox.md
--rw-r--r--   0     1001      127     1087 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/combobox.md
--rw-r--r--   0     1001      127      251 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/gridbox.md
--rw-r--r--   0     1001      127      741 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/groupbox.md
--rw-r--r--   0     1001      127      337 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/horizontalbox.md
--rw-r--r--   0     1001      127      569 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/index.rst
--rw-r--r--   0     1001      127     2305 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/lineedit.md
--rw-r--r--   0     1001      127     1293 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/listview.md
--rw-r--r--   0     1001      127      801 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md
--rw-r--r--   0     1001      127     1976 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/scrollview.md
--rw-r--r--   0     1001      127     1120 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/slider.md
--rw-r--r--   0     1001      127      841 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/spinbox.md
--rw-r--r--   0     1001      127      805 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/spinner.md
--rw-r--r--   0     1001      127     1071 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md
--rw-r--r--   0     1001      127     1489 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md
--rw-r--r--   0     1001      127     2176 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md
--rw-r--r--   0     1001      127     1037 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/switch.md
--rw-r--r--   0     1001      127      800 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md
--rw-r--r--   0     1001      127     2146 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/textedit.md
--rw-r--r--   0     1001      127      335 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/verticalbox.md
--rw-r--r--   0     1001      127      565 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/widgets.md
--rw-r--r--   0     1001      127      364 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/recipes/button_native.slint
--rw-r--r--   0     1001      127    28191 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/reference/src/recipes/recipes.md
--rw-r--r--   0     1001      127     3821 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/resources/slint-docs-highlight.html
--rw-r--r--   0     1001      127     5521 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/resources/slint-docs-preview.html
--rw-r--r--   0     1001      127    13863 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/site/index.html
--rw-r--r--   0     1001      127     3880 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/testing.md
--rw-r--r--   0     1001      127     1698 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/torizon.md
--rw-r--r--   0     1001      127     3775 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs/triage.md
--rw-r--r--   0     1001      127     6705 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/docs.rs
--rw-r--r--   0     1001      127    14341 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/lib.rs
--rw-r--r--   0     1001      127    20004 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/mcu.md
--rw-r--r--   0     1001      127     7535 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/private_unstable_api.rs
--rw-r--r--   0     1001      127     8721 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/tests/partial_renderer.rs
--rw-r--r--   0     1001      127      889 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/tests/show_strongref.rs
--rw-r--r--   0     1001      127     1119 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/tests/simple_macro.rs
--rw-r--r--   0     1001      127     2490 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/tests/spawn_local.rs
--rw-r--r--   0     1001      127     2557 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/slint/type-mappings.md
--rw-r--r--   0     1001      127     1109 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/android-activity/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      740 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/android-activity/README.md
--rw-r--r--   0     1001      127    34583 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/android-activity/androidwindowadapter.rs
--rw-r--r--   0     1001      127     4464 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/android-activity/build.rs
--rw-r--r--   0     1001      127    18055 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/android-activity/java/SlintAndroidJavaHelper.java
--rw-r--r--   0     1001      127    18156 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/android-activity/javahelper.rs
--rw-r--r--   0     1001      127     6133 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/android-activity/lib.rs
--rw-r--r--   0     1001      127     6405 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127    68116 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/api.rs
--rw-r--r--   0     1001      127    83639 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/dynamic_item_tree.rs
--rw-r--r--   0     1001      127     7555 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/dynamic_type.rs
--rw-r--r--   0     1001      127    73407 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/eval.rs
--rw-r--r--   0     1001      127    12240 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/eval_layout.rs
--rw-r--r--   0     1001      127    31460 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/ffi.rs
--rw-r--r--   0     1001      127     9875 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/global_component.rs
--rw-r--r--   0     1001      127     5912 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/highlight.rs
--rw-r--r--   0     1001      127     3015 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/lib.rs
--rw-r--r--   0     1001      127     1425 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/migration.rs
--rw-r--r--   0     1001      127     1795 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/tests.rs
--rw-r--r--   0     1001      127     2301 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/interpreter/value_model.rs
--rw-r--r--   0     1001      127      630 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/const-field-offset/Cargo.toml
--rw-r--r--   0     1001      127      610 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/const-field-offset/CHANGELOG.md
--rw-r--r--   0     1001      127    10280 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127     1078 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/const-field-offset/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      492 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/const-field-offset/README.md
--rw-r--r--   0     1001      127     6982 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/const-field-offset/src/lib.rs
--rw-r--r--   0     1001      127     4766 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/const-field-offset/tests/test_field_offset.rs
--rw-r--r--   0     1001      127      706 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/const-field-offset/macro/Cargo.toml
--rw-r--r--   0     1001      127    12200 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/const-field-offset/macro/macro.rs
--rw-r--r--   0     1001      127     4483 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      532 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/README.md
--rw-r--r--   0     1001      127     2766 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/accessibility.rs
--rw-r--r--   0     1001      127    13996 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/animations.rs
--rw-r--r--   0     1001      127    38608 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/api.rs
--rw-r--r--   0     1001      127     5210 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/callbacks.rs
--rw-r--r--   0     1001      127     2586 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/component_factory.rs
--rw-r--r--   0     1001      127     2553 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/context.rs
--rw-r--r--   0     1001      127     7694 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/future.rs
--rw-r--r--   0     1001      127     2503 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/bitmapfont.rs
--rw-r--r--   0     1001      127    14664 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/border_radius.rs
--rw-r--r--   0     1001      127     4038 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/boxshadowcache.rs
--rw-r--r--   0     1001      127    14919 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/brush.rs
--rw-r--r--   0     1001      127    17436 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/color.rs
--rw-r--r--   0     1001      127     7064 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/image/cache.rs
--rw-r--r--   0     1001      127     2528 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/image/htmlimage.rs
--rw-r--r--   0     1001      127     3408 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/image/svg.rs
--rw-r--r--   0     1001      127    48855 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/image.rs
--rw-r--r--   0     1001      127    15911 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/path.rs
--rw-r--r--   0     1001      127     6978 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics/rendering_metrics_collector.rs
--rw-r--r--   0     1001      127     8021 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/graphics.rs
--rw-r--r--   0     1001      127    33891 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/input.rs
--rw-r--r--   0     1001      127     8604 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/item_focus.rs
--rw-r--r--   0     1001      127    29328 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/item_rendering.rs
--rw-r--r--   0     1001      127    67985 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/item_tree.rs
--rw-r--r--   0     1001      127     8608 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/items/component_container.rs
--rw-r--r--   0     1001      127    17039 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/items/flickable.rs
--rw-r--r--   0     1001      127     8722 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/items/image.rs
--rw-r--r--   0     1001      127     5377 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/items/path.rs
--rw-r--r--   0     1001      127    65770 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/items/text.rs
--rw-r--r--   0     1001      127    46631 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/items.rs
--rw-r--r--   0     1001      127    27945 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/layout.rs
--rw-r--r--   0     1001      127     3222 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/lengths.rs
--rw-r--r--   0     1001      127     2237 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/lib.rs
--rw-r--r--   0     1001      127    47643 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/model/adapters.rs
--rw-r--r--   0     1001      127     6658 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/model/model_peer.rs
--rw-r--r--   0     1001      127    47290 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/model.rs
--rw-r--r--   0     1001      127    15948 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/platform.rs
--rw-r--r--   0     1001      127    15736 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/properties/ffi.rs
--rw-r--r--   0     1001      127    38401 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/properties/properties_animations.rs
--rw-r--r--   0     1001      127    58572 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/properties.rs
--rw-r--r--   0     1001      127     5015 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/renderer.rs
--rw-r--r--   0     1001      127    10886 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/rtti.rs
--rw-r--r--   0     1001      127    21418 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/sharedvector.rs
--rw-r--r--   0     1001      127     2865 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/slice.rs
--rw-r--r--   0     1001      127    29158 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/software_renderer/draw_functions.rs
--rw-r--r--   0     1001      127     3465 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/software_renderer/fixed.rs
--rw-r--r--   0     1001      127     4673 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/software_renderer/fonts/pixelfont.rs
--rw-r--r--   0     1001      127     3859 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/software_renderer/fonts/systemfonts.rs
--rw-r--r--   0     1001      127     7334 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/software_renderer/fonts/vectorfont.rs
--rw-r--r--   0     1001      127     5915 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/software_renderer/fonts.rs
--rw-r--r--   0     1001      127    99070 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/software_renderer.rs
--rw-r--r--   0     1001      127    13307 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/string.rs
--rw-r--r--   0     1001      127     4121 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/tests.rs
--rw-r--r--   0     1001      127    12929 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/textlayout/fragments.rs
--rw-r--r--   0     1001      127     3222 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/textlayout/glyphclusters.rs
--rw-r--r--   0     1001      127     1234 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/textlayout/linebreak_simple.rs
--rw-r--r--   0     1001      127     1260 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/textlayout/linebreak_unicode.rs
--rw-r--r--   0     1001      127    15364 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/textlayout/linebreaker.rs
--rw-r--r--   0     1001      127    13512 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/textlayout/shaping.rs
--rw-r--r--   0     1001      127    24952 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/textlayout.rs
--rw-r--r--   0     1001      127    31468 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/timers.rs
--rw-r--r--   0     1001      127     8559 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/translations.rs
--rw-r--r--   0     1001      127     1884 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/unsafe_single_threaded.rs
--rw-r--r--   0     1001      127    62402 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core/window.rs
--rw-r--r--   0     1001      127     1913 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/Cargo.toml
--rw-r--r--   0     1001      127    10280 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127    16830 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/LICENSES/CC-BY-ND-4.0.txt
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     1078 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      537 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/README.md
--rw-r--r--   0     1001      127     2420 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/build.rs
--rw-r--r--   0     1001      127    16358 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/builtin_macros.rs
--rw-r--r--   0     1001      127    18381 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/builtins.slint
--rw-r--r--   0     1001      127    19587 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/diagnostics.rs
--rw-r--r--   0     1001      127     2636 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/embedded_resources.rs
--rw-r--r--   0     1001      127    69622 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/expression_tree.rs
--rw-r--r--   0     1001      127     4420 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/fileaccess.rs
--rw-r--r--   0     1001      127   139818 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/generator/cpp.rs
--rw-r--r--   0     1001      127   122025 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/generator/rust.rs
--rw-r--r--   0     1001      127    19509 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/generator.rs
--rw-r--r--   0     1001      127    32752 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/langtype.rs
--rw-r--r--   0     1001      127    21425 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/layout.rs
--rw-r--r--   0     1001      127    15374 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/lexer.rs
--rw-r--r--   0     1001      127     9399 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/lib.rs
--rw-r--r--   0     1001      127     7020 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/literals.rs
--rw-r--r--   0     1001      127    31386 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/llr/expression.rs
--rw-r--r--   0     1001      127    13363 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/llr/item_tree.rs
--rw-r--r--   0     1001      127    40541 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/llr/lower_expression.rs
--rw-r--r--   0     1001      127    31339 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/llr/lower_to_item_tree.rs
--rw-r--r--   0     1001      127     6314 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/llr/optim_passes/count_property_use.rs
--rw-r--r--   0     1001      127     6235 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/llr/optim_passes/inline_expressions.rs
--rw-r--r--   0     1001      127    11380 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/llr/pretty_print.rs
--rw-r--r--   0     1001      127      654 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/llr.rs
--rw-r--r--   0     1001      127    11758 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/load_builtins.rs
--rw-r--r--   0     1001      127    39783 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/lookup.rs
--rw-r--r--   0     1001      127     7518 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/namedreference.rs
--rw-r--r--   0     1001      127   101372 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/object_tree.rs
--rw-r--r--   0     1001      127    10913 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/parser/document.rs
--rw-r--r--   0     1001      127    20594 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/parser/element.rs
--rw-r--r--   0     1001      127    14696 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/parser/expressions.rs
--rw-r--r--   0     1001      127     3102 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/parser/statements.rs
--rw-r--r--   0     1001      127     4561 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/parser/type.rs
--rw-r--r--   0     1001      127    36188 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/parser.rs
--rw-r--r--   0     1001      127     3949 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/apply_default_properties_from_style.rs
--rw-r--r--   0     1001      127    22379 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/binding_analysis.rs
--rw-r--r--   0     1001      127     1587 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/border_radius.rs
--rw-r--r--   0     1001      127     1793 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/check_expressions.rs
--rw-r--r--   0     1001      127     1941 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/check_public_api.rs
--rw-r--r--   0     1001      127     2309 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/check_rotation.rs
--rw-r--r--   0     1001      127     4580 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/clip.rs
--rw-r--r--   0     1001      127     2464 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/collect_custom_fonts.rs
--rw-r--r--   0     1001      127     1933 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/collect_globals.rs
--rw-r--r--   0     1001      127     1150 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/collect_init_code.rs
--rw-r--r--   0     1001      127     4172 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/collect_structs_and_enums.rs
--rw-r--r--   0     1001      127     1392 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/collect_subcomponents.rs
--rw-r--r--   0     1001      127     8043 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/compile_paths.rs
--rw-r--r--   0     1001      127     9466 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/const_propagation.rs
--rw-r--r--   0     1001      127     6155 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/deduplicate_property_read.rs
--rw-r--r--   0     1001      127    18877 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/default_geometry.rs
--rw-r--r--   0     1001      127    16260 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/embed_glyphs.rs
--rw-r--r--   0     1001      127    14883 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/embed_images.rs
--rw-r--r--   0     1001      127     5111 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/ensure_window.rs
--rw-r--r--   0     1001      127     6270 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/flickable.rs
--rw-r--r--   0     1001      127    10032 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/focus_handling.rs
--rw-r--r--   0     1001      127     4318 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/generate_item_indices.rs
--rw-r--r--   0     1001      127     6709 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/infer_aliases_types.rs
--rw-r--r--   0     1001      127    21709 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/inlining.rs
--rw-r--r--   0     1001      127     3241 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/lower_absolute_coordinates.rs
--rw-r--r--   0     1001      127     3268 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/lower_accessibility.rs
--rw-r--r--   0     1001      127     1697 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/lower_component_container.rs
--rw-r--r--   0     1001      127    31672 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/lower_layout.rs
--rw-r--r--   0     1001      127     5565 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/lower_popups.rs
--rw-r--r--   0     1001      127     5182 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/lower_property_to_element.rs
--rw-r--r--   0     1001      127     6916 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/lower_shadows.rs
--rw-r--r--   0     1001      127     9988 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/lower_states.rs
--rw-r--r--   0     1001      127     8355 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/lower_tabwidget.rs
--rw-r--r--   0     1001      127     2000 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/lower_text_input_interface.rs
--rw-r--r--   0     1001      127     6185 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/materialize_fake_properties.rs
--rw-r--r--   0     1001      127     6748 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/move_declarations.rs
--rw-r--r--   0     1001      127     2749 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/optimize_useless_rectangles.rs
--rw-r--r--   0     1001      127     4231 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/purity_check.rs
--rw-r--r--   0     1001      127     9197 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/remove_aliases.rs
--rw-r--r--   0     1001      127    19427 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/remove_return.rs
--rw-r--r--   0     1001      127     1656 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/remove_unused_properties.rs
--rw-r--r--   0     1001      127     5067 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/repeater_component.rs
--rw-r--r--   0     1001      127     5620 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/resolve_native_classes.rs
--rw-r--r--   0     1001      127    70883 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/resolving.rs
--rw-r--r--   0     1001      127     3046 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/unique_id.rs
--rw-r--r--   0     1001      127     4210 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/visible.rs
--rw-r--r--   0     1001      127     2961 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes/z_order.rs
--rw-r--r--   0     1001      127    10533 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/passes.rs
--rw-r--r--   0     1001      127    18378 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/pathutils.rs
--rw-r--r--   0     1001      127     8412 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/consistent_styles.rs
--rw-r--r--   0     1001      127     1237 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/accessibility/accessible_properties.slint
--rw-r--r--   0     1001      127     1774 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop1.slint
--rw-r--r--   0     1001      127     1826 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop2.slint
--rw-r--r--   0     1001      127      924 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_function.slint
--rw-r--r--   0     1001      127      643 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint
--rw-r--r--   0     1001      127     2458 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint
--rw-r--r--   0     1001      127     1854 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint
--rw-r--r--   0     1001      127     1144 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint
--rw-r--r--   0     1001      127     2120 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint
--rw-r--r--   0     1001      127      488 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_mappointtowindow.slint
--rw-r--r--   0     1001      127      923 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_self.slint
--rw-r--r--   0     1001      127      942 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/animate.slint
--rw-r--r--   0     1001      127      230 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/array.slint
--rw-r--r--   0     1001      127      788 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/assign.slint
--rw-r--r--   0     1001      127      585 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/box_shadow.slint
--rw-r--r--   0     1001      127     1021 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/children_placeholder.slint
--rw-r--r--   0     1001      127      301 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/children_placeholder_2.slint
--rw-r--r--   0     1001      127      663 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/clip.slint
--rw-r--r--   0     1001      127      492 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/comments.slint
--rw-r--r--   0     1001      127     2078 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/dialog.slint
--rw-r--r--   0     1001      127      631 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/dialog2.slint
--rw-r--r--   0     1001      127      499 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/double_binding.slint
--rw-r--r--   0     1001      127      270 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/double_color.slint
--rw-r--r--   0     1001      127     1137 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/duplicated_id.slint
--rw-r--r--   0     1001      127     1340 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/easing.slint
--rw-r--r--   0     1001      127      383 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/easing_not_called.slint
--rw-r--r--   0     1001      127      156 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/empty.slint
--rw-r--r--   0     1001      127      526 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/enums.slint
--rw-r--r--   0     1001      127      441 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/for.slint
--rw-r--r--   0     1001      127      492 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/image.slint
--rw-r--r--   0     1001      127      450 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/inline_component.slint
--rw-r--r--   0     1001      127      895 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/item_as_property.slint
--rw-r--r--   0     1001      127      465 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/layout.slint
--rw-r--r--   0     1001      127     1958 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/layout2.slint
--rw-r--r--   0     1001      127     2188 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/linear-gradient.slint
--rw-r--r--   0     1001      127      470 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/object_in_binding.slint
--rw-r--r--   0     1001      127      538 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/opacity.slint
--rw-r--r--   0     1001      127      905 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/parse_error.slint
--rw-r--r--   0     1001      127      535 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/path.slint
--rw-r--r--   0     1001      127     1114 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/path_commands.slint
--rw-r--r--   0     1001      127      541 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/path_for.slint
--rw-r--r--   0     1001      127     1056 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/percent.slint
--rw-r--r--   0     1001      127      707 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/popup.slint
--rw-r--r--   0     1001      127      333 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/property_animation.slint
--rw-r--r--   0     1001      127      983 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/property_declaration.slint
--rw-r--r--   0     1001      127      268 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/property_declaration_in_component.slint
--rw-r--r--   0     1001      127     1786 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/radial-gradient.slint
--rw-r--r--   0     1001      127      837 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/return.slint
--rw-r--r--   0     1001      127     1850 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/rotation.slint
--rw-r--r--   0     1001      127      456 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/rust-attr.slint
--rw-r--r--   0     1001      127     1781 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/self_assign.slint
--rw-r--r--   0     1001      127     1413 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/signal.slint
--rw-r--r--   0     1001      127     4436 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/states_transitions.slint
--rw-r--r--   0     1001      127      711 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/states_transitions2.slint
--rw-r--r--   0     1001      127      748 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/states_transitions3.slint
--rw-r--r--   0     1001      127      731 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/states_two_way.slint
--rw-r--r--   0     1001      127      731 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/sub_elements.slint
--rw-r--r--   0     1001      127      218 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/supersimple.slint
--rw-r--r--   0     1001      127      467 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/svg_path.slint
--rw-r--r--   0     1001      127     1600 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/tr.slint
--rw-r--r--   0     1001      127     3038 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/tr2.slint
--rw-r--r--   0     1001      127     1108 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/type_declaration.slint
--rw-r--r--   0     1001      127     1391 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/basic/unknown_item.slint
--rw-r--r--   0     1001      127      457 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/callbacks/init.slint
--rw-r--r--   0     1001      127      671 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/elements/component_container.slint
--rw-r--r--   0     1001      127     1202 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/elements/listview.slint
--rw-r--r--   0     1001      127      601 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/elements/popup.slint
--rw-r--r--   0     1001      127      538 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/elements/tabwidget.slint
--rw-r--r--   0     1001      127      898 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/elements/tabwidget2.slint
--rw-r--r--   0     1001      127      474 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/elements/tabwidget3.slint
--rw-r--r--   0     1001      127      436 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/exports/export_duplicates.slint
--rw-r--r--   0     1001      127      623 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/exports/reexport_duplicate.slint
--rw-r--r--   0     1001      127      326 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/exports/root_compo_export.slint
--rw-r--r--   0     1001      127      289 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/exports/root_compo_export2.slint
--rw-r--r--   0     1001      127      332 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/exports/single_global_missing_export.slint
--rw-r--r--   0     1001      127      288 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/exports/unused_compo.slint
--rw-r--r--   0     1001      127     1464 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/expressions/arithmetic_op.slint
--rw-r--r--   0     1001      127     1261 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/expressions/clamp.slint
--rw-r--r--   0     1001      127      999 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/expressions/comparison_operator.slint
--rw-r--r--   0     1001      127     1473 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/expressions/condition_operator.slint
--rw-r--r--   0     1001      127     3442 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/expressions/image-url.slint
--rw-r--r--   0     1001      127     1090 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/expressions/image-url2.slint
--rw-r--r--   0     1001      127     1355 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/expressions/minmax.slint
--rw-r--r--   0     1001      127      654 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/expressions/percent2.slint
--rw-r--r--   0     1001      127      456 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/expressions/strings.slint
--rw-r--r--   0     1001      127     1221 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/expressions/unary_op.slint
--rw-r--r--   0     1001      127      387 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/focus/focus_invalid.slint
--rw-r--r--   0     1001      127     1078 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/focus/focus_not_called.slint
--rw-r--r--   0     1001      127      595 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/focus/focus_wrong_args.slint
--rw-r--r--   0     1001      127     1707 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint
--rw-r--r--   0     1001      127      592 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/functions/function_double_qualified.slint
--rw-r--r--   0     1001      127     1814 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/functions/functions.slint
--rw-r--r--   0     1001      127     2990 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/functions/functions_call.slint
--rw-r--r--   0     1001      127     3353 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/functions/functions_purity.slint
--rw-r--r--   0     1001      127      597 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/bug_2719.slint
--rw-r--r--   0     1001      127     1018 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint
--rw-r--r--   0     1001      127      407 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/cyclic_import.slint
--rw-r--r--   0     1001      127      441 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/error_in_import.slint
--rw-r--r--   0     1001      127      252 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/error_in_import2.slint
--rw-r--r--   0     1001      127      295 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/error_in_import3.slint
--rw-r--r--   0     1001      127      410 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/font.slint
--rw-r--r--   0     1001      127      393 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/import_builtin.slint
--rw-r--r--   0     1001      127      411 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/import_error2.slint
--rw-r--r--   0     1001      127      944 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/import_errors.slint
--rw-r--r--   0     1001      127      207 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/import_parse_error1.slint
--rw-r--r--   0     1001      127      221 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/import_parse_error2.slint
--rw-r--r--   0     1001      127      238 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/import_parse_error3.slint
--rw-r--r--   0     1001      127      239 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/import_parse_error4.slint
--rw-r--r--   0     1001      127      503 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/import_parse_error5.slint
--rw-r--r--   0     1001      127      472 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/invalid_export.slint
--rw-r--r--   0     1001      127      379 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/imports/visibility_errors.slint
--rw-r--r--   0     1001      127      703 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/layout/if_in_grid.slint
--rw-r--r--   0     1001      127      441 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/layout/if_in_grid_row.slint
--rw-r--r--   0     1001      127      586 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/layout/min_max_conflict.slint
--rw-r--r--   0     1001      127      655 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/layout/spacing.slint
--rw-r--r--   0     1001      127      477 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/absolute-position.slint
--rw-r--r--   0     1001      127      691 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/array_index.slint
--rw-r--r--   0     1001      127      594 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/callback_alias.slint
--rw-r--r--   0     1001      127      641 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/callback_alias2.slint
--rw-r--r--   0     1001      127     1087 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/callback_alias3.slint
--rw-r--r--   0     1001      127      255 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/callback_alias_issue4938.slint
--rw-r--r--   0     1001      127      376 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/callback_not_called.slint
--rw-r--r--   0     1001      127      433 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/callback_return.slint
--rw-r--r--   0     1001      127     1814 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/color.slint
--rw-r--r--   0     1001      127     3112 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/conversion.slint
--rw-r--r--   0     1001      127     1807 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/dashes.slint
--rw-r--r--   0     1001      127     1250 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/deprecated_property.slint
--rw-r--r--   0     1001      127     1138 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/enum.slint
--rw-r--r--   0     1001      127     2598 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/for_lookup.slint
--rw-r--r--   0     1001      127     1211 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/global.slint
--rw-r--r--   0     1001      127      621 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/if.slint
--rw-r--r--   0     1001      127      920 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/issue_1461.slint
--rw-r--r--   0     1001      127     1287 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/property.slint
--rw-r--r--   0     1001      127     1704 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint
--rw-r--r--   0     1001      127     1439 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/signal_arg.slint
--rw-r--r--   0     1001      127     1444 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/two_way_binding.slint
--rw-r--r--   0     1001      127     1220 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint
--rw-r--r--   0     1001      127      392 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/lookup/two_way_binding_model.slint
--rw-r--r--   0     1001      127      903 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint
--rw-r--r--   0     1001      127     2695 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/input_output.slint
--rw-r--r--   0     1001      127     3062 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/input_output2.slint
--rw-r--r--   0     1001      127      593 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/new_component.slint
--rw-r--r--   0     1001      127     1020 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/new_lookup.slint
--rw-r--r--   0     1001      127     8651 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint
--rw-r--r--   0     1001      127      252 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/children_placeholder0.slint
--rw-r--r--   0     1001      127      263 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/export0.slint
--rw-r--r--   0     1001      127      219 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/export1.slint
--rw-r--r--   0     1001      127      362 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/if0.slint
--rw-r--r--   0     1001      127      278 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/if1.slint
--rw-r--r--   0     1001      127      285 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/if2.slint
--rw-r--r--   0     1001      127      224 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/if3.slint
--rw-r--r--   0     1001      127      361 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/if4.slint
--rw-r--r--   0     1001      127      398 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/property1.slint
--rw-r--r--   0     1001      127      902 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/property2.slint
--rw-r--r--   0     1001      127      846 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/state1.slint
--rw-r--r--   0     1001      127      244 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/state2.slint
--rw-r--r--   0     1001      127      307 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/state3.slint
--rw-r--r--   0     1001      127      707 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/struct.slint
--rw-r--r--   0     1001      127     9426 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/syntax_tests.rs
--rw-r--r--   0     1001      127      156 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/custom_style/TestStyle/std-widgets.slint
--rw-r--r--   0     1001      127      278 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/dependency_local.slint
--rw-r--r--   0     1001      127      393 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/dependency_test_main.slint
--rw-r--r--   0     1001      127      503 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/incpath/bug_2719_import.slint
--rw-r--r--   0     1001      127      461 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/incpath/bug_3674_alias_from_invalid_import.slint
--rw-r--r--   0     1001      127      262 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/incpath/dependency_from_incpath.slint
--rw-r--r--   0     1001      127      205 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/incpath/local_helper_type.slint
--rw-r--r--   0     1001      127      237 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/incpath/should_fail.slint
--rw-r--r--   0     1001      127      320 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/incpath/should_fail2.slint
--rw-r--r--   0     1001      127      280 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/incpath/should_fail3.slint
--rw-r--r--   0     1001      127      491 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/incpath/should_fail4.slint
--rw-r--r--   0     1001      127      208 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/library/dependency_from_library.slint
--rw-r--r--   0     1001      127      243 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/library/lib.slint
--rw-r--r--   0     1001      127      214 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/library/library_helper_type.slint
--rw-r--r--   0     1001      127      324 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/recursive_import1.slint
--rw-r--r--   0     1001      127      395 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/recursive_import2.slint
--rw-r--r--   0     1001      127      450 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/tests/typeloader/some_rust_file.rs
--rw-r--r--   0     1001      127    43496 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/typeloader.rs
--rw-r--r--   0     1001      127    19576 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/typeregister.rs
--rw-r--r--   0     1001      127    14083 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg
--rw-r--r--   0     1001      127    14073 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg
--rw-r--r--   0     1001      127     2358 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/combobox-base.slint
--rw-r--r--   0     1001      127     3861 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/common.slint
--rw-r--r--   0     1001      127     3184 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/lineedit-base.slint
--rw-r--r--   0     1001      127     4288 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/listview.slint
--rw-r--r--   0     1001      127     3920 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/slider-base.slint
--rw-r--r--   0     1001      127     2418 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/spinbox-base.slint
--rw-r--r--   0     1001      127     2510 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/spinner-base.slint
--rw-r--r--   0     1001      127     1202 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/standardbutton.slint
--rw-r--r--   0     1001      127     1080 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/common/tabwidget-base.slint
--rw-r--r--   0     1001      127      268 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic/std-widgets.slint
--rw-r--r--   0     1001      127      308 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/_arrow_down.svg
--rw-r--r--   0     1001      127      284 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/_arrow_up.svg
--rw-r--r--   0     1001      127      413 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/_check-mark.svg
--rw-r--r--   0     1001      127      148 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/_pane_down.svg
--rw-r--r--   0     1001      127     2710 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/button.slint
--rw-r--r--   0     1001      127     2726 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/checkbox.slint
--rw-r--r--   0     1001      127     3057 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/combobox.slint
--rw-r--r--   0     1001      127     4437 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/components.slint
--rw-r--r--   0     1001      127     1000 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/groupbox.slint
--rw-r--r--   0     1001      127      632 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/layouts.slint
--rw-r--r--   0     1001      127     2886 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/lineedit.slint
--rw-r--r--   0     1001      127      988 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/progressindicator.slint
--rw-r--r--   0     1001      127     5065 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/scrollview.slint
--rw-r--r--   0     1001      127     2930 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/slider.slint
--rw-r--r--   0     1001      127     3327 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/spinbox.slint
--rw-r--r--   0     1001      127      733 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/spinner.slint
--rw-r--r--   0     1001      127     1524 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2126 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     3420 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/styling.slint
--rw-r--r--   0     1001      127     2861 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/switch.slint
--rw-r--r--   0     1001      127     9124 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/tableview.slint
--rw-r--r--   0     1001      127     6075 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/tabwidget.slint
--rw-r--r--   0     1001      127     4438 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-base/textedit.slint
--rw-r--r--   0     1001      127      257 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-dark/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-light/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cosmic-light/std-widgets.slint
--rw-r--r--   0     1001      127      268 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino/color-scheme.slint
--rw-r--r--   0     1001      127      332 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino/std-widgets-impl.slint
--rw-r--r--   0     1001      127      215 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino/std-widgets.slint
--rw-r--r--   0     1001      127      513 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_arrow-down.svg
--rw-r--r--   0     1001      127      507 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_arrow-up.svg
--rw-r--r--   0     1001      127      780 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_check-mark.svg
--rw-r--r--   0     1001      127      623 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_chevron-down.svg
--rw-r--r--   0     1001      127      601 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_chevron-up.svg
--rw-r--r--   0     1001      127      918 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_down.svg
--rw-r--r--   0     1001      127      489 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_dropdown.svg
--rw-r--r--   0     1001      127      849 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_left.svg
--rw-r--r--   0     1001      127      815 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_right.svg
--rw-r--r--   0     1001      127     1135 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_up.svg
--rw-r--r--   0     1001      127     5134 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/button.slint
--rw-r--r--   0     1001      127     4547 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/checkbox.slint
--rw-r--r--   0     1001      127     5646 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/combobox.slint
--rw-r--r--   0     1001      127     3145 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/components.slint
--rw-r--r--   0     1001      127     1103 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/groupbox.slint
--rw-r--r--   0     1001      127      632 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/layouts.slint
--rw-r--r--   0     1001      127     3180 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/lineedit.slint
--rw-r--r--   0     1001      127     1404 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/progressindicator.slint
--rw-r--r--   0     1001      127     5563 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/scrollview.slint
--rw-r--r--   0     1001      127     3097 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/slider.slint
--rw-r--r--   0     1001      127     5483 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/spinbox.slint
--rw-r--r--   0     1001      127      739 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/spinner.slint
--rw-r--r--   0     1001      127     1524 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2216 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     4541 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/styling.slint
--rw-r--r--   0     1001      127     4097 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/switch.slint
--rw-r--r--   0     1001      127     8959 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/tableview.slint
--rw-r--r--   0     1001      127     5493 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/tabwidget.slint
--rw-r--r--   0     1001      127     6640 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-base/textedit.slint
--rw-r--r--   0     1001      127      257 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-dark/color-scheme.slint
--rw-r--r--   0     1001      127      332 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      215 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-light/color-scheme.slint
--rw-r--r--   0     1001      127      332 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      215 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/cupertino-light/std-widgets.slint
--rw-r--r--   0     1001      127      268 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent/std-widgets.slint
--rw-r--r--   0     1001      127      513 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/_arrow-down.svg
--rw-r--r--   0     1001      127      507 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/_arrow-up.svg
--rw-r--r--   0     1001      127      780 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/_check-mark.svg
--rw-r--r--   0     1001      127      623 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/_chevron-down.svg
--rw-r--r--   0     1001      127      601 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/_chevron-up.svg
--rw-r--r--   0     1001      127      918 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/_down.svg
--rw-r--r--   0     1001      127      489 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/_dropdown.svg
--rw-r--r--   0     1001      127      849 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/_left.svg
--rw-r--r--   0     1001      127      815 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/_right.svg
--rw-r--r--   0     1001      127     1135 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/_up.svg
--rw-r--r--   0     1001      127     4556 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/button.slint
--rw-r--r--   0     1001      127     3883 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/checkbox.slint
--rw-r--r--   0     1001      127     3773 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/combobox.slint
--rw-r--r--   0     1001      127     3363 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/components.slint
--rw-r--r--   0     1001      127      877 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/groupbox.slint
--rw-r--r--   0     1001      127      632 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/layouts.slint
--rw-r--r--   0     1001      127     3499 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/lineedit.slint
--rw-r--r--   0     1001      127     1023 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/progressindicator.slint
--rw-r--r--   0     1001      127     6590 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/scrollview.slint
--rw-r--r--   0     1001      127     3734 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/slider.slint
--rw-r--r--   0     1001      127     3992 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/spinbox.slint
--rw-r--r--   0     1001      127      733 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/spinner.slint
--rw-r--r--   0     1001      127     1524 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2126 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     6248 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/styling.slint
--rw-r--r--   0     1001      127     4616 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/switch.slint
--rw-r--r--   0     1001      127     9561 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/tableview.slint
--rw-r--r--   0     1001      127     5493 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/tabwidget.slint
--rw-r--r--   0     1001      127     4935 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-base/textedit.slint
--rw-r--r--   0     1001      127      257 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-dark/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-light/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/fluent-light/std-widgets.slint
--rw-r--r--   0     1001      127      268 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material/color-scheme.slint
--rw-r--r--   0     1001      127      347 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material/std-widgets-impl.slint
--rw-r--r--   0     1001      127      214 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material/std-widgets.slint
--rw-r--r--   0     1001      127      163 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/_arrow-downward.svg
--rw-r--r--   0     1001      127      115 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/_arrow-drop-down.svg
--rw-r--r--   0     1001      127      115 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/_arrow-drop-up.svg
--rw-r--r--   0     1001      127      161 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/_arrow-upward.svg
--rw-r--r--   0     1001      127      150 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/_check-mark.svg
--rw-r--r--   0     1001      127      145 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/_expand-more.svg
--rw-r--r--   0     1001      127     3239 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/button.slint
--rw-r--r--   0     1001      127     5664 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/checkbox.slint
--rw-r--r--   0     1001      127     3452 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/combobox.slint
--rw-r--r--   0     1001      127     4712 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/components.slint
--rw-r--r--   0     1001      127     1477 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/groupbox.slint
--rw-r--r--   0     1001      127      633 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/layouts.slint
--rw-r--r--   0     1001      127     2866 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/lineedit.slint
--rw-r--r--   0     1001      127     1010 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/progressindicator.slint
--rw-r--r--   0     1001      127     5014 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/scrollview.slint
--rw-r--r--   0     1001      127     4146 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/slider.slint
--rw-r--r--   0     1001      127     5090 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/spinbox.slint
--rw-r--r--   0     1001      127      737 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/spinner.slint
--rw-r--r--   0     1001      127     1373 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2213 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     3651 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/styling.slint
--rw-r--r--   0     1001      127     6174 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/switch.slint
--rw-r--r--   0     1001      127     8186 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/tableview.slint
--rw-r--r--   0     1001      127     4886 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-base/tabwidget.slint
--rw-r--r--   0     1001      127      257 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-dark/color-scheme.slint
--rw-r--r--   0     1001      127      331 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      214 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-light/color-scheme.slint
--rw-r--r--   0     1001      127      331 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      214 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/material-light/std-widgets.slint
--rw-r--r--   0     1001      127     1642 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/button.slint
--rw-r--r--   0     1001      127      350 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/checkbox.slint
--rw-r--r--   0     1001      127     1707 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/combobox.slint
--rw-r--r--   0     1001      127      582 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/groupbox.slint
--rw-r--r--   0     1001      127     2384 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/internal-scrollview.slint
--rw-r--r--   0     1001      127      613 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/layouts.slint
--rw-r--r--   0     1001      127     2377 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/lineedit.slint
--rw-r--r--   0     1001      127      307 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/progressindicator.slint
--rw-r--r--   0     1001      127     1026 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/scrollview.slint
--rw-r--r--   0     1001      127      422 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/slider.slint
--rw-r--r--   0     1001      127      834 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/spinbox.slint
--rw-r--r--   0     1001      127     1265 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/spinner.slint
--rw-r--r--   0     1001      127      374 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/std-widgets-impl.slint
--rw-r--r--   0     1001      127     1475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/std-widgets.slint
--rw-r--r--   0     1001      127      346 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/switch.slint
--rw-r--r--   0     1001      127     5310 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/tableview.slint
--rw-r--r--   0     1001      127     1564 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/widgets/qt/tabwidget.slint
--rw-r--r--   0     1001      127     1955 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     1078 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      507 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/README.md
--rw-r--r--   0     1001      127    15614 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/calloop_backend/input.rs
--rw-r--r--   0     1001      127    12022 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/calloop_backend.rs
--rw-r--r--   0     1001      127     8655 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/display/gbmdisplay.rs
--rw-r--r--   0     1001      127     2955 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/display/swdisplay.rs
--rw-r--r--   0     1001      127     9345 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/display/vulkandisplay.rs
--rw-r--r--   0     1001      127     3237 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/display.rs
--rw-r--r--   0     1001      127    12140 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/drmoutput.rs
--rw-r--r--   0     1001      127     6253 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/fullscreenwindowadapter.rs
--rw-r--r--   0     1001      127     2022 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/lib.rs
--rw-r--r--   0     1001      127      365 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/mouse-pointer.svg
--rw-r--r--   0     1001      127      882 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/noop_backend.rs
--rw-r--r--   0     1001      127     7507 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/renderer/femtovg.rs
--rw-r--r--   0     1001      127     6654 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/linuxkms/renderer/skia.rs
--rw-r--r--   0     1001      127     1383 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/README.md
--rw-r--r--   0     1001      127    10783 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/accessible_generated.rs
--rw-r--r--   0     1001      127     2995 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/build.rs
--rw-r--r--   0     1001      127    27433 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/key_generated.rs
--rw-r--r--   0     1001      127    10534 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/lib.rs
--rw-r--r--   0     1001      127    32883 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_accessible.rs
--rw-r--r--   0     1001      127    21040 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/button.rs
--rw-r--r--   0     1001      127     6862 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/checkbox.rs
--rw-r--r--   0     1001      127     9594 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/combobox.rs
--rw-r--r--   0     1001      127     8992 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/groupbox.rs
--rw-r--r--   0     1001      127     5930 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/lineedit.rs
--rw-r--r--   0     1001      127     8178 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/listviewitem.rs
--rw-r--r--   0     1001      127     7422 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/palette.rs
--rw-r--r--   0     1001      127     4945 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/progress_indicator.rs
--rw-r--r--   0     1001      127    19794 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/scrollview.rs
--rw-r--r--   0     1001      127    13934 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/slider.rs
--rw-r--r--   0     1001      127    12529 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/spinbox.rs
--rw-r--r--   0     1001      127     8594 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/stylemetrics.rs
--rw-r--r--   0     1001      127     5637 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/tableheadersection.rs
--rw-r--r--   0     1001      127    22411 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets/tabwidget.rs
--rw-r--r--   0     1001      127    12967 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_widgets.rs
--rw-r--r--   0     1001      127   103898 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/qt/qt_window.rs
--rw-r--r--   0     1001      127     2855 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/README.md
--rw-r--r--   0     1001      127      673 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/build.rs
--rw-r--r--   0     1001      127     6875 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/cached_image.rs
--rw-r--r--   0     1001      127    14877 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/d3d_surface.rs
--rw-r--r--   0     1001      127    34690 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/itemrenderer.rs
--rw-r--r--   0     1001      127    23253 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/lib.rs
--rw-r--r--   0     1001      127     6372 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/metal_surface.rs
--rw-r--r--   0     1001      127    15370 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/opengl_surface.rs
--rw-r--r--   0     1001      127     4611 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/software_surface.rs
--rw-r--r--   0     1001      127    11843 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/textlayout.rs
--rw-r--r--   0     1001      127    17420 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/skia/vulkan_surface.rs
--rw-r--r--   0     1001      127      738 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/macros/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/macros/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/macros/README.md
--rw-r--r--   0     1001      127    19345 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/rs/macros/lib.rs
--rw-r--r--   0     1001      127      571 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/macro/Cargo.toml
--rw-r--r--   0     1001      127    10280 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127     1078 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/macro/LICENSES/MIT.txt
--rw-r--r--   0     1001      127    31632 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/macro/macro.rs
--rw-r--r--   0     1001      127      603 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/testing/Cargo.toml
--rw-r--r--   0     1001      127      507 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/testing/README.md
--rw-r--r--   0     1001      127    10886 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/testing/lib.rs
--rw-r--r--   0     1001      127      532 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core-macros/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core-macros/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      590 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core-macros/README.md
--rw-r--r--   0     1001      127     7310 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/core-macros/lib.rs
--rw-r--r--   0     1001      127     3852 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     2320 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/README.md
--rw-r--r--   0     1001      127    21942 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/accesskit.rs
--rw-r--r--   0     1001      127      474 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/build.rs
--rw-r--r--   0     1001      127    30209 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/event_loop.rs
--rw-r--r--   0     1001      127    16654 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/lib.rs
--rw-r--r--   0     1001      127     8046 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/renderer/femtovg/glcontext.rs
--rw-r--r--   0     1001      127     2131 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/renderer/femtovg.rs
--rw-r--r--   0     1001      127     4558 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/renderer/skia.rs
--rw-r--r--   0     1001      127     6824 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/renderer/sw.rs
--rw-r--r--   0     1001      127    14717 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/wasm_input_helper.rs
--rw-r--r--   0     1001      127    32085 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/winit/winitwindowadapter.rs
--rw-r--r--   0     1001      127     2370 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/selector/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/selector/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      872 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/selector/README.md
--rw-r--r--   0     1001      127     2014 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/selector/build.rs
--rw-r--r--   0     1001      127     5859 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/backends/selector/lib.rs
--rw-r--r--   0     1001      127     1126 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     8815 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      635 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/README.md
--rw-r--r--   0     1001      127     7636 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/builtin_structs.rs
--rw-r--r--   0     1001      127    19223 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/enums.rs
--rw-r--r--   0     1001      127     8311 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/key_codes.rs
--rw-r--r--   0     1001      127     1322 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/lib.rs
--rw-r--r--   0     1001      127   757076 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/sharedfontdb/DejaVuSans.ttf
--rw-r--r--   0     1001      127      145 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/sharedfontdb/DejaVuSans.ttf.license
--rw-r--r--   0     1001      127     4526 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/sharedfontdb/fontconfig.rs
--rw-r--r--   0     1001      127     7491 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/common/sharedfontdb.rs
--rw-r--r--   0     1001      127     1919 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/femtovg/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/femtovg/README.md
--rw-r--r--   0     1001      127    26501 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/femtovg/fonts.rs
--rw-r--r--   0     1001      127     9732 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/femtovg/images.rs
--rw-r--r--   0     1001      127    60402 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/femtovg/itemrenderer.rs
--rw-r--r--   0     1001      127    23205 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/renderers/femtovg/lib.rs
--rw-r--r--   0     1001      127      471 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/parser-test-macro/Cargo.toml
--rw-r--r--   0     1001      127      887 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/parser-test-macro/README.md
--rw-r--r--   0     1001      127     5619 2024-04-18 11:51:20.000000 slint-1.6.0a5/internal/compiler/parser-test-macro/lib.rs
--rw-r--r--   0     1001      127      623 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/Cargo.toml
--rw-r--r--   0     1001      127     1796 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/CHANGELOG.md
--rw-r--r--   0     1001      127    10280 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127     1078 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      399 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/README.md
--rw-r--r--   0     1001      127     3723 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/src/compile_fail_tests.rs
--rw-r--r--   0     1001      127    18776 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/src/lib.rs
--rw-r--r--   0     1001      127    18973 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/src/vrc.rs
--rw-r--r--   0     1001      127     9552 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/tests/test_vrc.rs
--rw-r--r--   0     1001      127     5359 2024-04-18 11:51:20.000000 slint-1.6.0a5/helper_crates/vtable/tests/test_vtable.rs
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 slint-1.6.0a5/api/python/Cargo.toml
--rw-r--r--   0     1001      127       11 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/.gitignore
--rw-r--r--   0     1001      127     7397 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/README.md
--rw-r--r--   0     1001      127     4367 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/brush.rs
--rw-r--r--   0     1001      127     3303 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/errors.rs
--rw-r--r--   0     1001      127     1399 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/image.rs
--rw-r--r--   0     1001      127    10939 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/interpreter.rs
--rw-r--r--   0     1001      127     1421 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/lib.rs
--rw-r--r--   0     1001      127     6300 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/models.rs
--rw-r--r--   0     1001      127      348 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/noxfile.py
--rw-r--r--   0     1001      127     7684 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/slint/__init__.py
--rw-r--r--   0     1001      127     1889 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/slint/models.py
--rw-r--r--   0     1001      127     1164 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/tests/test_brush.py
--rw-r--r--   0     1001      127     1019 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/tests/test_callback_decorators.py
--rw-r--r--   0     1001      127     2369 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/tests/test_compiler.py
--rw-r--r--   0     1001      127     1095 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/tests/test_gc.py
--rw-r--r--   0     1001      127      831 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/tests/test_import.py
--rw-r--r--   0     1001      127     6577 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/tests/test_instance.py
--rw-r--r--   0     1001      127     1597 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/tests/test_load_file.py
--rw-r--r--   0     1001      127      905 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/tests/test_load_file.slint
--rw-r--r--   0     1001      127     3589 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/tests/test_models.py
--rw-r--r--   0     1001      127      832 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/tests/test_timers.py
--rw-r--r--   0     1001      127     2403 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/timer.rs
--rw-r--r--   0     1001      127     4717 2024-04-18 11:51:20.000000 slint-1.6.0a5/api/python/value.rs
--rw-r--r--   0     1001      127   207085 2024-04-18 11:51:27.000000 slint-1.6.0a5/Cargo.lock
--rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 slint-1.6.0a5/Cargo.toml
--rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 slint-1.6.0a5/pyproject.toml
--rw-r--r--   0     1001      127     7684 2024-04-18 11:51:20.000000 slint-1.6.0a5/slint/__init__.py
--rw-r--r--   0     1001      127     1889 2024-04-18 11:51:20.000000 slint-1.6.0a5/slint/models.py
--rw-r--r--   0        0        0     8944 1970-01-01 00:00:00.000000 slint-1.6.0a5/PKG-INFO
+-rw-r--r--   0     1001      127     3852 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     2320 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/README.md
+-rw-r--r--   0     1001      127    21942 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/accesskit.rs
+-rw-r--r--   0     1001      127      474 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/build.rs
+-rw-r--r--   0     1001      127    30209 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/event_loop.rs
+-rw-r--r--   0     1001      127    16654 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/lib.rs
+-rw-r--r--   0     1001      127     8046 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/renderer/femtovg/glcontext.rs
+-rw-r--r--   0     1001      127     2131 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/renderer/femtovg.rs
+-rw-r--r--   0     1001      127     4558 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/renderer/skia.rs
+-rw-r--r--   0     1001      127     6824 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/renderer/sw.rs
+-rw-r--r--   0     1001      127    14717 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/wasm_input_helper.rs
+-rw-r--r--   0     1001      127    32085 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/winitwindowadapter.rs
+-rw-r--r--   0     1001      127     4483 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      532 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/README.md
+-rw-r--r--   0     1001      127     2766 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/accessibility.rs
+-rw-r--r--   0     1001      127    13996 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/animations.rs
+-rw-r--r--   0     1001      127    38608 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/api.rs
+-rw-r--r--   0     1001      127     5210 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/callbacks.rs
+-rw-r--r--   0     1001      127     2586 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/component_factory.rs
+-rw-r--r--   0     1001      127     2553 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/context.rs
+-rw-r--r--   0     1001      127     7694 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/future.rs
+-rw-r--r--   0     1001      127     2503 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/bitmapfont.rs
+-rw-r--r--   0     1001      127    14664 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/border_radius.rs
+-rw-r--r--   0     1001      127     4038 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/boxshadowcache.rs
+-rw-r--r--   0     1001      127    14919 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/brush.rs
+-rw-r--r--   0     1001      127    17436 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/color.rs
+-rw-r--r--   0     1001      127     7064 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/image/cache.rs
+-rw-r--r--   0     1001      127     2528 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/image/htmlimage.rs
+-rw-r--r--   0     1001      127     3408 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/image/svg.rs
+-rw-r--r--   0     1001      127    48855 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/image.rs
+-rw-r--r--   0     1001      127    15911 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/path.rs
+-rw-r--r--   0     1001      127     6978 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/rendering_metrics_collector.rs
+-rw-r--r--   0     1001      127     8021 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics.rs
+-rw-r--r--   0     1001      127    33891 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/input.rs
+-rw-r--r--   0     1001      127     8604 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/item_focus.rs
+-rw-r--r--   0     1001      127    29328 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/item_rendering.rs
+-rw-r--r--   0     1001      127    67985 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/item_tree.rs
+-rw-r--r--   0     1001      127     8608 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items/component_container.rs
+-rw-r--r--   0     1001      127    17039 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items/flickable.rs
+-rw-r--r--   0     1001      127     8722 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items/image.rs
+-rw-r--r--   0     1001      127     5377 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items/path.rs
+-rw-r--r--   0     1001      127    65770 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items/text.rs
+-rw-r--r--   0     1001      127    46631 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items.rs
+-rw-r--r--   0     1001      127    27945 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/layout.rs
+-rw-r--r--   0     1001      127     3222 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/lengths.rs
+-rw-r--r--   0     1001      127     2237 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/lib.rs
+-rw-r--r--   0     1001      127    47643 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/model/adapters.rs
+-rw-r--r--   0     1001      127     6658 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/model/model_peer.rs
+-rw-r--r--   0     1001      127    47290 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/model.rs
+-rw-r--r--   0     1001      127    15948 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/platform.rs
+-rw-r--r--   0     1001      127    15736 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/properties/ffi.rs
+-rw-r--r--   0     1001      127    38401 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/properties/properties_animations.rs
+-rw-r--r--   0     1001      127    58572 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/properties.rs
+-rw-r--r--   0     1001      127     5015 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/renderer.rs
+-rw-r--r--   0     1001      127    10886 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/rtti.rs
+-rw-r--r--   0     1001      127    21418 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/sharedvector.rs
+-rw-r--r--   0     1001      127     2865 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/slice.rs
+-rw-r--r--   0     1001      127    29158 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/draw_functions.rs
+-rw-r--r--   0     1001      127     3465 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/fixed.rs
+-rw-r--r--   0     1001      127     4673 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/fonts/pixelfont.rs
+-rw-r--r--   0     1001      127     3859 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/fonts/systemfonts.rs
+-rw-r--r--   0     1001      127     7334 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/fonts/vectorfont.rs
+-rw-r--r--   0     1001      127     5915 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/fonts.rs
+-rw-r--r--   0     1001      127    99070 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer.rs
+-rw-r--r--   0     1001      127    13307 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/string.rs
+-rw-r--r--   0     1001      127     4121 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/tests.rs
+-rw-r--r--   0     1001      127    12929 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/fragments.rs
+-rw-r--r--   0     1001      127     3222 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/glyphclusters.rs
+-rw-r--r--   0     1001      127     1234 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/linebreak_simple.rs
+-rw-r--r--   0     1001      127     1260 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/linebreak_unicode.rs
+-rw-r--r--   0     1001      127    15364 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/linebreaker.rs
+-rw-r--r--   0     1001      127    13512 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/shaping.rs
+-rw-r--r--   0     1001      127    24952 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout.rs
+-rw-r--r--   0     1001      127    31468 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/timers.rs
+-rw-r--r--   0     1001      127     8559 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/translations.rs
+-rw-r--r--   0     1001      127     1884 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/unsafe_single_threaded.rs
+-rw-r--r--   0     1001      127    62402 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/window.rs
+-rw-r--r--   0     1001      127     1913 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/Cargo.toml
+-rw-r--r--   0     1001      127    10280 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127    16830 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/CC-BY-ND-4.0.txt
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      537 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/README.md
+-rw-r--r--   0     1001      127     2420 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/build.rs
+-rw-r--r--   0     1001      127    16358 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/builtin_macros.rs
+-rw-r--r--   0     1001      127    18381 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/builtins.slint
+-rw-r--r--   0     1001      127    19587 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/diagnostics.rs
+-rw-r--r--   0     1001      127     2636 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/embedded_resources.rs
+-rw-r--r--   0     1001      127    69622 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/expression_tree.rs
+-rw-r--r--   0     1001      127     4420 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/fileaccess.rs
+-rw-r--r--   0     1001      127   139818 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/generator/cpp.rs
+-rw-r--r--   0     1001      127   122025 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/generator/rust.rs
+-rw-r--r--   0     1001      127    19509 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/generator.rs
+-rw-r--r--   0     1001      127    32752 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/langtype.rs
+-rw-r--r--   0     1001      127    21425 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/layout.rs
+-rw-r--r--   0     1001      127    15374 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/lexer.rs
+-rw-r--r--   0     1001      127     9399 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/lib.rs
+-rw-r--r--   0     1001      127     7020 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/literals.rs
+-rw-r--r--   0     1001      127    31386 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/expression.rs
+-rw-r--r--   0     1001      127    13363 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/item_tree.rs
+-rw-r--r--   0     1001      127    40541 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/lower_expression.rs
+-rw-r--r--   0     1001      127    31339 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/lower_to_item_tree.rs
+-rw-r--r--   0     1001      127     6314 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/optim_passes/count_property_use.rs
+-rw-r--r--   0     1001      127     6235 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/optim_passes/inline_expressions.rs
+-rw-r--r--   0     1001      127    11380 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/pretty_print.rs
+-rw-r--r--   0     1001      127      654 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr.rs
+-rw-r--r--   0     1001      127    11758 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/load_builtins.rs
+-rw-r--r--   0     1001      127    39783 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/lookup.rs
+-rw-r--r--   0     1001      127     7518 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/namedreference.rs
+-rw-r--r--   0     1001      127   101372 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/object_tree.rs
+-rw-r--r--   0     1001      127    10913 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser/document.rs
+-rw-r--r--   0     1001      127    20594 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser/element.rs
+-rw-r--r--   0     1001      127    14696 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser/expressions.rs
+-rw-r--r--   0     1001      127     3102 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser/statements.rs
+-rw-r--r--   0     1001      127     4561 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser/type.rs
+-rw-r--r--   0     1001      127    36188 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser.rs
+-rw-r--r--   0     1001      127     3949 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/apply_default_properties_from_style.rs
+-rw-r--r--   0     1001      127    22379 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/binding_analysis.rs
+-rw-r--r--   0     1001      127     1587 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/border_radius.rs
+-rw-r--r--   0     1001      127     1793 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/check_expressions.rs
+-rw-r--r--   0     1001      127     1941 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/check_public_api.rs
+-rw-r--r--   0     1001      127     2309 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/check_rotation.rs
+-rw-r--r--   0     1001      127     4580 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/clip.rs
+-rw-r--r--   0     1001      127     2464 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/collect_custom_fonts.rs
+-rw-r--r--   0     1001      127     1933 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/collect_globals.rs
+-rw-r--r--   0     1001      127     1150 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/collect_init_code.rs
+-rw-r--r--   0     1001      127     4172 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/collect_structs_and_enums.rs
+-rw-r--r--   0     1001      127     1392 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/collect_subcomponents.rs
+-rw-r--r--   0     1001      127     8043 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/compile_paths.rs
+-rw-r--r--   0     1001      127     9466 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/const_propagation.rs
+-rw-r--r--   0     1001      127     6155 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/deduplicate_property_read.rs
+-rw-r--r--   0     1001      127    18877 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/default_geometry.rs
+-rw-r--r--   0     1001      127    16260 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/embed_glyphs.rs
+-rw-r--r--   0     1001      127    14883 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/embed_images.rs
+-rw-r--r--   0     1001      127     5111 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/ensure_window.rs
+-rw-r--r--   0     1001      127     6270 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/flickable.rs
+-rw-r--r--   0     1001      127    10032 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/focus_handling.rs
+-rw-r--r--   0     1001      127     4318 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/generate_item_indices.rs
+-rw-r--r--   0     1001      127     6709 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/infer_aliases_types.rs
+-rw-r--r--   0     1001      127    21709 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/inlining.rs
+-rw-r--r--   0     1001      127     3241 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_absolute_coordinates.rs
+-rw-r--r--   0     1001      127     3268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_accessibility.rs
+-rw-r--r--   0     1001      127     1697 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_component_container.rs
+-rw-r--r--   0     1001      127    31672 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_layout.rs
+-rw-r--r--   0     1001      127     5565 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_popups.rs
+-rw-r--r--   0     1001      127     5182 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_property_to_element.rs
+-rw-r--r--   0     1001      127     6916 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_shadows.rs
+-rw-r--r--   0     1001      127     9988 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_states.rs
+-rw-r--r--   0     1001      127     8355 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_tabwidget.rs
+-rw-r--r--   0     1001      127     2000 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_text_input_interface.rs
+-rw-r--r--   0     1001      127     6185 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/materialize_fake_properties.rs
+-rw-r--r--   0     1001      127     6748 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/move_declarations.rs
+-rw-r--r--   0     1001      127     2749 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/optimize_useless_rectangles.rs
+-rw-r--r--   0     1001      127     4231 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/purity_check.rs
+-rw-r--r--   0     1001      127     9197 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/remove_aliases.rs
+-rw-r--r--   0     1001      127    19427 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/remove_return.rs
+-rw-r--r--   0     1001      127     1656 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/remove_unused_properties.rs
+-rw-r--r--   0     1001      127     5067 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/repeater_component.rs
+-rw-r--r--   0     1001      127     5620 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/resolve_native_classes.rs
+-rw-r--r--   0     1001      127    70883 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/resolving.rs
+-rw-r--r--   0     1001      127     3046 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/unique_id.rs
+-rw-r--r--   0     1001      127     4210 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/visible.rs
+-rw-r--r--   0     1001      127     2961 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/z_order.rs
+-rw-r--r--   0     1001      127    10533 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes.rs
+-rw-r--r--   0     1001      127    18378 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/pathutils.rs
+-rw-r--r--   0     1001      127     8412 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/consistent_styles.rs
+-rw-r--r--   0     1001      127     1237 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/accessibility/accessible_properties.slint
+-rw-r--r--   0     1001      127     1774 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop1.slint
+-rw-r--r--   0     1001      127     1826 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop2.slint
+-rw-r--r--   0     1001      127      924 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_function.slint
+-rw-r--r--   0     1001      127      643 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint
+-rw-r--r--   0     1001      127     2458 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint
+-rw-r--r--   0     1001      127     1854 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint
+-rw-r--r--   0     1001      127     1144 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint
+-rw-r--r--   0     1001      127     2120 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint
+-rw-r--r--   0     1001      127      488 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_mappointtowindow.slint
+-rw-r--r--   0     1001      127      923 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_self.slint
+-rw-r--r--   0     1001      127      942 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/animate.slint
+-rw-r--r--   0     1001      127      230 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/array.slint
+-rw-r--r--   0     1001      127      788 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/assign.slint
+-rw-r--r--   0     1001      127      585 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/box_shadow.slint
+-rw-r--r--   0     1001      127     1021 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/children_placeholder.slint
+-rw-r--r--   0     1001      127      301 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/children_placeholder_2.slint
+-rw-r--r--   0     1001      127      663 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/clip.slint
+-rw-r--r--   0     1001      127      492 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/comments.slint
+-rw-r--r--   0     1001      127     2078 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/dialog.slint
+-rw-r--r--   0     1001      127      631 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/dialog2.slint
+-rw-r--r--   0     1001      127      499 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/double_binding.slint
+-rw-r--r--   0     1001      127      270 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/double_color.slint
+-rw-r--r--   0     1001      127     1137 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/duplicated_id.slint
+-rw-r--r--   0     1001      127     1340 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/easing.slint
+-rw-r--r--   0     1001      127      383 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/easing_not_called.slint
+-rw-r--r--   0     1001      127      156 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/empty.slint
+-rw-r--r--   0     1001      127      526 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/enums.slint
+-rw-r--r--   0     1001      127      441 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/for.slint
+-rw-r--r--   0     1001      127      492 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/image.slint
+-rw-r--r--   0     1001      127      450 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/inline_component.slint
+-rw-r--r--   0     1001      127      895 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/item_as_property.slint
+-rw-r--r--   0     1001      127      465 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/layout.slint
+-rw-r--r--   0     1001      127     1958 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/layout2.slint
+-rw-r--r--   0     1001      127     2188 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/linear-gradient.slint
+-rw-r--r--   0     1001      127      470 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/object_in_binding.slint
+-rw-r--r--   0     1001      127      538 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/opacity.slint
+-rw-r--r--   0     1001      127      905 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/parse_error.slint
+-rw-r--r--   0     1001      127      535 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/path.slint
+-rw-r--r--   0     1001      127     1114 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/path_commands.slint
+-rw-r--r--   0     1001      127      541 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/path_for.slint
+-rw-r--r--   0     1001      127     1056 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/percent.slint
+-rw-r--r--   0     1001      127      707 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/popup.slint
+-rw-r--r--   0     1001      127      333 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/property_animation.slint
+-rw-r--r--   0     1001      127      983 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/property_declaration.slint
+-rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/property_declaration_in_component.slint
+-rw-r--r--   0     1001      127     1786 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/radial-gradient.slint
+-rw-r--r--   0     1001      127      837 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/return.slint
+-rw-r--r--   0     1001      127     1850 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/rotation.slint
+-rw-r--r--   0     1001      127      456 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/rust-attr.slint
+-rw-r--r--   0     1001      127     1781 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/self_assign.slint
+-rw-r--r--   0     1001      127     1413 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/signal.slint
+-rw-r--r--   0     1001      127     4436 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions.slint
+-rw-r--r--   0     1001      127      711 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions2.slint
+-rw-r--r--   0     1001      127      748 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions3.slint
+-rw-r--r--   0     1001      127      731 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_two_way.slint
+-rw-r--r--   0     1001      127      731 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/sub_elements.slint
+-rw-r--r--   0     1001      127      218 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/supersimple.slint
+-rw-r--r--   0     1001      127      467 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/svg_path.slint
+-rw-r--r--   0     1001      127     1600 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/tr.slint
+-rw-r--r--   0     1001      127     3038 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/tr2.slint
+-rw-r--r--   0     1001      127     1108 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/type_declaration.slint
+-rw-r--r--   0     1001      127     1391 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/unknown_item.slint
+-rw-r--r--   0     1001      127      457 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/callbacks/init.slint
+-rw-r--r--   0     1001      127      671 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/component_container.slint
+-rw-r--r--   0     1001      127     1202 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/listview.slint
+-rw-r--r--   0     1001      127      601 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/popup.slint
+-rw-r--r--   0     1001      127      538 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/tabwidget.slint
+-rw-r--r--   0     1001      127      898 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/tabwidget2.slint
+-rw-r--r--   0     1001      127      474 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/tabwidget3.slint
+-rw-r--r--   0     1001      127      436 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/export_duplicates.slint
+-rw-r--r--   0     1001      127      623 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/reexport_duplicate.slint
+-rw-r--r--   0     1001      127      326 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/root_compo_export.slint
+-rw-r--r--   0     1001      127      289 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/root_compo_export2.slint
+-rw-r--r--   0     1001      127      332 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/single_global_missing_export.slint
+-rw-r--r--   0     1001      127      288 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/unused_compo.slint
+-rw-r--r--   0     1001      127     1464 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/arithmetic_op.slint
+-rw-r--r--   0     1001      127     1261 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/clamp.slint
+-rw-r--r--   0     1001      127      999 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/comparison_operator.slint
+-rw-r--r--   0     1001      127     1473 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/condition_operator.slint
+-rw-r--r--   0     1001      127     3442 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/image-url.slint
+-rw-r--r--   0     1001      127     1090 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/image-url2.slint
+-rw-r--r--   0     1001      127     1355 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/minmax.slint
+-rw-r--r--   0     1001      127      654 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/percent2.slint
+-rw-r--r--   0     1001      127      456 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/strings.slint
+-rw-r--r--   0     1001      127     1221 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/unary_op.slint
+-rw-r--r--   0     1001      127      387 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/focus/focus_invalid.slint
+-rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/focus/focus_not_called.slint
+-rw-r--r--   0     1001      127      595 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/focus/focus_wrong_args.slint
+-rw-r--r--   0     1001      127     1707 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint
+-rw-r--r--   0     1001      127      592 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/functions/function_double_qualified.slint
+-rw-r--r--   0     1001      127     1814 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions.slint
+-rw-r--r--   0     1001      127     2990 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions_call.slint
+-rw-r--r--   0     1001      127     3353 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions_purity.slint
+-rw-r--r--   0     1001      127      597 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/bug_2719.slint
+-rw-r--r--   0     1001      127     1018 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint
+-rw-r--r--   0     1001      127      407 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/cyclic_import.slint
+-rw-r--r--   0     1001      127      441 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/error_in_import.slint
+-rw-r--r--   0     1001      127      252 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/error_in_import2.slint
+-rw-r--r--   0     1001      127      295 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/error_in_import3.slint
+-rw-r--r--   0     1001      127      410 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/font.slint
+-rw-r--r--   0     1001      127      393 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_builtin.slint
+-rw-r--r--   0     1001      127      411 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_error2.slint
+-rw-r--r--   0     1001      127      944 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_errors.slint
+-rw-r--r--   0     1001      127      207 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_parse_error1.slint
+-rw-r--r--   0     1001      127      221 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_parse_error2.slint
+-rw-r--r--   0     1001      127      238 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_parse_error3.slint
+-rw-r--r--   0     1001      127      239 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_parse_error4.slint
+-rw-r--r--   0     1001      127      503 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_parse_error5.slint
+-rw-r--r--   0     1001      127      472 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/invalid_export.slint
+-rw-r--r--   0     1001      127      379 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/visibility_errors.slint
+-rw-r--r--   0     1001      127      703 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/layout/if_in_grid.slint
+-rw-r--r--   0     1001      127      441 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/layout/if_in_grid_row.slint
+-rw-r--r--   0     1001      127      586 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/layout/min_max_conflict.slint
+-rw-r--r--   0     1001      127      655 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/layout/spacing.slint
+-rw-r--r--   0     1001      127      477 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/absolute-position.slint
+-rw-r--r--   0     1001      127      691 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/array_index.slint
+-rw-r--r--   0     1001      127      594 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias.slint
+-rw-r--r--   0     1001      127      641 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias2.slint
+-rw-r--r--   0     1001      127     1087 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias3.slint
+-rw-r--r--   0     1001      127      255 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias_issue4938.slint
+-rw-r--r--   0     1001      127      376 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_not_called.slint
+-rw-r--r--   0     1001      127      433 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_return.slint
+-rw-r--r--   0     1001      127     1814 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/color.slint
+-rw-r--r--   0     1001      127     3112 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/conversion.slint
+-rw-r--r--   0     1001      127     1807 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/dashes.slint
+-rw-r--r--   0     1001      127     1250 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/deprecated_property.slint
+-rw-r--r--   0     1001      127     1138 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/enum.slint
+-rw-r--r--   0     1001      127     2598 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/for_lookup.slint
+-rw-r--r--   0     1001      127     1211 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/global.slint
+-rw-r--r--   0     1001      127      621 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/if.slint
+-rw-r--r--   0     1001      127      920 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/issue_1461.slint
+-rw-r--r--   0     1001      127     1287 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/property.slint
+-rw-r--r--   0     1001      127     1704 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint
+-rw-r--r--   0     1001      127     1439 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/signal_arg.slint
+-rw-r--r--   0     1001      127     1444 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/two_way_binding.slint
+-rw-r--r--   0     1001      127     1220 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint
+-rw-r--r--   0     1001      127      392 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/two_way_binding_model.slint
+-rw-r--r--   0     1001      127      903 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint
+-rw-r--r--   0     1001      127     2695 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/input_output.slint
+-rw-r--r--   0     1001      127     3062 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/input_output2.slint
+-rw-r--r--   0     1001      127      593 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/new_component.slint
+-rw-r--r--   0     1001      127     1020 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/new_lookup.slint
+-rw-r--r--   0     1001      127     8651 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint
+-rw-r--r--   0     1001      127      252 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/children_placeholder0.slint
+-rw-r--r--   0     1001      127      263 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/export0.slint
+-rw-r--r--   0     1001      127      219 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/export1.slint
+-rw-r--r--   0     1001      127      362 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/if0.slint
+-rw-r--r--   0     1001      127      278 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/if1.slint
+-rw-r--r--   0     1001      127      285 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/if2.slint
+-rw-r--r--   0     1001      127      224 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/if3.slint
+-rw-r--r--   0     1001      127      361 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/if4.slint
+-rw-r--r--   0     1001      127      398 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/property1.slint
+-rw-r--r--   0     1001      127      902 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/property2.slint
+-rw-r--r--   0     1001      127      846 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/state1.slint
+-rw-r--r--   0     1001      127      244 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/state2.slint
+-rw-r--r--   0     1001      127      307 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/state3.slint
+-rw-r--r--   0     1001      127      707 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/struct.slint
+-rw-r--r--   0     1001      127     9426 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax_tests.rs
+-rw-r--r--   0     1001      127      156 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/custom_style/TestStyle/std-widgets.slint
+-rw-r--r--   0     1001      127      278 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/dependency_local.slint
+-rw-r--r--   0     1001      127      393 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/dependency_test_main.slint
+-rw-r--r--   0     1001      127      503 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/bug_2719_import.slint
+-rw-r--r--   0     1001      127      461 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/bug_3674_alias_from_invalid_import.slint
+-rw-r--r--   0     1001      127      262 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/dependency_from_incpath.slint
+-rw-r--r--   0     1001      127      205 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/local_helper_type.slint
+-rw-r--r--   0     1001      127      237 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/should_fail.slint
+-rw-r--r--   0     1001      127      320 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/should_fail2.slint
+-rw-r--r--   0     1001      127      280 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/should_fail3.slint
+-rw-r--r--   0     1001      127      491 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/should_fail4.slint
+-rw-r--r--   0     1001      127      208 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/library/dependency_from_library.slint
+-rw-r--r--   0     1001      127      243 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/library/lib.slint
+-rw-r--r--   0     1001      127      214 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/library/library_helper_type.slint
+-rw-r--r--   0     1001      127      324 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/recursive_import1.slint
+-rw-r--r--   0     1001      127      395 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/recursive_import2.slint
+-rw-r--r--   0     1001      127      450 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/some_rust_file.rs
+-rw-r--r--   0     1001      127    43496 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/typeloader.rs
+-rw-r--r--   0     1001      127    19576 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/typeregister.rs
+-rw-r--r--   0     1001      127    14083 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg
+-rw-r--r--   0     1001      127    14073 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg
+-rw-r--r--   0     1001      127     2358 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/combobox-base.slint
+-rw-r--r--   0     1001      127     3861 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/common.slint
+-rw-r--r--   0     1001      127     3184 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/lineedit-base.slint
+-rw-r--r--   0     1001      127     4288 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/listview.slint
+-rw-r--r--   0     1001      127     3920 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/slider-base.slint
+-rw-r--r--   0     1001      127     2418 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/spinbox-base.slint
+-rw-r--r--   0     1001      127     2510 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/spinner-base.slint
+-rw-r--r--   0     1001      127     1202 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/standardbutton.slint
+-rw-r--r--   0     1001      127     1080 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/tabwidget-base.slint
+-rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic/std-widgets.slint
+-rw-r--r--   0     1001      127      308 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/_arrow_down.svg
+-rw-r--r--   0     1001      127      284 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/_arrow_up.svg
+-rw-r--r--   0     1001      127      413 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/_check-mark.svg
+-rw-r--r--   0     1001      127      148 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/_pane_down.svg
+-rw-r--r--   0     1001      127     2710 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/button.slint
+-rw-r--r--   0     1001      127     2726 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/checkbox.slint
+-rw-r--r--   0     1001      127     3057 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/combobox.slint
+-rw-r--r--   0     1001      127     4437 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/components.slint
+-rw-r--r--   0     1001      127     1000 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/groupbox.slint
+-rw-r--r--   0     1001      127      632 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/layouts.slint
+-rw-r--r--   0     1001      127     2886 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/lineedit.slint
+-rw-r--r--   0     1001      127      988 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/progressindicator.slint
+-rw-r--r--   0     1001      127     5065 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/scrollview.slint
+-rw-r--r--   0     1001      127     2930 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/slider.slint
+-rw-r--r--   0     1001      127     3327 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/spinbox.slint
+-rw-r--r--   0     1001      127      733 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/spinner.slint
+-rw-r--r--   0     1001      127     1524 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2126 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     3420 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/styling.slint
+-rw-r--r--   0     1001      127     2861 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/switch.slint
+-rw-r--r--   0     1001      127     9124 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/tableview.slint
+-rw-r--r--   0     1001      127     6075 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/tabwidget.slint
+-rw-r--r--   0     1001      127     4438 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/textedit.slint
+-rw-r--r--   0     1001      127      257 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-light/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-light/std-widgets.slint
+-rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino/color-scheme.slint
+-rw-r--r--   0     1001      127      332 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      215 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino/std-widgets.slint
+-rw-r--r--   0     1001      127      513 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_arrow-down.svg
+-rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_arrow-up.svg
+-rw-r--r--   0     1001      127      780 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_check-mark.svg
+-rw-r--r--   0     1001      127      623 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_chevron-down.svg
+-rw-r--r--   0     1001      127      601 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_chevron-up.svg
+-rw-r--r--   0     1001      127      918 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_down.svg
+-rw-r--r--   0     1001      127      489 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_dropdown.svg
+-rw-r--r--   0     1001      127      849 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_left.svg
+-rw-r--r--   0     1001      127      815 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_right.svg
+-rw-r--r--   0     1001      127     1135 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_up.svg
+-rw-r--r--   0     1001      127     5134 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/button.slint
+-rw-r--r--   0     1001      127     4547 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/checkbox.slint
+-rw-r--r--   0     1001      127     5646 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/combobox.slint
+-rw-r--r--   0     1001      127     3145 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/components.slint
+-rw-r--r--   0     1001      127     1103 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/groupbox.slint
+-rw-r--r--   0     1001      127      632 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/layouts.slint
+-rw-r--r--   0     1001      127     3180 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/lineedit.slint
+-rw-r--r--   0     1001      127     1404 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/progressindicator.slint
+-rw-r--r--   0     1001      127     5563 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/scrollview.slint
+-rw-r--r--   0     1001      127     3097 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/slider.slint
+-rw-r--r--   0     1001      127     5483 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/spinbox.slint
+-rw-r--r--   0     1001      127      739 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/spinner.slint
+-rw-r--r--   0     1001      127     1524 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2216 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     4541 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/styling.slint
+-rw-r--r--   0     1001      127     4097 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/switch.slint
+-rw-r--r--   0     1001      127     8959 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/tableview.slint
+-rw-r--r--   0     1001      127     5493 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/tabwidget.slint
+-rw-r--r--   0     1001      127     6640 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/textedit.slint
+-rw-r--r--   0     1001      127      257 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      332 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      215 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-light/color-scheme.slint
+-rw-r--r--   0     1001      127      332 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      215 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-light/std-widgets.slint
+-rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent/std-widgets.slint
+-rw-r--r--   0     1001      127      513 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_arrow-down.svg
+-rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_arrow-up.svg
+-rw-r--r--   0     1001      127      780 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_check-mark.svg
+-rw-r--r--   0     1001      127      623 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_chevron-down.svg
+-rw-r--r--   0     1001      127      601 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_chevron-up.svg
+-rw-r--r--   0     1001      127      918 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_down.svg
+-rw-r--r--   0     1001      127      489 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_dropdown.svg
+-rw-r--r--   0     1001      127      849 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_left.svg
+-rw-r--r--   0     1001      127      815 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_right.svg
+-rw-r--r--   0     1001      127     1135 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_up.svg
+-rw-r--r--   0     1001      127     4556 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/button.slint
+-rw-r--r--   0     1001      127     3883 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/checkbox.slint
+-rw-r--r--   0     1001      127     3773 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/combobox.slint
+-rw-r--r--   0     1001      127     3363 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/components.slint
+-rw-r--r--   0     1001      127      877 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/groupbox.slint
+-rw-r--r--   0     1001      127      632 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/layouts.slint
+-rw-r--r--   0     1001      127     3499 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/lineedit.slint
+-rw-r--r--   0     1001      127     1023 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/progressindicator.slint
+-rw-r--r--   0     1001      127     6590 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/scrollview.slint
+-rw-r--r--   0     1001      127     3734 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/slider.slint
+-rw-r--r--   0     1001      127     3992 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/spinbox.slint
+-rw-r--r--   0     1001      127      733 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/spinner.slint
+-rw-r--r--   0     1001      127     1524 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2126 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     6248 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/styling.slint
+-rw-r--r--   0     1001      127     4616 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/switch.slint
+-rw-r--r--   0     1001      127     9561 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/tableview.slint
+-rw-r--r--   0     1001      127     5493 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/tabwidget.slint
+-rw-r--r--   0     1001      127     4935 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/textedit.slint
+-rw-r--r--   0     1001      127      257 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-light/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-light/std-widgets.slint
+-rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material/color-scheme.slint
+-rw-r--r--   0     1001      127      347 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      214 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material/std-widgets.slint
+-rw-r--r--   0     1001      127      163 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_arrow-downward.svg
+-rw-r--r--   0     1001      127      115 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_arrow-drop-down.svg
+-rw-r--r--   0     1001      127      115 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_arrow-drop-up.svg
+-rw-r--r--   0     1001      127      161 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_arrow-upward.svg
+-rw-r--r--   0     1001      127      150 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_check-mark.svg
+-rw-r--r--   0     1001      127      145 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_expand-more.svg
+-rw-r--r--   0     1001      127     3239 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/button.slint
+-rw-r--r--   0     1001      127     5664 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/checkbox.slint
+-rw-r--r--   0     1001      127     3452 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/combobox.slint
+-rw-r--r--   0     1001      127     4712 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/components.slint
+-rw-r--r--   0     1001      127     1477 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/groupbox.slint
+-rw-r--r--   0     1001      127      633 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/layouts.slint
+-rw-r--r--   0     1001      127     2866 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/lineedit.slint
+-rw-r--r--   0     1001      127     1010 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/progressindicator.slint
+-rw-r--r--   0     1001      127     5014 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/scrollview.slint
+-rw-r--r--   0     1001      127     4146 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/slider.slint
+-rw-r--r--   0     1001      127     5090 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/spinbox.slint
+-rw-r--r--   0     1001      127      737 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/spinner.slint
+-rw-r--r--   0     1001      127     1373 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2213 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     3651 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/styling.slint
+-rw-r--r--   0     1001      127     6174 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/switch.slint
+-rw-r--r--   0     1001      127     8186 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/tableview.slint
+-rw-r--r--   0     1001      127     4886 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/tabwidget.slint
+-rw-r--r--   0     1001      127      257 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      331 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      214 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-light/color-scheme.slint
+-rw-r--r--   0     1001      127      331 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      214 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-light/std-widgets.slint
+-rw-r--r--   0     1001      127     1642 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/button.slint
+-rw-r--r--   0     1001      127      350 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/checkbox.slint
+-rw-r--r--   0     1001      127     1707 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/combobox.slint
+-rw-r--r--   0     1001      127      582 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/groupbox.slint
+-rw-r--r--   0     1001      127     2384 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/internal-scrollview.slint
+-rw-r--r--   0     1001      127      613 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/layouts.slint
+-rw-r--r--   0     1001      127     2377 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/lineedit.slint
+-rw-r--r--   0     1001      127      307 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/progressindicator.slint
+-rw-r--r--   0     1001      127     1026 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/scrollview.slint
+-rw-r--r--   0     1001      127      422 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/slider.slint
+-rw-r--r--   0     1001      127      834 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/spinbox.slint
+-rw-r--r--   0     1001      127     1265 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/spinner.slint
+-rw-r--r--   0     1001      127      374 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     1475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/std-widgets.slint
+-rw-r--r--   0     1001      127      346 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/switch.slint
+-rw-r--r--   0     1001      127     5310 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/tableview.slint
+-rw-r--r--   0     1001      127     1564 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/tabwidget.slint
+-rw-r--r--   0     1001      127     2855 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/README.md
+-rw-r--r--   0     1001      127      673 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/build.rs
+-rw-r--r--   0     1001      127     6875 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/cached_image.rs
+-rw-r--r--   0     1001      127    14877 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/d3d_surface.rs
+-rw-r--r--   0     1001      127    34690 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/itemrenderer.rs
+-rw-r--r--   0     1001      127    23253 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/lib.rs
+-rw-r--r--   0     1001      127     6372 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/metal_surface.rs
+-rw-r--r--   0     1001      127    15370 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/opengl_surface.rs
+-rw-r--r--   0     1001      127     4611 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/software_surface.rs
+-rw-r--r--   0     1001      127    11843 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/textlayout.rs
+-rw-r--r--   0     1001      127    17420 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/vulkan_surface.rs
+-rw-r--r--   0     1001      127     9884 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127     1881 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/README.md
+-rw-r--r--   0     1001      127     5140 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/android.rs
+-rw-r--r--   0     1001      127      548 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/compile_fail_tests.rs
+-rw-r--r--   0     1001      127     9447 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/building.md
+-rw-r--r--   0     1001      127     7147 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/development.md
+-rw-r--r--   0     1001      127     2881 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/install_qt.md
+-rw-r--r--   0     1001      127        5 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/.gitignore
+-rw-r--r--   0     1001      127     1013 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/README.md
+-rw-r--r--   0     1001      127      261 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/book.toml
+-rw-r--r--   0     1001      127      810 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt
+-rw-r--r--   0     1001      127      515 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md
+-rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/appwindow.slint
+-rw-r--r--   0     1001      127     1216 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/conclusion.md
+-rw-r--r--   0     1001      127     1337 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md
+-rw-r--r--   0     1001      127     2039 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md
+-rw-r--r--   0     1001      127     2483 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md
+-rw-r--r--   0     1001      127     2126 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/getting_started.md
+-rw-r--r--   0     1001      127      477 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/README.md
+-rw-r--r--   0     1001      127     1122 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg
+-rw-r--r--   0     1001      127     3210 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/at.png
+-rw-r--r--   0     1001      127      971 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg
+-rw-r--r--   0     1001      127     2265 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png
+-rw-r--r--   0     1001      127     1577 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg
+-rw-r--r--   0     1001      127     2613 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png
+-rw-r--r--   0     1001      127      837 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg
+-rw-r--r--   0     1001      127     1540 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png
+-rw-r--r--   0     1001      127      485 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cloud-solid.svg
+-rw-r--r--   0     1001      127     1454 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png
+-rw-r--r--   0     1001      127     2614 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg
+-rw-r--r--   0     1001      127     2894 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png
+-rw-r--r--   0     1001      127     1252 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg
+-rw-r--r--   0     1001      127     2497 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png
+-rw-r--r--   0     1001      127     6059 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png
+-rw-r--r--   0     1001      127      467 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/video-solid.svg
+-rw-r--r--   0     1001      127     1073 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/video.png
+-rw-r--r--   0     1001      127     1060 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md
+-rw-r--r--   0     1001      127      953 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/introduction.md
+-rw-r--r--   0     1001      127     2800 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp
+-rw-r--r--   0     1001      127      300 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/main_initial.cpp
+-rw-r--r--   0     1001      127      877 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp
+-rw-r--r--   0     1001      127     2620 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint
+-rw-r--r--   0     1001      127     2130 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md
+-rw-r--r--   0     1001      127      425 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_tile.slint
+-rw-r--r--   0     1001      127     2205 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint
+-rw-r--r--   0     1001      127     2760 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md
+-rw-r--r--   0     1001      127      262 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/book.toml
+-rw-r--r--   0     1001      127      527 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/SUMMARY.md
+-rw-r--r--   0     1001      127     1223 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/conclusion.md
+-rw-r--r--   0     1001      127     1191 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md
+-rw-r--r--   0     1001      127     2034 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md
+-rw-r--r--   0     1001      127     2031 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md
+-rw-r--r--   0     1001      127     1515 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/getting_started.md
+-rw-r--r--   0     1001      127      477 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/README.md
+-rw-r--r--   0     1001      127     1122 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg
+-rw-r--r--   0     1001      127     3210 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/at.png
+-rw-r--r--   0     1001      127      971 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg
+-rw-r--r--   0     1001      127     2265 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png
+-rw-r--r--   0     1001      127     1577 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg
+-rw-r--r--   0     1001      127     2613 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png
+-rw-r--r--   0     1001      127      837 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg
+-rw-r--r--   0     1001      127     1540 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bus.png
+-rw-r--r--   0     1001      127      485 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cloud-solid.svg
+-rw-r--r--   0     1001      127     1454 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cloud.png
+-rw-r--r--   0     1001      127     2614 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg
+-rw-r--r--   0     1001      127     2894 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cogs.png
+-rw-r--r--   0     1001      127     1252 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg
+-rw-r--r--   0     1001      127     2497 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png
+-rw-r--r--   0     1001      127     6059 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png
+-rw-r--r--   0     1001      127      467 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/video-solid.svg
+-rw-r--r--   0     1001      127     1073 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/video.png
+-rw-r--r--   0     1001      127     1060 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md
+-rw-r--r--   0     1001      127      960 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/introduction.md
+-rw-r--r--   0     1001      127     1797 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/main_game_logic.js
+-rw-r--r--   0     1001      127      275 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/main_initial.js
+-rw-r--r--   0     1001      127      631 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js
+-rw-r--r--   0     1001      127      265 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory.slint
+-rw-r--r--   0     1001      127     2620 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint
+-rw-r--r--   0     1001      127     2079 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_tile.md
+-rw-r--r--   0     1001      127      425 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_tile.slint
+-rw-r--r--   0     1001      127     2205 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint
+-rw-r--r--   0     1001      127      202 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/package.json
+-rw-r--r--   0     1001      127     2747 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md
+-rw-r--r--   0     1001      127      262 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/rust/book.toml
+-rw-r--r--   0     1001      127     3821 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/theme/head.hbs
+-rw-r--r--   0     1001      127       84 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/theme/highlight.css
+-rw-r--r--   0     1001      127      282 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/theme/highlight.js
+-rw-r--r--   0     1001      127      386 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/Pipfile
+-rw-r--r--   0     1001      127      256 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/_static/theme_tweak.css
+-rw-r--r--   0     1001      127      190 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/_templates/base.html
+-rw-r--r--   0     1001      127     4339 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/conf.py
+-rw-r--r--   0     1001      127      811 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/index.rst
+-rw-r--r--   0     1001      127     7746 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md
+-rw-r--r--   0     1001      127     1061 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_qt.md
+-rw-r--r--   0     1001      127     1692 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_winit.md
+-rw-r--r--   0     1001      127     7399 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md
+-rw-r--r--   0     1001      127     6034 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md
+-rw-r--r--   0     1001      127     3816 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/style.md
+-rw-r--r--   0     1001      127     1095 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/introduction/index.md
+-rw-r--r--   0     1001      127     2287 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/introduction/supported_platforms.md
+-rw-r--r--   0     1001      127     1418 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/callbacks.md
+-rw-r--r--   0     1001      127    40679 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/elements.md
+-rw-r--r--   0     1001      127      975 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/functions.md
+-rw-r--r--   0     1001      127     3227 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/globals.md
+-rw-r--r--   0     1001      127      267 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/index.rst
+-rw-r--r--   0     1001      127     3567 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/namespaces.md
+-rw-r--r--   0     1001      127     1144 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/container.md
+-rw-r--r--   0     1001      127     2165 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/file.md
+-rw-r--r--   0     1001      127     1591 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/focus.md
+-rw-r--r--   0     1001      127     1232 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/fonts.md
+-rw-r--r--   0     1001      127      262 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/index.rst
+-rw-r--r--   0     1001      127    13939 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/layouting.md
+-rw-r--r--   0     1001      127     1787 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/purity.md
+-rw-r--r--   0     1001      127     7822 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/translations.md
+-rw-r--r--   0     1001      127     2235 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/index.rst
+-rw-r--r--   0     1001      127     2270 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/animations.md
+-rw-r--r--   0     1001      127     1627 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/callbacks.md
+-rw-r--r--   0     1001      127      326 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/comments.md
+-rw-r--r--   0     1001      127      492 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/conditions.md
+-rw-r--r--   0     1001      127     1792 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/expressions.md
+-rw-r--r--   0     1001      127     1821 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/functions.md
+-rw-r--r--   0     1001      127     2776 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/globals.md
+-rw-r--r--   0     1001      127      413 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/identifiers.md
+-rw-r--r--   0     1001      127      402 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/index.rst
+-rw-r--r--   0     1001      127      851 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md
+-rw-r--r--   0     1001      127     3946 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/modules.md
+-rw-r--r--   0     1001      127     5168 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/properties.md
+-rw-r--r--   0     1001      127     1470 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/repetitions.md
+-rw-r--r--   0     1001      127      658 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/statements.md
+-rw-r--r--   0     1001      127     2210 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/states.md
+-rw-r--r--   0     1001      127    17651 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/types.md
+-rw-r--r--   0     1001      127      299 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/aboutslint.md
+-rw-r--r--   0     1001      127     1469 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/button.md
+-rw-r--r--   0     1001      127     1035 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/checkbox.md
+-rw-r--r--   0     1001      127     1087 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/combobox.md
+-rw-r--r--   0     1001      127      251 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/gridbox.md
+-rw-r--r--   0     1001      127      741 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/groupbox.md
+-rw-r--r--   0     1001      127      337 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/horizontalbox.md
+-rw-r--r--   0     1001      127      569 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/index.rst
+-rw-r--r--   0     1001      127     2305 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/lineedit.md
+-rw-r--r--   0     1001      127     1293 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/listview.md
+-rw-r--r--   0     1001      127      801 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md
+-rw-r--r--   0     1001      127     1976 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/scrollview.md
+-rw-r--r--   0     1001      127     1120 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/slider.md
+-rw-r--r--   0     1001      127      841 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/spinbox.md
+-rw-r--r--   0     1001      127      805 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/spinner.md
+-rw-r--r--   0     1001      127     1071 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md
+-rw-r--r--   0     1001      127     1489 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md
+-rw-r--r--   0     1001      127     2176 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md
+-rw-r--r--   0     1001      127     1037 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/switch.md
+-rw-r--r--   0     1001      127      800 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md
+-rw-r--r--   0     1001      127     2146 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/textedit.md
+-rw-r--r--   0     1001      127      335 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/verticalbox.md
+-rw-r--r--   0     1001      127      565 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/widgets.md
+-rw-r--r--   0     1001      127      364 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/recipes/button_native.slint
+-rw-r--r--   0     1001      127    28191 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/recipes/recipes.md
+-rw-r--r--   0     1001      127     3821 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/resources/slint-docs-highlight.html
+-rw-r--r--   0     1001      127     5521 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/resources/slint-docs-preview.html
+-rw-r--r--   0     1001      127    13863 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/site/index.html
+-rw-r--r--   0     1001      127     3880 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/testing.md
+-rw-r--r--   0     1001      127     1698 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/torizon.md
+-rw-r--r--   0     1001      127     3775 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/triage.md
+-rw-r--r--   0     1001      127     6705 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs.rs
+-rw-r--r--   0     1001      127    14341 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/lib.rs
+-rw-r--r--   0     1001      127    20004 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/mcu.md
+-rw-r--r--   0     1001      127     7535 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/private_unstable_api.rs
+-rw-r--r--   0     1001      127     8721 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/tests/partial_renderer.rs
+-rw-r--r--   0     1001      127      889 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/tests/show_strongref.rs
+-rw-r--r--   0     1001      127     1119 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/tests/simple_macro.rs
+-rw-r--r--   0     1001      127     2490 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/tests/spawn_local.rs
+-rw-r--r--   0     1001      127     2557 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/type-mappings.md
+-rw-r--r--   0     1001      127      706 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/macro/Cargo.toml
+-rw-r--r--   0     1001      127    12200 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/macro/macro.rs
+-rw-r--r--   0     1001      127      738 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/README.md
+-rw-r--r--   0     1001      127    19345 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/lib.rs
+-rw-r--r--   0     1001      127      471 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser-test-macro/Cargo.toml
+-rw-r--r--   0     1001      127      887 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser-test-macro/README.md
+-rw-r--r--   0     1001      127     5619 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser-test-macro/lib.rs
+-rw-r--r--   0     1001      127     1126 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     8815 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      635 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/README.md
+-rw-r--r--   0     1001      127     7636 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/builtin_structs.rs
+-rw-r--r--   0     1001      127    19223 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/enums.rs
+-rw-r--r--   0     1001      127     8311 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/key_codes.rs
+-rw-r--r--   0     1001      127     1322 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/lib.rs
+-rw-r--r--   0     1001      127   757076 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/sharedfontdb/DejaVuSans.ttf
+-rw-r--r--   0     1001      127      145 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/sharedfontdb/DejaVuSans.ttf.license
+-rw-r--r--   0     1001      127     4526 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/sharedfontdb/fontconfig.rs
+-rw-r--r--   0     1001      127     7491 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/sharedfontdb.rs
+-rw-r--r--   0     1001      127     1109 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      740 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/README.md
+-rw-r--r--   0     1001      127    34583 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/androidwindowadapter.rs
+-rw-r--r--   0     1001      127     4464 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/build.rs
+-rw-r--r--   0     1001      127    18055 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/java/SlintAndroidJavaHelper.java
+-rw-r--r--   0     1001      127    18156 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/javahelper.rs
+-rw-r--r--   0     1001      127     6133 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/lib.rs
+-rw-r--r--   0     1001      127     1955 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/README.md
+-rw-r--r--   0     1001      127    15614 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/calloop_backend/input.rs
+-rw-r--r--   0     1001      127    12022 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/calloop_backend.rs
+-rw-r--r--   0     1001      127     8655 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/display/gbmdisplay.rs
+-rw-r--r--   0     1001      127     2955 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/display/swdisplay.rs
+-rw-r--r--   0     1001      127     9345 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/display/vulkandisplay.rs
+-rw-r--r--   0     1001      127     3237 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/display.rs
+-rw-r--r--   0     1001      127    12140 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/drmoutput.rs
+-rw-r--r--   0     1001      127     6253 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/fullscreenwindowadapter.rs
+-rw-r--r--   0     1001      127     2022 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/lib.rs
+-rw-r--r--   0     1001      127      365 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/mouse-pointer.svg
+-rw-r--r--   0     1001      127      882 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/noop_backend.rs
+-rw-r--r--   0     1001      127     7507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/renderer/femtovg.rs
+-rw-r--r--   0     1001      127     6654 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/renderer/skia.rs
+-rw-r--r--   0     1001      127      532 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      590 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/README.md
+-rw-r--r--   0     1001      127     7310 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/lib.rs
+-rw-r--r--   0     1001      127     6405 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127    68116 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/api.rs
+-rw-r--r--   0     1001      127    83639 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/dynamic_item_tree.rs
+-rw-r--r--   0     1001      127     7555 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/dynamic_type.rs
+-rw-r--r--   0     1001      127    73407 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/eval.rs
+-rw-r--r--   0     1001      127    12240 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/eval_layout.rs
+-rw-r--r--   0     1001      127    31460 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/ffi.rs
+-rw-r--r--   0     1001      127     9875 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/global_component.rs
+-rw-r--r--   0     1001      127     5912 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/highlight.rs
+-rw-r--r--   0     1001      127     3015 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/lib.rs
+-rw-r--r--   0     1001      127     1425 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/migration.rs
+-rw-r--r--   0     1001      127     1795 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/tests.rs
+-rw-r--r--   0     1001      127     2301 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/value_model.rs
+-rw-r--r--   0     1001      127      571 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/macro/Cargo.toml
+-rw-r--r--   0     1001      127    10280 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/macro/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127    31632 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/macro/macro.rs
+-rw-r--r--   0     1001      127     1383 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/README.md
+-rw-r--r--   0     1001      127    10783 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/accessible_generated.rs
+-rw-r--r--   0     1001      127     2995 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/build.rs
+-rw-r--r--   0     1001      127    27433 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/key_generated.rs
+-rw-r--r--   0     1001      127    10534 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/lib.rs
+-rw-r--r--   0     1001      127    32883 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_accessible.rs
+-rw-r--r--   0     1001      127    21040 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/button.rs
+-rw-r--r--   0     1001      127     6862 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/checkbox.rs
+-rw-r--r--   0     1001      127     9594 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/combobox.rs
+-rw-r--r--   0     1001      127     8992 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/groupbox.rs
+-rw-r--r--   0     1001      127     5930 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/lineedit.rs
+-rw-r--r--   0     1001      127     8178 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/listviewitem.rs
+-rw-r--r--   0     1001      127     7422 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/palette.rs
+-rw-r--r--   0     1001      127     4945 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/progress_indicator.rs
+-rw-r--r--   0     1001      127    19794 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/scrollview.rs
+-rw-r--r--   0     1001      127    13934 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/slider.rs
+-rw-r--r--   0     1001      127    12529 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/spinbox.rs
+-rw-r--r--   0     1001      127     8594 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/stylemetrics.rs
+-rw-r--r--   0     1001      127     5637 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/tableheadersection.rs
+-rw-r--r--   0     1001      127    22411 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/tabwidget.rs
+-rw-r--r--   0     1001      127    12967 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets.rs
+-rw-r--r--   0     1001      127   103898 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_window.rs
+-rw-r--r--   0     1001      127     1919 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/README.md
+-rw-r--r--   0     1001      127    26501 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/fonts.rs
+-rw-r--r--   0     1001      127     9732 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/images.rs
+-rw-r--r--   0     1001      127    60402 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/itemrenderer.rs
+-rw-r--r--   0     1001      127    23205 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/lib.rs
+-rw-r--r--   0     1001      127      603 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/testing/Cargo.toml
+-rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/testing/README.md
+-rw-r--r--   0     1001      127    10886 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/testing/lib.rs
+-rw-r--r--   0     1001      127      623 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/Cargo.toml
+-rw-r--r--   0     1001      127     1796 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/CHANGELOG.md
+-rw-r--r--   0     1001      127    10280 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      399 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/README.md
+-rw-r--r--   0     1001      127     3723 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/src/compile_fail_tests.rs
+-rw-r--r--   0     1001      127    18776 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/src/lib.rs
+-rw-r--r--   0     1001      127    18973 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/src/vrc.rs
+-rw-r--r--   0     1001      127     9552 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/tests/test_vrc.rs
+-rw-r--r--   0     1001      127     5359 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/tests/test_vtable.rs
+-rw-r--r--   0     1001      127      768 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/build/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/build/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127    15366 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/build/lib.rs
+-rw-r--r--   0     1001      127     2370 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      872 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/README.md
+-rw-r--r--   0     1001      127     2014 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/build.rs
+-rw-r--r--   0     1001      127     5859 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/lib.rs
+-rw-r--r--   0     1001      127      630 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/Cargo.toml
+-rw-r--r--   0     1001      127      610 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/CHANGELOG.md
+-rw-r--r--   0     1001      127    10280 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      492 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/README.md
+-rw-r--r--   0     1001      127     6982 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/src/lib.rs
+-rw-r--r--   0     1001      127     4766 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/tests/test_field_offset.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 slint-1.6.0a6/api/python/Cargo.toml
+-rw-r--r--   0     1001      127       11 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/.gitignore
+-rw-r--r--   0     1001      127     7668 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/README.md
+-rw-r--r--   0     1001      127     4367 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/brush.rs
+-rw-r--r--   0     1001      127     3303 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/errors.rs
+-rw-r--r--   0     1001      127     1399 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/image.rs
+-rw-r--r--   0     1001      127    10939 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/interpreter.rs
+-rw-r--r--   0     1001      127     1421 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/lib.rs
+-rw-r--r--   0     1001      127     6300 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/models.rs
+-rw-r--r--   0     1001      127      348 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/noxfile.py
+-rw-r--r--   0     1001      127     7729 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/slint/__init__.py
+-rw-r--r--   0     1001      127     1889 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/slint/models.py
+-rw-r--r--   0     1001      127     1164 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_brush.py
+-rw-r--r--   0     1001      127     1019 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_callback_decorators.py
+-rw-r--r--   0     1001      127     2369 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_compiler.py
+-rw-r--r--   0     1001      127     1095 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_gc.py
+-rw-r--r--   0     1001      127     6577 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_instance.py
+-rw-r--r--   0     1001      127     1597 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_load_file.py
+-rw-r--r--   0     1001      127      905 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_load_file.slint
+-rw-r--r--   0     1001      127      687 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_loader.py
+-rw-r--r--   0     1001      127     3589 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_models.py
+-rw-r--r--   0     1001      127      832 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_timers.py
+-rw-r--r--   0     1001      127     2403 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/timer.rs
+-rw-r--r--   0     1001      127     4717 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/value.rs
+-rw-r--r--   0     1001      127   207085 2024-04-18 14:25:54.000000 slint-1.6.0a6/Cargo.lock
+-rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 slint-1.6.0a6/Cargo.toml
+-rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 slint-1.6.0a6/pyproject.toml
+-rw-r--r--   0     1001      127     7729 2024-04-18 14:25:49.000000 slint-1.6.0a6/slint/__init__.py
+-rw-r--r--   0     1001      127     1889 2024-04-18 14:25:49.000000 slint-1.6.0a6/slint/models.py
+-rw-r--r--   0        0        0     9215 1970-01-01 00:00:00.000000 slint-1.6.0a6/PKG-INFO
```

### Comparing `slint-1.6.0a5/api/rs/build/Cargo.toml` & `slint-1.6.0a6/api/rs/build/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/build/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/backends/winit/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/build/lib.rs` & `slint-1.6.0a6/api/rs/build/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/Cargo.toml` & `slint-1.6.0a6/api/rs/slint/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/core/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/core/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/LICENSES/MIT.txt` & `slint-1.6.0a6/internal/compiler/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/README.md` & `slint-1.6.0a6/api/rs/slint/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/android.rs` & `slint-1.6.0a6/api/rs/slint/android.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/compile_fail_tests.rs` & `slint-1.6.0a6/api/rs/slint/compile_fail_tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/building.md` & `slint-1.6.0a6/api/rs/slint/docs/building.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/development.md` & `slint-1.6.0a6/api/rs/slint/docs/development.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/install_qt.md` & `slint-1.6.0a6/api/rs/slint/docs/install_qt.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/README.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/conclusion.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/conclusion.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/getting_started.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/getting_started.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/at.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/at.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/icons/video.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/video.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/introduction.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/introduction.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/SUMMARY.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/conclusion.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/conclusion.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/getting_started.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/getting_started.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/at.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/at.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/bus.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bus.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/cloud.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cloud.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/cogs.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cogs.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/icons/video.png` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/video.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/introduction.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/introduction.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/main_game_logic.js` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/main_game_logic.js`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/memory_tile.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/quickstart/theme/head.hbs` & `slint-1.6.0a6/api/rs/slint/docs/quickstart/theme/head.hbs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/conf.py` & `slint-1.6.0a6/api/rs/slint/docs/reference/conf.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/index.rst` & `slint-1.6.0a6/api/rs/slint/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/backend_qt.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_qt.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/backend_winit.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_winit.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/advanced/style.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/style.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/introduction/index.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/introduction/index.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/introduction/supported_platforms.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/introduction/supported_platforms.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/callbacks.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/callbacks.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/elements.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/elements.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/functions.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/functions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/globals.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/globals.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/builtins/namespaces.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/namespaces.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/container.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/container.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/file.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/file.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/focus.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/focus.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/fonts.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/fonts.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/layouting.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/layouting.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/purity.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/purity.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/concepts/translations.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/translations.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/index.rst` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/index.rst`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/animations.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/animations.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/callbacks.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/callbacks.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/expressions.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/expressions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/functions.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/functions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/globals.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/globals.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/modules.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/modules.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/properties.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/properties.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/repetitions.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/repetitions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/statements.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/statements.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/states.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/states.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/syntax/types.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/types.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/button.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/button.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/checkbox.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/checkbox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/combobox.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/combobox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/groupbox.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/groupbox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/index.rst` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/index.rst`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/lineedit.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/lineedit.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/listview.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/listview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/scrollview.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/scrollview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/slider.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/slider.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/spinbox.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/spinbox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/spinner.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/spinner.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/switch.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/switch.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/textedit.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/textedit.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/language/widgets/widgets.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/widgets.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/reference/src/recipes/recipes.md` & `slint-1.6.0a6/api/rs/slint/docs/reference/src/recipes/recipes.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/resources/slint-docs-highlight.html` & `slint-1.6.0a6/api/rs/slint/docs/resources/slint-docs-highlight.html`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/resources/slint-docs-preview.html` & `slint-1.6.0a6/api/rs/slint/docs/resources/slint-docs-preview.html`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/site/index.html` & `slint-1.6.0a6/api/rs/slint/docs/site/index.html`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/testing.md` & `slint-1.6.0a6/api/rs/slint/docs/testing.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/torizon.md` & `slint-1.6.0a6/api/rs/slint/docs/torizon.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs/triage.md` & `slint-1.6.0a6/api/rs/slint/docs/triage.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/docs.rs` & `slint-1.6.0a6/api/rs/slint/docs.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/lib.rs` & `slint-1.6.0a6/api/rs/slint/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/mcu.md` & `slint-1.6.0a6/api/rs/slint/mcu.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/private_unstable_api.rs` & `slint-1.6.0a6/api/rs/slint/private_unstable_api.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/tests/partial_renderer.rs` & `slint-1.6.0a6/api/rs/slint/tests/partial_renderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/tests/show_strongref.rs` & `slint-1.6.0a6/api/rs/slint/tests/show_strongref.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/tests/simple_macro.rs` & `slint-1.6.0a6/api/rs/slint/tests/simple_macro.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/tests/spawn_local.rs` & `slint-1.6.0a6/api/rs/slint/tests/spawn_local.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/slint/type-mappings.md` & `slint-1.6.0a6/api/rs/slint/type-mappings.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/android-activity/Cargo.toml` & `slint-1.6.0a6/internal/backends/android-activity/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/compiler/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/android-activity/README.md` & `slint-1.6.0a6/internal/backends/android-activity/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/android-activity/androidwindowadapter.rs` & `slint-1.6.0a6/internal/backends/android-activity/androidwindowadapter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/android-activity/build.rs` & `slint-1.6.0a6/internal/backends/android-activity/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/android-activity/java/SlintAndroidJavaHelper.java` & `slint-1.6.0a6/internal/backends/android-activity/java/SlintAndroidJavaHelper.java`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/android-activity/javahelper.rs` & `slint-1.6.0a6/internal/backends/android-activity/javahelper.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/android-activity/lib.rs` & `slint-1.6.0a6/internal/backends/android-activity/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/Cargo.toml` & `slint-1.6.0a6/internal/interpreter/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/renderers/skia/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/api.rs` & `slint-1.6.0a6/internal/interpreter/api.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/dynamic_item_tree.rs` & `slint-1.6.0a6/internal/interpreter/dynamic_item_tree.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/dynamic_type.rs` & `slint-1.6.0a6/internal/interpreter/dynamic_type.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/eval.rs` & `slint-1.6.0a6/internal/interpreter/eval.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/eval_layout.rs` & `slint-1.6.0a6/internal/interpreter/eval_layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/ffi.rs` & `slint-1.6.0a6/internal/interpreter/ffi.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/global_component.rs` & `slint-1.6.0a6/internal/interpreter/global_component.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/highlight.rs` & `slint-1.6.0a6/internal/interpreter/highlight.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/lib.rs` & `slint-1.6.0a6/internal/interpreter/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/migration.rs` & `slint-1.6.0a6/internal/interpreter/migration.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/tests.rs` & `slint-1.6.0a6/internal/interpreter/tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/interpreter/value_model.rs` & `slint-1.6.0a6/internal/interpreter/value_model.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/const-field-offset/Cargo.toml` & `slint-1.6.0a6/helper_crates/const-field-offset/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/const-field-offset/CHANGELOG.md` & `slint-1.6.0a6/helper_crates/const-field-offset/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt` & `slint-1.6.0a6/internal/compiler/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/const-field-offset/LICENSES/MIT.txt` & `slint-1.6.0a6/api/rs/slint/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/const-field-offset/src/lib.rs` & `slint-1.6.0a6/helper_crates/const-field-offset/src/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/const-field-offset/tests/test_field_offset.rs` & `slint-1.6.0a6/helper_crates/const-field-offset/tests/test_field_offset.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/const-field-offset/macro/Cargo.toml` & `slint-1.6.0a6/helper_crates/const-field-offset/macro/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/const-field-offset/macro/macro.rs` & `slint-1.6.0a6/helper_crates/const-field-offset/macro/macro.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/Cargo.toml` & `slint-1.6.0a6/internal/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/api/rs/slint/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/README.md` & `slint-1.6.0a6/internal/core/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/accessibility.rs` & `slint-1.6.0a6/internal/core/accessibility.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/animations.rs` & `slint-1.6.0a6/internal/core/animations.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/api.rs` & `slint-1.6.0a6/internal/core/api.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/callbacks.rs` & `slint-1.6.0a6/internal/core/callbacks.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/component_factory.rs` & `slint-1.6.0a6/internal/core/component_factory.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/context.rs` & `slint-1.6.0a6/internal/core/context.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/future.rs` & `slint-1.6.0a6/internal/core/future.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/bitmapfont.rs` & `slint-1.6.0a6/internal/core/graphics/bitmapfont.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/border_radius.rs` & `slint-1.6.0a6/internal/core/graphics/border_radius.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/boxshadowcache.rs` & `slint-1.6.0a6/internal/core/graphics/boxshadowcache.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/brush.rs` & `slint-1.6.0a6/internal/core/graphics/brush.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/color.rs` & `slint-1.6.0a6/internal/core/graphics/color.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/image/cache.rs` & `slint-1.6.0a6/internal/core/graphics/image/cache.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/image/htmlimage.rs` & `slint-1.6.0a6/internal/core/graphics/image/htmlimage.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/image/svg.rs` & `slint-1.6.0a6/internal/core/graphics/image/svg.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/image.rs` & `slint-1.6.0a6/internal/core/graphics/image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/path.rs` & `slint-1.6.0a6/internal/core/graphics/path.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics/rendering_metrics_collector.rs` & `slint-1.6.0a6/internal/core/graphics/rendering_metrics_collector.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/graphics.rs` & `slint-1.6.0a6/internal/core/graphics.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/input.rs` & `slint-1.6.0a6/internal/core/input.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/item_focus.rs` & `slint-1.6.0a6/internal/core/item_focus.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/item_rendering.rs` & `slint-1.6.0a6/internal/core/item_rendering.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/item_tree.rs` & `slint-1.6.0a6/internal/core/item_tree.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/items/component_container.rs` & `slint-1.6.0a6/internal/core/items/component_container.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/items/flickable.rs` & `slint-1.6.0a6/internal/core/items/flickable.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/items/image.rs` & `slint-1.6.0a6/internal/core/items/image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/items/path.rs` & `slint-1.6.0a6/internal/core/items/path.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/items/text.rs` & `slint-1.6.0a6/internal/core/items/text.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/items.rs` & `slint-1.6.0a6/internal/core/items.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/layout.rs` & `slint-1.6.0a6/internal/core/layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/lengths.rs` & `slint-1.6.0a6/internal/core/lengths.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/lib.rs` & `slint-1.6.0a6/internal/core/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/model/adapters.rs` & `slint-1.6.0a6/internal/core/model/adapters.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/model/model_peer.rs` & `slint-1.6.0a6/internal/core/model/model_peer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/model.rs` & `slint-1.6.0a6/internal/core/model.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/platform.rs` & `slint-1.6.0a6/internal/core/platform.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/properties/ffi.rs` & `slint-1.6.0a6/internal/core/properties/ffi.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/properties/properties_animations.rs` & `slint-1.6.0a6/internal/core/properties/properties_animations.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/properties.rs` & `slint-1.6.0a6/internal/core/properties.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/renderer.rs` & `slint-1.6.0a6/internal/core/renderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/rtti.rs` & `slint-1.6.0a6/internal/core/rtti.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/sharedvector.rs` & `slint-1.6.0a6/internal/core/sharedvector.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/slice.rs` & `slint-1.6.0a6/internal/core/slice.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/software_renderer/draw_functions.rs` & `slint-1.6.0a6/internal/core/software_renderer/draw_functions.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/software_renderer/fixed.rs` & `slint-1.6.0a6/internal/core/software_renderer/fixed.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/software_renderer/fonts/pixelfont.rs` & `slint-1.6.0a6/internal/core/software_renderer/fonts/pixelfont.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/software_renderer/fonts/systemfonts.rs` & `slint-1.6.0a6/internal/core/software_renderer/fonts/systemfonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/software_renderer/fonts/vectorfont.rs` & `slint-1.6.0a6/internal/core/software_renderer/fonts/vectorfont.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/software_renderer/fonts.rs` & `slint-1.6.0a6/internal/core/software_renderer/fonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/software_renderer.rs` & `slint-1.6.0a6/internal/core/software_renderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/string.rs` & `slint-1.6.0a6/internal/core/string.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/tests.rs` & `slint-1.6.0a6/internal/core/tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/textlayout/fragments.rs` & `slint-1.6.0a6/internal/core/textlayout/fragments.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/textlayout/glyphclusters.rs` & `slint-1.6.0a6/internal/core/textlayout/glyphclusters.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/textlayout/linebreak_simple.rs` & `slint-1.6.0a6/internal/core/textlayout/linebreak_simple.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/textlayout/linebreak_unicode.rs` & `slint-1.6.0a6/internal/core/textlayout/linebreak_unicode.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/textlayout/linebreaker.rs` & `slint-1.6.0a6/internal/core/textlayout/linebreaker.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/textlayout/shaping.rs` & `slint-1.6.0a6/internal/core/textlayout/shaping.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/textlayout.rs` & `slint-1.6.0a6/internal/core/textlayout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/timers.rs` & `slint-1.6.0a6/internal/core/timers.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/translations.rs` & `slint-1.6.0a6/internal/core/translations.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/unsafe_single_threaded.rs` & `slint-1.6.0a6/internal/core/unsafe_single_threaded.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core/window.rs` & `slint-1.6.0a6/internal/core/window.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/Cargo.toml` & `slint-1.6.0a6/internal/compiler/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/LICENSES/Apache-2.0.txt` & `slint-1.6.0a6/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/LICENSES/CC-BY-ND-4.0.txt` & `slint-1.6.0a6/internal/compiler/LICENSES/CC-BY-ND-4.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/api/rs/macros/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/LICENSES/MIT.txt` & `slint-1.6.0a6/internal/backends/linuxkms/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/README.md` & `slint-1.6.0a6/internal/compiler/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/build.rs` & `slint-1.6.0a6/internal/compiler/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/builtin_macros.rs` & `slint-1.6.0a6/internal/compiler/builtin_macros.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/builtins.slint` & `slint-1.6.0a6/internal/compiler/builtins.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/diagnostics.rs` & `slint-1.6.0a6/internal/compiler/diagnostics.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/embedded_resources.rs` & `slint-1.6.0a6/internal/compiler/embedded_resources.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/expression_tree.rs` & `slint-1.6.0a6/internal/compiler/expression_tree.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/fileaccess.rs` & `slint-1.6.0a6/internal/compiler/fileaccess.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/generator/cpp.rs` & `slint-1.6.0a6/internal/compiler/generator/cpp.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/generator/rust.rs` & `slint-1.6.0a6/internal/compiler/generator/rust.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/generator.rs` & `slint-1.6.0a6/internal/compiler/generator.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/langtype.rs` & `slint-1.6.0a6/internal/compiler/langtype.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/layout.rs` & `slint-1.6.0a6/internal/compiler/layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/lexer.rs` & `slint-1.6.0a6/internal/compiler/lexer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/lib.rs` & `slint-1.6.0a6/internal/compiler/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/literals.rs` & `slint-1.6.0a6/internal/compiler/literals.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/llr/expression.rs` & `slint-1.6.0a6/internal/compiler/llr/expression.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/llr/item_tree.rs` & `slint-1.6.0a6/internal/compiler/llr/item_tree.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/llr/lower_expression.rs` & `slint-1.6.0a6/internal/compiler/llr/lower_expression.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/llr/lower_to_item_tree.rs` & `slint-1.6.0a6/internal/compiler/llr/lower_to_item_tree.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/llr/optim_passes/count_property_use.rs` & `slint-1.6.0a6/internal/compiler/llr/optim_passes/count_property_use.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/llr/optim_passes/inline_expressions.rs` & `slint-1.6.0a6/internal/compiler/llr/optim_passes/inline_expressions.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/llr/pretty_print.rs` & `slint-1.6.0a6/internal/compiler/llr/pretty_print.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/llr.rs` & `slint-1.6.0a6/internal/compiler/llr.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/load_builtins.rs` & `slint-1.6.0a6/internal/compiler/load_builtins.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/lookup.rs` & `slint-1.6.0a6/internal/compiler/lookup.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/namedreference.rs` & `slint-1.6.0a6/internal/compiler/namedreference.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/object_tree.rs` & `slint-1.6.0a6/internal/compiler/object_tree.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/parser/document.rs` & `slint-1.6.0a6/internal/compiler/parser/document.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/parser/element.rs` & `slint-1.6.0a6/internal/compiler/parser/element.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/parser/expressions.rs` & `slint-1.6.0a6/internal/compiler/parser/expressions.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/parser/statements.rs` & `slint-1.6.0a6/internal/compiler/parser/statements.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/parser/type.rs` & `slint-1.6.0a6/internal/compiler/parser/type.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/parser.rs` & `slint-1.6.0a6/internal/compiler/parser.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/apply_default_properties_from_style.rs` & `slint-1.6.0a6/internal/compiler/passes/apply_default_properties_from_style.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/binding_analysis.rs` & `slint-1.6.0a6/internal/compiler/passes/binding_analysis.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/border_radius.rs` & `slint-1.6.0a6/internal/compiler/passes/border_radius.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/check_expressions.rs` & `slint-1.6.0a6/internal/compiler/passes/check_expressions.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/check_public_api.rs` & `slint-1.6.0a6/internal/compiler/passes/check_public_api.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/check_rotation.rs` & `slint-1.6.0a6/internal/compiler/passes/check_rotation.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/clip.rs` & `slint-1.6.0a6/internal/compiler/passes/clip.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/collect_custom_fonts.rs` & `slint-1.6.0a6/internal/compiler/passes/collect_custom_fonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/collect_globals.rs` & `slint-1.6.0a6/internal/compiler/passes/collect_globals.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/collect_init_code.rs` & `slint-1.6.0a6/internal/compiler/passes/collect_init_code.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/collect_structs_and_enums.rs` & `slint-1.6.0a6/internal/compiler/passes/collect_structs_and_enums.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/collect_subcomponents.rs` & `slint-1.6.0a6/internal/compiler/passes/collect_subcomponents.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/compile_paths.rs` & `slint-1.6.0a6/internal/compiler/passes/compile_paths.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/const_propagation.rs` & `slint-1.6.0a6/internal/compiler/passes/const_propagation.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/deduplicate_property_read.rs` & `slint-1.6.0a6/internal/compiler/passes/deduplicate_property_read.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/default_geometry.rs` & `slint-1.6.0a6/internal/compiler/passes/default_geometry.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/embed_glyphs.rs` & `slint-1.6.0a6/internal/compiler/passes/embed_glyphs.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/embed_images.rs` & `slint-1.6.0a6/internal/compiler/passes/embed_images.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/ensure_window.rs` & `slint-1.6.0a6/internal/compiler/passes/ensure_window.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/flickable.rs` & `slint-1.6.0a6/internal/compiler/passes/flickable.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/focus_handling.rs` & `slint-1.6.0a6/internal/compiler/passes/focus_handling.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/generate_item_indices.rs` & `slint-1.6.0a6/internal/compiler/passes/generate_item_indices.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/infer_aliases_types.rs` & `slint-1.6.0a6/internal/compiler/passes/infer_aliases_types.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/inlining.rs` & `slint-1.6.0a6/internal/compiler/passes/inlining.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/lower_absolute_coordinates.rs` & `slint-1.6.0a6/internal/compiler/passes/lower_absolute_coordinates.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/lower_accessibility.rs` & `slint-1.6.0a6/internal/compiler/passes/lower_accessibility.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/lower_component_container.rs` & `slint-1.6.0a6/internal/compiler/passes/lower_component_container.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/lower_layout.rs` & `slint-1.6.0a6/internal/compiler/passes/lower_layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/lower_popups.rs` & `slint-1.6.0a6/internal/compiler/passes/lower_popups.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/lower_property_to_element.rs` & `slint-1.6.0a6/internal/compiler/passes/lower_property_to_element.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/lower_shadows.rs` & `slint-1.6.0a6/internal/compiler/passes/lower_shadows.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/lower_states.rs` & `slint-1.6.0a6/internal/compiler/passes/lower_states.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/lower_tabwidget.rs` & `slint-1.6.0a6/internal/compiler/passes/lower_tabwidget.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/lower_text_input_interface.rs` & `slint-1.6.0a6/internal/compiler/passes/lower_text_input_interface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/materialize_fake_properties.rs` & `slint-1.6.0a6/internal/compiler/passes/materialize_fake_properties.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/move_declarations.rs` & `slint-1.6.0a6/internal/compiler/passes/move_declarations.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/optimize_useless_rectangles.rs` & `slint-1.6.0a6/internal/compiler/passes/optimize_useless_rectangles.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/purity_check.rs` & `slint-1.6.0a6/internal/compiler/passes/purity_check.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/remove_aliases.rs` & `slint-1.6.0a6/internal/compiler/passes/remove_aliases.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/remove_return.rs` & `slint-1.6.0a6/internal/compiler/passes/remove_return.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/remove_unused_properties.rs` & `slint-1.6.0a6/internal/compiler/passes/remove_unused_properties.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/repeater_component.rs` & `slint-1.6.0a6/internal/compiler/passes/repeater_component.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/resolve_native_classes.rs` & `slint-1.6.0a6/internal/compiler/passes/resolve_native_classes.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/resolving.rs` & `slint-1.6.0a6/internal/compiler/passes/resolving.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/unique_id.rs` & `slint-1.6.0a6/internal/compiler/passes/unique_id.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/visible.rs` & `slint-1.6.0a6/internal/compiler/passes/visible.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes/z_order.rs` & `slint-1.6.0a6/internal/compiler/passes/z_order.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/passes.rs` & `slint-1.6.0a6/internal/compiler/passes.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/pathutils.rs` & `slint-1.6.0a6/internal/compiler/pathutils.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/consistent_styles.rs` & `slint-1.6.0a6/internal/compiler/tests/consistent_styles.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/accessibility/accessible_properties.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/accessibility/accessible_properties.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop1.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop1.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_function.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_function.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/analysis/binding_loop_self.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_self.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/animate.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/animate.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/assign.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/assign.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/box_shadow.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/box_shadow.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/children_placeholder.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/children_placeholder.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/clip.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/clip.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/dialog.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/dialog.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/dialog2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/dialog2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/duplicated_id.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/duplicated_id.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/easing.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/easing.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/enums.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/enums.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/item_as_property.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/item_as_property.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/layout2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/layout2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/linear-gradient.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/linear-gradient.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/opacity.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/opacity.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/parse_error.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/parse_error.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/path.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/path.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/path_commands.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/path_commands.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/path_for.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/path_for.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/percent.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/percent.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/popup.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/popup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/property_declaration.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/property_declaration.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/radial-gradient.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/radial-gradient.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/return.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/return.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/rotation.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/rotation.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/self_assign.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/self_assign.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/signal.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/signal.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/states_transitions.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/states_transitions2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/states_transitions3.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions3.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/states_two_way.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_two_way.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/sub_elements.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/sub_elements.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/tr.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/tr.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/tr2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/tr2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/type_declaration.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/type_declaration.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/basic/unknown_item.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/basic/unknown_item.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/elements/component_container.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/elements/component_container.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/elements/listview.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/elements/listview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/elements/popup.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/elements/popup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/elements/tabwidget.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/elements/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/elements/tabwidget2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/elements/tabwidget2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/exports/reexport_duplicate.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/exports/reexport_duplicate.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/expressions/arithmetic_op.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/arithmetic_op.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/expressions/clamp.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/clamp.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/expressions/comparison_operator.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/comparison_operator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/expressions/condition_operator.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/condition_operator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/expressions/image-url.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/image-url.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/expressions/image-url2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/image-url2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/expressions/minmax.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/minmax.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/expressions/percent2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/percent2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/expressions/unary_op.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/unary_op.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/focus/focus_not_called.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/focus/focus_not_called.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/focus/focus_wrong_args.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/focus/focus_wrong_args.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/functions/function_double_qualified.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/functions/function_double_qualified.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/functions/functions.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/functions/functions_call.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions_call.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/functions/functions_purity.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions_purity.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/imports/bug_2719.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/imports/bug_2719.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/imports/import_errors.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_errors.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/layout/if_in_grid.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/layout/if_in_grid.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/layout/min_max_conflict.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/layout/min_max_conflict.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/layout/spacing.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/layout/spacing.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/array_index.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/array_index.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/callback_alias.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/callback_alias2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/callback_alias3.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias3.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/color.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/color.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/conversion.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/conversion.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/dashes.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/dashes.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/deprecated_property.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/deprecated_property.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/enum.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/enum.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/for_lookup.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/for_lookup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/global.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/global.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/if.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/if.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/issue_1461.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/issue_1461.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/property.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/property.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/signal_arg.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/signal_arg.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/two_way_binding.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/two_way_binding.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/input_output.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/input_output.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/input_output2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/input_output2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/new_component.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/new_component.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/new_lookup.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/new_lookup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/property2.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/property2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/state1.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/state1.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax/parse_error/struct.slint` & `slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/struct.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/tests/syntax_tests.rs` & `slint-1.6.0a6/internal/compiler/tests/syntax_tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/typeloader.rs` & `slint-1.6.0a6/internal/compiler/typeloader.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/typeregister.rs` & `slint-1.6.0a6/internal/compiler/typeregister.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg` & `slint-1.6.0a6/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg` & `slint-1.6.0a6/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/combobox-base.slint` & `slint-1.6.0a6/internal/compiler/widgets/common/combobox-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/common.slint` & `slint-1.6.0a6/internal/compiler/widgets/common/common.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/lineedit-base.slint` & `slint-1.6.0a6/internal/compiler/widgets/common/lineedit-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/listview.slint` & `slint-1.6.0a6/internal/compiler/widgets/common/listview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/slider-base.slint` & `slint-1.6.0a6/internal/compiler/widgets/common/slider-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/spinbox-base.slint` & `slint-1.6.0a6/internal/compiler/widgets/common/spinbox-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/spinner-base.slint` & `slint-1.6.0a6/internal/compiler/widgets/common/spinner-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/standardbutton.slint` & `slint-1.6.0a6/internal/compiler/widgets/common/standardbutton.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/common/tabwidget-base.slint` & `slint-1.6.0a6/internal/compiler/widgets/common/tabwidget-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/button.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/button.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/checkbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/combobox.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/components.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/groupbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/layouts.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/lineedit.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/progressindicator.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/scrollview.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/slider.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/spinbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/spinner.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/std-widgets-base.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/styling.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/switch.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/tableview.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/tabwidget.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cosmic-base/textedit.slint` & `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/textedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_arrow-down.svg` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_arrow-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_check-mark.svg` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_check-mark.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_chevron-down.svg` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_chevron-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_chevron-up.svg` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_chevron-up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_down.svg` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_left.svg` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_left.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_right.svg` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_right.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/_up.svg` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/button.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/button.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/checkbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/combobox.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/components.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/groupbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/layouts.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/lineedit.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/progressindicator.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/scrollview.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/slider.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/spinbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/spinner.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/std-widgets-base.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/styling.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/switch.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/tableview.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/tabwidget.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/cupertino-base/textedit.slint` & `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/textedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/_arrow-down.svg` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_arrow-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/_check-mark.svg` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_check-mark.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/_chevron-down.svg` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_chevron-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/_chevron-up.svg` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_chevron-up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/_down.svg` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/_left.svg` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_left.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/_right.svg` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_right.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/_up.svg` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/button.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/button.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/checkbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/combobox.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/components.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/groupbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/layouts.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/lineedit.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/progressindicator.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/scrollview.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/slider.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/spinbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/spinner.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/std-widgets-base.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/std-widgets-impl.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/styling.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/switch.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/tableview.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/tabwidget.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/fluent-base/textedit.slint` & `slint-1.6.0a6/internal/compiler/widgets/fluent-base/textedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/button.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/button.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/checkbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/combobox.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/components.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/groupbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/layouts.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/lineedit.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/progressindicator.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/scrollview.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/slider.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/spinbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/spinner.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/std-widgets-base.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/std-widgets-impl.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/styling.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/switch.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/tableview.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/material-base/tabwidget.slint` & `slint-1.6.0a6/internal/compiler/widgets/material-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/button.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/button.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/combobox.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/groupbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/internal-scrollview.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/internal-scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/layouts.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/lineedit.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/scrollview.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/spinbox.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/spinner.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/std-widgets.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/std-widgets.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/tableview.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/widgets/qt/tabwidget.slint` & `slint-1.6.0a6/internal/compiler/widgets/qt/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/Cargo.toml` & `slint-1.6.0a6/internal/backends/linuxkms/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/common/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/common/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/LICENSES/MIT.txt` & `slint-1.6.0a6/helper_crates/vtable/macro/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/calloop_backend/input.rs` & `slint-1.6.0a6/internal/backends/linuxkms/calloop_backend/input.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/calloop_backend.rs` & `slint-1.6.0a6/internal/backends/linuxkms/calloop_backend.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/display/gbmdisplay.rs` & `slint-1.6.0a6/internal/backends/linuxkms/display/gbmdisplay.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/display/swdisplay.rs` & `slint-1.6.0a6/internal/backends/linuxkms/display/swdisplay.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/display/vulkandisplay.rs` & `slint-1.6.0a6/internal/backends/linuxkms/display/vulkandisplay.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/display.rs` & `slint-1.6.0a6/internal/backends/linuxkms/display.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/drmoutput.rs` & `slint-1.6.0a6/internal/backends/linuxkms/drmoutput.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/fullscreenwindowadapter.rs` & `slint-1.6.0a6/internal/backends/linuxkms/fullscreenwindowadapter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/lib.rs` & `slint-1.6.0a6/internal/backends/linuxkms/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/noop_backend.rs` & `slint-1.6.0a6/internal/backends/linuxkms/noop_backend.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/renderer/femtovg.rs` & `slint-1.6.0a6/internal/backends/linuxkms/renderer/femtovg.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/linuxkms/renderer/skia.rs` & `slint-1.6.0a6/internal/backends/linuxkms/renderer/skia.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/Cargo.toml` & `slint-1.6.0a6/internal/backends/qt/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/accessible_generated.rs` & `slint-1.6.0a6/internal/backends/qt/accessible_generated.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/build.rs` & `slint-1.6.0a6/internal/backends/qt/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/key_generated.rs` & `slint-1.6.0a6/internal/backends/qt/key_generated.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/lib.rs` & `slint-1.6.0a6/internal/backends/qt/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_accessible.rs` & `slint-1.6.0a6/internal/backends/qt/qt_accessible.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/button.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/button.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/checkbox.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/checkbox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/combobox.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/combobox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/groupbox.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/groupbox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/lineedit.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/lineedit.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/listviewitem.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/listviewitem.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/palette.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/palette.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/progress_indicator.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/progress_indicator.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/scrollview.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/scrollview.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/slider.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/slider.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/spinbox.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/spinbox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/stylemetrics.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/stylemetrics.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/tableheadersection.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/tableheadersection.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets/tabwidget.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets/tabwidget.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_widgets.rs` & `slint-1.6.0a6/internal/backends/qt/qt_widgets.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/qt/qt_window.rs` & `slint-1.6.0a6/internal/backends/qt/qt_window.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/Cargo.toml` & `slint-1.6.0a6/internal/renderers/skia/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/build.rs` & `slint-1.6.0a6/internal/renderers/skia/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/cached_image.rs` & `slint-1.6.0a6/internal/renderers/skia/cached_image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/d3d_surface.rs` & `slint-1.6.0a6/internal/renderers/skia/d3d_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/itemrenderer.rs` & `slint-1.6.0a6/internal/renderers/skia/itemrenderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/lib.rs` & `slint-1.6.0a6/internal/renderers/skia/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/metal_surface.rs` & `slint-1.6.0a6/internal/renderers/skia/metal_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/opengl_surface.rs` & `slint-1.6.0a6/internal/renderers/skia/opengl_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/software_surface.rs` & `slint-1.6.0a6/internal/renderers/skia/software_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/textlayout.rs` & `slint-1.6.0a6/internal/renderers/skia/textlayout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/skia/vulkan_surface.rs` & `slint-1.6.0a6/internal/renderers/skia/vulkan_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/macros/Cargo.toml` & `slint-1.6.0a6/api/rs/macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/macros/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/core-macros/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/rs/macros/lib.rs` & `slint-1.6.0a6/api/rs/macros/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/macro/Cargo.toml` & `slint-1.6.0a6/helper_crates/vtable/macro/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt` & `slint-1.6.0a6/helper_crates/vtable/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/macro/LICENSES/MIT.txt` & `slint-1.6.0a6/helper_crates/vtable/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/macro/macro.rs` & `slint-1.6.0a6/helper_crates/vtable/macro/macro.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/testing/Cargo.toml` & `slint-1.6.0a6/internal/backends/testing/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/testing/lib.rs` & `slint-1.6.0a6/internal/backends/testing/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core-macros/Cargo.toml` & `slint-1.6.0a6/internal/core-macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core-macros/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/interpreter/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core-macros/README.md` & `slint-1.6.0a6/internal/core-macros/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/core-macros/lib.rs` & `slint-1.6.0a6/internal/core-macros/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/Cargo.toml` & `slint-1.6.0a6/internal/backends/winit/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/backends/qt/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/README.md` & `slint-1.6.0a6/internal/backends/winit/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/accesskit.rs` & `slint-1.6.0a6/internal/backends/winit/accesskit.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/event_loop.rs` & `slint-1.6.0a6/internal/backends/winit/event_loop.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/lib.rs` & `slint-1.6.0a6/internal/backends/winit/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/renderer/femtovg/glcontext.rs` & `slint-1.6.0a6/internal/backends/winit/renderer/femtovg/glcontext.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/renderer/femtovg.rs` & `slint-1.6.0a6/internal/backends/winit/renderer/femtovg.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/renderer/skia.rs` & `slint-1.6.0a6/internal/backends/winit/renderer/skia.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/renderer/sw.rs` & `slint-1.6.0a6/internal/backends/winit/renderer/sw.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/wasm_input_helper.rs` & `slint-1.6.0a6/internal/backends/winit/wasm_input_helper.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/winit/winitwindowadapter.rs` & `slint-1.6.0a6/internal/backends/winit/winitwindowadapter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/selector/Cargo.toml` & `slint-1.6.0a6/internal/backends/selector/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/selector/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/selector/README.md` & `slint-1.6.0a6/internal/backends/selector/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/selector/build.rs` & `slint-1.6.0a6/internal/backends/selector/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/backends/selector/lib.rs` & `slint-1.6.0a6/internal/backends/selector/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/Cargo.toml` & `slint-1.6.0a6/internal/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/api/rs/build/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt` & `slint-1.6.0a6/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/README.md` & `slint-1.6.0a6/internal/common/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/builtin_structs.rs` & `slint-1.6.0a6/internal/common/builtin_structs.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/enums.rs` & `slint-1.6.0a6/internal/common/enums.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/key_codes.rs` & `slint-1.6.0a6/internal/common/key_codes.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/lib.rs` & `slint-1.6.0a6/internal/common/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/sharedfontdb/DejaVuSans.ttf` & `slint-1.6.0a6/internal/common/sharedfontdb/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/sharedfontdb/fontconfig.rs` & `slint-1.6.0a6/internal/common/sharedfontdb/fontconfig.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/common/sharedfontdb.rs` & `slint-1.6.0a6/internal/common/sharedfontdb.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/femtovg/Cargo.toml` & `slint-1.6.0a6/internal/renderers/femtovg/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a6/internal/backends/selector/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a6/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a6/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/femtovg/fonts.rs` & `slint-1.6.0a6/internal/renderers/femtovg/fonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/femtovg/images.rs` & `slint-1.6.0a6/internal/renderers/femtovg/images.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/femtovg/itemrenderer.rs` & `slint-1.6.0a6/internal/renderers/femtovg/itemrenderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/renderers/femtovg/lib.rs` & `slint-1.6.0a6/internal/renderers/femtovg/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/parser-test-macro/README.md` & `slint-1.6.0a6/internal/compiler/parser-test-macro/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/internal/compiler/parser-test-macro/lib.rs` & `slint-1.6.0a6/internal/compiler/parser-test-macro/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/Cargo.toml` & `slint-1.6.0a6/helper_crates/vtable/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/CHANGELOG.md` & `slint-1.6.0a6/helper_crates/vtable/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/LICENSES/Apache-2.0.txt` & `slint-1.6.0a6/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/LICENSES/MIT.txt` & `slint-1.6.0a6/helper_crates/const-field-offset/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/src/compile_fail_tests.rs` & `slint-1.6.0a6/helper_crates/vtable/src/compile_fail_tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/src/lib.rs` & `slint-1.6.0a6/helper_crates/vtable/src/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/src/vrc.rs` & `slint-1.6.0a6/helper_crates/vtable/src/vrc.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/tests/test_vrc.rs` & `slint-1.6.0a6/helper_crates/vtable/tests/test_vrc.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/helper_crates/vtable/tests/test_vtable.rs` & `slint-1.6.0a6/helper_crates/vtable/tests/test_vtable.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/Cargo.toml` & `slint-1.6.0a6/api/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/README.md` & `slint-1.6.0a6/api/python/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 cd examples/printerdemo/python
 pipenv update
 pipenv run python main.py
 ```
 
 ## Quick Start
 
-1. Add Slint from the Git development branch to your Python project: `pipenv install "git+https://github.com/slint-ui/slint#subdirectory=api/python&egg=slint"`
+1. Add Slint Python Package Index to your Python project: `pipenv install slint`
 2. Create a file called `appwindow.slint`:
 
 ```slint
 import { Button, VerticalBox } from "std-widgets.slint";
 
 export component AppWindow inherits Window {
     in-out property<int> counter: 42;
@@ -70,17 +70,16 @@
 }
 ```
 
 1. Create a file called `main.py`:
 
 ```python
 import slint
-import appwindow_slint
 
-class App(appwindow_slint.AppWindow):
+class App(slint.loader.appwindow.AppWindow):
     @slint.callback
     def request_increase_value(self):
         self.counter = self.counter + 1
 
 app = App()
 app.run()
 ```
@@ -89,15 +88,15 @@
 
 ## API Overview
 
 ### Instantiating a Component
 
 The following example shows how to instantiate a Slint component in Python:
 
-**`ui.slint`**
+**`app.slint`**
 
 ```slint
 export component MainWindow inherits Window {
     callback clicked <=> i-touch-area.clicked;
 
     in property <int> counter;
 
@@ -107,29 +106,33 @@
     i-touch-area := TouchArea {}
 }
 ```
 
 The exported component is exposed as a Python class. To access this class, you have two
 options:
 
-1. Call `slint.load_file("ui.slint")`. The returned object is a [namespace](https://docs.python.org/3/library/types.html#types.SimpleNamespace),
+1. Call `slint.load_file("app.slint")`. The returned object is a [namespace](https://docs.python.org/3/library/types.html#types.SimpleNamespace),
    that provides the `MainWindow` class:
    ```python
    import slint
-   components = slint.load_file("ui.slint")
+   components = slint.load_file("app.slint")
    main_window = components.MainWindow()
    ```
 
-2. Import the `.slint` file as module by treating it like a Python module where the `.slint` extension is replaced with `_slint`:
+2. Use Slint's auto-loader, which lazily loads `.slint` files from `sys.path`:
    ```python
-   import slint # needs to come first
-   from ui_slint import MainWindow
-   main_window = MainWindow()
+   import slint
+   # Look for for `app.slint` in `sys.path`:
+   main_window = slint.loader.app.MainWindow()
    ```
 
+   Any attribute lookup in `slint.loader` is searched for in `sys.path`. If a directory with the name exists, it is returned as a loader object, and subsequent
+   attribute lookups follow the same logic. If the name matches a file with the `.slint` extension, it is automatically loaded with `load_file` and the
+   [namespace](https://docs.python.org/3/library/types.html#types.SimpleNamespace) is returned.
+
 ### Accessing Properties
 
 [Properties](../slint/src/language/syntax/properties) declared as `out` or `in-out` in `.slint` files are visible as  properties on the component instance.
 
 ```python
 main_window.counter = 42
 print(main_window.counter)
```

### Comparing `slint-1.6.0a5/api/python/brush.rs` & `slint-1.6.0a6/api/python/brush.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/errors.rs` & `slint-1.6.0a6/api/python/errors.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/image.rs` & `slint-1.6.0a6/api/python/image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/interpreter.rs` & `slint-1.6.0a6/api/python/interpreter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/lib.rs` & `slint-1.6.0a6/api/python/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/models.rs` & `slint-1.6.0a6/api/python/models.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/slint/__init__.py` & `slint-1.6.0a6/api/python/slint/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -185,38 +185,39 @@
 
     module = types.SimpleNamespace()
     setattr(module, compdef.name, wrapper_class)
 
     return module
 
 
-class SlintModuleLoader:
-    def create_module(self, spec):
-        return None
-
-    def exec_module(self, module):
-        m = load_file(module.__name__)
-        module.__dict__.update(m.__dict__)
-
-
-class SlintModuleFinder:
-    def find_spec(self, name, path, target=None):
-        if "." in name:
-            return None
+class SlintAutoLoader:
+    def __init__(self, base_dir=None):
+        if base_dir:
+            self.local_dirs = [base_dir]
+        else:
+            self.local_dirs = None
+
+    def __getattr__(self, name):
+        for path in self.local_dirs or sys.path:
+            dir_candidate = os.path.join(path, name)
+            if os.path.isdir(dir_candidate):
+                loader = SlintAutoLoader(dir_candidate)
+                setattr(self, name, loader)
+                return loader
+
+            file_candidate = dir_candidate + ".slint"
+            if os.path.isfile(file_candidate):
+                type_namespace = load_file(file_candidate)
+                setattr(self, name, type_namespace)
+                return type_namespace
 
-        if not name.endswith("_slint"):
-            return None
+        return None
 
-        candidate_filename = name.removesuffix("_slint") + ".slint"
 
-        for path in sys.path:
-            candidate = os.path.join(path, candidate_filename)
-            if os.path.exists(candidate):
-                return ModuleSpec(os.path.realpath(candidate), SlintModuleLoader())
-        return None
+loader = SlintAutoLoader()
 
 
 def _callback_decorator(callable, info):
     if "name" not in info:
         info["name"] = callable.__name__
     setattr(callable, "slint.callback", info)
     return callable
@@ -231,16 +232,14 @@
         if name:
             info["name"] = name
         if global_name:
             info["global_name"] = global_name
         return lambda callback: _callback_decorator(callback, info)
 
 
-sys.meta_path.append(SlintModuleFinder())
-
 Image = native.PyImage
 Color = native.PyColor
 Brush = native.PyBrush
 Model = native.PyModelBase
 ListModel = models.ListModel
 Model = models.Model
 Timer = native.Timer
```

### Comparing `slint-1.6.0a5/api/python/slint/models.py` & `slint-1.6.0a6/api/python/slint/models.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/tests/test_brush.py` & `slint-1.6.0a6/api/python/tests/test_brush.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/tests/test_callback_decorators.py` & `slint-1.6.0a6/api/python/tests/test_callback_decorators.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/tests/test_compiler.py` & `slint-1.6.0a6/api/python/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/tests/test_gc.py` & `slint-1.6.0a6/api/python/tests/test_gc.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/tests/test_import.py` & `slint-1.6.0a6/api/python/tests/test_loader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # Copyright © SixtyFPS GmbH <info@slint.dev>
 # SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 import pytest
 from slint import slint as native
+from slint import loader
 import sys
 import os
 
 
 def test_magic_import():
-    import test_load_file_slint as compiledmodule
-    instance = compiledmodule.App()
+    instance = loader.test_load_file.App()
     del instance
 
 
 def test_magic_import_path():
     oldsyspath = sys.path
-    with pytest.raises(ModuleNotFoundError, match="No module named 'printerdemo_slint'"):
-        import printerdemo_slint
+    assert loader.printerdemo == None
     try:
         sys.path.append(os.path.join(os.path.dirname(__file__),
-                        "..", "..", "..", "examples", "printerdemo", "ui"))
-        import printerdemo_slint
-        instance = printerdemo_slint.MainWindow()
+                        "..", "..", ".."))
+        instance = loader.examples.printerdemo.ui.printerdemo.MainWindow()
         del instance
     finally:
         sys.path = oldsyspath
```

### Comparing `slint-1.6.0a5/api/python/tests/test_instance.py` & `slint-1.6.0a6/api/python/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/tests/test_load_file.py` & `slint-1.6.0a6/api/python/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/tests/test_load_file.slint` & `slint-1.6.0a6/api/python/tests/test_load_file.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/tests/test_models.py` & `slint-1.6.0a6/api/python/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/tests/test_timers.py` & `slint-1.6.0a6/api/python/tests/test_timers.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/timer.rs` & `slint-1.6.0a6/api/python/timer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/api/python/value.rs` & `slint-1.6.0a6/api/python/value.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/Cargo.lock` & `slint-1.6.0a6/Cargo.lock`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/Cargo.toml` & `slint-1.6.0a6/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/pyproject.toml` & `slint-1.6.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["maturin>=1,<2"]
 build-backend = "maturin"
 
 [project]
 name = "slint"
-version = "1.6.0a5"
+version = "1.6.0a6"
 requires-python = ">= 3.10"
 authors = [
     {name = "Slint Team", email = "info@slint.dev"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: MacOS X",
```

### Comparing `slint-1.6.0a5/slint/__init__.py` & `slint-1.6.0a6/slint/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -185,38 +185,39 @@
 
     module = types.SimpleNamespace()
     setattr(module, compdef.name, wrapper_class)
 
     return module
 
 
-class SlintModuleLoader:
-    def create_module(self, spec):
-        return None
-
-    def exec_module(self, module):
-        m = load_file(module.__name__)
-        module.__dict__.update(m.__dict__)
-
-
-class SlintModuleFinder:
-    def find_spec(self, name, path, target=None):
-        if "." in name:
-            return None
+class SlintAutoLoader:
+    def __init__(self, base_dir=None):
+        if base_dir:
+            self.local_dirs = [base_dir]
+        else:
+            self.local_dirs = None
+
+    def __getattr__(self, name):
+        for path in self.local_dirs or sys.path:
+            dir_candidate = os.path.join(path, name)
+            if os.path.isdir(dir_candidate):
+                loader = SlintAutoLoader(dir_candidate)
+                setattr(self, name, loader)
+                return loader
+
+            file_candidate = dir_candidate + ".slint"
+            if os.path.isfile(file_candidate):
+                type_namespace = load_file(file_candidate)
+                setattr(self, name, type_namespace)
+                return type_namespace
 
-        if not name.endswith("_slint"):
-            return None
+        return None
 
-        candidate_filename = name.removesuffix("_slint") + ".slint"
 
-        for path in sys.path:
-            candidate = os.path.join(path, candidate_filename)
-            if os.path.exists(candidate):
-                return ModuleSpec(os.path.realpath(candidate), SlintModuleLoader())
-        return None
+loader = SlintAutoLoader()
 
 
 def _callback_decorator(callable, info):
     if "name" not in info:
         info["name"] = callable.__name__
     setattr(callable, "slint.callback", info)
     return callable
@@ -231,16 +232,14 @@
         if name:
             info["name"] = name
         if global_name:
             info["global_name"] = global_name
         return lambda callback: _callback_decorator(callback, info)
 
 
-sys.meta_path.append(SlintModuleFinder())
-
 Image = native.PyImage
 Color = native.PyColor
 Brush = native.PyBrush
 Model = native.PyModelBase
 ListModel = models.ListModel
 Model = models.Model
 Timer = native.Timer
```

### Comparing `slint-1.6.0a5/slint/models.py` & `slint-1.6.0a6/slint/models.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a5/PKG-INFO` & `slint-1.6.0a6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: slint
-Version: 1.6.0a5
+Version: 1.6.0a6
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: MacOS X
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
@@ -78,15 +78,15 @@
 cd examples/printerdemo/python
 pipenv update
 pipenv run python main.py
 ```
 
 ## Quick Start
 
-1. Add Slint from the Git development branch to your Python project: `pipenv install "git+https://github.com/slint-ui/slint#subdirectory=api/python&egg=slint"`
+1. Add Slint Python Package Index to your Python project: `pipenv install slint`
 2. Create a file called `appwindow.slint`:
 
 ```slint
 import { Button, VerticalBox } from "std-widgets.slint";
 
 export component AppWindow inherits Window {
     in-out property<int> counter: 42;
@@ -105,17 +105,16 @@
 }
 ```
 
 1. Create a file called `main.py`:
 
 ```python
 import slint
-import appwindow_slint
 
-class App(appwindow_slint.AppWindow):
+class App(slint.loader.appwindow.AppWindow):
     @slint.callback
     def request_increase_value(self):
         self.counter = self.counter + 1
 
 app = App()
 app.run()
 ```
@@ -124,15 +123,15 @@
 
 ## API Overview
 
 ### Instantiating a Component
 
 The following example shows how to instantiate a Slint component in Python:
 
-**`ui.slint`**
+**`app.slint`**
 
 ```slint
 export component MainWindow inherits Window {
     callback clicked <=> i-touch-area.clicked;
 
     in property <int> counter;
 
@@ -142,29 +141,33 @@
     i-touch-area := TouchArea {}
 }
 ```
 
 The exported component is exposed as a Python class. To access this class, you have two
 options:
 
-1. Call `slint.load_file("ui.slint")`. The returned object is a [namespace](https://docs.python.org/3/library/types.html#types.SimpleNamespace),
+1. Call `slint.load_file("app.slint")`. The returned object is a [namespace](https://docs.python.org/3/library/types.html#types.SimpleNamespace),
    that provides the `MainWindow` class:
    ```python
    import slint
-   components = slint.load_file("ui.slint")
+   components = slint.load_file("app.slint")
    main_window = components.MainWindow()
    ```
 
-2. Import the `.slint` file as module by treating it like a Python module where the `.slint` extension is replaced with `_slint`:
+2. Use Slint's auto-loader, which lazily loads `.slint` files from `sys.path`:
    ```python
-   import slint # needs to come first
-   from ui_slint import MainWindow
-   main_window = MainWindow()
+   import slint
+   # Look for for `app.slint` in `sys.path`:
+   main_window = slint.loader.app.MainWindow()
    ```
 
+   Any attribute lookup in `slint.loader` is searched for in `sys.path`. If a directory with the name exists, it is returned as a loader object, and subsequent
+   attribute lookups follow the same logic. If the name matches a file with the `.slint` extension, it is automatically loaded with `load_file` and the
+   [namespace](https://docs.python.org/3/library/types.html#types.SimpleNamespace) is returned.
+
 ### Accessing Properties
 
 [Properties](../slint/src/language/syntax/properties) declared as `out` or `in-out` in `.slint` files are visible as  properties on the component instance.
 
 ```python
 main_window.counter = 42
 print(main_window.counter)
```

