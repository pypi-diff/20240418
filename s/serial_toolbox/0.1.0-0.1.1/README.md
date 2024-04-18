# Comparing `tmp/serial_toolbox-0.1.0.tar.gz` & `tmp/serial_toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serial_toolbox-0.1.0.tar", max compression
+gzip compressed data, was "serial_toolbox-0.1.1.tar", max compression
```

## Comparing `serial_toolbox-0.1.0.tar` & `serial_toolbox-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35184 2024-04-17 14:00:19.176430 serial_toolbox-0.1.0/LICENSE
--rw-r--r--   0        0        0      680 2024-04-17 14:02:35.157982 serial_toolbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      692 2024-04-17 14:01:35.426512 serial_toolbox-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-17 14:00:19.230977 serial_toolbox-0.1.0/serial_toolbox/__init__.py
--rw-r--r--   0        0        0     4632 2024-04-17 14:00:19.230977 serial_toolbox-0.1.0/serial_toolbox/connect.py
--rw-r--r--   0        0        0     5407 2024-04-17 14:00:19.231977 serial_toolbox-0.1.0/serial_toolbox/gui.py
--rw-r--r--   0        0        0     4368 2024-04-17 14:00:19.231977 serial_toolbox-0.1.0/serial_toolbox/interface_core.py
--rw-r--r--   0        0        0      911 2024-04-17 14:00:19.232977 serial_toolbox-0.1.0/serial_toolbox/log_init.py
--rw-r--r--   0        0        0     1510 1970-01-01 00:00:00.000000 serial_toolbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35184 2024-04-17 14:00:19.176430 serial_toolbox-0.1.1/LICENSE
+-rw-r--r--   0        0        0      681 2024-04-17 15:06:59.477652 serial_toolbox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      692 2024-04-17 14:01:35.426512 serial_toolbox-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 14:00:19.230977 serial_toolbox-0.1.1/serial_toolbox/__init__.py
+-rw-r--r--   0        0        0     4854 2024-04-17 15:06:16.439508 serial_toolbox-0.1.1/serial_toolbox/connect.py
+-rw-r--r--   0        0        0     5528 2024-04-17 15:06:16.445509 serial_toolbox-0.1.1/serial_toolbox/gui.py
+-rw-r--r--   0        0        0     4539 2024-04-17 15:06:16.454508 serial_toolbox-0.1.1/serial_toolbox/interface_core.py
+-rw-r--r--   0        0        0      911 2024-04-17 14:00:19.232977 serial_toolbox-0.1.1/serial_toolbox/log_init.py
+-rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 serial_toolbox-0.1.1/PKG-INFO
```

### Comparing `serial_toolbox-0.1.0/LICENSE` & `serial_toolbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_toolbox-0.1.0/pyproject.toml` & `serial_toolbox-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "serial_toolbox"
-version = "0.1.0"
+version = "0.1.1"
 description = "Utility functions for pySerial"
 authors = ["Takuya Sasatani <33111879+t-sasatani@users.noreply.github.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 pyserial = "^3.5"
 coloredlogs = "^15.0.1"
 myst-parser = "^2.0.0"
 matplotlib = "^3.8.4"
 customtkinter = "^5.2.2"
```

### Comparing `serial_toolbox-0.1.0/README.md` & `serial_toolbox-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `serial_toolbox-0.1.0/serial_toolbox/connect.py` & `serial_toolbox-0.1.1/serial_toolbox/connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 
 class port_manager:
     """
     A utility class for managing asynchronous communication over serial ports.
     """
     
     @classmethod
-    def select_port(cls, interactive: bool=False, baudrate: int=115200, timeout: float=0.1,
+    def select_port(cls, interactive: bool=False, portname: str=None, baudrate: int=115200, timeout: float=0.1,
                     logger: logging.Logger=None) -> serial.Serial:
         """
         Class method for selecting the port for serial communication.
         
         Parameters
         ----------
         interactive : bool, optional
             User interactive mode switch, default is False
+        portname : str, optional
+            User identifier for port, default is None
         baudrate : int, optional
             The baudrate, default is 9600
         timeout : float, optional
             The timeout, default is 0.1
         logger : logging.Logger, optional
             The logger object, default is None
 
@@ -33,15 +35,19 @@
             Initialized serial port.
         """
         if logger is None:
             logger = log_init()
         
         ser = serial.Serial()
         
-        print("Setup serial. [] is default value.")
+        if portname:
+            print("Setup port (" + portname + "). [] is default value.")
+        else:
+            print("Setup port. [] is default value.")
+
         if interactive:
             baudrate_input = input("baudrate [115200] >> ")
             if baudrate_input.strip():
                 baudrate = int(baudrate_input)
             timeout_input = input("timeout [0.1] >> ")
             if timeout_input.strip():
                 timeout = float(timeout_input)  # convert input to float
@@ -141,8 +147,8 @@
                     logger.info('waiting for closing serial port')
                     time.sleep(1)
                 logger.info('Finished closing serial port.')
             else:
                 logger.info('Serial port is available')
         except Exception as e:
             logger.error(e)
-            return None
+            return None
```

### Comparing `serial_toolbox-0.1.0/serial_toolbox/gui.py` & `serial_toolbox-0.1.1/serial_toolbox/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,11 +116,13 @@
         
 
 def serial_monitor_gui():
     """
     Start and run the customtkinter application. 
     This is the main entry point of the application that creates an instance of the Application class and executes the main loop.
     """
-
-    target_serial_interface = serial_interface(port_manager.select_port(interactive=True), terminal=False, max_queue_size=200)
+    port_interface = port_manager.select_port(interactive=True, portname="serial monitor")
+    if not port_interface:
+        return
+    target_serial_interface = serial_interface(port_interface=port_interface, terminal=False, max_queue_size=200)
     app = Application(target_serial_interface)
     app.mainloop()
```

### Comparing `serial_toolbox-0.1.0/serial_toolbox/interface_core.py` & `serial_toolbox-0.1.1/serial_toolbox/interface_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,18 +60,22 @@
         Continuously reads data from the serial port until stop_flag is set to True.
 
         Parameters
         ----------
         serial_port : serial.Serial
             Instance of the serial port to read from.
         """
-        while not self.stop_flag:
-            if serial_port.in_waiting:
-                line = serial_port.readline().decode('utf-8').strip()
-                self.process_data(line)
+        try:
+            while not self.stop_flag:
+                if serial_port.in_waiting:
+                    line = serial_port.readline().decode('utf-8').strip()
+                    self.process_data(line)
+        except Exception as e:
+            print(e)
+            return
         serial_port.close()
 
     def process_data(self, data):
         """
         Processes incoming data by adding the data to the data_queue.
 
         Parameters
@@ -116,16 +120,19 @@
     
     The reading thread continuously reads data from the serial port and prints to the console
     until KeyboardInterrupt is caught.
     
     The thread is closed properly by setting its stop_flag to True and waiting for
     the thread to finish execution before returning from the function.    
     """    
-    port = port_manager.select_port(interactive)
+    port = port_manager.select_port(interactive, portname="serial monitor")
+    if not port:
+        return
     interface = serial_interface(port)
+    
 
     print("\nSerial port monitor started. Press Ctrl+C to stop.\n")
 
     try:
         while True: 
             pass
     except KeyboardInterrupt:
```

### Comparing `serial_toolbox-0.1.0/serial_toolbox/log_init.py` & `serial_toolbox-0.1.1/serial_toolbox/log_init.py`

 * *Files identical despite different names*

### Comparing `serial_toolbox-0.1.0/PKG-INFO` & `serial_toolbox-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: serial_toolbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utility functions for pySerial
 License: AGPL-3.0
 Author: Takuya Sasatani
 Author-email: 33111879+t-sasatani@users.noreply.github.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: customtkinter (>=5.2.2,<6.0.0)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: myst-parser (>=2.0.0,<3.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
```

