# Comparing `tmp/naver_email_verifier-1.0.1.tar.gz` & `tmp/naver_email_verifier-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naver_email_verifier-1.0.1.tar", last modified: Thu Apr 18 05:44:54 2024, max compression
+gzip compressed data, was "naver_email_verifier-1.0.2.tar", last modified: Thu Apr 18 05:50:34 2024, max compression
```

## Comparing `naver_email_verifier-1.0.1.tar` & `naver_email_verifier-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 05:44:54.652297 naver_email_verifier-1.0.1/
--rw-rw-rw-   0        0        0     1089 2024-04-18 05:16:40.000000 naver_email_verifier-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      206 2024-04-18 05:44:54.651449 naver_email_verifier-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1427 2024-04-18 05:43:14.000000 naver_email_verifier-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 05:44:54.630366 naver_email_verifier-1.0.1/naver_email_verifier/
-drwxrwxrwx   0        0        0        0 2024-04-18 05:44:54.649399 naver_email_verifier-1.0.1/naver_email_verifier/__pycache__/
--rw-rw-rw-   0        0        0      176 2024-04-18 04:43:03.000000 naver_email_verifier-1.0.1/naver_email_verifier/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3906 2024-04-18 05:40:59.000000 naver_email_verifier-1.0.1/naver_email_verifier/__pycache__/verifier.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-18 05:44:54.647400 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/
--rw-rw-rw-   0        0        0      206 2024-04-18 05:44:54.000000 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-18 05:44:54.000000 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:44:54.000000 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-18 05:44:54.000000 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-18 05:44:54.000000 naver_email_verifier-1.0.1/naver_email_verifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 05:44:54.652297 naver_email_verifier-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      716 2024-04-18 05:43:30.000000 naver_email_verifier-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:50:34.917383 naver_email_verifier-1.0.2/
+-rw-rw-rw-   0        0        0     1089 2024-04-18 05:16:40.000000 naver_email_verifier-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      431 2024-04-18 05:50:34.915825 naver_email_verifier-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1427 2024-04-18 05:43:14.000000 naver_email_verifier-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 05:50:34.895254 naver_email_verifier-1.0.2/naver_email_verifier/
+drwxrwxrwx   0        0        0        0 2024-04-18 05:50:34.914818 naver_email_verifier-1.0.2/naver_email_verifier/__pycache__/
+-rw-rw-rw-   0        0        0      176 2024-04-18 04:43:03.000000 naver_email_verifier-1.0.2/naver_email_verifier/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4135 2024-04-18 05:45:00.000000 naver_email_verifier-1.0.2/naver_email_verifier/__pycache__/verifier.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-18 05:50:34.911788 naver_email_verifier-1.0.2/naver_email_verifier.egg-info/
+-rw-rw-rw-   0        0        0      431 2024-04-18 05:50:34.000000 naver_email_verifier-1.0.2/naver_email_verifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-18 05:50:34.000000 naver_email_verifier-1.0.2/naver_email_verifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:50:34.000000 naver_email_verifier-1.0.2/naver_email_verifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 05:50:34.000000 naver_email_verifier-1.0.2/naver_email_verifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-18 05:50:34.000000 naver_email_verifier-1.0.2/naver_email_verifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 05:50:34.917383 naver_email_verifier-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      971 2024-04-18 05:50:14.000000 naver_email_verifier-1.0.2/setup.py
```

### Comparing `naver_email_verifier-1.0.1/LICENSE` & `naver_email_verifier-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `naver_email_verifier-1.0.1/README.md` & `naver_email_verifier-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `naver_email_verifier-1.0.1/naver_email_verifier/__pycache__/verifier.cpython-311.pyc` & `naver_email_verifier-1.0.2/naver_email_verifier/__pycache__/verifier.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xdfad2066 (Thu Apr 18 05:21:35 2024 UTC)
-files sz: 2651
+moddate:  0x44b32066 (Thu Apr 18 05:44:36 2024 UTC)
+files sz: 2837
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a0102004700640284006403a6
@@ -56,16 +56,16 @@
                       18 STORE_NAME               4 (__init__)
          
           37          20 LOAD_CONST               6 ((None,))
                       22 LOAD_CONST               4 (<code object is_id_in_use_sync, file "D:\Dev\Python\naver_email_verifier\naver_email_verifier\verifier.py", line 37>)
                       24 MAKE_FUNCTION            1 (defaults)
                       26 STORE_NAME               5 (is_id_in_use_sync)
          
