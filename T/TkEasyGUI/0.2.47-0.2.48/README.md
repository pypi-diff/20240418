# Comparing `tmp/tkeasygui-0.2.47.tar.gz` & `tmp/tkeasygui-0.2.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkeasygui-0.2.47.tar", last modified: Wed Apr 17 09:16:08 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.48.tar", last modified: Wed Apr 17 16:23:31 2024, max compression
```

## Comparing `tkeasygui-0.2.47.tar` & `tkeasygui-0.2.48.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-17 09:16:08.102162 tkeasygui-0.2.47/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.47/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-17 09:16:08.101961 tkeasygui-0.2.47/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     3578 2024-04-16 00:24:05.000000 tkeasygui-0.2.47/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-17 09:16:08.099803 tkeasygui-0.2.47/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      329 2024-04-14 07:30:36.000000 tkeasygui-0.2.47/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    17342 2024-04-16 15:46:28.000000 tkeasygui-0.2.47/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      844 2024-04-16 15:46:10.000000 tkeasygui-0.2.47/TkEasyGUI/utils.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-17 09:16:06.000000 tkeasygui-0.2.47/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)   112752 2024-04-17 09:15:28.000000 tkeasygui-0.2.47/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-17 09:16:08.101695 tkeasygui-0.2.47/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-17 09:16:08.000000 tkeasygui-0.2.47/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      300 2024-04-17 09:16:08.000000 tkeasygui-0.2.47/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-17 09:16:08.000000 tkeasygui-0.2.47/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-17 09:16:08.000000 tkeasygui-0.2.47/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-17 09:16:08.000000 tkeasygui-0.2.47/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-17 09:16:02.000000 tkeasygui-0.2.47/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-17 09:16:08.102207 tkeasygui-0.2.47/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-17 16:23:31.866910 tkeasygui-0.2.48/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.48/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-17 16:23:31.866621 tkeasygui-0.2.48/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     3578 2024-04-16 00:24:05.000000 tkeasygui-0.2.48/README.md
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-17 16:23:31.864614 tkeasygui-0.2.48/TkEasyGUI/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      329 2024-04-14 07:30:36.000000 tkeasygui-0.2.48/TkEasyGUI/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    17301 2024-04-17 16:08:20.000000 tkeasygui-0.2.48/TkEasyGUI/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      882 2024-04-17 16:08:20.000000 tkeasygui-0.2.48/TkEasyGUI/utils.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-17 16:23:30.000000 tkeasygui-0.2.48/TkEasyGUI/version.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)   113907 2024-04-17 16:21:10.000000 tkeasygui-0.2.48/TkEasyGUI/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-17 16:23:31.866323 tkeasygui-0.2.48/TkEasyGUI.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     5982 2024-04-17 16:23:31.000000 tkeasygui-0.2.48/TkEasyGUI.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      300 2024-04-17 16:23:31.000000 tkeasygui-0.2.48/TkEasyGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-17 16:23:31.000000 tkeasygui-0.2.48/TkEasyGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-17 16:23:31.000000 tkeasygui-0.2.48/TkEasyGUI.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-17 16:23:31.000000 tkeasygui-0.2.48/TkEasyGUI.egg-info/top_level.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-17 16:17:45.000000 tkeasygui-0.2.48/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-17 16:23:31.866966 tkeasygui-0.2.48/setup.cfg
```

### Comparing `tkeasygui-0.2.47/LICENSE` & `tkeasygui-0.2.48/LICENSE`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.47/PKG-INFO` & `tkeasygui-0.2.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.47
+Version: 0.2.48
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
```

### Comparing `tkeasygui-0.2.47/README.md` & `tkeasygui-0.2.48/README.md`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.47/TkEasyGUI/dialogs.py` & `tkeasygui-0.2.48/TkEasyGUI/dialogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import subprocess
 import tkinter.filedialog as filedialog
 import tkinter.messagebox as messagebox
 from datetime import datetime, timedelta
 from tkinter import colorchooser
 from typing import Union
 
-from .utils import Window, Element, TextAlign, TextVAlign, FontType, PointType, EventMode, OrientationType, ListboxSelectMode, PadType, ReliefType
 from . import widgets as eg
