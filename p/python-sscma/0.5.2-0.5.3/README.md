# Comparing `tmp/python-sscma-0.5.2.tar.gz` & `tmp/python-sscma-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sscma-0.5.2.tar", last modified: Tue Apr 16 09:13:47 2024, max compression
+gzip compressed data, was "python-sscma-0.5.3.tar", last modified: Thu Apr 18 02:28:13 2024, max compression
```

## Comparing `python-sscma-0.5.2.tar` & `python-sscma-0.5.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 09:13:47.944944 python-sscma-0.5.2/
--rw-rw-rw-   0        0        0     2914 2024-04-16 09:13:47.944944 python-sscma-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2396 2024-04-16 08:12:13.000000 python-sscma-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 09:13:47.916429 python-sscma-0.5.2/python_sscma.egg-info/
--rw-rw-rw-   0        0        0     2914 2024-04-16 09:13:47.000000 python-sscma-0.5.2/python_sscma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2024-04-16 09:13:47.000000 python-sscma-0.5.2/python_sscma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 09:13:47.000000 python-sscma-0.5.2/python_sscma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-16 09:13:47.000000 python-sscma-0.5.2/python_sscma.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2024-04-16 09:13:47.000000 python-sscma-0.5.2/python_sscma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 09:13:47.000000 python-sscma-0.5.2/python_sscma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 09:13:47.945941 python-sscma-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1310 2024-04-16 09:12:35.000000 python-sscma-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 09:13:47.917426 python-sscma-0.5.2/sscma/
--rw-rw-rw-   0        0        0       87 2024-04-16 09:13:18.000000 python-sscma-0.5.2/sscma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 09:13:47.921426 python-sscma-0.5.2/sscma/cli/
--rw-rw-rw-   0        0        0        0 2024-04-16 06:11:20.000000 python-sscma-0.5.2/sscma/cli/__init__.py
--rw-rw-rw-   0        0        0      253 2024-04-16 06:30:55.000000 python-sscma-0.5.2/sscma/cli/cli.py
--rw-rw-rw-   0        0        0     4773 2024-04-16 06:49:24.000000 python-sscma-0.5.2/sscma/cli/client.py
--rw-rw-rw-   0        0        0     2367 2024-04-16 06:12:54.000000 python-sscma-0.5.2/sscma/cli/flahser.py
-drwxrwxrwx   0        0        0        0 2024-04-16 09:13:47.925429 python-sscma-0.5.2/sscma/flashers/
--rw-rw-rw-   0        0        0       73 2024-04-16 06:11:41.000000 python-sscma-0.5.2/sscma/flashers/__init__.py
--rw-rw-rw-   0        0        0      768 2024-04-16 06:01:44.000000 python-sscma-0.5.2/sscma/flashers/base.py
--rw-rw-rw-   0        0        0     5161 2024-04-16 06:09:27.000000 python-sscma-0.5.2/sscma/flashers/core.py
-drwxrwxrwx   0        0        0        0 2024-04-16 09:13:47.926428 python-sscma-0.5.2/sscma/fonts/
--rw-rw-rw-   0        0        0  1580784 2024-04-16 05:34:06.000000 python-sscma-0.5.2/sscma/fonts/Arial.ttf
-drwxrwxrwx   0        0        0        0 2024-04-16 09:13:47.934942 python-sscma-0.5.2/sscma/micro/
--rw-rw-rw-   0        0        0      341 2024-04-16 05:34:06.000000 python-sscma-0.5.2/sscma/micro/__init__.py
--rw-rw-rw-   0        0        0    13707 2024-04-16 05:34:06.000000 python-sscma-0.5.2/sscma/micro/client.py
--rw-rw-rw-   0        0        0     4730 2024-04-16 05:34:06.000000 python-sscma-0.5.2/sscma/micro/const.py
--rw-rw-rw-   0        0        0    24553 2024-04-16 06:21:15.000000 python-sscma-0.5.2/sscma/micro/device.py
--rw-rw-rw-   0        0        0     1231 2024-04-16 05:34:06.000000 python-sscma-0.5.2/sscma/micro/exceptions.py
--rw-rw-rw-   0        0        0    10869 2024-04-16 05:34:06.000000 python-sscma-0.5.2/sscma/micro/info.py
-drwxrwxrwx   0        0        0        0 2024-04-16 09:13:47.936941 python-sscma-0.5.2/sscma/utils/
--rw-rw-rw-   0        0        0        0 2024-01-11 03:24:44.000000 python-sscma-0.5.2/sscma/utils/__init__.py
--rw-rw-rw-   0        0        0      844 2024-01-11 03:24:44.000000 python-sscma-0.5.2/sscma/utils/image.py
-drwxrwxrwx   0        0        0        0 2024-04-16 09:13:47.943943 python-sscma-0.5.2/tests/
--rw-rw-rw-   0        0        0      122 2024-04-16 05:34:06.000000 python-sscma-0.5.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2239 2024-04-16 05:34:06.000000 python-sscma-0.5.2/tests/test_mqtt.py
--rw-rw-rw-   0        0        0     2039 2024-04-16 05:34:06.000000 python-sscma-0.5.2/tests/test_mqttclient.py
--rw-rw-rw-   0        0        0     2135 2024-04-16 05:34:06.000000 python-sscma-0.5.2/tests/test_serial.py
--rw-rw-rw-   0        0        0     1540 2024-04-16 05:34:06.000000 python-sscma-0.5.2/tests/test_serialclient.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.830465 python-sscma-0.5.3/
+-rw-rw-rw-   0        0        0     2888 2024-04-18 02:28:13.830465 python-sscma-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2370 2024-04-18 02:26:49.000000 python-sscma-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.801664 python-sscma-0.5.3/python_sscma.egg-info/
+-rw-rw-rw-   0        0        0     2888 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 02:28:13.830465 python-sscma-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1310 2024-04-16 09:12:35.000000 python-sscma-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.802661 python-sscma-0.5.3/sscma/
+-rw-rw-rw-   0        0        0       87 2024-04-18 02:26:20.000000 python-sscma-0.5.3/sscma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.806662 python-sscma-0.5.3/sscma/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-16 06:11:20.000000 python-sscma-0.5.3/sscma/cli/__init__.py
+-rw-rw-rw-   0        0        0      253 2024-04-18 01:46:33.000000 python-sscma-0.5.3/sscma/cli/cli.py
+-rw-rw-rw-   0        0        0     4547 2024-04-18 02:07:12.000000 python-sscma-0.5.3/sscma/cli/client.py
+-rw-rw-rw-   0        0        0     3008 2024-04-18 02:25:18.000000 python-sscma-0.5.3/sscma/cli/flahser.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.809662 python-sscma-0.5.3/sscma/flashers/
+-rw-rw-rw-   0        0        0       73 2024-04-16 06:11:41.000000 python-sscma-0.5.3/sscma/flashers/__init__.py
+-rw-rw-rw-   0        0        0      941 2024-04-18 02:20:10.000000 python-sscma-0.5.3/sscma/flashers/base.py
+-rw-rw-rw-   0        0        0     5256 2024-04-18 02:26:00.000000 python-sscma-0.5.3/sscma/flashers/core.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.810661 python-sscma-0.5.3/sscma/fonts/
+-rw-rw-rw-   0        0        0  1580784 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/fonts/Arial.ttf
+drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.820627 python-sscma-0.5.3/sscma/micro/
+-rw-rw-rw-   0        0        0      341 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/micro/__init__.py
+-rw-rw-rw-   0        0        0    13707 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/micro/client.py
+-rw-rw-rw-   0        0        0     4730 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/micro/const.py
+-rw-rw-rw-   0        0        0    24553 2024-04-16 06:21:15.000000 python-sscma-0.5.3/sscma/micro/device.py
+-rw-rw-rw-   0        0        0     1231 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/micro/exceptions.py
+-rw-rw-rw-   0        0        0    10869 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/micro/info.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.822627 python-sscma-0.5.3/sscma/utils/
+-rw-rw-rw-   0        0        0        0 2024-01-11 03:24:44.000000 python-sscma-0.5.3/sscma/utils/__init__.py
+-rw-rw-rw-   0        0        0      844 2024-01-11 03:24:44.000000 python-sscma-0.5.3/sscma/utils/image.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.828630 python-sscma-0.5.3/tests/
+-rw-rw-rw-   0        0        0      122 2024-04-16 05:34:06.000000 python-sscma-0.5.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2239 2024-04-16 05:34:06.000000 python-sscma-0.5.3/tests/test_mqtt.py
+-rw-rw-rw-   0        0        0     2039 2024-04-16 05:34:06.000000 python-sscma-0.5.3/tests/test_mqttclient.py
+-rw-rw-rw-   0        0        0     2135 2024-04-16 05:34:06.000000 python-sscma-0.5.3/tests/test_serial.py
+-rw-rw-rw-   0        0        0     1540 2024-04-16 05:34:06.000000 python-sscma-0.5.3/tests/test_serialclient.py
```

### Comparing `python-sscma-0.5.2/PKG-INFO` & `python-sscma-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sscma
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python library for sscma
 Home-page: https://github.com/Seeed-Studio/python-sscma
 Author: Seeed Studio
 Author-email: lht856@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -55,16 +55,15 @@
 Options:
   -B, --broker TEXT       Specify the MQTT broker address
   -U, --username TEXT     Specify the MQTT username
   -P, --password TEXT     Specify the MQTT password
   -D, --device TEXT       Specify the Device ID
   -p, --port TEXT         Specify the Port to connect to
   -b, --baudrate INTEGER  Specify the Baudrate for the serial connection