-          51          28 LOAD_CONST               6 ((None,))
-                      30 LOAD_CONST               5 (<code object is_id_in_use_async, file "D:\Dev\Python\naver_email_verifier\naver_email_verifier\verifier.py", line 51>)
+          54          28 LOAD_CONST               6 ((None,))
+                      30 LOAD_CONST               5 (<code object is_id_in_use_async, file "D:\Dev\Python\naver_email_verifier\naver_email_verifier\verifier.py", line 54>)
                       32 MAKE_FUNCTION            1 (defaults)
                       34 STORE_NAME               6 (is_id_in_use_async)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
          consts
             'NaverChecker'
             '\n    네이버 이메일 사용자 ID 사용 여부를 확인하는 클래스입니다.\n\n    이 클래스의 인스턴스는 내부적으로 `httpx.Client`를 사용하여 네이버에 HTTP 요청을 보냅니다.\n    클라이언트는 인스턴스가 소멸될 때까지 오픈 상태로 유지되며, 모든 요청에 대해 10초의 타임아웃이 설정됩니다.\n\n    이메일 ID가 이미 사용 중이라면 `is_id_in_use` 메소드는 `True`를 반환합니다.\n    하지만 이 결과가 100% 정확하다고 테스트는 못했으며, 일반적으로 잘 작동하는 것으로 확인되었습니다.\n\n    SMTP로 이메일 보내기 전에 간단하게 체크하기 좋습니다.\n\n    사용 예:\n    ```python\n    checker = NaverChecker()\n    is_used = checker.is_id_in_use("example_user_id")\n    print("존재하는 계정 입니다." if is_used else "존재 하지 않는 계정 입니다.")\n    ```\n    '
@@ -180,20 +180,22 @@
                nlocals   : 4
                stacksize : 7
                flags     : 3
                code
                   0x97007c0280077c006a0000000000000000007d027c006a010000000000
                   0000006a020000000000000000721a7407000000000000000000006a0400
                   000000000000006402ac03a6010000ab0100000000000000007c005f0100
-                  000000000000007c006a010000000000000000a005000000000000000000
-                  00000000000000000000007c006a06000000000000000064047c02690164
-                  057c0164069c02ac07a6030000ab0300000000000000007d037c036a0700
-                  00000000000000a0080000000000000000000000000000000000000000a6
-                  000000ab000000000000000000a009000000000000000000000000000000
-                  00000000006408a6010000ab0100000000000000005300
+                  0000000000000064047c017600721b7c01a0050000000000000000000000
+                  0000000000000000006404a6010000ab0100000000000000006405190000
+                  000000000000007d017c006a010000000000000000a00600000000000000
+                  000000000000000000000000007c006a07000000000000000064067c0269
+                  0164077c0164089c02ac09a6030000ab0300000000000000007d037c036a
+                  080000000000000000a00900000000000000000000000000000000000000
+                  00a6000000ab000000000000000000a00a00000000000000000000000000
+                  00000000000000640aa6010000ab0100000000000000005300
                 37           0 RESUME                   0
                
                 39           2 LOAD_FAST                2 (user_agent)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
                 40           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (user_agent)
@@ -209,168 +211,202 @@
                             66 LOAD_CONST               2 (10.0)
                             68 KW_NAMES                 3
                             70 PRECALL                  1
                             74 CALL                     1
                             84 LOAD_FAST                0 (self)
                             86 STORE_ATTR               1 (client)
                
