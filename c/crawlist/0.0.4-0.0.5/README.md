# Comparing `tmp/crawlist-0.0.4.tar.gz` & `tmp/crawlist-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlist-0.0.4.tar", last modified: Sat Apr 13 14:37:50 2024, max compression
+gzip compressed data, was "crawlist-0.0.5.tar", last modified: Thu Apr 18 06:13:31 2024, max compression
```

## Comparing `crawlist-0.0.4.tar` & `crawlist-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:37:50.623803 crawlist-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-13 14:37:40.000000 crawlist-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-13 14:37:40.000000 crawlist-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-13 14:37:50.623803 crawlist-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-13 14:37:40.000000 crawlist-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:37:50.619803 crawlist-0.0.4/crawlist/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:37:50.619803 crawlist-0.0.4/crawlist/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/analyzers/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/analyzers/dynamic_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/analyzers/pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/analyzers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/analyzers/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/analyzers/static_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/analyzers/trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/analyzers/valid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:37:50.619803 crawlist-0.0.4/crawlist/processings/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-13 14:37:40.000000 crawlist-0.0.4/crawlist/processings/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:37:50.623803 crawlist-0.0.4/crawlist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-13 14:37:50.000000 crawlist-0.0.4/crawlist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-13 14:37:50.000000 crawlist-0.0.4/crawlist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:37:50.000000 crawlist-0.0.4/crawlist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 14:37:50.000000 crawlist-0.0.4/crawlist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 14:37:50.000000 crawlist-0.0.4/crawlist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:37:50.623803 crawlist-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-13 14:37:40.000000 crawlist-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.630055 crawlist-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 06:13:27.000000 crawlist-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 06:13:27.000000 crawlist-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-18 06:13:31.630055 crawlist-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-18 06:13:27.000000 crawlist-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.626055 crawlist-0.0.5/crawlist/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.626055 crawlist-0.0.5/crawlist/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.626055 crawlist-0.0.5/crawlist/analyzers/pager/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/pager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/pager/dynamic_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/pager/pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/pager/static_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.630055 crawlist-0.0.5/crawlist/processings/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/processings/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/processings/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.630055 crawlist-0.0.5/crawlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-18 06:13:31.000000 crawlist-0.0.5/crawlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 06:13:31.000000 crawlist-0.0.5/crawlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:13:31.000000 crawlist-0.0.5/crawlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 06:13:31.000000 crawlist-0.0.5/crawlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 06:13:31.000000 crawlist-0.0.5/crawlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:13:31.630055 crawlist-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-18 06:13:27.000000 crawlist-0.0.5/setup.py
```

### Comparing `crawlist-0.0.4/LICENSE` & `crawlist-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.4/PKG-INFO` & `crawlist-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.4
+Version: 0.0.5
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `crawlist-0.0.4/README.md` & `crawlist-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.4/crawlist/analyzers/analyzer.py` & `crawlist-0.0.5/crawlist/analyzers/analyzer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import re
 import traceback
 from typing import Any, Generator
-from .selector import Selector
-from .pager import Pager
-from .trie import Trie
+
+from crawlist.analyzers.pager.pager import Pager
+from crawlist.analyzers.selector import Selector
+from crawlist.analyzers.trie import Trie
+from crawlist.annotation import check
+
 
 class BaseAnalyzer(object):
     """
     Analyzer interface, requires subclass method implementation
     """
 
+    @check
     def list(self, limit: int) -> Generator[Any, Any, None]:
         """
         List generator interface, generating one data at a time
         :param limit: Take the latest number of entries
         :return: Captured formatted list
         """
         for element in self.crawl(limit=limit):
             yield self.after(element)
 
+    @check
     def __call__(self, limit: int) -> Generator[Any, Any, None]:
         return self.list(limit=limit)
 
     def crawl(self, limit: int) -> Generator[Any, str, None]:
         raise NotImplementedError
 
     def after(self, html: str) -> Any:
@@ -89,15 +94,15 @@
     """
     Analyzer, beautify output
     """
 
     filter_list = ["\n", "\r", "\t", "<br>", "<br/>", "</br>"]
 
     def after(self, html: str) -> str:
-        # 去除html中无用信息
+        # Remove useless information from HTML
         result_list = []
         i = 0
         while i < len(html):
             flag = True
             for e in AnalyzerPrettify.filter_list:
                 if html[i:i + len(e)] == e:
                     i += len(e)
@@ -118,10 +123,10 @@
 class AnalyzerLinks(Analyzer):
     """
     Analyzer, extract all links
     """
     url_regex = r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+'
 
     def after(self, html: str) -> list:
-        # 使用正则表达式找到所有匹配项
+        # Use regular expressions to find all matches
         links = re.findall(AnalyzerLinks.url_regex, html)
         return links
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crawlist-0.0.4/crawlist/analyzers/dynamic_pager.py` & `crawlist-0.0.5/crawlist/analyzers/pager/dynamic_pager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 import parsel
 from selenium.webdriver.remote.webelement import WebElement
-from .valid import Valid
-from .pager import Pager
-from .selector import WebElementSelector
 from selenium.webdriver.remote.webdriver import WebDriver
-from webdriver_manager.chrome import ChromeDriverManager
-from selenium import webdriver as wd
-from selenium.webdriver.chrome.service import Service
+
+from crawlist.analyzers.pager.pager import Pager
+from crawlist.analyzers.driver import Driver, DefaultDriver
+from crawlist.analyzers.valid import Valid
+from crawlist.analyzers.selector import WebElementSelector
+from crawlist.annotation import check
 
 
 class DynamicPager(Pager):
-    def __init__(self, webdriver: WebDriver = None, interval: float = 0.1) -> None:
+    @check
+    def __init__(self, webdriver: Driver = None, interval: float = 0.1) -> None:
         """
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         if not webdriver:
-            option = wd.ChromeOptions()
-            option.add_argument("start-maximized")
-            option.page_load_strategy = 'eager'
-            option.add_argument("--headless")
-            option.add_argument("window-size=1920x3000")
-            agent = 'user-agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36"'
-            option.add_argument(agent)
-
-            self.webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()), options=option)
-            self.webdriver.implicitly_wait(10)
+            self.webdriver = DefaultDriver()()
         else:
-            self.webdriver = webdriver
+            self.webdriver = webdriver()
         super().__init__(interval=interval)
 
     def click_safety(self, button: WebElement) -> None:
         """
         Attempt to click the button multiple times
         :param button: Button elements
         """
@@ -40,73 +32,76 @@
             try:
                 button.click()
                 self.sleep()
                 break
             except Exception:
                 pass
 
-    def pre_load(self, webdriver: WebDriver = None) -> bool:
-        return False
+    def pre_load(self, webdriver: WebDriver) -> None:
+        pass
 
     def __del__(self):
         try:
             self.webdriver.quit()
         except:
             pass
 
 
 class DynamicRedirectPager(DynamicPager):
-    def __init__(self, uri: str, uri_split: str, webdriver: WebDriver = None, start: int = 1, offset: int = 1,
+    @check
+    def __init__(self, uri: str, uri_split: str, webdriver: Driver = None, start: int = 1, offset: int = 1,
                  interval: float = 0.1) -> None:
         """
         Based on dynamic web page analyzer (redirect page flipping)
         :param uri: First page link
         :param uri_split: Link pagination (using% v proxy) Example: https://www.boc.cn/sourcedb/whpj/index_%v.html
         :param webdriver: WebDriver object for selenium
         :param start: Start page
         :param offset: pagination interval
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert '%v' in uri_split
         assert Valid.is_valid_url(uri) and Valid.is_valid_url(uri_split.replace('%v', str(start)))
         assert offset >= 1 and start >= 0
-        super().__init__(webdriver=webdriver, interval=interval)
-        self.pre_load(webdriver)
         self.index = start
         self.offset = offset
         self.current_uri = uri
         self.uri_split = uri_split
+        super().__init__(webdriver=webdriver, interval=interval)
+        self.pre_load(self.webdriver)
+        self.sleep()
 
     def next(self) -> None:
         self.index += self.offset
         self.current_uri = self.uri_split.replace('%v', str(self.index))
         self.sleep()
 
     @property
     def html(self) -> str:
         self.webdriver.get(self.current_uri)
         return self.webdriver.page_source
 
 
 class DynamicListRedirectPager(DynamicPager):
-    def __init__(self, uris: list, webdriver: WebDriver = None, interval: float = 0.1) -> None:
+    @check
+    def __init__(self, uris: list, webdriver: Driver = None, interval: float = 0.1) -> None:
         """
         Based on dynamic web page analyzer (redirect page flipping)
         :param uris: A list containing multiple uris, executed in order downwards
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
-        assert isinstance(uris, list)
         for uri in uris:
             assert Valid.is_valid_url(uri)
         assert len(uris) > 0
-        super().__init__(webdriver=webdriver, interval=interval)
-        self.pre_load(webdriver)
-        self.index = 0
         self.uris = uris
+        self.index = 0
+        super().__init__(webdriver=webdriver, interval=interval)
+        self.pre_load(self.webdriver)
+        self.sleep()
 
     def next(self) -> None:
         if self.index >= len(self.uris):
             return
         self.index += 1
         self.sleep()
 
@@ -116,26 +111,27 @@
             return ""
         uri = self.uris[self.index]
         self.webdriver.get(uri)
         return self.webdriver.page_source
 
 
 class DynamicScrollPager(DynamicPager):
-    def __init__(self, uri: str, webdriver: WebDriver = None, interval: float = 1) -> None:
+    @check
+    def __init__(self, uri: str, webdriver: Driver = None, interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (scrolling and flipping)
         :param uri: webpage link, which is a scrolling page
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert Valid.is_valid_url(uri)
-        super().__init__(webdriver=webdriver, interval=interval)
-        if not self.pre_load(self.webdriver):
-            self.webdriver.get(uri)
         self.uri = uri
+        super().__init__(webdriver=webdriver, interval=interval)
+        self.pre_load(self.webdriver)
+        self.sleep()
 
     js_code = '''he = setInterval(() => {
                         document.documentElement.scrollTop += document.documentElement.scrollHeight
                         if (document.documentElement.scrollTop >= (document.documentElement.scrollHeight - document.documentElement.scrollWidth)) {
                             clearInterval(he)
                         }
                     },100)
@@ -145,61 +141,69 @@
         self.webdriver.execute_script(DynamicScrollPager.js_code)
         self.sleep()
 
     @property
     def html(self) -> str:
         return self.webdriver.page_source
 
+    def pre_load(self, webdriver: WebDriver) -> None:
+        webdriver.get(self.uri)
+
 
 class DynamicLineButtonPager(DynamicPager):
-    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: WebDriver = None,
+    @check
+    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver = None,
                  interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (row button page flipping)
         :param uri: webpage link, which is a row button for flipping pages
         :param button.selector: row button selector
         :param webdriver: WebDriver object for selenium
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert Valid.is_valid_url(uri)
+        self.uri = uri
         super().__init__(webdriver=webdriver, interval=interval)
-        if not self.pre_load(self.webdriver):
-            self.webdriver.get(uri)
+        self.pre_load(self.webdriver)
+        self.sleep()
         assert len(button_selector(self.webdriver, interval=interval)) > 0
-        self.uri = uri
         self.button = button_selector
 
     def next(self) -> None:
         button_element = self.button(self.webdriver, interval=self.interval)[0]
         self.click_safety(button_element)
         self.sleep()
 
     @property
     def html(self) -> str:
         return self.webdriver.page_source
 
+    def pre_load(self, webdriver: WebDriver) -> None:
+        webdriver.get(self.uri)
+
 
 class DynamicNumButtonPager(DynamicPager):
-    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: WebDriver = None, start: int = 1,
+    @check
+    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver = None, start: int = 1,
                  offset: int = 1, interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (digital button flipping)
         :param uri: webpage link, which is a numeric button for flipping pages
         :param button.selector: numeric button selector
         :param webdriver: WebDriver object for selenium
         :param start: Start page
         :param offset: pagination interval
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert Valid.is_valid_url(uri)
+        self.uri = uri
         super().__init__(webdriver=webdriver, interval=interval)
-        if not self.pre_load(self.webdriver):
-            self.webdriver.get(uri)
+        self.pre_load(self.webdriver)
+        self.sleep()
         assert len(button_selector(self.webdriver, interval=interval)) > 0
-        self.uri = uri
         self.index = 1
         self.offset = offset
         self.button = button_selector
         while start - 1:
             start -= 1
             self.next_one()
 
@@ -248,33 +252,37 @@
         :return: The selected button, if not found, is None
         """
         for element in elements:
             if DynamicNumButtonPager.check_num_button(element, num):
                 return element
         return None
 
+    def pre_load(self, webdriver: WebDriver) -> None:
+        webdriver.get(self.uri)
+
 
 class DynamicNextButtonPager(DynamicPager):
-    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: WebDriver = None, start: int = 1,
+    @check
+    def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: Driver = None, start: int = 1,
                  offset: int = 1, interval: float = 1) -> None:
         """
         Based on dynamic web page analyzer (click the next page button to page)
         :param uri: Web page link, which is a page that can be flipped by clicking the next page button
         :param button.selector: Click on the next page button selector
         :param webdriver: WebDriver object for selenium
         :param start: Start page
         :param offset: pagination interval
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert Valid.is_valid_url(uri)
+        self.uri = uri
         super().__init__(webdriver=webdriver, interval=interval)
-        if not self.pre_load(self.webdriver):
-            self.webdriver.get(uri)
+        self.pre_load(self.webdriver)
+        self.sleep()
         assert len(button_selector(self.webdriver, interval=interval)) > 0
-        self.uri = uri
         self.offset = offset
         self.button = button_selector
         while start - 1:
             start -= 1
             self.next_one()
 
     def next(self) -> None:
@@ -289,7 +297,10 @@
         if button:
             self.click_safety(button)
         self.sleep()
 
     @property
     def html(self) -> str:
         return self.webdriver.page_source
+
+    def pre_load(self, webdriver: WebDriver) -> None:
+        webdriver.get(self.uri)
```