-  --sample                Enable the sample mode
-  --invoke                Enable the invoke mode
+  --sample                Enable the Sample mode, default is Invoke mode
   -s, --save              Enable the save mode
   -o, --save_dir TEXT     Specify the Directory for saveing images
   -h, --headless          Run the program without displaying the images
   -v, --verbose           Show detailed information during processin
   --help                  Show this message and exit.
 ```
```

### Comparing `python-sscma-0.5.2/README.md` & `python-sscma-0.5.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,15 @@
 Options:
   -B, --broker TEXT       Specify the MQTT broker address
   -U, --username TEXT     Specify the MQTT username
   -P, --password TEXT     Specify the MQTT password
   -D, --device TEXT       Specify the Device ID
   -p, --port TEXT         Specify the Port to connect to
   -b, --baudrate INTEGER  Specify the Baudrate for the serial connection
-  --sample                Enable the sample mode
-  --invoke                Enable the invoke mode
+  --sample                Enable the Sample mode, default is Invoke mode
   -s, --save              Enable the save mode
   -o, --save_dir TEXT     Specify the Directory for saveing images
   -h, --headless          Run the program without displaying the images
   -v, --verbose           Show detailed information during processin
   --help                  Show this message and exit.
 ```
```

### Comparing `python-sscma-0.5.2/python_sscma.egg-info/PKG-INFO` & `python-sscma-0.5.3/python_sscma.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sscma
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python library for sscma
 Home-page: https://github.com/Seeed-Studio/python-sscma
 Author: Seeed Studio
 Author-email: lht856@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -55,16 +55,15 @@
 Options:
   -B, --broker TEXT       Specify the MQTT broker address
   -U, --username TEXT     Specify the MQTT username
   -P, --password TEXT     Specify the MQTT password
   -D, --device TEXT       Specify the Device ID
   -p, --port TEXT         Specify the Port to connect to
   -b, --baudrate INTEGER  Specify the Baudrate for the serial connection
