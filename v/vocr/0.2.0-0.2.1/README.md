# Comparing `tmp/vocr-0.2.0.tar.gz` & `tmp/vocr-0.2.1.tar.gz`

## Comparing `vocr-0.2.0.tar` & `vocr-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 vocr-0.2.0/src/vocr/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 vocr-0.2.0/src/vocr/__main__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 vocr-0.2.0/src/vocr/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vocr-0.2.0/src/vocr/py.typed
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 vocr-0.2.0/src/vocr/vocr.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 vocr-0.2.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 vocr-0.2.0/LICENSE
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 vocr-0.2.0/README.md
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 vocr-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 vocr-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 vocr-0.2.1/src/vocr/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 vocr-0.2.1/src/vocr/__main__.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 vocr-0.2.1/src/vocr/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vocr-0.2.1/src/vocr/py.typed
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 vocr-0.2.1/src/vocr/vocr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vocr-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 vocr-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 vocr-0.2.1/tests/test_ocr.py
+-rw-r--r--   0        0        0    16977 2020-02-02 00:00:00.000000 vocr-0.2.1/tests/img/sample1.jpg
+-rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 vocr-0.2.1/tests/img/sample2.jpg
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 vocr-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 vocr-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 vocr-0.2.1/README.md
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 vocr-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 vocr-0.2.1/PKG-INFO
```

### Comparing `vocr-0.2.0/src/vocr/vocr.py` & `vocr-0.2.1/src/vocr/vocr.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-from __future__ import annotations  # Maybe needed
-
-__all__ = ["VietOCR"]
-
-from pathlib import Path
-from typing import List, Literal, Union
-
-import cv2
-import pytesseract
-from cv2.typing import MatLike
-from joblib import Parallel, delayed
-from PIL import Image
-from tqdm import tqdm
-
-VALID_IMG_SUFFIX = [".jpg", ".jpeg", ".png"]
-
-
-class VietOCR_File:
-    """
-    Vietnamese image OCR - File
-    """
-
-    def __init__(self, image: Union[str, Path], *, lang: str = "vie") -> None:
-        self.image_path: Path = Path(image)
-        self.lang = lang
-
-    def __str__(self) -> str:
-        return self.__repr__()
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.image_path.name})"
-
-    def ocr_only(
-        self,
-        preprocess: Literal["thresh", "blur"] = "thresh",
-    ) -> str:
-        """OCR only (no output file)"""
-
-        # Load
-        img: MatLike = cv2.imread(self.image_path.__str__())  # Read img file
-        gray_img: MatLike = cv2.cvtColor(
-            img, cv2.COLOR_BGR2GRAY
-        )  # Convert to grayscale
-
-        # Preprocess
-        if preprocess == "thresh":  # Black white only
-            gray_img = cv2.threshold(
-                gray_img, 0, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU
-            )[1]
-        else:  # Blur
-            gray_img = cv2.medianBlur(gray_img, 3)
-
-        # Extract text
-        text = pytesseract.image_to_string(Image.fromarray(gray_img), lang=self.lang)
-
-        # Return
-        return text  # type: ignore
-
-    def ocr(
-        self,
-        save_destination: Union[str, Path, None] = None,
-        preprocess: Literal["thresh", "blur"] = "thresh",
-    ) -> None:
-        """OCR"""
-        if save_destination is None:
-            output_path = self.image_path.with_suffix(".txt")
-        else:
-            output_path = Path(save_destination)
-        with open(output_path, "w", encoding="utf-8") as f:
-            ocr_res = self.ocr_only(preprocess=preprocess)
-            f.write(ocr_res)
-
-
-class VietOCR_Directory:
-    """
-    Vietnamese image OCR - Directory
-    """
-
-    def __init__(self, image_dir: Union[str, Path], *, lang: str = "vie") -> None:
-        self.image_path: Path = Path(image_dir)
-        self.lang = lang
-
-    def __str__(self) -> str:
-        return self.__repr__()
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self.image_path.name})"
-
-    def list_of_img(self) -> List[Path]:
-        list_of_img = [
-            img
-            for img in self.image_path.iterdir()
-            if img.suffix.lower() in VALID_IMG_SUFFIX
-        ]
-        return list_of_img
-
-    def make_save_destination(
-        self,
-        save_destination: Union[str, Path, None] = None,
-    ) -> Path:
-        if save_destination is not None:
-            save_folder = Path(save_destination)
-        else:
-            save_folder = self.image_path.with_name(f"{self.image_path.name}_extracted")
-        save_folder.mkdir(exist_ok=True, parents=True)
-        return save_folder
-
-    def ocr(
-        self,
-        save_destination: Union[str, Path, None] = None,
-        preprocess: Literal["thresh", "blur"] = "thresh",
-    ) -> None:
-        """Performs OCR on img dir
-
-        :param save_destination: Folder location, defaults to None
-        :type save_destination: str | Path | None, optional
-        :param preprocess: Preprocess, defaults to "thresh"
-        :type preprocess: Literal[&quot;thresh&quot;, &quot;blur&quot;], optional
-        """
-        save_folder = self.make_save_destination(save_destination)
-        for img in tqdm(
-            self.list_of_img(), desc="Extracting text", unit_scale=True, ncols=88
-        ):
-            ocr_engine = VietOCR_File(img, lang=self.lang)
-            save_path = save_folder.joinpath(img.with_suffix(".txt").name)
-            ocr_engine.ocr(save_destination=save_path, preprocess=preprocess)
-
-    def ocr_multithread(
-        self,
-        n_jobs: int = -1,
-        save_destination: Union[str, Path, None] = None,
-        preprocess: Literal["thresh", "blur"] = "thresh",
-    ) -> None:
-        save_folder = self.make_save_destination(save_destination)
-
-        def _ocr(img: Path):
-            ocr_engine = VietOCR_File(img, lang=self.lang)
-            save_path = save_folder.joinpath(img.with_suffix(".txt").name)
-            ocr_engine.ocr(save_destination=save_path, preprocess=preprocess)
-
-        # Multithread
-        Parallel(n_jobs=n_jobs)(
-            delayed(_ocr)(img)
-            for img in tqdm(
-                self.list_of_img(), desc="Extracting text", unit_scale=True, ncols=88
-            )
-        )
-
-
-class VietOCR:
-    """
-    Vietnamese image OCR
-    """
-
-    def __init__(self, path: Union[str, Path], *, lang: str = "vie") -> None:
-        self.path: Path = Path(path)
-        if not self.path.exists():
-            raise ValueError("Path does not exist")
-        self.lang = lang
-
-        if self.path.is_dir():
-            self.engine = VietOCR_Directory(self.path, lang=self.lang)
-        else:
-            self.engine = VietOCR_File(self.path, lang=self.lang)  # type: ignore
-
-    def ocr(
-        self,
-        save_destination: Union[str, Path, None] = None,
-        preprocess: Literal["thresh", "blur"] = "thresh",
-    ) -> None:
-        try:
-            self.engine.ocr_multithread(
-                save_destination=save_destination, preprocess=preprocess
-            )
-        except Exception:
-            self.engine.ocr(save_destination=save_destination, preprocess=preprocess)
+from __future__ import annotations  # Maybe needed
+
+__all__ = ["VietOCR"]
+
+from pathlib import Path
+from typing import List, Literal, Union
+
+import cv2
+import pytesseract
+from cv2.typing import MatLike
+from joblib import Parallel, delayed
+from PIL import Image
+from tqdm import tqdm
+
+VALID_IMG_SUFFIX = [".jpg", ".jpeg", ".png"]
+
+
+class VietOCR_File:
+    """
+    Vietnamese image OCR - File
+    """
+
+    def __init__(self, image: Union[str, Path], *, lang: str = "vie") -> None:
+        self.image_path: Path = Path(image)
+        self.lang = lang
+
+    def __str__(self) -> str:
+        return self.__repr__()
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.image_path.name})"
+
+    def ocr_only(
+        self,
+        preprocess: Literal["thresh", "blur"] = "thresh",
+    ) -> str:
+        """OCR only (no output file)"""
+
+        # Load
+        img: MatLike = cv2.imread(self.image_path.__str__())  # Read img file
+        gray_img: MatLike = cv2.cvtColor(
+            img, cv2.COLOR_BGR2GRAY
+        )  # Convert to grayscale
+
+        # Preprocess
+        if preprocess == "thresh":  # Black white only
+            gray_img = cv2.threshold(
+                gray_img, 0, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU
+            )[1]
+        else:  # Blur
+            gray_img = cv2.medianBlur(gray_img, 3)
+
+        # Extract text
+        text = pytesseract.image_to_string(Image.fromarray(gray_img), lang=self.lang)
+
+        # Return
+        return text  # type: ignore
+
+    def ocr(
+        self,
+        save_destination: Union[str, Path, None] = None,
+        preprocess: Literal["thresh", "blur"] = "thresh",
+    ) -> None:
+        """OCR"""
+        if save_destination is None:
+            output_path = self.image_path.with_suffix(".txt")
+        else:
+            output_path = Path(save_destination)
+        with open(output_path, "w", encoding="utf-8") as f:
+            ocr_res = self.ocr_only(preprocess=preprocess)
+            f.write(ocr_res)
+
+
+class VietOCR_Directory:
+    """
+    Vietnamese image OCR - Directory
+    """
+
+    def __init__(self, image_dir: Union[str, Path], *, lang: str = "vie") -> None:
+        self.image_path: Path = Path(image_dir)
+        self.lang = lang
+
+    def __str__(self) -> str:
+        return self.__repr__()
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self.image_path.name})"
+
+    def list_of_img(self) -> List[Path]:
+        list_of_img = [
+            img
+            for img in self.image_path.iterdir()
+            if img.suffix.lower() in VALID_IMG_SUFFIX
+        ]
+        return list_of_img
+
+    def make_save_destination(
+        self,
+        save_destination: Union[str, Path, None] = None,
+    ) -> Path:
+        if save_destination is not None:
+            save_folder = Path(save_destination)
+        else:
+            save_folder = self.image_path.with_name(f"{self.image_path.name}_extracted")
+        save_folder.mkdir(exist_ok=True, parents=True)
+        return save_folder
+
+    def ocr(
+        self,
+        save_destination: Union[str, Path, None] = None,
+        preprocess: Literal["thresh", "blur"] = "thresh",
+    ) -> None:
+        """Performs OCR on img dir
+
+        :param save_destination: Folder location, defaults to None
+        :type save_destination: str | Path | None, optional
+        :param preprocess: Preprocess, defaults to "thresh"
+        :type preprocess: Literal[&quot;thresh&quot;, &quot;blur&quot;], optional
+        """
+        save_folder = self.make_save_destination(save_destination)
+        for img in tqdm(
+            self.list_of_img(), desc="Extracting text", unit_scale=True, ncols=88
+        ):
+            ocr_engine = VietOCR_File(img, lang=self.lang)
+            save_path = save_folder.joinpath(img.with_suffix(".txt").name)
+            ocr_engine.ocr(save_destination=save_path, preprocess=preprocess)
+
+    def ocr_multithread(
+        self,
+        n_jobs: int = -1,
+        save_destination: Union[str, Path, None] = None,
+        preprocess: Literal["thresh", "blur"] = "thresh",
+    ) -> None:
+        save_folder = self.make_save_destination(save_destination)
+
+        def _ocr(img: Path):
+            ocr_engine = VietOCR_File(img, lang=self.lang)
+            save_path = save_folder.joinpath(img.with_suffix(".txt").name)
+            ocr_engine.ocr(save_destination=save_path, preprocess=preprocess)
+
+        # Multithread
+        Parallel(n_jobs=n_jobs)(
+            delayed(_ocr)(img)
+            for img in tqdm(
+                self.list_of_img(), desc="Extracting text", unit_scale=True, ncols=88
+            )
+        )
+
+
+class VietOCR:
+    """
+    Vietnamese image OCR
+    """
+
+    def __init__(self, path: Union[str, Path], *, lang: str = "vie") -> None:
+        self.path: Path = Path(path)
+        if not self.path.exists():
+            raise ValueError("Path does not exist")
+        self.lang = lang
+
+        if self.path.is_dir():
+            self.engine = VietOCR_Directory(self.path, lang=self.lang)
+        else:
+            self.engine = VietOCR_File(self.path, lang=self.lang)  # type: ignore
+
+    def ocr(
+        self,
+        save_destination: Union[str, Path, None] = None,
+        preprocess: Literal["thresh", "blur"] = "thresh",
+    ) -> None:
+        try:
+            self.engine.ocr_multithread(
+                save_destination=save_destination, preprocess=preprocess
+            )
+        except Exception:
+            self.engine.ocr(save_destination=save_destination, preprocess=preprocess)
```

### Comparing `vocr-0.2.0/.gitignore` & `vocr-0.2.1/.gitignore`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintainted in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintainted in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
```

