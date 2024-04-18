# Comparing `tmp/displayrws-0.1.3.tar.gz` & `tmp/displayrws-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "displayrws-0.1.3.tar", last modified: Thu Apr 11 21:38:59 2024, max compression
+gzip compressed data, was "displayrws-0.1.4.tar", last modified: Tue Apr 16 15:21:24 2024, max compression
```

## Comparing `displayrws-0.1.3.tar` & `displayrws-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 21:38:59.245033 displayrws-0.1.3/
--rw-rw-rw-   0 runner    (1000) runner    (1000)    35141 2024-04-11 13:35:21.000000 displayrws-0.1.3/LICENSE
--rw-rw-rw-   0 runner    (1000) runner    (1000)       35 2024-04-11 13:35:21.000000 displayrws-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)     5428 2024-04-11 21:38:59.245033 displayrws-0.1.3/PKG-INFO
--rw-rw-rw-   0 runner    (1000) runner    (1000)     3777 2024-04-11 21:16:17.000000 displayrws-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 21:38:59.241034 displayrws-0.1.3/displayrws/
--rw-rw-rw-   0 runner    (1000) runner    (1000)      228 2024-04-11 21:16:17.000000 displayrws-0.1.3/displayrws/__init__.py
--rw-rw-rw-   0 runner    (1000) runner    (1000)        0 2024-04-11 21:37:33.000000 displayrws-0.1.3/displayrws/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 21:38:59.241034 displayrws-0.1.3/displayrws.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     5428 2024-04-11 21:38:59.000000 displayrws-0.1.3/displayrws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      325 2024-04-11 21:38:59.000000 displayrws-0.1.3/displayrws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 21:38:59.000000 displayrws-0.1.3/displayrws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-11 21:37:46.000000 displayrws-0.1.3/displayrws.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)      255 2024-04-11 21:38:59.000000 displayrws-0.1.3/displayrws.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-11 21:38:59.000000 displayrws-0.1.3/displayrws.egg-info/top_level.txt
--rw-rw-rw-   0 runner    (1000) runner    (1000)     2226 2024-04-11 20:07:20.000000 displayrws-0.1.3/pyproject.toml
--rw-rw-rw-   0 runner    (1000) runner    (1000)      213 2024-04-11 21:38:59.245033 displayrws-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-11 21:38:59.241034 displayrws-0.1.3/tests/
--rw-rw-rw-   0 runner    (1000) runner    (1000)      102 2024-04-11 14:48:05.000000 displayrws-0.1.3/tests/test_displayrws.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-16 15:21:24.067505 displayrws-0.1.4/
+-rw-rw-rw-   0 runner    (1000) runner    (1000)    35141 2024-04-16 14:44:49.000000 displayrws-0.1.4/LICENSE
+-rw-rw-rw-   0 runner    (1000) runner    (1000)       35 2024-04-16 14:44:49.000000 displayrws-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     5710 2024-04-16 15:21:24.067505 displayrws-0.1.4/PKG-INFO
+-rw-rw-rw-   0 runner    (1000) runner    (1000)     4059 2024-04-16 14:44:49.000000 displayrws-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-16 15:21:24.063506 displayrws-0.1.4/displayrws/
+-rw-rw-rw-   0 runner    (1000) runner    (1000)      228 2024-04-16 14:44:49.000000 displayrws-0.1.4/displayrws/__init__.py
+-rw-rw-rw-   0 runner    (1000) runner    (1000)        0 2024-04-16 15:19:58.000000 displayrws-0.1.4/displayrws/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-16 15:21:24.063506 displayrws-0.1.4/displayrws.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5710 2024-04-16 15:21:24.000000 displayrws-0.1.4/displayrws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      325 2024-04-16 15:21:24.000000 displayrws-0.1.4/displayrws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-16 15:21:24.000000 displayrws-0.1.4/displayrws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-16 15:20:11.000000 displayrws-0.1.4/displayrws.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)      255 2024-04-16 15:21:24.000000 displayrws-0.1.4/displayrws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-04-16 15:21:24.000000 displayrws-0.1.4/displayrws.egg-info/top_level.txt
+-rw-rw-rw-   0 runner    (1000) runner    (1000)     2226 2024-04-16 14:44:49.000000 displayrws-0.1.4/pyproject.toml
+-rw-rw-rw-   0 runner    (1000) runner    (1000)      213 2024-04-16 15:21:24.067505 displayrws-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-16 15:21:24.063506 displayrws-0.1.4/tests/
+-rw-rw-rw-   0 runner    (1000) runner    (1000)      102 2024-04-16 14:44:49.000000 displayrws-0.1.4/tests/test_displayrws.py
```

### Comparing `displayrws-0.1.3/LICENSE` & `displayrws-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `displayrws-0.1.3/PKG-INFO` & `displayrws-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: displayrws
-Version: 0.1.3
+Version: 0.1.4
 Summary: SPI Display and ESP32 project
 Author-email: RWS Datalab <datalab.codebase@rws.nl>
 Project-URL: homepage, https://gitlab.com/rwsdatalab/displayrws
 Project-URL: repository, https://gitlab.com/rwsdatalab/displayrws
 Project-URL: changelog, https://gitlab.com/rwsdatalab/displayrws/blob/main/CHANGELOG.rst
 Keywords: displayrws
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -42,30 +42,34 @@
 
 ##########
 displayrws
 ##########
 
 Dit project beschrijft hoe een 1,3 inch HD_IPS_TFT_LCD display van Joy-IT aangesloten kan worden op een ESP32.
 
+Benodigdheden:
 .. begin-inclusion-intro-marker-do-not-remove
 
 - ESP32 (type ESP-WROOM-32) bijv. van Joy-IT
 - kabeltjes
 - micro USB kabel
 - Display 240x240 pixel (SBC-LCD01)
 
 Verder is een computer met Python nodig.
 Toegang tot het USB device is noodzakelijk.
 
+############
+ Stappenplan
+############
 
-## Stappenplan
+Installeer Python
+===================
 
-. Installeer Python
-
-  ### Windows
+Windows
+~~~~~~~
 
   Klik op de Windows knop (Start).
 
   Type in:
 
   ```cmd```
 
@@ -77,24 +81,28 @@
 
   ```python get-pip.py```
 
   Wanneer Python nog niet geinstalleerd is, verschijnt er een Windows Store dialoog.
   In dit Windows Store dialoog, klik op Downloaden van Python.
 
 
-  ### Voor Linux:
+Voor Linux:
+~~~~~~~~~~~
 
   ```sudo apt install python3```
   ```sudo apt install python3-pip```
 
 
-. Installeer esphome:
+Installeer esphome:
+=====================
 
   ```pip install esphome```
+
   ```pip install pillow==10.2.0```
+
   ```pip install python-magic-bin``` (voor Windows)
 
   In Windows:
   wanneer deze melding te zien is:
 
   ```WARNING: The script esphome.exe is installed in C:\Users\<username>\AppData\Local\Packages\PythonSoftwareFoundation.Python..3.12_...\LocalCache...```
 
@@ -102,25 +110,27 @@
   ```set PATH="%PATH%;C:\your\path\here\"```
 
   Vervang C:\your\path\here\ door het path in de warning: C:\Users\<username>\AppData\Local\Packages\PythonSoftwareFoundation.Python....
 
   Sluit het Opdrachtprompt en start een nieuw Opdrachtprompt.
 
 
