# Comparing `tmp/accuweather-2.1.1.tar.gz` & `tmp/accuweather-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accuweather-2.1.1.tar", last modified: Sun Nov 26 20:17:55 2023, max compression
+gzip compressed data, was "accuweather-3.0.0.tar", last modified: Thu Apr 18 20:33:17 2024, max compression
```

## Comparing `accuweather-2.1.1.tar` & `accuweather-3.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:17:55.045539 accuweather-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11311 2023-11-26 20:17:45.000000 accuweather-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-26 20:17:45.000000 accuweather-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-11-26 20:17:55.045539 accuweather-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-11-26 20:17:45.000000 accuweather-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:17:55.045539 accuweather-2.1.1/accuweather/
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2023-11-26 20:17:45.000000 accuweather-2.1.1/accuweather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2023-11-26 20:17:45.000000 accuweather-2.1.1/accuweather/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-11-26 20:17:45.000000 accuweather-2.1.1/accuweather/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-26 20:17:45.000000 accuweather-2.1.1/accuweather/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2023-11-26 20:17:45.000000 accuweather-2.1.1/accuweather/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:17:55.045539 accuweather-2.1.1/accuweather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-11-26 20:17:55.000000 accuweather-2.1.1/accuweather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-11-26 20:17:55.000000 accuweather-2.1.1/accuweather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 20:17:55.000000 accuweather-2.1.1/accuweather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-26 20:17:55.000000 accuweather-2.1.1/accuweather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-26 20:17:55.000000 accuweather-2.1.1/accuweather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-11-26 20:17:45.000000 accuweather-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-26 20:17:45.000000 accuweather-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 20:17:55.045539 accuweather-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2023-11-26 20:17:45.000000 accuweather-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:17:55.045539 accuweather-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10590 2023-11-26 20:17:45.000000 accuweather-2.1.1/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:33:17.090337 accuweather-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11311 2024-04-18 20:33:09.000000 accuweather-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 20:33:09.000000 accuweather-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-18 20:33:17.090337 accuweather-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-18 20:33:09.000000 accuweather-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:33:17.090337 accuweather-3.0.0/accuweather/
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-04-18 20:33:09.000000 accuweather-3.0.0/accuweather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 20:33:09.000000 accuweather-3.0.0/accuweather/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 20:33:09.000000 accuweather-3.0.0/accuweather/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 20:33:09.000000 accuweather-3.0.0/accuweather/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-18 20:33:09.000000 accuweather-3.0.0/accuweather/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:33:17.090337 accuweather-3.0.0/accuweather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-18 20:33:17.000000 accuweather-3.0.0/accuweather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 20:33:17.000000 accuweather-3.0.0/accuweather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 20:33:17.000000 accuweather-3.0.0/accuweather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 20:33:17.000000 accuweather-3.0.0/accuweather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 20:33:17.000000 accuweather-3.0.0/accuweather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-18 20:33:09.000000 accuweather-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 20:33:09.000000 accuweather-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 20:33:17.090337 accuweather-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-18 20:33:09.000000 accuweather-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 20:33:17.090337 accuweather-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-18 20:33:09.000000 accuweather-3.0.0/tests/test_init.py
```

### Comparing `accuweather-2.1.1/LICENSE` & `accuweather-3.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Maciej Bieniek
+   Copyright 2024 Maciej Bieniek
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `accuweather-2.1.1/PKG-INFO` & `accuweather-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: accuweather
-Version: 2.1.1
+Version: 3.0.0
 Summary: Python wrapper for getting weather data from AccuWeather API.
 Home-page: https://github.com/bieniu/accuweather
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.0
 Requires-Dist: orjson
 
 [![GitHub Release][releases-shield]][releases]
 [![PyPI][pypi-releases-shield]][pypi-releases]
```

### Comparing `accuweather-2.1.1/README.md` & `accuweather-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `accuweather-2.1.1/accuweather/__init__.py` & `accuweather-3.0.0/accuweather/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AccuWeather:
     """Main class to perform AccuWeather API requests."""
 
