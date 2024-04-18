# Comparing `tmp/dublib-0.4.0.tar.gz` & `tmp/dublib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dublib-0.4.0.tar", last modified: Thu Apr  4 22:46:26 2024, max compression
+gzip compressed data, was "dublib-0.5.0.tar", last modified: Thu Apr 18 19:18:08 2024, max compression
```

## Comparing `dublib-0.4.0.tar` & `dublib-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:26.818866 dublib-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-04 22:46:22.000000 dublib-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-04 22:46:26.818866 dublib-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-04 22:46:22.000000 dublib-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-04 22:46:22.000000 dublib-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:46:26.818866 dublib-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:26.814866 dublib-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:26.818866 dublib-0.4.0/src/dublib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:26.818866 dublib-0.4.0/src/dublib/Exceptions/
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Exceptions/StyledPrinter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Exceptions/Terminalyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Exceptions/WebRequestor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Exceptions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8986 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Polyglot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/StyledPrinter.py
--rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/Terminalyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27075 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/WebRequestor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:22.000000 dublib-0.4.0/src/dublib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:46:26.818866 dublib-0.4.0/src/dublib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-04 22:46:26.000000 dublib-0.4.0/src/dublib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 22:46:26.000000 dublib-0.4.0/src/dublib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:46:26.000000 dublib-0.4.0/src/dublib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 22:46:26.000000 dublib-0.4.0/src/dublib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 22:46:26.000000 dublib-0.4.0/src/dublib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:08.365850 dublib-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 19:18:03.000000 dublib-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-18 19:18:08.365850 dublib-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 19:18:03.000000 dublib-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-18 19:18:03.000000 dublib-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:18:08.365850 dublib-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:08.361850 dublib-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:08.365850 dublib-0.5.0/src/dublib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:08.365850 dublib-0.5.0/src/dublib/Exceptions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Exceptions/StyledPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Exceptions/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Exceptions/WebRequestor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Exceptions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9391 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Polyglot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/StyledPrinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30603 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/WebRequestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:03.000000 dublib-0.5.0/src/dublib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:18:08.365850 dublib-0.5.0/src/dublib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-18 19:18:08.000000 dublib-0.5.0/src/dublib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-18 19:18:08.000000 dublib-0.5.0/src/dublib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:18:08.000000 dublib-0.5.0/src/dublib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 19:18:08.000000 dublib-0.5.0/src/dublib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 19:18:08.000000 dublib-0.5.0/src/dublib.egg-info/top_level.txt
```

### Comparing `dublib-0.4.0/LICENSE` & `dublib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dublib-0.4.0/PKG-INFO` & `dublib-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.4.0
+Version: 0.5.0
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -36,14 +36,15 @@
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: curl_cffi>=0.6.0
 Requires-Dist: fake_useragent
 Requires-Dist: httpx
 Requires-Dist: httpx[http2]
```

### Comparing `dublib-0.4.0/README.md` & `dublib-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dublib-0.4.0/pyproject.toml` & `dublib-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "cython"]
 
 [project]
 name = "dublib"
-version = "0.4.0"
+version = "0.5.0"
 description = "Коллекция модулей от DUB1401."
 authors = [
 	{name = "DUB1401", email="vlad.milosta@outlook.com"}
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
@@ -16,15 +16,16 @@
 	"Development Status :: 4 - Beta",
 	"License :: OSI Approved :: The Unlicense (Unlicense)",
 	"Natural Language :: Russian",
 	"Operating System :: OS Independent",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
-	"Programming Language :: Python :: 3.12"
+	"Programming Language :: Python :: 3.12",
+	"Programming Language :: Python :: 3.13"
 ]
 
 [project.urls]
 Documentation = "https://github.com/DUB1401/dublib/tree/main/docs"
 "Source Code" = "https://github.com/DUB1401/dublib"
 "Bug Tracker" = "https://github.com/DUB1401/dublib/issues"
 Changelog = "https://github.com/DUB1401/dublib/releases"
