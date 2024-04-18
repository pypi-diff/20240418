# Comparing `tmp/cmd_ai-0.1.7.tar.gz` & `tmp/cmd_ai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmd_ai-0.1.7.tar", last modified: Tue Jan 16 15:06:41 2024, max compression
+gzip compressed data, was "cmd_ai-0.2.1.tar", last modified: Thu Apr 18 16:28:28 2024, max compression
```

## Comparing `cmd_ai-0.1.7.tar` & `cmd_ai-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-16 15:06:41.565851 cmd_ai-0.1.7/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2546 2024-01-16 15:06:41.565851 cmd_ai-0.1.7/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2275 2024-01-16 15:06:38.000000 cmd_ai-0.1.7/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-16 15:06:41.561851 cmd_ai-0.1.7/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    15422 2024-01-16 15:06:40.000000 cmd_ai-0.1.7/bin/cmd_ai
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-16 15:06:41.565851 cmd_ai-0.1.7/cmd_ai/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      245 2023-11-21 14:40:25.000000 cmd_ai-0.1.7/cmd_ai/__init__.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1129 2023-11-21 16:13:50.000000 cmd_ai-0.1.7/cmd_ai/api_key.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7596 2024-01-12 15:46:05.000000 cmd_ai-0.1.7/cmd_ai/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9459 2024-01-05 12:51:47.000000 cmd_ai-0.1.7/cmd_ai/function_chmi.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2296 2023-12-28 08:29:31.000000 cmd_ai-0.1.7/cmd_ai/function_goog.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3228 2023-12-28 08:29:31.000000 cmd_ai-0.1.7/cmd_ai/function_webc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    17337 2024-01-12 15:56:37.000000 cmd_ai-0.1.7/cmd_ai/g_askme.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6149 2023-11-21 16:13:50.000000 cmd_ai-0.1.7/cmd_ai/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      555 2023-12-06 16:02:32.000000 cmd_ai-0.1.7/cmd_ai/pipe.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4916 2024-01-08 08:00:50.000000 cmd_ai-0.1.7/cmd_ai/speak.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7455 2024-01-15 09:50:11.000000 cmd_ai-0.1.7/cmd_ai/syscom.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8161 2024-01-15 09:50:11.000000 cmd_ai-0.1.7/cmd_ai/texts.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2736 2023-11-21 16:13:51.000000 cmd_ai-0.1.7/cmd_ai/topbar.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1077 2023-11-21 16:13:51.000000 cmd_ai-0.1.7/cmd_ai/unitname.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       21 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-01-16 15:06:41.565851 cmd_ai-0.1.7/cmd_ai.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2546 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      460 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       68 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        7 2024-01-16 15:06:41.000000 cmd_ai-0.1.7/cmd_ai.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-01-16 15:06:41.565851 cmd_ai-0.1.7/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1215 2024-01-02 20:26:23.000000 cmd_ai-0.1.7/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-18 16:28:28.386367 cmd_ai-0.2.1/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     2914 2024-04-18 16:28:28.386367 cmd_ai-0.2.1/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2440 2024-04-18 16:28:26.000000 cmd_ai-0.2.1/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-18 16:28:28.382367 cmd_ai-0.2.1/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    21189 2024-04-18 16:27:58.000000 cmd_ai-0.2.1/bin/cmd_ai
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-18 16:28:28.386367 cmd_ai-0.2.1/cmd_ai/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      245 2023-11-21 14:40:25.000000 cmd_ai-0.2.1/cmd_ai/__init__.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1129 2023-11-21 16:13:50.000000 cmd_ai-0.2.1/cmd_ai/api_key.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      608 2024-03-18 09:12:22.000000 cmd_ai-0.2.1/cmd_ai/best_examples.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7596 2024-01-22 08:00:22.000000 cmd_ai-0.2.1/cmd_ai/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9459 2024-01-05 12:51:47.000000 cmd_ai-0.2.1/cmd_ai/function_chmi.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2296 2023-12-28 08:29:31.000000 cmd_ai-0.2.1/cmd_ai/function_goog.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3228 2023-12-28 08:29:31.000000 cmd_ai-0.2.1/cmd_ai/function_webc.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1896 2024-04-18 15:32:23.000000 cmd_ai-0.2.1/cmd_ai/g_askdalle.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    17569 2024-04-18 14:58:55.000000 cmd_ai-0.2.1/cmd_ai/g_askme.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     3243 2024-04-18 16:22:26.000000 cmd_ai-0.2.1/cmd_ai/g_askvision.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6149 2023-11-21 16:13:50.000000 cmd_ai-0.2.1/cmd_ai/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      555 2023-12-06 16:02:32.000000 cmd_ai-0.2.1/cmd_ai/pipe.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4916 2024-01-08 08:00:50.000000 cmd_ai-0.2.1/cmd_ai/speak.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8096 2024-04-18 15:45:02.000000 cmd_ai-0.2.1/cmd_ai/syscom.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8548 2024-04-18 15:43:11.000000 cmd_ai-0.2.1/cmd_ai/texts.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2736 2023-11-21 16:13:51.000000 cmd_ai-0.2.1/cmd_ai/topbar.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1077 2023-11-21 16:13:51.000000 cmd_ai-0.2.1/cmd_ai/unitname.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       21 2024-04-18 16:28:27.000000 cmd_ai-0.2.1/cmd_ai/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-18 16:28:28.386367 cmd_ai-0.2.1/cmd_ai.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     2914 2024-04-18 16:28:28.000000 cmd_ai-0.2.1/cmd_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      527 2024-04-18 16:28:28.000000 cmd_ai-0.2.1/cmd_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-18 16:28:28.000000 cmd_ai-0.2.1/cmd_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       88 2024-04-18 16:28:28.000000 cmd_ai-0.2.1/cmd_ai.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        7 2024-04-18 16:28:28.000000 cmd_ai-0.2.1/cmd_ai.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-18 16:28:28.386367 cmd_ai-0.2.1/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1239 2024-02-14 13:35:42.000000 cmd_ai-0.2.1/setup.py
```

### Comparing `cmd_ai-0.1.7/PKG-INFO` & `cmd_ai-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 Metadata-Version: 2.1
 Name: cmd_ai