### Comparing `vocr-0.2.0/LICENSE` & `vocr-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 AbsoluteWinter
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2024 AbsoluteWinter
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `vocr-0.2.0/PKG-INFO` & `vocr-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocr
-Version: 0.2.0
+Version: 0.2.1
 Summary: Vietnamese OCR
 Project-URL: Homepage, https://github.com/AbsoluteWinter/vocr
 Project-URL: Repository, https://github.com/AbsoluteWinter/vocr
 Project-URL: Issues, https://github.com/AbsoluteWinter/vocr/issues
 Author: AbsoluteWinter
 License: MIT License
 License-File: LICENSE
@@ -26,17 +26,28 @@
 Requires-Dist: pytesseract
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pytest>=7.0.0; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# vocr
- 
-Vietnamese OCR
+# vocr - Vietnamese OCR
+
+
+| | |
+| :---: | :--- |
+| Package Info | ![Supported Python Version](https://img.shields.io/pypi/pyversions/vocr?logo=python) <br> ![PyPI Version](https://img.shields.io/pypi/v/vocr?logo=pypi) ![License](https://img.shields.io/pypi/l/vocr?logo=github&color=blue) <br> ![Download per month](https://img.shields.io/pypi/dm/vocr) |
+| Workflow | ![Test](https://github.com/AbsoluteWinter/vocr/actions/workflows/python-package.yml/badge.svg) <br> ![Release](https://github.com/AbsoluteWinter/vocr/actions/workflows/python-publish.yml/badge.svg) |
+| Repo | ![Repo Size](https://img.shields.io/github/repo-size/AbsoluteWinter/vocr) |
+
+<!-- ![Total Download](https://static.pepy.tech/badge/vocr) -->
+
+
+
+
 
 ## Prerequisite
 
 - [Tesseract](https://github.com/UB-Mannheim/tesseract) installed and added to PATH
 
 
 ## Install
```