-                44     >>   96 LOAD_FAST                0 (self)
-                            98 LOAD_ATTR                1 (client)
-                           108 LOAD_METHOD              5 (get)
-               
-                45         130 LOAD_FAST                0 (self)
-                           132 LOAD_ATTR                6 (base_url)
-               
-                46         142 LOAD_CONST               4 ('User-Agent')
-                           144 LOAD_FAST                2 (user_agent)
-                           146 BUILD_MAP                1
-               
-                47         148 LOAD_CONST               5 ('checkId')
-                           150 LOAD_FAST                1 (user_id)
-                           152 LOAD_CONST               6 (('m', 'id'))
-                           154 BUILD_CONST_KEY_MAP      2
-               
-                44         156 KW_NAMES                 7
-                           158 PRECALL                  3
-                           162 CALL                     3
-                           172 STORE_FAST               3 (response)
-               
-                49         174 LOAD_FAST                3 (response)
-                           176 LOAD_ATTR                7 (text)
-                           186 LOAD_METHOD              8 (strip)
-                           208 PRECALL                  0
-                           212 CALL                     0
-                           222 LOAD_METHOD              9 (endswith)
-                           244 LOAD_CONST               8 ('N')
-                           246 PRECALL                  1
-                           250 CALL                     1
-                           260 RETURN_VALUE
+                44     >>   96 LOAD_CONST               4 ('@naver.com')
+                            98 LOAD_FAST                1 (user_id)
+                           100 CONTAINS_OP              0
+                           102 POP_JUMP_FORWARD_IF_FALSE    27 (to 158)
+               
+                45         104 LOAD_FAST                1 (user_id)
+                           106 LOAD_METHOD              5 (split)
+                           128 LOAD_CONST               4 ('@naver.com')
+                           130 PRECALL                  1
+                           134 CALL                     1
+                           144 LOAD_CONST               5 (0)
+                           146 BINARY_SUBSCR
+                           156 STORE_FAST               1 (user_id)
+               
+                47     >>  158 LOAD_FAST                0 (self)
+                           160 LOAD_ATTR                1 (client)
+                           170 LOAD_METHOD              6 (get)
+               
+                48         192 LOAD_FAST                0 (self)
+                           194 LOAD_ATTR                7 (base_url)
+               
+                49         204 LOAD_CONST               6 ('User-Agent')
+                           206 LOAD_FAST                2 (user_agent)
+                           208 BUILD_MAP                1
+               
+                50         210 LOAD_CONST               7 ('checkId')
+                           212 LOAD_FAST                1 (user_id)
+                           214 LOAD_CONST               8 (('m', 'id'))
+                           216 BUILD_CONST_KEY_MAP      2
+               
+                47         218 KW_NAMES                 9
+                           220 PRECALL                  3
+                           224 CALL                     3
+                           234 STORE_FAST               3 (response)
+               
+                52         236 LOAD_FAST                3 (response)
+                           238 LOAD_ATTR                8 (text)
+                           248 LOAD_METHOD              9 (strip)
+                           270 PRECALL                  0
+                           274 CALL                     0
+                           284 LOAD_METHOD             10 (endswith)
+                           306 LOAD_CONST              10 ('N')
+                           308 PRECALL                  1
+                           312 CALL                     1
+                           322 RETURN_VALUE
                consts
                   'Synchronously checks the availability of a user ID.'
                   None
                   10.0
                   ('timeout',)
+                  '@naver.com'
+                  0
                   'User-Agent'
                   'checkId'
                   ('m', 'id')
                   ('headers', 'params')
                   'N'
-               names      ('user_agent', 'client', 'is_closed', 'httpx', 'Client', 'get', 'base_url', 'text', 'strip', 'endswith')
+               names      ('user_agent', 'client', 'is_closed', 'httpx', 'Client', 'split', 'get', 'base_url', 'text', 'strip', 'endswith')
                varnames   ('self', 'user_id', 'user_agent', 'response')
                freevars   ()
                cellvars   ()
                filename   'D:\\Dev\\Python\\naver_email_verifier\\naver_email_verifier\\verifier.py'
                name       'is_id_in_use_sync'
                firstlineno 37
-               lnotab 0x020204010e011801340222010c01060108fd1205
+               lnotab 0x020204010e01180134020801360222010c01060108fd1205
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 7
                flags     : 131
                code
                   0x4b00010097007c0280077c006a0000000000000000007d027c006a0100
                   000000000000006a020000000000000000721a7407000000000000000000
                   006a0400000000000000006402ac03a6010000ab0100000000000000007c
