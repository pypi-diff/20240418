# Comparing `tmp/songbirdcli-0.2.0.tar.gz` & `tmp/songbirdcli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songbirdcli-0.2.0.tar", last modified: Tue Apr 16 21:50:07 2024, max compression
+gzip compressed data, was "songbirdcli-0.2.1.tar", last modified: Wed Apr 17 21:16:00 2024, max compression
```

## Comparing `songbirdcli-0.2.0.tar` & `songbirdcli-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:50:07.192374 songbirdcli-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:50:07.184374 songbirdcli-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:50:07.188374 songbirdcli-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-04-16 21:50:07.192374 songbirdcli-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:50:07.192374 songbirdcli-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:50:07.188374 songbirdcli-0.2.0/songbirdcli/
--rw-r--r--   0 runner    (1001) docker     (127)    14631 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/songbirdcli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/songbirdcli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/songbirdcli/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/songbirdcli/requirements.txt.blank
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/songbirdcli/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/songbirdcli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:50:07.188374 songbirdcli-0.2.0/songbirdcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-04-16 21:50:07.000000 songbirdcli-0.2.0/songbirdcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-16 21:50:07.000000 songbirdcli-0.2.0/songbirdcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:50:07.000000 songbirdcli-0.2.0/songbirdcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-16 21:50:07.000000 songbirdcli-0.2.0/songbirdcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 21:50:07.000000 songbirdcli-0.2.0/songbirdcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:50:07.184374 songbirdcli-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:50:07.188374 songbirdcli-0.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-16 21:50:03.000000 songbirdcli-0.2.0/tests/unit/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.485056 songbirdcli-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.489055 songbirdcli-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.github/workflows/pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.489055 songbirdcli-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.489055 songbirdcli-0.2.1/docs/songbirdcli/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/docs/songbirdcli/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/docs/songbirdcli/helpers.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/docs/songbirdcli/settings.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/songbirdcli/
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/requirements.txt.blank
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/songbirdcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-17 21:16:00.000000 songbirdcli-0.2.1/songbirdcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-17 21:16:00.000000 songbirdcli-0.2.1/songbirdcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 21:16:00.000000 songbirdcli-0.2.1/songbirdcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-17 21:16:00.000000 songbirdcli-0.2.1/songbirdcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 21:16:00.000000 songbirdcli-0.2.1/songbirdcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.485056 songbirdcli-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/tests/unit/test_cli.py
```

### Comparing `songbirdcli-0.2.0/.github/workflows/docker.yml` & `songbirdcli-0.2.1/.github/workflows/docker.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-name: Docker Build/Publish Image
+name: docker
 on:
   push:
     branches: [main]
+    tags: '*'
   pull_request:
     branches: [main]
-  release:
-    types: [published]
 jobs:
   build:
     runs-on: ubuntu-22.04
     env:
       DOCKER_REGISTRY: docker.io
       DOCKER_IMAGE: cboin/songbird
       DOCKER_USERNAME: ${{ secrets.DOCKER_USERNAME }}
@@ -22,15 +21,15 @@
       DOCKER_PUSH: false
     steps:
       - uses: actions/checkout@v4
       - name: Get Commit or Tag
         id: vars
         run: |
           tag="${GITHUB_SHA:0:8}"
-          if [ "${GITHUB_EVENT_NAME}" == "release" ]; then
+          if [[ ${GITHUB_REF} == refs/tags* ]]; then
             ref="${GITHUB_REF}"
             tag=$(echo $GITHUB_REF | sed 's/refs\/tags\///g')
           fi
           echo "TAG=$tag" >> $GITHUB_OUTPUT
       - name: Set up Docker Buildx
         uses: docker/setup-buildx-action@v3
       - name: Prepare
@@ -52,14 +51,14 @@
           docker buildx build --platform ${{ steps.prepare.outputs.DOCKER_PLATFORM_AMD64 }},${{ steps.prepare.outputs.DOCKER_PLATFORM_ARM }} \
           --target ${{ steps.prepare.outputs.DOCKER_BUILD_TO_TARGET }} \
           -t ${{ steps.prepare.outputs.DOCKER_IMAGE }}:${{steps.prepare.outputs.VERSION}} \
           -t ${{ steps.prepare.outputs.DOCKER_IMAGE }}:latest \
           --file ./Dockerfile \
           -o type=image,push=false .
       - name: Run Buildx (push image)