-  --sample                Enable the sample mode
-  --invoke                Enable the invoke mode
+  --sample                Enable the Sample mode, default is Invoke mode
   -s, --save              Enable the save mode
   -o, --save_dir TEXT     Specify the Directory for saveing images
   -h, --headless          Run the program without displaying the images
   -v, --verbose           Show detailed information during processin
   --help                  Show this message and exit.
 ```
```

### Comparing `python-sscma-0.5.2/python_sscma.egg-info/SOURCES.txt` & `python-sscma-0.5.3/python_sscma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/setup.py` & `python-sscma-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/sscma/cli/client.py` & `python-sscma-0.5.3/sscma/cli/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,36 +6,31 @@
 import click
 
 from sscma.micro.client import SerialClient, MQTTClient
 from sscma.micro.device import Device
 from sscma.micro.const import *
 from sscma.utils.image import  image_from_base64
 
-logging.basicConfig(level=logging.INFO)
+logging.basicConfig(level=logging.WARNING)
 
 @click.command()
 @click.option('--broker', '-B', default=None, help='Specify the MQTT broker address')
 @click.option('--username', '-U', default=None, help='Specify the MQTT username')
 @click.option('--password', '-P', default=None, help='Specify the MQTT password')
 @click.option('--device', '-D', default=None, help='Specify the Device ID')
 @click.option('--port', '-p', default=None, help='Specify the Port to connect to')
 @click.option('--baudrate',  '-b', default=921600, help='Specify the Baudrate for the serial connection')
