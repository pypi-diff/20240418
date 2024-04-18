# Comparing `tmp/openfoodfacts-0.2.1.tar.gz` & `tmp/openfoodfacts-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfoodfacts-0.2.1.tar", max compression
+gzip compressed data, was "openfoodfacts-0.3.0.tar", max compression
```

## Comparing `openfoodfacts-0.2.1.tar` & `openfoodfacts-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1182 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/LICENSE
--rw-r--r--   0        0        0     4138 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/README.md
--rw-r--r--   0        0        0      465 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/__init__.py
--rw-r--r--   0        0        0    14488 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/api.py
--rw-r--r--   0        0        0     3577 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/dataset.py
--rw-r--r--   0        0        0     4937 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/images.py
--rw-r--r--   0        0        0     1482 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/ingredients.py
--rw-r--r--   0        0        0    39496 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/ocr.py
--rw-r--r--   0        0        0        0 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/py.typed
--rw-r--r--   0        0        0    14036 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/taxonomy.py
--rw-r--r--   0        0        0    24499 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/types.py
--rw-r--r--   0        0        0     7455 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/utils.py
--rw-r--r--   0        0        0      935 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4730 1970-01-01 00:00:00.000000 openfoodfacts-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1182 2024-04-18 09:13:23.730280 openfoodfacts-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4138 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/README.md
+-rw-r--r--   0        0        0      465 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/openfoodfacts/__init__.py
+-rw-r--r--   0        0        0    15329 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/openfoodfacts/api.py
+-rw-r--r--   0        0        0     3577 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/openfoodfacts/dataset.py
+-rw-r--r--   0        0        0     4937 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/openfoodfacts/images.py
+-rw-r--r--   0        0        0     1482 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/openfoodfacts/ingredients.py
+-rw-r--r--   0        0        0    42409 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/openfoodfacts/ocr.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/openfoodfacts/py.typed
+-rw-r--r--   0        0        0    14036 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/openfoodfacts/taxonomy.py
+-rw-r--r--   0        0        0    24499 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/openfoodfacts/types.py
+-rw-r--r--   0        0        0    10197 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/openfoodfacts/utils.py
+-rw-r--r--   0        0        0      935 2024-04-18 09:13:23.734280 openfoodfacts-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4730 1970-01-01 00:00:00.000000 openfoodfacts-0.3.0/PKG-INFO
```

### Comparing `openfoodfacts-0.2.1/LICENSE` & `openfoodfacts-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.1/README.md` & `openfoodfacts-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.1/openfoodfacts/api.py` & `openfoodfacts-0.3.0/openfoodfacts/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     )
     if r.status_code == 404 and return_none_on_404:
         return None
     r.raise_for_status()
     return r.json()
 
 
-def send_for_urlencoded_post_request(
+def send_form_urlencoded_post_request(
     url: str, body: Dict[str, Any], api_config: APIConfig
 ) -> requests.Response:
     cookies = None
     if api_config.username and api_config.password:
         body["user_id"] = api_config.username
         body["password"] = api_config.password
     elif api_config.session_cookie:
@@ -57,14 +57,34 @@
         auth=get_http_auth(api_config.environment),
         cookies=cookies,
     )
     r.raise_for_status()
     return r
 
 