### Comparing `crawlist-0.0.4/crawlist/analyzers/request.py` & `crawlist-0.0.5/crawlist/analyzers/request.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,22 +8,27 @@
 
 class Request(BaseRequest):
     """
     HTTP request object, if it needs to be rewritten, please inherit the Request object
     """
 
     def request(self, uri: str) -> str:
+        raise NotImplementedError
+
+    def __call__(self, uri) -> str:
+        return self.request(uri)
+
+
+class DefaultRequest(Request):
+
+    def request(self, uri: str) -> str:
         try:
             headers = {
                 "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36",
                 'Cache-Control': 'max-age=0',
             }
             r = requests.get(uri, headers=headers)
             r.raise_for_status()
             r.encoding = r.apparent_encoding
             return r.text
         except HTTPError:
             return ""
-
-    def __call__(self, uri) -> str:
-        return self.request(uri)
-
```

### Comparing `crawlist-0.0.4/crawlist/analyzers/selector.py` & `crawlist-0.0.5/crawlist/analyzers/selector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,112 +1,115 @@
 import parsel
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as Ec
 from selenium.webdriver.common.by import By
 
-from .valid import Valid
+from crawlist.analyzers.valid import Valid
+from crawlist.annotation import check
 
 
 class BaseSelector(object):
     pass
 
 
 class Selector(BaseSelector):
