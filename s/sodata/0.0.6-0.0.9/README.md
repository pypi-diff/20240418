# Comparing `tmp/sodata-0.0.6.tar.gz` & `tmp/sodata-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sodata-0.0.6.tar", last modified: Fri Apr 12 12:13:42 2024, max compression
+gzip compressed data, was "sodata-0.0.9.tar", last modified: Wed Apr 17 02:38:03 2024, max compression
```

## Comparing `sodata-0.0.6.tar` & `sodata-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-12 12:13:42.610291 sodata-0.0.6/
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      165 2024-04-12 12:13:42.610291 sodata-0.0.6/PKG-INFO
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      298 2024-04-09 07:45:32.000000 sodata-0.0.6/README.md
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       38 2024-04-12 12:13:42.610291 sodata-0.0.6/setup.cfg
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      380 2024-04-12 12:13:11.000000 sodata-0.0.6/setup.py
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-12 12:13:42.610291 sodata-0.0.6/sodata/
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      129 2024-04-10 06:25:35.000000 sodata-0.0.6/sodata/__init__.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      139 2024-04-09 12:56:22.000000 sodata-0.0.6/sodata/chunk_split.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)     1818 2024-04-12 11:50:05.000000 sodata-0.0.6/sodata/file_process.py
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)    14292 2024-04-12 11:55:39.000000 sodata-0.0.6/sodata/text_clean.py
-drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-12 12:13:42.610291 sodata-0.0.6/sodata.egg-info/
--rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      165 2024-04-12 12:13:42.000000 sodata-0.0.6/sodata.egg-info/PKG-INFO
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      252 2024-04-12 12:13:42.000000 sodata-0.0.6/sodata.egg-info/SOURCES.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        1 2024-04-12 12:13:42.000000 sodata-0.0.6/sodata.egg-info/dependency_links.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       48 2024-04-12 12:13:42.000000 sodata-0.0.6/sodata.egg-info/requires.txt
--rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        7 2024-04-12 12:13:42.000000 sodata-0.0.6/sodata.egg-info/top_level.txt
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-17 02:38:03.214994 sodata-0.0.9/
+-rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      386 2024-04-17 02:38:03.214994 sodata-0.0.9/PKG-INFO
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      298 2024-04-09 07:45:32.000000 sodata-0.0.9/README.md
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       38 2024-04-17 02:38:03.214994 sodata-0.0.9/setup.cfg
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      409 2024-04-17 02:38:00.000000 sodata-0.0.9/setup.py
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-17 02:38:03.214994 sodata-0.0.9/sodata/
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      197 2024-04-17 02:21:45.000000 sodata-0.0.9/sodata/__init__.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)     4596 2024-04-17 02:37:01.000000 sodata-0.0.9/sodata/chunk_clean.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)    11983 2024-04-16 03:07:11.000000 sodata-0.0.9/sodata/chunk_split.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)    10033 2024-04-16 03:07:11.000000 sodata-0.0.9/sodata/clean_rule.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)     3105 2024-04-16 12:43:17.000000 sodata-0.0.9/sodata/file_process.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      425 2024-04-17 02:19:04.000000 sodata-0.0.9/sodata/initialize.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      147 2024-04-16 06:20:23.000000 sodata-0.0.9/sodata/text_clean.py
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)    16237 2024-04-16 13:17:46.000000 sodata-0.0.9/sodata/text_split.py
+drwxrwxr-x   0 zhanghong  (1130) zhanghong  (1130)        0 2024-04-17 02:38:03.214994 sodata-0.0.9/sodata.egg-info/
+-rw-r--r--   0 zhanghong  (1130) zhanghong  (1130)      386 2024-04-17 02:38:03.000000 sodata-0.0.9/sodata.egg-info/PKG-INFO
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)      337 2024-04-17 02:38:03.000000 sodata-0.0.9/sodata.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        1 2024-04-17 02:38:03.000000 sodata-0.0.9/sodata.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)       71 2024-04-17 02:38:03.000000 sodata-0.0.9/sodata.egg-info/requires.txt
+-rw-rw-r--   0 zhanghong  (1130) zhanghong  (1130)        7 2024-04-17 02:38:03.000000 sodata-0.0.9/sodata.egg-info/top_level.txt
```

### Comparing `sodata-0.0.6/sodata/file_process.py` & `sodata-0.0.9/sodata/file_process.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,83 @@
 # -*- coding: utf-8 -*-
-# @File : chunk_split.py
+# @File : file_process.py
 # @Author : zh
 # @Time : 2024/4/9 15:38
 # @Desc : 数据处理过程中涉及到的文件操作
 import json
 import os
 
 