-@click.option('--sample', is_flag=True, help='Enable the sample mode')
-@click.option('--invoke', is_flag=True, default=True, help='Enable the invoke mode')
+@click.option('--sample', is_flag=True,  default=False, help='Enable the Sample mode, default is Invoke mode')
 @click.option('--save', '-s', is_flag=True, default=False, help='Enable the save mode')
 @click.option('--save_dir', '-o', default="save", help="Specify the Directory for saveing images")
 @click.option('--headless', '-h', is_flag=True,  help='Run the program without displaying the images')
 @click.option('--verbose', '-v', is_flag=True, help='Show detailed information during processin')
-def client(broker, username, password, device, port, baudrate, sample, invoke, save, save_dir, headless, verbose):
+def client(broker, username, password, device, port, baudrate, sample, save, save_dir, headless, verbose):
     try:
         
-        if sample and invoke:
-            click.echo("Error: 'sample' and 'invoke' options are mutually exclusive. Please choose one.")
-            return
-        
         try:
             if int(save) > 0:
                 if not os.path.exists(os.path.join(save_dir)):
                     os.mkdir(os.path.join(save_dir))
                 if not os.path.exists(os.path.join(save_dir, 'raw')):
                     os.mkdir(os.path.join(save_dir, 'raw'))
             if int(save) > 1:
@@ -85,15 +80,15 @@
             
         def on_connect(device):
             click.echo("Device connected")
             if not headless:
                 click.echo("\nEnter'ESC' to exit\n")
             if sample:
                 device.Sample(-1)
-            elif invoke:
+            else:
                 device.Invoke(-1)
             
         def on_disconnect(device):
             click.echo("Device disconnected")
             
         def on_log(device, log):
             click.echo(log)
```

### Comparing `python-sscma-0.5.2/sscma/cli/flahser.py` & `python-sscma-0.5.3/sscma/cli/flahser.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,49 +9,61 @@
         from serial.tools.list_ports_windows import comports
     elif os.name == 'posix':
         from serial.tools.list_ports_posix import comports
     else:
         raise ImportError("Sorry: no implementation for your platform ('{}') available".format(os.name))
     
     ports = comports()
+    selected_port = None
+    selected_flasher = None
 
     if len(ports) == 0:
         raise Exception('No Device Found')
     
  
-    if com is None:
-        # 如果未指定 com 口，则让用户选择
+    if com is None and len(ports) > 1:
+        # if we don't specify com port, let user select one
         click.echo("Multiple COM ports detected. Please select one:")
         for idx, port in enumerate(ports):
             click.echo(f"{idx + 1}. {port.device}")
         choice = click.prompt("Enter the number of the COM port", type=int)
         selected_port = ports[choice - 1]
     else:
         for port in ports:
-            if port.device == com:
-                selected_port = port
+            selected_port = port
+            if selected_port.device == com:
                 break
     
     for flasher in FLASHERS:
         if flasher.match(selected_port):
