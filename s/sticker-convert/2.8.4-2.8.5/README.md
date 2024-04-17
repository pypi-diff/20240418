# Comparing `tmp/sticker_convert-2.8.4.tar.gz` & `tmp/sticker_convert-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sticker_convert-2.8.4.tar", last modified: Fri Apr 12 16:58:55 2024, max compression
+gzip compressed data, was "sticker_convert-2.8.5.tar", last modified: Wed Apr 17 22:08:16 2024, max compression
```

## Comparing `sticker_convert-2.8.4.tar` & `sticker_convert-2.8.5.tar`

### file list

```diff
@@ -1,143 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.810012 sticker_convert-2.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49307 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26818 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:58:55.810012 sticker_convert-2.8.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.782012 sticker_convert-2.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.790012 sticker_convert-2.8.4/src/sticker_convert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18579 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37353 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.790012 sticker_convert-2.8.4/src/sticker_convert/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2726 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/download_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8516 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/download_kakao.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17853 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/download_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3063 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/download_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4614 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/downloaders/download_telegram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30707 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.790012 sticker_convert-2.8.4/src/sticker_convert/gui_components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.790012 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/comp_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/config_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/control_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/cred_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/input_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/output_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/progress_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/right_clicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/gui_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.790012 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31688 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/advanced_compression_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/base_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/line_get_auth_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/signal_get_auth_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.794012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.798012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.798012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.786012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.798012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/
--rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.786012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.786012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.798012 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/xcschememanagement.plist
--rwxr-xr-x   0 runner    (1001) docker     (127)    25608 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7732 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/job_option.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127) 10353636 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/NotoColorEmoji.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)     5404 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/appicon.icns
--rwxr-xr-x   0 runner    (1001) docker     (127)    38078 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/appicon.ico
--rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/appicon.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    11163 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/compression.json
--rw-r--r--   0 runner    (1001) docker     (127)   413367 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/emoji.json
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/help.json
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/input.json
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/resources/output.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/uploaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/compress_wastickers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6396 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15695 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_telegram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11254 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/uploaders/xcode_imessage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/utils/auth/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9829 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_kakao_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_line_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4925 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_signal_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/utils/files/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/cache_store.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/json_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/json_resources_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10088 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/metadata_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/run_bin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2156 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/files/sanitize_filename.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert/utils/media/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/media/apple_png_normalize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/media/codec_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/media/decrypt_kakao.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5732 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/media/format_verify.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/utils/url_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/src/sticker_convert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/src/sticker_convert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49307 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 16:58:55.000000 sticker_convert-2.8.4/src/sticker_convert.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:58:55.806012 sticker_convert-2.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-12 16:58:51.000000 sticker_convert-2.8.4/tests/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.581385 sticker_convert-2.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    49868 2024-04-17 22:08:16.581385 sticker_convert-2.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27377 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 22:08:16.581385 sticker_convert-2.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.553385 sticker_convert-2.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.561385 sticker_convert-2.8.5/src/sticker_convert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18621 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37353 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.561385 sticker_convert-2.8.5/src/sticker_convert/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/downloaders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3980 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/downloaders/download_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8516 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/downloaders/download_kakao.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17853 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/downloaders/download_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3063 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/downloaders/download_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4614 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/downloaders/download_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/downloaders/download_viber.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30707 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.561385 sticker_convert-2.8.5/src/sticker_convert/gui_components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.561385 sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/comp_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/config_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/control_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/cred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/input_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/output_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/progress_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/right_clicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/gui_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.565385 sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31688 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/advanced_compression_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/line_get_auth_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/signal_get_auth_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.565385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.565385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.565385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.565385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.565385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.565385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.565385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.565385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.565385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.569385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.569385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.569385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.569385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.557385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.569385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/
+-rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.557385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.557385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.569385 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/xcschememanagement.plist
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25775 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7732 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/job_option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.577385 sticker_convert-2.8.5/src/sticker_convert/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127) 10353636 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/resources/NotoColorEmoji.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5404 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/resources/appicon.icns
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38078 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/resources/appicon.ico
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/resources/appicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12156 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/resources/compression.json
+-rw-r--r--   0 runner    (1001) docker     (127)   413367 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/resources/emoji.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/resources/help.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/resources/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/resources/output.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.577385 sticker_convert-2.8.5/src/sticker_convert/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/uploaders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/uploaders/compress_wastickers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/uploaders/upload_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6396 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/uploaders/upload_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15695 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/uploaders/upload_telegram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11254 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/uploaders/xcode_imessage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.577385 sticker_convert-2.8.5/src/sticker_convert/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.577385 sticker_convert-2.8.5/src/sticker_convert/utils/auth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9829 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/auth/get_kakao_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/auth/get_line_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4925 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/auth/get_signal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.581385 sticker_convert-2.8.5/src/sticker_convert/utils/files/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/files/cache_store.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/files/json_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/files/json_resources_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10088 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/files/metadata_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/files/run_bin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2156 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/files/sanitize_filename.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.581385 sticker_convert-2.8.5/src/sticker_convert/utils/media/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/media/apple_png_normalize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/media/codec_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/media/decrypt_kakao.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5732 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/media/format_verify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      769 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/utils/url_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/src/sticker_convert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.581385 sticker_convert-2.8.5/src/sticker_convert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49868 2024-04-17 22:08:16.000000 sticker_convert-2.8.5/src/sticker_convert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-17 22:08:16.000000 sticker_convert-2.8.5/src/sticker_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 22:08:16.000000 sticker_convert-2.8.5/src/sticker_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-17 22:08:16.000000 sticker_convert-2.8.5/src/sticker_convert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-17 22:08:16.000000 sticker_convert-2.8.5/src/sticker_convert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 22:08:16.000000 sticker_convert-2.8.5/src/sticker_convert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:08:16.581385 sticker_convert-2.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14721 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-17 22:08:10.000000 sticker_convert-2.8.5/tests/test_export.py
```

### Comparing `sticker_convert-2.8.4/LICENSE` & `sticker_convert-2.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/PKG-INFO` & `sticker_convert-2.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sticker-convert
-Version: 2.8.4
+Version: 2.8.5
 Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, iMessage. Written in Python.
 Author-email: laggykiller <chaudominic2@gmail.com>
 Maintainer-email: laggykiller <chaudominic2@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -345,15 +345,15 @@
         Public License instead of this License.
         
 Project-URL: Homepage, https://github.com/laggykiller/sticker-convert
 Project-URL: Source, https://github.com/laggykiller/sticker-convert
 Project-URL: Documentation, https://github.com/laggykiller/sticker-convert
 Project-URL: Tracker, https://github.com/laggykiller/sticker-convert/issues
 Project-URL: Repository, https://github.com/laggykiller/sticker-convert