```

### Comparing `dublib-0.4.0/src/dublib/Exceptions/StyledPrinter.py` & `dublib-0.5.0/src/dublib/Exceptions/StyledPrinter.py`

 * *Files identical despite different names*

### Comparing `dublib-0.4.0/src/dublib/Exceptions/Terminalyzer.py` & `dublib-0.5.0/src/dublib/Exceptions/Terminalyzer.py`

 * *Files identical despite different names*

### Comparing `dublib-0.4.0/src/dublib/Exceptions/WebRequestor.py` & `dublib-0.5.0/src/dublib/Exceptions/WebRequestor.py`

 * *Files identical despite different names*

### Comparing `dublib-0.4.0/src/dublib/Methods.py` & `dublib-0.5.0/src/dublib/Methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -189,14 +189,25 @@
 		while not text[0].isalpha(): text.pop(0)
 		while not text[-1].isalpha(): text.pop()
 
 	except:
 		# Очистка строки.
 		text = ""
 
+def Zerotify(value: any) -> any:
+	"""
+	Преобразует значения, логически интерпретируемые в False, в тип None.
+		value – обрабатываемое значение.
+	"""
+
+	# Если значение логически интерпретируется в False, обнулить его.
+	if bool(value) == False: value = None
+
+	return value
+
 #==========================================================================================#
 # >>>>> ФУНКЦИИ РАБОТЫ С JSON <<<<< #
 #==========================================================================================#
 
 def ReadJSON(path: str) -> dict:
 	"""
 	Читает файл JSON и конвертирует его в словарь.
```

### Comparing `dublib-0.4.0/src/dublib/Polyglot.py` & `dublib-0.5.0/src/dublib/Polyglot.py`

 * *Files identical despite different names*

### Comparing `dublib-0.4.0/src/dublib/StyledPrinter.py` & `dublib-0.5.0/src/dublib/StyledPrinter.py`

 * *Files identical despite different names*

### Comparing `dublib-0.4.0/src/dublib/Terminalyzer.py` & `dublib-0.5.0/src/dublib/Terminalyzer.py`

 * *Files identical despite different names*

### Comparing `dublib-0.4.0/src/dublib/WebRequestor.py` & `dublib-0.5.0/src/dublib/WebRequestor.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import importlib
 import requests
 import logging
 import random
 import httpx
 import enum
+import json
 
 #==========================================================================================#
 # >>>>> ДОПОЛНИТЕЛЬНЫЕ КОНФИГУРАЦИИ БИБЛИОТЕК ЗАПРОСОВ <<<<< #
 #==========================================================================================#
 
 class _curl_cffi_config:
 	"""Дополнительная конфигурация библиотеки curl_cffi."""
@@ -109,28 +110,119 @@
 	"""Перечисление поддерживаемых библиотек запросов."""
 
 	curl_cffi = "curl_cffi"
 	requests = "requests"
 	httpx = "httpx"
 		
 class WebResponse:
-	"""Эмуляция структуры ответа библиотеки requests."""
+	"""Унифицированная объектная структура ответа библиотек запросов."""
+
+	#==========================================================================================#
+	# >>>>> СВОЙСТВА ТОЛЬКО ДЛЯ ЧТЕНИЯ <<<<< #
+	#==========================================================================================#
+
+	@property
+	def content(self) -> bytes | None:
+		"""Бинарное представление ответа."""
+
+		return self.__content
+
+	@property
+	def json(self) -> dict | None:
+		"""Десериализованное в словарь из JSON представление ответа."""
+
+		return self.__json
+
+	@property
+	def status_code(self) -> int | None:
+		"""Код ответа."""
+
+		return self.__status_code
+
+	@property
+	def text(self) -> str | None:
+		"""Текстовое представление ответа."""
+
+		return self.__text
+
+	#==========================================================================================#
+	# >>>>> ПРИВАТНЫЕ МЕТОДЫ <<<<< #
+	#==========================================================================================#
+
+	def __TryDeserialize(self, text: str) -> dict | None:
+		# Результат десериализации.
+		Result = None
+
+		try:
+			# Попытка десериализации.
+			Result = json.loads(text)
+
+		except: pass
+
+		return Result
+
+	#==========================================================================================#
+	# >>>>> ПУБЛИЧНЫЕ МЕТОДЫ <<<<< #
+	#==========================================================================================#
 
 	def __init__(self):
-		"""Эмуляция структуры ответа библиотеки requests."""
+		"""Унифицированная объектная структура ответа библиотек запросов."""
 
 		#---> Генерация динамических свойств.
 		#==========================================================================================#
 		# Статус ответа.
-		self.status_code = None
+		self.__status_code = None
 		# Бинарное представление ответа.
-		self.content = None
+		self.__content = None
+		# Десериализованное в словарь из JSON представление ответа.
+		self.__json = None
 		# Текстовое представление ответа.
-		self.text = None
-		
+		self.__text = None
+
+	def generate_by_text(self, text: str | None):
+		"""
+		Генерирует интерпретации ответа на основе текста.
+			text – текстовое представление ответа.
+		"""
+
+		# Если запрос успешен.
+		if text:
+			# Установка интерпретаций.
+			self.__status_code = 200
+			self.__text = text
+			self.__content = bytes(text)
+			self.__json = self.__TryDeserialize(text)
+
+	def parse_response(self, response: requests.Response | httpx.Response | curl_cffi_requests.Response):
+		"""
+		Парсит ответ библиотеки в унифицированный формат.
+			response – ответ библиотеки.
+		"""
+
+		# Установка кода ответа.
+		self.__status_code = response.status_code
+		self.__text = response.text
+		self.__content = response.content
+		self.__json = self.__TryDeserialize(response.text)
+
+	def set_data(self, status_code: int | None = None, text: str | None = None, content: bytes | None = None, json: dict | None = None):
+		"""
+		Присваивает значения интерпретациям ответа.
+			status_code – код ответа;
+			text – текстовое представление ответа;
+			content – бинарное представление ответа;
+			json – десериализованное в словарь из JSON представление ответа.
+		"""
+
+		# Проверка и установка типов значений.
+		if status_code: self.__status_code = status_code
+		if text: self.__text = text
+		if content: self.__content = content
+		if json: self.__json = json
+
 #==========================================================================================#
 # >>>>> ОСНОВНЫЕ КЛАССЫ <<<<< #
 #==========================================================================================#
 
 class WebConfig:
 	"""Конфигурация запросчика."""
 
@@ -354,15 +446,15 @@
 			headers – словарь заголовков;
 			cookies – словарь куков.
 		"""
 
 		# Обработка заголовков.
 		headers = self.__MergeHeaders(headers)
 		# Выполнение запроса.
