# Comparing `tmp/pysshpass-0.1.0.tar.gz` & `tmp/pysshpass-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysshpass-0.1.0.tar", last modified: Fri Oct 27 14:43:08 2023, max compression
+gzip compressed data, was "pysshpass-0.1.1.tar", last modified: Thu Apr 18 16:02:38 2024, max compression
```

## Comparing `pysshpass-0.1.0.tar` & `pysshpass-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-10-27 14:43:08.130157 pysshpass-0.1.0/
--rw-rw-rw-   0        0        0     4627 2023-10-27 14:43:08.128155 pysshpass-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-10-27 14:43:08.114035 pysshpass-0.1.0/PySSHPass/
--rw-rw-rw-   0        0        0        0 2023-10-27 13:45:59.000000 pysshpass-0.1.0/PySSHPass/__init__.py
--rw-rw-rw-   0        0        0     4695 2023-10-27 14:28:07.000000 pysshpass-0.1.0/PySSHPass/pysshpass.py
--rw-rw-rw-   0        0        0     4062 2023-10-27 14:23:55.000000 pysshpass-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-10-27 14:43:08.126142 pysshpass-0.1.0/pysshpass.egg-info/
--rw-rw-rw-   0        0        0     4627 2023-10-27 14:43:08.000000 pysshpass-0.1.0/pysshpass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-10-27 14:43:08.000000 pysshpass-0.1.0/pysshpass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-27 14:43:08.000000 pysshpass-0.1.0/pysshpass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-10-27 14:43:08.000000 pysshpass-0.1.0/pysshpass.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-10-27 14:43:08.000000 pysshpass-0.1.0/pysshpass.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-10-27 14:43:08.000000 pysshpass-0.1.0/pysshpass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-27 14:43:08.130157 pysshpass-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-10-27 14:42:40.000000 pysshpass-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 16:02:38.855693 pysshpass-0.1.1/
+-rw-rw-rw-   0        0        0    35149 2023-10-27 14:46:28.000000 pysshpass-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6668 2024-04-18 16:02:38.854694 pysshpass-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 16:02:38.840693 pysshpass-0.1.1/PySSHPass/
+-rw-rw-rw-   0        0        0        0 2023-10-27 13:45:59.000000 pysshpass-0.1.1/PySSHPass/__init__.py
+-rw-rw-rw-   0        0        0     4696 2024-04-18 15:52:00.000000 pysshpass-0.1.1/PySSHPass/pysshpass.py
+-rw-rw-rw-   0        0        0     6107 2024-04-18 16:02:36.000000 pysshpass-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 16:02:38.852693 pysshpass-0.1.1/pysshpass.egg-info/
+-rw-rw-rw-   0        0        0     6668 2024-04-18 16:02:38.000000 pysshpass-0.1.1/pysshpass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-18 16:02:38.000000 pysshpass-0.1.1/pysshpass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 16:02:38.000000 pysshpass-0.1.1/pysshpass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-18 16:02:38.000000 pysshpass-0.1.1/pysshpass.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-04-18 16:02:38.000000 pysshpass-0.1.1/pysshpass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-18 16:02:38.000000 pysshpass-0.1.1/pysshpass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 16:02:38.856692 pysshpass-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      943 2024-04-18 15:45:40.000000 pysshpass-0.1.1/setup.py
```

### Comparing `pysshpass-0.1.0/PKG-INFO` & `pysshpass-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pysshpass
-Version: 0.1.0
-Summary: Python-based SSH client designed to offer a multiplatform alternative to `sshpass`.
-Home-page: https://github.com/scottpeterman/pysshpass
-Author: Scott Peterman
-Author-email: scottpeterman@gmail.com
-License: GPLv3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: paramiko>=3.3.1
-Requires-Dist: click>=8.1.7
-
 ## pysshpass: A Multiplatform SSH Automation Utility
 
 ### Overview
 
 `pysshpass` is a Python-based SSH client designed to offer a multiplatform alternative to `sshpass`. This utility aims to address two core challenges:
 
 1. **Windows Compatibility**: Native `sshpass` options are limited on Windows, and `pysshpass` serves as a versatile replacement.
