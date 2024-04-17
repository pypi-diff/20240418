# Comparing `tmp/lazyvpn-0.0.7.tar.gz` & `tmp/lazyvpn-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/yuzhongl/stash/lazyvpn/dist/tmpb955q8nu/lazyvpn-0.0.7.tar", last modified: Thu Mar  4 18:44:02 2021, max compression
+gzip compressed data, was "dist/lazyvpn-0.0.8.tar", last modified: Fri Mar  5 20:01:36 2021, max compression
```

## Comparing `lazyvpn-0.0.7.tar` & `lazyvpn-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yuzhongl   (502) staff       (20)        0 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/
--rw-r--r--   0 yuzhongl   (502) staff       (20)      491 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/PKG-INFO
--rw-r--r--   0 yuzhongl   (502) staff       (20)       59 2021-03-02 00:03:39.000000 lazyvpn-0.0.7/README.md
-drwxr-xr-x   0 yuzhongl   (502) staff       (20)        0 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/bin/
--rwxr-xr-x   0 yuzhongl   (502) staff       (20)      699 2021-03-03 23:38:44.000000 lazyvpn-0.0.7/bin/lazyvpn
--rw-r--r--   0 yuzhongl   (502) staff       (20)     1397 2021-03-03 23:22:10.000000 lazyvpn-0.0.7/bin/lazyvpn.cmd
-drwxr-xr-x   0 yuzhongl   (502) staff       (20)        0 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/lazyvpn/
--rw-r--r--   0 yuzhongl   (502) staff       (20)       39 2021-03-04 18:41:30.000000 lazyvpn-0.0.7/lazyvpn/__init__.py
--rw-r--r--   0 yuzhongl   (502) staff       (20)    10923 2021-03-04 18:39:52.000000 lazyvpn-0.0.7/lazyvpn/config.py
--rw-r--r--   0 yuzhongl   (502) staff       (20)     1726 2021-03-03 04:47:57.000000 lazyvpn-0.0.7/lazyvpn/errors.py
--rw-r--r--   0 yuzhongl   (502) staff       (20)     2444 2021-03-04 18:39:25.000000 lazyvpn-0.0.7/lazyvpn/main.py
--rw-r--r--   0 yuzhongl   (502) staff       (20)     3333 2021-03-03 04:47:57.000000 lazyvpn-0.0.7/lazyvpn/ui.py
-drwxr-xr-x   0 yuzhongl   (502) staff       (20)        0 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/lazyvpn.egg-info/
--rw-r--r--   0 yuzhongl   (502) staff       (20)      491 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/lazyvpn.egg-info/PKG-INFO
--rw-r--r--   0 yuzhongl   (502) staff       (20)      296 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/lazyvpn.egg-info/SOURCES.txt
--rw-r--r--   0 yuzhongl   (502) staff       (20)        1 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/lazyvpn.egg-info/dependency_links.txt
--rw-r--r--   0 yuzhongl   (502) staff       (20)       67 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/lazyvpn.egg-info/requires.txt
--rw-r--r--   0 yuzhongl   (502) staff       (20)        8 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/lazyvpn.egg-info/top_level.txt
--rw-r--r--   0 yuzhongl   (502) staff       (20)       70 2021-03-04 18:44:02.000000 lazyvpn-0.0.7/setup.cfg
--rw-r--r--   0 yuzhongl   (502) staff       (20)      808 2021-03-04 18:43:30.000000 lazyvpn-0.0.7/setup.py
+drwxr-xr-x   0 yuzhongl   (502) staff       (20)        0 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/
+-rw-r--r--   0 yuzhongl   (502) staff       (20)      491 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/PKG-INFO
+-rw-r--r--   0 yuzhongl   (502) staff       (20)      798 2021-03-05 19:50:13.000000 lazyvpn-0.0.8/README.md
+drwxr-xr-x   0 yuzhongl   (502) staff       (20)        0 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/bin/
+-rwxr-xr-x   0 yuzhongl   (502) staff       (20)      699 2021-03-05 19:50:13.000000 lazyvpn-0.0.8/bin/lazyvpn
+-rw-r--r--   0 yuzhongl   (502) staff       (20)     1397 2021-03-05 19:50:13.000000 lazyvpn-0.0.8/bin/lazyvpn.cmd
+drwxr-xr-x   0 yuzhongl   (502) staff       (20)        0 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/lazyvpn/
+-rw-r--r--   0 yuzhongl   (502) staff       (20)       39 2021-03-05 19:56:21.000000 lazyvpn-0.0.8/lazyvpn/__init__.py
+-rw-r--r--   0 yuzhongl   (502) staff       (20)    10990 2021-03-05 19:50:13.000000 lazyvpn-0.0.8/lazyvpn/config.py
+-rw-r--r--   0 yuzhongl   (502) staff       (20)     1726 2021-03-05 19:50:13.000000 lazyvpn-0.0.8/lazyvpn/errors.py
+-rw-r--r--   0 yuzhongl   (502) staff       (20)     2102 2021-03-05 19:50:13.000000 lazyvpn-0.0.8/lazyvpn/main.py
+-rw-r--r--   0 yuzhongl   (502) staff       (20)     3333 2021-03-05 19:50:13.000000 lazyvpn-0.0.8/lazyvpn/ui.py
+drwxr-xr-x   0 yuzhongl   (502) staff       (20)        0 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/lazyvpn.egg-info/
+-rw-r--r--   0 yuzhongl   (502) staff       (20)      491 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/lazyvpn.egg-info/PKG-INFO
+-rw-r--r--   0 yuzhongl   (502) staff       (20)      296 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/lazyvpn.egg-info/SOURCES.txt
+-rw-r--r--   0 yuzhongl   (502) staff       (20)        1 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/lazyvpn.egg-info/dependency_links.txt
+-rw-r--r--   0 yuzhongl   (502) staff       (20)       43 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/lazyvpn.egg-info/requires.txt
+-rw-r--r--   0 yuzhongl   (502) staff       (20)        8 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/lazyvpn.egg-info/top_level.txt
+-rw-r--r--   0 yuzhongl   (502) staff       (20)       70 2021-03-05 20:01:36.000000 lazyvpn-0.0.8/setup.cfg
+-rw-r--r--   0 yuzhongl   (502) staff       (20)      808 2021-03-05 19:50:13.000000 lazyvpn-0.0.8/setup.py
```

### Comparing `lazyvpn-0.0.7/bin/lazyvpn` & `lazyvpn-0.0.8/bin/lazyvpn`

 * *Files identical despite different names*

### Comparing `lazyvpn-0.0.7/bin/lazyvpn.cmd` & `lazyvpn-0.0.8/bin/lazyvpn.cmd`

 * *Files identical despite different names*

### Comparing `lazyvpn-0.0.7/lazyvpn/config.py` & `lazyvpn-0.0.8/lazyvpn/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,33 +49,36 @@
 
         self.conf_profile = 'DEFAULT'
         self.action_configure = False
         self.username = None
         self.company_vpn_region = None
         self.up = False
         self.down = False