-. Zorg ervoor dat er genoeg rechten zijn om van het USB apparaat:
+Zorg ervoor dat er genoeg rechten zijn om van het USB apparaat:
+===============================================================
 
   Voor Linux:
 
   ```sudo usermod -a -G dialout [gebruikersnaam]```
 
   vervang: [gebruikersnaam] met jouw systeem gebruikersnaam.
 
   Restart jouw computer of log opnieuw in om deze rechten te effectueren.
 
-. Verbind met de kabeltjes van het ESP32 development board met het display:
+Verbind met de kabeltjes van het ESP32 development board met het display:
+=========================================================================
 
   SDA -> D13
 
   SCL -> D14
 
   DC -> D19
 
@@ -128,64 +138,68 @@
 
   RES -> D23
 
   GND -> GND (pin boven 3.3V)
 
   3V3 -> 3.3V (pin rechtsonder)
 
+
 .. image:: figs/pinouth.png
 
-. Verbind de USB kabel met het ESP32 board.
+Verbind de USB kabel met het ESP32 board.
+=========================================
 
 Het rode lampje moet branden.
 
-. In de USB devices controleer het USB ap
+In de USB devices controleer het USB apparaat
+=============================================
 
 In Linux:
   ```ls /dev/ttyU* -la```
 
 meestal staat er een nieuw USB device genaamd: ttyUSB01 of ttyUSB02 bij.
 
