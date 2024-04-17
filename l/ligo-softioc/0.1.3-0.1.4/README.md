# Comparing `tmp/ligo_softioc-0.1.3.tar.gz` & `tmp/ligo_softioc-0.1.4.tar.gz`

## Comparing `ligo_softioc-0.1.3.tar` & `ligo_softioc-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/setup.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/debian/changelog
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/debian/compat
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/debian/control
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/debian/copyright
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/debian/python3-ligo-softioc.install
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/debian/rules
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/debian/source/format
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/examples/active.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/examples/passive.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/src/ligo_softioc/__init__.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/src/ligo_softioc/alarm.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/src/ligo_softioc/alarm_family.py
--rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/src/ligo_softioc/soft_ioc.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/src/ligo_softioc/sorted_dict.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/src/ligo_softioc/util.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/.gitignore
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/COPYING
--rw-r--r--   0        0        0    35065 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/LICENSE
--rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    10227 2020-02-02 00:00:00.000000 ligo_softioc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/setup.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/examples/active.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/examples/alarm.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/examples/passive.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/examples/rename.py
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/src/print_ini
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/src/ligo_softioc/__init__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/src/ligo_softioc/alarm.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/src/ligo_softioc/alarm_family.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/src/ligo_softioc/load_ioc.py
+-rw-r--r--   0        0        0    22599 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/src/ligo_softioc/soft_ioc.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/src/ligo_softioc/sorted_dict.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/src/ligo_softioc/util.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/tests/test_load_ioc.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/COPYING
+-rw-r--r--   0        0        0    35065 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/LICENSE
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 ligo_softioc-0.1.4/PKG-INFO
```

### Comparing `ligo_softioc-0.1.3/examples/active.py` & `ligo_softioc-0.1.4/examples/active.py`

 * *Files 19% similar despite different names*

```diff
@@ -45,22 +45,24 @@
 
     # square INPUT and write it to SQUARED_OUTPUT
     ioc.setParam("SQUARED_OUTPUT", in_val ** 2)
 
     # set to how many times process() has run
     ioc.setParam("PROCESS_COUNT", process_count)
 
-if __name__ == "__main__":
 
-    # pass '-i' as the first command line argument
-    # to print the ini file rather than run the IOC.
-    if len(sys.argv) > 1 and sys.argv[1] == '-i':
-        print_ini = True
-    else:
-        print_ini = False
+def build_ioc() -> SoftIOC:
+    """
+    Build a new SoftIOC that's completely ready to run
+
+    Separate the ioc build from 'if __name__ == "__main__"'
+    so that halper scripts can load the IOC and create the object
+    to interrogate it.
+    :return:
+    """
 
     # setup the ioc with a channel prefix.
     # the ioc will by default run process() about 10 times per second
     ioc = SoftIOC(
         prefix="X1:IOC-",
         process_func=process)
 
@@ -78,12 +80,15 @@
     # call this when all channels are added.
     # and before you try to set the value of any channel
     ioc.finalize_channels()
 
     # setup the input varible so we know how it'll start
     ioc.setParam("INPUT", 0)
 
