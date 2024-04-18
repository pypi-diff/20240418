# Comparing `tmp/mantis-cli-9.0.4.tar.gz` & `tmp/mantis-cli-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mantis-cli-9.0.4.tar", last modified: Thu Dec 21 11:52:14 2023, max compression
+gzip compressed data, was "mantis-cli-9.1.0.tar", last modified: Sat Dec 30 20:05:16 2023, max compression
```

## Comparing `mantis-cli-9.0.4.tar` & `mantis-cli-9.1.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 erik       (502) staff       (20)        0 2023-12-21 11:52:14.411713 mantis-cli-9.0.4/
--rw-r--r--   0 erik       (502) staff       (20)     1265 2021-04-10 10:14:46.000000 mantis-cli-9.0.4/.gitignore
--rw-r--r--   0 erik       (502) staff       (20)    35147 2021-04-10 10:14:46.000000 mantis-cli-9.0.4/LICENSE
--rw-r--r--   0 erik       (502) staff       (20)       17 2021-04-10 10:14:46.000000 mantis-cli-9.0.4/MANIFEST.in
--rw-r--r--   0 erik       (502) staff       (20)      797 2023-12-21 11:52:14.411784 mantis-cli-9.0.4/PKG-INFO
--rw-r--r--   0 erik       (502) staff       (20)       12 2021-04-10 10:14:46.000000 mantis-cli-9.0.4/README.md
--rw-r--r--   0 erik       (502) staff       (20)      251 2022-07-13 13:47:25.000000 mantis-cli-9.0.4/TODO
-drwxr-xr-x   0 erik       (502) staff       (20)        0 2023-12-21 11:52:14.410504 mantis-cli-9.0.4/mantis/
--rw-r--r--   0 erik       (502) staff       (20)       18 2023-12-21 11:50:58.000000 mantis-cli-9.0.4/mantis/__init__.py
--rw-r--r--   0 erik       (502) staff       (20)       69 2023-08-22 16:40:23.000000 mantis-cli-9.0.4/mantis/__main__.py
--rw-r--r--   0 erik       (502) staff       (20)       76 2023-08-22 16:40:23.000000 mantis-cli-9.0.4/mantis/command_line.py
--rw-r--r--   0 erik       (502) staff       (20)     3862 2023-12-19 14:11:49.000000 mantis-cli-9.0.4/mantis/extensions.py
--rw-r--r--   0 erik       (502) staff       (20)     3524 2023-10-26 10:08:40.000000 mantis-cli-9.0.4/mantis/helpers.py
--rw-r--r--   0 erik       (502) staff       (20)     6030 2023-12-21 10:31:22.000000 mantis-cli-9.0.4/mantis/logic.py
--rw-r--r--   0 erik       (502) staff       (20)    34863 2023-12-21 11:49:46.000000 mantis-cli-9.0.4/mantis/managers.py
-drwxr-xr-x   0 erik       (502) staff       (20)        0 2023-12-21 11:52:14.411622 mantis-cli-9.0.4/mantis_cli.egg-info/
--rw-r--r--   0 erik       (502) staff       (20)      797 2023-12-21 11:52:14.000000 mantis-cli-9.0.4/mantis_cli.egg-info/PKG-INFO
--rw-r--r--   0 erik       (502) staff       (20)      372 2023-12-21 11:52:14.000000 mantis-cli-9.0.4/mantis_cli.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (502) staff       (20)        1 2023-12-21 11:52:14.000000 mantis-cli-9.0.4/mantis_cli.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (502) staff       (20)       52 2023-12-21 11:52:14.000000 mantis-cli-9.0.4/mantis_cli.egg-info/entry_points.txt
--rw-r--r--   0 erik       (502) staff       (20)        7 2023-12-21 11:52:14.000000 mantis-cli-9.0.4/mantis_cli.egg-info/top_level.txt
--rw-r--r--   0 erik       (502) staff       (20)       79 2023-12-21 11:52:14.411978 mantis-cli-9.0.4/setup.cfg
--rw-r--r--   0 erik       (502) staff       (20)     1132 2021-12-22 06:51:20.000000 mantis-cli-9.0.4/setup.py
+drwxr-xr-x   0 erik       (502) staff       (20)        0 2023-12-30 20:05:16.722827 mantis-cli-9.1.0/
+-rw-r--r--   0 erik       (502) staff       (20)     1265 2021-04-10 10:14:46.000000 mantis-cli-9.1.0/.gitignore
+-rw-r--r--   0 erik       (502) staff       (20)    35147 2021-04-10 10:14:46.000000 mantis-cli-9.1.0/LICENSE
+-rw-r--r--   0 erik       (502) staff       (20)       17 2021-04-10 10:14:46.000000 mantis-cli-9.1.0/MANIFEST.in
+-rw-r--r--   0 erik       (502) staff       (20)      797 2023-12-30 20:05:16.722889 mantis-cli-9.1.0/PKG-INFO
+-rw-r--r--   0 erik       (502) staff       (20)       12 2021-04-10 10:14:46.000000 mantis-cli-9.1.0/README.md
+-rw-r--r--   0 erik       (502) staff       (20)      251 2022-07-13 13:47:25.000000 mantis-cli-9.1.0/TODO
+drwxr-xr-x   0 erik       (502) staff       (20)        0 2023-12-30 20:05:16.721885 mantis-cli-9.1.0/mantis/
+-rw-r--r--   0 erik       (502) staff       (20)       18 2023-12-30 19:54:19.000000 mantis-cli-9.1.0/mantis/__init__.py
+-rw-r--r--   0 erik       (502) staff       (20)       69 2023-08-22 16:40:23.000000 mantis-cli-9.1.0/mantis/__main__.py
+-rw-r--r--   0 erik       (502) staff       (20)       76 2023-08-22 16:40:23.000000 mantis-cli-9.1.0/mantis/command_line.py
+-rw-r--r--   0 erik       (502) staff       (20)     1930 2023-12-30 18:55:43.000000 mantis-cli-9.1.0/mantis/crypto.py
+-rw-r--r--   0 erik       (502) staff       (20)     3016 2023-12-30 19:52:28.000000 mantis-cli-9.1.0/mantis/environment.py
+-rw-r--r--   0 erik       (502) staff       (20)     3862 2023-12-19 14:11:49.000000 mantis-cli-9.1.0/mantis/extensions.py
+-rw-r--r--   0 erik       (502) staff       (20)     1549 2023-12-30 18:57:08.000000 mantis-cli-9.1.0/mantis/helpers.py
+-rw-r--r--   0 erik       (502) staff       (20)     6030 2023-12-21 10:31:22.000000 mantis-cli-9.1.0/mantis/logic.py
+-rw-r--r--   0 erik       (502) staff       (20)    31922 2023-12-30 19:53:50.000000 mantis-cli-9.1.0/mantis/managers.py
+drwxr-xr-x   0 erik       (502) staff       (20)        0 2023-12-30 20:05:16.722733 mantis-cli-9.1.0/mantis_cli.egg-info/
+-rw-r--r--   0 erik       (502) staff       (20)      797 2023-12-30 20:05:16.000000 mantis-cli-9.1.0/mantis_cli.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (502) staff       (20)      411 2023-12-30 20:05:16.000000 mantis-cli-9.1.0/mantis_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (502) staff       (20)        1 2023-12-30 20:05:16.000000 mantis-cli-9.1.0/mantis_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (502) staff       (20)       52 2023-12-30 20:05:16.000000 mantis-cli-9.1.0/mantis_cli.egg-info/entry_points.txt
+-rw-r--r--   0 erik       (502) staff       (20)        7 2023-12-30 20:05:16.000000 mantis-cli-9.1.0/mantis_cli.egg-info/top_level.txt
+-rw-r--r--   0 erik       (502) staff       (20)       79 2023-12-30 20:05:16.723091 mantis-cli-9.1.0/setup.cfg
+-rw-r--r--   0 erik       (502) staff       (20)     1132 2021-12-22 06:51:20.000000 mantis-cli-9.1.0/setup.py
```

### Comparing `mantis-cli-9.0.4/.gitignore` & `mantis-cli-9.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mantis-cli-9.0.4/LICENSE` & `mantis-cli-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mantis-cli-9.0.4/PKG-INFO` & `mantis-cli-9.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mantis-cli
-Version: 9.0.4
+Version: 9.1.0
 Summary: Management command to build and deploy webapps, especially based on Django
 Home-page: https://github.com/PragmaticMates/mantis-cli
 Author: Erik Telepovský
 Author-email: info@pragmaticmates.com
 Maintainer: Pragmatic Mates
 Maintainer-email: info@pragmaticmates.com
 License: GNU General Public License (GPL)
