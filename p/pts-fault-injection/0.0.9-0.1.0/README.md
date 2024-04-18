# Comparing `tmp/pts_fault_injection-0.0.9.tar.gz` & `tmp/pts_fault_injection-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_fault_injection-0.0.9.tar", last modified: Fri Feb  2 11:21:04 2024, max compression
+gzip compressed data, was "dist/pts_fault_injection-0.1.0.tar", last modified: Thu Apr 18 13:26:39 2024, max compression
```

## Comparing `pts_fault_injection-0.0.9.tar` & `pts_fault_injection-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/
--rw-r--r--   0 root         (0) root         (0)     4002 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1043 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4002 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3470 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/pts_fault_injection/
--rw-rw-rw-   0 root         (0) root         (0)    23723 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/pts_fault_injection/fib_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     6146 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/pts_fault_injection/cmb_box.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/pts_fault_injection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6176 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/pts_fault_injection/load_box.py
--rw-rw-rw-   0 root         (0) root         (0)     7764 2024-02-02 11:20:55.000000 pts_fault_injection-0.0.9/pts_fault_injection/CANFWupdate.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-02 11:21:04.000000 pts_fault_injection-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     4002 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      969 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4002 2024-04-18 13:26:38.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 13:26:38.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-18 13:26:38.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-18 13:26:38.000000 pts_fault_injection-0.1.0/pts_fault_injection.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/pts_fault_injection/
+-rw-rw-rw-   0 root         (0) root         (0)    32907 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/pts_fault_injection/fib_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     8261 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/pts_fault_injection/cmb_box.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/pts_fault_injection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7658 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/pts_fault_injection/load_box.py
+-rw-rw-rw-   0 root         (0) root         (0)     7764 2024-04-18 13:26:30.000000 pts_fault_injection-0.1.0/pts_fault_injection/CANFWupdate.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 13:26:39.000000 pts_fault_injection-0.1.0/setup.cfg
```

### Comparing `pts_fault_injection-0.0.9/PKG-INFO` & `pts_fault_injection-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_fault_injection
-Version: 0.0.9
+Version: 0.1.0
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.0.9/setup.py` & `pts_fault_injection-0.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_fault_injection",
-    version="0.0.9",
+    version="0.1.0",
     author="Pass testing Solutions GmbH",
     description="Fault Injection box Diagnostics package Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/pts-fault-injection-box",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     py_modules=["pts_fault_injection"],
-    install_requires=['python-can==4.0.0', 'dash==2.5.1', 'cantools>=37.0.7', 'tabulate==0.8.10', 'uptime==3.0.1',
-                      'pyserial==3.5'],
+    install_requires=['python-can>=4.0.0', 'cantools>=37.0.7', 'uptime==3.0.1'],
     packages=find_packages(include=['pts_fault_injection']),
     package_data={'pts_fault_injection': ['dbc/*.dbc']},
     include_package_data=True,
 )
```

### Comparing `pts_fault_injection-0.0.9/pts_fault_injection.egg-info/PKG-INFO` & `pts_fault_injection-0.1.0/pts_fault_injection.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-fault-injection
-Version: 0.0.9
+Version: 0.1.0
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.0.9/LICENSE.txt` & `pts_fault_injection-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.9/README.md` & `pts_fault_injection-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.9/pts_fault_injection/fib_controller.py` & `pts_fault_injection-0.1.0/pts_fault_injection/fib_controller.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import can
 import sys
 import time
+from typing import List, Dict, Tuple, Union
 import logging
 import cantools
 from cantools.database.can.signal import NamedSignalValue
 
 broadcast_id = 0x600
 board_ids = {0: "Standard Signals 1",
              1: "Standard Signals 2",
@@ -17,87 +18,94 @@
              9: "Contactor Card",
              10: "HV Box Card",
              14: "DAC Board",
              15: "Break Out Box",
              16: "CMB Faults"
              }
 
-dac_setpoints = [-1, -1, -1, -1, -1, -1, -1, -1]  # 8 DAC Channels
-dac_mapping = {0: 9,
-               1: 1,
-               2: 5,
-               3: 3,
-               4: 4,
-               5: 5,
-               6: 6,
-               7: 7}  # DAC Channel : Message Channel
+dbc_dir = os.path.join(os.path.dirname(__file__)) + "/dbc/"
+can_db = cantools.database.Database()
+for file in os.listdir(dbc_dir):
+    if file.endswith(".dbc"):
+        can_db.add_dbc_file(os.path.join(os.getcwd(), dbc_dir + file))
 
 
 def test_card(card):
     funcs = {
         "AnalogSignal": AnalogSignalCard.test_analog_signal_card,
         "StandardSignal1": StandardSignalCard.test_standard_signal_card1,
         "StandardSignal2": StandardSignalCard.test_standard_signal_card2,
         "StandardSignal3": StandardSignalCard.test_standard_signal_card3,
         "StandardSignal4": StandardSignalCard.test_standard_signal_card4,
         "BusSignal": BusSignalCard.test_bus_signal_card,
         "HVSignal": HVSignalCard.test_hv_signal_card,
-        # "CellFault": self.test_cell_fault_board,
-        # "LoadboxContactorCard": self.test_lb_contactor_card
     }
     if card in funcs:
-        print(f"TESTING BOARD {card}")
+        logging.debug(f"TESTING BOARD {card}")
         funcs[card]()
     else:
         raise Exception(f"Signal Card {card} not present.")
 
 
 class FaultInjectionController(object):
     """
     Base class for the Fault Injection Box Controller
     """
     logging.basicConfig(format='%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s',
                         datefmt='%Y-%m-%d %H:%M:%S',
-                        level=logging.INFO)
+                        level=logging.getLogger().setLevel(logging.INFO))
 