-    # start the ioc or print the ini file and exit
-    if print_ini:
-        ioc.print_ini()
-    else:
-        ioc.start()
+    return ioc
+
+
+if __name__ == "__main__":
+
+    ioc = build_ioc()
+
+    ioc.start()
```

### Comparing `ligo_softioc-0.1.3/examples/passive.py` & `ligo_softioc-0.1.4/examples/passive.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
   X1:SYS-EXAMPLE_SINCE_LAST_PROCESS_SEC
   X1:SYS-EXAMPLE_SINCE_LAST_PROCESS_STR
   X1:SYS-EXAMPLE_SERVER_RUNNING
 """
 
 from ligo_softioc import SoftIOC
 
-if __name__ == "__main__":
+def build_ioc():
     # Setup the IOC with a channel prefix.
     # set `separate_server` to true to make this a passive IOC
     ioc = SoftIOC(
         prefix="X1:SYS-EXAMPLE_",
         separate_server=True
     )
 
@@ -66,15 +66,19 @@
     # call before pre-setting any channels
     ioc.finalize_channels()
 
     # some some preliminary values to channels
     ioc.setParam("FIRST_CHANNEL_STR", "N/A")
     ioc.setParam("SECOND_CHANNEL", -1.0)
     ioc.setParam("ANOTHER_CHANNEL", -1)
+    return ioc
+
+if __name__ == "__main__":
+
+    ioc = build_ioc()
 
-    # that's it.  start the IOC.
     ioc.start()
```

### Comparing `ligo_softioc-0.1.3/src/ligo_softioc/alarm.py` & `ligo_softioc-0.1.4/src/ligo_softioc/alarm.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.3/src/ligo_softioc/alarm_family.py` & `ligo_softioc-0.1.4/src/ligo_softioc/alarm_family.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.3/src/ligo_softioc/soft_ioc.py` & `ligo_softioc-0.1.4/src/ligo_softioc/soft_ioc.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,70 +7,127 @@
 from socket import gethostname
 import time
 from configparser import ConfigParser
 
 from gpstime import gpsnow, gpstime
 from pcaspy import Driver, SimpleServer
 
-from typing import Dict, Union, Callable, Optional, Set
+from typing import Dict, Union, Callable, Optional, Set, Any, List
 import pcaspy
 from .alarm import Alarm, AlarmGroup
 from .alarm_family import  AlarmFamily
 from .sorted_dict import  SortedDict
 
 
 from .util import gps_to_str, delta_seconds_to_readable, PyIOCError
 
 PREFIX_REGEX = re.compile(r"[A-Z0-9]{2}:[A-Z]{3}-([A-Z0-9]+_)+")
 PREFIX_LIMIT = 40
 SUBPREFIX_REGEX=re.compile(r"([A-Z0-9]+_)*")
 SUFFIX_REGEX=re.compile(r"([A-Z0-9]+_)*[A-Z0-9]+")
 
+DEFAULT_IOC_CHANNELS = ("GPS UPTIME_SEC START_GPS TIMESTAMP START_TIMESTAMP UPTIME_STR HOSTNAME PROCESS " +
+ "ERROR_GPS ERROR_MESSAGE ERROR_TIMESTAMP").split()
+
+IOC_CHANNELS = {
+            "START_GPS": {'type': 'int'},
+            "GPS": {'type': 'int'},
+            "TIMESTAMP": {'type': 'str'},
+            "START_TIMESTAMP": {'type': 'str'},
+            "UPTIME_SEC": {'type': 'int'},
+            "UPTIME_STR": {'type': 'str'},
+            "HOSTNAME": {'type': 'str'},
+            "PROCESS": {'type': 'str'},
+            "ERROR_MESSAGE": {'type': 'str'},
+            "ERROR_GPS": {'type': 'int'},
+            "ERROR_TIMESTAMP": {'type': 'str'},
+}
+
+SERVER_CHANNELS = {
+       "SERVER_START_GPS" : {'type': 'int'},
+       "SERVER_GPS" : {'type': 'int'},
+       "SERVER_START_TIMESTAMP" : {'type': 'str'},
+       "SERVER_UPTIME_SEC" : {'type': 'int'},
+       "SERVER_UPTIME_STR" : {'type': 'str'},
+       "LAST_PROCESS_GPS" : {'type': 'int'},
+       "LAST_PROCESS_TIMESTAMP" : {'type': 'str'},
+       "SINCE_LAST_PROCESS_SEC" : {'type': 'int'},
+       "SINCE_LAST_PROCESS_STR" : {'type': 'str'},
+       "SERVER_RUNNING" : {'type': 'int'},
+}
 
 class SoftIOC(Driver):
     def __init__(self, prefix: str, ioc_chan_prefix: str = "", separate_server=False, server_timeout_sec: int = 60,
                  process_period_sec: float = 0.1,
                  process_func: Optional[Callable] = None,
                  process_func_period_sec: float = 0.1,
-                 gps_name: str = "GPS",
-                 uptime_name: str = "UPTIME_SEC"
+                 custom_channel_names: Optional[Dict[str, str]] = None,
                  ):
         """
         Create EPICS soft IOC with standard LIGO channels
         :param prefix:  channel prefix for EPICS channels, e.g. 'X1:ABC-DEFG_HIJK123_'
         :param ioc_chan_prefix: additional prefix to add to IOC status channels.  Sometimes useful to differentiate from
+        other channels, e.g. "IOC_"
         :param separate_server: set to True if the channels are actually written from another application
