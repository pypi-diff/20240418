# Comparing `tmp/world_wall_clock-0.1.3.tar.gz` & `tmp/world_wall_clock-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "world_wall_clock-0.1.3.tar", max compression
+gzip compressed data, was "world_wall_clock-0.1.4.tar", max compression
```

## Comparing `world_wall_clock-0.1.3.tar` & `world_wall_clock-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2904 2023-10-26 14:21:29.083112 world_wall_clock-0.1.3/README.md
--rw-r--r--   0        0        0      809 2023-11-02 03:51:47.980090 world_wall_clock-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       47 2023-11-02 03:51:47.988090 world_wall_clock-0.1.3/world_wall_clock/__init__.py
--rw-r--r--   0        0        0       89 2023-10-20 20:59:16.806773 world_wall_clock-0.1.3/world_wall_clock/__main__.py
--rw-r--r--   0        0        0    22238 2023-11-02 03:51:47.988090 world_wall_clock-0.1.3/world_wall_clock/wwclock.py
--rw-r--r--   0        0        0     3648 1970-01-01 00:00:00.000000 world_wall_clock-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3226 2024-04-18 00:17:17.285453 world_wall_clock-0.1.4/README.md
+-rw-r--r--   0        0        0      950 2024-04-18 00:17:17.286453 world_wall_clock-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 00:17:17.298454 world_wall_clock-0.1.4/world_wall_clock/__init__.py
+-rw-r--r--   0        0        0       58 2024-04-18 00:17:17.298454 world_wall_clock-0.1.4/world_wall_clock/__main__.py
+-rw-r--r--   0        0        0    22034 2024-04-18 00:17:17.298454 world_wall_clock-0.1.4/world_wall_clock/wwclock.py
+-rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 world_wall_clock-0.1.4/PKG-INFO
```

### Comparing `world_wall_clock-0.1.3/README.md` & `world_wall_clock-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,30 @@
 ![Screeenshot of world-wall-clock](./screenshot.png)
 
 ## Installing world-wall-clock
 
 You can install world-wall-clock with the Python packaging tool
 [pip](https://pip.pypa.io/en/stable/). It is recommended to do so in a
 [virtual environment](https://docs.python.org/3/library/venv.html).
+Alternatively, you can use [pipx](https://pypa.github.io/pipx/) as a wrapper
+around pip that will handle setting up a virtual environment for you.
 
-### From PyPI
+### From PyPI, using pipx
+
+```sh
+pipx install world-wall-clock
+```
+
+### From PyPI, using pip in a virtual enviornment
 
 ```sh
 python -m pip install world-wall-clock
 ```
 
-### From the top level of the source repo
+### From the top level of the source repo, using pip in a virtual environment
 
 ```sh
 python -m pip install .
 ```
 
 ## Running world-wall-clock
 
@@ -83,14 +91,15 @@
 you've made using the `poetry run` command:
 
 ```sh
 poetry run wwclock
 ```
 
 The `poetry run` command will also allow you to run the suite of chosen dev
-tools for static type-checking, code formatting, and linting:
+tools for static type-checking, import sorting, code formatting, and linting:
 
 ```sh
 poetry run mypy --strict
+poetry run isort .
 poetry run black .
 poetry run flake8
 ```
```

### Comparing `world_wall_clock-0.1.3/world_wall_clock/wwclock.py` & `world_wall_clock-0.1.4/world_wall_clock/wwclock.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,37 +12,36 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from . import VERSION
-
 import abc
+import json
 from argparse import ArgumentParser, Namespace
 from collections.abc import Callable
-from datetime import date, datetime, timezone, tzinfo
-import json
+from datetime import date, datetime, tzinfo
 from pathlib import Path
 from typing import Any, List, Literal, Optional, Set, Tuple
-from zoneinfo import available_timezones, ZoneInfo
+from zoneinfo import ZoneInfo, available_timezones
 
 import urwid
 from xdg_base_dirs import xdg_config_home
 
 CURSES_AVAILABLE: bool
 try:
     import urwid.curses_display
 
     CURSES_AVAILABLE = True
 except ImportError:
     CURSES_AVAILABLE = False
 
 
+VERSION: str = "0.1.4"
 DEFAULT_CLOCKS: List[str] = [
     "Pacific/Niue",
     "America/Santiago",
     "UTC",
     "Europe/Vienna",
     "Africa/Nairobi",
     "Asia/Colombo",
@@ -86,18 +85,15 @@
         old_title: Optional[str] = self._title
         if isinstance(self.tz, ZoneInfo):
             tz: tzinfo = self.tz
             tzkey: Optional[str] = self.tz.key
             tzname: Optional[str] = tz.tzname(dt)
             self._title = tzkey if tzkey == tzname else f"{tzkey} ({tzname})"
         else:
-            dt_utc: datetime = datetime.utcfromtimestamp(dt.timestamp())
-            tz = timezone(dt - dt_utc)
-            self._title = tz.tzname(dt)
-            tzname = tz.tzname(dt)
+            self._title = tzname = dt.astimezone().tzname()
         if hasattr(self, "title_widget"):
             self.set_title(self._title)
         return old_title != self._title
 
     def update_clock(self, ts: Optional[float] = None) -> Tuple[datetime, bool]:
         dt: datetime = (
             datetime.fromtimestamp(ts, self.tz) if ts else datetime.now(self.tz)
@@ -116,16 +112,14 @@
     def __init__(self, maxlen: int, default: int = 0) -> None:
         self.maxlen: int = maxlen
         padded: str = str(default).rjust(maxlen, "0")
         super().__init__("", padded)
         self.set_edit_pos(0)
 
     def keypress(self, size: Tuple[int], key: str) -> Optional[str]:
-        if self.edit_pos >= self.maxlen:
-            self.set_edit_pos(self.maxlen - 1)
         if key in {"up", "down"}:
             return key
         if key == "tab":
             return "right"
         elif key == "backspace":
             return self.keypress(size, "left")
         elif key == "delete":
@@ -138,22 +132,22 @@
 
 
 class ListBoxMeta(urwid.WidgetMeta, abc.ABCMeta):
     pass
 
 
 class TZPickerBase(urwid.ListBox, metaclass=ListBoxMeta):
-    def append(self, label: str) -> None:
-        pass
+    @abc.abstractmethod
+    def append(self, label: str) -> None: ...
 
-    def remove(self, label: str) -> None:
-        pass
+    @abc.abstractmethod
+    def remove(self, label: str) -> None: ...
 
-    def get_tz(self) -> Optional[tzinfo]:
-        return None
+    @abc.abstractmethod
+    def get_tz(self) -> Optional[tzinfo]: ...
 
 
 class DatetimePicker(object):
     year: DatetimeIntEdit
     month: DatetimeIntEdit
     day: DatetimeIntEdit
     hour: DatetimeIntEdit
@@ -319,16 +313,15 @@
             edit_pos += 1
         if new_value > 59:
             new_value = 59
         return f"{new_value:02}", edit_pos + length
 
 
 class ActiveTZPicker(TZPickerBase):
-    def __init__(self, foreign_clocks: List[str], dp: DatetimePicker) -> None:
-        self.dp: DatetimePicker = dp
+    def __init__(self, foreign_clocks: List[str]) -> None:
         new_items: List[urwid.AttrMap] = [self.wrap_label("local")] + [
             self.wrap_label(tz) for tz in foreign_clocks
         ]
         self.list_walker: urwid.SimpleFocusListWalker = urwid.SimpleFocusListWalker(
             new_items, wrap_around=True
         )
         super().__init__(self.list_walker)
@@ -382,16 +375,17 @@
     def __init__(
         self,
         widget: urwid.Widget,
         palette: Set[Tuple[Any, ...]] = set(),
         screen: urwid.BaseScreen | None = None,
         handle_mouse: bool = True,
         input_filter: Callable[[List[str], List[int]], List[str]] | None = None,
-        unhandled_input: Callable[[str | Tuple[str, int, int, int]], bool]
-        | None = None,
+        unhandled_input: (
+            Callable[[str | Tuple[str, int, int, int]], bool] | None
+        ) = None,
         event_loop: urwid.EventLoop | None = None,
         pop_ups: bool = False,
         update_fn: Callable[[], Any] = lambda: None,
         refresh_rate: float = 10.0,
     ) -> None:
         self.update_fn: Callable[[], Any] = update_fn
         self.tick_secs: float = 1.0 / refresh_rate
@@ -437,14 +431,15 @@
                 self.foreign_clocks.remove(cb.label)
                 self.dp.tz.remove(cb.label)
             else:
                 self.foreign_clocks.append(cb.label)
                 self.dp.tz.append(cb.label)
             self.write_clock_list()
             self.fill_clock_grid(rebuild_clocks=True)
+            self.update_clocks()
             return None
 
         tz_checklist: List[urwid.CheckBox] = [
             urwid.CheckBox(tz, state=(tz in self.foreign_clocks))
             for tz in sorted(available_timezones())
         ]
         for b in tz_checklist:
@@ -506,15 +501,15 @@
         year, month, day, hour, mins = dt.timetuple()[:5]
         self.dp: DatetimePicker = DatetimePicker()
         self.dp.year = YearEdit(year, self.dp)
         self.dp.month = MonthEdit(month, self.dp)
         self.dp.day = DayEdit(day, self.dp)
         self.dp.hour = HourEdit(hour)
         self.dp.mins = MinuteEdit(mins)
-        self.dp.tz = ActiveTZPicker(self.foreign_clocks, self.dp)
+        self.dp.tz = ActiveTZPicker(self.foreign_clocks)
         self._new_tz_picker: bool = False
         widgets: List[Tuple[int, urwid.Widget] | urwid.Widget] = [
             (len(button.label) + 5, button),
             (4, self.dp.year),
             (1, urwid.Text("-")),
             (2, self.dp.month),
             (1, urwid.Text("-")),
@@ -635,19 +630,19 @@
     parser.add_argument(
         "-v", "--version", action="store_true", help="Print version number and exit"
     )
     return parser.parse_args()
 
 
 def main() -> None:
-    app: App = App()
     args: Namespace = parse_args()
     if args.version:
         print(VERSION)
         return
+    app: App = App()
     try:
         app.main_loop.run()
     except KeyboardInterrupt:
         return
 
 
 if __name__ == "__main__":
```

### Comparing `world_wall_clock-0.1.3/PKG-INFO` & `world_wall_clock-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: world-wall-clock
-Version: 0.1.3
+Version: 0.1.4
 Summary: TUI world clock application
 Home-page: https://github.com/ddelabru/world-wall-clock
 License: GPL-3.0-or-later
 Author: Dominic Delabruere
 Author-email: dominic.delabruere@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -25,22 +25,30 @@
 ![Screeenshot of world-wall-clock](./screenshot.png)
 
 ## Installing world-wall-clock
 
 You can install world-wall-clock with the Python packaging tool
 [pip](https://pip.pypa.io/en/stable/). It is recommended to do so in a
 [virtual environment](https://docs.python.org/3/library/venv.html).
+Alternatively, you can use [pipx](https://pypa.github.io/pipx/) as a wrapper
+around pip that will handle setting up a virtual environment for you.
 
-### From PyPI
+### From PyPI, using pipx
+
+```sh
+pipx install world-wall-clock
+```
+
+### From PyPI, using pip in a virtual enviornment
 
 ```sh
 python -m pip install world-wall-clock
 ```
 
-### From the top level of the source repo
+### From the top level of the source repo, using pip in a virtual environment
 
 ```sh
 python -m pip install .
 ```
 
 ## Running world-wall-clock
 
@@ -102,15 +110,16 @@
 you've made using the `poetry run` command:
 
 ```sh
 poetry run wwclock
 ```
 
 The `poetry run` command will also allow you to run the suite of chosen dev
-tools for static type-checking, code formatting, and linting:
+tools for static type-checking, import sorting, code formatting, and linting:
 
 ```sh
 poetry run mypy --strict
+poetry run isort .
 poetry run black .
 poetry run flake8
 ```
```