-    def __init__(self, dbc_dir=os.path.join(os.path.dirname(__file__))+"/dbc/"):
-        self.can_db = cantools.database.Database()
-        self.bus = None
-        self.dbc_dir = dbc_dir
-        logging.info(f"Searching for DBCs in {self.dbc_dir}")
-        for file in os.listdir(self.dbc_dir):
-            if file.endswith(".dbc"):
-                logging.info(f"adding {file}")
-                self.can_db.add_dbc_file(os.path.join(os.getcwd(), self.dbc_dir + file))
+    def __init__(self):
+        self._bus = None
+        self.card_state = 0
         self.signal_cards = [
-            StandardSignalCard(),
-            StandardSignalCard(),
-            StandardSignalCard(),
-            StandardSignalCard(),
-            AnalogSignalCard(),
-            BusSignalCard(),
-            SignalCard(),
-            HVSignalCard(),
+            StandardSignalCard(0),
+            StandardSignalCard(1),
+            StandardSignalCard(2),
+            StandardSignalCard(3),
+            AnalogSignalCard(4),
+            BusSignalCard(5),
+            HVSignalCard(6),
         ]
-        return
 
-    def can_connection(self, interface, channel, bitrate):
+    def can_connection(self, interface: str, channel: str, bitrate: int):
+        """
+        Sets up the CAN connection
+        :param interface: Type of interface: 'pcan', 'vector', 'socketcan'
+        :param channel: 'PCAN_USBBUSx', '0', 'canx'
+        :param bitrate: e.g. 500000
+        :return: None
+        """
         can.rc['interface'] = interface
         can.rc['channel'] = channel
         can.rc['bitrate'] = bitrate
         self.bus = can.interface.Bus()
 
-    def read_FW_Response(self):
+    @property
+    def bus(self):
+        return self._bus
+
+    @bus.setter
+    def bus(self, val):
+        self._bus = val
+        for sc in self.signal_cards:
+            sc.bus = val
+
+    def _read_fw_response(self) -> Tuple:
+        """
+        Reads back the FW version for board IDs
+        :return: tuple: board id, FW version
+        """
         time.sleep(1)
         wait_time = 1 + time.time()
         msg = self.bus.recv(timeout=1)
         rdy_IDs = []
         msg_buf = {}
         fw_versions = {}
-        print("Searching for ready controllers.")
+        logging.debug("Searching for ready controllers.")
         while wait_time > time.time():
             if msg is not None and msg.dlc > 0:
                 if 0x6FF > msg.arbitration_id > 0x600:
                     rdy_IDs.append(msg.arbitration_id)
                     msg_buf[msg.arbitration_id] = msg.data
                 sys.stdout.write(".")
                 sys.stdout.flush()
@@ -105,123 +113,201 @@
         try:
             for id in rdy_IDs:
                 fw_versions[id] = msg_buf[id].decode("ASCII")
         except Exception as e:
             raise Exception(f"\nError in finding FW versions for all responses {e}")
         return rdy_IDs, fw_versions
 
-    def read_FW_Versions(self):
+    def read_fw_versions(self) -> Dict:
+        """
+        Reads FW versions for the signal cards
+        :return: dict: FW version for each board with board ID
+        """
         # Writing FW Update Request
-        logging.info("Using broadcast ID " + hex(broadcast_id))
+        logging.debug("Using broadcast ID " + hex(broadcast_id))
         msg = can.Message(arbitration_id=broadcast_id, data=[ord('F'), ord('W'), ord('?'), 0, 0, 0, 0, 0],
                           is_extended_id=False)
         self.bus.send(msg)
         # Block until ready
-        ids, fw_versions = self.read_FW_Response()
+        ids, fw_versions = self._read_fw_response()
         for id in ids:
             try:
-                logging.info("\nFW Information from board: " + board_ids[id - broadcast_id - 1] + " with FW version: "
+                logging.debug("\nFW Information from board: " + board_ids[id - broadcast_id - 1] + " with FW version: "
                              + str(fw_versions[id]))
             except Exception as e:
-                # pass
                 raise Exception(f"ERR: Could not read FW version: {e}")
-            return fw_versions
+        return fw_versions
 
     def load_mapping(self):
         """
         This function loads the hil project specific signal mapping
         """
         return
 
-    def set(self, channel, command, value):
+    def set_single_relay(self, pin: int, command: str, value: bool) -> None:
         """
-        Sets or unsets a command on a specific channel
-        :param channel: int: channel number
-        :param command:
-        :param value: bool: set or unset the oc
+        Sets or resets a command on a specific pin on the FIB.
+        Pins are 1 Based like on the Connector
+        :param pin: pin-number one based
+        :param command: 'oc', 'dac', 'fr1', 'fr2', 'r12', 'r24', 'r51', 'r100', etc. based on the signal card
+        :param value: bool: True (Set relay) or False (reset relay)
         """
-        [card, signal] = self.get_fib_card(channel)
-        # get numer and send command
+        [card, signal] = self.get_fib_card(pin - 1)
+        # Get number and send command
         data = self.signal_cards[card].get_command_for_msg(signal, command, value)
-        self.send_relay_can_message(card, data, channel)
+        self.send_relay_can_message(card, data, pin)
+        self.signal_cards[card].update_state()
+        logging.debug(f"Sending command: {command} for Pin {pin} to Card: {card} with DL: {bin(data)}")
 
-    def send_relay_can_message(self, card, data, channel):
+    def set_multiple_relays(self, command: str, value: bool, pins: List[int] = None) -> None:
+        """
+        Sets or resets the relays for the list of pins
+        :param pins: list of pins one based
+        :param command: str: 'oc', 'fr1', 'fr2', 'r12', etc. based on the card (only one command at a time)
+        :param value: bool: True (Set relay) or False (reset relay)
+        :return: None
         """
-        creates a can message out of the state and sends it to the can connector
+        for pin in pins:
+            self.set_single_relay(pin, command, value)
 
-        CAN Message is RC_Cntrl , ID 0x210
+    def get_fib_state(self) -> Dict:
+        """
+        Returns the full Pin State of the FIB as a dictionary. Pins are one based
+        :return dict: {Pin number: Status}
+        """
+        states = {}
+        out = {}
+        pins = list(range(1, 71))
+        # Remove pin 49 (0 based) as it is not connected
+        pins.remove(50)
+        # First update and get states
+        for i in range(7):
+            states[i] = self.signal_cards[i].get_status()
+
+        for pin in pins:
+            card, signal = self.get_fib_card(pin - 1)
+            out[pin] = states[card][signal]
+        logging.debug(f"Status: {out}")
+        return out
+
+    def oc_all_relays(self) -> None:
+        """
+        Open Circuits all relays on the signal cards (except HV signal card)
+        """
+        # Get number and send command
+        self.set_multiple_relays("oc", True, list(range(1, 50))+list(range(51, 61)))
+
+    def send_card_can_message(self, card: int, data: bin) -> None:
+        """
+        Creates a can message out of the state and sends it to the can connector for a signal card
+        :param card: int: 0-5 for the Signal Cards
+        :param data: CAN Message is RC_Cntrl, ID 0x210
         Signals :
-            RC_mux -> fib Card (0-7) multiplexer
+            RC_mux -> FIB Card (0-7) multiplexer
             RC_cntrlXX -> 60 Bit for the relays XX is multiplexer eg (01 or 00)
         """
         mux_name = "RC_cntrl" + str(card).zfill(2)
+        cmd = {"RC_mux": card, mux_name: data}
+        self.send_can_message("RC_Cntrl", cmd)
 
+    def send_relay_can_message(self, card, data, channel) -> None:
+        """
+        Creates a CAN message out of the state and sends it to the can connector
+        CAN Message is RC_Cntrl, ID 0x210
+        Signals :
+            RC_mux -> FIB Card (0-7) multiplexer
+            RC_cntrlXX -> 60 Bit for the relays XX is multiplexer eg (01 or 00)
+        :param card: Card (0-7)
+        :param data: bin data to be sent to the controller
+        :param channel: output channel pin
+        """
+        mux_name = "RC_cntrl" + str(card).zfill(2)
         cmd = {"RC_mux": card, mux_name: data, "chan": channel}
         self.send_can_message("RC_Cntrl", cmd)
 
-    def send_can_message(self, msg_name, commands):
+    def send_can_message(self, msg_name: str, commands) -> None:
+        """
+        Reads the CAN message from the DBC file and sends it over the bus
+        :param msg_name: str: CAN Command message
+        :param commands: dict: dictionary of CAN msg and integer information
+        """
         try:
-            cmd_message = self.can_db.get_message_by_name(msg_name)
+            cmd_message = can_db.get_message_by_name(msg_name)
         except Exception as e:
-            print(f"ERROR: Message {msg_name} not found in Databases")
-            print(e)
+            logging.error(f"ERROR: {e}: Message {msg_name} not found in Databases")
             return None
 
-        # prepare a message with all signals
+        # Prepare a message with all signals
         signals = {}
         for signal in cmd_message.signals:
             if signal.name in commands:
                 signals[signal.name] = commands[signal.name]
             else:
                 signals[signal.name] = 0
 
         message = can.Message(arbitration_id=cmd_message.frame_id,
                               data=cmd_message.encode(signals, strict=False),
                               is_extended_id=False)
-        logging.info(f"sending message {message}")
-        self.bus.send(message)
+        logging.debug(f"Sending Message {message}")
+        self._bus.send(message)
 
-    def get_fib_card(self, channel):
+    def get_fib_card(self, channel: int) -> List:
         """
         Calculates the FIB card number for a specific channel
-        range 0-39 -> Standard signal card Id 10 steps
+        range 0-39 -> Standard signal card ID 10 steps
         range 40-49 -> Analog Signal card
         range 50-59 -> Bus Signal
         range 60-69 -> HV Signals
-        Parameters
-        ----------
-        channel : int
-            the channel to look for
-
-        Returns
-        -------
-        int
-            fib card number starting at 0
-
+        :param channel : the channel to look for
+        :return list : fib card number starting at 0, signal number on card
         """
-        if channel in range(0, 70):
+        analog_signal_backplane_map = {
+            40: 0,
+            41: 1,
+            42: 2,
+            43: 3,
+            44: 4,
+            45: 5,
+            46: 6,
+            47: 8,  # Skip channel because it is not connected on backplane
+            48: 9,
+        }
+        if channel in range(0, 40) or channel in range(50, 70):  # Standard signal cards, Bus and HV signals
             return [channel // 10, channel % 10]
+        if channel in range(40, 50):  # Analog Signal card
+            return [4, analog_signal_backplane_map[channel]]
         else:
             return [-1, -1]
 
+    def set_dac_channel(self, channel: int, value: float) -> bool:
+        """
+        Sets the DAC channel value 0-5V on the Analog signal Card based on pin (1 Based) of FIB
+        :param channel: Pin-number on the FIB
+        :param value: float: Voltage value between 0-5V
+        :return bool: True or False
+        """
+        if channel in range(41, 48):
+            self.signal_cards[4].set_dac_value(channel - 41, value)
+            logging.debug(f"Setting DAC for channel: {channel} to voltage: {value}")
+            return True
+        else:
+            logging.error(f"Channel {channel} has no DAC to set")
+            return False
+
 
 class SignalCard(object):
     """
     Base class for the Signal Cards
     """
-    def __init__(self, dbc_dir=os.path.join(os.path.dirname(__file__))+"/dbc/"):
-        self.bus = None
-        self.can_db = cantools.database.Database()
-        self.dbc_dir = dbc_dir
-        for file in os.listdir(self.dbc_dir):
-            if file.endswith(".dbc"):
-                self.can_db.add_dbc_file(os.path.join(os.getcwd(), self.dbc_dir + file))
 
+    def __init__(self, id=0):
+        self.bus = None
         self.state = 0
         self.cmd_len = None
+        self.id = id
 
     def can_connection(self, interface, channel, bitrate):
         """
         Establishes a CAN connection
         :param interface: this usage with PEAK CAN Dongle
         :param channel: PCAN_USBBUS
         :param bitrate: 500000
@@ -240,37 +326,36 @@
             return self.state | bit  # make 'or' to switch on
         else:
             return self.state & ~bit  # make 'and' with negated to switch off
 
     def get_command_for_msg(self, signal, command, value):
         return None
 
-    def parse_state(self):
-        return None
-
-    def send_can_message(self, msg_name, commands):
+    def send_can_message(self, msg_name, commands, remote=False):
         try:
-            cmd_message = self.can_db.get_message_by_name(msg_name)
+            cmd_message = can_db.get_message_by_name(msg_name)
         except Exception as e:
-            print(f"ERROR: Message {msg_name} not found in Databases")
-            print(e)
+            logging.error(f"ERROR: {e}: Message {msg_name} not found in Databases")
             return None
 
-        # prepare a message with all signals
-        signals = {}
-        for signal in cmd_message.signals:
-            if signal.name in commands:
-                signals[signal.name] = commands[signal.name]
-            else:
-                signals[signal.name] = 0
-
-        message = can.Message(arbitration_id=cmd_message.frame_id,
-                              data=cmd_message.encode(signals, strict=False),
-                              is_extended_id=False)
-        logging.info(f"sending message {message}")
+        # if not remote frame prepare a message with all signals
+        if not remote:
+            signals = {}
+            for signal in cmd_message.signals:
+                if signal.name in commands:
+                    signals[signal.name] = commands[signal.name]
+                else:
+                    signals[signal.name] = 0
+
+            message = can.Message(arbitration_id=cmd_message.frame_id,
+                                  data=cmd_message.encode(signals, strict=False),
+                                  is_extended_id=False)
+        else:
+            message = can.Message(arbitration_id=cmd_message.frame_id, is_remote_frame=True, is_extended_id=False)
+        logging.debug(f"sending message {message}")
         self.bus.send(message)
 
     @staticmethod
     def print_bin(num):
         x = []
         for b in num:
             x.append(bin(b))
@@ -287,123 +372,124 @@
         out = [0] * 8
         out[0] = out[0] | (card_id & 0xF)
         out[0] = out[0] | (relay_data & 0xF) << 4
         for i in range(7):
             out[i + 1] = out[i + 1] | ((relay_data >> (i * 8) + 4) & 0xFF)
         return out
 
-    def set_dac_value(self, channel, value):
-        """Short summary.
-        creates a can message out of the  dac state and sends it to the can connector
-
-        CAN Message is DAC_BMS_Cntrl , ID 0x220
-        Be aware of a weird channel mapping
-        """
-        dac_setpoints[channel] = value
-        # Generate Signal name DAC_BMS_Cntrl_XX_YY_Voltage
-        channel_msg = dac_mapping[channel] - 1
-        dac_no = str(channel_msg // 4 + 1).zfill(2)  # Calculate Dac index, each dac has 4 channels
-        ch_no = str((channel_msg % 4) + 1).zfill(2)  # channel is mod 4, both have to be filled to two digits
-        mux = (0x10 * (channel_msg // 4)) + (channel_msg % 4)  # mux is 0-3 + 0x10 after each 4 channels
-        cmd = {'DAC_BMS_Cntrl_Channel': mux, f"DAC_BMS_Cntrl_{dac_no}_{ch_no}_Voltage": value}
-        self.send_can_message("DAC_BMS_Cntrl", cmd)
-
-    def send_relay_can_message(self, card, data):
+    def send_relay_can_message(self, card, data) -> None:
         mux_name = "RC_cntrl" + str(card).zfill(2)
         cmd = {'RC_mux': card, mux_name: data}
         self.send_can_message("RC_Cntrl", cmd)
 
-    def send_relay_can_message_raw(self, card, data):
+    def send_relay_can_message_raw(self, card, data) -> None:
+        """
+        Sends raw CAN message to the card
+        :param card: int: card ID
+        :param data: bin: data to be sent
+        """
         message = can.Message(arbitration_id=528,
                               data=self.create_payload(card, data),
                               is_extended_id=False)
         self.bus.send(message)
 
-    def check_card(self, card, relays=None):
+    def update_state(self):
+        """
+        Updates the state of the card with a remote frame. Only for new FW Boxes
+        - Send a remote frame for relay control
+        - Wait for a state response for the correct card (timeout is 0.5s)
+        - Update internal state
+        """
+        # Clear messages in buffer
+        while self.bus.recv(timeout=0.01):
+            pass
+        self.send_can_message("RC_Cntrl", None, remote=True)
+        end_time = time.time() + 0.2
+        got_state = False
+        for msg in self.bus:
+            if time.time() > end_time:
+                break
+            if msg.arbitration_id == 0x300 + self.id:
+                # Decode Status message
+                logging.debug(msg)
+                signals = can_db.decode_message(msg.arbitration_id, msg.data)
+                if "RC_mux" in signals and signals["RC_mux"] == self.id:
+                    self.state = signals[f"RC_cntrl{str(self.id).zfill(2)}"]
+                    logging.debug(f"Got state for card {self.id}, {bin(self.state)}")
+                    got_state = True
+                    break
+        if not got_state:
+            logging.error(f"Could not retrieve state for card {self.id}")
+
+    def check_card(self, card: int, relays: List[int] = None):
+        """
+        Checks the card ID for appropriate operations
+        :param card: Card ID
+        :param relays: List of relays on the signal card
+        """
         if card > 16:
-            print(f"Card not there: {card}")
+            logging.debug(f"Card not there: {card}")
             return None
         if relays is None:
             max_relays = [32, 32, 32, 32, 48, 48, 32]  # max relays of cards
             relays = range(max_relays[card])
         if card == 4:  # analog card also set dac
             for ch in range(8):
                 self.set_dac_value(ch, 2)
         for relay_no in relays:
             rly_set = 1 << (relay_no)
-            print(f"Setting Card {card}, relay {relay_no}")
-            print(bin(rly_set))
+            logging.debug(f"Setting Card {card}, relay {relay_no}")
+            logging.debug(bin(rly_set))
             self.send_relay_can_message_raw(card, rly_set)
             time.sleep(0.5)
             self.send_relay_can_message_raw(card, 0)
             time.sleep(0.1)
 
 
 class StandardSignalCard(SignalCard):
-    """Short summary.
+    """
     Standard Signal card has 10 Signals with the following functions:
         - Short to Chassis (SC)
         - Short to Faultrail
         - Open Circuit to out
 
     Mapping always signal*3 +
         - 0 for SC
         - 1 for Fault Rail
         - 2 for open circuit
     """
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, id=0):
+        super().__init__(id)
         self.state = 0  # Todo get initial state from status message
         self.signals = 10
         self.cmd_len = 3  # amount of usable functions on card
         return
 
     def get_command_for_msg(self, signal, command, value):
+        # Make sure that state has been updated
+        self.update_state()
         # Check if channel in range
         if signal >= self.signals:
-            print(f"Warning: Channel {signal} in command not accepted")
+            logging.warning(f"Warning: Channel {signal} in command not accepted")
             return self.state
 
         # Calculate command
-        if command == "sc":
+        if command == "fr2":
             cmd = 0b001
-        elif command == "fr":
+        elif command == "fr1":
             cmd = 0b010
         elif command == "oc":
             cmd = 0b100
         else:
-            print(f"Warning: {command} not accepted")
+            logging.warning(f"Warning: {command} not accepted")
             return self.state
-
+        logging.debug(f"calculated bit {self.calculate_bit(signal, cmd, value)}")
         return self.calculate_bit(signal, cmd, value)
 
-    def parse_state(self):
-        """Short summary.
-        Returns a List with command to be set in CAN
-        Returns
-        Also here we need to shift by one if signal >= 5
-        -------
-        dict
-            dict with data to be updated in CAN
-
-        """
-        def get_sig(sig, cmd):
-            out = ((self.state >> (sig * self.cmd_len)) & cmd) > 0
-            if sig >= 5:
-                out = out >> 1
-            return out
-
-        out = {}
-        for signal in range(self.signals):
-            out[signal] = {"sc": get_sig(signal, 0b001),
-                           "fr": get_sig(signal, 0b010),
-                           "oc": get_sig(signal, 0b100)}
-        return out
-
     def calculate_bit(self, signal, cmd, value):
         """
         Standard signal card uses not all channels of expander
         After the first 5 signals we need to shift by one bit
         Therefore shift by one bit if signal >= 5 (zero based )
         """
         bit = cmd << signal * self.cmd_len
@@ -411,262 +497,362 @@
             bit = bit << 1
 
         if value:
             return self.state | bit  # make 'or' to switch on
         else:
             return self.state & ~bit  # make 'and' with negated to switch off
 
-    def test_standard_signal_card1(self):
+    def test_standard_signal_card1(self) -> None:
+        """
+        Function to test all the Standard Signal Card 1 relays
+        """
         used_ports = list(range(15)) + list(range(16, 31))  # zero based
         self.check_card(0, used_ports)
 
-    def test_standard_signal_card2(self):
+    def test_standard_signal_card2(self) -> None:
+        """
+        Function to test all the Standard Signal Card 2 relays
+        """
         used_ports = list(range(15)) + list(range(16, 31))  # zero based
         self.check_card(1, used_ports)
 
-    def test_standard_signal_card3(self):
+    def test_standard_signal_card3(self) -> None:
+        """
+        Function to test all the Standard Signal Card 3 relays
+        """
         used_ports = list(range(15)) + list(range(16, 31))  # zero based
         self.check_card(2, used_ports)
 
-    def test_standard_signal_card4(self):
+    def test_standard_signal_card4(self) -> None:
+        """
+        Function to test all the Standard Signal Card 4 relays
+        """
         used_ports = list(range(15)) + list(range(16, 31))  # zero based
         self.check_card(3, used_ports)
 
+    def get_status(self) -> Dict:
+        """
+        Returns the standard signal card status as dictionary
+        """
+        self.update_state()
+        out = {}
+        for i in range(10):
+            # If i >4, shift by one bit / see schematics 
+            offset = 0
+            if i > 4: offset = 1
+            out[i] = {
+                "fr1": bool((self.state >> 3 * i + offset) & 0b010),
+                "fr2": bool((self.state >> 3 * i + offset) & 0b001),
+                "oc": bool((self.state >> 3 * i + offset) & 0b100),
+            }
+        return out
+
 
 class AnalogSignalCard(SignalCard):
     """
     Analog Signal card has 8 Signals with the following functions:
-        - Short to Chassis (SC)
-        - Short to Fault Rail
+        - Short to Fault Rail 2 (FR2)
+        - Short to Fault Rail (FR1)
         - Connect DAC Output
         - Open Circuit to out
 
     And 2 signals that are resistor signals with the following functions:
-        - Short to Chassis (SC)
-        - Short to Fault Rail
+        - Short to Chassis (FR2)
+        - Short to Fault Rail (FR1)
         - Resistor 12R
         - Resistor 24R
         - Resistor 51R
         - Resistor 100R
         - Open Circuit to out
 
     Mapping always signal*4 +
-        - 0 for SC
-        - 1 for Fault Rail
+        - 0 for FR2
+        - 1 for Fault Rail FR1
         - 2 for Connect dac
         - 3 for open circuit
     """
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, id=4):
+        super().__init__(id)
         self.bus = self.bus
         self.state = 0  # Todo get initial state from status message
         self.signals = 10
         self.cmd_len = 4  # amount of usable functions on card