+        creates some useful tracking channels for the application
         :param server_timeout_sec: Number of seconds to wait for update from a server before declaring it has failed
         :param process_period_sec: time between process cycles for the iop
         :param process_func_period_sec: time between calls to process_func.  Can't be less than process_period_sec
         :param process_func: Called from the process routine of the IOC with the driver and now_gps as the
         first two arguments.
-        creates some useful tracking channels for the application
-        other channels, e.g. "IOC_"
+        :param channel_renames: A dictionary of IOC channel default names to use names.  {"GPS": "GPS_SEC"} will change
+        the GPS channel to GPS_SEC.
+
+
         """
-        global PREFIX_REGEX, PREFIX_LIMIT, SUBPREFIX_REGEX
+        global PREFIX_REGEX, PREFIX_LIMIT, SUBPREFIX_REGEX, IOC_CHANNELS
 
 
         if not PREFIX_REGEX.match(prefix):
             logging.warning(f"prefix is not in standard format: should be: 'X1:ABC-DEFG_HIJK123_'")
         if len(prefix) > PREFIX_LIMIT:
             logging.warning(f"prefix is too big.  prefix should be 40 characters or less.")
         self.prefix = prefix
         if not SUBPREFIX_REGEX.match(ioc_chan_prefix):
             logging.warning(f"io_chan_prefix not in standard formate: should be as 'IOC_'")
         if len(prefix) + len(ioc_chan_prefix) > PREFIX_LIMIT:
             logging.warning(f"prefix + io_chan_prefix is too big.  prefix should be 40 characters or less.")
         self.ioc_chan_prefix = ioc_chan_prefix
 
         # custom channel names
-        self.gps_name = gps_name
-        self.uptime_name = uptime_name
+        if custom_channel_names is None:
+            self.custom_channel_names = {}
+        else:
+            self.custom_channel_names  = custom_channel_names
+
+        ###  various useful channel sets to be populated later
 
+        # all the channels and their definitions
         self.channels: Dict[str, Dict] = {}
+
+        # channels that should be included in the ini file
         self.ini_channels: Set[str] = set()
+
+        # alarm channels
+        self.alarm_channels: Dict[str, Set[str]] = {}
+
+        # all channels added by the owning application
+        self.application_channels: Set[str] = set()
+
+        # add IOC prefix
+        if ioc_chan_prefix != "":
+            for chan in IOC_CHANNELS.keys():
+                if chan in self.custom_channel_names:
+                    base_val = self.custom_channel_names[chan]
+                else:
+                    base_val = chan
+                self.custom_channel_names[chan] = ioc_chan_prefix + base_val
+
+        self.check_double_customization()
+
         self._add_default_channels()
         self.separate_server = separate_server
         if separate_server:
             self._add_server_channels()
 
         self.alarm_families: Set[AlarmFamily] = set([])
         self.alarm_groups: Set[AlarmGroup] = set([])
@@ -83,52 +140,66 @@
         self.process_func_period_sec = process_func_period_sec
         self.epics_server = SimpleServer()
 
         self.are_channels_finalize = False
 
         self.finalization_started = False
 
+    def check_double_customization(self):
+        for k, v in self.custom_channel_names.items():
+            if v in self.custom_channel_names.keys():
+                raise ValueError(f"Double channel customization not allowed. {k} => {v} => {self.custom_channel_names[v]}.")
+
+    def get_real_chan_name(self, chan: str) -> str:
+        """
+        Return the real channel name, which may be different
+        if the names have been customized or if ioc_prefix is not empty
+        :param chan:
+        :return:
+        """
+        return self.custom_channel_names.get(chan, chan)
+
+    def get_full_chan_name(self, chan: str) -> str:
+        """
+        Get the full, correct channel name including prefix
+        :param chan:
+        :return:
+        """
+        return self.prefix + self.get_real_chan_name(chan)
+
     def start(self):
 
         if not self.are_channels_finalize:
             raise PyIOCError("call finalize_channels() on the IOC before starting")
 
-
-
         self._initialize_defaults()
         if self.separate_server:
             self._initialize_server_channels()
 
         self.process_thread = threading.Thread(target=self._process)
         self.process_thread.setDaemon(True)
         self.process_thread.start()
 
         while True:
             self.epics_server.process(self.process_period_sec)
 
     def _add_default_channels(self) -> None:
-        def_chans: Dict[str, Dict] = {
-            "START_GPS": {'type': 'int'},
-            self.gps_name: {'type': 'int'},
-            "TIMESTAMP": {'type': 'str'},
-            "START_TIMESTAMP": {'type': 'str'},
-            self.uptime_name: {'type': 'int'},
-            "UPTIME_STR": {'type': 'str'},
-            "HOSTNAME": {'type': 'str'},
-            "PROCESS": {'type': 'str'},
-            "ERROR_MESSAGE": {'type': 'str'},
-            "ERROR_GPS": {'type': 'int'},
-            "ERROR_TIMESTAMP": {'type': 'str'},
-        }
-        for k, v in def_chans.items():
-            self.channels[self.ioc_chan_prefix + k] = v
-
-        self.ini_channels.add(self.ioc_chan_prefix + self.gps_name)
-        self.ini_channels.add(self.ioc_chan_prefix + self.uptime_name)
-        self.ini_channels.add(self.ioc_chan_prefix + "START_GPS")
+        global IOC_CHANNELS
+
+        self._add_real_channels(IOC_CHANNELS)
+
+        self.ini_channels.add("GPS")
+        self.ini_channels.add("UPTIME_SEC")
+        self.ini_channels.add("START_GPS")
+
+    def setParam(self, chan, value):
+        super().setParam(self.get_real_chan_name(chan), value)
+
+    def getParam(self, chan) -> Any:
+        return super().getParam(self.get_real_chan_name(chan))
 
     def set_error_message(self, error_message: str) -> None:
         """
         Sets the error message and timestamp.
         Updates PVs immediately because maybe we are about to throw an exception.
         :param error_message:
         :return:
