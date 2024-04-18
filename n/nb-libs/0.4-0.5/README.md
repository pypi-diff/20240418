# Comparing `tmp/nb_libs-0.4.tar.gz` & `tmp/nb_libs-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nb_libs-0.4.tar", last modified: Fri Nov 17 02:18:58 2023, max compression
+gzip compressed data, was "dist\nb_libs-0.5.tar", last modified: Thu Apr 18 02:41:41 2024, max compression
```

## Comparing `nb_libs-0.4.tar` & `nb_libs-0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-11-17 02:18:58.000000 nb_libs-0.4/
--rw-rw-rw-   0        0        0     1980 2023-11-17 02:18:58.000000 nb_libs-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1261 2023-11-17 02:18:55.000000 nb_libs-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-11-17 02:18:58.000000 nb_libs-0.4/nb_libs.egg-info/
--rw-rw-rw-   0        0        0     1980 2023-11-17 02:18:57.000000 nb_libs-0.4/nb_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-11-17 02:18:57.000000 nb_libs-0.4/nb_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-17 02:18:57.000000 nb_libs-0.4/nb_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-11-17 02:18:57.000000 nb_libs-0.4/nb_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-11-17 02:18:57.000000 nb_libs-0.4/nb_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-17 02:18:58.000000 nb_libs-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1714 2023-11-17 02:18:55.000000 nb_libs-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-17 02:18:58.000000 nb_libs-0.4/tests/
--rw-rw-rw-   0        0        0      379 2023-03-15 02:57:54.000000 nb_libs-0.4/tests/test_restart_programe_by_interval.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:41:41.000000 nb_libs-0.5/
+-rw-rw-rw-   0        0        0     2255 2024-04-18 02:41:41.000000 nb_libs-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1536 2023-11-17 02:24:36.000000 nb_libs-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 02:41:41.000000 nb_libs-0.5/nb_libs.egg-info/
+-rw-rw-rw-   0        0        0     2255 2024-04-18 02:41:40.000000 nb_libs-0.5/nb_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-04-18 02:41:40.000000 nb_libs-0.5/nb_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:41:40.000000 nb_libs-0.5/nb_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-18 02:41:40.000000 nb_libs-0.5/nb_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 02:41:40.000000 nb_libs-0.5/nb_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 02:41:41.000000 nb_libs-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1714 2024-04-18 02:41:38.000000 nb_libs-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 02:41:41.000000 nb_libs-0.5/tests/
+-rw-rw-rw-   0        0        0      379 2023-03-15 02:57:54.000000 nb_libs-0.5/tests/test_restart_programe_by_interval.py
+-rw-rw-rw-   0        0        0      934 2024-02-29 11:16:03.000000 nb_libs-0.5/tests/tests_time.py
```

### Comparing `nb_libs-0.4/PKG-INFO` & `nb_libs-0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb_libs
-Version: 0.4
+Version: 0.5
 Summary: nb_libs
 Home-page: https://github.com/ydf0509/nb_libs
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -52,13 +52,16 @@
 好用的时间转换,类型兼容强,入参可以是时间戳 字符串 datatime类型 DatetimeConverter 类型.
 
 # 3 auto_git.GitBranchMerge
 
 git 自动化 分支合并.
 
 多人合作项目git开发流程一般是:
+```
+自己分支写代码 -> 自己分支 add -> 自己分支commit -> 设置自己分支在远程对应的分支名 -> 自己分支push到远程 -> 切换到开发develop分支 -> 
+在develop分支 git pull ->把自己分merge到develop分支 -> develop分支 push到远程 -> checkout到自己分支
 
-自己分支写代码 -> 自己分支commit -> 自己分支push到远程 -> 切换到开发develop分支 -> 在develop分支 git pull ->
-把自己分merge到develop分支 -> develop分支 push到远程 
-
-开发环境代码拉取develop代码重启部署,测试出现问题后,需要反复执行git繁琐的流程,整个过程如果手动人工操作git太折磨人了,
+开发环境代码拉取develop代码重启部署,测试出现问题后,需要反复执行以上的git繁琐的流程,整个过程如果手动人工操作git太折磨人了,
 auto_git.GitBranchMerge 一键执行以上操作,如果有某一步git命令出现错误或冲突,是会中断操作的,不用担心.
+
+当develop代码测试没问题后,提merge request 把自己分支合并到master分支,管理人员审核通过后会把用户分支的代码合并到master.
+```
```

### Comparing `nb_libs-0.4/README.md` & `nb_libs-0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -30,13 +30,16 @@
 好用的时间转换,类型兼容强,入参可以是时间戳 字符串 datatime类型 DatetimeConverter 类型.
 
 # 3 auto_git.GitBranchMerge
 
 git 自动化 分支合并.
 
 多人合作项目git开发流程一般是:
+```
+自己分支写代码 -> 自己分支 add -> 自己分支commit -> 设置自己分支在远程对应的分支名 -> 自己分支push到远程 -> 切换到开发develop分支 -> 
+在develop分支 git pull ->把自己分merge到develop分支 -> develop分支 push到远程 -> checkout到自己分支
 
-自己分支写代码 -> 自己分支commit -> 自己分支push到远程 -> 切换到开发develop分支 -> 在develop分支 git pull ->
-把自己分merge到develop分支 -> develop分支 push到远程 
+开发环境代码拉取develop代码重启部署,测试出现问题后,需要反复执行以上的git繁琐的流程,整个过程如果手动人工操作git太折磨人了,
+auto_git.GitBranchMerge 一键执行以上操作,如果有某一步git命令出现错误或冲突,是会中断操作的,不用担心.
 
-开发环境代码拉取develop代码重启部署,测试出现问题后,需要反复执行git繁琐的流程,整个过程如果手动人工操作git太折磨人了,
-auto_git.GitBranchMerge 一键执行以上操作,如果有某一步git命令出现错误或冲突,是会中断操作的,不用担心.
+当develop代码测试没问题后,提merge request 把自己分支合并到master分支,管理人员审核通过后会把用户分支的代码合并到master.
+```
```

### Comparing `nb_libs-0.4/nb_libs.egg-info/PKG-INFO` & `nb_libs-0.5/nb_libs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-libs
-Version: 0.4
+Version: 0.5
 Summary: nb_libs
 Home-page: https://github.com/ydf0509/nb_libs
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
@@ -52,13 +52,16 @@
 好用的时间转换,类型兼容强,入参可以是时间戳 字符串 datatime类型 DatetimeConverter 类型.
 
 # 3 auto_git.GitBranchMerge
 
 git 自动化 分支合并.
 
 多人合作项目git开发流程一般是:
+```
+自己分支写代码 -> 自己分支 add -> 自己分支commit -> 设置自己分支在远程对应的分支名 -> 自己分支push到远程 -> 切换到开发develop分支 -> 
+在develop分支 git pull ->把自己分merge到develop分支 -> develop分支 push到远程 -> checkout到自己分支
 
-自己分支写代码 -> 自己分支commit -> 自己分支push到远程 -> 切换到开发develop分支 -> 在develop分支 git pull ->
-把自己分merge到develop分支 -> develop分支 push到远程 
-
-开发环境代码拉取develop代码重启部署,测试出现问题后,需要反复执行git繁琐的流程,整个过程如果手动人工操作git太折磨人了,
+开发环境代码拉取develop代码重启部署,测试出现问题后,需要反复执行以上的git繁琐的流程,整个过程如果手动人工操作git太折磨人了,
 auto_git.GitBranchMerge 一键执行以上操作,如果有某一步git命令出现错误或冲突,是会中断操作的,不用担心.
+
+当develop代码测试没问题后,提merge request 把自己分支合并到master分支,管理人员审核通过后会把用户分支的代码合并到master.
+```
```

### Comparing `nb_libs-0.4/setup.py` & `nb_libs-0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # filepath = ((Path(__file__).parent / Path('README.md')).absolute()).as_posix()
 filepath = 'README.md'
 print(filepath)
 
 setup(
     name='nb_libs',  #
-    version="0.4",
+    version="0.5",
     description=('nb_libs'),
     keywords=["nb_libs",],
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
     # data_files=[filepath],
     author='bfzs',
```

