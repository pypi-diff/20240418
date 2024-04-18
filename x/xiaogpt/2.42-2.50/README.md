# Comparing `tmp/xiaogpt-2.42.tar.gz` & `tmp/xiaogpt-2.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.42.tar", last modified: Mon Apr 15 06:04:20 2024, max compression
+gzip compressed data, was "xiaogpt-2.50.tar", last modified: Thu Apr 18 03:33:53 2024, max compression
```

## Comparing `xiaogpt-2.42.tar` & `xiaogpt-2.50.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1063 2024-04-15 06:04:10.006637 xiaogpt-2.42/LICENSE
--rw-r--r--   0        0        0    23005 2024-04-15 06:04:10.006637 xiaogpt-2.42/README.md
--rw-r--r--   0        0        0     3906 2024-04-15 06:04:20.222632 xiaogpt-2.42/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/__main__.py
--rw-r--r--   0        0        0      919 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1840 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0     2289 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0     4738 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/cli.py
--rw-r--r--   0        0        0     6301 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      220 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     3979 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/tts/azure.py
--rw-r--r--   0        0        0     4660 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1172 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/tts/edge.py
--rw-r--r--   0        0        0     1096 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1533 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/tts/openai.py
--rw-r--r--   0        0        0     2072 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/utils.py
--rw-r--r--   0        0        0    15337 2024-04-15 06:04:10.006637 xiaogpt-2.42/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    28865 1970-01-01 00:00:00.000000 xiaogpt-2.42/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-18 03:33:49.898299 xiaogpt-2.50/LICENSE
+-rw-r--r--   0        0        0    23992 2024-04-18 03:33:49.898299 xiaogpt-2.50/README.md
+-rw-r--r--   0        0        0     4133 2024-04-18 03:33:53.230314 xiaogpt-2.50/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      919 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3656 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1840 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0     2289 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3657 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0     4738 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6726 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-04-18 03:33:49.898299 xiaogpt-2.50/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      279 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     3979 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/azure.py
+-rw-r--r--   0        0        0     4660 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1172 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/edge.py
+-rw-r--r--   0        0        0     1096 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1533 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/openai.py
+-rw-r--r--   0        0        0     3984 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/tts/volc.py
+-rw-r--r--   0        0        0     2072 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/utils.py
+-rw-r--r--   0        0        0    15513 2024-04-18 03:33:49.902299 xiaogpt-2.50/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    30311 1970-01-01 00:00:00.000000 xiaogpt-2.50/PKG-INFO
```

### Comparing `xiaogpt-2.42/LICENSE` & `xiaogpt-2.50/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/README.md` & `xiaogpt-2.50/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,41 +15,24 @@
 - ChatGPT
 - New Bing
 - [ChatGLM](http://open.bigmodel.cn/)
 - [Gemini](https://makersuite.google.com/app/apikey)
 - [通义千问](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
 
 ## 获取小米音响DID
-### Windows(使用 set 设置环境变量）
-```cmd
-pip install miservice_fork
-set MI_USER=xxxx
-set MI_PASS=xxx
-micli list 得到did
-set MI_DID=xxxx
-```
+系统和Shell|Linux *sh|Windows CMD用户|Windows PowerShell用户
+-|-|-|-
+1、安装包|`pip install miservice_fork`|`pip install miservice_fork`|`pip install miservice_fork`
+2、设置变量|`export MI_USER=xxx` <br> `export MI_PASS=xxx`|`set MI_USER=xxx`<br>`set MI_PASS=xxx`|`$env:MI_USER="xxx"` <br> `$env:MI_PASS="xxx"`
+3、取得MI_DID|`micli list` |`micli list` |`micli list` 
+4、设置MI_DID|`export MI_DID=xxx`| `set MI_DID=xxx`| `$env:MI_DID="xxx"`
 
+- 注意不同shell 对环境变量的处理是不同的，尤其是powershell赋值时，可能需要双引号来包括值。
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
 
-### Linux(使用 export 设置环境变量）
-```sh
-# 1、安装模块
-pip install miservice_fork
-
-# 2、设置环境用户参数
-export MI_USER=xxxx
-export MI_PASS=xxx
-
-# 3、使用micli list 得到did
-micli list
-
-# 4、根据did设置环境DID参数
-export MI_DID=xxxx
-```
-
 ## 一点原理
 
 [不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
 
 ## 准备
 
 1. ChatGPT id
@@ -174,16 +157,16 @@
 | gemini_key               | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                                                                                            |
 | qwen_key                 | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                                                                            |
 | cookie                   | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                                                                            |
 | mi_did                   | 设备did                                                                                     |                                                                                                           |                                                                                                                            |
 | use_command              | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                                                                            |
 | mute_xiaoai              | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                                                                            |
 | verbose                  | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                                                                            |
-| bot                      | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                                                                                            |
-| tts                      | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`                                                                                                 |
+| bot                      | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                           | `chatgptapi`                                                                                              |                                                                                                                            |
+| tts                      | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`                                                                                                 |
 | tts_voice                | TTS 的嗓音                                                                                  | `zh-CN-XiaoxiaoNeural`(edge), `alloy`(openai), `zh-CN-XiaoxiaoMultilingualNeural`(azure)                  |                                                                                                                            |
 | prompt                   | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                                                                                            |
 | keyword                  | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                                                                                            |
 | change_prompt_keyword    | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                                                                                            |
 | start_conversation       | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                                                                                            |
 | end_conversation         | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                                                                                            |
 | stream                   | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                                                                                            |
@@ -191,14 +174,19 @@
 | gpt_options              | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                                                                            |
 | bing_cookie_path         | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                                                                            |
 | bing_cookies             | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                                                                            |
 | deployment_id            | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                                                                            |
 | api_base                 | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |                                                                                                                            |
 | azure_tts_speech_key     | Azure TTS key                                                                               | null                                                                                                      |                                                                                                                            |
 | azure_tts_service_region | Azure TTS 服务地区                                                                          | `eastasia`                                                                                                | [Regions - Speech service - Azure AI services](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/regions) |
+| volc_accesskey | 火山引擎accesskey [参考](https://console.volcengine.com/iam/keymanage/)                                |                                                                                                 |  |
+| volc_secretkey | 火山引擎secretkey [参考](https://console.volcengine.com/iam/keymanage/)                                |                                                                                                 | |
+| volc_tts_app | 火山引擎  TTS app 服务   [参考]( https://console.volcengine.com/sami/)                          |                                  |  |
+| volc_tts_speaker | 火山引擎 TTS speaker   [参考]( https://www.volcengine.com/docs/6489/93478)                          |   `zh_female_qingxin`                               |  |
+
 
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
```

### Comparing `xiaogpt-2.42/pyproject.toml` & `xiaogpt-2.50/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,19 @@
     "langchain>=0.0.343",
     "beautifulsoup4>=4.12.0",
     "google-search-results>=2.4.2",
     "google-generativeai",
     "numexpr>=2.8.6",
     "dashscope>=1.10.0",
     "azure-cognitiveservices-speech>=1.37.0",
+    "multidict>=6.0.5",
+    "volcengine>=1.0.136",
 ]
 dynamic = []
-version = "2.42"
+version = "2.50"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
 
@@ -53,19 +55,21 @@
     "bingimagecreator==0.5.0",
     "cachetools==5.3.2",
     "certifi==2024.2.2",
     "charset-normalizer==3.3.2",
     "colorama==0.4.6 ; platform_system == \"Windows\"",
     "dashscope==1.10.0",
     "dataclasses-json==0.6.3",
+    "decorator==5.1.1",
     "distro==1.9.0",
     "edge-tts==6.1.10",
     "edgegpt==0.1.26",
     "exceptiongroup==1.2.0 ; python_version < \"3.11\"",
     "frozenlist==1.4.1",
+    "google==3.0.0",
     "google-ai-generativelanguage==0.6.1",
     "google-api-core==2.15.0",
     "google-api-core[grpc]==2.15.0",
     "google-api-python-client==2.125.0",
     "google-auth==2.26.1",
     "google-auth-httplib2==0.2.0",
     "google-generativeai==0.5.0",
@@ -87,47 +91,53 @@
     "langchain-core==0.1.42",
     "langchain-text-splitters==0.0.1",
     "langsmith==0.1.45",
     "markdown-it-py==3.0.0",
     "marshmallow==3.20.1",
     "mdurl==0.1.2",
     "miservice-fork==2.4.3",
-    "multidict==6.0.4",
+    "multidict==6.0.5",
     "mutagen==1.47.0",
     "mypy-extensions==1.0.0",
     "numexpr==2.10.0",
     "numpy==1.26.3",
     "openai==1.17.1",
     "orjson==3.10.0",
     "packaging==23.2",
     "prompt-toolkit==3.0.43",
     "proto-plus==1.23.0",
     "protobuf==4.25.1",
+    "py==1.11.0",
     "pyasn1==0.5.1",
     "pyasn1-modules==0.3.0",
+    "pycryptodome==3.9.9",
     "pydantic==2.5.3",
     "pydantic-core==2.14.6",
     "pygments==2.17.2",
     "pyjwt==2.8.0",
     "pyparsing==3.1.2 ; python_version > \"3.0\"",
+    "pytz==2020.5",
     "pyyaml==6.0.1",
     "regex==2023.12.25",
     "requests==2.31.0",
+    "retry==0.9.2",
     "rich==13.7.1",
     "rsa==4.9",
+    "six==1.16.0",
     "sniffio==1.3.0",
     "socksio==1.0.0",
     "soupsieve==2.5",
     "sqlalchemy==2.0.25",
     "tenacity==8.2.3",
     "tqdm==4.66.1",
     "typing-extensions==4.9.0",
     "typing-inspect==0.9.0",
     "uritemplate==4.1.1",
     "urllib3==2.1.0",
+    "volcengine==1.0.136",
     "wcwidth==0.2.13",
     "websockets==12.0",
     "yarl==1.9.4",
     "zhipuai==2.0.1",
 ]
 
 [tool.pdm]
```

### Comparing `xiaogpt-2.42/xiaogpt/bot/__init__.py` & `xiaogpt-2.50/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/bot/base_bot.py` & `xiaogpt-2.50/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.50/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.50/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.50/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.50/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/bot/newbing_bot.py` & `xiaogpt-2.50/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.50/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/cli.py` & `xiaogpt-2.50/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/config.py` & `xiaogpt-2.50/xiaogpt/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,14 +83,24 @@
     tts: Literal["mi", "edge", "azure", "openai"] = "mi"
     tts_voice: str | None = None
     gpt_options: dict[str, Any] = field(default_factory=dict)
     bing_cookie_path: str = ""
     bing_cookies: dict | None = None
     azure_tts_speech_key: str | None = None
     azure_tts_service_region: str = "eastasia"
+    volc_accesskey: str = os.getenv(
+        "VOLC_ACCESSKEY", ""
+    )  # https://console.volcengine.com/iam/keymanage/
+    volc_secretkey: str = os.getenv("VOLC_SECRETKEY", "")
+    volc_tts_app: str = os.getenv(
+        "VOLC_TTS_APP", ""
+    )  # https://console.volcengine.com/sami
+    volc_tts_speaker: str = os.getenv(
+        "VOLC_TTS_SPEAPER", "zh_female_qingxin"
+    )  # https://www.volcengine.com/docs/6489/93478
 
     def __post_init__(self) -> None:
         if self.proxy:
             validate_proxy(self.proxy)
         if self.bot == "newbing":
             if not (self.bing_cookie_path or self.bing_cookies):
                 raise Exception(
```

### Comparing `xiaogpt-2.42/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.50/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/langchain/chain.py` & `xiaogpt-2.50/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.50/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.50/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/tts/azure.py` & `xiaogpt-2.50/xiaogpt/tts/azure.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/tts/base.py` & `xiaogpt-2.50/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/tts/edge.py` & `xiaogpt-2.50/xiaogpt/tts/edge.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/tts/mi.py` & `xiaogpt-2.50/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/tts/openai.py` & `xiaogpt-2.50/xiaogpt/tts/openai.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/utils.py` & `xiaogpt-2.50/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.42/xiaogpt/xiaogpt.py` & `xiaogpt-2.50/xiaogpt/xiaogpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from xiaogpt.config import (
     COOKIE_TEMPLATE,
     LATEST_ASK_API,
     MI_ASK_SIMULATE_DATA,
     WAKEUP_KEYWORD,
     Config,
 )
-from xiaogpt.tts import TTS, EdgeTTS, MiTTS, AzureTTS
+from xiaogpt.tts import TTS, EdgeTTS, MiTTS, AzureTTS, VolcTTS
 from xiaogpt.tts.openai import OpenAITTS
 from xiaogpt.utils import (
     parse_cookie_string,
 )
 
 EOF = object()
 
@@ -58,15 +58,17 @@
             session._cookie_jar = self.cookie_jar
             while True:
                 self.log.debug(
                     "Listening new message, timestamp: %s", self.last_timestamp
                 )
                 new_record = await self.get_latest_ask_from_xiaoai(session)
                 start = time.perf_counter()
-                self.log.debug("Polling_event, timestamp: %s", self.last_timestamp)
+                self.log.debug(
+                    "Polling_event, timestamp: %s %s", self.last_timestamp, new_record
+                )
                 await self.polling_event.wait()
                 if (
                     self.config.mute_xiaoai
                     and new_record
                     and self.need_ask_gpt(new_record)
                 ):
                     await self.stop_if_xiaoai_is_playing()
@@ -258,14 +260,16 @@
     def tts(self) -> TTS:
         if self.config.tts == "edge":
             return EdgeTTS(self.mina_service, self.device_id, self.config)
         elif self.config.tts == "azure":
             return AzureTTS(self.mina_service, self.device_id, self.config)
         elif self.config.tts == "openai":
             return OpenAITTS(self.mina_service, self.device_id, self.config)
+        elif self.config.tts == "volc":
+            return VolcTTS(self.mina_service, self.device_id, self.config)
         else:
             return MiTTS(self.mina_service, self.device_id, self.config)
 
     async def wait_for_tts_finish(self):
         while True:
             if not await self.get_if_xiaoai_is_playing():
                 break
@@ -351,15 +355,14 @@
         )
         print(f"或用[green]{self.config.start_conversation}[/]开始持续对话")
         while True:
             self.polling_event.set()
             new_record = await self.last_record.get()
             self.polling_event.clear()  # stop polling when processing the question
             query = new_record.get("query", "").strip()
-
             if query == self.config.start_conversation:
                 if not self.in_conversation:
                     print("开始对话")
                     self.in_conversation = True
                     await self.wakeup_xiaoai()
                 await self.stop_if_xiaoai_is_playing()
                 continue
```

### Comparing `xiaogpt-2.42/PKG-INFO` & `xiaogpt-2.50/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.42
+Version: 2.50
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -20,14 +20,16 @@
 Requires-Dist: langchain>=0.0.343
 Requires-Dist: beautifulsoup4>=4.12.0
 Requires-Dist: google-search-results>=2.4.2
 Requires-Dist: google-generativeai
 Requires-Dist: numexpr>=2.8.6
 Requires-Dist: dashscope>=1.10.0
 Requires-Dist: azure-cognitiveservices-speech>=1.37.0
+Requires-Dist: multidict>=6.0.5
+Requires-Dist: volcengine>=1.0.136
 Requires-Dist: aiohttp==3.9.4; extra == "locked"
 Requires-Dist: aiosignal==1.3.1; extra == "locked"
 Requires-Dist: annotated-types==0.6.0; extra == "locked"
 Requires-Dist: anyio==3.7.1; extra == "locked"
 Requires-Dist: async-timeout==4.0.3; python_version < "3.11" and extra == "locked"
 Requires-Dist: attrs==23.2.0; extra == "locked"
 Requires-Dist: azure-cognitiveservices-speech==1.37.0; extra == "locked"
@@ -35,19 +37,21 @@
 Requires-Dist: bingimagecreator==0.5.0; extra == "locked"
 Requires-Dist: cachetools==5.3.2; extra == "locked"
 Requires-Dist: certifi==2024.2.2; extra == "locked"
 Requires-Dist: charset-normalizer==3.3.2; extra == "locked"
 Requires-Dist: colorama==0.4.6; platform_system == "Windows" and extra == "locked"
 Requires-Dist: dashscope==1.10.0; extra == "locked"
 Requires-Dist: dataclasses-json==0.6.3; extra == "locked"
+Requires-Dist: decorator==5.1.1; extra == "locked"
 Requires-Dist: distro==1.9.0; extra == "locked"
 Requires-Dist: edge-tts==6.1.10; extra == "locked"
 Requires-Dist: edgegpt==0.1.26; extra == "locked"
 Requires-Dist: exceptiongroup==1.2.0; python_version < "3.11" and extra == "locked"
 Requires-Dist: frozenlist==1.4.1; extra == "locked"
+Requires-Dist: google==3.0.0; extra == "locked"
 Requires-Dist: google-ai-generativelanguage==0.6.1; extra == "locked"
 Requires-Dist: google-api-core==2.15.0; extra == "locked"
 Requires-Dist: google-api-core[grpc]==2.15.0; extra == "locked"
 Requires-Dist: google-api-python-client==2.125.0; extra == "locked"
 Requires-Dist: google-auth==2.26.1; extra == "locked"
 Requires-Dist: google-auth-httplib2==0.2.0; extra == "locked"
 Requires-Dist: google-generativeai==0.5.0; extra == "locked"
@@ -69,47 +73,53 @@
 Requires-Dist: langchain-core==0.1.42; extra == "locked"
 Requires-Dist: langchain-text-splitters==0.0.1; extra == "locked"
 Requires-Dist: langsmith==0.1.45; extra == "locked"
 Requires-Dist: markdown-it-py==3.0.0; extra == "locked"
 Requires-Dist: marshmallow==3.20.1; extra == "locked"
 Requires-Dist: mdurl==0.1.2; extra == "locked"
 Requires-Dist: miservice-fork==2.4.3; extra == "locked"
-Requires-Dist: multidict==6.0.4; extra == "locked"
+Requires-Dist: multidict==6.0.5; extra == "locked"
 Requires-Dist: mutagen==1.47.0; extra == "locked"
 Requires-Dist: mypy-extensions==1.0.0; extra == "locked"
 Requires-Dist: numexpr==2.10.0; extra == "locked"
 Requires-Dist: numpy==1.26.3; extra == "locked"
 Requires-Dist: openai==1.17.1; extra == "locked"
 Requires-Dist: orjson==3.10.0; extra == "locked"
 Requires-Dist: packaging==23.2; extra == "locked"
 Requires-Dist: prompt-toolkit==3.0.43; extra == "locked"
 Requires-Dist: proto-plus==1.23.0; extra == "locked"
 Requires-Dist: protobuf==4.25.1; extra == "locked"
+Requires-Dist: py==1.11.0; extra == "locked"
 Requires-Dist: pyasn1==0.5.1; extra == "locked"
 Requires-Dist: pyasn1-modules==0.3.0; extra == "locked"
+Requires-Dist: pycryptodome==3.9.9; extra == "locked"
 Requires-Dist: pydantic==2.5.3; extra == "locked"
 Requires-Dist: pydantic-core==2.14.6; extra == "locked"
 Requires-Dist: pygments==2.17.2; extra == "locked"
 Requires-Dist: pyjwt==2.8.0; extra == "locked"
 Requires-Dist: pyparsing==3.1.2; python_version > "3.0" and extra == "locked"
+Requires-Dist: pytz==2020.5; extra == "locked"
 Requires-Dist: pyyaml==6.0.1; extra == "locked"
 Requires-Dist: regex==2023.12.25; extra == "locked"
 Requires-Dist: requests==2.31.0; extra == "locked"
+Requires-Dist: retry==0.9.2; extra == "locked"
 Requires-Dist: rich==13.7.1; extra == "locked"
 Requires-Dist: rsa==4.9; extra == "locked"
+Requires-Dist: six==1.16.0; extra == "locked"
 Requires-Dist: sniffio==1.3.0; extra == "locked"
 Requires-Dist: socksio==1.0.0; extra == "locked"
 Requires-Dist: soupsieve==2.5; extra == "locked"
 Requires-Dist: sqlalchemy==2.0.25; extra == "locked"
 Requires-Dist: tenacity==8.2.3; extra == "locked"
 Requires-Dist: tqdm==4.66.1; extra == "locked"
 Requires-Dist: typing-extensions==4.9.0; extra == "locked"
 Requires-Dist: typing-inspect==0.9.0; extra == "locked"
 Requires-Dist: uritemplate==4.1.1; extra == "locked"
 Requires-Dist: urllib3==2.1.0; extra == "locked"
+Requires-Dist: volcengine==1.0.136; extra == "locked"
 Requires-Dist: wcwidth==0.2.13; extra == "locked"
 Requires-Dist: websockets==12.0; extra == "locked"
 Requires-Dist: yarl==1.9.4; extra == "locked"
 Requires-Dist: zhipuai==2.0.1; extra == "locked"
 Provides-Extra: locked
 Description-Content-Type: text/markdown
 
@@ -130,41 +140,24 @@
 - ChatGPT
 - New Bing
 - [ChatGLM](http://open.bigmodel.cn/)
 - [Gemini](https://makersuite.google.com/app/apikey)
 - [通义千问](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
 
 ## 获取小米音响DID
-### Windows(使用 set 设置环境变量）
-```cmd
-pip install miservice_fork
-set MI_USER=xxxx
-set MI_PASS=xxx
-micli list 得到did
-set MI_DID=xxxx
-```
+系统和Shell|Linux *sh|Windows CMD用户|Windows PowerShell用户
+-|-|-|-
+1、安装包|`pip install miservice_fork`|`pip install miservice_fork`|`pip install miservice_fork`
+2、设置变量|`export MI_USER=xxx` <br> `export MI_PASS=xxx`|`set MI_USER=xxx`<br>`set MI_PASS=xxx`|`$env:MI_USER="xxx"` <br> `$env:MI_PASS="xxx"`
+3、取得MI_DID|`micli list` |`micli list` |`micli list` 
+4、设置MI_DID|`export MI_DID=xxx`| `set MI_DID=xxx`| `$env:MI_DID="xxx"`
 
+- 注意不同shell 对环境变量的处理是不同的，尤其是powershell赋值时，可能需要双引号来包括值。
 - 如果获取did报错时，请更换一下无线网络，有很大概率解决问题。
 
-### Linux(使用 export 设置环境变量）
-```sh
-# 1、安装模块
-pip install miservice_fork
-
-# 2、设置环境用户参数
-export MI_USER=xxxx
-export MI_PASS=xxx
-
-# 3、使用micli list 得到did
-micli list
-
-# 4、根据did设置环境DID参数
-export MI_DID=xxxx
-```
-
 ## 一点原理
 
 [不用 root 使用小爱同学和 ChatGPT 交互折腾记](https://github.com/yihong0618/gitblog/issues/258)
 
 ## 准备
 
 1. ChatGPT id
@@ -289,16 +282,16 @@
 | gemini_key               | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                                                                                            |
 | qwen_key                 | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                                                                            |
 | cookie                   | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                                                                            |
 | mi_did                   | 设备did                                                                                     |                                                                                                           |                                                                                                                            |
 | use_command              | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                                                                            |
 | mute_xiaoai              | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                                                                            |
 | verbose                  | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                                                                            |
-| bot                      | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                                                                                            |
-| tts                      | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`                                                                                                 |
+| bot                      | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                           | `chatgptapi`                                                                                              |                                                                                                                            |
+| tts                      | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`                                                                                                 |
 | tts_voice                | TTS 的嗓音                                                                                  | `zh-CN-XiaoxiaoNeural`(edge), `alloy`(openai), `zh-CN-XiaoxiaoMultilingualNeural`(azure)                  |                                                                                                                            |
 | prompt                   | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                                                                                            |
 | keyword                  | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                                                                                            |
 | change_prompt_keyword    | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                                                                                            |
 | start_conversation       | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                                                                                            |
 | end_conversation         | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                                                                                            |
 | stream                   | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                                                                                            |
@@ -306,14 +299,19 @@
 | gpt_options              | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                                                                            |
 | bing_cookie_path         | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                                                                            |
 | bing_cookies             | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                                                                            |
 | deployment_id            | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                                                                            |
 | api_base                 | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |                                                                                                                            |
 | azure_tts_speech_key     | Azure TTS key                                                                               | null                                                                                                      |                                                                                                                            |
 | azure_tts_service_region | Azure TTS 服务地区                                                                          | `eastasia`                                                                                                | [Regions - Speech service - Azure AI services](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/regions) |
+| volc_accesskey | 火山引擎accesskey [参考](https://console.volcengine.com/iam/keymanage/)                                |                                                                                                 |  |
+| volc_secretkey | 火山引擎secretkey [参考](https://console.volcengine.com/iam/keymanage/)                                |                                                                                                 | |
+| volc_tts_app | 火山引擎  TTS app 服务   [参考]( https://console.volcengine.com/sami/)                          |                                  |  |
+| volc_tts_speaker | 火山引擎 TTS speaker   [参考]( https://www.volcengine.com/docs/6489/93478)                          |   `zh_female_qingxin`                               |  |
+
 
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
```

