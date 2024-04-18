# Comparing `tmp/LangSegment-0.3.2-py3-none-any.whl.zip` & `tmp/LangSegment-0.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 21120 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    44709 b- defN 24-Apr-10 11:27 LangSegment/LangSegment.py
--rw-rw-rw-  2.0 fat      278 b- defN 24-Apr-10 11:27 LangSegment/__init__.py
--rw-rw-rw-  2.0 fat    15251 b- defN 24-Apr-10 11:29 LangSegment-0.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 11:29 LangSegment-0.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-10 11:29 LangSegment-0.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      478 b- defN 24-Apr-10 11:29 LangSegment-0.3.2.dist-info/RECORD
-6 files, 60820 bytes uncompressed, 20256 bytes compressed:  66.7%
+Zip file size: 21133 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    44726 b- defN 24-Apr-18 15:44 LangSegment/LangSegment.py
+-rw-rw-rw-  2.0 fat      278 b- defN 24-Apr-18 15:45 LangSegment/__init__.py
+-rw-rw-rw-  2.0 fat    15251 b- defN 24-Apr-18 15:45 LangSegment-0.3.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-18 15:45 LangSegment-0.3.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-18 15:45 LangSegment-0.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      478 b- defN 24-Apr-18 15:45 LangSegment-0.3.3.dist-info/RECORD
+6 files, 60837 bytes uncompressed, 20269 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: LangSegment/LangSegment.py
 Comment: 
 
 Filename: LangSegment/__init__.py
 Comment: 
 
-Filename: LangSegment-0.3.2.dist-info/METADATA
+Filename: LangSegment-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: LangSegment-0.3.2.dist-info/WHEEL
+Filename: LangSegment-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: LangSegment-0.3.2.dist-info/top_level.txt
+Filename: LangSegment-0.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: LangSegment-0.3.2.dist-info/RECORD
+Filename: LangSegment-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## LangSegment/LangSegment.py

```diff
@@ -313,15 +313,15 @@
             cleans_text = LangSegment._cleans_text(cleans_text)
             # fix:Langid's recognition of short sentences is inaccurate, and it is spliced longer.
             if not EOS and len(cleans_text) <= 2:
                 lines[nextId] = f'{text}{nextText}'
                 continue
             language,score = LangSegment._lang_classify(cleans_text)
             prev_language , prev_text = LangSegment._get_prev_data(words)
-            if language != LANG_ZH and all('\u4e00' <= c <= '\u9fff' for c in cleans_text):language,score = LANG_ZH,1
+            if language != LANG_ZH and all('\u4e00' <= c <= '\u9fff' for c in re.sub(r'\s','',cleans_text)):language,score = LANG_ZH,1
             if len(cleans_text) <= 5 and LangSegment._is_chinese(cleans_text):
                 filters_string = LangSegment._get_filters_string()
                 if score < LangSegment.LangPriorityThreshold and len(filters_string) > 0:
                     index_ja , index_zh = filters_string.find(LANG_JA) , filters_string.find(LANG_ZH)
                     if index_ja != -1 and index_ja < index_zh:language = LANG_JA
                     elif index_zh != -1 and index_zh < index_ja:language = LANG_ZH
                 if LangSegment._is_japanese_kana(cleans_text):language = LANG_JA
```

## LangSegment/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .LangSegment import LangSegment,getTexts,classify,getCounts,printList,setfilters,getfilters,setPriorityThreshold,getPriorityThreshold,setEnablePreview,getEnablePreview,setKeepPinyin,getKeepPinyin
 
 # release
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 
 
 # develop
 __develop__ = 'dev-0.0.1'
```

## Comparing `LangSegment-0.3.2.dist-info/METADATA` & `LangSegment-0.3.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LangSegment
-Version: 0.3.2
+Version: 0.3.3
 Summary: This is a multilingual tokenization tool that currently supports for zh/ja/en/ko, and more languages.
 Home-page: https://github.com/juntaosun/LangSegment
 Author: sunnyboxs
 License: BSD
 Keywords: language detection,language identification,langid,langid.py,nlp,language
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
@@ -36,15 +36,15 @@
 https://github.com/adbar/py3langid  
 
 
 功能：将文章或句子里的例如（中/英/日/韩），按不同语言自动识别分词，使文本更适合AI处理。    
 本代码专为各种 TTS 项目的前端文本多语种混合标注区分，多语言混合训练和推理而编写。
 
 ## 最近更新：News   
-* 版本：v0.3.2  fix （更新帮助见下文）。
+* 版本：v0.3.3  fix （更新帮助见下文）。
 * 添加支持： "zh"中文（数字拼音pinyin），保留多音字（音素）指定。 
 * 添加支持： "ru"俄语Russian / "th"泰语Thai。
 * 添加支持： "fr"法语French  / "vi"越南语Vietnamese。
 * 语言优先级，置信度评分和阀值。
 * 优化字符处理。fix: LangSegment.setfilters    
 * 更细致的处理，中日英韩，分词更精准！  
 * 多语言过滤组功能（默认:中/英/日/韩）！帮您自动清理不需要的语言内容。
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LangSegment Version: 0.3.2 Summary: This is a
+Metadata-Version: 2.1 Name: LangSegment Version: 0.3.3 Summary: This is a
 multilingual tokenization tool that currently supports for zh/ja/en/ko, and
 more languages. Home-page: https://github.com/juntaosun/LangSegment Author:
 sunnyboxs License: BSD Keywords: language detection,language
 identification,langid,langid.py,nlp,language Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
@@ -22,15 +22,15 @@
 TTS (Text-to-Speech) synthesis projects, preprocessing of multilingual text
 mixing for both training and inference. >Implementation based on
 py3langidï¼See LICENSE file for more info. https://github.com/adbar/py3langid
 åè½ï¼å°æç« æå¥å­éçä¾å¦ï¼ä¸­/è±/æ¥/
 é©ï¼ï¼æä¸åè¯­è¨èªå¨è¯å«åè¯ï¼ä½¿ææ¬æ´éåAIå¤çã
 æ¬ä»£ç ä¸ä¸ºåç§ TTS
 é¡¹ç®çåç«¯ææ¬å¤è¯­ç§æ··åæ æ³¨åºåï¼å¤è¯­è¨æ··åè®­ç»åæ¨çèç¼åã
-## æè¿æ´æ°ï¼News * çæ¬ï¼v0.3.2 fix ï¼æ´æ°å¸®å©è§ä¸æï¼ã *
+## æè¿æ´æ°ï¼News * çæ¬ï¼v0.3.3 fix ï¼æ´æ°å¸®å©è§ä¸æï¼ã *
 æ·»å æ¯æï¼
 "zh"ä¸­æï¼æ°å­æ¼é³pinyinï¼ï¼ä¿çå¤é³å­ï¼é³ç´ ï¼æå®ã *
 æ·»å æ¯æï¼ "ru"ä¿è¯­Russian / "th"æ³°è¯­Thaiã * æ·»å æ¯æï¼
 "fr"æ³è¯­French / "vi"è¶åè¯­Vietnameseã *
 è¯­è¨ä¼åçº§ï¼ç½®ä¿¡åº¦è¯ååéå¼ã * ä¼åå­ç¬¦å¤çãfix:
 LangSegment.setfilters * æ´ç»è´çå¤çï¼ä¸­æ¥è±é©ï¼åè¯æ´ç²¾åï¼
 * å¤è¯­è¨è¿æ»¤ç»åè½ï¼é»è®¤:ä¸­/è±/æ¥/
```