-    def __init__(  # noqa: PLR0913
+    def __init__(
         self,
         api_key: str,
         session: ClientSession,
         latitude: float | None = None,
         longitude: float | None = None,
         location_key: str | None = None,
         language: str = "en",
```

### Comparing `accuweather-2.1.1/accuweather/const.py` & `accuweather-3.0.0/accuweather/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants for AccuWeather library."""
+
 from __future__ import annotations
 
 ATTR_CURRENT_CONDITIONS: str = "currentconditions"
 ATTR_FORECAST_DAILY: str = "forecasts"
 ATTR_FORECAST_HOURLY: str = "forecasts_hourly"
 ATTR_GEOPOSITION: str = "geoposition"
```

### Comparing `accuweather-2.1.1/accuweather/exceptions.py` & `accuweather-3.0.0/accuweather/exceptions.py`

 * *Files identical despite different names*

### Comparing `accuweather-2.1.1/accuweather/utils.py` & `accuweather-3.0.0/accuweather/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utils for AccuWeather."""
+
 from __future__ import annotations
 
 from typing import Any
 
 from .const import (
     ENDPOINT,
     MAX_API_KEY_LENGTH,
```

### Comparing `accuweather-2.1.1/accuweather.egg-info/PKG-INFO` & `accuweather-3.0.0/accuweather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: accuweather
-Version: 2.1.1
+Version: 3.0.0
 Summary: Python wrapper for getting weather data from AccuWeather API.
 Home-page: https://github.com/bieniu/accuweather
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.0
 Requires-Dist: orjson
 
 [![GitHub Release][releases-shield]][releases]
 [![PyPI][pypi-releases-shield]][pypi-releases]
```

### Comparing `accuweather-2.1.1/setup.py` & `accuweather-3.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Setup module for accuweather."""
+
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "2.1.1"
+VERSION = "3.0.0"
 
 setup(
     name="accuweather",
     version=VERSION,
     author="Maciej Bieniek",
     description="Python wrapper for getting weather data from AccuWeather API.",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/bieniu/accuweather",
     license="Apache-2.0 License",
     packages=["accuweather"],
     package_data={"accuweather": ["py.typed"]},
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     install_requires=["aiohttp>=3.7.0", "orjson"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Typing :: Typed",
     ],
 )
```

### Comparing `accuweather-2.1.1/tests/test_init.py` & `accuweather-3.0.0/tests/test_init.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Tests for accuweather package."""
+
 from http import HTTPStatus
+from typing import Any
 
 import aiohttp
-import orjson
 import pytest
 from aiohttp import ClientSession
 from aioresponses import aioresponses
+from syrupy import SnapshotAssertion
 
 from accuweather import (
     AccuWeather,
     ApiError,
     InvalidApiKeyError,
     InvalidCoordinatesError,
     RequestsExceededError,
@@ -19,44 +21,16 @@
 INVALID_API_KEY = "abcdef"
 LATITUDE = 52.0677904
 LOCATION_KEY = "268068"
 LONGITUDE = 19.4795644
 VALID_API_KEY = "32-character-string-1234567890qw"
 
 
-@pytest.fixture()
-def location_data():
-    """Location data fixture."""
-    with open("tests/fixtures/location_data.json", encoding="utf-8") as file:
-        return orjson.loads(file.read())
-
-
-@pytest.fixture()
-def current_condition_data():
-    """Weather current condition data fixture."""
-    with open("tests/fixtures/current_condition_data.json", encoding="utf-8") as file:
-        return orjson.loads(file.read())
-
-
-@pytest.fixture()
-def daily_forecast_data():
-    """Daily forecast data fixture."""
-    with open("tests/fixtures/daily_forecast_data.json", encoding="utf-8") as file:
-        return orjson.loads(file.read())
-
-
-@pytest.fixture()
-def hourly_forecast_data():
-    """Hourly forecast data fixture."""
-    with open("tests/fixtures/hourly_forecast_data.json", encoding="utf-8") as file:
-        return orjson.loads(file.read())
-
-
-@pytest.mark.asyncio
-async def test_get_location(location_data):
+@pytest.mark.asyncio()
+async def test_get_location(location_data: dict[str, Any]) -> None:
     """Test with valid location data."""
     session = aiohttp.ClientSession()
 
     with aioresponses() as session_mock:
         session_mock.get(
             "https://dataservice.accuweather.com/locations/v1/cities/geoposition/search?apikey=32-character-string-1234567890qw&q=52.0677904%252C19.4795644&language=en-us",
             payload=location_data,
@@ -70,16 +44,20 @@
     await session.close()
 
     assert accuweather.location_name == "Piątek"
     assert accuweather.location_key == "268068"
     assert accuweather.requests_remaining == 23
 
 
-@pytest.mark.asyncio
-async def test_get_current_conditions(location_data, current_condition_data):
+@pytest.mark.asyncio()
+async def test_get_current_conditions(
+    location_data: dict[str, Any],
+    current_condition_data: dict[str, Any],
+    snapshot: SnapshotAssertion,
+) -> None:
     """Test with valid current condition data."""
     session = aiohttp.ClientSession()
 
     with aioresponses() as session_mock:
         session_mock.get(
             "https://dataservice.accuweather.com/currentconditions/v1/268068?apikey=32-character-string-1234567890qw&details=true&language=en-us",
             payload=current_condition_data,
@@ -93,31 +71,25 @@
         accuweather = AccuWeather(
             VALID_API_KEY, session, latitude=LATITUDE, longitude=LONGITUDE
         )
         current_conditions = await accuweather.async_get_current_conditions()
 
     await session.close()
 
-    assert current_conditions["WeatherIcon"] == 7
-    assert current_conditions["WeatherText"] == "Cloudy"
-    assert current_conditions["HasPrecipitation"] is False
-    assert current_conditions["PrecipitationType"] is None
-    assert current_conditions["Temperature"]["Metric"]["Value"] == 13.4
-    assert current_conditions["Temperature"]["Metric"]["Unit"] == "C"
-    assert current_conditions["Temperature"]["Imperial"]["Value"] == 56
-    assert current_conditions["Temperature"]["Imperial"]["Unit"] == "F"
-    assert current_conditions["UVIndex"] == 2
-    assert current_conditions["UVIndexText"] == "low"
-    assert current_conditions["PressureTendency"]["LocalizedText"] == "steady"
+    assert current_conditions == snapshot
 
     assert accuweather.requests_remaining == 23
 
 
-@pytest.mark.asyncio
-async def test_get_daily_forecast(location_data, daily_forecast_data):
+@pytest.mark.asyncio()
+async def test_get_daily_forecast(
+    location_data: dict[str, Any],
+    daily_forecast_data: dict[str, Any],
+    snapshot: SnapshotAssertion,
+) -> None:
     """Test with valid daily forecast data."""
     session = aiohttp.ClientSession()
 
     with aioresponses() as session_mock:
         session_mock.get(
             "https://dataservice.accuweather.com/forecasts/v1/daily/5day/268068?apikey=32-character-string-1234567890qw&details=true&metric=true&language=en-us",
             payload=daily_forecast_data,
@@ -132,31 +104,25 @@
         accuweather = AccuWeather(
             VALID_API_KEY, session, latitude=LATITUDE, longitude=LONGITUDE
         )
         forecast = await accuweather.async_get_daily_forecast()
 
     await session.close()
 
-    assert forecast[0]["IconDay"] == 18
-    assert forecast[0]["IconPhraseDay"] == "rain"
-    assert forecast[0]["PrecipitationProbabilityDay"] == 91
-    assert forecast[0]["WindDay"]["Speed"]["Value"] == 16.7
-    assert forecast[0]["TemperatureMax"]["Value"] == 16.2
-    assert forecast[0]["TemperatureMax"]["Unit"] == "C"
-    assert forecast[0]["UVIndex"]["Category"] == "low"
-    assert forecast[0]["PrecipitationTypeDay"] == "rain"
-    assert forecast[0]["PrecipitationIntensityDay"] == "light"
-    assert forecast[0]["ShortPhraseDay"] == "Cooler with periods of rain"
-    assert forecast[0]["LongPhraseDay"] == "Cooler with periods of rain"
-    assert forecast[0]["AirQuality"]["Category"] == "unhealthy"
+    assert forecast == snapshot
+
     assert accuweather.requests_remaining == 23
 
 
-@pytest.mark.asyncio
-async def test_get_hourly_forecast(location_data, hourly_forecast_data):
+@pytest.mark.asyncio()
+async def test_get_hourly_forecast(
+    location_data: dict[str, Any],
+    hourly_forecast_data: list[dict[str, Any]],
+    snapshot: SnapshotAssertion,
+) -> None:
     """Test with valid hourly forecast data."""
     session = aiohttp.ClientSession()
 
     with aioresponses() as session_mock:
         session_mock.get(
             "https://dataservice.accuweather.com/forecasts/v1/hourly/12hour/268068?apikey=32-character-string-1234567890qw&details=true&metric=true&language=en-us",
             payload=hourly_forecast_data,
@@ -171,41 +137,34 @@
         accuweather = AccuWeather(
             VALID_API_KEY, session, latitude=LATITUDE, longitude=LONGITUDE
         )
         forecast = await accuweather.async_get_hourly_forecast()
 
     await session.close()
 
-    assert forecast[0]["WeatherIcon"] == 18
-    assert forecast[0]["IconPhrase"] == "rain"
-    assert forecast[0]["HasPrecipitation"] is True
-    assert forecast[0]["UVIndex"] == 2
-    assert forecast[0]["UVIndexText"] == "low"
-    assert forecast[0]["PrecipitationType"] == "rain"
-    assert forecast[0]["PrecipitationIntensity"] == "light"
-    assert forecast[0]["Temperature"]["Value"] == 14.7
-    assert forecast[0]["Temperature"]["Unit"] == "C"
+    assert forecast == snapshot
+
     assert accuweather.requests_remaining == 23
 
 
-@pytest.mark.asyncio
-async def test_invalid_api_key_1():
+@pytest.mark.asyncio()
+async def test_invalid_api_key_1() -> None:
     """Test with invalid API key."""
     async with ClientSession() as session:
         with pytest.raises(
             InvalidApiKeyError,
             match="Your API Key must be a 32-character hexadecimal string",
         ):
             AccuWeather(
                 INVALID_API_KEY, session, latitude=LATITUDE, longitude=LONGITUDE
             )
 
 
-@pytest.mark.asyncio
-async def test_invalid_api_key_2():
+@pytest.mark.asyncio()
+async def test_invalid_api_key_2() -> None:
     """Test with invalid API key."""
     session = aiohttp.ClientSession()
 
     with aioresponses() as session_mock:
         session_mock.get(
             "https://dataservice.accuweather.com/currentconditions/v1/268068?apikey=32-character-string-1234567890qw&details=true&language=en-us",
             status=HTTPStatus.UNAUTHORIZED.value,
@@ -213,36 +172,36 @@
         accuweather = AccuWeather(VALID_API_KEY, session, location_key=LOCATION_KEY)
         with pytest.raises(InvalidApiKeyError, match="Invalid API key"):
             await accuweather.async_get_current_conditions()
 
     await session.close()
 
 
-@pytest.mark.asyncio
-async def test_invalid_coordinates_1():
+@pytest.mark.asyncio()
+async def test_invalid_coordinates_1() -> None:
     """Test with invalid coordinates."""
     async with ClientSession() as session:
         with pytest.raises(
             InvalidCoordinatesError, match="Your coordinates are invalid"
         ):
             AccuWeather(VALID_API_KEY, session, latitude=55.55, longitude="78.00")
 
 
-@pytest.mark.asyncio
-async def test_invalid_coordinates_2():
+@pytest.mark.asyncio()
+async def test_invalid_coordinates_2() -> None:
     """Test with invalid coordinates."""
     async with ClientSession() as session:
         with pytest.raises(
             InvalidCoordinatesError, match="Your coordinates are invalid"
         ):
             AccuWeather(VALID_API_KEY, session, latitude=199.99, longitude=90.0)
 
 
-@pytest.mark.asyncio
-async def test_api_error():
+@pytest.mark.asyncio()
+async def test_api_error() -> None:
     """Test with API error."""
     payload = {
         "Code": "ServiceError",
         "Message": "API error.",
     }
 
     session = aiohttp.ClientSession()
@@ -260,16 +219,16 @@
             ApiError, match="Invalid response from AccuWeather API: 404"
         ):
             await accuweather.async_get_location()
 
     await session.close()
 
 
-@pytest.mark.asyncio
-async def test_requests_exceeded_error():
+@pytest.mark.asyncio()
+async def test_requests_exceeded_error() -> None:
     """Test with requests exceeded error."""
     payload = {
         "Code": "ServiceUnavailable",
         "Message": "The allowed number of requests has been exceeded.",
     }
 
     session = aiohttp.ClientSession()
```