-Version: 0.1.7
+Version: 0.2.1
 Summary: Another ChatGTP project in commandline of linux
 Home-page: http://gitlab.com/me/cmd_ai
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: fire
+Requires-Dist: console
+Requires-Dist: click
+Requires-Dist: pandas
+Requires-Dist: openai
+Requires-Dist: prompt_toolkit
+Requires-Dist: googlesearch-python
+Requires-Dist: playsound
+Requires-Dist: unidecode
 
 Project cmd~ai~
 ===============
 
 *Another ChatGPT project that implements as a shell interface*
 
 README for version `0.0.8`
 
 EXAMPLE
 -------
 
 `cmd_ai "Jak bude zitra (pouze) ve Stredoceskem kraji?" -u -vcs`
 
+`cmd_ai -a dalle "Landscape with hills and lakes, photographic quality"`
+
 Installation
 ------------
 
 It should work with `pip3 install`, not tested yet.
 
 Needs `API_KEY` for OpenAI in `~/.openai.token` , than it creates own
 copy at `~/.config/cmd_ai/cfg.json`
@@ -48,15 +58,15 @@
 .e      execute code
 .r      reset messages, scripts
 .l      show tokens
 .m      show models
 .l number ... change limit tokens
 ________________ ROLES _____________
 .a   assistent
-.t   NO translator
+.t   translator
 .p   python coder
 .s   shell expert
 .d   NO dalle
 ________________ MODEL
 .i   NO use dalle
 .v   NO use vision
 ```
@@ -75,14 +85,18 @@
 Similar but for bash
 
 ### Piper
 
 Works only from commandline, when pipe (stdin) is detected. No memory,
 on task/question, asks before runs the code
 
+### Dalle
+
+Gets one image, 1024x1024, restricted prompt rewrite
+
 1.  [DONE]{.done .DONE} Commit message example
 
     ``` {.example}
     git diff | ai 'write a commit message, show it as git commit -a -m "message" command'
     ```
 
 DOING Function calls / tools
@@ -102,21 +116,19 @@
 ### WAITING Document upload
 
 -   it costs 0.20\$ per 1GB per day....
 
 Images
 ------
 
-### POSTPONED Dalle3
+### [DONE]{.done .DONE} Dalle3 {#dalle3}
 
-I need to test if this works or what
+First attmpt works also in cmdline (-a dalle)
 
 ### [TODO]{.todo .TODO} Upload for analysis to GPT-v {#upload-for-analysis-to-gpt-v}
 
 That would be interesting from commandline
 
 Dependencies
 ============
 
 -   googlesearch-python
-
-
```

### Comparing `cmd_ai-0.1.7/README.md` & `cmd_ai-0.2.1/cmd_ai.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,40 @@
+Metadata-Version: 2.1
+Name: cmd_ai
+Version: 0.2.1
+Summary: Another ChatGTP project in commandline of linux
+Home-page: http://gitlab.com/me/cmd_ai
+Author: jaromrax
+Author-email: jaromrax@gmail.com
+License: GPL2
+Description-Content-Type: text/markdown
+Requires-Dist: fire
+Requires-Dist: console
+Requires-Dist: click
+Requires-Dist: pandas
+Requires-Dist: openai
+Requires-Dist: prompt_toolkit
+Requires-Dist: googlesearch-python
+Requires-Dist: playsound
+Requires-Dist: unidecode
+
 Project cmd~ai~
 ===============
 
 *Another ChatGPT project that implements as a shell interface*
 
 README for version `0.0.8`
 
 EXAMPLE
 -------
 
 `cmd_ai "Jak bude zitra (pouze) ve Stredoceskem kraji?" -u -vcs`
 
+`cmd_ai -a dalle "Landscape with hills and lakes, photographic quality"`
+
 Installation
 ------------
 
 It should work with `pip3 install`, not tested yet.
 
 Needs `API_KEY` for OpenAI in `~/.openai.token` , than it creates own
 copy at `~/.config/cmd_ai/cfg.json`
@@ -37,15 +58,15 @@
 .e      execute code
 .r      reset messages, scripts
 .l      show tokens
 .m      show models
 .l number ... change limit tokens
 ________________ ROLES _____________
 .a   assistent