-        if: success()  && github.event_name == 'push' || github.event_name == 'release' # trigger a build and push to docker registry
+        if: success() && (github.event_name == 'push' || startsWith(github.ref, 'refs/tags/'))  # only trigger a build and push to docker registry on tag or commit sha off
         run: |
           docker buildx build --platform ${{ steps.prepare.outputs.DOCKER_PLATFORM_AMD64 }},${{ steps.prepare.outputs.DOCKER_PLATFORM_ARM }} \
           --target ${{ steps.prepare.outputs.DOCKER_BUILD_TO_TARGET }} \
           -t ${{ steps.prepare.outputs.DOCKER_IMAGE }}:${{steps.prepare.outputs.VERSION}} \
           -t ${{ steps.prepare.outputs.DOCKER_IMAGE }}:latest \
           --file ./Dockerfile -o type=image,push=true .
```

### Comparing `songbirdcli-0.2.0/.github/workflows/pypi-publish.yaml` & `songbirdcli-0.2.1/.github/workflows/pypi-publish.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 on: push
 
 jobs:
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
-    
+    if: github.ref != 'refs/heads/gh-pages' 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: "3.x"
     - name: Install pypa/build
```

### Comparing `songbirdcli-0.2.0/.github/workflows/tests.yaml` & `songbirdcli-0.2.1/.github/workflows/tests.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: tests
+name: python-tests
 
 on:
   # run tests on all PR's to main.
   pull_request:
     branches: [main]
 
 jobs:
```

### Comparing `songbirdcli-0.2.0/Dockerfile` & `songbirdcli-0.2.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.0/LICENSE` & `songbirdcli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.0/Makefile` & `songbirdcli-0.2.1/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -62,14 +62,30 @@
 update-requirements: env
 	pip uninstall songbirdcore
 	pip freeze --exclude-editable | xargs pip uninstall -y
 	rm $(APP_NAME)/$(REQUIREMENTS_FILE) || true
 	pip install -r $(APP_NAME)/requirements.txt.blank
 	pip freeze --exclude-editable > $(APP_NAME)/$(REQUIREMENTS_FILE)
 
+# documentation targets
+.PHONY: docs-lint
+docs-lint:
+	@echo linting files at docs/**/*.md
+	markdownlint docs/**/*.md
+
+.PHONY: docs-serve
+docs-serve:
+	@echo serving the site on http://localhost:8000
+	mkdocs serve
+
+.PHONY: docs-build
+docs-build:
+	@echo building the site
+	mkdocs build --strict --verbose --site-dir public
+
 .PHONY: build
 build:
 	docker build -t $(APP_NAME):latest .
 
 .PHONY: run-itunes
 run-itunes:
 	docker run -it --env-file docker.env \
```

### Comparing `songbirdcli-0.2.0/PKG-INFO` & `songbirdcli-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: songbirdcli
-Version: 0.2.0
+Version: 0.2.1
 Summary: Songbird's cli.
 Author: Christian Boin
+Project-URL: Documentation, https://cboin1996.github.io/songbird/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: Brotli==1.1.0
 Requires-Dist: cachetools==5.3.3
@@ -43,32 +44,36 @@
 Requires-Dist: pydantic-settings==2.2.1
 Requires-Dist: pydantic_core==2.18.1
 Requires-Dist: pyee==11.1.0
 Requires-Dist: pyparsing==3.1.2
 Requires-Dist: pyquery==2.0.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: requests-htmlc==0.0.4
+Requires-Dist: requests-htmlc==0.0.6
 Requires-Dist: requests-oauthlib==2.0.0
 Requires-Dist: rsa==4.9
-Requires-Dist: songbirdcore==0.0.5
+Requires-Dist: songbirdcore==0.0.7
 Requires-Dist: soupsieve==2.5
 Requires-Dist: toml==0.10.2
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: uritemplate==4.1.1
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: w3lib==2.1.2
 Requires-Dist: websockets==12.0
 Requires-Dist: yt-dlp==2024.4.9
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: click; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mike; extra == "dev"
+Requires-Dist: mkdocstrings-python; extra == "dev"
 Provides-Extra: package
 Requires-Dist: build; extra == "package"
 Requires-Dist: twine; extra == "package"
 
 # songbirdcli 🐦
 
 Music downloading client featuring mp3 or m4a tagging.
@@ -209,14 +214,16 @@
 ```bash
 pip install songbirdcli
 ```
 
 See [tests](./tests/unit/test_cli.py) for an example
 of configuring and running songbirdcli as a package.
 
