# Comparing `tmp/vjer-32.1.0.tar.gz` & `tmp/vjer-33.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vjer-32.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vjer-33.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vjer-32.1.0.tar` & `vjer-33.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1788 2024-04-12 02:21:43.862315 vjer-32.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2134 2024-04-12 02:21:43.862315 vjer-32.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     5245 2024-04-12 02:21:43.862315 vjer-32.1.0/.gitignore
--rw-r--r--   0        0        0     4999 2024-04-12 02:21:43.862315 vjer-32.1.0/.p4ignore
--rw-r--r--   0        0        0       42 2024-04-12 02:21:43.862315 vjer-32.1.0/.readthedocs.yml
--rw-r--r--   0        0        0    39968 2024-04-12 02:21:43.862315 vjer-32.1.0/CHANGELOG.md
--rw-r--r--   0        0        0       64 2024-04-12 02:21:43.862315 vjer-32.1.0/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2024-04-12 02:21:43.862315 vjer-32.1.0/LICENSE
--rw-r--r--   0        0        0       90 2024-04-12 02:21:43.862315 vjer-32.1.0/MANIFEST.in
--rw-r--r--   0        0        0      973 2024-04-12 02:21:43.862315 vjer-32.1.0/README.md
--rwxr-xr-x   0        0        0      878 2024-04-12 02:21:43.862315 vjer-32.1.0/cicd-support/cicd.sh
--rw-r--r--   0        0        0      634 2024-04-12 02:21:43.862315 vjer-32.1.0/docs/Makefile
--rw-r--r--   0        0        0     9167 2024-04-12 02:21:43.866315 vjer-32.1.0/docs/coding_standards.py
--rw-r--r--   0        0        0     2103 2024-04-12 02:21:43.866315 vjer-32.1.0/docs/conf.py
--rw-r--r--   0        0        0      795 2024-04-12 02:21:43.866315 vjer-32.1.0/docs/make.bat
--rw-r--r--   0        0        0       59 2024-04-12 02:21:43.866315 vjer-32.1.0/docs/modules.rst
--rw-r--r--   0        0        0      229 2024-04-12 02:21:43.866315 vjer-32.1.0/docs/requirements.txt
--rw-r--r--   0        0        0     2180 2024-04-12 02:22:13.610476 vjer-32.1.0/pyproject.toml
--rw-r--r--   0        0        0      305 2024-04-12 02:21:43.866315 vjer-32.1.0/util/New-Env.ps1
--rw-r--r--   0        0        0      259 2024-04-12 02:21:43.866315 vjer-32.1.0/util/Update-Env.ps1
--rw-r--r--   0        0        0      271 2024-04-12 02:21:43.866315 vjer-32.1.0/util/new-env.sh
--rw-r--r--   0        0        0      241 2024-04-12 02:21:43.866315 vjer-32.1.0/util/update-env.sh
--rw-r--r--   0        0        0      476 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer.yml
--rw-r--r--   0        0        0      654 2024-04-12 02:22:13.610476 vjer-32.1.0/vjer/__init__.py
--rw-r--r--   0        0        0      205 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/__main__.py
--rw-r--r--   0        0        0     5208 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/build.py
--rw-r--r--   0        0        0     1185 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/deploy.py
--rw-r--r--   0        0        0     2875 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/freeze.py
--rw-r--r--   0        0        0     1501 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/pre_release.py
--rw-r--r--   0        0        0        0 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/py.typed
--rw-r--r--   0        0        0     3525 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/release.py
--rw-r--r--   0        0        0      769 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/rollback.py
--rw-r--r--   0        0        0     3457 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/test.py
--rw-r--r--   0        0        0     2946 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/tool_reporter.py
--rw-r--r--   0        0        0    24942 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/utils.py
--rwxr-xr-x   0        0        0     2825 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/vjer.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 vjer-32.1.0/setup.py
--rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 vjer-32.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1788 2024-04-18 18:07:15.937749 vjer-33.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2134 2024-04-18 18:07:15.937749 vjer-33.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     5245 2024-04-18 18:07:15.937749 vjer-33.0.0/.gitignore
+-rw-r--r--   0        0        0     4999 2024-04-18 18:07:15.937749 vjer-33.0.0/.p4ignore
+-rw-r--r--   0        0        0       42 2024-04-18 18:07:15.937749 vjer-33.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0    40183 2024-04-18 18:07:15.937749 vjer-33.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       64 2024-04-18 18:07:15.937749 vjer-33.0.0/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2024-04-18 18:07:15.937749 vjer-33.0.0/LICENSE
+-rw-r--r--   0        0        0       90 2024-04-18 18:07:15.937749 vjer-33.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      973 2024-04-18 18:07:15.937749 vjer-33.0.0/README.md
+-rwxr-xr-x   0        0        0      878 2024-04-18 18:07:15.937749 vjer-33.0.0/cicd-support/cicd.sh
+-rw-r--r--   0        0        0      634 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/Makefile
+-rw-r--r--   0        0        0     9167 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/coding_standards.py
+-rw-r--r--   0        0        0     2103 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/conf.py
+-rw-r--r--   0        0        0      795 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/make.bat
+-rw-r--r--   0        0        0       59 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/modules.rst
+-rw-r--r--   0        0        0      229 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2180 2024-04-18 18:07:53.677923 vjer-33.0.0/pyproject.toml
+-rw-r--r--   0        0        0      305 2024-04-18 18:07:15.937749 vjer-33.0.0/util/New-Env.ps1
+-rw-r--r--   0        0        0      259 2024-04-18 18:07:15.937749 vjer-33.0.0/util/Update-Env.ps1
+-rwxr-xr-x   0        0        0      261 2024-04-18 18:07:15.937749 vjer-33.0.0/util/new-env.sh
+-rwxr-xr-x   0        0        0      234 2024-04-18 18:07:15.937749 vjer-33.0.0/util/update-env.sh
+-rw-r--r--   0        0        0      476 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer.yml
+-rw-r--r--   0        0        0      654 2024-04-18 18:07:53.677923 vjer-33.0.0/vjer/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/__main__.py
+-rw-r--r--   0        0        0     5278 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/build.py
+-rw-r--r--   0        0        0     1185 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/deploy.py
+-rw-r--r--   0        0        0     2875 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/freeze.py
+-rw-r--r--   0        0        0     1613 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/pre_release.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/py.typed
+-rw-r--r--   0        0        0     3170 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/release.py
+-rw-r--r--   0        0        0      769 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/rollback.py
+-rw-r--r--   0        0        0     3457 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/test.py
+-rw-r--r--   0        0        0     2946 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/tool_reporter.py
+-rw-r--r--   0        0        0    25691 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/utils.py
+-rwxr-xr-x   0        0        0     2825 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/vjer.py
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 vjer-33.0.0/setup.py
+-rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 vjer-33.0.0/PKG-INFO
```

### Comparing `vjer-32.1.0/.github/workflows/build.yml` & `vjer-33.0.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/.github/workflows/publish.yml` & `vjer-33.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/.gitignore` & `vjer-33.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/.p4ignore` & `vjer-33.0.0/.p4ignore`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/CHANGELOG.md` & `vjer-33.0.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,30 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## Current Release
 
-### [32.1.0] - 2024-04-11
+### [33.0.0] - 2024-04-18
+
+- Added
+  - Added support for multiple Docker tags and Helm versions at build. (GitHub #8)
 
 - Changed
-  - Cleanup version output and add --version option. (GitHub #8)
-  - Fix tagging on release. (GitHub #7)
+  - Required specification of full Docker and Helm repo info in config file.
 
 ## Release History
 
+### [32.1.0] - 2024-04-11
+
+- Changed
+  - Cleanup version output and add --version option. (GitHub #5)
+  - Fix tagging on release. (GitHub #7)
+
 ### [32.0.0] - 2024-04-10
 
 - Added
   - Added flit and bumpver support. (GitHub #2)
 
 - Removed
   - Removed implicit release steps. (GitHub #6)
```