-.t   NO translator
+.t   translator
 .p   python coder
 .s   shell expert
 .d   NO dalle
 ________________ MODEL
 .i   NO use dalle
 .v   NO use vision
 ```
@@ -64,14 +85,18 @@
 Similar but for bash
 
 ### Piper
 
 Works only from commandline, when pipe (stdin) is detected. No memory,
 on task/question, asks before runs the code
 
+### Dalle
+
+Gets one image, 1024x1024, restricted prompt rewrite
+
 1.  [DONE]{.done .DONE} Commit message example
 
     ``` {.example}
     git diff | ai 'write a commit message, show it as git commit -a -m "message" command'
     ```
 
 DOING Function calls / tools
@@ -91,17 +116,17 @@
 ### WAITING Document upload
 
 -   it costs 0.20\$ per 1GB per day....
 
 Images
 ------
 
-### POSTPONED Dalle3
+### [DONE]{.done .DONE} Dalle3 {#dalle3}
 
-I need to test if this works or what
+First attmpt works also in cmdline (-a dalle)
 
 ### [TODO]{.todo .TODO} Upload for analysis to GPT-v {#upload-for-analysis-to-gpt-v}
 
 That would be interesting from commandline
 
 Dependencies
 ============
```

### Comparing `cmd_ai-0.1.7/bin/cmd_ai` & `cmd_ai-0.2.1/bin/cmd_ai`

 * *Files 18% similar despite different names*