+    @check
     def __init__(self, pattern: str) -> None:
         """
         Selector
         :param pattern: Grab rules
         """
         assert self.valid(pattern)
         self.pattern = pattern
 
     def select(self, html: str) -> list[str]:
         raise NotImplementedError
 
-    def valid(self, pattern) -> bool:
+    def valid(self, pattern: str) -> bool:
         return True
 
     def __call__(self, html: str) -> list[str]:
         return self.select(html)
 
 
 class WebElementSelector(BaseSelector):
+    @check
     def __init__(self, pattern: str) -> None:
         """
         WebElement selector (selenium)
         :param pattern: Grab rules
         """
         assert self.valid(pattern)
         self.pattern = pattern
 
     def select(self, webdriver: WebDriver, interval: float = 0.1) -> list[WebElement]:
         raise NotImplementedError
 
-    def valid(self, pattern) -> bool:
+    def valid(self, pattern: str) -> bool:
         raise NotImplementedError
 
     def __call__(self, webdriver: WebDriver, interval: float = 0.1) -> list[WebElement]:
         return self.select(webdriver, interval)
 
 
 class CssSelector(Selector):
     """
     css selector
     """
 
     def select(self, html: str) -> list[str]:
         return parsel.Selector(text=html).css(self.pattern).getall()
 
