# Comparing `tmp/nonebot_plugin_ottohzys-0.2.0.tar.gz` & `tmp/nonebot_plugin_ottohzys-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ottohzys-0.2.0.tar", last modified: Sun Mar 10 07:21:25 2024, max compression
+gzip compressed data, was "nonebot_plugin_ottohzys-0.2.1.tar", last modified: Thu Apr 18 16:26:44 2024, max compression
```

## Comparing `nonebot_plugin_ottohzys-0.2.0.tar` & `nonebot_plugin_ottohzys-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4147 2024-03-10 07:21:12.768895 nonebot_plugin_ottohzys-0.2.0/README.md
--rw-r--r--   0        0        0      755 2024-03-10 07:21:12.768895 nonebot_plugin_ottohzys-0.2.0/nonebot_plugin_ottohzys/__init__.py
--rw-r--r--   0        0        0     2991 2024-03-10 07:21:12.768895 nonebot_plugin_ottohzys-0.2.0/nonebot_plugin_ottohzys/__main__.py
--rw-r--r--   0        0        0      165 2024-03-10 07:21:12.768895 nonebot_plugin_ottohzys-0.2.0/nonebot_plugin_ottohzys/config.py
--rw-r--r--   0        0        0     6324 2024-03-10 07:21:12.768895 nonebot_plugin_ottohzys-0.2.0/nonebot_plugin_ottohzys/hzys.py
--rw-r--r--   0        0        0      512 2024-03-10 07:21:12.768895 nonebot_plugin_ottohzys-0.2.0/nonebot_plugin_ottohzys/res/chinglish.json
--rw-r--r--   0        0        0     2520 2024-03-10 07:21:12.768895 nonebot_plugin_ottohzys-0.2.0/nonebot_plugin_ottohzys/resource.py
--rw-r--r--   0        0        0      766 2024-03-10 07:21:25.820843 nonebot_plugin_ottohzys-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 nonebot_plugin_ottohzys-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4004 2024-04-18 16:26:30.776193 nonebot_plugin_ottohzys-0.2.1/README.md
+-rw-r--r--   0        0        0      755 2024-04-18 16:26:30.776193 nonebot_plugin_ottohzys-0.2.1/nonebot_plugin_ottohzys/__init__.py
+-rw-r--r--   0        0        0     3105 2024-04-18 16:26:30.776193 nonebot_plugin_ottohzys-0.2.1/nonebot_plugin_ottohzys/__main__.py
+-rw-r--r--   0        0        0      165 2024-04-18 16:26:30.776193 nonebot_plugin_ottohzys-0.2.1/nonebot_plugin_ottohzys/config.py
+-rw-r--r--   0        0        0     6418 2024-04-18 16:26:30.776193 nonebot_plugin_ottohzys-0.2.1/nonebot_plugin_ottohzys/hzys.py
+-rw-r--r--   0        0        0      512 2024-04-18 16:26:30.776193 nonebot_plugin_ottohzys-0.2.1/nonebot_plugin_ottohzys/res/chinglish.json
+-rw-r--r--   0        0        0     3356 2024-04-18 16:26:30.776193 nonebot_plugin_ottohzys-0.2.1/nonebot_plugin_ottohzys/resource.py
+-rw-r--r--   0        0        0      763 2024-04-18 16:26:44.020257 nonebot_plugin_ottohzys-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4643 1970-01-01 00:00:00.000000 nonebot_plugin_ottohzys-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_ottohzys-0.2.0/README.md` & `nonebot_plugin_ottohzys-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -133,25 +133,23 @@
 
 ### [Rouphy](https://github.com/Rouphy)
 
 - 插件点子
 
 ## 💰 赞助
 