-                  005f0100000000000000007c006a010000000000000000a0050000000000
-                  0000000000000000000000000000007c006a06000000000000000064047c
-                  02690164057c0164069c02ac07a6030000ab030000000000000000830064
-                  017b035600970386047d037c036a070000000000000000a0080000000000
-                  000000000000000000000000000000a6000000ab000000000000000000a0
-                  0900000000000000000000000000000000000000006408a6010000ab0100
-                  000000000000005300
-                51           0 RETURN_GENERATOR
+                  005f01000000000000000064047c017600721b7c01a00500000000000000
+                  000000000000000000000000006404a6010000ab01000000000000000064
+                  05190000000000000000007d017c006a010000000000000000a006000000
+                  00000000000000000000000000000000007c006a07000000000000000064
+                  067c02690164077c0164089c02ac09a6030000ab03000000000000000083
+                  0064017b035600970386047d037c036a080000000000000000a009000000
+                  0000000000000000000000000000000000a6000000ab0000000000000000
+                  00a00a0000000000000000000000000000000000000000640aa6010000ab
+                  0100000000000000005300
+                54           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                53           6 LOAD_FAST                2 (user_agent)
+                56           6 LOAD_FAST                2 (user_agent)
                              8 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 24)
                
-                54          10 LOAD_FAST                0 (self)
+                57          10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (user_agent)
                             22 STORE_FAST               2 (user_agent)
                
-                55     >>   24 LOAD_FAST                0 (self)
+                58     >>   24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                1 (async_client)
                             36 LOAD_ATTR                2 (is_closed)
                             46 POP_JUMP_FORWARD_IF_FALSE    26 (to 100)
                
-                56          48 LOAD_GLOBAL              7 (NULL + httpx)
+                59          48 LOAD_GLOBAL              7 (NULL + httpx)
                             60 LOAD_ATTR                4 (AsyncClient)
                             70 LOAD_CONST               2 (10.0)
                             72 KW_NAMES                 3
                             74 PRECALL                  1
                             78 CALL                     1
                             88 LOAD_FAST                0 (self)
                             90 STORE_ATTR               1 (async_client)
                
-                58     >>  100 LOAD_FAST                0 (self)
-                           102 LOAD_ATTR                1 (async_client)
-                           112 LOAD_METHOD              5 (get)
-               
-                59         134 LOAD_FAST                0 (self)
-                           136 LOAD_ATTR                6 (base_url)
-               
-                60         146 LOAD_CONST               4 ('User-Agent')
-                           148 LOAD_FAST                2 (user_agent)
-                           150 BUILD_MAP                1
-               
-                61         152 LOAD_CONST               5 ('checkId')
-                           154 LOAD_FAST                1 (user_id)
-                           156 LOAD_CONST               6 (('m', 'id'))
-                           158 BUILD_CONST_KEY_MAP      2
-               
-                58         160 KW_NAMES                 7
-                           162 PRECALL                  3
-                           166 CALL                     3
-                           176 GET_AWAITABLE            0
-                           178 LOAD_CONST               1 (None)
-                       >>  180 SEND                     3 (to 188)
-                           182 YIELD_VALUE
-                           184 RESUME                   3
-                           186 JUMP_BACKWARD_NO_INTERRUPT     4 (to 180)
-                       >>  188 STORE_FAST               3 (response)
-               
-                63         190 LOAD_FAST                3 (response)
-                           192 LOAD_ATTR                7 (text)
-                           202 LOAD_METHOD              8 (strip)
-                           224 PRECALL                  0
-                           228 CALL                     0
-                           238 LOAD_METHOD              9 (endswith)
-                           260 LOAD_CONST               8 ('N')
-                           262 PRECALL                  1
-                           266 CALL                     1
-                           276 RETURN_VALUE
+                61     >>  100 LOAD_CONST               4 ('@naver.com')
+                           102 LOAD_FAST                1 (user_id)
+                           104 CONTAINS_OP              0
+                           106 POP_JUMP_FORWARD_IF_FALSE    27 (to 162)
+               
+                62         108 LOAD_FAST                1 (user_id)
+                           110 LOAD_METHOD              5 (split)
+                           132 LOAD_CONST               4 ('@naver.com')
+                           134 PRECALL                  1
+                           138 CALL                     1
+                           148 LOAD_CONST               5 (0)
+                           150 BINARY_SUBSCR
+                           160 STORE_FAST               1 (user_id)
+               
+                64     >>  162 LOAD_FAST                0 (self)
+                           164 LOAD_ATTR                1 (async_client)
+                           174 LOAD_METHOD              6 (get)
+               
+                65         196 LOAD_FAST                0 (self)
+                           198 LOAD_ATTR                7 (base_url)
+               
+                66         208 LOAD_CONST               6 ('User-Agent')
+                           210 LOAD_FAST                2 (user_agent)
+                           212 BUILD_MAP                1
+               
+                67         214 LOAD_CONST               7 ('checkId')
+                           216 LOAD_FAST                1 (user_id)
+                           218 LOAD_CONST               8 (('m', 'id'))
+                           220 BUILD_CONST_KEY_MAP      2
+               
+                64         222 KW_NAMES                 9
+                           224 PRECALL                  3
+                           228 CALL                     3
+                           238 GET_AWAITABLE            0
+                           240 LOAD_CONST               1 (None)
+                       >>  242 SEND                     3 (to 250)
+                           244 YIELD_VALUE
+                           246 RESUME                   3
+                           248 JUMP_BACKWARD_NO_INTERRUPT     4 (to 242)
+                       >>  250 STORE_FAST               3 (response)
+               
+                69         252 LOAD_FAST                3 (response)
+                           254 LOAD_ATTR                8 (text)
+                           264 LOAD_METHOD              9 (strip)
+                           286 PRECALL                  0
+                           290 CALL                     0
+                           300 LOAD_METHOD             10 (endswith)
+                           322 LOAD_CONST              10 ('N')
+                           324 PRECALL                  1
+                           328 CALL                     1
+                           338 RETURN_VALUE
                consts
                   'Asynchronously checks the availability of a user ID.'
                   None
                   10.0
                   ('timeout',)