@@ -64,29 +49,41 @@
 - Working with multi-modal command-line interfaces
 - Gathering information during network audits, especially for devices not well-supported by existing automation libraries
 
 ---
 ### CLI Usage
 
 ```commandline
->python pysshpass.py --help
-Usage: pysshpass.py [OPTIONS]
+pysshpass --help
+Usage: pysshpass [OPTIONS]
 
-Options:
-  -h, --host TEXT         SSH Host (ip:port)  [required]
-  -u, --user TEXT         SSH Username  [required]
-  -p, --password TEXT     SSH Password  [required]
-  -c, --cmds TEXT         Commands to run, separated by comma
-  --invoke-shell          Invoke shell before running the command
-  --prompt TEXT           Prompt to look for before breaking the shell     
-  --prompt-count INTEGER  Number of prompts to look for before breaking the
-                          shell
-  -t, --timeout INTEGER   Command timeout duration in seconds
-  --help                  Show this message and exit.
+  SSH Client for running remote commands.
 
+  Sample Usage: pysshpass -h "172.16.1.101" -u "cisco" -p "cisco" -c "term len
+  0,show users,show run,show cdp neigh,show int desc" --invoke-shell --prompt
+  "#" --prompt-count 4 -t 15
+
+Options:
+  -h, --host TEXT                 SSH Host (ip:port)  [required]
+  -u, --user TEXT                 SSH Username  [required]
+  -p, --password TEXT             SSH Password  [required]
+  -c, --cmds TEXT                 Commands to run, separated by comma
+  --invoke-shell                  Invoke shell before running the command
+                                  [default=True]
+  --prompt TEXT                   Prompt to look for before breaking the shell
+  --prompt-count INTEGER          Number of prompts to look for before
+                                  breaking the shell
+  -t, --timeout INTEGER           Command timeout duration in seconds
+  --auto-add-policy               Automatically add the host key
+                                  [default=True]
+  --look-for-keys                 Look for local SSH key [default=False]
+  -i, --inter-command-time INTEGER
+                                  Inter-command time in seconds [default is 1
+                                  second]
+  --help                          Show this message and exit.
 
 
 ```
 ---
 ### Function `read_output`
 
 - This function reads the output of the SSH session in real-time and prints it to the standard output.
@@ -104,7 +101,43 @@
 
 ### User Prompt Management
 
 - The code uses a queue (`output_queue`) to communicate between the main function and the thread that reads the SSH output.
 - A timer (`timeout`) ensures the script doesn't hang indefinitely waiting for a prompt.
 
 ---
+
+## More Usage Examples
+- Commands are comma separated. Repeated comma's represent blank carriage returns, which can be useful in making sure you hit your expected prompt count instead of waiting for timeout
+
+#### 1. Cisco Router
+```markdown
+- **Device**: Cisco Router
+- **Command**: show version
+- **Usage**:
+  ```
+  pysshpass -h "192.168.1.1" -u "admin" -p "password" -c "terminal length 0,show version" --invoke-shell --prompt "#" --prompt-count 3 -t 10
+  ```
+#### 2. Aruba Switch
+```markdown
+- **Device**: Aruba Switch
+- **Command**: show interfaces brief
+- **Usage**:
+  ```
+  pysshpass -h "192.168.1.2" -u "admin" -p "password" -c "no paging,show interfaces brief" --invoke-shell --prompt ">" --prompt-count 2 -t 10
+  ```
+  
+#### 3. Palo Alto Firewall
+```markdown
+- **Device**: Palo Alto Firewall
+- **Command**: show system info
+- **Usage**:
+  ```
+  pysshpass -h "192.168.1.3" -u "admin" -p "password" -c "set cli pager off,show system info,," --invoke-shell --prompt ">" --prompt-count 2 -t 10
+  ```
+
+### General Tips
+- Adjust the `--prompt-count` and `--timeout` parameters based on the expected number of prompts and network responsiveness.
+- Ensure that IP addresses, usernames, and passwords are correctly configured for your specific setup.
+- Adjust "," for carriage returns and prompt count as needed
+
+---
```

### Comparing `pysshpass-0.1.0/PySSHPass/pysshpass.py` & `pysshpass-0.1.1/PySSHPass/pysshpass.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # CLI configuration using click
 @click.command()
 @click.option('--host', '-h', required=True, help='SSH Host (ip:port)')
 @click.option('--user', '-u', required=True, help='SSH Username')
 @click.option('--password', '-p', required=True, help='SSH Password')
 @click.option('--cmds', '-c', default='', help='Commands to run, separated by comma')
-@click.option('--invoke-shell', is_flag=True, help='Invoke shell before running the command [default=True]')
+@click.option('--invoke-shell', is_flag=True, help='Invoke shell before running the command [default=False]')
 @click.option('--prompt', default='', help='Prompt to look for before breaking the shell')
 @click.option('--prompt-count', default=1, help='Number of prompts to look for before breaking the shell')
 @click.option('--timeout', '-t', default=5, help='Command timeout duration in seconds')
 @click.option('--auto-add-policy', is_flag=True, default=True, help='Automatically add the host key [default=True]')
 @click.option('--look-for-keys', is_flag=True, default=False, help='Look for local SSH key [default=False]')
 @click.option('--inter-command-time', '-i', default=1, help='Inter-command time in seconds [default is 1 second]')
 def ssh_client(host, user, password, cmds, invoke_shell, prompt, prompt_count, timeout, auto_add_policy, look_for_keys, inter_command_time):
```

### Comparing `pysshpass-0.1.0/pysshpass.egg-info/PKG-INFO` & `pysshpass-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pysshpass
-Version: 0.1.0
-Summary: Python-based SSH client designed to offer a multiplatform alternative to `sshpass`.
+Version: 0.1.1
+Summary: Python-based SSH client designed to offer a multiplatform alternative to Netmiko or `sshpass`.
 Home-page: https://github.com/scottpeterman/pysshpass
 Author: Scott Peterman
 Author-email: scottpeterman@gmail.com
 License: GPLv3
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: paramiko>=3.3.1
-Requires-Dist: click>=8.1.7
+License-File: LICENSE
 
 ## pysshpass: A Multiplatform SSH Automation Utility
 
 ### Overview
 
 `pysshpass` is a Python-based SSH client designed to offer a multiplatform alternative to `sshpass`. This utility aims to address two core challenges:
 