```diff
@@ -19,16 +19,21 @@
 import re
 
 
 from cmd_ai import config # , key_enter, topbar, unitname
 from cmd_ai import texts
 from cmd_ai.api_key import get_api_key
 from cmd_ai.g_askme import g_askme
+from cmd_ai.g_askdalle import g_askdalle
+from cmd_ai.g_askvision import g_askvision
 from cmd_ai.syscom import process_syscom
 from cmd_ai.version import __version__
+from cmd_ai import best_examples
+
+# from cmd_ai import best_examples
 
 from cmd_ai.speak import str_to_mp3
 import select
 import click
 
 # ===============================================================================================
 
@@ -200,58 +205,108 @@
         if config.SOURCECODE_EXISTS or config.PYSCRIPT_EXISTS or config.SHSCRIPT_EXISTS:
             print("x... CODE present .... no reading...sorry")
         else:
             str_to_mp3( resiw,  readme=True, lang=config.READALOUDSET[modu])
 
 
 
-def pipe_mode(question):
+def pipe_mode():
     """
     detect mode - pipe or not
     """
-    if question is None or question=="" or len(question)<5: return None
+    # this was blocking the detection of pipe...
+    #if question is None or question=="" or len(question)<5: return None
+    # LET US CONSIDER IT IS PIPE:
+    #print(f"D... {fg.lightgray}Pipe mode OR NOT???? {fg.default}")
     if select.select([sys.stdin, ], [], [], 0.0)[0]:
-        #print(f"D... {fg.lightgray}Pipe mode! {fg.default}")
+        print(f"D... {fg.lightslategray}Pipe mode detected! {fg.default}")
 
         mstdin = []
         for line in sys.stdin:
             mstdin.append( line.strip() )
         return mstdin
+    # UNCLESS IT IS NOT
     else:
+        # print(f"D... {fg.lightgray} NO Pipe  {fg.default}")
         return None #print("No pipe")
 
 
 ###################################################################
 #####################################################
 ###########################################
 ######################################
 
-def main(cmd="", debug=False, u_switch = False, g_switch=False, vcs=False, ven=False):
-    """Main function of the project"""
+def main(cmd=None, budget=False, debug=False,
+         u_switch = False, g_switch=False, csspeak=False, enspeak=False,
+         version = False,
+         multilineinput = False,
+         limit_tokens = None,
+         assistant = None,
+         examples = False):
+    """
+chatGPT commandline interface
 
+ it can run
+ - interactive
+ - as a standalone command ( cmd_ai "Say Hi")
+ - in pipe ( echo "Say Hi" | cmd_ai -a  pythonista) ; default assistant is Ubuntu 22 expert
+Parameters
+  assistant :   ... assistant name: assistant or None | translator | sheller | pythonista | dalle
+  limit_tokens : ...  limit  tokens. 300 is very basic -l
+  multilineinput : ... tricky, use Alt-Enter instead of enter. Do not use in pipe
+  budget : ... print the budget on this pc, split by month and by day in the last month
+  u_switch : ... add ability - spectial utils - testing
+  g_switch : ... add google search 1st five ability
+  version : ... program version
+  examples : ... show examples
+"""
+    #                        HELP help
+    if examples:
+        best_examples.main()
+        return 0
+    if version:
+        print(__version__)
+        return 0
     # ======== DEFINE THE CONFIG FILE HERE ========
 
 
     if os.path.exists(  os.path.expanduser(config.CONFIG['pricelog'] ) ):
         # dateparse = lambda x: dt.datetime.strptime(x, '%Y-%m-%d %H:%M:%S')
         df = pd.read_csv( os.path.expanduser(config.CONFIG['pricelog']) ,
                           delim_whitespace=True,
                           names = ['date','time', 'in','out','price']
                          )#, parse_dates=['datetime'], date_parser=dateparse)
 
         df['datetime'] = pd.to_datetime(df.date)
-        df = df.groupby(df['datetime'])['price'].sum()#transform('sum')
-        print("____________________________________")
-        print(df)
+        df['year'] = pd.to_datetime(df.date).apply(lambda x:x.year)
+        df['month'] = pd.to_datetime(df.date).apply(lambda x:x.month)
+        #df.index = df['datetime']
+        #df['priced'] = df.groupby(df['datetime'])['price'].sum()
+        df1 = df.groupby('month', sort=False).agg({'datetime':'last','price':'sum'})# , 'in':'sum','out':'sum'
+        # first by mothn
+        df = df.groupby('datetime',sort=False).agg({'price':'sum', 'in':'sum','out':'sum','year':'first','month':'first'})
+
+        if budget:
+            print("____________________________________")
+            print(df1)#.iloc[-30:-1,:]  )
+            print("____________________________________")
+        print(df.loc[ df['month']==2 ]  )#.iloc[-30:-1,:]  )
         print("____________________________________")
 
+    if budget: return
 
     config.CONFIG["filename"] = "~/.config/cmd_ai/cfg.json"
     config.load_config()
 
+    # ================================= changes to config FROM HERE ==========
+    if limit_tokens is not None:
+        config.CONFIG['limit_tokens'] = limit_tokens
+    print("D... init tokens",config.CONFIG['limit_tokens'] ,  limit_tokens )
+
+
     if config.CONFIG["api_key"] is None:
         res = get_api_key()
         if res is not None:
             config.CONFIG["api_key"] = res
             res = input("> save api_key to config?   y/n")
             if res == "y":
                 print(config.CONFIG["api_key"])
@@ -265,22 +320,22 @@
     config.started_total = dt.datetime.now()
 
     # in CON config.PYSCRIPT = "/tmp/gpt_code.py"
     config.PYSCRIPT_EXISTS = False
     config.SHSCRIPT_EXISTS = False
 
 
-    config.pipeinput = pipe_mode(cmd)
+    config.pipeinput = pipe_mode()
     if config.pipeinput is not None:
         pass
         # system prompt must be linux expert
 
     config.client = OpenAI(api_key=get_api_key())
     config.myPromptSession = PromptSession(
-        history=FileHistory(os.path.expanduser("~/.cmd_ai.history"))
+        history=FileHistory(os.path.expanduser("~/.cmd_ai.history")) #, multiline=True
     )
 
     # config.load_config()
     # config.save_config()
 
     if cmd == "usage":
         print(
@@ -302,26 +357,40 @@
     # for i in models.data:
     #     if i.id.find("gpt") >= 0:
     #         mids.append(i.id)
     # for i in sorted(mids):
     #     print("   ", i)
 
     print("                            ", fg.cyan, ".h for help", fg.default)
-    if cmd == "":
+
+    # DECIDE WHETHER PIPE .....
+
+    # if config.pipeinput is not None:
+    #     print("=========== PIPE ========")
+    # else:
+    #     print("=========== RUN INTERACTIVE ========")
+    # sys.exit(0)
+
+    if config.pipeinput is not None and multilineinput:
+        print(fg.red, "X... no multiline input allowed for PIPE mode") # it crashes
+        sys.exit(1)
+
+    if (config.pipeinput is None) and (cmd is None): #if cmd == "":
+        # print("========================= NONE PIPE MODE ===================")
         while True:
 
             SYSCOM = False
-            inp = config.myPromptSession.prompt("> ")
+            inp = config.myPromptSession.prompt("> ", multiline=multilineinput)
             config.started_task = dt.datetime.now()
 
             #print("D:1")
             inp = inp.strip()
-            if config.CONFIG["current_role"] == "pythonista" and  inp[0]!=".":
+            if config.CONFIG["current_role"] == "pythonista" and  inp[0]!="." and len(inp)>2:
                 inp = f"{inp} (Write python code)."
-            if config.CONFIG["current_role"] == "sheller" and  inp[0]!=".":
+            if config.CONFIG["current_role"] == "sheller" and  inp[0]!="." and len(inp)>2:
                 inp = f"{inp} (Write bash code if needed)."
 
 
             if inp.strip() == "":
                 continue
             if len(inp.strip()) == 1:
                 print(f"!... {fg.red}  one letter prompt not allowed, use .h  {fg.default}")
@@ -334,82 +403,136 @@
             else:
                 config.CONFIG['last_prompt'] = inp
                 #print(fg.white, inp)
             print(fg.default)
 
             if SYSCOM:
                 process_syscom(inp)
+            elif config.CONFIG["current_role"] == "dalle":
+                print("D... in DALLE role ...")
+                res = g_askdalle(inp)
+                print("D...  done:", res)
             else:
-                #print("D:2")
-                res,stoplength = g_askme(inp, model="gpt-4-1106-preview")
-
+                # ================================================vision OR gpt
+                stoplength = False
+                if config.CONFIG["current_role"] == "vision":
+                    print("D... in VISION role ...")
+                    res, stoplength = g_askvision(inp)
+                    #print("D...  done:", res)
+                else:
+                    #print("D:2")
+                    res,stoplength = g_askme(inp, model="gpt-4-1106-preview")
+                # --------------------- and I continue as normal--------------
                 # append the response...
                 config.messages.append( {"role":"assistant", "content":res} ) # always user/assistant
                 # this I want to be json
                 with open( os.path.expanduser( config.CONFIG['current_messages'] ), "w" )  as f:
                     try:
                         f.write( json.dumps( config.messages, indent=2, separators=(',', ': ')) )
                     except:
-                        print(fg.red,f"X... I cannot write json to {config.CONFIG['current_messages']} ")
+                        print(fg.red,f"X... I cannot write {len(config.messages)} messages to json {config.CONFIG['current_messages']}. web content? ")
                     #f.write( str(config.messages) )
 
                 display_response(res)
                 if stoplength:
                     print(f"!... {fg.red} stopped because : not enough tokens, try .l {fg.default}")
-    else:
-        # commandline.  OR pipe on commandline
-        inp = cmd # command
+    else:# cmd is not None:
+        # print("========================= fire and forget mode ===================")
+        # commandline.  OR pipe on commandline ====================================
+        #  this gets more complex with --assistant  SWITCH
+        #
 
+        inp = cmd # command
+        if inp is None: inp = "" # protection for pipe and different assistant
         # for cmdline, I operate the switches here
         if u_switch:
             process_syscom(".u")
         elif g_switch:
             process_syscom(".g")
 
-        if vcs:#_switch:
+        if csspeak:#_switch:
             config.READALOUD = 2 #
-        elif ven:#_switch:
+        elif enspeak:#_switch:
             config.READALOUD = 1 #
         #print("cs=",vcs,"en=",ven)
         #str_to_mp3( "Žluťoučký kůň",  readme=True, lang=config.READALOUDSET[config.READALOUD%len(config.READALOUDSET)])
 
-        print(f"i...  {bg.green}{fg.white} Ubuntu expert {bg.default}{fg.default}")
-        config.messages.append({"role": "system", "content": texts.role_piper})
-        config.CONFIG["current_role"] = "piper"
+        if assistant is None:
+            print(f"i...  {bg.green}{fg.white} Ubuntu expert {bg.default}{fg.default}")
+            config.messages.append({"role": "system", "content": texts.role_piper})
+            config.CONFIG["current_role"] = "piper"
+        else:
+            print(f"i...  {bg.green}{fg.white} {assistant}  {bg.default}{fg.default}")
+            if assistant == "translator":
+                config.messages.append({"role": "system", "content": texts.role_translator})
+            elif assistant == "assistant":
+                config.messages.append({"role": "system", "content": texts.role_assistant})
+            elif assistant == "sheller":
+                config.messages.append({"role": "system", "content": texts.role_sheller})
+            elif assistant == "pythonista":
+                config.messages.append({"role": "system", "content": texts.role_pythonista})
+            elif assistant == "dalle":
+                config.messages.append({"role": "system", "content": texts.role_dalle})
+            elif assistant == "vision":
+                config.messages.append({"role": "system", "content": texts.role_vision})
+            else:
+                print("X... NOT KNOWN ASSISTANT:  translator | assistant | sheller | pythonista | piper | dalle | vision")
+                sys.exit(1)
+            config.CONFIG["current_role"] = assistant
+
 
         if config.pipeinput is not None: # pipe + cmd
-            nl = '\n'.join(config.pipeinput)
+            print(f"i...  {bg.green}{fg.white} Using PIPE {bg.default}{fg.default}")
+            pipe_input = '\n'.join(config.pipeinput)
+            # print(pipe_input)
+            if assistant is None:
+                # (Write bash code if required). ....  ??
+                inp = f"Here is some linux command output:\n```{pipe_input}```\n{inp}"
+            else:
+                # I hope that assistant knows what to do
+                if inp is not None or len(inp)> 0:
+                    print(fg.red,f"i... disregarding text: /{inp}/", fg.default)
+                inp = pipe_input
+        #print(fx.italic,inp, fx.default,"\n")
 
-            # (Write bash code if required).
-            inp = f"Here is some linux command output:\n```{nl}```\n{cmd}"
-            print(f"i...  {bg.green}{fg.white} Pipe expert {bg.default}{fg.default}")
+        if assistant != "dalle":
 
-        #print(fx.italic,inp, fx.default,"\n")
+            res = ""
+            stoplength = False
+            # --------------------------------------------------------
+            if assistant == "vision":
+                res,stoplength = g_askvision(inp)
+            else:
+                res,stoplength = g_askme(inp, model="gpt-4-1106-preview")
 
-        res,stoplength = g_askme(inp, model="gpt-4-1106-preview")
+            #= ----------------------------------------------
+            config.messages.append( {"role":"assistant", "content":res} ) # always user/assistant
+
+            with open( os.path.expanduser( config.CONFIG['current_messages'] ), "w" )  as f:
+                f.write( str(cmd) )
+            display_response(res)
+            if stoplength:
+                print(f"!... {fg.red} stopped because : not enough tokens, try .l {fg.default}")
+
+            if config.SHSCRIPT_EXISTS:
+                click.echo('Run the code? [yn] ', nl=False)
+                c = click.getchar()
+                click.echo()
+                if c == 'y':
+                    click.echo('We will go on')
+                    process_syscom(".e")
+                elif c == 'n':
+                    click.echo('Abort!')
+                else:
+                    click.echo('not n nor y : Abort ')
+                #if click.confirm('Run the code?', abort=True, default=False):
+                #    process_syscom(".e")
+
+        else:
+            res = g_askdalle(inp)
 
-        config.messages.append( {"role":"assistant", "content":res} ) # always user/assistant
 
-        with open( os.path.expanduser( config.CONFIG['current_messages'] ), "w" )  as f:
-            f.write( str(cmd) )
-        display_response(res)
-        if stoplength:
-            print(f"!... {fg.red} stopped because : not enough tokens, try .l {fg.default}")
-
-        if config.SHSCRIPT_EXISTS:
-            click.echo('Run the code? [yn] ', nl=False)
-            c = click.getchar()
-            click.echo()
-            if c == 'y':
-                click.echo('We will go on')
-                process_syscom(".e")
-            elif c == 'n':
-                click.echo('Abort!')
-            else:
-                click.echo('Invalid input :(')
-            #if click.confirm('Run the code?', abort=True, default=False):
-            #    process_syscom(".e")
 
 # ====================================================================
 
 if __name__ == "__main__":
     Fire(main)
```

