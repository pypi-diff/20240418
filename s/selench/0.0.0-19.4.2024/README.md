# Comparing `tmp/selench-0.0.0.tar.gz` & `tmp/selench-19.4.2024.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selench-0.0.0.tar", last modified: Thu Mar 16 18:15:30 2023, max compression
+gzip compressed data, was "selench-19.4.2024.tar", last modified: Thu Apr 18 21:28:59 2024, max compression
```

## Comparing `selench-0.0.0.tar` & `selench-19.4.2024.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:30.503027 selench-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-16 18:15:19.000000 selench-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-16 18:15:30.503027 selench-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-16 18:15:19.000000 selench-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:30.499027 selench-0.0.0/selench/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-16 18:15:19.000000 selench-0.0.0/selench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-03-16 18:15:19.000000 selench-0.0.0/selench/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28578 2023-03-16 18:15:19.000000 selench-0.0.0/selench/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-03-16 18:15:19.000000 selench-0.0.0/selench/wait_for.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:15:30.503027 selench-0.0.0/selench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-16 18:15:30.000000 selench-0.0.0/selench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-16 18:15:30.000000 selench-0.0.0/selench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 18:15:30.000000 selench-0.0.0/selench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-16 18:15:30.000000 selench-0.0.0/selench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 18:15:30.000000 selench-0.0.0/selench.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 18:15:30.503027 selench-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-16 18:15:19.000000 selench-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:59.533492 selench-19.4.2024/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 21:28:55.000000 selench-19.4.2024/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-18 21:28:59.533492 selench-19.4.2024/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-18 21:28:55.000000 selench-19.4.2024/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:59.529492 selench-19.4.2024/selench/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 21:28:55.000000 selench-19.4.2024/selench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28313 2024-04-18 21:28:55.000000 selench-19.4.2024/selench/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-04-18 21:28:55.000000 selench-19.4.2024/selench/wait_for.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:59.533492 selench-19.4.2024/selench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-18 21:28:59.000000 selench-19.4.2024/selench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-18 21:28:59.000000 selench-19.4.2024/selench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:28:59.000000 selench-19.4.2024/selench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 21:28:59.000000 selench-19.4.2024/selench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 21:28:59.000000 selench-19.4.2024/selench.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:28:59.533492 selench-19.4.2024/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-18 21:28:55.000000 selench-19.4.2024/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:59.529492 selench-19.4.2024/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-18 21:28:55.000000 selench-19.4.2024/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-18 21:28:55.000000 selench-19.4.2024/tests/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-18 21:28:55.000000 selench-19.4.2024/tests/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-18 21:28:55.000000 selench-19.4.2024/tests/test_switch_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-18 21:28:55.000000 selench-19.4.2024/tests/test_wait_for.py
```

### Comparing `selench-0.0.0/LICENSE` & `selench-19.4.2024/LICENSE`

 * *Files identical despite different names*

### Comparing `selench-0.0.0/PKG-INFO` & `selench-19.4.2024/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,71 @@
 Metadata-Version: 2.1
 Name: selench
-Version: 0.0.0
-Summary: Selenium WebDriver wrapper for Python
+Version: 19.4.2024
+Summary: Selenium wrapper for Python
 Home-page: https://github.com/dsymbol/selench
 Author: dsymbol
 License: OSI Approved :: MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: selenium==4.19.0
 
 # Selench
 
-Selench is a Python WebDriver wrapper that simplifies the use of the Selenium library. 
+Selench is a wrapper that simplifies the use of the Selenium library. 
 It provides a more concise syntax that makes the code more readable and easier to understand.
 
 ### Key Features
 
 - Elements have an explicit wait time by default
 - Element type detection ( CSS & XPATH )
 
 ## Installation
 