@@ -64,29 +64,41 @@
 - Working with multi-modal command-line interfaces
 - Gathering information during network audits, especially for devices not well-supported by existing automation libraries
 
 ---
 ### CLI Usage
 
 ```commandline
->python pysshpass.py --help
-Usage: pysshpass.py [OPTIONS]
+pysshpass --help
+Usage: pysshpass [OPTIONS]
 
-Options:
-  -h, --host TEXT         SSH Host (ip:port)  [required]
-  -u, --user TEXT         SSH Username  [required]
-  -p, --password TEXT     SSH Password  [required]
-  -c, --cmds TEXT         Commands to run, separated by comma
-  --invoke-shell          Invoke shell before running the command
-  --prompt TEXT           Prompt to look for before breaking the shell     
-  --prompt-count INTEGER  Number of prompts to look for before breaking the
-                          shell
-  -t, --timeout INTEGER   Command timeout duration in seconds
-  --help                  Show this message and exit.
+  SSH Client for running remote commands.
+
+  Sample Usage: pysshpass -h "172.16.1.101" -u "cisco" -p "cisco" -c "term len
+  0,show users,show run,show cdp neigh,show int desc" --invoke-shell --prompt
+  "#" --prompt-count 4 -t 15
 
+Options:
+  -h, --host TEXT                 SSH Host (ip:port)  [required]
+  -u, --user TEXT                 SSH Username  [required]
+  -p, --password TEXT             SSH Password  [required]
+  -c, --cmds TEXT                 Commands to run, separated by comma
+  --invoke-shell                  Invoke shell before running the command
+                                  [default=True]
+  --prompt TEXT                   Prompt to look for before breaking the shell
+  --prompt-count INTEGER          Number of prompts to look for before
+                                  breaking the shell
+  -t, --timeout INTEGER           Command timeout duration in seconds
+  --auto-add-policy               Automatically add the host key
+                                  [default=True]
+  --look-for-keys                 Look for local SSH key [default=False]
+  -i, --inter-command-time INTEGER
+                                  Inter-command time in seconds [default is 1
+                                  second]
+  --help                          Show this message and exit.
 
 
 ```
 ---
 ### Function `read_output`
 
 - This function reads the output of the SSH session in real-time and prints it to the standard output.
@@ -104,7 +116,44 @@
 
 ### User Prompt Management
 
 - The code uses a queue (`output_queue`) to communicate between the main function and the thread that reads the SSH output.
 - A timer (`timeout`) ensures the script doesn't hang indefinitely waiting for a prompt.
 
 ---
+
+## More Usage Examples
+- Commands are comma separated. Repeated comma's represent blank carriage returns, which can be useful in making sure you hit your expected prompt count instead of waiting for timeout
+
+#### 1. Cisco Router
+```markdown
+- **Device**: Cisco Router
+- **Command**: show version
+- **Usage**:
+  ```
+  pysshpass -h "192.168.1.1" -u "admin" -p "password" -c "terminal length 0,show version" --invoke-shell --prompt "#" --prompt-count 3 -t 10
+  ```
+#### 2. Aruba Switch
+```markdown
+- **Device**: Aruba Switch
+- **Command**: show interfaces brief
+- **Usage**:
+  ```
+  pysshpass -h "192.168.1.2" -u "admin" -p "password" -c "no paging,show interfaces brief" --invoke-shell --prompt ">" --prompt-count 2 -t 10
+  ```
+  
+#### 3. Palo Alto Firewall
+```markdown
+- **Device**: Palo Alto Firewall
+- **Command**: show system info
+- **Usage**:
+  ```
+  pysshpass -h "192.168.1.3" -u "admin" -p "password" -c "set cli pager off,show system info,," --invoke-shell --prompt ">" --prompt-count 2 -t 10
+  ```
+
+### General Tips
+- Adjust the `--prompt-count` and `--timeout` parameters based on the expected number of prompts and network responsiveness.
+- Ensure that IP addresses, usernames, and passwords are correctly configured for your specific setup.
+- Adjust "," for carriage returns and prompt count as needed
+
+---
+
```

### Comparing `pysshpass-0.1.0/setup.py` & `pysshpass-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pysshpass',
-    version='0.1.0',
-    description='Python-based SSH client designed to offer a multiplatform alternative to `sshpass`.',
+    version='0.1.1',
+    description='Python-based SSH client designed to offer a multiplatform alternative to Netmiko or `sshpass`.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Scott Peterman',
     author_email='scottpeterman@gmail.com',
     url='https://github.com/scottpeterman/pysshpass',
     packages=find_packages(),
     include_package_data=True,
```