### Comparing `cmd_ai-0.1.7/cmd_ai/api_key.py` & `cmd_ai-0.2.1/cmd_ai/api_key.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.7/cmd_ai/config.py` & `cmd_ai-0.2.1/cmd_ai/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "pyscript":"/tmp/cmd_ai_code.py",
     "shscript":"/tmp/cmd_ai_bash.py",
     "sourcecode":"/tmp/cmd_ai_sourcecode",
     "sourcecodeext":"txt",
     "current_messages":"/tmp/cmd_ai_messages.txt",
     "last_prompt":"undefined",
     "last_response":"/tmp/cmd_ai_last_response.txt",
-    "conversations":"./conversations.org",
+    "conversations":"~/conversations.org",
     "current_role":"assistant",
     "quit": False,  # this is howto quit
 }
 
 
 # This is the list of all tools - functions available =NEW=
 available_functions = {} # later on we fill
```

### Comparing `cmd_ai-0.1.7/cmd_ai/function_chmi.py` & `cmd_ai-0.2.1/cmd_ai/function_chmi.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.7/cmd_ai/function_goog.py` & `cmd_ai-0.2.1/cmd_ai/function_goog.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.7/cmd_ai/function_webc.py` & `cmd_ai-0.2.1/cmd_ai/function_webc.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.7/cmd_ai/g_askme.py` & `cmd_ai-0.2.1/cmd_ai/g_askme.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,16 @@
         f.write(f"{now} {tokens_in} {tokens_out} {price}")
         f.write("\n")
 
 
 
 ###================================================================================
 