+class RobotoffResource:
+    def __init__(self, api_config: APIConfig):
+        self.api_config = api_config
+        self.base_url = URLBuilder.robotoff(environment=api_config.environment)
+
+    def predict_lang(self, text: str, k: int = 10, threshold: float = 0.01) -> JSONType:
+        """Predict the language of a text.
+
+        :param text: the text to predict the language of
+        :param k: the number of predictions to return, defaults to 10
+        :param threshold: the minimum probability for a prediction to be
+            returned, defaults to 0.01
+        :return: the API response
+        """
+        return http_session.post(
+            url=f"{self.base_url}/api/v1/predict/lang",
+            data={"text": text, "k": k, "threshold": threshold},
+        ).json()
+
+
 class FacetResource:
     def __init__(self, api_config: APIConfig):
         self.api_config = api_config
         self.base_url = URLBuilder.country(
             self.api_config.flavor,
             environment=api_config.environment,
             country_code=self.api_config.country.name,
@@ -204,15 +224,15 @@
 
     def update(self, body: Dict[str, Any]):
         """Create a new product or update an existing one."""
         if not body.get("code"):
             raise ValueError("missing code from body")
 
         url = f"{self.base_url}/cgi/product_jqm2.pl"
-        return send_for_urlencoded_post_request(url, body, self.api_config)
+        return send_form_urlencoded_post_request(url, body, self.api_config)
 
     def select_image(
         self,
         code: str,
         image_id: str,
         image_key: str,
         rotate: Optional[int] = None,
@@ -335,14 +355,15 @@
             session_cookie=session_cookie,
             timeout=timeout,
         )
         self.password = password
         self.country = country
         self.product = ProductResource(self.api_config)
         self.facet = FacetResource(self.api_config)
+        self.robotoff = RobotoffResource(self.api_config)
 
 
 def parse_ingredients(text: str, lang: str, api_config: APIConfig) -> list[JSONType]:
     """Parse ingredients text using Product Opener API.
 
     It is only available for `off` flavor (food).
```

### Comparing `openfoodfacts-0.2.1/openfoodfacts/dataset.py` & `openfoodfacts-0.3.0/openfoodfacts/dataset.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.1/openfoodfacts/images.py` & `openfoodfacts-0.3.0/openfoodfacts/images.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.1/openfoodfacts/ingredients.py` & `openfoodfacts-0.3.0/openfoodfacts/ingredients.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.1/openfoodfacts/ocr.py` & `openfoodfacts-0.3.0/openfoodfacts/ocr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+import base64
 import enum
+import io
 import itertools
 import json
 import math
 import operator
 import re
 from collections import Counter, defaultdict
+from pathlib import Path
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import requests
 
 from .types import JSONType
-from .utils import get_logger, http_session
+from .utils import _pillow_available, get_logger, http_session
+
+if _pillow_available:
+    from PIL import Image
 
 # Some classes documentation were adapted from Google documentation on
 # https://cloud.google.com/vision/docs/reference/rpc/google.cloud.vision.v1#google.cloud.vision.v1.Symbol
 
 
 logger = get_logger(__name__)
 
@@ -1148,7 +1154,87 @@
 class SafeSearchAnnotationLikelihood(enum.IntEnum):
     UNKNOWN = 1
     VERY_UNLIKELY = 2
     UNLIKELY = 3
     POSSIBLE = 4
     LIKELY = 5
     VERY_LIKELY = 6
+
+
+def get_base64_from_image(
+    image: Union["Image.Image", Path, str], session: Optional[requests.Session] = None
+) -> str:
+    """Return the base64 representation of an image.
+
+    :param image: the image to convert to base64. Can be a PIL Image, a Path
+        object, or a URL
+    :param session: the requests Session to use to download the image if
+        `image` is a URL, optional (the default session is used if not set)
+    :raises TypeError: if `image` is not a PIL Image, a Path object, or a URL
+    :return: the base64 representation of the image
+    """
+    if _pillow_available and isinstance(image, Image.Image):
+        image_bytes_fp = io.BytesIO()
+        image.save(image_bytes_fp, format="PNG")
+        image_bytes = image_bytes_fp.getvalue()
+    elif isinstance(image, Path):
+        image_bytes = image.read_bytes()
+    elif isinstance(image, str):
+        if not session:
+            session = http_session
+        image_bytes = session.get(image).content
+    else:
+        raise TypeError(f"Invalid type: {type(image)}")
+
+    return base64.b64encode(image_bytes).decode("utf-8")
+
+
+class OCRFeature(str, enum.Enum):
+    """The OCR features supported by Google Cloud Vision API."""
+
+    TEXT_DETECTION = enum.auto()
+    LOGO_DETECTION = enum.auto()
+    LABEL_DETECTION = enum.auto()
+    SAFE_SEARCH_DETECTION = enum.auto()
+    FACE_DETECTION = enum.auto()
+
+
+def run_ocr_on_image_batch(
+    images: list[Union["Image.Image", Path, str]],
+    api_key: str,
+    features: Optional[list[OCRFeature]] = None,
+    session: Optional[requests.Session] = None,
+) -> requests.Response:
+    """Run Google Cloud Vision OCR on a batch of images.
+
+    :param images: a list of images to run OCR on. Can be PIL Images, Path
+        or URLs
+    :param api_key: the Google Cloud Vision API key to use
+    :param features: the list of OCR features to use, defaults to
+        [OCRFeature.TEXT_DETECTION]
+    :param session: the requests Session to use to download the images if
+        `images` contains URLs, optional (the default session is used if not
+        set)
+    :return: the requests Response object
+    """
+    if session is None:
+        session = http_session
+
+    if features is None:
+        features = [OCRFeature.TEXT_DETECTION]
+    else:
+        features = list(set(features))
+
+    base64_images = [get_base64_from_image(image, session=session) for image in images]
+    r = session.post(
+        f"https://vision.googleapis.com/v1/images:annotate?key={api_key}",
+        json={
+            "requests": [
+                {
+                    "features": [{"type": feature.name} for feature in features],
+                    "image": {"content": base64_image},
+                }
+                for base64_image in base64_images
+            ]
+        },
+    )
+    return r
```

### Comparing `openfoodfacts-0.2.1/openfoodfacts/taxonomy.py` & `openfoodfacts-0.3.0/openfoodfacts/taxonomy.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.1/openfoodfacts/types.py` & `openfoodfacts-0.3.0/openfoodfacts/types.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.1/openfoodfacts/utils.py` & `openfoodfacts-0.3.0/openfoodfacts/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,69 @@
 import gzip
 import json
 import logging
 import shutil
 import time
+from io import BytesIO
 from pathlib import Path
 from typing import Callable, Dict, Iterable, List, Optional, Union
 
 import requests
 import tqdm
 
 from .types import COUNTRY_CODE_TO_NAME, Country, Environment, Flavor
 
 _orjson_available = True
 try:
     import orjson
 except ImportError:
     _orjson_available = False
 
+_pillow_available = True
+try:
+    import PIL
+    from PIL import Image
+except ImportError:
+    _pillow_available = False
+
 http_session = requests.Session()
 http_session.headers.update({"User-Agent": "openfoodfacts-python"})
 
 
+def configure_root_logger(
+    logger: logging.Logger,
+    level: int = logging.INFO,
+    formatter_string: Optional[str] = None,
+):
+    logger.setLevel(level)
+    handler = logging.StreamHandler()
+
+    if formatter_string is None:
+        formatter_string = "%(asctime)s :: %(levelname)s :: %(message)s"
+
+    formatter = logging.Formatter(formatter_string)
+    handler.setFormatter(formatter)
+    handler.setLevel(level)
+    logger.addHandler(handler)
+    return logger
+
+
+def get_logger(name=None, level: int = logging.INFO) -> logging.Logger:
+    logger = logging.getLogger(name)
+    logger.setLevel(level)
+
+    if name is None:
+        configure_root_logger(logger, level)
+
+    return logger
+
+
+logger = get_logger(__name__)
+
+
 class URLBuilder:
     """URLBuilder allows to generate URLs for Product Opener/Robotoff.
 
     Example usage: URLBuilder.robotoff() returns the Robotoff URL.
     """
 
     @staticmethod
@@ -80,42 +119,14 @@
         return URLBuilder._get_url(
             prefix=country_code,
             tld=environment.value,
             base_domain=flavor.get_base_domain(),
         )
 
 
-def get_logger(name=None, level: int = logging.INFO) -> logging.Logger:
-    logger = logging.getLogger(name)
-    logger.setLevel(level)
-
-    if name is None:
-        configure_root_logger(logger, level)
-
-    return logger
-
-
-def configure_root_logger(
-    logger: logging.Logger,
-    level: int = logging.INFO,
-    formatter_string: Optional[str] = None,
-):
-    logger.setLevel(level)
-    handler = logging.StreamHandler()
-
-    if formatter_string is None:
-        formatter_string = "%(asctime)s :: %(levelname)s :: %(message)s"
-
-    formatter = logging.Formatter(formatter_string)
-    handler.setFormatter(formatter)
-    handler.setLevel(level)
-    logger.addHandler(handler)
-    return logger
-
-
 def jsonl_iter(jsonl_path: Union[str, Path]) -> Iterable[Dict]:
     """Iterate over elements of a JSONL file.
 
     :param jsonl_path: the path of the JSONL file. Both plain (.jsonl) and
         gzipped (jsonl.gz) files are supported.
     :yield: dict contained in the JSONL file
     """
@@ -255,7 +266,88 @@
 
     return True
 
 
 def get_country_name(country: Country) -> str:
     """Return country name code (ex: `en:portugal`) from `Country`."""
     return COUNTRY_CODE_TO_NAME[country]
+
+
+class AssetLoadingException(Exception):
+    """Exception raised by `get_asset_from_url` when an asset cannot be fetched
+    from URL or if loading failed.
+    """
+
+    pass
+
+
+def get_asset_from_url(
+    asset_url: str,
+    error_raise: bool = True,
+    session: Optional[requests.Session] = None,
+    auth: Optional[tuple[str, str]] = None,
+) -> Optional[requests.Response]:
+    try:
+        if session:
+            r = session.get(asset_url, auth=auth)
+        else:
+            r = requests.get(asset_url, auth=auth)
+    except (
+        requests.exceptions.ConnectionError,
+        requests.exceptions.SSLError,
+        requests.exceptions.Timeout,
+    ) as e:
+        error_message = "Cannot download %s"
+        if error_raise:
+            raise AssetLoadingException(error_message % asset_url) from e
+        logger.info(error_message, asset_url, exc_info=e)
+        return None
+
+    if not r.ok:
+        error_message = "Cannot download %s: HTTP %s"
+        error_args = (asset_url, r.status_code)
+        if error_raise:
+            raise AssetLoadingException(error_message % error_args)
+        logger.log(
+            logging.INFO if r.status_code < 500 else logging.WARNING,
+            error_message,
+            *error_args,
+        )
+        return None
+
+    return r
+
+
+def get_image_from_url(
+    image_url: str, error_raise: bool = True, session: Optional[requests.Session] = None
+) -> Optional["Image.Image"]:
+    """Fetch an image from `image_url` and load it.
+
+    :param image_url: URL of the image to load
+    :param error_raise: if True, raises a `AssetLoadingException` if an error
+      occured, defaults to False. If False, None is returned if an error
+      occured.
+    :param session: requests Session to use, by default no session is used.
+    :return: the Pillow Image or None.
+    """
+    if not _pillow_available:
+        raise ImportError("Pillow is required to load images")
+
+    r = get_asset_from_url(image_url, error_raise, session)
+    if r is None:
+        return None
+    content_bytes = r.content
+
+    try:
+        return Image.open(BytesIO(content_bytes))
+    except PIL.UnidentifiedImageError:
+        error_message = f"Cannot identify image {image_url}"
+        if error_raise:
+            raise AssetLoadingException(error_message)
+        logger.info(error_message)
+    except PIL.Image.DecompressionBombError:
+        error_message = f"Decompression bomb error for image {image_url}"
+        if error_raise:
+            raise AssetLoadingException(error_message)
+        logger.info(error_message)
+
+    return None
```

### Comparing `openfoodfacts-0.2.1/pyproject.toml` & `openfoodfacts-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openfoodfacts"
-version = "0.2.1"
+version = "0.3.0"
 description = "Official Python SDK of Open Food Facts"
 authors = ["The Open Food Facts team"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `openfoodfacts-0.2.1/PKG-INFO` & `openfoodfacts-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfoodfacts
-Version: 0.2.1
+Version: 0.3.0
 Summary: Official Python SDK of Open Food Facts
 License: Apache 2.0
 Author: The Open Food Facts team
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