-		Response = self.__Session.get(url, params = params, headers = headers, cookies = cookies, proxies = self.__GetProxy())
+		Response.parse_response(self.__Session.get(url, params = params, headers = headers, cookies = cookies, proxies = self.__GetProxy()))
 
 		return Response
 
 	def __curl_cffi_POST(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None) -> curl_cffi_requests.Response:
 		"""
 		Отправляет POST запрос через библиотеку curl_cffi.
 			url – адрес запроса;
@@ -372,15 +464,15 @@
 			data – данные запроса;
 			json – сериализованное тело запроса.
 		"""
 		
 		# Обработка заголовков.
 		headers = self.__MergeHeaders(headers)
 		# Выполнение запроса.
-		Response = self.__Session.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, proxies = self.__GetProxy())
+		Response.parse_response(self.__Session.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, proxies = self.__GetProxy()))
 		
 		return Response
 	
 	#==========================================================================================#
 	# >>>>> МЕТОДЫ ЗАПРОСОВ БИБЛИОТЕКИ HTTPX <<<<< #
 	#==========================================================================================#
 
@@ -392,15 +484,15 @@
 			headers – словарь заголовков;
 			cookies – словарь куков.
 		"""
 
 		# Обработка заголовков.
 		headers = self.__MergeHeaders(headers)
 		# Выполнение запроса.
-		Response = self.__Session.get(url, params = params, headers = headers, cookies = cookies, follow_redirects = self.__Config.redirecting)
+		Response.parse_response(self.__Session.get(url, params = params, headers = headers, cookies = cookies, follow_redirects = self.__Config.redirecting))
 
 		return Response
 
 	def __httpx_POST(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None) -> httpx.Response:
 		"""
 		Отправляет POST запрос через библиотеку httpx.
 			url – адрес запроса;