```

### Comparing `mantis-cli-9.0.4/mantis/extensions.py` & `mantis-cli-9.1.0/mantis/extensions.py`

 * *Files identical despite different names*

### Comparing `mantis-cli-9.0.4/mantis/logic.py` & `mantis-cli-9.1.0/mantis/logic.py`

 * *Files identical despite different names*

### Comparing `mantis-cli-9.0.4/mantis/managers.py` & `mantis-cli-9.1.0/mantis/managers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,32 @@
 import datetime
 import requests
 from distutils.util import strtobool
 from os import path
 from os.path import dirname, normpath
 from time import sleep
 
-from mantis.helpers import CLI, Colors, Crypto, load_config
+from mantis.crypto import Crypto
+from mantis.environment import Environment
+from mantis.helpers import CLI, Colors, load_config
 
 
 class DefaultManager(object):
     environment_id = None
 
     def __init__(self, config=None, environment_id=None, mode='remote'):
         self.environment_id = environment_id
         self.mode = mode
+
+        # init config
         self.init_config(config)
+
+        # init environment
+        self.init_environment()
+
         self.KEY = self.read_key()
         self.encrypt_deterministically = self.config.get('encrypt_deterministically', False)
 
     @property
     def host(self):
         return self.connection_details['host']
 
@@ -47,15 +55,15 @@
             'user': None,
             'port': None
         }
 
         if hasattr(self, property_name):
             return getattr(self, property_name)
 