-    def valid(self, pattern) -> bool:
+    def valid(self, pattern: str) -> bool:
         return Valid.is_valid_css(pattern)
 
 
 class XpathSelector(Selector):
     """
     xpath selector
     """
 
     def select(self, html: str) -> list[str]:
         return parsel.Selector(text=html).xpath(self.pattern).getall()
 
-    def valid(self, pattern) -> bool:
+    def valid(self, pattern: str) -> bool:
         return Valid.is_valid_xpath(pattern)
 
 
 class RegexSelector(Selector):
     """
     regex selector
     """
 
     def select(self, html: str) -> list[str]:
         return parsel.Selector(text=html).re(self.pattern)
 
-    def valid(self, pattern) -> bool:
+    def valid(self, pattern: str) -> bool:
         return Valid.is_valid_regex(pattern)
 
 
 class CssWebElementSelector(WebElementSelector):
 
     def select(self, webdriver: WebDriver, interval: float = 0.1) -> list[WebElement]:
         WebDriverWait(webdriver, interval).until(
             Ec.presence_of_element_located((By.CSS_SELECTOR, self.pattern)))
         return webdriver.find_elements(
             By.CSS_SELECTOR, self.pattern)
 
-    def valid(self, pattern) -> bool:
+    def valid(self, pattern: str) -> bool:
         return Valid.is_valid_css(pattern)
 
 
 class XpathWebElementSelector(WebElementSelector):
 
     def select(self, webdriver: WebDriver, interval: float = 0.1) -> list[WebElement]:
         WebDriverWait(webdriver, interval).until(
             Ec.presence_of_element_located((By.XPATH, self.pattern)))
         return webdriver.find_elements(
             By.XPATH, self.pattern)
 