+                  '@naver.com'
+                  0
                   'User-Agent'
                   'checkId'
                   ('m', 'id')
                   ('headers', 'params')
                   'N'
-               names      ('user_agent', 'async_client', 'is_closed', 'httpx', 'AsyncClient', 'get', 'base_url', 'text', 'strip', 'endswith')
+               names      ('user_agent', 'async_client', 'is_closed', 'httpx', 'AsyncClient', 'split', 'get', 'base_url', 'text', 'strip', 'endswith')
                varnames   ('self', 'user_id', 'user_agent', 'response')
                freevars   ()
                cellvars   ()
                filename   'D:\\Dev\\Python\\naver_email_verifier\\naver_email_verifier\\verifier.py'
                name       'is_id_in_use_async'
-               firstlineno 51
-               lnotab 0x060204010e011801340222010c01060108fd1e05
+               firstlineno 54
+               lnotab 0x060204010e01180134020801360222010c01060108fd1e05
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', 'is_id_in_use_sync', 'is_id_in_use_async')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\Dev\\Python\\naver_email_verifier\\naver_email_verifier\\verifier.py'
          name       'NaverChecker'
          firstlineno 6
-         lnotab 0x0a010413060b080e
+         lnotab 0x0a010413060b0811
       'NaverChecker'
    names      ('base64', 'httpx', 'NaverChecker')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\Dev\\Python\\naver_email_verifier\\naver_email_verifier\\verifier.py'
    name       '<module>'
```

### Comparing `naver_email_verifier-1.0.1/setup.py` & `naver_email_verifier-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,25 @@
             package = dirpath.replace(os.path.sep, ".")
             packages.append(package)
     return packages
 
 
 setup(
     name="naver_email_verifier",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_pyc_packages(),
     package_data={"": ["*.pyc"]},
     exclude_package_data={"": ["*.py"]},
     install_requires=[
         "httpx",
     ],
     author="Seok Won Choi",
     author_email="ikr@kakao.com",
     description="A Python library for verifying Naver email addresses.",
+    url="https://github.com/Alfex4936/naver-email-verifier",
+    license="MIT",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
 )
```