@@ -136,55 +207,72 @@
         now_gps = gpsnow()
         self.setParam("ERROR_MESSAGE", error_message)
         self.setParam("ERROR_GPS", now_gps)
         self.setParam("ERROR_TIMESTAMP", gps_to_str(now_gps))
         self.updatePVs()
 
     def _add_server_channels(self) -> None:
-        self.channels["SERVER_START_GPS"] = {'type': 'int'}
-        self.channels["SERVER_GPS"] = {'type': 'int'}
-        self.channels["SERVER_START_TIMESTAMP"] = {'type': 'str'}
-        self.channels["SERVER_UPTIME_SEC"] = {'type': 'str'}
-        self.channels["SERVER_UPTIME_STR"] = {'type': 'str'}
-        self.channels["LAST_PROCESS_GPS"] = {'type': 'int'}
-        self.channels["LAST_PROCESS_TIMESTAMP"] = {'type': 'str'}
-        self.channels["SINCE_LAST_PROCESS_SEC"] = {'type': 'int'}
-        self.channels["SINCE_LAST_PROCESS_STR"] = {'type': 'str'}
-        self.channels["SERVER_RUNNING"] = {'type': 'int'}
+        global SERVER_CHANNELS
+
+        self._add_real_channels(SERVER_CHANNELS)
 
         self.ini_channels.add("SERVER_GPS")
         self.ini_channels.add("SERVER_UPTIME_SEC")
         self.ini_channels.add("LAST_PROCESS_GPS")
         self.ini_channels.add("SINCE_LAST_PROCESS_SEC")
         self.ini_channels.add("SERVER_START_GPS")
         self.ini_channels.add("SERVER_RUNNING")
 
-    def add_channels(self, chans: Dict[str, Dict]) -> None:
+    def _add_real_channel(self, channel: str, channel_def: Dict):
+        """
+        Add a single channel, but make sure to use the real channel name
+        :param channel:
+        :param channel_def:
+        :return:
+        """
+        self._add_real_channels(
+            {channel:  channel_def}
+        )
+
+    def _add_real_channels(self, channels: Dict[str, Dict]):
+        """
+        Add channels, but make sure we've got the real names
+        :param channels:
+        :return:
+        """
+        self._add_channels({self.get_real_chan_name(k): v for k,v in channels.items()})
+
+    def _add_channels(self, chans: Dict[str, Dict]) -> None:
         """
         Add a dictionary of channel-names: epics chan defs
         self.prefix is added to the front of the channel names
         :param chans: Dictionary of channel-name : EPICs channel definition (definition is also a dictionary)
         :return:
         """
         global SUFFIX_REGEX
         for k, v in chans.items():
             if k in self.channels:
                 logging.warning(f"adding channel {v}, but it already was added")
             if not SUFFIX_REGEX.match(k):
                 logging.warning(f"{k} is not a standard channel name")
             self.channels[k] = v
 