+        self.dac_setpoints = [-1, -1, -1, -1, -1, -1, -1, -1]  # 8 DAC Channels
+        self.dac_mapping = {
+            0: 9,
+            1: 1,
+            2: 5,
+            3: 2,
+            4: 4,
+            5: 3,
+            6: 6,
+            7: 7}  # DAC Channel : Message Channel
         return
 
-    def parse_state(self):
-        """Short summary.
-        Returns a List with command to be set in CAN
-        Returns
-        -------
-        dict
-            dict with data to be updated in CAN
-
-        """
-
-        def get_sig(sig, cmd):
-            return ((self.state >> (sig * 4)) & cmd) > 0
-
+    def get_status(self) -> Dict:
+        # Analog channels:
+        self.update_state()
         out = {}
-        for signal in range(0, 8):
-            out[signal] = {"sc": get_sig(signal, 0b0001),
-                           "fr": get_sig(signal, 0b0010),
-                           "dac": get_sig(signal, 0b0100),
-                           "oc": get_sig(signal, 0b1000)
-                           }
-        for signal in range(8, self.signals):
-            out[signal] = {"sc": get_sig(signal, 0b0000001),
-                           "fr": get_sig(signal, 0b0000010),
-                           "r12": get_sig(signal, 0b0000100),
-                           "r24": get_sig(signal, 0b0001000),
-                           "r51": get_sig(signal, 0b0010000),
-                           "r100": get_sig(signal, 0b0100000),
-                           "oc": get_sig(signal, 0b1000000)
-                           }
+        for i in range(8):
+            out[i] = {
+                "fr1": bool((self.state >> 4 * i) & 0b0010),
+                "fr2": bool((self.state >> 4 * i) & 0b0001),
+                "dac": bool((self.state >> 4 * i) & 0b0100),
+                "oc": bool((self.state >> 4 * i) & 0b1000),
+            }
+        out[8] = {
+            "fr1": bool((self.state >> 32 & 0b0000010)),
+            "fr2": bool((self.state >> 32 & 0b0000001)),
+            "r12": bool((self.state >> 32 & 0b0000100)),
+            "r24": bool((self.state >> 32 & 0b0001000)),
+            "r51": bool((self.state >> 32 & 0b0010000)),
+            "r100": bool((self.state >> 32 & 0b0100000)),
+            "oc": bool((self.state >> 32 & 0b1000000)),
+        }
+        out[9] = {
+            "fr1": bool((self.state >> 40 & 0b0000010)),
+            "fr2": bool((self.state >> 40 & 0b0000001)),
+            "r330": bool((self.state >> 40 & 0b0000100)),
+            "r680": bool((self.state >> 40 & 0b0001000)),
+            "r1300": bool((self.state >> 40 & 0b0010000)),
+            "r2700": bool((self.state >> 40 & 0b0100000)),
+            "oc": bool((self.state >> 40 & 0b1000000)),
+        }
+
         return out
 