-        if 'local' in self.environment_id:
+        if 'local' in self.env.id:
             details = {
                 'host': 'localhost',
                 'user': None,
                 'port': None
             }
         elif self.connection:
             if self.connection.startswith('ssh://'):
@@ -81,15 +89,15 @@
         # set project path
         self.project_path = self.config.get('project_path', f'/home/{self.user}/public_html/web')
 
         return details
 
     @property
     def docker_connection(self):
-        if 'local' in self.environment_id:
+        if 'local' in self.env.id:
             return ''
 
         if self.mode == 'remote':
             if self.connection.startswith('ssh://'):
                 return f'DOCKER_HOST="{self.connection}"'
             elif self.connection.startswith('context://'):
                 context_name = self.connection.replace('context://', '')
@@ -103,68 +111,56 @@
 
         configs_folder_path = self.config.get('configs_folder_path', '')
         configs_folder_name = self.config.get('configs_folder_name', 'configs')
         self.configs_path = f'{configs_folder_path}{configs_folder_name}'
         self.configs_compose_folder = self.config.get('configs_compose_folder', 'compose')
         self.key_file = path.join(f'{dirname(self.config_file)}', 'mantis.key')
 
-        # environment files
-        self.environment_file_prefix = self.config.get('environment_file_prefix', '')
+        # Get environment settings
+        self.PROJECT_NAME = self.config['project_name']
 
