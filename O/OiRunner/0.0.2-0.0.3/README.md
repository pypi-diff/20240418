# Comparing `tmp/OiRunner-0.0.2.tar.gz` & `tmp/oirunner-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OiRunner-0.0.2.tar", last modified: Sun Mar 31 03:55:38 2024, max compression
+gzip compressed data, was "oirunner-0.0.3.tar", last modified: Thu Apr 18 06:41:19 2024, max compression
```

## Comparing `OiRunner-0.0.2.tar` & `oirunner-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,40 @@
-drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-31 03:55:38.780882 OiRunner-0.0.2/
--rw-rw-r--   0 ste1      (1000) ste1      (1000)     3093 2024-03-31 00:03:36.000000 OiRunner-0.0.2/.gitignore
--rw-rw-r--   0 ste1      (1000) ste1      (1000)     1063 2024-03-30 14:51:20.000000 OiRunner-0.0.2/LICENSE
--rw-rw-r--   0 ste1      (1000) ste1      (1000)       33 2024-03-30 23:51:49.000000 OiRunner-0.0.2/MANIFEST.in
-drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-31 03:55:38.779882 OiRunner-0.0.2/OiRunner/
--rw-rw-r--   0 ste1      (1000) ste1      (1000)        0 2024-03-30 15:11:27.000000 OiRunner-0.0.2/OiRunner/__init__.py
--rw-rw-r--   0 ste1      (1000) ste1      (1000)     8789 2024-03-31 03:38:04.000000 OiRunner-0.0.2/OiRunner/run.py
-drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-31 03:55:38.779882 OiRunner-0.0.2/OiRunner.egg-info/
--rw-r--r--   0 ste1      (1000) ste1      (1000)      270 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/PKG-INFO
--rw-rw-r--   0 ste1      (1000) ste1      (1000)      264 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/SOURCES.txt
--rw-rw-r--   0 ste1      (1000) ste1      (1000)        1 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/dependency_links.txt
--rw-rw-r--   0 ste1      (1000) ste1      (1000)       44 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/entry_points.txt
--rw-rw-r--   0 ste1      (1000) ste1      (1000)        9 2024-03-31 03:55:38.000000 OiRunner-0.0.2/OiRunner.egg-info/top_level.txt
--rw-r--r--   0 ste1      (1000) ste1      (1000)      270 2024-03-31 03:55:38.779882 OiRunner-0.0.2/PKG-INFO
--rw-rw-r--   0 ste1      (1000) ste1      (1000)       46 2024-03-30 14:51:20.000000 OiRunner-0.0.2/README.md
--rw-rw-r--   0 ste1      (1000) ste1      (1000)       99 2024-03-30 15:13:42.000000 OiRunner-0.0.2/pyproject.toml
--rw-rw-r--   0 ste1      (1000) ste1      (1000)       38 2024-03-31 03:55:38.780882 OiRunner-0.0.2/setup.cfg
--rw-rw-r--   0 ste1      (1000) ste1      (1000)      504 2024-03-31 03:55:11.000000 OiRunner-0.0.2/setup.py
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-18 06:41:19.856913 oirunner-0.0.3/
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)     3103 2024-04-11 06:52:11.000000 oirunner-0.0.3/.gitignore
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)     1063 2024-03-30 14:51:20.000000 oirunner-0.0.3/LICENSE
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       33 2024-03-30 23:51:49.000000 oirunner-0.0.3/MANIFEST.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)      485 2024-04-11 03:51:13.000000 oirunner-0.0.3/Makefile
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-18 06:41:19.853913 oirunner-0.0.3/OiRunner/
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)     8995 2024-04-14 08:37:22.000000 oirunner-0.0.3/OiRunner/BetterRunner.py
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-30 15:11:27.000000 oirunner-0.0.3/OiRunner/__init__.py
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-18 06:41:19.856913 oirunner-0.0.3/OiRunner.egg-info/
+-rw-r--r--   0 ste1      (1000) ste1      (1000)      270 2024-04-18 06:41:19.000000 oirunner-0.0.3/OiRunner.egg-info/PKG-INFO
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)      712 2024-04-18 06:41:19.000000 oirunner-0.0.3/OiRunner.egg-info/SOURCES.txt
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)        1 2024-04-18 06:41:19.000000 oirunner-0.0.3/OiRunner.egg-info/dependency_links.txt
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       53 2024-04-18 06:41:19.000000 oirunner-0.0.3/OiRunner.egg-info/entry_points.txt
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       15 2024-04-18 06:41:19.000000 oirunner-0.0.3/OiRunner.egg-info/top_level.txt
+-rw-r--r--   0 ste1      (1000) ste1      (1000)      270 2024-04-18 06:41:19.856913 oirunner-0.0.3/PKG-INFO
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       46 2024-03-30 14:51:20.000000 oirunner-0.0.3/README.md
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       99 2024-03-30 15:13:42.000000 oirunner-0.0.3/pyproject.toml
+-rw-rw-r--   0 ste1      (1000) ste1      (1000)       38 2024-04-18 06:41:19.856913 oirunner-0.0.3/setup.cfg
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)      513 2024-04-18 06:40:49.000000 oirunner-0.0.3/setup.py
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-18 06:41:19.854913 oirunner-0.0.3/tests/
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-03-31 13:34:05.000000 oirunner-0.0.3/tests/__init__.py
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-18 06:41:19.855913 oirunner-0.0.3/tests/data/
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       25 2024-04-07 08:13:00.000000 oirunner-0.0.3/tests/data/a.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)      205 2024-04-11 05:47:40.000000 oirunner-0.0.3/tests/data/check.cpp
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)    26344 2024-04-11 06:51:41.000000 oirunner-0.0.3/tests/data/check.out
+drwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-18 06:41:19.855913 oirunner-0.0.3/tests/data/check_data/
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        1 2024-04-11 05:50:21.000000 oirunner-0.0.3/tests/data/check_data/1.ans
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        2 2024-04-11 05:50:18.000000 oirunner-0.0.3/tests/data/check_data/1.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-11 06:54:28.000000 oirunner-0.0.3/tests/data/check_data/1.out
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       12 2024-04-11 05:50:40.000000 oirunner-0.0.3/tests/data/check_data/2.ans
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        2 2024-04-11 05:50:28.000000 oirunner-0.0.3/tests/data/check_data/2.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-11 06:54:37.000000 oirunner-0.0.3/tests/data/check_data/2.out
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        5 2024-04-11 05:50:54.000000 oirunner-0.0.3/tests/data/check_data/3.ans
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        2 2024-04-11 05:50:48.000000 oirunner-0.0.3/tests/data/check_data/3.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-11 06:54:42.000000 oirunner-0.0.3/tests/data/check_data/3.out
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        0 2024-04-07 07:56:52.000000 oirunner-0.0.3/tests/data/empty1.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)        2 2024-04-07 08:17:43.000000 oirunner-0.0.3/tests/data/empty2.in
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       23 2024-03-31 16:33:50.000000 oirunner-0.0.3/tests/data/fail.cpp
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)       96 2024-03-31 13:39:27.000000 oirunner-0.0.3/tests/data/success.cpp
+-rwxrwxr-x   0 ste1      (1000) ste1      (1000)     6445 2024-04-11 13:40:53.000000 oirunner-0.0.3/tests/test_basic.py
```

### Comparing `OiRunner-0.0.2/.gitignore` & `oirunner-0.0.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
+a.out
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
@@ -46,14 +47,15 @@
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
+~*/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `OiRunner-0.0.2/LICENSE` & `oirunner-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OiRunner-0.0.2/OiRunner/run.py` & `oirunner-0.0.3/OiRunner/BetterRunner.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,216 +2,228 @@
 import argparse
 import sys
 import os
 import shutil
 import time
 
 
-class BetterRunner:
-    def __init__(self):
+class Functions:
+
+    def __init__(self) -> None:
         pass
 
-    def cmd_parse(self):
-        '''
-        命令行解析
+    def _modify_file(self, file_name: str, file_type: str) -> int:
         '''
-        pa = argparse.ArgumentParser()
-        pa.add_argument('filename', help="要编译的cpp文件(省略'.cpp')")
-        pa.add_argument('-n', '--name', default="a", help="生成的可执行文件名(省略'.exe')")
-        pa.add_argument('-j', '--judge', action='store_true', help="是否评测")
-        # pa.add_argument('-u','--use_multiple_processes',action='store_true',help="是否使用多进程评测")
-        pa.add_argument('-p', '--print', action='store_true', help="是否显示输出")
-        pa.add_argument('-if', '--inputfile', default='in.txt', help="输入文件名")
-        pa.add_argument('-of', '--outputfile', default='out.txt', help="输出文件名")
-        pa.add_argument('-af', '--answerfile', default='ans.txt', help="答案文件名")
-        pa.add_argument('-g', '--gdb', action='store_true', help="答案错误时是否使用gdb打开")
-        pa.add_argument('-gf', '--gdbfile', default=None, help="gdb调试输入文件")
-        pa.add_argument('--directgdb', action='store_true', help="直接使用gdb调试")
-        pa.add_argument('--onlyinput', action='store_true', help="使用文件输入（-j时无效）")
-        pa.add_argument('--onlyoutput', action='store_true', help="使用文件输出（-j时无效）")
-        self.args = pa.parse_args()
+        Split the file into multiple files by line, with the output file located at ~tmp/.
 
-        self.args.use_multiple_processes = False
-        self.input_file = self.args.inputfile
-        self.output_file = self.args.outputfile
-        self.answer_file = self.args.answerfile
-        if sys.platform == "linux":
-            self.args.name = "./" + self.args.name + '.out'
-        elif sys.platform == "win32":
-            self.args.name = self.args.name + '.exe'
+        参数：
+        file_name -- 传入文件名
+        file_type -- 输出文件扩展名
 
-    def compile(self):
-        '''
-        编译文件
-        '''
-        try:
-            compile = sp.Popen(['g++', self.args.filename + '.cpp', '-g', '-o', self.args.name])
-            compile.wait()
-            if compile.returncode == 0:
-                print("编译成功")
-            else:
-                print("编译失败")
-                exit(0)
-        except KeyboardInterrupt:
-            print("\n手动退出，祝AC~(^v^)")
-            exit(0)
+        返回值：
+        i -- 输出文件数量
 
-    def _modify_file(self, file_name, file_type):
-        '''
-        将文件按行分割
+        可能异常：
+        SystemExit -- 文件为空
         '''
         i = 1
         a = ""
-        if not os.path.exists('~tmp'):
-            os.mkdir('~tmp')
+        flag = 0
+        if not os.path.exists("~tmp"):
+            os.mkdir("~tmp")
         with open(file_name, "r") as f:
             for line in f:
+                flag = 1
                 if line.rstrip():
                     a += f"{line}"
                 else:
                     if not a:
                         print(f"error:{file_name}文件为空")
-                        shutil.rmtree('~tmp')
-                        exit(0)
+                        shutil.rmtree("~tmp")
+                        sys.exit()
                     with open(f"~tmp/{i}.{file_type}", "w") as _f:
                         _f.write(a)
                     i += 1
                     a = ""
+            if not flag:
+                print(f"error:{file_name}文件为空")
+                shutil.rmtree("~tmp")
+                sys.exit()
+
         if a:
             with open(f"~tmp/{i}.{file_type}", "w") as _f:
                 _f.write(a)
         return i
 
-    def _output(self, num):
+    def _output(self, num: int, opt_file: str) -> None:
         '''
-        将分割后的文件合并输出
+        将分割后的文件合并输出。
+
+        参数：
+        num -- 要合并的文件数量。
+        opt_file -- 输出文件名。
         '''
         a = ""
         for file_num in range(1, num+1):
             a += f"#{file_num}:\n"
             with open(f"~tmp/{file_num}.out", "r") as _f:
                 for line in _f:
                     a += f"{line}"
 
-        with open(self.args.outputfile, "w") as _out:
+        with open(opt_file, "w") as _out:
             _out.write(a)
 
-    def _check(self, opt_file, ipt_file, ans_file, file_num=0, run_file=None):
+
+class BetterRunner:
+    def __init__(self) -> None:
+        self.input_file = "in.txt"
+        self.output_file = "out.txt"
+        self.answer_file = "ans.txt"
+        self.func = Functions()
+
+    def cmd_parse(self) -> None:
         '''
-        本地评测
+        命令行解析
+        '''
+        pa = argparse.ArgumentParser()
+        pa.add_argument("filename", help="要编译的cpp文件(省略'.cpp')")
+        pa.add_argument("-n", "--name", default="a", help="生成的可执行文件名(省略'.exe')")
+        pa.add_argument("-j", "--judge", action="store_true", help="是否评测")
+        pa.add_argument("-p", "--print", action="store_true", help="是否显示输出")
+        pa.add_argument("-if", "--inputfile", default="in.txt", help="输入文件名")
+        pa.add_argument("-of", "--outputfile", default="out.txt", help="输出文件名")
+        pa.add_argument("-af", "--answerfile", default="ans.txt", help="答案文件名")
+        pa.add_argument("-g", "--gdb", action="store_true", help="答案错误时是否使用gdb打开")
+        pa.add_argument("--directgdb", action="store_true", help="直接使用gdb调试")
+        pa.add_argument("--onlyinput", action="store_true", help="使用文件输入（-j时无效）")
+        pa.add_argument("--onlyoutput", action="store_true", help="使用文件输出（-j时无效）")
+        self.args = pa.parse_args()
+        self.input_file = self.args.inputfile
+        self.output_file = self.args.outputfile
+        self.answer_file = self.args.answerfile
+        if sys.platform == "linux":
+            self.args.name = "./" + self.args.name + ".out"
+        elif sys.platform == "win32":
+            self.args.name = self.args.name + ".exe"
+
+    def compile(self) -> None:
+        '''
+        编译文件，生成可执行文件。
+
+        可能异常：
+        SystemExit -- 编译失败
+        '''
+        try:
+            compile = sp.Popen(["g++", self.args.filename + ".cpp", "-g", "-o", self.args.name])
+            compile.wait()
+            if compile.returncode == 0:
+                print("编译成功")
+            else:
+                print("编译失败")
+                sys.exit()
+
+        # Can't sent Ctrl+c and get the messages.
+        except KeyboardInterrupt:  # pragma: no cover
+            print("\n手动退出，祝AC~(^v^)")
+            sys.exit()
+
+    def _check(self, opt_file: str, ipt_file: str, ans_file: str,
+               file_num: int = 0, run_file: str | None = None, if_print: bool | None = None) -> bool:
+        '''
+        本地评测，并获取结果。
+
+        参数：
+        opt_file -- 输出文件名
+        ipt_file -- 输入文件名
+        ans_file -- 答案文件名
+        file_num -- 文件编号
+        run_file -- 可执行文件名（None为使用命令行参数值）
+
+        返回值：
+        if_pass -- 测试是否通过
         '''
 
         print(f"#{file_num}:")
 
         if run_file is None:
             run_file = self.args.name
+        if if_print is None:
+            if_print = self.args.print
 
         with open(opt_file, "w") as _out, open(ipt_file, "r") as _in:
             run = sp.Popen([run_file], stdin=_in, stdout=_out)
 
-            if not self.args.use_multiple_processes:
-                ft = time.time()
-                run.wait()
-                now = time.time() - ft
+            ft = time.time()
+            run.wait()
+            now = time.time() - ft
 
             if run.returncode != 0:
                 print(f"返回值为{run.returncode}，程序运行可能有问题")
 
         with open(ans_file, "r") as ans, open(opt_file, "r") as my_ans:
-            ans = [line.rstrip() for line in ans if line.rstrip()]
-            my_ans = [line.rstrip() for line in my_ans if line.rstrip()]
-            if ans == my_ans:
-                if self.args.print:
-                    # print(f"标准答案：{ans}\n实际答案：{my_ans}")
+            ans_list = [line.rstrip() for line in ans if line.rstrip()]
+            my_ans_list = [line.rstrip() for line in my_ans if line.rstrip()]
+            if ans_list == my_ans_list:
+                if if_print:
                     print(f"答案正确，用时{now:.5}")
                 else:
                     print("答案正确")
                 return True
             else:
-                if self.args.print:
-                    # print(f"标准答案：{ans}\n实际答案：{my_ans}")
+                if if_print:
+                    if len(ans_list) < 10:
+                        print(f"标准答案：{ans_list}\n实际答案：{my_ans_list}")
+                    else:
+                        print("答案行数过大")
                     print("答案错误")
                     print("错误数据：")
                     with open(ipt_file, "r") as _in:
-                        for line in _in:
-                            if line.rstrip():
-                                print(line.rstrip())
+                        data_list = [line.rstrip() for line in _in if line.rstrip()]
+                        data: str = ""
+                        for data_line in data_list:
+                            data += data_line
+                            data += "\n"
+                        if len(data) < 100:
+                            print(data)
+                        else:
+                            print("数据字数过多")
                 else:
                     print("答案错误")
 
                 return False
 
-    def _copy_file(self, i):
-        '''
-        复制文件，为多进程评测准备
-        '''
-        for file_num in range(1, i + 1):
-            dst = os.path.join(r'~tmp/', f"{file_num}_{self.args.name}")
-            shutil.copy2(self.args.name, dst)
-
-    def _debug(self):
-        """
-        使用gdb调试
-        """
-        if self.args.gdbfile is None:
-            gdb = sp.Popen(['gdb', self.args.name])
-            gdb.wait()
-        else:
-            with open(self.args.gdbfile, "r") as f:
-                gdb = sp.Popen(['gdb', self.args.name], stdin=sp.PIPE, text=True)
-                for line in f:
-                    if line.rstrip():
-                        line = str(line.rstrip()) + "\n"
-                        # if line != "r":
-                        #     line = line + "\n"
-                        gdb.stdin.write(line)
-                        gdb.stdin.flush()
-                # print(gdb.stdout.read())
-                # gdb.stdin.close()
-
-                gdb.stdin = sys.stdin
-                gdb.wait()
-
-    def run(self):
-        """
-        程序主函数
-        """
+    def run(self) -> None:
+        '''程序运行主函数'''
         try:
             if self.args.directgdb:
-                self._debug()
-                exit(0)
+                gdb = sp.Popen(["gdb", self.args.name])
+                gdb.wait()
+                sys.exit()
 
             if self.args.judge:
                 flag = 0
 
-                if os.path.exists('~tmp'):
-                    shutil.rmtree('~tmp')
-                self._modify_file(self.args.inputfile, "in")
-                i = self._modify_file(self.args.answerfile, "ans")
-                if self.args.use_multiple_processes:
-                    self._copy_file(i)
+                if os.path.exists("~tmp"):
+                    shutil.rmtree("~tmp")
+                self.func._modify_file(self.input_file, "in")
+                i = self.func._modify_file(self.answer_file, "ans")
 
                 for file_num in range(1, i + 1):
-
-                    if self.args.use_multiple_processes:
-                        judge = self._check(f"~tmp/{file_num}.out", f"~tmp/{file_num}.in", f"~tmp/{file_num}.ans",
-                                            file_num, f"~tmp/{file_num}_{self.args.name}")
-                    else:
-                        judge = self._check(f"~tmp/{file_num}.out", f"~tmp/{file_num}.in", f"~tmp/{file_num}.ans",
-                                            file_num)
-
+                    judge = self._check(f"~tmp/{file_num}.out", f"~tmp/{file_num}.in", f"~tmp/{file_num}.ans",
+                                        file_num)
                     if not judge:
                         flag += 1
 
                 print(f"#final:正确率{((i - flag) / i) : .2%}")
-                self._output(i)
-                shutil.rmtree('~tmp')
+                self.func._output(i, self.output_file)
+                shutil.rmtree("~tmp")
 
                 if self.args.gdb and flag > 0:
-                    self._debug()
+                    gdb = sp.Popen(["gdb", self.args.name])
+                    gdb.wait()
 
             else:
                 if self.args.onlyinput:
                     with open(self.input_file, "r") as _in:
                         print("文件已执行")
                         run = sp.Popen([self.args.name], stdin=_in)
 
@@ -223,16 +235,16 @@
                     run = sp.Popen([self.args.name])
 
                 run.wait()
                 if run.returncode != 0:
                     print(f"返回值为{run.returncode}，程序运行可能有问题")
 
         except KeyboardInterrupt:
-            if os.path.exists('~tmp'):
-                shutil.rmtree('~tmp')
+            if os.path.exists("~tmp"):
+                shutil.rmtree("~tmp")
             print("\n手动退出，祝AC~(^v^)")
 
 
 def main():
     runner = BetterRunner()
     runner.cmd_parse()
     runner.compile()
```

