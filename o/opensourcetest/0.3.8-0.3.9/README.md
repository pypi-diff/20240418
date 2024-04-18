# Comparing `tmp/opensourcetest-0.3.8.tar.gz` & `tmp/opensourcetest-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourcetest-0.3.8.tar", max compression
+gzip compressed data, was "opensourcetest-0.3.9.tar", max compression
```

## Comparing `opensourcetest-0.3.8.tar` & `opensourcetest-0.3.9.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0    11357 2021-05-21 09:27:16.615552 opensourcetest-0.3.8/LICENSE
--rw-r--r--   0        0        0     3367 2021-09-30 03:55:01.188182 opensourcetest-0.3.8/README.md
--rw-r--r--   0        0        0     1038 2022-05-05 06:37:31.881314 opensourcetest-0.3.8/opensourcetest/__init__.py
--rw-r--r--   0        0        0      350 2021-05-21 09:27:16.620224 opensourcetest-0.3.8/opensourcetest/__main__.py
--rw-r--r--   0        0        0       75 2021-05-21 09:27:16.620309 opensourcetest-0.3.8/opensourcetest/appmodel/.gitignore
--rw-r--r--   0        0        0      728 2021-05-21 09:27:16.620439 opensourcetest-0.3.8/opensourcetest/appmodel/ActivityObject/Login_activity/Login_activity.yaml
--rw-r--r--   0        0        0       47 2021-05-21 09:27:16.620493 opensourcetest-0.3.8/opensourcetest/appmodel/ActivityObject/Login_activity/__init__.py
--rw-r--r--   0        0        0     1053 2021-05-21 09:27:16.620562 opensourcetest-0.3.8/opensourcetest/appmodel/ActivityObject/Login_activity/loginActivity.py
--rw-r--r--   0        0        0        0 2021-05-21 09:27:16.620590 opensourcetest-0.3.8/opensourcetest/appmodel/ActivityObject/__init__.py
--rw-r--r--   0        0        0      420 2021-05-21 09:27:16.620675 opensourcetest-0.3.8/opensourcetest/appmodel/ActivityObject/yamlChoice.py
--rw-r--r--   0        0        0       47 2021-05-21 09:27:16.620760 opensourcetest-0.3.8/opensourcetest/appmodel/Base/__init__.py
--rw-r--r--   0        0        0      165 2021-05-21 09:27:16.620823 opensourcetest-0.3.8/opensourcetest/appmodel/Base/assertMethod.py
--rw-r--r--   0        0        0     4896 2021-05-21 09:27:16.620932 opensourcetest-0.3.8/opensourcetest/appmodel/Base/base.py
--rw-r--r--   0        0        0       47 2021-05-21 09:27:16.621022 opensourcetest-0.3.8/opensourcetest/appmodel/Common/__init__.py
--rw-r--r--   0        0        0     1443 2021-05-21 09:27:16.621111 opensourcetest-0.3.8/opensourcetest/appmodel/Common/fileOperation.py
--rw-r--r--   0        0        0      418 2021-05-21 09:27:16.621178 opensourcetest-0.3.8/opensourcetest/appmodel/Common/fileOption.py
--rw-r--r--   0        0        0      880 2021-05-21 09:27:16.621271 opensourcetest-0.3.8/opensourcetest/appmodel/Common/publicMethod.py
--rw-r--r--   0        0        0       47 2021-05-21 09:27:16.621358 opensourcetest-0.3.8/opensourcetest/appmodel/Conf/__init__.py
--rw-r--r--   0        0        0      354 2021-05-21 09:27:16.621420 opensourcetest-0.3.8/opensourcetest/appmodel/Conf/config.yaml
--rw-r--r--   0        0        0        0 2021-05-21 09:27:16.621479 opensourcetest-0.3.8/opensourcetest/appmodel/Logs/__init__.py
--rw-r--r--   0        0        0     9242 2021-05-21 09:27:16.621577 opensourcetest-0.3.8/opensourcetest/appmodel/Logs/log.log
--rw-r--r--   0        0        0      156 2021-05-21 09:27:16.621706 opensourcetest-0.3.8/opensourcetest/appmodel/TestCases/Login/__init__.py
--rw-r--r--   0        0        0      271 2021-05-21 09:27:16.621779 opensourcetest-0.3.8/opensourcetest/appmodel/TestCases/Login/conftest.py
--rw-r--r--   0        0        0     1846 2021-05-21 09:27:16.621849 opensourcetest-0.3.8/opensourcetest/appmodel/TestCases/Login/test_loginActivityCase.py
--rw-r--r--   0        0        0       47 2021-05-21 09:27:16.623041 opensourcetest-0.3.8/opensourcetest/appmodel/TestCases/__init__.py
--rw-r--r--   0        0        0     1484 2021-05-21 09:27:16.623169 opensourcetest-0.3.8/opensourcetest/appmodel/conftest.py
--rw-r--r--   0        0        0      542 2021-05-21 09:27:16.623244 opensourcetest-0.3.8/opensourcetest/appmodel/pytest.ini
--rw-r--r--   0        0        0    12814 2021-05-21 09:27:16.623337 opensourcetest-0.3.8/opensourcetest/appmodel/readme.md
--rw-r--r--   0        0        0       21 2021-05-21 09:45:48.579908 opensourcetest-0.3.8/opensourcetest/appmodel/requirements.txt
--rw-r--r--   0        0        0      425 2021-05-21 09:27:16.623478 opensourcetest-0.3.8/opensourcetest/appmodel/run.py
--rw-r--r--   0        0        0      257 2021-05-21 09:27:16.623592 opensourcetest-0.3.8/opensourcetest/banner/banner_top.txt
--rw-r--r--   0        0        0      276 2021-05-21 09:27:16.623744 opensourcetest-0.3.8/opensourcetest/builtin/__init__.py
--rw-r--r--   0        0        0     3615 2021-05-21 09:27:16.623838 opensourcetest-0.3.8/opensourcetest/builtin/assertChecker.py
--rw-r--r--   0        0        0     5153 2021-05-21 09:27:16.623920 opensourcetest-0.3.8/opensourcetest/builtin/assertScreenShot.py
--rw-r--r--   0        0        0     6237 2021-05-21 09:27:16.624004 opensourcetest-0.3.8/opensourcetest/builtin/autoParamInjection.py
--rw-r--r--   0        0        0     1669 2021-05-21 09:27:16.624075 opensourcetest-0.3.8/opensourcetest/builtin/baseAppRunner.py
--rw-r--r--   0        0        0     4753 2021-05-21 09:27:16.624152 opensourcetest-0.3.8/opensourcetest/builtin/baseRequest.py
--rw-r--r--   0        0        0     2631 2021-05-21 09:27:16.624229 opensourcetest-0.3.8/opensourcetest/builtin/baseUiRunner.py
--rw-r--r--   0        0        0     3244 2021-05-21 09:27:16.624296 opensourcetest-0.3.8/opensourcetest/builtin/check.py
--rw-r--r--   0        0        0      824 2021-05-21 09:27:16.624357 opensourcetest-0.3.8/opensourcetest/builtin/exceptions.py
--rw-r--r--   0        0        0     5009 2021-05-21 09:27:16.624429 opensourcetest-0.3.8/opensourcetest/builtin/locate.py
--rw-r--r--   0        0        0     4769 2021-05-21 09:27:16.624507 opensourcetest-0.3.8/opensourcetest/builtin/models.py
--rw-r--r--   0        0        0     5304 2021-05-21 09:27:16.624611 opensourcetest-0.3.8/opensourcetest/builtin/ostDriver.py
--rw-r--r--   0        0        0     2818 2022-03-16 02:55:59.273565 opensourcetest-0.3.8/opensourcetest/builtin/ostHttp.py
--rw-r--r--   0        0        0     4915 2021-05-21 09:27:16.624773 opensourcetest-0.3.8/opensourcetest/cli.py
--rw-r--r--   0        0        0      276 2021-05-21 09:27:16.624896 opensourcetest-0.3.8/opensourcetest/common/__init__.py
--rw-r--r--   0        0        0      633 2021-05-21 09:27:16.624967 opensourcetest-0.3.8/opensourcetest/common/comFileOperation.py
--rw-r--r--   0        0        0      907 2021-05-21 09:27:16.625061 opensourcetest-0.3.8/opensourcetest/common/consolelog.py
--rw-r--r--   0        0        0     1437 2021-12-03 06:20:14.425057 opensourcetest-0.3.8/opensourcetest/common/dockerOperation.py
--rw-r--r--   0        0        0     1455 2021-05-21 09:27:16.625176 opensourcetest-0.3.8/opensourcetest/common/fileOperation.py
--rw-r--r--   0        0        0     1125 2021-05-21 09:27:16.625233 opensourcetest-0.3.8/opensourcetest/common/pictureOperation.py
--rw-r--r--   0        0        0     2980 2021-05-21 09:27:16.630978 opensourcetest-0.3.8/opensourcetest/common/urlOperation.py
--rw-r--r--   0        0        0      752 2021-05-21 09:27:16.631098 opensourcetest-0.3.8/opensourcetest/common/yamlOperation.py
--rw-r--r--   0        0        0       60 2021-05-21 09:27:16.632195 opensourcetest-0.3.8/opensourcetest/httpmodel/.gitignore
--rw-r--r--   0        0        0       46 2021-05-21 09:27:16.636658 opensourcetest-0.3.8/opensourcetest/httpmodel/Base/__init__.py
--rw-r--r--   0        0        0      153 2021-05-21 09:27:16.636743 opensourcetest-0.3.8/opensourcetest/httpmodel/Base/baseAssert.py
--rw-r--r--   0        0        0     1227 2021-05-21 09:27:16.636842 opensourcetest-0.3.8/opensourcetest/httpmodel/Base/requestEngine.py
--rw-r--r--   0        0        0       46 2021-05-21 09:27:16.637959 opensourcetest-0.3.8/opensourcetest/httpmodel/Common/FileOption/__init__.py
--rw-r--r--   0        0        0      519 2021-05-21 09:27:16.639023 opensourcetest-0.3.8/opensourcetest/httpmodel/Common/FileOption/yamlOption.py
--rw-r--r--   0        0        0      308 2021-05-21 09:27:16.639171 opensourcetest-0.3.8/opensourcetest/httpmodel/Common/StringOption/StringOperate.py
--rw-r--r--   0        0        0       47 2021-05-21 09:27:16.639235 opensourcetest-0.3.8/opensourcetest/httpmodel/Common/StringOption/__init__.py
--rw-r--r--   0        0        0      280 2021-05-21 09:27:16.639304 opensourcetest-0.3.8/opensourcetest/httpmodel/Common/__init__.py
--rw-r--r--   0        0        0      119 2021-05-21 09:27:16.640416 opensourcetest-0.3.8/opensourcetest/httpmodel/Conf/conf.yml
--rw-r--r--   0        0        0      644 2022-01-28 07:59:50.249527 opensourcetest-0.3.8/opensourcetest/httpmodel/Parameter/Login/Login.yaml
--rw-r--r--   0        0        0       46 2021-05-21 09:27:16.640658 opensourcetest-0.3.8/opensourcetest/httpmodel/Parameter/__init__.py
--rw-r--r--   0        0        0      267 2022-01-05 09:46:20.704976 opensourcetest-0.3.8/opensourcetest/httpmodel/Parameter/yamlChoice.py
--rw-r--r--   0        0        0     6754 2021-05-21 09:27:16.641403 opensourcetest-0.3.8/opensourcetest/httpmodel/README.md
--rw-r--r--   0        0        0     1033 2022-01-05 06:55:38.933354 opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/00564fc7-75d7-4165-acfc-3b51c7ce5717-result.json
--rw-r--r--   0        0        0      197 2022-01-05 06:55:38.932559 opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/4cfbf69f-e633-4cf9-b9a2-3d1e3c6395b9-container.json
--rw-r--r--   0        0        0     2542 2022-01-05 06:55:38.932943 opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/810ec528-f048-4d6c-91d3-476775b940e5-attachment.txt
--rw-r--r--   0        0        0     1784 2022-01-05 06:55:39.032945 opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/9e8be04f-b323-4585-9743-94ec9f9dc1ef-result.json
--rw-r--r--   0        0        0      197 2022-01-05 06:55:39.031800 opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/d07c14df-03df-4d39-94df-349806da41b0-container.json
--rw-r--r--   0        0        0     2187 2022-01-05 06:55:39.032399 opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/d1149fe0-2a4c-49ca-8d7c-7443629471a8-attachment.txt
--rw-r--r--   0        0        0      197 2022-01-05 06:55:38.932125 opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/e38c1fb2-152f-4fef-bc14-1700f4b9d45a-container.json
--rw-r--r--   0        0        0      197 2022-01-05 06:55:39.032020 opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/ed6c06a0-6f73-411c-a86d-c57dcea4f816-container.json
--rw-r--r--   0        0        0       46 2021-05-21 09:27:16.641655 opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/__init__.py
--rw-r--r--   0        0        0     1215 2022-01-28 07:59:50.245048 opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/test_login.py
--rw-r--r--   0        0        0      434 2021-05-21 09:27:16.641837 opensourcetest-0.3.8/opensourcetest/httpmodel/conftest.py
--rw-r--r--   0        0        0      293 2021-05-21 09:27:16.641898 opensourcetest-0.3.8/opensourcetest/httpmodel/pytest.ini
--rw-r--r--   0        0        0       21 2021-05-21 09:45:48.563968 opensourcetest-0.3.8/opensourcetest/httpmodel/requirements.txt
--rw-r--r--   0        0        0      503 2021-05-21 09:27:16.642011 opensourcetest-0.3.8/opensourcetest/httpmodel/run.py
--rw-r--r--   0        0        0      274 2021-05-21 09:27:16.642114 opensourcetest-0.3.8/opensourcetest/interface/__init__.py
--rw-r--r--   0        0        0     1081 2021-05-21 09:27:16.642240 opensourcetest-0.3.8/opensourcetest/interface/assertServer.py
--rw-r--r--   0        0        0     2320 2021-05-21 09:27:16.643272 opensourcetest-0.3.8/opensourcetest/scaffold.py
--rw-r--r--   0        0        0       75 2021-05-21 09:27:16.643395 opensourcetest-0.3.8/opensourcetest/uimodel/.gitignore
--rw-r--r--   0        0        0        0 2021-05-21 09:27:16.643464 opensourcetest-0.3.8/opensourcetest/uimodel/Base/__init__.py
--rw-r--r--   0        0        0      194 2021-05-21 09:27:16.643530 opensourcetest-0.3.8/opensourcetest/uimodel/Base/assertMethod.py
--rw-r--r--   0        0        0    13642 2021-05-21 09:27:16.643635 opensourcetest-0.3.8/opensourcetest/uimodel/Base/base.py
--rw-r--r--   0        0        0        0 2021-05-21 09:27:16.643699 opensourcetest-0.3.8/opensourcetest/uimodel/Common/__init__.py
--rw-r--r--   0        0        0     1443 2021-05-21 09:27:16.645910 opensourcetest-0.3.8/opensourcetest/uimodel/Common/fileOperation.py
--rw-r--r--   0        0        0      892 2021-05-21 09:27:16.645991 opensourcetest-0.3.8/opensourcetest/uimodel/Common/publicMethod.py
--rw-r--r--   0        0        0      550 2021-05-21 09:27:16.646074 opensourcetest-0.3.8/opensourcetest/uimodel/Common/stringOperation.py
--rw-r--r--   0        0        0      154 2021-05-21 09:27:16.646171 opensourcetest-0.3.8/opensourcetest/uimodel/Conf/__init__.py
--rw-r--r--   0        0        0      442 2021-05-21 09:27:16.646233 opensourcetest-0.3.8/opensourcetest/uimodel/Conf/config.yaml
--rw-r--r--   0        0        0       49 2021-05-21 09:27:16.646384 opensourcetest-0.3.8/opensourcetest/uimodel/LocalSeleniumServer/selenium_run_script/run_by_chrome.bat
--rw-r--r--   0        0        0       50 2021-05-21 09:27:16.646437 opensourcetest-0.3.8/opensourcetest/uimodel/LocalSeleniumServer/selenium_run_script/run_by_firefox.bat
--rw-r--r--   0        0        0       45 2021-05-21 09:27:16.646497 opensourcetest-0.3.8/opensourcetest/uimodel/LocalSeleniumServer/selenium_run_script/run_by_ie.bat
--rw-r--r--   0        0        0 10649576 2021-05-21 09:27:16.727760 opensourcetest-0.3.8/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_jar/selenium-server-standalone-3.141.0.jar
--rw-r--r--   0        0        0       82 2021-05-21 09:27:16.729590 opensourcetest-0.3.8/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_script/selenium_server_hub.bat
--rw-r--r--   0        0        0      134 2021-05-21 09:27:16.729681 opensourcetest-0.3.8/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_script/selenium_server_node1.bat
--rw-r--r--   0        0        0      134 2021-05-21 09:27:16.729732 opensourcetest-0.3.8/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_script/selenium_server_node2.bat
--rw-r--r--   0        0        0      134 2021-05-21 09:27:16.729779 opensourcetest-0.3.8/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_script/selenium_server_node3.bat
--rw-r--r--   0        0        0      292 2021-05-21 09:27:16.729842 opensourcetest-0.3.8/opensourcetest/uimodel/LocalSeleniumServer/start_server_windows.bat
--rw-r--r--   0        0        0        0 2021-05-21 09:27:16.729896 opensourcetest-0.3.8/opensourcetest/uimodel/Logs/__init__.py
--rw-r--r--   0        0        0     6128 2021-05-21 09:27:16.729990 opensourcetest-0.3.8/opensourcetest/uimodel/Logs/log.log
--rw-r--r--   0        0        0     1076 2021-05-21 09:27:16.730118 opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/Login_page/Login_page.yaml
--rw-r--r--   0        0        0       46 2021-05-21 09:27:16.730167 opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/Login_page/__init__.py
--rw-r--r--   0        0        0     1722 2021-05-21 09:27:16.730243 opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/Register_page/Register_page.yaml
--rw-r--r--   0        0        0       46 2021-05-21 09:27:16.730298 opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/Register_page/__init__.py
--rw-r--r--   0        0        0        0 2021-05-21 09:27:16.730328 opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/__init__.py
--rw-r--r--   0        0        0     3640 2021-05-21 09:27:16.730403 opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/loginPage.py
--rw-r--r--   0        0        0     4484 2021-05-21 09:27:16.730472 opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/registerPage.py
--rw-r--r--   0        0        0      653 2021-05-21 09:27:16.730527 opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/yamlChoice.py
--rw-r--r--   0        0        0       47 2021-05-21 09:27:16.730657 opensourcetest-0.3.8/opensourcetest/uimodel/TestCases/Login/__init__.py
--rw-r--r--   0        0        0      991 2021-05-21 09:27:16.730754 opensourcetest-0.3.8/opensourcetest/uimodel/TestCases/Login/test_loginPageCase.py
--rw-r--r--   0        0        0       46 2021-05-21 09:27:16.730855 opensourcetest-0.3.8/opensourcetest/uimodel/TestCases/Register/__init__.py
--rw-r--r--   0        0        0      936 2021-05-21 09:27:16.730925 opensourcetest-0.3.8/opensourcetest/uimodel/TestCases/Register/test_registerPageCase.py
--rw-r--r--   0        0        0       47 2021-05-21 09:27:16.730978 opensourcetest-0.3.8/opensourcetest/uimodel/TestCases/__init__.py
--rw-r--r--   0        0        0      734 2021-05-21 09:27:16.731035 opensourcetest-0.3.8/opensourcetest/uimodel/TestCases/conftest.py
--rw-r--r--   0        0        0      682 2021-05-21 09:27:16.731100 opensourcetest-0.3.8/opensourcetest/uimodel/conftest.py
--rw-r--r--   0        0        0      543 2021-05-21 09:27:16.732211 opensourcetest-0.3.8/opensourcetest/uimodel/pytest.ini
--rw-r--r--   0        0        0    15135 2021-05-21 09:27:16.732271 opensourcetest-0.3.8/opensourcetest/uimodel/readme.md
--rw-r--r--   0        0        0       22 2021-05-21 09:45:48.572750 opensourcetest-0.3.8/opensourcetest/uimodel/requirements.txt
--rw-r--r--   0        0        0      425 2021-05-21 09:27:16.732364 opensourcetest-0.3.8/opensourcetest/uimodel/run.py
--rw-r--r--   0        0        0      348 2021-05-21 09:27:16.732406 opensourcetest-0.3.8/opensourcetest/uimodel/start_run_all_browser.bat
--rw-r--r--   0        0        0     1750 2022-05-05 06:37:31.877756 opensourcetest-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     6358 2022-05-05 06:39:58.650047 opensourcetest-0.3.8/setup.py
--rw-r--r--   0        0        0     5136 2022-05-05 06:39:58.650361 opensourcetest-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-05-21 09:27:16.615552 opensourcetest-0.3.9/LICENSE
+-rw-r--r--   0        0        0     3367 2021-09-30 03:55:01.188182 opensourcetest-0.3.9/README.md
+-rw-r--r--   0        0        0     1038 2022-10-18 10:17:09.341914 opensourcetest-0.3.9/opensourcetest/__init__.py
+-rw-r--r--   0        0        0      350 2021-05-21 09:27:16.620224 opensourcetest-0.3.9/opensourcetest/__main__.py
+-rw-r--r--   0        0        0       75 2021-05-21 09:27:16.620309 opensourcetest-0.3.9/opensourcetest/appmodel/.gitignore
+-rw-r--r--   0        0        0      728 2021-05-21 09:27:16.620439 opensourcetest-0.3.9/opensourcetest/appmodel/ActivityObject/Login_activity/Login_activity.yaml
+-rw-r--r--   0        0        0       47 2021-05-21 09:27:16.620493 opensourcetest-0.3.9/opensourcetest/appmodel/ActivityObject/Login_activity/__init__.py
+-rw-r--r--   0        0        0     1053 2021-05-21 09:27:16.620562 opensourcetest-0.3.9/opensourcetest/appmodel/ActivityObject/Login_activity/loginActivity.py
+-rw-r--r--   0        0        0        0 2021-05-21 09:27:16.620590 opensourcetest-0.3.9/opensourcetest/appmodel/ActivityObject/__init__.py
+-rw-r--r--   0        0        0      420 2021-05-21 09:27:16.620675 opensourcetest-0.3.9/opensourcetest/appmodel/ActivityObject/yamlChoice.py
+-rw-r--r--   0        0        0       47 2021-05-21 09:27:16.620760 opensourcetest-0.3.9/opensourcetest/appmodel/Base/__init__.py
+-rw-r--r--   0        0        0      165 2021-05-21 09:27:16.620823 opensourcetest-0.3.9/opensourcetest/appmodel/Base/assertMethod.py
+-rw-r--r--   0        0        0     4896 2021-05-21 09:27:16.620932 opensourcetest-0.3.9/opensourcetest/appmodel/Base/base.py
+-rw-r--r--   0        0        0       47 2021-05-21 09:27:16.621022 opensourcetest-0.3.9/opensourcetest/appmodel/Common/__init__.py
+-rw-r--r--   0        0        0     1443 2021-05-21 09:27:16.621111 opensourcetest-0.3.9/opensourcetest/appmodel/Common/fileOperation.py
+-rw-r--r--   0        0        0      418 2021-05-21 09:27:16.621178 opensourcetest-0.3.9/opensourcetest/appmodel/Common/fileOption.py
+-rw-r--r--   0        0        0      880 2021-05-21 09:27:16.621271 opensourcetest-0.3.9/opensourcetest/appmodel/Common/publicMethod.py
+-rw-r--r--   0        0        0       47 2021-05-21 09:27:16.621358 opensourcetest-0.3.9/opensourcetest/appmodel/Conf/__init__.py
+-rw-r--r--   0        0        0      354 2021-05-21 09:27:16.621420 opensourcetest-0.3.9/opensourcetest/appmodel/Conf/config.yaml
+-rw-r--r--   0        0        0        0 2021-05-21 09:27:16.621479 opensourcetest-0.3.9/opensourcetest/appmodel/Logs/__init__.py
+-rw-r--r--   0        0        0     9242 2021-05-21 09:27:16.621577 opensourcetest-0.3.9/opensourcetest/appmodel/Logs/log.log
+-rw-r--r--   0        0        0      156 2021-05-21 09:27:16.621706 opensourcetest-0.3.9/opensourcetest/appmodel/TestCases/Login/__init__.py
+-rw-r--r--   0        0        0      271 2021-05-21 09:27:16.621779 opensourcetest-0.3.9/opensourcetest/appmodel/TestCases/Login/conftest.py
+-rw-r--r--   0        0        0     1846 2021-05-21 09:27:16.621849 opensourcetest-0.3.9/opensourcetest/appmodel/TestCases/Login/test_loginActivityCase.py
+-rw-r--r--   0        0        0       47 2021-05-21 09:27:16.623041 opensourcetest-0.3.9/opensourcetest/appmodel/TestCases/__init__.py
+-rw-r--r--   0        0        0     1484 2021-05-21 09:27:16.623169 opensourcetest-0.3.9/opensourcetest/appmodel/conftest.py
+-rw-r--r--   0        0        0      542 2021-05-21 09:27:16.623244 opensourcetest-0.3.9/opensourcetest/appmodel/pytest.ini
+-rw-r--r--   0        0        0    12814 2021-05-21 09:27:16.623337 opensourcetest-0.3.9/opensourcetest/appmodel/readme.md
+-rw-r--r--   0        0        0       21 2021-05-21 09:45:48.579908 opensourcetest-0.3.9/opensourcetest/appmodel/requirements.txt
+-rw-r--r--   0        0        0      425 2021-05-21 09:27:16.623478 opensourcetest-0.3.9/opensourcetest/appmodel/run.py
+-rw-r--r--   0        0        0      257 2021-05-21 09:27:16.623592 opensourcetest-0.3.9/opensourcetest/banner/banner_top.txt
+-rw-r--r--   0        0        0      276 2021-05-21 09:27:16.623744 opensourcetest-0.3.9/opensourcetest/builtin/__init__.py
+-rw-r--r--   0        0        0     3615 2021-05-21 09:27:16.623838 opensourcetest-0.3.9/opensourcetest/builtin/assertChecker.py
+-rw-r--r--   0        0        0     5153 2021-05-21 09:27:16.623920 opensourcetest-0.3.9/opensourcetest/builtin/assertScreenShot.py
+-rw-r--r--   0        0        0     6237 2021-05-21 09:27:16.624004 opensourcetest-0.3.9/opensourcetest/builtin/autoParamInjection.py
+-rw-r--r--   0        0        0     1669 2021-05-21 09:27:16.624075 opensourcetest-0.3.9/opensourcetest/builtin/baseAppRunner.py
+-rw-r--r--   0        0        0     4939 2022-10-18 10:10:37.801645 opensourcetest-0.3.9/opensourcetest/builtin/baseRequest.py
+-rw-r--r--   0        0        0     2631 2021-05-21 09:27:16.624229 opensourcetest-0.3.9/opensourcetest/builtin/baseUiRunner.py
+-rw-r--r--   0        0        0     3244 2021-05-21 09:27:16.624296 opensourcetest-0.3.9/opensourcetest/builtin/check.py
+-rw-r--r--   0        0        0      824 2021-05-21 09:27:16.624357 opensourcetest-0.3.9/opensourcetest/builtin/exceptions.py
+-rw-r--r--   0        0        0     5009 2021-05-21 09:27:16.624429 opensourcetest-0.3.9/opensourcetest/builtin/locate.py
+-rw-r--r--   0        0        0     4769 2021-05-21 09:27:16.624507 opensourcetest-0.3.9/opensourcetest/builtin/models.py
+-rw-r--r--   0        0        0     5304 2021-05-21 09:27:16.624611 opensourcetest-0.3.9/opensourcetest/builtin/ostDriver.py
+-rw-r--r--   0        0        0     2818 2022-03-16 02:55:59.273565 opensourcetest-0.3.9/opensourcetest/builtin/ostHttp.py
+-rw-r--r--   0        0        0     4915 2021-05-21 09:27:16.624773 opensourcetest-0.3.9/opensourcetest/cli.py
+-rw-r--r--   0        0        0      276 2021-05-21 09:27:16.624896 opensourcetest-0.3.9/opensourcetest/common/__init__.py
+-rw-r--r--   0        0        0      633 2021-05-21 09:27:16.624967 opensourcetest-0.3.9/opensourcetest/common/comFileOperation.py
+-rw-r--r--   0        0        0      907 2021-05-21 09:27:16.625061 opensourcetest-0.3.9/opensourcetest/common/consolelog.py
+-rw-r--r--   0        0        0     1437 2021-12-03 06:20:14.425057 opensourcetest-0.3.9/opensourcetest/common/dockerOperation.py
+-rw-r--r--   0        0        0     1455 2021-05-21 09:27:16.625176 opensourcetest-0.3.9/opensourcetest/common/fileOperation.py
+-rw-r--r--   0        0        0     1125 2021-05-21 09:27:16.625233 opensourcetest-0.3.9/opensourcetest/common/pictureOperation.py
+-rw-r--r--   0        0        0     2980 2021-05-21 09:27:16.630978 opensourcetest-0.3.9/opensourcetest/common/urlOperation.py
+-rw-r--r--   0        0        0      752 2021-05-21 09:27:16.631098 opensourcetest-0.3.9/opensourcetest/common/yamlOperation.py
+-rw-r--r--   0        0        0       60 2021-05-21 09:27:16.632195 opensourcetest-0.3.9/opensourcetest/httpmodel/.gitignore
+-rw-r--r--   0        0        0       46 2021-05-21 09:27:16.636658 opensourcetest-0.3.9/opensourcetest/httpmodel/Base/__init__.py
+-rw-r--r--   0        0        0      153 2021-05-21 09:27:16.636743 opensourcetest-0.3.9/opensourcetest/httpmodel/Base/baseAssert.py
+-rw-r--r--   0        0        0     1227 2021-05-21 09:27:16.636842 opensourcetest-0.3.9/opensourcetest/httpmodel/Base/requestEngine.py
+-rw-r--r--   0        0        0       46 2021-05-21 09:27:16.637959 opensourcetest-0.3.9/opensourcetest/httpmodel/Common/FileOption/__init__.py
+-rw-r--r--   0        0        0      519 2021-05-21 09:27:16.639023 opensourcetest-0.3.9/opensourcetest/httpmodel/Common/FileOption/yamlOption.py
+-rw-r--r--   0        0        0      308 2021-05-21 09:27:16.639171 opensourcetest-0.3.9/opensourcetest/httpmodel/Common/StringOption/StringOperate.py
+-rw-r--r--   0        0        0       47 2021-05-21 09:27:16.639235 opensourcetest-0.3.9/opensourcetest/httpmodel/Common/StringOption/__init__.py
+-rw-r--r--   0        0        0      280 2021-05-21 09:27:16.639304 opensourcetest-0.3.9/opensourcetest/httpmodel/Common/__init__.py
+-rw-r--r--   0        0        0      119 2021-05-21 09:27:16.640416 opensourcetest-0.3.9/opensourcetest/httpmodel/Conf/conf.yml
+-rw-r--r--   0        0        0      644 2022-01-28 07:59:50.249527 opensourcetest-0.3.9/opensourcetest/httpmodel/Parameter/Login/Login.yaml
+-rw-r--r--   0        0        0       46 2021-05-21 09:27:16.640658 opensourcetest-0.3.9/opensourcetest/httpmodel/Parameter/__init__.py
+-rw-r--r--   0        0        0      267 2022-01-05 09:46:20.704976 opensourcetest-0.3.9/opensourcetest/httpmodel/Parameter/yamlChoice.py
+-rw-r--r--   0        0        0     6754 2021-05-21 09:27:16.641403 opensourcetest-0.3.9/opensourcetest/httpmodel/README.md
+-rw-r--r--   0        0        0     1033 2022-01-05 06:55:38.933354 opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/00564fc7-75d7-4165-acfc-3b51c7ce5717-result.json
+-rw-r--r--   0        0        0      197 2022-01-05 06:55:38.932559 opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/4cfbf69f-e633-4cf9-b9a2-3d1e3c6395b9-container.json
+-rw-r--r--   0        0        0     2542 2022-01-05 06:55:38.932943 opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/810ec528-f048-4d6c-91d3-476775b940e5-attachment.txt
+-rw-r--r--   0        0        0     1784 2022-01-05 06:55:39.032945 opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/9e8be04f-b323-4585-9743-94ec9f9dc1ef-result.json
+-rw-r--r--   0        0        0      197 2022-01-05 06:55:39.031800 opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/d07c14df-03df-4d39-94df-349806da41b0-container.json
+-rw-r--r--   0        0        0     2187 2022-01-05 06:55:39.032399 opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/d1149fe0-2a4c-49ca-8d7c-7443629471a8-attachment.txt
+-rw-r--r--   0        0        0      197 2022-01-05 06:55:38.932125 opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/e38c1fb2-152f-4fef-bc14-1700f4b9d45a-container.json
+-rw-r--r--   0        0        0      197 2022-01-05 06:55:39.032020 opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/ed6c06a0-6f73-411c-a86d-c57dcea4f816-container.json
+-rw-r--r--   0        0        0       46 2021-05-21 09:27:16.641655 opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/__init__.py
+-rw-r--r--   0        0        0     1215 2022-01-28 07:59:50.245048 opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/test_login.py
+-rw-r--r--   0        0        0      434 2021-05-21 09:27:16.641837 opensourcetest-0.3.9/opensourcetest/httpmodel/conftest.py
+-rw-r--r--   0        0        0      293 2021-05-21 09:27:16.641898 opensourcetest-0.3.9/opensourcetest/httpmodel/pytest.ini
+-rw-r--r--   0        0        0       21 2021-05-21 09:45:48.563968 opensourcetest-0.3.9/opensourcetest/httpmodel/requirements.txt
+-rw-r--r--   0        0        0      503 2021-05-21 09:27:16.642011 opensourcetest-0.3.9/opensourcetest/httpmodel/run.py
+-rw-r--r--   0        0        0      274 2021-05-21 09:27:16.642114 opensourcetest-0.3.9/opensourcetest/interface/__init__.py
+-rw-r--r--   0        0        0     1081 2021-05-21 09:27:16.642240 opensourcetest-0.3.9/opensourcetest/interface/assertServer.py
+-rw-r--r--   0        0        0     2320 2021-05-21 09:27:16.643272 opensourcetest-0.3.9/opensourcetest/scaffold.py
+-rw-r--r--   0        0        0       75 2021-05-21 09:27:16.643395 opensourcetest-0.3.9/opensourcetest/uimodel/.gitignore
+-rw-r--r--   0        0        0        0 2021-05-21 09:27:16.643464 opensourcetest-0.3.9/opensourcetest/uimodel/Base/__init__.py
+-rw-r--r--   0        0        0      194 2021-05-21 09:27:16.643530 opensourcetest-0.3.9/opensourcetest/uimodel/Base/assertMethod.py
+-rw-r--r--   0        0        0    13642 2021-05-21 09:27:16.643635 opensourcetest-0.3.9/opensourcetest/uimodel/Base/base.py
+-rw-r--r--   0        0        0        0 2021-05-21 09:27:16.643699 opensourcetest-0.3.9/opensourcetest/uimodel/Common/__init__.py
+-rw-r--r--   0        0        0     1443 2021-05-21 09:27:16.645910 opensourcetest-0.3.9/opensourcetest/uimodel/Common/fileOperation.py
+-rw-r--r--   0        0        0      892 2021-05-21 09:27:16.645991 opensourcetest-0.3.9/opensourcetest/uimodel/Common/publicMethod.py
+-rw-r--r--   0        0        0      550 2021-05-21 09:27:16.646074 opensourcetest-0.3.9/opensourcetest/uimodel/Common/stringOperation.py
+-rw-r--r--   0        0        0      154 2021-05-21 09:27:16.646171 opensourcetest-0.3.9/opensourcetest/uimodel/Conf/__init__.py
+-rw-r--r--   0        0        0      442 2021-05-21 09:27:16.646233 opensourcetest-0.3.9/opensourcetest/uimodel/Conf/config.yaml
+-rw-r--r--   0        0        0       49 2021-05-21 09:27:16.646384 opensourcetest-0.3.9/opensourcetest/uimodel/LocalSeleniumServer/selenium_run_script/run_by_chrome.bat
+-rw-r--r--   0        0        0       50 2021-05-21 09:27:16.646437 opensourcetest-0.3.9/opensourcetest/uimodel/LocalSeleniumServer/selenium_run_script/run_by_firefox.bat
+-rw-r--r--   0        0        0       45 2021-05-21 09:27:16.646497 opensourcetest-0.3.9/opensourcetest/uimodel/LocalSeleniumServer/selenium_run_script/run_by_ie.bat
+-rw-r--r--   0        0        0 10649576 2021-05-21 09:27:16.727760 opensourcetest-0.3.9/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_jar/selenium-server-standalone-3.141.0.jar
+-rw-r--r--   0        0        0       82 2021-05-21 09:27:16.729590 opensourcetest-0.3.9/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_script/selenium_server_hub.bat
+-rw-r--r--   0        0        0      134 2021-05-21 09:27:16.729681 opensourcetest-0.3.9/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_script/selenium_server_node1.bat
+-rw-r--r--   0        0        0      134 2021-05-21 09:27:16.729732 opensourcetest-0.3.9/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_script/selenium_server_node2.bat
+-rw-r--r--   0        0        0      134 2021-05-21 09:27:16.729779 opensourcetest-0.3.9/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_script/selenium_server_node3.bat
+-rw-r--r--   0        0        0      292 2021-05-21 09:27:16.729842 opensourcetest-0.3.9/opensourcetest/uimodel/LocalSeleniumServer/start_server_windows.bat
+-rw-r--r--   0        0        0        0 2021-05-21 09:27:16.729896 opensourcetest-0.3.9/opensourcetest/uimodel/Logs/__init__.py
+-rw-r--r--   0        0        0     6128 2021-05-21 09:27:16.729990 opensourcetest-0.3.9/opensourcetest/uimodel/Logs/log.log
+-rw-r--r--   0        0        0     1076 2021-05-21 09:27:16.730118 opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/Login_page/Login_page.yaml
+-rw-r--r--   0        0        0       46 2021-05-21 09:27:16.730167 opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/Login_page/__init__.py
+-rw-r--r--   0        0        0     1722 2021-05-21 09:27:16.730243 opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/Register_page/Register_page.yaml
+-rw-r--r--   0        0        0       46 2021-05-21 09:27:16.730298 opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/Register_page/__init__.py
+-rw-r--r--   0        0        0        0 2021-05-21 09:27:16.730328 opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/__init__.py
+-rw-r--r--   0        0        0     3640 2021-05-21 09:27:16.730403 opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/loginPage.py
+-rw-r--r--   0        0        0     4484 2021-05-21 09:27:16.730472 opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/registerPage.py
+-rw-r--r--   0        0        0      653 2021-05-21 09:27:16.730527 opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/yamlChoice.py
+-rw-r--r--   0        0        0       47 2021-05-21 09:27:16.730657 opensourcetest-0.3.9/opensourcetest/uimodel/TestCases/Login/__init__.py
+-rw-r--r--   0        0        0      991 2021-05-21 09:27:16.730754 opensourcetest-0.3.9/opensourcetest/uimodel/TestCases/Login/test_loginPageCase.py
+-rw-r--r--   0        0        0       46 2021-05-21 09:27:16.730855 opensourcetest-0.3.9/opensourcetest/uimodel/TestCases/Register/__init__.py
+-rw-r--r--   0        0        0      936 2021-05-21 09:27:16.730925 opensourcetest-0.3.9/opensourcetest/uimodel/TestCases/Register/test_registerPageCase.py
+-rw-r--r--   0        0        0       47 2021-05-21 09:27:16.730978 opensourcetest-0.3.9/opensourcetest/uimodel/TestCases/__init__.py
+-rw-r--r--   0        0        0      734 2021-05-21 09:27:16.731035 opensourcetest-0.3.9/opensourcetest/uimodel/TestCases/conftest.py
+-rw-r--r--   0        0        0      682 2021-05-21 09:27:16.731100 opensourcetest-0.3.9/opensourcetest/uimodel/conftest.py
+-rw-r--r--   0        0        0      543 2021-05-21 09:27:16.732211 opensourcetest-0.3.9/opensourcetest/uimodel/pytest.ini
+-rw-r--r--   0        0        0    15135 2021-05-21 09:27:16.732271 opensourcetest-0.3.9/opensourcetest/uimodel/readme.md
+-rw-r--r--   0        0        0       22 2021-05-21 09:45:48.572750 opensourcetest-0.3.9/opensourcetest/uimodel/requirements.txt
+-rw-r--r--   0        0        0      425 2021-05-21 09:27:16.732364 opensourcetest-0.3.9/opensourcetest/uimodel/run.py
+-rw-r--r--   0        0        0      348 2021-05-21 09:27:16.732406 opensourcetest-0.3.9/opensourcetest/uimodel/start_run_all_browser.bat
+-rw-r--r--   0        0        0     1750 2022-10-18 10:16:41.550402 opensourcetest-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6358 2022-10-18 10:17:14.142670 opensourcetest-0.3.9/setup.py
+-rw-r--r--   0        0        0     5136 2022-10-18 10:17:14.142981 opensourcetest-0.3.9/PKG-INFO
```

### Comparing `opensourcetest-0.3.8/LICENSE` & `opensourcetest-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/README.md` & `opensourcetest-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/__init__.py` & `opensourcetest-0.3.9/opensourcetest/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 __description__ = "We need more free software interface testing."
 
 from opensourcetest.builtin.ostHttp import ost_http_runner
 from opensourcetest.builtin.baseRequest import BaseRequest
 from opensourcetest.builtin.baseUiRunner import ost_ui_runner, ost_ui_cmd_runner
 from opensourcetest.builtin.baseAppRunner import ost_app_runner, ost_app_cmd_runner
 from opensourcetest.builtin.assertChecker import AssertChecker