### Comparing `vjer-32.1.0/LICENSE` & `vjer-33.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/README.md` & `vjer-33.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/cicd-support/cicd.sh` & `vjer-33.0.0/cicd-support/cicd.sh`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/docs/Makefile` & `vjer-33.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/docs/coding_standards.py` & `vjer-33.0.0/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/docs/conf.py` & `vjer-33.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/docs/make.bat` & `vjer-33.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/pyproject.toml` & `vjer-33.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "xmlrunner.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "v32.1.0"
+current_version = "v33.0.0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip ci]"
 commit = true
 tag = false
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `vjer-32.1.0/vjer/__init__.py` & `vjer-33.0.0/vjer/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
            '__author__', '__email__',
            '__license__', '__copyright__')
 
 __title__ = 'Vjer'
 __summary__ = 'CI/CD Toolkit'
 __uri__ = 'https://github.com/tardis4500/vjer/'
 
-__version__ = '32.1.0'
+__version__ = '33.0.0'
 __build_name__ = '{var:build_name}'
 __build_date__ = '{var:build_date}'
 
 __author__ = 'Jeffery G. Smith'
 __email__ = 'web@pobox.com'
 
 __license__ = 'MIT'
```

### Comparing `vjer-32.1.0/vjer/build.py` & `vjer-33.0.0/vjer/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,24 +98,25 @@
             if ('stream' in line) and (line['stream'] != '\n'):
                 self.log_message(line['stream'].strip())
         if error:
             raise error
         if push_image:
             self.log_message('Pushing image to registry', True)
             self.registry_client.get_image(self.image_tag).push()