-def g_ask_chat(prompt, temp, model, limit_tokens=300, total_model_tokens=4096 * 2 - 50, tool=False):
+def g_ask_chat(prompt, temp, model,  total_model_tokens=4096 * 2 - 50, tool=False):
+    #
     """
     CORE ChatGPT function
     """
     # global task_assis, limit_tokens
     global GLOBAL_DEPTH # track depth...
 
     # ---- if no system present, add it
@@ -115,15 +116,17 @@
     # add the message~
     if tool:
         config.messages.append( prompt )
     else:
         config.messages.append({"role": "user", "content": prompt})
 
     #max_tokens = total_model_tokens - num_tokens_from_messages()
+    max_tokens = 300 # total_model_tokens - num_tokens_from_messages()
     limit_tokens = config.CONFIG['limit_tokens']
+    print("D... g_ask_chat: conf tokens:", config.CONFIG['limit_tokens'])
     if limit_tokens < 30000: # ;max_tokens
         max_tokens = limit_tokens
     print(
         f"i...  {fx.italic}{fg.lightslategray}max_tokens: {max_tokens}, model: {model};  {fg.default}"
     )
     # DEBUG PURPLE
     #print(fg.lightpurple,config.messages,fg.default)
@@ -447,22 +450,25 @@
 }
 
 
 def g_askme(
         prompt,
         temp=0.0,
         model="gpt-4-1106-preview",
-        limit_tokens=300,
+        # limit_tokens=300,
         total_model_tokens=4096 * 2 - 50, # guess
         tool = False
 ):
-
+    """
+    CALL g_ask_chat()
+    """
     #estimate_tokens = num_tokens_from_messages() + len(prompt) + 600
     #estimate_tokens = 300
     estimate_tokens = config.CONFIG['limit_tokens']
+    print("D....  g_ask estimate tokens", estimate_tokens)
     resdi = g_ask_chat(
         prompt, temp, model, estimate_tokens, tool=tool
     )
 
     if resdi is None:
         return None
     return resdi