-            return flasher, selected_port.device
+            selected_flasher = flasher
+            break
+        
+    if selected_flasher is None and selected_port is not None:
+            click.echo(("Found device {}. Please select flasher.").format(selected_flasher))
+            for idx, flasher in enumerate(FLASHERS):
+                click.echo(f"{idx + 1}. {flasher.name()}")
+                choice = click.prompt("Enter the number of the flasher", type=int)
+                selected_flasher = FLASHERS[choice - 1]
+            else:
+                click.echo("No device found. Exiting.")
     
-    return None, None
+    return selected_flasher, selected_port.device
 
 @click.command()
 @click.option('--port', '-p', default=None, help='Port to connect to')
 @click.option('--file', '-f', default=None, help='File to write to the device')
 @click.option('--baudrate',  '-b', default=921600, help='Baud rate for the serial connection')
 @click.option('--offset', '-o', default='0x00', help='Offset to write the file to')
 def flasher(port, baudrate, file, offset):
     try:
         Flasher, device = get_flasher_by_port(port)
         
-        if not Flasher:
-            click.echo("No flasher found. Exiting.")
+        if Flasher is None or device is None:
+            click.echo("No device found. Exiting.")
             return
         
         flasher = Flasher(device, baudrate=baudrate)
         if file:
             with open(file, 'rb') as file:
                 data = file.read()
                 click.echo(("Found device {}. Writing file to device...").format(device))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python-sscma-0.5.2/sscma/flashers/base.py` & `python-sscma-0.5.3/sscma/flashers/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,22 @@
     def __init__(self, *args, **kwargs):
         """Initialize the programmer.
 
         This method should be overridden by the subclass.
         """
         pass
     
+    @classmethod
+    def name():
+        """Get the name of the programmer.
+
+        This method should be overridden by the subclass.
+        """
+        pass
+    
 
     @classmethod
     @abstractmethod
     def match(port):
         """Match the programmer.
 
         This method should be overridden by the subclass.
```

### Comparing `python-sscma-0.5.2/sscma/flashers/core.py` & `python-sscma-0.5.3/sscma/flashers/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from xmodem import XMODEM
 
 from sscma.flashers.base import BaseFlasher
 
 
 class HimaxFlasher(BaseFlasher):
     
+    _NAME = "Himax Flasher"
+    
     _USB = [{"vid": 0x1A86, "pid": 0x55D2},
             {"vid": 0x1A86, "pid": 0x55D3}]
     
     def __init__(self, port, baudrate=921600, timeout=1):
         self.port = port
         self.baudrate = baudrate
         self.timeout = timeout
@@ -26,22 +28,26 @@
         self.log = logging.getLogger('sscma.flasher')
         
         #logging.getLogger('xmodem.XMODEM').setLevel(logging.CRITICAL + 1)
 
     
         super().__init__()
         
+    def name():
+        return HimaxFlasher._NAME
+        
     def match(port):
+
         for usb in HimaxFlasher._USB:
             if usb['vid'] == port.vid and usb['pid'] == port.pid:
                 return True
         return False
         
 
-        
+    
     def getc(self, size, timeout=1):
         data = self.serial.read(size) or None
         return data
     
     def putc(self, data, timeout=1):
         return self.serial.write(data) or None
```

### Comparing `python-sscma-0.5.2/sscma/fonts/Arial.ttf` & `python-sscma-0.5.3/sscma/fonts/Arial.ttf`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/sscma/micro/client.py` & `python-sscma-0.5.3/sscma/micro/client.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/sscma/micro/const.py` & `python-sscma-0.5.3/sscma/micro/const.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/sscma/micro/device.py` & `python-sscma-0.5.3/sscma/micro/device.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/sscma/micro/exceptions.py` & `python-sscma-0.5.3/sscma/micro/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/sscma/micro/info.py` & `python-sscma-0.5.3/sscma/micro/info.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/sscma/utils/image.py` & `python-sscma-0.5.3/sscma/utils/image.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/tests/test_mqtt.py` & `python-sscma-0.5.3/tests/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/tests/test_mqttclient.py` & `python-sscma-0.5.3/tests/test_mqttclient.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/tests/test_serial.py` & `python-sscma-0.5.3/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.2/tests/test_serialclient.py` & `python-sscma-0.5.3/tests/test_serialclient.py`

 * *Files identical despite different names*

