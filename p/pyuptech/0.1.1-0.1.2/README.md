# Comparing `tmp/pyuptech-0.1.1.tar.gz` & `tmp/pyuptech-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuptech-0.1.1.tar", last modified: Wed Apr 17 10:37:33 2024, max compression
+gzip compressed data, was "pyuptech-0.1.2.tar", last modified: Thu Apr 18 11:06:03 2024, max compression
```

## Comparing `pyuptech-0.1.1.tar` & `pyuptech-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       11 2024-04-17 10:37:11.415692 pyuptech-0.1.1/README.md
--rw-r--r--   0        0        0      430 2024-04-17 10:37:33.379686 pyuptech-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      477 2024-04-17 10:37:11.415692 pyuptech-0.1.1/src/pyuptech/__init__.py
--rw-r--r--   0        0        0       35 2024-04-17 10:37:11.415692 pyuptech-0.1.1/src/pyuptech/modules/constant.py
--rw-r--r--   0        0        0     1007 2024-04-17 10:37:11.415692 pyuptech-0.1.1/src/pyuptech/modules/loader.py
--rw-r--r--   0        0        0      524 2024-04-17 10:37:11.415692 pyuptech-0.1.1/src/pyuptech/modules/logger.py
--rw-r--r--   0        0        0    10112 2024-04-17 10:37:11.415692 pyuptech-0.1.1/src/pyuptech/modules/screen.py
--rw-r--r--   0        0        0    10259 2024-04-17 10:37:11.415692 pyuptech-0.1.1/src/pyuptech/modules/sensors.py
--rw-r--r--   0        0        0        0 2024-04-17 10:37:11.419692 pyuptech-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1105 2024-04-17 10:37:11.419692 pyuptech-0.1.1/tests/perf_tests.py
--rw-r--r--   0        0        0      288 1970-01-01 00:00:00.000000 pyuptech-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5865 2024-04-18 11:05:42.276506 pyuptech-0.1.2/README.md
+-rw-r--r--   0        0        0      430 2024-04-18 11:06:03.152718 pyuptech-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      865 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/constant.py
+-rw-r--r--   0        0        0     1007 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/loader.py
+-rw-r--r--   0        0        0      577 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/logger.py
+-rw-r--r--   0        0        0     1659 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/pins.py
+-rw-r--r--   0        0        0    10454 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/screen.py
+-rw-r--r--   0        0        0     8701 2024-04-18 11:05:42.276506 pyuptech-0.1.2/src/pyuptech/modules/sensors.py
+-rw-r--r--   0        0        0        0 2024-04-18 11:05:42.276506 pyuptech-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1105 2024-04-18 11:05:42.276506 pyuptech-0.1.2/tests/perf_tests.py
+-rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 pyuptech-0.1.2/PKG-INFO
```

### Comparing `pyuptech-0.1.1/src/pyuptech/modules/loader.py` & `pyuptech-0.1.2/src/pyuptech/modules/loader.py`

 * *Files identical despite different names*

### Comparing `pyuptech-0.1.1/src/pyuptech/modules/logger.py` & `pyuptech-0.1.2/src/pyuptech/modules/logger.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import logging
-import coloredlogs
 
+import coloredlogs
 
 # 初始化logger
 _logger = logging.getLogger("pyuptech")
-coloredlogs.install(logger=_logger)
+coloredlogs.install(logger=_logger, level=logging.DEBUG)
 
-def set_log_level(level: int|str):
+
+def set_log_level(level: int | str):
     """
     设置日志级别
     :param level: 日志级别
     :return:
     """
     _logger.setLevel(level)
 
-if __name__ == '__main__':
+
+set_log_level(logging.INFO)
+if __name__ == "__main__":
 
     _logger.debug("This is a debug log.")
     _logger.info("This is a info log.")
     _logger.warning("This is a warning log.")
     _logger.error("This is a error log.")
     _logger.critical("This is a critical log.")
```

### Comparing `pyuptech-0.1.1/src/pyuptech/modules/screen.py` & `pyuptech-0.1.2/src/pyuptech/modules/screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from typing import Literal, Self
 
 from .constant import LIB_FILE_PATH
 from .loader import load_lib
+from .logger import _logger
 
 
 class FontSize(Enum):
     """
     All supported font size enum
     """
 
@@ -61,29 +62,40 @@
 
     This class represents an LCD screen and provides methods to manipulate it.
     Each method returns self to enable chainable calls.
     """
 
     lib = load_lib(LIB_FILE_PATH)
 
-    def __init__(self, init_screen: bool = True):
+    def __init__(self, screen_dir: Literal[1, 2] = None):
+        """
+        Initializes the Screen class.
+
+        Parameters:
+            screen_dir (Literal[1, 2], optional): The direction to open the screen in. Defaults to None.
+
+        Returns:
+            None
+        """
 
-        if init_screen:
-            self.open(direction=2).fill_screen(Color.BLACK).refresh()
+        if screen_dir is not None:
+            self.open(direction=screen_dir).fill_screen(Color.BLACK).refresh()
 
     def open(self, direction: Literal[1, 2] = 2) -> Self:
         """
         Open the LCD and set the displaying direction.
 
         Args:
           direction (Literal[1, 2]): Display direction; 1 for vertical, 2 for horizontal.
 
         Returns:
           Self for chainable calls.
         """
+
+        _logger.info(f"Open LCD with direction: {direction}")
         self.lib.lcd_open(direction)
         return self
 
     def refresh(self) -> Self:
         """
         Refresh the screen, printing the display data from the cache onto the screen.