-            # add any custom channel that's not a string to the INI file
-            if 'type' not in v or v['type'] != 'str':
-                if not self.finalization_started:
-                    self.ini_channels.add(k)
+    def add_channels(self, chans: Dict[str, Dict]) -> None:
+        """
+        Public function that adds channels but also records them as application channels.
+        :param chans:
+        :return:
+        """
+        self._add_channels(chans)
+        for chan in chans.keys():
+            self.application_channels.add(chan)
 
     def add_channel(self, channel: str, channel_def: Dict) -> None:
         """
-        Add a single channel
+        Add a single channel.
         :param channel: The channel name.  self.prefix is prepended.
         :param channel_def: The channel definition.  A dicitionary in th pcaspy style.
         :return:
         """
         self.add_channels({channel: channel_def})
 
     def add(self, item: Union[Alarm, AlarmGroup, AlarmFamily]) -> None:
@@ -244,64 +332,91 @@
                 raise PyIOCError(msg)
         for ag in self.alarm_groups:
             fam_membership = [ag in f for f in self.alarm_families]
             if not any(fam_membership):
                 msg = (f"alarm group '{ag.name}' not found in any AlarmFamily added to the driver")
                 raise PyIOCError(msg)
 
+    def bulk_ini_add(self, channels: Set[str]):
+        usable_chans = set()
+        for c in channels:
+            real_c = self.get_real_chan_name(c)
+            chan_def = self.channels[real_c]
+            if 'type' not in chan_def or chan_def['type'] != 'str':
+                usable_chans.add(c)
+
+        self.ini_channels = self.ini_channels.union(usable_chans)
+
     def finalize_channels(self) -> None:
         self.finalization_started = True
         self._finalize_alarms()
         for af in self.alarm_families:
-            self.add_channels(af.get_channels())
-            self.ini_channels = self.ini_channels.union(af.get_ini_channels())
+            channels = af.get_channels()
+            self.ini_channels.add(f"{af.name.upper()}_GPS_TIME")
+
+            self._add_real_channels(channels)
+            self.alarm_channels[af.name] = set(channels.keys())
+
+        self.bulk_ini_add(self.application_channels)
+
+        self.check_unused_custom_channels()
         self.are_channels_finalize = True
 
         self.epics_server.createPV(self.prefix, self.channels)
         super(SoftIOC, self).__init__()
 
+    def check_unused_custom_channels(self):
+        """
+        Check if any custom channel names were never used.
+        If so, it's probably a typo.
+        :return:
+        """
+        for k, v in self.custom_channel_names.items():
+            if v not in self.channels:
+                logging.warning(f"custom channel mapping '{k}' => '{v}' was never used")
+
     def _process_uptime(self, now_gps: int) -> None:
         """
         Update values of some of the default channels
         :param now_gps:
         :return:
         """
 
         uptime_sec = int(now_gps - self.start_gps)
-        self.setParam(self.ioc_chan_prefix + self.uptime_name, uptime_sec)
-        self.setParam(self.ioc_chan_prefix + "UPTIME_STR", delta_seconds_to_readable(uptime_sec))
+        self.setParam("UPTIME_SEC", uptime_sec)
+        self.setParam("UPTIME_STR", delta_seconds_to_readable(uptime_sec))
 
     def _process_gpstime(self, now_gps: int) -> None:
         """
         Handle GPS channels
         :param now_gps:
         :return:
         """
-        self.setParam(self.ioc_chan_prefix + self.gps_name, now_gps)
-        self.setParam(self.ioc_chan_prefix + "TIMESTAMP", gps_to_str(now_gps))
+        self.setParam("GPS", now_gps)
+        self.setParam("TIMESTAMP", gps_to_str(now_gps))
 
     def _initialize_defaults(self) -> None:
         """
         Initialize some of the values of the default channels.
         Should be run once when the IOC is started.
         :param driver:
         :return:
         """
         self.start_gps = gpsnow()