+            if self.step_info.tags:
+                self.tag_images(self.image_tag, [f'{self.image_name}:{t}' for t in self.step_info.tags])
 
     def build_flit(self) -> None:
         """Run a Python flit build."""
         self.flit_build()
 
     def build_helm(self) -> None:
         """Build method for Helm charts."""
         helm('dependency', 'build', self.helm_chart_root)
-        helm('package', self.helm_chart_root)
-        self.copy_artifact(self.helm_package.name)
+        self.helm_build()
 
 
 def build() -> None:
     """This is the main entry point."""
     VjerAction('build', cast(VjerStep, BuildStep)).execute()
 
 # cSpell:ignore batcave fileutil pythonval buildargs vjer
```

### Comparing `vjer-32.1.0/vjer/deploy.py` & `vjer-33.0.0/vjer/deploy.py`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/vjer/freeze.py` & `vjer-33.0.0/vjer/freeze.py`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/vjer/pre_release.py` & `vjer-33.0.0/vjer/pre_release.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module provides pre_release actions."""
 
 # Import standard modules
 from typing import cast
 
 # Import project modules
 from .release import ReleaseStep
-from .utils import VjerAction, VjerStep, helm
+from .utils import VjerAction, VjerStep
 
 
 class PreReleaseStep(ReleaseStep):
     """Provide pre_release support.
 
     Attributes:
         is_pre_release: Specifies to the ReleaseStep parent class that this is a pre_release action.
@@ -25,19 +25,24 @@
         """Perform a bumpver on release."""
         if not self.step_info.args:
             self.step_info.args = {'tag-num': True}
         super().release_bumpver()
 
     def release_helm(self) -> None:
         """Pre_release a Helm chart."""
+        self._release_helm()
+        for version in self.step_info.extra_versions:
+            self.project.version = version
+            self._release_helm()
+
+    def _release_helm(self) -> None:
         if self.helm_repo.type == 'oci':
             self.update_version_files()
             try:
-                helm('package', self.helm_chart_root)
-                self.copy_artifact(self.helm_package.name)
+                self.helm_build()
             finally:
                 self.update_version_files(reset=True)
         else:
             list(self.project.artifacts_dir.glob('*.tgz'))[0].rename(self.helm_package)
         super().release_helm()
```

### Comparing `vjer-32.1.0/vjer/release.py` & `vjer-33.0.0/vjer/release.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """This module provides release actions."""
 
 # Import standard modules
 from typing import cast
 
 # Import third-party modules
-from batcave.cloudmgr import gcloud
 from batcave.sysutil import SysCmdRunner
 
 # Import project modules
 from .utils import helm, VjerAction, VjerStep
 
 bumpver_update = SysCmdRunner('bumpver', 'update', syscmd_args={'ignore_stderr': True}).run
 