```

### Comparing `pyuptech-0.1.1/src/pyuptech/modules/sensors.py` & `pyuptech-0.1.2/src/pyuptech/modules/sensors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 import ctypes
 from time import perf_counter_ns
-from typing import Callable, Sequence, Self
+from typing import Self
 
 from .constant import LIB_FILE_PATH
 from .loader import _logger
 from .loader import load_lib
 
 E6 = 1000000
 
-PinModeSetter = Callable[[int], None]
-PinSetter = Callable[[int], None]
-PinGetter = Callable[[], int]
-
-IndexedGetter = Callable[[int], int]
-IndexedSetter = Callable[[int, int], None]
-
 OUTPUT = 1
 INPUT = 0
 HIGH = 1
 LOW = 0
 
 
 class OnBoardSensors:
@@ -62,21 +55,23 @@
         self.__adc_min_sample_interval_ns = value * E6
 
     @staticmethod
     def adc_io_open():
         """
         open the adc-io plug
         """
+        _logger.info("Initializing ADC-IO")
         return OnBoardSensors.__lib.adc_io_open()
 
     @staticmethod
     def adc_io_close():
         """
         close the adc-io plug
         """
+        _logger.info("Closing ADC-IO")
         OnBoardSensors.__lib.adc_io_close()
 
     @staticmethod
     def adc_all_channels():
         """
         这个函数的功能是从ADC（模拟到数字转换器）获取多个值，
         并将这些值存储到指定的内存位置。它通过spi_xfer函数调用来与ADC进行通信，并将获取的结果转换为16位整数，
@@ -108,21 +103,20 @@
           }
           while (a1 + 18 != v3);                 // 当a1和v3的和不等于18时循环
 
           return 0;                             // 返回0表示操作成功
         }
         """
         current = perf_counter_ns()
-        if (
-            current - OnBoardSensors.last_update_timestamp
-            < OnBoardSensors.__adc_min_sample_interval_ns
-        ):
+        samp_interval = OnBoardSensors.__adc_min_sample_interval_ns
+        if current - OnBoardSensors.last_update_timestamp < samp_interval:
             OnBoardSensors.last_update_timestamp = current
             return OnBoardSensors.acc_all
         OnBoardSensors.__lib.ADC_GetAll(OnBoardSensors._adc_all)
+
         return OnBoardSensors._adc_all
 
     def set_io_level(self, index: int, level: int) -> Self:
         """
         int __fastcall adc_io_Set(unsigned int a1, char a2)
         {
           char v3[12]; // [sp+4h] [bp-Ch] BYREF
@@ -254,17 +248,17 @@
             gyro: -+2000 degree/s
             sampling rate: 1kHz
         """
         _logger.info("initializing MPU6500")
         success = OnBoardSensors.__lib.mpu6500_dmp_init()
 
         if success:
-            _logger.critical("Failed to initialize MPU6500")
+            _logger.warning("Failed to initialize MPU6500")
         else:
-            _logger.info("#MPU6500 successfully initialized")
+            _logger.info("MPU6500 successfully initialized")
         return self
 
     @staticmethod
     def acc_all():
         """
         get the acceleration from MPU6500
         """
@@ -294,83 +288,7 @@
         OnBoardSensors.__lib.mpu6500_Get_Attitude(OnBoardSensors._atti_all)
 
         return OnBoardSensors._atti_all
 
     @staticmethod
     def get_handle(attr_name: str):
         return getattr(OnBoardSensors.__lib, attr_name)
-
-
-def pin_setter_constructor(indexed_setter: IndexedSetter, pin: int) -> PinSetter:
-    """
-
-    Args:
-        indexed_setter: the function that
-        pin: the pin to be connected
-
-    Returns:
-
-    """
-
-    def set_pin_level(level: int):
-        indexed_setter(pin, level)
-
-    return set_pin_level
-
-
-def pin_getter_constructor(indexed_getter: IndexedGetter, pin: int) -> PinGetter:
-    """
-
-    Args:
-        indexed_getter:
-        pin:
-
-    Returns:
-
-    """
-
-    def get_pin_level() -> int:
-        return indexed_getter(pin)
-
-    return get_pin_level
-
-
-def pin_mode_setter_constructor(
-    indexed_mode_setter: IndexedSetter, pin: int
-) -> PinModeSetter:
-    """
-
-    Args:
-        indexed_mode_setter: the function that sets the pin mode
-        pin: the pin to be connected
-
-    Returns:
-        the function that sets the pin mode with built-in pin value
-
-    """
-
-    def set_pin_mode(mode: int):
-        indexed_mode_setter(pin, mode)
-
-    return set_pin_mode
-
-
-def multiple_pin_mode_setter_constructor(
-    indexed_mode_setter: IndexedSetter, pins: Sequence[int]
-) -> PinModeSetter:
-    """
-
-    Args:
-        pins: the pin to be connected
-        indexed_mode_setter: the function that sets the pin mode
-
-
-    Returns:
-        the function that sets the pin mode with built-in pin value
-
-    """
-
-    def set_pin_mode(mode: int):
-        for pin in pins:
-            indexed_mode_setter(pin, mode)
-
-    return set_pin_mode
```

### Comparing `pyuptech-0.1.1/tests/perf_tests.py` & `pyuptech-0.1.2/tests/perf_tests.py`

 * *Files identical despite different names*