```

### Comparing `opensourcetest-0.3.8/opensourcetest/appmodel/ActivityObject/Login_activity/Login_activity.yaml` & `opensourcetest-0.3.9/opensourcetest/appmodel/ActivityObject/Login_activity/Login_activity.yaml`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/appmodel/ActivityObject/Login_activity/loginActivity.py` & `opensourcetest-0.3.9/opensourcetest/appmodel/ActivityObject/Login_activity/loginActivity.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/appmodel/Base/base.py` & `opensourcetest-0.3.9/opensourcetest/appmodel/Base/base.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/appmodel/Common/fileOperation.py` & `opensourcetest-0.3.9/opensourcetest/appmodel/Common/fileOperation.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/appmodel/Common/publicMethod.py` & `opensourcetest-0.3.9/opensourcetest/appmodel/Common/publicMethod.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/appmodel/Logs/log.log` & `opensourcetest-0.3.9/opensourcetest/appmodel/Logs/log.log`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/appmodel/TestCases/Login/test_loginActivityCase.py` & `opensourcetest-0.3.9/opensourcetest/appmodel/TestCases/Login/test_loginActivityCase.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/appmodel/conftest.py` & `opensourcetest-0.3.9/opensourcetest/appmodel/conftest.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/appmodel/pytest.ini` & `opensourcetest-0.3.9/opensourcetest/appmodel/pytest.ini`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/appmodel/readme.md` & `opensourcetest-0.3.9/opensourcetest/appmodel/readme.md`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/assertChecker.py` & `opensourcetest-0.3.9/opensourcetest/builtin/assertChecker.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/assertScreenShot.py` & `opensourcetest-0.3.9/opensourcetest/builtin/assertScreenShot.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/autoParamInjection.py` & `opensourcetest-0.3.9/opensourcetest/builtin/autoParamInjection.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/baseAppRunner.py` & `opensourcetest-0.3.9/opensourcetest/builtin/baseAppRunner.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/baseRequest.py` & `opensourcetest-0.3.9/opensourcetest/builtin/baseRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 @Auth    : chineseluo
 @Email   : 848257135@qq.com
 @File    : baseRequest.py
 @IDE     : PyCharm
 ------------------------------------
 """
 import os
+import json
 import jmespath
 import requests
 import logging
 import urllib3
 from opensourcetest.common.consolelog import log_output
 from opensourcetest.builtin.models import OSTRespData, OSTReqData, OSTReqRespData, MethodEnum
 from opensourcetest.common.yamlOperation import YamlFileOption
@@ -79,28 +80,30 @@
             result = self.__post(url=url, params=send_params, data=send_data, json=send_json, **kwargs)
         elif method == MethodEnum.DELETE:
             result = self.__delete(url=url, params=send_params, data=send_data, json=send_json, **kwargs)
         elif method == MethodEnum.PUT:
             result = self.__put(url=url, params=send_params, data=send_data, json=send_json, **kwargs)
         else:
             logging.error(f"Please pass the correct request method parameters! The current error parameter is:{method}")
-
+        result.encoding = "utf-8"
+        body = json.loads(result.request.body) if isinstance(result.request.body, bytes) else result.request.body
         ost_req = OSTReqData(
             method=result.request.method,
             url=result.request.url,
             headers=result.request.headers,
             cookies=result.request._cookies,
-            body=result.request.body
+            body=body
         )
         log_output(ost_req, "request")
         if result.headers["Content-Type"].find("json") != -1:
             try:
                 ost_rep_body = result.json()
             except Exception as e:
                 logging.warning("Failed to parse data with JSON, switch to text parsing！")
+                result.encoding = "utf-8"
                 ost_rep_body = result.text
         elif result.headers["Content-Type"].find("xml") != -1 \
                 or result.headers["Content-Type"].find("html") != -1 \
                 or result.headers["Content-Type"].find("text") != -1:
             result.encoding = "gb2312"
             ost_rep_body = result.text
         else:
```

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/baseUiRunner.py` & `opensourcetest-0.3.9/opensourcetest/builtin/baseUiRunner.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/check.py` & `opensourcetest-0.3.9/opensourcetest/builtin/check.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/exceptions.py` & `opensourcetest-0.3.9/opensourcetest/builtin/exceptions.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/locate.py` & `opensourcetest-0.3.9/opensourcetest/builtin/locate.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/models.py` & `opensourcetest-0.3.9/opensourcetest/builtin/models.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/ostDriver.py` & `opensourcetest-0.3.9/opensourcetest/builtin/ostDriver.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/builtin/ostHttp.py` & `opensourcetest-0.3.9/opensourcetest/builtin/ostHttp.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/cli.py` & `opensourcetest-0.3.9/opensourcetest/cli.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/common/comFileOperation.py` & `opensourcetest-0.3.9/opensourcetest/common/comFileOperation.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/common/consolelog.py` & `opensourcetest-0.3.9/opensourcetest/common/consolelog.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/common/dockerOperation.py` & `opensourcetest-0.3.9/opensourcetest/common/dockerOperation.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/common/fileOperation.py` & `opensourcetest-0.3.9/opensourcetest/common/fileOperation.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/common/pictureOperation.py` & `opensourcetest-0.3.9/opensourcetest/common/pictureOperation.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/common/urlOperation.py` & `opensourcetest-0.3.9/opensourcetest/common/urlOperation.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/common/yamlOperation.py` & `opensourcetest-0.3.9/opensourcetest/common/yamlOperation.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/httpmodel/Base/requestEngine.py` & `opensourcetest-0.3.9/opensourcetest/httpmodel/Base/requestEngine.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/httpmodel/Common/FileOption/yamlOption.py` & `opensourcetest-0.3.9/opensourcetest/httpmodel/Common/FileOption/yamlOption.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/httpmodel/Parameter/Login/Login.yaml` & `opensourcetest-0.3.9/opensourcetest/httpmodel/Parameter/Login/Login.yaml`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/httpmodel/README.md` & `opensourcetest-0.3.9/opensourcetest/httpmodel/README.md`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/00564fc7-75d7-4165-acfc-3b51c7ce5717-result.json` & `opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/00564fc7-75d7-4165-acfc-3b51c7ce5717-result.json`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/810ec528-f048-4d6c-91d3-476775b940e5-attachment.txt` & `opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/810ec528-f048-4d6c-91d3-476775b940e5-attachment.txt`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/9e8be04f-b323-4585-9743-94ec9f9dc1ef-result.json` & `opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/9e8be04f-b323-4585-9743-94ec9f9dc1ef-result.json`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/Report/allure-results/d1149fe0-2a4c-49ca-8d7c-7443629471a8-attachment.txt` & `opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/Report/allure-results/d1149fe0-2a4c-49ca-8d7c-7443629471a8-attachment.txt`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/httpmodel/TestCases/test_login.py` & `opensourcetest-0.3.9/opensourcetest/httpmodel/TestCases/test_login.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/interface/assertServer.py` & `opensourcetest-0.3.9/opensourcetest/interface/assertServer.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/scaffold.py` & `opensourcetest-0.3.9/opensourcetest/scaffold.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/Base/base.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/Base/base.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/Common/fileOperation.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/Common/fileOperation.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/Common/publicMethod.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/Common/publicMethod.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/Common/stringOperation.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/Common/stringOperation.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_jar/selenium-server-standalone-3.141.0.jar` & `opensourcetest-0.3.9/opensourcetest/uimodel/LocalSeleniumServer/selenium_server_jar/selenium-server-standalone-3.141.0.jar`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/Logs/log.log` & `opensourcetest-0.3.9/opensourcetest/uimodel/Logs/log.log`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/Login_page/Login_page.yaml` & `opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/Login_page/Login_page.yaml`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/Register_page/Register_page.yaml` & `opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/Register_page/Register_page.yaml`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/loginPage.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/loginPage.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/registerPage.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/registerPage.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/PageObject/yamlChoice.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/PageObject/yamlChoice.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/TestCases/Login/test_loginPageCase.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/TestCases/Login/test_loginPageCase.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/TestCases/Register/test_registerPageCase.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/TestCases/Register/test_registerPageCase.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/TestCases/conftest.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/TestCases/conftest.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/conftest.py` & `opensourcetest-0.3.9/opensourcetest/uimodel/conftest.py`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/pytest.ini` & `opensourcetest-0.3.9/opensourcetest/uimodel/pytest.ini`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/opensourcetest/uimodel/readme.md` & `opensourcetest-0.3.9/opensourcetest/uimodel/readme.md`

 * *Files identical despite different names*

### Comparing `opensourcetest-0.3.8/pyproject.toml` & `opensourcetest-0.3.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opensourcetest"
-version = "0.3.8"
+version = "0.3.9"
 description = "We need more free software interface testing."
 license = "Apache-2.0"
 readme = "README.md"
 authors = ["chineseluo <848257135@qq.com>"]
 
 homepage = "https://github.com/chineseluo/opensourcetest"
 repository = "https://github.com/chineseluo/opensourcetest"
```

### Comparing `opensourcetest-0.3.8/setup.py` & `opensourcetest-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 {'console_scripts': ['OST = opensourcetest.cli:main',
                      'Opensourcetest = opensourcetest.cli:main',
                      'Ost = opensourcetest.cli:main',
                      'opensourcetest = opensourcetest.cli:main']}
 
 setup_kwargs = {
     'name': 'opensourcetest',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'We need more free software interface testing.',
     'long_description': '# **OpenSourceTest**\n\n# [![pyversions](https://img.shields.io/badge/opensourcetest-v0.3.x-green)](https://pypi.org/project/opensourcetest/)[![pyversions](https://img.shields.io/badge/pypi-v0.3.x-orange)](https://pypi.org/project/opensourcetest-test-test/)[![pyversions](https://img.shields.io/badge/pytest-5.x-green)](https://docs.pytest.org)[![pyversions](https://img.shields.io/badge/requests-2.x-green)](http://docs.python-requests.org/en/master/ )[![pyversions](https://img.shields.io/badge/allure-2.x-green)](https://docs.qameta.io/allure/  )\n\n`OpenSourceTest`将为您创建更加自由的软件自动化测试，不是为了简单而简单，而是为您提供更自由的可扩展的，适用于不同功能场景的`UI`自动化、APP自动化或接口自动化测试框架。\n\n## **设计思想**\n\n- 不丢弃轮子本身的优秀特性\n- 不过度封装\n- 提供更加多的可操作对象给使用者，即时你使用基本框架已经满足需求\n- 拥抱开源\n\n## **主要特点**\n\n### 支持创建`UI`自动化测试框架\n\n- 以[`yaml`][yaml]格式定义`UI`元素对象，[`yaml`][yaml]对象自动注入\n- 支持本地及远程分布式测试\n- 支持生成不同浏览器测试报告\n- 支持docker容器测试\n\n### 支持创建接口自动化测试框架\n\n- 继承 [`requests`][requests]的所有强大功能\n- 以[`yaml`][yaml]格式定义接口，[`yaml`][yaml]对象自动注入\n- 使用[`jmespath`][jmespath]提取和验证[`json`][json]响应\n\n### 支持创建APP自动化框架\n\n- 以[`yaml`][yaml]格式定义`UI`元素对象，[`yaml`][yaml]对象自动注入\n\n### 其他\n\n- 完美兼容[`pytest`][pytest]，您可以使用您想使用的任何[`pytest`][pytest]格式\n- 完美兼容[`allure`][allure]，您可以使用您想使用的任何[`allure`][allure]命令\n- 支持**CLI**命令，直接创建您所需要的项目架构\n\n## **OST计划**\n\n**即将上线微服务架构运维命令自动化测试框架CLI_TEST，基于云原生基础组件的测试框架，敬请期待，满足在集群内部的组件自动化测试，哈哈哈哈**\n\n![OST](/docs/images/OST.png)\n\n## **打赏支持**\n\n**OpenSourceTest由来自中国的成都-阿木木在空闲时间维护。虽然我致力于OpenSourceTest，因为我热爱这个项目，但是如果可能的话，希望可以得到一杯咖啡的打赏支持，您的打赏是我最大的支持。我会将打赏的胖友名单放入赞助者列表中，用以表示感谢。**\n\n\u200b\t**这些钱也将被用来维护框架，购买服务器，以及直播公开课等活动**\n\n\u200b\t**感谢各位胖友对OpenSourceTest框架的打赏，您的打赏支持是我最大的迭代更新的动力，也希望opensourcetest可以在日常工作中帮助到您，QAQ**\n\n\u200b\t**成为打赏者[become a sponsor](/docs/sponsors.md)**\n\n\u200b\t**联系作者：[成都-阿木木](mailto:848257135@qq.com)**\n\n**微信赞赏收款码**\n\n<img src="/docs/images/sponsors/wei.png" height="400" width="400" />\n\n\n\n## **OpenSourceTest 社区**\n\n欢迎测试小伙伴加群，讨论测试框架技术！\n\n<img src="/docs/images/community.jpg"/>\n\n\n[json]: http://json.com/\n[yaml]: http://www.yaml.org/\n[requests]: http://docs.python-requests.org/en/master/\n[pytest]: https://docs.pytest.org/\n[pydantic]: https://pydantic-docs.helpmanual.io/\n[jmespath]: https://jmespath.org/\n[allure]: https://docs.qameta.io/allure/',
     'author': 'chineseluo',
     'author_email': '848257135@qq.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/chineseluo/opensourcetest',
```

### Comparing `opensourcetest-0.3.8/PKG-INFO` & `opensourcetest-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourcetest
-Version: 0.3.8
+Version: 0.3.9
 Summary: We need more free software interface testing.
 Home-page: https://github.com/chineseluo/opensourcetest
 License: Apache-2.0
 Keywords: HTTP,http,Http,api,ui,UI,automated testing,interface,test,requests,pytest,allure,pytest-xdist
 Author: chineseluo
 Author-email: 848257135@qq.com
 Requires-Python: >=3.6,<4.0
```