@@ -18,39 +17,33 @@
 
     Attributes:
         is_pre_release: Specifies that this is not a pre_release action.
     """
     is_pre_release = False
 
     def _execute(self) -> None:
-        if self.is_pre_release and self.step_info.release_only:
+        if self.step_info.release_only and self.is_pre_release:
             self.log_message('Skipping on pre_release')
             return
+        if self.step_info.pre_release_only and not self.is_pre_release:
+            self.log_message('Skipping on release')
+            return
         super()._execute()
 
     def release_bumpver(self) -> None:
         """Perform a bumpver on release."""
         bumpver_update(**(self.step_info.args if self.step_info.args else {'tag': 'final', 'tag-commit': True}))
 
     def release_docker(self) -> None:
         """Perform a release of a Docker image by tagging."""
         self._docker_init()
-        if (registry := self.container_registry).type not in ('gcp', 'jfrog'):
-            (image := self.registry_client.get_image(self.image_tag)).pull()
         default_tags = [self.version_tag.lower()]
         if not self.is_pre_release:
             default_tags.append(f'{self.image_name}:latest'.lower())
-        for tag in self.step_info.tags if self.step_info.tags else default_tags:
-            self.log_message(f'Tagging image: {tag}')
-            match registry.type:
-                case 'gcp':
-                    gcloud('container', 'images', 'add-tag', self.image_tag, tag, syscmd_args={'ignore_stderr': True})
-                case  _:
-                    image.tag(tag)
-                    image.push()
+        self.tag_images(self.image_tag, self.step_info.tags if self.step_info.tags else default_tags)
 
     def release_flit_build(self) -> None:
         """Run a Python flit build."""
         self.flit_build()
 
     def release_github(self) -> None:
         """Create a GitHub release."""
```

### Comparing `vjer-32.1.0/vjer/rollback.py` & `vjer-33.0.0/vjer/rollback.py`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/vjer/test.py` & `vjer-33.0.0/vjer/test.py`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/vjer/tool_reporter.py` & `vjer-33.0.0/vjer/tool_reporter.py`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/vjer/utils.py` & `vjer-33.0.0/vjer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from stat import S_IWUSR
 from string import Template
 from sys import exit as sys_exit, stderr
 from typing import Callable, cast, Optional
 
 # Import third-party modules
 from batcave.automation import Action
-from batcave.cloudmgr import Cloud, CloudType
+from batcave.cloudmgr import Cloud, CloudType, gcloud
 from batcave.cms import Client, ClientType
 from batcave.expander import Expander, file_expander
 from batcave.lang import BatCaveError, BatCaveException, PathName, DEFAULT_ENCODING, WIN32, yaml_to_dotmap
 from batcave.platarch import Platform
 from batcave.sysutil import CMDError, SysCmdRunner, syscmd
 from bumpver.config import init as bumpver_config
 from dotmap import DotMap
@@ -36,18 +36,17 @@
 
 _CONFIG_SECTIONS = ('project', 'test', 'build', 'deploy', 'rollback', 'release')
 _PROJECT_DEFAULTS = DotMap(build_artifacts='artifacts',
                            build_num_var='VJER_BUILD_NUM',
                            chart_root='helm-chart',
                            container_registry=DotMap(type='local', name=''),
                            dockerfile='Dockerfile',
-                           gcp_artifact_region='us',
                            test_results='test_results',
                            version_service=DotMap(type='vjer'))
-_VALID_SCHEMAS = [2]
+_VALID_SCHEMAS = [3]
 
 PROJECT_CFG_FILE = getenv('VJER_CFG', 'vjer.yml')
 TOOL_REPORT = Path(__file__).parent.absolute() / 'tool_report.yml'
 
 HELM_CHART_FILE = 'Chart.yaml'
 DEFAULT_VERSION_FILES = {'helm': [HELM_CHART_FILE, 'values.yaml']}
 
@@ -265,19 +264,17 @@
                 self._sections[section].update(yaml_as_dict[section])
 
     def _set_defaults(self) -> None:
         self.project.update_defaults(DotMap(artifacts_dir=self.project.project_root / self.project.build_artifacts,
                                             test_results_dir=self.project.project_root / self.project.test_results))
         if hasattr(self.project, 'artifact_repo'):
             if hasattr(self.project, 'docker_repo'):
-                self.project.update_defaults(DotMap(container_registry=DotMap(type='local',
-                                                                              name=f'{self.project.gcp_artifact_region}-docker.pkg.dev/{self.project.artifact_repo}/{self.project.docker_repo}')))
+                self.project.update_defaults(DotMap(container_registry=DotMap(self.project.docker_repo)))
             if hasattr(self.project, 'helm_repo'):
-                self.project.update_defaults(DotMap(chart_repo=DotMap(type='oci',
-                                                                      name=f'oci://{self.project.gcp_artifact_region}-docker.pkg.dev/{self.project.artifact_repo}/{self.project.helm_repo}')))
+                self.project.update_defaults(DotMap(chart_repo=DotMap(self.project.helm_repo)))
 
     def _set_version(self) -> None:
         match self.project.version_service.type:
             case 'bumpver':
                 self.project.version = bumpver_config()[1].pep440_version
             case 'environment':
                 self.project.version = getenv(self.project.version_service.variable, '').rstrip('.')
@@ -354,15 +351,15 @@
         Args:
             login (optional, default=True): If True, login to the Docker image registry.
             mode (optional, default='pull'): The mode for which this initialization will be used.
 
         Returns:
             Nothing.
         """
