# Comparing `tmp/go_task_bin-3.35.1.tar.gz` & `tmp/go_task_bin-3.36.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go_task_bin-3.35.1.tar", last modified: Sun Mar 10 14:08:42 2024, max compression
+gzip compressed data, was "go_task_bin-3.36.0.tar", last modified: Thu Apr 18 05:27:35 2024, max compression
```

## Comparing `go_task_bin-3.35.1.tar` & `go_task_bin-3.36.0.tar`

### file list

```diff
@@ -1,592 +1,408 @@
--rw-r--r--   0        0        0     1074 2024-03-10 14:06:44.975322 go_task_bin-3.35.1/LICENSE
--rw-r--r--   0        0        0     1031 2024-03-10 14:06:44.975322 go_task_bin-3.35.1/README.md
--rw-r--r--   0        0        0        0 2024-03-10 14:06:44.975322 go_task_bin-3.35.1/go_task_bin/__init__.py
--rw-r--r--   0        0        0     1051 2024-03-10 14:06:44.975322 go_task_bin-3.35.1/pdm_build.py
--rw-r--r--   0        0        0     1198 2024-03-10 14:08:42.144477 go_task_bin-3.35.1/pyproject.toml
--rw-r--r--   0        0        0      231 2024-03-10 14:06:46.603338 go_task_bin-3.35.1/task/.editorconfig
--rw-r--r--   0        0        0       37 2024-03-10 14:06:46.595338 go_task_bin-3.35.1/task/.git
--rw-r--r--   0        0        0       12 2024-03-10 14:06:46.603338 go_task_bin-3.35.1/task/.gitattributes
--rw-r--r--   0        0        0     3217 2024-03-10 14:06:46.603338 go_task_bin-3.35.1/task/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      521 2024-03-10 14:06:46.603338 go_task_bin-3.35.1/task/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       88 2024-03-10 14:06:46.603338 go_task_bin-3.35.1/task/.github/FUNDING.yml
--rw-r--r--   0        0        0      387 2024-03-10 14:06:46.603338 go_task_bin-3.35.1/task/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      552 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      368 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      462 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/dependabot.yml
--rw-r--r--   0        0        0      225 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/pull_request_template.md
--rw-r--r--   0        0        0     1463 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/workflows/issue-awaiting-response.yml
--rw-r--r--   0        0        0      838 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/workflows/issue-closed.yml
--rw-r--r--   0        0        0     6565 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/workflows/issue-experiment.yml
--rw-r--r--   0        0        0      813 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/workflows/issue-needs-triage.yml
--rw-r--r--   0        0        0      862 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/workflows/lint.yml
--rw-r--r--   0        0        0      476 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/workflows/release.yml
--rw-r--r--   0        0        0      989 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/workflows/sync-translated-documents.yml
--rw-r--r--   0        0        0      872 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/workflows/test.yml
--rw-r--r--   0        0        0      907 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.github/workflows/upload-source-documents.yml
--rw-r--r--   0        0        0      445 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.gitignore
--rw-r--r--   0        0        0      387 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.golangci.yml
--rw-r--r--   0        0        0     3037 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.goreleaser.yml
--rw-r--r--   0        0        0       77 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.mockery.yaml
--rw-r--r--   0        0        0        8 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.nvmrc
--rw-r--r--   0        0        0      125 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.prettierrc.yml
--rw-r--r--   0        0        0       76 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/.vscode/settings-sample.json
--rw-r--r--   0        0        0    36819 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/CHANGELOG.md
--rw-r--r--   0        0        0     1080 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/LICENSE
--rw-r--r--   0        0        0      631 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/README.md
--rw-r--r--   0        0        0     2930 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/Taskfile.yml
--rw-r--r--   0        0        0      586 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/args/args.go
--rw-r--r--   0        0        0     2393 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/args/args_test.go
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/bin/.keep
--rw-r--r--   0        0        0     2939 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/cmd/release/main.go
--rw-r--r--   0        0        0     4874 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/cmd/sleepit/sleepit.go
--rw-r--r--   0        0        0     4584 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/cmd/task/task.go
--rw-r--r--   0        0        0     1329 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/completion/bash/task.bash
--rw-r--r--   0        0        0     2342 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/completion/fish/task.fish
--rw-r--r--   0        0        0     1992 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/completion/ps/task.ps1
--rwxr-xr-x   0        0        0     2431 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/completion/zsh/_task
--rw-r--r--   0        0        0      436 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/concurrency.go
--rw-r--r--   0        0        0      233 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/.gitignore
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/.nojekyll
--rw-r--r--   0        0        0     1470 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/Taskfile.yml
--rw-r--r--   0        0        0       70 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/babel.config.ts
--rw-r--r--   0        0        0     6842 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/blog/2023-09-02-introducing-experiments.md
--rw-r--r--   0        0        0      279 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/blog/authors.yml
--rw-r--r--   0        0        0      242 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/constants.ts
--rw-r--r--   0        0        0      440 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/crowdin.yml
--rw-r--r--   0        0        0    41112 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/api_reference.md
--rw-r--r--   0        0        0    36867 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/changelog.md
--rw-r--r--   0        0        0     1529 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/community.md
--rw-r--r--   0        0        0     7797 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/contributing.md
--rw-r--r--   0        0        0      711 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/deprecations/deprecations.md
--rw-r--r--   0        0        0      655 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/deprecations/template.md
--rw-r--r--   0        0        0     1247 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/deprecations/version_2_schema.md
--rw-r--r--   0        0        0     1914 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/donate.md
--rw-r--r--   0        0        0     8039 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/experiments/any_variables.mdx
--rw-r--r--   0        0        0     5677 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/experiments/experiments.md
--rw-r--r--   0        0        0     1531 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/experiments/gentle_force.md
--rw-r--r--   0        0        0     4253 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/experiments/remote_taskfiles.md
--rw-r--r--   0        0        0     1126 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/experiments/template.md
--rw-r--r--   0        0        0     2585 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/faq.md
--rw-r--r--   0        0        0     6923 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/installation.md
--rw-r--r--   0        0        0     2908 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/integrations.md
--rw-r--r--   0        0        0     1978 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/intro.md
--rw-r--r--   0        0        0     2799 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/releasing.md
--rw-r--r--   0        0        0     2974 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/styleguide.md
--rw-r--r--   0        0        0     5456 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/taskfile_versions.md
--rw-r--r--   0        0        0      765 2024-03-10 14:06:46.607338 go_task_bin-3.35.1/task/docs/docs/translate.md
--rw-r--r--   0        0        0    44548 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/docs/usage.md
--rw-r--r--   0        0        0     6280 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/docusaurus.config.ts
--rw-r--r--   0        0        0    16509 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/en/code.json
--rw-r--r--   0        0        0      103 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/en/docusaurus-plugin-content-docs/current.json
--rw-r--r--   0        0        0     1779 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/en/docusaurus-theme-classic/footer.json
--rw-r--r--   0        0        0      955 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/en/docusaurus-theme-classic/navbar.json
--rw-r--r--   0        0        0    16913 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/code.json
--rw-r--r--   0        0        0     6850 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-blog/2023-09-02-introducing-experiments.md
--rw-r--r--   0        0        0      279 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-blog/authors.yml
--rw-r--r--   0        0        0      108 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current.json
--rw-r--r--   0        0        0    41457 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/api_reference.md
--rw-r--r--   0        0        0    33739 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/changelog.md
--rw-r--r--   0        0        0     1529 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/community.md
--rw-r--r--   0        0        0     7750 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/contributing.md
--rw-r--r--   0        0        0      711 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/deprecations/deprecations.md
--rw-r--r--   0        0        0      651 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/deprecations/template.md
--rw-r--r--   0        0        0     1248 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/deprecations/version_2_schema.md
--rw-r--r--   0        0        0     1921 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/donate.md
--rw-r--r--   0        0        0     4191 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/any_variables.md
--rw-r--r--   0        0        0     3184 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/any_variables.mdx
--rw-r--r--   0        0        0     5521 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/experiments.md
--rw-r--r--   0        0        0     1532 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/gentle_force.md
--rw-r--r--   0        0        0     4218 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/remote_taskfiles.md
--rw-r--r--   0        0        0     1123 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/template.md
--rw-r--r--   0        0        0     3777 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/workflow.md
--rw-r--r--   0        0        0     2581 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/faq.md
--rw-r--r--   0        0        0     6886 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/installation.md
--rw-r--r--   0        0        0     2944 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/integrations.md
--rw-r--r--   0        0        0     1963 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/intro.md
--rw-r--r--   0        0        0     2798 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/releasing.md
--rw-r--r--   0        0        0     2875 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/styleguide.md
--rw-r--r--   0        0        0     5441 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/taskfile_versions.md
--rw-r--r--   0        0        0      766 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/translate.md
--rw-r--r--   0        0        0    42065 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/usage.md
--rw-r--r--   0        0        0     1779 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-theme-classic/footer.json
--rw-r--r--   0        0        0      961 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-theme-classic/navbar.json
--rw-r--r--   0        0        0    17144 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/code.json
--rw-r--r--   0        0        0     6850 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-blog/2023-09-02-introducing-experiments.md
--rw-r--r--   0        0        0      279 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-blog/authors.yml
--rw-r--r--   0        0        0      106 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current.json
--rw-r--r--   0        0        0    41455 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/api_reference.md
--rw-r--r--   0        0        0    33739 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/changelog.md
--rw-r--r--   0        0        0     1675 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/community.md
--rw-r--r--   0        0        0     7750 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/contributing.md
--rw-r--r--   0        0        0      828 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/deprecations/deprecations.md
--rw-r--r--   0        0        0      651 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/deprecations/template.md
--rw-r--r--   0        0        0     1248 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/deprecations/version_2_schema.md
--rw-r--r--   0        0        0     2124 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/donate.md
--rw-r--r--   0        0        0     4191 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/experiments/any_variables.md
--rw-r--r--   0        0        0     3184 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/experiments/any_variables.mdx
--rw-r--r--   0        0        0     5910 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/experiments/experiments.md
--rw-r--r--   0        0        0     1532 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/experiments/gentle_force.md
--rw-r--r--   0        0        0     4218 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/experiments/remote_taskfiles.md
--rw-r--r--   0        0        0     1123 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/experiments/template.md
--rw-r--r--   0        0        0     3777 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/experiments/workflow.md
--rw-r--r--   0        0        0     2594 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/faq.md
--rw-r--r--   0        0        0     6886 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/installation.md
--rw-r--r--   0        0        0     2902 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/integrations.md
--rw-r--r--   0        0        0     2203 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/intro.md
--rw-r--r--   0        0        0     2798 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/releasing.md
--rw-r--r--   0        0        0     3281 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/styleguide.md
--rw-r--r--   0        0        0     6281 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/taskfile_versions.md
--rw-r--r--   0        0        0      875 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/translate.md
--rw-r--r--   0        0        0    42065 2024-03-10 14:06:46.611338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-plugin-content-docs/current/usage.md
--rw-r--r--   0        0        0     1792 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-theme-classic/footer.json
--rw-r--r--   0        0        0      967 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/fr-FR/docusaurus-theme-classic/navbar.json
--rw-r--r--   0        0        0    16684 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/code.json
--rw-r--r--   0        0        0     6850 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-blog/2023-09-02-introducing-experiments.md
--rw-r--r--   0        0        0      280 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-blog/authors.yml
--rw-r--r--   0        0        0      105 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current.json
--rw-r--r--   0        0        0    42270 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/api_reference.md
--rw-r--r--   0        0        0    33739 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/changelog.md
--rw-r--r--   0        0        0     1529 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/community.md
--rw-r--r--   0        0        0     7839 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/contributing.md
--rw-r--r--   0        0        0      711 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/deprecations/deprecations.md
--rw-r--r--   0        0        0      651 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/deprecations/template.md
--rw-r--r--   0        0        0     1248 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/deprecations/version_2_schema.md
--rw-r--r--   0        0        0     1928 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/donate.md
--rw-r--r--   0        0        0     4191 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/experiments/any_variables.md
--rw-r--r--   0        0        0     3184 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/experiments/any_variables.mdx
--rw-r--r--   0        0        0     5521 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/experiments/experiments.md
--rw-r--r--   0        0        0     1532 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/experiments/gentle_force.md
--rw-r--r--   0        0        0     4218 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/experiments/remote_taskfiles.md
--rw-r--r--   0        0        0     1123 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/experiments/template.md
--rw-r--r--   0        0        0     3777 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/experiments/workflow.md
--rw-r--r--   0        0        0     3088 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/faq.md
--rw-r--r--   0        0        0     8937 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/installation.md
--rw-r--r--   0        0        0     2902 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/integrations.md
--rw-r--r--   0        0        0     2216 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/intro.md
--rw-r--r--   0        0        0     3405 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/releasing.md
--rw-r--r--   0        0        0     3344 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/styleguide.md
--rw-r--r--   0        0        0     5447 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/taskfile_versions.md
--rw-r--r--   0        0        0      952 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/translate.md
--rw-r--r--   0        0        0    46262 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-plugin-content-docs/current/usage.md
--rw-r--r--   0        0        0     1805 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-theme-classic/footer.json
--rw-r--r--   0        0        0      971 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ja-JP/docusaurus-theme-classic/navbar.json
--rw-r--r--   0        0        0    17034 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/code.json
--rw-r--r--   0        0        0     6850 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-blog/2023-09-02-introducing-experiments.md
--rw-r--r--   0        0        0      279 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-blog/authors.yml
--rw-r--r--   0        0        0      107 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current.json
--rw-r--r--   0        0        0    44780 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/api_reference.md
--rw-r--r--   0        0        0    33739 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/changelog.md
--rw-r--r--   0        0        0     1530 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/community.md
--rw-r--r--   0        0        0     7750 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/contributing.md
--rw-r--r--   0        0        0      711 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/deprecations/deprecations.md
--rw-r--r--   0        0        0      651 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/deprecations/template.md
--rw-r--r--   0        0        0     1248 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/deprecations/version_2_schema.md
--rw-r--r--   0        0        0     1999 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/donate.md
--rw-r--r--   0        0        0     4191 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/experiments/any_variables.md
--rw-r--r--   0        0        0     3184 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/experiments/any_variables.mdx
--rw-r--r--   0        0        0     5521 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/experiments/experiments.md
--rw-r--r--   0        0        0     1532 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/experiments/gentle_force.md
--rw-r--r--   0        0        0     4218 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/experiments/remote_taskfiles.md
--rw-r--r--   0        0        0     1123 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/experiments/template.md
--rw-r--r--   0        0        0     3777 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/experiments/workflow.md
--rw-r--r--   0        0        0     2598 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/faq.md
--rw-r--r--   0        0        0     7547 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/installation.md
--rw-r--r--   0        0        0     2902 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/integrations.md
--rw-r--r--   0        0        0     2215 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/intro.md
--rw-r--r--   0        0        0     2798 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/releasing.md
--rw-r--r--   0        0        0     2879 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/styleguide.md
--rw-r--r--   0        0        0     5444 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/taskfile_versions.md
--rw-r--r--   0        0        0      821 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/translate.md
--rw-r--r--   0        0        0    42072 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-plugin-content-docs/current/usage.md
--rw-r--r--   0        0        0     1785 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-theme-classic/footer.json
--rw-r--r--   0        0        0      958 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/pt-BR/docusaurus-theme-classic/navbar.json
--rw-r--r--   0        0        0    18726 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/code.json
--rw-r--r--   0        0        0     6850 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-blog/2023-09-02-introducing-experiments.md
--rw-r--r--   0        0        0      279 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-blog/authors.yml
--rw-r--r--   0        0        0      103 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current.json
--rw-r--r--   0        0        0    41922 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/api_reference.md
--rw-r--r--   0        0        0    33739 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/changelog.md
--rw-r--r--   0        0        0     2013 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/community.md
--rw-r--r--   0        0        0    12310 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/contributing.md
--rw-r--r--   0        0        0      711 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/deprecations/deprecations.md
--rw-r--r--   0        0        0      651 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/deprecations/template.md
--rw-r--r--   0        0        0     1248 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/deprecations/version_2_schema.md
--rw-r--r--   0        0        0     2831 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/donate.md
--rw-r--r--   0        0        0     4191 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/experiments/any_variables.md
--rw-r--r--   0        0        0     3184 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/experiments/any_variables.mdx
--rw-r--r--   0        0        0     5521 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/experiments/experiments.md
--rw-r--r--   0        0        0     1532 2024-03-10 14:06:46.615338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/experiments/gentle_force.md
--rw-r--r--   0        0        0     4218 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/experiments/remote_taskfiles.md
--rw-r--r--   0        0        0     1123 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/experiments/template.md
--rw-r--r--   0        0        0     3777 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/experiments/workflow.md
--rw-r--r--   0        0        0     3524 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/faq.md
--rw-r--r--   0        0        0     9990 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/installation.md
--rw-r--r--   0        0        0     4148 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/integrations.md
--rw-r--r--   0        0        0     2933 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/intro.md
--rw-r--r--   0        0        0     3687 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/releasing.md
--rw-r--r--   0        0        0     3959 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/styleguide.md
--rw-r--r--   0        0        0     7204 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/taskfile_versions.md
--rw-r--r--   0        0        0     1181 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/translate.md
--rw-r--r--   0        0        0    48601 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-plugin-content-docs/current/usage.md
--rw-r--r--   0        0        0     1779 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-theme-classic/footer.json
--rw-r--r--   0        0        0      955 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/ru-RU/docusaurus-theme-classic/navbar.json
--rw-r--r--   0        0        0    16805 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/code.json
--rw-r--r--   0        0        0     6850 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-blog/2023-09-02-introducing-experiments.md
--rw-r--r--   0        0        0      284 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-blog/authors.yml
--rw-r--r--   0        0        0      106 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current.json
--rw-r--r--   0        0        0    41457 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/api_reference.md
--rw-r--r--   0        0        0    33739 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/changelog.md
--rw-r--r--   0        0        0     1529 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/community.md
--rw-r--r--   0        0        0     7750 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/contributing.md
--rw-r--r--   0        0        0      711 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/deprecations/deprecations.md
--rw-r--r--   0        0        0      651 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/deprecations/template.md
--rw-r--r--   0        0        0     1248 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/deprecations/version_2_schema.md
--rw-r--r--   0        0        0     1977 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/donate.md
--rw-r--r--   0        0        0     4191 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/experiments/any_variables.md
--rw-r--r--   0        0        0     3184 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/experiments/any_variables.mdx
--rw-r--r--   0        0        0     5600 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/experiments/experiments.md
--rw-r--r--   0        0        0     1532 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/experiments/gentle_force.md
--rw-r--r--   0        0        0     4218 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/experiments/remote_taskfiles.md
--rw-r--r--   0        0        0     1123 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/experiments/template.md
--rw-r--r--   0        0        0     3777 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/experiments/workflow.md
--rw-r--r--   0        0        0     2581 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/faq.md
--rw-r--r--   0        0        0     7329 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/installation.md
--rw-r--r--   0        0        0     2902 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/integrations.md
--rw-r--r--   0        0        0     1963 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/intro.md
--rw-r--r--   0        0        0     2798 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/releasing.md
--rw-r--r--   0        0        0     2875 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/styleguide.md
--rw-r--r--   0        0        0     5441 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/taskfile_versions.md
--rw-r--r--   0        0        0      766 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/translate.md
--rw-r--r--   0        0        0    42078 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-plugin-content-docs/current/usage.md
--rw-r--r--   0        0        0     1784 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-theme-classic/footer.json
--rw-r--r--   0        0        0      962 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/tr-TR/docusaurus-theme-classic/navbar.json
--rw-r--r--   0        0        0    16407 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/code.json
--rw-r--r--   0        0        0     6850 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-blog/2023-09-02-introducing-experiments.md
--rw-r--r--   0        0        0      281 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-blog/authors.yml
--rw-r--r--   0        0        0      103 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current.json
--rw-r--r--   0        0        0    34113 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/api_reference.md
--rw-r--r--   0        0        0    33684 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/changelog.md
--rw-r--r--   0        0        0     1383 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/community.md
--rw-r--r--   0        0        0     7302 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/contributing.md
--rw-r--r--   0        0        0      711 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/deprecations/deprecations.md
--rw-r--r--   0        0        0      651 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/deprecations/template.md
--rw-r--r--   0        0        0     1248 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/deprecations/version_2_schema.md
--rw-r--r--   0        0        0     1912 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/donate.md
--rw-r--r--   0        0        0     4191 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/experiments/any_variables.md
--rw-r--r--   0        0        0     3184 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/experiments/any_variables.mdx
--rw-r--r--   0        0        0     5521 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/experiments/experiments.md
--rw-r--r--   0        0        0     1532 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/experiments/gentle_force.md
--rw-r--r--   0        0        0     4218 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/experiments/remote_taskfiles.md
--rw-r--r--   0        0        0     1123 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/experiments/template.md
--rw-r--r--   0        0        0     3777 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/experiments/workflow.md
--rw-r--r--   0        0        0     2481 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/faq.md
--rw-r--r--   0        0        0     6650 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/installation.md
--rw-r--r--   0        0        0     2797 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/integrations.md
--rw-r--r--   0        0        0     1878 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/intro.md
--rw-r--r--   0        0        0     2638 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/releasing.md
--rw-r--r--   0        0        0     2782 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/styleguide.md
--rw-r--r--   0        0        0     5239 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/taskfile_versions.md
--rw-r--r--   0        0        0      754 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/translate.md
--rw-r--r--   0        0        0    40234 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-plugin-content-docs/current/usage.md
--rw-r--r--   0        0        0     1772 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-theme-classic/footer.json
--rw-r--r--   0        0        0      959 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/i18n/zh-Hans/docusaurus-theme-classic/navbar.json
--rw-r--r--   0        0        0     1417 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/package.json
--rw-r--r--   0        0        0      208 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/prettier.config.js
--rw-r--r--   0        0        0      271 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/sidebars.ts
--rw-r--r--   0        0        0     1050 2024-03-10 14:06:46.619338 go_task_bin-3.35.1/task/docs/src/api/crowdin.js
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/src/components/.keep
--rw-r--r--   0        0        0     1202 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/src/css/carbon.css
--rw-r--r--   0        0        0     2252 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/src/css/custom.css
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/src/pages/.keep
--rw-r--r--   0        0        0     1342 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/src/themes/prismDark.js
--rw-r--r--   0        0        0     1679 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/src/themes/prismLight.js
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/.nojekyll
--rw-r--r--   0        0        0       13 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/CNAME
--rw-r--r--   0        0        0     7281 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/img/appwrite.svg
--rw-r--r--   0        0        0   173915 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/img/favicon.ico
--rw-r--r--   0        0        0    13524 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/img/logo.png
--rw-r--r--   0        0        0      435 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/img/logo.svg
--rw-r--r--   0        0        0      360 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/img/logo_mono.svg
--rw-r--r--   0        0        0    19847 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/img/og-image.png
--rw-r--r--   0        0        0     1276 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/img/pix.png
--rwxr-xr-x   0        0        0     9634 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/install.sh
--rw-r--r--   0        0        0      784 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/js/carbon.js
--rw-r--r--   0        0        0    21627 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/static/schema.json
--rw-r--r--   0        0        0       87 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/tsconfig.json
--rw-r--r--   0        0        0   355529 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/docs/yarn.lock
--rw-r--r--   0        0        0     1558 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/errors/errors.go
--rw-r--r--   0        0        0     3645 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/errors/errors_task.go
--rw-r--r--   0        0        0     4674 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/errors/errors_taskfile.go
--rw-r--r--   0        0        0      946 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/go.mod
--rw-r--r--   0        0        0     6014 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/go.sum
--rw-r--r--   0        0        0      445 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/hash.go
--rw-r--r--   0        0        0     5727 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/help.go
--rw-r--r--   0        0        0      770 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/init.go
--rwxr-xr-x   0        0        0     9634 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/install-task.sh
--rw-r--r--   0        0        0     5871 2024-03-10 14:06:46.623338 go_task_bin-3.35.1/task/internal/compiler/compiler.go
--rw-r--r--   0        0        0      380 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/compiler/env.go
--rw-r--r--   0        0        0      569 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/deepcopy/deepcopy.go
--rw-r--r--   0        0        0      659 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/editors/output.go
--rw-r--r--   0        0        0      430 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/env/env.go
--rw-r--r--   0        0        0      287 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/execext/devnull.go
--rw-r--r--   0        0        0     3349 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/execext/exec.go
--rw-r--r--   0        0        0     1082 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/exp/maps.go
--rw-r--r--   0        0        0     2529 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/experiments/experiments.go
--rw-r--r--   0        0        0     1031 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/filepathext/filepathext.go
--rw-r--r--   0        0        0      518 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/fingerprint/checker.go
--rw-r--r--   0        0        0     1094 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/fingerprint/glob.go
--rw-r--r--   0        0        0      388 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/fingerprint/sources.go
--rw-r--r--   0        0        0     2791 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/fingerprint/sources_checksum.go
--rw-r--r--   0        0        0      396 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/fingerprint/sources_checksum_test.go
--rw-r--r--   0        0        0      459 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/fingerprint/sources_none.go
--rw-r--r--   0        0        0     3521 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/fingerprint/sources_timestamp.go
--rw-r--r--   0        0        0      890 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/fingerprint/status.go
--rw-r--r--   0        0        0     2938 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/fingerprint/task.go
--rw-r--r--   0        0        0     5500 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/fingerprint/task_test.go
--rw-r--r--   0        0        0     5875 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/flags/flags.go
--rw-r--r--   0        0        0     1191 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/goext/meta.go
--rw-r--r--   0        0        0      439 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/hash/hash.go
--rw-r--r--   0        0        0     3325 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/logger/logger.go
--rw-r--r--   0        0        0     6003 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/mocks/sources_checkable.go
--rw-r--r--   0        0        0     2592 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/mocks/status_checkable.go
--rw-r--r--   0        0        0     3805 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/omap/orderedmap.go
--rw-r--r--   0        0        0     2607 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/omap/orderedmap_test.go
--rw-r--r--   0        0        0      976 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/output/group.go
--rw-r--r--   0        0        0      235 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/output/interleaved.go
--rw-r--r--   0        0        0     1246 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/output/output.go
--rw-r--r--   0        0        0     3500 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/output/output_test.go
--rw-r--r--   0        0        0     1302 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/output/prefixed.go
--rw-r--r--   0        0        0      286 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/slicesext/slicesext.go
--rw-r--r--   0        0        0     1063 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/sort/sorter.go
--rw-r--r--   0        0        0     1895 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/sort/sorter_test.go
--rw-r--r--   0        0        0     2531 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/summary/summary.go
--rw-r--r--   0        0        0     3636 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/summary/summary_test.go
--rw-r--r--   0        0        0      308 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/sysinfo/uid.go
--rw-r--r--   0        0        0      208 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/sysinfo/uid_win.go
--rw-r--r--   0        0        0     2034 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/templater/funcs.go
--rw-r--r--   0        0        0     2713 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/templater/templater.go
--rw-r--r--   0        0        0      165 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/term/term.go
--rw-r--r--   0        0        0      348 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/internal/version/version.go
--rw-r--r--   0        0        0      924 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/package-lock.json
--rw-r--r--   0        0        0      807 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/package.json
--rw-r--r--   0        0        0      804 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/precondition.go
--rw-r--r--   0        0        0      679 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/requires.go
--rw-r--r--   0        0        0     5714 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/setup.go
--rw-r--r--   0        0        0      700 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/signals.go
--rw-r--r--   0        0        0     7605 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/signals_test.go
--rw-r--r--   0        0        0     1172 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/status.go
--rw-r--r--   0        0        0    13335 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/task.go
--rw-r--r--   0        0        0    60570 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/task_test.go
--rw-r--r--   0        0        0      185 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/call.go
--rw-r--r--   0        0        0     2490 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/cmd.go
--rw-r--r--   0        0        0      842 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/dep.go
--rw-r--r--   0        0        0     1156 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/for.go
--rw-r--r--   0        0        0      530 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/glob.go
--rw-r--r--   0        0        0     4145 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/include.go
--rw-r--r--   0        0        0      247 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/location.go
--rw-r--r--   0        0        0     1373 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/output.go
--rw-r--r--   0        0        0     2431 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/platforms.go
--rw-r--r--   0        0        0     1522 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/platforms_test.go
--rw-r--r--   0        0        0     1150 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/precondition.go
--rw-r--r--   0        0        0      976 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/precondition_test.go
--rw-r--r--   0        0        0      318 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/requires.go
--rw-r--r--   0        0        0     5704 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/task.go
--rw-r--r--   0        0        0     2128 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/taskfile.go
--rw-r--r--   0        0        0     1887 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/taskfile_test.go
--rw-r--r--   0        0        0     4111 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/tasks.go
--rw-r--r--   0        0        0     3559 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/ast/var.go
--rw-r--r--   0        0        0     1232 2024-03-10 14:06:46.627338 go_task_bin-3.35.1/task/taskfile/cache.go
--rw-r--r--   0        0        0      998 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/taskfile/dotenv.go
--rw-r--r--   0        0        0     2040 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/taskfile/node.go
--rw-r--r--   0        0        0      909 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/taskfile/node_base.go
--rw-r--r--   0        0        0     1045 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/taskfile/node_file.go
--rw-r--r--   0        0        0     1445 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/taskfile/node_http.go
--rw-r--r--   0        0        0      793 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/taskfile/node_stdin.go
--rw-r--r--   0        0        0     7770 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/taskfile/reader.go
--rw-r--r--   0        0        0     2546 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/taskfile/taskfile.go
--rw-r--r--   0        0        0      243 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/alias/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/alias/Taskfile2.yml
--rw-r--r--   0        0        0      111 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/alias/alias-summary.txt
--rw-r--r--   0        0        0       90 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/alias/alias.txt
--rw-r--r--   0        0        0       21 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/checksum/.gitignore
--rw-r--r--   0        0        0      428 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/checksum/Taskfile.yml
--rw-r--r--   0        0        0       14 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/checksum/ignore_me.txt
--rw-r--r--   0        0        0       14 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/checksum/source.txt
--rw-r--r--   0        0        0      351 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/concurrency/Taskfile.yml
--rw-r--r--   0        0        0      104 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/cyclic/Taskfile.yml
--rw-r--r--   0        0        0      243 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/deferred/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/deps/.gitignore
--rw-r--r--   0        0        0      703 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/deps/Taskfile.yml
--rw-r--r--   0        0        0       72 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dir/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dir/dynamic_var/.gitignore
--rw-r--r--   0        0        0      649 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dir/dynamic_var/Taskfile.yml
--rw-r--r--   0        0        0      377 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dir/dynamic_var/subdirectory/Taskfile.yml
--rw-r--r--   0        0        0      136 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dir/dynamic_var_on_created_dir/Taskfile.yml
--rw-r--r--   0        0        0       90 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dir/explicit_doesnt_exist/Taskfile.yml
--rw-r--r--   0        0        0       88 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dir/explicit_exists/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dir/explicit_exists/exists/.keep
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/.gitignore
--rw-r--r--   0        0        0      168 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/default/Taskfile.yml
--rw-r--r--   0        0        0       31 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/env_var_in_path/.env.testing
--rw-r--r--   0        0        0      119 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/env_var_in_path/Taskfile.yml
--rw-r--r--   0        0        0      158 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/error_included_envs/Taskfile.yml
--rw-r--r--   0        0        0       23 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/include1/.env
--rw-r--r--   0        0        0       31 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/include1/Taskfile.yml
--rw-r--r--   0        0        0       23 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/include1/envs/.env
--rw-r--r--   0        0        0       31 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/local_env_in_path/.env.testing
--rw-r--r--   0        0        0      148 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/local_env_in_path/Taskfile.yml
--rw-r--r--   0        0        0       31 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/local_var_in_path/.env.testing
--rw-r--r--   0        0        0      195 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/local_var_in_path/Taskfile.yml
--rw-r--r--   0        0        0      131 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv/missing_env/Taskfile.yml
--rw-r--r--   0        0        0        8 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv_task/default/.env
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv_task/default/.gitignore
--rw-r--r--   0        0        0      456 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dotenv_task/default/Taskfile.yml
--rw-r--r--   0        0        0       63 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dry/Taskfile.yml
--rw-r--r--   0        0        0      121 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dry_checksum/Taskfile.yml
--rw-r--r--   0        0        0       13 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/dry_checksum/source.txt
--rw-r--r--   0        0        0       32 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/empty_task/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/env/.gitignore
--rw-r--r--   0        0        0      499 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/env/Taskfile.yml
--rw-r--r--   0        0        0      101 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/error_code/Taskfile.yml
--rw-r--r--   0        0        0      280 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/evaluate_symlinks_in_paths/Taskfile.yaml
--rw-r--r--   0        0        0       19 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/evaluate_symlinks_in_paths/shared/b
--rw-r--r--   0        0        0       25 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/evaluate_symlinks_in_paths/shared/inner_shared/c
--rw-r--r--   0        0        0       12 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/evaluate_symlinks_in_paths/src/a
--rw-r--r--   0        0        0       89 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/exit_immediately/Taskfile.yml
--rw-r--r--   0        0        0       80 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/expand/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/file_names/.gitignore
--rw-r--r--   0        0        0       58 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/file_names/Taskfile.dist.yaml/Taskfile.dist.yaml
--rw-r--r--   0        0        0       58 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/file_names/Taskfile.dist.yml/Taskfile.dist.yml
--rw-r--r--   0        0        0       58 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/file_names/Taskfile.yaml/Taskfile.yaml
--rw-r--r--   0        0        0       58 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/file_names/Taskfile.yml/Taskfile.yml
--rw-r--r--   0        0        0     1635 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/for/Taskfile.yml
--rw-r--r--   0        0        0        4 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/for/bar.txt
--rw-r--r--   0        0        0        4 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/for/foo.txt
--rw-r--r--   0        0        0      295 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/force/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/generates/.gitignore
--rw-r--r--   0        0        0      986 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/generates/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/generates/sub/.keep
--rw-r--r--   0        0        0      262 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/ignore_errors/Taskfile.yml
--rw-r--r--   0        0        0       80 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/ignore_nil_elements/cmds/Taskfile.yml
--rw-r--r--   0        0        0      116 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/ignore_nil_elements/deps/Taskfile.yml
--rw-r--r--   0        0        0       94 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/ignore_nil_elements/includes/Taskfile.yml
--rw-r--r--   0        0        0       81 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/ignore_nil_elements/includes/inc.yml
--rw-r--r--   0        0        0      123 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/ignore_nil_elements/preconditions/Taskfile.yml
--rw-r--r--   0        0        0       66 2024-03-10 14:06:46.631338 go_task_bin-3.35.1/task/testdata/ignore_signals/Taskfile.yml
--rw-r--r--   0        0        0      385 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/include_with_vars/Taskfile.yml
--rw-r--r--   0        0        0      229 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/include_with_vars/include/Taskfile.include.yml
--rw-r--r--   0        0        0      266 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/include_with_vars_multi_level/Taskfile.yml
--rw-r--r--   0        0        0       97 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/include_with_vars_multi_level/bar/Taskfile.yml
--rw-r--r--   0        0        0       97 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/include_with_vars_multi_level/foo/Taskfile.yml
--rw-r--r--   0        0        0      102 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/include_with_vars_multi_level/lib/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes/.gitignore
--rw-r--r--   0        0        0      768 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes/Taskfile.yml
--rw-r--r--   0        0        0       93 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes/Taskfile2.yml
--rw-r--r--   0        0        0       55 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes/Taskfile_darwin.yml
--rw-r--r--   0        0        0       55 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes/Taskfile_linux.yml
--rw-r--r--   0        0        0       55 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes/Taskfile_windows.yml
--rw-r--r--   0        0        0       95 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes/included/Taskfile.yml
--rw-r--r--   0        0        0      225 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes/module1/Taskfile.yml
--rw-r--r--   0        0        0      213 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes/module2/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_call_root_task/.gitignore
--rw-r--r--   0        0        0      122 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_call_root_task/Taskfile.yml
--rw-r--r--   0        0        0       69 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_call_root_task/Taskfile2.yml
--rw-r--r--   0        0        0      173 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_cycle/Taskfile.yml
--rw-r--r--   0        0        0      109 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_cycle/one/Taskfile.yml
--rw-r--r--   0        0        0      109 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_cycle/one/two/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_deps/.gitignore
--rw-r--r--   0        0        0      110 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_deps/Taskfile.yml
--rw-r--r--   0        0        0      267 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_deps/Taskfile2.yml
--rw-r--r--   0        0        0        9 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_empty/.gitignore
--rw-r--r--   0        0        0       50 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_empty/Taskfile.yml
--rw-r--r--   0        0        0      125 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_empty/Taskfile2.yml
--rw-r--r--   0        0        0       51 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_incorrect/Taskfile.yml
--rw-r--r--   0        0        0       28 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_incorrect/incomplete.yml
--rw-r--r--   0        0        0      188 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_internal/Taskfile.yml
--rw-r--r--   0        0        0       70 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_internal/Taskfile2.yml
--rw-r--r--   0        0        0      196 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_interpolation/Taskfile.yml
--rw-r--r--   0        0        0       66 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_interpolation/included/Taskfile.yml
--rw-r--r--   0        0        0      161 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_multi_level/Taskfile.yml
--rw-r--r--   0        0        0        4 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_multi_level/called_one.txt
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_multi_level/called_three.txt
--rw-r--r--   0        0        0        4 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_multi_level/called_two.txt
--rw-r--r--   0        0        0       85 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_multi_level/one/Taskfile.yml
--rw-r--r--   0        0        0      101 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_multi_level/one/two/Taskfile.yml
--rw-r--r--   0        0        0       62 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_multi_level/one/two/three/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_optional/.gitignore
--rw-r--r--   0        0        0      162 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_optional/Taskfile.yml
--rw-r--r--   0        0        0      149 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_optional_explicit_false/Taskfile.yml
--rw-r--r--   0        0        0      115 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_optional_implicit_false/Taskfile.yml
--rw-r--r--   0        0        0      133 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_rel_path/Taskfile.yml
--rw-r--r--   0        0        0       32 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_rel_path/common/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_rel_path/included/Taskfile.yml
--rw-r--r--   0        0        0      129 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_shadowed_default/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_shadowed_default/Taskfile2.yml
--rw-r--r--   0        0        0        9 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_shadowed_default/file.txt
--rw-r--r--   0        0        0       64 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_unshadowed_default/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_unshadowed_default/Taskfile2.yml
--rw-r--r--   0        0        0        9 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_unshadowed_default/file.txt
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_yaml/.gitignore
--rw-r--r--   0        0        0      226 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_yaml/Custom.ext
--rw-r--r--   0        0        0      115 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_yaml/included/Taskfile.yaml
--rw-r--r--   0        0        0      109 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/includes_yaml/included/custom.yaml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/init/.gitignore
--rw-r--r--   0        0        0      167 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/internal_task/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/label_list/Taskfile.yml
--rw-r--r--   0        0        0       76 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/label_status/Taskfile.yml
--rw-r--r--   0        0        0      104 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/label_summary/Taskfile.yml
--rw-r--r--   0        0        0       82 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/label_uptodate/Taskfile.yml
--rw-r--r--   0        0        0      105 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/label_var/Taskfile.yml
--rw-r--r--   0        0        0       90 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/list_desc_interpolation/Taskfile.yml
--rw-r--r--   0        0        0      164 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/list_mixed_desc/Taskfile.yml
--rw-r--r--   0        0        0      199 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/output_group/Taskfile.yml
--rw-r--r--   0        0        0      255 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/output_group_error_only/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/params/.gitignore
--rw-r--r--   0        0        0     1255 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/params/Taskfile.yml
--rw-r--r--   0        0        0     1584 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/platforms/Taskfile.yml
--rw-r--r--   0        0        0      285 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/precondition/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/precondition/foo.txt
--rw-r--r--   0        0        0      226 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/prompt/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/run/.gitignore
--rw-r--r--   0        0        0      468 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/run/Taskfile.yml
--rw-r--r--   0        0        0      201 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/shopts/command_level/Taskfile.yml
--rw-r--r--   0        0        0      175 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/shopts/global_level/Taskfile.yml
--rw-r--r--   0        0        0      183 2024-03-10 14:06:46.635338 go_task_bin-3.35.1/task/testdata/shopts/task_level/Taskfile.yml
--rw-r--r--   0        0        0      174 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/short_task_notation/Taskfile.yml
--rw-r--r--   0        0        0     1350 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/silent/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/single_cmd_dep/.gitignore
--rw-r--r--   0        0        0       99 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/single_cmd_dep/Taskfile.yml
--rw-r--r--   0        0        0      282 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/special_vars/Taskfile.yml
--rw-r--r--   0        0        0      214 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/special_vars/included/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/special_vars/subdir/.gitkeep
--rw-r--r--   0        0        0       92 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/split_args/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/status/.gitignore
--rw-r--r--   0        0        0      331 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/status/Taskfile.yml
--rw-r--r--   0        0        0       14 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/status_vars/.gitignore
--rw-r--r--   0        0        0      170 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/status_vars/Taskfile.yml
--rw-r--r--   0        0        0       14 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/status_vars/source.txt
--rw-r--r--   0        0        0      566 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/summary/Taskfile.yml
--rw-r--r--   0        0        0      346 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/summary/task-with-summary.txt
--rw-r--r--   0        0        0       78 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/taskfile_walk/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/taskfile_walk/foo/bar/.gitkeep
--rw-r--r--   0        0        0       96 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/user_working_dir/Taskfile.yml
--rw-r--r--   0        0        0       74 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/user_working_dir_with_includes/Taskfile.yml
--rw-r--r--   0        0        0      101 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/user_working_dir_with_includes/included/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/user_working_dir_with_includes/somedir/.keep
--rw-r--r--   0        0        0       27 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/vars/.env
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/vars/.gitignore
--rw-r--r--   0        0        0     1008 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/vars/Taskfile.yml
--rw-r--r--   0        0        0     2188 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/vars/any/Taskfile.yml
--rw-r--r--   0        0        0     1978 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/vars/any2/Taskfile.yml
--rw-r--r--   0        0        0      276 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/vars/any2/example.json
--rw-r--r--   0        0        0      111 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/vars/any2/example.yaml
--rw-r--r--   0        0        0       93 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/version/v1/Taskfile.yml
--rw-r--r--   0        0        0       93 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/version/v2/Taskfile.yml
--rw-r--r--   0        0        0       93 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/version/v3/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/watcher_interval/.gitignore
--rw-r--r--   0        0        0      194 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/watcher_interval/Taskfile.yaml
--rw-r--r--   0        0        0      519 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/testdata/wildcards/Taskfile.yml
--rw-r--r--   0        0        0     8516 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/variables.go
--rw-r--r--   0        0        0     4215 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/watch.go
--rw-r--r--   0        0        0     2030 2024-03-10 14:06:46.639338 go_task_bin-3.35.1/task/watch_test.go
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 go_task_bin-3.35.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-18 05:25:30.803037 go_task_bin-3.36.0/LICENSE
+-rw-r--r--   0        0        0     1031 2024-04-18 05:25:30.803037 go_task_bin-3.36.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:30.803037 go_task_bin-3.36.0/go_task_bin/__init__.py
+-rw-r--r--   0        0        0     1384 2024-04-18 05:25:30.803037 go_task_bin-3.36.0/pdm_build.py
+-rw-r--r--   0        0        0     1245 2024-04-18 05:27:35.819217 go_task_bin-3.36.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.editorconfig
+-rw-r--r--   0        0        0       37 2024-04-18 05:25:32.395039 go_task_bin-3.36.0/task/.git
+-rw-r--r--   0        0        0       12 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.gitattributes
+-rw-r--r--   0        0        0     3217 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      521 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       88 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/FUNDING.yml
+-rw-r--r--   0        0        0      387 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      552 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      368 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      462 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/dependabot.yml
+-rw-r--r--   0        0        0      225 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1463 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/issue-awaiting-response.yml
+-rw-r--r--   0        0        0      838 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/issue-closed.yml
+-rw-r--r--   0        0        0     6565 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/issue-experiment.yml
+-rw-r--r--   0        0        0      813 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/issue-needs-triage.yml
+-rw-r--r--   0        0        0      865 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      476 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/release.yml
+-rw-r--r--   0        0        0      872 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/test.yml
+-rw-r--r--   0        0        0      922 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/upload-source-documents.yml
+-rw-r--r--   0        0        0      445 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.gitignore
+-rw-r--r--   0        0        0      387 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.golangci.yml
+-rw-r--r--   0        0        0     3037 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.goreleaser.yml
+-rw-r--r--   0        0        0       77 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.mockery.yaml
+-rw-r--r--   0        0        0        8 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.nvmrc
+-rw-r--r--   0        0        0      125 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.prettierrc.yml
+-rw-r--r--   0        0        0      324 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.vscode/settings-sample.json
+-rw-r--r--   0        0        0    37761 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/CHANGELOG.md
+-rw-r--r--   0        0        0     1080 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/LICENSE
+-rw-r--r--   0        0        0      634 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/README.md
+-rw-r--r--   0        0        0     2948 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/Taskfile.yml
+-rw-r--r--   0        0        0      586 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/args/args.go
+-rw-r--r--   0        0        0     2393 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/args/args_test.go
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/bin/.keep
+-rw-r--r--   0        0        0     3288 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/cmd/release/main.go
+-rw-r--r--   0        0        0     4874 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/cmd/sleepit/sleepit.go
+-rw-r--r--   0        0        0     4466 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/cmd/task/task.go
+-rw-r--r--   0        0        0     1329 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/completion/bash/task.bash
+-rw-r--r--   0        0        0     2342 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/completion/fish/task.fish
+-rw-r--r--   0        0        0     1992 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/completion/ps/task.ps1
+-rwxr-xr-x   0        0        0     2431 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/completion/zsh/_task
+-rw-r--r--   0        0        0      436 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/concurrency.go
+-rw-r--r--   0        0        0     1558 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/errors/errors.go
+-rw-r--r--   0        0        0     3645 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/errors/errors_task.go
+-rw-r--r--   0        0        0     4674 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/errors/errors_taskfile.go
+-rw-r--r--   0        0        0      979 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/go.mod
+-rw-r--r--   0        0        0     5796 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/go.sum
+-rw-r--r--   0        0        0      445 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/hash.go
+-rw-r--r--   0        0        0     5727 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/help.go
+-rw-r--r--   0        0        0      770 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/init.go
+-rwxr-xr-x   0        0        0     9634 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/install-task.sh
+-rw-r--r--   0        0        0     5633 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/compiler/compiler.go
+-rw-r--r--   0        0        0      380 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/compiler/env.go
+-rw-r--r--   0        0        0     3621 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/deepcopy/deepcopy.go
+-rw-r--r--   0        0        0      659 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/editors/output.go
+-rw-r--r--   0        0        0      430 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/env/env.go
+-rw-r--r--   0        0        0      287 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/execext/devnull.go
+-rw-r--r--   0        0        0     3349 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/execext/exec.go
+-rw-r--r--   0        0        0     1082 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/exp/maps.go
+-rw-r--r--   0        0        0     2550 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/experiments/experiments.go
+-rw-r--r--   0        0        0     1031 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/filepathext/filepathext.go
+-rw-r--r--   0        0        0      518 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/checker.go
+-rw-r--r--   0        0        0     1094 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/glob.go
+-rw-r--r--   0        0        0      388 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/sources.go
+-rw-r--r--   0        0        0     2791 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/sources_checksum.go
+-rw-r--r--   0        0        0      396 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/sources_checksum_test.go
+-rw-r--r--   0        0        0      459 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/sources_none.go
+-rw-r--r--   0        0        0     3521 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/sources_timestamp.go
+-rw-r--r--   0        0        0      890 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/status.go
+-rw-r--r--   0        0        0     2938 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/task.go
+-rw-r--r--   0        0        0     5500 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/task_test.go
+-rw-r--r--   0        0        0     5766 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/flags/flags.go
+-rw-r--r--   0        0        0     1191 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/goext/meta.go
+-rw-r--r--   0        0        0      439 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/hash/hash.go
+-rw-r--r--   0        0        0     4053 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/logger/logger.go
+-rw-r--r--   0        0        0     6003 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/mocks/sources_checkable.go
+-rw-r--r--   0        0        0     2592 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/mocks/status_checkable.go
+-rw-r--r--   0        0        0     3805 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/omap/orderedmap.go
+-rw-r--r--   0        0        0     2607 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/omap/orderedmap_test.go
+-rw-r--r--   0        0        0     1058 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/output/group.go
+-rw-r--r--   0        0        0      292 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/output/interleaved.go
+-rw-r--r--   0        0        0     1075 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/output/output.go
+-rw-r--r--   0        0        0     3496 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/output/output_test.go
+-rw-r--r--   0        0        0     1359 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/output/prefixed.go
+-rw-r--r--   0        0        0      286 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/slicesext/slicesext.go
+-rw-r--r--   0        0        0     1063 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/sort/sorter.go
+-rw-r--r--   0        0        0     1895 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/sort/sorter_test.go
+-rw-r--r--   0        0        0     2531 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/summary/summary.go
+-rw-r--r--   0        0        0     3636 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/summary/summary_test.go
+-rw-r--r--   0        0        0      308 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/sysinfo/uid.go
+-rw-r--r--   0        0        0      208 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/sysinfo/uid_win.go
+-rw-r--r--   0        0        0     2034 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/templater/funcs.go
+-rw-r--r--   0        0        0     2817 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/templater/templater.go
+-rw-r--r--   0        0        0      165 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/term/term.go
+-rw-r--r--   0        0        0      348 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/version/version.go
+-rw-r--r--   0        0        0      924 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/package-lock.json
+-rw-r--r--   0        0        0      807 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/package.json
+-rw-r--r--   0        0        0      804 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/precondition.go
+-rw-r--r--   0        0        0      679 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/requires.go
+-rw-r--r--   0        0        0     5731 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/setup.go
+-rw-r--r--   0        0        0      700 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/signals.go
+-rw-r--r--   0        0        0     7605 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/signals_test.go
+-rw-r--r--   0        0        0     1172 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/status.go
+-rw-r--r--   0        0        0    13331 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/task.go
+-rw-r--r--   0        0        0    62564 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/task_test.go
+-rw-r--r--   0        0        0      185 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/call.go
+-rw-r--r--   0        0        0     2490 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/cmd.go
+-rw-r--r--   0        0        0      921 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/dep.go
+-rw-r--r--   0        0        0     1156 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/for.go
+-rw-r--r--   0        0        0      530 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/glob.go
+-rw-r--r--   0        0        0     2938 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/include.go
+-rw-r--r--   0        0        0      247 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/location.go
+-rw-r--r--   0        0        0     1373 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/output.go
+-rw-r--r--   0        0        0     2431 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/platforms.go
+-rw-r--r--   0        0        0     1522 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/platforms_test.go
+-rw-r--r--   0        0        0     1150 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/precondition.go
+-rw-r--r--   0        0        0      976 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/precondition_test.go
+-rw-r--r--   0        0        0      318 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/requires.go
+-rw-r--r--   0        0        0     5704 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/task.go
+-rw-r--r--   0        0        0     2128 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/taskfile.go
+-rw-r--r--   0        0        0     1887 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/taskfile_test.go
+-rw-r--r--   0        0        0     4111 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/tasks.go
+-rw-r--r--   0        0        0     3559 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/var.go
+-rw-r--r--   0        0        0     1232 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/cache.go
+-rw-r--r--   0        0        0     1011 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/dotenv.go
+-rw-r--r--   0        0        0     2100 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/node.go
+-rw-r--r--   0        0        0     1013 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/node_base.go
+-rw-r--r--   0        0        0     2752 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/node_file.go
+-rw-r--r--   0        0        0     2592 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/node_http.go
+-rw-r--r--   0        0        0     1444 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/node_stdin.go
+-rw-r--r--   0        0        0     7476 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/reader.go
+-rw-r--r--   0        0        0     5106 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/taskfile.go
+-rw-r--r--   0        0        0      243 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/alias/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/alias/Taskfile2.yml
+-rw-r--r--   0        0        0      111 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/alias/alias-summary.txt
+-rw-r--r--   0        0        0       90 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/alias/alias.txt
+-rw-r--r--   0        0        0       21 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/checksum/.gitignore
+-rw-r--r--   0        0        0      428 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/checksum/Taskfile.yml
+-rw-r--r--   0        0        0       14 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/checksum/ignore_me.txt
+-rw-r--r--   0        0        0       14 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/checksum/source.txt
+-rw-r--r--   0        0        0      351 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/concurrency/Taskfile.yml
+-rw-r--r--   0        0        0      104 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/cyclic/Taskfile.yml
+-rw-r--r--   0        0        0      243 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/deferred/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/deps/.gitignore
+-rw-r--r--   0        0        0      703 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/deps/Taskfile.yml
+-rw-r--r--   0        0        0       72 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/dynamic_var/.gitignore
+-rw-r--r--   0        0        0      649 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/dynamic_var/Taskfile.yml
+-rw-r--r--   0        0        0      377 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/dynamic_var/subdirectory/Taskfile.yml
+-rw-r--r--   0        0        0      136 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/dynamic_var_on_created_dir/Taskfile.yml
+-rw-r--r--   0        0        0       90 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/explicit_doesnt_exist/Taskfile.yml
+-rw-r--r--   0        0        0       88 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/explicit_exists/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/explicit_exists/exists/.keep
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/.gitignore
+-rw-r--r--   0        0        0      168 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/default/Taskfile.yml
+-rw-r--r--   0        0        0       31 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/env_var_in_path/.env.testing
+-rw-r--r--   0        0        0      119 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/env_var_in_path/Taskfile.yml
+-rw-r--r--   0        0        0      158 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/error_included_envs/Taskfile.yml
+-rw-r--r--   0        0        0       23 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/include1/.env
+-rw-r--r--   0        0        0       31 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/include1/Taskfile.yml
+-rw-r--r--   0        0        0       23 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/include1/envs/.env
+-rw-r--r--   0        0        0       31 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/local_env_in_path/.env.testing
+-rw-r--r--   0        0        0      148 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/local_env_in_path/Taskfile.yml
+-rw-r--r--   0        0        0       31 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/local_var_in_path/.env.testing
+-rw-r--r--   0        0        0      195 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/local_var_in_path/Taskfile.yml
+-rw-r--r--   0        0        0      131 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/missing_env/Taskfile.yml
+-rw-r--r--   0        0        0        8 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv_task/default/.env
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv_task/default/.gitignore
+-rw-r--r--   0        0        0      456 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv_task/default/Taskfile.yml
+-rw-r--r--   0        0        0       63 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dry/Taskfile.yml
+-rw-r--r--   0        0        0      121 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dry_checksum/Taskfile.yml
+-rw-r--r--   0        0        0       13 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dry_checksum/source.txt
+-rw-r--r--   0        0        0       32 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/empty_task/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/env/.gitignore
+-rw-r--r--   0        0        0      499 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/env/Taskfile.yml
+-rw-r--r--   0        0        0      101 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/error_code/Taskfile.yml
+-rw-r--r--   0        0        0      280 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/evaluate_symlinks_in_paths/Taskfile.yaml
+-rw-r--r--   0        0        0       19 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/evaluate_symlinks_in_paths/shared/b
+-rw-r--r--   0        0        0       25 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/evaluate_symlinks_in_paths/shared/inner_shared/c
+-rw-r--r--   0        0        0       12 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/evaluate_symlinks_in_paths/src/a
+-rw-r--r--   0        0        0       89 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/exit_immediately/Taskfile.yml
+-rw-r--r--   0        0        0       80 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/expand/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/file_names/.gitignore
+-rw-r--r--   0        0        0       58 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/file_names/Taskfile.dist.yaml/Taskfile.dist.yaml
+-rw-r--r--   0        0        0       58 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/file_names/Taskfile.dist.yml/Taskfile.dist.yml
+-rw-r--r--   0        0        0       58 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/file_names/Taskfile.yaml/Taskfile.yaml
+-rw-r--r--   0        0        0       58 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/file_names/Taskfile.yml/Taskfile.yml
+-rw-r--r--   0        0        0     1635 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/cmds/Taskfile.yml
+-rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/cmds/bar.txt
+-rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/cmds/foo.txt
+-rw-r--r--   0        0        0     1876 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/deps/Taskfile.yml
+-rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/deps/bar.txt
+-rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/deps/foo.txt
+-rw-r--r--   0        0        0      295 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/force/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/generates/.gitignore
+-rw-r--r--   0        0        0      986 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/generates/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/generates/sub/.keep
+-rw-r--r--   0        0        0      262 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_errors/Taskfile.yml
+-rw-r--r--   0        0        0       80 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_nil_elements/cmds/Taskfile.yml
+-rw-r--r--   0        0        0      116 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_nil_elements/deps/Taskfile.yml
+-rw-r--r--   0        0        0       94 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_nil_elements/includes/Taskfile.yml
+-rw-r--r--   0        0        0       81 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_nil_elements/includes/inc.yml
+-rw-r--r--   0        0        0      123 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_nil_elements/preconditions/Taskfile.yml
+-rw-r--r--   0        0        0       66 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_signals/Taskfile.yml
+-rw-r--r--   0        0        0      385 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars/Taskfile.yml
+-rw-r--r--   0        0        0      229 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars/include/Taskfile.include.yml
+-rw-r--r--   0        0        0      266 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars_multi_level/Taskfile.yml
+-rw-r--r--   0        0        0       97 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars_multi_level/bar/Taskfile.yml
+-rw-r--r--   0        0        0       97 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars_multi_level/foo/Taskfile.yml
+-rw-r--r--   0        0        0      130 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars_multi_level/lib/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/.gitignore
+-rw-r--r--   0        0        0      768 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/Taskfile.yml
+-rw-r--r--   0        0        0       93 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/Taskfile2.yml
+-rw-r--r--   0        0        0       55 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/Taskfile_darwin.yml
+-rw-r--r--   0        0        0       55 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/Taskfile_linux.yml
+-rw-r--r--   0        0        0       55 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/Taskfile_windows.yml
+-rw-r--r--   0        0        0       95 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/included/Taskfile.yml
+-rw-r--r--   0        0        0      225 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/module1/Taskfile.yml
+-rw-r--r--   0        0        0      213 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/module2/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_call_root_task/.gitignore
+-rw-r--r--   0        0        0      122 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_call_root_task/Taskfile.yml
+-rw-r--r--   0        0        0       69 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_call_root_task/Taskfile2.yml
+-rw-r--r--   0        0        0      173 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_cycle/Taskfile.yml
+-rw-r--r--   0        0        0      109 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_cycle/one/Taskfile.yml
+-rw-r--r--   0        0        0      109 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_cycle/one/two/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_deps/.gitignore
+-rw-r--r--   0        0        0      110 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_deps/Taskfile.yml
+-rw-r--r--   0        0        0      267 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_deps/Taskfile2.yml
+-rw-r--r--   0        0        0        9 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_empty/.gitignore
+-rw-r--r--   0        0        0       50 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_empty/Taskfile.yml
+-rw-r--r--   0        0        0      125 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_empty/Taskfile2.yml
+-rw-r--r--   0        0        0       51 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_incorrect/Taskfile.yml
+-rw-r--r--   0        0        0       28 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_incorrect/incomplete.yml
+-rw-r--r--   0        0        0      188 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_internal/Taskfile.yml
+-rw-r--r--   0        0        0       70 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_internal/Taskfile2.yml
+-rw-r--r--   0        0        0      196 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_interpolation/Taskfile.yml
+-rw-r--r--   0        0        0       66 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_interpolation/included/Taskfile.yml
+-rw-r--r--   0        0        0      161 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/Taskfile.yml
+-rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/called_one.txt
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/called_three.txt
+-rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/called_two.txt
+-rw-r--r--   0        0        0       85 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/one/Taskfile.yml
+-rw-r--r--   0        0        0      101 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/one/two/Taskfile.yml
+-rw-r--r--   0        0        0       62 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/one/two/three/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_optional/.gitignore
+-rw-r--r--   0        0        0      162 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_optional/Taskfile.yml
+-rw-r--r--   0        0        0      149 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_optional_explicit_false/Taskfile.yml
+-rw-r--r--   0        0        0      115 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_optional_implicit_false/Taskfile.yml
+-rw-r--r--   0        0        0      133 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_rel_path/Taskfile.yml
+-rw-r--r--   0        0        0       32 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_rel_path/common/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_rel_path/included/Taskfile.yml
+-rw-r--r--   0        0        0      129 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_shadowed_default/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_shadowed_default/Taskfile2.yml
+-rw-r--r--   0        0        0        9 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_shadowed_default/file.txt
+-rw-r--r--   0        0        0       64 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_unshadowed_default/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_unshadowed_default/Taskfile2.yml
+-rw-r--r--   0        0        0        9 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_unshadowed_default/file.txt
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_yaml/.gitignore
+-rw-r--r--   0        0        0      226 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_yaml/Custom.ext
+-rw-r--r--   0        0        0      115 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_yaml/included/Taskfile.yaml
+-rw-r--r--   0        0        0      109 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/includes_yaml/included/custom.yaml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/init/.gitignore
+-rw-r--r--   0        0        0      167 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/internal_task/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/label_list/Taskfile.yml
+-rw-r--r--   0        0        0       76 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/label_status/Taskfile.yml
+-rw-r--r--   0        0        0      104 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/label_summary/Taskfile.yml
+-rw-r--r--   0        0        0       82 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/label_uptodate/Taskfile.yml
+-rw-r--r--   0        0        0      105 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/label_var/Taskfile.yml
+-rw-r--r--   0        0        0       90 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/list_desc_interpolation/Taskfile.yml
+-rw-r--r--   0        0        0      164 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/list_mixed_desc/Taskfile.yml
+-rw-r--r--   0        0        0      199 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/output_group/Taskfile.yml
+-rw-r--r--   0        0        0      255 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/output_group_error_only/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/params/.gitignore
+-rw-r--r--   0        0        0     1255 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/params/Taskfile.yml
+-rw-r--r--   0        0        0     1584 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/platforms/Taskfile.yml
+-rw-r--r--   0        0        0      285 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/precondition/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/precondition/foo.txt
+-rw-r--r--   0        0        0      226 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/prompt/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/run/.gitignore
+-rw-r--r--   0        0        0      468 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/run/Taskfile.yml
+-rw-r--r--   0        0        0      201 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/shopts/command_level/Taskfile.yml
+-rw-r--r--   0        0        0      175 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/shopts/global_level/Taskfile.yml
+-rw-r--r--   0        0        0      183 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/shopts/task_level/Taskfile.yml
+-rw-r--r--   0        0        0      174 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/short_task_notation/Taskfile.yml
+-rw-r--r--   0        0        0     1350 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/silent/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/single_cmd_dep/.gitignore
+-rw-r--r--   0        0        0       99 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/single_cmd_dep/Taskfile.yml
+-rw-r--r--   0        0        0      282 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/special_vars/Taskfile.yml
+-rw-r--r--   0        0        0      214 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/special_vars/included/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/special_vars/subdir/.gitkeep
+-rw-r--r--   0        0        0       92 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/split_args/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/status/.gitignore
+-rw-r--r--   0        0        0      331 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/status/Taskfile.yml
+-rw-r--r--   0        0        0       14 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/status_vars/.gitignore
+-rw-r--r--   0        0        0      170 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/status_vars/Taskfile.yml
+-rw-r--r--   0        0        0       14 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/status_vars/source.txt
+-rw-r--r--   0        0        0      566 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/summary/Taskfile.yml
+-rw-r--r--   0        0        0      346 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/summary/task-with-summary.txt
+-rw-r--r--   0        0        0       78 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/taskfile_walk/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/taskfile_walk/foo/bar/.gitkeep
+-rw-r--r--   0        0        0       96 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/user_working_dir/Taskfile.yml
+-rw-r--r--   0        0        0       74 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/user_working_dir_with_includes/Taskfile.yml
+-rw-r--r--   0        0        0      101 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/user_working_dir_with_includes/included/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/user_working_dir_with_includes/somedir/.keep
+-rw-r--r--   0        0        0       27 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/.env
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/.gitignore
+-rw-r--r--   0        0        0     1008 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/Taskfile.yml
+-rw-r--r--   0        0        0     2188 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/any/Taskfile.yml
+-rw-r--r--   0        0        0     2385 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/any2/Taskfile.yml
+-rw-r--r--   0        0        0      276 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/any2/example.json
+-rw-r--r--   0        0        0      111 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/any2/example.yaml
+-rw-r--r--   0        0        0       93 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/version/v1/Taskfile.yml
+-rw-r--r--   0        0        0       93 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/version/v2/Taskfile.yml
+-rw-r--r--   0        0        0       93 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/version/v3/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/watcher_interval/.gitignore
+-rw-r--r--   0        0        0      194 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/watcher_interval/Taskfile.yaml
+-rw-r--r--   0        0        0      519 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/wildcards/Taskfile.yml
+-rw-r--r--   0        0        0     9862 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/variables.go
+-rw-r--r--   0        0        0     4215 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/watch.go
+-rw-r--r--   0        0        0     2041 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/watch_test.go
+-rw-r--r--   0        0        0      238 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/.nojekyll
+-rw-r--r--   0        0        0     1523 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/Taskfile.yml
+-rw-r--r--   0        0        0       70 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/babel.config.ts
+-rw-r--r--   0        0        0     6842 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/blog/2023-09-02-introducing-experiments.md
+-rw-r--r--   0        0        0      279 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/blog/authors.yml
+-rw-r--r--   0        0        0      242 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/constants.ts
+-rw-r--r--   0        0        0      359 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/crowdin.yml
+-rw-r--r--   0        0        0    41797 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/docs/api_reference.mdx
+-rw-r--r--   0        0        0    37809 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/docs/changelog.mdx
+-rw-r--r--   0        0        0     1529 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/community.mdx
+-rw-r--r--   0        0        0     7804 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/contributing.mdx
+-rw-r--r--   0        0        0      711 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/deprecations/deprecations.mdx
+-rw-r--r--   0        0        0      655 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/deprecations/template.mdx
+-rw-r--r--   0        0        0     1245 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/deprecations/version_2_schema.mdx
+-rw-r--r--   0        0        0     8037 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/experiments/any_variables.mdx
+-rw-r--r--   0        0        0     5677 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/experiments/experiments.mdx
+-rw-r--r--   0        0        0     1536 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/experiments/gentle_force.mdx
+-rw-r--r--   0        0        0     4244 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/experiments/remote_taskfiles.mdx
+-rw-r--r--   0        0        0     1124 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/experiments/template.mdx
+-rw-r--r--   0        0        0     2583 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/faq.mdx
+-rw-r--r--   0        0        0     6941 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/installation.mdx
+-rw-r--r--   0        0        0     2911 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/integrations.mdx
+-rw-r--r--   0        0        0     1993 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/intro.mdx
+-rw-r--r--   0        0        0     2797 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/releasing.mdx
+-rw-r--r--   0        0        0     2974 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/styleguide.mdx
+-rw-r--r--   0        0        0     5454 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/taskfile_versions.mdx
+-rw-r--r--   0        0        0      763 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/translate.mdx
+-rw-r--r--   0        0        0    45153 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/usage.mdx
+-rw-r--r--   0        0        0     6526 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docusaurus.config.ts
+-rw-r--r--   0        0        0     1508 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/package.json
+-rw-r--r--   0        0        0      208 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/prettier.config.js
+-rw-r--r--   0        0        0      271 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/sidebars.ts
+-rw-r--r--   0        0        0     1050 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/api/crowdin.js
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/components/.keep
+-rw-r--r--   0        0        0     1202 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/css/carbon.css
+-rw-r--r--   0        0        0     3089 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/css/custom.css
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/pages/.keep
+-rw-r--r--   0        0        0     1922 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/pages/donate.md
+-rw-r--r--   0        0        0     1342 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/themes/prismDark.js
+-rw-r--r--   0        0        0     1679 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/themes/prismLight.js
+-rw-r--r--   0        0        0        0 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/.nojekyll
+-rw-r--r--   0        0        0       13 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/CNAME
+-rw-r--r--   0        0        0      109 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/Taskfile.yml
+-rw-r--r--   0        0        0     7281 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/appwrite.svg
+-rw-r--r--   0        0        0   173915 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/favicon.ico
+-rw-r--r--   0        0        0     1321 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/icon-discord.svg
+-rw-r--r--   0        0        0     1227 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/icon-github.svg
+-rw-r--r--   0        0        0     1717 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/icon-mastodon.svg
+-rw-r--r--   0        0        0     1742 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/icon-twitter.svg
+-rw-r--r--   0        0        0    13524 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/logo.png
+-rw-r--r--   0        0        0      435 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/logo.svg
+-rw-r--r--   0        0        0      360 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/logo_mono.svg
+-rw-r--r--   0        0        0    19847 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/og-image.png
+-rw-r--r--   0        0        0     1276 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/pix.png
+-rwxr-xr-x   0        0        0     9634 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/install.sh
+-rw-r--r--   0        0        0      784 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/js/carbon.js
+-rw-r--r--   0        0        0    22415 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/schema.json
+-rw-r--r--   0        0        0       87 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/tsconfig.json
+-rw-r--r--   0        0        0    41797 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/api_reference.mdx
+-rw-r--r--   0        0        0    37809 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/changelog.mdx
+-rw-r--r--   0        0        0     1529 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/community.mdx
+-rw-r--r--   0        0        0     7804 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/contributing.mdx
+-rw-r--r--   0        0        0      711 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/deprecations.mdx
+-rw-r--r--   0        0        0      655 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/template.mdx
+-rw-r--r--   0        0        0     1245 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/version_2_schema.mdx
+-rw-r--r--   0        0        0     8037 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/any_variables.mdx
+-rw-r--r--   0        0        0     5677 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/experiments.mdx
+-rw-r--r--   0        0        0     1536 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/gentle_force.mdx
+-rw-r--r--   0        0        0     4244 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/remote_taskfiles.mdx
+-rw-r--r--   0        0        0     1124 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/template.mdx
+-rw-r--r--   0        0        0     2583 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/faq.mdx
+-rw-r--r--   0        0        0     6941 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/installation.mdx
+-rw-r--r--   0        0        0     2911 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/integrations.mdx
+-rw-r--r--   0        0        0     1993 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/intro.mdx
+-rw-r--r--   0        0        0     2797 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/releasing.mdx
+-rw-r--r--   0        0        0     2974 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/styleguide.mdx
+-rw-r--r--   0        0        0     5454 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/taskfile_versions.mdx
+-rw-r--r--   0        0        0      763 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/translate.mdx
+-rw-r--r--   0        0        0    45153 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/usage.mdx
+-rw-r--r--   0        0        0      174 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_sidebars/version-latest-sidebars.json
+-rw-r--r--   0        0        0       15 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versions.json
+-rw-r--r--   0        0        0   364377 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/yarn.lock
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 go_task_bin-3.36.0/PKG-INFO
```

### Comparing `go_task_bin-3.35.1/LICENSE` & `go_task_bin-3.36.0/LICENSE`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/README.md` & `go_task_bin-3.36.0/README.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/pyproject.toml` & `go_task_bin-3.36.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "go-task-bin"
 description = "task - A task runner / simpler Make alternative written in Go"
-version = "3.35.1"
+version = "3.36.0"
 authors = [
     { name = "dowon", email = "ks2515@naver.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
@@ -27,18 +27,20 @@
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/Bing-su/pip-binary-factory"
+taskfile = "https://taskfile.dev"
 
 [build-system]
 requires = [
     "pdm-backend",
+    "wheel",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.build]
 is-purelib = false
 source-includes = [
     "task/",
```

### Comparing `go_task_bin-3.35.1/task/.github/CODE_OF_CONDUCT.md` & `go_task_bin-3.36.0/task/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/.github/CONTRIBUTING.md` & `go_task_bin-3.36.0/task/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/.github/ISSUE_TEMPLATE/config.yml` & `go_task_bin-3.36.0/task/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/.github/workflows/issue-awaiting-response.yml` & `go_task_bin-3.36.0/task/.github/workflows/issue-awaiting-response.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/.github/workflows/issue-closed.yml` & `go_task_bin-3.36.0/task/.github/workflows/issue-closed.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/.github/workflows/issue-experiment.yml` & `go_task_bin-3.36.0/task/.github/workflows/issue-experiment.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/.github/workflows/issue-needs-triage.yml` & `go_task_bin-3.36.0/task/.github/workflows/issue-needs-triage.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/.github/workflows/lint.yml` & `go_task_bin-3.36.0/task/.github/workflows/lint.yml`

 * *Files 2% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 
       - uses: actions/checkout@v3
 
       - name: install check-jsonschema
         run: python -m pip install 'check-jsonschema==0.27.3'
 
       - name: check-jsonschema (metaschema)
-        run: check-jsonschema --check-metaschema docs/static/schema.json
+        run: check-jsonschema --check-metaschema website/static/schema.json
```

### Comparing `go_task_bin-3.35.1/task/.github/workflows/test.yml` & `go_task_bin-3.36.0/task/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/.github/workflows/upload-source-documents.yml` & `go_task_bin-3.36.0/task/.github/workflows/upload-source-documents.yml`

 * *Files 26% similar despite different names*

```diff
@@ -15,24 +15,24 @@
       - uses: actions/checkout@v2
 
       - name: Verify changed files
         id: changed-files
         uses: tj-actions/changed-files@v41
         with:
           files: |
-            docs/docs
-            docs/blog
-            docs/i18n/en
-            docs/src/pages
+            website/docs
+            website/blog
+            website/i18n/en
+            website/src/pages
 
       - name: Install Task
         uses: arduino/setup-task@v1
         with:
           version: 3.x
           repo-token: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Upload source documents
         if: steps.changed-files.outputs.any_changed == 'true'
         run: task crowdin:push
         env:
           CROWDIN_PERSONAL_TOKEN: ${{ secrets.CROWDIN_PERSONAL_TOKEN }}
-        working-directory: ./docs
+        working-directory: ./website
```

### Comparing `go_task_bin-3.35.1/task/.goreleaser.yml` & `go_task_bin-3.36.0/task/.goreleaser.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/CHANGELOG.md` & `go_task_bin-3.36.0/task/website/docs/changelog.mdx`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,34 @@
+---
+slug: /changelog/
+sidebar_position: 14
+---
+
 # Changelog
 
+## v3.36.0 - 2024-04-08
+
+- Added support for
+  [looping over dependencies](https://taskfile.dev/usage/#looping-over-dependencies)
+  (#1299, #1541 by @pd93).
+- When using the
+  "[Remote Taskfiles](https://taskfile.dev/experiments/remote-taskfiles/)"
+  experiment, you are now able to use
+  [remote Taskfiles as your entrypoint](https://taskfile.dev/experiments/remote-taskfiles/#root-remote-taskfiles).
+  - `includes` in remote Taskfiles will now also resolve correctly (#1347 by
+    @pd93).
+- When using the
+  "[Any Variables](https://taskfile.dev/experiments/any-variables/)"
+  experiments, templating is now supported in collection-type variables (#1477,
+  #1511, #1526 by @pd93).
+- Fixed a bug where variables being passed to an included Taskfile were not
+  available when defining global variables (#1503, #1533 by @pd93).
+- Improved support to customized colors by allowing 8-bit colors and multiple
+  ANSI attributes (#1576 by @pd93).
+
 ## v3.35.1 - 2024-03-04
 
 - Fixed a bug where the `TASKFILE_DIR` variable was sometimes incorrect (#1522,
   #1523 by @pd93).
 - Added a new `TASKFILE` special variable that holds the root Taskfile path
   (#1523 by @pd93).
 - Fixed various issues related to running a Taskfile from a subdirectory (#1529,
```

### Comparing `go_task_bin-3.35.1/task/LICENSE` & `go_task_bin-3.36.0/task/LICENSE`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/README.md` & `go_task_bin-3.36.0/task/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
   <a href="https://taskfile.dev">
-    <img src="docs/static/img/logo.svg" width="200px" height="200px" />
+    <img src="website/static/img/logo.svg" width="200px" height="200px" />
   </a>
 
   <h1>Task</h1>
 
   <p>
     Task is a task runner / build tool that aims to be simpler and easier to use than, for example, <a href="https://www.gnu.org/software/make/">GNU Make<a>.
   </p>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
-                          _[_d_o_c_s_/_s_t_a_t_i_c_/_i_m_g_/_l_o_g_o_._s_v_g_]
+                         _[_w_e_b_s_i_t_e_/_s_t_a_t_i_c_/_i_m_g_/_l_o_g_o_._s_v_g_]
                               ************ TTaasskk ************
  Task is a task runner / build tool that aims to be simpler and easier to use
                          than, for example, _G_N_U_ _M_a_k_e_.
           _I_n_s_t_a_l_l_a_t_i_o_n | _D_o_c_u_m_e_n_t_a_t_i_o_n | _T_w_i_t_t_e_r | _M_a_s_t_o_d_o_n | _D_i_s_c_o_r_d
```

### Comparing `go_task_bin-3.35.1/task/Taskfile.yml` & `go_task_bin-3.36.0/task/Taskfile.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 version: '3'
 
 includes:
-  docs:
-    aliases: [d]
-    taskfile: ./docs
-    dir: ./docs
+  website:
+    aliases: [w, docs, d]
+    taskfile: ./website
+    dir: ./website
 
 vars:
   BIN: "{{.ROOT_DIR}}/bin"
 
 env:
   CGO_ENABLED: '0'
```

### Comparing `go_task_bin-3.35.1/task/args/args.go` & `go_task_bin-3.36.0/task/args/args.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/args/args_test.go` & `go_task_bin-3.36.0/task/args/args_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/cmd/release/main.go` & `go_task_bin-3.36.0/task/cmd/release/main.go`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 	"os"
 	"os/exec"
 	"regexp"
 	"strings"
 	"time"
 
 	"github.com/Masterminds/semver/v3"
+	"github.com/otiai10/copy"
 )
 
 const (
 	changelogSource = "CHANGELOG.md"
-	changelogTarget = "docs/docs/changelog.md"
+	changelogTarget = "website/docs/changelog.mdx"
+	docsSource      = "website/docs"
+	docsTarget      = "website/versioned_docs/version-latest"
 )
 
 var (
 	changelogReleaseRegex = regexp.MustCompile(`## Unreleased`)
 	versionRegex          = regexp.MustCompile(`(?m)^  "version": "\d+\.\d+\.\d+",$`)
 )
 
@@ -53,14 +56,18 @@
 		return err
 	}
 
 	if err := setJSONVersion("package-lock.json", version); err != nil {
 		return err
 	}
 
+	if err := docs(); err != nil {
+		return err
+	}
+
 	return nil
 }
 
 func getVersion() (*semver.Version, error) {
 	cmd := exec.Command("git", "describe", "--tags", "--abbrev=0")
 	b, err := cmd.Output()
 	if err != nil {
@@ -131,7 +138,17 @@
 
 	// Replace the version
 	new := versionRegex.ReplaceAllString(string(b), fmt.Sprintf(`  "version": "%s",`, version.String()))
 
 	// Write the JSON file
 	return os.WriteFile(fileName, []byte(new), 0o644)
 }
+
+func docs() error {
+	if err := os.RemoveAll(docsTarget); err != nil {
+		return err
+	}
+	if err := copy.Copy(docsSource, docsTarget); err != nil {
+		return err
+	}
+	return nil
+}
```

### Comparing `go_task_bin-3.35.1/task/cmd/sleepit/sleepit.go` & `go_task_bin-3.36.0/task/cmd/sleepit/sleepit.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/cmd/task/task.go` & `go_task_bin-3.36.0/task/cmd/task/task.go`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 package main
 
 import (
 	"context"
 	"fmt"
 	"log"
 	"os"
-	"path/filepath"
 	"strings"
 
 	"github.com/spf13/pflag"
 	"mvdan.cc/sh/v3/syntax"
 
 	"github.com/go-task/task/v3"
 	"github.com/go-task/task/v3/args"
@@ -90,19 +89,14 @@
 		home, err := os.UserHomeDir()
 		if err != nil {
 			return fmt.Errorf("task: Failed to get user home directory: %w", err)
 		}
 		dir = home
 	}
 
-	if entrypoint != "" {
-		dir = filepath.Dir(entrypoint)
-		entrypoint = filepath.Base(entrypoint)
-	}
-
 	var taskSorter sort.TaskSorter
 	switch flags.TaskSort {
 	case "none":
 		taskSorter = &sort.Noop{}
 	case "alphanumeric":
 		taskSorter = &sort.AlphaNumeric{}
 	}
```

### Comparing `go_task_bin-3.35.1/task/completion/bash/task.bash` & `go_task_bin-3.36.0/task/completion/bash/task.bash`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/completion/fish/task.fish` & `go_task_bin-3.36.0/task/completion/fish/task.fish`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/completion/ps/task.ps1` & `go_task_bin-3.36.0/task/completion/ps/task.ps1`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/completion/zsh/_task` & `go_task_bin-3.36.0/task/completion/zsh/_task`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/Taskfile.yml` & `go_task_bin-3.36.0/task/website/Taskfile.yml`

 * *Files 10% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     summary: Requires GIT_USER and GIT_PASS envs to be previous set
     cmds:
       - npx docusaurus deploy
 
   upgrade:
     desc: Upgrade Docusaurus
     cmds:
-      - yarn upgrade @docusaurus/core@latest @docusaurus/preset-classic@latest @docusaurus/module-type-aliases@latest
+      - yarn upgrade @docusaurus/core@latest @docusaurus/preset-classic@latest @docusaurus/module-type-aliases@latest @docusaurus/tsconfig@latest @docusaurus/types@latest
 
   crowdin:push:
     desc: Upload source files to a Crowdin project
     deps: [yarn:install]
     cmds:
       - npx crowdin push
```

### Comparing `go_task_bin-3.35.1/task/docs/blog/2023-09-02-introducing-experiments.md` & `go_task_bin-3.36.0/task/website/blog/2023-09-02-introducing-experiments.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/docs/api_reference.md` & `go_task_bin-3.36.0/task/website/docs/api_reference.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,25 @@
 | `TASK_COLOR_GREEN`   | `32`    | Color used for green.                                                                                             |
 | `TASK_COLOR_CYAN`    | `36`    | Color used for cyan.                                                                                              |
 | `TASK_COLOR_YELLOW`  | `33`    | Color used for yellow.                                                                                            |
 | `TASK_COLOR_MAGENTA` | `35`    | Color used for magenta.                                                                                           |
 | `TASK_COLOR_RED`     | `31`    | Color used for red.                                                                                               |
 | `FORCE_COLOR`        |         | Force color output usage.                                                                                         |
 
+All color variables are [ANSI color codes][ansi]. You can specify multiple codes
+separated by a semicolon. For example: `31;1` will make the text bold and red.
+Task also supports 8-bit color (256 colors). You can specify these colors by
+using the sequence `38;2;R:G:B` for foreground colors and `48;2;R:G:B` for
+background colors where `R`, `G` and `B` should be replaced with values between
+0 and 255.
+
+For convenience, we allow foreground colors to be specified using shorthand,
+comma-separated syntax: `R,G,B`. For example, `255,0,0` is equivalent to
+`38;2;255:0:0`.
+
 ## Taskfile Schema
 
 | Attribute  | Type                               | Default       | Description                                                                                                                                                            |
 | ---------- | ---------------------------------- | ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `version`  | `string`                           |               | Version of the Taskfile. The current version is `3`.                                                                                                                   |
 | `output`   | `string`                           | `interleaved` | Output mode. Available options: `interleaved`, `group` and `prefixed`.                                                                                                 |
 | `method`   | `string`                           | `checksum`    | Default method in this Taskfile. Can be overridden in a task by task basis. Available options: `checksum`, `timestamp` and `none`.                                     |
@@ -369,7 +380,11 @@
 :::
 
 #### Requires
 
 | Attribute | Type       | Default | Description                                                                                        |
 | --------- | ---------- | ------- | -------------------------------------------------------------------------------------------------- |
 | `vars`    | `[]string` |         | List of variable or environment variable names that must be set if this task is to execute and run |
+
+{/* prettier-ignore-start */}
+[ansi]: https://en.wikipedia.org/wiki/ANSI_escape_code
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/changelog.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/changelog.mdx`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,34 @@
 ---
 slug: /changelog/
 sidebar_position: 14
 ---
 
 # Changelog
 
+## v3.36.0 - 2024-04-08
+
+- Added support for
+  [looping over dependencies](https://taskfile.dev/usage/#looping-over-dependencies)
+  (#1299, #1541 by @pd93).
+- When using the
+  "[Remote Taskfiles](https://taskfile.dev/experiments/remote-taskfiles/)"
+  experiment, you are now able to use
+  [remote Taskfiles as your entrypoint](https://taskfile.dev/experiments/remote-taskfiles/#root-remote-taskfiles).
+  - `includes` in remote Taskfiles will now also resolve correctly (#1347 by
+    @pd93).
+- When using the
+  "[Any Variables](https://taskfile.dev/experiments/any-variables/)"
+  experiments, templating is now supported in collection-type variables (#1477,
+  #1511, #1526 by @pd93).
+- Fixed a bug where variables being passed to an included Taskfile were not
+  available when defining global variables (#1503, #1533 by @pd93).
+- Improved support to customized colors by allowing 8-bit colors and multiple
+  ANSI attributes (#1576 by @pd93).
+
 ## v3.35.1 - 2024-03-04
 
 - Fixed a bug where the `TASKFILE_DIR` variable was sometimes incorrect (#1522,
   #1523 by @pd93).
 - Added a new `TASKFILE` special variable that holds the root Taskfile path
   (#1523 by @pd93).
 - Fixed various issues related to running a Taskfile from a subdirectory (#1529,
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/community.md` & `go_task_bin-3.36.0/task/website/docs/community.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/docs/contributing.md` & `go_task_bin-3.36.0/task/website/docs/contributing.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -68,29 +68,29 @@
 `task package` which will generate a `.vsix` file that can be used to manually
 install the extension.
 
 ### Updating documentation
 
 Task uses [Docusaurus][docusaurus] to host a documentation server. The code for
 this is located in the core Task repository. This can be setup and run locally
-by using `task docs` (requires `nodejs` & `yarn`). All content is written in
-Markdown and is located in the `docs/docs` directory. All Markdown documents
+by using `task website` (requires `nodejs` & `yarn`). All content is written in
+Markdown and is located in the `website/docs` directory. All Markdown documents
 should have an 80 character line wrap limit (enforced by Prettier).
 
-When making a change, consider whether a change to the [Usage
-Guide](/usage) is necessary. This document contains descriptions and
-examples of how to use Task features. If you're adding a new feature, try to
-find an appropriate place to add a new section. If you're updating an existing
-feature, ensure that the documentation and any examples are up-to-date. Ensure
-that any examples follow the [Taskfile Styleguide](/styleguide).
+When making a change, consider whether a change to the [Usage Guide](/usage) is
+necessary. This document contains descriptions and examples of how to use Task
+features. If you're adding a new feature, try to find an appropriate place to
+add a new section. If you're updating an existing feature, ensure that the
+documentation and any examples are up-to-date. Ensure that any examples follow
+the [Taskfile Styleguide](/styleguide).
 
 If you added a new field, command or flag, ensure that you add it to the
-[API Reference](/api). New fields also need to be added to the
-[JSON Schema][json-schema]. The descriptions for fields in the API reference and
-the schema should match.
+[API Reference](/api). New fields also need to be added to the [JSON
+Schema][json-schema]. The descriptions for fields in the API reference and the
+schema should match.
 
 ### Writing tests
 
 A lot of Task's tests are held in the `task_test.go` file in the project root
 and this is where you'll most likely want to add new ones too. Most of these
 tests also have a subdirectory in the `testdata` directory where any
 Taskfiles/data required to run the tests are stored.
@@ -143,25 +143,25 @@
 > I'm stuck, where can I get help?
 
 If you have questions, feel free to ask them in the `#help` forum channel on our
 [Discord server][discord-server] or open a [Discussion][discussion] on GitHub.
 
 ---
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [task]: https://github.com/go-task/task
 [vscode-task]: https://github.com/go-task/vscode-task
 [go]: https://go.dev
 [gofumpt]: https://github.com/mvdan/gofumpt
 [golangci-lint]: https://golangci-lint.run
 [prettier]: https://prettier.io
 [nodejs]: https://nodejs.org/en/
 [yarn]: https://yarnpkg.com/
 [docusaurus]: https://docusaurus.io
-[json-schema]: https://github.com/go-task/task/blob/main/docs/static/schema.json
+[json-schema]: https://github.com/go-task/task/blob/main/website/static/schema.json
 [task-open-issues]: https://github.com/go-task/task/issues
 [vscode-task-open-issues]: https://github.com/go-task/vscode-task/issues
 [good-first-issue]: https://github.com/go-task/task/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22
 [discord-server]: https://discord.gg/6TY36E39UK
 [discussion]: https://github.com/go-task/task/discussions
 [conventional-commits]: https://www.conventionalcommits.org
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/deprecations/deprecations.md` & `go_task_bin-3.36.0/task/website/docs/deprecations/deprecations.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/docs/deprecations/template.md` & `go_task_bin-3.36.0/task/website/docs/deprecations/template.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/docs/deprecations/version_2_schema.md` & `go_task_bin-3.36.0/task/website/docs/deprecations/version_2_schema.mdx`

 * *Files 3% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 
 In December 2023, the final version of Task that supports the version 2 schema
 ([v3.33.0][v3.33.0]) was published and all legacy code was removed from Task's
 main branch. To use a more recent version of Task, you will need to ensure that
 your Taskfile uses the version 3 schema instead. A list of changes between
 version 2 and version 3 are available in the [Task v3 Release Notes][v3.0.0].
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [v3.0.0]: https://github.com/go-task/task/releases/tag/v3.0.0
 [v3.33.0]: https://github.com/go-task/task/releases/tag/v3.33.0
 [deprecation-notice]: https://github.com/go-task/task/issues/1197
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/donate.md` & `go_task_bin-3.36.0/task/website/src/pages/donate.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ---
 slug: /donate/
-sidebar_position: 16
+hide_table_of_contents: true
 ---
 
 # Donate
 
 If you find this project useful, you can consider donating by using one of the
 channels listed below.
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/experiments/any_variables.mdx` & `go_task_bin-3.36.0/task/website/docs/experiments/any_variables.mdx`

 * *Files 4% similar despite different names*

```diff
@@ -336,11 +336,11 @@
         cmd: echo {{.ITEM}}
 ```
 
 When looping over a map we also make an additional `{{.KEY}}` variable availabe
 that holds the string value of the map key. Remember that maps are unordered, so
 the order in which the items are looped over is random.
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [enabling-experiments]: /experiments/#enabling-experiments
 [slim-sprig]: https://go-task.github.io/slim-sprig/
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/experiments/experiments.md` & `go_task_bin-3.36.0/task/website/docs/experiments/experiments.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/docs/experiments/gentle_force.md` & `go_task_bin-3.36.0/task/website/docs/experiments/gentle_force.mdx`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 - The `--force` flag
 
 :::
 
 :::info
 
-To enable this experiment, set the environment variable: `TASK_X_FORCE=1`. Check
-out [our guide to enabling experiments ][enabling-experiments] for more
-information.
+To enable this experiment, set the environment variable:
+`TASK_X_GENTLE_FORCE=1`. Check out [our guide to enabling experiments
+][enabling-experiments] for more information.
 
 :::
 
 The `--force` flag currently forces _all_ tasks to run regardless of the status
 checks. This can be useful, but we have found that most of the time users only
 expect the direct task they are calling to be forced and _not_ all of its
 dependant tasks.
@@ -40,10 +40,10 @@
 functionality.
 
 If you want to migrate, but continue to force all dependant tasks to run, you
 should replace all uses of the `--force` flag with `--force-all`. Alternatively,
 if you want to adopt the new behavior, you can continue to use the `--force`
 flag as you do now!
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [enabling-experiments]: /experiments/#enabling-experiments
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/experiments/remote_taskfiles.md` & `go_task_bin-3.36.0/task/website/docs/experiments/remote_taskfiles.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -76,18 +76,17 @@
 2. Consider using a pinned version of the remote Taskfile (e.g. A link
    containing a commit hash) to prevent Task from automatically accepting a
    prompt that says a remote Taskfile has changed.
 
 Task currently supports both `http` and `https` URLs. However, the `http`
 requests will not execute by default unless you run the task with the
 `--insecure` flag. This is to protect you from accidentally running a remote
-Taskfile that is hosted on and unencrypted connection. Sources that are not
-protected by TLS are vulnerable to [man-in-the-middle
-attacks][man-in-the-middle-attacks] and should be avoided unless you know what
-you are doing.
+Taskfile that is via an unencrypted connection. Sources that are not protected
+by TLS are vulnerable to [man-in-the-middle attacks][man-in-the-middle-attacks]
+and should be avoided unless you know what you are doing.
 
 ## Caching & Running Offline
 
 Whenever you run a remote Taskfile, the latest copy will be downloaded from the
 internet and cached locally. If for whatever reason, you lose access to the
 internet, you will still be able to run your tasks by specifying the `--offline`
 flag. This will tell Task to use the latest cached version of the file instead
@@ -95,11 +94,11 @@
 the cached version of the remote files without running any tasks.
 
 By default, Task will timeout requests to download remote files after 10 seconds
 and look for a cached copy instead. This timeout can be configured by setting
 the `--timeout` flag and specifying a duration. For example, `--timeout 5s` will
 set the timeout to 5 seconds.
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [enabling-experiments]: /experiments/#enabling-experiments
 [man-in-the-middle-attacks]: https://en.wikipedia.org/wiki/Man-in-the-middle_attack
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/experiments/template.md` & `go_task_bin-3.36.0/task/website/docs/experiments/template.mdx`

 * *Files 18% similar despite different names*

```diff
@@ -33,10 +33,10 @@
 
 :::
 
 \{Short description of the feature\}
 
 \{Short explanation of how users should migrate to the new behavior\}
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [enabling-experiments]: /experiments/#enabling-experiments
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/faq.md` & `go_task_bin-3.36.0/task/website/docs/faq.mdx`

 * *Files 10% similar despite different names*

```diff
@@ -91,11 +91,11 @@
 We want to make improvements to this part of Task and the issues below track
 this work. Constructive comments and contributions are very welcome!
 
 - #197
 - [mvdan/sh#93](https://github.com/mvdan/sh/issues/93)
 - [mvdan/sh#97](https://github.com/mvdan/sh/issues/97)
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [git-bash]: https://gitforwindows.org/
 [wsl]: https://learn.microsoft.com/en-us/windows/wsl/install
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/installation.md` & `go_task_bin-3.36.0/task/website/docs/installation.mdx`

 * *Files 6% similar despite different names*

```diff
@@ -25,31 +25,31 @@
 [on the official Homebrew repository](https://formulae.brew.sh/formula/go-task),
 so you also have that option if you prefer:
 
 ```shell
 brew install go-task
 ```
 
-### Tea
+### pkgx
 
-If you're on macOS or Linux and have [tea][tea] installed, getting Task is as
+If you're on macOS or Linux and have [pkgx](https://pkgx.sh/) installed, getting Task is as
 simple as running:
 
 ```shell
-tea task
+pkgx task
 ```
 
-or, if you have tea’s magic enabled:
+or, if you have pkgx integration enabled:
 
 ```shell
 task
 ```
 
 This installation method is community owned. After a new release of Task, they
-are automatically released by tea in a minimum of time.
+are automatically released by pkgx in a minimum of time.
 
 ### Snap
 
 Task is available in [Snapcraft][snapcraft], but keep in mind that your Linux
 distribution should allow classic confinement for Snaps to Task work right:
 
 ```shell
@@ -286,18 +286,18 @@
 
 Add the line and save the file:
 
 ```shell
 Invoke-Expression -Command path/to/task.ps1
 ```
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [go]: https://golang.org/
 [snapcraft]: https://snapcraft.io/task
 [homebrew]: https://brew.sh/
 [installscript]: https://github.com/go-task/task/blob/main/install-task.sh
 [releases]: https://github.com/go-task/task/releases
 [godownloader]: https://github.com/goreleaser/godownloader
 [choco]: https://chocolatey.org/
 [scoop]: https://scoop.sh/
 [tea]: https://tea.xyz/
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/integrations.md` & `go_task_bin-3.36.0/task/website/docs/integrations.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ![Task for Visual Studio Code](https://github.com/go-task/vscode-task/blob/main/res/preview.png?raw=true)
 
 ## Schema
 
 This was initially created by @KROSF in
 [this Gist](https://gist.github.com/KROSF/c5435acf590acd632f71bb720f685895) and
 is now officially maintained in
-[this file](https://github.com/go-task/task/blob/main/docs/static/schema.json)
+[this file](https://github.com/go-task/task/blob/main/website/static/schema.json)
 and made available at https://taskfile.dev/schema.json. This schema can be used
 to validate Taskfiles and provide autocompletion in many code editors:
 
 ### Visual Studio Code
 
 To integrate the schema into VS Code, you need to install the
 [YAML extension](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml)
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/intro.md` & `go_task_bin-3.36.0/task/website/docs/intro.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ---
 slug: /
 sidebar_position: 1
 title: Home
+hide_title: true
 ---
 
-# Task
-
 <div align="center">
-  <img id="logo" src="img/logo.svg" height="250px" width="250px" />
+  <img id="logo" src="/img/logo.svg" height="250px" width="250px" />
 </div>
+<br />
 
 Task is a task runner / build tool that aims to be simpler and easier to use
 than, for example, [GNU Make][make].
 
 Since it's written in [Go][go], Task is just a single binary and has no other
 dependencies, which means you don't need to mess with any complicated install
 setups just to use a build tool.
@@ -46,16 +46,16 @@
 - Truly cross-platform: while most build tools only work well on Linux or macOS,
   Task also supports Windows thanks to [this shell interpreter for Go][sh].
 - Great for code generation: you can easily
   [prevent a task from running](/usage#prevent-unnecessary-work) if a given set
   of files haven't changed since last run (based either on its timestamp or
   content).
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [make]: https://www.gnu.org/software/make/
 [go]: https://go.dev/
 [yaml]: http://yaml.org/
 [homebrew]: https://brew.sh/
 [snapcraft]: https://snapcraft.io/
 [scoop]: https://scoop.sh/
 [sh]: https://github.com/mvdan/sh
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/releasing.md` & `go_task_bin-3.36.0/task/website/docs/releasing.mdx`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 # Nix
 
 Nix is a community owned installation method. Nix package maintainers usually
 take care of updating versions there by editing
 [this file](https://github.com/NixOS/nixpkgs/blob/nixos-unstable/pkgs/development/tools/go-task/default.nix).
 If you think its Task version is outdated, open an issue to let us know.
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [goreleaser]: https://goreleaser.com/
 [homebrewtap]: https://github.com/go-task/homebrew-tap
 [gotaskrb]: https://github.com/go-task/homebrew-tap/blob/main/Formula/go-task.rb
 [packagejson]: https://github.com/go-task/task/blob/main/package.json#L3
 [snappackage]: https://github.com/go-task/snap
 [snapcraftyaml]: https://github.com/go-task/snap/blob/main/snap/snapcraft.yaml#L2
 [snapcraftdashboard]: https://snapcraft.io/task/releases
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/styleguide.md` & `go_task_bin-3.36.0/task/website/docs/styleguide.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/docs/taskfile_versions.md` & `go_task_bin-3.36.0/task/website/docs/taskfile_versions.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -251,13 +251,13 @@
 The variable priority order was also different:
 
 1. Call variables
 2. Environment
 3. Task variables
 4. `Taskvars.yml` variables
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [deprecate-version-2-schema]: /deprecations/version-2-schema/
 [output]: /usage#output-syntax
 [ignore_errors]: /usage#ignore-errors
 [includes]: /usage#including-other-taskfiles
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/translate.md` & `go_task_bin-3.36.0/task/website/docs/translate.mdx`

 * *Files 4% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 is periodically updated with progress from Crowdin.
 
 If you want to have access to the Crowdin project to be able to suggest
 translations, please ask for access on the [#translations channel on our Discord
 server][discord]. If a given language is not being shown to Crowdin yet, just
 ask and we can configure it.
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [crowdin]: https://crowdin.com/project/taskfile
 [discord]: https://discord.gg/6TY36E39UK
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docs/usage.md` & `go_task_bin-3.36.0/task/website/docs/usage.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -1193,14 +1193,51 @@
       - echo 'foo'
 
   task-bar:
     cmds:
       - echo 'bar'
 ```
 
+### Looping over dependencies
+
+All of the above looping techniques can also be applied to the `deps` property.
+This allows you to combine loops with concurrency:
+
+```yaml
+version: '3'
+
+tasks:
+  default:
+    deps:
+      - for: [foo, bar]
+        task: my-task
+        vars:
+          FILE: '{{.ITEM}}'
+
+  my-task:
+    cmds:
+      - echo '{{.FILE}}'
+```
+
+It is important to note that as `deps` are run in parallel, the order in which
+the iterations are run is not guaranteed and the output may vary. For example,
+the output of the above example may be either:
+
+```shell
+foo
+bar
+```
+
+or
+
+```shell
+bar
+foo
+```
+
 ## Forwarding CLI arguments to commands
 
 If `--` is given in the CLI, all following parameters are added to a special
 `.CLI_ARGS` variable. This is useful to forward arguments to another command.
 
 The below example will run `yarn install`.
 
@@ -1913,10 +1950,10 @@
 
 Note that when setting `watch: true` to a task, it'll only run in watch mode
 when running from the CLI via `task my-watch-task`, but won't run in watch mode
 if called by another task, either directly or as a dependency.
 
 :::
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [gotemplate]: https://golang.org/pkg/text/template/
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/docusaurus.config.ts` & `go_task_bin-3.36.0/task/website/docusaurus.config.ts`

 * *Files 8% similar despite different names*

```diff
@@ -88,15 +88,27 @@
   presets: [
     [
       'classic',
       {
         docs: {
           routeBasePath: '/',
           sidebarPath: './sidebars.ts',
-          remarkPlugins: [remarkGithub, remarkGfm]
+          remarkPlugins: [remarkGithub, remarkGfm],
+          includeCurrentVersion: true,
+          versions: {
+            current: {
+              label: `Next 🚧`,
+              path: 'next',
+              badge: false
+            },
+            latest: {
+              label: 'Latest',
+              badge: false
+            }
+          }
         },
         blog: {},
         theme: {
           customCss: [
             './src/css/custom.css',
             './src/css/carbon.css',
           ]
@@ -133,71 +145,63 @@
       logo: {
         alt: 'Task Logo',
         src: 'img/logo.svg'
       },
       items: [
         {
           type: 'doc',
-          docId: 'installation',
-          position: 'left',
-          label: 'Installation'
-        },
-        {
-          type: 'doc',
-          docId: 'usage',
+          docId: 'intro',
           position: 'left',
-          label: 'Usage'
-        },
-        {
-          type: 'doc',
-          docId: 'api_reference',
-          position: 'left',
-          label: 'API'
+          label: 'Docs'
         },
         {
           to: 'blog',
           label: 'Blog',
           position: 'left'
         },
         {
-          type: 'doc',
-          docId: 'donate',
+          to: '/donate',
           position: 'left',
           label: 'Donate'
         },
         {
+          type: 'docsVersionDropdown',
+          position: 'right',
+          dropdownActiveClassDisabled: true,
+        },
+        {
           type: 'localeDropdown',
-          position: 'left',
+          position: 'right',
           dropdownItemsAfter: [
             {
               to: '/translate/',
               label: 'Help Us Translate'
             }
           ]
         },
         {
           href: GITHUB_URL,
-          label: 'GitHub',
-          position: 'right'
+          position: 'right',
+          className: "header-icon-link icon-github",
+        },
+        {
+          href: DISCORD_URL,
+          position: 'right',
+          className: "header-icon-link icon-discord",
         },
         {
           href: TWITTER_URL,
-          label: 'Twitter',
-          position: 'right'
+          position: 'right',
+          className: "header-icon-link icon-twitter",
         },
         {
           href: MASTODON_URL,
-          label: 'Mastodon',
           rel: 'me',
-          position: 'right'
-        },
-        {
-          href: DISCORD_URL,
-          label: 'Discord',
-          position: 'right'
+          position: 'right',
+          className: "header-icon-link icon-mastodon",
         }
       ]
     },
     footer: {
       style: 'dark',
       links: [
         {
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/api_reference.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/api_reference.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -7,57 +7,59 @@
 
 # API Reference
 
 ## CLI
 
 Task command line tool has the following syntax:
 
-```bash
+```shell
 task [--flags] [tasks...] [-- CLI_ARGS...]
 ```
 
 :::tip
 
-If `--` is given, all remaining arguments will be assigned to a special `CLI_ARGS` variable
+If `--` is given, all remaining arguments will be assigned to a special
+`CLI_ARGS` variable
 
 :::
 
-| Short | Flag                        | Type     | Default                                      | Description                                                                                                                                                                                                    |
-| ----- | --------------------------- | -------- | -------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `-c`  | `--color`                   | `bool`   | `true`                                       | Colored output. Enabled by default. Set flag to `false` or use `NO_COLOR=1` to disable.                                                                                                                        |
-| `-C`  | `--concurrency`             | `int`    | `0`                                          | Limit number tasks to run concurrently. Zero means unlimited.                                                                                                                                                  |
-| `-d`  | `--dir`                     | `string` | Working directory                            | Sets directory of execution.                                                                                                                                                                                   |
-| `-n`  | `--dry`                     | `bool`   | `false`                                      | Compiles and prints tasks in the order that they would be run, without executing them.                                                                                                                         |
-| `-x`  | `--exit-code`               | `bool`   | `false`                                      | Pass-through the exit code of the task command.                                                                                                                                                                |
-| `-f`  | `--force`                   | `bool`   | `false`                                      | Forces execution even when the task is up-to-date.                                                                                                                                                             |
-| `-g`  | `--global`                  | `bool`   | `false`                                      | Runs global Taskfile, from `$HOME/Taskfile.{yml,yaml}`.                                                                                                                                                        |
-| `-h`  | `--help`                    | `bool`   | `false`                                      | Shows Task usage.                                                                                                                                                                                              |
-| `-i`  | `--init`                    | `bool`   | `false`                                      | Creates a new Taskfile.yml in the current folder.                                                                                                                                                              |
-| `-I`  | `--interval`                | `string` | `5s`                                         | Sets a different watch interval when using `--watch`, the default being 5 seconds. This string should be a valid [Go Duration](https://pkg.go.dev/time#ParseDuration).                                         |
-| `-l`  | `--list`                    | `bool`   | `false`                                      | Lists tasks with description of current Taskfile.                                                                                                                                                              |
-| `-a`  | `--list-all`                | `bool`   | `false`                                      | Lists tasks with or without a description.                                                                                                                                                                     |
+| Short | Flag                        | Type     | Default                                      | Description                                                                                                                                                                                  |
+| ----- | --------------------------- | -------- | -------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `-c`  | `--color`                   | `bool`   | `true`                                       | Colored output. Enabled by default. Set flag to `false` or use `NO_COLOR=1` to disable.                                                                                                      |
+| `-C`  | `--concurrency`             | `int`    | `0`                                          | Limit number tasks to run concurrently. Zero means unlimited.                                                                                                                                |
+| `-d`  | `--dir`                     | `string` | Working directory                            | Sets directory of execution.                                                                                                                                                                 |
+| `-n`  | `--dry`                     | `bool`   | `false`                                      | Compiles and prints tasks in the order that they would be run, without executing them.                                                                                                       |
+| `-x`  | `--exit-code`               | `bool`   | `false`                                      | Pass-through the exit code of the task command.                                                                                                                                              |
+| `-f`  | `--force`                   | `bool`   | `false`                                      | Forces execution even when the task is up-to-date.                                                                                                                                           |
+| `-g`  | `--global`                  | `bool`   | `false`                                      | Runs global Taskfile, from `$HOME/Taskfile.{yml,yaml}`.                                                                                                                                      |
+| `-h`  | `--help`                    | `bool`   | `false`                                      | Shows Task usage.                                                                                                                                                                            |
+| `-i`  | `--init`                    | `bool`   | `false`                                      | Creates a new Taskfile.yml in the current folder.                                                                                                                                            |
+| `-I`  | `--interval`                | `string` | `5s`                                         | Sets a different watch interval when using `--watch`, the default being 5 seconds. This string should be a valid [Go Duration](https://pkg.go.dev/time#ParseDuration).                       |
+| `-l`  | `--list`                    | `bool`   | `false`                                      | Lists tasks with description of current Taskfile.                                                                                                                                            |
+| `-a`  | `--list-all`                | `bool`   | `false`                                      | Lists tasks with or without a description.                                                                                                                                                   |
 |       | `--sort`                    | `string` | `default`                                    | Changes the order of the tasks when listed.<br />`default` - Alphanumeric with root tasks first<br />`alphanumeric` - Alphanumeric<br />`none` - No sorting (As they appear in the Taskfile) |
-|       | `--json`                    | `bool`   | `false`                                      | See [JSON Output](#json-output)                                                                                                                                                                                |
-| `-o`  | `--output`                  | `string` | Default set in the Taskfile or `intervealed` | Sets output style: [`interleaved`/`group`/`prefixed`].                                                                                                                                                         |
-|       | `--output-group-begin`      | `string` |                                              | Message template to print before a task's grouped output.                                                                                                                                                      |
-|       | `--output-group-end`        | `string` |                                              | Message template to print after a task's grouped output.                                                                                                                                                       |
-|       | `--output-group-error-only` | `bool`   | `false`                                      | Swallow command output on zero exit code.                                                                                                                                                                      |
-| `-p`  | `--parallel`                | `bool`   | `false`                                      | Executes tasks provided on command line in parallel.                                                                                                                                                           |
-| `-s`  | `--silent`                  | `bool`   | `false`                                      | Disables echoing.                                                                                                                                                                                              |
-| `-y`  | `--yes`                     | `bool`   | `false`                                      | Assume "yes" as answer to all prompts.                                                                                                                                                                         |
-|       | `--status`                  | `bool`   | `false`                                      | Exits with non-zero exit code if any of the given tasks is not up-to-date.                                                                                                                                     |
-|       | `--summary`                 | `bool`   | `false`                                      | Show summary about a task.                                                                                                                                                                                     |
-| `-t`  | `--taskfile`                | `string` | `Taskfile.yml` or `Taskfile.yaml`            |                                                                                                                                                                                                                |
-| `-v`  | `--verbose`                 | `bool`   | `false`                                      | Enables verbose mode.                                                                                                                                                                                          |
-|       | `--version`                 | `bool`   | `false`                                      | Show Task version.                                                                                                                                                                                             |
-| `-w`  | `--watch`                   | `bool`   | `false`                                      | Enables watch of the given task.                                                                                                                                                                               |
+|       | `--json`                    | `bool`   | `false`                                      | See [JSON Output](#json-output)                                                                                                                                                              |
+| `-o`  | `--output`                  | `string` | Default set in the Taskfile or `intervealed` | Sets output style: [`interleaved`/`group`/`prefixed`].                                                                                                                                       |
+|       | `--output-group-begin`      | `string` |                                              | Message template to print before a task's grouped output.                                                                                                                                    |
+|       | `--output-group-end`        | `string` |                                              | Message template to print after a task's grouped output.                                                                                                                                     |
+|       | `--output-group-error-only` | `bool`   | `false`                                      | Swallow command output on zero exit code.                                                                                                                                                    |
+| `-p`  | `--parallel`                | `bool`   | `false`                                      | Executes tasks provided on command line in parallel.                                                                                                                                         |
+| `-s`  | `--silent`                  | `bool`   | `false`                                      | Disables echoing.                                                                                                                                                                            |
+| `-y`  | `--yes`                     | `bool`   | `false`                                      | Assume "yes" as answer to all prompts.                                                                                                                                                       |
+|       | `--status`                  | `bool`   | `false`                                      | Exits with non-zero exit code if any of the given tasks is not up-to-date.                                                                                                                   |
+|       | `--summary`                 | `bool`   | `false`                                      | Show summary about a task.                                                                                                                                                                   |
+| `-t`  | `--taskfile`                | `string` | `Taskfile.yml` or `Taskfile.yaml`            |                                                                                                                                                                                              |
+| `-v`  | `--verbose`                 | `bool`   | `false`                                      | Enables verbose mode.                                                                                                                                                                        |
+|       | `--version`                 | `bool`   | `false`                                      | Show Task version.                                                                                                                                                                           |
+| `-w`  | `--watch`                   | `bool`   | `false`                                      | Enables watch of the given task.                                                                                                                                                             |
 
 ## Exit Codes
 
-Task will sometimes exit with specific exit codes. These codes are split into three groups with the following ranges:
+Task will sometimes exit with specific exit codes. These codes are split into
+three groups with the following ranges:
 
 - General errors (0-99)
 - Taskfile errors (100-199)
 - Task errors (200-299)
 
 A full list of the exit codes and their descriptions can be found below:
 
@@ -77,25 +79,29 @@
 | 201  | An error occurred while executing a command inside of a task |
 | 202  | The user tried to invoke a task that is internal             |
 | 203  | There a multiple tasks with the same name or alias           |
 | 204  | A task was called too many times                             |
 | 205  | A task was cancelled by the user                             |
 | 206  | A task was not executed due to missing required variables    |
 
-These codes can also be found in the repository in [`errors/errors.go`](https://github.com/go-task/task/blob/main/errors/errors.go).
+These codes can also be found in the repository in
+[`errors/errors.go`](https://github.com/go-task/task/blob/main/errors/errors.go).
 
 :::info
 
-When Task is run with the `-x`/`--exit-code` flag, the exit code of any failed commands will be passed through to the user instead.
+When Task is run with the `-x`/`--exit-code` flag, the exit code of any failed
+commands will be passed through to the user instead.
 
 :::
 
 ## JSON Output
 
-When using the `--json` flag in combination with either the `--list` or `--list-all` flags, the output will be a JSON object with the following structure:
+When using the `--json` flag in combination with either the `--list` or
+`--list-all` flags, the output will be a JSON object with the following
+structure:
 
 ```json
 {
   "tasks": [
     {
       "name": "",
       "desc": "",
@@ -118,16 +124,18 @@
 There are some special variables that is available on the templating system:
 
 | Var                | Description                                                                                                                                              |
 | ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `CLI_ARGS`         | Contain all extra arguments passed after `--` when calling Task through the CLI.                                                                         |
 | `CLI_FORCE`        | A boolean containing whether the `--force` or `--force-all` flags were set.                                                                              |
 | `TASK`             | The name of the current task.                                                                                                                            |
-| `ROOT_DIR`         | The absolute path of the root Taskfile.                                                                                                                  |
-| `TASKFILE_DIR`     | The absolute path of the included Taskfile.                                                                                                              |
+| `ROOT_TASKFILE`    | The absolute path of the root Taskfile.                                                                                                                  |
+| `ROOT_DIR`         | The absolute path of the root Taskfile directory.                                                                                                        |
+| `TASKFILE`         | The absolute path of the included Taskfile.                                                                                                              |
+| `TASKFILE_DIR`     | The absolute path of the included Taskfile directory.                                                                                                    |
 | `USER_WORKING_DIR` | The absolute path of the directory `task` was called from.                                                                                               |
 | `CHECKSUM`         | The checksum of the files listed in `sources`. Only available within the `status` prop and if method is set to `checksum`.                               |
 | `TIMESTAMP`        | The date object of the greatest timestamp of the files listed in `sources`. Only available within the `status` prop and if method is set to `timestamp`. |
 | `TASK_VERSION`     | The current version of task.                                                                                                                             |
 | `ITEM`             | The value of the current iteration when using the `for` property. Can be changed to a different variable name using `as:`.                               |
 
 ## ENV
@@ -142,14 +150,25 @@
 | `TASK_COLOR_GREEN`   | `32`    | Color used for green.                                                                                             |
 | `TASK_COLOR_CYAN`    | `36`    | Color used for cyan.                                                                                              |
 | `TASK_COLOR_YELLOW`  | `33`    | Color used for yellow.                                                                                            |
 | `TASK_COLOR_MAGENTA` | `35`    | Color used for magenta.                                                                                           |
 | `TASK_COLOR_RED`     | `31`    | Color used for red.                                                                                               |
 | `FORCE_COLOR`        |         | Force color output usage.                                                                                         |
 
+All color variables are [ANSI color codes][ansi]. You can specify multiple codes
+separated by a semicolon. For example: `31;1` will make the text bold and red.
+Task also supports 8-bit color (256 colors). You can specify these colors by
+using the sequence `38;2;R:G:B` for foreground colors and `48;2;R:G:B` for
+background colors where `R`, `G` and `B` should be replaced with values between
+0 and 255.
+
+For convenience, we allow foreground colors to be specified using shorthand,
+comma-separated syntax: `R,G,B`. For example, `255,0,0` is equivalent to
+`38;2;255:0:0`.
+
 ## Taskfile Schema
 
 | Attribute  | Type                               | Default       | Description                                                                                                                                                            |
 | ---------- | ---------------------------------- | ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `version`  | `string`                           |               | Version of the Taskfile. The current version is `3`.                                                                                                                   |
 | `output`   | `string`                           | `interleaved` | Output mode. Available options: `interleaved`, `group` and `prefixed`.                                                                                                 |
 | `method`   | `string`                           | `checksum`    | Default method in this Taskfile. Can be overridden in a task by task basis. Available options: `checksum`, `timestamp` and `none`.                                     |
@@ -173,15 +192,16 @@
 | `optional` | `bool`                | `false`                       | If `true`, no errors will be thrown if the specified file does not exist.                                                                                                                                                                                |
 | `internal` | `bool`                | `false`                       | Stops any task in the included Taskfile from being callable on the command line. These commands will also be omitted from the output when used with `--list`.                                                                                            |
 | `aliases`  | `[]string`            |                               | Alternative names for the namespace of the included Taskfile.                                                                                                                                                                                            |
 | `vars`     | `map[string]Variable` |                               | A set of variables to apply to the included Taskfile.                                                                                                                                                                                                    |
 
 :::info
 
-Informing only a string like below is equivalent to setting that value to the `taskfile` attribute.
+Informing only a string like below is equivalent to setting that value to the
+`taskfile` attribute.
 
 ```yaml
 includes:
   foo: ./path
 ```
 
 :::
@@ -202,29 +222,41 @@
   STATIC: static
   DYNAMIC:
     sh: echo "dynamic"
 ```
 
 :::
 
+:::info
+
+In a variables map, variables defined later may reference variables defined
+earlier (declaration order is respected):
+
+```yaml
+vars:
+  FIRST_VAR: "hello"
+  SECOND_VAR: "{{.FIRST_VAR}} world"
+```
+
+:::
+
 ### Task
 
 | Attribute       | Type                               | Default                                               | Description                                                                                                                                                                                                                                                                                              |
 | --------------- | ---------------------------------- | ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `cmds`          | [`[]Command`](#command)            |                                                       | A list of shell commands to be executed.                                                                                                                                                                                                                                                                 |
 | `deps`          | [`[]Dependency`](#dependency)      |                                                       | A list of dependencies of this task. Tasks defined here will run in parallel before this task.                                                                                                                                                                                                           |
 | `label`         | `string`                           |                                                       | Overrides the name of the task in the output when a task is run. Supports variables.                                                                                                                                                                                                                     |
 | `desc`          | `string`                           |                                                       | A short description of the task. This is displayed when calling `task --list`.                                                                                                                                                                                                                           |
 | `prompt`        | `string`                           |                                                       | A prompt that will be presented before a task is run. Declining will cancel running the current and any subsequent tasks.                                                                                                                                                                                |
 | `summary`       | `string`                           |                                                       | A longer description of the task. This is displayed when calling `task --summary [task]`.                                                                                                                                                                                                                |
 | `aliases`       | `[]string`                         |                                                       | A list of alternative names by which the task can be called.                                                                                                                                                                                                                                             |
 | `sources`       | `[]string`                         |                                                       | A list of sources to check before running this task. Relevant for `checksum` and `timestamp` methods. Can be file paths or star globs.                                                                                                                                                                   |
 | `generates`     | `[]string`                         |                                                       | A list of files meant to be generated by this task. Relevant for `timestamp` method. Can be file paths or star globs.                                                                                                                                                                                    |
 | `status`        | `[]string`                         |                                                       | A list of commands to check if this task should run. The task is skipped otherwise. This overrides `method`, `sources` and `generates`.                                                                                                                                                                  |
-| `requires`      | `[]string`                         |                                                       | A list of variables which should be set if this task is to run, if any of these variables are unset the task will error and not run.                                                                                                                                                                     |
 | `preconditions` | [`[]Precondition`](#precondition)  |                                                       | A list of commands to check if this task should run. If a condition is not met, the task will error.                                                                                                                                                                                                     |
 | `requires`      | [`Requires`](#requires)            |                                                       | A list of required variables which should be set if this task is to run, if any variables listed are unset the task will error and not run.                                                                                                                                                              |
 | `dir`           | `string`                           |                                                       | The directory in which this task should run. Defaults to the current working directory.                                                                                                                                                                                                                  |
 | `vars`          | [`map[string]Variable`](#variable) |                                                       | A set of variables that can be used in the task.                                                                                                                                                                                                                                                         |
 | `env`           | [`map[string]Variable`](#variable) |                                                       | A set of environment variables that will be made available to shell commands.                                                                                                                                                                                                                            |
 | `dotenv`        | `[]string`                         |                                                       | A list of `.env` file paths to be parsed.                                                                                                                                                                                                                                                                |
 | `silent`        | `bool`                             | `false`                                               | Hides task name and command from output. The command's output will still be redirected to `STDOUT` and `STDERR`. When combined with the `--list` flag, task descriptions will be hidden.                                                                                                                 |
@@ -236,15 +268,16 @@
 | `run`           | `string`                           | The one declared globally in the Taskfile or `always` | Specifies whether the task should run again or not if called more than once. Available options: `always`, `once` and `when_changed`.                                                                                                                                                                     |
 | `platforms`     | `[]string`                         | All platforms                                         | Specifies which platforms the task should be run on. [Valid GOOS and GOARCH values allowed](https://github.com/golang/go/blob/main/src/go/build/syslist.go). Task will be skipped otherwise.                                                                                                             |
 | `set`           | `[]string`                         |                                                       | Specify options for the [`set` builtin](https://www.gnu.org/software/bash/manual/html_node/The-Set-Builtin.html).                                                                                                                                                                                        |
 | `shopt`         | `[]string`                         |                                                       | Specify option for the [`shopt` builtin](https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html).                                                                                                                                                                                     |
 
 :::info
 
-These alternative syntaxes are available. They will set the given values to `cmds` and everything else will be set to their default values:
+These alternative syntaxes are available. They will set the given values to
+`cmds` and everything else will be set to their default values:
 
 ```yaml
 tasks:
   foo: echo "foo"
 
   foobar:
     - echo "foo"
@@ -291,33 +324,38 @@
 | --------- | ---------------------------------- | ------- | ---------------------------------------------------------------------------------------------------------------- |
 | `task`    | `string`                           |         | The task to be execute as a dependency.                                                                          |
 | `vars`    | [`map[string]Variable`](#variable) |         | Optional additional variables to be passed to this task.                                                         |
 | `silent`  | `bool`                             | `false` | Hides task name and command from output. The command's output will still be redirected to `STDOUT` and `STDERR`. |
 
 :::tip
 
-If you don't want to set additional variables, it's enough to declare the dependency as a list of strings (they will be assigned to `task`):
+If you don't want to set additional variables, it's enough to declare the
+dependency as a list of strings (they will be assigned to `task`):
 
 ```yaml
 tasks:
   foo:
     deps: [foo, bar]
 ```
 
 :::
 
 #### For
 
-The `for` parameter can be defined as a string, a list of strings or a map. If it is defined as a string, you can give it any of the following values:
+The `for` parameter can be defined as a string, a list of strings or a map. If
+it is defined as a string, you can give it any of the following values:
 
-- `source` - Will run the command for each source file defined on the task. (Glob patterns will be resolved, so `*.go` will run for every Go file that matches).
+- `source` - Will run the command for each source file defined on the task.
+  (Glob patterns will be resolved, so `*.go` will run for every Go file that
+  matches).
 
 If it is defined as a list of strings, the command will be run for each value.
 
-Finally, the `for` parameter can be defined as a map when you want to use a variable to define the values to loop over:
+Finally, the `for` parameter can be defined as a map when you want to use a
+variable to define the values to loop over:
 
 | Attribute | Type     | Default          | Description                                  |
 | --------- | -------- | ---------------- | -------------------------------------------- |
 | `var`     | `string` |                  | The name of the variable to use as an input. |
 | `split`   | `string` | (any whitespace) | What string the variable should be split on. |
 | `as`      | `string` | `ITEM`           | The name of the iterator variable.           |
 
@@ -326,22 +364,27 @@
 | Attribute | Type     | Default | Description                                                                                                  |
 | --------- | -------- | ------- | ------------------------------------------------------------------------------------------------------------ |
 | `sh`      | `string` |         | Command to be executed. If a non-zero exit code is returned, the task errors without executing its commands. |
 | `msg`     | `string` |         | Optional message to print if the precondition isn't met.                                                     |
 
 :::tip
 
-If you don't want to set a different message, you can declare a precondition like this and the value will be assigned to `sh`:
+If you don't want to set a different message, you can declare a precondition
+like this and the value will be assigned to `sh`:
 
 ```yaml
 tasks:
   foo:
     precondition: test -f Taskfile.yml
 ```
 
 :::
 
 #### Requires
 
 | Attribute | Type       | Default | Description                                                                                        |
 | --------- | ---------- | ------- | -------------------------------------------------------------------------------------------------- |
 | `vars`    | `[]string` |         | List of variable or environment variable names that must be set if this task is to execute and run |
+
+{/* prettier-ignore-start */}
+[ansi]: https://en.wikipedia.org/wiki/ANSI_escape_code
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/changelog.md` & `go_task_bin-3.36.0/task/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,490 +1,795 @@
----
-slug: /changelog/
-sidebar_position: 14
----
-
 # Changelog
 
+## v3.36.0 - 2024-04-08
+
+- Added support for
+  [looping over dependencies](https://taskfile.dev/usage/#looping-over-dependencies)
+  (#1299, #1541 by @pd93).
+- When using the
+  "[Remote Taskfiles](https://taskfile.dev/experiments/remote-taskfiles/)"
+  experiment, you are now able to use
+  [remote Taskfiles as your entrypoint](https://taskfile.dev/experiments/remote-taskfiles/#root-remote-taskfiles).
+  - `includes` in remote Taskfiles will now also resolve correctly (#1347 by
+    @pd93).
+- When using the
+  "[Any Variables](https://taskfile.dev/experiments/any-variables/)"
+  experiments, templating is now supported in collection-type variables (#1477,
+  #1511, #1526 by @pd93).
+- Fixed a bug where variables being passed to an included Taskfile were not
+  available when defining global variables (#1503, #1533 by @pd93).
+- Improved support to customized colors by allowing 8-bit colors and multiple
+  ANSI attributes (#1576 by @pd93).
+
+## v3.35.1 - 2024-03-04
+
+- Fixed a bug where the `TASKFILE_DIR` variable was sometimes incorrect (#1522,
+  #1523 by @pd93).
+- Added a new `TASKFILE` special variable that holds the root Taskfile path
+  (#1523 by @pd93).
+- Fixed various issues related to running a Taskfile from a subdirectory (#1529,
+  #1530 by @pd93).
+
+## v3.35.0 - 2024-02-28
+
+- Added support for
+  [wildcards in task names](https://taskfile.dev/usage/#wildcard-arguments)
+  (#836, #1489 by @pd93).
+- Added the ability to
+  [run Taskfiles via stdin](https://taskfile.dev/usage/#reading-a-taskfile-from-stdin)
+  (#655, #1483 by @pd93).
+- Bumped minimum Go version to 1.21 (#1500 by @pd93).
+- Fixed bug related to the `--list` flag (#1509, #1512 by @pd93, #1514, #1520 by
+  @pd93).
+- Add mention on the documentation to the fact that the variable declaration
+  order is respected (#1510 by @kirkrodrigues).
+- Improved style guide docs (#1495 by @iwittkau).
+- Removed duplicated entry for `requires` on the API docs (#1491 by
+  @teatimeguest).
+
+## v3.34.1 - 2024-01-27
+
+- Fixed prompt regression on
+  [Remote Taskfiles experiment](https://taskfile.dev/experiments/remote-taskfiles/)
+  (#1486, #1487 by @pd93).
+
+## v3.34.0 - 2024-01-25
+
+- Removed support for `version: 2` schemas. See the
+  [deprecation notice on our website](https://taskfile.dev/deprecations/version-2-schema)
+  (#1197, #1447 by @pd93).
+- Fixed a couple of issues in the JSON Schema + added a CI step to ensure it's
+  correct (#1471, #1474, #1476 by @sirosen).
+- Added
+  [Any Variables experiment proposal 2](https://taskfile.dev/experiments/any-variables/?proposal=2)
+  (#1415, #1444 by @pd93).
+- Updated the experiments and deprecations documentation format (#1445 by
+  @pd93).
+- Added new template function: `spew`, which can be used to print variables for
+  debugging purposes (#1452 by @pd93).
+- Added new template function: `merge`, which can be used to merge any number of
+  map variables (#1438, #1464 by @pd93).
+- Small change on the API when using as a library: `call.Direct` became
+  `call.Indirect` (#1459 by @pd93).
+- Refactored the public `read` and `taskfile` packages and introduced
+  `taskfile/ast` (#1450 by @pd93).
+- `ast.IncludedTaskfiles` renamed to `ast.Includes` and `orderedmap` package
+  renamed to `omap` plus some internal refactor work (#1456 by @pd93).
+- Fix zsh completion script to allow lowercase `taskfile` file names (#1482 by
+  @xontab).
+- Improvements on how we check the Taskfile version (#1465 by @pd93).
+- Added a new `ROOT_TASKFILE` special variable (#1468, #1469 by @pd93).
+- Fix experiment flags in `.env` when the `--dir` or `--taskfile` flags were
+  used (#1478 by @pd93).
+
 ## v3.33.1 - 2023-12-21
 
-- Added support for looping over map variables with the [Any Variables experiment](https://taskfile.dev/experiments/any_variables) enabled (#1435, #1437 by @pd93).
-- Fixed a bug where dynamic variables were causing errors during fast compilation (#1435, #1437 by @pd93)
+- Added support for looping over map variables with the
+  [Any Variables experiment](https://taskfile.dev/experiments/any-variables)
+  enabled (#1435, #1437 by @pd93).
+- Fixed a bug where dynamic variables were causing errors during fast
+  compilation (#1435, #1437 by @pd93)
 
 ## v3.33.0 - 2023-12-20
 
-- Added [Any Variables experiment](https://taskfile.dev/experiments/any-variables) (#1415, #1421 by @pd93).
+- Added
+  [Any Variables experiment](https://taskfile.dev/experiments/any-variables)
+  (#1415, #1421 by @pd93).
 - Updated Docusaurus to v3 (#1432 by @pd93).
 - Added `aliases` to `--json` flag output (#1430, #1431 by @pd93).
-- Added new `CLI_FORCE` special variable containing whether the `--force` or `--force-all` flags were set (#1412, #1434 by @pd93).
+- Added new `CLI_FORCE` special variable containing whether the `--force` or
+  `--force-all` flags were set (#1412, #1434 by @pd93).
 
 ## v3.32.0 - 2023-11-29
 
 - Added ability to exclude some files from `sources:` by using `exclude:` (#225,
-
-  # 1324 by @pd93 and @andreynering).
-- The [Remote Taskfiles experiment](https://taskfile.dev/experiments/remote-taskfiles) now prefers remote files over cached ones by default (#1317, #1345 by @pd93).
-- Added `--timeout` flag to the [Remote Taskfiles experiment](https://taskfile.dev/experiments/remote-taskfiles) (#1317, #1345 by @pd93).
-- Fix bug where dynamic `vars:` and `env:` were being executed when they should actually be skipped by `platforms:` (#1273, #1377 by @andreynering).
+  #1324 by @pd93 and @andreynering).
+- The
+  [Remote Taskfiles experiment](https://taskfile.dev/experiments/remote-taskfiles)
+  now prefers remote files over cached ones by default (#1317, #1345 by @pd93).
+- Added `--timeout` flag to the
+  [Remote Taskfiles experiment](https://taskfile.dev/experiments/remote-taskfiles)
+  (#1317, #1345 by @pd93).
+- Fix bug where dynamic `vars:` and `env:` were being executed when they should
+  actually be skipped by `platforms:` (#1273, #1377 by @andreynering).
 - Fix `schema.json` to make `silent` valid in `cmds` that use `for` (#1385,
-
-  # 1386 by @iainvm).
-- Add new `--no-status` flag to skip expensive status checks when running `task --list --json` (#1348, #1368 by @amancevice).
+  #1386 by @iainvm).
+- Add new `--no-status` flag to skip expensive status checks when running
+  `task --list --json` (#1348, #1368 by @amancevice).
 
 ## v3.31.0 - 2023-10-07
 
-- Enabled the `--yes` flag for the [Remote Taskfiles experiment](https://taskfile.dev/experiments/remote-taskfiles) (#1317, #1344 by @pd93).
-- Add ability to set `watch: true` in a task to automatically run it in watch mode (#231, #1361 by @andreynering).
-- Fixed a bug on the watch mode where paths that contained `.git` (like `.github`), for example, were also being ignored (#1356 by @butuzov).
+- Enabled the `--yes` flag for the
+  [Remote Taskfiles experiment](https://taskfile.dev/experiments/remote-taskfiles)
+  (#1317, #1344 by @pd93).
+- Add ability to set `watch: true` in a task to automatically run it in watch
+  mode (#231, #1361 by @andreynering).
+- Fixed a bug on the watch mode where paths that contained `.git` (like
+  `.github`), for example, were also being ignored (#1356 by @butuzov).
 - Fixed a nil pointer error when running a Taskfile with no contents (#1341,
-
-  # 1342 by @pd93).
-- Added a new [exit code](https://taskfile.dev/api/#exit-codes) (107) for when a Taskfile does not contain a schema version (#1342 by @pd93).
-- Increased limit of maximum task calls from 100 to 1000 for now, as some people have been reaching this limit organically now that we have loops. This check exists to detect recursive calls, but will be removed in favor of a better algorithm soon (#1321, #1332).
+  #1342 by @pd93).
+- Added a new [exit code](https://taskfile.dev/api/#exit-codes) (107) for when a
+  Taskfile does not contain a schema version (#1342 by @pd93).
+- Increased limit of maximum task calls from 100 to 1000 for now, as some people
+  have been reaching this limit organically now that we have loops. This check
+  exists to detect recursive calls, but will be removed in favor of a better
+  algorithm soon (#1321, #1332).
 - Fixed templating on descriptions on `task --list` (#1343 by @blackjid).
-- Fixed a bug where precondition errors were incorrectly being printed when task execution was aborted (#1337, #1338 by @sylv-io).
+- Fixed a bug where precondition errors were incorrectly being printed when task
+  execution was aborted (#1337, #1338 by @sylv-io).
 
 ## v3.30.1 - 2023-09-14
 
-- Fixed a regression where some special variables weren't being set correctly (#1331, #1334 by @pd93).
+- Fixed a regression where some special variables weren't being set correctly
+  (#1331, #1334 by @pd93).
 
 ## v3.30.0 - 2023-09-13
 
 - Prep work for Remote Taskfiles (#1316 by @pd93).
-- Added the [Remote Taskfiles experiment](https://taskfile.dev/experiments/remote-taskfiles) as a draft (#1152, #1317 by @pd93).
-- Improve performance of content checksuming on `sources:` by replacing md5 with [XXH3](https://xxhash.com/) which is much faster. This is a soft breaking change because checksums will be invalidated when upgrading to this release (#1325 by @ReillyBrogan).
+- Added the
+  [Remote Taskfiles experiment](https://taskfile.dev/experiments/remote-taskfiles)
+  as a draft (#1152, #1317 by @pd93).
+- Improve performance of content checksuming on `sources:` by replacing md5 with
+  [XXH3](https://xxhash.com/) which is much faster. This is a soft breaking
+  change because checksums will be invalidated when upgrading to this release
+  (#1325 by @ReillyBrogan).
 
 ## v3.29.1 - 2023-08-26
 
 - Update to Go 1.21 (bump minimum version to 1.20) (#1302 by @pd93)
-- Fix a missing a line break on log when using `--watch` mode (#1285, #1297 by @FilipSolich).
+- Fix a missing a line break on log when using `--watch` mode (#1285, #1297 by
+  @FilipSolich).
 - Fix `defer` on JSON Schema (#1288 by @calvinmclean and @andreynering).
-- Fix bug in usage of special variables like `{{.USER_WORKING_DIR}}` in combination with `includes` (#1046, #1205, #1250, #1293, #1312, #1274 by @andarto, #1309 by @andreynering).
-- Fix bug on `--status` flag. Running this flag should not have side-effects: it should not update the checksum on `.task`, only report its status (#1305,
-
-  # 1307 by @visciang, #1313 by @andreynering).
+- Fix bug in usage of special variables like `{{.USER_WORKING_DIR}}` in
+  combination with `includes` (#1046, #1205, #1250, #1293, #1312, #1274 by
+  @andarto, #1309 by @andreynering).
+- Fix bug on `--status` flag. Running this flag should not have side-effects: it
+  should not update the checksum on `.task`, only report its status (#1305,
+  #1307 by @visciang, #1313 by @andreynering).
 
 ## v3.28.0 - 2023-07-24
 
-- Added the ability to [loop over commands and tasks](https://taskfile.dev/usage/#looping-over-values) using `for` (#82, #1220 by @pd93).
-- Fixed variable propagation in multi-level includes (#778, #996, #1256 by @hudclark).
-- Fixed a bug where the `--exit-code` code flag was not returning the correct exit code when calling commands indirectly (#1266, #1270 by @pd93).
-- Fixed a `nil` panic when a dependency was commented out or left empty (#1263 by @neomantra).
+- Added the ability to
+  [loop over commands and tasks](https://taskfile.dev/usage/#looping-over-values)
+  using `for` (#82, #1220 by @pd93).
+- Fixed variable propagation in multi-level includes (#778, #996, #1256 by
+  @hudclark).
+- Fixed a bug where the `--exit-code` code flag was not returning the correct
+  exit code when calling commands indirectly (#1266, #1270 by @pd93).
+- Fixed a `nil` panic when a dependency was commented out or left empty (#1263
+  by @neomantra).
 
 ## v3.27.1 - 2023-06-30
 
-- Fix panic when a `.env` directory (not file) is present on current directory (#1244, #1245 by @pd93).
+- Fix panic when a `.env` directory (not file) is present on current directory
+  (#1244, #1245 by @pd93).
 
 ## v3.27.0 - 2023-06-29
 
 - Allow Taskfiles starting with lowercase characters (#947, #1221 by @pd93).
-  - e.g. `taskfile.yml`, `taskfile.yaml`, `taskfile.dist.yml` & `taskfile.dist.yaml`
-- Bug fixes were made to the [npm installation method](https://taskfile.dev/installation/#npm). (#1190, by @sounisi5011).
-- Added the [gentle force experiment](https://taskfile.dev/experiments/gentle-force) as a draft (#1200, #1216 by @pd93).
-- Added an `--experiments` flag to allow you to see which experiments are enabled (#1242 by @pd93).
-- Added ability to specify which variables are required in a task (#1203, #1204 by @benc-uk).
+  - e.g. `taskfile.yml`, `taskfile.yaml`, `taskfile.dist.yml` &
+    `taskfile.dist.yaml`
+- Bug fixes were made to the
+  [npm installation method](https://taskfile.dev/installation/#npm). (#1190, by
+  @sounisi5011).
+- Added the
+  [gentle force experiment](https://taskfile.dev/experiments/gentle-force) as a
+  draft (#1200, #1216 by @pd93).
+- Added an `--experiments` flag to allow you to see which experiments are
+  enabled (#1242 by @pd93).
+- Added ability to specify which variables are required in a task (#1203, #1204
+  by @benc-uk).
 
 ## v3.26.0 - 2023-06-10
 
 - Only rewrite checksum files in `.task` if the checksum has changed (#1185,
-
-  # 1194 by @deviantintegral).
-- Added [experiments documentation](https://taskfile.dev/experiments) to the website (#1198 by @pd93).
-- Deprecated `version: 2` schema. This will be removed in the next major release (#1197, #1198, #1199 by @pd93).
-- Added a new `prompt:` prop to set a warning prompt to be shown before running a potential dangurous task (#100, #1163 by @MaxCheetham, [Documentation](https://taskfile.dev/usage/#warning-prompts)).
-- Added support for single command task syntax. With this change, it's now possible to declare just `cmd:` in a task, avoiding the more complex `cmds: []` when you have only a single command for that task (#1130, #1131 by @timdp).
+  #1194 by @deviantintegral).
+- Added [experiments documentation](https://taskfile.dev/experiments) to the
+  website (#1198 by @pd93).
+- Deprecated `version: 2` schema. This will be removed in the next major release
+  (#1197, #1198, #1199 by @pd93).
+- Added a new `prompt:` prop to set a warning prompt to be shown before running
+  a potential dangurous task (#100, #1163 by @MaxCheetham,
+  [Documentation](https://taskfile.dev/usage/#warning-prompts)).
+- Added support for single command task syntax. With this change, it's now
+  possible to declare just `cmd:` in a task, avoiding the more complex
+  `cmds: []` when you have only a single command for that task (#1130, #1131 by
+  @timdp).
 
 ## v3.25.0 - 2023-05-22
 
 - Support `silent:` when calling another tasks (#680, #1142 by @danquah).
 - Improve PowerShell completion script (#1168 by @trim21).
-- Add more languages to the website menu and show translation progress percentage (#1173 by @misitebao).
-- Starting on this release, official binaries for FreeBSD will be available to download (#1068 by @andreynering).
+- Add more languages to the website menu and show translation progress
+  percentage (#1173 by @misitebao).
+- Starting on this release, official binaries for FreeBSD will be available to
+  download (#1068 by @andreynering).
 - Fix some errors being unintendedly supressed (#1134 by @clintmod).
 - Fix a nil pointer error when `version` is omitted from a Taskfile (#1148,
-
-  # 1149 by @pd93).
-- Fix duplicate error message when a task does not exists (#1141, #1144 by @pd93).
+  #1149 by @pd93).
+- Fix duplicate error message when a task does not exists (#1141, #1144 by
+  @pd93).
 
 ## v3.24.0 - 2023-04-15
 
 - Fix Fish shell completion for tasks with aliases (#1113 by @patricksjackson).
-- The default branch was renamed from `master` to `main` (#1049, #1048 by @pd93).
+- The default branch was renamed from `master` to `main` (#1049, #1048 by
+  @pd93).
 - Fix bug where "up-to-date" logs were not being omitted for silent tasks (#546,
-
-  # 1107 by @danquah).
-- Add `.hg` (Mercurial) to the list of ignored directories when using `--watch` (#1098 by @misery).
+  #1107 by @danquah).
+- Add `.hg` (Mercurial) to the list of ignored directories when using `--watch`
+  (#1098 by @misery).
 - More improvements to the release tool (#1096 by @pd93).
 - Enforce [gofumpt](https://github.com/mvdan/gofumpt) linter (#1099 by @pd93)
-- Add `--sort` flag for use with `--list` and `--list-all` (#946, #1105 by @pd93).
-- Task now has [custom exit codes](https://taskfile.dev/api/#exit-codes) depending on the error (#1114 by @pd93).
+- Add `--sort` flag for use with `--list` and `--list-all` (#946, #1105 by
+  @pd93).
+- Task now has [custom exit codes](https://taskfile.dev/api/#exit-codes)
+  depending on the error (#1114 by @pd93).
 
 ## v3.23.0 - 2023-03-26
 
-Task now has an [official extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=task.vscode-task) contributed by @pd93! :tada: The extension is maintained in a [new repository](https://github.com/go-task/vscode-task) under the `go-task` organization. We're looking to gather feedback from the community so please give it a go and let us know what you think via a [discussion](https://github.com/go-task/vscode-task/discussions), [issue](https://github.com/go-task/vscode-task/issues) or on our [Discord](https://discord.gg/6TY36E39UK)!
+Task now has an
+[official extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=task.vscode-task)
+contributed by @pd93! :tada: The extension is maintained in a
+[new repository](https://github.com/go-task/vscode-task) under the `go-task`
+organization. We're looking to gather feedback from the community so please give
+it a go and let us know what you think via a
+[discussion](https://github.com/go-task/vscode-task/discussions),
+[issue](https://github.com/go-task/vscode-task/issues) or on our
+[Discord](https://discord.gg/6TY36E39UK)!
 
 > **NOTE:** The extension _requires_ v3.23.0 to be installed in order to work.
 
-- The website was integrated with [Crowdin](https://crowdin.com/project/taskfile) to allow the community to contribute with translations! [Chinese](https://taskfile.dev/zh-Hans/) is the first language available (#1057, #1058 by @misitebao).
+- The website was integrated with
+  [Crowdin](https://crowdin.com/project/taskfile) to allow the community to
+  contribute with translations! [Chinese](https://taskfile.dev/zh-Hans/) is the
+  first language available (#1057, #1058 by @misitebao).
 - Added task location data to the `--json` flag output (#1056 by @pd93)
-- Change the name of the file generated by `task --init` from `Taskfile.yaml` to `Taskfile.yml` (#1062 by @misitebao).
-- Added new `splitArgs` template function (`{{splitArgs "foo bar 'foo bar baz'"}}`) to ensure string is split as arguments (#1040, #1059 by @dhanusaputra).
+- Change the name of the file generated by `task --init` from `Taskfile.yaml` to
+  `Taskfile.yml` (#1062 by @misitebao).
+- Added new `splitArgs` template function
+  (`{{splitArgs "foo bar 'foo bar baz'"}}`) to ensure string is split as
+  arguments (#1040, #1059 by @dhanusaputra).
 - Fix the value of `{{.CHECKSUM}}` variable in status (#1076, #1080 by @pd93).
 - Fixed deep copy implementation (#1072 by @pd93)
 - Created a tool to assist with releases (#1086 by @pd93).
 
 ## v3.22.0 - 2023-03-10
 
-- Add a brand new `--global` (`-g`) flag that will run a Taskfile from your `$HOME` directory. This is useful to have automation that you can run from anywhere in your system! ([Documentation](https://taskfile.dev/usage/#running-a-global-taskfile), #1029 by @andreynering).
-- Add ability to set `error_only: true` on the `group` output mode. This will instruct Task to only print a command output if it returned with a non-zero exit code (#664, #1022 by @jaedle).
-- Fixed bug where `.task/checksum` file was sometimes not being created when task also declares a `status:` (#840, #1035 by @harelwa, #1037 by @pd93).
-- Refactored and decoupled fingerprinting from the main Task executor (#1039 by @pd93).
-- Fixed deadlock issue when using `run: once` (#715, #1025 by @theunrepentantgeek).
+- Add a brand new `--global` (`-g`) flag that will run a Taskfile from your
+  `$HOME` directory. This is useful to have automation that you can run from
+  anywhere in your system!
+  ([Documentation](https://taskfile.dev/usage/#running-a-global-taskfile), #1029
+  by @andreynering).
+- Add ability to set `error_only: true` on the `group` output mode. This will
+  instruct Task to only print a command output if it returned with a non-zero
+  exit code (#664, #1022 by @jaedle).
+- Fixed bug where `.task/checksum` file was sometimes not being created when
+  task also declares a `status:` (#840, #1035 by @harelwa, #1037 by @pd93).
+- Refactored and decoupled fingerprinting from the main Task executor (#1039 by
+  @pd93).
+- Fixed deadlock issue when using `run: once` (#715, #1025 by
+  @theunrepentantgeek).
 
 ## v3.21.0 - 2023-02-22
 
 - Added new `TASK_VERSION` special variable (#990, #1014 by @ja1code).
-- Fixed a bug where tasks were sometimes incorrectly marked as internal (#1007 by @pd93).
+- Fixed a bug where tasks were sometimes incorrectly marked as internal (#1007
+  by @pd93).
 - Update to Go 1.20 (bump minimum version to 1.19) (#1010 by @pd93)
-- Added environment variable `FORCE_COLOR` support to force color output. Usefull for environments without TTY (#1003 by @automation-stack)
+- Added environment variable `FORCE_COLOR` support to force color output.
+  Usefull for environments without TTY (#1003 by @automation-stack)
 
 ## v3.20.0 - 2023-01-14
 
-- Improve behavior and performance of status checking when using the `timestamp` mode (#976, #977 by @aminya).
+- Improve behavior and performance of status checking when using the `timestamp`
+  mode (#976, #977 by @aminya).
 - Performance optimizations were made for large Taskfiles (#982 by @pd93).
-- Add ability to configure options for the [`set`](https://www.gnu.org/software/bash/manual/html_node/The-Set-Builtin.html) and [`shopt`](https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html) builtins (#908, #929 by @pd93, [Documentation](http://taskfile.dev/usage/#set-and-shopt)).
-- Add new `platforms:` attribute to `task` and `cmd`, so it's now possible to choose in which platforms that given task or command will be run on. Possible values are operating system (GOOS), architecture (GOARCH) or a combination of the two. Example: `platforms: [linux]`, `platforms: [amd64]` or `platforms: [linux/amd64]`. Other platforms will be skipped (#978, #980 by @leaanthony).
+- Add ability to configure options for the
+  [`set`](https://www.gnu.org/software/bash/manual/html_node/The-Set-Builtin.html)
+  and
+  [`shopt`](https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html)
+  builtins (#908, #929 by @pd93,
+  [Documentation](http://taskfile.dev/usage/#set-and-shopt)).
+- Add new `platforms:` attribute to `task` and `cmd`, so it's now possible to
+  choose in which platforms that given task or command will be run on. Possible
+  values are operating system (GOOS), architecture (GOARCH) or a combination of
+  the two. Example: `platforms: [linux]`, `platforms: [amd64]` or
+  `platforms: [linux/amd64]`. Other platforms will be skipped (#978, #980 by
+  @leaanthony).
 
 ## v3.19.1 - 2022-12-31
 
-- Small bug fix: closing `Taskfile.yml` once we're done reading it (#963, #964 by @HeCorr).
-- Fixes a bug in v2 that caused a panic when using a `Taskfile_{{OS}}.yml` file (#961, #971 by @pd93).
-- Fixed a bug where watch intervals set in the Taskfile were not being respected (#969, #970 by @pd93)
-- Add `--json` flag (alias `-j`) with the intent to improve support for code editors and add room to other possible integrations. This is basic for now, but we plan to add more info in the near future (#936 by @davidalpert, #764).
+- Small bug fix: closing `Taskfile.yml` once we're done reading it (#963, #964
+  by @HeCorr).
+- Fixes a bug in v2 that caused a panic when using a `Taskfile_{{OS}}.yml` file
+  (#961, #971 by @pd93).
+- Fixed a bug where watch intervals set in the Taskfile were not being respected
+  (#969, #970 by @pd93)
+- Add `--json` flag (alias `-j`) with the intent to improve support for code
+  editors and add room to other possible integrations. This is basic for now,
+  but we plan to add more info in the near future (#936 by @davidalpert, #764).
 
 ## v3.19.0 - 2022-12-05
 
-- Installation via npm now supports [pnpm](https://pnpm.io/) as well ([go-task/go-npm#2](https://github.com/go-task/go-npm/issues/2), [go-task/go-npm#3](https://github.com/go-task/go-npm/pull/3)).
-- It's now possible to run Taskfiles from subdirectories! A new `USER_WORKING_DIR` special variable was added to add even more flexibility for monorepos (#289, #920).
+- Installation via npm now supports [pnpm](https://pnpm.io/) as well
+  ([go-task/go-npm#2](https://github.com/go-task/go-npm/issues/2),
+  [go-task/go-npm#3](https://github.com/go-task/go-npm/pull/3)).
+- It's now possible to run Taskfiles from subdirectories! A new
+  `USER_WORKING_DIR` special variable was added to add even more flexibility for
+  monorepos (#289, #920).
 - Add task-level `dotenv` support (#389, #904).
 - It's now possible to use global level variables on `includes` (#942, #943).
-- The website got a brand new [translation to Chinese](https://task-zh.readthedocs.io/zh_CN/latest/) by [@DeronW](https://github.com/DeronW). Thanks!
+- The website got a brand new
+  [translation to Chinese](https://task-zh.readthedocs.io/zh_CN/latest/) by
+  [@DeronW](https://github.com/DeronW). Thanks!
 
 ## v3.18.0 - 2022-11-12
 
-- Show aliases on `task --list --silent` (`task --ls`). This means that aliases will be completed by the completion scripts (#919).
-- Tasks in the root Taskfile will now be displayed first in `--list`/`--list-all` output (#806, #890).
-- It's now possible to call a `default` task in an included Taskfile by using just the namespace. For example: `docs:default` is now automatically aliased to `docs` (#661, #815).
+- Show aliases on `task --list --silent` (`task --ls`). This means that aliases
+  will be completed by the completion scripts (#919).
+- Tasks in the root Taskfile will now be displayed first in
+  `--list`/`--list-all` output (#806, #890).
+- It's now possible to call a `default` task in an included Taskfile by using
+  just the namespace. For example: `docs:default` is now automatically aliased
+  to `docs` (#661, #815).
 
 ## v3.17.0 - 2022-10-14
 
-- Add a "Did you mean ...?" suggestion when a task does not exits another one with a similar name is found (#867, #880).
+- Add a "Did you mean ...?" suggestion when a task does not exits another one
+  with a similar name is found (#867, #880).
 - Now YAML parse errors will print which Taskfile failed to parse (#885, #887).
 - Add ability to set `aliases` for tasks and namespaces (#268, #340, #879).
 - Improvements to Fish shell completion (#897).
-- Added ability to set a different watch interval by setting `interval: '500ms'` or using the `--interval=500ms` flag (#813, #865).
+- Added ability to set a different watch interval by setting `interval: '500ms'`
+  or using the `--interval=500ms` flag (#813, #865).
 - Add colored output to `--list`, `--list-all` and `--summary` flags (#845,
-
-  # 874).
-- Fix unexpected behavior where `label:` was being shown instead of the task name on `--list` (#603, #877).
+  #874).
+- Fix unexpected behavior where `label:` was being shown instead of the task
+  name on `--list` (#603, #877).
 
 ## v3.16.0 - 2022-09-29
 
-- Add `npm` as new installation method: `npm i -g @go-task/cli` (#870, #871, [npm package](https://www.npmjs.com/package/@go-task/cli)).
-- Add support to marking tasks and includes as internal, which will hide them from `--list` and `--list-all` (#818).
+- Add `npm` as new installation method: `npm i -g @go-task/cli` (#870, #871,
+  [npm package](https://www.npmjs.com/package/@go-task/cli)).
+- Add support to marking tasks and includes as internal, which will hide them
+  from `--list` and `--list-all` (#818).
 
 ## v3.15.2 - 2022-09-08
 
-- Fix error when using variable in `env:` introduced in the previous release (#858, #866).
+- Fix error when using variable in `env:` introduced in the previous release
+  (#858, #866).
 - Fix handling of `CLI_ARGS` (`--`) in Bash completion (#863).
-- On zsh completion, add ability to replace `--list-all` with `--list` as already possible on the Bash completion (#861).
+- On zsh completion, add ability to replace `--list-all` with `--list` as
+  already possible on the Bash completion (#861).
 
 ## v3.15.0 - 2022-09-03
 
-- Add new special variables `ROOT_DIR` and `TASKFILE_DIR`. This was a highly requested feature (#215, #857, [Documentation](https://taskfile.dev/api/#special-variables)).
+- Add new special variables `ROOT_DIR` and `TASKFILE_DIR`. This was a highly
+  requested feature (#215, #857,
+  [Documentation](https://taskfile.dev/api/#special-variables)).
 - Follow symlinks on `sources` (#826, #831).
 - Improvements and fixes to Bash completion (#835, #844).
 
 ## v3.14.1 - 2022-08-03
 
-- Always resolve relative include paths relative to the including Taskfile (#822, #823).
-- Fix ZSH and PowerShell completions to consider all tasks instead of just the public ones (those with descriptions) (#803).
+- Always resolve relative include paths relative to the including Taskfile
+  (#822, #823).
+- Fix ZSH and PowerShell completions to consider all tasks instead of just the
+  public ones (those with descriptions) (#803).
 
 ## v3.14.0 - 2022-07-08
 
-- Add ability to override the `.task` directory location with the `TASK_TEMP_DIR` environment variable.
-- Allow to override Task colors using environment variables: `TASK_COLOR_RESET`, `TASK_COLOR_BLUE`, `TASK_COLOR_GREEN`, `TASK_COLOR_CYAN`, `TASK_COLOR_YELLOW`, `TASK_COLOR_MAGENTA` and `TASK_COLOR_RED` (#568, #792).
-- Fixed bug when using the `output: group` mode where STDOUT and STDERR were being print in separated blocks instead of in the right order (#779).
-- Starting on this release, ARM architecture binaries are been released to Snap as well (#795).
-- i386 binaries won't be available anymore on Snap because Ubuntu removed the support for this architecture.
-- Upgrade mvdan.cc/sh, which fixes a bug with associative arrays (#785, [mvdan/sh#884](https://github.com/mvdan/sh/issues/884), [mvdan/sh#893](https://github.com/mvdan/sh/pull/893)).
+- Add ability to override the `.task` directory location with the
+  `TASK_TEMP_DIR` environment variable.
+- Allow to override Task colors using environment variables: `TASK_COLOR_RESET`,
+  `TASK_COLOR_BLUE`, `TASK_COLOR_GREEN`, `TASK_COLOR_CYAN`, `TASK_COLOR_YELLOW`,
+  `TASK_COLOR_MAGENTA` and `TASK_COLOR_RED` (#568, #792).
+- Fixed bug when using the `output: group` mode where STDOUT and STDERR were
+  being print in separated blocks instead of in the right order (#779).
+- Starting on this release, ARM architecture binaries are been released to Snap
+  as well (#795).
+- i386 binaries won't be available anymore on Snap because Ubuntu removed the
+  support for this architecture.
+- Upgrade mvdan.cc/sh, which fixes a bug with associative arrays (#785,
+  [mvdan/sh#884](https://github.com/mvdan/sh/issues/884),
+  [mvdan/sh#893](https://github.com/mvdan/sh/pull/893)).
 
 ## v3.13.0 - 2022-06-13
 
 - Added `-n` as an alias to `--dry` (#776, #777).
-- Fix behavior of interrupt (SIGINT, SIGTERM) signals. Task will now give time for the processes running to do cleanup work (#458, #479, #728, #769).
-- Add new `--exit-code` (`-x`) flag that will pass-through the exit form the command being ran (#755).
+- Fix behavior of interrupt (SIGINT, SIGTERM) signals. Task will now give time
+  for the processes running to do cleanup work (#458, #479, #728, #769).
+- Add new `--exit-code` (`-x`) flag that will pass-through the exit form the
+  command being ran (#755).
 
 ## v3.12.1 - 2022-05-10
 
-- Fixed bug where, on Windows, variables were ending with `\r` because we were only removing the final `\n` but not `\r\n` (#717).
+- Fixed bug where, on Windows, variables were ending with `\r` because we were
+  only removing the final `\n` but not `\r\n` (#717).
 
 ## v3.12.0 - 2022-03-31
 
-- The `--list` and `--list-all` flags can now be combined with the `--silent` flag to print the task names only, without their description (#691).
-- Added support for multi-level inclusion of Taskfiles. This means that included Taskfiles can also include other Taskfiles. Before this was limited to one level (#390, #623, #656).
-- Add ability to specify vars when including a Taskfile. [Check out the documentation](https://taskfile.dev/#/usage?id=vars-of-included-taskfiles) for more information (#677).
+- The `--list` and `--list-all` flags can now be combined with the `--silent`
+  flag to print the task names only, without their description (#691).
+- Added support for multi-level inclusion of Taskfiles. This means that included
+  Taskfiles can also include other Taskfiles. Before this was limited to one
+  level (#390, #623, #656).
+- Add ability to specify vars when including a Taskfile.
+  [Check out the documentation](https://taskfile.dev/#/usage?id=vars-of-included-taskfiles)
+  for more information (#677).
 
 ## v3.11.0 - 2022-02-19
 
-- Task now supports printing begin and end messages when using the `group` output mode, useful for grouping tasks in CI systems. [Check out the documentation](http://taskfile.dev/#/usage?id=output-syntax) for more information (#647, #651).
-- Add `Taskfile.dist.yml` and `Taskfile.dist.yaml` to the supported file name list. [Check out the documentation](https://taskfile.dev/#/usage?id=supported-file-names) for more information (#498, #666).
+- Task now supports printing begin and end messages when using the `group`
+  output mode, useful for grouping tasks in CI systems.
+  [Check out the documentation](http://taskfile.dev/#/usage?id=output-syntax)
+  for more information (#647, #651).
+- Add `Taskfile.dist.yml` and `Taskfile.dist.yaml` to the supported file name
+  list.
+  [Check out the documentation](https://taskfile.dev/#/usage?id=supported-file-names)
+  for more information (#498, #666).
 
 ## v3.10.0 - 2022-01-04
 
-- A new `--list-all` (alias `-a`) flag is now available. It's similar to the exiting `--list` (`-l`) but prints all tasks, even those without a description (#383, #401).
-- It's now possible to schedule cleanup commands to run once a task finishes with the `defer:` keyword ([Documentation](https://taskfile.dev/#/usage?id=doing-task-cleanup-with-defer),
-
-  # 475, #626).
-- Remove long deprecated and undocumented `$` variable prefix and `^` command prefix (#642, #644, #645).
-- Add support for `.yaml` extension (as an alternative to `.yml`). This was requested multiple times throughout the years. Enjoy! (#183, #184, #369, #584,
-
-  # 621).
-- Fixed error when computing a variable when the task directory do not exist yet (#481, #579).
+- A new `--list-all` (alias `-a`) flag is now available. It's similar to the
+  exiting `--list` (`-l`) but prints all tasks, even those without a description
+  (#383, #401).
+- It's now possible to schedule cleanup commands to run once a task finishes
+  with the `defer:` keyword
+  ([Documentation](https://taskfile.dev/#/usage?id=doing-task-cleanup-with-defer),
+  #475, #626).
+- Remove long deprecated and undocumented `$` variable prefix and `^` command
+  prefix (#642, #644, #645).
+- Add support for `.yaml` extension (as an alternative to `.yml`). This was
+  requested multiple times throughout the years. Enjoy! (#183, #184, #369, #584,
+  #621).
+- Fixed error when computing a variable when the task directory do not exist yet
+  (#481, #579).
 
 ## v3.9.2 - 2021-12-02
 
-- Upgrade [mvdan/sh](https://github.com/mvdan/sh) which contains a fix a for a important regression on Windows (#619, [mvdan/sh#768](https://github.com/mvdan/sh/issues/768), [mvdan/sh#769](https://github.com/mvdan/sh/pull/769)).
+- Upgrade [mvdan/sh](https://github.com/mvdan/sh) which contains a fix a for a
+  important regression on Windows (#619,
+  [mvdan/sh#768](https://github.com/mvdan/sh/issues/768),
+  [mvdan/sh#769](https://github.com/mvdan/sh/pull/769)).
 
 ## v3.9.1 - 2021-11-28
 
 - Add logging in verbose mode for when a task starts and finishes (#533, #588).
 - Fix an issue with preconditions and context errors (#597, #598).
-- Quote each `{{.CLI_ARGS}}` argument to prevent one with spaces to become many (#613).
+- Quote each `{{.CLI_ARGS}}` argument to prevent one with spaces to become many
+  (#613).
 - Fix nil pointer when `cmd:` was left empty (#612, #614).
-- Upgrade [mvdan/sh](https://github.com/mvdan/sh) which contains two relevant fixes:
-  - Fix quote of empty strings in `shellQuote` (#609, [mvdan/sh#763](https://github.com/mvdan/sh/issues/763)).
-  - Fix issue of wrong environment variable being picked when there's another very similar one (#586, [mvdan/sh#745](https://github.com/mvdan/sh/pull/745)).
-- Install shell completions automatically when installing via Homebrew (#264, #592, [go-task/homebrew-tap#2](https://github.com/go-task/homebrew-tap/pull/2)).
+- Upgrade [mvdan/sh](https://github.com/mvdan/sh) which contains two relevant
+  fixes:
+  - Fix quote of empty strings in `shellQuote` (#609,
+    [mvdan/sh#763](https://github.com/mvdan/sh/issues/763)).
+  - Fix issue of wrong environment variable being picked when there's another
+    very similar one (#586,
+    [mvdan/sh#745](https://github.com/mvdan/sh/pull/745)).
+- Install shell completions automatically when installing via Homebrew (#264,
+  #592,
+  [go-task/homebrew-tap#2](https://github.com/go-task/homebrew-tap/pull/2)).
 
 ## v3.9.0 - 2021-10-02
 
-- A new `shellQuote` function was added to the template system (`{{shellQuote "a string"}}`) to ensure a string is safe for use in shell ([mvdan/sh#727](https://github.com/mvdan/sh/pull/727), [mvdan/sh#737](https://github.com/mvdan/sh/pull/737), [Documentation](https://pkg.go.dev/mvdan.cc/sh/v3@v3.4.0/syntax#Quote))
-- In this version [mvdan.cc/sh](https://github.com/mvdan/sh) was upgraded with some small fixes and features
-  - The `read -p` flag is now supported (#314, [mvdan/sh#551](https://github.com/mvdan/sh/issues/551), [mvdan/sh#772](https://github.com/mvdan/sh/pull/722))
-  - The `pwd -P` and `pwd -L` flags are now supported (#553, [mvdan/sh#724](https://github.com/mvdan/sh/issues/724), [mvdan/sh#728](https://github.com/mvdan/sh/pull/728))
-  - The `$GID` environment variable is now correctly being set (#561, [mvdan/sh#723](https://github.com/mvdan/sh/pull/723))
+- A new `shellQuote` function was added to the template system
+  (`{{shellQuote "a string"}}`) to ensure a string is safe for use in shell
+  ([mvdan/sh#727](https://github.com/mvdan/sh/pull/727),
+  [mvdan/sh#737](https://github.com/mvdan/sh/pull/737),
+  [Documentation](https://pkg.go.dev/mvdan.cc/sh/v3@v3.4.0/syntax#Quote))
+- In this version [mvdan.cc/sh](https://github.com/mvdan/sh) was upgraded with
+  some small fixes and features
+  - The `read -p` flag is now supported (#314,
+    [mvdan/sh#551](https://github.com/mvdan/sh/issues/551),
+    [mvdan/sh#772](https://github.com/mvdan/sh/pull/722))
+  - The `pwd -P` and `pwd -L` flags are now supported (#553,
+    [mvdan/sh#724](https://github.com/mvdan/sh/issues/724),
+    [mvdan/sh#728](https://github.com/mvdan/sh/pull/728))
+  - The `$GID` environment variable is now correctly being set (#561,
+    [mvdan/sh#723](https://github.com/mvdan/sh/pull/723))
 
 ## v3.8.0 - 2021-09-26
 
-- Add `interactive: true` setting to improve support for interactive CLI apps (#217, #563).
+- Add `interactive: true` setting to improve support for interactive CLI apps
+  (#217, #563).
 - Fix some `nil` errors (#534, #573).
 - Add ability to declare an included Taskfile as optional (#519, #552).
-- Add support for including Taskfiles in the home directory by using `~` (#539, #557).
+- Add support for including Taskfiles in the home directory by using `~` (#539,
+  #557).
 
 ## v3.7.3 - 2021-09-04
 
 - Add official support to Apple M1 (#564, #567).
-- Our [official Homebrew tap](https://github.com/go-task/homebrew-tap) will support more platforms, including Apple M1
+- Our [official Homebrew tap](https://github.com/go-task/homebrew-tap) will
+  support more platforms, including Apple M1
 
 ## v3.7.0 - 2021-07-31
 
-- Add `run:` setting to control if tasks should run multiple times or not. Available options are `always` (the default), `when_changed` (if a variable modified the task) and `once` (run only once no matter what). This is a long time requested feature. Enjoy! (#53, #359).
+- Add `run:` setting to control if tasks should run multiple times or not.
+  Available options are `always` (the default), `when_changed` (if a variable
+  modified the task) and `once` (run only once no matter what). This is a long
+  time requested feature. Enjoy! (#53, #359).
 
 ## v3.6.0 - 2021-07-10
 
 - Allow using both `sources:` and `status:` in the same task (#411, #427, #477).
-- Small optimization and bug fix: don't compute variables if not needed for `dotenv:` (#517).
+- Small optimization and bug fix: don't compute variables if not needed for
+  `dotenv:` (#517).
 
 ## v3.5.0 - 2021-07-04
 
 - Add support for interpolation in `dotenv:` (#433, #434, #453).
 
 ## v3.4.3 - 2021-05-30
 
-- Add support for the `NO_COLOR` environment variable. (#459, [fatih/color#137](https://github.com/fatih/color/pull/137)).
-- Fix bug where sources were not considering the right directory in `--watch` mode (#484, #485).
+- Add support for the `NO_COLOR` environment variable. (#459,
+  [fatih/color#137](https://github.com/fatih/color/pull/137)).
+- Fix bug where sources were not considering the right directory in `--watch`
+  mode (#484, #485).
 
 ## v3.4.2 - 2021-04-23
 
 - On watch, report which file failed to read (#472).
 - Do not try to catch SIGKILL signal, which are not actually possible (#476).
-- Improve version reporting when building Task from source using Go Modules (#462, #473).
+- Improve version reporting when building Task from source using Go Modules
+  (#462, #473).
 
 ## v3.4.1 - 2021-04-17
 
-- Improve error reporting when parsing YAML: in some situations where you would just see an generic error, you'll now see the actual error with more detail: the YAML line the failed to parse, for example (#467).
-- A JSON Schema was published [here](https://json.schemastore.org/taskfile.json) and is automatically being used by some editors like Visual Studio Code (#135).
+- Improve error reporting when parsing YAML: in some situations where you would
+  just see an generic error, you'll now see the actual error with more detail:
+  the YAML line the failed to parse, for example (#467).
+- A JSON Schema was published [here](https://json.schemastore.org/taskfile.json)
+  and is automatically being used by some editors like Visual Studio Code
+  (#135).
 - Print task name before the command in the log output (#398).
 
 ## v3.3.0 - 2021-03-20
 
-- Add support for delegating CLI arguments to commands with `--` and a special `CLI_ARGS` variable (#327).
-- Add a `--concurrency` (alias `-C`) flag, to limit the number of tasks that run concurrently. This is useful for heavy workloads. (#345).
+- Add support for delegating CLI arguments to commands with `--` and a special
+  `CLI_ARGS` variable (#327).
+- Add a `--concurrency` (alias `-C`) flag, to limit the number of tasks that run
+  concurrently. This is useful for heavy workloads. (#345).
 
 ## v3.2.2 - 2021-01-12
 
-- Improve performance of `--list` and `--summary` by skipping running shell variables for these flags (#332).
-- Fixed a bug where an environment in a Taskfile was not always overridable by the system environment (#425).
+- Improve performance of `--list` and `--summary` by skipping running shell
+  variables for these flags (#332).
+- Fixed a bug where an environment in a Taskfile was not always overridable by
+  the system environment (#425).
 - Fixed environment from .env files not being available as variables (#379).
 - The install script is now working for ARM platforms (#428).
 
 ## v3.2.1 - 2021-01-09
 
-- Fixed some bugs and regressions regarding dynamic variables and directories (#426).
-- The [slim-sprig](https://github.com/go-task/slim-sprig) package was updated with the upstream [sprig](https://github.com/Masterminds/sprig).
+- Fixed some bugs and regressions regarding dynamic variables and directories
+  (#426).
+- The [slim-sprig](https://github.com/go-task/slim-sprig) package was updated
+  with the upstream [sprig](https://github.com/Masterminds/sprig).
 
 ## v3.2.0 - 2021-01-07
 
-- Fix the `.task` directory being created in the task directory instead of the Taskfile directory (#247).
-- Fix a bug where dynamic variables (those declared with `sh:`) were not running in the task directory when the task has a custom dir or it was in an included Taskfile (#384).
-- The watch feature (via the `--watch` flag) got a few different bug fixes and should be more stable now (#423, #365).
+- Fix the `.task` directory being created in the task directory instead of the
+  Taskfile directory (#247).
+- Fix a bug where dynamic variables (those declared with `sh:`) were not running
+  in the task directory when the task has a custom dir or it was in an included
+  Taskfile (#384).
+- The watch feature (via the `--watch` flag) got a few different bug fixes and
+  should be more stable now (#423, #365).
 
 ## v3.1.0 - 2021-01-03
 
-- Fix a bug when the checksum up-to-date resolution is used by a task with a custom `label:` attribute (#412).
-- Starting from this release, we're releasing official ARMv6 and ARM64 binaries for Linux (#375, #418).
-- Task now respects the order of declaration of included Taskfiles when evaluating variables declaring by them (#393).
-- `set -e` is now automatically set on every command. This was done to fix an issue where multiline string commands wouldn't really fail unless the sentence was in the last line (#403).
+- Fix a bug when the checksum up-to-date resolution is used by a task with a
+  custom `label:` attribute (#412).
+- Starting from this release, we're releasing official ARMv6 and ARM64 binaries
+  for Linux (#375, #418).
+- Task now respects the order of declaration of included Taskfiles when
+  evaluating variables declaring by them (#393).
+- `set -e` is now automatically set on every command. This was done to fix an
+  issue where multiline string commands wouldn't really fail unless the sentence
+  was in the last line (#403).
 
 ## v3.0.1 - 2020-12-26
 
-- Allow use as a library by moving the required packages out of the `internal` directory (#358).
+- Allow use as a library by moving the required packages out of the `internal`
+  directory (#358).
 - Do not error if a specified dotenv file does not exist (#378, #385).
 - Fix panic when you have empty tasks in your Taskfile (#338, #362).
 
 ## v3.0.0 - 2020-08-16
 
 - On `v3`, all CLI variables will be considered global variables (#336, #341)
 - Add support to `.env` like files (#324, #356).
 - Add `label:` to task so you can override the task name in the logs (#321,
-
-  # 337).
+  #337).
 - Refactor how variables work on version 3 (#311).
 - Disallow `expansions` on v3 since it has no effect.
 - `Taskvars.yml` is not automatically included anymore.
 - `Taskfile_{{OS}}.yml` is not automatically included anymore.
-- Allow interpolation on `includes`, so you can manually include a Taskfile based on operation system, for example.
+- Allow interpolation on `includes`, so you can manually include a Taskfile
+  based on operation system, for example.
 - Expose `.TASK` variable in templates with the task name (#252).
 - Implement short task syntax (#194, #240).
-- Added option to make included Taskfile run commands on its own directory (#260, #144)
+- Added option to make included Taskfile run commands on its own directory
+  (#260, #144)
 - Taskfiles in version 1 are not supported anymore (#237).
-- Added global `method:` option. With this option, you can set a default method to all tasks in a Taskfile (#246).
+- Added global `method:` option. With this option, you can set a default method
+  to all tasks in a Taskfile (#246).
 - Changed default method from `timestamp` to `checksum` (#246).
-- New magic variables are now available when using `status:`: `.TIMESTAMP` which contains the greatest modification date from the files listed in `sources:`, and `.CHECKSUM`, which contains a checksum of all files listed in `status:`. This is useful for manual checking when using external, or even remote, artifacts when using `status:` (#216).
-- We're now using [slim-sprig](https://github.com/go-task/slim-sprig) instead of [sprig](https://github.com/Masterminds/sprig), which allowed a file size reduction of about 22% (#219).
-- We now use some colors on Task output to better distinguish message types - commands are green, errors are red, etc (#207).
+- New magic variables are now available when using `status:`: `.TIMESTAMP` which
+  contains the greatest modification date from the files listed in `sources:`,
+  and `.CHECKSUM`, which contains a checksum of all files listed in `status:`.
+  This is useful for manual checking when using external, or even remote,
+  artifacts when using `status:` (#216).
+- We're now using [slim-sprig](https://github.com/go-task/slim-sprig) instead of
+  [sprig](https://github.com/Masterminds/sprig), which allowed a file size
+  reduction of about 22% (#219).
+- We now use some colors on Task output to better distinguish message types -
+  commands are green, errors are red, etc (#207).
 
 ## v2.8.1 - 2020-05-20
 
 - Fix error code for the `--help` flag (#300, #330).
 - Print version to stdout instead of stderr (#299, #329).
 - Supress `context` errors when using the `--watch` flag (#313, #317).
 - Support templating on description (#276, #283).
 
 ## v2.8.0 - 2019-12-07
 
-- Add `--parallel` flag (alias `-p`) to run tasks given by the command line in parallel (#266).
-- Fixed bug where calling the `task` CLI only informing global vars would not execute the `default` task.
-- Add hability to silent all tasks by adding `silent: true` a the root of the Taskfile.
+- Add `--parallel` flag (alias `-p`) to run tasks given by the command line in
+  parallel (#266).
+- Fixed bug where calling the `task` CLI only informing global vars would not
+  execute the `default` task.
+- Add hability to silent all tasks by adding `silent: true` a the root of the
+  Taskfile.
 
 ## v2.7.1 - 2019-11-10
 
 - Fix error being raised when `exit 0` was called (#251).
 
 ## v2.7.0 - 2019-09-22
 
 - Fixed panic bug when assigning a global variable (#229, #243).
-- A task with `method: checksum` will now re-run if generated files are deleted (#228, #238).
+- A task with `method: checksum` will now re-run if generated files are deleted
+  (#228, #238).
 
 ## v2.6.0 - 2019-07-21
 
 - Fixed some bugs regarding minor version checks on `version:`.
 - Add `preconditions:` to task (#205).
 - Create directory informed on `dir:` if it doesn't exist (#209, #211).
-- We now have a `--taskfile` flag (alias `-t`), which can be used to run another Taskfile (other than the default `Taskfile.yml`) (#221).
-- It's now possible to install Task using Homebrew on Linux ([go-task/homebrew-tap#1](https://github.com/go-task/homebrew-tap/pull/1)).
+- We now have a `--taskfile` flag (alias `-t`), which can be used to run another
+  Taskfile (other than the default `Taskfile.yml`) (#221).
+- It's now possible to install Task using Homebrew on Linux
+  ([go-task/homebrew-tap#1](https://github.com/go-task/homebrew-tap/pull/1)).
 
 ## v2.5.2 - 2019-05-11
 
-- Reverted YAML upgrade due issues with CRLF on Windows (#201, [go-yaml/yaml#450](https://github.com/go-yaml/yaml/issues/450)).
+- Reverted YAML upgrade due issues with CRLF on Windows (#201,
+  [go-yaml/yaml#450](https://github.com/go-yaml/yaml/issues/450)).
 - Allow setting global variables through the CLI (#192).
 
 ## 2.5.1 - 2019-04-27
 
-- Fixed some issues with interactive command line tools, where sometimes the output were not being shown, and similar issues (#114, #190, #200).
+- Fixed some issues with interactive command line tools, where sometimes the
+  output were not being shown, and similar issues (#114, #190, #200).
 - Upgraded [go-yaml/yaml](https://github.com/go-yaml/yaml) from v2 to v3.
 
 ## v2.5.0 - 2019-03-16
 
-- We moved from the taskfile.org domain to the new fancy taskfile.dev domain. While stuff is being redirected, we strongly recommend to everyone that use [this install script](https://taskfile.dev/#/installation?id=install-script) to use the new taskfile.dev domain on scripts from now on.
+- We moved from the taskfile.org domain to the new fancy taskfile.dev domain.
+  While stuff is being redirected, we strongly recommend to everyone that use
+  [this install script](https://taskfile.dev/#/installation?id=install-script)
+  to use the new taskfile.dev domain on scripts from now on.
 - Fixed to the ZSH completion (#182).
-- Add [`--summary` flag along with `summary:` task attribute](https://taskfile.org/#/usage?id=display-summary-of-task) (#180).
+- Add
+  [`--summary` flag along with `summary:` task attribute](https://taskfile.org/#/usage?id=display-summary-of-task)
+  (#180).
 
 ## v2.4.0 - 2019-02-21
 
-- Allow calling a task of the root Taskfile from an included Taskfile by prefixing it with `:` (#161, #172).
+- Allow calling a task of the root Taskfile from an included Taskfile by
+  prefixing it with `:` (#161, #172).
 - Add flag to override the `output` option (#173).
-- Fix bug where Task was persisting the new checksum on the disk when the Dry Mode is enabled (#166).
+- Fix bug where Task was persisting the new checksum on the disk when the Dry
+  Mode is enabled (#166).
 - Fix file timestamp issue when the file name has spaces (#176).
 - Mitigating path expanding issues on Windows (#170).
 
 ## v2.3.0 - 2019-01-02
 
 - On Windows, Task can now be installed using [Scoop](https://scoop.sh/) (#152).
 - Fixed issue with file/directory globing (#153).
 - Added ability to globally set environment variables (#138, #159).
 
 ## v2.2.1 - 2018-12-09
 
-- This repository now uses Go Modules (#143). We'll still keep the `vendor` directory in sync for some time, though;
-- Fixing a bug when the Taskfile has no tasks but includes another Taskfile (#150);
-- Fix a bug when calling another task or a dependency in an included Taskfile (#151).
+- This repository now uses Go Modules (#143). We'll still keep the `vendor`
+  directory in sync for some time, though;
+- Fixing a bug when the Taskfile has no tasks but includes another Taskfile
+  (#150);
+- Fix a bug when calling another task or a dependency in an included Taskfile
+  (#151).
 
 ## v2.2.0 - 2018-10-25
 
-- Added support for [including other Taskfiles](https://taskfile.org/#/usage?id=including-other-taskfiles) (#98)
-  - This should be considered experimental. For now, only including local files is supported, but support for including remote Taskfiles is being discussed. If you have any feedback, please comment on #98.
+- Added support for
+  [including other Taskfiles](https://taskfile.org/#/usage?id=including-other-taskfiles)
+  (#98)
+  - This should be considered experimental. For now, only including local files
+    is supported, but support for including remote Taskfiles is being discussed.
+    If you have any feedback, please comment on #98.
 - Task now have a dedicated documentation site: https://taskfile.org
-  - Thanks to [Docsify](https://docsify.js.org/) for making this pretty easy. To check the source code, just take a look at the [docs](https://github.com/go-task/task/tree/main/docs) directory of this repository. Contributions to the documentation is really appreciated.
+  - Thanks to [Docsify](https://docsify.js.org/) for making this pretty easy. To
+    check the source code, just take a look at the
+    [docs](https://github.com/go-task/task/tree/main/docs) directory of this
+    repository. Contributions to the documentation is really appreciated.
 
 ## v2.1.1 - 2018-09-17
 
-- Fix suggestion to use `task --init` not being shown anymore (when a `Taskfile.yml` is not found)
-- Fix error when using checksum method and no file exists for a source glob (#131)
+- Fix suggestion to use `task --init` not being shown anymore (when a
+  `Taskfile.yml` is not found)
+- Fix error when using checksum method and no file exists for a source glob
+  (#131)
 - Fix signal handling when the `--watch` flag is given (#132)
 
 ## v2.1.0 - 2018-08-19
 
 - Add a `ignore_error` option to task and command (#123)
 - Add a dry run mode (`--dry` flag) (#126)
 
 ## v2.0.3 - 2018-06-24
 
 - Expand environment variables on "dir", "sources" and "generates" (#116)
 - Fix YAML merging syntax (#112)
 - Add ZSH completion (#111)
-- Implement new `output` option. Please check out the [documentation](https://github.com/go-task/task#output-syntax)
+- Implement new `output` option. Please check out the
+  [documentation](https://github.com/go-task/task#output-syntax)
 
 ## v2.0.2 - 2018-05-01
 
 - Fix merging of YAML anchors (#112)
 
 ## v2.0.1 - 2018-03-11
 
 - Fixes panic on `task --list`
 
 ## v2.0.0 - 2018-03-08
 
 Version 2.0.0 is here, with a new Taskfile format.
 
-Please, make sure to read the [Taskfile versions](https://github.com/go-task/task/blob/main/TASKFILE_VERSIONS.md) document, since it describes in depth what changed for this version.
+Please, make sure to read the
+[Taskfile versions](https://github.com/go-task/task/blob/main/TASKFILE_VERSIONS.md)
+document, since it describes in depth what changed for this version.
 
 - New Taskfile version 2 (#77)
-- Possibility to have global variables in the `Taskfile.yml` instead of `Taskvars.yml` (#66)
+- Possibility to have global variables in the `Taskfile.yml` instead of
+  `Taskvars.yml` (#66)
 - Small improvements and fixes
 
 ## v1.4.4 - 2017-11-19
 
 - Handle SIGINT and SIGTERM (#75);
 - List: print message with there's no task with description;
 - Expand home dir ("~" symbol) on paths (#74);
@@ -497,29 +802,31 @@
 
 ## v1.4.3 - 2017-09-07
 
 - Allow assigning variables to tasks at run time via CLI (#33)
 - Added suport for multiline variables from sh (#64)
 - Fixes env: remove square braces and evaluate shell (#62)
 - Watch: change watch library and few fixes and improvements
-- When use watching, cancel and restart long running process on file change (#59 and #60)
+- When use watching, cancel and restart long running process on file change (#59
+  and #60)
 
 ## v1.4.2 - 2017-07-30
 
 - Flag to set directory of execution
 - Always echo command if is verbose mode
 - Add silent mode to disable echoing of commands
 - Fixes and improvements of variables (#56)
 
 ## v1.4.1 - 2017-07-15
 
 - Allow use of YAML for dynamic variables instead of $ prefix
   - `VAR: {sh: echo Hello}` instead of `VAR: $echo Hello`
 - Add `--list` (or `-l`) flag to print existing tasks
-- OS specific Taskvars file (e.g. `Taskvars_windows.yml`, `Taskvars_linux.yml`, etc)
+- OS specific Taskvars file (e.g. `Taskvars_windows.yml`, `Taskvars_linux.yml`,
+  etc)
 - Consider task up-to-date on equal timestamps (#49)
 - Allow absolute path in generates section (#48)
 - Bugfix: allow templating when calling deps (#42)
 - Fix panic for invalid task in cyclic dep detection
 - Better error output for dynamic variables in Taskvars.yml (#41)
 - Allow template evaluation in parameters
 
@@ -539,19 +846,21 @@
 - Add status option to prevent task from running (#27)
 - Allow interpolation on `generates` and `sources` attributes (#26)
 
 ## v1.3.0 - 2017-04-24
 
 - Migrate from os/exec.Cmd to a native Go sh/bash interpreter
   - This is a potentially breaking change if you use Windows.
-  - Now, `cmd` is not used anymore on Windows. Always use Bash-like syntax for your commands, even on Windows.
+  - Now, `cmd` is not used anymore on Windows. Always use Bash-like syntax for
+    your commands, even on Windows.
 - Add "ToSlash" and "FromSlash" to template functions
 - Use functions defined on github.com/Masterminds/sprig
 - Do not redirect stdin while running variables commands
-- Using `context` and `errgroup` packages (this will make other tasks to be cancelled, if one returned an error)
+- Using `context` and `errgroup` packages (this will make other tasks to be
+  cancelled, if one returned an error)
 
 ## v1.2.0 - 2017-04-02
 
 - More tests and Travis integration
 - Watch a task (experimental)
 - Possibility to call another task
 - Fix "=" not being reconized in variables/environment variables
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/community.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/community.mdx`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 ---
 slug: /community/
 sidebar_position: 9
 ---
 
 # Community
 
-Some of the work to improve the Task ecosystem is done by the community, be it installation methods or integrations with code editor. I (the author) am thankful for everyone that helps me to improve the overall experience.
+Some of the work to improve the Task ecosystem is done by the community, be it
+installation methods or integrations with code editor. I (the author) am
+thankful for everyone that helps me to improve the overall experience.
 
 ## Translations
 
-We use [Crowdin](https://crowdin.com/project/taskfile) to translate our document.
+We use [Crowdin](https://crowdin.com/project/taskfile) to translate our
+document.
 
 ## Integrations
 
-Many of our integrations are contributed and maintained by the community. You can view the full list of community integrations [here](/integrations#community-integrations).
+Many of our integrations are contributed and maintained by the community. You
+can view the full list of community integrations
+[here](/integrations#community-integrations).
 
 ## Installation methods
 
 Some installation methods are maintained by third party:
 
 - [GitHub Actions](https://github.com/arduino/setup-task) by @arduino
 - [AUR](https://aur.archlinux.org/packages/go-task-bin) by @carlsmedstad
 - [Scoop](https://github.com/ScoopInstaller/Main/blob/master/bucket/task.json)
 - [Fedora](https://packages.fedoraproject.org/pkgs/golang-github-task/go-task/)
 - [NixOS](https://github.com/NixOS/nixpkgs/blob/master/pkgs/development/tools/go-task/default.nix)
 - [Conda](https://github.com/conda-forge/go-task-feedstock/)
 
 ## More
 
-Also, thanks for all the [code contributors](https://github.com/go-task/task/graphs/contributors), [financial contributors](https://opencollective.com/task), all those who [reported bugs](https://github.com/go-task/task/issues?q=is%3Aissue) and [answered questions](https://github.com/go-task/task/discussions).
+Also, thanks for all the
+[code contributors](https://github.com/go-task/task/graphs/contributors),
+[financial contributors](https://opencollective.com/task), all those who
+[reported bugs](https://github.com/go-task/task/issues?q=is%3Aissue) and
+[answered questions](https://github.com/go-task/task/discussions).
 
-If you know something that is missing in this document, please submit a pull request.
+If you know something that is missing in this document, please submit a pull
+request.
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/contributing.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/contributing.mdx`

 * *Files 5% similar despite different names*

```diff
@@ -1,101 +1,167 @@
 ---
 slug: /contributing/
 sidebar_position: 11
 ---
 
 # Contributing
 
-Contributions to Task are very welcome, but we ask that you read this document before submitting a PR.
+Contributions to Task are very welcome, but we ask that you read this document
+before submitting a PR.
 
 :::note
 
-This document applies to the core [Task][task] repository _and_ [Task for Visual Studio Code][vscode-task].
+This document applies to the core [Task][task] repository _and_ [Task for Visual
+Studio Code][vscode-task].
 
 :::
 
 ## Before you start
 
-- **Check existing work** - Is there an existing PR? Are there issues discussing the feature/change you want to make? Please make sure you consider/address these discussions in your work.
-- **Backwards compatibility** - Will your change break existing Taskfiles? It is much more likely that your change will merged if it backwards compatible. Is there an approach you can take that maintains this compatibility? If not, consider opening an issue first so that API changes can be discussed before you invest your time into a PR.
-- **Experiments** - If there is no way to make your change backward compatible then there is a procedure to introduce breaking changes into minor versions. We call these "\[experiments\]\[experiments\]". If you're intending to work on an experiment, then please read the \[experiments workflow\]\[experiments-workflow\] document carefully and submit a proposal first.
+- **Check existing work** - Is there an existing PR? Are there issues discussing
+  the feature/change you want to make? Please make sure you consider/address
+  these discussions in your work.
+- **Backwards compatibility** - Will your change break existing Taskfiles? It is
+  much more likely that your change will merged if it backwards compatible. Is
+  there an approach you can take that maintains this compatibility? If not,
+  consider opening an issue first so that API changes can be discussed before
+  you invest your time into a PR.
+- **Experiments** - If there is no way to make your change backward compatible
+  then there is a procedure to introduce breaking changes into minor versions.
+  We call these "[experiments][experiments]". If you're intending to work on an
+  experiment, then please read the [experiments workflow][experiments-workflow]
+  document carefully and submit a proposal first.
 
 ## 1. Setup
 
-- **Go** - Task is written in [Go][go]. We always support the latest two major Go versions, so make sure your version is recent enough.
-- **Node.js** - [Node.js][nodejs] is used to host Task's documentation server and is required if you want to run this server locally. It is also required if you want to contribute to the Visual Studio Code extension.
+- **Go** - Task is written in [Go][go]. We always support the latest two major
+  Go versions, so make sure your version is recent enough.
+- **Node.js** - [Node.js][nodejs] is used to host Task's documentation server
+  and is required if you want to run this server locally. It is also required if
+  you want to contribute to the Visual Studio Code extension.
 - **Yarn** - [Yarn][yarn] is the Node.js package manager used by Task.
 
 ## 2. Making changes
 
-- **Code style** - Try to maintain the existing code style where possible. Go code should be formatted by [`gofumpt`][gofumpt] and linted using [`golangci-lint`][golangci-lint]. Any Markdown or TypeScript files should be formatted and linted by [Prettier][prettier]. This style is enforced by our CI to ensure that we have a consistent style across the project. You can use the `task lint` command to lint the code locally and the `task lint:fix` command to automatically fix any issues that are found.
-- **Documentation** - Ensure that you add/update any relevant documentation. See the [updating documentation](#updating-documentation) section below.
-- **Tests** - Ensure that you add/update any relevant tests and that all tests are passing before submitting the PR. See the [writing tests](#writing-tests) section below.
+- **Code style** - Try to maintain the existing code style where possible. Go
+  code should be formatted by [`gofumpt`][gofumpt] and linted using
+  [`golangci-lint`][golangci-lint]. Any Markdown or TypeScript files should be
+  formatted and linted by [Prettier][prettier]. This style is enforced by our CI
+  to ensure that we have a consistent style across the project. You can use the
+  `task lint` command to lint the code locally and the `task lint:fix` command
+  to automatically fix any issues that are found.
+- **Documentation** - Ensure that you add/update any relevant documentation. See
+  the [updating documentation](#updating-documentation) section below.
+- **Tests** - Ensure that you add/update any relevant tests and that all tests
+  are passing before submitting the PR. See the [writing tests](#writing-tests)
+  section below.
 
 ### Running your changes
 
-To run Task with working changes, you can use `go run ./cmd/task`. To run a development build of task against a test Taskfile in `testdata`, you can use `go run ./cmd/task --dir ./testdata/<my_test_dir> <task_name>`.
-
-To run Task for Visual Studio Code, you can open the project in VSCode and hit F5 (or whatever you debug keybind is set to). This will open a new VSCode window with the extension running. Debugging this way is recommended as it will allow you to set breakpoints and step through the code. Otherwise, you can run `task package` which will generate a `.vsix` file that can be used to manually install the extension.
+To run Task with working changes, you can use `go run ./cmd/task`. To run a
+development build of task against a test Taskfile in `testdata`, you can use
+`go run ./cmd/task --dir ./testdata/<my_test_dir> <task_name>`.
+
+To run Task for Visual Studio Code, you can open the project in VSCode and hit
+F5 (or whatever you debug keybind is set to). This will open a new VSCode window
+with the extension running. Debugging this way is recommended as it will allow
+you to set breakpoints and step through the code. Otherwise, you can run
+`task package` which will generate a `.vsix` file that can be used to manually
+install the extension.
 
 ### Updating documentation
 
-Task uses [Docusaurus][docusaurus] to host a documentation server. The code for this is located in the core Task repository. This can be setup and run locally by using `task docs` (requires `nodejs` & `yarn`). All content is written in Markdown and is located in the `docs/docs` directory. All Markdown documents should have an 80 character line wrap limit (enforced by Prettier).
-
-When making a change, consider whether a change to the [Usage Guide](/usage) is necessary. This document contains descriptions and examples of how to use Task features. If you're adding a new feature, try to find an appropriate place to add a new section. If you're updating an existing feature, ensure that the documentation and any examples are up-to-date. Ensure that any examples follow the [Taskfile Styleguide](/styleguide).
-
-If you added a new field, command or flag, ensure that you add it to the [API Reference](/api). New fields also need to be added to the [JSON Schema][json-schema]. The descriptions for fields in the API reference and the schema should match.
+Task uses [Docusaurus][docusaurus] to host a documentation server. The code for
+this is located in the core Task repository. This can be setup and run locally
+by using `task website` (requires `nodejs` & `yarn`). All content is written in
+Markdown and is located in the `website/docs` directory. All Markdown documents
+should have an 80 character line wrap limit (enforced by Prettier).
+
+When making a change, consider whether a change to the [Usage Guide](/usage) is
+necessary. This document contains descriptions and examples of how to use Task
+features. If you're adding a new feature, try to find an appropriate place to
+add a new section. If you're updating an existing feature, ensure that the
+documentation and any examples are up-to-date. Ensure that any examples follow
+the [Taskfile Styleguide](/styleguide).
+
+If you added a new field, command or flag, ensure that you add it to the
+[API Reference](/api). New fields also need to be added to the [JSON
+Schema][json-schema]. The descriptions for fields in the API reference and the
+schema should match.
 
 ### Writing tests
 
-A lot of Task's tests are held in the `task_test.go` file in the project root and this is where you'll most likely want to add new ones too. Most of these tests also have a subdirectory in the `testdata` directory where any Taskfiles/data required to run the tests are stored.
-
-When making a changes, consider whether new tests are required. These tests should ensure that the functionality you are adding will continue to work in the future. Existing tests may also need updating if you have changed Task's behavior.
-
-You may also consider adding unit tests for any new functions you have added. The unit tests should follow the Go convention of being location in a file named `*_test.go` in the same package as the code being tested.
+A lot of Task's tests are held in the `task_test.go` file in the project root
+and this is where you'll most likely want to add new ones too. Most of these
+tests also have a subdirectory in the `testdata` directory where any
+Taskfiles/data required to run the tests are stored.
+
+When making a changes, consider whether new tests are required. These tests
+should ensure that the functionality you are adding will continue to work in the
+future. Existing tests may also need updating if you have changed Task's
+behavior.
+
+You may also consider adding unit tests for any new functions you have added.
+The unit tests should follow the Go convention of being location in a file named
+`*_test.go` in the same package as the code being tested.
 
 ## 3. Committing your code
 
-Try to write meaningful commit messages and avoid having too many commits on the PR. Most PRs should likely have a single commit (although for bigger PRs it may be reasonable to split it in a few). Git squash and rebase is your friend!
-
-If you're not sure how to format your commit message, check out [Conventional Commits][conventional-commits]. This style is not enforced, but it is a good way to make your commit messages more readable and consistent.
+Try to write meaningful commit messages and avoid having too many commits on the
+PR. Most PRs should likely have a single commit (although for bigger PRs it may
+be reasonable to split it in a few). Git squash and rebase is your friend!
+
+If you're not sure how to format your commit message, check out [Conventional
+Commits][conventional-commits]. This style is not enforced, but it is a good way
+to make your commit messages more readable and consistent.
 
 ## 4. Submitting a PR
 
-- **Describe your changes** - Ensure that you provide a comprehensive description of your changes.
-- **Issue/PR links** - Link any previous work such as related issues or PRs. Please describe how your changes differ to/extend this work.
-- **Examples** - Add any examples or screenshots that you think are useful to demonstrate the effect of your changes.
-- **Draft PRs** - If your changes are incomplete, but you would like to discuss them, open the PR as a draft and add a comment to start a discussion. Using comments rather than the PR description allows the description to be updated later while preserving any discussions.
+- **Describe your changes** - Ensure that you provide a comprehensive
+  description of your changes.
+- **Issue/PR links** - Link any previous work such as related issues or PRs.
+  Please describe how your changes differ to/extend this work.
+- **Examples** - Add any examples or screenshots that you think are useful to
+  demonstrate the effect of your changes.
+- **Draft PRs** - If your changes are incomplete, but you would like to discuss
+  them, open the PR as a draft and add a comment to start a discussion. Using
+  comments rather than the PR description allows the description to be updated
+  later while preserving any discussions.
 
 ## FAQ
 
 > I want to contribute, where do I start?
 
-Take a look at the list of [open issues for Task][task-open-issues] or [Task for Visual Studio Code][vscode-task-open-issues]. We have a [good first issue][good-first-issue] label for simpler issues that are ideal for first time contributions.
-
-All kinds of contributions are welcome, whether its a typo fix or a shiny new feature. You can also contribute by upvoting/commenting on issues, helping to answer questions or contributing to other [community projects](/community).
+Take a look at the list of [open issues for Task][task-open-issues] or [Task for
+Visual Studio Code][vscode-task-open-issues]. We have a [good first
+issue][good-first-issue] label for simpler issues that are ideal for first time
+contributions.
+
+All kinds of contributions are welcome, whether its a typo fix or a shiny new
+feature. You can also contribute by upvoting/commenting on issues, helping to
+answer questions or contributing to other [community projects](/community).
 
 > I'm stuck, where can I get help?
 
-If you have questions, feel free to ask them in the `#help` forum channel on our [Discord server][discord-server] or open a [Discussion][discussion] on GitHub.
+If you have questions, feel free to ask them in the `#help` forum channel on our
+[Discord server][discord-server] or open a [Discussion][discussion] on GitHub.
 
 ---
 
-<!-- prettier-ignore-start -->
-
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [task]: https://github.com/go-task/task
 [vscode-task]: https://github.com/go-task/vscode-task
 [go]: https://go.dev
 [gofumpt]: https://github.com/mvdan/gofumpt
 [golangci-lint]: https://golangci-lint.run
 [prettier]: https://prettier.io
 [nodejs]: https://nodejs.org/en/
 [yarn]: https://yarnpkg.com/
 [docusaurus]: https://docusaurus.io
-[json-schema]: https://github.com/go-task/task/blob/main/docs/static/schema.json
+[json-schema]: https://github.com/go-task/task/blob/main/website/static/schema.json
 [task-open-issues]: https://github.com/go-task/task/issues
 [vscode-task-open-issues]: https://github.com/go-task/vscode-task/issues
 [good-first-issue]: https://github.com/go-task/task/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22
 [discord-server]: https://discord.gg/6TY36E39UK
 [discussion]: https://github.com/go-task/task/discussions
 [conventional-commits]: https://www.conventionalcommits.org
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/deprecations/deprecations.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/deprecations.mdx`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 ---
 slug: /deprecations/
 sidebar_position: 7
 ---
 
 # Deprecations
 
-As Task evolves, it occasionally outgrows some of its functionality. This can be because they are no longer useful, because another feature has replaced it or because of a change in the way that Task works internally.
+As Task evolves, it occasionally outgrows some of its functionality. This can be
+because they are no longer useful, because another feature has replaced it or
+because of a change in the way that Task works internally.
 
-When this happens, we mark the functionality as deprecated. This means that it will be removed in a future version of Task. This functionality will continue to work until that time, but we strongly recommend that you do not implement this functionality in new Taskfiles and make a plan to migrate away from it as soon as possible.
+When this happens, we mark the functionality as deprecated. This means that it
+will be removed in a future version of Task. This functionality will continue to
+work until that time, but we strongly recommend that you do not implement this
+functionality in new Taskfiles and make a plan to migrate away from it as soon
+as possible.
 
-You can view a full list of active deprecations in the "Deprecations" section of the sidebar.
+You can view a full list of active deprecations in the "Deprecations" section of
+the sidebar.
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/deprecations/template.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/template.mdx`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ---
-#This is a template for an experiments documentation
-#Copy this page and fill in the details as necessary
+# This is a template for an experiments documentation
+# Copy this page and fill in the details as necessary
 title: '--- Template ---'
-sidebar_position: -1 #Always push to the top
-draft: true #Hide in production
+sidebar_position: -1 # Always push to the top
+draft: true # Hide in production
 ---
 
 # \{Name of Deprecated Feature\} (#\{Issue\})
 
 :::warning
 
 This deprecation breaks the following functionality:
@@ -15,8 +15,9 @@
 - \{list any existing functionality that will be broken by this deprecation\}
 - \{if there are no breaking changes, remove this admonition\}
 
 :::
 
 \{Short description of the feature/behavior and why it is being deprecated\}
 
-\{Short explanation of any replacement features/behaviors and how users should migrate to it\}
+\{Short explanation of any replacement features/behaviors and how users should
+migrate to it\}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/deprecations/version_2_schema.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/version_2_schema.mdx`

 * *Files 17% similar despite different names*

```diff
@@ -9,17 +9,25 @@
 This deprecation breaks the following functionality:
 
 - Any Taskfiles that use the version 2 schema
 - `Taskvar.yml` files
 
 :::
 
-The Taskfile version 2 schema was introduced in March 2018 and replaced by version 3 in August 2019. In May 2023 [we published a deprecation notice][deprecation-notice] for the version 2 schema on the basis that the vast majority of users had already upgraded to version 3 and removing support for version 2 would allow us to tidy up the codebase and focus on new functionality instead.
+The Taskfile version 2 schema was introduced in March 2018 and replaced by
+version 3 in August 2019. In May 2023 [we published a deprecation
+notice][deprecation-notice] for the version 2 schema on the basis that the vast
+majority of users had already upgraded to version 3 and removing support for
+version 2 would allow us to tidy up the codebase and focus on new functionality
+instead.
+
+In December 2023, the final version of Task that supports the version 2 schema
+([v3.33.0][v3.33.0]) was published and all legacy code was removed from Task's
+main branch. To use a more recent version of Task, you will need to ensure that
+your Taskfile uses the version 3 schema instead. A list of changes between
+version 2 and version 3 are available in the [Task v3 Release Notes][v3.0.0].
 
-In December 2023, the final version of Task that supports the version 2 schema ([v3.33.0][v3.33.0]) was published and all legacy code was removed from Task's main branch. To use a more recent version of Task, you will need to ensure that your Taskfile uses the version 3 schema instead. A list of changes between version 2 and version 3 are available in the [Task v3 Release Notes][v3.0.0].
-
-<!-- prettier-ignore-start -->
-
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [v3.0.0]: https://github.com/go-task/task/releases/tag/v3.0.0
 [v3.33.0]: https://github.com/go-task/task/releases/tag/v3.33.0
 [deprecation-notice]: https://github.com/go-task/task/issues/1197
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/experiments.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/experiments.mdx`

 * *Files 13% similar despite different names*

```diff
@@ -3,77 +3,129 @@
 sidebar_position: 6
 ---
 
 # Experiments
 
 :::caution
 
-All experimental features are subject to breaking changes and/or removal _at any time_. We strongly recommend that you do not use these features in a production environment. They are intended for testing and feedback only.
+All experimental features are subject to breaking changes and/or removal _at any
+time_. We strongly recommend that you do not use these features in a production
+environment. They are intended for testing and feedback only.
 
 :::
 
-In order to allow Task to evolve quickly, we roll out breaking changes to minor versions behind experimental flags. This allows us to gather feedback on breaking changes before committing to a major release. This document describes the current set of experimental features and their status in the [workflow](#workflow).
+In order to allow Task to evolve quickly, we sometimes roll out breaking changes
+to minor versions behind experimental flags. This allows us to gather feedback
+on breaking changes before committing to a major release. This process can also
+be used to gather feedback on important non-breaking features before their
+design is completed. This document describes the
+[experiment workflow](#workflow) and how you can get involved.
 
-You can view a full list of active experiments in the "Experiments" section of the sidebar.
+You can view the full list of active experiments in the sidebar submenu to the
+left of the page and click on each one to find out more about it.
 
 ## Enabling Experiments
 
-You can enable an experimental feature by doing one of the following:
-
-1. Using the relevant environment variable in front of a task command. For example, `TASK_X_{FEATURE}=1 task {my-task}`. This is intended for one-off invocations of Task to test out experimental features.
-1. Using the relevant environment variable in your "dotfiles" (e.g. `.bashrc`, `.zshrc` etc.). This is intended for permanently enabling experimental features in your environment.
-1. Creating a `.env` file in the same directory as your root Taskfile that contains the relevant environment variables. This allows you to enable an experimental feature at a project level. For example:
-
-```shell title=".env"
-TASK_X_FEATURE=1
-```
-
-## Current Experimental Features and Deprecations
-
-Each section below details an experiment or deprecation and explains what the flags/environment variables to enable the experiment are and how the feature's behavior will change. It will also explain what you need to do to migrate any existing Taskfiles to the new behavior.
+Task uses environment variables to detect whether or not an experiment is
+enabled. All of the experiment variables will begin with the same `TASK_X_`
+prefix followed by the name of the experiment. You can find the exact name for
+each experiment on their respective pages in the sidebar. If the variable is set
+`=1` then it will be enabled. Some experiments may have multiple proposals, in
+which case, you will need to set the variable equal to the number of the
+proposal that you want to enable (`=2`, `=3` etc).
+
+There are three main ways to set the environment variables for an experiment.
+Which method you use depends on how you intend to use the experiment:
+
+1. Prefixing your task commands with the relevant environment variable(s). For
+   example, `TASK_X_{FEATURE}=1 task {my-task}`. This is intended for one-off
+   invocations of Task to test out experimental features.
+1. Adding the relevant environment variable(s) in your "dotfiles" (e.g.
+   `.bashrc`, `.zshrc` etc.). This will permanently enable experimental features
+   for your personal environment.
+
+   ```shell title="~/.bashrc"
+   export TASK_X_FEATURE=1
+   ```
+
+1. Creating a `.env` file in the same directory as your root Taskfile that
+   contains the relevant environment variable(s). This allows you to enable an
+   experimental feature at a project level. If you commit the `.env` file to
+   source control then other users of your project will also have these
+   experiments enabled.
+
+   ```shell title=".env"
+   TASK_X_FEATURE=1
+   ```
 
 ## Workflow
 
-Experiments are a way for us to test out new features in Task before committing to them in a major release. Because this concept is built around the idea of feedback from our community, we have built a workflow for the process of introducing these changes. This ensures that experiments are given the attention and time that they need and that we are getting the best possible results out of them.
-
-The sections below describe the various stages that an experiment must go through from its proposal all the way to being released in a major version of Task.
+Experiments are a way for us to test out new features in Task before committing
+to them in a major release. Because this concept is built around the idea of
+feedback from our community, we have built a workflow for the process of
+introducing these changes. This ensures that experiments are given the attention
+and time that they need and that we are getting the best possible results out of
+them.
+
+The sections below describe the various stages that an experiment must go
+through from its proposal all the way to being released in a major version of
+Task.
 
 ### 1. Proposal
 
-All experimental features start with a proposal in the form of a GitHub issue. If the maintainers decide that an issue has enough support and is a breaking change or is complex/controversial enough to require user feedback, then the issue will be marked with the ![proposal][] label. At this point, the issue becomes a proposal and a period of consultation begins. During this period, we request that users provide feedback on the proposal and how it might effect their use of Task. It is up to the discretion of the maintainers to decide how long this period lasts.
+All experimental features start with a proposal in the form of a GitHub issue.
+If the maintainers decide that an issue has enough support and is a breaking
+change or is complex/controversial enough to require user feedback, then the
+issue will be marked with the `experiment: proposal` label. At this point, the
+issue becomes a proposal and a period of consultation begins. During this
+period, we request that users provide feedback on the proposal and how it might
+effect their use of Task. It is up to the discretion of the maintainers to
+decide how long this period lasts.
 
 ### 2. Draft
 
-Once a proposal's consultation ends, a contributor may pick up the work and begin the initial implementation. Once a PR is opened, the maintainers will ensure that it meets the requirements for an experimental feature (i.e. flags are in the right format etc) and merge the feature. Once this code is released, the status will be updated via the ![draft][] label. This indicates that an implementation is now available for use in a release and the experiment is open for feedback.
+Once a proposal's consultation ends, a contributor may pick up the work and
+begin the initial implementation. Once a PR is opened, the maintainers will
+ensure that it meets the requirements for an experimental feature (i.e. flags
+are in the right format etc) and merge the feature. Once this code is released,
+the status will be updated via the `experiment: draft` label. This indicates
+that an implementation is now available for use in a release and the experiment
+is open for feedback.
 
 :::note
 
-During the draft period, major changes to the implementation may be made based on the feedback received from users. There are _no stability guarantees_ and experimental features may be abandoned _at any time_.
+During the draft period, major changes to the implementation may be made based
+on the feedback received from users. There are _no stability guarantees_ and
+experimental features may be abandoned _at any time_.
 
 :::
 
 ### 3. Candidate
 
-Once an acceptable level of consensus has been reached by the community and feedback/changes are less frequent/significant, the status may be updated via the ![candidate][] label. This indicates that a proposal is _likely_ to accepted and will enter a period for final comments and minor changes.
+Once an acceptable level of consensus has been reached by the community and
+feedback/changes are less frequent/significant, the status may be updated via
+the `experiment: candidate` label. This indicates that a proposal is _likely_ to
+accepted and will enter a period for final comments and minor changes.
 
 ### 4. Stable
 
-Once a suitable amount of time has passed with no changes or feedback, an experiment will be given the ![stable][] label. At this point, the functionality will be treated like any other feature in Task and any changes _must_ be backward compatible. This allows users to migrate to the new functionality without having to worry about anything breaking in future releases. This provides the best experience for users migrating to a new major version.
+Once a suitable amount of time has passed with no changes or feedback, an
+experiment will be given the `experiment: stable` label. At this point, the
+functionality will be treated like any other feature in Task and any changes
+_must_ be backward compatible. This allows users to migrate to the new
+functionality without having to worry about anything breaking in future
+releases. This provides the best experience for users migrating to a new major
+version.
 
 ### 5. Released
 
-When making a new major release of Task, all experiments marked as ![stable][] will move to ![released][] and their behaviors will become the new default in Task. Experiments in an earlier stage (i.e. not stable) cannot be released and so will continue to be experiments in the new version.
+When making a new major release of Task, all experiments marked as
+`experiment: stable` will move to `experiment: released` and their behaviors
+will become the new default in Task. Experiments in an earlier stage (i.e. not
+stable) cannot be released and so will continue to be experiments in the new
+version.
 
 ### Abandoned / Superseded
 
-If an experiment is unsuccessful at any point then it will be given the ![abandoned][] or ![superseded][] labels depending on which is more suitable. These experiments will be removed from Task.
-
-<!-- prettier-ignore-start -->
-
-<!-- prettier-ignore-end -->
-[proposal]: https://img.shields.io/badge/experiment:%20proposal-purple
-[draft]: https://img.shields.io/badge/experiment:%20draft-purple
-[candidate]: https://img.shields.io/badge/experiment:%20candidate-purple
-[stable]: https://img.shields.io/badge/experiment:%20stable-purple
-[released]: https://img.shields.io/badge/experiment:%20released-purple
-[abandoned]: https://img.shields.io/badge/experiment:%20abandoned-purple
-[superseded]: https://img.shields.io/badge/experiment:%20superseded-purple
+If an experiment is unsuccessful at any point then it will be given the
+`experiment: abandoned` or `experiment: superseded` labels depending on which is
+more suitable. These experiments will be removed from Task.
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/gentle_force.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/gentle_force.mdx`

 * *Files 10% similar despite different names*

```diff
@@ -2,35 +2,48 @@
 slug: /experiments/gentle-force/
 ---
 
 # Gentle Force (#1200)
 
 :::caution
 
-All experimental features are subject to breaking changes and/or removal _at any time_. We strongly recommend that you do not use these features in a production environment. They are intended for testing and feedback only.
+All experimental features are subject to breaking changes and/or removal _at any
+time_. We strongly recommend that you do not use these features in a production
+environment. They are intended for testing and feedback only.
 
 :::
 
 :::warning
 
 This experiment breaks the following functionality:
 
 - The `--force` flag
 
 :::
 
 :::info
 
-To enable this experiment, set the environment variable: `TASK_X_FORCE=1`. Check out [our guide to enabling experiments ][enabling-experiments] for more information.
+To enable this experiment, set the environment variable:
+`TASK_X_GENTLE_FORCE=1`. Check out [our guide to enabling experiments
+][enabling-experiments] for more information.
 
 :::
 
-The `--force` flag currently forces _all_ tasks to run regardless of the status checks. This can be useful, but we have found that most of the time users only expect the direct task they are calling to be forced and _not_ all of its dependant tasks.
+The `--force` flag currently forces _all_ tasks to run regardless of the status
+checks. This can be useful, but we have found that most of the time users only
+expect the direct task they are calling to be forced and _not_ all of its
+dependant tasks.
+
+This experiment changes the `--force` flag to only force the directly called
+task. All dependant tasks will have their statuses checked as normal and will
+only run if Task considers them to be out of date. A new `--force-all` flag will
+also be added to maintain the current behavior for users that need this
+functionality.
+
+If you want to migrate, but continue to force all dependant tasks to run, you
+should replace all uses of the `--force` flag with `--force-all`. Alternatively,
+if you want to adopt the new behavior, you can continue to use the `--force`
+flag as you do now!
 
-This experiment changes the `--force` flag to only force the directly called task. All dependant tasks will have their statuses checked as normal and will only run if Task considers them to be out of date. A new `--force-all` flag will also be added to maintain the current behavior for users that need this functionality.
-
-If you want to migrate, but continue to force all dependant tasks to run, you should replace all uses of the `--force` flag with `--force-all`. Alternatively, if you want to adopt the new behavior, you can continue to use the `--force` flag as you do now!
-
-<!-- prettier-ignore-start -->
-
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [enabling-experiments]: /experiments/#enabling-experiments
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/remote_taskfiles.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/remote_taskfiles.mdx`

 * *Files 9% similar despite different names*

```diff
@@ -2,65 +2,103 @@
 slug: /experiments/remote-taskfiles/
 ---
 
 # Remote Taskfiles (#1317)
 
 :::caution
 
-All experimental features are subject to breaking changes and/or removal _at any time_. We strongly recommend that you do not use these features in a production environment. They are intended for testing and feedback only.
+All experimental features are subject to breaking changes and/or removal _at any
+time_. We strongly recommend that you do not use these features in a production
+environment. They are intended for testing and feedback only.
 
 :::
 
 :::info
 
-To enable this experiment, set the environment variable: `TASK_X_REMOTE_TASKFILES=1`. Check out [our guide to enabling experiments ][enabling-experiments] for more information.
+To enable this experiment, set the environment variable:
+`TASK_X_REMOTE_TASKFILES=1`. Check out [our guide to enabling experiments
+][enabling-experiments] for more information.
 
 :::
 
-This experiment allows you to specify a remote Taskfile URL when including a Taskfile. For example:
+This experiment allows you to specify a remote Taskfile URL when including a
+Taskfile. For example:
 
 ```yaml
 version: '3'
 
 includes:
   my-remote-namespace: https://raw.githubusercontent.com/my-org/my-repo/main/Taskfile.yml
 ```
 
-This works exactly the same way that including a local file does. Any tasks in the remote Taskfile will be available to run from your main Taskfile via the namespace `my-remote-namespace`. For example, if the remote file contains the following:
+This works exactly the same way that including a local file does. Any tasks in
+the remote Taskfile will be available to run from your main Taskfile via the
+namespace `my-remote-namespace`. For example, if the remote file contains the
+following:
 
 ```yaml
 version: '3'
 
 tasks:
   hello:
     silent: true
     cmds:
       - echo "Hello from the remote Taskfile!"
 ```
 
-and you run `task my-remote-namespace:hello`, it will print the text: "Hello from the remote Taskfile!" to your console.
+and you run `task my-remote-namespace:hello`, it will print the text: "Hello
+from the remote Taskfile!" to your console.
 
 ## Security
 
-Running commands from sources that you do not control is always a potential security risk. For this reason, we have added some checks when using remote Taskfiles:
-
-1. When running a task from a remote Taskfile for the first time, Task will print a warning to the console asking you to check that you are sure that you trust the source of the Taskfile. If you do not accept the prompt, then Task will exit with code `104` (not trusted) and nothing will run. If you accept the prompt, the remote Taskfile will run and further calls to the remote Taskfile will not prompt you again.
-2. Whenever you run a remote Taskfile, Task will create and store a checksum of the file that you are running. If the checksum changes, then Task will print another warning to the console to inform you that the contents of the remote file has changed. If you do not accept the prompt, then Task will exit with code `104` (not trusted) and nothing will run. If you accept the prompt, the checksum will be updated and the remote Taskfile will run.
-
-Sometimes you need to run Task in an environment that does not have an interactive terminal, so you are not able to accept a prompt. In these cases you are able to tell task to accept these prompts automatically by using the `--yes` flag. Before enabling this flag, you should:
+Running commands from sources that you do not control is always a potential
+security risk. For this reason, we have added some checks when using remote
+Taskfiles:
+
+1. When running a task from a remote Taskfile for the first time, Task will
+   print a warning to the console asking you to check that you are sure that you
+   trust the source of the Taskfile. If you do not accept the prompt, then Task
+   will exit with code `104` (not trusted) and nothing will run. If you accept
+   the prompt, the remote Taskfile will run and further calls to the remote
+   Taskfile will not prompt you again.
+2. Whenever you run a remote Taskfile, Task will create and store a checksum of
+   the file that you are running. If the checksum changes, then Task will print
+   another warning to the console to inform you that the contents of the remote
+   file has changed. If you do not accept the prompt, then Task will exit with
+   code `104` (not trusted) and nothing will run. If you accept the prompt, the
+   checksum will be updated and the remote Taskfile will run.
+
+Sometimes you need to run Task in an environment that does not have an
+interactive terminal, so you are not able to accept a prompt. In these cases you
+are able to tell task to accept these prompts automatically by using the `--yes`
+flag. Before enabling this flag, you should:
 
 1. Be sure that you trust the source and contents of the remote Taskfile.
-2. Consider using a pinned version of the remote Taskfile (e.g. A link containing a commit hash) to prevent Task from automatically accepting a prompt that says a remote Taskfile has changed.
-
-Task currently supports both `http` and `https` URLs. However, the `http` requests will not execute by default unless you run the task with the `--insecure` flag. This is to protect you from accidentally running a remote Taskfile that is hosted on and unencrypted connection. Sources that are not protected by TLS are vulnerable to [man-in-the-middle attacks][man-in-the-middle-attacks] and should be avoided unless you know what you are doing.
+2. Consider using a pinned version of the remote Taskfile (e.g. A link
+   containing a commit hash) to prevent Task from automatically accepting a
+   prompt that says a remote Taskfile has changed.
+
+Task currently supports both `http` and `https` URLs. However, the `http`
+requests will not execute by default unless you run the task with the
+`--insecure` flag. This is to protect you from accidentally running a remote
+Taskfile that is via an unencrypted connection. Sources that are not protected
+by TLS are vulnerable to [man-in-the-middle attacks][man-in-the-middle-attacks]
+and should be avoided unless you know what you are doing.
 
 ## Caching & Running Offline
 
-Whenever you run a remote Taskfile, the latest copy will be downloaded from the internet and cached locally. If for whatever reason, you lose access to the internet, you will still be able to run your tasks by specifying the `--offline` flag. This will tell Task to use the latest cached version of the file instead of trying to download it. You are able to use the `--download` flag to update the cached version of the remote files without running any tasks.
-
-By default, Task will timeout requests to download remote files after 10 seconds and look for a cached copy instead. This timeout can be configured by setting the `--timeout` flag and specifying a duration. For example, `--timeout 5s` will set the timeout to 5 seconds.
-
-<!-- prettier-ignore-start -->
+Whenever you run a remote Taskfile, the latest copy will be downloaded from the
+internet and cached locally. If for whatever reason, you lose access to the
+internet, you will still be able to run your tasks by specifying the `--offline`
+flag. This will tell Task to use the latest cached version of the file instead
+of trying to download it. You are able to use the `--download` flag to update
+the cached version of the remote files without running any tasks.
+
+By default, Task will timeout requests to download remote files after 10 seconds
+and look for a cached copy instead. This timeout can be configured by setting
+the `--timeout` flag and specifying a duration. For example, `--timeout 5s` will
+set the timeout to 5 seconds.
 
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [enabling-experiments]: /experiments/#enabling-experiments
 [man-in-the-middle-attacks]: https://en.wikipedia.org/wiki/Man-in-the-middle_attack
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/experiments/template.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/template.mdx`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 ---
-#This is a template for an experiments documentation
-#Copy this page and fill in the details as necessary
+# This is a template for an experiments documentation
+# Copy this page and fill in the details as necessary
 title: '--- Template ---'
-sidebar_position: -1 #Always push to the top
-draft: true #Hide in production
+sidebar_position: -1 # Always push to the top
+draft: true # Hide in production
 ---
 
 # \{Name of Experiment\} (#\{Issue\})
 
 :::caution
 
-All experimental features are subject to breaking changes and/or removal _at any time_. We strongly recommend that you do not use these features in a production environment. They are intended for testing and feedback only.
+All experimental features are subject to breaking changes and/or removal _at any
+time_. We strongly recommend that you do not use these features in a production
+environment. They are intended for testing and feedback only.
 
 :::
 
 :::warning
 
 This experiment breaks the following functionality:
 
 - \{list any existing functionality that will be broken by this experiment\}
 - \{if there are no breaking changes, remove this admonition\}
 
 :::
 
 :::info
 
-To enable this experiment, set the environment variable: `TASK_X_{feature}=1`. Check out [our guide to enabling experiments ][enabling-experiments] for more information.
+To enable this experiment, set the environment variable: `TASK_X_{feature}=1`.
+Check out [our guide to enabling experiments ][enabling-experiments] for more
+information.
 
 :::
 
 \{Short description of the feature\}
 
 \{Short explanation of how users should migrate to the new behavior\}
 
-<!-- prettier-ignore-start -->
-
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [enabling-experiments]: /experiments/#enabling-experiments
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/faq.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/faq.mdx`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,36 @@
 
 # FAQ
 
 This page contains a list of frequently asked questions about Task.
 
 ## Why won't my task update my shell environment?
 
-This is a limitation of how shells work. Task runs as a subprocess of your current shell, so it can't change the environment of the shell that started it. This limitation is shared by other task runners and build tools too.
-
-A common way to work around this is to create a task that will generate output that can be parsed by your shell. For example, to set an environment variable on your shell you can write a task like this:
+This is a limitation of how shells work. Task runs as a subprocess of your
+current shell, so it can't change the environment of the shell that started it.
+This limitation is shared by other task runners and build tools too.
+
+A common way to work around this is to create a task that will generate output
+that can be parsed by your shell. For example, to set an environment variable on
+your shell you can write a task like this:
 
 ```yaml
 my-shell-env:
   cmds:
     - echo "export FOO=foo"
     - echo "export BAR=bar"
 ```
 
-Now run `eval $(task my-shell-env)` and the variables `$FOO` and `$BAR` will be available in your shell.
+Now run `eval $(task my-shell-env)` and the variables `$FOO` and `$BAR` will be
+available in your shell.
 
 ## I can't reuse my shell in a task's commands
 
-Task runs each command as a separate shell process, so something you do in one command won't effect any future commands. For example, this won't work:
+Task runs each command as a separate shell process, so something you do in one
+command won't effect any future commands. For example, this won't work:
 
 ```yaml
 version: '3'
 
 tasks:
   foo:
     cmds:
@@ -47,43 +53,49 @@
     cmds:
       - |
         a=foo
         echo $a
       # outputs "foo"
 ```
 
-Or for more complex multi-line commands it is recommended to move your code into a separate file and call that instead:
+Or for more complex multi-line commands it is recommended to move your code into
+a separate file and call that instead:
 
 ```yaml
 version: '3'
 
 tasks:
   foo:
     cmds:
       - ./foo-printer.bash
 ```
 
-```bash
+```shell
 #!/bin/bash
 a=foo
 echo $a
 ```
 
 ## 'x' builtin command doesn't work on Windows
 
-The default shell on Windows (`cmd` and `powershell`) do not have commands like `rm` and `cp` available as builtins. This means that these commands won't work. If you want to make your Taskfile fully cross-platform, you'll need to work around this limitation using one of the following methods:
+The default shell on Windows (`cmd` and `powershell`) do not have commands like
+`rm` and `cp` available as builtins. This means that these commands won't work.
+If you want to make your Taskfile fully cross-platform, you'll need to work
+around this limitation using one of the following methods:
 
 - Use the `{{OS}}` function to run an OS-specific script.
-- Use something like `{{if eq OS "windows"}}powershell {{end}}<my_cmd>` to detect windows and run the command in Powershell directly.
-- Use a shell on Windows that supports these commands as builtins, such as [Git Bash][git-bash] or [WSL][wsl].
+- Use something like `{{if eq OS "windows"}}powershell {{end}}<my_cmd>` to
+  detect windows and run the command in Powershell directly.
+- Use a shell on Windows that supports these commands as builtins, such as [Git
+  Bash][git-bash] or [WSL][wsl].
 
-We want to make improvements to this part of Task and the issues below track this work. Constructive comments and contributions are very welcome!
+We want to make improvements to this part of Task and the issues below track
+this work. Constructive comments and contributions are very welcome!
 
 - #197
 - [mvdan/sh#93](https://github.com/mvdan/sh/issues/93)
 - [mvdan/sh#97](https://github.com/mvdan/sh/issues/97)
 
-<!-- prettier-ignore-start -->
-
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [git-bash]: https://gitforwindows.org/
 [wsl]: https://learn.microsoft.com/en-us/windows/wsl/install
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/installation.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/installation.mdx`

 * *Files 9% similar despite different names*

```diff
@@ -7,158 +7,192 @@
 
 Task offers many installation methods. Check out the available methods below.
 
 ## Package Managers
 
 ### Homebrew
 
-If you're on macOS or Linux and have [Homebrew][homebrew] installed, getting Task is as simple as running:
+If you're on macOS or Linux and have [Homebrew][homebrew] installed, getting
+Task is as simple as running:
 
-```bash
+```shell
 brew install go-task/tap/go-task
 ```
 
-The above Formula is [maintained by ourselves](https://github.com/go-task/homebrew-tap/blob/main/Formula/go-task.rb).
+The above Formula is
+[maintained by ourselves](https://github.com/go-task/homebrew-tap/blob/main/Formula/go-task.rb).
 
-Recently, Task was also made available [on the official Homebrew repository](https://formulae.brew.sh/formula/go-task), so you also have that option if you prefer:
+Recently, Task was also made available
+[on the official Homebrew repository](https://formulae.brew.sh/formula/go-task),
+so you also have that option if you prefer:
 
-```bash
+```shell
 brew install go-task
 ```
 
-### Tea
+### pkgx
 
-If you're on macOS or Linux and have [tea][tea] installed, getting Task is as simple as running:
+If you're on macOS or Linux and have [pkgx](https://pkgx.sh/) installed, getting Task is as
+simple as running:
 
-```bash
-tea task
+```shell
+pkgx task
 ```
 
-or, if you have tea’s magic enabled:
+or, if you have pkgx integration enabled:
 
-```bash
+```shell
 task
 ```
-This installation method is community owned. After a new release of Task, they are automatically released by tea in a minimum of time.
+
+This installation method is community owned. After a new release of Task, they
+are automatically released by pkgx in a minimum of time.
 
 ### Snap
 
-Task is available in [Snapcraft][snapcraft], but keep in mind that your Linux distribution should allow classic confinement for Snaps to Task work right:
+Task is available in [Snapcraft][snapcraft], but keep in mind that your Linux
+distribution should allow classic confinement for Snaps to Task work right:
 
-```bash
+```shell
 sudo snap install task --classic
 ```
 
 ### Chocolatey
 
-If you're on Windows and have [Chocolatey][choco] installed, getting Task is as simple as running:
+If you're on Windows and have [Chocolatey][choco] installed, getting Task is as
+simple as running:
 
-```bash
+```shell
 choco install go-task
 ```
 
 This installation method is community owned.
 
 ### Scoop
 
-If you're on Windows and have [Scoop][scoop] installed, getting Task is as simple as running:
+If you're on Windows and have [Scoop][scoop] installed, getting Task is as
+simple as running:
 
-```cmd
+```shell
 scoop install task
 ```
 
-This installation method is community owned. After a new release of Task, it may take some time until it's available on Scoop.
+This installation method is community owned. After a new release of Task, it may
+take some time until it's available on Scoop.
 
 ### AUR
 
-If you're on Arch Linux you can install Task from [AUR](https://aur.archlinux.org/packages/go-task-bin) using your favorite package manager such as `yay`, `pacaur` or `yaourt`:
+If you're on Arch Linux you can install Task from
+[AUR](https://aur.archlinux.org/packages/go-task-bin) using your favorite
+package manager such as `yay`, `pacaur` or `yaourt`:
 
-```cmd
+```shell
 yay -S go-task-bin
 ```
 
-Alternatively, there's [this package](https://aur.archlinux.org/packages/go-task) which installs from the source code instead of downloading the binary from the [releases page](https://github.com/go-task/task/releases):
+Alternatively, there's
+[this package](https://aur.archlinux.org/packages/go-task) which installs from
+the source code instead of downloading the binary from the
+[releases page](https://github.com/go-task/task/releases):
 
-```cmd
+```shell
 yay -S go-task
 ```
 
 This installation method is community owned.
 
 ### Fedora
 
-If you're on Fedora Linux you can install Task from the official [Fedora](https://packages.fedoraproject.org/pkgs/golang-github-task/go-task/) repository using `dnf`:
+If you're on Fedora Linux you can install Task from the official
+[Fedora](https://packages.fedoraproject.org/pkgs/golang-github-task/go-task/)
+repository using `dnf`:
 
-```cmd
+```shell
 sudo dnf install go-task
 ```
 
-This installation method is community owned. After a new release of Task, it may take some time until it's available in [Fedora](https://packages.fedoraproject.org/pkgs/golang-github-task/go-task/).
+This installation method is community owned. After a new release of Task, it may
+take some time until it's available in
+[Fedora](https://packages.fedoraproject.org/pkgs/golang-github-task/go-task/).
 
 ### Nix
 
-If you're on NixOS or have Nix installed you can install Task from [nixpkgs](https://github.com/NixOS/nixpkgs):
+If you're on NixOS or have Nix installed you can install Task from
+[nixpkgs](https://github.com/NixOS/nixpkgs):
 
-```cmd
+```shell
 nix-env -iA nixpkgs.go-task
 ```
 
-This installation method is community owned. After a new release of Task, it may take some time until it's available in [nixpkgs](https://github.com/NixOS/nixpkgs).
+This installation method is community owned. After a new release of Task, it may
+take some time until it's available in
+[nixpkgs](https://github.com/NixOS/nixpkgs).
 
 ### npm
 
-You can also use Node and npm to install Task by installing [this package](https://www.npmjs.com/package/@go-task/cli).
+You can also use Node and npm to install Task by installing
+[this package](https://www.npmjs.com/package/@go-task/cli).
 
-```bash
+```shell
 npm install -g @go-task/cli
 ```
 
 ### Winget
 
-If you are using Windows and installed the [winget](https://github.com/microsoft/winget-cli) package management tool, you can install Task from [winget-pkgs](https://github.com/microsoft/winget-pkgs).
+If you are using Windows and installed the
+[winget](https://github.com/microsoft/winget-cli) package management tool, you
+can install Task from [winget-pkgs](https://github.com/microsoft/winget-pkgs).
 
-```bash
+```shell
 winget install Task.Task
 ```
 
 ## Get The Binary
 
 ### Binary
 
-You can download the binary from the [releases page on GitHub][releases] and add to your `$PATH`.
+You can download the binary from the [releases page on GitHub][releases] and add
+to your `$PATH`.
 
 DEB and RPM packages are also available.
 
 The `task_checksums.txt` file contains the SHA-256 checksum for each file.
 
 ### Install Script
 
-We also have an [install script][installscript] which is very useful in scenarios like CI. Many thanks to [GoDownloader][godownloader] for enabling the easy generation of this script.
+We also have an [install script][installscript] which is very useful in
+scenarios like CI. Many thanks to [GoDownloader][godownloader] for enabling the
+easy generation of this script.
 
-By default, it installs on the `./bin` directory relative to the working directory:
+By default, it installs on the `./bin` directory relative to the working
+directory:
 
-```bash
+```shell
 sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d
 ```
 
-It is possible to override the installation directory with the `-b` parameter. On Linux, common choices are `~/.local/bin` and `~/bin` to install for the current user or `/usr/local/bin` to install for all users:
+It is possible to override the installation directory with the `-b` parameter.
+On Linux, common choices are `~/.local/bin` and `~/bin` to install for the
+current user or `/usr/local/bin` to install for all users:
 
-```bash
+```shell
 sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d -b ~/.local/bin
 ```
 
 :::caution
 
-On macOS and Windows, `~/.local/bin` and `~/bin` are not added to `$PATH` by default.
+On macOS and Windows, `~/.local/bin` and `~/bin` are not added to `$PATH` by
+default.
 
 :::
 
 ### GitHub Actions
 
-If you want to install Task in GitHub Actions you can try using [this action](https://github.com/arduino/setup-task) by the Arduino team:
+If you want to install Task in GitHub Actions you can try using
+[this action](https://github.com/arduino/setup-task) by the Arduino team:
 
 ```yaml
 - name: Install Task
   uses: arduino/setup-task@v1
   with:
     version: 3.x
     repo-token: ${{ secrets.GITHUB_TOKEN }}
@@ -166,31 +200,35 @@
 
 This installation method is community owned.
 
 ## Build From Source
 
 ### Go Modules
 
-Ensure that you have a supported version of [Go][go] properly installed and setup. You can find the minimum required version of Go in the [go.mod](https://github.com/go-task/task/blob/main/go.mod#L3) file.
+Ensure that you have a supported version of [Go][go] properly installed and
+setup. You can find the minimum required version of Go in the
+[go.mod](https://github.com/go-task/task/blob/main/go.mod#L3) file.
 
 You can then install the latest release globally by running:
 
-```bash
+```shell
 go install github.com/go-task/task/v3/cmd/task@latest
 ```
 
 Or you can install into another directory:
 
-```bash
+```shell
 env GOBIN=/bin go install github.com/go-task/task/v3/cmd/task@latest
 ```
 
 :::tip
 
-For CI environments we recommend using the [install script](#install-script) instead, which is faster and more stable, since it'll just download the latest released binary.
+For CI environments we recommend using the [install script](#install-script)
+instead, which is faster and more stable, since it'll just download the latest
+released binary.
 
 :::
 
 ## Setup completions
 
 Download the autocompletion file corresponding to your shell.
 
@@ -198,15 +236,15 @@
 
 ### Bash
 
 First, ensure that you installed bash-completion using your package manager.
 
 Make the completion file executable:
 
-```
+```shell
 chmod +x path/to/task.bash
 ```
 
 After, add this to your `~/.bash_profile`:
 
 ```shell
 source path/to/task.bash
@@ -237,30 +275,29 @@
 mv path/to/task.fish ~/.config/fish/completions/task.fish
 ```
 
 ### PowerShell
 
 Open your profile script with:
 
-```
+```powershell
 mkdir -Path (Split-Path -Parent $profile) -ErrorAction SilentlyContinue
 notepad $profile
 ```
 
 Add the line and save the file:
 
 ```shell
 Invoke-Expression -Command path/to/task.ps1
 ```
 
-<!-- prettier-ignore-start -->
-
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [go]: https://golang.org/
 [snapcraft]: https://snapcraft.io/task
 [homebrew]: https://brew.sh/
 [installscript]: https://github.com/go-task/task/blob/main/install-task.sh
 [releases]: https://github.com/go-task/task/releases
 [godownloader]: https://github.com/goreleaser/godownloader
 [choco]: https://chocolatey.org/
 [scoop]: https://scoop.sh/
 [tea]: https://tea.xyz/
+{/* prettier-ignore-end */}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/integrations.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/integrations.mdx`

 * *Files 13% similar despite different names*

```diff
@@ -3,60 +3,82 @@
 sidebar_position: 8
 ---
 
 # Integrations
 
 ## Visual Studio Code Extension
 
-Task has an [official extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=task.vscode-task). El código de ese proyecto puede ser encontrado [aquí](https://github.com/go-task/vscode-task). Para usar la extensión es necesario tener instalada la versión v3.23.0+ de Task.
+Task has an
+[official extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=task.vscode-task).
+The code for this project can be found
+[here](https://github.com/go-task/vscode-task). To use this extension, you must
+have Task v3.23.0+ installed on your system.
 
-La extensión proporciona las siguientes funcionalidades (y más...):
+This extension provides the following features (and more):
 
 - View tasks in the sidebar.
-- Ejecuta tareas desde la barra lateral y la paleta de comandos.
+- Run tasks from the sidebar and command palette.
 - Go to definition from the sidebar and command palette.
 - Run last task command.
 - Multi-root workspace support.
 - Initialize a Taskfile in the current workspace.
 
-To get autocompletion and validation for your Taskfile, see the [Schema](#schema) section below.
+To get autocompletion and validation for your Taskfile, see the
+[Schema](#schema) section below.
 
 ![Task for Visual Studio Code](https://github.com/go-task/vscode-task/blob/main/res/preview.png?raw=true)
 
 ## Schema
 
-This was initially created by @KROSF in [this Gist](https://gist.github.com/KROSF/c5435acf590acd632f71bb720f685895) and is now officially maintained in [this file](https://github.com/go-task/task/blob/main/docs/static/schema.json) and made available at https://taskfile.dev/schema.json. This schema can be used to validate Taskfiles and provide autocompletion in many code editors:
+This was initially created by @KROSF in
+[this Gist](https://gist.github.com/KROSF/c5435acf590acd632f71bb720f685895) and
+is now officially maintained in
+[this file](https://github.com/go-task/task/blob/main/website/static/schema.json)
+and made available at https://taskfile.dev/schema.json. This schema can be used
+to validate Taskfiles and provide autocompletion in many code editors:
 
 ### Visual Studio Code
 
-To integrate the schema into VS Code, you need to install the [YAML extension](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml) by Red Hat. Any `Taskfile.yml` in your project should automatically be detected and validation/autocompletion should work. If this doesn't work or you want to manually configure it for files with a different name, you can add the following to your `settings.json`:
+To integrate the schema into VS Code, you need to install the
+[YAML extension](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml)
+by Red Hat. Any `Taskfile.yml` in your project should automatically be detected
+and validation/autocompletion should work. If this doesn't work or you want to
+manually configure it for files with a different name, you can add the following
+to your `settings.json`:
 
 ```json
 // settings.json
 {
   "yaml.schemas": {
     "https://taskfile.dev/schema.json": [
       "**/Taskfile.yml",
       "./path/to/any/other/taskfile.yml"
     ]
   }
 }
 ```
 
-You can also configure the schema directly inside of a Taskfile by adding the following comment to the top of the file:
+You can also configure the schema directly inside of a Taskfile by adding the
+following comment to the top of the file:
 
 ```yaml
 # yaml-language-server: $schema=https://taskfile.dev/schema.json
 version: '3'
 ```
 
-You can find more information on this in the [YAML language server project](https://github.com/redhat-developer/yaml-language-server).
+You can find more information on this in the
+[YAML language server project](https://github.com/redhat-developer/yaml-language-server).
 
 ## Community Integrations
 
-In addition to our official integrations, there is an amazing community of developers who have created their own integrations for Task:
+In addition to our official integrations, there is an amazing community of
+developers who have created their own integrations for Task:
 
-- [Sublime Text Plugin](https://packagecontrol.io/packages/Taskfile) [[source](https://github.com/biozz/sublime-taskfile)] by @biozz
-- [IntelliJ Plugin](https://plugins.jetbrains.com/plugin/17058-taskfile) [[source](https://github.com/lechuckroh/task-intellij-plugin)] by @lechuckroh
-- [mk](https://github.com/pycontribs/mk) command line tool recognizes Taskfiles natively.
+- [Sublime Text Plugin](https://packagecontrol.io/packages/Taskfile)
+  [[source](https://github.com/biozz/sublime-taskfile)] by @biozz
+- [IntelliJ Plugin](https://plugins.jetbrains.com/plugin/17058-taskfile)
+  [[source](https://github.com/lechuckroh/task-intellij-plugin)] by @lechuckroh
+- [mk](https://github.com/pycontribs/mk) command line tool recognizes Taskfiles
+  natively.
 
-If you have made something that integrates with Task, please feel free to open a PR to add it to this list.
+If you have made something that integrates with Task, please feel free to open a
+PR to add it to this list.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/intro.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/intro.mdx`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 ---
 slug: /
 sidebar_position: 1
 title: Home
+hide_title: true
 ---
 
-# Task
-
 <div align="center">
-  <img id="logo" src="img/logo.svg" height="250px" width="250px" />
+  <img id="logo" src="/img/logo.svg" height="250px" width="250px" />
 </div>
+<br />
 
-Task is a task runner / build tool that aims to be simpler and easier to use than, for example, [GNU Make][make].
+Task is a task runner / build tool that aims to be simpler and easier to use
+than, for example, [GNU Make][make].
 
-Since it's written in [Go][go], Task is just a single binary and has no other dependencies, which means you don't need to mess with any complicated install setups just to use a build tool.
+Since it's written in [Go][go], Task is just a single binary and has no other
+dependencies, which means you don't need to mess with any complicated install
+setups just to use a build tool.
 
-Once [installed](/installation), you just need to describe your build tasks using a simple [YAML][yaml] schema in a file called `Taskfile.yml`:
+Once [installed](/installation), you just need to describe your build tasks
+using a simple [YAML][yaml] schema in a file called `Taskfile.yml`:
 
 ```yaml title="Taskfile.yml"
 version: '3'
 
 tasks:
   hello:
     cmds:
       - echo 'Hello World from Task!'
     silent: true
 ```
 
 And call it by running `task hello` from your terminal.
 
-The above example is just the start, you can take a look at the [usage](/usage) guide to check the full schema documentation and Task features.
+The above example is just the start, you can take a look at the [usage](/usage)
+guide to check the full schema documentation and Task features.
 
 ## Features
 
-- [Easy installation](/installation): just download a single binary, add to `$PATH` and you're done! Or you can also install using [Homebrew][homebrew], [Snapcraft][snapcraft], or [Scoop][scoop] if you want.
-- Available on CIs: by adding [this simple command](/installation#install-script) to install on your CI script and you're ready to use Task as part of your CI pipeline;
-- Truly cross-platform: while most build tools only work well on Linux or macOS, Task also supports Windows thanks to [this shell interpreter for Go][sh].
-- Great for code generation: you can easily [prevent a task from running](/usage#prevent-unnecessary-work) if a given set of files haven't changed since last run (based either on its timestamp or content).
-
-<!-- prettier-ignore-start -->
+- [Easy installation](/installation): just download a single binary, add to
+  `$PATH` and you're done! Or you can also install using [Homebrew][homebrew],
+  [Snapcraft][snapcraft], or [Scoop][scoop] if you want.
+- Available on CIs: by adding
+  [this simple command](/installation#install-script) to install on your CI
+  script and you're ready to use Task as part of your CI pipeline;
+- Truly cross-platform: while most build tools only work well on Linux or macOS,
+  Task also supports Windows thanks to [this shell interpreter for Go][sh].
+- Great for code generation: you can easily
+  [prevent a task from running](/usage#prevent-unnecessary-work) if a given set
+  of files haven't changed since last run (based either on its timestamp or
+  content).
 
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [make]: https://www.gnu.org/software/make/
 [go]: https://go.dev/
 [yaml]: http://yaml.org/
 [homebrew]: https://brew.sh/
 [snapcraft]: https://snapcraft.io/
 [scoop]: https://scoop.sh/
 [sh]: https://github.com/mvdan/sh
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/releasing.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/releasing.mdx`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,72 @@
 ---
 slug: /releasing/
 sidebar_position: 13
 ---
 
 # Releasing
 
-The release process of Task is done with the help of [GoReleaser][goreleaser]. You can test the release process locally by calling the `test-release` task of the Taskfile.
-
-[GitHub Actions](https://github.com/go-task/task/actions) should release artifacts automatically when a new Git tag is pushed to `main` branch (raw executables and DEB and RPM packages).
-
-Since v3.15.0, raw executables can also be reproduced and verified locally by checking out a specific tag and calling `goreleaser build`, using the Go version defined in the above GitHub Actions.
+The release process of Task is done with the help of [GoReleaser][goreleaser].
+You can test the release process locally by calling the `test-release` task of
+the Taskfile.
+
+[GitHub Actions](https://github.com/go-task/task/actions) should release
+artifacts automatically when a new Git tag is pushed to `main` branch (raw
+executables and DEB and RPM packages).
+
+Since v3.15.0, raw executables can also be reproduced and verified locally by
+checking out a specific tag and calling `goreleaser build`, using the Go version
+defined in the above GitHub Actions.
 
 # Homebrew
 
-Goreleaser will automatically push a new commit to the [Formula/go-task.rb][gotaskrb] file in the [Homebrew tap][homebrewtap] repository to release the new version.
+Goreleaser will automatically push a new commit to the
+[Formula/go-task.rb][gotaskrb] file in the [Homebrew tap][homebrewtap]
+repository to release the new version.
 
 # npm
 
-To release to npm update the version in the [`package.json`][packagejson] file and then run `task npm:publish` to push it.
+To release to npm update the version in the [`package.json`][packagejson] file
+and then run `task npm:publish` to push it.
 
 # Snapcraft
 
-The [snap package][snappackage] requires to manual steps to release a new version:
+The [snap package][snappackage] requires to manual steps to release a new
+version:
 
 - Updating the current version on [snapcraft.yaml][snapcraftyaml].
-- Moving both `amd64`, `armhf` and `arm64` new artifacts to the stable channel on the [Snapcraft dashboard][snapcraftdashboard].
+- Moving both `amd64`, `armhf` and `arm64` new artifacts to the stable channel
+  on the [Snapcraft dashboard][snapcraftdashboard].
 
 # winget
 
-winget also requires manual steps to be completed. By running `task goreleaser:test` locally, manifest files will be generated on `dist/winget/manifests/t/Task/Task/v{version}`. [Upload the manifest directory into this fork](https://github.com/go-task/winget-pkgs/tree/master/manifests/t/Task/Task) and open a pull request into [this repository](https://github.com/microsoft/winget-pkgs).
+winget also requires manual steps to be completed. By running
+`task goreleaser:test` locally, manifest files will be generated on
+`dist/winget/manifests/t/Task/Task/v{version}`.
+[Upload the manifest directory into this fork](https://github.com/go-task/winget-pkgs/tree/master/manifests/t/Task/Task)
+and open a pull request into
+[this repository](https://github.com/microsoft/winget-pkgs).
 
 # Scoop
 
-Scoop is a command-line package manager for the Windows operating system. Scoop package manifests are maintained by the community. Scoop owners usually take care of updating versions there by editing [this file](https://github.com/ScoopInstaller/Main/blob/master/bucket/task.json). If you think its Task version is outdated, open an issue to let us know.
+Scoop is a command-line package manager for the Windows operating system. Scoop
+package manifests are maintained by the community. Scoop owners usually take
+care of updating versions there by editing
+[this file](https://github.com/ScoopInstaller/Main/blob/master/bucket/task.json).
+If you think its Task version is outdated, open an issue to let us know.
 
 # Nix
 
-Nix is a community owned installation method. Nix package maintainers usually take care of updating versions there by editing [this file](https://github.com/NixOS/nixpkgs/blob/nixos-unstable/pkgs/development/tools/go-task/default.nix). If you think its Task version is outdated, open an issue to let us know.
-
-<!-- prettier-ignore-start -->
+Nix is a community owned installation method. Nix package maintainers usually
+take care of updating versions there by editing
+[this file](https://github.com/NixOS/nixpkgs/blob/nixos-unstable/pkgs/development/tools/go-task/default.nix).
+If you think its Task version is outdated, open an issue to let us know.
 
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [goreleaser]: https://goreleaser.com/
 [homebrewtap]: https://github.com/go-task/homebrew-tap
 [gotaskrb]: https://github.com/go-task/homebrew-tap/blob/main/Formula/go-task.rb
 [packagejson]: https://github.com/go-task/task/blob/main/package.json#L3
 [snappackage]: https://github.com/go-task/snap
 [snapcraftyaml]: https://github.com/go-task/snap/blob/main/snap/snapcraft.yaml#L2
 [snapcraftdashboard]: https://snapcraft.io/task/releases
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/styleguide.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/styleguide.mdx`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 ---
 slug: /styleguide/
 sidebar_position: 10
 ---
 
-# Styleguide
+# Style guide
 
-This is the official Task styleguide for `Taskfile.yml` files. This guide contains some basic instructions to keep your Taskfile clean and familiar to other users.
+This is the official style guide for `Taskfile.yml` files. It provides basic
+instructions for keeping your Taskfiles clean and familiar to other users.
 
-This contains general guidelines, but they don't necessarily need to be strictly followed. Feel free to disagree and proceed differently at some point if you need or want to. Also, feel free to open issues or pull requests with improvements to this guide.
+This guide contains general guidelines, but they do not necessarily need to be
+followed strictly. Feel free to disagree and do things differently if you need
+or want to. Any improvements to this guide are welcome! Please open an issue or
+create a pull request to contribute.
 
-## Use the correct order of keywords
+## Use the suggested ordering of the main sections
 
-- `version:`
-- `includes:`
-- Configuration ones, like `output:`, `silent:`, `method:` and `run:`
-- `vars:`
-- `env:`, `dotenv:`
-- `tasks:`
+```yaml
+version:
+includes:
+# optional configurations (output, silent, method, run, etc.)
+vars:
+env: # followed or replaced by dotenv
+tasks:
+```
 
-## Use 2 spaces for indentation
+## Use two spaces for indentation
 
 This is the most common convention for YAML files, and Task follows it.
 
 ```yaml
 # bad
 tasks:
     foo:
@@ -33,15 +39,15 @@
 # good
 tasks:
   foo:
     cmds:
       - echo 'foo'
 ```
 
-## Separate with spaces the mains sections
+## Separate the main sections with empty lines
 
 ```yaml
 # bad
 version: '3'
 includes:
   docker: ./docker/Taskfile.yml
 output: prefixed
@@ -67,15 +73,15 @@
 env:
   BAR: baz
 
 tasks:
   # ...
 ```
 
-## Add spaces between tasks
+## Separate tasks with empty lines
 
 ```yaml
 # bad
 version: '3'
 
 tasks:
   foo:
@@ -102,15 +108,15 @@
       - echo 'bar'
 
   baz:
     cmds:
       - echo 'baz'
 ```
 
-## Use upper-case variable names
+## Use only uppercase letters for variable names
 
 ```yaml
 # bad
 version: '3'
 
 vars:
   binary_name: myapp
@@ -129,15 +135,15 @@
 
 tasks:
   build:
     cmds:
       - go build -o {{.BINARY_NAME}} .
 ```
 
-## Don't wrap vars in spaces when templating
+## Avoid using whitespace when templating variables
 
 ```yaml
 # bad
 version: '3'
 
 tasks:
   greet:
@@ -150,17 +156,18 @@
 
 tasks:
   greet:
     cmds:
       - echo '{{.MESSAGE}}'
 ```
 
-This convention is also used by most people for any Go templating.
+This convention is also commonly used in templates for the Go programming
+language.
 
-## Separate task name words with a dash
+## Use kebab case for task names
 
 ```yaml
 # bad
 version: '3'
 
 tasks:
   do_something_fancy:
@@ -173,15 +180,15 @@
 
 tasks:
   do-something-fancy:
     cmds:
       - echo 'Do something'
 ```
 
-## Use colon for task namespacing
+## Use a colon to separate the task namespace and name
 
 ```yaml
 # good
 version: '3'
 
 tasks:
   docker:build:
@@ -191,15 +198,15 @@
   docker:run:
     cmds:
       - docker-compose ...
 ```
 
 This is also done automatically when using included Taskfiles.
 
-## Prefer external scripts over complex multi-line commands
+## Prefer using external scripts instead of multi-line commands
 
 ```yaml
 # bad
 version: '3'
 
 tasks:
   build:
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/taskfile_versions.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/taskfile_versions.mdx`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 ---
 slug: /taskfile-versions/
 sidebar_position: 5
 ---
 
 # Taskfile Versions
 
-The Taskfile syntax and features changed with time. This document explains what changed on each version and how to upgrade your Taskfile.
+The Taskfile syntax and features changed with time. This document explains what
+changed on each version and how to upgrade your Taskfile.
 
 ## What the Taskfile version mean
 
-The Taskfile version follows the Task version. E.g. the change to Taskfile version `2` means that Task `v2.0.0` should be release to support it.
+The Taskfile version follows the Task version. E.g. the change to Taskfile
+version `2` means that Task `v2.0.0` should be release to support it.
 
-The `version:` key on Taskfile accepts a semver string, so either `2`, `2.0` or `2.0.0` is accepted. If you choose to use `2.0` Task will not enable future `2.1` features, but if you choose to use `2`, then any `2.x.x` features will be available, but not `3.0.0+`.
+The `version:` key on Taskfile accepts a semver string, so either `2`, `2.0` or
+`2.0.0` is accepted. If you choose to use `2.0` Task will not enable future
+`2.1` features, but if you choose to use `2`, then any `2.x.x` features will be
+available, but not `3.0.0+`.
 
 ## Version 3 ![latest](https://img.shields.io/badge/latest-brightgreen)
 
 These are some major changes done on `v3`:
 
 - Task's output will now be colored
 - Added support for `.env` like files
-- Added `label:` setting to task so one can override how the task name appear in the logs
-- A global `method:` was added to allow setting the default method, and Task's default changed to `checksum`
-- Two magic variables were added when using `status:`: `CHECKSUM` and `TIMESTAMP` which contains, respectively, the XXH3 checksum and greatest modification timestamp of the files listed on `sources:`
+- Added `label:` setting to task so one can override how the task name appear in
+  the logs
+- A global `method:` was added to allow setting the default method, and Task's
+  default changed to `checksum`
+- Two magic variables were added when using `status:`: `CHECKSUM` and
+  `TIMESTAMP` which contains, respectively, the XXH3 checksum and greatest
+  modification timestamp of the files listed on `sources:`
 - Also, the `TASK` variable is always available with the current task name
 - CLI variables are always treated as global variables
-- Added `dir:` option to `includes` to allow choosing on which directory an included Taskfile will run:
+- Added `dir:` option to `includes` to allow choosing on which directory an
+  included Taskfile will run:
 
 ```yaml
 includes:
   docs:
     taskfile: ./docs
     dir: ./docs
 ```
@@ -55,25 +65,29 @@
 ```yaml
 version: '3'
 
 tasks:
   print: echo "Hello, World!"
 ```
 
-- There was a major refactor on how variables are handled. They're now easier to understand. The `expansions:` setting was removed as it became unnecessary. This is the order in which Task will process variables, each level can see the variables set by the previous one and override those.
+- There was a major refactor on how variables are handled. They're now easier to
+  understand. The `expansions:` setting was removed as it became unnecessary.
+  This is the order in which Task will process variables, each level can see the
+  variables set by the previous one and override those.
   - Environment variables
   - Global + CLI variables
   - Call variables
   - Task variables
 
 ## Version 2.6
 
 :::caution
 
-v2 schemas are [no longer supported by the latest version of Task][deprecate-version-2-schema].
+v2 schemas are [no longer supported by the latest version of
+Task][deprecate-version-2-schema].
 
 :::
 
 Version 2.6 comes with `preconditions` stanza in tasks.
 
 ```yaml
 version: '2'
@@ -88,15 +102,16 @@
 
 Please check the [documentation][includes]
 
 ## Version 2.2
 
 :::caution
 
-v2 schemas are [no longer supported by the latest version of Task][deprecate-version-2-schema].
+v2 schemas are [no longer supported by the latest version of
+Task][deprecate-version-2-schema].
 
 :::
 
 Version 2.2 comes with a global `includes` options to include other Taskfiles:
 
 ```yaml
 version: '2'
@@ -106,33 +121,37 @@
   docker: ./DockerTasks.yml
 ```
 
 ## Version 2.1
 
 :::caution
 
-v2 schemas are [no longer supported by the latest version of Task][deprecate-version-2-schema].
+v2 schemas are [no longer supported by the latest version of
+Task][deprecate-version-2-schema].
 
 :::
 
-Version 2.1 includes a global `output` option, to allow having more control over how commands output are printed to the console (see [documentation][output] for more info):
+Version 2.1 includes a global `output` option, to allow having more control over
+how commands output are printed to the console (see [documentation][output] for
+more info):
 
 ```yaml
 version: '2'
 
 output: prefixed
 
 tasks:
   server:
     cmds:
       - go run main.go
   prefix: server
 ```
 
-From this version it's also possible to ignore errors of a command or task (check documentation [here][ignore_errors]):
+From this version it's also possible to ignore errors of a command or task
+(check documentation [here][ignore_errors]):
 
 ```yaml
 version: '2'
 
 tasks:
   example-1:
     cmds:
@@ -147,30 +166,33 @@
     ignore_error: true
 ```
 
 ## Version 2.0
 
 :::caution
 
-v2 schemas are [no longer supported by the latest version of Task][deprecate-version-2-schema].
+v2 schemas are [no longer supported by the latest version of
+Task][deprecate-version-2-schema].
 
 :::
 
-At version 2, we introduced the `version:` key, to allow us to evolve Task with new features without breaking existing Taskfiles. The new syntax is as follows:
+At version 2, we introduced the `version:` key, to allow us to evolve Task with
+new features without breaking existing Taskfiles. The new syntax is as follows:
 
 ```yaml
 version: '2'
 
 tasks:
   echo:
     cmds:
       - echo "Hello, World!"
 ```
 
-Version 2 allows you to write global variables directly in the Taskfile, if you don't want to create a `Taskvars.yml`:
+Version 2 allows you to write global variables directly in the Taskfile, if you
+don't want to create a `Taskvars.yml`:
 
 ```yaml
 version: '2'
 
 vars:
   GREETING: Hello, World!
 
@@ -184,15 +206,16 @@
 
 1. Task variables
 2. Call variables
 3. Taskfile variables
 4. Taskvars file variables
 5. Environment variables
 
-A new global option was added to configure the number of variables expansions (which default to 2):
+A new global option was added to configure the number of variables expansions
+(which default to 2):
 
 ```yaml
 version: '2'
 
 expansions: 3
 
 vars:
@@ -212,29 +235,29 @@
 
 :::caution
 
 v1 schema support was removed in Task >= v3.0.0.
 
 :::
 
-In the first version of the `Taskfile`, the `version:` key was not available, because the tasks was in the root of the YAML document. Like this:
+In the first version of the `Taskfile`, the `version:` key was not available,
+because the tasks was in the root of the YAML document. Like this:
 
 ```yaml
 echo:
   cmds:
     - echo "Hello, World!"
 ```
 
 The variable priority order was also different:
 
 1. Call variables
 2. Environment
 3. Task variables
 4. `Taskvars.yml` variables
 
-<!-- prettier-ignore-start -->
-
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [deprecate-version-2-schema]: /deprecations/version-2-schema/
 [output]: /usage#output-syntax
 [ignore_errors]: /usage#ignore-errors
 [includes]: /usage#including-other-taskfiles
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/translate.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/translate.mdx`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 sidebar_position: 12
 ---
 
 # Translate
 
 Want to help us translate this documentation? In this document we explain how.
 
-Do NOT edit translated markdown files directly on the GitHub repository! We use [Crowdin][crowdin] to allow contributors on work on translations. The repository is periodically updated with progress from Crowdin.
+Do NOT edit translated markdown files directly on the GitHub repository! We use
+[Crowdin][crowdin] to allow contributors on work on translations. The repository
+is periodically updated with progress from Crowdin.
+
+If you want to have access to the Crowdin project to be able to suggest
+translations, please ask for access on the [#translations channel on our Discord
+server][discord]. If a given language is not being shown to Crowdin yet, just
+ask and we can configure it.
 
-If you want to have access to the Crowdin project to be able to suggest translations, please ask for access on the [#translations channel on our Discord server][discord]. If a given language is not being shown to Crowdin yet, just ask and we can configure it.
-
-<!-- prettier-ignore-start -->
-
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [crowdin]: https://crowdin.com/project/taskfile
 [discord]: https://discord.gg/6TY36E39UK
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/i18n/es-ES/docusaurus-plugin-content-docs/current/usage.md` & `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/usage.mdx`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 sidebar_position: 3
 ---
 
 # Usage
 
 ## Getting started
 
-Create a file called `Taskfile.yml` in the root of your project. The `cmds` attribute should contain the commands of a task. The example below allows compiling a Go app and uses [esbuild](https://esbuild.github.io/) to concat and minify multiple CSS files into a single one.
+Create a file called `Taskfile.yml` in the root of your project. The `cmds`
+attribute should contain the commands of a task. The example below allows
+compiling a Go app and uses [esbuild](https://esbuild.github.io/) to concat and
+minify multiple CSS files into a single one.
 
 ```yaml
 version: '3'
 
 tasks:
   build:
     cmds:
@@ -20,19 +23,22 @@
   assets:
     cmds:
       - esbuild --bundle --minify css/index.css > public/bundle.css
 ```
 
 Running the tasks is as simple as running:
 
-```bash
+```shell
 task assets build
 ```
 
-Task uses [mvdan.cc/sh](https://mvdan.cc/sh/), a native Go sh interpreter. So you can write sh/bash commands, and it will work even on Windows, where `sh` or `bash` are usually not available. Just remember any executable called must be available by the OS or in PATH.
+Task uses [mvdan.cc/sh](https://mvdan.cc/sh/), a native Go sh interpreter. So
+you can write sh/bash commands, and it will work even on Windows, where `sh` or
+`bash` are usually not available. Just remember any executable called must be
+available by the OS or in PATH.
 
 If you omit a task name, "default" will be assumed.
 
 ## Supported file names
 
 Task will look for the following file names, in order of priority:
 
@@ -41,47 +47,64 @@
 - Taskfile.yaml
 - taskfile.yaml
 - Taskfile.dist.yml
 - taskfile.dist.yml
 - Taskfile.dist.yaml
 - taskfile.dist.yaml
 
-The intention of having the `.dist` variants is to allow projects to have one committed version (`.dist`) while still allowing individual users to override the Taskfile by adding an additional `Taskfile.yml` (which would be on `.gitignore`).
+The intention of having the `.dist` variants is to allow projects to have one
+committed version (`.dist`) while still allowing individual users to override
+the Taskfile by adding an additional `Taskfile.yml` (which would be on
+`.gitignore`).
 
 ### Running a Taskfile from a subdirectory
 
-If a Taskfile cannot be found in the current working directory, it will walk up the file tree until it finds one (similar to how `git` works). When running Task from a subdirectory like this, it will behave as if you ran it from the directory containing the Taskfile.
-
-You can use this functionality along with the special `{{.USER_WORKING_DIR}}` variable to create some very useful reusable tasks. For example, if you have a monorepo with directories for each microservice, you can `cd` into a microservice directory and run a task command to bring it up without having to create multiple tasks or Taskfiles with identical content. For example:
+If a Taskfile cannot be found in the current working directory, it will walk up
+the file tree until it finds one (similar to how `git` works). When running Task
+from a subdirectory like this, it will behave as if you ran it from the
+directory containing the Taskfile.
+
+You can use this functionality along with the special `{{.USER_WORKING_DIR}}`
+variable to create some very useful reusable tasks. For example, if you have a
+monorepo with directories for each microservice, you can `cd` into a
+microservice directory and run a task command to bring it up without having to
+create multiple tasks or Taskfiles with identical content. For example:
 
 ```yaml
 version: '3'
 
 tasks:
   up:
     dir: '{{.USER_WORKING_DIR}}'
     preconditions:
       - test -f docker-compose.yml
     cmds:
       - docker-compose up -d
 ```
 
-In this example, we can run `cd <service>` and `task up` and as long as the `<service>` directory contains a `docker-compose.yml`, the Docker composition will be brought up.
+In this example, we can run `cd <service>` and `task up` and as long as the
+`<service>` directory contains a `docker-compose.yml`, the Docker composition
+will be brought up.
 
 ### Running a global Taskfile
 
-If you call Task with the `--global` (alias `-g`) flag, it will look for your home directory instead of your working directory. In short, Task will look for a Taskfile that matches `$HOME/{T,t}askfile.{yml,yaml}` .
+If you call Task with the `--global` (alias `-g`) flag, it will look for your
+home directory instead of your working directory. In short, Task will look for a
+Taskfile that matches `$HOME/{T,t}askfile.{yml,yaml}` .
 
 This is useful to have automation that you can run from anywhere in your system!
 
 :::info
 
-When running your global Taskfile with `-g`, tasks will run on `$HOME` by default, and not on your working directory!
+When running your global Taskfile with `-g`, tasks will run on `$HOME` by
+default, and not on your working directory!
 
-As mentioned in the previous section, the `{{.USER_WORKING_DIR}}` special variable can be very handy here to run stuff on the directory you're calling `task -g` from.
+As mentioned in the previous section, the `{{.USER_WORKING_DIR}}` special
+variable can be very handy here to run stuff on the directory you're calling
+`task -g` from.
 
 ```yaml
 version: '3'
 
 tasks:
   from-home:
     cmds:
@@ -91,14 +114,26 @@
     dir: '{{.USER_WORKING_DIR}}'
     cmds:
       - pwd
 ```
 
 :::
 
+### Reading a Taskfile from stdin
+
+Taskfile also supports reading from stdin. This is useful if you are generating
+Taskfiles dynamically and don't want write them to disk. This works just like
+any other program that supports stdin. For example:
+
+```shell
+task < <(cat ./Taskfile.yml)
+# OR
+cat ./Taskfile.yml | task
+```
+
 ## Environment variables
 
 ### Task
 
 You can use `env` to set custom environment variables for a specific task:
 
 ```yaml
@@ -108,15 +143,16 @@
   greet:
     cmds:
       - echo $GREETING
     env:
       GREETING: Hey, there!
 ```
 
-Additionally, you can set global environment variables that will be available to all tasks:
+Additionally, you can set global environment variables that will be available to
+all tasks:
 
 ```yaml
 version: '3'
 
 env:
   GREETING: Hey, there!
 
@@ -124,27 +160,29 @@
   greet:
     cmds:
       - echo $GREETING
 ```
 
 :::info
 
-`env` supports expansion and retrieving output from a shell command just like variables, as you can see in the [Variables](#variables) section.
+`env` supports expansion and retrieving output from a shell command just like
+variables, as you can see in the [Variables](#variables) section.
 
 :::
 
 ### .env files
 
-You can also ask Task to include `.env` like files by using the `dotenv:` setting:
+You can also ask Task to include `.env` like files by using the `dotenv:`
+setting:
 
-```bash title=".env"
+```shell title=".env"
 KEYNAME=VALUE
 ```
 
-```bash title="testing/.env"
+```shell title="testing/.env"
 ENDPOINT=testing.com
 ```
 
 ```yaml title="Taskfile.yml"
 version: '3'
 
 env:
@@ -169,15 +207,16 @@
 tasks:
   greet:
     dotenv: ['.env', '{{.ENV}}/.env.', '{{.HOME}}/.env']
     cmds:
       - echo "Using $KEYNAME and endpoint $ENDPOINT"
 ```
 
-Environment variables specified explicitly at the task-level will override variables defined in dotfiles:
+Environment variables specified explicitly at the task-level will override
+variables defined in dotfiles:
 
 ```yaml
 version: '3'
 
 env:
   ENV: testing
 
@@ -188,67 +227,81 @@
       KEYNAME: DIFFERENT_VALUE
     cmds:
       - echo "Using $KEYNAME and endpoint $ENDPOINT"
 ```
 
 :::info
 
-Please note that you are not currently able to use the `dotenv` key inside included Taskfiles.
+Please note that you are not currently able to use the `dotenv` key inside
+included Taskfiles.
 
 :::
 
 ## Including other Taskfiles
 
-If you want to share tasks between different projects (Taskfiles), you can use the importing mechanism to include other Taskfiles using the `includes` keyword:
+If you want to share tasks between different projects (Taskfiles), you can use
+the importing mechanism to include other Taskfiles using the `includes` keyword:
 
 ```yaml
 version: '3'
 
 includes:
   docs: ./documentation # will look for ./documentation/Taskfile.yml
   docker: ./DockerTasks.yml
 ```
 
-The tasks described in the given Taskfiles will be available with the informed namespace. So, you'd call `task docs:serve` to run the `serve` task from `documentation/Taskfile.yml` or `task docker:build` to run the `build` task from the `DockerTasks.yml` file.
+The tasks described in the given Taskfiles will be available with the informed
+namespace. So, you'd call `task docs:serve` to run the `serve` task from
+`documentation/Taskfile.yml` or `task docker:build` to run the `build` task from
+the `DockerTasks.yml` file.
 
-Relative paths are resolved relative to the directory containing the including Taskfile.
+Relative paths are resolved relative to the directory containing the including
+Taskfile.
 
 ### OS-specific Taskfiles
 
-With `version: '2'`, task automatically includes any `Taskfile_{{OS}}.yml` if it exists (for example: `Taskfile_windows.yml`, `Taskfile_linux.yml` or `Taskfile_darwin.yml`). Since this behavior was a bit too implicit, it was removed on version 3, but you still can have a similar behavior by explicitly importing these files:
+With `version: '2'`, task automatically includes any `Taskfile_{{OS}}.yml` if it
+exists (for example: `Taskfile_windows.yml`, `Taskfile_linux.yml` or
+`Taskfile_darwin.yml`). Since this behavior was a bit too implicit, it was
+removed on version 3, but you still can have a similar behavior by explicitly
+importing these files:
 
 ```yaml
 version: '3'
 
 includes:
   build: ./Taskfile_{{OS}}.yml
 ```
 
 ### Directory of included Taskfile
 
-By default, included Taskfile's tasks are run in the current directory, even if the Taskfile is in another directory, but you can force its tasks to run in another directory by using this alternative syntax:
+By default, included Taskfile's tasks are run in the current directory, even if
+the Taskfile is in another directory, but you can force its tasks to run in
+another directory by using this alternative syntax:
 
 ```yaml
 version: '3'
 
 includes:
   docs:
     taskfile: ./docs/Taskfile.yml
     dir: ./docs
 ```
 
 :::info
 
-The included Taskfiles must be using the same schema version as the main Taskfile uses.
+The included Taskfiles must be using the same schema version as the main
+Taskfile uses.
 
 :::
 
 ### Optional includes
 
-Includes marked as optional will allow Task to continue execution as normal if the included file is missing.
+Includes marked as optional will allow Task to continue execution as normal if
+the included file is missing.
 
 ```yaml
 version: '3'
 
 includes:
   tests:
     taskfile: ./tests/Taskfile.yml
@@ -259,28 +312,32 @@
     cmds:
       - echo "This command can still be successfully executed if
         ./tests/Taskfile.yml does not exist"
 ```
 
 ### Internal includes
 
-Includes marked as internal will set all the tasks of the included file to be internal as well (see the [Internal tasks](#internal-tasks) section below). This is useful when including utility tasks that are not intended to be used directly by the user.
+Includes marked as internal will set all the tasks of the included file to be
+internal as well (see the [Internal tasks](#internal-tasks) section below). This
+is useful when including utility tasks that are not intended to be used directly
+by the user.
 
 ```yaml
 version: '3'
 
 includes:
   tests:
     taskfile: ./taskfiles/Utils.yml
     internal: true
 ```
 
 ### Vars of included Taskfiles
 
-You can also specify variables when including a Taskfile. This may be useful for having reusable Taskfile that can be tweaked or even included more than once:
+You can also specify variables when including a Taskfile. This may be useful for
+having reusable Taskfile that can be tweaked or even included more than once:
 
 ```yaml
 version: '3'
 
 includes:
   backend:
     taskfile: ./taskfiles/Docker.yml
@@ -291,34 +348,43 @@
     taskfile: ./taskfiles/Docker.yml
     vars:
       DOCKER_IMAGE: frontend_image
 ```
 
 ### Namespace aliases
 
-When including a Taskfile, you can give the namespace a list of `aliases`. This works in the same way as [task aliases](#task-aliases) and can be used together to create shorter and easier-to-type commands.
+When including a Taskfile, you can give the namespace a list of `aliases`. This
+works in the same way as [task aliases](#task-aliases) and can be used together
+to create shorter and easier-to-type commands.
 
 ```yaml
 version: '3'
 
 includes:
   generate:
     taskfile: ./taskfiles/Generate.yml
     aliases: [gen]
 ```
 
 :::info
 
-Vars declared in the included Taskfile have preference over the variables in the including Taskfile! If you want a variable in an included Taskfile to be overridable, use the [default function](https://go-task.github.io/slim-sprig/defaults.html): `MY_VAR: '{{.MY_VAR | default "my-default-value"}}'`.
+Vars declared in the included Taskfile have preference over the variables in the
+including Taskfile! If you want a variable in an included Taskfile to be
+overridable, use the
+[default function](https://go-task.github.io/slim-sprig/defaults.html):
+`MY_VAR: '{{.MY_VAR | default "my-default-value"}}'`.
 
 :::
 
 ## Internal tasks
 
-Internal tasks are tasks that cannot be called directly by the user. They will not appear in the output when running `task --list|--list-all`. Other tasks may call internal tasks in the usual way. This is useful for creating reusable, function-like tasks that have no useful purpose on the command line.
+Internal tasks are tasks that cannot be called directly by the user. They will
+not appear in the output when running `task --list|--list-all`. Other tasks may
+call internal tasks in the usual way. This is useful for creating reusable,
+function-like tasks that have no useful purpose on the command line.
 
 ```yaml
 version: '3'
 
 tasks:
   build-image-1:
     cmds:
@@ -330,15 +396,17 @@
     internal: true
     cmds:
       - docker build -t {{.DOCKER_IMAGE}} .
 ```
 
 ## Task directory
 
-By default, tasks will be executed in the directory where the Taskfile is located. But you can easily make the task run in another folder, informing `dir`:
+By default, tasks will be executed in the directory where the Taskfile is
+located. But you can easily make the task run in another folder, informing
+`dir`:
 
 ```yaml
 version: '3'
 
 tasks:
   serve:
     dir: public/www
@@ -347,17 +415,20 @@
       - caddy
 ```
 
 If the directory does not exist, `task` creates it.
 
 ## Task dependencies
 
-> Dependencies run in parallel, so dependencies of a task should not depend one another. If you want to force tasks to run serially, take a look at the [Calling Another Task](#calling-another-task) section below.
+> Dependencies run in parallel, so dependencies of a task should not depend one
+> another. If you want to force tasks to run serially, take a look at the
+> [Calling Another Task](#calling-another-task) section below.
 
-You may have tasks that depend on others. Just pointing them on `deps` will make them run automatically before running the parent task:
+You may have tasks that depend on others. Just pointing them on `deps` will make
+them run automatically before running the parent task:
 
 ```yaml
 version: '3'
 
 tasks:
   build:
     deps: [assets]
@@ -365,15 +436,16 @@
       - go build -v -i main.go
 
   assets:
     cmds:
       - esbuild --bundle --minify css/index.css > public/bundle.css
 ```
 
-In the above example, `assets` will always run right before `build` if you run `task build`.
+In the above example, `assets` will always run right before `build` if you run
+`task build`.
 
 A task can have only dependencies and no commands to group tasks together:
 
 ```yaml
 version: '3'
 
 tasks:
@@ -385,23 +457,26 @@
       - esbuild --bundle --minify js/index.js > public/bundle.js
 
   css:
     cmds:
       - esbuild --bundle --minify css/index.css > public/bundle.css
 ```
 
-If there is more than one dependency, they always run in parallel for better performance.
+If there is more than one dependency, they always run in parallel for better
+performance.
 
 :::tip
 
-You can also make the tasks given by the command line run in parallel by using the `--parallel` flag (alias `-p`). Example: `task --parallel js css`.
+You can also make the tasks given by the command line run in parallel by using
+the `--parallel` flag (alias `-p`). Example: `task --parallel js css`.
 
 :::
 
-If you want to pass information to dependencies, you can do that the same manner as you would to [call another task](#calling-another-task):
+If you want to pass information to dependencies, you can do that the same manner
+as you would to [call another task](#calling-another-task):
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     deps:
@@ -416,19 +491,25 @@
   echo_sth:
     cmds:
       - echo {{.TEXT}}
 ```
 
 ## Platform specific tasks and commands
 
-If you want to restrict the running of tasks to explicit platforms, this can be achieved using the `platforms:` key. Tasks can be restricted to a specific OS, architecture or a combination of both. On a mismatch, the task or command will be skipped, and no error will be thrown.
+If you want to restrict the running of tasks to explicit platforms, this can be
+achieved using the `platforms:` key. Tasks can be restricted to a specific OS,
+architecture or a combination of both. On a mismatch, the task or command will
+be skipped, and no error will be thrown.
+
+The values allowed as OS or Arch are valid `GOOS` and `GOARCH` values, as
+defined by the Go language
+[here](https://github.com/golang/go/blob/master/src/go/build/syslist.go).
 
-The values allowed as OS or Arch are valid `GOOS` and `GOARCH` values, as defined by the Go language [here](https://github.com/golang/go/blob/master/src/go/build/syslist.go).
-
-The `build-windows` task below will run only on Windows, and on any architecture:
+The `build-windows` task below will run only on Windows, and on any
+architecture:
 
 ```yaml
 version: '3'
 
 tasks:
   build-windows:
     platforms: [windows]
@@ -483,15 +564,17 @@
       - cmd: echo 'Running command on Windows (amd64) and macOS'
         platforms: [windows/amd64, darwin]
       - cmd: echo 'Running on all platforms'
 ```
 
 ## Calling another task
 
-When a task has many dependencies, they are executed concurrently. This will often result in a faster build pipeline. However, in some situations, you may need to call other tasks serially. In this case, use the following syntax:
+When a task has many dependencies, they are executed concurrently. This will
+often result in a faster build pipeline. However, in some situations, you may
+need to call other tasks serially. In this case, use the following syntax:
 
 ```yaml
 version: '3'
 
 tasks:
   main-task:
     cmds:
@@ -504,15 +587,16 @@
       - echo "Task to be called"
 
   another-task:
     cmds:
       - echo "Another task"
 ```
 
-Using the `vars` and `silent` attributes you can choose to pass variables and toggle [silent mode](#silent-mode) on a call-by-call basis:
+Using the `vars` and `silent` attributes you can choose to pass variables and
+toggle [silent mode](#silent-mode) on a call-by-call basis:
 
 ```yaml
 version: '3'
 
 tasks:
   greet:
     vars:
@@ -527,23 +611,26 @@
         silent: true
 ```
 
 The above syntax is also supported in `deps`.
 
 :::tip
 
-NOTE: If you want to call a task declared in the root Taskfile from within an [included Taskfile](#including-other-taskfiles), add a leading `:` like this: `task: :task-name`.
+NOTE: If you want to call a task declared in the root Taskfile from within an
+[included Taskfile](#including-other-taskfiles), add a leading `:` like this:
+`task: :task-name`.
 
 :::
 
 ## Prevent unnecessary work
 
 ### By fingerprinting locally generated files and their sources
 
-If a task generates something, you can inform Task the source and generated files, so Task will prevent running them if not necessary.
+If a task generates something, you can inform Task the source and generated
+files, so Task will prevent running them if not necessary.
 
 ```yaml
 version: '3'
 
 tasks:
   build:
     deps: [js, css]
@@ -563,31 +650,37 @@
       - esbuild --bundle --minify css/index.css > public/bundle.css
     sources:
       - src/css/**/*.css
     generates:
       - public/bundle.css
 ```
 
-`sources` and `generates` can be files or glob patterns. When given, Task will compare the checksum of the source files to determine if it's necessary to run the task. If not, it will just print a message like `Task "js" is up to date`.
-
-`exclude:` can also be used to exclude files from fingerprinting. Sources are evaluated in order, so `exclude:` must come after the positive glob it is negating.
+`sources` and `generates` can be files or glob patterns. When given, Task will
+compare the checksum of the source files to determine if it's necessary to run
+the task. If not, it will just print a message like `Task "js" is up to date`.
+
+`exclude:` can also be used to exclude files from fingerprinting. Sources are
+evaluated in order, so `exclude:` must come after the positive glob it is
+negating.
 
 ```yaml
 version: '3'
 
 tasks:
   css:
     sources:
       - mysources/**/*.css
       - exclude: mysources/ignoreme.css
     generates:
       - public/bundle.css
 ```
 
-If you prefer these check to be made by the modification timestamp of the files, instead of its checksum (content), just set the `method` property to `timestamp`.
+If you prefer these check to be made by the modification timestamp of the files,
+instead of its checksum (content), just set the `method` property to
+`timestamp`.
 
 ```yaml
 version: '3'
 
 tasks:
   build:
     cmds:
@@ -595,51 +688,70 @@
     sources:
       - ./*.go
     generates:
       - app{{exeExt}}
     method: timestamp
 ```
 
-In situations where you need more flexibility the `status` keyword can be used. You can even combine the two. See the documentation for [status](#using-programmatic-checks-to-indicate-a-task-is-up-to-date) for an example.
+In situations where you need more flexibility the `status` keyword can be used.
+You can even combine the two. See the documentation for
+[status](#using-programmatic-checks-to-indicate-a-task-is-up-to-date) for an
+example.
 
 :::info
 
-By default, task stores checksums on a local `.task` directory in the project's directory. Most of the time, you'll want to have this directory on `.gitignore` (or equivalent) so it isn't committed. (If you have a task for code generation that is committed it may make sense to commit the checksum of that task as well, though).
+By default, task stores checksums on a local `.task` directory in the project's
+directory. Most of the time, you'll want to have this directory on `.gitignore`
+(or equivalent) so it isn't committed. (If you have a task for code generation
+that is committed it may make sense to commit the checksum of that task as well,
+though).
+
+If you want these files to be stored in another directory, you can set a
+`TASK_TEMP_DIR` environment variable in your machine. It can contain a relative
+path like `tmp/task` that will be interpreted as relative to the project
+directory, or an absolute or home path like `/tmp/.task` or `~/.task`
+(subdirectories will be created for each project).
 
-If you want these files to be stored in another directory, you can set a `TASK_TEMP_DIR` environment variable in your machine. It can contain a relative path like `tmp/task` that will be interpreted as relative to the project directory, or an absolute or home path like `/tmp/.task` or `~/.task` (subdirectories will be created for each project).
-
-```bash
+```shell
 export TASK_TEMP_DIR='~/.task'
 ```
 
 :::
 
 :::info
 
-Each task has only one checksum stored for its `sources`. If you want to distinguish a task by any of its input variables, you can add those variables as part of the task's label, and it will be considered a different task.
-
-This is useful if you want to run a task once for each distinct set of inputs until the sources actually change. For example, if the sources depend on the value of a variable, or you if you want the task to rerun if some arguments change even if the source has not.
+Each task has only one checksum stored for its `sources`. If you want to
+distinguish a task by any of its input variables, you can add those variables as
+part of the task's label, and it will be considered a different task.
+
+This is useful if you want to run a task once for each distinct set of inputs
+until the sources actually change. For example, if the sources depend on the
+value of a variable, or you if you want the task to rerun if some arguments
+change even if the source has not.
 
 :::
 
 :::tip
 
 The method `none` skips any validation and always run the task.
 
 :::
 
 :::info
 
-For the `checksum` (default) or `timestamp` method to work, it is only necessary to inform the source files. When the `timestamp` method is used, the last time of the running the task is considered as a generate.
+For the `checksum` (default) or `timestamp` method to work, it is only necessary
+to inform the source files. When the `timestamp` method is used, the last time
+of the running the task is considered as a generate.
 
 :::
 
 ### Using programmatic checks to indicate a task is up to date
 
-Alternatively, you can inform a sequence of tests as `status`. If no error is returned (exit status 0), the task is considered up-to-date:
+Alternatively, you can inform a sequence of tests as `status`. If no error is
+returned (exit status 0), the task is considered up-to-date:
 
 ```yaml
 version: '3'
 
 tasks:
   generate-files:
     cmds:
@@ -649,27 +761,39 @@
     # test existence of files
     status:
       - test -d directory
       - test -f directory/file1.txt
       - test -f directory/file2.txt
 ```
 
-Normally, you would use `sources` in combination with `generates` - but for tasks that generate remote artifacts (Docker images, deploys, CD releases) the checksum source and timestamps require either access to the artifact or for an out-of-band refresh of the `.checksum` fingerprint file.
-
-Two special variables `{{.CHECKSUM}}` and `{{.TIMESTAMP}}` are available for interpolation within `status` commands, depending on the method assigned to fingerprint the sources. Only `source` globs are fingerprinted.
-
-Note that the `{{.TIMESTAMP}}` variable is a "live" Go `time.Time` struct, and can be formatted using any of the methods that `time.Time` responds to.
-
-See [the Go Time documentation](https://golang.org/pkg/time/) for more information.
-
-You can use `--force` or `-f` if you want to force a task to run even when up-to-date.
-
-Also, `task --status [tasks]...` will exit with a non-zero exit code if any of the tasks are not up-to-date.
-
-`status` can be combined with the [fingerprinting](#by-fingerprinting-locally-generated-files-and-their-sources) to have a task run if either the the source/generated artifacts changes, or the programmatic check fails:
+Normally, you would use `sources` in combination with `generates` - but for
+tasks that generate remote artifacts (Docker images, deploys, CD releases) the
+checksum source and timestamps require either access to the artifact or for an
+out-of-band refresh of the `.checksum` fingerprint file.
+
+Two special variables `{{.CHECKSUM}}` and `{{.TIMESTAMP}}` are available for
+interpolation within `status` commands, depending on the method assigned to
+fingerprint the sources. Only `source` globs are fingerprinted.
+
+Note that the `{{.TIMESTAMP}}` variable is a "live" Go `time.Time` struct, and
+can be formatted using any of the methods that `time.Time` responds to.
+
+See [the Go Time documentation](https://golang.org/pkg/time/) for more
+information.
+
+You can use `--force` or `-f` if you want to force a task to run even when
+up-to-date.
+
+Also, `task --status [tasks]...` will exit with a non-zero exit code if any of
+the tasks are not up-to-date.
+
+`status` can be combined with the
+[fingerprinting](#by-fingerprinting-locally-generated-files-and-their-sources)
+to have a task run if either the the source/generated artifacts changes, or the
+programmatic check fails:
 
 ```yaml
 version: '3'
 
 tasks:
   build:prod:
     desc: Build for production usage.
@@ -685,15 +809,19 @@
     # But also run the task if the last build was not a production build.
     status:
       - grep -q '"dev": false' ./vendor/composer/installed.json
 ```
 
 ### Using programmatic checks to cancel the execution of a task and its dependencies
 
-In addition to `status` checks, `preconditions` checks are the logical inverse of `status` checks. That is, if you need a certain set of conditions to be _true_ you can use the `preconditions` stanza. `preconditions` are similar to `status` lines, except they support `sh` expansion, and they SHOULD all return 0.
+In addition to `status` checks, `preconditions` checks are the logical inverse
+of `status` checks. That is, if you need a certain set of conditions to be
+_true_ you can use the `preconditions` stanza. `preconditions` are similar to
+`status` lines, except they support `sh` expansion, and they SHOULD all
+return 0.
 
 ```yaml
 version: '3'
 
 tasks:
   generate-files:
     cmds:
@@ -703,19 +831,24 @@
     # test existence of files
     preconditions:
       - test -f .env
       - sh: '[ 1 = 0 ]'
         msg: "One doesn't equal Zero, Halting"
 ```
 
-Preconditions can set specific failure messages that can tell a user what steps to take using the `msg` field.
+Preconditions can set specific failure messages that can tell a user what steps
+to take using the `msg` field.
 
-If a task has a dependency on a sub-task with a precondition, and that precondition is not met - the calling task will fail. Note that a task executed with a failing precondition will not run unless `--force` is given.
-
-Unlike `status`, which will skip a task if it is up to date and continue executing tasks that depend on it, a `precondition` will fail a task, along with any other tasks that depend on it.
+If a task has a dependency on a sub-task with a precondition, and that
+precondition is not met - the calling task will fail. Note that a task executed
+with a failing precondition will not run unless `--force` is given.
+
+Unlike `status`, which will skip a task if it is up to date and continue
+executing tasks that depend on it, a `precondition` will fail a task, along with
+any other tasks that depend on it.
 
 ```yaml
 version: '3'
 
 tasks:
   task-will-fail:
     preconditions:
@@ -729,21 +862,25 @@
     cmds:
       - task: task-will-fail
       - echo "I will not run"
 ```
 
 ### Limiting when tasks run
 
-If a task executed by multiple `cmds` or multiple `deps` you can control when it is executed using `run`. `run` can also be set at the root of the Taskfile to change the behavior of all the tasks unless explicitly overridden.
+If a task executed by multiple `cmds` or multiple `deps` you can control when it
+is executed using `run`. `run` can also be set at the root of the Taskfile to
+change the behavior of all the tasks unless explicitly overridden.
 
 Supported values for `run`:
 
-- `always` (default) always attempt to invoke the task regardless of the number of previous executions
+- `always` (default) always attempt to invoke the task regardless of the number
+  of previous executions
 - `once` only invoke this task once regardless of the number of references
-- `when_changed` only invokes the task once for each unique set of variables passed into the task
+- `when_changed` only invokes the task once for each unique set of variables
+  passed into the task
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     cmds:
@@ -765,17 +902,22 @@
     run: once
     cmds:
       - sleep 5 # long operation like installing packages
 ```
 
 ### Ensuring required variables are set
 
-If you want to check that certain variables are set before running a task then you can use `requires`. This is useful when might not be clear to users which variables are needed, or if you want clear message about what is required. Also some tasks could have dangerous side effects if run with un-set variables.
-
-Using `requires` you specify an array of strings in the `vars` sub-section under `requires`, these strings are variable names which are checked prior to running the task. If any variables are un-set the the task will error and not run.
+If you want to check that certain variables are set before running a task then
+you can use `requires`. This is useful when might not be clear to users which
+variables are needed, or if you want clear message about what is required. Also
+some tasks could have dangerous side effects if run with un-set variables.
+
+Using `requires` you specify an array of strings in the `vars` sub-section under
+`requires`, these strings are variable names which are checked prior to running
+the task. If any variables are un-set the the task will error and not run.
 
 Environmental variables are also checked.
 
 Syntax:
 
 ```yaml
 requires:
@@ -801,38 +943,44 @@
     # Make sure these variables are set before running
     requires:
       vars: [IMAGE_NAME, IMAGE_TAG]
 ```
 
 ## Variables
 
-When doing interpolation of variables, Task will look for the below. They are listed below in order of importance (i.e. most important first):
+When doing interpolation of variables, Task will look for the below. They are
+listed below in order of importance (i.e. most important first):
 
 - Variables declared in the task definition
-- Variables given while calling a task from another (See [Calling another task](#calling-another-task) above)
-- Variables of the [included Taskfile](#including-other-taskfiles) (when the task is included)
-- Variables of the [inclusion of the Taskfile](#vars-of-included-taskfiles) (when the task is included)
+- Variables given while calling a task from another (See
+  [Calling another task](#calling-another-task) above)
+- Variables of the [included Taskfile](#including-other-taskfiles) (when the
+  task is included)
+- Variables of the [inclusion of the Taskfile](#vars-of-included-taskfiles)
+  (when the task is included)
 - Global variables (those declared in the `vars:` option in the Taskfile)
 - Environment variables
 
 Example of sending parameters with environment variables:
 
-```bash
+```shell
 $ TASK_VARIABLE=a-value task do-something
 ```
 
 :::tip
 
 A special variable `.TASK` is always available containing the task name.
 
 :::
 
-Since some shells do not support the above syntax to set environment variables (Windows) tasks also accept a similar style when not at the beginning of the command.
+Since some shells do not support the above syntax to set environment variables
+(Windows) tasks also accept a similar style when not at the beginning of the
+command.
 
-```bash
+```shell
 $ task write-file FILE=file.txt "CONTENT=Hello, World!" print "MESSAGE=All done!"
 ```
 
 Example of locally declared vars:
 
 ```yaml
 version: '3'
@@ -857,15 +1005,17 @@
   greet:
     cmds:
       - echo "{{.GREETING}}"
 ```
 
 ### Dynamic variables
 
-The below syntax (`sh:` prop in a variable) is considered a dynamic variable. The value will be treated as a command and the output assigned. If there are one or more trailing newlines, the last newline will be trimmed.
+The below syntax (`sh:` prop in a variable) is considered a dynamic variable.
+The value will be treated as a command and the output assigned. If there are one
+or more trailing newlines, the last newline will be trimmed.
 
 ```yaml
 version: '3'
 
 tasks:
   build:
     cmds:
@@ -875,19 +1025,22 @@
         sh: git log -n 1 --format=%h
 ```
 
 This works for all types of variables.
 
 ## Looping over values
 
-As of v3.28.0, Task allows you to loop over certain values and execute a command for each. There are a number of ways to do this depending on the type of value you want to loop over.
+As of v3.28.0, Task allows you to loop over certain values and execute a command
+for each. There are a number of ways to do this depending on the type of value
+you want to loop over.
 
 ### Looping over a static list
 
-The simplest kind of loop is an explicit one. This is useful when you want to loop over a set of values that are known ahead of time.
+The simplest kind of loop is an explicit one. This is useful when you want to
+loop over a set of values that are known ahead of time.
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     cmds:
@@ -908,17 +1061,22 @@
       - foo.txt
       - bar.txt
     cmds:
       - for: sources
         cmd: cat {{ .ITEM }}
 ```
 
-This will also work if you use globbing syntax in your sources. For example, if you specify a source for `*.txt`, the loop will iterate over all files that match that glob.
-
-Source paths will always be returned as paths relative to the task directory. If you need to convert this to an absolute path, you can use the built-in `joinPath` function. There are some [special variables](/api/#special-variables) that you may find useful for this.
+This will also work if you use globbing syntax in your sources. For example, if
+you specify a source for `*.txt`, the loop will iterate over all files that
+match that glob.
+
+Source paths will always be returned as paths relative to the task directory. If
+you need to convert this to an absolute path, you can use the built-in
+`joinPath` function. There are some [special variables](/api/#special-variables)
+that you may find useful for this.
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     vars:
@@ -930,29 +1088,32 @@
     cmds:
       - for: sources
         cmd: cat {{joinPath .MY_DIR .ITEM}}
 ```
 
 ### Looping over variables
 
-To loop over the contents of a variable, you simply need to specify the variable you want to loop over. By default, variables will be split on any whitespace characters.
+To loop over the contents of a variable, you simply need to specify the variable
+you want to loop over. By default, variables will be split on any whitespace
+characters.
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     vars:
       MY_VAR: foo.txt bar.txt
     cmds:
       - for: { var: MY_VAR }
         cmd: cat {{.ITEM}}
 ```
 
-If you need to split on a different character, you can do this by specifying the `split` property:
+If you need to split on a different character, you can do this by specifying the
+`split` property:
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     vars:
@@ -975,15 +1136,16 @@
     cmds:
       - for: { var: MY_VAR }
         cmd: cat {{.ITEM}}
 ```
 
 ### Renaming variables
 
-If you want to rename the iterator variable to make it clearer what the value contains, you can do so by specifying the `as` property:
+If you want to rename the iterator variable to make it clearer what the value
+contains, you can do so by specifying the `as` property:
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     vars:
@@ -991,15 +1153,17 @@
     cmds:
       - for: { var: MY_VAR, as: FILE }
         cmd: cat {{.FILE}}
 ```
 
 ### Looping over tasks
 
-Because the `for` property is defined at the `cmds` level, you can also use it alongside the `task` keyword to run tasks multiple times with different variables.
+Because the `for` property is defined at the `cmds` level, you can also use it
+alongside the `task` keyword to run tasks multiple times with different
+variables.
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     cmds:
@@ -1029,51 +1193,139 @@
       - echo 'foo'
 
   task-bar:
     cmds:
       - echo 'bar'
 ```
 
+### Looping over dependencies
+
+All of the above looping techniques can also be applied to the `deps` property.
+This allows you to combine loops with concurrency:
+
+```yaml
+version: '3'
+
+tasks:
+  default:
+    deps:
+      - for: [foo, bar]
+        task: my-task
+        vars:
+          FILE: '{{.ITEM}}'
+
+  my-task:
+    cmds:
+      - echo '{{.FILE}}'
+```
+
+It is important to note that as `deps` are run in parallel, the order in which
+the iterations are run is not guaranteed and the output may vary. For example,
+the output of the above example may be either:
+
+```shell
+foo
+bar
+```
+
+or
+
+```shell
+bar
+foo
+```
+
 ## Forwarding CLI arguments to commands
 
-If `--` is given in the CLI, all following parameters are added to a special `.CLI_ARGS` variable. This is useful to forward arguments to another command.
+If `--` is given in the CLI, all following parameters are added to a special
+`.CLI_ARGS` variable. This is useful to forward arguments to another command.
 
 The below example will run `yarn install`.
 
-```bash
+```shell
 $ task yarn -- install
 ```
 
 ```yaml
 version: '3'
 
 tasks:
   yarn:
     cmds:
       - yarn {{.CLI_ARGS}}
 ```
 
+## Wildcard arguments
+
+Another way to parse arguments into a task is to use a wildcard in your task's
+name. Wildcards are denoted by an asterisk (`*`) and can be used multiple times
+in a task's name to pass in multiple arguments.
+
+Matching arguments will be captured and stored in the `.MATCH` variable and can
+then be used in your task's commands like any other variable. This variable is
+an array of strings and so will need to be indexed to access the individual
+arguments. We suggest creating a named variable for each argument to make it
+clear what they contain:
+
+```yaml
+version: '3'
+
+tasks:
+  echo-*:
+    vars:
+      TEXT: '{{index .MATCH 0}}'
+    cmds:
+      - echo {{.TEXT}}
+
+  run-*-*:
+    vars:
+      ARG_1: '{{index .MATCH 0}}'
+      ARG_2: '{{index .MATCH 1}}'
+    cmds:
+      - echo {{.ARG_1}} {{.ARG_2}}
+```
+
+```shell
+# This call matches the "echo-*" task and the string "hello" is captured by the
+# wildcard and stored in the .MATCH variable. We then index the .MATCH array and
+# store the result in the .TEXT variable which is then echoed out in the cmds.
+$ task echo-hello
+hello
+# You can use whitespace in your arguments as long as you quote the task name
+$ task "echo-hello world"
+hello world
+# And you can pass multiple arguments
+$ task run-foo-bar
+foo bar
+```
+
+If multiple matching tasks are found, an error occurs. If you are using included
+Taskfiles, tasks in parent files will be considered first.
+
 ## Doing task cleanup with `defer`
 
-With the `defer` keyword, it's possible to schedule cleanup to be run once the task finishes. The difference with just putting it as the last command is that this command will run even when the task fails.
+With the `defer` keyword, it's possible to schedule cleanup to be run once the
+task finishes. The difference with just putting it as the last command is that
+this command will run even when the task fails.
 
 In the example below, `rm -rf tmpdir/` will run even if the third command fails:
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     cmds:
       - mkdir -p tmpdir/
       - defer: rm -rf tmpdir/
       - echo 'Do work on tmpdir/'
 ```
 
-If you want to move the cleanup command into another task, that is possible as well:
+If you want to move the cleanup command into another task, that is possible as
+well:
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     cmds:
@@ -1082,44 +1334,69 @@
       - echo 'Do work on tmpdir/'
 
   cleanup: rm -rf tmpdir/
 ```
 
 :::info
 
-Due to the nature of how the [Go's own `defer` work](https://go.dev/tour/flowcontrol/13), the deferred commands are executed in the reverse order if you schedule multiple of them.
+Due to the nature of how the
+[Go's own `defer` work](https://go.dev/tour/flowcontrol/13), the deferred
+commands are executed in the reverse order if you schedule multiple of them.
 
 :::
 
 ## Go's template engine
 
-Task parse commands as [Go's template engine][gotemplate] before executing them. Variables are accessible through dot syntax (`.VARNAME`).
+Task parse commands as [Go's template engine][gotemplate] before executing them.
+Variables are accessible through dot syntax (`.VARNAME`).
 
-All functions by the Go's [slim-sprig lib](https://go-task.github.io/slim-sprig/) are available. The following example gets the current date in a given format:
+All functions by the Go's
+[slim-sprig lib](https://go-task.github.io/slim-sprig/) are available. The
+following example gets the current date in a given format:
 
 ```yaml
 version: '3'
 
 tasks:
   print-date:
     cmds:
       - echo {{now | date "2006-01-02"}}
 ```
 
 Task also adds the following functions:
 
-- `OS`: Returns the operating system. Possible values are `windows`, `linux`, `darwin` (macOS) and `freebsd`.
-- `ARCH`: return the architecture Task was compiled to: `386`, `amd64`, `arm` or `s390x`.
+- `OS`: Returns the operating system. Possible values are `windows`, `linux`,
+  `darwin` (macOS) and `freebsd`.
+- `ARCH`: return the architecture Task was compiled to: `386`, `amd64`, `arm` or
+  `s390x`.
 - `splitLines`: Splits Unix (`\n`) and Windows (`\r\n`) styled newlines.
-- `catLines`: Replaces Unix (`\n`) and Windows (`\r\n`) styled newlines with a space.
-- `toSlash`: Does nothing on Unix, but on Windows converts a string from `\` path format to `/`.
-- `fromSlash`: Opposite of `toSlash`. Does nothing on Unix, but on Windows converts a string from `/` path format to `\`.
-- `exeExt`: Returns the right executable extension for the current OS (`".exe"` for Windows, `""` for others).
-- `shellQuote`: Quotes a string to make it safe for use in shell scripts. Task uses [this Go function](https://pkg.go.dev/mvdan.cc/sh/v3@v3.4.0/syntax#Quote) for this. The Bash dialect is assumed.
-- `splitArgs`: Splits a string as if it were a command's arguments. Task uses [this Go function](https://pkg.go.dev/mvdan.cc/sh/v3@v3.4.0/shell#Fields)
+- `catLines`: Replaces Unix (`\n`) and Windows (`\r\n`) styled newlines with a
+  space.
+- `toSlash`: Does nothing on Unix, but on Windows converts a string from `\`
+  path format to `/`.
+- `fromSlash`: Opposite of `toSlash`. Does nothing on Unix, but on Windows
+  converts a string from `/` path format to `\`.
+- `exeExt`: Returns the right executable extension for the current OS (`".exe"`
+  for Windows, `""` for others).
+- `shellQuote`: Quotes a string to make it safe for use in shell scripts. Task
+  uses [this Go function](https://pkg.go.dev/mvdan.cc/sh/v3@v3.4.0/syntax#Quote)
+  for this. The Bash dialect is assumed.
+- `splitArgs`: Splits a string as if it were a command's arguments. Task uses
+  [this Go function](https://pkg.go.dev/mvdan.cc/sh/v3@v3.4.0/shell#Fields)
+- `joinPath`: Joins any number of arguments into a path. The same as Go's
+  [filepath.Join](https://pkg.go.dev/path/filepath#Join).
+- `relPath`: Converts an absolute path (second argument) into a relative path,
+  based on a base path (first argument). The same as Go's
+  [filepath.Rel](https://pkg.go.dev/path/filepath#Rel).
+- `merge`: Creates a new map that is a copy of the first map with the keys of
+  each subsequent map merged into it. If there is a duplicate key, the value of
+  the last map with that key is used.
+- `spew`: Returns the Go representation of a specific variable. Useful for
+  debugging. Uses the [davecgh/go-spew](https://github.com/davecgh/go-spew)
+  package.
 
 Example:
 
 ```yaml
 version: '3'
 
 tasks:
@@ -1140,15 +1417,16 @@
         {{range $i, $line := .CONTENT | splitLines -}}
         {{printf "%3d" $i}}: {{$line}}
         {{end}}EOF
 ```
 
 ## Help
 
-Running `task --list` (or `task -l`) lists all tasks with a description. The following Taskfile:
+Running `task --list` (or `task -l`) lists all tasks with a description. The
+following Taskfile:
 
 ```yaml
 version: '3'
 
 tasks:
   build:
     desc: Build the go binary.
@@ -1167,24 +1445,25 @@
   css:
     cmds:
       - esbuild --bundle --minify css/index.css > public/bundle.css
 ```
 
 would print the following output:
 
-```bash
+```shell
 * build:   Build the go binary.
 * test:    Run all the go tests.
 ```
 
 If you want to see all tasks, there's a `--list-all` (alias `-a`) flag as well.
 
 ## Display summary of task
 
-Running `task --summary task-name` will show a summary of a task. The following Taskfile:
+Running `task --summary task-name` will show a summary of a task. The following
+Taskfile:
 
 ```yaml
 version: '3'
 
 tasks:
   release:
     deps: [build]
@@ -1214,21 +1493,27 @@
 dependencies:
  - build
 
 commands:
  - your-release-tool
 ```
 
-If a summary is missing, the description will be printed. If the task does not have a summary or a description, a warning is printed.
+If a summary is missing, the description will be printed. If the task does not
+have a summary or a description, a warning is printed.
 
 Please note: _showing the summary will not execute the command_.
 
 ## Task aliases
 
-Aliases are alternative names for tasks. They can be used to make it easier and quicker to run tasks with long or hard-to-type names. You can use them on the command line, when [calling sub-tasks](#calling-another-task) in your Taskfile and when [including tasks](#including-other-taskfiles) with aliases from another Taskfile. They can also be used together with [namespace aliases](#namespace-aliases).
+Aliases are alternative names for tasks. They can be used to make it easier and
+quicker to run tasks with long or hard-to-type names. You can use them on the
+command line, when [calling sub-tasks](#calling-another-task) in your Taskfile
+and when [including tasks](#including-other-taskfiles) with aliases from another
+Taskfile. They can also be used together with
+[namespace aliases](#namespace-aliases).
 
 ```yaml
 version: '3'
 
 tasks:
   generate:
     aliases: [gen]
@@ -1239,15 +1524,17 @@
     aliases: [gen-mocks]
     cmds:
       - echo "generating..."
 ```
 
 ## Overriding task name
 
-Sometimes you may want to override the task name printed on the summary, up-to-date messages to STDOUT, etc. In this case, you can just set `label:`, which can also be interpolated with variables:
+Sometimes you may want to override the task name printed on the summary,
+up-to-date messages to STDOUT, etc. In this case, you can just set `label:`,
+which can also be interpolated with variables:
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     - task: print
@@ -1261,17 +1548,19 @@
     label: 'print-{{.MESSAGE}}'
     cmds:
       - echo "{{.MESSAGE}}"
 ```
 
 ## Warning Prompts
 
-Warning Prompts are used to prompt a user for confirmation before a task is executed.
+Warning Prompts are used to prompt a user for confirmation before a task is
+executed.
 
-Below is an example using `prompt` with a dangerous command, that is called between two safe commands:
+Below is an example using `prompt` with a dangerous command, that is called
+between two safe commands:
 
 ```yaml
 version: '3'
 
 tasks:
   example:
     cmds:
@@ -1289,61 +1578,68 @@
 
   dangerous:
     prompt: This is a dangerous command... Do you want to continue?
     cmds:
       - echo 'dangerous command'
 ```
 
-```bash
+```shell
 ❯ task dangerous
 task: "This is a dangerous command... Do you want to continue?" [y/N]
 ```
 
-Warning prompts are called before executing a task. If a prompt is denied Task will exit with [exit code](/api#exit-codes) 205. If approved, Task will continue as normal.
+Warning prompts are called before executing a task. If a prompt is denied Task
+will exit with [exit code](/api#exit-codes) 205. If approved, Task will continue
+as normal.
 
-```bash
+```shell
 ❯ task example
 not dangerous command
 task: "This is a dangerous command. Do you want to continue?" [y/N]
 y
 dangerous command
 another not dangerous command
 ```
 
-To skip warning prompts automatically, you can use the `--yes` (alias `-y`) option when calling the task. By including this option, all warnings, will be automatically confirmed, and no prompts will be shown.
+To skip warning prompts automatically, you can use the `--yes` (alias `-y`)
+option when calling the task. By including this option, all warnings, will be
+automatically confirmed, and no prompts will be shown.
 
 :::caution
 
-Tasks with prompts always fail by default on non-terminal environments, like a CI, where an `stdin` won't be available for the user to answer. In those cases, use `--yes` (`-y`) to force all tasks with a prompt to run.
+Tasks with prompts always fail by default on non-terminal environments, like a
+CI, where an `stdin` won't be available for the user to answer. In those cases,
+use `--yes` (`-y`) to force all tasks with a prompt to run.
 
 :::
 
 ## Silent mode
 
-Silent mode disables the echoing of commands before Task runs it. For the following Taskfile:
+Silent mode disables the echoing of commands before Task runs it. For the
+following Taskfile:
 
 ```yaml
 version: '3'
 
 tasks:
   echo:
     cmds:
       - echo "Print something"
 ```
 
 Normally this will be printed:
 
-```sh
+```shell
 echo "Print something"
 Print something
 ```
 
 With silent mode on, the below will be printed instead:
 
-```sh
+```shell
 Print something
 ```
 
 There are four ways to enable silent mode:
 
 - At command level:
 
@@ -1393,50 +1689,61 @@
   echo:
     cmds:
       - echo "This will print nothing" > /dev/null
 ```
 
 ## Dry run mode
 
-Dry run mode (`--dry`) compiles and steps through each task, printing the commands that would be run without executing them. This is useful for debugging your Taskfiles.
+Dry run mode (`--dry`) compiles and steps through each task, printing the
+commands that would be run without executing them. This is useful for debugging
+your Taskfiles.
 
 ## Ignore errors
 
-You have the option to ignore errors during command execution. Given the following Taskfile:
+You have the option to ignore errors during command execution. Given the
+following Taskfile:
 
 ```yaml
 version: '3'
 
 tasks:
   echo:
     cmds:
       - exit 1
       - echo "Hello World"
 ```
 
-Task will abort the execution after running `exit 1` because the status code `1` stands for `EXIT_FAILURE`. However, it is possible to continue with execution using `ignore_error`:
+Task will abort the execution after running `exit 1` because the status code `1`
+stands for `EXIT_FAILURE`. However, it is possible to continue with execution
+using `ignore_error`:
 
 ```yaml
 version: '3'
 
 tasks:
   echo:
     cmds:
       - cmd: exit 1
         ignore_error: true
       - echo "Hello World"
 ```
 
-`ignore_error` can also be set for a task, which means errors will be suppressed for all commands. Nevertheless, keep in mind that this option will not propagate to other tasks called either by `deps` or `cmds`!
+`ignore_error` can also be set for a task, which means errors will be suppressed
+for all commands. Nevertheless, keep in mind that this option will not propagate
+to other tasks called either by `deps` or `cmds`!
 
 ## Output syntax
 
-By default, Task just redirects the STDOUT and STDERR of the running commands to the shell in real-time. This is good for having live feedback for logging printed by commands, but the output can become messy if you have multiple commands running simultaneously and printing lots of stuff.
+By default, Task just redirects the STDOUT and STDERR of the running commands to
+the shell in real-time. This is good for having live feedback for logging
+printed by commands, but the output can become messy if you have multiple
+commands running simultaneously and printing lots of stuff.
 
-To make this more customizable, there are currently three different output options you can choose:
+To make this more customizable, there are currently three different output
+options you can choose:
 
 - `interleaved` (default)
 - `group`
 - `prefixed`
 
 To choose another one, just set it to root in the Taskfile:
 
@@ -1445,17 +1752,24 @@
 
 output: 'group'
 
 tasks:
   # ...
 ```
 
-The `group` output will print the entire output of a command once after it finishes, so you will not have live feedback for commands that take a long time to run.
-
-When using the `group` output, you can optionally provide a templated message to print at the start and end of the group. This can be useful for instructing CI systems to group all of the output for a given task, such as with [GitHub Actions' `::group::` command](https://docs.github.com/en/actions/learn-github-actions/workflow-commands-for-github-actions#grouping-log-lines) or [Azure Pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/scripts/logging-commands?expand=1&view=azure-devops&tabs=bash#formatting-commands).
+The `group` output will print the entire output of a command once after it
+finishes, so you will not have live feedback for commands that take a long time
+to run.
+
+When using the `group` output, you can optionally provide a templated message to
+print at the start and end of the group. This can be useful for instructing CI
+systems to group all of the output for a given task, such as with
+[GitHub Actions' `::group::` command](https://docs.github.com/en/actions/learn-github-actions/workflow-commands-for-github-actions#grouping-log-lines)
+or
+[Azure Pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/scripts/logging-commands?expand=1&view=azure-devops&tabs=bash#formatting-commands).
 
 ```yaml
 version: '3'
 
 output:
   group:
     begin: '::group::{{.TASK}}'
@@ -1464,22 +1778,24 @@
 tasks:
   default:
     cmds:
       - echo 'Hello, World!'
     silent: true
 ```
 
-```bash
+```shell
 $ task default
 ::group::default
 Hello, World!
 ::endgroup::
 ```
 
-When using the `group` output, you may swallow the output of the executed command on standard output and standard error if it does not fail (zero exit code).
+When using the `group` output, you may swallow the output of the executed
+command on standard output and standard error if it does not fail (zero exit
+code).
 
 ```yaml
 version: '3'
 
 silent: true
 
 output:
@@ -1487,22 +1803,24 @@
     error_only: true
 
 tasks:
   passes: echo 'output-of-passes'
   errors: echo 'output-of-errors' && exit 1
 ```
 
-```bash
+```shell
 $ task passes
 $ task errors
 output-of-errors
 task: Failed to run task "errors": exit status 1
 ```
 
-The `prefix` output will prefix every line printed by a command with `[task-name]` as the prefix, but you can customize the prefix for a command with the `prefix:` attribute:
+The `prefix` output will prefix every line printed by a command with
+`[task-name] ` as the prefix, but you can customize the prefix for a command
+with the `prefix:` attribute:
 
 ```yaml
 version: '3'
 
 output: prefixed
 
 tasks:
@@ -1518,107 +1836,124 @@
   print:
     cmds:
       - echo "{{.TEXT}}"
     prefix: 'print-{{.TEXT}}'
     silent: true
 ```
 
-```bash
+```shell
 $ task default
 [print-foo] foo
 [print-bar] bar
 [print-baz] baz
 ```
 
 :::tip
 
 The `output` option can also be specified by the `--output` or `-o` flags.
 
 :::
 
 ## Interactive CLI application
 
-When running interactive CLI applications inside Task they can sometimes behave weirdly, especially when the [output mode](#output-syntax) is set to something other than `interleaved` (the default), or when interactive apps are run in parallel with other tasks.
+When running interactive CLI applications inside Task they can sometimes behave
+weirdly, especially when the [output mode](#output-syntax) is set to something
+other than `interleaved` (the default), or when interactive apps are run in
+parallel with other tasks.
 
-The `interactive: true` tells Task this is an interactive application and Task will try to optimize for it:
+The `interactive: true` tells Task this is an interactive application and Task
+will try to optimize for it:
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     cmds:
       - vim my-file.txt
     interactive: true
 ```
 
-If you still have problems running an interactive app through Task, please open an issue about it.
+If you still have problems running an interactive app through Task, please open
+an issue about it.
 
 ## Short task syntax
 
-Starting on Task v3, you can now write tasks with a shorter syntax if they have the default settings (e.g. no custom `env:`, `vars:`, `desc:`, `silent:` , etc):
+Starting on Task v3, you can now write tasks with a shorter syntax if they have
+the default settings (e.g. no custom `env:`, `vars:`, `desc:`, `silent:` , etc):
 
 ```yaml
 version: '3'
 
 tasks:
   build: go build -v -o ./app{{exeExt}} .
 
   run:
     - task: build
     - ./app{{exeExt}} -h localhost -p 8080
 ```
 
 ## `set` and `shopt`
 
-It's possible to specify options to the [`set`](https://www.gnu.org/software/bash/manual/html_node/The-Set-Builtin.html) and [`shopt`](https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html) builtins. This can be added at global, task or command level.
+It's possible to specify options to the
+[`set`](https://www.gnu.org/software/bash/manual/html_node/The-Set-Builtin.html)
+and
+[`shopt`](https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html)
+builtins. This can be added at global, task or command level.
 
 ```yaml
 version: '3'
 
 set: [pipefail]
 shopt: [globstar]
 
 tasks:
   # `globstar` required for double star globs to work
   default: echo **/*.go
 ```
 
 :::info
 
-Keep in mind that not all options are available in the [shell interpreter library](https://github.com/mvdan/sh) that Task uses.
+Keep in mind that not all options are available in the
+[shell interpreter library](https://github.com/mvdan/sh) that Task uses.
 
 :::
 
 ## Watch tasks
 
-With the flags `--watch` or `-w` task will watch for file changes and run the task again. This requires the `sources` attribute to be given, so task knows which files to watch.
-
-The default watch interval is 5 seconds, but it's possible to change it by either setting `interval: '500ms'` in the root of the Taskfile passing it as an argument like `--interval=500ms`.
+With the flags `--watch` or `-w` task will watch for file changes and run the
+task again. This requires the `sources` attribute to be given, so task knows
+which files to watch.
+
+The default watch interval is 5 seconds, but it's possible to change it by
+either setting `interval: '500ms'` in the root of the Taskfile or by passing it
+as an argument like `--interval=500ms`.
 
-Also, it's possible to set `watch: true` in a given task and it'll automatically run in watch mode:
+Also, it's possible to set `watch: true` in a given task and it'll automatically
+run in watch mode:
 
 ```yaml
 version: '3'
 
 interval: 500ms
 
 tasks:
   build:
     desc: Builds the Go application
     watch: true
     sources:
       - '**/*.go'
     cmds:
-      - go build  # ...
+      - go build # ...
 ```
 
 :::info
 
-Note that when setting `watch: true` to a task, it'll only run in watch mode when running from the CLI via `task my-watch-task`, but won't run in watch mode if called by another task, either directly or as a dependency.
+Note that when setting `watch: true` to a task, it'll only run in watch mode
+when running from the CLI via `task my-watch-task`, but won't run in watch mode
+if called by another task, either directly or as a dependency.
 
 :::
 
-<!-- prettier-ignore-start -->
-
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-start */}
 [gotemplate]: https://golang.org/pkg/text/template/
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.35.1/task/docs/package.json` & `go_task_bin-3.36.0/task/website/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.969047619047619%*

 * *Differences: {"'dependencies'": "{'@docusaurus/core': '^3.2.0', '@docusaurus/preset-classic': '^3.2.0'}",*

 * * "'devDependencies'": "{'@crowdin/cli': '^3.19.2', '@crowdin/crowdin-api-client': '^1.33.0', "*

 * *                      "'@docusaurus/module-type-aliases': '^3.2.0', '@docusaurus/tsconfig': "*

 * *                      "'^3.2.0', '@docusaurus/types': '^3.2.0'}",*

 * * "'scripts'": "{'crowdin:sync': 'docusaurus write-translations && crowdin upload && crowdin "*

 * *              "download'}"}*

```diff
@@ -8,31 +8,31 @@
         "production": [
             ">0.5%",
             "not dead",
             "not op_mini all"
         ]
     },
     "dependencies": {
-        "@docusaurus/core": "^3.0.1",
-        "@docusaurus/preset-classic": "^3.0.1",
+        "@docusaurus/core": "^3.2.0",
+        "@docusaurus/preset-classic": "^3.2.0",
         "@mdx-js/react": "^3.0.0",
         "clsx": "^2.0.0",
         "prism-react-renderer": "^2.1.0",
         "raw-loader": "^4.0.2",
         "react": "^18.2.0",
         "react-dom": "^18.2.0",
         "remark-gfm": "^4.0.0",
         "remark-github": "^12.0.0"
     },
     "devDependencies": {
-        "@crowdin/cli": "^3.10.1",
-        "@crowdin/crowdin-api-client": "^1.22.1",
-        "@docusaurus/module-type-aliases": "^3.0.1",
-        "@docusaurus/tsconfig": "^3.0.1",
-        "@docusaurus/types": "^3.0.1",
+        "@crowdin/cli": "^3.19.2",
+        "@crowdin/crowdin-api-client": "^1.33.0",
+        "@docusaurus/module-type-aliases": "^3.2.0",
+        "@docusaurus/tsconfig": "^3.2.0",
+        "@docusaurus/types": "^3.2.0",
         "@types/react": "^18.2.29",
         "typescript": "^5.3.3"
     },
     "engines": {
         "node": ">=18.0"
     },
     "name": "taskfile-dev",
@@ -40,14 +40,15 @@
     "repository": {
         "type": "git",
         "url": "https://github.com/go-task/task"
     },
     "scripts": {
         "build": "docusaurus build",
         "clear": "docusaurus clear",
+        "crowdin:sync": "docusaurus write-translations && crowdin upload && crowdin download",
         "deploy": "docusaurus deploy",
         "docusaurus": "docusaurus",
         "serve": "docusaurus serve",
         "start": "docusaurus start",
         "swizzle": "docusaurus swizzle",
         "write-heading-ids": "docusaurus write-heading-ids",
         "write-translations": "docusaurus write-translations"
```

### Comparing `go_task_bin-3.35.1/task/docs/src/api/crowdin.js` & `go_task_bin-3.36.0/task/website/src/api/crowdin.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/src/css/carbon.css` & `go_task_bin-3.36.0/task/website/src/css/carbon.css`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/src/css/custom.css` & `go_task_bin-3.36.0/task/website/src/css/custom.css`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   --ifm-color-primary-light: #4CA59D;
   --ifm-color-primary-lighter: #559F98;
   --ifm-color-primary-lightest: #5D9993;
   --ifm-code-font-size: 95%;
   --docusaurus-highlighted-code-line-bg: rgba(0, 0, 0, 0.1);
 
   --ifm-navbar-link-color: #fffdf9;
-  --ifm-navbar-link-hover-color: #fffdf9;
+  --ifm-navbar-link-hover-color: #43aba2;
 }
 .menu__link--sublist.menu__link--active,
 .menu__link--sublist.menu__link--active:hover {
   background-color: #43aba2 !important;
 }
 
 [data-theme='light'] {
@@ -72,7 +72,48 @@
   display: flex;
   justify-content: center;
 }
 
 .gold-sponsors table img {
   width: 200px;
 }
+
+.menu__list-item:has(.header-icon-link) {
+  float: left;
+}
+
+.menu__list-item:has(.header-icon-link) .header-icon-link {
+  margin-top: 10px;
+}
+
+.header-icon-link::before {
+  content: '';
+  width: 24px;
+  height: 24px;
+  display: flex;
+  background-color: var(--ifm-navbar-link-color);
+  transition: background-color var(--ifm-transition-fast)
+    var(--ifm-transition-timing-default);
+  mask-size: contain;
+  mask-repeat: no-repeat;
+  mask-position: center;
+}
+
+.header-icon-link:hover::before {
+  background-color: var(--ifm-navbar-link-hover-color);
+}
+
+.icon-github::before {
+  mask-image: url('/img/icon-github.svg');
+}
+
+.icon-discord::before {
+  mask-image: url('/img/icon-discord.svg');
+}
+
+.icon-mastodon::before {
+  mask-image: url('/img/icon-mastodon.svg');
+}
+
+.icon-twitter::before {
+  mask-image: url('/img/icon-twitter.svg');
+}
```

### Comparing `go_task_bin-3.35.1/task/docs/src/themes/prismDark.js` & `go_task_bin-3.36.0/task/website/src/themes/prismDark.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/src/themes/prismLight.js` & `go_task_bin-3.36.0/task/website/src/themes/prismLight.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/static/img/appwrite.svg` & `go_task_bin-3.36.0/task/website/static/img/appwrite.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/static/img/favicon.ico` & `go_task_bin-3.36.0/task/website/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/static/img/logo.png` & `go_task_bin-3.36.0/task/website/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/static/img/og-image.png` & `go_task_bin-3.36.0/task/website/static/img/og-image.png`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/static/img/pix.png` & `go_task_bin-3.36.0/task/website/static/img/pix.png`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/static/install.sh` & `go_task_bin-3.36.0/task/install-task.sh`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/static/js/carbon.js` & `go_task_bin-3.36.0/task/website/static/js/carbon.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/docs/static/schema.json` & `go_task_bin-3.36.0/task/website/static/schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9820495854591836%*

 * *Differences: {"'definitions'": "{'task': {'properties': {'deps': {'$ref': '#/definitions/deps', delete: "*

 * *                  "['type', 'items']}}}, 'cmd': {'anyOf': {4: {'$ref': "*

 * *                  "'#/definitions/for_cmds_call'}}}, 'deps': OrderedDict([('type', 'array'), "*

 * *                  "('items', OrderedDict([('oneOf', [OrderedDict([('type', 'string')]), "*

 * *                  "OrderedDict([('$ref', '#/definitions/task_call')]), OrderedDict([('$ref', "*

 * *                  "'#/definitions/for_deps_call')])])]))]), 'for_c […]*

```diff
@@ -168,15 +168,15 @@
                 {
                     "$ref": "#/definitions/task_call"
                 },
                 {
                     "$ref": "#/definitions/defer_call"
                 },
                 {
-                    "$ref": "#/definitions/for_call"
+                    "$ref": "#/definitions/for_cmds_call"
                 }
             ]
         },
         "cmd_call": {
             "additionalProperties": false,
             "properties": {
                 "cmd": {
@@ -247,25 +247,54 @@
                 }
             },
             "required": [
                 "defer"
             ],
             "type": "object"
         },
+        "deps": {
+            "items": {
+                "oneOf": [
+                    {
+                        "type": "string"
+                    },
+                    {
+                        "$ref": "#/definitions/task_call"
+                    },
+                    {
+                        "$ref": "#/definitions/for_deps_call"
+                    }
+                ]
+            },
+            "type": "array"
+        },
         "env": {
             "$ref": "#/definitions/vars"
         },
+        "for": {
+            "anyOf": [
+                {
+                    "$ref": "#/definitions/for_list"
+                },
+                {
+                    "$ref": "#/definitions/for_attribute"
+                },
+                {
+                    "$ref": "#/definitions/for_var"
+                }
+            ]
+        },
         "for_attribute": {
             "description": "The task attribute to iterate over",
             "enum": [
                 "sources"
             ],
             "type": "string"
         },
-        "for_call": {
+        "for_cmds_call": {
             "additionalProperties": false,
             "oneOf": [
                 {
                     "required": [
                         "cmd"
                     ]
                 },
@@ -277,26 +306,52 @@
             ],
             "properties": {
                 "cmd": {
                     "description": "Command to run",
                     "type": "string"
                 },
                 "for": {
-                    "anyOf": [
-                        {
-                            "$ref": "#/definitions/for_list"
-                        },
-                        {
-                            "$ref": "#/definitions/for_attribute"
-                        },
-                        {
-                            "$ref": "#/definitions/for_var"
-                        }
+                    "$ref": "#/definitions/for"
+                },
+                "silent": {
+                    "description": "Silent mode disables echoing of command before Task runs it",
+                    "type": "boolean"
+                },
+                "task": {
+                    "description": "Task to run",
+                    "type": "string"
+                },
+                "vars": {
+                    "$ref": "#/definitions/vars",
+                    "description": "Values passed to the task called"
+                }
+            },
+            "required": [
+                "for"
+            ],
+            "type": "object"
+        },
+        "for_deps_call": {
+            "additionalProperties": false,
+            "oneOf": [
+                {
+                    "required": [
+                        "cmd"
                     ]
                 },
+                {
+                    "required": [
+                        "task"
+                    ]
+                }
+            ],
+            "properties": {
+                "for": {
+                    "$ref": "#/definitions/for"
+                },
                 "silent": {
                     "description": "Silent mode disables echoing of command before Task runs it",
                     "type": "boolean"
                 },
                 "task": {
                     "description": "Task to run",
                     "type": "string"
@@ -474,26 +529,16 @@
                     "description": "The command to be executed."
                 },
                 "cmds": {
                     "$ref": "#/definitions/cmds",
                     "description": "A list of commands to be executed."
                 },
                 "deps": {
-                    "description": "A list of dependencies of this task. Tasks defined here will run in parallel before this task.",
-                    "items": {
-                        "oneOf": [
-                            {
-                                "type": "string"
-                            },
-                            {
-                                "$ref": "#/definitions/task_call"
-                            }
-                        ]
-                    },
-                    "type": "array"
+                    "$ref": "#/definitions/deps",
+                    "description": "A list of dependencies of this task. Tasks defined here will run in parallel before this task."
                 },
                 "desc": {
                     "description": "A short description of the task. This is displayed when calling `task --list`.",
                     "type": "string"
                 },
                 "dir": {
                     "description": "The directory in which this task should run. Defaults to the current working directory.",
```

### Comparing `go_task_bin-3.35.1/task/docs/yarn.lock` & `go_task_bin-3.36.0/task/website/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -384,15 +384,15 @@
   resolved "https://registry.npmjs.org/@babel/highlight/-/highlight-7.23.4.tgz"
   integrity sha512-acGdbYSfp2WheJoJm/EBBBLh/ID8KDc64ISZ9DYtBmC8/Q204PZJLHyzeB5qMzJ5trcOkybd78M4x2KWsUq++A==
   dependencies:
     "@babel/helper-validator-identifier" "^7.22.20"
     chalk "^2.4.2"
     js-tokens "^4.0.0"
 
-"@babel/parser@^7.22.15", "@babel/parser@^7.22.7", "@babel/parser@^7.23.6":
+"@babel/parser@^7.22.15", "@babel/parser@^7.23.6":
   version "7.23.6"
   resolved "https://registry.npmjs.org/@babel/parser/-/parser-7.23.6.tgz"
   integrity sha512-Z2uID7YJ7oNvAI20O9X0bblw7Qqs8Q2hFy0R9tAfnfLkp5MW0UH9eUvnDSnFwKZ0AvgS1ucqR4KzvVHgnke1VQ==
 
 "@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression@^7.23.3":
   version "7.23.3"
   resolved "https://registry.npmjs.org/@babel/plugin-bugfix-safari-id-destructuring-collision-in-function-expression/-/plugin-bugfix-safari-id-destructuring-collision-in-function-expression-7.23.3.tgz"
@@ -1141,21 +1141,28 @@
   version "7.23.6"
   resolved "https://registry.npmjs.org/@babel/runtime-corejs3/-/runtime-corejs3-7.23.6.tgz"
   integrity sha512-Djs/ZTAnpyj0nyg7p1J6oiE/tZ9G2stqAFlLGZynrW+F3k2w2jGK2mLOBxzYIOcZYA89+c3d3wXKpYLcpwcU6w==
   dependencies:
     core-js-pure "^3.30.2"
     regenerator-runtime "^0.14.0"
 
-"@babel/runtime@^7.1.2", "@babel/runtime@^7.10.3", "@babel/runtime@^7.12.13", "@babel/runtime@^7.12.5", "@babel/runtime@^7.22.6", "@babel/runtime@^7.8.4":
+"@babel/runtime@^7.1.2", "@babel/runtime@^7.10.3", "@babel/runtime@^7.12.13", "@babel/runtime@^7.22.6", "@babel/runtime@^7.8.4":
   version "7.23.6"
   resolved "https://registry.npmjs.org/@babel/runtime/-/runtime-7.23.6.tgz"
   integrity sha512-zHd0eUrf5GZoOWVCXp6koAKQTfZV07eit6bGPmJgnZdnSAvvZee6zniW2XMF7Cmc4ISOOnPy3QaSiIJGJkVEDQ==
   dependencies:
     regenerator-runtime "^0.14.0"
 
+"@babel/runtime@^7.12.5":
+  version "7.24.4"
+  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.24.4.tgz#de795accd698007a66ba44add6cc86542aff1edd"
+  integrity sha512-dkxf7+hn8mFBwKjs9bvBlArzLVxVbS8usaPUDd5p2a9JCL9tB8OaOVN1isD4+Xyk4ns89/xeOmbQvgdK7IIVdA==
+  dependencies:
+    regenerator-runtime "^0.14.0"
+
 "@babel/template@^7.22.15":
   version "7.22.15"
   resolved "https://registry.npmjs.org/@babel/template/-/template-7.22.15.tgz"
   integrity sha512-QPErUVm4uyJa60rkI73qneDacvdvzxshT3kksGqlGWYdOTIUOwJ7RDUL8sGqslY1uXWSL6xMFKEXDS3ox2uF0w==
   dependencies:
     "@babel/code-frame" "^7.22.13"
     "@babel/parser" "^7.22.15"
@@ -1187,29 +1194,29 @@
     to-fast-properties "^2.0.0"
 
 "@colors/colors@1.5.0":
   version "1.5.0"
   resolved "https://registry.npmjs.org/@colors/colors/-/colors-1.5.0.tgz"
   integrity sha512-ooWCrlZP11i8GImSjTHYHLkvFDP48nS4+204nGb1RiX/WXYHmJA2III9/e2DWVabCESdW7hBAEzHRqUn9OUVvQ==
 
-"@crowdin/cli@^3.10.1":
-  version "3.10.1"
-  resolved "https://registry.npmjs.org/@crowdin/cli/-/cli-3.10.1.tgz"
-  integrity sha512-CBzABy2voC+T1KpgQYI1DIBGANahG9Vuwiqp0GJERVAWhqp1Tveie3N2rCkzjZT8N8E5SHp/z+OpstrdZYOA+g==
+"@crowdin/cli@^3.19.2":
+  version "3.19.2"
+  resolved "https://registry.yarnpkg.com/@crowdin/cli/-/cli-3.19.2.tgz#d81d85c78d7235c6c273bae72c93631dc0aedab6"
+  integrity sha512-eO/BFcLl2m96dRlEth3hsbbPJNsiTZaLqsAkot27eE4DS5+IpkV0NbcBgMsja+t0ugPAPYQ7Crc+AruO5ywvmg==
   dependencies:
     command-exists-promise "^2.0.2"
-    node-fetch "2.6.7"
-    shelljs "^0.8.4"
-    tar "^4.4.8"
-    yauzl "^2.10.0"
-
-"@crowdin/crowdin-api-client@^1.22.1":
-  version "1.22.1"
-  resolved "https://registry.npmjs.org/@crowdin/crowdin-api-client/-/crowdin-api-client-1.22.1.tgz"
-  integrity sha512-2T4JWuatKBpdb8zYUd0HmXjOD3HCCd7I6LKWG7ZEVid9+JAXItjB8+xLL+AupYJM8iHflnZjggs/wadQZovOuA==
+    node-fetch "2.7.0"
+    shelljs "^0.8.5"
+    tar "^6.2.0"
+    yauzl "^3.1.0"
+
+"@crowdin/crowdin-api-client@^1.33.0":
+  version "1.33.0"
+  resolved "https://registry.yarnpkg.com/@crowdin/crowdin-api-client/-/crowdin-api-client-1.33.0.tgz#35211b3b9b69b52b5681ab2d761d6f877f13b6f7"
+  integrity sha512-A8KFGwxRLKKqZEQAM3BAE6XZuuOmvRtNKhcG6bhEbqDMpdEeeR1un3iDXrQALUFfddMAZ5QK5saIkCdEl7nSYA==
   dependencies:
     axios "^1"
 
 "@discoveryjs/json-ext@0.5.7":
   version "0.5.7"
   resolved "https://registry.npmjs.org/@discoveryjs/json-ext/-/json-ext-0.5.7.tgz"
   integrity sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==
@@ -1225,37 +1232,36 @@
   integrity sha512-9Ahcrs5z2jq/DcAvYtvlqEBHImbm4YJI8M9y0x6Tqg598P40HTEkX7hsMcIuThI+hTFxRGZ9hll0Wygm2yEjng==
   dependencies:
     "@algolia/autocomplete-core" "1.9.3"
     "@algolia/autocomplete-preset-algolia" "1.9.3"
     "@docsearch/css" "3.5.2"
     algoliasearch "^4.19.1"
 
-"@docusaurus/core@3.0.1", "@docusaurus/core@^3.0.1":
-  version "3.0.1"
-  resolved "https://registry.yarnpkg.com/@docusaurus/core/-/core-3.0.1.tgz#ad9a66b20802ea81b25e65db75d4ca952eda7e01"
-  integrity sha512-CXrLpOnW+dJdSv8M5FAJ3JBwXtL6mhUWxFA8aS0ozK6jBG/wgxERk5uvH28fCeFxOGbAT9v1e9dOMo1X2IEVhQ==
+"@docusaurus/core@3.2.0", "@docusaurus/core@^3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/core/-/core-3.2.0.tgz#10acb993fb76960890d1aa43025245aaa8dcdbbb"
+  integrity sha512-WTO6vW4404nhTmK9NL+95nd13I1JveFwZ8iOBYxb4xt+N2S3KzY+mm+1YtWw2vV37FbYfH+w+KrlrRaWuy5Hzw==
   dependencies:
     "@babel/core" "^7.23.3"
     "@babel/generator" "^7.23.3"
     "@babel/plugin-syntax-dynamic-import" "^7.8.3"
     "@babel/plugin-transform-runtime" "^7.22.9"
     "@babel/preset-env" "^7.22.9"
     "@babel/preset-react" "^7.22.5"
     "@babel/preset-typescript" "^7.22.5"
     "@babel/runtime" "^7.22.6"
     "@babel/runtime-corejs3" "^7.22.6"
     "@babel/traverse" "^7.22.8"
-    "@docusaurus/cssnano-preset" "3.0.1"
-    "@docusaurus/logger" "3.0.1"
-    "@docusaurus/mdx-loader" "3.0.1"
+    "@docusaurus/cssnano-preset" "3.2.0"
+    "@docusaurus/logger" "3.2.0"
+    "@docusaurus/mdx-loader" "3.2.0"
     "@docusaurus/react-loadable" "5.5.2"
-    "@docusaurus/utils" "3.0.1"
-    "@docusaurus/utils-common" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
-    "@slorber/static-site-generator-webpack-plugin" "^4.0.7"
+    "@docusaurus/utils" "3.2.0"
+    "@docusaurus/utils-common" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     "@svgr/webpack" "^6.5.1"
     autoprefixer "^10.4.14"
     babel-loader "^9.1.3"
     babel-plugin-dynamic-import-node "^2.3.3"
     boxen "^6.2.1"
     chalk "^4.1.2"
     chokidar "^3.5.3"
@@ -1268,22 +1274,24 @@
     css-loader "^6.8.1"
     css-minimizer-webpack-plugin "^4.2.2"
     cssnano "^5.1.15"
     del "^6.1.1"
     detect-port "^1.5.1"
     escape-html "^1.0.3"
     eta "^2.2.0"
+    eval "^0.1.8"
     file-loader "^6.2.0"
     fs-extra "^11.1.1"
     html-minifier-terser "^7.2.0"
     html-tags "^3.3.1"
     html-webpack-plugin "^5.5.3"
     leven "^3.1.0"
     lodash "^4.17.21"
     mini-css-extract-plugin "^2.7.6"
+    p-map "^4.0.0"
     postcss "^8.4.26"
     postcss-loader "^7.3.3"
     prompts "^2.4.2"
     react-dev-utils "^12.0.1"
     react-helmet-async "^1.3.0"
     react-loadable "npm:@docusaurus/react-loadable@5.5.2"
     react-loadable-ssr-addon-v5-slorber "^1.0.1"
@@ -1300,42 +1308,40 @@
     url-loader "^4.1.1"
     webpack "^5.88.1"
     webpack-bundle-analyzer "^4.9.0"
     webpack-dev-server "^4.15.1"
     webpack-merge "^5.9.0"
     webpackbar "^5.0.2"
 
-"@docusaurus/cssnano-preset@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/cssnano-preset/-/cssnano-preset-3.0.1.tgz"
-  integrity sha512-wjuXzkHMW+ig4BD6Ya1Yevx9UJadO4smNZCEljqBoQfIQrQskTswBs7lZ8InHP7mCt273a/y/rm36EZhqJhknQ==
+"@docusaurus/cssnano-preset@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/cssnano-preset/-/cssnano-preset-3.2.0.tgz#0e0fbf19873a726f92e670b9d511e9f2828d6097"
+  integrity sha512-H88RXGUia7r/VF3XfyoA4kbwgpUZcKsObF6VvwBOP91EdArTf6lnHbJ/x8Ca79KS/zf98qaWyBGzW+5ez58Iyw==
   dependencies:
     cssnano-preset-advanced "^5.3.10"
     postcss "^8.4.26"
     postcss-sort-media-queries "^4.4.1"
     tslib "^2.6.0"
 
-"@docusaurus/logger@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/logger/-/logger-3.0.1.tgz"
-  integrity sha512-I5L6Nk8OJzkVA91O2uftmo71LBSxe1vmOn9AMR6JRCzYeEBrqneWMH02AqMvjJ2NpMiviO+t0CyPjyYV7nxCWQ==
+"@docusaurus/logger@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/logger/-/logger-3.2.0.tgz#99d2b09478bcba69c964ec0c8600d855fb8e9e0f"
+  integrity sha512-Z1R1NcOGXZ8CkIJSvjvyxnuDDSlx/+1xlh20iVTw1DZRjonFmI3T3tTgk40YpXyWUYQpIgAoqqPMpuseMMdgRQ==
   dependencies:
     chalk "^4.1.2"
     tslib "^2.6.0"
 
-"@docusaurus/mdx-loader@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/mdx-loader/-/mdx-loader-3.0.1.tgz"
-  integrity sha512-ldnTmvnvlrONUq45oKESrpy+lXtbnTcTsFkOTIDswe5xx5iWJjt6eSa0f99ZaWlnm24mlojcIGoUWNCS53qVlQ==
+"@docusaurus/mdx-loader@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/mdx-loader/-/mdx-loader-3.2.0.tgz#d17f17ae1bb38255643c82705dda719b23c27831"
+  integrity sha512-JtkI5o6R/rJSr1Y23cHKz085aBJCvJw3AYHihJ7r+mBX+O8EuQIynG0e6/XpbSCpr7Ino0U50UtxaXcEbFwg9Q==
   dependencies:
-    "@babel/parser" "^7.22.7"
-    "@babel/traverse" "^7.22.8"
-    "@docusaurus/logger" "3.0.1"
-    "@docusaurus/utils" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
+    "@docusaurus/logger" "3.2.0"
+    "@docusaurus/utils" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     "@mdx-js/mdx" "^3.0.0"
     "@slorber/remark-comment" "^1.0.0"
     escape-html "^1.0.3"
     estree-util-value-to-estree "^3.0.1"
     file-loader "^6.2.0"
     fs-extra "^11.1.1"
     image-size "^1.0.2"
@@ -1350,321 +1356,326 @@
     tslib "^2.6.0"
     unified "^11.0.3"
     unist-util-visit "^5.0.0"
     url-loader "^4.1.1"
     vfile "^6.0.1"
     webpack "^5.88.1"
 
-"@docusaurus/module-type-aliases@3.0.1", "@docusaurus/module-type-aliases@^3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/module-type-aliases/-/module-type-aliases-3.0.1.tgz"
-  integrity sha512-DEHpeqUDsLynl3AhQQiO7AbC7/z/lBra34jTcdYuvp9eGm01pfH1wTVq8YqWZq6Jyx0BgcVl/VJqtE9StRd9Ag==
+"@docusaurus/module-type-aliases@3.2.0", "@docusaurus/module-type-aliases@^3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/module-type-aliases/-/module-type-aliases-3.2.0.tgz#ef883d8418f37e551eca72adc409014e720786d4"
+  integrity sha512-jRSp9YkvBwwNz6Xgy0RJPsnie+Ebb//gy7GdbkJ2pW2gvvlYKGib2+jSF0pfIzvyZLulfCynS1KQdvDKdSl8zQ==
   dependencies:
     "@docusaurus/react-loadable" "5.5.2"
-    "@docusaurus/types" "3.0.1"
+    "@docusaurus/types" "3.2.0"
     "@types/history" "^4.7.11"
     "@types/react" "*"
     "@types/react-router-config" "*"
     "@types/react-router-dom" "*"
     react-helmet-async "*"
     react-loadable "npm:@docusaurus/react-loadable@5.5.2"
 
-"@docusaurus/plugin-content-blog@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/plugin-content-blog/-/plugin-content-blog-3.0.1.tgz"
-  integrity sha512-cLOvtvAyaMQFLI8vm4j26svg3ktxMPSXpuUJ7EERKoGbfpJSsgtowNHcRsaBVmfuCsRSk1HZ/yHBsUkTmHFEsg==
+"@docusaurus/plugin-content-blog@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/plugin-content-blog/-/plugin-content-blog-3.2.0.tgz#b7b43e71634272a80a9532dc166731332391cb4b"
+  integrity sha512-MABqwjSicyHmYEfQueMthPCz18JkVxhK3EGhXTSRWwReAZ0UTuw9pG6+Wo+uXAugDaIcJH28rVZSwTDINPm2bw==
   dependencies:
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/logger" "3.0.1"
-    "@docusaurus/mdx-loader" "3.0.1"
-    "@docusaurus/types" "3.0.1"
-    "@docusaurus/utils" "3.0.1"
-    "@docusaurus/utils-common" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/logger" "3.2.0"
+    "@docusaurus/mdx-loader" "3.2.0"
+    "@docusaurus/types" "3.2.0"
+    "@docusaurus/utils" "3.2.0"
+    "@docusaurus/utils-common" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     cheerio "^1.0.0-rc.12"
     feed "^4.2.2"
     fs-extra "^11.1.1"
     lodash "^4.17.21"
     reading-time "^1.5.0"
     srcset "^4.0.0"
     tslib "^2.6.0"
     unist-util-visit "^5.0.0"
     utility-types "^3.10.0"
     webpack "^5.88.1"
 
-"@docusaurus/plugin-content-docs@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/plugin-content-docs/-/plugin-content-docs-3.0.1.tgz"
-  integrity sha512-dRfAOA5Ivo+sdzzJGXEu33yAtvGg8dlZkvt/NEJ7nwi1F2j4LEdsxtfX2GKeETB2fP6XoGNSQnFXqa2NYGrHFg==
+"@docusaurus/plugin-content-docs@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/plugin-content-docs/-/plugin-content-docs-3.2.0.tgz#6e4f727a0cce301b9d9361bf41ca6a978fe79475"
+  integrity sha512-uuqhahmsBnirxOz+SXksnWt7+wc+iN4ntxNRH48BUgo7QRNLATWjHCgI8t6zrMJxK4o+QL9DhLaPDlFHs91B3Q==
   dependencies:
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/logger" "3.0.1"
-    "@docusaurus/mdx-loader" "3.0.1"
-    "@docusaurus/module-type-aliases" "3.0.1"
-    "@docusaurus/types" "3.0.1"
-    "@docusaurus/utils" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/logger" "3.2.0"
+    "@docusaurus/mdx-loader" "3.2.0"
+    "@docusaurus/module-type-aliases" "3.2.0"
+    "@docusaurus/types" "3.2.0"
+    "@docusaurus/utils" "3.2.0"
+    "@docusaurus/utils-common" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     "@types/react-router-config" "^5.0.7"
     combine-promises "^1.1.0"
     fs-extra "^11.1.1"
     js-yaml "^4.1.0"
     lodash "^4.17.21"
     tslib "^2.6.0"
     utility-types "^3.10.0"
     webpack "^5.88.1"
 
-"@docusaurus/plugin-content-pages@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/plugin-content-pages/-/plugin-content-pages-3.0.1.tgz"
-  integrity sha512-oP7PoYizKAXyEttcvVzfX3OoBIXEmXTMzCdfmC4oSwjG4SPcJsRge3mmI6O8jcZBgUPjIzXD21bVGWEE1iu8gg==
+"@docusaurus/plugin-content-pages@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/plugin-content-pages/-/plugin-content-pages-3.2.0.tgz#df28a6ee6b52c4b292a726f29f39b119756caf44"
+  integrity sha512-4ofAN7JDsdb4tODO9OIrizWY5DmEJXr0eu+UDIkLqGP+gXXTahJZv8h2mlxO+lPXGXRCVBOfA14OG1hOYJVPwA==
   dependencies:
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/mdx-loader" "3.0.1"
-    "@docusaurus/types" "3.0.1"
-    "@docusaurus/utils" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/mdx-loader" "3.2.0"
+    "@docusaurus/types" "3.2.0"
+    "@docusaurus/utils" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     fs-extra "^11.1.1"
     tslib "^2.6.0"
     webpack "^5.88.1"
 
-"@docusaurus/plugin-debug@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/plugin-debug/-/plugin-debug-3.0.1.tgz"
-  integrity sha512-09dxZMdATky4qdsZGzhzlUvvC+ilQ2hKbYF+wez+cM2mGo4qHbv8+qKXqxq0CQZyimwlAOWQLoSozIXU0g0i7g==
+"@docusaurus/plugin-debug@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/plugin-debug/-/plugin-debug-3.2.0.tgz#643d13d403685c2b9bdb3b65bec8050847b920a3"
+  integrity sha512-p6WxtO5XZGz66y6QNQtCJwBefq4S6/w75XaXVvH1/2P9uaijvF7R+Cm2EWQZ5WsvA5wl//DFWblyDHRyVC207Q==
   dependencies:
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/types" "3.0.1"
-    "@docusaurus/utils" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/types" "3.2.0"
+    "@docusaurus/utils" "3.2.0"
     fs-extra "^11.1.1"
     react-json-view-lite "^1.2.0"
     tslib "^2.6.0"
 
-"@docusaurus/plugin-google-analytics@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/plugin-google-analytics/-/plugin-google-analytics-3.0.1.tgz"
-  integrity sha512-jwseSz1E+g9rXQwDdr0ZdYNjn8leZBnKPjjQhMBEiwDoenL3JYFcNW0+p0sWoVF/f2z5t7HkKA+cYObrUh18gg==
+"@docusaurus/plugin-google-analytics@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/plugin-google-analytics/-/plugin-google-analytics-3.2.0.tgz#770151947c0ee49500586e9200631852ab97e23a"
+  integrity sha512-//TepJTEyAZSvBwHKEbXHu9xT/VkK3wUil2ZakKvQZYfUC01uWn6A1E3toa8R7WhCy1xPUeIukqmJy1Clg8njQ==
   dependencies:
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/types" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/types" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     tslib "^2.6.0"
 
-"@docusaurus/plugin-google-gtag@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/plugin-google-gtag/-/plugin-google-gtag-3.0.1.tgz"
-  integrity sha512-UFTDvXniAWrajsulKUJ1DB6qplui1BlKLQZjX4F7qS/qfJ+qkKqSkhJ/F4VuGQ2JYeZstYb+KaUzUzvaPK1aRQ==
+"@docusaurus/plugin-google-gtag@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/plugin-google-gtag/-/plugin-google-gtag-3.2.0.tgz#65fc7ddc242185c3a10e60308471564075229406"
+  integrity sha512-3s6zxlaMMb87MW2Rxy6EnSRDs0WDEQPuHilZZH402C8kOrUnIwlhlfjWZ4ZyLDziGl/Eec/DvD0PVqj0qHRomA==
   dependencies:
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/types" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/types" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     "@types/gtag.js" "^0.0.12"
     tslib "^2.6.0"
 
-"@docusaurus/plugin-google-tag-manager@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/plugin-google-tag-manager/-/plugin-google-tag-manager-3.0.1.tgz"
-  integrity sha512-IPFvuz83aFuheZcWpTlAdiiX1RqWIHM+OH8wS66JgwAKOiQMR3+nLywGjkLV4bp52x7nCnwhNk1rE85Cpy/CIw==
+"@docusaurus/plugin-google-tag-manager@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/plugin-google-tag-manager/-/plugin-google-tag-manager-3.2.0.tgz#730c28a43ff5073f595509c6cb77ce4311a2e369"
+  integrity sha512-rAKtsJ11vPHA7dTAqWCgyIy7AyFRF/lpI77Zd/4HKgqcIvIayVBvL3QtelhUazfYTLTH6ls6kQ9wjMcIFxRiGg==
   dependencies:
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/types" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/types" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     tslib "^2.6.0"
 
-"@docusaurus/plugin-sitemap@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/plugin-sitemap/-/plugin-sitemap-3.0.1.tgz"
-  integrity sha512-xARiWnjtVvoEniZudlCq5T9ifnhCu/GAZ5nA7XgyLfPcNpHQa241HZdsTlLtVcecEVVdllevBKOp7qknBBaMGw==
+"@docusaurus/plugin-sitemap@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/plugin-sitemap/-/plugin-sitemap-3.2.0.tgz#cae7c92a8631072fff39dd5caf5ea7608c795540"
+  integrity sha512-gnWDFt6MStjLkdtt63Lzc+14EPSd8B6mzJGJp9GQMvWDUoMAUijUqpVIHYQq+DPMcI4PJZ5I2nsl5XFf1vOldA==
   dependencies:
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/logger" "3.0.1"
-    "@docusaurus/types" "3.0.1"
-    "@docusaurus/utils" "3.0.1"
-    "@docusaurus/utils-common" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/logger" "3.2.0"
+    "@docusaurus/types" "3.2.0"
+    "@docusaurus/utils" "3.2.0"
+    "@docusaurus/utils-common" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     fs-extra "^11.1.1"
     sitemap "^7.1.1"
     tslib "^2.6.0"
 
-"@docusaurus/preset-classic@^3.0.1":
-  version "3.0.1"
-  resolved "https://registry.yarnpkg.com/@docusaurus/preset-classic/-/preset-classic-3.0.1.tgz#d363ac837bba967095ed2a896d13c54f3717d6b5"
-  integrity sha512-il9m9xZKKjoXn6h0cRcdnt6wce0Pv1y5t4xk2Wx7zBGhKG1idu4IFHtikHlD0QPuZ9fizpXspXcTzjL5FXc1Gw==
+"@docusaurus/preset-classic@^3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/preset-classic/-/preset-classic-3.2.0.tgz#f64d970eace76c61e4f1b4b7d85d9f69d4a2dd0e"
+  integrity sha512-t7tXyk8kUgT7hUqEOgSJnPs+Foem9ucuan/a9QVYaVFCDjp92Sb2FpCY8bVasAokYCjodYe2LfpAoSCj5YDYWg==
   dependencies:
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/plugin-content-blog" "3.0.1"
-    "@docusaurus/plugin-content-docs" "3.0.1"
-    "@docusaurus/plugin-content-pages" "3.0.1"
-    "@docusaurus/plugin-debug" "3.0.1"
-    "@docusaurus/plugin-google-analytics" "3.0.1"
-    "@docusaurus/plugin-google-gtag" "3.0.1"
-    "@docusaurus/plugin-google-tag-manager" "3.0.1"
-    "@docusaurus/plugin-sitemap" "3.0.1"
-    "@docusaurus/theme-classic" "3.0.1"
-    "@docusaurus/theme-common" "3.0.1"
-    "@docusaurus/theme-search-algolia" "3.0.1"
-    "@docusaurus/types" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/plugin-content-blog" "3.2.0"
+    "@docusaurus/plugin-content-docs" "3.2.0"
+    "@docusaurus/plugin-content-pages" "3.2.0"
+    "@docusaurus/plugin-debug" "3.2.0"
+    "@docusaurus/plugin-google-analytics" "3.2.0"
+    "@docusaurus/plugin-google-gtag" "3.2.0"
+    "@docusaurus/plugin-google-tag-manager" "3.2.0"
+    "@docusaurus/plugin-sitemap" "3.2.0"
+    "@docusaurus/theme-classic" "3.2.0"
+    "@docusaurus/theme-common" "3.2.0"
+    "@docusaurus/theme-search-algolia" "3.2.0"
+    "@docusaurus/types" "3.2.0"
 
 "@docusaurus/react-loadable@5.5.2", "react-loadable@npm:@docusaurus/react-loadable@5.5.2":
   version "5.5.2"
   resolved "https://registry.npmjs.org/@docusaurus/react-loadable/-/react-loadable-5.5.2.tgz"
   integrity sha512-A3dYjdBGuy0IGT+wyLIGIKLRE+sAk1iNk0f1HjNDysO7u8lhL4N3VEm+FAubmJbAztn94F7MxBTPmnixbiyFdQ==
   dependencies:
     "@types/react" "*"
     prop-types "^15.6.2"
 
-"@docusaurus/theme-classic@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/theme-classic/-/theme-classic-3.0.1.tgz"
-  integrity sha512-XD1FRXaJiDlmYaiHHdm27PNhhPboUah9rqIH0lMpBt5kYtsGjJzhqa27KuZvHLzOP2OEpqd2+GZ5b6YPq7Q05Q==
+"@docusaurus/theme-classic@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/theme-classic/-/theme-classic-3.2.0.tgz#4aa229f1a4b1b4c138a5c80089f1d8146f56252c"
+  integrity sha512-4oSO5BQOJ5ja7WYdL6jK1n4J96tp+VJHamdwao6Ea252sA3W3vvR0otTflG4p4XVjNZH6hlPQoi5lKW0HeRgfQ==
   dependencies:
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/mdx-loader" "3.0.1"
-    "@docusaurus/module-type-aliases" "3.0.1"
-    "@docusaurus/plugin-content-blog" "3.0.1"
-    "@docusaurus/plugin-content-docs" "3.0.1"
-    "@docusaurus/plugin-content-pages" "3.0.1"
-    "@docusaurus/theme-common" "3.0.1"
-    "@docusaurus/theme-translations" "3.0.1"
-    "@docusaurus/types" "3.0.1"
-    "@docusaurus/utils" "3.0.1"
-    "@docusaurus/utils-common" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/mdx-loader" "3.2.0"
+    "@docusaurus/module-type-aliases" "3.2.0"
+    "@docusaurus/plugin-content-blog" "3.2.0"
+    "@docusaurus/plugin-content-docs" "3.2.0"
+    "@docusaurus/plugin-content-pages" "3.2.0"
+    "@docusaurus/theme-common" "3.2.0"
+    "@docusaurus/theme-translations" "3.2.0"
+    "@docusaurus/types" "3.2.0"
+    "@docusaurus/utils" "3.2.0"
+    "@docusaurus/utils-common" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     "@mdx-js/react" "^3.0.0"
     clsx "^2.0.0"
     copy-text-to-clipboard "^3.2.0"
     infima "0.2.0-alpha.43"
     lodash "^4.17.21"
     nprogress "^0.2.0"
     postcss "^8.4.26"
     prism-react-renderer "^2.3.0"
     prismjs "^1.29.0"
     react-router-dom "^5.3.4"
     rtlcss "^4.1.0"
     tslib "^2.6.0"
     utility-types "^3.10.0"
 
-"@docusaurus/theme-common@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/theme-common/-/theme-common-3.0.1.tgz"
-  integrity sha512-cr9TOWXuIOL0PUfuXv6L5lPlTgaphKP+22NdVBOYah5jSq5XAAulJTjfe+IfLsEG4L7lJttLbhW7LXDFSAI7Ag==
+"@docusaurus/theme-common@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/theme-common/-/theme-common-3.2.0.tgz#67f5f1a1e265e1f1a5b9fa7bfb4bf7b98dfcf981"
+  integrity sha512-sFbw9XviNJJ+760kAcZCQMQ3jkNIznGqa6MQ70E5BnbP+ja36kGgPOfjcsvAcNey1H1Rkhh3p2Mhf4HVLdKVVw==
   dependencies:
-    "@docusaurus/mdx-loader" "3.0.1"
-    "@docusaurus/module-type-aliases" "3.0.1"
-    "@docusaurus/plugin-content-blog" "3.0.1"
-    "@docusaurus/plugin-content-docs" "3.0.1"
-    "@docusaurus/plugin-content-pages" "3.0.1"
-    "@docusaurus/utils" "3.0.1"
-    "@docusaurus/utils-common" "3.0.1"
+    "@docusaurus/mdx-loader" "3.2.0"
+    "@docusaurus/module-type-aliases" "3.2.0"
+    "@docusaurus/plugin-content-blog" "3.2.0"
+    "@docusaurus/plugin-content-docs" "3.2.0"
+    "@docusaurus/plugin-content-pages" "3.2.0"
+    "@docusaurus/utils" "3.2.0"
+    "@docusaurus/utils-common" "3.2.0"
     "@types/history" "^4.7.11"
     "@types/react" "*"
     "@types/react-router-config" "*"
     clsx "^2.0.0"
     parse-numeric-range "^1.3.0"
     prism-react-renderer "^2.3.0"
     tslib "^2.6.0"
     utility-types "^3.10.0"
 
-"@docusaurus/theme-search-algolia@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/theme-search-algolia/-/theme-search-algolia-3.0.1.tgz"
-  integrity sha512-DDiPc0/xmKSEdwFkXNf1/vH1SzJPzuJBar8kMcBbDAZk/SAmo/4lf6GU2drou4Ae60lN2waix+jYWTWcJRahSA==
+"@docusaurus/theme-search-algolia@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/theme-search-algolia/-/theme-search-algolia-3.2.0.tgz#05338b37753dd13899fb0296f2c57130e9893dbf"
+  integrity sha512-PgvF4qHoqJp8+GfqClUbTF/zYNOsz4De251IuzXon7+7FAXwvb2qmYtA2nEwyMbB7faKOz33Pxzv+y+153KS/g==
   dependencies:
     "@docsearch/react" "^3.5.2"
-    "@docusaurus/core" "3.0.1"
-    "@docusaurus/logger" "3.0.1"
-    "@docusaurus/plugin-content-docs" "3.0.1"
-    "@docusaurus/theme-common" "3.0.1"
-    "@docusaurus/theme-translations" "3.0.1"
-    "@docusaurus/utils" "3.0.1"
-    "@docusaurus/utils-validation" "3.0.1"
+    "@docusaurus/core" "3.2.0"
+    "@docusaurus/logger" "3.2.0"
+    "@docusaurus/plugin-content-docs" "3.2.0"
+    "@docusaurus/theme-common" "3.2.0"
+    "@docusaurus/theme-translations" "3.2.0"
+    "@docusaurus/utils" "3.2.0"
+    "@docusaurus/utils-validation" "3.2.0"
     algoliasearch "^4.18.0"
     algoliasearch-helper "^3.13.3"
     clsx "^2.0.0"
     eta "^2.2.0"
     fs-extra "^11.1.1"
     lodash "^4.17.21"
     tslib "^2.6.0"
     utility-types "^3.10.0"
 
-"@docusaurus/theme-translations@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/theme-translations/-/theme-translations-3.0.1.tgz"
-  integrity sha512-6UrbpzCTN6NIJnAtZ6Ne9492vmPVX+7Fsz4kmp+yor3KQwA1+MCzQP7ItDNkP38UmVLnvB/cYk/IvehCUqS3dg==
+"@docusaurus/theme-translations@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/theme-translations/-/theme-translations-3.2.0.tgz#02a0e9bd0ed8cebc21a2f1e5b6d252b0e5ee39a9"
+  integrity sha512-VXzZJBuyVEmwUYyud+7IgJQEBRM6R2u/s10Rp3DOP19CBQxeKgHYTKkKhFtDeKMHDassb665kjgOi0YlJfUT6w==
   dependencies:
     fs-extra "^11.1.1"
     tslib "^2.6.0"
 
-"@docusaurus/tsconfig@^3.0.1":
-  version "3.0.1"
-  resolved "https://registry.yarnpkg.com/@docusaurus/tsconfig/-/tsconfig-3.0.1.tgz#170f230c34ff12e55995bd7e9f1f21db33035d8f"
-  integrity sha512-hT2HCdNE3pWTzXV/7cSsowfmaOxXVOTFOXmkqaYjBWjaxjJ3FO0nHbdJ8rF6Da7PvWmIPbUekdP5gep1XCJ7Vg==
+"@docusaurus/tsconfig@^3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/tsconfig/-/tsconfig-3.2.0.tgz#19160b8beda905bcf26a56d786608cc9dc3900e8"
+  integrity sha512-gWGa/72TYRxSRRxGFU2G6Au0yif6zmbkAgzW3+SeXAxoq1a7OLytMLGEwaHjMoIRXl7WbThnpx4gZVwo0xRRAg==
 
-"@docusaurus/types@3.0.1", "@docusaurus/types@^3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/types/-/types-3.0.1.tgz"
-  integrity sha512-plyX2iU1tcUsF46uQ01pAd4JhexR7n0iiQ5MSnBFX6M6NSJgDYdru/i1/YNPKOnQHBoXGLHv0dNT6OAlDWNjrg==
+"@docusaurus/types@3.2.0", "@docusaurus/types@^3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/types/-/types-3.2.0.tgz#c5bfd000ad4f72e9a7e6beff79905f9ea165fcd3"
+  integrity sha512-uG3FfTkkkbZIPPNYx6xRfZHKeGyRd/inIT1cqvYt1FobFLd+7WhRXrSBqwJ9JajJjEAjNioRMVFgGofGf/Wdww==
   dependencies:
+    "@mdx-js/mdx" "^3.0.0"
     "@types/history" "^4.7.11"
     "@types/react" "*"
     commander "^5.1.0"
     joi "^17.9.2"
     react-helmet-async "^1.3.0"
     utility-types "^3.10.0"
     webpack "^5.88.1"
     webpack-merge "^5.9.0"
 
-"@docusaurus/utils-common@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/utils-common/-/utils-common-3.0.1.tgz"
-  integrity sha512-W0AxD6w6T8g6bNro8nBRWf7PeZ/nn7geEWM335qHU2DDDjHuV4UZjgUGP1AQsdcSikPrlIqTJJbKzer1lRSlIg==
+"@docusaurus/utils-common@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/utils-common/-/utils-common-3.2.0.tgz#6163a2c415d150d6df73a8aceec6004f0ba3bb06"
+  integrity sha512-WEQT5L2lT/tBQgDRgeZQAIi9YJBrwEILb1BuObQn1St3T/4K1gx5fWwOT8qdLOov296XLd1FQg9Ywu27aE9svw==
   dependencies:
     tslib "^2.6.0"
 
-"@docusaurus/utils-validation@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/utils-validation/-/utils-validation-3.0.1.tgz"
-  integrity sha512-ujTnqSfyGQ7/4iZdB4RRuHKY/Nwm58IIb+41s5tCXOv/MBU2wGAjOHq3U+AEyJ8aKQcHbxvTKJaRchNHYUVUQg==
+"@docusaurus/utils-validation@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/utils-validation/-/utils-validation-3.2.0.tgz#b53463d9dc6eb335a2ad93ed4b3c397162533e6d"
+  integrity sha512-rCzMTqwNrBrEOyU8EaD1fYWdig4TDhfj+YLqB8DY68VUAqSIgbY+yshpqFKB0bznFYNBJbn0bGpvVuImQOa/vA==
   dependencies:
-    "@docusaurus/logger" "3.0.1"
-    "@docusaurus/utils" "3.0.1"
+    "@docusaurus/logger" "3.2.0"
+    "@docusaurus/utils" "3.2.0"
+    "@docusaurus/utils-common" "3.2.0"
     joi "^17.9.2"
     js-yaml "^4.1.0"
     tslib "^2.6.0"
 
-"@docusaurus/utils@3.0.1":
-  version "3.0.1"
-  resolved "https://registry.npmjs.org/@docusaurus/utils/-/utils-3.0.1.tgz"
-  integrity sha512-TwZ33Am0q4IIbvjhUOs+zpjtD/mXNmLmEgeTGuRq01QzulLHuPhaBTTAC/DHu6kFx3wDgmgpAlaRuCHfTcXv8g==
+"@docusaurus/utils@3.2.0":
+  version "3.2.0"
+  resolved "https://registry.yarnpkg.com/@docusaurus/utils/-/utils-3.2.0.tgz#1312221d224eb2cbaaaf53d24efca3e1e976db3e"
+  integrity sha512-3rgrE7iL60yV2JQivlcoxUNNTK2APmn+OHLUmTvX2pueIM8DEOCEFHpJO4MiWjFO7V/Wq3iA/W1M03JnjdugVw==
   dependencies:
-    "@docusaurus/logger" "3.0.1"
+    "@docusaurus/logger" "3.2.0"
+    "@docusaurus/utils-common" "3.2.0"
     "@svgr/webpack" "^6.5.1"
     escape-string-regexp "^4.0.0"
     file-loader "^6.2.0"
     fs-extra "^11.1.1"
     github-slugger "^1.5.0"
     globby "^11.1.0"
     gray-matter "^4.0.3"
     jiti "^1.20.0"
     js-yaml "^4.1.0"
     lodash "^4.17.21"
     micromatch "^4.0.5"
+    prompts "^2.4.2"
     resolve-pathname "^3.0.0"
     shelljs "^0.8.5"
     tslib "^2.6.0"
     url-loader "^4.1.1"
     webpack "^5.88.1"
 
-"@hapi/hoek@^9.0.0":
+"@hapi/hoek@^9.0.0", "@hapi/hoek@^9.3.0":
   version "9.3.0"
-  resolved "https://registry.npmjs.org/@hapi/hoek/-/hoek-9.3.0.tgz"
+  resolved "https://registry.yarnpkg.com/@hapi/hoek/-/hoek-9.3.0.tgz#8368869dcb735be2e7f5cb7647de78e167a251fb"
   integrity sha512-/c6rf4UJlmHlC9b5BaNvzAcFv7HZ2QHaV0D4/HNlBdvFnvQq8RI4kYdhyPCl7Xj+oWvTWQ8ujhqS53LIgAe6KQ==
 
-"@hapi/topo@^5.0.0":
+"@hapi/topo@^5.1.0":
   version "5.1.0"
-  resolved "https://registry.npmjs.org/@hapi/topo/-/topo-5.1.0.tgz"
+  resolved "https://registry.yarnpkg.com/@hapi/topo/-/topo-5.1.0.tgz#dc448e332c6c6e37a4dc02fd84ba8d44b9afb012"
   integrity sha512-foQZKJig7Ob0BMAYBfcJk8d77QtOe7Wo4ox7ff1lQYoNNAb6jwcY1ncdoy2e9wQZzvNy7ODZCYJkK8kzmcAnAg==
   dependencies:
     "@hapi/hoek" "^9.0.0"
 
 "@jest/schemas@^29.6.3":
   version "29.6.3"
   resolved "https://registry.npmjs.org/@jest/schemas/-/schemas-29.6.3.tgz"
@@ -1688,50 +1699,64 @@
   version "0.1.1"
   resolved "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.1.1.tgz"
   integrity sha512-sQXCasFk+U8lWYEe66WxRDOE9PjVz4vSM51fTu3Hw+ClTpUSQb718772vH3pyS5pShp6lvQM7SxgIDXXXmOX7w==
   dependencies:
     "@jridgewell/set-array" "^1.0.0"
     "@jridgewell/sourcemap-codec" "^1.4.10"
 
-"@jridgewell/gen-mapping@^0.3.0", "@jridgewell/gen-mapping@^0.3.2":
+"@jridgewell/gen-mapping@^0.3.2":
   version "0.3.2"
   resolved "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.2.tgz"
   integrity sha512-mh65xKQAzI6iBcFzwv28KVWSmCkdRBWoOh+bYQGW3+6OZvbbN3TqMGo5hqYxQniRcH9F2VZIoJCm4pa3BPDK/A==
   dependencies:
     "@jridgewell/set-array" "^1.0.1"
     "@jridgewell/sourcemap-codec" "^1.4.10"
     "@jridgewell/trace-mapping" "^0.3.9"
 
+"@jridgewell/gen-mapping@^0.3.5":
+  version "0.3.5"
+  resolved "https://registry.yarnpkg.com/@jridgewell/gen-mapping/-/gen-mapping-0.3.5.tgz#dcce6aff74bdf6dad1a95802b69b04a2fcb1fb36"
+  integrity sha512-IzL8ZoEDIBRWEzlCcRhOaCupYyN5gdIK+Q6fbFdPDg6HqX6jpkItn7DFIpW9LQzXG6Df9sA7+OKnq0qlz/GaQg==
+  dependencies:
+    "@jridgewell/set-array" "^1.2.1"
+    "@jridgewell/sourcemap-codec" "^1.4.10"
+    "@jridgewell/trace-mapping" "^0.3.24"
+
 "@jridgewell/resolve-uri@^3.1.0":
-  version "3.1.0"
-  resolved "https://registry.npmjs.org/@jridgewell/resolve-uri/-/resolve-uri-3.1.0.tgz"
-  integrity sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==
+  version "3.1.2"
+  resolved "https://registry.yarnpkg.com/@jridgewell/resolve-uri/-/resolve-uri-3.1.2.tgz#7a0ee601f60f99a20c7c7c5ff0c80388c1189bd6"
+  integrity sha512-bRISgCIjP20/tbWSPWMEi54QVPRZExkuD9lJL+UIxUKtwVJA8wW1Trb1jMs1RFXo1CBTNZ/5hpC9QvmKWdopKw==
 
-"@jridgewell/set-array@^1.0.0", "@jridgewell/set-array@^1.0.1":
+"@jridgewell/set-array@^1.0.0":
   version "1.1.1"
   resolved "https://registry.npmjs.org/@jridgewell/set-array/-/set-array-1.1.1.tgz"
   integrity sha512-Ct5MqZkLGEXTVmQYbGtx9SVqD2fqwvdubdps5D3djjAkgkKwT918VNOz65pEHFaYTeWcukmJmH5SwsA9Tn2ObQ==
 
+"@jridgewell/set-array@^1.0.1", "@jridgewell/set-array@^1.2.1":
+  version "1.2.1"
+  resolved "https://registry.yarnpkg.com/@jridgewell/set-array/-/set-array-1.2.1.tgz#558fb6472ed16a4c850b889530e6b36438c49280"
+  integrity sha512-R8gLRTZeyp03ymzP/6Lil/28tGeGEzhx1q2k703KGWRAI1VdvPIXdG70VJc2pAMw3NA6JKL5hhFu1sJX0Mnn/A==
+
 "@jridgewell/source-map@^0.3.3":
-  version "0.3.5"
-  resolved "https://registry.npmjs.org/@jridgewell/source-map/-/source-map-0.3.5.tgz"
-  integrity sha512-UTYAUj/wviwdsMfzoSJspJxbkH5o1snzwX0//0ENX1u/55kkZZkcTZP6u9bwKGkv+dkk9at4m1Cpt0uY80kcpQ==
+  version "0.3.6"
+  resolved "https://registry.yarnpkg.com/@jridgewell/source-map/-/source-map-0.3.6.tgz#9d71ca886e32502eb9362c9a74a46787c36df81a"
+  integrity sha512-1ZJTZebgqllO79ue2bm3rIGud/bOe0pP5BjSRCRxxYkEZS8STV7zN84UBbiYu7jy+eCKSnVIUgoWWE/tt+shMQ==
   dependencies:
-    "@jridgewell/gen-mapping" "^0.3.0"
-    "@jridgewell/trace-mapping" "^0.3.9"
+    "@jridgewell/gen-mapping" "^0.3.5"
+    "@jridgewell/trace-mapping" "^0.3.25"
 
 "@jridgewell/sourcemap-codec@^1.4.10", "@jridgewell/sourcemap-codec@^1.4.14":
-  version "1.4.14"
-  resolved "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz"
-  integrity sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==
-
-"@jridgewell/trace-mapping@^0.3.17", "@jridgewell/trace-mapping@^0.3.9":
-  version "0.3.20"
-  resolved "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.20.tgz"
-  integrity sha512-R8LcPeWZol2zR8mmH3JeKQ6QRCFb7XgUhV9ZlGhHLGyg4wpPiPZNQOOWhFZhxKw8u//yTbNGI42Bx/3paXEQ+Q==
+  version "1.4.15"
+  resolved "https://registry.yarnpkg.com/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.15.tgz#d7c6e6755c78567a951e04ab52ef0fd26de59f32"
+  integrity sha512-eF2rxCRulEKXHTRiDrDy6erMYWqNw4LPdQ8UQA4huuxaQsVeRPFl2oM8oDGxMFhJUWZf9McpLtJasDDZb/Bpeg==
+
+"@jridgewell/trace-mapping@^0.3.17", "@jridgewell/trace-mapping@^0.3.20", "@jridgewell/trace-mapping@^0.3.24", "@jridgewell/trace-mapping@^0.3.25", "@jridgewell/trace-mapping@^0.3.9":
+  version "0.3.25"
+  resolved "https://registry.yarnpkg.com/@jridgewell/trace-mapping/-/trace-mapping-0.3.25.tgz#15f190e98895f3fc23276ee14bc76b675c2e50f0"
+  integrity sha512-vNk6aEwybGtawWmy/PzwnGDOjCkLWSD2wqvjGGAgOAwCGWySYXfYoxt00IJkTF+8Lb57DwOb3Aa0o9CApepiYQ==
   dependencies:
     "@jridgewell/resolve-uri" "^3.1.0"
     "@jridgewell/sourcemap-codec" "^1.4.14"
 
 "@leichtgewicht/ip-codec@^2.0.1":
   version "2.0.4"
   resolved "https://registry.npmjs.org/@leichtgewicht/ip-codec/-/ip-codec-2.0.4.tgz"
@@ -1816,29 +1841,29 @@
     config-chain "^1.1.11"
 
 "@polka/url@^1.0.0-next.20":
   version "1.0.0-next.21"
   resolved "https://registry.npmjs.org/@polka/url/-/url-1.0.0-next.21.tgz"
   integrity sha512-a5Sab1C4/icpTZVzZc5Ghpz88yQtGOyNqYXcZgOssB2uuAr+wF/MvN6bgtW32q7HHrvBki+BsZ0OuNv6EV3K9g==
 
-"@sideway/address@^4.1.3":
-  version "4.1.4"
-  resolved "https://registry.npmjs.org/@sideway/address/-/address-4.1.4.tgz"
-  integrity sha512-7vwq+rOHVWjyXxVlR76Agnvhy8I9rpzjosTESvmhNeXOXdZZB15Fl+TI9x1SiHZH5Jv2wTGduSxFDIaq0m3DUw==
+"@sideway/address@^4.1.5":
+  version "4.1.5"
+  resolved "https://registry.yarnpkg.com/@sideway/address/-/address-4.1.5.tgz#4bc149a0076623ced99ca8208ba780d65a99b9d5"
+  integrity sha512-IqO/DUQHUkPeixNQ8n0JA6102hT9CmaljNTPmQ1u8MEhBo/R4Q8eKLN/vGZxuebwOroDB4cbpjheD4+/sKFK4Q==
   dependencies:
     "@hapi/hoek" "^9.0.0"
 
 "@sideway/formula@^3.0.1":
   version "3.0.1"
-  resolved "https://registry.npmjs.org/@sideway/formula/-/formula-3.0.1.tgz"
+  resolved "https://registry.yarnpkg.com/@sideway/formula/-/formula-3.0.1.tgz#80fcbcbaf7ce031e0ef2dd29b1bfc7c3f583611f"
   integrity sha512-/poHZJJVjx3L+zVD6g9KgHfYnb443oi7wLu/XKojDviHy6HOEOA6z1Trk5aR1dGcmPenJEgb2sK2I80LeS3MIg==
 
 "@sideway/pinpoint@^2.0.0":
   version "2.0.0"
-  resolved "https://registry.npmjs.org/@sideway/pinpoint/-/pinpoint-2.0.0.tgz"
+  resolved "https://registry.yarnpkg.com/@sideway/pinpoint/-/pinpoint-2.0.0.tgz#cff8ffadc372ad29fd3f78277aeb29e632cc70df"
   integrity sha512-RNiOoTPkptFtSVzQevY/yWtZwf/RxyVnPy/OcA9HBM3MlGDnBEYL5B41H0MTn0Uec8Hi+2qUtTfG2WWZBmMejQ==
 
 "@sinclair/typebox@^0.27.8":
   version "0.27.8"
   resolved "https://registry.npmjs.org/@sinclair/typebox/-/typebox-0.27.8.tgz"
   integrity sha512-+Fj43pSMwJs4KRrH/938Uf+uAELIgVBmQzg/q1YG10djyfA3TnrU8N8XzqCh/okZdszqBQTZf96idMfE5lnwTA==
 
@@ -1857,23 +1882,14 @@
   resolved "https://registry.npmjs.org/@slorber/remark-comment/-/remark-comment-1.0.0.tgz"
   integrity sha512-RCE24n7jsOj1M0UPvIQCHTe7fI0sFL4S2nwKVWwHyVr/wI/H8GosgsJGyhnsZoGFnD/P2hLf1mSbrrgSLN93NA==
   dependencies:
     micromark-factory-space "^1.0.0"
     micromark-util-character "^1.1.0"
     micromark-util-symbol "^1.0.1"
 
-"@slorber/static-site-generator-webpack-plugin@^4.0.7":
-  version "4.0.7"
-  resolved "https://registry.npmjs.org/@slorber/static-site-generator-webpack-plugin/-/static-site-generator-webpack-plugin-4.0.7.tgz"
-  integrity sha512-Ug7x6z5lwrz0WqdnNFOMYrDQNTPAprvHLSh6+/fmml3qUiz6l5eq+2MzLKWtn/q5K5NpSiFsZTP/fck/3vjSxA==
-  dependencies:
-    eval "^0.1.8"
-    p-map "^4.0.0"
-    webpack-sources "^3.2.2"
-
 "@svgr/babel-plugin-add-jsx-attribute@^6.5.1":
   version "6.5.1"
   resolved "https://registry.npmjs.org/@svgr/babel-plugin-add-jsx-attribute/-/babel-plugin-add-jsx-attribute-6.5.1.tgz"
   integrity sha512-9PYGcXrAxitycIjRmZB+Q0JaN07GZIWaTBIGQzfaZv+qr1n8X1XUEJ5rZ/vx6OVD9RRYlrNnXWExQXcmZeD/BQ==
 
 "@svgr/babel-plugin-remove-jsx-attribute@*":
   version "8.0.0"
@@ -2029,39 +2045,39 @@
   version "4.1.12"
   resolved "https://registry.npmjs.org/@types/debug/-/debug-4.1.12.tgz"
   integrity sha512-vIChWdVG3LG1SMxEvI/AK+FWJthlrqlTu7fbrlywTkkaONwk/UAGaULXRlf8vkzFBLVm0zkMdCquhL5aOjhXPQ==
   dependencies:
     "@types/ms" "*"
 
 "@types/eslint-scope@^3.7.3":
-  version "3.7.3"
-  resolved "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.3.tgz"
-  integrity sha512-PB3ldyrcnAicT35TWPs5IcwKD8S333HMaa2VVv4+wdvebJkjWuW/xESoB8IwRcog8HYVYamb1g/R31Qv5Bx03g==
+  version "3.7.7"
+  resolved "https://registry.yarnpkg.com/@types/eslint-scope/-/eslint-scope-3.7.7.tgz#3108bd5f18b0cdb277c867b3dd449c9ed7079ac5"
+  integrity sha512-MzMFlSLBqNF2gcHWO0G1vP/YQyfvrxZ0bF+u7mzUdZ1/xK4A4sru+nraZz5i3iEIk1l1uyicaDVTB4QbbEkAYg==
   dependencies:
     "@types/eslint" "*"
     "@types/estree" "*"
 
 "@types/eslint@*":
-  version "8.4.2"
-  resolved "https://registry.npmjs.org/@types/eslint/-/eslint-8.4.2.tgz"
-  integrity sha512-Z1nseZON+GEnFjJc04sv4NSALGjhFwy6K0HXt7qsn5ArfAKtb63dXNJHf+1YW6IpOIYRBGUbu3GwJdj8DGnCjA==
+  version "8.56.7"
+  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.56.7.tgz#c33b5b5a9cfb66881beb7b5be6c34aa3e81d3366"
+  integrity sha512-SjDvI/x3zsZnOkYZ3lCt9lOZWZLB2jIlNKz+LBgCtDurK0JZcwucxYHn1w2BJkD34dgX9Tjnak0txtq4WTggEA==
   dependencies:
     "@types/estree" "*"
     "@types/json-schema" "*"
 
 "@types/estree-jsx@^1.0.0":
   version "1.0.3"
   resolved "https://registry.npmjs.org/@types/estree-jsx/-/estree-jsx-1.0.3.tgz"
   integrity sha512-pvQ+TKeRHeiUGRhvYwRrQ/ISnohKkSJR14fT2yqyZ4e9K5vqc7hrtY2Y1Dw0ZwAzQ6DQsxsaCUuSIIi8v0Cq6w==
   dependencies:
     "@types/estree" "*"
 
-"@types/estree@*", "@types/estree@^1.0.0":
+"@types/estree@*", "@types/estree@^1.0.0", "@types/estree@^1.0.5":
   version "1.0.5"
-  resolved "https://registry.npmjs.org/@types/estree/-/estree-1.0.5.tgz"
+  resolved "https://registry.yarnpkg.com/@types/estree/-/estree-1.0.5.tgz#a6ce3e556e00fd9895dd872dd172ad0d4bd687f4"
   integrity sha512-/kYRxGDLWzHOB7q+wtSUQlFrtcdUccpfy+X+9iMBpHK8QLLhx2wIPYuS5DYtR9Wa/YlZAbIovy7qVdB1Aq6Lyw==
 
 "@types/express-serve-static-core@*", "@types/express-serve-static-core@^4.17.18":
   version "4.17.28"
   resolved "https://registry.npmjs.org/@types/express-serve-static-core/-/express-serve-static-core-4.17.28.tgz"
   integrity sha512-P1BJAEAW3E2DJUlkgq4tOL3RyMunoWXqbSCygWo5ZIWTjUgN1YnaXWW4VWl/oc8vs/XoYibEGBKP0uZyF4AHig==
   dependencies:
@@ -2089,15 +2105,15 @@
   resolved "https://registry.npmjs.org/@types/hast/-/hast-3.0.3.tgz"
   integrity sha512-2fYGlaDy/qyLlhidX42wAH0KBi2TCjKMH8CHmBXgRlJ3Y+OXTiqsPQ6IWarZKwF1JoUcAJdPogv1d4b0COTpmQ==
   dependencies:
     "@types/unist" "*"
 
 "@types/history@^4.7.11":
   version "4.7.11"
-  resolved "https://registry.npmjs.org/@types/history/-/history-4.7.11.tgz"
+  resolved "https://registry.yarnpkg.com/@types/history/-/history-4.7.11.tgz#56588b17ae8f50c53983a524fc3cc47437969d64"
   integrity sha512-qjDJRrmvBMiTx+jyLxvLfJU7UznFuokDv4f3WRuriHKERccVpFU+8XMQUAbDzoiJCsmexxRExQeMwwCdamSKDA==
 
 "@types/html-minifier-terser@^6.0.0":
   version "6.1.0"
   resolved "https://registry.npmjs.org/@types/html-minifier-terser/-/html-minifier-terser-6.1.0.tgz"
   integrity sha512-oh/6byDPnL1zeNXFrDXFLyZjkr1MsBG667IM792caf1L2UPOOMf65NFzjUH/ltyfwjAGfs1rsX1eftK0jC/KIg==
 
@@ -2128,15 +2144,20 @@
 "@types/istanbul-reports@^3.0.0":
   version "3.0.1"
   resolved "https://registry.npmjs.org/@types/istanbul-reports/-/istanbul-reports-3.0.1.tgz"
   integrity sha512-c3mAZEuK0lvBp8tmuL74XRKn1+y2dcwOUpH7x4WrF6gk1GIgiluDRgMYQtw2OFcBvAJWlt6ASU3tSqxp0Uu0Aw==
   dependencies:
     "@types/istanbul-lib-report" "*"
 
-"@types/json-schema@*", "@types/json-schema@^7.0.4", "@types/json-schema@^7.0.5", "@types/json-schema@^7.0.8", "@types/json-schema@^7.0.9":
+"@types/json-schema@*", "@types/json-schema@^7.0.8":
+  version "7.0.15"
+  resolved "https://registry.yarnpkg.com/@types/json-schema/-/json-schema-7.0.15.tgz#596a1747233694d50f6ad8a7869fcb6f56cf5841"
+  integrity sha512-5+fP8P8MFNC+AyZCDxrB2pkZFPGzqQWUzpSeuuVLvm8VMcorNYavBqoFcxK8bQz4Qsbn4oUEEem4wDLfcysGHA==
+
+"@types/json-schema@^7.0.4", "@types/json-schema@^7.0.5", "@types/json-schema@^7.0.9":
   version "7.0.11"
   resolved "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.11.tgz"
   integrity sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==
 
 "@types/mdast@^4.0.0", "@types/mdast@^4.0.2":
   version "4.0.3"
   resolved "https://registry.npmjs.org/@types/mdast/-/mdast-4.0.3.tgz"
@@ -2162,15 +2183,22 @@
 "@types/node-forge@^1.3.0":
   version "1.3.10"
   resolved "https://registry.npmjs.org/@types/node-forge/-/node-forge-1.3.10.tgz"
   integrity sha512-y6PJDYN4xYBxwd22l+OVH35N+1fCYWiuC3aiP2SlXVE6Lo7SS+rSx9r89hLxrP4pn6n1lBGhHJ12pj3F3Mpttw==
   dependencies:
     "@types/node" "*"
 
-"@types/node@*", "@types/node@^17.0.5":
+"@types/node@*":
+  version "20.12.4"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.12.4.tgz#af5921bd75ccdf3a3d8b3fa75bf3d3359268cd11"
+  integrity sha512-E+Fa9z3wSQpzgYQdYmme5X3OTuejnnTx88A6p6vkkJosR3KBz+HpE3kqNm98VE6cfLFcISx7zW7MsJkH6KwbTw==
+  dependencies:
+    undici-types "~5.26.4"
+
+"@types/node@^17.0.5":
   version "17.0.36"
   resolved "https://registry.npmjs.org/@types/node/-/node-17.0.36.tgz"
   integrity sha512-V3orv+ggDsWVHP99K3JlwtH20R7J4IhI1Kksgc+64q5VxgfRkQG8Ws3MFm/FZOKDYGy9feGFlZ70/HpCNe9QaA==
 
 "@types/parse-json@^4.0.0":
   version "4.0.0"
   resolved "https://registry.npmjs.org/@types/parse-json/-/parse-json-4.0.0.tgz"
@@ -2178,17 +2206,17 @@
 
 "@types/prismjs@^1.26.0":
   version "1.26.3"
   resolved "https://registry.npmjs.org/@types/prismjs/-/prismjs-1.26.3.tgz"
   integrity sha512-A0D0aTXvjlqJ5ZILMz3rNfDBOx9hHxLZYv2by47Sm/pqW35zzjusrZTryatjN/Rf8Us2gZrJD+KeHbUSTux1Cw==
 
 "@types/prop-types@*":
-  version "15.7.5"
-  resolved "https://registry.npmjs.org/@types/prop-types/-/prop-types-15.7.5.tgz"
-  integrity sha512-JCB8C6SnDoQf0cNycqd/35A7MjcnK+ZTqE7judS6o7utxUCg6imJg3QK2qzHKszlTjcj2cn+NwMB2i96ubpj7w==
+  version "15.7.12"
+  resolved "https://registry.yarnpkg.com/@types/prop-types/-/prop-types-15.7.12.tgz#12bb1e2be27293c1406acb6af1c3f3a1481d98c6"
+  integrity sha512-5zvhXYtRNRluoE/jAp4GVsSduVUzNWKkOZrCDBWYtE7biZywwdC2AcEzg+cSMLFRfVgeAFqpfNabiPjxFddV1Q==
 
 "@types/qs@*":
   version "6.9.7"
   resolved "https://registry.npmjs.org/@types/qs/-/qs-6.9.7.tgz"
   integrity sha512-FGa1F62FT09qcrueBA6qYTrJPVDzah9a+493+o2PCXsesWHIn27G98TsSMs3WPNbZIEj4+VJf6saSFpvD+3Zsw==
 
 "@types/range-parser@*":
@@ -2218,15 +2246,23 @@
   version "5.1.20"
   resolved "https://registry.npmjs.org/@types/react-router/-/react-router-5.1.20.tgz"
   integrity sha512-jGjmu/ZqS7FjSH6owMcD5qpq19+1RS9DeVRqfl1FeBMxTDQAGwlMWOcs52NDoXaNKyG3d1cYQFMs9rCrb88o9Q==
   dependencies:
     "@types/history" "^4.7.11"
     "@types/react" "*"
 
-"@types/react@*", "@types/react@^18.2.29":
+"@types/react@*":
+  version "18.2.74"
+  resolved "https://registry.yarnpkg.com/@types/react/-/react-18.2.74.tgz#2d52eb80e4e7c4ea8812c89181d6d590b53f958c"
+  integrity sha512-9AEqNZZyBx8OdZpxzQlaFEVCSFUM2YXJH46yPOiOpm078k6ZLOCcuAzGum/zK8YBwY+dbahVNbHrbgrAwIRlqw==
+  dependencies:
+    "@types/prop-types" "*"
+    csstype "^3.0.2"
+
+"@types/react@^18.2.29":
   version "18.2.45"
   resolved "https://registry.npmjs.org/@types/react/-/react-18.2.45.tgz"
   integrity sha512-TtAxCNrlrBp8GoeEp1npd5g+d/OejJHFxS3OWmrPBMFaVQMSN0OFySozJio5BHxTuTeug00AVXVAjfDSfk+lUg==
   dependencies:
     "@types/prop-types" "*"
     "@types/scheduler" "*"
     csstype "^3.0.2"
@@ -2240,17 +2276,17 @@
   version "1.2.4"
   resolved "https://registry.npmjs.org/@types/sax/-/sax-1.2.4.tgz"
   integrity sha512-pSAff4IAxJjfAXUG6tFkO7dsSbTmf8CtUpfhhZ5VhkRpC4628tJhh3+V6H1E+/Gs9piSzYKT5yzHO5M4GG9jkw==
   dependencies:
     "@types/node" "*"
 
 "@types/scheduler@*":
-  version "0.16.2"
-  resolved "https://registry.npmjs.org/@types/scheduler/-/scheduler-0.16.2.tgz"
-  integrity sha512-hppQEBDmlwhFAXKJX2KnWLYu5yMfi91yazPb2l+lbJiwW+wdo1gNeRA+3RgNSO39WYX2euey41KEwnqesU2Jew==
+  version "0.23.0"
+  resolved "https://registry.yarnpkg.com/@types/scheduler/-/scheduler-0.23.0.tgz#0a6655b3e2708eaabca00b7372fafd7a792a7b09"
+  integrity sha512-YIoDCTH3Af6XM5VuwGG/QL/CJqga1Zm3NkU3HZ4ZHK2fRMPYP1VczsTUqtsf43PH/iJNVlPHAo2oWX7BSdB2Hw==
 
 "@types/serve-index@^1.9.1":
   version "1.9.1"
   resolved "https://registry.npmjs.org/@types/serve-index/-/serve-index-1.9.1.tgz"
   integrity sha512-d/Hs3nWDxNL2xAczmOVZNj92YZCS6RGxfBPjKzuu/XirCgXdpKEb88dYNbrYGint6IVWLNP+yonwVAuRC0T2Dg==
   dependencies:
     "@types/express" "*"
@@ -2300,173 +2336,178 @@
     "@types/yargs-parser" "*"
 
 "@ungap/structured-clone@^1.0.0":
   version "1.2.0"
   resolved "https://registry.npmjs.org/@ungap/structured-clone/-/structured-clone-1.2.0.tgz"
   integrity sha512-zuVdFrMJiuCDQUMCzQaD6KL28MjnqqN8XnAqiEq9PNm/hCPTSGfrXCOfwj1ow4LFb/tNymJPwsNbVePc1xFqrQ==
 
-"@webassemblyjs/ast@1.11.6", "@webassemblyjs/ast@^1.11.5":
-  version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/ast/-/ast-1.11.6.tgz"
-  integrity sha512-IN1xI7PwOvLPgjcf180gC1bqn3q/QaOCwYUahIOhbYUu8KA/3tw2RT/T0Gidi1l7Hhj5D/INhJxiICObqpMu4Q==
+"@webassemblyjs/ast@1.12.1", "@webassemblyjs/ast@^1.12.1":
+  version "1.12.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/ast/-/ast-1.12.1.tgz#bb16a0e8b1914f979f45864c23819cc3e3f0d4bb"
+  integrity sha512-EKfMUOPRRUTy5UII4qJDGPpqfwjOmZ5jeGFwid9mnoqIFK+e0vqoi1qH56JpmZSzEL53jKnNzScdmftJyG5xWg==
   dependencies:
     "@webassemblyjs/helper-numbers" "1.11.6"
     "@webassemblyjs/helper-wasm-bytecode" "1.11.6"
 
 "@webassemblyjs/floating-point-hex-parser@1.11.6":
   version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.6.tgz"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/floating-point-hex-parser/-/floating-point-hex-parser-1.11.6.tgz#dacbcb95aff135c8260f77fa3b4c5fea600a6431"
   integrity sha512-ejAj9hfRJ2XMsNHk/v6Fu2dGS+i4UaXBXGemOfQ/JfQ6mdQg/WXtwleQRLLS4OvfDhv8rYnVwH27YJLMyYsxhw==
 
 "@webassemblyjs/helper-api-error@1.11.6":
   version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.6.tgz"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-api-error/-/helper-api-error-1.11.6.tgz#6132f68c4acd59dcd141c44b18cbebbd9f2fa768"
   integrity sha512-o0YkoP4pVu4rN8aTJgAyj9hC2Sv5UlkzCHhxqWj8butaLvnpdc2jOwh4ewE6CX0txSfLn/UYaV/pheS2Txg//Q==
 
-"@webassemblyjs/helper-buffer@1.11.6":
-  version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/helper-buffer/-/helper-buffer-1.11.6.tgz"
-  integrity sha512-z3nFzdcp1mb8nEOFFk8DrYLpHvhKC3grJD2ardfKOzmbmJvEf/tPIqCY+sNcwZIY8ZD7IkB2l7/pqhUhqm7hLA==
+"@webassemblyjs/helper-buffer@1.12.1":
+  version "1.12.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-buffer/-/helper-buffer-1.12.1.tgz#6df20d272ea5439bf20ab3492b7fb70e9bfcb3f6"
+  integrity sha512-nzJwQw99DNDKr9BVCOZcLuJJUlqkJh+kVzVl6Fmq/tI5ZtEyWT1KZMyOXltXLZJmDtvLCDgwsyrkohEtopTXCw==
 
 "@webassemblyjs/helper-numbers@1.11.6":
   version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.6.tgz"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-numbers/-/helper-numbers-1.11.6.tgz#cbce5e7e0c1bd32cf4905ae444ef64cea919f1b5"
   integrity sha512-vUIhZ8LZoIWHBohiEObxVm6hwP034jwmc9kuq5GdHZH0wiLVLIPcMCdpJzG4C11cHoQ25TFIQj9kaVADVX7N3g==
   dependencies:
     "@webassemblyjs/floating-point-hex-parser" "1.11.6"
     "@webassemblyjs/helper-api-error" "1.11.6"
     "@xtuc/long" "4.2.2"
 
 "@webassemblyjs/helper-wasm-bytecode@1.11.6":
   version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.6.tgz"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-bytecode/-/helper-wasm-bytecode-1.11.6.tgz#bb2ebdb3b83aa26d9baad4c46d4315283acd51e9"
   integrity sha512-sFFHKwcmBprO9e7Icf0+gddyWYDViL8bpPjJJl0WHxCdETktXdmtWLGVzoHbqUcY4Be1LkNfwTmXOJUFZYSJdA==
 
-"@webassemblyjs/helper-wasm-section@1.11.6":
-  version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.11.6.tgz"
-  integrity sha512-LPpZbSOwTpEC2cgn4hTydySy1Ke+XEu+ETXuoyvuyezHO3Kjdu90KK95Sh9xTbmjrCsUwvWwCOQQNta37VrS9g==
+"@webassemblyjs/helper-wasm-section@1.12.1":
+  version "1.12.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/helper-wasm-section/-/helper-wasm-section-1.12.1.tgz#3da623233ae1a60409b509a52ade9bc22a37f7bf"
+  integrity sha512-Jif4vfB6FJlUlSbgEMHUyk1j234GTNG9dBJ4XJdOySoj518Xj0oGsNi59cUQF4RRMS9ouBUxDDdyBVfPTypa5g==
   dependencies:
-    "@webassemblyjs/ast" "1.11.6"
-    "@webassemblyjs/helper-buffer" "1.11.6"
+    "@webassemblyjs/ast" "1.12.1"
+    "@webassemblyjs/helper-buffer" "1.12.1"
     "@webassemblyjs/helper-wasm-bytecode" "1.11.6"
-    "@webassemblyjs/wasm-gen" "1.11.6"
+    "@webassemblyjs/wasm-gen" "1.12.1"
 
 "@webassemblyjs/ieee754@1.11.6":
   version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/ieee754/-/ieee754-1.11.6.tgz"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/ieee754/-/ieee754-1.11.6.tgz#bb665c91d0b14fffceb0e38298c329af043c6e3a"
   integrity sha512-LM4p2csPNvbij6U1f19v6WR56QZ8JcHg3QIJTlSwzFcmx6WSORicYj6I63f9yU1kEUtrpG+kjkiIAkevHpDXrg==
   dependencies:
     "@xtuc/ieee754" "^1.2.0"
 
 "@webassemblyjs/leb128@1.11.6":
   version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/leb128/-/leb128-1.11.6.tgz"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/leb128/-/leb128-1.11.6.tgz#70e60e5e82f9ac81118bc25381a0b283893240d7"
   integrity sha512-m7a0FhE67DQXgouf1tbN5XQcdWoNgaAuoULHIfGFIEVKA6tu/edls6XnIlkmS6FrXAquJRPni3ZZKjw6FSPjPQ==
   dependencies:
     "@xtuc/long" "4.2.2"
 
 "@webassemblyjs/utf8@1.11.6":
   version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/utf8/-/utf8-1.11.6.tgz"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/utf8/-/utf8-1.11.6.tgz#90f8bc34c561595fe156603be7253cdbcd0fab5a"
   integrity sha512-vtXf2wTQ3+up9Zsg8sa2yWiQpzSsMyXj0qViVP6xKGCUT8p8YJ6HqI7l5eCnWx1T/FYdsv07HQs2wTFbbof/RA==
 
-"@webassemblyjs/wasm-edit@^1.11.5":
-  version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/wasm-edit/-/wasm-edit-1.11.6.tgz"
-  integrity sha512-Ybn2I6fnfIGuCR+Faaz7YcvtBKxvoLV3Lebn1tM4o/IAJzmi9AWYIPWpyBfU8cC+JxAO57bk4+zdsTjJR+VTOw==
+"@webassemblyjs/wasm-edit@^1.12.1":
+  version "1.12.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-edit/-/wasm-edit-1.12.1.tgz#9f9f3ff52a14c980939be0ef9d5df9ebc678ae3b"
+  integrity sha512-1DuwbVvADvS5mGnXbE+c9NfA8QRcZ6iKquqjjmR10k6o+zzsRVesil54DKexiowcFCPdr/Q0qaMgB01+SQ1u6g==
   dependencies:
-    "@webassemblyjs/ast" "1.11.6"
-    "@webassemblyjs/helper-buffer" "1.11.6"
+    "@webassemblyjs/ast" "1.12.1"
+    "@webassemblyjs/helper-buffer" "1.12.1"
     "@webassemblyjs/helper-wasm-bytecode" "1.11.6"
-    "@webassemblyjs/helper-wasm-section" "1.11.6"
-    "@webassemblyjs/wasm-gen" "1.11.6"
-    "@webassemblyjs/wasm-opt" "1.11.6"
-    "@webassemblyjs/wasm-parser" "1.11.6"
-    "@webassemblyjs/wast-printer" "1.11.6"
-
-"@webassemblyjs/wasm-gen@1.11.6":
-  version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/wasm-gen/-/wasm-gen-1.11.6.tgz"
-  integrity sha512-3XOqkZP/y6B4F0PBAXvI1/bky7GryoogUtfwExeP/v7Nzwo1QLcq5oQmpKlftZLbT+ERUOAZVQjuNVak6UXjPA==
+    "@webassemblyjs/helper-wasm-section" "1.12.1"
+    "@webassemblyjs/wasm-gen" "1.12.1"
+    "@webassemblyjs/wasm-opt" "1.12.1"
+    "@webassemblyjs/wasm-parser" "1.12.1"
+    "@webassemblyjs/wast-printer" "1.12.1"
+
+"@webassemblyjs/wasm-gen@1.12.1":
+  version "1.12.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-gen/-/wasm-gen-1.12.1.tgz#a6520601da1b5700448273666a71ad0a45d78547"
+  integrity sha512-TDq4Ojh9fcohAw6OIMXqiIcTq5KUXTGRkVxbSo1hQnSy6lAM5GSdfwWeSxpAo0YzgsgF182E/U0mDNhuA0tW7w==
   dependencies:
-    "@webassemblyjs/ast" "1.11.6"
+    "@webassemblyjs/ast" "1.12.1"
     "@webassemblyjs/helper-wasm-bytecode" "1.11.6"
     "@webassemblyjs/ieee754" "1.11.6"
     "@webassemblyjs/leb128" "1.11.6"
     "@webassemblyjs/utf8" "1.11.6"
 
-"@webassemblyjs/wasm-opt@1.11.6":
-  version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/wasm-opt/-/wasm-opt-1.11.6.tgz"
-  integrity sha512-cOrKuLRE7PCe6AsOVl7WasYf3wbSo4CeOk6PkrjS7g57MFfVUF9u6ysQBBODX0LdgSvQqRiGz3CXvIDKcPNy4g==
+"@webassemblyjs/wasm-opt@1.12.1":
+  version "1.12.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-opt/-/wasm-opt-1.12.1.tgz#9e6e81475dfcfb62dab574ac2dda38226c232bc5"
+  integrity sha512-Jg99j/2gG2iaz3hijw857AVYekZe2SAskcqlWIZXjji5WStnOpVoat3gQfT/Q5tb2djnCjBtMocY/Su1GfxPBg==
+  dependencies:
+    "@webassemblyjs/ast" "1.12.1"
+    "@webassemblyjs/helper-buffer" "1.12.1"
+    "@webassemblyjs/wasm-gen" "1.12.1"
+    "@webassemblyjs/wasm-parser" "1.12.1"
+
+"@webassemblyjs/wasm-parser@1.12.1", "@webassemblyjs/wasm-parser@^1.12.1":
+  version "1.12.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wasm-parser/-/wasm-parser-1.12.1.tgz#c47acb90e6f083391e3fa61d113650eea1e95937"
+  integrity sha512-xikIi7c2FHXysxXe3COrVUPSheuBtpcfhbpFj4gmu7KRLYOzANztwUU0IbsqvMqzuNK2+glRGWCEqZo1WCLyAQ==
   dependencies:
-    "@webassemblyjs/ast" "1.11.6"
-    "@webassemblyjs/helper-buffer" "1.11.6"
-    "@webassemblyjs/wasm-gen" "1.11.6"
-    "@webassemblyjs/wasm-parser" "1.11.6"
-
-"@webassemblyjs/wasm-parser@1.11.6", "@webassemblyjs/wasm-parser@^1.11.5":
-  version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/wasm-parser/-/wasm-parser-1.11.6.tgz"
-  integrity sha512-6ZwPeGzMJM3Dqp3hCsLgESxBGtT/OeCvCZ4TA1JUPYgmhAx38tTPR9JaKy0S5H3evQpO/h2uWs2j6Yc/fjkpTQ==
-  dependencies:
-    "@webassemblyjs/ast" "1.11.6"
+    "@webassemblyjs/ast" "1.12.1"
     "@webassemblyjs/helper-api-error" "1.11.6"
     "@webassemblyjs/helper-wasm-bytecode" "1.11.6"
     "@webassemblyjs/ieee754" "1.11.6"
     "@webassemblyjs/leb128" "1.11.6"
     "@webassemblyjs/utf8" "1.11.6"
 
-"@webassemblyjs/wast-printer@1.11.6":
-  version "1.11.6"
-  resolved "https://registry.npmjs.org/@webassemblyjs/wast-printer/-/wast-printer-1.11.6.tgz"
-  integrity sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==
+"@webassemblyjs/wast-printer@1.12.1":
+  version "1.12.1"
+  resolved "https://registry.yarnpkg.com/@webassemblyjs/wast-printer/-/wast-printer-1.12.1.tgz#bcecf661d7d1abdaf989d8341a4833e33e2b31ac"
+  integrity sha512-+X4WAlOisVWQMikjbcvY2e0rwPsKQ9F688lksZhBcPycBBuii3O7m8FACbDMWDojpAqvjIncrG8J0XHKyQfVeA==
   dependencies:
-    "@webassemblyjs/ast" "1.11.6"
+    "@webassemblyjs/ast" "1.12.1"
     "@xtuc/long" "4.2.2"
 
 "@xtuc/ieee754@^1.2.0":
   version "1.2.0"
-  resolved "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz"
+  resolved "https://registry.yarnpkg.com/@xtuc/ieee754/-/ieee754-1.2.0.tgz#eef014a3145ae477a1cbc00cd1e552336dceb790"
   integrity sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==
 
 "@xtuc/long@4.2.2":
   version "4.2.2"
-  resolved "https://registry.npmjs.org/@xtuc/long/-/long-4.2.2.tgz"
+  resolved "https://registry.yarnpkg.com/@xtuc/long/-/long-4.2.2.tgz#d291c6a4e97989b5c61d9acf396ae4fe133a718d"
   integrity sha512-NuHqBY1PB/D8xU6s/thBgOAiAP7HOYDQ32+BFZILJ8ivkUkAHQnWfn6WhL79Owj1qmUnoN/YPhktdIoucipkAQ==
 
 accepts@~1.3.4, accepts@~1.3.5, accepts@~1.3.8:
   version "1.3.8"
   resolved "https://registry.npmjs.org/accepts/-/accepts-1.3.8.tgz"
   integrity sha512-PYAthTa2m2VKxuvSD3DPC/Gy+U+sOA1LAuT8mkmRuvw+NACSaeXEQ+NHcVF7rONl6qcaxV3Uuemwawk+7+SJLw==
   dependencies:
     mime-types "~2.1.34"
     negotiator "0.6.3"
 
 acorn-import-assertions@^1.9.0:
   version "1.9.0"
-  resolved "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.9.0.tgz"
+  resolved "https://registry.yarnpkg.com/acorn-import-assertions/-/acorn-import-assertions-1.9.0.tgz#507276249d684797c84e0734ef84860334cfb1ac"
   integrity sha512-cmMwop9x+8KFhxvKrKfPYmN6/pKTYYHBqLa0DfvVZcKMJWNyWLnaqND7dx/qn66R7ewM1UX5XMaDVP5wlVTaVA==
 
 acorn-jsx@^5.0.0:
   version "5.3.2"
   resolved "https://registry.npmjs.org/acorn-jsx/-/acorn-jsx-5.3.2.tgz"
   integrity sha512-rq9s+JNhf0IChjtDXxllJ7g41oZk5SlXtp0LHwyA5cejwn7vKmKp4pPri6YEePv2PU65sAsegbXtIinmDFDXgQ==
 
 acorn-walk@^8.0.0:
   version "8.2.0"
   resolved "https://registry.npmjs.org/acorn-walk/-/acorn-walk-8.2.0.tgz"
   integrity sha512-k+iyHEuPgSw6SbuDpGQM+06HQUa04DZ3o+F6CSzXMvvI5KMvnaEqXe+YVe555R9nn6GPt404fos4wcgpw12SDA==
 
-acorn@^8.0.0, acorn@^8.0.4, acorn@^8.7.1, acorn@^8.8.2:
+acorn@^8.0.0, acorn@^8.0.4:
   version "8.11.2"
   resolved "https://registry.npmjs.org/acorn/-/acorn-8.11.2.tgz"
   integrity sha512-nc0Axzp/0FILLEVsm4fNwLCwMttvhEI263QtVPQcbpfZZ3ts0hLsZGOpE6czNlid7CJ9MlyH8reXkpsf3YUY4w==
 
+acorn@^8.7.1, acorn@^8.8.2:
+  version "8.11.3"
+  resolved "https://registry.yarnpkg.com/acorn/-/acorn-8.11.3.tgz#71e0b14e13a4ec160724b38fb7b0f233b1b81d7a"
+  integrity sha512-Y9rRfJG5jcKOE0CLisYbojUjIrIEE7AGMzA/Sm4BslANhbS+cDMpgBdcPT91oJ7OuJ9hYJBx59RjbhxVnrF8Xg==
+
 address@^1.0.1, address@^1.1.2:
   version "1.2.0"
   resolved "https://registry.npmjs.org/address/-/address-1.2.0.tgz"
   integrity sha512-tNEZYz5G/zYunxFm7sfhAxkXEuLj3K6BKwv6ZURlsF6yiUQ65z0Q2wZW9L5cPUl9ocofGvXOdFYbFHp0+6MOig==
 
 aggregate-error@^3.0.0:
   version "3.1.0"
@@ -2481,27 +2522,27 @@
   resolved "https://registry.npmjs.org/ajv-formats/-/ajv-formats-2.1.1.tgz"
   integrity sha512-Wx0Kx52hxE7C18hkMEggYlEifqWZtYaRgouJor+WMdPnQyEK13vgEWyVNup7SoeeoLMsr4kf5h6dOW11I15MUA==
   dependencies:
     ajv "^8.0.0"
 
 ajv-keywords@^3.4.1, ajv-keywords@^3.5.2:
   version "3.5.2"
-  resolved "https://registry.npmjs.org/ajv-keywords/-/ajv-keywords-3.5.2.tgz"
+  resolved "https://registry.yarnpkg.com/ajv-keywords/-/ajv-keywords-3.5.2.tgz#31f29da5ab6e00d1c2d329acf7b5929614d5014d"
   integrity sha512-5p6WTN0DdTGVQk6VjcEju19IgaHudalcfabD7yhDGeA6bcQnmL+CpveLJq/3hvfwd1aof6L386Ougkx6RfyMIQ==
 
 ajv-keywords@^5.1.0:
   version "5.1.0"
   resolved "https://registry.npmjs.org/ajv-keywords/-/ajv-keywords-5.1.0.tgz"
   integrity sha512-YCS/JNFAUyr5vAuhk1DWm1CBxRHW9LbJ2ozWeemrIqpbsqKjHVxYPyi5GC0rjZIT5JxJ3virVTS8wk4i/Z+krw==
   dependencies:
     fast-deep-equal "^3.1.3"
 
 ajv@^6.12.2, ajv@^6.12.5:
   version "6.12.6"
-  resolved "https://registry.npmjs.org/ajv/-/ajv-6.12.6.tgz"
+  resolved "https://registry.yarnpkg.com/ajv/-/ajv-6.12.6.tgz#baf5a62e802b07d977034586f8c3baf5adf26df4"
   integrity sha512-j3fVLgvTo527anyYyJOGTYJbG+vnnQYvE0m5mmkc1TK+nxAppkCLMIL0aZ4dblVCNoGShhm+kzE4ZUykBoMg4g==
   dependencies:
     fast-deep-equal "^3.1.1"
     fast-json-stable-stringify "^2.0.0"
     json-schema-traverse "^0.4.1"
     uri-js "^4.2.2"
 
@@ -2719,29 +2760,29 @@
   integrity sha512-vyL2OymJxmarO8gxMr0mhChsO9QGwhynfuu4+MHTAW6czfq9humCB7rKpUjDd9YUiDPU4mzpyupFSvOClAwbmQ==
 
 binary-extensions@^2.0.0:
   version "2.2.0"
   resolved "https://registry.npmjs.org/binary-extensions/-/binary-extensions-2.2.0.tgz"
   integrity sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==
 
-body-parser@1.20.1:
-  version "1.20.1"
-  resolved "https://registry.npmjs.org/body-parser/-/body-parser-1.20.1.tgz"
-  integrity sha512-jWi7abTbYwajOytWCQc37VulmWiRae5RyTpaCyDcS5/lMdtwSz5lOpDE67srw/HYe35f1z3fDQw+3txg7gNtWw==
+body-parser@1.20.2:
+  version "1.20.2"
+  resolved "https://registry.yarnpkg.com/body-parser/-/body-parser-1.20.2.tgz#6feb0e21c4724d06de7ff38da36dad4f57a747fd"
+  integrity sha512-ml9pReCu3M61kGlqoTm2umSXTlRTuGTx0bfYj+uIUKKYycG5NtSbeetV3faSU6R7ajOPw0g/J1PvK4qNy7s5bA==
   dependencies:
     bytes "3.1.2"
-    content-type "~1.0.4"
+    content-type "~1.0.5"
     debug "2.6.9"
     depd "2.0.0"
     destroy "1.2.0"
     http-errors "2.0.0"
     iconv-lite "0.4.24"
     on-finished "2.4.1"
     qs "6.11.0"
-    raw-body "2.5.1"
+    raw-body "2.5.2"
     type-is "~1.6.18"
     unpipe "1.0.0"
 
 bonjour-service@^1.0.11:
   version "1.0.12"
   resolved "https://registry.npmjs.org/bonjour-service/-/bonjour-service-1.0.12.tgz"
   integrity sha512-pMmguXYCu63Ug37DluMKEHdxc+aaIf/ay4YbF8Gxtba+9d3u+rmEWy61VK3Z3hp8Rskok3BunHYnG0dUHAsblw==
@@ -2795,15 +2836,15 @@
 braces@^3.0.2, braces@~3.0.2:
   version "3.0.2"
   resolved "https://registry.npmjs.org/braces/-/braces-3.0.2.tgz"
   integrity sha512-b8um+L1RzM3WDSzvhm6gIz1yfTbBt6YTlcEKAvsmqCZZFw46z626lVj9j1yEPW33H5H+lBQpZMP1k8l+78Ha0A==
   dependencies:
     fill-range "^7.0.1"
 
-browserslist@^4.0.0, browserslist@^4.14.5, browserslist@^4.18.1, browserslist@^4.21.10, browserslist@^4.21.4, browserslist@^4.22.2:
+browserslist@^4.0.0, browserslist@^4.18.1, browserslist@^4.21.10, browserslist@^4.21.4, browserslist@^4.22.2:
   version "4.22.2"
   resolved "https://registry.npmjs.org/browserslist/-/browserslist-4.22.2.tgz"
   integrity sha512-0UgcrvQmBDvZHFGdYUehrCNIazki7/lUP3kkoi/r3YB2amZbFM9J43ZRkJTXBUZK4gmx56+Sqk9+Vs9mwZx9+A==
   dependencies:
     caniuse-lite "^1.0.30001565"
     electron-to-chromium "^1.4.601"
     node-releases "^2.0.14"
@@ -2812,15 +2853,15 @@
 buffer-crc32@~0.2.3:
   version "0.2.13"
   resolved "https://registry.npmjs.org/buffer-crc32/-/buffer-crc32-0.2.13.tgz"
   integrity sha512-VO9Ht/+p3SN7SKWqcrgEzjGbRSJYTx+Q1pTQC0wrWqHx0vpJraQ6GtHx8tvcg1rlK1byhU5gccxgOgj7B0TDkQ==
 
 buffer-from@^1.0.0:
   version "1.1.2"
-  resolved "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.2.tgz"
+  resolved "https://registry.yarnpkg.com/buffer-from/-/buffer-from-1.1.2.tgz#2b146a6fd72e80b4f55d255f35ed59a3a9a41bd5"
   integrity sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==
 
 bytes@3.0.0:
   version "3.0.0"
   resolved "https://registry.npmjs.org/bytes/-/bytes-3.0.0.tgz"
   integrity sha512-pMhOfFDPiv9t5jjIXkHosWmkSyQbvsgEVNkz0ERHbuLh2T/7j4Mqqpz523Fe8MVY89KC6Sh/QfS2sM+SjgFDcw==
 
@@ -2885,19 +2926,24 @@
   integrity sha512-bsTwuIg/BZZK/vreVTYYbSWoe2F+71P7K5QGEX+pT250DZbfU1MQ5prOKpPR+LL6uWKK3KMwMCAS74QB3Um1uw==
   dependencies:
     browserslist "^4.0.0"
     caniuse-lite "^1.0.0"
     lodash.memoize "^4.1.2"
     lodash.uniq "^4.5.0"
 
-caniuse-lite@^1.0.0, caniuse-lite@^1.0.30001538, caniuse-lite@^1.0.30001565:
+caniuse-lite@^1.0.0, caniuse-lite@^1.0.30001538:
   version "1.0.30001570"
   resolved "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001570.tgz"
   integrity sha512-+3e0ASu4sw1SWaoCtvPeyXp+5PsjigkSt8OXZbF9StH5pQWbxEjLAZE3n8Aup5udop1uRiKA7a4utUk/uoSpUw==
 
+caniuse-lite@^1.0.30001565:
+  version "1.0.30001605"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001605.tgz#ca12d7330dd8bcb784557eb9aa64f0037870d9d6"
+  integrity sha512-nXwGlFWo34uliI9z3n6Qc0wZaf7zaZWA1CPZ169La5mV3I/gem7bst0vr5XQH5TJXZIMfDeZyOrZnSlVzKxxHQ==
+
 ccount@^2.0.0:
   version "2.0.1"
   resolved "https://registry.npmjs.org/ccount/-/ccount-2.0.1.tgz"
   integrity sha512-eyrF0jiFpY+3drT6383f1qhkbGsLSifNAjA61IUjZjmLCWjItY6LB9ft9YhoDgwfmclB2zhu51Lc7+95b8NRAg==
 
 chalk@^2.4.2:
   version "2.4.2"
@@ -2982,22 +3028,22 @@
     is-binary-path "~2.1.0"
     is-glob "~4.0.1"
     normalize-path "~3.0.0"
     readdirp "~3.6.0"
   optionalDependencies:
     fsevents "~2.3.2"
 
-chownr@^1.1.4:
-  version "1.1.4"
-  resolved "https://registry.npmjs.org/chownr/-/chownr-1.1.4.tgz"
-  integrity sha512-jJ0bqzaylmJtVnNgzTeSOs8DPavpbYgEr/b0YL8/2GO3xJEhInFmhKMUnEJQjZumK7KXGFhUy89PrsJWlakBVg==
+chownr@^2.0.0:
+  version "2.0.0"
+  resolved "https://registry.yarnpkg.com/chownr/-/chownr-2.0.0.tgz#15bfbe53d2eab4cf70f18a8cd68ebe5b3cb1dece"
+  integrity sha512-bIomtDF5KGpdogkLd9VspvFzk9KfpyyGlS8YFVZl7TGPBHL5snIOnxeshwVgPteQ9b4Eydl+pVbIyE1DcvCWgQ==
 
 chrome-trace-event@^1.0.2:
   version "1.0.3"
-  resolved "https://registry.npmjs.org/chrome-trace-event/-/chrome-trace-event-1.0.3.tgz"
+  resolved "https://registry.yarnpkg.com/chrome-trace-event/-/chrome-trace-event-1.0.3.tgz#1015eced4741e15d06664a957dbbf50d041e26ac"
   integrity sha512-p3KULyQg4S7NIHixdwbGX+nFHkoBiA4YQmyWtjb8XngSKV124nJmRysgAeujbUVb15vh+RvFUfCPqU7rXk+hZg==
 
 ci-info@^3.2.0:
   version "3.9.0"
   resolved "https://registry.npmjs.org/ci-info/-/ci-info-3.9.0.tgz"
   integrity sha512-NIxF55hv4nSqQswkAeiOi1r83xy8JldOFDTWiug55KBu9Jnblncd2U6ViHmYgHf01TPZS77NJBhBMKdWj9HQMQ==
 
@@ -3025,15 +3071,15 @@
   dependencies:
     string-width "^4.2.0"
   optionalDependencies:
     "@colors/colors" "1.5.0"
 
 clone-deep@^4.0.1:
   version "4.0.1"
-  resolved "https://registry.npmjs.org/clone-deep/-/clone-deep-4.0.1.tgz"
+  resolved "https://registry.yarnpkg.com/clone-deep/-/clone-deep-4.0.1.tgz#c19fd9bdbbf85942b4fd979c84dcf7d5f07c2387"
   integrity sha512-neHB9xuzh/wk0dIHweyAXv2aPGZIVk3pLMe+/RNzINf17fe0OG96QroktYAUm7SM1PBnzTabaLboqqxDyMU+SQ==
   dependencies:
     is-plain-object "^2.0.4"
     kind-of "^6.0.2"
     shallow-clone "^3.0.0"
 
 clsx@^2.0.0:
@@ -3105,20 +3151,20 @@
 commander@^10.0.0:
   version "10.0.1"
   resolved "https://registry.npmjs.org/commander/-/commander-10.0.1.tgz"
   integrity sha512-y4Mg2tXshplEbSGzx7amzPwKKOCGuoSRP/CjEdwwk0FOGlUbq6lKuoyDZTNZkmxHdJtp54hdfY/JUrdL7Xfdug==
 
 commander@^2.20.0:
   version "2.20.3"
-  resolved "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz"
+  resolved "https://registry.yarnpkg.com/commander/-/commander-2.20.3.tgz#fd485e84c03eb4881c20722ba48035e8531aeb33"
   integrity sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==
 
 commander@^5.1.0:
   version "5.1.0"
-  resolved "https://registry.npmjs.org/commander/-/commander-5.1.0.tgz"
+  resolved "https://registry.yarnpkg.com/commander/-/commander-5.1.0.tgz#46abbd1652f8e059bddaef99bbdcb2ad9cf179ae"
   integrity sha512-P0CysNDQ7rtVw4QIQtm+MRxV66vKFSvlsQvGYXZWR3qFU0jlMKHZZZgw8e+8DSah4UDKMqnknRDQz+xuQXQ/Zg==
 
 commander@^7.2.0:
   version "7.2.0"
   resolved "https://registry.npmjs.org/commander/-/commander-7.2.0.tgz"
   integrity sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==
 
@@ -3194,33 +3240,33 @@
 content-disposition@0.5.4:
   version "0.5.4"
   resolved "https://registry.npmjs.org/content-disposition/-/content-disposition-0.5.4.tgz"
   integrity sha512-FveZTNuGw04cxlAiWbzi6zTAL/lhehaWbTtgluJh4/E95DqMwTmha3KZN1aAWA8cFIhHzMZUvLevkw5Rqk+tSQ==
   dependencies:
     safe-buffer "5.2.1"
 
-content-type@~1.0.4:
+content-type@~1.0.4, content-type@~1.0.5:
   version "1.0.5"
   resolved "https://registry.npmjs.org/content-type/-/content-type-1.0.5.tgz"
   integrity sha512-nTjqfcBFEipKdXCv4YDQWCfmcLZKm81ldF0pAopTvyrFGVbcR6P/VAAd5G7N+0tTr8QqiU0tFadD6FK4NtJwOA==
 
 convert-source-map@^2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/convert-source-map/-/convert-source-map-2.0.0.tgz"
   integrity sha512-Kvp459HrV2FEJ1CAsi1Ku+MY3kasH19TFykTz2xWmMeq6bk2NU3XXvfJ+Q61m0xktWwt+1HSYf3JZsTms3aRJg==
 
 cookie-signature@1.0.6:
   version "1.0.6"
   resolved "https://registry.npmjs.org/cookie-signature/-/cookie-signature-1.0.6.tgz"
   integrity sha512-QADzlaHc8icV8I7vbaJXJwod9HWYp8uCqf1xa4OfNu1T7JVxQIrUgOWtHdNDtPiywmFbiS12VjotIXLrKM3orQ==
 
-cookie@0.5.0:
-  version "0.5.0"
-  resolved "https://registry.npmjs.org/cookie/-/cookie-0.5.0.tgz"
-  integrity sha512-YZ3GUyn/o8gfKJlnlX7g7xq4gyO6OSuhGPKaaGssGB2qgDUS0gPgtTvoyZLTt9Ab6dC4hfc9dV5arkvc/OCmrw==
+cookie@0.6.0:
+  version "0.6.0"
+  resolved "https://registry.yarnpkg.com/cookie/-/cookie-0.6.0.tgz#2798b04b071b0ecbff0dbb62a505a8efa4e19051"
+  integrity sha512-U71cyTamuh1CRNCfpGY6to28lxvNwPG4Guz/EVjgf3Jmzv0vlDp1atT9eS5dDjMYHucpHbWns6Lwf3BKz6svdw==
 
 copy-text-to-clipboard@^3.2.0:
   version "3.2.0"
   resolved "https://registry.npmjs.org/copy-text-to-clipboard/-/copy-text-to-clipboard-3.2.0.tgz"
   integrity sha512-RnJFp1XR/LOBDckxTib5Qjr/PMfkatD0MUCQgdpqS8MdKiNUzBjAQBEN6oUy+jW7LI93BBG3DtMB2KOOKpGs2Q==
 
 copy-webpack-plugin@^11.0.0:
@@ -3442,15 +3488,15 @@
   resolved "https://registry.npmjs.org/csso/-/csso-4.2.0.tgz"
   integrity sha512-wvlcdIbf6pwKEk7vHj8/Bkc0B4ylXZruLvOgs9doS5eOsOpuodOV2zJChSpkp+pRpYQLQMeF04nr3Z68Sta9jA==
   dependencies:
     css-tree "^1.1.2"
 
 csstype@^3.0.2:
   version "3.1.3"
-  resolved "https://registry.npmjs.org/csstype/-/csstype-3.1.3.tgz"
+  resolved "https://registry.yarnpkg.com/csstype/-/csstype-3.1.3.tgz#d80ff294d114fb0e6ac500fbf85b60137d7eff81"
   integrity sha512-M1uQkMl8rQK/szD0LNhtqxIPLpimGm8sOBwU7lLnCpSbTyY3yeU1Vc7l4KT5zT4s/yOxHH5O7tIuuLOCnLADRw==
 
 debounce@^1.2.1:
   version "1.2.1"
   resolved "https://registry.npmjs.org/debounce/-/debounce-1.2.1.tgz"
   integrity sha512-XRRe6Glud4rd/ZGQfiV1ruXSfbvfJedlV9Y6zOlP+2K04vBYiJEte6stfFkCP03aMnY5tsipamumUjL14fofug==
 
@@ -3702,17 +3748,17 @@
 
 ee-first@1.1.1:
   version "1.1.1"
   resolved "https://registry.npmjs.org/ee-first/-/ee-first-1.1.1.tgz"
   integrity sha512-WMwm9LhRUo+WUaRN+vRuETqG89IgZphVSNkdFgeb6sS/E4OrDIN7t48CAewSHXc6C8lefD8KKfr5vY61brQlow==
 
 electron-to-chromium@^1.4.601:
-  version "1.4.614"
-  resolved "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.614.tgz"
-  integrity sha512-X4ze/9Sc3QWs6h92yerwqv7aB/uU8vCjZcrMjA8N9R1pjMFRe44dLsck5FzLilOYvcXuDn93B+bpGYyufc70gQ==
+  version "1.4.725"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.725.tgz#a599369caa3619ca3ba90a61c0ad03e28158681e"
+  integrity sha512-OGkMXLY7XH6ykHE5ZOVVIMHaGAvvxqw98cswTKB683dntBJre7ufm9wouJ0ExDm0VXhHenU8mREvxIbV5nNoVQ==
 
 emoji-regex@^8.0.0:
   version "8.0.0"
   resolved "https://registry.npmjs.org/emoji-regex/-/emoji-regex-8.0.0.tgz"
   integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
 
 emoji-regex@^9.2.2:
@@ -3736,18 +3782,18 @@
   integrity sha512-dqx7eA9YaqyvYtUhJwT4rC1HIp82j5ybS1/vQ42ur+jBe17dJMwZE4+gvL1XadSFfxaPFFGt3Xsw+Y8akThDlw==
 
 encodeurl@~1.0.2:
   version "1.0.2"
   resolved "https://registry.npmjs.org/encodeurl/-/encodeurl-1.0.2.tgz"
   integrity sha512-TPJXq8JqFaVYm2CWmPvnP2Iyo4ZSM7/QKcSmuMLDObfpH5fi7RUGmd/rTDf+rut/saiDiQEeVTNgAmJEdAOx0w==
 
-enhanced-resolve@^5.15.0:
-  version "5.15.0"
-  resolved "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.15.0.tgz"
-  integrity sha512-LXYT42KJ7lpIKECr2mAXIaMldcNCh/7E0KBKOu4KSfkHmP+mZmSs+8V5gBAqisWBy0OO4W5Oyys0GO1Y8KtdKg==
+enhanced-resolve@^5.16.0:
+  version "5.16.0"
+  resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.16.0.tgz#65ec88778083056cb32487faa9aef82ed0864787"
+  integrity sha512-O+QWCviPNSSLAD9Ucn8Awv+poAkqn3T1XY5/N7kR7rQO9yfSGWkYZDwpJ+iKF7B8rxaQKWngSqACpgzeapSyoA==
   dependencies:
     graceful-fs "^4.2.4"
     tapable "^2.2.0"
 
 entities@^2.0.0:
   version "2.2.0"
   resolved "https://registry.npmjs.org/entities/-/entities-2.2.0.tgz"
@@ -3762,22 +3808,22 @@
   version "1.3.2"
   resolved "https://registry.npmjs.org/error-ex/-/error-ex-1.3.2.tgz"
   integrity sha512-7dFHNmqeFSEt2ZBsCriorKnn3Z2pj+fd9kmI6QoWw4//DL+icEBfc0U7qJCisqrTsKTjw4fNFy2pW9OqStD84g==
   dependencies:
     is-arrayish "^0.2.1"
 
 es-module-lexer@^1.2.1:
-  version "1.4.1"
-  resolved "https://registry.npmjs.org/es-module-lexer/-/es-module-lexer-1.4.1.tgz"
-  integrity sha512-cXLGjP0c4T3flZJKQSuziYoq7MlT+rnvfZjfp7h+I7K9BNX54kP9nyWvdbwjQ4u1iWbOL4u96fgeZLToQlZC7w==
+  version "1.5.0"
+  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-1.5.0.tgz#4878fee3789ad99e065f975fdd3c645529ff0236"
+  integrity sha512-pqrTKmwEIgafsYZAGw9kszYzmagcE/n4dbgwGWLEXg7J4QFJVQRBld8j3Q3GNez79jzxZshq0bcT962QHOghjw==
 
 escalade@^3.1.1:
-  version "3.1.1"
-  resolved "https://registry.npmjs.org/escalade/-/escalade-3.1.1.tgz"
-  integrity sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==
+  version "3.1.2"
+  resolved "https://registry.yarnpkg.com/escalade/-/escalade-3.1.2.tgz#54076e9ab29ea5bf3d8f1ed62acffbb88272df27"
+  integrity sha512-ErCHMCae19vR8vQGe50xIsVomy19rg6gFu3+r3jkEO46suLMWBksvVyoGgQV+jOfl84ZSOSlmv6Gxa89PmTGmA==
 
 escape-goat@^4.0.0:
   version "4.0.0"
   resolved "https://registry.npmjs.org/escape-goat/-/escape-goat-4.0.0.tgz"
   integrity sha512-2Sd4ShcWxbx6OY1IHyla/CVNwvg7XwZVoXZHcSu9w9SReNP1EzzD5T8NWKIR38fIqEns9kDWKUQTXXAmlDrdPg==
 
 escape-html@^1.0.3, escape-html@~1.0.3:
@@ -3798,40 +3844,40 @@
 escape-string-regexp@^5.0.0:
   version "5.0.0"
   resolved "https://registry.npmjs.org/escape-string-regexp/-/escape-string-regexp-5.0.0.tgz"
   integrity sha512-/veY75JbMK4j1yjvuUxuVsiS/hr/4iHs9FTT6cgTexxdE0Ly/glccBAkloH/DofkjRbZU3bnoj38mOmhkZ0lHw==
 
 eslint-scope@5.1.1:
   version "5.1.1"
-  resolved "https://registry.npmjs.org/eslint-scope/-/eslint-scope-5.1.1.tgz"
+  resolved "https://registry.yarnpkg.com/eslint-scope/-/eslint-scope-5.1.1.tgz#e786e59a66cb92b3f6c1fb0d508aab174848f48c"
   integrity sha512-2NxwbF/hZ0KpepYN0cNbo+FN6XoK7GaHlQhgx/hIZl6Va0bF45RQOOwhLIy8lQDbuCiadSLCBnH2CFYquit5bw==
   dependencies:
     esrecurse "^4.3.0"
     estraverse "^4.1.1"
 
 esprima@^4.0.0:
   version "4.0.1"
   resolved "https://registry.npmjs.org/esprima/-/esprima-4.0.1.tgz"
   integrity sha512-eGuFFw7Upda+g4p+QHvnW0RyTX/SVeJBDM/gCtMARO0cLuT2HcEKnTPvhjV6aGeqrCB/sbNop0Kszm0jsaWU4A==
 
 esrecurse@^4.3.0:
   version "4.3.0"
-  resolved "https://registry.npmjs.org/esrecurse/-/esrecurse-4.3.0.tgz"
+  resolved "https://registry.yarnpkg.com/esrecurse/-/esrecurse-4.3.0.tgz#7ad7964d679abb28bee72cec63758b1c5d2c9921"
   integrity sha512-KmfKL3b6G+RXvP8N1vr3Tq1kL/oCFgn2NYXEtqP8/L3pKapUA4G8cFVaoF3SU323CD4XypR/ffioHmkti6/Tag==
   dependencies:
     estraverse "^5.2.0"
 
 estraverse@^4.1.1:
   version "4.3.0"
-  resolved "https://registry.npmjs.org/estraverse/-/estraverse-4.3.0.tgz"
+  resolved "https://registry.yarnpkg.com/estraverse/-/estraverse-4.3.0.tgz#398ad3f3c5a24948be7725e83d11a7de28cdbd1d"
   integrity sha512-39nnKffWz8xN1BU/2c79n9nB9HDzo0niYUqx6xyqUnyoAnQyyWpOTdZEeiCch8BBu515t4wp9ZmgVfVhn9EBpw==
 
 estraverse@^5.2.0:
   version "5.3.0"
-  resolved "https://registry.npmjs.org/estraverse/-/estraverse-5.3.0.tgz"
+  resolved "https://registry.yarnpkg.com/estraverse/-/estraverse-5.3.0.tgz#2eea5290702f26ab8fe5370370ff86c965d21123"
   integrity sha512-MMdARuVEQziNTeJD8DgMqmhwR11BRQ/cBP+pLtYdSTnf3MIO8fFeiINEbX36ZdNlfU/7A9f3gUw49B3oQsvwBA==
 
 estree-util-attach-comments@^3.0.0:
   version "3.0.0"
   resolved "https://registry.npmjs.org/estree-util-attach-comments/-/estree-util-attach-comments-3.0.0.tgz"
   integrity sha512-cKUwm/HUcTDsYh/9FgnuFqpfquUbwIqwKM26BVCGDPVgvaCl/nDCCjUfiLlx6lsEZ3Z4RFxNbOQ60pkaEwFxGw==
   dependencies:
@@ -3910,15 +3956,15 @@
 eventemitter3@^4.0.0:
   version "4.0.7"
   resolved "https://registry.npmjs.org/eventemitter3/-/eventemitter3-4.0.7.tgz"
   integrity sha512-8guHBZCwKnFhYdHr2ysuRWErTwhoN2X8XELRlrRwpmfeY2jjuUN4taQMsULKUVo1K4DvZl+0pgfyoysHxvmvEw==
 
 events@^3.2.0:
   version "3.3.0"
-  resolved "https://registry.npmjs.org/events/-/events-3.3.0.tgz"
+  resolved "https://registry.yarnpkg.com/events/-/events-3.3.0.tgz#31a95ad0a924e2d2c419a813aeb2c4e878ea7400"
   integrity sha512-mQw+2fkQbALzQ7V0MY0IqdnXNOeTtP4r0lN9z7AAawCXgqea7bDii20AYrIBrFd/Hx0M2Ocz6S111CaFkUcb0Q==
 
 execa@^5.0.0:
   version "5.1.1"
   resolved "https://registry.npmjs.org/execa/-/execa-5.1.1.tgz"
   integrity sha512-8uSpZZocAZRBAPIEINJj3Lo9HyGitllczc27Eh5YYojjMFMn8yHMDMaUHE2Jqfq05D/wucwI4JGURyXt1vchyg==
   dependencies:
@@ -3929,24 +3975,24 @@
     merge-stream "^2.0.0"
     npm-run-path "^4.0.1"
     onetime "^5.1.2"
     signal-exit "^3.0.3"
     strip-final-newline "^2.0.0"
 
 express@^4.17.3:
-  version "4.18.2"
-  resolved "https://registry.npmjs.org/express/-/express-4.18.2.tgz"
-  integrity sha512-5/PsL6iGPdfQ/lKM1UuielYgv3BUoJfz1aUwU9vHZ+J7gyvwdQXFEBIEIaxeGf0GIcreATNyBExtalisDbuMqQ==
+  version "4.19.2"
+  resolved "https://registry.yarnpkg.com/express/-/express-4.19.2.tgz#e25437827a3aa7f2a827bc8171bbbb664a356465"
+  integrity sha512-5T6nhjsT+EOMzuck8JjBHARTHfMht0POzlA60WV2pMD3gyXw2LZnZ+ueGdNxG+0calOJcWKbpFcuzLZ91YWq9Q==
   dependencies:
     accepts "~1.3.8"
     array-flatten "1.1.1"
-    body-parser "1.20.1"
+    body-parser "1.20.2"
     content-disposition "0.5.4"
     content-type "~1.0.4"
-    cookie "0.5.0"
+    cookie "0.6.0"
     cookie-signature "1.0.6"
     debug "2.6.9"
     depd "2.0.0"
     encodeurl "~1.0.2"
     escape-html "~1.0.3"
     etag "~1.8.1"
     finalhandler "1.2.0"
@@ -3979,15 +4025,15 @@
 extend@^3.0.0:
   version "3.0.2"
   resolved "https://registry.npmjs.org/extend/-/extend-3.0.2.tgz"
   integrity sha512-fjquC59cD7CyW6urNXK0FBufkZcoiGG80wTuPujX590cB5Ttln20E2UB4S/WARVqhXffZl2LNgS+gQdPIIim/g==
 
 fast-deep-equal@^3.1.1, fast-deep-equal@^3.1.3:
   version "3.1.3"
-  resolved "https://registry.npmjs.org/fast-deep-equal/-/fast-deep-equal-3.1.3.tgz"
+  resolved "https://registry.yarnpkg.com/fast-deep-equal/-/fast-deep-equal-3.1.3.tgz#3a7d56b559d6cbc3eb512325244e619a65c6c525"
   integrity sha512-f3qQ9oQy9j2AhBe/H9VC91wLmKBCCU/gDOnKNAYG5hswO7BLKj09Hc5HYNz9cGI++xlpDCIgDaitVs03ATR84Q==
 
 fast-glob@^3.2.11, fast-glob@^3.2.9, fast-glob@^3.3.0:
   version "3.3.2"
   resolved "https://registry.npmjs.org/fast-glob/-/fast-glob-3.3.2.tgz"
   integrity sha512-oX2ruAFQwf/Orj8m737Y5adxDQO0LAB7/S5MnxCdTNDd4p6BsyIVsv9JQsATbTSq8KHRpLwIHbVlUNatxd+1Ow==
   dependencies:
@@ -3995,15 +4041,15 @@
     "@nodelib/fs.walk" "^1.2.3"
     glob-parent "^5.1.2"
     merge2 "^1.3.0"
     micromatch "^4.0.4"
 
 fast-json-stable-stringify@^2.0.0:
   version "2.1.0"
-  resolved "https://registry.npmjs.org/fast-json-stable-stringify/-/fast-json-stable-stringify-2.1.0.tgz"
+  resolved "https://registry.yarnpkg.com/fast-json-stable-stringify/-/fast-json-stable-stringify-2.1.0.tgz#874bf69c6f404c2b5d99c481341399fd55892633"
   integrity sha512-lhd/wF+Lk98HZoTCtlVraHtfh5XYijIjalXck7saUtuanSDyLMxnHhSXEDJqHxD7msR8D0uCmqlkwjCV8xvwHw==
 
 fast-url-parser@1.1.3:
   version "1.1.3"
   resolved "https://registry.npmjs.org/fast-url-parser/-/fast-url-parser-1.1.3.tgz"
   integrity sha512-5jOCVXADYNuRkKFzNJ0dCCewsZiYo0dz8QNYljkOpFC6r2U4OBmKtvm/Tsuh4w1YYdDqDb31a8TVhBJ2OJKdqQ==
   dependencies:
@@ -4026,21 +4072,14 @@
 faye-websocket@^0.11.3:
   version "0.11.4"
   resolved "https://registry.npmjs.org/faye-websocket/-/faye-websocket-0.11.4.tgz"
   integrity sha512-CzbClwlXAuiRQAlUyfqPgvPoNKTckTPGfwZV4ZdAhVcP2lh9KUxJg2b5GkE7XbjKQ3YJnQ9z6D9ntLAlB+tP8g==
   dependencies:
     websocket-driver ">=0.5.1"
 
-fd-slicer@~1.1.0:
-  version "1.1.0"
-  resolved "https://registry.npmjs.org/fd-slicer/-/fd-slicer-1.1.0.tgz"
-  integrity sha512-cE1qsB/VwyQozZ+q1dGxR8LBYNZeofhEdUNGSMbQD3Gw2lAzX9Zb3uIU6Ebc/Fmyjo9AWWfnn0AUCHqtevs/8g==
-  dependencies:
-    pend "~1.2.0"
-
 feed@^4.2.2:
   version "4.2.2"
   resolved "https://registry.npmjs.org/feed/-/feed-4.2.2.tgz"
   integrity sha512-u5/sxGfiMfZNtJ3OvQpXcvotFpYkL0n9u9mM2vkui2nGo8b4wvDkJ8gAkYqbA8QpGyFCv3RK0Z+Iv+9veCS9bQ==
   dependencies:
     xml-js "^1.6.11"
 
@@ -4106,21 +4145,21 @@
   integrity sha512-v2ZsoEuVHYy8ZIlYqwPe/39Cy+cFDzp4dXPaxNvkEuouymu+2Jbz0PxpKarJHYJTmv2HWT3O382qY8l4jMWthw==
   dependencies:
     locate-path "^7.1.0"
     path-exists "^5.0.0"
 
 flat@^5.0.2:
   version "5.0.2"
-  resolved "https://registry.npmjs.org/flat/-/flat-5.0.2.tgz"
+  resolved "https://registry.yarnpkg.com/flat/-/flat-5.0.2.tgz#8ca6fe332069ffa9d324c327198c598259ceb241"
   integrity sha512-b6suED+5/3rTpUBdG1gupIl8MPFCAMA0QXwmljLhvCUKcUvdE4gWky9zpuGCcXHOsz4J9wPGNWq6OKpmIzz3hQ==
 
 follow-redirects@^1.0.0, follow-redirects@^1.15.0:
-  version "1.15.4"
-  resolved "https://registry.yarnpkg.com/follow-redirects/-/follow-redirects-1.15.4.tgz#cdc7d308bf6493126b17ea2191ea0ccf3e535adf"
-  integrity sha512-Cr4D/5wlrb0z9dgERpUL3LrmPKVDsETIJhaCMeDfuFYcqa5bldGV6wBsAN6X/vxlXQtFBMrXdXxdL8CbDTGniw==
+  version "1.15.6"
+  resolved "https://registry.yarnpkg.com/follow-redirects/-/follow-redirects-1.15.6.tgz#7f815c0cda4249c74ff09e95ef97c23b5fd0399b"
+  integrity sha512-wWN62YITEaOpSK584EZXJafH1AGpO8RVgElfkuXbTOrPX4fIfOyEpW/CsiNd8JdYrAoOvafRTOEnvsO++qCqFA==
 
 fork-ts-checker-webpack-plugin@^6.5.0:
   version "6.5.3"
   resolved "https://registry.npmjs.org/fork-ts-checker-webpack-plugin/-/fork-ts-checker-webpack-plugin-6.5.3.tgz"
   integrity sha512-SbH/l9ikmMWycd5puHJKTkZJKddF4iRLyW3DeZ08HTI7NGyLS38MXd/KGgeWumQO7YNQbW2u/NtPT2YowbPaGQ==
   dependencies:
     "@babel/code-frame" "^7.8.3"
@@ -4186,20 +4225,20 @@
   integrity sha512-hcg3ZmepS30/7BSFqRvoo3DOMQu7IjqxO5nCDt+zM9XWjb33Wg7ziNT+Qvqbuc3+gWpzO02JubVyk2G4Zvo1OQ==
   dependencies:
     at-least-node "^1.0.0"
     graceful-fs "^4.2.0"
     jsonfile "^6.0.1"
     universalify "^2.0.0"
 
-fs-minipass@^1.2.7:
-  version "1.2.7"
-  resolved "https://registry.npmjs.org/fs-minipass/-/fs-minipass-1.2.7.tgz"
-  integrity sha512-GWSSJGFy4e9GUeCcbIkED+bgAoFyj7XF1mV8rma3QW4NIqX9Kyx79N/PF61H5udOV3aY1IaMLs6pGbH71nlCTA==
+fs-minipass@^2.0.0:
+  version "2.1.0"
+  resolved "https://registry.yarnpkg.com/fs-minipass/-/fs-minipass-2.1.0.tgz#7f5036fdbf12c63c169190cbe4199c852271f9fb"
+  integrity sha512-V/JgOLFCS+R6Vcq0slCuaeWEdNC3ouDlJMNIsacH2VtALiu9mV4LPrHc5cDl8k5aw6J8jwgWWpiTo5RYhmIzvg==
   dependencies:
-    minipass "^2.6.0"
+    minipass "^3.0.0"
 
 fs-monkey@^1.0.4:
   version "1.0.5"
   resolved "https://registry.npmjs.org/fs-monkey/-/fs-monkey-1.0.5.tgz"
   integrity sha512-8uMbBjrhzW76TYgEV27Y5E//W2f/lTFmx78P2w19FZSxarhI/798APGQyuGCwmkNxgwGRhrLfvWyLBvNtuOmew==
 
 fs.realpath@^1.0.0:
@@ -4259,15 +4298,15 @@
   resolved "https://registry.npmjs.org/glob-parent/-/glob-parent-6.0.2.tgz"
   integrity sha512-XxwI8EOhVQgWp6iDL+3b0r86f4d6AX6zSU55HfB4ydCEuXLXc5FcYeOu+nnGftS4TEju/11rt4KJPTMgbfmv4A==
   dependencies:
     is-glob "^4.0.3"
 
 glob-to-regexp@^0.4.1:
   version "0.4.1"
-  resolved "https://registry.npmjs.org/glob-to-regexp/-/glob-to-regexp-0.4.1.tgz"
+  resolved "https://registry.yarnpkg.com/glob-to-regexp/-/glob-to-regexp-0.4.1.tgz#c75297087c851b9a578bd217dd59a92f59fe546e"
   integrity sha512-lkX1HJXwyMcprw/5YUZc2s7DrpAiHB21/V+E1rHUrVNokkvB6bqMzT0VfV6/86ZNabt1k14YOIaT7nDvOX3Iiw==
 
 glob@^7.0.0, glob@^7.1.3, glob@^7.1.6:
   version "7.2.3"
   resolved "https://registry.npmjs.org/glob/-/glob-7.2.3.tgz"
   integrity sha512-nFR0zLpU2YCaRxwoCJvL6UvCH2JFyFVIvwTLsIf21AuHlMskA1hhTdk+LlYJtOlYt9v6dvszD2BGRqBL+iQK9Q==
   dependencies:
@@ -4354,17 +4393,17 @@
     responselike "^3.0.0"
 
 graceful-fs@4.2.10:
   version "4.2.10"
   resolved "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.10.tgz"
   integrity sha512-9ByhssR2fPVsNZj478qUUbKfmL0+t5BDVyjShtyZZLiK7ZDAArFFfopyOTj0M05wE2tJPisA4iTnnXl2YoPvOA==
 
-graceful-fs@^4.1.2, graceful-fs@^4.1.6, graceful-fs@^4.2.0, graceful-fs@^4.2.4, graceful-fs@^4.2.6, graceful-fs@^4.2.9:
+graceful-fs@^4.1.2, graceful-fs@^4.1.6, graceful-fs@^4.2.0, graceful-fs@^4.2.11, graceful-fs@^4.2.4, graceful-fs@^4.2.6, graceful-fs@^4.2.9:
   version "4.2.11"
-  resolved "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.11.tgz"
+  resolved "https://registry.yarnpkg.com/graceful-fs/-/graceful-fs-4.2.11.tgz#4183e4e8bf08bb6e05bbb2f7d2e0c8f712ca40e3"
   integrity sha512-RbJ5/jmFcNNCcDV5o9eTnBLJ/HszWV0P73bc+Ff4nS/rJj+YaS6IGyiOL0VoBYX+l1Wrl3k63h/KrH+nhJ0XvQ==
 
 gray-matter@^4.0.3:
   version "4.0.3"
   resolved "https://registry.npmjs.org/gray-matter/-/gray-matter-4.0.3.tgz"
   integrity sha512-5v6yZd4JK3eMI3FqqCouswVqwugaA9r4dNZB1wwcmrD02QkV5H0y7XBQW8QwQqEaZY1pM9aqORSORhJRdNK44Q==
   dependencies:
@@ -4388,15 +4427,15 @@
 has-flag@^3.0.0:
   version "3.0.0"
   resolved "https://registry.npmjs.org/has-flag/-/has-flag-3.0.0.tgz"
   integrity sha512-sKJf1+ceQBr4SMkvQnBDNDtf4TXpVhVGateu0t918bl30FnbE2m4vNLX+VWe/dpjlb+HugGYzW7uQXH98HPEYw==
 
 has-flag@^4.0.0:
   version "4.0.0"
-  resolved "https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz"
+  resolved "https://registry.yarnpkg.com/has-flag/-/has-flag-4.0.0.tgz#944771fd9c81c81265c4d6941860da06bb59479b"
   integrity sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==
 
 has-property-descriptors@^1.0.0:
   version "1.0.1"
   resolved "https://registry.npmjs.org/has-property-descriptors/-/has-property-descriptors-1.0.1.tgz"
   integrity sha512-VsX8eaIewvas0xnvinAe9bw4WfIeODpGYikiWYLH+dma0Jw6KHYqWiWfhQlgOVK8D6PvjubK5Uc4P0iIhIcNVg==
   dependencies:
@@ -4816,15 +4855,15 @@
 interpret@^1.0.0:
   version "1.4.0"
   resolved "https://registry.npmjs.org/interpret/-/interpret-1.4.0.tgz"
   integrity sha512-agE4QfB2Lkp9uICn7BAqoscw4SZP9kTE2hxiFI3jBPmXJfdqiahTbUuKGsMoN2GtqL9AxhYioAcVvgsb1HvRbA==
 
 invariant@^2.2.4:
   version "2.2.4"
-  resolved "https://registry.npmjs.org/invariant/-/invariant-2.2.4.tgz"
+  resolved "https://registry.yarnpkg.com/invariant/-/invariant-2.2.4.tgz#610f3c92c9359ce1db616e538008d23ff35158e6"
   integrity sha512-phJfQVBuaJM5raOpJjSfkiD6BpbCE4Ns//LaXl6wGYtUBY83nWS6Rf9tXm2e8VaK60JEjYldbPif/A2B1C2gNA==
   dependencies:
     loose-envify "^1.0.0"
 
 ipaddr.js@1.9.1:
   version "1.9.1"
   resolved "https://registry.npmjs.org/ipaddr.js/-/ipaddr.js-1.9.1.tgz"
@@ -4957,15 +4996,15 @@
 is-plain-obj@^4.0.0:
   version "4.1.0"
   resolved "https://registry.npmjs.org/is-plain-obj/-/is-plain-obj-4.1.0.tgz"
   integrity sha512-+Pgi+vMuUNkJyExiMBt5IlFoMyKnr5zhJ4Uspz58WOhBF5QoIZkFyNHIbBAtHwzVAgk5RtndVNsDRN61/mmDqg==
 
 is-plain-object@^2.0.4:
   version "2.0.4"
-  resolved "https://registry.npmjs.org/is-plain-object/-/is-plain-object-2.0.4.tgz"
+  resolved "https://registry.yarnpkg.com/is-plain-object/-/is-plain-object-2.0.4.tgz#2c163b3fafb1b606d9d17928f05c2a1c38e07677"
   integrity sha512-h5PpgXkWitc38BBMYawTYMWJHFZJVnBquFE57xFpjB8pJFiF6gZ+bU+WyI/yqXiFR5mdLsgYNaPe8uao6Uv9Og==
   dependencies:
     isobject "^3.0.1"
 
 is-plain-object@^5.0.0:
   version "5.0.0"
   resolved "https://registry.npmjs.org/is-plain-object/-/is-plain-object-5.0.0.tgz"
@@ -5023,15 +5062,15 @@
 isexe@^2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/isexe/-/isexe-2.0.0.tgz"
   integrity sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==
 
 isobject@^3.0.1:
   version "3.0.1"
-  resolved "https://registry.npmjs.org/isobject/-/isobject-3.0.1.tgz"
+  resolved "https://registry.yarnpkg.com/isobject/-/isobject-3.0.1.tgz#4e431e92b11a9731636aa1f9c8d1ccbcfdab78df"
   integrity sha512-WhB9zCku7EGTj/HQQRz5aUQEUeoQZH2bWcltRErOpymJ4boYE6wL9Tbr23krRPSZ+C5zqNSrSw+Cc7sZZ4b7vg==
 
 jest-util@^29.7.0:
   version "29.7.0"
   resolved "https://registry.npmjs.org/jest-util/-/jest-util-29.7.0.tgz"
   integrity sha512-z6EbKajIpqGKU56y5KBUgy1dt1ihhQJgWzUlZHArA/+X2ad7Cb5iF+AK1EWVL/Bo7Rz9uurpqw6SiBCefUbCGA==
   dependencies:
@@ -5040,15 +5079,15 @@
     chalk "^4.0.0"
     ci-info "^3.2.0"
     graceful-fs "^4.2.9"
     picomatch "^2.2.3"
 
 jest-worker@^27.4.5:
   version "27.5.1"
-  resolved "https://registry.npmjs.org/jest-worker/-/jest-worker-27.5.1.tgz"
+  resolved "https://registry.yarnpkg.com/jest-worker/-/jest-worker-27.5.1.tgz#8d146f0900e8973b106b6f73cc1e9a8cb86f8db0"
   integrity sha512-7vuh85V5cdDofPyxn58nrPjBktZo0u9x1g8WtjQol+jZDaE+fhN+cIvTj11GndBnMnyfrUOG1sZQxCdjKh+DKg==
   dependencies:
     "@types/node" "*"
     merge-stream "^2.0.0"
     supports-color "^8.0.0"
 
 jest-worker@^29.1.2:
@@ -5063,27 +5102,27 @@
 
 jiti@^1.18.2, jiti@^1.20.0:
   version "1.21.0"
   resolved "https://registry.npmjs.org/jiti/-/jiti-1.21.0.tgz"
   integrity sha512-gFqAIbuKyyso/3G2qhiO2OM6shY6EPP/R0+mkDbyspxKazh8BXDC5FiFsUjlczgdNz/vfra0da2y+aHrusLG/Q==
 
 joi@^17.9.2:
-  version "17.11.0"
-  resolved "https://registry.npmjs.org/joi/-/joi-17.11.0.tgz"
-  integrity sha512-NgB+lZLNoqISVy1rZocE9PZI36bL/77ie924Ri43yEvi9GUUMPeyVIr8KdFTMUlby1p0PBYMk9spIxEUQYqrJQ==
-  dependencies:
-    "@hapi/hoek" "^9.0.0"
-    "@hapi/topo" "^5.0.0"
-    "@sideway/address" "^4.1.3"
+  version "17.12.3"
+  resolved "https://registry.yarnpkg.com/joi/-/joi-17.12.3.tgz#944646979cd3b460178547b12ba37aca8482f63d"
+  integrity sha512-2RRziagf555owrm9IRVtdKynOBeITiDpuZqIpgwqXShPncPKNiRQoiGsl/T8SQdq+8ugRzH2LqY67irr2y/d+g==
+  dependencies:
+    "@hapi/hoek" "^9.3.0"
+    "@hapi/topo" "^5.1.0"
+    "@sideway/address" "^4.1.5"
     "@sideway/formula" "^3.0.1"
     "@sideway/pinpoint" "^2.0.0"
 
 "js-tokens@^3.0.0 || ^4.0.0", js-tokens@^4.0.0:
   version "4.0.0"
-  resolved "https://registry.npmjs.org/js-tokens/-/js-tokens-4.0.0.tgz"
+  resolved "https://registry.yarnpkg.com/js-tokens/-/js-tokens-4.0.0.tgz#19203fb59991df98e3a287050d4647cdeaf32499"
   integrity sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==
 
 js-yaml@^3.13.1:
   version "3.14.1"
   resolved "https://registry.npmjs.org/js-yaml/-/js-yaml-3.14.1.tgz"
   integrity sha512-okMH7OXXJ7YrN9Ok3/SXrnu4iX9yOk+25nqX4imS2npuvTYDmo/QEZoqwZkYaIDk3jVvBOTOIEgEhaLOynBS9g==
   dependencies:
@@ -5110,20 +5149,20 @@
 json-buffer@3.0.1:
   version "3.0.1"
   resolved "https://registry.npmjs.org/json-buffer/-/json-buffer-3.0.1.tgz"
   integrity sha512-4bV5BfR2mqfQTJm+V5tPPdf+ZpuhiIvTuAB5g8kcrXOZpTT/QwwVRWBywX1ozr6lEuPdbHxwaJlm9G6mI2sfSQ==
 
 json-parse-even-better-errors@^2.3.0, json-parse-even-better-errors@^2.3.1:
   version "2.3.1"
-  resolved "https://registry.npmjs.org/json-parse-even-better-errors/-/json-parse-even-better-errors-2.3.1.tgz"
+  resolved "https://registry.yarnpkg.com/json-parse-even-better-errors/-/json-parse-even-better-errors-2.3.1.tgz#7c47805a94319928e05777405dc12e1f7a4ee02d"
   integrity sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==
 
 json-schema-traverse@^0.4.1:
   version "0.4.1"
-  resolved "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz"
+  resolved "https://registry.yarnpkg.com/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz#69f6a87d9513ab8bb8fe63bdb0979c448e684660"
   integrity sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==
 
 json-schema-traverse@^1.0.0:
   version "1.0.0"
   resolved "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz"
   integrity sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==
 
@@ -5146,15 +5185,15 @@
   resolved "https://registry.npmjs.org/keyv/-/keyv-4.5.4.tgz"
   integrity sha512-oxVHkHR/EJf2CNXnWxRLW6mg7JyCCUcG0DtEGmL2ctUo1PNTin1PUil+r/+4r5MpVgC/fn1kjsx7mjSujKqIpw==
   dependencies:
     json-buffer "3.0.1"
 
 kind-of@^6.0.0, kind-of@^6.0.2:
   version "6.0.3"
-  resolved "https://registry.npmjs.org/kind-of/-/kind-of-6.0.3.tgz"
+  resolved "https://registry.yarnpkg.com/kind-of/-/kind-of-6.0.3.tgz#07c05034a6c349fa06e24fa35aa76db4580ce4dd"
   integrity sha512-dcS1ul+9tmeD95T+x28/ehLgd9mENa3LsvDTtzm3vyBEO7RPptvAD+t44WVXaUjTBRcrpFeFlC8WCruUR456hw==
 
 kleur@^3.0.3:
   version "3.0.3"
   resolved "https://registry.npmjs.org/kleur/-/kleur-3.0.3.tgz"
   integrity sha512-eTIzlVOSUR+JxdDFepEYcBMtZ9Qqdef+rnzWdRZuMbOywu5tO2w2N7rqjoANZ5k9vywhL6Br1VRjUIgTQx4E8w==
 
@@ -5186,15 +5225,15 @@
 lines-and-columns@^1.1.6:
   version "1.2.4"
   resolved "https://registry.npmjs.org/lines-and-columns/-/lines-and-columns-1.2.4.tgz"
   integrity sha512-7ylylesZQ/PV29jhEDl3Ufjo6ZX7gCqJr5F7PKrqc93v7fzSymt1BpwEU8nAUXs8qzzvqhbjhK5QZg6Mt/HkBg==
 
 loader-runner@^4.2.0:
   version "4.3.0"
-  resolved "https://registry.npmjs.org/loader-runner/-/loader-runner-4.3.0.tgz"
+  resolved "https://registry.yarnpkg.com/loader-runner/-/loader-runner-4.3.0.tgz#c1b4a163b99f614830353b16755e7149ac2314e1"
   integrity sha512-3R/1M+yS3j5ou80Me59j7F9IMs4PXs3VqRrm0TU3AbKPxlmpoY1TNscJV/oGJXo8qCatFGTfDbY6W6ipGOYXfg==
 
 loader-utils@^2.0.0:
   version "2.0.4"
   resolved "https://registry.npmjs.org/loader-utils/-/loader-utils-2.0.4.tgz"
   integrity sha512-xXqpXoINfFhgua9xiqD8fPFHgkoq1mmmpE92WlDbm9rNRd/EbRb+Gqf908T2DMfuHjjJlksiK2RbHVOdD/MqSw==
   dependencies:
@@ -5533,15 +5572,15 @@
 merge-descriptors@1.0.1:
   version "1.0.1"
   resolved "https://registry.npmjs.org/merge-descriptors/-/merge-descriptors-1.0.1.tgz"
   integrity sha512-cCi6g3/Zr1iqQi6ySbseM1Xvooa98N0w31jzUYrXPX2xqObmFGHJ0tQ5u74H3mVh7wLouTseZyYIq39g8cNp1w==
 
 merge-stream@^2.0.0:
   version "2.0.0"
-  resolved "https://registry.npmjs.org/merge-stream/-/merge-stream-2.0.0.tgz"
+  resolved "https://registry.yarnpkg.com/merge-stream/-/merge-stream-2.0.0.tgz#52823629a14dd00c9770fb6ad47dc6310f2c1f60"
   integrity sha512-abv/qOcuPfk3URPfDzmZU1LKmuw8kT+0nIHvKrKgFrwifol/doWcdA4ZqsWQ8ENrFKkd67Mfpo/LovbIUsbt3w==
 
 merge2@^1.3.0, merge2@^1.4.1:
   version "1.4.1"
   resolved "https://registry.npmjs.org/merge2/-/merge2-1.4.1.tgz"
   integrity sha512-8q7VEgMJW4J8tcfVPy8g09NcQwZdbwFEqhe/WZkoIzjn/3TGDwtOCYtXGxA3O8tPzpczCCDgv+P2P5y00ZJOOg==
 
@@ -5972,15 +6011,15 @@
   integrity sha512-DMy+ERcEW2q8Z2Po+WNXuw3c5YaUSFjAO5GsJqfEl7UjvtIuFKO6ZrKvcItdy98dwFI2N1tg3zNIdKaQT+aNdA==
   dependencies:
     braces "^3.0.2"
     picomatch "^2.3.1"
 
 mime-db@1.52.0, "mime-db@>= 1.43.0 < 2":
   version "1.52.0"
-  resolved "https://registry.npmjs.org/mime-db/-/mime-db-1.52.0.tgz"
+  resolved "https://registry.yarnpkg.com/mime-db/-/mime-db-1.52.0.tgz#bbabcdc02859f4987301c856e3387ce5ec43bf70"
   integrity sha512-sPU4uV7dYlvtWJxwwxHD0PuihVNiE7TyAbQ5SWxDCB9mUYvOgroQOwYQQOKPJ8CIbE+1ETVlOoK1UC2nU3gYvg==
 
 mime-db@~1.33.0:
   version "1.33.0"
   resolved "https://registry.npmjs.org/mime-db/-/mime-db-1.33.0.tgz"
   integrity sha512-BHJ/EKruNIqJf/QahvxwQZXKygOQ256myeN/Ew+THcAa5q+PjyTTMMeNQC4DZw5AwfvelsUrA6B67NKMqXDbzQ==
 
@@ -6033,40 +6072,43 @@
 minimatch@3.1.2, minimatch@^3.0.4, minimatch@^3.0.5, minimatch@^3.1.1:
   version "3.1.2"
   resolved "https://registry.npmjs.org/minimatch/-/minimatch-3.1.2.tgz"
   integrity sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==
   dependencies:
     brace-expansion "^1.1.7"
 
-minimist@^1.2.0, minimist@^1.2.6:
+minimist@^1.2.0:
   version "1.2.8"
   resolved "https://registry.npmjs.org/minimist/-/minimist-1.2.8.tgz"
   integrity sha512-2yyAR8qBkN3YuheJanUpWC5U3bb5osDywNB8RzDVlDwDHbocAJveqqj1u8+SVD7jkWT4yvsHCpWqqWqAxb0zCA==
 
-minipass@^2.6.0, minipass@^2.9.0:
-  version "2.9.0"
-  resolved "https://registry.npmjs.org/minipass/-/minipass-2.9.0.tgz"
-  integrity sha512-wxfUjg9WebH+CUDX/CdbRlh5SmfZiy/hpkxaRI16Y9W56Pa75sWgd/rvFilSgrauD9NyFymP/+JFV3KwzIsJeg==
+minipass@^3.0.0:
+  version "3.3.6"
+  resolved "https://registry.yarnpkg.com/minipass/-/minipass-3.3.6.tgz#7bba384db3a1520d18c9c0e5251c3444e95dd94a"
+  integrity sha512-DxiNidxSEK+tHG6zOIklvNOwm3hvCrbUrdtzY74U6HKTJxvIDfOUL5W5P2Ghd3DTkhhKPYGqeNUIh5qcM4YBfw==
   dependencies:
-    safe-buffer "^5.1.2"
-    yallist "^3.0.0"
+    yallist "^4.0.0"
 
-minizlib@^1.3.3:
-  version "1.3.3"
-  resolved "https://registry.npmjs.org/minizlib/-/minizlib-1.3.3.tgz"
-  integrity sha512-6ZYMOEnmVsdCeTJVE0W9ZD+pVnE8h9Hma/iOwwRDsdQoePpoX56/8B6z3P9VNwppJuBKNRuFDRNRqRWexT9G9Q==
-  dependencies:
-    minipass "^2.9.0"
+minipass@^5.0.0:
+  version "5.0.0"
+  resolved "https://registry.yarnpkg.com/minipass/-/minipass-5.0.0.tgz#3e9788ffb90b694a5d0ec94479a45b5d8738133d"
+  integrity sha512-3FnjYuehv9k6ovOEbyOswadCDPX1piCfhV8ncmYtHOjuPwylVWsghTLo7rabjC3Rx5xD4HDx8Wm1xnMF7S5qFQ==
 
-mkdirp@^0.5.5:
-  version "0.5.6"
-  resolved "https://registry.npmjs.org/mkdirp/-/mkdirp-0.5.6.tgz"
-  integrity sha512-FP+p8RB8OWpF3YZBCrP5gtADmtXApB5AMLn+vdyA+PyxCjrCs00mjyUozssO33cwDeT3wNGdLxJ5M//YqtHAJw==
+minizlib@^2.1.1:
+  version "2.1.2"
+  resolved "https://registry.yarnpkg.com/minizlib/-/minizlib-2.1.2.tgz#e90d3466ba209b932451508a11ce3d3632145931"
+  integrity sha512-bAxsR8BVfj60DWXHE3u30oHzfl4G7khkSuPW+qvpd7jFRHm7dLxOjUk1EHACJ/hxLY8phGJ0YhYHZo7jil7Qdg==
   dependencies:
-    minimist "^1.2.6"
+    minipass "^3.0.0"
+    yallist "^4.0.0"
+
+mkdirp@^1.0.3:
+  version "1.0.4"
+  resolved "https://registry.yarnpkg.com/mkdirp/-/mkdirp-1.0.4.tgz#3eb5ed62622756d79a5f0e2a221dfebad75c2f7e"
+  integrity sha512-vVqVZQyf3WLx2Shd0qJ9xuvqgAyKPLAiqITEtqW0oIUjzo3PePDd6fW9iFz30ef7Ysp/oiWqbhszeGWW2T6Gzw==
 
 mrmime@^1.0.0:
   version "1.0.1"
   resolved "https://registry.npmjs.org/mrmime/-/mrmime-1.0.1.tgz"
   integrity sha512-hzzEagAgDyoU1Q6yg5uI+AorQgdvMCur3FcKf7NhMKWsaYg+RnbTyHRa/9IlLF9rf455MOCtcqqrQQ83pPP7Uw==
 
 ms@2.0.0:
@@ -6100,15 +6142,15 @@
 negotiator@0.6.3:
   version "0.6.3"
   resolved "https://registry.npmjs.org/negotiator/-/negotiator-0.6.3.tgz"
   integrity sha512-+EUsqGPLsM+j/zdChZjsnX51g4XrHFOIXwfnCVPGlQk/k5giakcKsuxCObBRu6DSm9opw/O6slWbJdghQM4bBg==
 
 neo-async@^2.6.2:
   version "2.6.2"
-  resolved "https://registry.npmjs.org/neo-async/-/neo-async-2.6.2.tgz"
+  resolved "https://registry.yarnpkg.com/neo-async/-/neo-async-2.6.2.tgz#b4aafb93e3aeb2d8174ca53cf163ab7d7308305f"
   integrity sha512-Yd3UES5mWCSqR+qNT93S3UoYUkqAZ9lLg8a7g9rimsWmYGK8cVToA4/sF3RrshdyV3sAGMXVUmpMYOw+dLpOuw==
 
 no-case@^3.0.4:
   version "3.0.4"
   resolved "https://registry.npmjs.org/no-case/-/no-case-3.0.4.tgz"
   integrity sha512-fgAN3jGAh+RoxUGZHTSOLJIqUc2wmoBwGR4tbpNAKmmovFoWq0OdRkb0VkldReO2a2iBT/OEulG9XSUc10r3zg==
   dependencies:
@@ -6121,29 +6163,29 @@
   integrity sha512-E2WEOVsgs7O16zsURJ/eH8BqhF029wGpEOnv7Urwdo2wmQanOACwJQh0devF9D9RhoZru0+9JXIS0dBXIAz+lA==
   dependencies:
     "@sindresorhus/is" "^4.6.0"
     char-regex "^1.0.2"
     emojilib "^2.4.0"
     skin-tone "^2.0.0"
 
-node-fetch@2.6.7:
-  version "2.6.7"
-  resolved "https://registry.npmjs.org/node-fetch/-/node-fetch-2.6.7.tgz"
-  integrity sha512-ZjMPFEfVx5j+y2yF35Kzx5sF7kDzxuDj6ziH4FFbOp87zKDZNx8yExJIb05OGF4Nlt9IHFIMBkRl41VdvcNdbQ==
+node-fetch@2.7.0:
+  version "2.7.0"
+  resolved "https://registry.yarnpkg.com/node-fetch/-/node-fetch-2.7.0.tgz#d0f0fa6e3e2dc1d27efcd8ad99d550bda94d187d"
+  integrity sha512-c4FRfUm/dbcWZ7U+1Wq0AwCyFL+3nt2bEw05wfxSz+DWpWsitgmSgYmy2dQdWyKC1694ELPqMs/YzUSNozLt8A==
   dependencies:
     whatwg-url "^5.0.0"
 
 node-forge@^1:
   version "1.3.1"
   resolved "https://registry.npmjs.org/node-forge/-/node-forge-1.3.1.tgz"
   integrity sha512-dPEtOeMvF9VMcYV/1Wb8CPoVAXtp6MKMlcbAt4ddqmGqUJ6fQZFXkNZNkNlfevtNkGtaSoXf/vNNNSvgrdXwtA==
 
 node-releases@^2.0.14:
   version "2.0.14"
-  resolved "https://registry.npmjs.org/node-releases/-/node-releases-2.0.14.tgz"
+  resolved "https://registry.yarnpkg.com/node-releases/-/node-releases-2.0.14.tgz#2ffb053bceb8b2be8495ece1ab6ce600c4461b0b"
   integrity sha512-y10wOWt8yZpqXmOgRo77WaHEmhYQYGNA6y421PKsKYWEK8aW+cqAphborZDhqfyKrbZEN92CN1X2KbafY2s7Yw==
 
 normalize-path@^3.0.0, normalize-path@~3.0.0:
   version "3.0.0"
   resolved "https://registry.npmjs.org/normalize-path/-/normalize-path-3.0.0.tgz"
   integrity sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==
 
@@ -6179,15 +6221,15 @@
   resolved "https://registry.npmjs.org/nth-check/-/nth-check-2.1.1.tgz"
   integrity sha512-lqjrjmaOoAnWfMmBPL+XNnynZh2+swxiX3WUE0s4yEHI6m+AwrK2UZOimIRl3X/4QctVqS8AiZjFqyOGrMXb/w==
   dependencies:
     boolbase "^1.0.0"
 
 object-assign@^4.1.1:
   version "4.1.1"
-  resolved "https://registry.npmjs.org/object-assign/-/object-assign-4.1.1.tgz"
+  resolved "https://registry.yarnpkg.com/object-assign/-/object-assign-4.1.1.tgz#2109adc7965887cfc05cbbd442cac8bfbb360863"
   integrity sha512-rJgTQnkUnH1sFw8yT6VSU3zD3sWmu6sZhIseY8VX+GRu3P6F7Fu+JNDoXfklElbLJSnc3FUQHVe4cU5hj+BcUg==
 
 object-inspect@^1.9.0:
   version "1.13.1"
   resolved "https://registry.npmjs.org/object-inspect/-/object-inspect-1.13.1.tgz"
   integrity sha512-5qoj1RUiKOMsCCNLV1CBiPYE10sziTsnmNxkAI/rZhiD63CF7IqdFGC/XzjWjpSgLf0LxXX3bDFIh0E18f6UhQ==
 
@@ -6469,15 +6511,15 @@
   dependencies:
     "@types/estree" "^1.0.0"
     estree-walker "^3.0.0"
     is-reference "^3.0.0"
 
 picocolors@^1.0.0:
   version "1.0.0"
-  resolved "https://registry.npmjs.org/picocolors/-/picocolors-1.0.0.tgz"
+  resolved "https://registry.yarnpkg.com/picocolors/-/picocolors-1.0.0.tgz#cb5bdc74ff3f51892236eaf79d68bc44564ab81c"
   integrity sha512-1fygroTLlHu66zi26VoTDv8yRgm0Fccecssto+MhsZ0D/DGW2sm8E8AjW7NU5VVTRt5GxbeZ5qBuJr+HyLYkjQ==
 
 picomatch@^2.0.4, picomatch@^2.2.1, picomatch@^2.2.3, picomatch@^2.3.1:
   version "2.3.1"
   resolved "https://registry.npmjs.org/picomatch/-/picomatch-2.3.1.tgz"
   integrity sha512-JU3teHTNjmE2VCGFzuY8EXzCDVwEqB2a8fsIvwaStHhAWJEeVd1o1QD80CU6+ZdEXXSLbSsuLwJjkCBWqRQUVA==
 
@@ -6822,15 +6864,15 @@
   integrity sha512-NxNv/kLguCA7p3jE8oL2aEBsrJWgAakBpgmgK6lpPWV+WuOmY6r2/zbAVnP+T8bQlA0nzHXSJSJW0Hq7ylaD2Q==
   dependencies:
     kleur "^3.0.3"
     sisteransi "^1.0.5"
 
 prop-types@^15.6.2, prop-types@^15.7.2:
   version "15.8.1"
-  resolved "https://registry.npmjs.org/prop-types/-/prop-types-15.8.1.tgz"
+  resolved "https://registry.yarnpkg.com/prop-types/-/prop-types-15.8.1.tgz#67d87bf1a694f48435cf332c24af10214a3140b5"
   integrity sha512-oj87CgZICdulUohogVAR7AjlC0327U4el4L6eAvOqCeudMDVU0NThNaV+b9Df4dXgSP1gXMTnPdhfe/2qDH5cg==
   dependencies:
     loose-envify "^1.4.0"
     object-assign "^4.1.1"
     react-is "^16.13.1"
 
 property-information@^6.0.0:
@@ -6859,15 +6901,15 @@
 punycode@^1.3.2:
   version "1.4.1"
   resolved "https://registry.npmjs.org/punycode/-/punycode-1.4.1.tgz"
   integrity sha512-jmYNElW7yvO7TV33CjSmvSiE2yco3bV2czu/OzDKdMNVZQWfxCblURLhf+47syQRBntjfLdd/H0egrzIG+oaFQ==
 
 punycode@^2.1.0:
   version "2.3.1"
-  resolved "https://registry.npmjs.org/punycode/-/punycode-2.3.1.tgz"
+  resolved "https://registry.yarnpkg.com/punycode/-/punycode-2.3.1.tgz#027422e2faec0b25e1549c3e1bd8309b9133b6e5"
   integrity sha512-vYt7UD1U9Wg6138shLtLOvdAu+8DsC/ilFtEVHcH+wydcSpNE20AfSOduf6MkRFahL5FY7X1oU7nKVZFtfq8Fg==
 
 pupa@^3.1.0:
   version "3.1.0"
   resolved "https://registry.npmjs.org/pupa/-/pupa-3.1.0.tgz"
   integrity sha512-FLpr4flz5xZTSJxSeaheeMKN/EDzMdK7b8PTOC6a5PYFKTucWbdqjgqaEyH0shFiSJrVB1+Qqi4Tk19ccU6Aug==
   dependencies:
@@ -6895,33 +6937,33 @@
 quick-lru@^5.1.1:
   version "5.1.1"
   resolved "https://registry.npmjs.org/quick-lru/-/quick-lru-5.1.1.tgz"
   integrity sha512-WuyALRjWPDGtt/wzJiadO5AXY+8hZ80hVpe6MyivgraREW751X3SbhRvG3eLKOYN+8VEvqLcf3wdnt44Z4S4SA==
 
 randombytes@^2.1.0:
   version "2.1.0"
-  resolved "https://registry.npmjs.org/randombytes/-/randombytes-2.1.0.tgz"
+  resolved "https://registry.yarnpkg.com/randombytes/-/randombytes-2.1.0.tgz#df6f84372f0270dc65cdf6291349ab7a473d4f2a"
   integrity sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==
   dependencies:
     safe-buffer "^5.1.0"
 
 range-parser@1.2.0:
   version "1.2.0"
   resolved "https://registry.npmjs.org/range-parser/-/range-parser-1.2.0.tgz"
   integrity sha512-kA5WQoNVo4t9lNx2kQNFCxKeBl5IbbSNBl1M/tLkw9WCn+hxNBAW5Qh8gdhs63CJnhjJ2zQWFoqPJP2sK1AV5A==
 
 range-parser@^1.2.1, range-parser@~1.2.1:
   version "1.2.1"
   resolved "https://registry.npmjs.org/range-parser/-/range-parser-1.2.1.tgz"
   integrity sha512-Hrgsx+orqoygnmhFbKaHE6c296J+HTAQXoxEF6gNupROmmGJRoyzfG3ccAveqCBrwr/2yxQ5BVd/GTl5agOwSg==
 
-raw-body@2.5.1:
-  version "2.5.1"
-  resolved "https://registry.npmjs.org/raw-body/-/raw-body-2.5.1.tgz"
-  integrity sha512-qqJBtEyVgS0ZmPGdCFPWJ3FreoqvG4MVQln/kCgF7Olq95IbOp0/BWyMwbdtn4VTvkM8Y7khCQ2Xgk/tcrCXig==
+raw-body@2.5.2:
+  version "2.5.2"
+  resolved "https://registry.yarnpkg.com/raw-body/-/raw-body-2.5.2.tgz#99febd83b90e08975087e8f1f9419a149366b68a"
+  integrity sha512-8zGqypfENjCIqGhgXToC8aB2r7YrBX+AQAfIPs/Mlk+BtPTztOvTS01NRW/3Eh60J+a48lt8qsCzirQ6loCVfA==
   dependencies:
     bytes "3.1.2"
     http-errors "2.0.0"
     iconv-lite "0.4.24"
     unpipe "1.0.0"
 
 raw-loader@^4.0.2:
@@ -6983,31 +7025,31 @@
 react-error-overlay@^6.0.11:
   version "6.0.11"
   resolved "https://registry.npmjs.org/react-error-overlay/-/react-error-overlay-6.0.11.tgz"
   integrity sha512-/6UZ2qgEyH2aqzYZgQPxEnz33NJ2gNsnHA2o5+o4wW9bLM/JYQitNP9xPhsXwC08hMMovfGe/8retsdDsczPRg==
 
 react-fast-compare@^3.2.0:
   version "3.2.2"
-  resolved "https://registry.npmjs.org/react-fast-compare/-/react-fast-compare-3.2.2.tgz"
+  resolved "https://registry.yarnpkg.com/react-fast-compare/-/react-fast-compare-3.2.2.tgz#929a97a532304ce9fee4bcae44234f1ce2c21d49"
   integrity sha512-nsO+KSNgo1SbJqJEYRE9ERzo7YtYbou/OqjSQKxV7jcKox7+usiUVZOAC+XnDOABXggQTno0Y1CpVnuWEc1boQ==
 
 react-helmet-async@*, react-helmet-async@^1.3.0:
   version "1.3.0"
-  resolved "https://registry.npmjs.org/react-helmet-async/-/react-helmet-async-1.3.0.tgz"
+  resolved "https://registry.yarnpkg.com/react-helmet-async/-/react-helmet-async-1.3.0.tgz#7bd5bf8c5c69ea9f02f6083f14ce33ef545c222e"
   integrity sha512-9jZ57/dAn9t3q6hneQS0wukqC2ENOBgMNVEhb/ZG9ZSxUetzVIw4iAmEU38IaVg3QGYauQPhSeUTuIUtFglWpg==
   dependencies:
     "@babel/runtime" "^7.12.5"
     invariant "^2.2.4"
     prop-types "^15.7.2"
     react-fast-compare "^3.2.0"
     shallowequal "^1.1.0"
 
 react-is@^16.13.1, react-is@^16.6.0, react-is@^16.7.0:
   version "16.13.1"
-  resolved "https://registry.npmjs.org/react-is/-/react-is-16.13.1.tgz"
+  resolved "https://registry.yarnpkg.com/react-is/-/react-is-16.13.1.tgz#789729a4dc36de2999dc156dd6c1d9c18cea56a4"
   integrity sha512-24e6ynE2H+OKt4kqsOvNd8kBpV65zoxbA4BVsEOB3ARVWQki/DHzaUoC5KuON/BiccDaCCTZBuOcfZs70kR8bQ==
 
 react-json-view-lite@^1.2.0:
   version "1.2.1"
   resolved "https://registry.npmjs.org/react-json-view-lite/-/react-json-view-lite-1.2.1.tgz"
   integrity sha512-Itc0g86fytOmKZoIoJyGgvNqohWSbh3NXIKNgH6W6FT9PC1ck4xas1tT3Rr/b3UlFXyA9Jjaw9QSXdZy2JwGMQ==
 
@@ -7118,15 +7160,15 @@
 regenerate@^1.4.2:
   version "1.4.2"
   resolved "https://registry.npmjs.org/regenerate/-/regenerate-1.4.2.tgz"
   integrity sha512-zrceR/XhGYU/d/opr2EKO7aRHUeiBI8qjtfHqADTwZd6Szfy16la6kqD0MIUs5z5hx6AaKa+PixpPrR289+I0A==
 
 regenerator-runtime@^0.14.0:
   version "0.14.1"
-  resolved "https://registry.npmjs.org/regenerator-runtime/-/regenerator-runtime-0.14.1.tgz"
+  resolved "https://registry.yarnpkg.com/regenerator-runtime/-/regenerator-runtime-0.14.1.tgz#356ade10263f685dda125100cd862c1db895327f"
   integrity sha512-dYnhHh0nJoMfnkZs6GmmhFknAGRrLznOu5nc9ML+EJxGvrx6H7teuevqVqCuPcPK//3eDrrjQhehXVx9cnkGdw==
 
 regenerator-transform@^0.15.2:
   version "0.15.2"
   resolved "https://registry.npmjs.org/regenerator-transform/-/regenerator-transform-0.15.2.tgz"
   integrity sha512-hfMp2BoF0qOk3uc5V20ALGDS2ddjQaLrdl7xrGXvAIow7qeWRM2VA2HuCHkUKk9slq3VwEwLNK3DFBqDfPGYtg==
   dependencies:
@@ -7369,15 +7411,15 @@
     queue-microtask "^1.2.2"
 
 safe-buffer@5.1.2, safe-buffer@~5.1.0, safe-buffer@~5.1.1:
   version "5.1.2"
   resolved "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.1.2.tgz"
   integrity sha512-Gd2UZBJDkXlY7GbJxfsE8/nvKkUEU1G38c1siN6QP6a9PT9MmHB8GnpscSmMJSoF8LOIrt8ud/wPtojys4G6+g==
 
-safe-buffer@5.2.1, safe-buffer@>=5.1.0, safe-buffer@^5.1.0, safe-buffer@^5.1.2, safe-buffer@^5.2.1, safe-buffer@~5.2.0:
+safe-buffer@5.2.1, safe-buffer@>=5.1.0, safe-buffer@^5.1.0, safe-buffer@~5.2.0:
   version "5.2.1"
   resolved "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.2.1.tgz"
   integrity sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==
 
 "safer-buffer@>= 2.1.2 < 3":
   version "2.1.2"
   resolved "https://registry.npmjs.org/safer-buffer/-/safer-buffer-2.1.2.tgz"
@@ -7478,21 +7520,28 @@
     http-errors "2.0.0"
     mime "1.6.0"
     ms "2.1.3"
     on-finished "2.4.1"
     range-parser "~1.2.1"
     statuses "2.0.1"
 
-serialize-javascript@^6.0.0, serialize-javascript@^6.0.1:
+serialize-javascript@^6.0.0:
   version "6.0.1"
   resolved "https://registry.npmjs.org/serialize-javascript/-/serialize-javascript-6.0.1.tgz"
   integrity sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==
   dependencies:
     randombytes "^2.1.0"
 
+serialize-javascript@^6.0.1:
+  version "6.0.2"
+  resolved "https://registry.yarnpkg.com/serialize-javascript/-/serialize-javascript-6.0.2.tgz#defa1e055c83bf6d59ea805d8da862254eb6a6c2"
+  integrity sha512-Saa1xPByTTq2gdeFZYLLo+RFE35NHZkAbqZeWNd3BpzppeVisAqpDjcp8dyf6uIvEqJRd46jemmyA4iFIeVk8g==
+  dependencies:
+    randombytes "^2.1.0"
+
 serve-handler@^6.1.5:
   version "6.1.5"
   resolved "https://registry.npmjs.org/serve-handler/-/serve-handler-6.1.5.tgz"
   integrity sha512-ijPFle6Hwe8zfmBxJdE+5fta53fdIY0lHISJvuikXB3VYFafRjMRpOffSPvCYsbKyBA7pvy9oYr/BT1O3EArlg==
   dependencies:
     bytes "3.0.0"
     content-disposition "0.5.2"
@@ -7544,22 +7593,22 @@
 setprototypeof@1.2.0:
   version "1.2.0"
   resolved "https://registry.npmjs.org/setprototypeof/-/setprototypeof-1.2.0.tgz"
   integrity sha512-E5LDX7Wrp85Kil5bhZv46j8jOeboKq5JMmYM3gVGdGH8xFpPWXUMsNrlODCrkoxMEeNi/XZIwuRvY4XNwYMJpw==
 
 shallow-clone@^3.0.0:
   version "3.0.1"
-  resolved "https://registry.npmjs.org/shallow-clone/-/shallow-clone-3.0.1.tgz"
+  resolved "https://registry.yarnpkg.com/shallow-clone/-/shallow-clone-3.0.1.tgz#8f2981ad92531f55035b01fb230769a40e02efa3"
   integrity sha512-/6KqX+GVUdqPuPPd2LxDDxzX6CAbjJehAAOKlNpqqUpAqPM6HeL8f+o3a+JsyGjn2lv0WY8UsTgUJjU9Ok55NA==
   dependencies:
     kind-of "^6.0.2"
 
 shallowequal@^1.1.0:
   version "1.1.0"
-  resolved "https://registry.npmjs.org/shallowequal/-/shallowequal-1.1.0.tgz"
+  resolved "https://registry.yarnpkg.com/shallowequal/-/shallowequal-1.1.0.tgz#188d521de95b9087404fd4dcb68b13df0ae4e7f8"
   integrity sha512-y0m1JoUZSlPAjXVtPPW70aZWfIL/dSP7AFkRnniLCrK/8MDKog3TySTBmckD+RObVxH0v4Tox67+F14PdED2oQ==
 
 shebang-command@^2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/shebang-command/-/shebang-command-2.0.0.tgz"
   integrity sha512-kHxr2zZpYtdmrN1qDjrrX/Z1rR1kG8Dx+gkpK1G4eXmvXswmcE1hTWBWYUzlraYw1/yZp6YuDY77YtvbN0dmDA==
   dependencies:
@@ -7571,15 +7620,15 @@
   integrity sha512-7++dFhtcx3353uBaq8DDR4NuxBetBzC7ZQOhmTQInHEd6bSrXdiEyzCvG07Z44UYdLShWUyXt5M/yhz8ekcb1A==
 
 shell-quote@^1.7.3, shell-quote@^1.8.1:
   version "1.8.1"
   resolved "https://registry.npmjs.org/shell-quote/-/shell-quote-1.8.1.tgz"
   integrity sha512-6j1W9l1iAs/4xYBI1SYOVZyFcCis9b4KCLQ8fgAGG07QvzaRLVVRQvAy85yNmmZSjYjg4MWh4gNvlPujU/5LpA==
 
-shelljs@^0.8.4, shelljs@^0.8.5:
+shelljs@^0.8.5:
   version "0.8.5"
   resolved "https://registry.npmjs.org/shelljs/-/shelljs-0.8.5.tgz"
   integrity sha512-TiwcRcrkhHvbrZbnRcFYMLl30Dfov3HKqzp5tO5b4pt6G/SezKcYhmDg15zXVBswHmctSAQKznqNW2LO5tTDow==
   dependencies:
     glob "^7.0.0"
     interpret "^1.0.0"
     rechoir "^0.6.2"
@@ -7656,23 +7705,23 @@
 source-map-js@^1.0.2:
   version "1.0.2"
   resolved "https://registry.npmjs.org/source-map-js/-/source-map-js-1.0.2.tgz"
   integrity sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==
 
 source-map-support@~0.5.20:
   version "0.5.21"
-  resolved "https://registry.npmjs.org/source-map-support/-/source-map-support-0.5.21.tgz"
+  resolved "https://registry.yarnpkg.com/source-map-support/-/source-map-support-0.5.21.tgz#04fe7c7f9e1ed2d662233c28cb2b35b9f63f6e4f"
   integrity sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==
   dependencies:
     buffer-from "^1.0.0"
     source-map "^0.6.0"
 
 source-map@^0.6.0, source-map@^0.6.1, source-map@~0.6.0:
   version "0.6.1"
-  resolved "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz"
+  resolved "https://registry.yarnpkg.com/source-map/-/source-map-0.6.1.tgz#74722af32e9614e9c287a8d0bbde48b5e2f1a263"
   integrity sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==
 
 source-map@^0.7.0:
   version "0.7.4"
   resolved "https://registry.npmjs.org/source-map/-/source-map-0.7.4.tgz"
   integrity sha512-l3BikUxvPOcn5E74dZiq5BGsTb5yEwhaTSzccU6t4sDOH8NWJCstKO5QT2CvtFoK6F0saL7p9xHAqHOlCPJygA==
 
@@ -7851,15 +7900,15 @@
   resolved "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz"
   integrity sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==
   dependencies:
     has-flag "^4.0.0"
 
 supports-color@^8.0.0:
   version "8.1.1"
-  resolved "https://registry.npmjs.org/supports-color/-/supports-color-8.1.1.tgz"
+  resolved "https://registry.yarnpkg.com/supports-color/-/supports-color-8.1.1.tgz#cd6fc17e28500cff56c1b86c0a7fd4a54a73005c"
   integrity sha512-MpUEN2OodtUzxvKQl72cUF7RQ5EiHsGvSsVG0ia9c5RbWGL2CI4C7EpPS8UTBIplnlzZiNuV56w+FuNxy3ty2Q==
   dependencies:
     has-flag "^4.0.0"
 
 supports-preserve-symlinks-flag@^1.0.0:
   version "1.0.0"
   resolved "https://registry.npmjs.org/supports-preserve-symlinks-flag/-/supports-preserve-symlinks-flag-1.0.0.tgz"
@@ -7886,51 +7935,71 @@
 tapable@^1.0.0:
   version "1.1.3"
   resolved "https://registry.npmjs.org/tapable/-/tapable-1.1.3.tgz"
   integrity sha512-4WK/bYZmj8xLr+HUCODHGF1ZFzsYffasLUgEiMBY4fgtltdO6B4WJtlSbPaDTLpYTcGVwM2qLnFTICEcNxs3kA==
 
 tapable@^2.0.0, tapable@^2.1.1, tapable@^2.2.0:
   version "2.2.1"
-  resolved "https://registry.npmjs.org/tapable/-/tapable-2.2.1.tgz"
+  resolved "https://registry.yarnpkg.com/tapable/-/tapable-2.2.1.tgz#1967a73ef4060a82f12ab96af86d52fdb76eeca0"
   integrity sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==
 
-tar@^4.4.8:
-  version "4.4.19"
-  resolved "https://registry.npmjs.org/tar/-/tar-4.4.19.tgz"
-  integrity sha512-a20gEsvHnWe0ygBY8JbxoM4w3SJdhc7ZAuxkLqh+nvNQN2IOt0B5lLgM490X5Hl8FF0dl0tOf2ewFYAlIFgzVA==
-  dependencies:
-    chownr "^1.1.4"
-    fs-minipass "^1.2.7"
-    minipass "^2.9.0"
-    minizlib "^1.3.3"
-    mkdirp "^0.5.5"
-    safe-buffer "^5.2.1"
-    yallist "^3.1.1"
+tar@^6.2.0:
+  version "6.2.1"
+  resolved "https://registry.yarnpkg.com/tar/-/tar-6.2.1.tgz#717549c541bc3c2af15751bea94b1dd068d4b03a"
+  integrity sha512-DZ4yORTwrbTj/7MZYq2w+/ZFdI6OZ/f9SFHR+71gIVUZhOQPHzVCLpvRnPgyaMpfWxxk/4ONva3GQSyNIKRv6A==
+  dependencies:
+    chownr "^2.0.0"
+    fs-minipass "^2.0.0"
+    minipass "^5.0.0"
+    minizlib "^2.1.1"
+    mkdirp "^1.0.3"
+    yallist "^4.0.0"
 
-terser-webpack-plugin@^5.3.7, terser-webpack-plugin@^5.3.9:
+terser-webpack-plugin@^5.3.10:
+  version "5.3.10"
+  resolved "https://registry.yarnpkg.com/terser-webpack-plugin/-/terser-webpack-plugin-5.3.10.tgz#904f4c9193c6fd2a03f693a2150c62a92f40d199"
+  integrity sha512-BKFPWlPDndPs+NGGCr1U59t0XScL5317Y0UReNrHaw9/FwhPENlq6bfgs+4yPfyP51vqC1bQ4rp1EfXW5ZSH9w==
+  dependencies:
+    "@jridgewell/trace-mapping" "^0.3.20"
+    jest-worker "^27.4.5"
+    schema-utils "^3.1.1"
+    serialize-javascript "^6.0.1"
+    terser "^5.26.0"
+
+terser-webpack-plugin@^5.3.9:
   version "5.3.9"
   resolved "https://registry.npmjs.org/terser-webpack-plugin/-/terser-webpack-plugin-5.3.9.tgz"
   integrity sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==
   dependencies:
     "@jridgewell/trace-mapping" "^0.3.17"
     jest-worker "^27.4.5"
     schema-utils "^3.1.1"
     serialize-javascript "^6.0.1"
     terser "^5.16.8"
 
-terser@^5.10.0, terser@^5.15.1, terser@^5.16.8:
+terser@^5.10.0, terser@^5.15.1:
   version "5.26.0"
   resolved "https://registry.npmjs.org/terser/-/terser-5.26.0.tgz"
   integrity sha512-dytTGoE2oHgbNV9nTzgBEPaqAWvcJNl66VZ0BkJqlvp71IjO8CxdBx/ykCNb47cLnCmCvRZ6ZR0tLkqvZCdVBQ==
   dependencies:
     "@jridgewell/source-map" "^0.3.3"
     acorn "^8.8.2"
     commander "^2.20.0"
     source-map-support "~0.5.20"
 
+terser@^5.16.8, terser@^5.26.0:
+  version "5.30.3"
+  resolved "https://registry.yarnpkg.com/terser/-/terser-5.30.3.tgz#f1bb68ded42408c316b548e3ec2526d7dd03f4d2"
+  integrity sha512-STdUgOUx8rLbMGO9IOwHLpCqolkDITFFQSMYYwKE1N2lY6MVSaeoi10z/EhWxRc6ybqoVmKSkhKYH/XUpl7vSA==
+  dependencies:
+    "@jridgewell/source-map" "^0.3.3"
+    acorn "^8.8.2"
+    commander "^2.20.0"
+    source-map-support "~0.5.20"
+
 text-table@^0.2.0:
   version "0.2.0"
   resolved "https://registry.npmjs.org/text-table/-/text-table-0.2.0.tgz"
   integrity sha512-N+8UisAXDGk8PFXP4HAzVR9nbfmVJ3zYLAWiTIoqC5v5isinhr+r5uaO8+7r3BMfuNIufIsA7RdpVgacC2cSpw==
 
 thunky@^1.0.2:
   version "1.1.0"
@@ -8022,14 +8091,19 @@
     is-typedarray "^1.0.0"
 
 typescript@^5.3.3:
   version "5.3.3"
   resolved "https://registry.yarnpkg.com/typescript/-/typescript-5.3.3.tgz#b3ce6ba258e72e6305ba66f5c9b452aaee3ffe37"
   integrity sha512-pXWcraxM0uxAS+tN0AG/BF2TyqmHO014Z070UsJ+pFvYuRSq8KH8DmWpnbXe0pEPDHXZV3FcAbJkijJ5oNEnWw==
 
+undici-types@~5.26.4:
+  version "5.26.5"
+  resolved "https://registry.yarnpkg.com/undici-types/-/undici-types-5.26.5.tgz#bcd539893d00b56e964fd2657a4866b221a65617"
+  integrity sha512-JlCMO+ehdEIKqlFxk6IfVoAUVmgz7cU7zD/h9XZ0qzeosSHmUJVOzSQvvYSYWXkFXC+IfLKSIffhv0sVZup6pA==
+
 unicode-canonical-property-names-ecmascript@^2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/unicode-canonical-property-names-ecmascript/-/unicode-canonical-property-names-ecmascript-2.0.0.tgz"
   integrity sha512-yY5PpDlfVIU5+y/BSCxAJRBIS1Zc2dDG3Ujq+sR0U+JjUevW2JhocOF+soROYDSaAezOzOKuyyixhD6mBknSmQ==
 
 unicode-emoji-modifier-base@^1.0.0:
   version "1.0.0"
@@ -8135,15 +8209,15 @@
 unpipe@1.0.0, unpipe@~1.0.0:
   version "1.0.0"
   resolved "https://registry.npmjs.org/unpipe/-/unpipe-1.0.0.tgz"
   integrity sha512-pjy2bYhSsufwWlKwPc+l3cN7+wuJlK6uz0YdJEOlQDbl6jo/YlPi4mb8agUkVC8BF7V8NuzeyPNqRksA3hztKQ==
 
 update-browserslist-db@^1.0.13:
   version "1.0.13"
-  resolved "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.13.tgz"
+  resolved "https://registry.yarnpkg.com/update-browserslist-db/-/update-browserslist-db-1.0.13.tgz#3c5e4f5c083661bd38ef64b6328c26ed6c8248c4"
   integrity sha512-xebP81SNcPuNpPP3uzeW1NYXxI3rxyJzF3pD6sH4jE7o/IX+WtSpwnVU+qIsDPyk0d3hmFQ7mjqc6AtV604hbg==
   dependencies:
     escalade "^3.1.1"
     picocolors "^1.0.0"
 
 update-notifier@^6.0.2:
   version "6.0.2"
@@ -8163,15 +8237,15 @@
     pupa "^3.1.0"
     semver "^7.3.7"
     semver-diff "^4.0.0"
     xdg-basedir "^5.1.0"
 
 uri-js@^4.2.2:
   version "4.4.1"
-  resolved "https://registry.npmjs.org/uri-js/-/uri-js-4.4.1.tgz"
+  resolved "https://registry.yarnpkg.com/uri-js/-/uri-js-4.4.1.tgz#9b1a52595225859e55f669d928f88c6c57f2a77e"
   integrity sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==
   dependencies:
     punycode "^2.1.0"
 
 url-loader@^4.1.1:
   version "4.1.1"
   resolved "https://registry.npmjs.org/url-loader/-/url-loader-4.1.1.tgz"
@@ -8188,17 +8262,17 @@
 
 utila@~0.4:
   version "0.4.0"
   resolved "https://registry.npmjs.org/utila/-/utila-0.4.0.tgz"
   integrity sha512-Z0DbgELS9/L/75wZbro8xAnT50pBVFQZ+hUEueGDU5FN51YSCYM+jdxsfCiHjwNP/4LCDD0i/graKpeBnOXKRA==
 
 utility-types@^3.10.0:
-  version "3.10.0"
-  resolved "https://registry.npmjs.org/utility-types/-/utility-types-3.10.0.tgz"
-  integrity sha512-O11mqxmi7wMKCo6HKFt5AhO4BwY3VV68YU07tgxfz8zJTIxr4BpsezN49Ffwy9j3ZpwwJp4fkRwjRzq3uWE6Rg==
+  version "3.11.0"
+  resolved "https://registry.yarnpkg.com/utility-types/-/utility-types-3.11.0.tgz#607c40edb4f258915e901ea7995607fdf319424c"
+  integrity sha512-6Z7Ma2aVEWisaL6TvBCy7P8rm2LQoPv6dJ7ecIaIixHcwfbJ0x7mWdbcwlIM5IGQxPZSFYeqRCqlOOeKoJYMkw==
 
 utils-merge@1.0.1:
   version "1.0.1"
   resolved "https://registry.npmjs.org/utils-merge/-/utils-merge-1.0.1.tgz"
   integrity sha512-pMZTvIkT1d+TFGvDOqodOclx0QWkkgi6Tdoa8gC8ffGAAqz9pzPTZWAybbsHHoED/ztMtkv/VoYTYyShUn81hA==
 
 uuid@^8.3.2:
@@ -8237,18 +8311,18 @@
   resolved "https://registry.npmjs.org/vfile/-/vfile-6.0.1.tgz"
   integrity sha512-1bYqc7pt6NIADBJ98UiG0Bn/CHIVOoZ/IyEkqIruLg0mE1BKzkOXY2D6CSqQIcKqgadppE5lrxgWXJmXd7zZJw==
   dependencies:
     "@types/unist" "^3.0.0"
     unist-util-stringify-position "^4.0.0"
     vfile-message "^4.0.0"
 
-watchpack@^2.4.0:
-  version "2.4.0"
-  resolved "https://registry.npmjs.org/watchpack/-/watchpack-2.4.0.tgz"
-  integrity sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==
+watchpack@^2.4.1:
+  version "2.4.1"
+  resolved "https://registry.yarnpkg.com/watchpack/-/watchpack-2.4.1.tgz#29308f2cac150fa8e4c92f90e0ec954a9fed7fff"
+  integrity sha512-8wrBCMtVhqcXP2Sup1ctSkga6uc2Bx0IIvKyT7yTFier5AXHooSI+QyQQAtTb7+E0IUCCKyTFmXqdqgum2XWGg==
   dependencies:
     glob-to-regexp "^0.4.1"
     graceful-fs "^4.1.2"
 
 wbuf@^1.1.0, wbuf@^1.7.3:
   version "1.7.3"
   resolved "https://registry.npmjs.org/wbuf/-/wbuf-1.7.3.tgz"
@@ -8282,17 +8356,17 @@
     is-plain-object "^5.0.0"
     opener "^1.5.2"
     picocolors "^1.0.0"
     sirv "^2.0.3"
     ws "^7.3.1"
 
 webpack-dev-middleware@^5.3.1:
-  version "5.3.3"
-  resolved "https://registry.npmjs.org/webpack-dev-middleware/-/webpack-dev-middleware-5.3.3.tgz"
-  integrity sha512-hj5CYrY0bZLB+eTO+x/j67Pkrquiy7kWepMHmUMoPsmcUaeEnQJqFzHJOyxgWlq746/wUuA64p9ta34Kyb01pA==
+  version "5.3.4"
+  resolved "https://registry.yarnpkg.com/webpack-dev-middleware/-/webpack-dev-middleware-5.3.4.tgz#eb7b39281cbce10e104eb2b8bf2b63fce49a3517"
+  integrity sha512-BVdTqhhs+0IfoeAf7EoH5WE+exCmqGerHfDM0IL096Px60Tq2Mn9MAbnaGUe6HiMa41KMCYF19gyzZmBcq/o4Q==
   dependencies:
     colorette "^2.0.10"
     memfs "^3.4.3"
     mime-types "^2.1.31"
     range-parser "^1.2.1"
     schema-utils "^4.0.0"
 
@@ -8330,54 +8404,54 @@
     sockjs "^0.3.24"
     spdy "^4.0.2"
     webpack-dev-middleware "^5.3.1"
     ws "^8.13.0"
 
 webpack-merge@^5.9.0:
   version "5.10.0"
-  resolved "https://registry.npmjs.org/webpack-merge/-/webpack-merge-5.10.0.tgz"
+  resolved "https://registry.yarnpkg.com/webpack-merge/-/webpack-merge-5.10.0.tgz#a3ad5d773241e9c682803abf628d4cd62b8a4177"
   integrity sha512-+4zXKdx7UnO+1jaN4l2lHVD+mFvnlZQP/6ljaJVb4SZiwIKeUnrT5l0gkT8z+n4hKpC+jpOv6O9R+gLtag7pSA==
   dependencies:
     clone-deep "^4.0.1"
     flat "^5.0.2"
     wildcard "^2.0.0"
 
-webpack-sources@^3.2.2, webpack-sources@^3.2.3:
+webpack-sources@^3.2.3:
   version "3.2.3"
-  resolved "https://registry.npmjs.org/webpack-sources/-/webpack-sources-3.2.3.tgz"
+  resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-3.2.3.tgz#2d4daab8451fd4b240cc27055ff6a0c2ccea0cde"
   integrity sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==
 
 webpack@^5.88.1:
-  version "5.89.0"
-  resolved "https://registry.npmjs.org/webpack/-/webpack-5.89.0.tgz"
-  integrity sha512-qyfIC10pOr70V+jkmud8tMfajraGCZMBWJtrmuBymQKCrLTRejBI8STDp1MCyZu/QTdZSeacCQYpYNQVOzX5kw==
+  version "5.91.0"
+  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.91.0.tgz#ffa92c1c618d18c878f06892bbdc3373c71a01d9"
+  integrity sha512-rzVwlLeBWHJbmgTC/8TvAcu5vpJNII+MelQpylD4jNERPwpBJOE2lEcko1zJX3QJeLjTTAnQxn/OJ8bjDzVQaw==
   dependencies:
     "@types/eslint-scope" "^3.7.3"
-    "@types/estree" "^1.0.0"
-    "@webassemblyjs/ast" "^1.11.5"
-    "@webassemblyjs/wasm-edit" "^1.11.5"
-    "@webassemblyjs/wasm-parser" "^1.11.5"
+    "@types/estree" "^1.0.5"
+    "@webassemblyjs/ast" "^1.12.1"
+    "@webassemblyjs/wasm-edit" "^1.12.1"
+    "@webassemblyjs/wasm-parser" "^1.12.1"
     acorn "^8.7.1"
     acorn-import-assertions "^1.9.0"
-    browserslist "^4.14.5"
+    browserslist "^4.21.10"
     chrome-trace-event "^1.0.2"
-    enhanced-resolve "^5.15.0"
+    enhanced-resolve "^5.16.0"
     es-module-lexer "^1.2.1"
     eslint-scope "5.1.1"
     events "^3.2.0"
     glob-to-regexp "^0.4.1"
-    graceful-fs "^4.2.9"
+    graceful-fs "^4.2.11"
     json-parse-even-better-errors "^2.3.1"
     loader-runner "^4.2.0"
     mime-types "^2.1.27"
     neo-async "^2.6.2"
     schema-utils "^3.2.0"
     tapable "^2.1.1"
-    terser-webpack-plugin "^5.3.7"
-    watchpack "^2.4.0"
+    terser-webpack-plugin "^5.3.10"
+    watchpack "^2.4.1"
     webpack-sources "^3.2.3"
 
 webpackbar@^5.0.2:
   version "5.0.2"
   resolved "https://registry.npmjs.org/webpackbar/-/webpackbar-5.0.2.tgz"
   integrity sha512-BmFJo7veBDgQzfWXl/wwYXr/VFus0614qZ8i9znqcl9fnEdiVkdbi0TedLQ6xAK92HZHDJ0QmyQ0fmuZPAgCYQ==
   dependencies:
@@ -8427,15 +8501,15 @@
   resolved "https://registry.npmjs.org/widest-line/-/widest-line-4.0.1.tgz"
   integrity sha512-o0cyEG0e8GPzT4iGHphIOh0cJOV8fivsXxddQasHPHfoZf1ZexrfeA21w2NaEN1RHE+fXlfISmOE8R9N3u3Qig==
   dependencies:
     string-width "^5.0.1"
 
 wildcard@^2.0.0:
   version "2.0.1"
-  resolved "https://registry.npmjs.org/wildcard/-/wildcard-2.0.1.tgz"
+  resolved "https://registry.yarnpkg.com/wildcard/-/wildcard-2.0.1.tgz#5ab10d02487198954836b6349f74fff961e10f67"
   integrity sha512-CC1bOL87PIWSBhDcTrdeLo6eGT7mCFtrg0uIJtqJUFyK+eJnzl8A1niH56uu7KMa5XFrtiV+AQuHO3n7DsHnLQ==
 
 wrap-ansi@^8.0.1, wrap-ansi@^8.1.0:
   version "8.1.0"
   resolved "https://registry.npmjs.org/wrap-ansi/-/wrap-ansi-8.1.0.tgz"
   integrity sha512-si7QWI6zUMq56bESFvagtmzMdGOtoxfR+Sez11Mobfc7tm+VkUckk9bW2UeffTGVUbOksxmSw0AA2gs8g71NCQ==
   dependencies:
@@ -8476,36 +8550,36 @@
 xml-js@^1.6.11:
   version "1.6.11"
   resolved "https://registry.npmjs.org/xml-js/-/xml-js-1.6.11.tgz"
   integrity sha512-7rVi2KMfwfWFl+GpPg6m80IVMWXLRjO+PxTq7V2CDhoGak0wzYzFgUY2m4XJ47OGdXd8eLE8EmwfAmdjw7lC1g==
   dependencies:
     sax "^1.2.4"
 
-yallist@^3.0.0, yallist@^3.0.2, yallist@^3.1.1:
+yallist@^3.0.2:
   version "3.1.1"
   resolved "https://registry.npmjs.org/yallist/-/yallist-3.1.1.tgz"
   integrity sha512-a4UGQaWPH59mOXUYnAG2ewncQS4i4F43Tv3JoAM+s2VDAmS9NsK8GpDMLrCHPksFT7h3K6TOoUNn2pb7RoXx4g==
 
 yallist@^4.0.0:
   version "4.0.0"
   resolved "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz"
   integrity sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==
 
 yaml@^1.10.0, yaml@^1.10.2, yaml@^1.7.2:
   version "1.10.2"
   resolved "https://registry.npmjs.org/yaml/-/yaml-1.10.2.tgz"
   integrity sha512-r3vXyErRCYJ7wg28yvBY5VSoAF8ZvlcW9/BwUzEtUsjvX/DKs24dIkuwjtuprwJJHsbyUbLApepYTR1BN4uHrg==
 
-yauzl@^2.10.0:
-  version "2.10.0"
-  resolved "https://registry.npmjs.org/yauzl/-/yauzl-2.10.0.tgz"
-  integrity sha512-p4a9I6X6nu6IhoGmBqAcbJy1mlC4j27vEPZX9F4L4/vZT3Lyq1VkFHw/V/PUcB9Buo+DG3iHkT0x3Qya58zc3g==
+yauzl@^3.1.0:
+  version "3.1.2"
+  resolved "https://registry.yarnpkg.com/yauzl/-/yauzl-3.1.2.tgz#f3f3d3bdb8b98fbd367e37e1596ad45210da1533"
+  integrity sha512-621iCPgEG1wXViDZS/L3h9F8TgrdQV1eayJlJ8j5A2SZg8OdY/1DLf+VxNeD+q5QbMFEAbjjR8nITj7g4nKa0Q==
   dependencies:
     buffer-crc32 "~0.2.3"
-    fd-slicer "~1.1.0"
+    pend "~1.2.0"
 
 yocto-queue@^0.1.0:
   version "0.1.0"
   resolved "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz"
   integrity sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==
 
 yocto-queue@^1.0.0:
```

### Comparing `go_task_bin-3.35.1/task/errors/errors.go` & `go_task_bin-3.36.0/task/errors/errors.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/errors/errors_task.go` & `go_task_bin-3.36.0/task/errors/errors_task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/errors/errors_taskfile.go` & `go_task_bin-3.36.0/task/errors/errors_taskfile.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/go.mod` & `go_task_bin-3.36.0/task/go.mod`

 * *Files 20% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 	github.com/Masterminds/semver/v3 v3.2.1
 	github.com/davecgh/go-spew v1.1.1
 	github.com/fatih/color v1.16.0
 	github.com/go-task/slim-sprig/v3 v3.0.0
 	github.com/joho/godotenv v1.5.1
 	github.com/mattn/go-zglob v0.0.4
 	github.com/mitchellh/hashstructure/v2 v2.0.2
+	github.com/otiai10/copy v1.14.0
 	github.com/radovskyb/watcher v1.0.7
 	github.com/sajari/fuzzy v1.0.0
 	github.com/spf13/pflag v1.0.5
-	github.com/stretchr/testify v1.8.4
+	github.com/stretchr/testify v1.9.0
 	github.com/zeebo/xxh3 v1.0.2
-	golang.org/x/sync v0.6.0
-	golang.org/x/term v0.17.0
+	golang.org/x/sync v0.7.0
+	golang.org/x/term v0.19.0
 	gopkg.in/yaml.v3 v3.0.1
 	mvdan.cc/sh/v3 v3.8.0
 )
 
 require (
 	github.com/klauspost/cpuid/v2 v2.0.9 // indirect
 	github.com/mattn/go-colorable v0.1.13 // indirect
 	github.com/mattn/go-isatty v0.0.20 // indirect
 	github.com/pmezard/go-difflib v1.0.0 // indirect
-	github.com/stretchr/objx v0.5.0 // indirect
-	golang.org/x/sys v0.17.0 // indirect
+	github.com/stretchr/objx v0.5.2 // indirect
+	golang.org/x/sys v0.19.0 // indirect
 	gopkg.in/check.v1 v1.0.0-20180628173108-788fd7840127 // indirect
 )
```

### Comparing `go_task_bin-3.35.1/task/go.sum` & `go_task_bin-3.36.0/task/go.sum`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 github.com/Masterminds/semver/v3 v3.2.1 h1:RN9w6+7QoMeJVGyfmbcgs28Br8cvmnucEXnY0rYXWg0=
 github.com/Masterminds/semver/v3 v3.2.1/go.mod h1:qvl/7zhW3nngYb5+80sSMF+FG2BjYrf8m9wsX0PNOMQ=
 github.com/creack/pty v1.1.21 h1:1/QdRyBaHHJP61QkWMXlOIBfsgdDeeKfK8SYVUWJKf0=
 github.com/creack/pty v1.1.21/go.mod h1:MOBLtS5ELjhRRrroQr9kyvTxUAFNvYEK993ew/Vr4O4=
-github.com/davecgh/go-spew v1.1.0/go.mod h1:J7Y8YcW2NihsgmVo/mv3lAwl/skON4iLHjSsI+c5H38=
 github.com/davecgh/go-spew v1.1.1 h1:vj9j/u1bqnvCEfJOwUhtlOARqs3+rkHYY13jYWTU97c=
 github.com/davecgh/go-spew v1.1.1/go.mod h1:J7Y8YcW2NihsgmVo/mv3lAwl/skON4iLHjSsI+c5H38=
 github.com/fatih/color v1.16.0 h1:zmkK9Ngbjj+K0yRhTVONQh1p/HknKYSlNT+vZCzyokM=
 github.com/fatih/color v1.16.0/go.mod h1:fL2Sau1YI5c0pdGEVCbKQbLXB6edEj1ZgiY4NijnWvE=
 github.com/frankban/quicktest v1.14.6 h1:7Xjx+VpznH+oBnejlPUj8oUpdxnVs4f8XU8WnHkI4W8=
 github.com/frankban/quicktest v1.14.6/go.mod h1:4ptaffx2x8+WTWXmUCuVU6aPUX1/Mz7zb5vbUoiM6w0=
 github.com/go-task/slim-sprig/v3 v3.0.0 h1:sUs3vkvUymDpBKi3qH1YSqBQk9+9D/8M2mN1vB6EwHI=
@@ -26,45 +25,44 @@
 github.com/mattn/go-isatty v0.0.16/go.mod h1:kYGgaQfpe5nmfYZH+SKPsOc2e4SrIfOl2e/yFXSvRLM=
 github.com/mattn/go-isatty v0.0.20 h1:xfD0iDuEKnDkl03q4limB+vH+GxLEtL/jb4xVJSWWEY=
 github.com/mattn/go-isatty v0.0.20/go.mod h1:W+V8PltTTMOvKvAeJH7IuucS94S2C6jfK/D7dTCTo3Y=
 github.com/mattn/go-zglob v0.0.4 h1:LQi2iOm0/fGgu80AioIJ/1j9w9Oh+9DZ39J4VAGzHQM=
 github.com/mattn/go-zglob v0.0.4/go.mod h1:MxxjyoXXnMxfIpxTK2GAkw1w8glPsQILx3N5wrKakiY=
 github.com/mitchellh/hashstructure/v2 v2.0.2 h1:vGKWl0YJqUNxE8d+h8f6NJLcCJrgbhC4NcD46KavDd4=
 github.com/mitchellh/hashstructure/v2 v2.0.2/go.mod h1:MG3aRVU/N29oo/V/IhBX8GR/zz4kQkprJgF2EVszyDE=
+github.com/otiai10/copy v1.14.0 h1:dCI/t1iTdYGtkvCuBG2BgR6KZa83PTclw4U5n2wAllU=
+github.com/otiai10/copy v1.14.0/go.mod h1:ECfuL02W+/FkTWZWgQqXPWZgW9oeKCSQ5qVfSc4qc4w=
+github.com/otiai10/mint v1.5.1 h1:XaPLeE+9vGbuyEHem1JNk3bYc7KKqyI/na0/mLd/Kks=
+github.com/otiai10/mint v1.5.1/go.mod h1:MJm72SBthJjz8qhefc4z1PYEieWmy8Bku7CjcAqyUSM=
 github.com/pmezard/go-difflib v1.0.0 h1:4DBwDE0NGyQoBHbLQYPwSUPoCMWR5BEzIk/f1lZbAQM=
 github.com/pmezard/go-difflib v1.0.0/go.mod h1:iKH77koFhYxTK1pcRnkKkqfTogsbg7gZNVY4sRDYZ/4=
 github.com/radovskyb/watcher v1.0.7 h1:AYePLih6dpmS32vlHfhCeli8127LzkIgwJGcwwe8tUE=
 github.com/radovskyb/watcher v1.0.7/go.mod h1:78okwvY5wPdzcb1UYnip1pvrZNIVEIh/Cm+ZuvsUYIg=
 github.com/rogpeppe/go-internal v1.12.0 h1:exVL4IDcn6na9z1rAb56Vxr+CgyK3nn3O+epU5NdKM8=
 github.com/rogpeppe/go-internal v1.12.0/go.mod h1:E+RYuTGaKKdloAfM02xzb0FW3Paa99yedzYV+kq4uf4=
 github.com/sajari/fuzzy v1.0.0 h1:+FmwVvJErsd0d0hAPlj4CxqxUtQY/fOoY0DwX4ykpRY=
 github.com/sajari/fuzzy v1.0.0/go.mod h1:OjYR6KxoWOe9+dOlXeiCJd4dIbED4Oo8wpS89o0pwOo=
 github.com/spf13/pflag v1.0.5 h1:iy+VFUOCP1a+8yFto/drg2CJ5u0yRoB7fZw3DKv/JXA=
 github.com/spf13/pflag v1.0.5/go.mod h1:McXfInJRrz4CZXVZOBLb0bTZqETkiAhM9Iw0y3An2Bg=
-github.com/stretchr/objx v0.1.0/go.mod h1:HFkY916IF+rwdDfMAkV7OtwuqBVzrE8GR6GFx+wExME=
-github.com/stretchr/objx v0.4.0/go.mod h1:YvHI0jy2hoMjB+UWwv71VJQ9isScKT/TqJzVSSt89Yw=
-github.com/stretchr/objx v0.5.0 h1:1zr/of2m5FGMsad5YfcqgdqdWrIhu+EBEJRhR1U7z/c=
-github.com/stretchr/objx v0.5.0/go.mod h1:Yh+to48EsGEfYuaHDzXPcE3xhTkx73EhmCGUpEOglKo=
-github.com/stretchr/testify v1.7.1/go.mod h1:6Fq8oRcR53rry900zMqJjRRixrwX3KX962/h/Wwjteg=
-github.com/stretchr/testify v1.8.0/go.mod h1:yNjHg4UonilssWZ8iaSj1OCr/vHnekPRkoO+kdMU+MU=
-github.com/stretchr/testify v1.8.4 h1:CcVxjf3Q8PM0mHUKJCdn+eZZtm5yQwehR5yeSVQQcUk=
-github.com/stretchr/testify v1.8.4/go.mod h1:sz/lmYIOXD/1dqDmKjjqLyZ2RngseejIcXlSw2iwfAo=
+github.com/stretchr/objx v0.5.2 h1:xuMeJ0Sdp5ZMRXx/aWO6RZxdr3beISkG5/G/aIRr3pY=
+github.com/stretchr/objx v0.5.2/go.mod h1:FRsXN1f5AsAjCGJKqEizvkpNtU+EGNCLh3NxZ/8L+MA=
+github.com/stretchr/testify v1.9.0 h1:HtqpIVDClZ4nwg75+f6Lvsy/wHu+3BoSGCbBAcpTsTg=
+github.com/stretchr/testify v1.9.0/go.mod h1:r2ic/lqez/lEtzL7wO/rwa5dbSLXVDPFyf8C91i36aY=
 github.com/zeebo/assert v1.3.0 h1:g7C04CbJuIDKNPFHmsk4hwZDO5O+kntRxzaUoNXj+IQ=
 github.com/zeebo/assert v1.3.0/go.mod h1:Pq9JiuJQpG8JLJdtkwrJESF0Foym2/D9XMU5ciN/wJ0=
 github.com/zeebo/xxh3 v1.0.2 h1:xZmwmqxHZA8AI603jOQ0tMqmBr9lPeFwGg6d+xy9DC0=
 github.com/zeebo/xxh3 v1.0.2/go.mod h1:5NWz9Sef7zIDm2JHfFlcQvNekmcEl9ekUZQQKCYaDcA=
-golang.org/x/sync v0.6.0 h1:5BMeUDZ7vkXGfEr1x9B4bRcTH4lpkTkpdh0T/J+qjbQ=
-golang.org/x/sync v0.6.0/go.mod h1:Czt+wKu1gCyEFDUtn0jG5QVvpJ6rzVqr5aXyt9drQfk=
+golang.org/x/sync v0.7.0 h1:YsImfSBoP9QPYL0xyKJPq0gcaJdG3rInoqxTWbfQu9M=
+golang.org/x/sync v0.7.0/go.mod h1:Czt+wKu1gCyEFDUtn0jG5QVvpJ6rzVqr5aXyt9drQfk=
 golang.org/x/sys v0.0.0-20220811171246-fbc7d0a398ab/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.6.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
-golang.org/x/sys v0.17.0 h1:25cE3gD+tdBA7lp7QfhuV+rJiE9YXTcS3VG1SqssI/Y=
-golang.org/x/sys v0.17.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
-golang.org/x/term v0.17.0 h1:mkTF7LCd6WGJNL3K1Ad7kwxNfYAW6a8a8QqtMblp/4U=
-golang.org/x/term v0.17.0/go.mod h1:lLRBjIVuehSbZlaOtGMbcMncT+aqLLLmKrsjNrUguwk=
+golang.org/x/sys v0.19.0 h1:q5f1RH2jigJ1MoAWp2KTp3gm5zAGFUTarQZ5U386+4o=
+golang.org/x/sys v0.19.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
+golang.org/x/term v0.19.0 h1:+ThwsDv+tYfnJFhF4L8jITxu1tdTWRTZpdsWgEgjL6Q=
+golang.org/x/term v0.19.0/go.mod h1:2CuTdWZ7KHSQwUzKva0cbMg6q2DMI3Mmxp+gKJbskEk=
 gopkg.in/check.v1 v0.0.0-20161208181325-20d25e280405/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/check.v1 v1.0.0-20180628173108-788fd7840127 h1:qIbj1fsPNlZgppZ+VLlY7N33q108Sa+fhmuc+sWQYwY=
 gopkg.in/check.v1 v1.0.0-20180628173108-788fd7840127/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
-gopkg.in/yaml.v3 v3.0.0-20200313102051-9f266ea9e77c/go.mod h1:K4uyk7z7BCEPqu6E+C64Yfv1cQ7kz7rIZviUmN+EgEM=
 gopkg.in/yaml.v3 v3.0.1 h1:fxVm/GzAzEWqLHuvctI91KS9hhNmmWOoWu0XTYJS7CA=
 gopkg.in/yaml.v3 v3.0.1/go.mod h1:K4uyk7z7BCEPqu6E+C64Yfv1cQ7kz7rIZviUmN+EgEM=
 mvdan.cc/sh/v3 v3.8.0 h1:ZxuJipLZwr/HLbASonmXtcvvC9HXY9d2lXZHnKGjFc8=
 mvdan.cc/sh/v3 v3.8.0/go.mod h1:w04623xkgBVo7/IUK89E0g8hBykgEpN0vgOj3RJr6MY=
```

### Comparing `go_task_bin-3.35.1/task/help.go` & `go_task_bin-3.36.0/task/help.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/init.go` & `go_task_bin-3.36.0/task/init.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/install-task.sh` & `go_task_bin-3.36.0/task/website/static/install.sh`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/compiler/compiler.go` & `go_task_bin-3.36.0/task/internal/compiler/compiler.go`

 * *Files 4% similar despite different names*

```diff
@@ -55,28 +55,17 @@
 		for k, v := range specialVars {
 			result.Set(k, ast.Var{Value: v})
 		}
 	}
 
 	getRangeFunc := func(dir string) func(k string, v ast.Var) error {
 		return func(k string, v ast.Var) error {
-			tr := templater.Templater{Vars: result}
+			cache := &templater.Cache{Vars: result}
 			// Replace values
-			newVar := ast.Var{}
-			switch value := v.Value.(type) {
-			case string:
-				newVar.Value = tr.Replace(value)
-			default:
-				newVar.Value = value
-			}
-			newVar.Sh = tr.Replace(v.Sh)
-			newVar.Ref = v.Ref
-			newVar.Json = tr.Replace(v.Json)
-			newVar.Yaml = tr.Replace(v.Yaml)
-			newVar.Dir = v.Dir
+			newVar := templater.ReplaceVar(v, cache)
 			// If the variable is a reference, we can resolve it
 			if newVar.Ref != "" {
 				newVar.Value = result.Get(newVar.Ref).Value
 			}
 			// If the variable should not be evaluated, but is nil, set it to an empty string
 			// This stops empty interface errors when using the templater to replace values later
 			if !evaluateShVars && newVar.Value == nil {
@@ -85,15 +74,15 @@
 			}
 			// If the variable should not be evaluated and it is set, we can set it and return
 			if !evaluateShVars {
 				result.Set(k, ast.Var{Value: newVar.Value})
 				return nil
 			}
 			// Now we can check for errors since we've handled all the cases when we don't want to evaluate
-			if err := tr.Err(); err != nil {
+			if err := cache.Err(); err != nil {
 				return err
 			}
 			// Evaluate JSON
 			if newVar.Json != "" {
 				if err := json.Unmarshal([]byte(newVar.Json), &newVar.Value); err != nil {
 					return err
 				}
@@ -120,34 +109,34 @@
 	}
 	rangeFunc := getRangeFunc(c.Dir)
 
 	var taskRangeFunc func(k string, v ast.Var) error
 	if t != nil {
 		// NOTE(@andreynering): We're manually joining these paths here because
 		// this is the raw task, not the compiled one.
-		tr := templater.Templater{Vars: result}
-		dir := tr.Replace(t.Dir)
-		if err := tr.Err(); err != nil {
+		cache := &templater.Cache{Vars: result}
+		dir := templater.Replace(t.Dir, cache)
+		if err := cache.Err(); err != nil {
 			return nil, err
 		}
 		dir = filepathext.SmartJoin(c.Dir, dir)
 		taskRangeFunc = getRangeFunc(dir)
 	}
 
 	if err := c.TaskfileEnv.Range(rangeFunc); err != nil {
 		return nil, err
 	}
 	if err := c.TaskfileVars.Range(rangeFunc); err != nil {
 		return nil, err
 	}
 	if t != nil {
-		if err := t.IncludedTaskfileVars.Range(taskRangeFunc); err != nil {
+		if err := t.IncludeVars.Range(rangeFunc); err != nil {
 			return nil, err
 		}
-		if err := t.IncludeVars.Range(rangeFunc); err != nil {
+		if err := t.IncludedTaskfileVars.Range(taskRangeFunc); err != nil {
 			return nil, err
 		}
 	}
 
 	if t == nil || call == nil {
 		return result, nil
 	}
```

### Comparing `go_task_bin-3.35.1/task/internal/editors/output.go` & `go_task_bin-3.36.0/task/internal/editors/output.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/execext/exec.go` & `go_task_bin-3.36.0/task/internal/execext/exec.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/exp/maps.go` & `go_task_bin-3.36.0/task/internal/exp/maps.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/experiments/experiments.go` & `go_task_bin-3.36.0/task/internal/experiments/experiments.go`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 package experiments
 
 import (
 	"fmt"
 	"io"
 	"os"
-	"path"
+	"path/filepath"
 	"slices"
 	"strings"
 	"text/tabwriter"
 
 	"github.com/joho/godotenv"
 	"github.com/spf13/pflag"
 
@@ -67,19 +67,19 @@
 	var dir, taskfile string
 	fs := pflag.NewFlagSet("experiments", pflag.ContinueOnError)
 	fs.StringVarP(&dir, "dir", "d", "", "Sets directory of execution.")
 	fs.StringVarP(&taskfile, "taskfile", "t", "", `Choose which Taskfile to run. Defaults to "Taskfile.yml".`)
 	_ = fs.Parse(os.Args[1:])
 	// If the directory is set, find a .env file in that directory.
 	if dir != "" {
-		return path.Join(dir, ".env")
+		return filepath.Join(dir, ".env")
 	}
 	// If the taskfile is set, find a .env file in the directory containing the Taskfile.
 	if taskfile != "" {
-		return path.Join(path.Dir(taskfile), ".env")
+		return filepath.Join(filepath.Dir(taskfile), ".env")
 	}
 	// Otherwise just use the current working directory.
 	return ".env"
 }
 
 func readDotEnv() {
 	env, _ := godotenv.Read(getEnvFilePath())
```

### Comparing `go_task_bin-3.35.1/task/internal/filepathext/filepathext.go` & `go_task_bin-3.36.0/task/internal/filepathext/filepathext.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/fingerprint/checker.go` & `go_task_bin-3.36.0/task/internal/fingerprint/checker.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/fingerprint/glob.go` & `go_task_bin-3.36.0/task/internal/fingerprint/glob.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/fingerprint/sources_checksum.go` & `go_task_bin-3.36.0/task/internal/fingerprint/sources_checksum.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/fingerprint/sources_timestamp.go` & `go_task_bin-3.36.0/task/internal/fingerprint/sources_timestamp.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/fingerprint/status.go` & `go_task_bin-3.36.0/task/internal/fingerprint/status.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/fingerprint/task.go` & `go_task_bin-3.36.0/task/internal/fingerprint/task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/fingerprint/task_test.go` & `go_task_bin-3.36.0/task/internal/fingerprint/task_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/flags/flags.go` & `go_task_bin-3.36.0/task/internal/flags/flags.go`

 * *Files 2% similar despite different names*

```diff
@@ -127,18 +127,14 @@
 	}
 
 	if Global && Dir != "" {
 		log.Fatal("task: You can't set both --global and --dir")
 		return nil
 	}
 
-	if Dir != "" && Entrypoint != "" {
-		return errors.New("task: You can't set both --dir and --taskfile")
-	}
-
 	if Output.Name != "group" {
 		if Output.Group.Begin != "" {
 			return errors.New("task: You can't set --output-group-begin without --output=group")
 		}
 		if Output.Group.End != "" {
 			return errors.New("task: You can't set --output-group-end without --output=group")
 		}
```

### Comparing `go_task_bin-3.35.1/task/internal/goext/meta.go` & `go_task_bin-3.36.0/task/internal/goext/meta.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/logger/logger.go` & `go_task_bin-3.36.0/task/internal/logger/logger.go`

 * *Files 16% similar despite different names*

```diff
@@ -21,51 +21,70 @@
 
 type (
 	Color     func() PrintFunc
 	PrintFunc func(io.Writer, string, ...any)
 )
 
 func Default() PrintFunc {
-	return color.New(envColor("TASK_COLOR_RESET", color.Reset)).FprintfFunc()
+	return color.New(envColor("TASK_COLOR_RESET", color.Reset)...).FprintfFunc()
 }
 
 func Blue() PrintFunc {
-	return color.New(envColor("TASK_COLOR_BLUE", color.FgBlue)).FprintfFunc()
+	return color.New(envColor("TASK_COLOR_BLUE", color.FgBlue)...).FprintfFunc()
 }
 
 func Green() PrintFunc {
-	return color.New(envColor("TASK_COLOR_GREEN", color.FgGreen)).FprintfFunc()
+	return color.New(envColor("TASK_COLOR_GREEN", color.FgGreen)...).FprintfFunc()
 }
 
 func Cyan() PrintFunc {
-	return color.New(envColor("TASK_COLOR_CYAN", color.FgCyan)).FprintfFunc()
+	return color.New(envColor("TASK_COLOR_CYAN", color.FgCyan)...).FprintfFunc()
 }
 
 func Yellow() PrintFunc {
-	return color.New(envColor("TASK_COLOR_YELLOW", color.FgYellow)).FprintfFunc()
+	return color.New(envColor("TASK_COLOR_YELLOW", color.FgYellow)...).FprintfFunc()
 }
 
 func Magenta() PrintFunc {
-	return color.New(envColor("TASK_COLOR_MAGENTA", color.FgMagenta)).FprintfFunc()
+	return color.New(envColor("TASK_COLOR_MAGENTA", color.FgMagenta)...).FprintfFunc()
 }
 
 func Red() PrintFunc {
-	return color.New(envColor("TASK_COLOR_RED", color.FgRed)).FprintfFunc()
+	return color.New(envColor("TASK_COLOR_RED", color.FgRed)...).FprintfFunc()
 }
 
-func envColor(env string, defaultColor color.Attribute) color.Attribute {
+func envColor(env string, defaultColor color.Attribute) []color.Attribute {
 	if os.Getenv("FORCE_COLOR") != "" {
 		color.NoColor = false
 	}
 
-	override, err := strconv.Atoi(os.Getenv(env))
-	if err == nil {
-		return color.Attribute(override)
+	// Fetch the environment variable
+	override := os.Getenv(env)
+
+	// First, try splitting the string by commas (RGB shortcut syntax) and if it
+	// matches, then prepend the 256-color foreground escape sequence.
+	// Otherwise, split by semicolons (ANSI color codes) and use them as is.
+	attributeStrs := strings.Split(override, ",")
+	if len(attributeStrs) == 3 {
+		attributeStrs = append([]string{"38", "2"}, attributeStrs...)
+	} else {
+		attributeStrs = strings.Split(override, ";")
+	}
+
+	// Loop over the attributes and convert them to integers
+	attributes := make([]color.Attribute, len(attributeStrs))
+	for i, attributeStr := range attributeStrs {
+		attribute, err := strconv.Atoi(attributeStr)
+		if err != nil {
+			return []color.Attribute{defaultColor}
+		}
+		attributes[i] = color.Attribute(attribute)
 	}
-	return defaultColor
+
+	return attributes
 }
 
 // Logger is just a wrapper that prints stuff to STDOUT or STDERR,
 // with optional color.
 type Logger struct {
 	Stdin      io.Reader
 	Stdout     io.Writer
```

### Comparing `go_task_bin-3.35.1/task/internal/mocks/sources_checkable.go` & `go_task_bin-3.36.0/task/internal/mocks/sources_checkable.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/mocks/status_checkable.go` & `go_task_bin-3.36.0/task/internal/mocks/status_checkable.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/omap/orderedmap.go` & `go_task_bin-3.36.0/task/internal/omap/orderedmap.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/omap/orderedmap_test.go` & `go_task_bin-3.36.0/task/internal/omap/orderedmap_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/output/group.go` & `go_task_bin-3.36.0/task/internal/output/group.go`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 package output
 
 import (
 	"bytes"
 	"io"
+
+	"github.com/go-task/task/v3/internal/templater"
 )
 
 type Group struct {
 	Begin, End string
 	ErrorOnly  bool
 }
 
-func (g Group) WrapWriter(stdOut, _ io.Writer, _ string, tmpl Templater) (io.Writer, io.Writer, CloseFunc) {
+func (g Group) WrapWriter(stdOut, _ io.Writer, _ string, cache *templater.Cache) (io.Writer, io.Writer, CloseFunc) {
 	gw := &groupWriter{writer: stdOut}
 	if g.Begin != "" {
-		gw.begin = tmpl.Replace(g.Begin) + "\n"
+		gw.begin = templater.Replace(g.Begin, cache) + "\n"
 	}
 	if g.End != "" {
-		gw.end = tmpl.Replace(g.End) + "\n"
+		gw.end = templater.Replace(g.End, cache) + "\n"
 	}
 	return gw, gw, func(err error) error {
 		if g.ErrorOnly && err == nil {
 			return nil
 		}
 
 		return gw.close()
```

### Comparing `go_task_bin-3.35.1/task/internal/output/output_test.go` & `go_task_bin-3.36.0/task/internal/output/output_test.go`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 	assert.Equal(t, "", b.String())
 
 	require.NoError(t, cleanup(nil))
 	assert.Equal(t, "out\nout\nerr\nerr\nout\nerr\n", b.String())
 }
 
 func TestGroupWithBeginEnd(t *testing.T) {
-	tmpl := templater.Templater{
+	tmpl := templater.Cache{
 		Vars: &ast.Vars{
 			OrderedMap: omap.FromMap(map[string]ast.Var{
 				"VAR1": {Value: "example-value"},
 			}),
 		},
 	}
```

### Comparing `go_task_bin-3.35.1/task/internal/output/prefixed.go` & `go_task_bin-3.36.0/task/internal/output/prefixed.go`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 package output
 
 import (
 	"bytes"
 	"fmt"
 	"io"
 	"strings"
+
+	"github.com/go-task/task/v3/internal/templater"
 )
 
 type Prefixed struct{}
 
-func (Prefixed) WrapWriter(stdOut, _ io.Writer, prefix string, _ Templater) (io.Writer, io.Writer, CloseFunc) {
+func (Prefixed) WrapWriter(stdOut, _ io.Writer, prefix string, _ *templater.Cache) (io.Writer, io.Writer, CloseFunc) {
 	pw := &prefixWriter{writer: stdOut, prefix: prefix}
 	return pw, pw, func(error) error { return pw.close() }
 }
 
 type prefixWriter struct {
 	writer io.Writer
 	prefix string
```

### Comparing `go_task_bin-3.35.1/task/internal/sort/sorter.go` & `go_task_bin-3.36.0/task/internal/sort/sorter.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/sort/sorter_test.go` & `go_task_bin-3.36.0/task/internal/sort/sorter_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/summary/summary.go` & `go_task_bin-3.36.0/task/internal/summary/summary.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/summary/summary_test.go` & `go_task_bin-3.36.0/task/internal/summary/summary_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/internal/templater/funcs.go` & `go_task_bin-3.36.0/task/internal/templater/funcs.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/package-lock.json` & `go_task_bin-3.36.0/task/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'version'": "'3.36.0'"}*

```diff
@@ -24,9 +24,9 @@
             },
             "integrity": "sha512-vQbdtBvesHm8EUFHX8QKg4rbBodmu9VsAXH1ozpbiN5jdTMOYHTCMM31EurAYmY+rNNtxJQ4JGy6t383RPlqbw==",
             "resolved": "https://registry.npmjs.org/@go-task/go-npm/-/go-npm-0.2.0.tgz",
             "version": "0.2.0"
         }
     },
     "requires": true,
-    "version": "3.35.1"
+    "version": "3.36.0"
 }
```

### Comparing `go_task_bin-3.35.1/task/package.json` & `go_task_bin-3.36.0/task/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'3.36.0'"}*

```diff
@@ -26,9 +26,9 @@
         "type": "git",
         "url": "https://github.com/go-task/task.git"
     },
     "scripts": {
         "postinstall": "go-npm install",
         "preuninstall": "go-npm uninstall"
     },
-    "version": "3.35.1"
+    "version": "3.36.0"
 }
```

### Comparing `go_task_bin-3.35.1/task/precondition.go` & `go_task_bin-3.36.0/task/precondition.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/requires.go` & `go_task_bin-3.36.0/task/requires.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/setup.go` & `go_task_bin-3.36.0/task/setup.go`

 * *Files 1% similar despite different names*

```diff
@@ -50,19 +50,19 @@
 	}
 	e.setupDefaults()
 	e.setupConcurrencyState()
 	return nil
 }
 
 func (e *Executor) getRootNode() (taskfile.Node, error) {
-	node, err := taskfile.NewRootNode(e.Dir, e.Entrypoint, e.Insecure)
+	node, err := taskfile.NewRootNode(e.Logger, e.Entrypoint, e.Dir, e.Insecure, e.Timeout)
 	if err != nil {
 		return nil, err
 	}
-	e.Dir = node.BaseDir()
+	e.Dir = node.Dir()
 	return node, err
 }
 
 func (e *Executor) readTaskfile(node taskfile.Node) error {
 	var err error
 	e.Taskfile, err = taskfile.Read(
 		node,
```

### Comparing `go_task_bin-3.35.1/task/signals.go` & `go_task_bin-3.36.0/task/signals.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/signals_test.go` & `go_task_bin-3.36.0/task/signals_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/status.go` & `go_task_bin-3.36.0/task/status.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/task.go` & `go_task_bin-3.36.0/task/task.go`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,15 @@
 		}
 
 		outputWrapper := e.Output
 		if t.Interactive {
 			outputWrapper = output.Interleaved{}
 		}
 		vars, err := e.Compiler.FastGetVariables(t, call)
-		outputTemplater := &templater.Templater{Vars: vars}
+		outputTemplater := &templater.Cache{Vars: vars}
 		if err != nil {
 			return fmt.Errorf("task: failed to get variables: %w", err)
 		}
 		stdOut, stdErr, close := outputWrapper.WrapWriter(e.Stdout, e.Stderr, t.Prefix, outputTemplater)
 
 		err = execext.RunCommand(ctx, &execext.RunCommandOptions{
 			Command:   cmd.Cmd,
```

### Comparing `go_task_bin-3.35.1/task/task_test.go` & `go_task_bin-3.36.0/task/task_test.go`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 	"fmt"
 	"io"
 	"os"
 	"path/filepath"
 	"regexp"
 	"runtime"
 	"strings"
+	"sync"
 	"testing"
 
 	"github.com/Masterminds/semver/v3"
 	"github.com/stretchr/testify/assert"
 	"github.com/stretchr/testify/require"
 
 	"github.com/go-task/task/v3"
@@ -22,14 +23,29 @@
 	"github.com/go-task/task/v3/taskfile/ast"
 )
 
 func init() {
 	_ = os.Setenv("NO_COLOR", "1")
 }
 
+// SyncBuffer is a threadsafe buffer for testing.
+// Some times replace stdout/stderr with a buffer to capture output.
+// stdout and stderr are threadsafe, but a regular bytes.Buffer is not.
+// Using this instead helps prevents race conditions with output.
+type SyncBuffer struct {
+	buf bytes.Buffer
+	mu  sync.Mutex
+}
+
+func (sb *SyncBuffer) Write(p []byte) (n int, err error) {
+	sb.mu.Lock()
+	defer sb.mu.Unlock()
+	return sb.buf.Write(p)
+}
+
 // fileContentTest provides a basic reusable test-case for running a Taskfile
 // and inspect generated files.
 type fileContentTest struct {
 	Dir        string
 	Entrypoint string
 	Target     string
 	TrimSpace  bool
@@ -53,15 +69,15 @@
 		Stderr:     io.Discard,
 	}
 	require.NoError(t, e.Setup(), "e.Setup()")
 	require.NoError(t, e.Run(context.Background(), &ast.Call{Task: fct.Target}), "e.Run(target)")
 
 	for name, expectContent := range fct.Files {
 		t.Run(fct.name(name), func(t *testing.T) {
-			path := filepathext.SmartJoin(fct.Dir, name)
+			path := filepathext.SmartJoin(e.Dir, name)
 			b, err := os.ReadFile(path)
 			require.NoError(t, err, "Error reading file")
 			s := string(b)
 			if fct.TrimSpace {
 				s = strings.TrimSpace(s)
 			}
 			assert.Equal(t, expectContent, s, "unexpected file content in %s", path)
@@ -1103,16 +1119,16 @@
 	err := e.Setup()
 	require.Error(t, err)
 	assert.Equal(t, expected, err.Error())
 }
 
 func TestIncludesFromCustomTaskfile(t *testing.T) {
 	tt := fileContentTest{
+		Entrypoint: "testdata/includes_yaml/Custom.ext",
 		Dir:        "testdata/includes_yaml",
-		Entrypoint: "Custom.ext",
 		Target:     "default",
 		TrimSpace:  true,
 		Files: map[string]string{
 			"main.txt":                         "main",
 			"included_with_yaml_extension.txt": "included_with_yaml_extension",
 			"included_with_custom_file.txt":    "included_with_custom_file",
 		},
@@ -1466,24 +1482,20 @@
 			"include.txt": "INCLUDE1='from_include1' INCLUDE2='from_include2'\n",
 		},
 	}
 	tt.Run(t)
 }
 
 func TestDotenvShouldErrorWhenIncludingDependantDotenvs(t *testing.T) {
-	const dir = "testdata/dotenv/error_included_envs"
-	const entry = "Taskfile.yml"
-
 	var buff bytes.Buffer
 	e := task.Executor{
-		Dir:        dir,
-		Entrypoint: entry,
-		Summary:    true,
-		Stdout:     &buff,
-		Stderr:     &buff,
+		Dir:     "testdata/dotenv/error_included_envs",
+		Summary: true,
+		Stdout:  &buff,
+		Stderr:  &buff,
 	}
 
 	err := e.Setup()
 	require.Error(t, err)
 	assert.Contains(t, err.Error(), "move the dotenv")
 }
 
@@ -1765,15 +1777,15 @@
 task: [foo:lib:greet] echo 'Hello foo'
 Hello foo
 task: [bar:lib:greet] echo 'Hello bar'
 Hello bar
 `)
 	require.NoError(t, e.Run(context.Background(), &ast.Call{Task: "default"}))
 	t.Log(buff.String())
-	assert.Equal(t, strings.TrimSpace(buff.String()), expectedOutputOrder)
+	assert.Equal(t, expectedOutputOrder, strings.TrimSpace(buff.String()))
 }
 
 func TestErrorCode(t *testing.T) {
 	const dir = "testdata/error_code"
 	tests := []struct {
 		name     string
 		task     string
@@ -2195,15 +2207,15 @@
 			}
 			require.NoError(t, e.Setup())
 			require.NoError(t, e.Run(context.Background(), &ast.Call{Task: "task-with-dep"}))
 		})
 	}
 }
 
-func TestFor(t *testing.T) {
+func TestForCmds(t *testing.T) {
 	tests := []struct {
 		name           string
 		expectedOutput string
 	}{
 		{
 			name:           "loop-explicit",
 			expectedOutput: "a\nb\nc\n",
@@ -2236,25 +2248,85 @@
 			name:           "loop-different-tasks",
 			expectedOutput: "1\n2\n3\n",
 		},
 	}
 
 	for _, test := range tests {
 		t.Run(test.name, func(t *testing.T) {
-			var buff bytes.Buffer
+			var stdOut bytes.Buffer
+			var stdErr bytes.Buffer
 			e := task.Executor{
-				Dir:    "testdata/for",
+				Dir:    "testdata/for/cmds",
+				Stdout: &stdOut,
+				Stderr: &stdErr,
+				Silent: true,
+				Force:  true,
+			}
+			require.NoError(t, e.Setup())
+			require.NoError(t, e.Run(context.Background(), &ast.Call{Task: test.name}))
+			assert.Equal(t, test.expectedOutput, stdOut.String())
+		})
+	}
+}
+
+func TestForDeps(t *testing.T) {
+	tests := []struct {
+		name                   string
+		expectedOutputContains []string
+	}{
+		{
+			name:                   "loop-explicit",
+			expectedOutputContains: []string{"a\n", "b\n", "c\n"},
+		},
+		{
+			name:                   "loop-sources",
+			expectedOutputContains: []string{"bar\n", "foo\n"},
+		},
+		{
+			name:                   "loop-sources-glob",
+			expectedOutputContains: []string{"bar\n", "foo\n"},
+		},
+		{
+			name:                   "loop-vars",
+			expectedOutputContains: []string{"foo\n", "bar\n"},
+		},
+		{
+			name:                   "loop-vars-sh",
+			expectedOutputContains: []string{"bar\n", "foo\n"},
+		},
+		{
+			name:                   "loop-task",
+			expectedOutputContains: []string{"foo\n", "bar\n"},
+		},
+		{
+			name:                   "loop-task-as",
+			expectedOutputContains: []string{"foo\n", "bar\n"},
+		},
+		{
+			name:                   "loop-different-tasks",
+			expectedOutputContains: []string{"1\n", "2\n", "3\n"},
+		},
+	}
+
+	for _, test := range tests {
+		t.Run(test.name, func(t *testing.T) {
+			// We need to use a sync buffer here as deps are run concurrently
+			var buff SyncBuffer
+			e := task.Executor{
+				Dir:    "testdata/for/deps",
 				Stdout: &buff,
 				Stderr: &buff,
 				Silent: true,
 				Force:  true,
 			}
 			require.NoError(t, e.Setup())
 			require.NoError(t, e.Run(context.Background(), &ast.Call{Task: test.name}))
-			assert.Equal(t, test.expectedOutput, buff.String())
+			for _, expectedOutputContains := range test.expectedOutputContains {
+				assert.Contains(t, buff.buf.String(), expectedOutputContains)
+			}
 		})
 	}
 }
 
 func TestWildcard(t *testing.T) {
 	tests := []struct {
 		name           string
```

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/cmd.go` & `go_task_bin-3.36.0/task/taskfile/ast/cmd.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/dep.go` & `go_task_bin-3.36.0/task/taskfile/ast/dep.go`

 * *Files 23% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 
 	"gopkg.in/yaml.v3"
 )
 
 // Dep is a task dependency
 type Dep struct {
 	Task   string
+	For    *For
 	Vars   *Vars
 	Silent bool
 }
 
 func (d *Dep) DeepCopy() *Dep {
 	if d == nil {
 		return nil
 	}
 	return &Dep{
 		Task:   d.Task,
+		For:    d.For.DeepCopy(),
 		Vars:   d.Vars.DeepCopy(),
 		Silent: d.Silent,
 	}
 }
 
 func (d *Dep) UnmarshalYAML(node *yaml.Node) error {
 	switch node.Kind {
@@ -34,21 +36,23 @@
 		}
 		d.Task = task
 		return nil
 
 	case yaml.MappingNode:
 		var taskCall struct {
 			Task   string
+			For    *For
 			Vars   *Vars
 			Silent bool
 		}
 		if err := node.Decode(&taskCall); err != nil {
 			return err
 		}
 		d.Task = taskCall.Task
+		d.For = taskCall.For
 		d.Vars = taskCall.Vars
 		d.Silent = taskCall.Silent
 		return nil
 	}
 
 	return fmt.Errorf("cannot unmarshal %s into dependency", node.ShortTag())
 }
```

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/for.go` & `go_task_bin-3.36.0/task/taskfile/ast/for.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/glob.go` & `go_task_bin-3.36.0/task/taskfile/ast/glob.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/include.go` & `go_task_bin-3.36.0/task/taskfile/ast/include.go`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 package ast
 
 import (
 	"fmt"
-	"path/filepath"
-	"strings"
 
 	"gopkg.in/yaml.v3"
 
-	"github.com/go-task/task/v3/internal/execext"
-	"github.com/go-task/task/v3/internal/filepathext"
 	omap "github.com/go-task/task/v3/internal/omap"
 )
 
 // Include represents information about included taskfiles
 type Include struct {
 	Namespace      string
 	Taskfile       string
 	Dir            string
 	Optional       bool
 	Internal       bool
 	Aliases        []string
 	AdvancedImport bool
 	Vars           *Vars
-	BaseDir        string // The directory from which the including taskfile was loaded; used to resolve relative paths
 }
 
 // Includes represents information about included tasksfiles
 type Includes struct {
 	omap.OrderedMap[string, Include]
 }
 
@@ -116,43 +111,9 @@
 		Namespace:      include.Namespace,
 		Taskfile:       include.Taskfile,
 		Dir:            include.Dir,
 		Optional:       include.Optional,
 		Internal:       include.Internal,
 		AdvancedImport: include.AdvancedImport,
 		Vars:           include.Vars.DeepCopy(),
-		BaseDir:        include.BaseDir,
 	}
 }
-
-// FullTaskfilePath returns the fully qualified path to the included taskfile
-func (include *Include) FullTaskfilePath() (string, error) {
-	return include.resolvePath(include.Taskfile)
-}
-
-// FullDirPath returns the fully qualified path to the included taskfile's working directory
-func (include *Include) FullDirPath() (string, error) {
-	return include.resolvePath(include.Dir)
-}
-
-func (include *Include) resolvePath(path string) (string, error) {
-	// If the file is remote, we don't need to resolve the path
-	if strings.Contains(include.Taskfile, "://") {
-		return path, nil
-	}
-
-	path, err := execext.Expand(path)
-	if err != nil {
-		return "", err
-	}
-
-	if filepathext.IsAbs(path) {
-		return path, nil
-	}
-
-	result, err := filepath.Abs(filepathext.SmartJoin(include.BaseDir, path))
-	if err != nil {
-		return "", fmt.Errorf("task: error resolving path %s relative to %s: %w", path, include.BaseDir, err)
-	}
-
-	return result, nil
-}
```

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/output.go` & `go_task_bin-3.36.0/task/taskfile/ast/output.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/platforms.go` & `go_task_bin-3.36.0/task/taskfile/ast/platforms.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/platforms_test.go` & `go_task_bin-3.36.0/task/taskfile/ast/platforms_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/precondition.go` & `go_task_bin-3.36.0/task/taskfile/ast/precondition.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/precondition_test.go` & `go_task_bin-3.36.0/task/taskfile/ast/precondition_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/task.go` & `go_task_bin-3.36.0/task/taskfile/ast/task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/taskfile.go` & `go_task_bin-3.36.0/task/taskfile/ast/taskfile.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/taskfile_test.go` & `go_task_bin-3.36.0/task/taskfile/ast/taskfile_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/tasks.go` & `go_task_bin-3.36.0/task/taskfile/ast/tasks.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/ast/var.go` & `go_task_bin-3.36.0/task/taskfile/ast/var.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/cache.go` & `go_task_bin-3.36.0/task/taskfile/cache.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/taskfile/dotenv.go` & `go_task_bin-3.36.0/task/taskfile/dotenv.go`

 * *Files 23% similar despite different names*

```diff
@@ -18,19 +18,18 @@
 
 	vars, err := c.GetTaskfileVariables()
 	if err != nil {
 		return nil, err
 	}
 
 	env := &ast.Vars{}
-
-	tr := templater.Templater{Vars: vars}
+	cache := &templater.Cache{Vars: vars}
 
 	for _, dotEnvPath := range tf.Dotenv {
-		dotEnvPath = tr.Replace(dotEnvPath)
+		dotEnvPath = templater.Replace(dotEnvPath, cache)
 		if dotEnvPath == "" {
 			continue
 		}
 		dotEnvPath = filepathext.SmartJoin(dir, dotEnvPath)
 
 		if _, err := os.Stat(dotEnvPath); os.IsNotExist(err) {
 			continue
```

### Comparing `go_task_bin-3.35.1/task/taskfile/node.go` & `go_task_bin-3.36.0/task/taskfile/node.go`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 package taskfile
 
 import (
 	"context"
 	"os"
 	"path/filepath"
 	"strings"
+	"time"
 
 	"github.com/go-task/task/v3/errors"
 	"github.com/go-task/task/v3/internal/experiments"
+	"github.com/go-task/task/v3/internal/logger"
 )
 
 type Node interface {
 	Read(ctx context.Context) ([]byte, error)
 	Parent() Node
 	Location() string
+	Dir() string
 	Optional() bool
 	Remote() bool
-	BaseDir() string
+	ResolveEntrypoint(entrypoint string) (string, error)
+	ResolveDir(dir string) (string, error)
 }
 
 func NewRootNode(
-	dir string,
+	l *logger.Logger,
 	entrypoint string,
+	dir string,
 	insecure bool,
+	timeout time.Duration,
 ) (Node, error) {
 	dir = getDefaultDir(entrypoint, dir)
 	// Check if there is something to read on STDIN
 	stat, _ := os.Stdin.Stat()
 	if (stat.Mode()&os.ModeCharDevice) == 0 && stat.Size() > 0 {
 		return NewStdinNode(dir)
 	}
-	// If no entrypoint is specified, search for a taskfile
-	if entrypoint == "" {
-		root, err := ExistsWalk(dir)
-		if err != nil {
-			return nil, err
-		}
-		return NewNode(root, insecure)
-	}
-	// Use the specified entrypoint
-	uri := filepath.Join(dir, entrypoint)
-	return NewNode(uri, insecure)
+	return NewNode(l, entrypoint, dir, insecure, timeout)
 }
 
 func NewNode(
-	uri string,
+	l *logger.Logger,
+	entrypoint string,
+	dir string,
 	insecure bool,
+	timeout time.Duration,
 	opts ...NodeOption,
 ) (Node, error) {
 	var node Node
 	var err error
-	switch getScheme(uri) {
+	switch getScheme(entrypoint) {
 	case "http", "https":
-		node, err = NewHTTPNode(uri, insecure, opts...)
+		node, err = NewHTTPNode(l, entrypoint, dir, insecure, timeout, opts...)
 	default:
 		// If no other scheme matches, we assume it's a file
-		node, err = NewFileNode(uri, opts...)
+		node, err = NewFileNode(l, entrypoint, dir, opts...)
 	}
 	if node.Remote() && !experiments.RemoteTaskfiles.Enabled {
 		return nil, errors.New("task: Remote taskfiles are not enabled. You can read more about this experiment and how to enable it at https://taskfile.dev/experiments/remote-taskfiles")
 	}
 	return node, err
 }
```

### Comparing `go_task_bin-3.35.1/task/taskfile/node_base.go` & `go_task_bin-3.36.0/task/taskfile/node_base.go`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 	// BaseNode is a generic node that implements the Parent() and Optional()
 	// methods of the NodeReader interface. It does not implement the Read() method
 	// and it designed to be embedded in other node types so that this boilerplate
 	// code does not need to be repeated.
 	BaseNode struct {
 		parent   Node
 		optional bool
+		dir      string
 	}
 )
 
-func NewBaseNode(opts ...NodeOption) *BaseNode {
+func NewBaseNode(dir string, opts ...NodeOption) *BaseNode {
 	node := &BaseNode{
 		parent:   nil,
 		optional: false,
+		dir:      dir,
 	}
 
 	// Apply options
 	for _, opt := range opts {
 		opt(node)
 	}
 
@@ -41,7 +43,11 @@
 		node.optional = optional
 	}
 }
 
 func (node *BaseNode) Optional() bool {
 	return node.optional
 }
+
+func (node *BaseNode) Dir() string {
+	return node.dir
+}
```

### Comparing `go_task_bin-3.35.1/task/taskfile/reader.go` & `go_task_bin-3.36.0/task/taskfile/reader.go`

 * *Files 11% similar despite different names*

```diff
@@ -44,48 +44,41 @@
 		}
 
 		// Check that the Taskfile is set and has a schema version
 		if tf == nil || tf.Version == nil {
 			return nil, &errors.TaskfileVersionCheckError{URI: node.Location()}
 		}
 
-		if dir := node.BaseDir(); dir != "" {
-			_ = tf.Includes.Range(func(namespace string, include ast.Include) error {
-				// Set the base directory for resolving relative paths, but only if not already set
-				if include.BaseDir == "" {
-					include.BaseDir = dir
-					tf.Includes.Set(namespace, include)
-				}
-				return nil
-			})
-		}
-
 		err = tf.Includes.Range(func(namespace string, include ast.Include) error {
-			tr := templater.Templater{Vars: tf.Vars}
+			cache := &templater.Cache{Vars: tf.Vars}
 			include = ast.Include{
 				Namespace:      include.Namespace,
-				Taskfile:       tr.Replace(include.Taskfile),
-				Dir:            tr.Replace(include.Dir),
+				Taskfile:       templater.Replace(include.Taskfile, cache),
+				Dir:            templater.Replace(include.Dir, cache),
 				Optional:       include.Optional,
 				Internal:       include.Internal,
 				Aliases:        include.Aliases,
 				AdvancedImport: include.AdvancedImport,
 				Vars:           include.Vars,
-				BaseDir:        include.BaseDir,
 			}
-			if err := tr.Err(); err != nil {
+			if err := cache.Err(); err != nil {
 				return err
 			}
 
-			uri, err := include.FullTaskfilePath()
+			entrypoint, err := node.ResolveEntrypoint(include.Taskfile)
 			if err != nil {
 				return err
 			}
 
-			includeReaderNode, err := NewNode(uri, insecure,
+			dir, err := node.ResolveDir(include.Dir)
+			if err != nil {
+				return err
+			}
+
+			includeReaderNode, err := NewNode(l, entrypoint, dir, insecure, timeout,
 				WithParent(node),
 				WithOptional(include.Optional),
 			)
 			if err != nil {
 				if include.Optional {
 					return nil
 				}
@@ -105,19 +98,14 @@
 			}
 
 			if len(includedTaskfile.Dotenv) > 0 {
 				return ErrIncludedTaskfilesCantHaveDotenvs
 			}
 
 			if include.AdvancedImport {
-				dir, err := include.FullDirPath()
-				if err != nil {
-					return err
-				}
-
 				// nolint: errcheck
 				includedTaskfile.Vars.Range(func(k string, v ast.Var) error {
 					o := v
 					o.Dir = dir
 					includedTaskfile.Vars.Set(k, o)
 					return nil
 				})
```

### Comparing `go_task_bin-3.35.1/task/testdata/deps/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/deps/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/dir/dynamic_var/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/dir/dynamic_var/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/for/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/for/cmds/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/generates/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/generates/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/includes/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/includes/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/params/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/params/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/platforms/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/platforms/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/silent/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/silent/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/summary/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/summary/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/vars/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/vars/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/vars/any/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/vars/any/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/testdata/vars/any2/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/vars/any2/Taskfile.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 version: '3'
 
 tasks:
   default:
     - task: map
+    - task: nested-map
+    - task: slice
     - task: ref
     - task: ref-sh
     - task: ref-dep
     - task: json
     - task: yaml
 
   map:
@@ -15,14 +17,32 @@
         map: {"name":"Alice","age":30,"children":[{"name":"Bob","age":5},{"name":"Charlie","age":3},{"name":"Diane","age":1}]}
     cmds:
       - task: print-var
         vars:
           VAR:
             ref: MAP
 
+  nested-map:
+    vars:
+      FOO: "foo"
+      nested:
+        map:
+          variables:
+            work: "{{.FOO}}"
+    cmds:
+      - echo {{.nested.variables.work}}
+
+  slice:
+    vars:
+      FOO: "foo"
+      BAR: "bar"
+      slice_variables_work: ["{{.FOO}}","{{.BAR}}"]
+    cmds:
+      - echo {{index .slice_variables_work 0}} {{index .slice_variables_work 1}}
+
   ref:
     vars:
       MAP:
         map: {"name":"Alice","age":30,"children":[{"name":"Bob","age":5},{"name":"Charlie","age":3},{"name":"Diane","age":1}]}
       MAP_REF:
         ref: MAP
     cmds:
```

### Comparing `go_task_bin-3.35.1/task/testdata/wildcards/Taskfile.yml` & `go_task_bin-3.36.0/task/testdata/wildcards/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.35.1/task/variables.go` & `go_task_bin-3.36.0/task/variables.go`

 * *Files 27% similar despite different names*

```diff
@@ -38,38 +38,38 @@
 	} else {
 		vars, err = e.Compiler.FastGetVariables(origTask, call)
 	}
 	if err != nil {
 		return nil, err
 	}
 
-	r := templater.Templater{Vars: vars}
+	cache := &templater.Cache{Vars: vars}
 
 	new := ast.Task{
 		Task:                 origTask.Task,
-		Label:                r.Replace(origTask.Label),
-		Desc:                 r.Replace(origTask.Desc),
-		Prompt:               r.Replace(origTask.Prompt),
-		Summary:              r.Replace(origTask.Summary),
+		Label:                templater.Replace(origTask.Label, cache),
+		Desc:                 templater.Replace(origTask.Desc, cache),
+		Prompt:               templater.Replace(origTask.Prompt, cache),
+		Summary:              templater.Replace(origTask.Summary, cache),
 		Aliases:              origTask.Aliases,
-		Sources:              r.ReplaceGlobs(origTask.Sources),
-		Generates:            r.ReplaceGlobs(origTask.Generates),
-		Dir:                  r.Replace(origTask.Dir),
+		Sources:              templater.ReplaceGlobs(origTask.Sources, cache),
+		Generates:            templater.ReplaceGlobs(origTask.Generates, cache),
+		Dir:                  templater.Replace(origTask.Dir, cache),
 		Set:                  origTask.Set,
 		Shopt:                origTask.Shopt,
 		Vars:                 nil,
 		Env:                  nil,
-		Dotenv:               r.ReplaceSlice(origTask.Dotenv),
+		Dotenv:               templater.Replace(origTask.Dotenv, cache),
 		Silent:               origTask.Silent,
 		Interactive:          origTask.Interactive,
 		Internal:             origTask.Internal,
-		Method:               r.Replace(origTask.Method),
-		Prefix:               r.Replace(origTask.Prefix),
+		Method:               templater.Replace(origTask.Method, cache),
+		Prefix:               templater.Replace(origTask.Prefix, cache),
 		IgnoreError:          origTask.IgnoreError,
-		Run:                  r.Replace(origTask.Run),
+		Run:                  templater.Replace(origTask.Run, cache),
 		IncludeVars:          origTask.IncludeVars,
 		IncludedTaskfileVars: origTask.IncludedTaskfileVars,
 		Platforms:            origTask.Platforms,
 		Location:             origTask.Location,
 		Requires:             origTask.Requires,
 		Watch:                origTask.Watch,
 	}
@@ -100,17 +100,17 @@
 					dotenvEnvs.Set(key, ast.Var{Value: value})
 				}
 			}
 		}
 	}
 
 	new.Env = &ast.Vars{}
-	new.Env.Merge(r.ReplaceVars(e.Taskfile.Env))
-	new.Env.Merge(r.ReplaceVars(dotenvEnvs))
-	new.Env.Merge(r.ReplaceVars(origTask.Env))
+	new.Env.Merge(templater.ReplaceVars(e.Taskfile.Env, cache))
+	new.Env.Merge(templater.ReplaceVars(dotenvEnvs, cache))
+	new.Env.Merge(templater.ReplaceVars(origTask.Env, cache))
 	if evaluateShVars {
 		err = new.Env.Range(func(k string, v ast.Var) error {
 			// If the variable is not dynamic, we can set it and return
 			if v.Value != nil || v.Sh == "" {
 				new.Env.Set(k, ast.Var{Value: v.Value})
 				return nil
 			}
@@ -129,64 +129,17 @@
 	if len(origTask.Cmds) > 0 {
 		new.Cmds = make([]*ast.Cmd, 0, len(origTask.Cmds))
 		for _, cmd := range origTask.Cmds {
 			if cmd == nil {
 				continue
 			}
 			if cmd.For != nil {
-				var keys []string
-				var list []any
-				// Get the list from the explicit for list
-				if cmd.For.List != nil && len(cmd.For.List) > 0 {
-					list = cmd.For.List
-				}
-				// Get the list from the task sources
-				if cmd.For.From == "sources" {
-					glist, err := fingerprint.Globs(new.Dir, new.Sources)
-					if err != nil {
-						return nil, err
-					}
-					// Make the paths relative to the task dir
-					for i, v := range glist {
-						if glist[i], err = filepath.Rel(new.Dir, v); err != nil {
-							return nil, err
-						}
-					}
-					list = asAnySlice(glist)
-				}
-				// Get the list from a variable and split it up
-				if cmd.For.Var != "" {
-					if vars != nil {
-						v := vars.Get(cmd.For.Var)
-						// If the variable is dynamic, then it hasn't been resolved yet
-						// and we can't use it as a list. This happens when fast compiling a task
-						// for use in --list or --list-all etc.
-						if v.Value != nil && v.Sh == "" {
-							switch value := v.Value.(type) {
-							case string:
-								if cmd.For.Split != "" {
-									list = asAnySlice(strings.Split(value, cmd.For.Split))
-								} else {
-									list = asAnySlice(strings.Fields(value))
-								}
-							case []any:
-								list = value
-							case map[string]any:
-								for k, v := range value {
-									keys = append(keys, k)
-									list = append(list, v)
-								}
-							default:
-								return nil, errors.TaskfileInvalidError{
-									URI: origTask.Location.Taskfile,
-									Err: errors.New("var must be a delimiter-separated string or a list"),
-								}
-							}
-						}
-					}
+				list, keys, err := itemsFromFor(cmd.For, new.Dir, new.Sources, vars, origTask.Location)
+				if err != nil {
+					return nil, err
 				}
 				// Name the iterator variable
 				var as string
 				if cmd.For.As != "" {
 					as = cmd.For.As
 				} else {
 					as = "ITEM"
@@ -196,25 +149,25 @@
 					extra := map[string]any{
 						as: loopValue,
 					}
 					if len(keys) > 0 {
 						extra["KEY"] = keys[i]
 					}
 					newCmd := cmd.DeepCopy()
-					newCmd.Cmd = r.ReplaceWithExtra(cmd.Cmd, extra)
-					newCmd.Task = r.ReplaceWithExtra(cmd.Task, extra)
-					newCmd.Vars = r.ReplaceVarsWithExtra(cmd.Vars, extra)
+					newCmd.Cmd = templater.ReplaceWithExtra(cmd.Cmd, cache, extra)
+					newCmd.Task = templater.ReplaceWithExtra(cmd.Task, cache, extra)
+					newCmd.Vars = templater.ReplaceVarsWithExtra(cmd.Vars, cache, extra)
 					new.Cmds = append(new.Cmds, newCmd)
 				}
 				continue
 			}
 			newCmd := cmd.DeepCopy()
-			newCmd.Cmd = r.Replace(cmd.Cmd)
-			newCmd.Task = r.Replace(cmd.Task)
-			newCmd.Vars = r.ReplaceVars(cmd.Vars)
+			newCmd.Cmd = templater.Replace(cmd.Cmd, cache)
+			newCmd.Task = templater.Replace(cmd.Task, cache)
+			newCmd.Vars = templater.ReplaceVars(cmd.Vars, cache)
 			// Loop over the command's variables and resolve any references to other variables
 			err := cmd.Vars.Range(func(k string, v ast.Var) error {
 				if v.Ref != "" {
 					refVal := vars.Get(v.Ref)
 					newCmd.Vars.Set(k, refVal)
 				}
 				return nil
@@ -227,17 +180,44 @@
 	}
 	if len(origTask.Deps) > 0 {
 		new.Deps = make([]*ast.Dep, 0, len(origTask.Deps))
 		for _, dep := range origTask.Deps {
 			if dep == nil {
 				continue
 			}
+			if dep.For != nil {
+				list, keys, err := itemsFromFor(dep.For, new.Dir, new.Sources, vars, origTask.Location)
+				if err != nil {
+					return nil, err
+				}
+				// Name the iterator variable
+				var as string
+				if dep.For.As != "" {
+					as = dep.For.As
+				} else {
+					as = "ITEM"
+				}
+				// Create a new command for each item in the list
+				for i, loopValue := range list {
+					extra := map[string]any{
+						as: loopValue,
+					}
+					if len(keys) > 0 {
+						extra["KEY"] = keys[i]
+					}
+					newDep := dep.DeepCopy()
+					newDep.Task = templater.ReplaceWithExtra(dep.Task, cache, extra)
+					newDep.Vars = templater.ReplaceVarsWithExtra(dep.Vars, cache, extra)
+					new.Deps = append(new.Deps, newDep)
+				}
+				continue
+			}
 			newDep := dep.DeepCopy()
-			newDep.Task = r.Replace(dep.Task)
-			newDep.Vars = r.ReplaceVars(dep.Vars)
+			newDep.Task = templater.Replace(dep.Task, cache)
+			newDep.Vars = templater.ReplaceVars(dep.Vars, cache)
 			// Loop over the dep's variables and resolve any references to other variables
 			err := dep.Vars.Range(func(k string, v ast.Var) error {
 				if v.Ref != "" {
 					refVal := vars.Get(v.Ref)
 					newDep.Vars.Set(k, refVal)
 				}
 				return nil
@@ -252,16 +232,16 @@
 	if len(origTask.Preconditions) > 0 {
 		new.Preconditions = make([]*ast.Precondition, 0, len(origTask.Preconditions))
 		for _, precondition := range origTask.Preconditions {
 			if precondition == nil {
 				continue
 			}
 			newPrecondition := precondition.DeepCopy()
-			newPrecondition.Sh = r.Replace(precondition.Sh)
-			newPrecondition.Msg = r.Replace(precondition.Msg)
+			newPrecondition.Sh = templater.Replace(precondition.Sh, cache)
+			newPrecondition.Msg = templater.Replace(precondition.Msg, cache)
 			new.Preconditions = append(new.Preconditions, newPrecondition)
 		}
 	}
 
 	if len(origTask.Status) > 0 {
 		timestampChecker := fingerprint.NewTimestampChecker(e.TempDir, e.Dry)
 		checksumChecker := fingerprint.NewChecksumChecker(e.TempDir, e.Dry)
@@ -272,27 +252,88 @@
 				return nil, err
 			}
 			vars.Set(strings.ToUpper(checker.Kind()), ast.Var{Live: value})
 		}
 
 		// Adding new variables, requires us to refresh the templaters
 		// cache of the the values manually
-		r.ResetCache()
+		cache.ResetCache()
 
-		new.Status = r.ReplaceSlice(origTask.Status)
+		new.Status = templater.Replace(origTask.Status, cache)
 	}
 
 	// We only care about templater errors if we are evaluating shell variables
-	if evaluateShVars && r.Err() != nil {
-		return &new, r.Err()
+	if evaluateShVars && cache.Err() != nil {
+		return &new, cache.Err()
 	}
 
 	return &new, nil
 }
 
 func asAnySlice[T any](slice []T) []any {
 	ret := make([]any, len(slice))
 	for i, v := range slice {
 		ret[i] = v
 	}
 	return ret
 }
+
+func itemsFromFor(
+	f *ast.For,
+	dir string,
+	sources []*ast.Glob,
+	vars *ast.Vars,
+	location *ast.Location,
+) ([]any, []string, error) {
+	var keys []string // The list of keys to loop over (only if looping over a map)
+	var values []any  // The list of values to loop over
+	// Get the list from the explicit for list
+	if f.List != nil && len(f.List) > 0 {
+		values = f.List
+	}
+	// Get the list from the task sources
+	if f.From == "sources" {
+		glist, err := fingerprint.Globs(dir, sources)
+		if err != nil {
+			return nil, nil, err
+		}
+		// Make the paths relative to the task dir
+		for i, v := range glist {
+			if glist[i], err = filepath.Rel(dir, v); err != nil {
+				return nil, nil, err
+			}
+		}
+		values = asAnySlice(glist)
+	}
+	// Get the list from a variable and split it up
+	if f.Var != "" {
+		if vars != nil {
+			v := vars.Get(f.Var)
+			// If the variable is dynamic, then it hasn't been resolved yet
+			// and we can't use it as a list. This happens when fast compiling a task
+			// for use in --list or --list-all etc.
+			if v.Value != nil && v.Sh == "" {
+				switch value := v.Value.(type) {
+				case string:
+					if f.Split != "" {
+						values = asAnySlice(strings.Split(value, f.Split))
+					} else {
+						values = asAnySlice(strings.Fields(value))
+					}
+				case []any:
+					values = value
+				case map[string]any:
+					for k, v := range value {
+						keys = append(keys, k)
+						values = append(values, v)
+					}
+				default:
+					return nil, nil, errors.TaskfileInvalidError{
+						URI: location.Taskfile,
+						Err: errors.New("loop var must be a delimiter-separated string, list or a map"),
+					}
+				}
+			}
+		}
+	}
+	return values, keys, nil
+}
```

### Comparing `go_task_bin-3.35.1/task/watch.go` & `go_task_bin-3.36.0/task/watch.go`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 				return fmt.Errorf("task: %s: %w", s, err)
 			}
 			for _, f := range files {
 				absFile, err := filepath.Abs(f)
 				if err != nil {
 					return err
 				}
-				if shouldIgnoreFile(absFile) {
+				if ShouldIgnoreFile(absFile) {
 					continue
 				}
 				if _, ok := watchedFiles[absFile]; ok {
 					continue
 				}
 				if err := w.Add(absFile); err != nil {
 					return err
@@ -176,15 +176,15 @@
 		if err := registerTaskFiles(c); err != nil {
 			return err
 		}
 	}
 	return nil
 }
 
-func shouldIgnoreFile(path string) bool {
+func ShouldIgnoreFile(path string) bool {
 	ignorePaths := []string{
 		"/.task",
 		"/.git",
 		"/.hg",
 		"/node_modules",
 	}
 	for _, p := range ignorePaths {
```

### Comparing `go_task_bin-3.35.1/task/watch_test.go` & `go_task_bin-3.36.0/task/watch_test.go`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 	go func(ctx context.Context) {
 		for {
 			select {
 			case <-ctx.Done():
 				return
 			default:
-				err := e.Run(ctx, ast.Task: "default"})
+				err := e.Run(ctx, &ast.Call{Task: "default"})
 				if err != nil {
 					return
 				}
 			}
 		}
 	}(ctx)
 
@@ -90,11 +90,11 @@
 		{"/.github/workflows/build.yaml", false},
 	}
 
 	for k, ct := range tt {
 		ct := ct
 		t.Run(fmt.Sprintf("ignore - %d", k), func(t *testing.T) {
 			t.Parallel()
-			require.Equal(t, shouldIgnoreFile(ct.path), ct.expect)
+			require.Equal(t, task.ShouldIgnoreFile(ct.path), ct.expect)
 		})
 	}
 }
```

### Comparing `go_task_bin-3.35.1/PKG-INFO` & `go_task_bin-3.36.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: go-task-bin
-Version: 3.35.1
+Version: 3.36.0
 Summary: task - A task runner / simpler Make alternative written in Go
-Keywords: build build-tool devops go make makefile runner task task-runner taskfile tool
+Keywords: build,build-tool,devops,go,make,makefile,runner,task,task-runner,taskfile,tool
 Author-Email: dowon <ks2515@naver.com>
 License: MIT
 Classifier: Programming Language :: Other
 Classifier: Topic :: Software Development :: Build Tools
 Project-URL: Repository, https://github.com/Bing-su/pip-binary-factory
+Project-URL: Taskfile, https://taskfile.dev
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # go-task-bin
 
 https://github.com/go-task/task
```