-. Voer uit:
+Voer uit:
+=========
 
   ```git clone https://gitlab.com/rwsdatalab/public/codebase/tools/displayrws.git```
+
   ````cd displayrws```
 
-. Voer uit:
+Voer uit:
+=========
 
   ```esphome run spi-display-image.yaml```
 
-Wanneer wordt gevraagd hoe te verbinden met het de ESP32 selecteer dan het USB apparaat bijv. /dev/USB01
-In Windows heet dit apparaat COM4.
+  Wanneer wordt gevraagd hoe te verbinden met het de ESP32 selecteer dan het USB apparaat bijv. /dev/USB01
+  In Windows heet dit apparaat COM4.
 
-. Nadat het flashen van de chip klaar is verschijnt er een blauwe vierkant met de tekst: RWS Datalab.
+  Nadat het flashen van de chip klaar is verschijnt er een blauwe vierkant met de tekst: RWS Datalab.
 
-. Maak bijv. een cirkel.
+  Maak bijv. een cirkel.
 
-Gebruik deze handleiding:
-https://esphome.io/components/display/index.html
+  Gebruik deze handleiding:
+  https://esphome.io/components/display/index.html
 
-## Handleiding ESP32
+#################
+Handleiding ESP32
+#################
 
 https://joy-it.net/files/files/Produkte/SBC-NodeMCU-ESP32/SBC-NodeMCU-ESP32-Manual-2021-06-29.pdf
 
 
 .. end-inclusion-intro-marker-do-not-remove
 
 
-Documentation
--------------
-
-Include a link to your project's full documentation here.
-
 
 .. begin-inclusion-license-marker-do-not-remove
 
+
 License
--------
+=======
 
 Copyright (c) 2024, Rijkswaterstaat
 
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `displayrws-0.1.3/README.rst` & `displayrws-0.1.4/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 ##########
 displayrws
 ##########
 
 Dit project beschrijft hoe een 1,3 inch HD_IPS_TFT_LCD display van Joy-IT aangesloten kan worden op een ESP32.
 
+Benodigdheden:
 .. begin-inclusion-intro-marker-do-not-remove
 
 - ESP32 (type ESP-WROOM-32) bijv. van Joy-IT
 - kabeltjes
 - micro USB kabel
 - Display 240x240 pixel (SBC-LCD01)
 
 Verder is een computer met Python nodig.
 Toegang tot het USB device is noodzakelijk.
 
+############
+ Stappenplan
+############
 
-## Stappenplan
+Installeer Python
+===================
 
-. Installeer Python
-
-  ### Windows
+Windows
+~~~~~~~
 
   Klik op de Windows knop (Start).
 
   Type in:
 
   ```cmd```
 
@@ -35,24 +39,28 @@
 
   ```python get-pip.py```
 
   Wanneer Python nog niet geinstalleerd is, verschijnt er een Windows Store dialoog.
   In dit Windows Store dialoog, klik op Downloaden van Python.
 
 
-  ### Voor Linux:
+Voor Linux:
+~~~~~~~~~~~
 
   ```sudo apt install python3```
   ```sudo apt install python3-pip```
 
 
-. Installeer esphome:
+Installeer esphome:
+=====================
 
   ```pip install esphome```
+
   ```pip install pillow==10.2.0```
+
   ```pip install python-magic-bin``` (voor Windows)
 
   In Windows:
   wanneer deze melding te zien is:
 
   ```WARNING: The script esphome.exe is installed in C:\Users\<username>\AppData\Local\Packages\PythonSoftwareFoundation.Python..3.12_...\LocalCache...```
 
@@ -60,25 +68,27 @@
   ```set PATH="%PATH%;C:\your\path\here\"```
 
   Vervang C:\your\path\here\ door het path in de warning: C:\Users\<username>\AppData\Local\Packages\PythonSoftwareFoundation.Python....
 
   Sluit het Opdrachtprompt en start een nieuw Opdrachtprompt.
 
 
-. Zorg ervoor dat er genoeg rechten zijn om van het USB apparaat:
+Zorg ervoor dat er genoeg rechten zijn om van het USB apparaat:
+===============================================================
 
   Voor Linux:
 
   ```sudo usermod -a -G dialout [gebruikersnaam]```
 
   vervang: [gebruikersnaam] met jouw systeem gebruikersnaam.
 
   Restart jouw computer of log opnieuw in om deze rechten te effectueren.
 