-        if self.environment_id:
-            self.environment_folder = self.config.get('environment_folder', 'environments')
-            self.environment_path = path.join(self.configs_path, self.environment_folder, f'.{self.environment_id}')
-
-            if not os.path.exists(self.environment_path):
-                CLI.error(f"Environment path '{self.environment_path}' does not exist")
-
-            for dirpath, directories, files in os.walk(self.environment_path):
-                environment_filenames = list(filter(lambda f: f.endswith('.env'), files))
-                encrypted_environment_filenames = list(filter(lambda f: f.endswith('.env.encrypted'), files))
-                self.environment_files = list(map(lambda x: path.join(dirpath, x), environment_filenames))
-                self.encrypted_environment_files = list(map(lambda x: path.join(dirpath, x), encrypted_environment_filenames))
+    def init_environment(self):
+        self.env = Environment(
+            environment_id=self.environment_id,
+            folder=self.config.get('environment_folder', 'environments'),
+            file_prefix=self.config.get('environment_file_prefix', '')
+        )
 
         # connection
-        self.connection = self.config.get('connections', {}).get(self.environment_id, None)
-
-        # Get environment settings
-        self.PROJECT_NAME = self.config['project_name']
+        self.connection = self.config.get('connections', {}).get(self.env.id, None)
 
         # containers
         # self.CONTAINER_PREFIX = self.config['containers']['prefix']
         self.CONTAINER_PREFIX = self.PROJECT_NAME
         self.IMAGE_PREFIX = self.PROJECT_NAME
 
         if 'containers' in self.config:
             # TODO: refactor
             self.CONTAINER_WEBSERVER = f"{self.CONTAINER_PREFIX}{self.get_container_suffix('webserver')}"
 
             self.compose_name = self.config['compose']['name']
             self.COMPOSE_PREFIX = 'docker-compose' if self.compose_name == '' else f'docker-compose.{self.compose_name}'
-            self.compose_configs = [
-                f'{self.configs_path}/{self.configs_compose_folder}/{self.COMPOSE_PREFIX}.yml', # TODO: deprecated
-                f'{self.configs_path}/{self.configs_compose_folder}/{self.COMPOSE_PREFIX}.{self.environment_id}.yml',
-            ]
+            self.compose_config = f'{self.configs_path}/{self.configs_compose_folder}/{self.COMPOSE_PREFIX}.{self.env.id}.yml',
 
         # TODO: refactor
-        self.DATABASE = self.config.get('cache', 'postgres')
+        self.DATABASE = self.config.get('db', 'postgres')
         self.CACHE = self.config.get('cache', 'redis')
         self.WEBSERVER = self.config.get('webserver', 'nginx')
 
-        self.database_config = f'{self.configs_path}/{self.DATABASE}/{self.environment_file_prefix}{self.environment_id}.conf'
-        self.cache_config = f'{self.configs_path}/{self.CACHE}/{self.environment_file_prefix}{self.environment_id}.conf'
+        self.database_config = f'{self.configs_path}/{self.DATABASE}/{self.env.file_prefix}{self.env.id}.conf'
+        self.cache_config = f'{self.configs_path}/{self.CACHE}/{self.env.file_prefix}{self.env.id}.conf'
         self.webserver_html = f'{self.configs_path}/{self.WEBSERVER}/html/'
         self.webserver_config_proxy = f'{self.configs_path}/{self.WEBSERVER}/proxy_directives.conf'
         self.webserver_config_default = f'{self.configs_path}/{self.WEBSERVER}/default.conf'
-        self.webserver_config_site = f'{self.configs_path}/{self.WEBSERVER}/sites/{self.environment_file_prefix}{self.environment_id}.conf'
+        self.webserver_config_site = f'{self.configs_path}/{self.WEBSERVER}/sites/{self.env.file_prefix}{self.env.id}.conf'
         self.htpasswd = f'{self.configs_path}/{self.WEBSERVER}/secrets/.htpasswd'
 
     def check_environment_encryption(self, env_file):
         decrypted_environment = self.decrypt_env(env_file=env_file, return_value=True)        # .env.encrypted