-    def valid(self, pattern) -> bool:
+    def valid(self, pattern: str) -> bool:
         return Valid.is_valid_xpath(pattern)
```

### Comparing `crawlist-0.0.4/crawlist/analyzers/static_pager.py` & `crawlist-0.0.5/crawlist/analyzers/pager/static_pager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-from .request import Request
-from .valid import Valid
-from .pager import Pager
+from crawlist.analyzers.pager.pager import Pager
+from crawlist.analyzers.request import Request, DefaultRequest
+from crawlist.analyzers.valid import Valid
+from crawlist.annotation import check
 
 
 class StaticPager(Pager):
+    @check
     def __init__(self, request: Request = None, interval: float = 0.1):
         """
         :param request: Request object
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         if not request:
-            self.request = Request()
+            self.request = DefaultRequest()
         else:
             self.request = request
         super().__init__(interval=interval)
 
 
 class StaticRedirectPager(StaticPager):
+    @check
     def __init__(self, uri: str, uri_split: str, request: Request = None, start: int = 1, offset: int = 1,
                  interval: float = 0.1) -> None:
         """
         Based on static web page analyzer (redirect page flipping)
         :param uri: First page link
         :param uri_split: Link pagination (using %v instead) Example: https://www.boc.cn/sourcedb/whpj/index_%v.html
         :param request: Request object
@@ -44,14 +47,15 @@
 
     @property
     def html(self) -> str:
         return self.request(self.current_uri)
 
 
 class StaticListRedirectPager(StaticPager):
+    @check
     def __init__(self, uris: list, request: Request = None, interval: float = 0.1) -> None:
         """
         Based on static web page analyzer (redirect page flipping)
         :param uris: A list containing multiple uris, executed in order downwards
         :param request: Request object
         :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
```

### Comparing `crawlist-0.0.4/crawlist/analyzers/trie.py` & `crawlist-0.0.5/crawlist/analyzers/trie.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.4/crawlist/analyzers/valid.py` & `crawlist-0.0.5/crawlist/analyzers/valid.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.4/crawlist/processings/action.py` & `crawlist-0.0.5/crawlist/processings/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 
+from crawlist.annotation import check
+
 
 class Action:
 
     @staticmethod
+    @check(exclude="driver")
     def click(driver: WebDriver, xpath: str) -> bool:
         """
         Handling click events
         :param driver: selenium webdriver
         :param xpath: Click on the xpath path of the button
         :return: Whether successful
         """
@@ -28,14 +31,15 @@
             try:
                 element.click()
             except Exception:
                 return False
         return True
 
     @staticmethod
+    @check(exclude="driver")
     def inputKeyword(driver: WebDriver, xpath: str, keyword: str) -> bool:
         """
         Handling keyboard input events
         :param driver: selenium webdriver
         :param xpath: The xpath path of the input box
         :param keyword: keyword needs to be passed in
         :return: Whether successful