-. Verbind met de kabeltjes van het ESP32 development board met het display:
+Verbind met de kabeltjes van het ESP32 development board met het display:
+=========================================================================
 
   SDA -> D13
 
   SCL -> D14
 
   DC -> D19
 
@@ -86,64 +96,68 @@
 
   RES -> D23
 
   GND -> GND (pin boven 3.3V)
 
   3V3 -> 3.3V (pin rechtsonder)
 
+
 .. image:: figs/pinouth.png
 
-. Verbind de USB kabel met het ESP32 board.
+Verbind de USB kabel met het ESP32 board.
+=========================================
 
 Het rode lampje moet branden.
 
-. In de USB devices controleer het USB ap
+In de USB devices controleer het USB apparaat
+=============================================
 
 In Linux:
   ```ls /dev/ttyU* -la```
 
 meestal staat er een nieuw USB device genaamd: ttyUSB01 of ttyUSB02 bij.
 
-. Voer uit:
+Voer uit:
+=========
 
   ```git clone https://gitlab.com/rwsdatalab/public/codebase/tools/displayrws.git```
+
   ````cd displayrws```
 
-. Voer uit:
+Voer uit:
+=========
 
   ```esphome run spi-display-image.yaml```
 
-Wanneer wordt gevraagd hoe te verbinden met het de ESP32 selecteer dan het USB apparaat bijv. /dev/USB01
-In Windows heet dit apparaat COM4.
+  Wanneer wordt gevraagd hoe te verbinden met het de ESP32 selecteer dan het USB apparaat bijv. /dev/USB01
+  In Windows heet dit apparaat COM4.
 
-. Nadat het flashen van de chip klaar is verschijnt er een blauwe vierkant met de tekst: RWS Datalab.
+  Nadat het flashen van de chip klaar is verschijnt er een blauwe vierkant met de tekst: RWS Datalab.
 
-. Maak bijv. een cirkel.
+  Maak bijv. een cirkel.
 
-Gebruik deze handleiding:
-https://esphome.io/components/display/index.html
+  Gebruik deze handleiding:
+  https://esphome.io/components/display/index.html
 
-## Handleiding ESP32
+#################
+Handleiding ESP32
+#################
 
 https://joy-it.net/files/files/Produkte/SBC-NodeMCU-ESP32/SBC-NodeMCU-ESP32-Manual-2021-06-29.pdf
 
 
 .. end-inclusion-intro-marker-do-not-remove
 
 
-Documentation
--------------
-
-Include a link to your project's full documentation here.
-
 
 .. begin-inclusion-license-marker-do-not-remove
 
+
 License
--------
+=======
 
 Copyright (c) 2024, Rijkswaterstaat
 
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `displayrws-0.1.3/displayrws.egg-info/PKG-INFO` & `displayrws-0.1.4/displayrws.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: displayrws
-Version: 0.1.3
+Version: 0.1.4
 Summary: SPI Display and ESP32 project
 Author-email: RWS Datalab <datalab.codebase@rws.nl>
 Project-URL: homepage, https://gitlab.com/rwsdatalab/displayrws
 Project-URL: repository, https://gitlab.com/rwsdatalab/displayrws
 Project-URL: changelog, https://gitlab.com/rwsdatalab/displayrws/blob/main/CHANGELOG.rst
 Keywords: displayrws
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -42,30 +42,34 @@
 
 ##########
 displayrws
 ##########
 
 Dit project beschrijft hoe een 1,3 inch HD_IPS_TFT_LCD display van Joy-IT aangesloten kan worden op een ESP32.
 
+Benodigdheden:
 .. begin-inclusion-intro-marker-do-not-remove
 
 - ESP32 (type ESP-WROOM-32) bijv. van Joy-IT
 - kabeltjes
 - micro USB kabel
 - Display 240x240 pixel (SBC-LCD01)
 
 Verder is een computer met Python nodig.
 Toegang tot het USB device is noodzakelijk.
 
+############
+ Stappenplan
+############
 
-## Stappenplan
+Installeer Python
+===================
 
-. Installeer Python
-
-  ### Windows
+Windows
+~~~~~~~
 
   Klik op de Windows knop (Start).
 
   Type in:
 
   ```cmd```
 
@@ -77,24 +81,28 @@
 
   ```python get-pip.py```
 
   Wanneer Python nog niet geinstalleerd is, verschijnt er een Windows Store dialoog.
   In dit Windows Store dialoog, klik op Downloaden van Python.
 
 