-def process_txt_file(filepath, encodings=['utf-8', 'gb18030', 'gbk', 'gb2312', 'latin-1', 'ascii']):
-    """
-    尝试使用不同的编码读取和转换文本文件。
-    @param filepath:  待处理的txt文件路径
-    @param encodings:  尝试的编码列表
-    @return:  返回处理后的文本数据
-    """
-    for encoding in encodings:
-        try:
-            with open(filepath, 'r', encoding=encoding) as f:
-                content = f.read()
-            # 成功读取后转换编码到utf-8（如果已经是utf-8则不需要转换）
-            return content.encode('utf-8').decode('utf-8')
-        except UnicodeDecodeError:
-            continue
-    raise UnicodeDecodeError(f"Failed to decode {filepath} with given encodings.")
-
-def process_folder_and_save_to_jsonl(folder_path, output_file):
-    """
-    递归遍历文件夹，处理每个txt文件，然后将数据保存为一整个JSONL格式。
-    @param folder_path: 待转换的txt文本路径
-    @param output_file: 输出文件路径
-    @return:
-    """
-    for root, dirs, files in os.walk(folder_path):
-        for file in files:
-            if file.endswith('.txt'):
-                filepath = os.path.join(root, file)
-                try:
-                    text_data = process_txt_file(filepath)
-                    with open(output_file, 'a', encoding='utf-8') as fp:
-                        fp.write(json.dumps({"text": text_data}, ensure_ascii=False) + '\n')
-                    print(f"Processed and saved {file} successfully.")
-                except UnicodeDecodeError as e:
-                    print(e)
+class FileProcessTool:
+    def __init__(self) -> None:
+        pass
+
+    def count_lines(self, file_path: str) -> int:
+        """
+        计算文件行数
+        Args:
+            file_path: 文件路径
+        Returns:
+            lines_num: 行数
+        """
+        lines_num = 0
+        with open(file_path, 'rb') as f:
+            while True:
+                data = f.read(2 ** 20)
+                if not data:
+                    break
+                lines_num += data.count(b'\n')
+        return lines_num
+
+    def process_txt_file(self, filepath: str,
+                         encodings: list[str] = ['utf-8', 'gb18030', 'gbk', 'gb2312', 'latin-1', 'ascii']) -> str:
+        """
+        尝试使用不同的编码读取和转换文本文件。
+        Args:
+            filepath: 待处理的txt文件路径
+            encodings: 尝试的编码列表
+        Returns:
+            content:返回处理后的文本数据
+        """
+        content = None
+        for encoding in encodings:
+            try:
+                with open(filepath, 'r', encoding=encoding) as file:
+                    content = file.read()
+                # 成功读取后转换编码到utf-8（如果已经是utf-8则不需要转换）
+                return content.encode('utf-8').decode('utf-8')
+            except UnicodeDecodeError:
+                continue
+        raise UnicodeDecodeError(f"Failed to decode {filepath} with given encodings.")
+
+    def save_to_jsonl(self, text_data: str, output_file: str) -> None:
+        """
+        将文本数据保存为JSON Lines格式。
+        Args:
+            text_data: 待保存的整本小说文本数据
+            output_file: 输出文件路径
+        Returns:
+        """
+        with open(output_file, 'a', encoding='utf-8') as file:
+            file.write(json.dumps({"text": text_data}, ensure_ascii=False) + '\n')
+
+    def process_folder_and_save_to_jsonl(self, txt_folder_path: str, output_file: str) -> None:
+        """
+        递归遍历文件夹，处理每个txt文件，然后将数据保存为一整个JSONL格式。
+        Args:
+            txt_folder_path:  待转换的txt文本路径
+            output_file:  输出文件路径
+        Returns:
+        """
+        for root, dirs, files in os.walk(txt_folder_path):
+            for file in files:
+                if file.endswith('.txt'):
+                    filepath = os.path.join(root, file)
+                    try:
+                        text_data = self.process_txt_file(filepath)
+                        with open(output_file, 'a', encoding='utf-8') as fp:
+                            fp.write(json.dumps({"text": text_data}, ensure_ascii=False) + '\n')
+                        print(f"Processed and saved {file} successfully.")
+                    except UnicodeDecodeError as e:
+                        print(e)
+
```

### Comparing `sodata-0.0.6/sodata/text_clean.py` & `sodata-0.0.9/sodata/clean_rule.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,252 +1,134 @@
-# -*- coding: utf-8 -*-
-# @File : chunk_split.py
-# @Author : zh
-# @Time : 2024/4/9 15:38
-# @Desc : 清除小说文本中的无效数据
-
-import pandas as pd
-import jionlp as jio
-
-from tqdm import tqdm
-from concurrent.futures import ThreadPoolExecutor
-from datasketch import MinHash, MinHashLSH
-import regex as re
-
-# 特定小说数据清洗替换规则
-rules = [
-    # 净化分隔符
-    (re.compile(
-        r"([—\–_×ꁘ*/#-※]{3,})+.*?\1.*?\1|([—\–_×ꁘ*/#-※]{3,})+.*?\1",
-        re.MULTILINE | re.IGNORECASE), ""),
-
-    # 净化网址
-    (re.compile(
-        r"<(center|font)(?:\t(?!src\b)|\S)+?</\1>|(?:[\n<_]|[A-Z]+\.)br/?>|<‎‎‏‎‏‎‏‎‏‏‎‏‏/[a-z]{1,6}>|&\b[A-Z;]+\b;|(?<![A-Z])&?(nbsp|quot|amp|lt|gt);|#[A-Z][0-9A-Z]{4};|\r\n|\b[记首本一]\W?[住发书秒]\W?[域网记]\W?[名址站住][^\n\u4e00-\u9fcc，、。；！？—…（）“”【】]+|(?<![:=]\t?[\"'])https?:/[/_A-Z\d\.\-]+\.(?:com|net|org|edu|x?html?|php|aspx??|txt|json|zip|cn|cc|tw|hk|us|in|info|pro|xyz|club|work|space)\b(?:/[/_A-Z\d\-]*)?(?![/_A-Z\d\-\.\?])|(?m)^\b[a-z0-9\.]{3,21}\b\.[a-z]{2,4}/?(?:\n|$)|(?<=[\n。])[\w&&[^\u4e00-\u9fcc]]+\.(?:com|org|xyz)$|w(?:\?_/[a-z\d\.]){6,18}(?<=m)"
-        r"|&?(nbsp|quot|amp|lt|gt)"
-        , re.IGNORECASE | re.MULTILINE), ""),
-
-    # 净化标点
-    (re.compile(
-        r"(?<=[（【，、：]|[。；！？—…][”」]?)(?!(?<=[：…])…|(?<=—)—|(?<=[：！？])[！？])[，、。：；！？—…]+|(?<=“)——\b|(?<=\B\n|“)[，、。！？…]+(?=[\w“「（【《])|(?<=…)\n…+|\b[，、。：；]+(?=[）】][，、。：；！？…])|(?<=^|\n)[？]+(?=[“「《\w])|(?<=\b「[^\n「」]{1,16})[！—…]+\B(?=」\b)|(?<=”\n?)[“”＂‘’]+(?=\n?“)|(?<=”)[\"＂](?=\n|$)|\b[：](?=「\b[\w，！…]{1,9}」(?:后\b|的声))|(?<=\n)[^\w「」…●]+$"
-        , re.MULTILINE), ""),
-
-    # 净化词语
-    (re.compile(
-        r"(?<=\n)(?:[（【]?PS\d?\b|作者按：|作者有话要?说|作者的话[：\n]|——(?:题外|作者的)话——\n)[^\n]*(?:\n[^\n]+){0,15}$|(?<=[^\n）】：]\n)[（【][^\n]+$|(?<=\n)(?=[—…]{2}\n|[^\n]{1,49}$)(?=[\s\S]{0,49}?(?:码字|存稿|[本新]书|书[友评]|[首追]订|订阅|[打万]赏|[求月]票|公众号|求收藏|推荐票|支持正版|\b起\W{2}点\Wapp更新|过度章|[章更]\d[KW]|[新补有更][一二三四五两]章|[右点午晚天时章]更新|推荐\w{0,9}\u300A|[第天晚有的这就旧再][\d一二三四五两加爆]更|更新\d{0,4}字))[^\n]+(?:\n[^\n]+){0,2}$|(?m)^(?:HTTPS?:|-?WAP\b|[wωщш]{3}\.|[（【]?PS\d?[：:]|您可以在百度里|百度搜索|按键返回|版权所有|本作品来自|本站访问地址|本书仅供个人|本书版权归|本章尚未结束|本章未完[^\n]+(?:\n【[^\n]+】$)?|【(?:话说|讲真|推荐下|鉴于大环境如此|认识十年的老书友\w+)，|【[^\n【】]+】【】|【[\w，！]{0,24}?(?:\b新章节|\b[上下]一章|阅读尽在|野果阅读|本站可能|[追听]书|[读书阁源]的?APP)|纯文字在线|测试章节\b|\W{0,3}到进行查看|当前网址|顶点手机|顶点地址|飞速中文|\W?点此\w{0,2}报错|感谢[\w、]*(?:书友|[打万]赏)|\W?更新预告\b|更多(?:免费)?好书|广个告|欢迎广大书友|华书阁|\W?加入书签|精校小说|交流好书|看书福利|看无广告|看[\w\\]+\\就\\|每天更新时间|免费阅读|期待精彩继续|起点欢迎广大书友|亲\W(?:本站|点击)|求推荐|请退出转码|请\w?[记藏]\w?本[书站]|全文字无广告|全文字小说|如果觉得此文|搜读小说|搜索关注|「收集免费好书」|手机(?:访问|站全新|版?阅读)|书籍全\W更新快|书客居阅读|天才[一壹]秒|天才本站|推本书\b|网站即将关闭|网站最新地址|网页版章节|网为你提供|为您提供大神|微信关注|温馨提示\W为防止(?:最新章|内容获取)|无弹窗|下载后请在24小时|下载\w{1,4}APP|[想要]{0,2}看最新章节|新书期间|新书上传|新?笔趣|[一三1]秒钟?记住|以下是：为你提供|永久地址|域名更换|阅读网址|\W{0,4}看?最快[最更]新|\W{0,3}章节(?:报错|[有错]误|重复)|支持\w+阅读|中文域名|转载请保留|注册本站|TXT下载|\d+(?:READ|SHU|TXT|YD|ZW|字大章|字奉上)|\W?送\d+现金红包|\w+(?:手机版：\b[A-Z\.]{2}|提醒您：看完记得收藏)|本书由\S{1,19}?收集|[（【]推荐\w+的《|看?《[^\n《》]{0,19}?》最[快新]|为[你您]提供\S{1,19}?更新|喜欢\S{1,19}?请大家收藏|阅读\S{1,19}?最新章节请)[^\n]*$(?:\n[^\n]+$(?!\n)|\n[^\n\w“”—…※]{0,9}$|\n第\w{1,7}章[^\n]{0,19}$|\n\d+[\.\t][^\n\d][^\n]{0,19}$)?\n?|^(?=[\w《])[^\n]{0,59}?(?:[退支][出持]阅读模式|模式阅读|免费阅读|页继续阅读|最新章节|畅阅无阻|收藏书签|[求个月的]月票|书[币友][\w「」]+[打万]赏)[^\n\w]{0,9}(?:\n[\s\S]{1,99}$(?!\n)|$\n?)"
-        , re.MULTILINE), ""),
-
-    # 净化段落
-    (re.compile(
-        r"(?<=[（【，、：]|[。；！？—…][”」]?)(?!(?<=[：…])…|(?<=—)—|(?<=[：！？])[！？])[，、。：；！？—…]+|(?<=“)——\b|(?<=\B\n|“)[，、。！？…]+(?=[\w“「（【《])|(?<=…)\n…+|\b[，、。：；]+(?=[）】][，、。：；！？…])|(?<=^|\n)[？]+(?=[“「《\w])|(?<=\b「[^\n「」]{1,16})[！—…]+\B(?=」\b)|(?<=”\n?)[“”＂‘’]+(?=\n?“)|(?<=”)[\"＂](?=\n|$)|\b[：](?=「\b[\w，！…]{1,9}」(?:后\b|的声))|(?<=\n)[^\w「」…●]+$"
-        , re.MULTILINE), ""),
-
-    # 净化杂项
-    (re.compile(
-        r"(?:“”|‘’|「」|【】|（）|\(\)|<>)[，]?|(?<=^\b[\w、。！？—…]{0,4}(\w[。！？—…]{1,4}))\n\b(?=[\w、。！？—…]{0,4}\1$)|(?<=^\w[^\n\w]{1,4})\n\b(?=\w[^\n\w]{1,4}$)|(?<=[，、]|[^：]“[！？…]{1,9}”|[\n：]“[^\n“”]{0,32}[。！？—…]|[（【][^\n：（）【】]{0,32})\n\b|\n\b(?=[^\n：（）【】]{0,32}[）】])|\b\n(?=(?<![：][\+\-]?\b[\w\+\-，、%]{1,15}\b\n)[！？…])|\n\B(?=[，、：；]|(?<=\b：\n)“)|(?<=\d%?[→])\n(?=\d)|(?:\b[！—…]+\B|\n\b)(?=(?:[”’」]|」「\w{1,3}[—…]{2}」)?(?:[时式][的地]|的[^的确]|为由|之[声类流]|一声\b|[着后]\b|地\w着\b))|(?<=[。！？—…][”]?)\w$"
-        , re.IGNORECASE | re.MULTILINE), ""),
-
-    # 01 ☁️杂项去除
-    (re.compile(
-        r"\u001a|：  ）|.*章节目录.*|『|』|(&[a-z]*|<)-->>\s(.* |  ;)|-->>\s|r \/>|&nbsp;|&amp;|zwnj;|请牢记.*|正在更新.*|防止失联.*|.*域名.*|.*网址.*|.*看书的|：，，.|蓝星，夏国.*(\s.*)+|陌上.*最快.*更新.*|琇.{0,2}||[ωxwmMΧ].{5,12}[ＭmtΤΜ]"
-        , re.IGNORECASE | re.MULTILINE), ""),
-
-    # 02 ☁️标题净化
-    (re.compile(
-        r"\s第.*章|[\(（【].*?[求更谢乐发订合补加].*?[】）\)]|[\(\)]|晋江.*"
-        , re.IGNORECASE | re.MULTILINE), ""),
-
-    # 03 ☁️晋江-仅感谢
-    (re.compile(
-        r"感谢.*的小天使(.*\s*)*|##.*感谢(灌|投|支持).*|感谢(在|为).*小天使.*|.*(扔|投|砸)了.*时间.*|.*\d瓶；.*|.*(手榴弹|营养液|地雷|浅水炸弹|深水炸弹|深水鱼雷|火箭炮|投雷).*|非常感谢.*努力.*|.*\s.*文学城.*"
-        , re.IGNORECASE | re.MULTILINE), ""),
-
-    # 03 ☁️晋江-完整有话说
-    (re.compile(
-        r"作者有话要说(.*\s*)*|๑作者有话说(.|\n)*|##作者有话要说[\s\S]+|◎作者有话说：[\s\S]+|作者有话要说：[\s\S]+"
-        , re.IGNORECASE | re.MULTILINE), ""),
-
-    # 连续的点替换为省略号，中文破折号替换
-    (re.compile(r"\.{3,}"), "…"),  # 连续的英文点
-    (re.compile(r"·{3,}"), "…"),  # 连续的中文点
-    (re.compile(r"\b·\b"), ""),  # 孤立的中点
-
-    # 正确的小数点处理，这里假设前后都是数字，则不替换
-    (re.compile(r"(?<=\d)．(?=\d)"), "."),
-
-    # 数字间的冒号处理，这里简化为直接替换
-    (re.compile(r"(?<=\d)：(?=\d)"), ":"),
-
-    # 逗号、冒号、分号的不当使用处理，简化为替换为中文符号
-    (re.compile(r","), "，"),
-    (re.compile(r":"), "："),
-    (re.compile(r";"), "；"),
-
-    # 中文破折号的使用
-    (re.compile(r"—"), "一"),
-
-    # 连续的感叹号或问号处理
-    (re.compile(r"!{2,}"), "！"),
-    (re.compile(r"\?{2,}"), "？"),
-
-    # 星号处理
-    (re.compile(r"\*{2,}"), "※"),
-
-    # 方块和乘号的处理
-    (re.compile(r"□"), ""),
-    (re.compile(r"×"), "x"),
-
-    # 移除行首的null字符串
-    (re.compile(r"^null\n", re.MULTILINE), ""),
-
-    # 移除仅包含标点的行
-    (re.compile(r"^[，、。：；！？…~]+\n?", re.MULTILINE), ""),
-
-    # 移除标点前不当的波浪线和下划线
-    (re.compile(r"[~_]+(?=[。！？…])", re.MULTILINE), ""),
-
-    # 在特定标点（感叹号或问号）前不恰当使用的符号
-    (re.compile(r"\b[。—…~\-]+(?<!\d\-)(?=[！？])"), ""),
-
-    # 移除连续的逗号或顿号
-    (re.compile(r"[，、]+(?=[，、。：；！？…~]|——)"), ""),
-
-    # 移除冒号和分号前的空格
-    (re.compile(r"\s+(?=[：；])"), ""),
-
-    # 移除行尾的空白
-    (re.compile(r"\s+$", re.MULTILINE), ""),
-
-    # 删除标题
-    (re.compile(r"第[零〇一二三四五六七八九十百千两壹贰叁肆伍陆柒捌玖拾佰陌仟阡\d]{1,7}[章节回卷篇集]", re.MULTILINE),
-     ""),
-
-    # 不恰当的点的替换成省略号
-    (re.compile(
-        r"[\u2025\u2026\u002e\u00b7\u0387\u1802\u2022\u2024\u2027\u2219\u22c5\u22ef\u2505\u2810\u2e31\u2e33\u30fb\u318d\ua78f\uff0e\uff65]{2,}"
-        r"|[\u2e30\u3002\uff61\uffee]{2,}"
-        r"|[，、；（【《]+$"
-        r"|[，、](?=[”＂\"]\n)"
-        r"|^(?:[ꁘ\s]+|[。．\u002e～~·]+)$", re.DOTALL), "……"),
-
-    # 不恰当的点的替换成破折号
-    (re.compile(
-        r"([\u002d\u2010-\u2015\u2212\u2500\u2501\u268a\u268b\u2e3a\u2e3b\uff0d\uff70\uffda~〜])"
-        r"(?:\1+|[\u2010-\u2013]+|(?<=\u2014|\u2015)(?!\d)|(?<=\w[～~])\B|(?<!\u002d)[。，、]+)"
-        r"|^[—\–_×ꁘ]{2,}$",
-        re.MULTILINE | re.IGNORECASE), "——"),
-]
-
-def count_lines(file_path):
-    """
-    每次读取 1MB 的数据,计算文件行数
-    @param file_path: 文件路径
-    @return:  返回文件行数
-    """
-    lines_num = 0
-    with open(file_path, 'rb') as f:
-        while True:
-            data = f.read(2 ** 20)
-            if not data:
-                break
-            lines_num += data.count(b'\n')
-    return lines_num
-
-
-def remove_duplicates_exact(paragraphs):
-    """
-    精确匹配去重
-    @param paragraphs: 待去重段落列表：list
-    @return:唯一段落列表：list ；重复段落列表：list
-    """
-    unique_set = set()
-    unique_paragraphs = []
-    repeated_text = []
-    for p in paragraphs:
-        if p in unique_set:
-            repeated_text.append(p)
-            continue
-        unique_set.add(p)
-        unique_paragraphs.append(p)
-    return unique_paragraphs, repeated_text
-
-def remove_duplicates_minhash(paragraphs, num_perm=128):
-    """
-    MinHash去重
-    @param paragraphs: 待去重段落列表：list
-    @param num_perm: 用于生成MinHash的排列数，较大的 num_perm 值会提高准确性，但也会增加计算成本
-    @return:  唯一段落列表：list ；重复段落列表：list
-    """
-    lsh = MinHashLSH(threshold=0.5, num_perm=num_perm)
-    minhashes = {} #存储每个段落的 MinHash 对象
-
-    for i, p in enumerate(paragraphs):
-        m = MinHash(num_perm=num_perm)
-        for d in p:
-            m.update(d.encode('utf-8'))
-        lsh.insert(f"p{i}", m)#将每个段落的 MinHash 对象插入到 MinHashLSH 中
-        minhashes[f"p{i}"] = m
-
-    unique_keys = set()
-    ordered_unique_keys = []  # 用于保持原始顺序的唯一键列表
-    ordered_repeated = [] # 保持原始顺序的重复段落列表
-    for i, p in enumerate(paragraphs):
-        key = f"p{i}"
-        if key in unique_keys:
-            # x = []
-            # x.append(paragraphs[key], paragraphs[i])
-            ordered_repeated.append(paragraphs[i])
-            continue
-        duplicates = lsh.query(minhashes[key])
-        unique_keys.update(duplicates)
-        ordered_unique_keys.append(key)  # 仅当键是唯一的时候才添加
-
-    # 使用有序的唯一键列表来生成最终的唯一段落列表
-    unique_indices = [int(k[1:]) for k in ordered_unique_keys]
-    unique_paragraphs = [paragraphs[i] for i in sorted(unique_indices)]  # 根据索引排序以保持原始顺序
-    return unique_paragraphs, ordered_repeated
-
-def cascade_deduplication(text_dirty):
-    """
-    精确匹配去重级联MinHash去重
-    @param text_dirty: chunk文本
-    @return: 清洗后的文本：str ；重复段落列表：list
-    """
-    # 以一行为单位处理
-    paragraphs = text_dirty.split('\n')
-    # Step 1: 精确匹配去重
-    unique_paragraphs, repeated_text = remove_duplicates_exact(paragraphs)
-    # Step 2: MinHash去重
-    # unique_paragraphs, ordered_repeated= remove_duplicates_minhash(paragraphs)
-
-    text_clean = '\n'.join(unique_paragraphs)
-    return text_clean, repeated_text
-
-
-def clean_text(text):
-    '''
-    对文本chunk块清洗
-    Args:
-        text:文本chunk块
-
-    Returns:
-        清洗后的文本：str;去重的段落列表：list
-    '''
-
-
-
-
-
-    raw_text = text
-    # 应用替换规则清洗
-    for pattern, replacement in rules:
-        # dirty_text_list.extend(re.findall(pattern, text))
-        text = re.sub(pattern, replacement, text)
-     # 通用清洗
-    text = jio.clean_text(text, remove_parentheses=False, delete_prefix=True)#remove_parentheses=False 表示不移除括号，delete_prefix=True 表示删除前缀
-
-    text, ordered_repeated = cascade_deduplication(text)
-    # dirty_text_list.append(ordered_repeated)
-    if "@" in text or "^" in text or "PS：" in text or "更新时间" in text or "回复时间" in text or "回复日期" in text or (
-            "《" in text and "》" in text):
-        return '',[]
-    return text,ordered_repeated
+# -*- coding: utf-8 -*- 
+# @File : clean_rule.py.py
+# @Author : zh 
+# @Time : 2024/4/16 上午10:54
+# @Desc : 清洗文本数据的规则
+import regex as re
+
+# 不影响语义分割文本的正则表达式
+split_pattern = '(。|？|！|\…\…)'
+# 特定小说数据清洗替换规则
+rules = [
+    # 净化分隔符
+    (re.compile(
+        r"([—\–_×ꁘ*/#-※]{3,})+.*?\1.*?\1|([—\–_×ꁘ*/#-※]{3,})+.*?\1",
+        re.MULTILINE | re.IGNORECASE), ""),
+
+    # 净化网址
+    (re.compile(
+        r"<(center|font)(?:\t(?!src\b)|\S)+?</\1>|(?:[\n<_]|[A-Z]+\.)br/?>|<‎‎‏‎‏‎‏‎‏‏‎‏‏/[a-z]{1,6}>|&\b[A-Z;]+\b;|(?<![A-Z])&?(nbsp|quot|amp|lt|gt);|#[A-Z][0-9A-Z]{4};|\r\n|\b[记首本一]\W?[住发书秒]\W?[域网记]\W?[名址站住][^\n\u4e00-\u9fcc，、。；！？—…（）“”【】]+|(?<![:=]\t?[\"'])https?:/[/_A-Z\d\.\-]+\.(?:com|net|org|edu|x?html?|php|aspx??|txt|json|zip|cn|cc|tw|hk|us|in|info|pro|xyz|club|work|space)\b(?:/[/_A-Z\d\-]*)?(?![/_A-Z\d\-\.\?])|(?m)^\b[a-z0-9\.]{3,21}\b\.[a-z]{2,4}/?(?:\n|$)|(?<=[\n。])[\w&&[^\u4e00-\u9fcc]]+\.(?:com|org|xyz)$|w(?:\?_/[a-z\d\.]){6,18}(?<=m)"
+        r"|&?(nbsp|quot|amp|lt|gt)"
+        , re.IGNORECASE | re.MULTILINE), ""),
+
+    # 净化标点
+    (re.compile(
+        r"(?<=[（【，、：]|[。；！？—…][”」]?)(?!(?<=[：…])…|(?<=—)—|(?<=[：！？])[！？])[，、。：；！？—…]+|(?<=“)——\b|(?<=\B\n|“)[，、。！？…]+(?=[\w“「（【《])|(?<=…)\n…+|\b[，、。：；]+(?=[）】][，、。：；！？…])|(?<=^|\n)[？]+(?=[“「《\w])|(?<=\b「[^\n「」]{1,16})[！—…]+\B(?=」\b)|(?<=”\n?)[“”＂‘’]+(?=\n?“)|(?<=”)[\"＂](?=\n|$)|\b[：](?=「\b[\w，！…]{1,9}」(?:后\b|的声))|(?<=\n)[^\w「」…●]+$"
+        , re.MULTILINE), ""),
+
+    # 净化词语
+    (re.compile(
+        r"(?<=\n)(?:[（【]?PS\d?\b|作者按：|作者有话要?说|作者的话[：\n]|——(?:题外|作者的)话——\n)[^\n]*(?:\n[^\n]+){0,15}$|(?<=[^\n）】：]\n)[（【][^\n]+$|(?<=\n)(?=[—…]{2}\n|[^\n]{1,49}$)(?=[\s\S]{0,49}?(?:码字|存稿|[本新]书|书[友评]|[首追]订|订阅|[打万]赏|[求月]票|公众号|求收藏|推荐票|支持正版|\b起\W{2}点\Wapp更新|过度章|[章更]\d[KW]|[新补有更][一二三四五两]章|[右点午晚天时章]更新|推荐\w{0,9}\u300A|[第天晚有的这就旧再][\d一二三四五两加爆]更|更新\d{0,4}字))[^\n]+(?:\n[^\n]+){0,2}$|(?m)^(?:HTTPS?:|-?WAP\b|[wωщш]{3}\.|[（【]?PS\d?[：:]|您可以在百度里|百度搜索|按键返回|版权所有|本作品来自|本站访问地址|本书仅供个人|本书版权归|本章尚未结束|本章未完[^\n]+(?:\n【[^\n]+】$)?|【(?:话说|讲真|推荐下|鉴于大环境如此|认识十年的老书友\w+)，|【[^\n【】]+】【】|【[\w，！]{0,24}?(?:\b新章节|\b[上下]一章|阅读尽在|野果阅读|本站可能|[追听]书|[读书阁源]的?APP)|纯文字在线|测试章节\b|\W{0,3}到进行查看|当前网址|顶点手机|顶点地址|飞速中文|\W?点此\w{0,2}报错|感谢[\w、]*(?:书友|[打万]赏)|\W?更新预告\b|更多(?:免费)?好书|广个告|欢迎广大书友|华书阁|\W?加入书签|精校小说|交流好书|看书福利|看无广告|看[\w\\]+\\就\\|每天更新时间|免费阅读|期待精彩继续|起点欢迎广大书友|亲\W(?:本站|点击)|求推荐|请退出转码|请\w?[记藏]\w?本[书站]|全文字无广告|全文字小说|如果觉得此文|搜读小说|搜索关注|「收集免费好书」|手机(?:访问|站全新|版?阅读)|书籍全\W更新快|书客居阅读|天才[一壹]秒|天才本站|推本书\b|网站即将关闭|网站最新地址|网页版章节|网为你提供|为您提供大神|微信关注|温馨提示\W为防止(?:最新章|内容获取)|无弹窗|下载后请在24小时|下载\w{1,4}APP|[想要]{0,2}看最新章节|新书期间|新书上传|新?笔趣|[一三1]秒钟?记住|以下是：为你提供|永久地址|域名更换|阅读网址|\W{0,4}看?最快[最更]新|\W{0,3}章节(?:报错|[有错]误|重复)|支持\w+阅读|中文域名|转载请保留|注册本站|TXT下载|\d+(?:READ|SHU|TXT|YD|ZW|字大章|字奉上)|\W?送\d+现金红包|\w+(?:手机版：\b[A-Z\.]{2}|提醒您：看完记得收藏)|本书由\S{1,19}?收集|[（【]推荐\w+的《|看?《[^\n《》]{0,19}?》最[快新]|为[你您]提供\S{1,19}?更新|喜欢\S{1,19}?请大家收藏|阅读\S{1,19}?最新章节请)[^\n]*$(?:\n[^\n]+$(?!\n)|\n[^\n\w“”—…※]{0,9}$|\n第\w{1,7}章[^\n]{0,19}$|\n\d+[\.\t][^\n\d][^\n]{0,19}$)?\n?|^(?=[\w《])[^\n]{0,59}?(?:[退支][出持]阅读模式|模式阅读|免费阅读|页继续阅读|最新章节|畅阅无阻|收藏书签|[求个月的]月票|书[币友][\w「」]+[打万]赏)[^\n\w]{0,9}(?:\n[\s\S]{1,99}$(?!\n)|$\n?)"
+        , re.MULTILINE), ""),
+
+    # 净化段落
+    (re.compile(
+        r"(?<=[（【，、：]|[。；！？—…][”」]?)(?!(?<=[：…])…|(?<=—)—|(?<=[：！？])[！？])[，、。：；！？—…]+|(?<=“)——\b|(?<=\B\n|“)[，、。！？…]+(?=[\w“「（【《])|(?<=…)\n…+|\b[，、。：；]+(?=[）】][，、。：；！？…])|(?<=^|\n)[？]+(?=[“「《\w])|(?<=\b「[^\n「」]{1,16})[！—…]+\B(?=」\b)|(?<=”\n?)[“”＂‘’]+(?=\n?“)|(?<=”)[\"＂](?=\n|$)|\b[：](?=「\b[\w，！…]{1,9}」(?:后\b|的声))|(?<=\n)[^\w「」…●]+$"
+        , re.MULTILINE), ""),
+
+    # 净化杂项
+    (re.compile(
+        r"(?:“”|‘’|「」|【】|（）|\(\)|<>)[，]?|(?<=^\b[\w、。！？—…]{0,4}(\w[。！？—…]{1,4}))\n\b(?=[\w、。！？—…]{0,4}\1$)|(?<=^\w[^\n\w]{1,4})\n\b(?=\w[^\n\w]{1,4}$)|(?<=[，、]|[^：]“[！？…]{1,9}”|[\n：]“[^\n“”]{0,32}[。！？—…]|[（【][^\n：（）【】]{0,32})\n\b|\n\b(?=[^\n：（）【】]{0,32}[）】])|\b\n(?=(?<![：][\+\-]?\b[\w\+\-，、%]{1,15}\b\n)[！？…])|\n\B(?=[，、：；]|(?<=\b：\n)“)|(?<=\d%?[→])\n(?=\d)|(?:\b[！—…]+\B|\n\b)(?=(?:[”’」]|」「\w{1,3}[—…]{2}」)?(?:[时式][的地]|的[^的确]|为由|之[声类流]|一声\b|[着后]\b|地\w着\b))|(?<=[。！？—…][”]?)\w$"
+        , re.IGNORECASE | re.MULTILINE), ""),
+
+    # 01 ☁️杂项去除
+    (re.compile(
+        r"\u001a|：  ）|.*章节目录.*|『|』|(&[a-z]*|<)-->>\s(.* |  ;)|-->>\s|r \/>|&nbsp;|&amp;|zwnj;|请牢记.*|正在更新.*|防止失联.*|.*域名.*|.*网址.*|.*看书的|：，，.|蓝星，夏国.*(\s.*)+|陌上.*最快.*更新.*|琇.{0,2}||[ωxwmMΧ].{5,12}[ＭmtΤΜ]"
+        , re.IGNORECASE | re.MULTILINE), ""),
+
+    # 02 ☁️标题净化
+    (re.compile(
+        r"\s第.*章|[\(（【].*?[求更谢乐发订合补加].*?[】）\)]|[\(\)]|晋江.*"
+        , re.IGNORECASE | re.MULTILINE), ""),
+
+    # 03 ☁️晋江-仅感谢
+    (re.compile(
+        r"感谢.*的小天使(.*\s*)*|##.*感谢(灌|投|支持).*|感谢(在|为).*小天使.*|.*(扔|投|砸)了.*时间.*|.*\d瓶；.*|.*(手榴弹|营养液|地雷|浅水炸弹|深水炸弹|深水鱼雷|火箭炮|投雷).*|非常感谢.*努力.*|.*\s.*文学城.*"
+        , re.IGNORECASE | re.MULTILINE), ""),
+
+    # 03 ☁️晋江-完整有话说
+    (re.compile(
+        r"作者有话要说(.*\s*)*|๑作者有话说(.|\n)*|##作者有话要说[\s\S]+|◎作者有话说：[\s\S]+|作者有话要说：[\s\S]+"
+        , re.IGNORECASE | re.MULTILINE), ""),
+
+    # 连续的点替换为省略号，中文破折号替换
+    (re.compile(r"\.{3,}"), "…"),  # 连续的英文点
+    (re.compile(r"·{3,}"), "…"),  # 连续的中文点
+    (re.compile(r"\b·\b"), ""),  # 孤立的中点
+
+    # 正确的小数点处理，这里假设前后都是数字，则不替换
+    (re.compile(r"(?<=\d)．(?=\d)"), "."),
+
+    # 数字间的冒号处理，这里简化为直接替换
+    (re.compile(r"(?<=\d)：(?=\d)"), ":"),
+
+    # 逗号、冒号、分号的不当使用处理，简化为替换为中文符号
+    (re.compile(r","), "，"),
+    (re.compile(r":"), "："),
+    (re.compile(r";"), "；"),
+
+    # 中文破折号的使用
+    (re.compile(r"—"), "一"),
+
+    # 连续的感叹号或问号处理
+    (re.compile(r"!{2,}"), "！"),
+    (re.compile(r"\?{2,}"), "？"),
+
+    # 星号处理
+    (re.compile(r"\*{2,}"), "※"),
+
+    # 方块和乘号的处理
+    (re.compile(r"□"), ""),
+    (re.compile(r"×"), "x"),
+
+    # 移除行首的null字符串
+    (re.compile(r"^null\n", re.MULTILINE), ""),
+
+    # 移除仅包含标点的行
+    (re.compile(r"^[，、。：；！？…~]+\n?", re.MULTILINE), ""),
+
+    # 移除标点前不当的波浪线和下划线
+    (re.compile(r"[~_]+(?=[。！？…])", re.MULTILINE), ""),
+
+    # 在特定标点（感叹号或问号）前不恰当使用的符号
+    (re.compile(r"\b[。—…~\-]+(?<!\d\-)(?=[！？])"), ""),
+
+    # 移除连续的逗号或顿号
+    (re.compile(r"[，、]+(?=[，、。：；！？…~]|——)"), ""),
+
+    # 移除冒号和分号前的空格
+    (re.compile(r"\s+(?=[：；])"), ""),
+
+    # 移除行尾的空白
+    (re.compile(r"\s+$", re.MULTILINE), ""),
+
+    # 删除标题
+    (re.compile(r"第[零〇一二三四五六七八九十百千两壹贰叁肆伍陆柒捌玖拾佰陌仟阡\d]{1,7}[章节回卷篇集]", re.MULTILINE),
+     ""),
+
+    # 不恰当的点的替换成省略号
+    (re.compile(
+        r"[\u2025\u2026\u002e\u00b7\u0387\u1802\u2022\u2024\u2027\u2219\u22c5\u22ef\u2505\u2810\u2e31\u2e33\u30fb\u318d\ua78f\uff0e\uff65]{2,}"
+        r"|[\u2e30\u3002\uff61\uffee]{2,}"
+        r"|[，、；（【《]+$"
+        r"|[，、](?=[”＂\"]\n)"
+        r"|^(?:[ꁘ\s]+|[。．\u002e～~·]+)$", re.DOTALL), "……"),
+
+    # 不恰当的点的替换成破折号
+    (re.compile(
+        r"([\u002d\u2010-\u2015\u2212\u2500\u2501\u268a\u268b\u2e3a\u2e3b\uff0d\uff70\uffda~〜])"
+        r"(?:\1+|[\u2010-\u2013]+|(?<=\u2014|\u2015)(?!\d)|(?<=\w[～~])\B|(?<!\u002d)[。，、]+)"
+        r"|^[—\–_×ꁘ]{2,}$",
+        re.MULTILINE | re.IGNORECASE), "——"),
+]
+
+
```