-        self.setParam(self.ioc_chan_prefix + "START_GPS", self.start_gps)
-        self.setParam(self.ioc_chan_prefix + "START_TIMESTAMP", gps_to_str(self.start_gps))
-        self.setParam(self.ioc_chan_prefix + "HOSTNAME", gethostname())
+        self.setParam("START_GPS", self.start_gps)
+        self.setParam("START_TIMESTAMP", gps_to_str(self.start_gps))
+        self.setParam("HOSTNAME", gethostname())
 
         # try to guess if we're running from systemd
         systemd_key = "INVOCATION_ID"
         if (systemd_key in os.environ) and (len(os.environ[systemd_key]) > 0):
             ioc_process = "systemd"
         else:
             ioc_process = "unknown"
-        self.setParam(self.ioc_chan_prefix + "PROCESS", ioc_process)
+        self.setParam("PROCESS", ioc_process)
 
     def _process_server_channels(self, now_gps) -> None:
         """
         Call once per update to update the separate server channels
         Call only if there is a separate server
         :param driver:
         :param now_gps:
@@ -390,18 +505,19 @@
 
     def chan_to_type(self, chan: str) -> int:
         """
         Return the DAQ type number for the given channel name
         :param chan:
         :return:
         """
-        if 'type' not in self.channels[chan]:
+        real_chan = self.get_real_chan_name(chan)
+        if 'type' not in self.channels[real_chan]:
             t = 'float'
         else:
-            t = self.channels[chan]['type']
+            t = self.channels[real_chan]['type']
         if t == 'float':
             return 4
         elif t == 'double':
             return 5
         elif t == 'int':
             return 2
         elif t == 'uint':
@@ -430,15 +546,69 @@
         :return:
         """
         cfp = ConfigParser(dict_type=SortedDict)
 
         chans = list(self.ini_channels)
         chans.sort()
         for chan in self.ini_channels:
-            fullname = f"{self.prefix}{chan}"
+            fullname = self.get_full_chan_name(chan)
             cfp.add_section(fullname)
             cfp[fullname]['datatype'] = str(self.chan_to_type(chan))
         cfp.write(fstream)
 
     def print_ini(self):
         self.write_ini(sys.stdout)
 
+    def get_ioc_channels(self) -> List[str]:
+        """
+        Get full channel names for all standard IOC channels in alphabetical order
+        :return:
+        """
+        global IOC_CHANNELS
+        chans = [self.get_full_chan_name(c) for c in IOC_CHANNELS.keys()]
+        chans.sort()
+        return chans
+
+    def get_server_channels(self) -> List[str]:
+        """
+        Get full channel names for all standard external server channels in alphabetical order
+        This list is empty if the 'separate_server' flag was false when the SoftIOC was created.
+        :return:
+        """
+        global SERVER_CHANNELS
+        chans = [self.get_full_chan_name(c) for c in SERVER_CHANNELS.keys()]
+        chans.sort()
+        return chans
+
+    def get_alarm_families(self) -> List[str]:
+        """
+        Return an alphabetical list of alarm families
+        :return:
+        """
+        fams = list(self.alarm_channels.keys())
+        fams.sort()
+        return fams
+
+    def get_alarm_channels(self, family: str) -> List[str]:
+        """
+        Return an alphabetical list of channels for a particular alarm family
+        :param family: 
+        :return: 
+        """
+        chans = [self.get_full_chan_name(c) for c in self.alarm_channels[family]]
+        chans.sort()
+        return chans
+
+    def get_application_channels(self) -> List[str]:
+        chans = [self.get_full_chan_name(c) for c in self.application_channels]
+        chans.sort()
+        return chans
+
+    def get_ini_channels(self) -> List[str]:
+        chans = [self.get_full_chan_name(c) for c in self.ini_channels]
+        chans.sort()
+        return chans
+
+    def get_all_channels(self) -> List[str]:
+        chans = [self.get_full_chan_name(c) for c in self.channels.keys()]
+        chans.sort()
+        return chans
```

### Comparing `ligo_softioc-0.1.3/src/ligo_softioc/sorted_dict.py` & `ligo_softioc-0.1.4/src/ligo_softioc/sorted_dict.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.3/src/ligo_softioc/util.py` & `ligo_softioc-0.1.4/src/ligo_softioc/util.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.3/COPYING` & `ligo_softioc-0.1.4/COPYING`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.3/LICENSE` & `ligo_softioc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.3/README.md` & `ligo_softioc-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 This example IOC, also in `examples/active.py`, read an input dchannel and squares it, writing the result to an output channel.
 
 It also reports the number of times the IOC process function has been run.
 
 ```
 from ligo_softioc import SoftIOC