-  ### Voor Linux:
+Voor Linux:
+~~~~~~~~~~~
 
   ```sudo apt install python3```
   ```sudo apt install python3-pip```
 
 
-. Installeer esphome:
+Installeer esphome:
+=====================
 
   ```pip install esphome```
+
   ```pip install pillow==10.2.0```
+
   ```pip install python-magic-bin``` (voor Windows)
 
   In Windows:
   wanneer deze melding te zien is:
 
   ```WARNING: The script esphome.exe is installed in C:\Users\<username>\AppData\Local\Packages\PythonSoftwareFoundation.Python..3.12_...\LocalCache...```
 
@@ -102,25 +110,27 @@
   ```set PATH="%PATH%;C:\your\path\here\"```
 
   Vervang C:\your\path\here\ door het path in de warning: C:\Users\<username>\AppData\Local\Packages\PythonSoftwareFoundation.Python....
 
   Sluit het Opdrachtprompt en start een nieuw Opdrachtprompt.
 
 
-. Zorg ervoor dat er genoeg rechten zijn om van het USB apparaat:
+Zorg ervoor dat er genoeg rechten zijn om van het USB apparaat:
+===============================================================
 
   Voor Linux:
 
   ```sudo usermod -a -G dialout [gebruikersnaam]```
 
   vervang: [gebruikersnaam] met jouw systeem gebruikersnaam.
 
   Restart jouw computer of log opnieuw in om deze rechten te effectueren.
 
-. Verbind met de kabeltjes van het ESP32 development board met het display:
+Verbind met de kabeltjes van het ESP32 development board met het display:
+=========================================================================
 
   SDA -> D13
 
   SCL -> D14
 
   DC -> D19
 
@@ -128,64 +138,68 @@
 
   RES -> D23
 
   GND -> GND (pin boven 3.3V)
 
   3V3 -> 3.3V (pin rechtsonder)
 
+
 .. image:: figs/pinouth.png
 
-. Verbind de USB kabel met het ESP32 board.
+Verbind de USB kabel met het ESP32 board.
+=========================================
 
 Het rode lampje moet branden.
 
-. In de USB devices controleer het USB ap
+In de USB devices controleer het USB apparaat
+=============================================
 
 In Linux:
   ```ls /dev/ttyU* -la```
 
 meestal staat er een nieuw USB device genaamd: ttyUSB01 of ttyUSB02 bij.
 
-. Voer uit:
+Voer uit:
+=========
 
   ```git clone https://gitlab.com/rwsdatalab/public/codebase/tools/displayrws.git```
+
   ````cd displayrws```
 
-. Voer uit:
+Voer uit:
+=========
 
   ```esphome run spi-display-image.yaml```
 
-Wanneer wordt gevraagd hoe te verbinden met het de ESP32 selecteer dan het USB apparaat bijv. /dev/USB01
-In Windows heet dit apparaat COM4.
+  Wanneer wordt gevraagd hoe te verbinden met het de ESP32 selecteer dan het USB apparaat bijv. /dev/USB01
+  In Windows heet dit apparaat COM4.
 
-. Nadat het flashen van de chip klaar is verschijnt er een blauwe vierkant met de tekst: RWS Datalab.
+  Nadat het flashen van de chip klaar is verschijnt er een blauwe vierkant met de tekst: RWS Datalab.
 
-. Maak bijv. een cirkel.
+  Maak bijv. een cirkel.
 
-Gebruik deze handleiding:
-https://esphome.io/components/display/index.html
+  Gebruik deze handleiding:
+  https://esphome.io/components/display/index.html
 
-## Handleiding ESP32
+#################
+Handleiding ESP32
+#################
 
 https://joy-it.net/files/files/Produkte/SBC-NodeMCU-ESP32/SBC-NodeMCU-ESP32-Manual-2021-06-29.pdf
 
 
 .. end-inclusion-intro-marker-do-not-remove
 
 
-Documentation
--------------
-
-Include a link to your project's full documentation here.
-
 
 .. begin-inclusion-license-marker-do-not-remove
 
+
 License
--------
+=======
 
 Copyright (c) 2024, Rijkswaterstaat
 
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `displayrws-0.1.3/pyproject.toml` & `displayrws-0.1.4/pyproject.toml`

 * *Files identical despite different names*

