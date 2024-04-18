# Comparing `tmp/telstracalltocsv-2.0.tar.gz` & `tmp/telstracalltocsv-2.0.1.tar.gz`

## Comparing `telstracalltocsv-2.0.tar` & `telstracalltocsv-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/INSTRUCTIONS.md
--rw-r--r--   0        0        0    23150 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/accesstoken_field5.png
--rw-r--r--   0        0        0    42532 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/accountuuid_field6.png
--rw-r--r--   0        0        0    15055 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/address_field1.png
--rw-r--r--   0        0        0    40900 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/contextmenu_field2.png
--rw-r--r--   0        0        0    46573 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/entry_field4.png
--rw-r--r--   0        0        0    59221 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/filter_field3.png
--rw-r--r--   0        0        0    62981 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/fpr_field6.png
--rw-r--r--   0        0        0    38312 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/login_field1.png
--rw-r--r--   0        0        0    66024 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/network_field3.png
--rw-r--r--   0        0        0    19568 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/password_field4.png
--rw-r--r--   0        0        0    40748 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/telstracall.png
--rw-r--r--   0        0        0    72180 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/assets/telstracall.svg
--rwxr-xr-x   0        0        0    16516 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/src/telstracalltocsv/__main__.py
--rw-r--r--   0        0        0    34916 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/COPYING.md
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/pyproject.toml
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 telstracalltocsv-2.0/PKG-INFO
+-rw-r--r--   0        0        0     7266 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/INSTRUCTIONS.md
+-rw-r--r--   0        0        0    23150 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/accesstoken_field5.png
+-rw-r--r--   0        0        0    42532 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/accountuuid_field6.png
+-rw-r--r--   0        0        0    15055 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/address_field1.png
+-rw-r--r--   0        0        0    40900 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/contextmenu_field2.png
+-rw-r--r--   0        0        0    46573 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/entry_field4.png
+-rw-r--r--   0        0        0    59221 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/filter_field3.png
+-rw-r--r--   0        0        0    62981 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/fpr_field6.png
+-rw-r--r--   0        0        0    38312 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/login_field1.png
+-rw-r--r--   0        0        0    66024 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/network_field3.png
+-rw-r--r--   0        0        0    19568 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/password_field4.png
+-rw-r--r--   0        0        0    40748 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/telstracall.png
+-rw-r--r--   0        0        0    72180 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/assets/telstracall.svg
+-rwxr-xr-x   0        0        0    14909 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/src/telstracalltocsv/__main__.py
+-rw-r--r--   0        0        0    34916 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/COPYING.md
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/README.md
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 telstracalltocsv-2.0.1/PKG-INFO
```

### Comparing `telstracalltocsv-2.0/INSTRUCTIONS.md` & `telstracalltocsv-2.0.1/INSTRUCTIONS.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 ## Tutorial
 
 This is a beginners' guide which assumes basic knowledge of computers. If you need help, please open a Discussion and tag it appropriately.
 
 **Estimated time: 15 minutes**
 
 ### Step 1: Getting your Key
-(Relevant for Firefox, Safari with Developer Mode enabled and Google Chrome/Chromium. Most other browsers support this method in some way or another, but they are not consistent with this documentation. Screenshots are from Firefox.)
+(Relevant for Firefox, Safari with Developer Mode enabled and Google Chrome/Chromium. Most other browsers support this method in some way or another, but they are not consistent with this documentation. Screenshots are from Firefox. **Important: If you are on Android, you can download Kiwi Browser from the Play Store which has the necessary developer tools to follow this tutorial.**)
 
 ![](assets/address_field1.png)