-        self.registry_client = Cloud(CloudType[self.container_registry.type], login=login)
+        self.registry_client = Cloud(CloudType.gcloud if (self.container_registry.type == 'gcp') else CloudType.local, login=login)
         self.docker_client = Cloud(CloudType.local)
         registry_name_path = f'{self.container_registry.name}/' if login else ''
         self.image_name = f'{registry_name_path}{self.step_info.image if self.step_info.image else self.project.name}'
         self.version_tag = f'{self.image_name}:{self.project.version}'
         self.image_tag = f'{self.version_tag}-{self.build.build_num}'.lower()
 
     def _execute(self) -> None:
@@ -444,14 +441,42 @@
         copytree(str(src), str(use_dest), dirs_exist_ok=True)
 
     def flit_build(self) -> None:
         """Run a Python flit build."""
         flit_builder(Path('pyproject.toml'))
         self.copy_artifact('dist')
 
+    def helm_build(self) -> None:
+        """Build a Helm chart."""
+        helm('package', self.helm_chart_root)
+        self.copy_artifact(self.helm_package.name)
+
+    def tag_images(self, source_tag: str, tags: list[str]) -> None:
+        """Tag Docker images.
+
+        Args:
+            source_Tag: The tag of the existing image to which to add the new tags.
+            tags: The list of tags to add.
+
+        Returns:
+            Nothing.
+        """
+        if (registry := self.container_registry).type not in ('gcp', 'gcp-art'):
+            (image := self.registry_client.get_image(source_tag)).pull()
+        for tag in tags:
+            self.log_message(f'Tagging image: {tag}')
+            match registry.type:
+                case 'gcp':
+                    gcloud('container', 'images', 'add-tag', source_tag, tag, syscmd_args={'ignore_stderr': True})
+                case 'gcp-art':
+                    gcloud('artifacts', 'docker', 'tags', 'add', source_tag, tag, syscmd_args={'ignore_stderr': True})
+                case  _:
+                    image.tag(tag)
+                    image.push()
+
     def tag_source(self, tag: str, label: Optional[str] = None) -> None:
         """Tag the source in Git.
 
         Args:
             tag: The label which which to tag the source.
             label (optional, default=None): The annotation to apply to the tag.
```

### Comparing `vjer-32.1.0/vjer/vjer.py` & `vjer-33.0.0/vjer/vjer.py`

 * *Files identical despite different names*

### Comparing `vjer-32.1.0/setup.py` & `vjer-33.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 extras_require = \
 {'dev': ['flit', 'twine'], 'test': ['types-PyYAML', 'types-requests']}
 
 entry_points = \
 {'console_scripts': ['vjer = vjer.vjer:main']}
 
 setup(name='vjer',
-      version='32.1.0',
+      version='33.0.0',
       description='Vjer CI/CD module.',
       author=None,
       author_email='"Jeffery G. Smith" <web@pobox.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `vjer-32.1.0/PKG-INFO` & `vjer-33.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vjer
-Version: 32.1.0
+Version: 33.0.0
 Summary: Vjer CI/CD module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