-    def get_command_for_msg(self, signal, command, value):
+    def set_dac_value(self, channel, value):
+        """
+        Creates a CAN message out of the DAC state and sends it to the CAN connector
+        CAN Message is DAC_BMS_Cntrl , ID 0x220
+        Be aware of a weird channel mapping
+        :param channel: Pin-number
+        :param value: Voltage value
+        """
+        self.dac_setpoints[channel] = value
+        # Generate Signal name DAC_BMS_Cntrl_XX_YY_Voltage
+        channel_msg = self.dac_mapping[channel] - 1
+        dac_no = str(channel_msg // 4 + 1).zfill(2)  # Calculate Dac index, each dac has 4 channels
+        ch_no = str((channel_msg % 4) + 1).zfill(2)  # channel is mod 4, both have to be filled to two digits
+        mux = (0x10 * (channel_msg // 4)) + (channel_msg % 4)  # mux is 0-3 + 0x10 after each 4 channels
+        cmd = {'DAC_BMS_Cntrl_Channel': mux, f"DAC_BMS_Cntrl_{dac_no}_{ch_no}_Voltage": value}
+        self.send_can_message("DAC_BMS_Cntrl", cmd)
+
+    def get_command_for_msg(self, signal: int, command: str, value: Union[bool, float]):
+        """
+        Gets the CAN message command to be sent for the standard signal card
+        :param signal: int: correct signal for the FIB card
+        :param command: str: command for the FIB card
+        :param value: bool or float based on the command
+        :return: Bin command
+        """
         # Check if channel in range
+        self.update_state()
         if signal >= self.signals:
-            print(f"Warning: Channel {signal} in command not accepted")
+            logging.warning(f"Warning: Channel {signal} in command not accepted")
             return self.state
 
-        # calculate command
+        elif command == "dac_voltage":
+            if signal in range(0, 7):
+                self.set_dac_value(signal, float(value))
+                return self.state
+        # Calculate command
         elif signal in range(0, 8):
-            if command == "sc":
+            if command == "fr2":
                 cmd = 0b0001
-            elif command == "fr":
+            elif command == "fr1":
                 cmd = 0b0010
             elif command == "dac":
                 cmd = 0b0100
             elif command == "oc":
                 cmd = 0b1000
-        elif signal in range(8, self.signals):
-            if command == "sc":
+        elif signal == 8:
+            if command == "fr2":
                 cmd = 0b0000001
-            elif command == "fr":
+            elif command == "fr1":
                 cmd = 0b0000010
             elif command == "r12":
                 cmd = 0b0000100
             elif command == "r24":
                 cmd = 0b0001000
             elif command == "r51":
                 cmd = 0b0010000
             elif command == "r100":
                 cmd = 0b0100000
             elif command == "oc":
                 cmd = 0b1000000
-
-        elif command == "dac_voltage":
-            if signal in range(0, 7):
-                self.set_dac_value(signal, float(value))
-                return self.state
+        elif signal == 9:
+            if command == "fr2":
+                cmd = 0b0000001
+            elif command == "fr1":
+                cmd = 0b0000010
+            elif command == "r330":
+                cmd = 0b0000100
+            elif command == "r680":
+                cmd = 0b0001000
+            elif command == "r1300":
+                cmd = 0b0010000
+            elif command == "r2700":
+                cmd = 0b0100000
+            elif command == "oc":
+                cmd = 0b1000000
         else:
-            print(f"Warning: {command} not accepted")
+            logging.warning(f"Warning: {command} not accepted")
             return self.state
+        if signal == 9:
+            # Due to inconsistent command length we need to do a little hack for the last signal
+            bit = cmd << 40
+            if value:
+                return self.state | bit  # make 'or' to switch on
+            else:
+                return self.state & ~bit  # make 'and' with negated to switch off
         return self.calculate_bit(signal, cmd, value)
 
-    def test_analog_signal_card(self):
+    def test_analog_signal_card(self) -> None:
+        """
+        Function to test all the Analog Signal card relays
+        """
         used_ports = list(range(39)) + list(range(40, 48))  # zero based
         self.check_card(4, used_ports)
 
 
 class BusSignalCard(SignalCard):
     """
     Bus Signal card has 12 Signals with the following functions:
         - Fault Rail 2 (First Bit)
         - Fault Rail 1 (second Bit)
         - Additional Input (third bit)
         - Open Circuit (fourth bit)
+    On FIB boot up, in the Bus Signal card, the relays 3 & 4 are NO by software instead of NC (default for other cards)
+    This is to facilitate the CAN H and CAN L connections to the DSUB-9 connector going to the load box, usually in a HiL.
     """
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, id=5):
+        super().__init__(id)
         self.bus = self.bus
         self.state = 0  # Todo get initial state from status message
         self.signals = 12
         self.cmd_len = 4  # amount of usable functions on card
         return
 
-    def parse_state(self):
+    def get_command_for_msg(self, signal, command, value):
         """
-        Returns a List with command to be set in can
-        :return dict: dict with data to be updated in can
+        Gets the CAN message command to be sent for the Bus signal card
+        :param signal: int: correct signal for the FIB card
+        :param command: str: command for the FIB card
+        :param value: bool or float based on the command
+        :return: Bin command
         """
-
-        def get_sig(sig, cmd):
-            return ((self.state >> (sig * 4)) & cmd) > 0
-
-        out = {}
-        for signal in range(0, 12):
-            out[signal] = {"fr2": get_sig(signal, 0b0001),
-                           "fr1": get_sig(signal, 0b0010),
-                           "in": get_sig(signal, 0b0100),
-                           "oc": get_sig(signal, 0b1000)
-                           }
-        return out
-
-    def get_command_for_msg(self, signal, command, value):
-        cmd = {}
+        cmd = None
+        self.update_state()
         # Check if channel is in range
         if signal >= self.signals:
-            print(f"Warning: Channel {signal} in command not accepted")
+            logging.warning(f"Warning: Channel {signal} in command not accepted")
             return self.state
 
         # calculate command
         elif signal in range(0, self.signals):
             if command == "fr2":
                 cmd = 0b0001
             elif command == "fr1":
                 cmd = 0b0010
             elif command == "in":
                 cmd = 0b0100
             elif command == "oc":
                 cmd = 0b1000
         else:
-            print(f"Warning: {command} not accepted")
+            logging.warning(f"Warning: {command} not accepted")
             return self.state
         return self.calculate_bit(signal, cmd, value)
 
-    def test_bus_signal_card(self):
+    def get_status(self):
+        self.update_state()
+        out = {}
+        for i in range(10):
+            out[i] = {
+                "fr1": bool((self.state >> 4 * i) & 0b0010),
+                "fr2": bool((self.state >> 4 * i) & 0b0001),
+                "in": bool((self.state >> 4 * i) & 0b0100),
+                "oc": bool((self.state >> 4 * i) & 0b1000),
+            }
+        return out
+
+    def test_bus_signal_card(self) -> None:
+        """
+        Function to test all the Bus Signal card relays
+        """
         used_ports = list(range(3 * 16))  # zero based
         self.check_card(5, used_ports)
 
 
 class HVSignalCard(SignalCard):
     """
     HV Signal card has 8 HV Signals with the following functions:
         - Short to Chassis (SC) via resistor
         - Open Circuit
     There are also 2 Channels for ISOSPI Connection which allow Open Circuit
     Channel 1-8 -> HV
     Channel 9,10 -> ISOSPI
     """
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, id=6):
+        super().__init__(id)
         # Initial State is complicated. All first 16 Bits are 'on'
         # On the second 16 Bit we need to switch on only every second
         self.bus = self.bus
-        self.state = int(b"01010101010101011111111111111111", 2)  # Todo get initial state from status message
+        # Todo get initial state from status message
+        # self.state = int(b"01010101010101011111111111111111", 2)
         self.signals = 10
         self.cmd_len = 2  # amount of usable functions on card
         return
 
     def get_command_for_msg(self, signal, command, value):
+        """
+        Gets the CAN message command to be sent for the HV signal card
+        :param signal: int: correct signal for the FIB card
+        :param command: str: command for the FIB card
+        :param value: bool or float based on the command
+        :return: Bin command
+        """
+        self.update_state()
+        cmd = None
         # Check if channel in range
         if signal >= self.signals:
-            print(f"Warning: Channel {signal} in command not accepted")
+            logging.warning(f"Warning: Channel {signal} in command not accepted")
             return self.state
 
         # Calculate command
-        if command == "oc":
-            cmd = 0b01
-        elif command == "sc":
-            cmd = 0b10
-        else:
-            print(f"Warning: {command} not accepted")
+        if signal in range(8):
+            if command == "oc":
+                cmd = 0b01
+            elif command == "sc":
+                cmd = 0b10
+        if signal in range(8, 10):
+            if command == "oc":
+                cmd = 0b10
+            elif command == "in":
+                cmd = 0b01
+        if cmd == None:
+            logging.warning(f"Warning: {command} not accepted")
             return self.state
         return self.calculate_bit(signal, cmd, value)
 
-    def parse_state(self):
-        """
-        Returns a List with command to be set in CAN
-        Returns
-        Also here we need to shift
-        BE careful as signals for HV Card are inverted
-        -------
-        dict
-            dict with data to be updated in can
-
-        """
-
-        def get_sig(sig, cmd):
-            if sig >= 8:
-                return ((self.state >> ((sig - 8) * self.cmd_len)) & ~cmd) > 0
-            if sig < 8:
-                return ((self.state >> (16 + sig * self.cmd_len)) & cmd) > 0
-            return out
-
+    def get_status(self) -> Dict:
+        self.update_state()
         out = {}
-        for signal in range(self.signals):
-            out[signal] = {
-                "oc": get_sig(signal, 0b001),
-                "sc": get_sig(signal, 0b010),
+        for i in range(8):
+            out[i] = {
+                "oc": not bool((self.state >> 16 + (2 * i)) & 0b01),
+                "sc": bool((self.state >> 16 + (2 * i)) & 0b10),
+            }
+        for i in range(8, 10):
+            out[i] = {
+                "oc": not bool((self.state >> 16 + (2 * (i - 8))) & 0b01),
+                "in": bool((self.state >> 16 + (2 * (i - 8))) & 0b10),
             }
         return out
 
     def calculate_bit(self, signal, cmd, value):
         """
         HV signal card uses not all channels of expander the first expander
         is connected to ISOSPI channels. second one is for HV Signals
@@ -675,22 +861,37 @@
         if signal >= 8:
             bit = cmd << ((signal - 8) * self.cmd_len)
         else:
             bit = cmd << ((signal * self.cmd_len) + 16)
 
         # HV OC Signals are reed relays and need and are inverted -> On is not SC, Off is SC
         # HV SC Signals are not inverted, so we need to distinguish
-        if value:
-            if cmd == 0b01:
-                return self.state & ~bit  # make 'or' to switch on
+        if signal < 8:
+            if value:
+                if cmd == 0b01:
+                    return self.state & ~bit  # make 'or' to switch on
+                else:
+                    return self.state | bit  # make 'or' to switch on
             else:
-                return self.state | bit  # make 'or' to switch on
+                if cmd == 0b01:
+                    return self.state | bit  # make 'and' with negated to switch off
+                else:
+                    return self.state & ~bit  # make 'and' with negated to switch off
         else:
-            if cmd == 0b01:
-                return self.state | bit  # make 'and' with negated to switch off
+            # Unfortunately ISOSPI the commands are swapped
+            if value:
+                if cmd == 0b10:
+                    return self.state & ~bit  # make 'or' to switch on
+                else:
+                    return self.state | bit  # make 'or' to switch on
             else:
-                return self.state & ~bit  # make 'and' with negated to switch off
+                if cmd == 0b10:
+                    return self.state | bit  # make 'and' with negated to switch off
+                else:
+                    return self.state & ~bit  # make 'and' with negated to switch off
 
-    def test_hv_signal_card(self):
+    def test_hv_signal_card(self) -> None:
+        """
+        Function to test all the HV Signal card relays
+        """
         used_ports = list(range(4)) + list(range(16, 32))  # zero based
         self.check_card(6, used_ports)
-
```

### Comparing `pts_fault_injection-0.0.9/pts_fault_injection/CANFWupdate.py` & `pts_fault_injection-0.1.0/pts_fault_injection/CANFWupdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,18 @@
              10: "HV Box Card",
              14: "DAC Board",
              15: "Break Out Box",
              16: "CMB Faults",
              0x20: "BMS DAC",
              0x21: "CMB DAC 1",
              0x22: "CMB DAC 2",
-             0x24: "CMB DAC 3",
-             0x25: "CMB DAC 4",
-             0x26: "CMB DAC 5",
-             0x27: "CMB DAC 6"
+             0x23: "CMB DAC 3",
+             0x24: "CMB DAC 4",
+             0x25: "CMB DAC 5",
+             0x26: "CMB DAC 6"
              }
 
 
 def read_until_Y():
     msg = bus.recv(timeout=2)
     # logger.debug(msg)
     while True:
```