-Keywords: telegram,line,tgs,whatsapp,kakao,signal,imessage,wastickers
+Keywords: telegram,line,tgs,whatsapp,kakao,signal,imessage,wastickers,viber
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -365,15 +365,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiolimiter~=1.1.0
 Requires-Dist: anyio~=4.3.0
 Requires-Dist: apngasm_python~=1.2.3
 Requires-Dist: av~=12.0.0
 Requires-Dist: beautifulsoup4~=4.12.3
-Requires-Dist: rookiepy~=0.3.7
+Requires-Dist: rookiepy~=0.4.0
 Requires-Dist: imagequant~=1.1.1
 Requires-Dist: memory-tempfile~=2.2.3
 Requires-Dist: mergedeep~=1.3.4
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: Pillow~=10.3.0
 Requires-Dist: pyoxipng~=9.0.0
 Requires-Dist: python-telegram-bot~=21.1
@@ -387,15 +387,15 @@
 
 # sticker-convert
 ![imgs/banner.png](imgs/banner.png)
 ![imgs/screenshot](imgs/screenshot.png)
 
 - A python script for creating, downloading, converting+compressing and uploading stickers from multiple instant messaging applications.
 - With GUI and CLI that runs on Windows, MacOS and Linux
-- Currently supports Signal, Telegram, WhatsApp (Create .wastickers), Line (Download only), Kakao (Download only), iMessage (Create Xcode sticker pack project)
+- Currently supports Signal, Telegram, WhatsApp (Create .wastickers), Line (Download only), Kakao (Download only), Viber (Download only), iMessage (Create Xcode sticker pack project)
 - Supports static and animated stickers, with transparency support
 
 ## Downloads
 - [Pre-compiled releases](https://github.com/laggykiller/sticker-convert/releases) for Windows, MacOS and Linux (As AppImage).
     - Windows: Unzip the downloaded file and run `sticker-convert.exe`
     - MacOS: Unzip the downloaded file, hold control and open `hold_control_and_click_open_me.command` for the first time, then `sticker-convert.app` in the future
     - Linux: `chmod +x` the downloaded AppImage and run it
@@ -425,14 +425,15 @@
 | Application                           | ⬇️ Download                         | ⬆️ Upload                                          |
 | ------------------------------------- | ------------------------------------| --------------------------------------------------- |
 | [Signal](docs/guide_signal.md)        | ✅                                  | ✅ (Require `uuid` & `password` or manually)       |
 | [Telegram](docs/guide_telegram.md)    | ✅ (Require `token`)                | ✅ (Require `token` & `user_id` or manually)       |
 | [WhatsApp](docs/guide_whatsapp.md)    | ⭕ (By Android or WhatsApp Web)     | ⭕ (Create `.wastickers`, import by Sticker Maker) |
 | [Line](docs/guide_line.md)            | ✅                                  | 🚫 (Need to submit for manual approval)            |
 | [Kakao](docs/guide_kakao.md)          | ✅ (Need 'share link' for animated) | 🚫 (Need to submit for manual approval)            |
+| [Viber](docs/guide_viber.md)          | ✅                                  | 🚫 (Manually upload through Viber app)             |
 | [iMessage](docs/guide_imessage.md)    | 🚫                                  | ⭕ (Create Xcode stickerpack project for sideload) |
 
 ✅ = Supported ⭕ = Partially supported 🚫 = Not supported
 
 - Signal
     - Download: Supported. (e.g. `https://signal.art/addstickers/#pack_id=xxxxx&pack_key=xxxxx`)
     - Upload: Supported
@@ -451,14 +452,17 @@
         - Search on official site: https://store.line.me/stickershop
         - Search on non-official site (Include region locked and expired packs): http://www.line-stickers.com/
         - For more information: https://github.com/doubleplusc/Line-sticker-downloader
     - Upload: Not supported. You need to manually submit sticker pack for approval before you can use in app.
 - Kakao
     - Download: Supported (e.g. `https://e.kakao.com/t/xxxxx` OR `kakaotalk://store/emoticon/4404400` OR `https://emoticon.kakao.com/items/xxxxx` OR `4404400`). It is rather complicated, learn more from [docs/guide_kakao.md](docs/guide_kakao.md)
     - Upload: Not supported. You need to manually submit sticker pack for approval before you can use in app.
+- Viber
+    - Download: Supported (e.g. `https://stickers.viber.com/pages/example` OR `https://stickers.viber.com/pages/custom-sticker-packs/example`)
+    - Upload: The program can convert images to png with 490x490 for uploading to viber manually. It should be noted that Viber is able to resize images for you, so it may not be necessary to use sticker-convert for creating Viber sticker pack.
 - iMessage
     - Download: Not supported.
     - Upload: The program can create Xcode project for iMessage sticker pack, which could then be compiled and sideloaded using Xcode.
 
 ## How to use (GUI)
 1. Run `sticker-convert.exe`, `sticker-convert.app` or `python3 src/sticker-convert.py`
 2. Choose input source.
```

### Comparing `sticker_convert-2.8.4/README.md` & `sticker_convert-2.8.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # sticker-convert
 ![imgs/banner.png](imgs/banner.png)
 ![imgs/screenshot](imgs/screenshot.png)
 
 - A python script for creating, downloading, converting+compressing and uploading stickers from multiple instant messaging applications.
 - With GUI and CLI that runs on Windows, MacOS and Linux
-- Currently supports Signal, Telegram, WhatsApp (Create .wastickers), Line (Download only), Kakao (Download only), iMessage (Create Xcode sticker pack project)
+- Currently supports Signal, Telegram, WhatsApp (Create .wastickers), Line (Download only), Kakao (Download only), Viber (Download only), iMessage (Create Xcode sticker pack project)
 - Supports static and animated stickers, with transparency support
 
 ## Downloads
 - [Pre-compiled releases](https://github.com/laggykiller/sticker-convert/releases) for Windows, MacOS and Linux (As AppImage).
     - Windows: Unzip the downloaded file and run `sticker-convert.exe`
     - MacOS: Unzip the downloaded file, hold control and open `hold_control_and_click_open_me.command` for the first time, then `sticker-convert.app` in the future
     - Linux: `chmod +x` the downloaded AppImage and run it
@@ -38,14 +38,15 @@
 | Application                           | ⬇️ Download                         | ⬆️ Upload                                          |
 | ------------------------------------- | ------------------------------------| --------------------------------------------------- |
 | [Signal](docs/guide_signal.md)        | ✅                                  | ✅ (Require `uuid` & `password` or manually)       |
 | [Telegram](docs/guide_telegram.md)    | ✅ (Require `token`)                | ✅ (Require `token` & `user_id` or manually)       |
 | [WhatsApp](docs/guide_whatsapp.md)    | ⭕ (By Android or WhatsApp Web)     | ⭕ (Create `.wastickers`, import by Sticker Maker) |
 | [Line](docs/guide_line.md)            | ✅                                  | 🚫 (Need to submit for manual approval)            |
 | [Kakao](docs/guide_kakao.md)          | ✅ (Need 'share link' for animated) | 🚫 (Need to submit for manual approval)            |
+| [Viber](docs/guide_viber.md)          | ✅                                  | 🚫 (Manually upload through Viber app)             |
 | [iMessage](docs/guide_imessage.md)    | 🚫                                  | ⭕ (Create Xcode stickerpack project for sideload) |
 
 ✅ = Supported ⭕ = Partially supported 🚫 = Not supported
 
 - Signal
     - Download: Supported. (e.g. `https://signal.art/addstickers/#pack_id=xxxxx&pack_key=xxxxx`)
     - Upload: Supported
@@ -64,14 +65,17 @@
         - Search on official site: https://store.line.me/stickershop
         - Search on non-official site (Include region locked and expired packs): http://www.line-stickers.com/
         - For more information: https://github.com/doubleplusc/Line-sticker-downloader
     - Upload: Not supported. You need to manually submit sticker pack for approval before you can use in app.
 - Kakao
     - Download: Supported (e.g. `https://e.kakao.com/t/xxxxx` OR `kakaotalk://store/emoticon/4404400` OR `https://emoticon.kakao.com/items/xxxxx` OR `4404400`). It is rather complicated, learn more from [docs/guide_kakao.md](docs/guide_kakao.md)
     - Upload: Not supported. You need to manually submit sticker pack for approval before you can use in app.
+- Viber
+    - Download: Supported (e.g. `https://stickers.viber.com/pages/example` OR `https://stickers.viber.com/pages/custom-sticker-packs/example`)
+    - Upload: The program can convert images to png with 490x490 for uploading to viber manually. It should be noted that Viber is able to resize images for you, so it may not be necessary to use sticker-convert for creating Viber sticker pack.
 - iMessage
     - Download: Not supported.
     - Upload: The program can create Xcode project for iMessage sticker pack, which could then be compiled and sideloaded using Xcode.
 
 ## How to use (GUI)
 1. Run `sticker-convert.exe`, `sticker-convert.app` or `python3 src/sticker-convert.py`
 2. Choose input source.
```

### Comparing `sticker_convert-2.8.4/pyproject.toml` & `sticker_convert-2.8.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "sticker-convert"
 description = "Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, iMessage. Written in Python."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
-keywords = ["telegram", "line", "tgs", "whatsapp", "kakao", "signal", "imessage", "wastickers"]
+keywords = ["telegram", "line", "tgs", "whatsapp", "kakao", "signal", "imessage", "wastickers", "viber"]
 authors = [
   {name = "laggykiller", email = "chaudominic2@gmail.com" } # Optional
 ]
 maintainers = [
   {name = "laggykiller", email = "chaudominic2@gmail.com" } # Optional
 ]
 classifiers = [
```

### Comparing `sticker_convert-2.8.4/src/sticker_convert/cli.py` & `sticker_convert-2.8.5/src/sticker_convert/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,15 @@
     def get_opt_input(self, args: Namespace) -> InputOption:
         download_options = {
             "auto": args.download_auto,
             "signal": args.download_signal,
             "line": args.download_line,
             "telegram": args.download_telegram,
             "kakao": args.download_kakao,
+            "viber": args.download_viber,
         }
 
         download_option = "local"
         url = ""
         for k, v in download_options.items():
             if v:
                 download_option = k
```

### Comparing `sticker_convert-2.8.4/src/sticker_convert/converter.py` & `sticker_convert-2.8.5/src/sticker_convert/converter.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/definitions.py` & `sticker_convert-2.8.5/src/sticker_convert/definitions.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/downloaders/download_base.py` & `sticker_convert-2.8.5/src/sticker_convert/downloaders/download_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any, List, Optional, Tuple
 
+import anyio
 import requests
 
 from sticker_convert.job_option import CredOption
 from sticker_convert.utils.callback import CallbackProtocol, CallbackReturn
 
 
 class DownloadBase:
@@ -24,41 +25,77 @@
         self.opt_cred = opt_cred
         self.cb = cb
         self.cb_return = cb_return
 
     def download_multiple_files(
         self, targets: List[Tuple[str, Path]], retries: int = 3, **kwargs: Any
     ) -> None:
+        anyio.run(self.download_multiple_files_async, targets, retries, **kwargs)
+
+    async def download_multiple_files_async(
+        self, targets: List[Tuple[str, Path]], retries: int = 3, **kwargs: Any
+    ) -> None:
         # targets format: [(url1, dest2), (url2, dest2), ...]
         self.cb.put(
             ("bar", None, {"set_progress_mode": "determinate", "steps": len(targets)})
         )
 
-        for url, dest in targets:
-            self.download_file(url, dest, retries, show_progress=False, **kwargs)
+        async with anyio.create_task_group() as tg:
+            for url, dest in targets:
+                tg.start_soon(self.download_file_async, url, dest, retries, **kwargs)
+
+    async def download_file_async(
+        self,
+        url: str,
+        dest: Path,
+        retries: int = 3,
+        **kwargs: Any,
+    ) -> None:
+        for retry in range(retries):
+            try:
+                response = requests.get(url, allow_redirects=True, **kwargs)
+
+                if not response.ok:
+                    self.cb.put("update_bar")
+                    raise requests.exceptions.RequestException(
+                        f"Error {response.status_code}"
+                    )
+
+                self.cb.put(f"Downloading {url}")
+                with open(dest, "wb+") as f:
+                    f.write(response.content)
+                self.cb.put(f"Downloaded {url}")
+                break
+
+            except requests.exceptions.RequestException as e:
+                self.cb.put(
+                    f"Cannot download {url} (tried {retry+1}/{retries} times): {e}"
+                )
 
-            self.cb.put("update_bar")
+        self.cb.put("update_bar")
 
     def download_file(
         self,
         url: str,
         dest: Optional[Path] = None,
         retries: int = 3,
         show_progress: bool = True,
         **kwargs: Any,
     ) -> bytes:
         result = b""
         chunk_size = 102400
 
         for retry in range(retries):
             try:
-                response = requests.get(url, stream=True, **kwargs)
+                response = requests.get(
+                    url, stream=True, allow_redirects=True, **kwargs
+                )
                 total_length = int(response.headers.get("content-length"))  # type: ignore
 
-                if response.status_code != 200:
+                if not response.ok:
                     return b""
                 self.cb.put(f"Downloading {url}")
 
                 if show_progress:
                     steps = (total_length / chunk_size) + 1
                     self.cb.put(
                         (
@@ -71,20 +108,20 @@
                 for chunk in response.iter_content(chunk_size=chunk_size):
                     if chunk:
                         result += chunk
                         if show_progress:
                             self.cb.put("update_bar")
 
                 break
-            except requests.exceptions.RequestException:
-                msg = f"Cannot download {url} (tried {retry+1}/{retries} times)"
-                self.cb.put(msg)
+            except requests.exceptions.RequestException as e:
+                self.cb.put(
+                    f"Cannot download {url} (tried {retry+1}/{retries} times): {e}"
+                )
 
         if not result:
             return b""
         if dest:
             with open(dest, "wb+") as f:
                 f.write(result)
-            msg = f"Downloaded {url}"
-            self.cb.put(msg)
+            self.cb.put(f"Downloaded {url}")
             return b""
         return result
```

### Comparing `sticker_convert-2.8.4/src/sticker_convert/downloaders/download_kakao.py` & `sticker_convert-2.8.5/src/sticker_convert/downloaders/download_kakao.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/downloaders/download_line.py` & `sticker_convert-2.8.5/src/sticker_convert/downloaders/download_line.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/downloaders/download_signal.py` & `sticker_convert-2.8.5/src/sticker_convert/downloaders/download_signal.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/downloaders/download_telegram.py` & `sticker_convert-2.8.5/src/sticker_convert/downloaders/download_telegram.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui.py` & `sticker_convert-2.8.5/src/sticker_convert/gui.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/comp_frame.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/comp_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/config_frame.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/config_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/control_frame.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/control_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/cred_frame.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/cred_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/input_frame.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/input_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/output_frame.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/output_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/progress_frame.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/progress_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/frames/right_clicker.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/frames/right_clicker.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/gui_utils.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/gui_utils.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/advanced_compression_window.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/advanced_compression_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/base_window.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/base_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/line_get_auth_window.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/line_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/gui_components/windows/signal_get_auth_window.py` & `sticker_convert-2.8.5/src/sticker_convert/gui_components/windows/signal_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate` & `sticker_convert-2.8.5/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/job.py` & `sticker_convert-2.8.5/src/sticker_convert/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from urllib.parse import urlparse
 
 from sticker_convert.converter import StickerConvert
 from sticker_convert.downloaders.download_kakao import DownloadKakao
 from sticker_convert.downloaders.download_line import DownloadLine
 from sticker_convert.downloaders.download_signal import DownloadSignal
 from sticker_convert.downloaders.download_telegram import DownloadTelegram
+from sticker_convert.downloaders.download_viber import DownloadViber
 from sticker_convert.job_option import CompOption, CredOption, InputOption, OutputOption
 from sticker_convert.uploaders.compress_wastickers import CompressWastickers
 from sticker_convert.uploaders.upload_signal import UploadSignal
 from sticker_convert.uploaders.upload_telegram import UploadTelegram
 from sticker_convert.uploaders.xcode_imessage import XcodeImessage
 from sticker_convert.utils.callback import CallbackReturn, CbQueueType, ResultsListType, WorkQueueType
 from sticker_convert.utils.files.json_resources_loader import OUTPUT_JSON
@@ -523,14 +524,17 @@
 
         if self.opt_input.option == "telegram":
             downloaders.append(DownloadTelegram.start)
 
         if self.opt_input.option == "kakao":
             downloaders.append(DownloadKakao.start)
 
+        if self.opt_input.option == "viber":
+            downloaders.append(DownloadViber.start)
+
         if len(downloaders) > 0:
             self.executor.cb("Downloading...")
         else:
             self.executor.cb("Nothing to download")
             return True
 
         self.executor.start_workers(processes=1)
```

### Comparing `sticker_convert-2.8.4/src/sticker_convert/job_option.py` & `sticker_convert-2.8.5/src/sticker_convert/job_option.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/resources/NotoColorEmoji.ttf` & `sticker_convert-2.8.5/src/sticker_convert/resources/NotoColorEmoji.ttf`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/resources/appicon.icns` & `sticker_convert-2.8.5/src/sticker_convert/resources/appicon.icns`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/resources/appicon.ico` & `sticker_convert-2.8.5/src/sticker_convert/resources/appicon.ico`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/resources/appicon.png` & `sticker_convert-2.8.5/src/sticker_convert/resources/appicon.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/resources/compression.json` & `sticker_convert-2.8.5/src/sticker_convert/resources/compression.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'viber'": "OrderedDict([('size_max', OrderedDict([('img', 0), ('vid', 0)])), ('format', "*

 * *            "OrderedDict([('img', '.png'), ('vid', '.png')])), ('fps', OrderedDict([('min', 1), "*

 * *            "('max', 1), ('power', 1)])), ('res', OrderedDict([('w', OrderedDict([('min', 490), "*

 * *            "('max', 490)])), ('h', OrderedDict([('min', 490), ('max', 490)])), ('power', 1)])), "*

 * *            "('quality', OrderedDict([('min', 95), ('max', 95), ('power', 1)])), ('color', "*

 * *            "OrderedDict([('min' […]*

```diff
@@ -465,14 +465,61 @@
         "scale_filter": "bicubic",
         "size_max": {
             "img": 512000,
             "vid": 256000
         },
         "steps": 16
     },
+    "viber": {
+        "bg_color": "",
+        "color": {
+            "max": 257,
+            "min": 257,
+            "power": 1
+        },
+        "default_emoji": "\ud83d\ude00",
+        "duration": {
+            "max": 0,
+            "min": 0
+        },
+        "fake_vid": false,
+        "format": {
+            "img": ".png",
+            "vid": ".png"
+        },
+        "fps": {
+            "max": 1,
+            "min": 1,
+            "power": 1
+        },
+        "padding_percent": 0,
+        "quality": {
+            "max": 95,
+            "min": 95,
+            "power": 1
+        },
+        "quantize_method": "imagequant",
+        "res": {
+            "h": {
+                "max": 490,
+                "min": 490
+            },
+            "power": 1,
+            "w": {
+                "max": 490,
+                "min": 490
+            }
+        },
+        "scale_filter": "bicubic",
+        "size_max": {
+            "img": 0,
+            "vid": 0
+        },
+        "steps": 1
+    },
     "whatsapp": {
         "bg_color": "",
         "color": {
             "max": 257,
             "min": 32,
             "power": 3
         },
```

### Comparing `sticker_convert-2.8.4/src/sticker_convert/resources/emoji.json` & `sticker_convert-2.8.5/src/sticker_convert/resources/emoji.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/resources/help.json` & `sticker_convert-2.8.5/src/sticker_convert/resources/help.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/resources/input.json` & `sticker_convert-2.8.5/src/sticker_convert/resources/input.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'viber'": "OrderedDict([('full_name', 'Download from Viber'), ('help', 'Download viber stickers "*

 * *            "from a URL as input'), ('example', 'Example: https://stickers.viber.com/pages/example "*

 * *            "OR https://stickers.viber.com/pages/custom-sticker-packs/example'), ('address_lbls', "*

 * *            "'URL address / ID'), ('metadata_provides', OrderedDict([('title', True), ('author', "*

 * *            'False)]))])'}*

```diff
@@ -54,9 +54,19 @@
         "example": "Example: https://telegram.me/addstickers/xxxxx\n OR https://telegram.me/addemoji/xxxxx",
         "full_name": "Download from Telegram",
         "help": "Download telegram stickers from a URL as input",
         "metadata_provides": {
             "author": false,
             "title": true
         }
+    },
+    "viber": {
+        "address_lbls": "URL address / ID",
+        "example": "Example: https://stickers.viber.com/pages/example OR https://stickers.viber.com/pages/custom-sticker-packs/example",
+        "full_name": "Download from Viber",
+        "help": "Download viber stickers from a URL as input",
+        "metadata_provides": {
+            "author": false,
+            "title": true
+        }
     }
 }
```

### Comparing `sticker_convert-2.8.4/src/sticker_convert/resources/output.json` & `sticker_convert-2.8.5/src/sticker_convert/resources/output.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/uploaders/compress_wastickers.py` & `sticker_convert-2.8.5/src/sticker_convert/uploaders/compress_wastickers.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_base.py` & `sticker_convert-2.8.5/src/sticker_convert/uploaders/upload_base.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_signal.py` & `sticker_convert-2.8.5/src/sticker_convert/uploaders/upload_signal.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/uploaders/upload_telegram.py` & `sticker_convert-2.8.5/src/sticker_convert/uploaders/upload_telegram.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/uploaders/xcode_imessage.py` & `sticker_convert-2.8.5/src/sticker_convert/uploaders/xcode_imessage.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_kakao_auth.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/auth/get_kakao_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_line_auth.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/auth/get_line_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/auth/get_signal_auth.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/auth/get_signal_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/callback.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/callback.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/files/cache_store.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/files/cache_store.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/files/json_manager.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/files/json_manager.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/files/json_resources_loader.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/files/json_resources_loader.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/files/metadata_handler.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/files/metadata_handler.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/files/run_bin.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/files/run_bin.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/files/sanitize_filename.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/files/sanitize_filename.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/media/apple_png_normalize.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/media/apple_png_normalize.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/media/codec_info.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/media/codec_info.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/media/decrypt_kakao.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/media/decrypt_kakao.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/media/format_verify.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/media/format_verify.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert/utils/url_detect.py` & `sticker_convert-2.8.5/src/sticker_convert/utils/url_detect.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/src/sticker_convert.egg-info/PKG-INFO` & `sticker_convert-2.8.5/src/sticker_convert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sticker-convert
-Version: 2.8.4
+Version: 2.8.5
 Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, iMessage. Written in Python.
 Author-email: laggykiller <chaudominic2@gmail.com>
 Maintainer-email: laggykiller <chaudominic2@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -345,15 +345,15 @@
         Public License instead of this License.
         
 Project-URL: Homepage, https://github.com/laggykiller/sticker-convert
 Project-URL: Source, https://github.com/laggykiller/sticker-convert
 Project-URL: Documentation, https://github.com/laggykiller/sticker-convert
 Project-URL: Tracker, https://github.com/laggykiller/sticker-convert/issues
 Project-URL: Repository, https://github.com/laggykiller/sticker-convert
-Keywords: telegram,line,tgs,whatsapp,kakao,signal,imessage,wastickers
+Keywords: telegram,line,tgs,whatsapp,kakao,signal,imessage,wastickers,viber
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -365,15 +365,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiolimiter~=1.1.0
 Requires-Dist: anyio~=4.3.0
 Requires-Dist: apngasm_python~=1.2.3
 Requires-Dist: av~=12.0.0
 Requires-Dist: beautifulsoup4~=4.12.3
-Requires-Dist: rookiepy~=0.3.7
+Requires-Dist: rookiepy~=0.4.0
 Requires-Dist: imagequant~=1.1.1
 Requires-Dist: memory-tempfile~=2.2.3
 Requires-Dist: mergedeep~=1.3.4
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: Pillow~=10.3.0
 Requires-Dist: pyoxipng~=9.0.0
 Requires-Dist: python-telegram-bot~=21.1
@@ -387,15 +387,15 @@
 
 # sticker-convert
 ![imgs/banner.png](imgs/banner.png)
 ![imgs/screenshot](imgs/screenshot.png)
 
 - A python script for creating, downloading, converting+compressing and uploading stickers from multiple instant messaging applications.
 - With GUI and CLI that runs on Windows, MacOS and Linux
-- Currently supports Signal, Telegram, WhatsApp (Create .wastickers), Line (Download only), Kakao (Download only), iMessage (Create Xcode sticker pack project)
+- Currently supports Signal, Telegram, WhatsApp (Create .wastickers), Line (Download only), Kakao (Download only), Viber (Download only), iMessage (Create Xcode sticker pack project)
 - Supports static and animated stickers, with transparency support
 
 ## Downloads
 - [Pre-compiled releases](https://github.com/laggykiller/sticker-convert/releases) for Windows, MacOS and Linux (As AppImage).
     - Windows: Unzip the downloaded file and run `sticker-convert.exe`
     - MacOS: Unzip the downloaded file, hold control and open `hold_control_and_click_open_me.command` for the first time, then `sticker-convert.app` in the future
     - Linux: `chmod +x` the downloaded AppImage and run it
@@ -425,14 +425,15 @@
 | Application                           | ⬇️ Download                         | ⬆️ Upload                                          |
 | ------------------------------------- | ------------------------------------| --------------------------------------------------- |
 | [Signal](docs/guide_signal.md)        | ✅                                  | ✅ (Require `uuid` & `password` or manually)       |
 | [Telegram](docs/guide_telegram.md)    | ✅ (Require `token`)                | ✅ (Require `token` & `user_id` or manually)       |
 | [WhatsApp](docs/guide_whatsapp.md)    | ⭕ (By Android or WhatsApp Web)     | ⭕ (Create `.wastickers`, import by Sticker Maker) |
 | [Line](docs/guide_line.md)            | ✅                                  | 🚫 (Need to submit for manual approval)            |
 | [Kakao](docs/guide_kakao.md)          | ✅ (Need 'share link' for animated) | 🚫 (Need to submit for manual approval)            |
+| [Viber](docs/guide_viber.md)          | ✅                                  | 🚫 (Manually upload through Viber app)             |
 | [iMessage](docs/guide_imessage.md)    | 🚫                                  | ⭕ (Create Xcode stickerpack project for sideload) |
 
 ✅ = Supported ⭕ = Partially supported 🚫 = Not supported
 
 - Signal
     - Download: Supported. (e.g. `https://signal.art/addstickers/#pack_id=xxxxx&pack_key=xxxxx`)
     - Upload: Supported
@@ -451,14 +452,17 @@
         - Search on official site: https://store.line.me/stickershop
         - Search on non-official site (Include region locked and expired packs): http://www.line-stickers.com/
         - For more information: https://github.com/doubleplusc/Line-sticker-downloader
     - Upload: Not supported. You need to manually submit sticker pack for approval before you can use in app.
 - Kakao
     - Download: Supported (e.g. `https://e.kakao.com/t/xxxxx` OR `kakaotalk://store/emoticon/4404400` OR `https://emoticon.kakao.com/items/xxxxx` OR `4404400`). It is rather complicated, learn more from [docs/guide_kakao.md](docs/guide_kakao.md)
     - Upload: Not supported. You need to manually submit sticker pack for approval before you can use in app.
+- Viber
+    - Download: Supported (e.g. `https://stickers.viber.com/pages/example` OR `https://stickers.viber.com/pages/custom-sticker-packs/example`)
+    - Upload: The program can convert images to png with 490x490 for uploading to viber manually. It should be noted that Viber is able to resize images for you, so it may not be necessary to use sticker-convert for creating Viber sticker pack.
 - iMessage
     - Download: Not supported.
     - Upload: The program can create Xcode project for iMessage sticker pack, which could then be compiled and sideloaded using Xcode.
 
 ## How to use (GUI)
 1. Run `sticker-convert.exe`, `sticker-convert.app` or `python3 src/sticker-convert.py`
 2. Choose input source.
```

### Comparing `sticker_convert-2.8.4/src/sticker_convert.egg-info/SOURCES.txt` & `sticker_convert-2.8.5/src/sticker_convert.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/sticker_convert.egg-info/top_level.txt
 src/sticker_convert/downloaders/__init__.py
 src/sticker_convert/downloaders/download_base.py
 src/sticker_convert/downloaders/download_kakao.py
 src/sticker_convert/downloaders/download_line.py
 src/sticker_convert/downloaders/download_signal.py
 src/sticker_convert/downloaders/download_telegram.py
+src/sticker_convert/downloaders/download_viber.py
 src/sticker_convert/gui_components/__init__.py
 src/sticker_convert/gui_components/gui_utils.py
 src/sticker_convert/gui_components/frames/__init__.py
 src/sticker_convert/gui_components/frames/comp_frame.py
 src/sticker_convert/gui_components/frames/config_frame.py
 src/sticker_convert/gui_components/frames/control_frame.py
 src/sticker_convert/gui_components/frames/cred_frame.py
```

### Comparing `sticker_convert-2.8.4/tests/test_compression.py` & `sticker_convert-2.8.5/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.4/tests/test_download.py` & `sticker_convert-2.8.5/tests/test_download.py`

 * *Files 8% similar despite different names*

```diff
@@ -408,7 +408,49 @@
         url="https://emoticon.kakao.com/items/lV6K2fWmU7CpXlHcP9-ysQJx9rg=?referer=share_link",
         expected_file_count=24,
         expected_file_formats=[".png"],
         with_title=True,
         with_author=True,
         with_emoji=False,
     )
+
+
+@pytest.mark.skipif(not TEST_DOWNLOAD, reason="TEST_DOWNLOAD not set")
+def test_download_viber_custom_sticker_packs(tmp_path: LocalPath) -> None:
+    _run_sticker_convert(
+        tmp_path=tmp_path,
+        source="viber",
+        url="https://stickers.viber.com/pages/custom-sticker-packs/11eefcc8e3c228308e3fafd9b834679a19de752fb5c38390",
+        expected_file_count=2,
+        expected_file_formats=[".png"],
+        with_title=True,
+        with_author=False,
+        with_emoji=False,
+    )
+
+
+@pytest.mark.skipif(not TEST_DOWNLOAD, reason="TEST_DOWNLOAD not set")
+def test_download_viber_official_sticker_packs(tmp_path: LocalPath) -> None:
+    _run_sticker_convert(
+        tmp_path=tmp_path,
+        source="viber",
+        url="https://stickers.viber.com/pages/spring_2024",
+        expected_file_count=14,
+        expected_file_formats=[".png"],
+        with_title=True,
+        with_author=False,
+        with_emoji=False,
+    )
+
+
+@pytest.mark.skipif(not TEST_DOWNLOAD, reason="TEST_DOWNLOAD not set")
+def test_download_viber_official_sound_sticker_packs(tmp_path: LocalPath) -> None:
+    _run_sticker_convert(
+        tmp_path=tmp_path,
+        source="viber",
+        url="https://stickers.viber.com/pages/spring_2024",
+        expected_file_count=24,
+        expected_file_formats=[".png", ".mp3"],
+        with_title=True,
+        with_author=False,
+        with_emoji=False,
+    )
```

### Comparing `sticker_convert-2.8.4/tests/test_export.py` & `sticker_convert-2.8.5/tests/test_export.py`

 * *Files identical despite different names*