-        loaded_environment = self.load_environment(env_file)                         # .env
+        loaded_environment = self.env.load(env_file)                                          # .env
 
         if decrypted_environment is None:
             env_file_encrypted = f'{env_file}.encrypted'
             CLI.error(f'Encrypted environment {env_file_encrypted} is empty!')
 
         if loaded_environment is None:
             CLI.error(f'Loaded environment {env_file} is empty!')
@@ -223,72 +219,72 @@
 
     def encrypt_env(self, params='', env_file=None, return_value=False):
         if env_file is None:
             CLI.info(f'Environment file not specified. Walking all environment files...')
 
             values = {}
 
-            for env_file in self.environment_files:
+            for env_file in self.env.files:
                 value = self.encrypt_env(params=params, env_file=env_file, return_value=return_value)
                 if return_value:
                     values.update(value)
 
             return values if return_value else None
 
         CLI.info(f'Encrypting environment file {env_file}...')
         env_file_encrypted = f'{env_file}.encrypted'
 
         if not self.KEY:
             CLI.error('Missing mantis key! (%s)' % self.key_file)
 
-        decrypted_lines = self.read_environment(env_file)
+        decrypted_lines = self.env.read(env_file)
 
         if not decrypted_lines:
             return None
 
         encrypted_lines = []
         encrypted_env = {}
 
         for line in decrypted_lines:
-            if self.is_valid_line(line):
-                var, decrypted_value = self.parse_line(line)
+            if Environment.is_valid_line(line):
+                var, decrypted_value = Environment.parse_line(line)
                 encrypted_value = Crypto.encrypt(decrypted_value, self.KEY, self.encrypt_deterministically)
                 encrypted_lines.append(f'{var}={encrypted_value}')
                 encrypted_env[var] = encrypted_value
             else:
                 encrypted_lines.append(line)
 
             if not return_value and 'force' not in params:
                 print(encrypted_lines[-1])
 
         if return_value:
             return encrypted_env
 
         if 'force' in params:
-            self._save_file(env_file_encrypted, encrypted_lines)
+            Environment.save(env_file_encrypted, encrypted_lines)
             CLI.success(f'Saved to file {env_file_encrypted}')
         else:
             # save to file?
             CLI.warning(f'Save to file {env_file_encrypted}?')
 
             save_to_file = input("(Y)es or (N)o: ")
 
             if save_to_file.lower() == 'y':
-                self._save_file(env_file_encrypted, encrypted_lines)
+                Environment.save(env_file_encrypted, encrypted_lines)
                 CLI.success(f'Saved to file {env_file_encrypted}')
             else:
                 CLI.warning(f'Save it to {env_file_encrypted} manually.')
 
     def decrypt_env(self, params='', env_file=None, return_value=False):
         if env_file is None:
             CLI.info(f'Environment file not specified. Walking all environment files...')
 
             values = {}
 
-            for encrypted_env_file in self.encrypted_environment_files:
+            for encrypted_env_file in self.env.encrypted_files:
                 env_file = encrypted_env_file.rstrip('.encrypted')
                 value = self.decrypt_env(params=params, env_file=env_file, return_value=return_value)
                 if return_value:
                     values.update(value)
 
             return values if return_value else None
 
@@ -296,133 +292,86 @@
 
         if not return_value:
             CLI.info(f'Decrypting environment file {env_file_encrypted}...')
 
         if not self.KEY:
             CLI.error('Missing mantis key!')
 
-        encrypted_lines = self.read_environment(env_file_encrypted)
+        encrypted_lines = self.env.read(env_file_encrypted)
 
         if encrypted_lines is None:
             return None
 
         if not encrypted_lines:
             return {}
 
         decrypted_lines = []
         decrypted_env = {}
 
         for line in encrypted_lines:
-            if self.is_valid_line(line):
-                var, encrypted_value = self.parse_line(line)
+            if Environment.is_valid_line(line):
+                var, encrypted_value = Environment.parse_line(line)
                 decrypted_value = Crypto.decrypt(encrypted_value, self.KEY, self.encrypt_deterministically)
                 decrypted_lines.append(f'{var}={decrypted_value}')
                 decrypted_env[var] = decrypted_value
             else:
                 decrypted_lines.append(line)
 
             if not return_value and 'force' not in params:
                 print(decrypted_lines[-1])
 
         if return_value:
             return decrypted_env
 
         if 'force' in params:
-            self._save_file(env_file, decrypted_lines)
+            Environment.save(env_file, decrypted_lines)
             CLI.success(f'Saved to file {env_file}')
         else:
             # save to file?
             CLI.warning(f'Save to file {env_file}?')
 
             save_to_file = input("(Y)es or (N)o: ")
 
             if save_to_file.lower() == 'y':
-                self._save_file(env_file, decrypted_lines)
+                Environment.save(env_file, decrypted_lines)
                 CLI.success(f'Saved to file {env_file}')
             else:
                 CLI.warning(f'Save it to {env_file} manually.')
 
-    def _save_file(self, path, lines):
-        with open(path, "w") as f:
-            for line in lines:
-                f.write(f'{line}\n')
-
     def check_env(self):
         # check if pair file exists
-        for encrypted_env_file in self.encrypted_environment_files:
+        for encrypted_env_file in self.env.encrypted_files:
             env_file = encrypted_env_file.rstrip('.encrypted')
             if not os.path.exists(env_file):
                 CLI.warning(f'Environment file {env_file} does not exist')
 
-        for env_file in self.environment_files:
+        for env_file in self.env.files:
             env_file_encrypted = f'{env_file}.encrypted'
 
             # check if pair file exists
             if not os.path.exists(env_file_encrypted):
                 CLI.warning(f'Environment file {env_file_encrypted} does not exist')
                 continue
 
             # check encryption values
             self.check_environment_encryption(env_file)
 
-    def read_environment(self, path):
-        if not os.path.exists(path):
-            CLI.error(f'Environment file {path} does not exist')
-            return None
-
-        with open(path) as f:
-            return f.read().splitlines()
-
-    def load_environment(self, path=None):
-        # if not path is specified, load variables from all environment files
-        if not path:
-            CLI.info(f'Environment file path not specified. Walking all environment files...')
-
-            values = {}
-
-            for env_file in self.environment_files:
-                env_values = self.load_environment(path=env_file)
-                values.update(env_values)
-
-            return values
-
-        # read environment file
-        lines = self.read_environment(path)
-
-        # TODO: refactor
-        return dict(
-            (
-                self.parse_line(line)[0],
-                self.parse_line(line)[1]
-            )
-            for line in lines if self.is_valid_line(line)
-        )
-
-    def is_valid_line(self, line):
-        return not line.startswith('#') and line.rstrip("\n") != ''
-
-    def parse_line(self, line):
-        if not self.is_valid_line(line):
-            return None
-
-        return line.split('=', maxsplit=1)
-
     def cmd(self, command):
         command = command.strip()
 
         error_message = "Error during running command '%s'" % command
 
         try:
             if os.system(command) != 0:
                 CLI.error(error_message)
                 # raise Exception(error_message)
         except:
             CLI.error(error_message)
             # raise Exception(error_message)
-    
+
     def contexts(self):
         self.cmd('docker context ls')
 
     def create_context(self):
         CLI.info('Creating docker context')
         protocol = input("Protocol: (U)nix or (S)sh: ")
 
@@ -461,15 +410,15 @@
         # create context
         self.cmd(command)
         self.contexts()
 
     def get_container_suffix(self, service):
         delimiter = '-'
         return self.config.get('containers', {}).get('suffixes', {}).get(service, f'{delimiter}{service}')