-
+import sys
 
 process_count = 0
 
 def process(ioc: SoftIOC, gps_time_sec: int) -> None:
     """
     Update the custom channels.
 
@@ -40,15 +40,25 @@
 
     # square INPUT and write it to SQUARED_OUTPUT
     ioc.setParam("SQUARED_OUTPUT", in_val ** 2)
 
     # set to how many times process() has run
     ioc.setParam("PROCESS_COUNT", process_count)
 
-if __name__ == "__main__":
+
+def build_ioc() -> SoftIOC:
+    """
+    Build a new SoftIOC that's completely ready to run
+
+    Separate the ioc build from 'if __name__ == "__main__"'
+    so that halper scripts can load the IOC and create the object
+    to interrogate it.
+    :return:
+    """
+
     # setup the ioc with a channel prefix.
     # the ioc will by default run process() about 10 times per second
     ioc = SoftIOC(
         prefix="X1:IOC-",
         process_func=process)
 
     # add in some channels
@@ -65,17 +75,53 @@
     # call this when all channels are added.
     # and before you try to set the value of any channel
     ioc.finalize_channels()
 
     # setup the input varible so we know how it'll start
     ioc.setParam("INPUT", 0)
 
-    # start the ioc
+    return ioc
+
+
+if __name__ == "__main__":
+
+    ioc = build_ioc()
+
     ioc.start()
+
+```
+
+## build_ioc function
+
+The SoftIOC object should be built in a function called 'build_ioc'.  
+This function should return the SoftIOC object.
+
+The 'build_ioc' function is necessary to run helper scripts like 'softioc_print_ini'.
+Such scripts will call the build_ioc function to get the SoftIOC object for introspection.
+
+Any arguments to the 'build_ioc' function should be type annoted.
+
+Pass build_ioc arguments on the command line to the helper scripts after a '--' argument.
+
+For example, if build_ioc is defined as 
+
 ```
+def build_ioc(foo: int, bar: str):
+    ...
+```
+
+Then 'print_ini' is called as
+
+```
+print_ini ioc.py -- 123 abc
+```
+
+Then the command line arguments `['123', 'abc']` will be converted to `[123, 'abc']`
+and passed to build_ioc().
+
 
 ## Auto-generated channels
 The following channels are autogenerated. The values are also set automatically.
 
 These channels use the normal prefix, but the prefix can be lengthened with
 an optional parameter to SoftIOC.
 
@@ -172,27 +218,14 @@
 SERVER_RUNNING
 : A value that indicates if the server has run recnetly
 0 - Invalid state.  SINCE_LAST_PROCESS_SEC is negative.
 1 - Running.  SINCE_LAST_PROCESS_SEC is less than or equal to the maximum allowed, default 60 seconds.
 2 - Stalled.  SINCE_LAST_PROCESS_SEC is greater than the maximum allowed.
 Set automatically by SoftIOC.
 
-
-## Printing an INI file.
-
-Add in all channels, call `finalize_channels()` on the SoftIOC, then call `print_ini()` on the SoftIOC.
-
-Send to std output, one line per name in alphabetical order, each surrounded by square brackets:
-
-- All custom channels that aren't strings.
-- From the automatic channels: START_GPS, GPS, UPTIME_SEC,
-- If separate_server == True,
-SERVER_START_GPS, SERVER_GPS, SERVER_UPTIME_SEC, LAST_PROCESS_GPS, SINCE_LAST_PROCESS_SEC, SERVER_RUNNING,
-- If there are any alarm families, print the GPS_TIME channel on the alarm family.
-
 ## Alarms
 
 Alarms can be optionally added to the SoftIOC.
 
 Create an alarm object, then add it to the soft IOC before calling `finalize_channels()`.
 
 ```
```

### Comparing `ligo_softioc-0.1.3/pyproject.toml` & `ligo_softioc-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.3/PKG-INFO` & `ligo_softioc-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ligo-softioc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Support library for writing EPICS SoftIOCs in Python.
 Project-URL: Homepage, https://git.ligo.org/cds/admin/softioc
 Project-URL: Issues, https://git.ligo.org/cds/admin/softioc/-/issues
 Author-email: Erik von Reis <evonreis@caltech.edu>
 License-File: COPYING
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -32,15 +32,15 @@
 
 This example IOC, also in `examples/active.py`, read an input dchannel and squares it, writing the result to an output channel.
 
 It also reports the number of times the IOC process function has been run.
 
 ```
 from ligo_softioc import SoftIOC
-
+import sys
 
 process_count = 0
 
 def process(ioc: SoftIOC, gps_time_sec: int) -> None:
     """
     Update the custom channels.
 
