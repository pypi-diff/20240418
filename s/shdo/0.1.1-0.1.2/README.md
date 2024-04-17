# Comparing `tmp/shdo-0.1.1.tar.gz` & `tmp/shdo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shdo-0.1.1.tar", last modified: Mon Apr  8 23:15:25 2024, max compression
+gzip compressed data, was "shdo-0.1.2.tar", last modified: Wed Apr 17 22:44:40 2024, max compression
```

## Comparing `shdo-0.1.1.tar` & `shdo-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 23:15:25.894862 shdo-0.1.1/
--rw-rw-rw-   0        0        0      350 2024-04-08 23:15:25.892394 shdo-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2036 2024-04-08 14:07:04.000000 shdo-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 23:15:25.894862 shdo-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      640 2024-04-08 23:15:22.000000 shdo-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 23:15:25.890590 shdo-0.1.1/shdo.egg-info/
--rw-rw-rw-   0        0        0      350 2024-04-08 23:15:25.000000 shdo-0.1.1/shdo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-04-08 23:15:25.000000 shdo-0.1.1/shdo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 23:15:25.000000 shdo-0.1.1/shdo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-08 23:15:25.000000 shdo-0.1.1/shdo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-08 23:15:25.000000 shdo-0.1.1/shdo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18488 2024-04-08 23:15:09.000000 shdo-0.1.1/shdo.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:44:40.307176 shdo-0.1.2/
+-rw-rw-rw-   0        0        0      350 2024-04-17 22:44:40.304953 shdo-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2118 2024-04-17 22:40:49.000000 shdo-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 22:44:40.308173 shdo-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      640 2024-04-17 22:41:28.000000 shdo-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 22:44:40.302585 shdo-0.1.2/shdo.egg-info/
+-rw-rw-rw-   0        0        0      350 2024-04-17 22:44:39.000000 shdo-0.1.2/shdo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-17 22:44:40.000000 shdo-0.1.2/shdo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 22:44:39.000000 shdo-0.1.2/shdo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-17 22:44:39.000000 shdo-0.1.2/shdo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-17 22:44:39.000000 shdo-0.1.2/shdo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16216 2024-04-17 22:39:16.000000 shdo-0.1.2/shdo.py
```

### Comparing `shdo-0.1.1/README.md` & `shdo-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# SHDO
+# shdo
 
-Shdo is a tool to escalate privilege (like sudo) for Android that don't need any computer to be installed.
+shdo is a tool to escalate privilege (like sudo) for Android that don't need any computer to be installed.
 
 
 ## Features
 
-- Fast pairing with 'shdo-pair'
-- Fast command execution with 'shdo'
+- Fast pairing with **shdo-pair**
+- Fast command execution with **shdo**
 - Bruteforce all ports needed for pairing or execution
-- Automatically move scripts or executables to permissive folders
-- Check if the adb daemon is running
 
 
 ## How to Install
 