-感谢大家的赞助！你们的赞助将是我继续创作的动力！
+**[赞助我](https://blog.lgc2333.top/donate)**
 
-- [爱发电](https://afdian.net/@lgc2333)
-- <details>
-    <summary>赞助二维码（点击展开）</summary>
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
-  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
+## 📝 更新日志
 
-  </details>
+### 0.2.1
 
-## 📝 更新日志
+- 优化资源下载
 
 ### 0.2.0
 
 - 适配 Pydantic V1 & V2
 - 支持多平台
 
 ### 0.1.2
```

#### html2text {}

```diff
@@ -22,15 +22,13 @@
 ç´æ¥ä½¿ç¨æä»¤ `ottohzys` æ¥çå¸®å© ## ð èç³» QQï¼3076823485
 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [sakaneko117/HUOZI](https://github.com/sakaneko117/
 HUOZI) & [CwavGuy/HUOZI_aolianfeiallin.top](https://github.com/CwavGuy/
 HUOZI_aolianfeiallin.top) & [HanaYabuki/otto-hzys](https://github.com/
 HanaYabuki/otto-hzys) - é å¥½çè½®å­ ### [Rouphy](https://github.com/Rouphy)
-- æä»¶ç¹å­ ## ð° èµå©
-æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
-[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 -
-æ¯æå¤å¹³å° ### 0.1.2 - æ·»å åæ° `-N` (`--
+- æä»¶ç¹å­ ## ð° èµå© **[èµå©æ](https://blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 0.2.1 - ä¼åèµæºä¸è½½ ### 0.2.0 - éé Pydantic V1
+& V2 - æ¯æå¤å¹³å° ### 0.1.2 - æ·»å åæ° `-N` (`--
 normalize`)ï¼æ¹åé¨ååæ° - ä¿®å¤ä¸ç³»åç²å¿å¤§æå¯¼è´ç
 Bugï¼ææ¯åºç© ### 0.1.1 - éæé¨åä»£ç 
```

### Comparing `nonebot_plugin_ottohzys-0.2.0/nonebot_plugin_ottohzys/__init__.py` & `nonebot_plugin_ottohzys-0.2.1/nonebot_plugin_ottohzys/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nonebot.plugin import PluginMetadata, inherit_supported_adapters, require
 
 require("nonebot_plugin_alconna")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __plugin_meta__ = PluginMetadata(
     name="大电老师活字印刷",
     description="大家好啊，今天来点大家想看的东西",
     usage="直接使用指令【ottohzys】加上文本就行了，不带参数查看详细帮助，不会用我阐述你的梦",
     type="application",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-ottohzys",
     config=ConfigModel,
```

### Comparing `nonebot_plugin_ottohzys-0.2.0/nonebot_plugin_ottohzys/__main__.py` & `nonebot_plugin_ottohzys-0.2.1/nonebot_plugin_ottohzys/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,17 @@
 @cmd_otto.handle()
 async def _(matcher: Matcher, err: ParserExit = ShellCommandArgs()):
     await matcher.finish(f"解析指令参数出错：{err.message}")
 
 
 @cmd_otto.handle()
 async def _(matcher: Matcher, args: Namespace = ShellCommandArgs()):
+    # if not check_resource_sync():
+    #     await matcher.finish("未找到需要的资源文件，请检查")
+
     sentence = " ".join(str(x) for x in args.sentence).strip()
     reverse: bool = args.reverse
     ysdd: bool = not args.no_ysdd
     normalize: bool = not args.no_normalize
     speed: float = args.speed
     pitch: float = args.pitch
     pause: float = args.pause
```

### Comparing `nonebot_plugin_ottohzys-0.2.0/nonebot_plugin_ottohzys/hzys.py` & `nonebot_plugin_ottohzys-0.2.1/nonebot_plugin_ottohzys/hzys.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import psola
 import soundfile as sf
 from async_lru import alru_cache
 from nonebot import logger
 from numpy.typing import NDArray
 from pypinyin import lazy_pinyin
 
-from .resource import CHINGLISH_MAP, TOKENS_DIR, YSDD_TOKEN_MAP, YSDD_TOKENS_DIR
+from .resource import TOKENS_DIR, YSDD_TOKENS_DIR, get_chinglish_map, get_ysdd_token_map
 
 SoundArrayType = NDArray[np.float64]
 
 TARGET_SAMPLE_RATE = 44100
 """目标采样率"""
 
 
@@ -137,20 +137,22 @@
                 flattened = [y for x in splitted for y in x if y.pron]
                 tmp.extend(flattened)
 
         return tmp
 
     # 替换原声大碟
     if ysdd_mode:
-        for token, sentences in YSDD_TOKEN_MAP.items():
+        ysdd_token_map = get_ysdd_token_map()
+        for token, sentences in ysdd_token_map.items():
             for s in sentences:
                 pre_proc_pron = replace_pron(s, PreProcPron(token, is_ysdd=True))
 
     # 替换字母
-    for ch, pron in CHINGLISH_MAP.items():
+    chinglish_map = get_chinglish_map()
+    for ch, pron in chinglish_map.items():
         pre_proc_pron = replace_pron(
             ch,
             *(PreProcPron(pron, is_pinyin=True) for pron in pron.split()),
         )
 
     # 拼音化
     ret = []
```

### Comparing `nonebot_plugin_ottohzys-0.2.0/nonebot_plugin_ottohzys/res/chinglish.json` & `nonebot_plugin_ottohzys-0.2.1/nonebot_plugin_ottohzys/res/chinglish.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ottohzys-0.2.0/pyproject.toml` & `nonebot_plugin_ottohzys-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 dynamic = []
 description = "otto!"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.0",
-    "nonebot-plugin-alconna>=0.40.0rc1",
+    "nonebot-plugin-alconna>=0.40.1",
     "soundfile>=0.12.1",
     "numpy>=1.24.4",
     "pypinyin>=0.49.0",
     "psola>=0.0.1",
     "anyio>=3.6.2",
     "httpx>=0.25.0",
     "async-lru>=2.0.4",
 ]
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/lgc-NB2Dev/nonebot-plugin-ottohzys"
```

### Comparing `nonebot_plugin_ottohzys-0.2.0/PKG-INFO` & `nonebot_plugin_ottohzys-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ottohzys
-Version: 0.2.0
+Version: 0.2.1
 Summary: otto!
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-ottohzys
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-ottohzys
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.2.0
-Requires-Dist: nonebot-plugin-alconna>=0.40.0rc1
+Requires-Dist: nonebot-plugin-alconna>=0.40.1
 Requires-Dist: soundfile>=0.12.1
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: pypinyin>=0.49.0
 Requires-Dist: psola>=0.0.1
 Requires-Dist: anyio>=3.6.2
 Requires-Dist: httpx>=0.25.0
 Requires-Dist: async-lru>=2.0.4
@@ -153,25 +153,23 @@
 
 ### [Rouphy](https://github.com/Rouphy)
 
 - 插件点子
 
 ## 💰 赞助
 
-感谢大家的赞助！你们的赞助将是我继续创作的动力！
+**[赞助我](https://blog.lgc2333.top/donate)**
 
-- [爱发电](https://afdian.net/@lgc2333)
-- <details>
-    <summary>赞助二维码（点击展开）</summary>
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
 
-  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
+## 📝 更新日志
 
-  </details>
+### 0.2.1
 
-## 📝 更新日志
+- 优化资源下载
 
 ### 0.2.0
 
 - 适配 Pydantic V1 & V2
 - 支持多平台
 
 ### 0.1.2
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ottohzys Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ottohzys Version: 0.2.1 Summary:
 otto! Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-ottohzys Author-
 Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-ottohzys Requires-Python: <4.0,>=3.9 Requires-Dist:
-nonebot2>=2.2.0 Requires-Dist: nonebot-plugin-alconna>=0.40.0rc1 Requires-Dist:
+nonebot2>=2.2.0 Requires-Dist: nonebot-plugin-alconna>=0.40.1 Requires-Dist:
 soundfile>=0.12.1 Requires-Dist: numpy>=1.24.4 Requires-Dist: pypinyin>=0.49.0
 Requires-Dist: psola>=0.0.1 Requires-Dist: anyio>=3.6.2 Requires-Dist:
 httpx>=0.25.0 Requires-Dist: async-lru>=2.0.4 Description-Content-Type: text/
 markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
    # NoneBot-Plugin-ottoHzys _â¿ å¤§çµèå¸æ´»å­å°å· â¿_[python]_[_p_d_m_-
@@ -32,15 +32,13 @@
 ç´æ¥ä½¿ç¨æä»¤ `ottohzys` æ¥çå¸®å© ## ð èç³» QQï¼3076823485
 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://
 jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [sakaneko117/HUOZI](https://github.com/sakaneko117/
 HUOZI) & [CwavGuy/HUOZI_aolianfeiallin.top](https://github.com/CwavGuy/
 HUOZI_aolianfeiallin.top) & [HanaYabuki/otto-hzys](https://github.com/
 HanaYabuki/otto-hzys) - é å¥½çè½®å­ ### [Rouphy](https://github.com/Rouphy)
-- æä»¶ç¹å­ ## ð° èµå©
-æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
-[ç±åçµ](https://afdian.net/@lgc2333) - èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
-[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png) ## ð æ´æ°æ¥å¿ ### 0.2.0 - éé Pydantic V1 & V2 -
-æ¯æå¤å¹³å° ### 0.1.2 - æ·»å åæ° `-N` (`--
+- æä»¶ç¹å­ ## ð° èµå© **[èµå©æ](https://blog.lgc2333.top/donate)**
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ ##
+ð æ´æ°æ¥å¿ ### 0.2.1 - ä¼åèµæºä¸è½½ ### 0.2.0 - éé Pydantic V1
+& V2 - æ¯æå¤å¹³å° ### 0.1.2 - æ·»å åæ° `-N` (`--
 normalize`)ï¼æ¹åé¨ååæ° - ä¿®å¤ä¸ç³»åç²å¿å¤§æå¯¼è´ç
 Bugï¼ææ¯åºç© ### 0.1.1 - éæé¨åä»£ç 
```