@@ -57,15 +57,25 @@
 
     # square INPUT and write it to SQUARED_OUTPUT
     ioc.setParam("SQUARED_OUTPUT", in_val ** 2)
 
     # set to how many times process() has run
     ioc.setParam("PROCESS_COUNT", process_count)
 
-if __name__ == "__main__":
+
+def build_ioc() -> SoftIOC:
+    """
+    Build a new SoftIOC that's completely ready to run
+
+    Separate the ioc build from 'if __name__ == "__main__"'
+    so that halper scripts can load the IOC and create the object
+    to interrogate it.
+    :return:
+    """
+
     # setup the ioc with a channel prefix.
     # the ioc will by default run process() about 10 times per second
     ioc = SoftIOC(
         prefix="X1:IOC-",
         process_func=process)
 
     # add in some channels
@@ -82,17 +92,53 @@
     # call this when all channels are added.
     # and before you try to set the value of any channel
     ioc.finalize_channels()
 
     # setup the input varible so we know how it'll start
     ioc.setParam("INPUT", 0)
 
-    # start the ioc
+    return ioc
+
+
+if __name__ == "__main__":
+
+    ioc = build_ioc()
+
     ioc.start()
+
+```
+
+## build_ioc function
+
+The SoftIOC object should be built in a function called 'build_ioc'.  
+This function should return the SoftIOC object.
+
+The 'build_ioc' function is necessary to run helper scripts like 'softioc_print_ini'.
+Such scripts will call the build_ioc function to get the SoftIOC object for introspection.
+
+Any arguments to the 'build_ioc' function should be type annoted.
+
+Pass build_ioc arguments on the command line to the helper scripts after a '--' argument.
+
+For example, if build_ioc is defined as 
+
 ```
+def build_ioc(foo: int, bar: str):
+    ...
+```
+
+Then 'print_ini' is called as
+
+```
+print_ini ioc.py -- 123 abc
+```
+
+Then the command line arguments `['123', 'abc']` will be converted to `[123, 'abc']`
+and passed to build_ioc().
+
 
 ## Auto-generated channels
 The following channels are autogenerated. The values are also set automatically.
 
 These channels use the normal prefix, but the prefix can be lengthened with
 an optional parameter to SoftIOC.
 
@@ -189,27 +235,14 @@
 SERVER_RUNNING
 : A value that indicates if the server has run recnetly
 0 - Invalid state.  SINCE_LAST_PROCESS_SEC is negative.
 1 - Running.  SINCE_LAST_PROCESS_SEC is less than or equal to the maximum allowed, default 60 seconds.
 2 - Stalled.  SINCE_LAST_PROCESS_SEC is greater than the maximum allowed.
 Set automatically by SoftIOC.
 
-
-## Printing an INI file.
-
-Add in all channels, call `finalize_channels()` on the SoftIOC, then call `print_ini()` on the SoftIOC.
-
-Send to std output, one line per name in alphabetical order, each surrounded by square brackets:
-
-- All custom channels that aren't strings.
-- From the automatic channels: START_GPS, GPS, UPTIME_SEC,
-- If separate_server == True,
-SERVER_START_GPS, SERVER_GPS, SERVER_UPTIME_SEC, LAST_PROCESS_GPS, SINCE_LAST_PROCESS_SEC, SERVER_RUNNING,
-- If there are any alarm families, print the GPS_TIME channel on the alarm family.
-
 ## Alarms
 
 Alarms can be optionally added to the SoftIOC.
 
 Create an alarm object, then add it to the soft IOC before calling `finalize_channels()`.
 
 ```
```