+from .utils import (
+    FontType,
+)
 
 #------------------------------------------------------------------------------
 # Dialogs
 #------------------------------------------------------------------------------
 # like PySimpleGUI
 
 def popup_buttons(message: str, title: str = "Question", buttons: list[str] = ["OK", "Cancel"], 
@@ -416,19 +418,25 @@
     """Display a message in a popup window with OK and Cancel buttons. Return True or False. (use Tkinter)"""
     return messagebox.askokcancel(title, message)
 
 def ask_retry_cancel(message: str, title: str="Question") -> bool:
     """Display a message in a popup window with Retry and Cancel buttons. Return True or False. (use Tkinter)"""
     return messagebox.askretrycancel(title, message)
 
-def show_message(message: str, title: str="Information") -> None:
+def show_message(
+        message: str,
+        title: str="Information"
+    ) -> None:
     """show message in a popup window"""
     messagebox.showinfo(title, message)
 
 def show_info(message: str, title: str="Information") -> None:
     """show message in a popup window"""
     messagebox.showinfo(title, message)
 
-def msgbox(message: str, title: str="Message") -> None:
+def msgbox(
+        message: str, # message
+        title: str="Message" # dialog title
+    ) -> None:
     """show message in a popup window like VB"""
     messagebox.showinfo(title, message)
```

### Comparing `tkeasygui-0.2.47/TkEasyGUI/utils.py` & `tkeasygui-0.2.48/TkEasyGUI/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from typing import Literal, Union, TypeVar
+"""
+TkEasyGUI utilities functions
+"""
+
+from typing import Literal, TypeVar, Union
+
 import pyperclip
 
 # define TypeAlias
 Window = TypeVar("Window")
 Element = TypeVar("Element")
 TextAlign = Literal["left", "right", "center"]
 TextVAlign = Literal["top", "bottom", "center"]
@@ -10,16 +15,14 @@
 PointType = Union[tuple[int, int], tuple[float, float]]
 EventMode = Literal["user", "system"]
 OrientationType = Literal["v", "h", "vertical", "horizontal"]
 ListboxSelectMode = Literal["multiple", "browse", "extended", "single"]
 PadType = Union[int, tuple[int, int], tuple[tuple[int, int], tuple[int, int]]]
 ReliefType = Literal["flat", "groove", "raised", "ridge", "solid", "sunken"]
 
-
-
 def set_clipboard(text):
     """copy text to clipboard"""
     pyperclip.copy(text)
 
 def get_clipboard():
     """get text from clipboard"""
     return pyperclip.paste()
```

### Comparing `tkeasygui-0.2.47/TkEasyGUI/widgets.py` & `tkeasygui-0.2.48/TkEasyGUI/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,38 @@
 """
 import io
 import os
 import platform
 import sys
 import tkinter as tk
 import tkinter.font as tkfont
-from tkinter import font as tkinter_font
-from tkinter import scrolledtext
 from datetime import datetime
 from queue import Queue
-from tkinter import ttk
-from typing import Any, Literal, Union
-# from typing import TypeAlias
+from tkinter import font as tkinter_font
+from tkinter import scrolledtext, ttk
+from typing import Any, Union
 
+# from typing import TypeAlias
 from PIL import Image as PILImage
 from PIL import ImageTk
 
-from . import utils
-from .utils import Window, Element, TextAlign, TextVAlign, FontType, PointType, EventMode, OrientationType, ListboxSelectMode, PadType, ReliefType
-from . import dialogs
+from . import dialogs, utils
+from .utils import (
+    Element,
+    EventMode,
+    FontType,
+    ListboxSelectMode,
+    OrientationType,
+    PadType,
+    PointType,
+    ReliefType,
+    TextAlign,
+    TextVAlign,
+    Window,
+)
 
 #------------------------------------------------------------------------------
 # Const
 #------------------------------------------------------------------------------
 WINDOW_CLOSED: str = "WINDOW_CLOSED"
 WIN_CLOSED: str = "WINDOW_CLOSED"
 WINDOW_TIMEOUT: str = "-TIMEOUT-"
@@ -67,29 +77,42 @@
     win = get_root_window()
     win.withdraw()
     style = get_ttk_style()
     style.theme_use(name)
     _tkeasygui_info["theme"] = name
 
 def get_tnemes() -> list[str]:
-    """Get themes"""
+    """
+    Get theme list
+    ```py
+    print(get_themes())
+    ```
+    """
     win = get_root_window()
     win.withdraw()
     return ttk.Style().theme_names()
 
 def get_current_theme() -> str:
     """Get current theme"""
     return _tkeasygui_info.get("theme", "")
 
 def set_default_theme() -> None:
-    """Set default theme"""
+    """
+    Set default theme
+    ```py
+    print(get_themes())
+    ```
+    """
     if is_mac():
+        # ('aqua', 'clam', 'alt', 'default', 'classic')
         set_theme("aqua")
     elif is_win():
+        # ('winnative', 'clam', 'alt', 'default', 'classic', 'vista', 'xpnative')
         # set_theme("winnative")
+        # set_theme("default")
         set_theme("vista")
     else:
         set_theme("clam")
 
 def convert_color_rgb16(color_name: str) -> tuple[int, int, int]:
     """Convert color to RGB, return (r, g, b) tuple. range=0-65535"""
     root = get_root_window()
@@ -173,25 +196,26 @@
 class Window:
     """
     Main window object in TkEasyGUI
     """
     def __init__(
                 self,
                 title: str,
-                layout: list[list[Element]],
-                size: Union[tuple[str, int], None] = None, 
+                layout: list[list[Element]], # set elements layout
+                size: Union[tuple[str, int], None] = None, # window size
                 resizable:bool = False,
                 font: Union[FontType, None] = None,
-                modal: bool = False, 
+                modal: bool = False, # modal window
                 keep_on_top:bool = False, # keep on top
                 no_titlebar: bool = False, # hide titlebar
                 grab_anywhere: bool = False, # can move window by dragging anywhere
-                alpha_channel: float = 1.0,
+                alpha_channel: float = 1.0, # window alpha channel
                 enable_key_events: bool = False, # enable keyboard events
                 return_keyboard_events: bool = False, # enable keyboard events (for compatibility)
+                use_ttk: bool = False, # use ttk style (default=False) (experimental)
                 **kw) -> None:
         """Create a window with a layout of widgets."""
         self.modal: bool = modal
         # check active window
         active_win = _get_active_window()
         if active_win is None:
             active_win = get_root_window()
@@ -219,16 +243,18 @@
         self._start_y: Union[int, None] = None
         self._mouse_x: Union[int, None] = None
         self._mouse_y: Union[int, None] = None
         self.alpha_channel: float = alpha_channel
         self.enable_key_events: bool = enable_key_events
         self.return_keyboard_events: bool = return_keyboard_events
         self.font_size_average: tuple[int, int] = (12, 10)
+        self.use_ttk: bool = use_ttk
         # Frame
         self.frame: ttk.Frame = ttk.Frame(self.window, padding=10)
+        self.frame.configure(style="TFrame")
         # set window properties
         self.window.title(title)
         self.window.protocol("WM_DELETE_WINDOW", lambda : self._close_handler())
         if size is not None:
             self.window.geometry(f"{size[0]}x{size[1]}")
         self.window.resizable(resizable, resizable)
         # create widgets
@@ -739,15 +765,15 @@
         self.key: str|int|None = key
         if self.key is not None:
             register_element_key(self.key) # for checking unique key
         if self.has_value and (self.key is None or self.key == ""):
             self.key = generate_element_id()
         self.element_type: str = element_type
         self.ttk_style_name: str = ttk_style_name
-        self.use_ttk: bool = True if ttk_style_name != "" else False
+        self.use_ttk: bool = False # use ttk style
         self.metadata = metadata
         self.style_name: str = self._generate_style_name(key)
         self.props: dict[str, Any] = kw
         self.widget: Any|None = None
         self.expand_x: bool = False
         self.expand_y: bool = False
         self.anchor: Union[str, None] = None
@@ -763,22 +789,22 @@
         self.pady: int|tuple[int,int]|None = None
         self.font: Union[FontType, None] = None
         self.has_font_prop: bool = True
         self.col_no: int = -1
         self.row_no: int = -1
     
     def get_name(self) -> str:
-        """Get element name."""
+        """Get key of element."""
         if self.key is None:
             return "-unknown-"
         return str(self.key)
     
     def bind(self, event_name: str, handle_name: str, propagate: bool=True, event_mode: EventMode = "user") -> None:
         """
-        Bind event. @see `Window.bind`
+        Bind event. @see [Window.bind](#windowbind)
         """
         self._bind_dict[event_name] = (handle_name, propagate, event_mode)
         if self.window is not None:
             self.window.bind(self, event_name, handle_name, propagate=propagate, event_mode=event_mode)
 
     def disptach_event(self, values: Union[dict[str, Any], None] = None) -> None:
         """Dispatch event"""
@@ -852,15 +878,15 @@
         if self.pady is not None:
             props["pady"] = self.pady
         # anchor
         if self.anchor is not None:
             props["anchor"] = self.anchor
         return props
 
-    def convert_props(self, props: dict[str, Any]) -> dict[str, Any]:
+    def _convert_props(self, props: dict[str, Any]) -> dict[str, Any]:
         result = {}
         # copy
         for key, val in props.items():
             result[key] = val
         # check props
         # size
         if "size" in result:
@@ -896,42 +922,41 @@
             self.bind_events(bind_events)
         # disabled
         if "disabled" in result:
             result["state"] = tk.DISABLED if result.pop("disabled") else tk.NORMAL
         return result
 
     def set_disabled(self, disabled: bool) -> None:
+        """
+        Set disabled widgets state
+        """
         self.disabled = disabled
         state = tk.DISABLED if disabled else tk.NORMAL
-        self.widget_update(state=state)
+        self._widget_update(state=state)
 
     def bind_events(self, events: dict[str, str], event_mode: EventMode="user") -> Element:
         """
-        Bind user events
-        **Example**
-        ```
-        # (1) bind events in the constructor
-        eg.Canvas(key="-canvas-", bind_events={"<ButtonPress>": "on", "<ButtonRelease>": "off"})
-        # (2) bind events in the method
-        eg.Canvas(key="-canvas-").bind_events({"<ButtonPress>": "on", "<ButtonRelease>": "off"})
-        ```
+        Bind user events. @see [custom events](/docs/custom_events.md)
         """
         for event_name, handle_name in events.items():
             self.bind(event_name, handle_name, event_mode=event_mode)
         return self
 
     def create(self, win: Window, parent: tk.Widget) -> Any:
         """Create a widget."""
         return None
 
     def prepare_create(self, win: Window) -> None:
         # convert properties
         if (win.font is not None) and (self.font is None) and self.has_font_prop:
             self.props["font"] = self.font = win.font
-        self.props = self.convert_props(self.props)
+        self.props = self._convert_props(self.props)
+        # check ttk
+        if self.use_ttk is None:
+            self.use_ttk = win.use_ttk
         # check use ttk
         if not self.use_ttk:
             return
         # set style
         style = get_ttk_style()
         style_name = self.style_name
         # create style
@@ -985,24 +1010,24 @@
         """Get the value of the widget."""
         return "-"
     
     def update(self, *args, **kw) -> None:
         """update widget configuration."""
         pass
     
-    def widget_update(self, **kw) -> None:
+    def _widget_update(self, **kw) -> None:
         # update element's props
         for k, v in kw.items():
             self.props[k] = v
-        kw = self.convert_props(kw)
+        kw = self._convert_props(kw)
         try:
             if (self.widget is not None)and(len(kw) > 0):
                 self.widget.configure(**kw)
         except Exception as e:
-            print(f"TkEasyGUI.Element.widget_update.Error: key='{self.key}', try to update {kw}, {e}", file=sys.stderr)
+            print(f"TkEasyGUI.Element._widget_update.Error: key='{self.key}', props={kw}. {e}", file=sys.stderr)
 
     def get_prev_widget(self, target_key: Union[str, None] = None) -> tk.Widget:
         """Get the previous widget."""
         # check target_key
         target: tk.Widget = None
         if target_key:
             if target_key in self.window.key_elements:
@@ -1084,15 +1109,15 @@
 
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
     def update(self, *args, **kw) -> None:
         """Update the widget."""
-        self.widget_update(**kw)
+        self._widget_update(**kw)
     
     def __getattr__(self, name):
         """Get unknown attribute."""
         if name in ["Widget"]:
             return self.widget
         return super().__getattr__(name)
 
@@ -1134,15 +1159,15 @@
 
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
     def update(self, *args, **kw) -> None:
         """Update the widget."""
-        self.widget_update(**kw)
+        self._widget_update(**kw)
     
     def __getattr__(self, name):
         """Get unknown attribute."""
         if name in ["Widget"]:
             return self.widget
         return super().__getattr__(name)
 
@@ -1194,21 +1219,21 @@
     
     def get_text(self) -> str:
         return self.props["text"]
     
     def set_text(self, text: str) -> None:
         """Set the text of the widget."""
         self.props["text"] = text
-        self.widget_update(text=text)
+        self._widget_update(text=text)
 
     def update(self, text: Union[str, None] = None, *args, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
-        self.widget_update(**kw)
+        self._widget_update(**kw)
 
 class Label(Text):
     """
     Label element (alias of Text)
     """
     pass
 
@@ -1298,31 +1323,31 @@
     
     def get_text(self) -> str:
         return self.props["text"]
     
     def set_text(self, text: str) -> None:
         """Set the text of the widget."""
         self.props["text"] = text
-        self.widget_update(text=text)
+        self._widget_update(text=text)
 
     def update(self, text: Union[str, None] = None, *args, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
-        self.widget_update(**kw)
+        self._widget_update(**kw)
 
 class Button(Element):
     """Button element."""
     def __init__(
                 self,
                 button_text: str = "",
                 key: Union[str, None] = None,
                 disabled: bool = None,
                 size: Union[tuple[int, int], None] = None,
-                use_ttk_buttons: bool = False,
+                use_ttk_buttons: Union[bool, None] = None,
                 tooltip: Union[str, None] = None, # (TODO) tooltip
                 button_color: Union[str, tuple[str, str], None] = None,
                 # text props
                 text_align: Union[TextAlign, None] = "left", # text align
                 font: Union[FontType, None] = None, # font
                 color: Union[str, None] = None, # text color
                 text_color: Union[str, None] = None, # same as color
@@ -1352,14 +1377,15 @@
         self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
         self.bind_events({
             "<Button-3>": "right_click",
             "<Return>": "return",
         }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
+        """Create a Button widget."""
         if self.use_ttk:
             self.widget = ttk.Button(
                 parent,
                 command=lambda: self.disptach_event({"event_type": "command"}),
                 **self.props)
         else:
             self.widget = tk.Button(
@@ -1376,43 +1402,44 @@
                 props["text_color"] = button_color[0]
                 props["background_color"] = button_color[1]
             elif len(button_color) == 1:
                 props["background_color"] = button_color[0]
         else:
             props["background_color"] = button_color
         if update:
-            self.widget_update(props)
+            self._widget_update(props)
 
     def get(self) -> Any:
-        """Get the value of the widget."""
+        """Returns the text of the button.."""
         return self.get_text()
     
     def set_text(self, text: str) -> None:
-        """Set the text of the widget."""
+        """Set the text of the button."""
         self.props["text"] = text
-        self.widget_update(text=text)
+        self._widget_update(text=text)
     
     def get_text(self) -> str:
+        """Get the text of the button."""
         return self.props["text"]
 
     def update(self,
                text: Union[str, None] = None, 
                disabled: Union[bool, None] = None,
                button_color: Union[str, tuple[str,str], None] = None,
                **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.props["text"] = text
-            self.widget_update(text=text)
+            self._widget_update(text=text)
         if disabled is not None:
             self.set_disabled(disabled)
         if button_color is not None:
             self.set_button_color(button_color, update=False)
         # other
-        self.widget_update(**kw)
+        self._widget_update(**kw)
     
     def __getattr__(self, name: str) -> Any:
         """Get unknown attribute. """
         # Get the text of the button. (compatibility with PySimpleGUI)
         if name == "GetText":
             return self.get_text
         elif name == "ButtonText":
@@ -1432,14 +1459,15 @@
                 enable_events: bool=False,
                 # other
                 metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         if key is None or key == "":
             key = text
         super().__init__("Checkbox", "TCheckbutton", key, True, metadata, **kw)
+        self.use_ttk = True
         self.default_value = default
         self.props["text"] = text
         if enable_events:
             self.bind_events({
                 "<Button-3>": "right_click"
             }, "system")
 
@@ -1460,27 +1488,27 @@
     def get(self) -> Any:
         """Get the value of the widget."""
         return self.get_value()
 
     def set_text(self, text: str) -> None:
         """Set the text of the widget."""
         self.props["text"] = text
-        self.widget_update(text=text)
+        self._widget_update(text=text)
 
     def update(self, *args, **kw) -> None:
         """Update the widget."""
         if len(args) >= 1:
             self.set_value(args[0])
         if len(args) >= 2:
             self.set_text(args[1])
         if "text" in kw:
             self.set_text(kw.pop("text"))
         if "value" in kw:
             self.set_value(kw.pop("value"))
-        self.widget_update(**kw)
+        self._widget_update(**kw)
 
 class Radio(Element):
     """Checkbox element."""
     def __init__(
                 self, text: str="",
                 group_id: Union[int, str] = "group",
                 default: bool = False,
@@ -1488,14 +1516,15 @@
                 enable_events: bool = False,
                 # other
                 metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         if key is None or key == "":
             key = text
         super().__init__("Radio", "TRadiobutton", key, True, metadata, **kw)
+        self.use_ttk = True
         self.default_value = default
         self.value: int = 0
         self.props["text"] = text
         self.group_id: str = str(group_id)
         if enable_events:
             self.bind_events({
                 "<Button-3>": "right_click"
@@ -1535,21 +1564,21 @@
     def get(self) -> Any:
         """Get the value of the widget."""
         return self.is_selected()
 
     def set_text(self, text: str) -> None:
         """Set the text of the widget."""
         self.props["text"] = text
-        self.widget_update(text=text)
+        self._widget_update(text=text)
 
     def update(self, text: Union[str, None] = None, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
-        self.widget_update(**kw)
+        self._widget_update(**kw)
 
 class Input(Element):
     """
     Text input element.
     """
     def __init__(
                 self,
@@ -1573,14 +1602,15 @@
                 expand_y: bool = False,
                 pad: Union[PadType, None] = None,
                 # other
                 metadata: Union[dict[str, Any], None] = None,
                 **kw
                 ) -> None:
         super().__init__("Input", "TEntry", key, True, metadata, **kw)
+        self.use_ttk = False
         self.readonly: bool = readonly
         self.enable_events: bool = enable_events
         if default_text is not None: # compatibility with PySimpleGUI
             text = default_text
         self.default_text = text # default text @see Input.create
         self._set_text_props(font=font, text_align=text_align, color=color, text_color=text_color, background_color=background_color)
         if readonly_background_color is not None:
@@ -1605,23 +1635,23 @@
                 "<Button-1>": "click",
                 "<Button-3>": "right_click"
             }, "system")
     
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         """create Input widget"""
         # check props
-        if "height" in self.props:
-            self.props.pop("height") # no property
+        # if "height" in self.props:
+        #     self.props.pop("height") # no property
         # set default text
         self.text_var = tk.StringVar(value=self.default_text)
         # create
-        self.widget = ttk.Entry(
+        self.widget = tk.Entry(
             parent,
             textvariable=self.text_var,
-            style=self.style_name,
+            # style=self.style_name,
             **self.props)
         # set readonly
         if self.readonly:
             self.set_readonly(self.readonly)
         # trace change
         if self.enable_events:
             self.text_var.trace_add("write",
@@ -1649,27 +1679,27 @@
     
     def get_selected_text(self) -> str:
         """get selected text"""
         if self.widget is None:
             return ""
         try:
             return self.widget.selection_get()
-        except Exception as e:
+        except Exception:
             return ""
 
     def copy_selected_text(self) -> None:
         """Copy selected text"""
         text = self.get_selected_text()
         utils.set_clipboard(text)
 
     def set_readonly(self, readonly: bool) -> None:
         """set readonly"""
         self.readonly = readonly
         state = "readonly" if self.readonly else "normal"
-        self.widget_update(state=state)
+        self._widget_update(state=state)
 
     def update(self, text: Union[str, None] = None, readonly: Union[bool, None] = None, **kw) -> None:
         """Update the widget."""
         if self.widget is None:
             return
         # check readonly
         if readonly is not None:
@@ -1679,15 +1709,15 @@
             if self.readonly:
                 self.set_readonly(False)
                 self.set_text(text)
                 self.set_readonly(True)
             else:
                 self.set_text(text)
         # update others
-        self.widget_update(**kw)
+        self._widget_update(**kw)
     
     def select_all(self) -> None:
         """select_all"""
         if self.widget is None:
             return
         input: tk.Entry = self.widget
         input.select_range(0, "end")
@@ -1865,15 +1895,15 @@
     
     def get_selected_text(self) -> str:
         """Get the selected text."""
         if self.widget is None:
             return ""
         try:
             text = self.widget.selection_get()
-        except Exception as e:
+        except Exception:
             text = ""
         return text
     
     def copy(self) -> str:
         """Copy the selected text."""
         if self.widget is None:
             return
@@ -1902,33 +1932,33 @@
 
     def update(self, text: Union[str, None] = None, readonly: Union[bool, None] = None, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
         if readonly is not None:
             self.set_readonly(readonly)
-        self.widget_update(**kw)
+        self._widget_update(**kw)
 
     def set_readonly(self, readonly: bool) -> None:
         """Set readonly"""
         self.readonly = readonly
         state = tk.DISABLED if readonly else tk.NORMAL
-        self.widget_update(state=state)
+        self._widget_update(state=state)
 
     def set_text(self, text: str) -> None:
         """Set text"""
         if self.widget is None:
             return
         if self.readonly:
-            self.widget_update(state=tk.NORMAL)
+            self._widget_update(state=tk.NORMAL)
         self.props["text"] = text
         self.widget.delete("1.0", "end") # clear text
         self.widget.insert("1.0", text) # set text
         if self.readonly:
-            self.widget_update(state=tk.DISABLED)
+            self._widget_update(state=tk.DISABLED)
     
     def get_selection_pos(self) -> tuple[str, str]:
         """Get selection position, returns (start_pos, end_pos)."""
         if self.widget is None:
             return ("", "")
         try:
             sel_start, sel_end = self.widget.tag_ranges("sel")
@@ -2031,15 +2061,14 @@
         """select all text"""
         if self.widget is None:
             return
         text: tk.Text = self.widget
         text.tag_add(tk.SEL, "1.0", tk.END)
         text.mark_set(tk.INSERT, '1.0')
         self.widget.see(tk.INSERT)
-        print("@select_all")
 
     def print(self, text: str, text_color: Union[str, None] = None, background_color: Union[str, None] = None, end:str="\n") -> None:
         """Print text."""
         text += end
         if self.widget is None:
             return
         tags: list[str] = []
@@ -2061,23 +2090,23 @@
     """Output element. (alias of Multiline) TODO: implement"""
     pass
 
 class Slider(Element):
     """Slider element."""
     def __init__(
                 self,
-                range: tuple[float, float] = (1, 10),
-                default_value: Union[float, None] = None,
-                resolution: Union[float, None] = None,
-                orientation: OrientationType = "horizontal",
+                range: tuple[float, float] = (1, 10), # value range (from, to)
+                default_value: Union[float, None] = None, # default value
+                resolution: Union[float, None] = None, # value resolution
+                orientation: OrientationType = "horizontal", # orientation (h|v|horizontal|vertical)
                 tick_interval: Union[float, None] = None, # tick marks interval on the scale
                 enable_events: bool = False, # enable changing events
                 enable_changed_events: bool = False, # enable changed event
-                disable_number_display: bool = False,
-                size: Union[tuple[int, int], None] = None, # horizontal: (bar_length, thumb_size), vertical: (thumb_size, bar_length)
+                disable_number_display: bool = False, # hide number display
+                size: Union[tuple[int, int], None] = None, # size (unit: character) / horizontal: (bar_length, thumb_size), vertical: (thumb_size, bar_length)
                 key: Union[str, None] = None,
                 # other
                 default: Union[float, None] = None, # same as default_value
                 metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         style_name = "Horizontal.TScale" if (orientation == "h" or orientation == "horizontal") else "Vertical.TScale"
         super().__init__("Slider", style_name, key, True, metadata, **kw)
@@ -2126,48 +2155,58 @@
             self.props["width"] = width
             self.props["length"] = length
         # var
         self.scale_var = tk.DoubleVar()
         self.scale_var.set(self.default_value)
         # command
         command = None
+        def on_command(*event):
+            self.disptach_event({"event_type": "change", "event": event})
         if self.enable_events:
-            command = lambda *event: self.disptach_event({"event_type": "change", "event": event})
+            command = on_command
         # widget
         self.widget = tk.Scale(
             parent,
             from_=self.range[0],
             to=self.range[1],
             resolution=self.resolution,
             command=command,
             variable=self.scale_var,
             **self.props)
         return self.widget
 
     def get(self) -> Any:
-        """Return Widget"""
-        print(f"@[{self.key}].get=", self.scale_var.get())
+        """Return slider value."""
         return self.scale_var.get()
     
     def set(self, value: float) -> None:
-        """Set the value of the widget."""
-        self._value = value
+        """Set value of Slider"""
         self.widget.set(value)
+    
+    def set_range(self, from_: float, to: float) -> None:
+        """Set the range of the slider."""
+        self.widget.config(from_=from_, to=to)
+
+    def get_range(self) -> tuple[float, float]:
+        return (self.widget.cget("from"), self.widget.cget("to"))
 
     def update(self,
                value: Union[float, None]=None,
+               range: Union[tuple[float, float], None]=None,
                disable_number_display: Union[bool, None]=None,
                **kw) -> None:
         """Update the widget."""
+        if range is not None:
+            self.set_range(range[0], range[1])
         if disable_number_display is not None:
             self.props["showvalue"] = 0 if disable_number_display else 1
         if value is not None:
             self.set(value)
         else:
-            self.widget_update(**kw)
+            self._widget_update(**kw)
 
 class Canvas(Element):
     """Canvas element."""
     def __init__(
                 self,
                 key: Union[str, None] = None,
                 enable_events: bool = False,
@@ -2194,15 +2233,15 @@
     
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
     def update(self, *args, **kw) -> None:
         """Update the widget."""
-        self.widget_update(**kw)
+        self._widget_update(**kw)
     
     def __getattr__(self, name):
         """Get unknown attribute."""
         if name in ["Widget", "tk_canvas", "TKCanvas"]: # compatibility with PySimpleGUI
             return self.widget
         return super().__getattr__(name)
 
@@ -2240,15 +2279,15 @@
 
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
     def update(self, *args, **kw) -> None:
         """Update the widget."""
-        self.widget_update(**kw)
+        self._widget_update(**kw)
     
     def __getattr__(self, name):
         """Get unknown attribute."""
         if name in ["Widget"]:
             return self.widget
         return super().__getattr__(name)
     
@@ -2372,15 +2411,15 @@
                **kw) -> None:
         """Update the widget."""
         if size is not None:
             self.size = size
             self.widget.configure(width=size[0], height=size[1])
         if (source is not None) or (filename is not None) or (data is not None):
             self.set_image(source, filename, data)
-        self.widget_update(**kw)
+        self._widget_update(**kw)
     
     def __getattr__(self, name):
         """Get unknown attribute."""
         if name in ["Widget", "tk_canvas", "tktext_label"]:
             return self.widget
         return super().__getattr__(name)
 
@@ -2392,14 +2431,15 @@
                 background_color: Union[str, None] = None,
                 pad: PadType = 5,
                 size: tuple[int, int]=(5, 100),
                 # other
                 metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("VSeparator", "TSeparator", key, False, metadata, **kw)
+        self.use_ttk = True
         size = (pad, size[1])
         self.size = self.props["size"] = size
         self.props["padx"] = pad
         if background_color is not None:
             self.props["background"] = background_color
         self.props["expand_y"] = True
     
@@ -2415,14 +2455,15 @@
                 background_color: Union[str, None] = None,
                 pad: PadType = 5,
                 size: tuple[int, int] = (100, 5),
                 # other
                 metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         super().__init__("HSeparator", "TSeparator", key, False, metadata, **kw)
+        self.use_ttk = True
         size = (size[1], pad)
         self.size = self.props["size"] = size
         self.props["pady"] = pad
         if background_color is not None:
             self.props["background"] = background_color
         self.props["expand_x"] = True
     
@@ -2501,15 +2542,15 @@
         if self.widget is None:
             return
         if len(args) >= 1:
             values = args[0]
             self.set_values(values)
         if "values" in kw:
             self.set_values(kw.pop("values"))
-        self.widget_update(**kw)
+        self._widget_update(**kw)
 
 class Combo(Element):
     """Combo element."""
     def __init__(
                 self,
                 values: list[str]=[],
                 default_value: str="",
@@ -2535,15 +2576,15 @@
         self.set_value(self.default_value)
         return self.widget
 
     def set_values(self, values: list[str]) -> None:
         """Set values to list"""
         self.values = values
         if self.widget is not None:
-            self.widget_update(values=self.values)
+            self._widget_update(values=self.values)
     
     def set_value(self, v: str) -> None:
         """Set the value of the widget."""
         self.value.set(v)
 
     def get(self) -> Any:
         """Get the value of the widget."""
@@ -2557,15 +2598,15 @@
             return
         if len(args) >= 1:
             self.set_value(args[0])
         if "values" in kw:
             self.set_values(kw.pop("values"))
         if "value" in kw:
             self.set_value(kw.pop("value"))
-        self.widget_update(**kw)
+        self._widget_update(**kw)
 
 class Table(Element):
     """Table element."""
     def __init__(
                 self,
                 values: list[list[str]] = [],
                 headings: list[str] = [],
@@ -2589,14 +2630,15 @@
                 pad: Union[PadType, None] = None,
                 # other
                 metadata: Union[dict[str, Any], None] = None,
                 **kw) -> None:
         """Create a table."""
         # super().__init__("Table", "Treeview", key, metadata, **kw)
         super().__init__("Table", "", key, True, metadata, **kw)
+        self.ttk = True
         self.values = values
         self.headings = headings
         self.enable_events = enable_events
         self.select_mode = select_mode
         self.auto_size_columns = auto_size_columns
         self.max_col_width = max_col_width
         self.col_widths = col_widths
@@ -2710,15 +2752,15 @@
             tree = self.widget
             for i in tree.get_children(): # clear all
                 tree.delete(i)
         # set values
         self.set_values(self.values, self.headings)
         # 
         del kw["values"]
-        self.widget_update(**kw)
+        self._widget_update(**kw)
 
 #------------------------------------------------------------------------------
 # Browse elements
 
 class FileBrowse(Element):
     """FileBrowse element."""
     def __init__(
@@ -2786,21 +2828,21 @@
         if (target is not None) and (result is not None) and (result != ""):
             target.update(result)
         return result
     
     def set_text(self, text: str) -> None:
         """Set the text of the button."""
         self.props["text"] = text
-        self.widget_update(text=text)
+        self._widget_update(text=text)
 
     def update(self, text: Union[str, None] = None, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
-        self.widget_update(**kw)
+        self._widget_update(**kw)
 
 class FilesBrowse(FileBrowse):
     """FilesBrowse element."""
     def __init__(
                 self,
                 button_text: str = "...",
                 key: Union[str, None] = None,
```

### Comparing `tkeasygui-0.2.47/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.48/TkEasyGUI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.47
+Version: 0.2.48
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
```

### Comparing `tkeasygui-0.2.47/pyproject.toml` & `tkeasygui-0.2.48/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TkEasyGUI"
-version = "0.2.47"
+version = "0.2.48"
 dependencies = [
   "Pillow",
   "pyperclip",
 ]
 requires-python = ">=3.9"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
```