```

### Comparing `cmd_ai-0.1.7/cmd_ai/key_enter.py` & `cmd_ai-0.2.1/cmd_ai/key_enter.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.7/cmd_ai/pipe.py` & `cmd_ai-0.2.1/cmd_ai/pipe.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.7/cmd_ai/speak.py` & `cmd_ai-0.2.1/cmd_ai/speak.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.7/cmd_ai/syscom.py` & `cmd_ai-0.2.1/cmd_ai/syscom.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 We create a unit, that will be the test_ unit by ln -s simoultaneously. Runs with 'pytest'
 """
 import sys
 import subprocess as sp
 from console import fg,bg,fx
 from fire import Fire
 import os
-from cmd_ai import config, texts
+from cmd_ai import config, texts, best_examples
 from cmd_ai.version import __version__
 import json
 # print("v... unit 'unitname' loaded, version:",__version__)
 
 
 def process_syscom(cmd):
 
     # ***************************************
     if cmd.strip() == ".q":
         sys.exit(0)
 
     # ***************************************
     elif cmd.strip() == ".h":
         print(texts.HELP)
+        print("_______________")
+        print(best_examples.main())
 
     # ***************************************
     elif cmd.strip() == ".c":
         mmm = config.CONFIG["current_messages"]
         print(f"i... {fg.pink} .. I try to catch up with  {mmm} ... {fg.default}")
         CONT = []
         if os.path.exists(mmm):
@@ -65,14 +67,18 @@
                 print(" ... extension to process :  ",config.CONFIG['sourcecodeext'])
                 if config.CONFIG['sourcecodeext']=="dot":
                     sp.run(['dot','-Tpng', OUTFILE, "-o", "dot.png"])
                     #dot -Tpng dd.dot -o dd.png
                 elif config.CONFIG['sourcecodeext']=="python":
                     sp.run(['python3', OUTFILE ])
                     #dot -Tpng dd.dot -o dd.png
+                elif config.CONFIG['sourcecodeext']=="bash":
+                    sp.run(['chmod','+x', OUTFILE ])
+                    sp.run(['bash','-c', OUTFILE ])
+                    #dot -Tpng dd.dot -o dd.png
                 else:
                     print("X... undefined extension")
             else:
                 print(f"X... file {OUTFILE} not found")
 
     # ***************************************
     elif cmd.strip() == ".r":
@@ -113,23 +119,29 @@
     # *************************************** shell expert
     elif cmd.strip() == ".s":
         print(f"i...  {bg.green}{fg.white} Shell expert {bg.default}{fg.default}")
         config.messages.append({"role": "system", "content": texts.role_sheller})
         config.CONFIG["current_role"] = "sheller"
 
 
-    # *************************************** dalle
+    # *************************************** dalle - no need of content....
     elif cmd.strip() == ".d":
-        print(f"i...  {bg.green}{fg.white} NO Dalle expert {bg.default}{fg.default}")
+        print(f"i...  {bg.green}{fg.white} DALLE expert {bg.default}{fg.default}")
         config.messages.append({"role": "system", "content": texts.role_dalle})
         config.CONFIG["current_role"] = "dalle"
 
-    # *************************************** tramslator
+    # *************************************** vision ... no need of content...
+    elif cmd.strip() == ".i":
+        print(f"i...  {bg.green}{fg.white} VISION expert {bg.default}{fg.default}")
+        config.messages.append({"role": "system", "content": texts.role_vision})
+        config.CONFIG["current_role"] = "vision"
+
+    # *************************************** translator
     elif cmd.strip() == ".t":
-        print(f"i...  {bg.green}{fg.white} NO Translator from english to czech {bg.default}{fg.default}")
+        print(f"i...  {bg.green}{fg.white} Translator from english to czech {bg.default}{fg.default}")
         config.messages.append({"role": "system", "content": texts.role_translator})
         config.CONFIG["current_role"] = "translator"
 
     # *************************************** assistant
     elif cmd.strip() == ".a":
         print(f"i...  {bg.green}{fg.white} Brief assistant {bg.default}{fg.default}")
         config.messages.append({"role": "system", "content": texts.role_assistant})
```

### Comparing `cmd_ai-0.1.7/cmd_ai/texts.py` & `cmd_ai-0.2.1/cmd_ai/texts.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,17 @@
 .u      add other functions ... CHMI weather (test)
 .v      read the answer aloud
 .c      catch up messages after crash...
 ________________ ROLES _______________
 .a   assistent (default in INTERACTIVE and CMDLINE)
 .p   python coder
 .s   shell expert (default in PIPE)
-.d   NO dalle yet
-.t   NO translator yet
-________________ SPECIAL MODELS _____
-.i   NO use dalle yet
-.v   NO use vision yet
+.d   dalle 3 ... most exact prompt variant
+.t   translator
+.i   use vision - low detail
 """
 
 
 
 
 
 #######################################################################
@@ -95,31 +93,35 @@
 role_assistant = """You are the assistant that responds questions correctly and fulfills given tasks. You use a short and brief language, you do not repeat yourself nor the users' questions. You make the answers short but precise."""
 
 # The code must be always safe and secure, no harm for the filesystem nor for the network.
 role_pythonista = """You are PYTHON program writer. The prompts instruct you to create a python code. The code must be able to run from the commandline, for this use Fire and default values. For graphs, use matplotlib. You use a short and brief language. Never repeat user questions. Make the answers short but precise. Do not give examples how to run the code from shell. Never use example paths e.g. '/path/to/', if not specified, use the current directory. Provide maximum ONE code block per response. Do not show how to install packages, unless explicitelly asked."""
 
 
 
