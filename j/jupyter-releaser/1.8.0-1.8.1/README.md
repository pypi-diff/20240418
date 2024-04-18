# Comparing `tmp/jupyter_releaser-1.8.0.tar.gz` & `tmp/jupyter_releaser-1.8.1.tar.gz`

## Comparing `jupyter_releaser-1.8.0.tar` & `jupyter_releaser-1.8.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.readthedocs.yml
--rw-r--r--   0        0        0   138805 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/RELEASE.md
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/actions/check-release/action.yml
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/actions/finalize-release/action.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/actions/install-releaser/action.yml
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/actions/populate-release/action.yml
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/actions/prep-release/action.yml
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/actions/publish-changelog/action.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/scripts/bump_tag.sh
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/scripts/install-releaser.sh
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/workflows/generate-changelog.yml
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/workflows/prep-self-release.yml
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/workflows/publish-changelog.yml
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/workflows/publish-self-release.yml
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/make.bat
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/conf.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/index.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/_static/custom.css
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/_static/images/logo/favicon.svg
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/_static/images/logo/logo.svg
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/background/index.rst
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/background/theory.md
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/get_started/generate_changelog.md
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/get_started/index.rst
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/get_started/making_release_from_releaser.md
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/get_started/making_release_from_repo.md
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/how_to_guides/convert_repo_from_releaser.md
--rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/how_to_guides/convert_repo_from_repo.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/how_to_guides/index.rst
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/how_to_guides/maintain_fork.md
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/how_to_guides/write_config.md
--rw-r--r--   0        0        0   507289 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/images/draft_github_release.png
--rw-r--r--   0        0        0   586032 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/images/final_github_release.png
--rw-r--r--   0        0        0   169812 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/images/fork_fetch.png
--rw-r--r--   0        0        0   276246 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/images/generate_changelog.png
--rw-r--r--   0        0        0    39051 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/images/prep_release.png
--rw-r--r--   0        0        0   212895 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/images/prep_release_next_step.png
--rw-r--r--   0        0        0    35251 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/images/prep_release_repo.png
--rw-r--r--   0        0        0    74988 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/images/publish_release.png
--rw-r--r--   0        0        0   177023 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/images/publish_release_next_step.png
--rw-r--r--   0        0        0   191024 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/images/publish_release_repo.png
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/reference/api_docs.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/reference/configuration.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/reference/faq.md
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/reference/index.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/docs/source/reference/releaser_cli.rst
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/example-workflows/full-release.yml
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/example-workflows/prep-release.yml
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/example-workflows/publish-changelog.yml
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/example-workflows/publish-release.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/__main__.py
--rw-r--r--   0        0        0    13172 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/changelog.py
--rw-r--r--   0        0        0    20884 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/cli.py
--rw-r--r--   0        0        0    21689 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/lib.py
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/mock_github.py
--rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/npm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/py.typed
--rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/python.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/schema.json
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/tee.py
--rw-r--r--   0        0        0    24794 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/actions/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/actions/common.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/actions/finalize_release.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/actions/generate_changelog.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/actions/populate_release.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/actions/prep_release.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/jupyter_releaser/actions/publish_changelog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/tests/__init__.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/tests/conftest.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/tests/test_changelog.py
--rw-r--r--   0        0        0    28051 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/tests/test_cli.py
--rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/tests/test_functions.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/tests/test_mock_github.py
--rw-r--r--   0        0        0     9625 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/tests/util.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/.gitignore
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/LICENSE
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/README.md
--rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.readthedocs.yml
+-rw-r--r--   0        0        0   139924 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/RELEASE.md
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/actions/check-release/action.yml
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/actions/finalize-release/action.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/actions/install-releaser/action.yml
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/actions/populate-release/action.yml
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/actions/prep-release/action.yml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/actions/publish-changelog/action.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/scripts/bump_tag.sh
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/scripts/install-releaser.sh
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/workflows/generate-changelog.yml
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/workflows/prep-self-release.yml
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/workflows/publish-changelog.yml
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/workflows/publish-self-release.yml
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/make.bat
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/conf.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/index.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/_static/custom.css
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/_static/images/logo/favicon.svg
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/_static/images/logo/logo.svg
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/background/index.rst
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/background/theory.md
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/get_started/generate_changelog.md
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/get_started/index.rst
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/get_started/making_release_from_releaser.md
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/get_started/making_release_from_repo.md
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/how_to_guides/convert_repo_from_releaser.md
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/how_to_guides/convert_repo_from_repo.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/how_to_guides/index.rst
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/how_to_guides/maintain_fork.md
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/how_to_guides/write_config.md
+-rw-r--r--   0        0        0   507289 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/images/draft_github_release.png
+-rw-r--r--   0        0        0   586032 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/images/final_github_release.png
+-rw-r--r--   0        0        0   169812 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/images/fork_fetch.png
+-rw-r--r--   0        0        0   276246 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/images/generate_changelog.png
+-rw-r--r--   0        0        0    39051 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/images/prep_release.png
+-rw-r--r--   0        0        0   212895 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/images/prep_release_next_step.png
+-rw-r--r--   0        0        0    35251 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/images/prep_release_repo.png
+-rw-r--r--   0        0        0    74988 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/images/publish_release.png
+-rw-r--r--   0        0        0   177023 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/images/publish_release_next_step.png
+-rw-r--r--   0        0        0   191024 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/images/publish_release_repo.png
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/reference/api_docs.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/reference/configuration.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/reference/faq.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/reference/index.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/docs/source/reference/releaser_cli.rst
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/example-workflows/full-release.yml
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/example-workflows/prep-release.yml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/example-workflows/publish-changelog.yml
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/example-workflows/publish-release.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/__init__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/__main__.py
+-rw-r--r--   0        0        0    13172 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/changelog.py
+-rw-r--r--   0        0        0    20884 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/cli.py
+-rw-r--r--   0        0        0    21787 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/lib.py
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/mock_github.py
+-rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/npm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/py.typed
+-rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/python.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/schema.json
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/tee.py
+-rw-r--r--   0        0        0    24794 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/actions/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/actions/common.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/actions/finalize_release.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/actions/generate_changelog.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/actions/populate_release.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/actions/prep_release.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/jupyter_releaser/actions/publish_changelog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/tests/__init__.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/tests/conftest.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/tests/test_changelog.py
+-rw-r--r--   0        0        0    28051 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/tests/test_cli.py
+-rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/tests/test_functions.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/tests/test_mock_github.py
+-rw-r--r--   0        0        0     9625 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/tests/util.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/.gitignore
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/LICENSE
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/README.md
+-rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 jupyter_releaser-1.8.1/PKG-INFO
```

### Comparing `jupyter_releaser-1.8.0/.pre-commit-config.yaml` & `jupyter_releaser-1.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/CHANGELOG.md` & `jupyter_releaser-1.8.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.8.1
+
+([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...ba6e1a5170e41cc76e14d9ab77bb16b0d8fe6cda))
+
+### Bugs fixed
+
+- Normalise package name before comparison [#568](https://github.com/jupyter-server/jupyter_releaser/pull/568) ([@krassowski](https://github.com/krassowski))
+
+### Maintenance and upkeep improvements
+
+- Revert "Set all min deps" [#566](https://github.com/jupyter-server/jupyter_releaser/pull/566) ([@blink1073](https://github.com/blink1073))
+- Set all min deps [#565](https://github.com/jupyter-server/jupyter_releaser/pull/565) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_releaser/graphs/contributors?from=2024-03-25&to=2024-04-18&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Ablink1073+updated%3A2024-03-25..2024-04-18&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Akrassowski+updated%3A2024-03-25..2024-04-18&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.8.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...fcf07a4695f124af2d61817a9cfb3b38bcdef3f6))
 
 ### Bugs fixed
 
 - Print out error for npm upload [#564](https://github.com/jupyter-server/jupyter_releaser/pull/564) ([@krassowski](https://github.com/krassowski))
@@ -21,16 +42,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_releaser/graphs/contributors?from=2024-03-04&to=2024-03-25&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Ablink1073+updated%3A2024-03-04..2024-03-25&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Akrassowski+updated%3A2024-03-04..2024-03-25&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.7.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...a349a2057b04cf9e83a4df97fa7c13cd4f2a755d))
 
 ### Enhancements made
 
 - Add ability to disable admin user check via flag [#559](https://github.com/jupyter-server/jupyter_releaser/pull/559) ([@ElioDiNino](https://github.com/ElioDiNino))
```

### Comparing `jupyter_releaser-1.8.0/CONTRIBUTING.md` & `jupyter_releaser-1.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/actions/check-release/action.yml` & `jupyter_releaser-1.8.1/.github/actions/check-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/actions/finalize-release/action.yml` & `jupyter_releaser-1.8.1/.github/actions/finalize-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/actions/populate-release/action.yml` & `jupyter_releaser-1.8.1/.github/actions/populate-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/actions/prep-release/action.yml` & `jupyter_releaser-1.8.1/.github/actions/prep-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/actions/publish-changelog/action.yml` & `jupyter_releaser-1.8.1/.github/actions/publish-changelog/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/workflows/check-release.yml` & `jupyter_releaser-1.8.1/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/workflows/generate-changelog.yml` & `jupyter_releaser-1.8.1/.github/workflows/generate-changelog.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/workflows/prep-release.yml` & `jupyter_releaser-1.8.1/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/workflows/prep-self-release.yml` & `jupyter_releaser-1.8.1/.github/workflows/prep-self-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/workflows/publish-changelog.yml` & `jupyter_releaser-1.8.1/.github/workflows/publish-changelog.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/workflows/publish-release.yml` & `jupyter_releaser-1.8.1/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/workflows/publish-self-release.yml` & `jupyter_releaser-1.8.1/.github/workflows/publish-self-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.github/workflows/test.yml` & `jupyter_releaser-1.8.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/Makefile` & `jupyter_releaser-1.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/make.bat` & `jupyter_releaser-1.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/conf.py` & `jupyter_releaser-1.8.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/_static/images/logo/favicon.svg` & `jupyter_releaser-1.8.1/docs/source/_static/images/logo/favicon.svg`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/_static/images/logo/logo.svg` & `jupyter_releaser-1.8.1/docs/source/_static/images/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/background/theory.md` & `jupyter_releaser-1.8.1/docs/source/background/theory.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/get_started/generate_changelog.md` & `jupyter_releaser-1.8.1/docs/source/get_started/generate_changelog.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/get_started/making_release_from_releaser.md` & `jupyter_releaser-1.8.1/docs/source/get_started/making_release_from_releaser.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/get_started/making_release_from_repo.md` & `jupyter_releaser-1.8.1/docs/source/get_started/making_release_from_repo.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/how_to_guides/convert_repo_from_releaser.md` & `jupyter_releaser-1.8.1/docs/source/how_to_guides/convert_repo_from_releaser.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/how_to_guides/convert_repo_from_repo.md` & `jupyter_releaser-1.8.1/docs/source/how_to_guides/convert_repo_from_repo.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/how_to_guides/write_config.md` & `jupyter_releaser-1.8.1/docs/source/how_to_guides/write_config.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/images/draft_github_release.png` & `jupyter_releaser-1.8.1/docs/source/images/draft_github_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/images/final_github_release.png` & `jupyter_releaser-1.8.1/docs/source/images/final_github_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/images/fork_fetch.png` & `jupyter_releaser-1.8.1/docs/source/images/fork_fetch.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/images/generate_changelog.png` & `jupyter_releaser-1.8.1/docs/source/images/generate_changelog.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/images/prep_release.png` & `jupyter_releaser-1.8.1/docs/source/images/prep_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/images/prep_release_next_step.png` & `jupyter_releaser-1.8.1/docs/source/images/prep_release_next_step.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/images/prep_release_repo.png` & `jupyter_releaser-1.8.1/docs/source/images/prep_release_repo.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/images/publish_release.png` & `jupyter_releaser-1.8.1/docs/source/images/publish_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/images/publish_release_next_step.png` & `jupyter_releaser-1.8.1/docs/source/images/publish_release_next_step.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/images/publish_release_repo.png` & `jupyter_releaser-1.8.1/docs/source/images/publish_release_repo.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/reference/api_docs.rst` & `jupyter_releaser-1.8.1/docs/source/reference/api_docs.rst`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/docs/source/reference/faq.md` & `jupyter_releaser-1.8.1/docs/source/reference/faq.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/example-workflows/full-release.yml` & `jupyter_releaser-1.8.1/example-workflows/full-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/example-workflows/prep-release.yml` & `jupyter_releaser-1.8.1/example-workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/example-workflows/publish-changelog.yml` & `jupyter_releaser-1.8.1/example-workflows/publish-changelog.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/example-workflows/publish-release.yml` & `jupyter_releaser-1.8.1/example-workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/changelog.py` & `jupyter_releaser-1.8.1/jupyter_releaser/changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/cli.py` & `jupyter_releaser-1.8.1/jupyter_releaser/cli.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/lib.py` & `jupyter_releaser-1.8.1/jupyter_releaser/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from datetime import datetime, timezone
 from glob import glob
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import Type, Union
 
 import mdformat
+from packaging.utils import canonicalize_name
 from packaging.version import parse as parse_version
 from pkginfo import SDist, Wheel
 
 from jupyter_releaser import changelog, npm, python, util
 
 
 def bump_version(version_spec, version_cmd, changelog_path, tag_format):
@@ -392,15 +393,15 @@
             warnings.warn(
                 f"The NPM tag '{npm_tag}' will be ignored as at tag option is set in NPM command; '{npm_cmd}'.",
                 stacklevel=2,
             )
 
     res = python_package.split(":")
     python_package_path = res[0]
-    python_package_name = res[1].replace("-", "_") if len(res) == 2 else ""
+    python_package_name = canonicalize_name(res[1]) if len(res) == 2 else ""
 
     if release_url and len(glob(f"{dist_dir}/*.whl")):
         twine_token = python.get_pypi_token(release_url, python_package_path)
 
         if twine_token:
             # tell GitHub Actions to mask the token in any console logs,
             # to avoid leaking it
@@ -423,24 +424,25 @@
         name = Path(path).name
         util.log(f"Handling dist file {path}")
         suffix = Path(path).suffix
         if suffix in [".gz", ".whl"]:
             dist: Union[Type[SDist], Type[Wheel]]
             dist = SDist if suffix == ".gz" else Wheel
             pkg = dist(path)
-            if not python_package_name or python_package_name == pkg.name:
+            pkg_name = canonicalize_name(pkg.name)
+            if not python_package_name or python_package_name == pkg_name:
                 env = os.environ.copy()
                 env["TWINE_PASSWORD"] = twine_token
                 # NOTE: Do not print the env since a twine token extracted from
                 # a PYPI_TOKEN_MAP will not be sanitized in output
                 util.retry(f"{twine_cmd} {name}", cwd=dist_dir, env=env, echo=True)
                 found = True
             else:
                 warnings.warn(
-                    f"Python package name {pkg.name} does not match with name in "
+                    f"Python package name {pkg_name} does not match with name in "
                     f"jupyter releaser config: {python_package_name}. Skipping uploading dist file {path}",
                     stacklevel=2,
                 )
         elif suffix == ".tgz":
             # Ignore already published versions
             try:
                 util.run(f"{npm_cmd} {name}", cwd=dist_dir, quiet=True, quiet_error=True, echo=True)
```

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/mock_github.py` & `jupyter_releaser-1.8.1/jupyter_releaser/mock_github.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/npm.py` & `jupyter_releaser-1.8.1/jupyter_releaser/npm.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/python.py` & `jupyter_releaser-1.8.1/jupyter_releaser/python.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/schema.json` & `jupyter_releaser-1.8.1/jupyter_releaser/schema.json`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/tee.py` & `jupyter_releaser-1.8.1/jupyter_releaser/tee.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/util.py` & `jupyter_releaser-1.8.1/jupyter_releaser/util.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/actions/common.py` & `jupyter_releaser-1.8.1/jupyter_releaser/actions/common.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/actions/generate_changelog.py` & `jupyter_releaser-1.8.1/jupyter_releaser/actions/generate_changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/actions/populate_release.py` & `jupyter_releaser-1.8.1/jupyter_releaser/actions/populate_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/actions/prep_release.py` & `jupyter_releaser-1.8.1/jupyter_releaser/actions/prep_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/jupyter_releaser/actions/publish_changelog.py` & `jupyter_releaser-1.8.1/jupyter_releaser/actions/publish_changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/tests/conftest.py` & `jupyter_releaser-1.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/tests/test_changelog.py` & `jupyter_releaser-1.8.1/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/tests/test_cli.py` & `jupyter_releaser-1.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/tests/test_functions.py` & `jupyter_releaser-1.8.1/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/tests/test_mock_github.py` & `jupyter_releaser-1.8.1/tests/test_mock_github.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/tests/util.py` & `jupyter_releaser-1.8.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/.gitignore` & `jupyter_releaser-1.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/LICENSE` & `jupyter_releaser-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/README.md` & `jupyter_releaser-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/pyproject.toml` & `jupyter_releaser-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.8.0/PKG-INFO` & `jupyter_releaser-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter_releaser
-Version: 1.8.0
+Version: 1.8.1
 Summary: Jupyter Releaser for Python and/or npm packages.
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: Copyright (c) 2021 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