+        self.get_args()
 
-        if create_config and not os.path.isfile(self.LAZYVPN_CONFIG):
-            self.ui.notify('No lazy-vpn configuration file found, starting first-time configuration...')
-            self.update_config_file()
+        if self.action_configure or (create_config and not os.path.isfile(self.LAZYVPN_CONFIG)):
+            if self.action_configure:
+                self.update_config_file()
+                raise errors.LazyVpnExitSuccess()
+            else:
+                self.ui.notify('No lazy-vpn configuration file found, starting first-time configuration...')
+                self.update_config_file()
 
     def get_args(self):
         """Get the CLI args"""
         parser = argparse.ArgumentParser(
             description="Create connection to VPN via Okta"
         )
         parser.add_argument('--profile', '-p', help='If set, the specified configuration profile will be used instead of the default.')
         parser.add_argument('--action-configure', '--configure', '-c', action='store_true', help="If set, will prompt user for configuration parameters and then exit.")
         parser.add_argument('--up', '-u', action='store_true', help='connect to vpn')
         parser.add_argument('--down', '-d', action='store_true', help='disconnect from vpn')
         args = parser.parse_args(self.ui.args)
         self.action_configure = args.action_configure
         self.conf_profile = args.profile or 'DEFAULT'
-        if not self.action_configure and args.up == args.down:
-            raise ValueError("Can't have both be UP and DOWN the same value")
         return args
 
     def _handle_config(self, config, profile_config, include_inherits=True):
         if "inherits" in profile_config.keys() and include_inherits:
             self.ui.message("Using inherited config: " + profile_config["inherits"])
             if profile_config["inherits"] not in config:
                 raise errors.LazyVpnError(self.conf_profile + " inherits from " + profile_config["inherits"] + ", but could not find " + profile_config["inherits"])
@@ -135,14 +138,15 @@
         # Prompt user for config details and store in config_dict
         config_dict = defaults
         config_dict['okta_username'] = self._get_okta_username(defaults['okta_username'])
         self.get_okta_password(config_dict['okta_username'])
         config_dict['company_vpn_region'] = self._get_company_vpn_region(DEFAULT_VPN_REGION)
         self.write_config_file(config_dict)
 
+
     def write_config_file(self, config_dict):
         config = configparser.ConfigParser()
         config.read(self.LAZYVPN_CONFIG)
         config[self.conf_profile] = config_dict
         # write out the conf file
         with open(self.LAZYVPN_CONFIG, 'w') as configfile:
             config.write(configfile)
```

### Comparing `lazyvpn-0.0.7/lazyvpn/errors.py` & `lazyvpn-0.0.8/lazyvpn/errors.py`

 * *Files identical despite different names*

### Comparing `lazyvpn-0.0.7/lazyvpn/ui.py` & `lazyvpn-0.0.8/lazyvpn/ui.py`

 * *Files identical despite different names*

### Comparing `lazyvpn-0.0.7/setup.py` & `lazyvpn-0.0.8/setup.py`

 * *Files identical despite different names*