-    
+
     def get_container_name(self, service):
         suffix = self.get_container_suffix(service)
         return f'{self.CONTAINER_PREFIX}{suffix}'.replace('_', '-')
 
     def get_image_suffix(self, service):
         delimiter = '_'
         return self.config.get('containers', {}).get('suffixes', {}).get(service, f'{delimiter}{service}')
@@ -619,15 +568,15 @@
         elif context == 'compose':
             CLI.warning('Uploading configs for context "compose" [docker compose configs and environment]')
         elif context == 'mantis':
             CLI.warning('Uploading configs for mantis [mantis.json]')
         else:
             CLI.error(f'Unknown context "{context}". Available: services, compose, mantis or all')
 
-        if self.environment_id == 'local':
+        if self.env.id == 'local':
             print('Skipping for local...')
         elif self.mode == 'host':
             CLI.warning('Not uploading due to host mode! Be sure your configs on host are up to date!')
         else:
             CLI.info('Uploading...')
 
             # TODO: refactor
@@ -640,25 +589,24 @@
             elif context == 'mantis':
                 if os.path.exists(self.config_file):
                     self.cmd(f'rsync -arvz -e \'ssh -p {self.port}\' -rvzh --progress {self.config_file} {self.user}@{self.host}:{self.project_path}/configs/')
                 else:
                     CLI.info(f'{self.config_file} does not exists. Skipping...')
 
             elif context == 'compose':
-                for env_file in self.environment_files:
+                for env_file in self.env.files:
                     if os.path.exists(env_file):
                         self.cmd(f'rsync -arvz -e \'ssh -p {self.port}\' -rvzh --progress {env_file} {self.user}@{self.host}:{self.project_path}/configs/environments/')  # TODO: paths
                     else:
                         CLI.info(f'{env_file} does not exists. Skipping...')
 
-                for config in self.compose_configs:
-                    if os.path.exists(config):
-                        self.cmd(f'rsync -arvz -e \'ssh -p {self.port}\' -rvzh --progress {config} {self.user}@{self.host}:{self.project_path}/configs/{self.configs_compose_folder}/')
-                    else:
-                        CLI.info(f'{config} does not exists. Skipping...')
+                if os.path.exists(self.compose_config):
+                    self.cmd(f'rsync -arvz -e \'ssh -p {self.port}\' -rvzh --progress {self.compose_config} {self.user}@{self.host}:{self.project_path}/configs/{self.configs_compose_folder}/')
+                else:
+                    CLI.info(f'{self.compose_config} does not exists. Skipping...')
 
     def restart(self):
         CLI.info('Restarting...')
         steps = 4
 
         # run down project containers
         CLI.step(1, steps, 'Running down project containers...')
@@ -698,15 +646,15 @@
         step = 1
         CLI.step(step, steps, f'Zero downtime services: {zero_downtime_services}')
 
         for service in zero_downtime_services:
             container = self.get_container_name(service)
 
             # run new container
-            self.docker_compose(f'--project-name={self.PROJECT_NAME} run -d --service-ports --name={container}-new {service}')
+            self.docker_compose(f'run -d --service-ports --name={container}-new {service}')
 
             # healthcheck
             # TODO: configurable retries number
             num_retries = 30
             # num_retries = 20
 
             self.healthcheck(retries=num_retries, service=f'{service}-new', break_if_successful=True)
@@ -757,15 +705,15 @@
 
                 CLI.info(f'Removing container [{container}]...')
                 self.docker(f'container rm {container}')
             else:
                 CLI.info(f'{container} was not running')
 
             CLI.info(f'Creating new container [{container}]...')
-            self.docker_compose(f'--project-name={self.PROJECT_NAME} run -d --service-ports --name={container} {service}')
+            self.docker_compose(f'run -d --service-ports --name={container} {service}')
 
     def stop(self, params=None):
         CLI.info('Stopping containers...')
 
         containers = self.get_containers() if not params else params.split(' ')
 
         steps = len(containers)