-role_translator = """ You translate scientific text prompts from English to Czech. Use clean and concise language. Reformulate the translated text to be clean and fluent.
+role_translator = """ You translate scientific text prompts from English to Czech. Use clean and concise language. Reformulate the translated text clean and fluent.
 It contains specific nuclear physics terminology so
  - "beam" means "svazek" in Czech
  - "target" means "terč" in Czech
  - "beam time" means "urychlovačový čas" in Czech
  - "beam dump" means "zařízení pro zastavení svazku" in Czech
  - "is promissing" mean "je slibná" or "je slibný" in Czech
+ In a case I give you a text in SRT subtitles format : `line_number \n time-start --> time-end \n some_sentence(s) \n\n`. The time is in the format of srt: hh:mm:ss,fff - in that case you keep the format exactly he same and translate the sentences to czech.
 """
 
 #  and secure, no harm for the filesystem nor for the network
 role_sheller = """ You are an Ubuntu 22 commandline and bash expert. The code must be always safe. You use a short and brief language. Do not repeat the user questions.  Do not repeat yourself. You make the answers short but precise. Only shell code, no examples how to run. Never use example paths e.g. '/path/to/', if not specified, use the current directory. One code block per response maximum.
 """
 
 #  and secure, no harm for the filesystem nor for the network
 role_piper = """ You are an Ubuntu 22 commandline and bash expert. But not only. You use a short and brief language. Do not repeat the user questions.  Do not repeat yourself. You make the answers short but precise. No examples how to run. Never use example paths e.g. '/path/to/', '/path/to/search', replace it with the current directory.
 """
 
+role_dalle = """I NEED to test how the tool works with extremely simple prompts. DO NOT add any detail, just use it AS-IS:"""
+
+role_vision = """What is in the picture?"""
 
 #######################################################################
 #     O R G
 #######################################################################
 
 
 org_header = r"""
```

### Comparing `cmd_ai-0.1.7/cmd_ai/topbar.py` & `cmd_ai-0.2.1/cmd_ai/topbar.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.7/cmd_ai/unitname.py` & `cmd_ai-0.2.1/cmd_ai/unitname.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.1.7/cmd_ai.egg-info/PKG-INFO` & `cmd_ai-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-Metadata-Version: 2.1
-Name: cmd-ai
-Version: 0.1.7
-Summary: Another ChatGTP project in commandline of linux
-Home-page: http://gitlab.com/me/cmd_ai
-Author: jaromrax
-Author-email: jaromrax@gmail.com
-License: GPL2
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 Project cmd~ai~
 ===============
 
 *Another ChatGPT project that implements as a shell interface*
 
 README for version `0.0.8`
 
 EXAMPLE
 -------
 
 `cmd_ai "Jak bude zitra (pouze) ve Stredoceskem kraji?" -u -vcs`
 
+`cmd_ai -a dalle "Landscape with hills and lakes, photographic quality"`
+
 Installation
 ------------
 
 It should work with `pip3 install`, not tested yet.
 
 Needs `API_KEY` for OpenAI in `~/.openai.token` , than it creates own
 copy at `~/.config/cmd_ai/cfg.json`
@@ -48,15 +39,15 @@
 .e      execute code
 .r      reset messages, scripts
 .l      show tokens
 .m      show models
 .l number ... change limit tokens
 ________________ ROLES _____________
 .a   assistent
-.t   NO translator
+.t   translator
 .p   python coder
 .s   shell expert
 .d   NO dalle
 ________________ MODEL
 .i   NO use dalle
 .v   NO use vision
 ```
@@ -75,14 +66,18 @@
 Similar but for bash
 
 ### Piper
 
 Works only from commandline, when pipe (stdin) is detected. No memory,
 on task/question, asks before runs the code
 
+### Dalle
+
+Gets one image, 1024x1024, restricted prompt rewrite
+
 1.  [DONE]{.done .DONE} Commit message example
 
     ``` {.example}
     git diff | ai 'write a commit message, show it as git commit -a -m "message" command'
     ```
 
 DOING Function calls / tools
@@ -102,21 +97,19 @@
 ### WAITING Document upload
 
 -   it costs 0.20\$ per 1GB per day....
 
 Images
 ------
 
-### POSTPONED Dalle3
+### [DONE]{.done .DONE} Dalle3 {#dalle3}
 
-I need to test if this works or what
+First attmpt works also in cmdline (-a dalle)
 
 ### [TODO]{.todo .TODO} Upload for analysis to GPT-v {#upload-for-analysis-to-gpt-v}
 
 That would be interesting from commandline
 
 Dependencies
 ============
 
 -   googlesearch-python
-
-
```

### Comparing `cmd_ai-0.1.7/setup.py` & `cmd_ai-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,9 +36,9 @@
     license="GPL2",
     version=get_version("cmd_ai/version.py"),
     packages=["cmd_ai"],
     package_data={"cmd_ai": ["data/*"]},
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     scripts=["bin/cmd_ai"],
-    install_requires=["fire", "console", "click", "pandas", "openai", "prompt_toolkit","googlesearch-python"],
+    install_requires=["fire", "console", "click", "pandas", "openai", "prompt_toolkit","googlesearch-python","playsound","unidecode"],
 )
```