@@ -410,15 +502,15 @@
 			data – данные запроса;
 			json – сериализованное тело запроса.
 		"""
 		
 		# Обработка заголовков.
 		headers = self.__MergeHeaders(headers)
 		# Выполнение запроса.
-		Response = self.__Session.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, follow_redirects = self.__Config.redirecting)
+		Response.parse_response(self.__Session.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, follow_redirects = self.__Config.redirecting))
 		
 		return Response
 	
 	#==========================================================================================#
 	# >>>>> МЕТОДЫ ЗАПРОСОВ БИБЛИОТЕКИ REQUESTS <<<<< #
 	#==========================================================================================#
 
@@ -434,21 +526,20 @@
 		# Обработка заголовков.
 		headers = self.__MergeHeaders(headers)
 		# Эмуляция ответа.
 		Response = WebResponse()
 		
 		try:
 			# Выполнение запроса.
-			Response = self.__Session.get(url, params = params, headers = headers, cookies = cookies, proxies = self.__GetProxy(), allow_redirects = self.__Config.redirecting)
+			Response.parse_response(self.__Session.get(url, params = params, headers = headers, cookies = cookies, proxies = self.__GetProxy(), allow_redirects = self.__Config.redirecting))
 
 		except requests.exceptions.ProxyError as ExceptionData:
 			# Установка значений ответа.
-			Response.status_code = 407
-			Response.text = str(ExceptionData)
-			Response.content = bytes(ExceptionData)
+			Response.generate_by_text(str(ExceptionData))
+			Response.set_data(status_code = 407)
 
 		return Response
 	
 	def __requests_POST(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None) -> requests.Response:
 		"""
 		Отправляет POST запрос через библиотеку requests.
 			url – адрес запроса;
@@ -462,21 +553,20 @@
 		# Обработка заголовков.
 		headers = self.__MergeHeaders(headers)
 		# Эмуляция ответа.
 		Response = WebResponse()
 
 		try:
 			# Выполнение запроса.
-			Response = self.__Session.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, proxies = self.__GetProxy(), allow_redirects = self.__Config.redirecting)
+			Response.parse_response(self.__Session.post(url, params = params, headers = headers, cookies = cookies, data = data, json = json, proxies = self.__GetProxy(), allow_redirects = self.__Config.redirecting))
 		
 		except requests.exceptions.ProxyError as ExceptionData:
 			# Установка значений ответа.
-			Response.status_code = 407
-			Response.text = str(ExceptionData)
-			Response.content = bytes(ExceptionData)
+			Response.generate_by_text(str(ExceptionData))
+			Response.set_data(status_code = 407)
 
 		return Response
 		
 	#==========================================================================================#
 	# >>>>> ОБЩИЕ МЕТОДЫ <<<<< #
 	#==========================================================================================#
 		
@@ -526,15 +616,15 @@
 		# Если используется библиотека httpx, реинициализировать сессию.
 		if self.__Config.lib == WebLibs.httpx: self.__Initialize()
 	
 	#==========================================================================================#
 	# >>>>> ЗАПРОСЫ <<<<< #
 	#==========================================================================================#	
 	
-	def get(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, tries: int = 1) -> requests.Response | httpx.Response:
+	def get(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, tries: int = 1) -> WebResponse:
 		"""
 		Отправляет GET запрос.
 			url – адрес запроса;
 			params – словарь параметров запроса;
 			headers – словарь заголовков;
 			cookies – словарь куков;
 			tries – количество попыток повтора при неудачном выполнении.
@@ -577,15 +667,15 @@
 
 			except Exception as ExceptionData:
 				# Запись в лог ошибки: не удалось выполнить запрос.
 				if self.__Config.logging: logging.error(f"[{LibName}-GET] Description: \"" + str(ExceptionData) + "\".")
 		
 		return Response
 	
-	def post(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None, tries: int = 1) -> requests.Response | httpx.Response:
+	def post(self, url: str, params: dict | None = None, headers: dict | None = None, cookies: dict | None = None, data: any = None, json: dict | None = None, tries: int = 1) -> WebResponse:
 		"""
 		Отправляет POST запрос.
 			url – адрес запроса;
 			params – словарь параметров запроса;
 			headers – словарь заголовков;
 			cookies – словарь куков;
 			data – отправляемые данные;
```

### Comparing `dublib-0.4.0/src/dublib.egg-info/PKG-INFO` & `dublib-0.5.0/src/dublib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.4.0
+Version: 0.5.0
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -36,14 +36,15 @@
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: curl_cffi>=0.6.0
 Requires-Dist: fake_useragent
 Requires-Dist: httpx
 Requires-Dist: httpx[http2]
```