@@ -45,14 +49,15 @@
         try:
             element.send_keys(keyword)
         except Exception:
             return False
         return True
 
     @staticmethod
+    @check(exclude="driver")
     def sendEnter(driver: WebDriver, xpath: str) -> bool:
         """
         Press the enter key once
         :param driver: selenium webdriver
         :param xpath: The xpath path of the input box
         :return: Whether successful
         """
@@ -61,14 +66,15 @@
         try:
             element.send_keys(Keys.RETURN)
         except Exception:
             return False
         return True
 
     @staticmethod
+    @check(exclude="driver")
     def switchLastTab(driver: WebDriver) -> bool:
         """
         Switch to the last handle
         :param driver: selenium webdriver
         :return: Whether successful
         """
         try:
@@ -77,14 +83,15 @@
                 return False
             driver.switch_to.window(window_handles[-1])
         except Exception as e:
             return False
         return True
 
     @staticmethod
+    @check(exclude="driver")
     def switchTab(driver: WebDriver, index: int) -> bool:
         """
         Switch to the index handle
         :param driver: selenium webdriver
         :param index: The index handle
         :return: Whether successful
         """
@@ -92,14 +99,15 @@
             window_handles = driver.window_handles
             driver.switch_to.window(window_handles[index])
         except Exception as e:
             return False
         return True
 
     @staticmethod
+    @check(exclude="driver")
     def searchRedirect(driver: WebDriver, url: str, keyword: str) -> bool:
         """
         Replace % s in the path with keyword and redirect it
         :param driver:  selenium webdriver
         :param url: Link containing %s
         :param keyword: keyword needs to be passed in
         :return: Whether successful
@@ -108,14 +116,15 @@
             url = url.replace(r"%s", keyword)
             driver.get(url)
         except Exception:
             return False
         return True
 
     @staticmethod
+    @check(exclude="driver")
     def redirect(driver: WebDriver, url: str) -> bool:
         """
         Direct redirection
         :param driver:  selenium webdriver
         :param url: Links that require redirection
         :return: Whether successful
         """
```

### Comparing `crawlist-0.0.4/crawlist.egg-info/PKG-INFO` & `crawlist-0.0.5/crawlist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.4
+Version: 0.0.5
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `crawlist-0.0.4/crawlist.egg-info/SOURCES.txt` & `crawlist-0.0.5/crawlist.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 crawlist/__init__.py
 crawlist/__version__.py
+crawlist/annotation.py
 crawlist.egg-info/PKG-INFO
 crawlist.egg-info/SOURCES.txt
 crawlist.egg-info/dependency_links.txt
 crawlist.egg-info/requires.txt
 crawlist.egg-info/top_level.txt
 crawlist/analyzers/__init__.py
 crawlist/analyzers/analyzer.py
-crawlist/analyzers/dynamic_pager.py
-crawlist/analyzers/pager.py
+crawlist/analyzers/driver.py
 crawlist/analyzers/request.py
 crawlist/analyzers/selector.py
-crawlist/analyzers/static_pager.py
 crawlist/analyzers/trie.py
 crawlist/analyzers/valid.py
+crawlist/analyzers/pager/__init__.py
+crawlist/analyzers/pager/dynamic_pager.py
+crawlist/analyzers/pager/pager.py
+crawlist/analyzers/pager/static_pager.py
 crawlist/processings/__init__.py
-crawlist/processings/action.py
+crawlist/processings/action.py
+crawlist/processings/script.py
```

### Comparing `crawlist-0.0.4/setup.py` & `crawlist-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlist'
 DESCRIPTION = 'A universal solution for web crawling lists'
 URL = 'https://github.com/WwwwwyDev/crawlist'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwyDev'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 # What packages are required for this module to be executed?
 REQUIRED = [
     'parsel', 'selenium>=4.0.0', 'cssselect', 'lxml', 'requests', 'webdriver-manager'
 ]
 
 # What packages are optional?
 EXTRAS = {
```