-The easiest way to install the latest version from PyPI is by using
-[pip](https://pip.pypa.io/):
+To install the library, use pip:
 
 ```bash
 pip install selench
 ```
 
-Alternatively, install directly from the GitHub repository:
+Alternatively, install the latest directly from the GitHub repository:
 ```bash
 pip install git+https://github.com/dsymbol/selench.git
 ```
 
-## Documentation
-
-The documentation can be found at https://dsymbol.github.io/selench/
-
 ## Examples
 
-Here are some examples of how to use Selench:
+Navigate to DuckDuckGo and search for 'Hello World!'
 
 ```py
 from selench import Selench, Keys
 
-# Create a new Selench instance
 driver = Selench()
-
-# Navigate to google
-driver.get('https://google.com')
-
-# Search google for 'Hello World!'
-driver.element('input[name="q"]').send_keys('Hello World!', Keys.ENTER)
-
-# Quit the driver
+driver.get('https://duckduckgo.com')
+driver.element('[name=q]').send_keys('Hello World!', Keys.ENTER)
 driver.quit()
 ```
 
-Using PyTest:
+Using PyTest: navigate to DuckDuckGo and search for 'github' assert titles contain 'github'
 
 ```py
 from selench import Selench, Keys
 import pytest
 
-# Create a fixture to provide the driver instance to the test functions
 @pytest.fixture
 def driver():
     driver = Selench()
     yield driver
     driver.quit()
 
 def test_ddg_search_query(driver):
-    # Define a search query
     keyword = 'github'
-    
-    # Navigate to duckduckgo
     driver.get('https://duckduckgo.com/')
-    
-    # Search duckduckgo for the keyword
-    driver.element('*[name="q"]').send_keys(keyword, Keys.ENTER)
-    
-    # Wait for the page title to contain the keyword
+    driver.element('[name=q]').send_keys(keyword, Keys.ENTER)
     driver.wait_for.title_to_contain(keyword)
-    
-    # Find all the result titles
-    titles = driver.elements('a[data-testid="result-title-a"] span')
+    titles = driver.elements('a[data-testid=result-title-a] span')
 
-    # Check that the keyword is present in each title
     for title in titles:
         assert keyword in title.text.lower()
 ```
-
```

### Comparing `selench-0.0.0/README.md` & `selench-19.4.2024/selench.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,71 @@
+Metadata-Version: 2.1
+Name: selench
+Version: 19.4.2024
+Summary: Selenium wrapper for Python
+Home-page: https://github.com/dsymbol/selench
+Author: dsymbol
+License: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: selenium==4.19.0
+
 # Selench
 
-Selench is a Python WebDriver wrapper that simplifies the use of the Selenium library. 
+Selench is a wrapper that simplifies the use of the Selenium library. 
 It provides a more concise syntax that makes the code more readable and easier to understand.
 
 ### Key Features
 
 - Elements have an explicit wait time by default
 - Element type detection ( CSS & XPATH )
 
 ## Installation
 
-The easiest way to install the latest version from PyPI is by using
-[pip](https://pip.pypa.io/):
+To install the library, use pip:
 
 ```bash
 pip install selench
 ```
 
-Alternatively, install directly from the GitHub repository:
+Alternatively, install the latest directly from the GitHub repository:
 ```bash
 pip install git+https://github.com/dsymbol/selench.git
 ```
 
-## Documentation
-
-The documentation can be found at https://dsymbol.github.io/selench/
-
 ## Examples
 
-Here are some examples of how to use Selench:
+Navigate to DuckDuckGo and search for 'Hello World!'
 
 ```py
 from selench import Selench, Keys
 
-# Create a new Selench instance
 driver = Selench()
-
-# Navigate to google
-driver.get('https://google.com')
-
-# Search google for 'Hello World!'
-driver.element('input[name="q"]').send_keys('Hello World!', Keys.ENTER)
-
-# Quit the driver
+driver.get('https://duckduckgo.com')
+driver.element('[name=q]').send_keys('Hello World!', Keys.ENTER)
 driver.quit()
 ```
 
-Using PyTest:
+Using PyTest: navigate to DuckDuckGo and search for 'github' assert titles contain 'github'
 
 ```py
 from selench import Selench, Keys
 import pytest
 
-# Create a fixture to provide the driver instance to the test functions
 @pytest.fixture
 def driver():
     driver = Selench()
     yield driver
     driver.quit()
 
 def test_ddg_search_query(driver):
-    # Define a search query
     keyword = 'github'
-    
-    # Navigate to duckduckgo
     driver.get('https://duckduckgo.com/')
-    
-    # Search duckduckgo for the keyword
-    driver.element('*[name="q"]').send_keys(keyword, Keys.ENTER)
-    
-    # Wait for the page title to contain the keyword
+    driver.element('[name=q]').send_keys(keyword, Keys.ENTER)
     driver.wait_for.title_to_contain(keyword)
-    
-    # Find all the result titles
-    titles = driver.elements('a[data-testid="result-title-a"] span')
+    titles = driver.elements('a[data-testid=result-title-a] span')
 
-    # Check that the keyword is present in each title
     for title in titles:
         assert keyword in title.text.lower()
-```
+```
```

### Comparing `selench-0.0.0/selench/driver.py` & `selench-19.4.2024/selench/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,58 +6,59 @@
     from selench import Selench, Keys
 
     driver = Selench()
     driver.get('https://google.com')
     driver.element('input[name="q"]').send_keys('Hello World!', Keys.ENTER)
     driver.quit()
 """
+import json
+from pathlib import Path
+from typing import Literal, List, Union
 
-import os
-import pickle
-from typing import List, Literal, Union
-
+from selenium import webdriver
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver import ActionChains
 from selenium.webdriver.common.alert import Alert
 from selenium.webdriver.common.by import By
+from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as ec
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.support.wait import WebDriverWait
 
-from .browser import Browser
 from .wait_for import WaitFor
 
 
 class Selench:
     """
     This is the main class that holds all the methods to interact with the browser.
 
     Args:
-        browser: The browser to use.
+        driver: WebDriver instance used to interact with the browser.
         wait: The default explicit wait time for WebDriverWait.
-        executable_path: The path to the driver executable.
-        headless: Run browser in headless mode.
-        user_agent: The user agent to use.
-        incognito: Run browser in incognito mode.
-        binary_location: The location of the browser executable.
     """
 
     def __init__(
             self,
-            browser: Literal["chrome", "firefox"] = "chrome",
+            driver: WebDriver | Literal["Chrome", "Firefox", "Edge"] = "Chrome",
             wait: int = 10,
-            executable_path: str = None,
-            headless: bool = False,
-            user_agent: str = None,
-            incognito: bool = False,
-            binary_location: str = None
-    ):
-        self._webdriver = Browser(browser, executable_path, headless, user_agent, incognito,
-                                  binary_location).create_driver()
+    ) -> None:
+        if isinstance(driver, WebDriver):
+            self._webdriver = driver
+        elif isinstance(driver, str):
+            if driver.lower() == "chrome":
+                self._webdriver = webdriver.Chrome()
+            elif driver.lower() == "firefox":
+                self._webdriver = webdriver.Firefox()
+            elif driver.lower() == "edge":
+                self._webdriver = webdriver.Edge()
+            else:
+                raise Exception("Unknown browser pass as WebDriver object")
+        else:
+            raise Exception("Unknown type passed to driver")
         self.wait = wait
         self._wait_for = WaitFor(self)
 
     @property
     def webdriver(self):
         """
         This property provides access to the underlying webdriver instance.
@@ -414,33 +415,26 @@
         """
         ActionChains(self.webdriver).scroll_by_amount(x, y).perform()
 
     def scroll_to_page_bottom(self):
         """
         Scroll the page to the bottom.
         """
-        self.driver.execute_js('window.scrollTo(0, document.body.scrollHeight)')
+        self.execute_js('window.scrollTo(0, document.body.scrollHeight)')
 
-    def drag_and_drop(self, draggable: WebElement, droppable: WebElement, alternative=False):
+    def drag_and_drop(self, draggable: WebElement, droppable: WebElement):
         """
         Perform a drag and drop action on the provided web elements.
 
         Args:
             draggable: The web element to be dragged.
             droppable: The web element to be dropped on.
-            alternative: Whether to use an alternative method for the drag and drop action. Default is False.
         """
-        if not alternative:
-            ActionChains(self.webdriver).click_and_hold(draggable).move_to_element(droppable).perform()
-            ActionChains(self.webdriver).release().perform()
-        else:
-            file_path = os.path.join(os.path.dirname(__file__), 'js', 'drag_and_drop.js')
-            with open(file_path, "r") as f:
-                javascript = f.read()
-            self.driver.execute_js(javascript, draggable, droppable)
+        ActionChains(self.webdriver).click_and_hold(draggable).move_to_element(droppable).perform()
+        ActionChains(self.webdriver).release().perform()
 
     def select_element(self, element_or_selector: Union[str, WebElement]) -> Select:
         """
         Convert a web element to a Select object. The Select object provides a convenient way to interact with
         select elements (drop-down lists) on a webpage. It allows the user to select one or more options from the list,
         and also provides methods to retrieve the selected options, as well as other useful information about the select element.
 
@@ -689,35 +683,37 @@
 
     def delete_all_cookies(self) -> None:
         """
         Delete all cookies for the current session.
         """
         self.webdriver.delete_all_cookies()
 
-    def session(self, path: str = "cookies.pkl", prompt=False) -> None:
+    def session(self, path: str = "cookies.json", prompt=False) -> None:
         """
         Save and load session cookies to and from a specified file path.
         If file path doesn't exist, it saves the current session cookies to the specified path.
         Otherwise, it loads the session cookies from the specified path.
 
         Args:
             path (str): The file path to save or load the session cookies from. Default is "cookies.pkl"
             prompt (bool): Prompts the user to press enter before saving session cookies. Default is False
         """
-        if os.path.exists(path):
-            with open(path, "rb") as f:
-                cookies = pickle.load(f)
+        path = Path(path).absolute()
+
+        if path.exists():
+            with path.open("r", encoding="utf-8") as f:
+                cookies = json.load(f)
             [self.add_cookie(cookie) for cookie in cookies]
             self.refresh()
         else:
             if prompt:
                 input("Press ENTER once ready to save the session")
             cookies = self.get_all_cookies()
-            with open(path, "wb") as f:
-                pickle.dump(cookies, f)
+            with path.open("w", encoding="utf-8") as f:
+                json.dump(cookies, f, indent=4)
 
     def screenshot(self, path: str = "screenshot.png") -> bool:
         """
         Saves a screenshot of the current window to a PNG image file.
 
         Args:
             path: The file path to save the screenshot. Default is "screenshot.png"
```

### Comparing `selench-0.0.0/selench/wait_for.py` & `selench-19.4.2024/selench/wait_for.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 class WaitFor:
     """
     This class provides methods for waiting for certain conditions to be met in a web page
     using Selenium's WebDriverWait and ExpectedConditions.
     """
+
     def __init__(self, driver):
         self._driver = driver
 
     def element_clickable(self, selector: str, timeout: int = None) -> WebElement:
         """
         An Expectation for checking an element is visible and enabled such that you can click it.
 
@@ -170,22 +171,47 @@
             True if text is present in the element.
 
         Raises:
             Exception: If the element does not contain text.
 
         Example::
 
-            driver.wait_for.element_text_to_be('//div[@id="msg"]', 'welcome')
+            driver.wait_for.element_text_to_include('//div[@id="msg"]', 'welcome')
         """
         if not timeout: timeout = self._driver.wait
         locator = self._driver._detect_locator_type(selector)
         element = WebDriverWait(self._driver.webdriver, timeout).until(ec.text_to_be_present_in_element(locator, text),
                                                                        f"Element text is not `{text}`")
         return element
 
+    def element_text_to_be(self, selector: str, text: str, timeout: int = None) -> bool:
+        """
+        An expectation for checking if the given text exactly matches the text within the specified element.
+
+        Args:
+            selector: The selector of the element.
+            text: The expected text to be present within the element.
+            timeout: Maximum time to wait in seconds. Default is None, which means use the default wait time.
+
+        Returns:
+            True if the text exactly matches the element's text.
+
+        Example::
+
+            driver.wait_for.element_text_to_be('#my-element', 'Hello')
+        """
+
+        if not timeout: timeout = self._driver.wait
+        locator = self._driver._detect_locator_type(selector)
+        element = WebDriverWait(self._driver.webdriver, timeout).until(
+            lambda d: bool(d.find_element(*locator).text == text),
+            message=f"Element text doesn't match {text}"
+        )
+        return element
+
     def element_attribute_text_to_include(self, selector: str, attribute: str, text: str, timeout: int = None) -> bool:
         """
         An expectation for checking if the given text is present in the element’s attribute.
 
         Args:
             selector: The selector of the element.
             attribute: The name of the attribute to check for the presence of the given text.
```

### Comparing `selench-0.0.0/setup.py` & `selench-19.4.2024/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selench',
-    version='0.0.0',
+    version='19.04.2024',
     packages=find_packages(),
     url='https://github.com/dsymbol/selench',
     license='OSI Approved :: MIT License',
     author='dsymbol',
-    description='Selenium WebDriver wrapper for Python',
+    description='Selenium wrapper for Python',
     include_package_data=True,
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     install_requires=[
-        'selenium'
+        'selenium==4.19.0'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ]
 )
```