-To install the tool first you will need the Termux application. Because the Termux app is not updated anymore on the Play Store you will need to download it from an alternative store: [F-Droid](https://f-droid.org/fr/packages/com.termux/).
+To install the tool first you will need the **Termux** application. Because the Termux app is not updated anymore on the Play Store you will need to download it from an alternative store: [F-Droid](https://f-droid.org/fr/packages/com.termux/).
 
 After installing Termux we will use it to install three things: the Android Debug Bridge (ADB), Python 3 and Shdo.
 
 To install **ADB** just run the command to install the packages:
 > apt-get install android-tools
 
 Then you will need **Python 3** to run the shdo tool. You can simply install it with the following command:
@@ -26,27 +24,28 @@
 
 When Python 3 is installed you can install **shdo** by running:
 > pip install shdo
 
 
 ## How to Use
 
-First you need to pair shdo with your ADB daemon. To do that you can use the **shdo-pair** command.
+First you need to pair shdo with your ADB daemon. To do that you can use the **shdo-pair** command with your pairing code.
+And to get your pairing code just go into the Developer Settings then into Wireless Debugging and hit **Pair device with pairing code**.
 > shdo-pair PAIRING_CODE
 
 The only problem is that the code disapear everytime you leave the Settings app. To bypass this problem we can use **Applications Split-Screening** to keep our Settings app alive, and enter the code in the other Termux window.
 
-![Split-Screening between Termux and Settings](split-screen.png)
+![Split-Screening between Termux and Settings](./img/split-screen.png)
 
 When the pairing is done you can run as much command as you want with **shell** privileges using shdo direclty:
 > shdo COMMAND
 
-![whoami results example](whoami.png)
+![whoami results example](./img/whoami.png)
 
 If you don't want to do the pairing every few days/weeks you can disable the **adb authorization timeout** in the Developer Settings. That way your pairing will also still works after reboots.
 
-![disable adb authorization timeout](timeout.png)
+![disable adb authorization timeout](./img/timeout.png)
 
 
 ## Credits
 
 - [Mathias Bochet](https://www.linkedin.com/in/mathias-bochet/) (aka Zen)
```

### Comparing `shdo-0.1.1/setup.py` & `shdo-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='shdo',
-    version='0.1.1',
+    version='0.1.2',
     packages=['shdo'],
     package_dir={'shdo': '.'},
     py_modules=['shdo'],
     entry_points={
         'console_scripts': [
             'shdo = shdo:main',
             'shdo-pair = shdo:main',
```

### Comparing `shdo-0.1.1/shdo.py` & `shdo-0.1.2/shdo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 from sys import argv as sys_argv
 from os import environ
 
 # import the file functions
 from os.path import exists as file_exists
 from shutil import copy as file_copy, SameFileError
 
-# import the path function
-from os.path import expanduser as path_get_user_directory
-from os.path import join as path_join
-
 # import the network functions
 from socket import socket as socket_open, AF_INET, SOCK_STREAM
 
 # import the command execution functions
 from os import system
 from subprocess import Popen, PIPE
 
@@ -23,26 +19,24 @@
 # import the user functions
 from getpass import getuser
 from os import getcwd, stat
 from pwd import getpwuid
 
 
 # shdo settings
-SHDO_AUTO_BOUNCE = True
-SHDO_BOUNCE_FOLDER_PATH = "/storage/self/primary/"
-SHDO_DEBUG_FOLDER_PATH = "/data/local/tmp/"
-ADB_SERVER_PORT_FILENAME = ".last_adb_server_port"
+ADB_SERVER_PORT_FILENAME = "~/.last_adb_server_port"
 
 
 # shdo global variables
 adb_is_paired = None
 current_adb_port = None
 connected_adb_port = None
 
 
+# main function
 def main():
 
     # parse the command line parameters
     argc = len(sys_argv)
     argv = sys_argv
 
     # check if there is no command
@@ -132,63 +126,19 @@
         if _adb.connect(verbose=verbose) == False:
 
             # print the error if needed
             print("Error: Couldn't connect to the adb server. Are you sure the adb server is paired with Termux ? Are you sure the adb wi-fi is on ?")
             
             # couldn't connect to the adb server
             return None
-        
-    # auto-bounce the file or executable if needed
-    if SHDO_AUTO_BOUNCE == True and command is not None:
-
-        # check if the command is an executable (bash, elf, ...)
-        if file_exists(command) == True:
-
-            # remove extra dot
-            if command.startswith("./") == True:
-                filename = command[2:]
-
-            # check if we're in a Termux folder
-            if _terminal.in_termux_folder() == True:
-
-                # copy the file to the bounce folder
-                if verbose == True:
-                    print(f"[*] Copying the file {filename} to bounce folder...", end='', flush=True)
-                bounce_path = SHDO_BOUNCE_FOLDER_PATH + filename
-                try:
-                    file_copy(filename, bounce_path)
-                except SameFileError:
-                    pass
-                if verbose == True:
-                    print("done.")
-
-            # check if we're in a Termux folder
-            if _terminal.in_shell_folder() == False:
-
-                # copy the file to the debug folder
-                if verbose == True:
-                    print(f"[*] Copying the file {filename} to debug folder...", end='', flush=True)
-                debug_path = SHDO_DEBUG_FOLDER_PATH + filename
-                _adb.shell(f"cp '{bounce_path}' '{debug_path}'")
-                if verbose == True:
-                    print("done.")
-
-            # give execution permission to the script or executable
-            if verbose == True:
-                print(f"[*] Giving the file {filename} execution permission...", end='', flush=True)
-            _adb.shell(f"chmod 755 '{debug_path}'")
-            if verbose == True:
-                print("done.")
-            
-            # change the command by its new path
-            command = debug_path
 
     # build the full command
     full_command = f"'{command}'" if command is not None else None
-    full_command += f" {parameters}" if parameters is not None else ""
+    if command is not None:
+        full_command += f" {parameters}" if parameters is not None else ""
         
     # run the elevated command
     return _adb.execute(full_command, verbose=verbose)
 
 
 # handle everything about android debug bridge
 class _adb:
@@ -468,21 +418,17 @@
 class _cache:
         
     # load the adb server port
     def load(verbose=False):
         if verbose == True:
             print("[*] Loading adb server port from a file...", end='', flush=True)
 
-        # build the file path
-        home = path_get_user_directory("~")
-        filepath = path_join(home, ADB_SERVER_PORT_FILENAME)
-
         # open the file
         try:
-            with open(filepath, 'r') as file:
+            with open(ADB_SERVER_PORT_FILENAME, 'r') as file:
 
                 # read the adb server port from the file
                 adb_server_port = int(file.read())
 
         # check for errors
         except FileNotFoundError:
             if verbose == True:
@@ -497,19 +443,17 @@
 
     # save the adb server port
     def save(adb_server_port, verbose=False):
 
         # build the cache file path
         if verbose == True:
             print("[*] Saving adb server port to a file...", end='', flush=True)
-        home = path_get_user_directory("~")
-        filepath = path_join(home, ADB_SERVER_PORT_FILENAME)
 
         # save the cache file
-        with open(filepath, 'w') as file:
+        with open(ADB_SERVER_PORT_FILENAME, 'w') as file:
             file.write(str(adb_server_port))
         if verbose == True:
             print("success.")
 
 
 # handle everything about network
 class _network:
```