+
+
 ![](assets/login_field1.png)
 ___
 Go to [https://myservices.telstra.com.au](https://myservices.telstra.com.au).
 
-Enter your e-mail address, then press `Continue.`
+Enter your e-mail address, then press `Continue`.
 ___
 ___
 ![](assets/contextmenu_field2.png)
 ___
 Right-click anywhere on the following page, and click `Inspect` or `Inspect Element`, depending on your browser. The same can also be accomplished using `Ctrl/Cmd-Shift-I` in Firefox, or the F12 key in most browsers.
 ___
 ___
 ![](assets/network_field3.png)
 ![](assets/filter_field3.png)
 ___
 Find and click `Network` in the sidebar that opened.
 
-In the `Filter URLs` box, type `token.oauth2.`
+In the `Filter URLs` box, type `token.oauth2`.
 ___
 ___
 ![](assets/password_field4.png)
 ![](assets/entry_field4.png)
 
 Enter your password and press `Sign in`.
 
@@ -60,18 +62,19 @@
 **Required Reading**
 
 Depending on your operating system, you need to open one of the following applications:
 
 - GNU/Linux: The terminal emulator you have installed, such as Konsole or GNOME Terminal
 - Windows: Command Prompt or PowerShell
 - macOS: Terminal, or another terminal emulator you have installed such as iTerm2.
+- Android: Get [F-Droid](f-droid.org), an app store for open-source applications. From F-Droid, download Termux and use that to enter the commands from this tutorial. Do not download Termux from the Play Store.
 
 All of these applications will give you a text prompt that looks something like this:
 
-GNU/Linux or macOS:
+GNU/Linux, macOS or Android:
 ```sh
 user@computer ~ $
 ```
 
 Windows:
 ```
 C:\>
@@ -81,15 +84,15 @@
 
 **Installing**
 
 We need to download and install TelstraCallToCSV. We can do this using Python's `pip` package manager, which allows us to easily install TelstraCallToCSV and its dependencies in a single command from a central software repository for usage with Python.
 
 Run the following command to download and install TelstraCallToCSV from PyPi, the Python Package Index:
 
-GNU/Linux or macOS:
+GNU/Linux, macOS or Android:
 ```sh
 python3 -m pip install telstracalltocsv
 ```
 
 Windows:
 ```
 py -m pip install telstracalltocsv
@@ -97,15 +100,15 @@
 
 This command will output some text as it downloads and installs TelstraCallToCSV and its dependencies, but no interaction is required.
 
 **Configuring**
 
 TelstraCallToCSV has a built in configuration file which is not set up by default. Before running TelstraCallToCSV, you must set this up:
 
-GNU/Linux or macOS:
+GNU/Linux, macOS or Android:
 ```sh
 python3 -m telstracalltocsv --configure
 ```
 
 Windows:
 ```
 py -m telstracalltocsv --configure
@@ -114,15 +117,15 @@
 You will be prompted for your Account UUID and your Phone Number. Type or copy in the information, then press Enter.
 
 
 **Running**
 
 Finally, run TelstraCallToCSV, substituting `<key>` with your key gathered from Step 1.
 
-GNU/Linux or macOS:
+GNU/Linux, macOS or Android:
 ```sh
 python3 -m telstracalltocsv <key>
 ```
 
 Windows:
 ```
 py -m telstracalltocsv <key>
@@ -170,31 +173,28 @@
 positional arguments:
   key                   My Telstra session key
 
 options:
   -h, --help            show this help message and exit
   -c, --copying         show the license information
   -v, --version         show the version information
-  -C, --clean           clean all CSV files in the current directory- use with caution!
   --configure           write/create the configuration file
   -P PHONE, --phone PHONE
                         override the default account phone number in the config
   -M MONTHS, --months MONTHS
                         specify how many months back to download (default: 6, the max)
 
 TelstraCallToCSV Copyright (c) 2023 capta1nt0ad. This program comes with ABSOLUTELY NO WARRANTY; for details type `telstracall --copying`. This is free software, and you are welcome to redistribute it under the conditions of the
 GNU General Public License v3.
 ```
 
 Most notably:
 
 `--configure` allows you to reconfigure your Account UUID and Phone Number. (For advanced users: the configuration file is in JSON and is located in `~/.telstracall`.)
 
-`--clean` will delete all the CSV files in the current directory. You should make sure there are no CSV files in the current directory before running TelstraCallToCSV, because if it fails, this will be automatically run.
-
 `-P` or `--phone` allows you to specify a phone number to override the one in the configuration. Note that you still need to have a phone number in the configuration even with this option.
 
 `-M` or `--months` allows you to download a specific number of months, rather than the default maximum of 6. (Telstra does not allow you to request back more than 6 months of data, and there is no way to work around this.)
 
 ___
 ___
```

### Comparing `telstracalltocsv-2.0/assets/accesstoken_field5.png` & `telstracalltocsv-2.0.1/assets/accesstoken_field5.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/accountuuid_field6.png` & `telstracalltocsv-2.0.1/assets/accountuuid_field6.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/address_field1.png` & `telstracalltocsv-2.0.1/assets/address_field1.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/contextmenu_field2.png` & `telstracalltocsv-2.0.1/assets/contextmenu_field2.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/entry_field4.png` & `telstracalltocsv-2.0.1/assets/entry_field4.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/filter_field3.png` & `telstracalltocsv-2.0.1/assets/filter_field3.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/fpr_field6.png` & `telstracalltocsv-2.0.1/assets/fpr_field6.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/login_field1.png` & `telstracalltocsv-2.0.1/assets/login_field1.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/network_field3.png` & `telstracalltocsv-2.0.1/assets/network_field3.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/password_field4.png` & `telstracalltocsv-2.0.1/assets/password_field4.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/telstracall.png` & `telstracalltocsv-2.0.1/assets/telstracall.png`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/assets/telstracall.svg` & `telstracalltocsv-2.0.1/assets/telstracall.svg`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/src/telstracalltocsv/__main__.py` & `telstracalltocsv-2.0.1/src/telstracalltocsv/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
 
-import glob
 import os
 import json
 import sys
 
 from colorama import Fore, Style
 
 
@@ -34,21 +33,14 @@
     )
 
     parser.add_argument(
         "-v", "--version", help="show the version information", action="store_true"
     )
 
     parser.add_argument(
-        "-C",
-        "--clean",
-        help="clean all CSV files in the current directory- use with caution!",
-        action="store_true",
-    )
-
-    parser.add_argument(
         "--configure", help="write/create the configuration file", action="store_true"
     )
 
     parser.add_argument(
         "-P", "--phone", help="override the default account phone number in the config"
     )
 