@@ -783,23 +731,23 @@
 
         for index, container in enumerate(containers):
             CLI.step(index + 1, steps, f'Starting {container}')
             self.docker(f'container start {container}')
 
     def run(self, params):
         CLI.info(f'Running {params}...')
-        self.docker_compose(f'--project-name={self.PROJECT_NAME} run {params}')
+        self.docker_compose(f'run {params}')
 
     def up(self, params=''):
         CLI.info(f'Starting up {params}...')
-        self.docker_compose(f'--project-name={self.PROJECT_NAME} up {params} -d')
+        self.docker_compose(f'up {params} -d')
 
     def down(self, params=''):
         CLI.info(f'Running down {params}...')
-        self.docker_compose(f'--project-name={self.PROJECT_NAME} down {params}')
+        self.docker_compose(f'down {params}')
 
     def remove(self, params=''):
         CLI.info('Removing containers...')
 
         containers = self.get_containers() if params == '' else params.split(' ')
 
         steps = len(containers)
@@ -857,43 +805,39 @@
         for index, container in enumerate(containers):
             CLI.step(index + 1, steps, f'{container} logs')
             self.docker(f'logs {container} {lines}')
 
     def bash(self, params):
         CLI.info('Running bash...')
         self.docker(f'exec -it --user root {params} /bin/bash')
-        # self.docker_compose(f'--project-name={self.PROJECT_NAME} run --entrypoint /bin/bash {container}')
+        # self.docker_compose(f'run --entrypoint /bin/bash {container}')
 
     def sh(self, params):
         CLI.info('Logging to container...')
         self.docker(f'exec -it --user root {params} /bin/sh')
 
     def exec(self, params):
         container, command = params.split(' ', maxsplit=1)
         CLI.info(f'Executing command "{command}" in container {container}...')
         self.docker(f'exec -it {container} {command}')
 
     def get_containers(self):
         containers = self.docker(f'container ls -a --format \'{{{{.Names}}}}\'', return_output=True)\
             .strip('\n').strip().split('\n')
+
+        # Remove empty strings
+        containers = list(filter(None, containers))
+
         print(containers)
         return containers
 
     def get_containers_starting_with(self, start_with):
         return [i for i in self.get_containers() if i.startswith(start_with)]
 
     def docker(self, command, return_output=False):
         if return_output:
             return os.popen(f'{self.docker_connection} docker {command}').read()
 
         self.cmd(f'{self.docker_connection} docker {command}')
 
     def docker_compose(self, command):
-        docker_compose_file = f'{self.configs_path}/{self.configs_compose_folder}/{self.COMPOSE_PREFIX}.yml'
-        docker_compose_environment_file = f'{self.configs_path}/{self.configs_compose_folder}/{self.COMPOSE_PREFIX}.{self.environment_id}.yml'
-
-        if os.path.exists(docker_compose_file):
-            # compose file inheritance (multiple compose file deployment)
-            self.cmd(f'{self.docker_connection} docker compose -f {docker_compose_file} -f {docker_compose_environment_file} {command}')
-        else:
-            # single compose file usage
-            self.cmd(f'{self.docker_connection} docker compose -f {docker_compose_environment_file} {command}')
+        self.cmd(f'{self.docker_connection} docker compose -f {self.compose_config} --project-name={self.PROJECT_NAME} {command}')
```

### Comparing `mantis-cli-9.0.4/mantis_cli.egg-info/PKG-INFO` & `mantis-cli-9.1.0/mantis_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mantis-cli
-Version: 9.0.4
+Version: 9.1.0
 Summary: Management command to build and deploy webapps, especially based on Django
 Home-page: https://github.com/PragmaticMates/mantis-cli
 Author: Erik Telepovský
 Author-email: info@pragmaticmates.com
 Maintainer: Pragmatic Mates
 Maintainer-email: info@pragmaticmates.com
 License: GNU General Public License (GPL)
```

### Comparing `mantis-cli-9.0.4/setup.py` & `mantis-cli-9.1.0/setup.py`

 * *Files identical despite different names*