+For API documentation, view [here](https://cboin1996.github.io/songbird/)
+
 ## Development
 
 To run the application locally, you can use a vscode debugger.
 You should also setup a .env file
 with the parameter `RUN_LOCAL=True`.
 
 ### Requirements
```

### Comparing `songbirdcli-0.2.0/README.md` & `songbirdcli-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,16 @@
 ```bash
 pip install songbirdcli
 ```
 
 See [tests](./tests/unit/test_cli.py) for an example
 of configuring and running songbirdcli as a package.
 
+For API documentation, view [here](https://cboin1996.github.io/songbird/)
+
 ## Development
 
 To run the application locally, you can use a vscode debugger.
 You should also setup a .env file
 with the parameter `RUN_LOCAL=True`.
 
 ### Requirements
```

### Comparing `songbirdcli-0.2.0/songbirdcli/cli.py` & `songbirdcli-0.2.1/songbirdcli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,31 @@
 
 from songbirdcore.models import modes, itunes_api
 from songbirdcore import itunes
 from songbirdcore import youtube
 from songbirdcore import gdrive
 from songbirdcore import common
 
+"""Entrypoint for songbirdcli. Run cli.py as a script to run songbirdcli.
+See the README.md for configuration details.
+"""
+
 logger = logging.getLogger(__name__)
 
 
-def validate_essentials(config: settings.SongbirdCliConfig):
+def validate_essentials(config: settings.SongbirdCliConfig) -> bool:
+    """perform startup validation of the configuration,
+    ensuring pre-conditions are met
+
+    Args:
+        config (settings.SongbirdCliConfig): the songbirdcli pydantic model
+
+    Returns:
+        bool: True if success, False otherwise
+    """
     success = True
     if config.gdrive_enabled:
         if not os.path.exists(config.get_gdrive_folder_path()):
             logger.error(
                 f"You must create the path {config.get_gdrive_folder_path()} \
              to use google drive feature! If using docker, use bind mounts. See README for more info."
             )
@@ -101,15 +114,15 @@
     render_wait: float,
     render_retries: int,
     render_sleep: int,
 ) -> str:
     """Download a song from youtube.
 
     Args:
-        file_name (str): the absolute path of where to save the file
+        file_path_no_format (str): the absolute path of where to save the file (excluding file format)
         youtube_home_url (str): the url to youtube's home page
         youtube_search_url (str): the search url for youtube
         youtube_query_payload (str): the query payload for youtube's search api
         file_format (str): desired file format
         render_timeout (int): amount of time before abandoning a render
         render_wait (float): the amount of time before attempting a render
         render_retries (int): the number of retries for a render
@@ -199,14 +212,15 @@
             return
 
     if song_properties is None:
         song_properties = helpers.parse_itunes_search_api(song_name, modes.Modes.SONG)
 
     if song_properties is None:
         return
+
     file_path_no_format = os.path.join(config.get_local_folder_path(), song_name)
     file_path = file_path_no_format + "." + file_format
     downloaded_file_path = None
     # make sure file doesnt already exist
     duped_filepath = common.fname_duper(file_path, config.fname_dup_limit, 1, "_dup")
     if duped_filepath is None:
         return
@@ -326,14 +340,20 @@
         msg = "Saved locally."
 
     logger.info(msg)
     return True
 
 
 def run(config: settings.SongbirdCliConfig):
+    """main entrypoint for songbirdcli. Expects the songbirdcli config object.
+
+    Args:
+        config (settings.SongbirdCliConfig): songbirdcli settings pydantic model
+
+    """
     try:
         common.set_logger_config_globally(log_level=config.log_level)
         common.name_plate(entries=[f"--cli {config.version}"])
         # only need folders on OS if we are running locally. Otherwise user is expected to provied folders
         # via bind mounts
         if config.run_local:
             initialize_dirs(
```

### Comparing `songbirdcli-0.2.0/songbirdcli/helpers.py` & `songbirdcli-0.2.1/songbirdcli/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 helpers.py module for helping with parsing inputs
 """
 
-from typing import Optional, List
+from typing import Optional, List, Union, Any
 from songbirdcore import common, itunes
 from songbirdcore.models import modes, itunes_api
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def launch_album_mode(artist_album_string=""):
     """
     Args:
         artist_album_string (str): the album/artist to search for.
+
     Returns: the list of song properties gathered from the search.
 
     """
     while True:
         album_props = parse_itunes_search_api(
             search_variable=artist_album_string, mode=modes.Modes.ALBUM, lookup=False
         )
@@ -43,15 +44,27 @@
 
         return songs_in_album_props
 
 
 # entity is usually song for searching songs
 def parse_itunes_search_api(
     search_variable: str, mode: modes.Modes, limit: int = 20, lookup: bool = False
-) -> itunes_api.ItunesApiSongModel:
+) -> Optional[Union[bool, itunes_api.ItunesApiSongModel]]:
+    """perform a query of the items api, allowing user to select
+    an item from the returned list of options
+
+    Args:
+        search_variable (str): the value for the query
+        mode (modes.Modes): the mode to run
+        limit (int, optional): number of results. Defaults to 20.
+        lookup (bool, optional): whether to enable 'lookup' mode in itunes api. Defaults to False.
+
+    Returns:
+        Optional[Union[itunes_api.ItunesApiSongModel]]: returns the selected song properties, an empty list if the user continues without selection, or None if the user quits or an error occurred.
+    """
     parsed_results_list = itunes.query_api(search_variable, limit, mode, lookup=lookup)
 
     # Present results to user
     common.pretty_list_of_basemodel_printer(parsed_results_list)
     logger.info("Searched for: %s" % (search_variable))
     # Only one item can be selected
     user_selection = select_items_from_list(
@@ -63,24 +76,33 @@
 
     # user has quit
     if user_selection is None:
         logger.info("Quitting.")
         return
     if len(user_selection) == 0:
         logger.info("Continuing without properties.")
-        return []
+        return True
 
     print(f"Selected item: ")
     for k, v in user_selection[0].model_dump().items():
         print(" - %s : %s" % (k, v))
 
     return user_selection[0]
 
 
-def remove_songs_selected(song_properties_list):
+def remove_songs_selected(song_properties_list) -> Optional[List]:
+    """Given a list of songs properties, allow the user to remove
+    via stdio
+
+    Args:
+        song_properties_list (Any): the list of song properties
+
+    Returns:
+        Optional[List]: the properties list after selection
+    """
     common.pretty_list_of_basemodel_printer(song_properties_list)
     input_string = "Enter song id's (1 4 5 etc.) you dont want from this album"
     user_input = select_items_from_list(
         input_string,
         song_properties_list,
         n_choices=len(song_properties_list) - 1,
         sep=" ",
@@ -93,25 +115,27 @@
     # user selects all songs
     if user_input == []:
         return song_properties_list
     # otherwise, user gets the processed list with their items removed
     return user_input
 
 
-def get_input(prompt: str, out_type=None, quit_str="q", choices: Optional[List] = None):
+def get_input(
+    prompt: str, out_type=None, quit_str="q", choices: Optional[List] = None
+) -> Optional[Any]:
     """Given a prompt, get input from stdio and perform basic type validation
 
     Args:
         prompt (str): the prompt to use
         out_type (type, optional): expected type for input. Defaults to None.
         quit_str (str, optional): a character to signify quitting from the input gatherer. Defaults to "q".
         choices (Optional[List], optional): valid character options to parse as input. Defaults to None.
 
     Returns:
-        type: the type, or None if quit or invalid type received.
+        Optional[Any]: the typed user input, or None if quit or invalid type received.
     """
     while True:
         built_prompt = prompt
         if choices is not None:
             built_prompt += f" , choices=({choices})"
         built_prompt += " ['q' quits]: "
         inp = input(built_prompt)
@@ -195,15 +219,17 @@
         sep    (str): the separator for the input
         lyst (List): the list to perform input validation against
         n_choices (int): the number of choices allowed
         quit_str (str): The string to cancel validation and exit. Defaults to "q".
         opposite (bool): return everything BUT the user selection
         no_selection_value (any): value to indicate no selection wanted from the user
         return_value (bool): if true, return the value, otherwise return the indicies of selections
-    Returns Optiona[List]: None if user quits, [] if user selects nothing, otherwise a list of the users selections are returned.
+
+    Returns:
+        Optiona[List]: None if user quits, [] if user selects nothing, otherwise a list of the users selections are returned.
     """
     tries = 0
     low = 0
     high = len(lyst) - 1
     # provide useful ranges to user
     if high == -1:
         range_display = ""
```

### Comparing `songbirdcli-0.2.0/songbirdcli/requirements.txt` & `songbirdcli-0.2.1/songbirdcli/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 pydantic-settings==2.2.1
 pydantic_core==2.18.1
 pyee==11.1.0
 pyparsing==3.1.2
 pyquery==2.0.0
 python-dotenv==1.0.1
 requests==2.31.0
-requests-htmlc==0.0.4
+requests-htmlc==0.0.6
 requests-oauthlib==2.0.0
 rsa==4.9
-songbirdcore==0.0.5
+songbirdcore==0.0.7
 soupsieve==2.5
 toml==0.10.2
 typing_extensions==4.11.0
 uritemplate==4.1.1
 urllib3==2.2.1
 w3lib==2.1.2
 websockets==12.0
```

### Comparing `songbirdcli-0.2.0/songbirdcli/settings.py` & `songbirdcli-0.2.1/songbirdcli/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,26 +60,26 @@
 
     def get_data_path(self):
         return os.path.join(self.root_path, self.data_path)
 
     def get_local_folder_path(self):
         return os.path.join(self.get_data_path(), self.local_song_store_str)
 
-    def get_itunes_folder_path(self):
+    def get_itunes_folder_path(self) -> str:
         """If you run the app locally, configure the itunes path as an absolute path. Otherwise, the program will
         use the local container storage and assume to be running in a docker container.
 
         Returns:
             str: the path to where itunes destined songs should live
         """
         if self.run_local:
             return self.itunes_folder_path
         return os.path.join(self.get_data_path(), self.itunes_folder_path)
 
-    def get_itunes_lib_path(self):
+    def get_itunes_lib_path(self) -> str:
         """If you run the app locally, configure the itunes path as an absolute path. Otherwise, the program will
         use the local container storage and assume to be running in a docker container.
 
         Returns:
             str: the path to where itunes destined songs should live
         """
         if self.run_local:
```

### Comparing `songbirdcli-0.2.0/songbirdcli.egg-info/PKG-INFO` & `songbirdcli-0.2.1/songbirdcli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: songbirdcli
-Version: 0.2.0
+Version: 0.2.1
 Summary: Songbird's cli.
 Author: Christian Boin
+Project-URL: Documentation, https://cboin1996.github.io/songbird/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: Brotli==1.1.0
 Requires-Dist: cachetools==5.3.3
@@ -43,32 +44,36 @@
 Requires-Dist: pydantic-settings==2.2.1
 Requires-Dist: pydantic_core==2.18.1
 Requires-Dist: pyee==11.1.0
 Requires-Dist: pyparsing==3.1.2
 Requires-Dist: pyquery==2.0.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: requests-htmlc==0.0.4
+Requires-Dist: requests-htmlc==0.0.6
 Requires-Dist: requests-oauthlib==2.0.0
 Requires-Dist: rsa==4.9
-Requires-Dist: songbirdcore==0.0.5
+Requires-Dist: songbirdcore==0.0.7
 Requires-Dist: soupsieve==2.5
 Requires-Dist: toml==0.10.2
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: uritemplate==4.1.1
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: w3lib==2.1.2
 Requires-Dist: websockets==12.0
 Requires-Dist: yt-dlp==2024.4.9
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: click; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mike; extra == "dev"
+Requires-Dist: mkdocstrings-python; extra == "dev"
 Provides-Extra: package
 Requires-Dist: build; extra == "package"
 Requires-Dist: twine; extra == "package"
 
 # songbirdcli 🐦
 
 Music downloading client featuring mp3 or m4a tagging.
@@ -209,14 +214,16 @@
 ```bash
 pip install songbirdcli
 ```
 
 See [tests](./tests/unit/test_cli.py) for an example
 of configuring and running songbirdcli as a package.
 
+For API documentation, view [here](https://cboin1996.github.io/songbird/)
+
 ## Development
 
 To run the application locally, you can use a vscode debugger.
 You should also setup a .env file
 with the parameter `RUN_LOCAL=True`.
 
 ### Requirements
```

### Comparing `songbirdcli-0.2.0/songbirdcli.egg-info/SOURCES.txt` & `songbirdcli-0.2.1/songbirdcli.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 .dockerignore
 .gitignore
 Dockerfile
 LICENSE
 Makefile
 README.md
+markdownlint.yaml
+mkdocs.yml
 pyproject.toml
 .github/workflows/docker.yml
+.github/workflows/pages.yaml
 .github/workflows/pypi-publish.yaml
 .github/workflows/style.yml
 .github/workflows/tests.yaml
+docs/index.md
+docs/songbirdcli/cli.md
+docs/songbirdcli/helpers.md
+docs/songbirdcli/settings.md
 songbirdcli/cli.py
 songbirdcli/helpers.py
 songbirdcli/requirements.txt
 songbirdcli/requirements.txt.blank
 songbirdcli/settings.py
 songbirdcli/version.py
 songbirdcli.egg-info/PKG-INFO
```

### Comparing `songbirdcli-0.2.0/tests/unit/test_cli.py` & `songbirdcli-0.2.1/tests/unit/test_cli.py`

 * *Files identical despite different names*