@@ -74,28 +66,18 @@
     if args.copying:
         print("TelstraCallToCSV is licensed under the GNU General Public License version 3 (or later).")
         print("See https://www.gnu.org/licenses/gpl-3.0-standalone.html for more information.")
 
     if args.version:
         print("TelstraCallToCSV version 2.0.0")
 
-    if args.clean:
-        if glob.glob("*.csv") != []:
-            print(Fore.BLUE + ":: " + Fore.RESET + "Cleaning up...")
-            for files in glob.glob("*.csv"):
-                os.remove(files)
-            print(Fore.GREEN + ":: " + Fore.RESET + "Finished all jobs.")
-
-        else:
-            print(Fore.BLUE + ":: " + Fore.RESET + "Nothing to clean up.")
-
     if args.configure:
         configurator()
 
-    if args.copying or args.version or args.clean:
+    if args.copying or args.version:
         sys.exit(0)
 
     # Config file
 
     if not os.path.isfile(os.path.join(os.path.expanduser("~"), ".telstracall")):
         print(
             Fore.RED
@@ -224,18 +206,14 @@
             print(
                 Fore.YELLOW
                 + "         HINT: Log in again and double-check your key."
                 + Fore.RESET
             )
 
             print()
-
-            print(Fore.RED + ":: " + Fore.RESET + "Cleaning up...")
-            for files in glob.glob("*.csv"):
-                os.remove(files)
             print(Fore.RED + ":: " + Fore.RESET + "Finished all jobs.")
             sys.exit(76)
 
         if response.status_code == 403:
             print(
                 Fore.RED
                 + "The remote host returned an HTTP error "
@@ -246,18 +224,14 @@
             print(
                 Fore.YELLOW
                 + "         HINT: Check the configuration (--configure)."
                 + Fore.RESET
             )
 
             print()
-
-            print(Fore.RED + ":: " + Fore.RESET + "Cleaning up...")
-            for files in glob.glob("*.csv"):
-                os.remove(files)
             print(Fore.RED + ":: " + Fore.RESET + "Finished all jobs.")
             sys.exit(76)
 
         elif response.status_code != 200:
             print(
                 Fore.RED
                 + "The remote host returned an HTTP error "
@@ -271,18 +245,14 @@
                 + "         HINT: We may be being rate limited.\n"
                 + "         HINT: Please run the program again.\n"
                 + "         HINT: Otherwise, please file a bug report."
                 + Fore.RESET
             )
 
             print()
-
-            print(Fore.RED + ":: " + Fore.RESET + "Cleaning up...")
-            for files in glob.glob("*.csv"):
-                os.remove(files)
             print(Fore.RED + ":: " + Fore.RESET + "Finished all jobs.")
             sys.exit(76)
 
         print("Done.")
 
         filename = str(start_date) + ".csv"
 
@@ -388,18 +358,14 @@
                     )
                     print(
                         Fore.YELLOW + "         HINT: Log in again and "
                         "double-check your key." + Fore.RESET
                     )
 
                     print()
-
-                    print(Fore.RED + ":: " + Fore.RESET + "Cleaning up...")
-                    for files in glob.glob("*.csv"):
-                        os.remove(files)
                     print(Fore.RED + ":: " + Fore.RESET + "Finished all jobs.")
                     sys.exit(76)
 
                 if response.status_code == 403:
                     print(
                         Fore.RED
                         + "The remote host returned an HTTP error "
@@ -410,18 +376,14 @@
                     print(
                         Fore.YELLOW
                         + "         HINT: Check the configuration (--configure)."
                         + Fore.RESET
                     )
 
                     print()
-
-                    print(Fore.RED + ":: " + Fore.RESET + "Cleaning up...")
-                    for files in glob.glob("*.csv"):
-                        os.remove(files)
                     print(Fore.RED + ":: " + Fore.RESET + "Finished all jobs.")
                     sys.exit(76)
 
                 elif response.status_code != 200:
                     print(
                         Fore.RED
                         + "The remote host returned an HTTP error "
@@ -435,18 +397,14 @@
                         + "         HINT: We may be being rate limited.\n"
                         + "         HINT: Please run the program again.\n"
                         + "         HINT: Otherwise, please file a bug report."
                         + Fore.RESET
                     )
 
                     print()
-
-                    print(Fore.RED + ":: " + Fore.RESET + "Cleaning up...")
-                    for files in glob.glob("*.csv"):
-                        os.remove(files)
                     print(Fore.RED + ":: " + Fore.RESET + "Finished all jobs.")
                     sys.exit(76)
 
                 jparser = json.loads(response.text)
 
                 day_no = 0
 
@@ -513,11 +471,9 @@
 
 if __name__ == "__main__":
     try:
         main()
         print(Fore.GREEN + "\n:: " + Fore.RESET + "Finished all jobs.")
 
     except KeyboardInterrupt:
-        print(Fore.YELLOW + "\n\n:: " + Fore.RESET + "Aborted. Cleaning up...")
-        for files in glob.glob("*.csv"):
-            os.remove(files)
+        print(Fore.YELLOW + "\n\n:: " + Fore.RESET + "Aborted.")
         print(Fore.GREEN + ":: " + Fore.RESET + "Finished all jobs.")
```

### Comparing `telstracalltocsv-2.0/COPYING.md` & `telstracalltocsv-2.0.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `telstracalltocsv-2.0/README.md` & `telstracalltocsv-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 <h3 align="center"><a href="https://github.com/Capta1nT0ad/TelstraCallToCSV/blob/master/INSTRUCTIONS.md">Tutorial</a></h4>
 
 <p align="center">
 <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/badge/License-GPL%20v3-blue.svg"></a>
 <a href="https://en.wikipedia.org/wiki/Free_and_open-source_software"><img src="https://img.shields.io/badge/FOSS-100%25-green.svg?style=flat"></a>
 </p>
 
-TelstraCallToCSV is a Free and Open Source program for GNU/Linux, Windows and macOS that provides an easy command-line interface to download and export Telstra prepaid call histories to CSV files by utilising the same API that the My Telstra web interface uses to get information and our very own parser to save it to a CSV file.
+TelstraCallToCSV is a Free and Open Source program for GNU/Linux, Windows, macOS and Android that provides an easy command-line interface to download and export Telstra prepaid call histories to CSV files by utilising the same API that the My Telstra web interface uses to get information and our very own parser to save it to a CSV file.
 
 ## FAQ
 ### Q: Why does this exist?
 
-A: A few years ago, Telstra upgraded (really?) their web interface and removed the ability to download call histories as CSV files for prepaid plans. I saw that many others online (including myself) had expressed their frustration with this change (on https://whirlpool.net and other sites), and after taking quick look at the JSON format for call history, it became clear that it would be trivial to build a utility like this to export the information efficiently to CSV files.
+A: A few years ago, Telstra upgraded (really?) their web interface and removed the ability to download call histories as CSV files for prepaid plans. I saw that many others online (including myself) had expressed their frustration with this change (on https://whirlpool.net and other sites), and after taking a quick look at the JSON format for call history, it became clear that it would be trivial to build a utility like this to export the information efficiently to CSV files.
 
 ### Q: Are you stealing my login credentials?
 
-A: The only request the device makes is to Telstra's own server to download the call history content. Other than that, no data ever leaves your device and *most importantly*, is never sent to a third-party server like mine.
+A: The only request the device makes is to Telstra's own server to download the call history content. Other than that, no data ever leaves your device and, *most importantly*, is never sent to a third-party server like mine.
 
 This is the beauty of FOSS software: you yourself can review the code extremely easily and personally vet it. This program only defines two different HTTP requests and they are both to Telstra's API, where information like your Account UUID and Access Token are securely sent over HTTPS.
 
 ### Q: Is this legal / against Telstra's legal policies?
 
 A: No.
 
-I have attempted to look over all of Telstra's policies that would be relevant to this project and have found that the only usage of their web services that they specifically disallow is defined as usage that would distrupt the experience of other users.
+I have attempted to look over all of Telstra's policies that would be relevant to this project and have found that the only usage of their web services that they specifically disallow is defined as usage that would disrupt the experience of other users.
 
 What this program does is effectively indistinguishable from a normal My Testra user's activity on the Call History dashboard, so there is no distruption to Telstra's service from this program and especially no risk of your My Telstra account being denied access to their services.
 
 ### Q: What is the 'legacy' branch?
 
 A: TelstraCallToCSV actually originated two years ago as a simple parser for the call history format of My Telstra. Recently, it has evolved into a '2.0' version which allows you to automatically fetch six months back of call history without having to manually feed information in and copy it out. The 'legacy' branch provides this old version of TelstraCallToCSV in case you want to feed in your own JSON file.
 
@@ -52,15 +52,14 @@
 positional arguments:
   key                   My Telstra session key
 
 options:
   -h, --help            show this help message and exit
   -c, --copying         show the license information
   -v, --version         show the version information
-  -C, --clean           clean all CSV files in the current directory- use with caution!
   --configure           write/create the configuration file
   -P PHONE, --phone PHONE
                         override the default account phone number in the config
   -M MONTHS, --months MONTHS
                         specify how many months back to download (default: 6, the max)
 
 TelstraCallToCSV Copyright (c) 2023 capta1nt0ad. This program comes with ABSOLUTELY NO WARRANTY; for details type `telstracall --copying`. This is free software, and you are welcome to redistribute it under the conditions of the
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_lg3cegfq_/tmpqvwb0xt2_TarContainer/0/15.md", line 10, column 122: Levels of opening and closing headings don't match*

```diff
@@ -1,52 +1,52 @@
                            [assets/telstracall.png]
                         ************ TTeellssttrraaCCaallllTTooCCSSVV ************
      ********** ccoonnvveerrttss yyoouurr TTeellssttrraa pprreeppaaiidd ccaallll hhiissttoorryy ttoo CCSSVV ffiilleess.. **********
                               ******** _TT_uu_tt_oo_rr_ii_aa_ll ********
        _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_G_P_L_%_2_0_v_3_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
             _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_F_O_S_S_-_1_0_0_%_2_5_-_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]
-TelstraCallToCSV is a Free and Open Source program for GNU/Linux, Windows and
-macOS that provides an easy command-line interface to download and export
-Telstra prepaid call histories to CSV files by utilising the same API that the
-My Telstra web interface uses to get information and our very own parser to
-save it to a CSV file. ## FAQ ### Q: Why does this exist? A: A few years ago,
-Telstra upgraded (really?) their web interface and removed the ability to
-download call histories as CSV files for prepaid plans. I saw that many others
-online (including myself) had expressed their frustration with this change (on
-https://whirlpool.net and other sites), and after taking quick look at the JSON
-format for call history, it became clear that it would be trivial to build a
-utility like this to export the information efficiently to CSV files. ### Q:
-Are you stealing my login credentials? A: The only request the device makes is
-to Telstra's own server to download the call history content. Other than that,
-no data ever leaves your device and *most importantly*, is never sent to a
-third-party server like mine. This is the beauty of FOSS software: you yourself
-can review the code extremely easily and personally vet it. This program only
-defines two different HTTP requests and they are both to Telstra's API, where
-information like your Account UUID and Access Token are securely sent over
-HTTPS. ### Q: Is this legal / against Telstra's legal policies? A: No. I have
-attempted to look over all of Telstra's policies that would be relevant to this
-project and have found that the only usage of their web services that they
-specifically disallow is defined as usage that would distrupt the experience of
-other users. What this program does is effectively indistinguishable from a
-normal My Testra user's activity on the Call History dashboard, so there is no
-distruption to Telstra's service from this program and especially no risk of
-your My Telstra account being denied access to their services. ### Q: What is
-the 'legacy' branch? A: TelstraCallToCSV actually originated two years ago as a
-simple parser for the call history format of My Telstra. Recently, it has
-evolved into a '2.0' version which allows you to automatically fetch six months
-back of call history without having to manually feed information in and copy it
-out. The 'legacy' branch provides this old version of TelstraCallToCSV in case
-you want to feed in your own JSON file. ## Usage **For a detailed guide to
-using TelstraCallToCSV, please see the _T_u_t_o_r_i_a_l.** Otherwise, the `--help`
-output from TelstraCallToCSV is below. ``` usage: TelstraCallToCSV [-h] [-c] [-
-v] [-C] [--configure] [-P PHONE] [-M MONTHS] [key] A simple Python program to
-export Telstra call histories to CSV files. positional arguments: key My
-Telstra session key options: -h, --help show this help message and exit -c, --
-copying show the license information -v, --version show the version information
--C, --clean clean all CSV files in the current directory- use with caution! --
+TelstraCallToCSV is a Free and Open Source program for GNU/Linux, Windows,
+macOS and Android that provides an easy command-line interface to download and
+export Telstra prepaid call histories to CSV files by utilising the same API
+that the My Telstra web interface uses to get information and our very own
+parser to save it to a CSV file. ## FAQ ### Q: Why does this exist? A: A few
+years ago, Telstra upgraded (really?) their web interface and removed the
+ability to download call histories as CSV files for prepaid plans. I saw that
+many others online (including myself) had expressed their frustration with this
+change (on https://whirlpool.net and other sites), and after taking a quick
+look at the JSON format for call history, it became clear that it would be
+trivial to build a utility like this to export the information efficiently to
+CSV files. ### Q: Are you stealing my login credentials? A: The only request
+the device makes is to Telstra's own server to download the call history
+content. Other than that, no data ever leaves your device and, *most
+importantly*, is never sent to a third-party server like mine. This is the
+beauty of FOSS software: you yourself can review the code extremely easily and
+personally vet it. This program only defines two different HTTP requests and
+they are both to Telstra's API, where information like your Account UUID and
+Access Token are securely sent over HTTPS. ### Q: Is this legal / against
+Telstra's legal policies? A: No. I have attempted to look over all of Telstra's
+policies that would be relevant to this project and have found that the only
+usage of their web services that they specifically disallow is defined as usage
+that would disrupt the experience of other users. What this program does is
+effectively indistinguishable from a normal My Testra user's activity on the
+Call History dashboard, so there is no distruption to Telstra's service from
+this program and especially no risk of your My Telstra account being denied
+access to their services. ### Q: What is the 'legacy' branch? A:
+TelstraCallToCSV actually originated two years ago as a simple parser for the
+call history format of My Telstra. Recently, it has evolved into a '2.0'
+version which allows you to automatically fetch six months back of call history
+without having to manually feed information in and copy it out. The 'legacy'
+branch provides this old version of TelstraCallToCSV in case you want to feed
+in your own JSON file. ## Usage **For a detailed guide to using
+TelstraCallToCSV, please see the _T_u_t_o_r_i_a_l.** Otherwise, the `--help` output
+from TelstraCallToCSV is below. ``` usage: TelstraCallToCSV [-h] [-c] [-v] [-C]
+[--configure] [-P PHONE] [-M MONTHS] [key] A simple Python program to export
+Telstra call histories to CSV files. positional arguments: key My Telstra
+session key options: -h, --help show this help message and exit -c, --copying
+show the license information -v, --version show the version information --
 configure write/create the configuration file -P PHONE, --phone PHONE override
 the default account phone number in the config -M MONTHS, --months MONTHS
 specify how many months back to download (default: 6, the max) TelstraCallToCSV
 Copyright (c) 2023 capta1nt0ad. This program comes with ABSOLUTELY NO WARRANTY;
 for details type `telstracall --copying`. This is free software, and you are
 welcome to redistribute it under the conditions of the GNU General Public
 License v3. ``` ## License ``` TelstraCallToCSV converts your Telstra prepaid
```

### Comparing `telstracalltocsv-2.0/pyproject.toml` & `telstracalltocsv-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/telstracalltocsv"]
 
 [project]
 name = "telstracalltocsv"
-version = "2.0"
+version = "2.0.1"
 authors = [
   { name="Capta1nT0ad" },
 ]
 description = "TelstraCallToCSV exports Telstra prepaid call logs to CSV files."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `telstracalltocsv-2.0/PKG-INFO` & `telstracalltocsv-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: telstracalltocsv
-Version: 2.0
+Version: 2.0.1
 Summary: TelstraCallToCSV exports Telstra prepaid call logs to CSV files.
 Project-URL: Homepage, https://github.com/Capta1nT0ad/TelstraCallToCSV
 Project-URL: Issues, https://github.com/Capta1nT0ad/TelstraCallToCSV/issues
 Author: Capta1nT0ad
 License-File: COPYING.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -27,32 +27,32 @@
 <h3 align="center"><a href="https://github.com/Capta1nT0ad/TelstraCallToCSV/blob/master/INSTRUCTIONS.md">Tutorial</a></h4>
 
 <p align="center">
 <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/badge/License-GPL%20v3-blue.svg"></a>
 <a href="https://en.wikipedia.org/wiki/Free_and_open-source_software"><img src="https://img.shields.io/badge/FOSS-100%25-green.svg?style=flat"></a>
 </p>
 
-TelstraCallToCSV is a Free and Open Source program for GNU/Linux, Windows and macOS that provides an easy command-line interface to download and export Telstra prepaid call histories to CSV files by utilising the same API that the My Telstra web interface uses to get information and our very own parser to save it to a CSV file.
+TelstraCallToCSV is a Free and Open Source program for GNU/Linux, Windows, macOS and Android that provides an easy command-line interface to download and export Telstra prepaid call histories to CSV files by utilising the same API that the My Telstra web interface uses to get information and our very own parser to save it to a CSV file.
 
 ## FAQ
 ### Q: Why does this exist?
 
-A: A few years ago, Telstra upgraded (really?) their web interface and removed the ability to download call histories as CSV files for prepaid plans. I saw that many others online (including myself) had expressed their frustration with this change (on https://whirlpool.net and other sites), and after taking quick look at the JSON format for call history, it became clear that it would be trivial to build a utility like this to export the information efficiently to CSV files.
+A: A few years ago, Telstra upgraded (really?) their web interface and removed the ability to download call histories as CSV files for prepaid plans. I saw that many others online (including myself) had expressed their frustration with this change (on https://whirlpool.net and other sites), and after taking a quick look at the JSON format for call history, it became clear that it would be trivial to build a utility like this to export the information efficiently to CSV files.
 
 ### Q: Are you stealing my login credentials?
 
-A: The only request the device makes is to Telstra's own server to download the call history content. Other than that, no data ever leaves your device and *most importantly*, is never sent to a third-party server like mine.
+A: The only request the device makes is to Telstra's own server to download the call history content. Other than that, no data ever leaves your device and, *most importantly*, is never sent to a third-party server like mine.
 
 This is the beauty of FOSS software: you yourself can review the code extremely easily and personally vet it. This program only defines two different HTTP requests and they are both to Telstra's API, where information like your Account UUID and Access Token are securely sent over HTTPS.
 
 ### Q: Is this legal / against Telstra's legal policies?
 
 A: No.
 
-I have attempted to look over all of Telstra's policies that would be relevant to this project and have found that the only usage of their web services that they specifically disallow is defined as usage that would distrupt the experience of other users.
+I have attempted to look over all of Telstra's policies that would be relevant to this project and have found that the only usage of their web services that they specifically disallow is defined as usage that would disrupt the experience of other users.
 
 What this program does is effectively indistinguishable from a normal My Testra user's activity on the Call History dashboard, so there is no distruption to Telstra's service from this program and especially no risk of your My Telstra account being denied access to their services.
 
 ### Q: What is the 'legacy' branch?
 
 A: TelstraCallToCSV actually originated two years ago as a simple parser for the call history format of My Telstra. Recently, it has evolved into a '2.0' version which allows you to automatically fetch six months back of call history without having to manually feed information in and copy it out. The 'legacy' branch provides this old version of TelstraCallToCSV in case you want to feed in your own JSON file.
 
@@ -69,15 +69,14 @@
 positional arguments:
   key                   My Telstra session key
 
 options:
   -h, --help            show this help message and exit
   -c, --copying         show the license information
   -v, --version         show the version information
-  -C, --clean           clean all CSV files in the current directory- use with caution!
   --configure           write/create the configuration file
   -P PHONE, --phone PHONE
                         override the default account phone number in the config
   -M MONTHS, --months MONTHS
                         specify how many months back to download (default: 6, the max)
 
 TelstraCallToCSV Copyright (c) 2023 capta1nt0ad. This program comes with ABSOLUTELY NO WARRANTY; for details type `telstracall --copying`. This is free software, and you are welcome to redistribute it under the conditions of the
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_lg3cegfq_/tmpqvwb0xt2_TarContainer/0/17", line 27, column 122: Levels of opening and closing headings don't match*

```diff
@@ -1,61 +1,61 @@
-Metadata-Version: 2.1 Name: telstracalltocsv Version: 2.0 Summary:
+Metadata-Version: 2.3 Name: telstracalltocsv Version: 2.0.1 Summary:
 TelstraCallToCSV exports Telstra prepaid call logs to CSV files. Project-URL:
 Homepage, https://github.com/Capta1nT0ad/TelstraCallToCSV Project-URL: Issues,
 https://github.com/Capta1nT0ad/TelstraCallToCSV/issues Author: Capta1nT0ad
 License-File: COPYING.md Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Requires-Python:
 >=3.8 Requires-Dist: colorama Requires-Dist: python-dateutil Requires-Dist:
 requests Description-Content-Type: text/markdown
                            [assets/telstracall.png]
                         ************ TTeellssttrraaCCaallllTTooCCSSVV ************
      ********** ccoonnvveerrttss yyoouurr TTeellssttrraa pprreeppaaiidd ccaallll hhiissttoorryy ttoo CCSSVV ffiilleess.. **********
                               ******** _TT_uu_tt_oo_rr_ii_aa_ll ********
        _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_G_P_L_%_2_0_v_3_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
             _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_F_O_S_S_-_1_0_0_%_2_5_-_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]
-TelstraCallToCSV is a Free and Open Source program for GNU/Linux, Windows and
-macOS that provides an easy command-line interface to download and export
-Telstra prepaid call histories to CSV files by utilising the same API that the
-My Telstra web interface uses to get information and our very own parser to
-save it to a CSV file. ## FAQ ### Q: Why does this exist? A: A few years ago,
-Telstra upgraded (really?) their web interface and removed the ability to
-download call histories as CSV files for prepaid plans. I saw that many others
-online (including myself) had expressed their frustration with this change (on
-https://whirlpool.net and other sites), and after taking quick look at the JSON
-format for call history, it became clear that it would be trivial to build a
-utility like this to export the information efficiently to CSV files. ### Q:
-Are you stealing my login credentials? A: The only request the device makes is
-to Telstra's own server to download the call history content. Other than that,
-no data ever leaves your device and *most importantly*, is never sent to a
-third-party server like mine. This is the beauty of FOSS software: you yourself
-can review the code extremely easily and personally vet it. This program only
-defines two different HTTP requests and they are both to Telstra's API, where
-information like your Account UUID and Access Token are securely sent over
-HTTPS. ### Q: Is this legal / against Telstra's legal policies? A: No. I have
-attempted to look over all of Telstra's policies that would be relevant to this
-project and have found that the only usage of their web services that they
-specifically disallow is defined as usage that would distrupt the experience of
-other users. What this program does is effectively indistinguishable from a
-normal My Testra user's activity on the Call History dashboard, so there is no
-distruption to Telstra's service from this program and especially no risk of
-your My Telstra account being denied access to their services. ### Q: What is
-the 'legacy' branch? A: TelstraCallToCSV actually originated two years ago as a
-simple parser for the call history format of My Telstra. Recently, it has
-evolved into a '2.0' version which allows you to automatically fetch six months
-back of call history without having to manually feed information in and copy it
-out. The 'legacy' branch provides this old version of TelstraCallToCSV in case
-you want to feed in your own JSON file. ## Usage **For a detailed guide to
-using TelstraCallToCSV, please see the _T_u_t_o_r_i_a_l.** Otherwise, the `--help`
-output from TelstraCallToCSV is below. ``` usage: TelstraCallToCSV [-h] [-c] [-
-v] [-C] [--configure] [-P PHONE] [-M MONTHS] [key] A simple Python program to
-export Telstra call histories to CSV files. positional arguments: key My
-Telstra session key options: -h, --help show this help message and exit -c, --
-copying show the license information -v, --version show the version information
--C, --clean clean all CSV files in the current directory- use with caution! --
+TelstraCallToCSV is a Free and Open Source program for GNU/Linux, Windows,
+macOS and Android that provides an easy command-line interface to download and
+export Telstra prepaid call histories to CSV files by utilising the same API
+that the My Telstra web interface uses to get information and our very own
+parser to save it to a CSV file. ## FAQ ### Q: Why does this exist? A: A few
+years ago, Telstra upgraded (really?) their web interface and removed the
+ability to download call histories as CSV files for prepaid plans. I saw that
+many others online (including myself) had expressed their frustration with this
+change (on https://whirlpool.net and other sites), and after taking a quick
+look at the JSON format for call history, it became clear that it would be
+trivial to build a utility like this to export the information efficiently to
+CSV files. ### Q: Are you stealing my login credentials? A: The only request
+the device makes is to Telstra's own server to download the call history
+content. Other than that, no data ever leaves your device and, *most
+importantly*, is never sent to a third-party server like mine. This is the
+beauty of FOSS software: you yourself can review the code extremely easily and
+personally vet it. This program only defines two different HTTP requests and
+they are both to Telstra's API, where information like your Account UUID and
+Access Token are securely sent over HTTPS. ### Q: Is this legal / against
+Telstra's legal policies? A: No. I have attempted to look over all of Telstra's
+policies that would be relevant to this project and have found that the only
+usage of their web services that they specifically disallow is defined as usage
+that would disrupt the experience of other users. What this program does is
+effectively indistinguishable from a normal My Testra user's activity on the
+Call History dashboard, so there is no distruption to Telstra's service from
+this program and especially no risk of your My Telstra account being denied
+access to their services. ### Q: What is the 'legacy' branch? A:
+TelstraCallToCSV actually originated two years ago as a simple parser for the
+call history format of My Telstra. Recently, it has evolved into a '2.0'
+version which allows you to automatically fetch six months back of call history
+without having to manually feed information in and copy it out. The 'legacy'
+branch provides this old version of TelstraCallToCSV in case you want to feed
+in your own JSON file. ## Usage **For a detailed guide to using
+TelstraCallToCSV, please see the _T_u_t_o_r_i_a_l.** Otherwise, the `--help` output
+from TelstraCallToCSV is below. ``` usage: TelstraCallToCSV [-h] [-c] [-v] [-C]
+[--configure] [-P PHONE] [-M MONTHS] [key] A simple Python program to export
+Telstra call histories to CSV files. positional arguments: key My Telstra
+session key options: -h, --help show this help message and exit -c, --copying
+show the license information -v, --version show the version information --
 configure write/create the configuration file -P PHONE, --phone PHONE override
 the default account phone number in the config -M MONTHS, --months MONTHS
 specify how many months back to download (default: 6, the max) TelstraCallToCSV
 Copyright (c) 2023 capta1nt0ad. This program comes with ABSOLUTELY NO WARRANTY;
 for details type `telstracall --copying`. This is free software, and you are
 welcome to redistribute it under the conditions of the GNU General Public
 License v3. ``` ## License ``` TelstraCallToCSV converts your Telstra prepaid
```

