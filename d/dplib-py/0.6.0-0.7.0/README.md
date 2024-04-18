# Comparing `tmp/dplib_py-0.6.0.tar.gz` & `tmp/dplib_py-0.7.0.tar.gz`

## Comparing `dplib_py-0.6.0.tar` & `dplib_py-0.7.0.tar`

### file list

```diff
@@ -1,244 +1,267 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/.env.example
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 dplib_py-0.6.0/mkdocs.yaml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dplib_py-0.6.0/.github/codecov.yaml
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.6.0/.github/issue_template.md
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.6.0/.github/pull_request_template.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.6.0/.github/stale.yaml
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 dplib_py-0.6.0/.github/workflows/general.yaml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/dialect-full.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/dialect-invalid.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/dialect.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/empty.json
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/package-custom-profile.json
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/package-full.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/package-invalid-dereferencing.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/package-invalid.json
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/profile.json
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/resource-full.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/resource-invalid-dereferencing.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/resource-invalid.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/resource.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/resource.yaml
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/schema-full.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/schema-invalid.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/schema-types.json
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/schema.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/text.txt
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/cassettes/test_check_package_custom_profile.yaml
--rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/cassettes/test_dialect_profile.yaml
--rw-r--r--   0        0        0    60589 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/cassettes/test_package_profile.yaml
--rw-r--r--   0        0        0   220871 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/cassettes/test_resource_profile.yaml
--rw-r--r--   0        0        0   169730 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/cassettes/test_schema_profile.yaml
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/plugins/ckan/package.json
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/plugins/datacite/package.json
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/plugins/dcat/package.xml
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/plugins/github/package.json
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 dplib_py-0.6.0/data/plugins/zenodo/package.json
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/contributing.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/converting-metadata.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/index.md
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/installation.md
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/validating-metadata.md
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/working-with-models.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/.theme/.keep
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/actions/dialect.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/actions/package.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/actions/resource.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/actions/schema.md
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/assets/favicon-color.png
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/assets/favicon-shaddow.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/assets/favicon.ico
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/assets/favicon.png
--rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/assets/logo-dark.svg
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/assets/logo-light.svg
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/models/dialect.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/models/package.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/models/resource.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/models/schema.md
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/plugins/ckan.md
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/plugins/cli.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/plugins/datacite.md
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/plugins/dcat.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/plugins/github.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/plugins/pandas.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/plugins/polars.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/plugins/sql.md
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dplib_py-0.6.0/docs/plugins/zenodo.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/conftest.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/error.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/py.typed
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/settings.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/__spec__/__init__.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/__spec__/test_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/dialect/__init__.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/dialect/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/dialect/__spec__/__init__.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/dialect/__spec__/test_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/metadata/__init__.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/metadata/check.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/metadata/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/package/__init__.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/package/check.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/package/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/package/__spec__/__init__.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/package/__spec__/test_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/resource/__init__.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/resource/check.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/resource/convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/resource/__spec__/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/resource/__spec__/test_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/schema/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/schema/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/schema/__spec__/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/actions/schema/__spec__/test_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/errors/__init__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/errors/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/helpers/__init__.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/helpers/data.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/helpers/file.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/helpers/path.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/helpers/profile.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/helpers/resource.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/contributor.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/license.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/source.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/dialect/__init__.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/dialect/dialect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/dialect/__spec__/__init__.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/dialect/__spec__/test_dialect.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/package/__init__.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/package/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/package/__spec__/__init__.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/package/__spec__/test_package.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/profile/__init__.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/profile/profile.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/profile/rule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/profile/__spec__/__init__.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/profile/__spec__/test_profile.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/resource/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/resource/hash.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/resource/resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/resource/__spec__/__init__.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/resource/__spec__/test_resource.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/schema/__init__.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/schema/constraints.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/schema/field.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/schema/fieldType.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/schema/foreignKey.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/schema/foreignKeyReference.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/schema/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/schema/__spec__/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/schema/__spec__/test_field.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/models/schema/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/ckan/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/ckan/models/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/ckan/models/organization.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/ckan/models/package.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/ckan/models/resource.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/ckan/models/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/ckan/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/ckan/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/__main__.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/program.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/main.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/__spec__/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/__spec__/test_version.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/dialect/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/dialect/check.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/dialect/main.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/package/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/package/check.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/package/convert.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/package/main.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/resource/__init__.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/resource/check.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/resource/convert.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/resource/main.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/schema/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/schema/check.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/commands/schema/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/helpers/__init__.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/helpers/check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/options/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/options/convert.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/options/path.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/cli/options/system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/models/__init__.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/models/contributor.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/models/description.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/models/identifier.py
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/models/package.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/models/rights.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/models/subject.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/models/title.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/models/__spec__/__init__.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/datacite/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/models/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/models/dumpers.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/models/helpers.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/models/loaders.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/models/namespaces.py
--rw-r--r--   0        0        0    11120 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/models/package.py
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/models/resource.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/models/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/dcat/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/github/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/github/models/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/github/models/license.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/github/models/owner.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/github/models/package.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/github/models/resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/github/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/github/models/__spec__/test_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/pandas/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/pandas/models/__init__.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/pandas/models/field.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/pandas/models/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/pandas/models/__spec__/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/polars/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/polars/models/__init__.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/polars/models/field.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/polars/models/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/polars/models/__spec__/__init__.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/polars/models/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/sql/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/sql/models/__init__.py
--rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/sql/models/field.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/sql/models/schema.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/sql/models/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/sql/models/__spec__/__init__.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/sql/models/__spec__/test_schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/models/__init__.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/models/creator.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/models/files.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/models/metadata.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/models/package.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/models/pid.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/models/resource.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/models/subject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/models/__spec__/__init__.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/plugins/zenodo/models/__spec__/test_package.py
--rw-r--r--   0        0        0   107400 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/profiles/data-package.json
--rw-r--r--   0        0        0    85144 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/profiles/data-resource.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/profiles/metadata-profile.json
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/profiles/table-dialect.json
--rw-r--r--   0        0        0    68276 2020-02-02 00:00:00.000000 dplib_py-0.6.0/dplib/profiles/table-schema.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 dplib_py-0.6.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 dplib_py-0.6.0/LICENSE.md
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 dplib_py-0.6.0/README.md
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 dplib_py-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 dplib_py-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.env.example
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 dplib_py-0.7.0/mkdocs.yaml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.github/codecov.yaml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.github/issue_template.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.github/stale.yaml
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.github/workflows/general.yaml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/dialect-full.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/dialect-invalid.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/dialect.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/empty.json
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/package-custom-profile.json
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/package-full.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/package-invalid-dereferencing.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/package-invalid.json
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/profile.json
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/resource-full.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/resource-invalid-dereferencing.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/resource-invalid.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/resource.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/resource.yaml
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/schema-full.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/schema-invalid.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/schema-types.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/schema.json
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/text.txt
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/cassettes/test_check_package_custom_profile.yaml
+-rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/cassettes/test_dialect_profile.yaml
+-rw-r--r--   0        0        0    60589 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/cassettes/test_package_profile.yaml
+-rw-r--r--   0        0        0   220871 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/cassettes/test_resource_profile.yaml
+-rw-r--r--   0        0        0   169730 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/cassettes/test_schema_profile.yaml
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/plugins/ckan/package.json
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/plugins/datacite/package.json
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/plugins/dcat/package.xml
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/plugins/github/package.json
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 dplib_py-0.7.0/data/plugins/zenodo/package.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/changelog.md
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/contributing.md
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/converting-metadata.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/index.md
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/installation.md
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/validating-metadata.md
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/working-with-models.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/.theme/.keep
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/actions/dialect.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/actions/package.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/actions/resource.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/actions/schema.md
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/favicon-color.png
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/favicon-shaddow.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/favicon.ico
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/favicon.png
+-rw-r--r--   0        0        0     8911 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/logo-dark.svg
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/assets/logo-light.svg
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/models/dialect.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/models/package.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/models/resource.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/models/schema.md
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/ckan.md
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/cli.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/datacite.md
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/dcat.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/github.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/pandas.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/polars.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/sql.md
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 dplib_py-0.7.0/docs/plugins/zenodo.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/conftest.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/py.typed
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/settings.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/__spec__/test_dialect_check.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/__spec__/test_package_check.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/__spec__/test_resource_check.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/__spec__/test_schema_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/dialect/__init__.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/dialect/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/metadata/__init__.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/metadata/check.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/metadata/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/package/__init__.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/package/check.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/package/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/resource/__init__.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/resource/check.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/resource/convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/schema/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/actions/schema/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/errors/__init__.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/errors/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/data.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/file.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/path.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/profile.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/helpers/resource.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/__init__.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/contributor.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/license.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/source.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/dialect/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/dialect/dialect.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/dialect/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/dialect/__spec__/__init__.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/dialect/__spec__/test_dialect.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/field.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/types.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/__spec__/test_field.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/base.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/collection.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/json.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/string.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/constraints/value.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/any.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/array.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/base.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/boolean.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/date.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/datetime.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/duration.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/geojson.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/geopoint.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/integer.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/list.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/number.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/object.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/string.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/time.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/year.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/field/datatypes/yearmonth.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/package/__init__.py
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/package/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/package/__spec__/__init__.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/package/__spec__/test_package.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/__init__.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/hash.py
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/__spec__/__init__.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/__spec__/test_resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/datatypes/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/resource/datatypes/table.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/foreignKey.py
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/schema.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/__spec__/__init__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/models/schema/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/organization.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/package.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/resource.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/ckan/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/__main__.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/program.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/main.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/__spec__/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/__spec__/test_version.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/dialect/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/dialect/check.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/dialect/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/package/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/package/check.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/package/convert.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/package/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/resource/__init__.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/resource/check.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/resource/convert.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/resource/main.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/schema/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/schema/check.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/commands/schema/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/helpers/__init__.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/helpers/check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/options/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/options/convert.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/options/path.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/cli/options/system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/contributor.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/description.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/identifier.py
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/package.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/rights.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/subject.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/title.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/datacite/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/dumpers.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/helpers.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/loaders.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/namespaces.py
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/package.py
+-rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/resource.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/dcat/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/license.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/owner.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/package.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/github/models/__spec__/test_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/pandas/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/pandas/models/__init__.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/pandas/models/field.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/pandas/models/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/pandas/models/__spec__/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/models/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/models/field.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/models/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/polars/models/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/__init__.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/field.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/schema.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/sql/models/__spec__/test_schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/__init__.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/creator.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/files.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/metadata.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/package.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/pid.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/resource.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/subject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/__spec__/__init__.py
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/plugins/zenodo/models/__spec__/test_package.py
+-rw-r--r--   0        0        0   107095 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/1.0/datapackage.json
+-rw-r--r--   0        0        0    85332 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/1.0/dataresource.json
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/1.0/tabledialect.json
+-rw-r--r--   0        0        0    65533 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/1.0/tableschema.json
+-rw-r--r--   0        0        0   142568 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/2.0/datapackage.json
+-rw-r--r--   0        0        0   117144 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/2.0/dataresource.json
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/2.0/tabledialect.json
+-rw-r--r--   0        0        0    94827 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/profiles/2.0/tableschema.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/system/__init__.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/system/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/system/__spec__/__init__.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 dplib_py-0.7.0/dplib/system/__spec__/test_model.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 dplib_py-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 dplib_py-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 dplib_py-0.7.0/README.md
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 dplib_py-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 dplib_py-0.7.0/PKG-INFO
```

### Comparing `dplib_py-0.6.0/mkdocs.yaml` & `dplib_py-0.7.0/mkdocs.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -117,14 +117,15 @@
   - Home:
       - Welcome: index.md
       - Installation: installation.md
       - Working with Models: working-with-models.md
       - Validating Metadata: validating-metadata.md
       - Converting Metadata: converting-metadata.md
       - Contributing: contributing.md
+      - Changelog: changelog.md
   - Models:
       - Package: models/package.md
       - Resource: models/resource.md
       - Dialect: models/dialect.md
       - Schema: models/schema.md
   - Actions:
       - Package: actions/package.md
```

#### html2text {}

```diff
@@ -27,15 +27,15 @@
 pymdownx.inlinehilite - pymdownx.snippets - pymdownx.superfences -
 pymdownx.extra - pymdownx.emoji: emoji_index: !!python/name:
 material.extensions.emoji.twemoji emoji_generator: !!python/name:
 materialx.emoji.to_svg - pymdownx.tabbed: alternate_style: true -
 pymdownx.snippets: check_paths: true # Navigation nav: - Home: - Welcome:
 index.md - Installation: installation.md - Working with Models: working-with-
 models.md - Validating Metadata: validating-metadata.md - Converting Metadata:
-converting-metadata.md - Contributing: contributing.md - Models: - Package:
-models/package.md - Resource: models/resource.md - Dialect: models/dialect.md -
-Schema: models/schema.md - Actions: - Package: actions/package.md - Resource:
-actions/resource.md - Dialect: actions/dialect.md - Schema: actions/schema.md -
-Plugins: - CKAN: plugins/ckan.md - CLI: plugins/cli.md - DataCite: plugins/
-datacite.md - DCAT: plugins/dcat.md - GitHub: plugins/github.md - Pandas:
-plugins/pandas.md - Polars: plugins/polars.md - SQL: plugins/sql.md - Zenodo:
-plugins/zenodo.md
+converting-metadata.md - Contributing: contributing.md - Changelog:
+changelog.md - Models: - Package: models/package.md - Resource: models/
+resource.md - Dialect: models/dialect.md - Schema: models/schema.md - Actions:
+- Package: actions/package.md - Resource: actions/resource.md - Dialect:
+actions/dialect.md - Schema: actions/schema.md - Plugins: - CKAN: plugins/
+ckan.md - CLI: plugins/cli.md - DataCite: plugins/datacite.md - DCAT: plugins/
+dcat.md - GitHub: plugins/github.md - Pandas: plugins/pandas.md - Polars:
+plugins/polars.md - SQL: plugins/sql.md - Zenodo: plugins/zenodo.md
```

### Comparing `dplib_py-0.6.0/.github/stale.yaml` & `dplib_py-0.7.0/.github/stale.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/.github/workflows/general.yaml` & `dplib_py-0.7.0/.github/workflows/general.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,28 +16,28 @@
   # Test (Linux)
 
   test-linux:
     if: github.event_name != 'schedule' || github.repository_owner == 'frictionlessdata'
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.9, "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: Checkout repository
         uses: actions/checkout@v2
       - name: Install Python
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
       - name: Prepare environment
         run: pip3 install hatch
       - name: Prepare variables
         run: cp .env.example .env
       - name: Test software
-        run: hatch run ci:test +py=${{ matrix.py || matrix.python-version }}
+        run: hatch run +py=${{ matrix.py || matrix.python-version }} ci:test
       - name: Report coverage
         uses: codecov/codecov-action@v2
 
   # Test (MacOS)
 
   test-macos:
     if: github.event_name != 'schedule' || github.repository_owner == 'frictionlessdata'
@@ -51,15 +51,15 @@
           python-version: "3.10"
       - name: Prepare environment
         run: pip3 install hatch
       - name: Prepare variables
         run: cp .env.example .env
       - name: Test software
         # https://stackoverflow.com/questions/9678408/cant-install-psycopg2-with-pip-in-virtualenv-on-mac-os-x-10-7
-        run: LDFLAGS=`echo $(pg_config --ldflags)` hatch run ci:test
+        run: LDFLAGS=`echo $(pg_config --ldflags)` hatch run +py=3.10 ci:test
 
   # Test (Windows)
 
   test-windows:
     if: github.event_name != 'schedule' || github.repository_owner == 'frictionlessdata'
     runs-on: windows-latest
     steps:
@@ -70,15 +70,15 @@
         with:
           python-version: "3.10"
       - name: Prepare environment
         run: pip3 install hatch
       - name: Prepare variables
         run: cp .env.example .env
       - name: Test software
-        run: hatch run ci:test
+        run: hatch run +py=3.10 ci:test
 
   # Deploy
 
   deploy:
     if: github.event_name == 'push'
     runs-on: ubuntu-latest
     steps:
@@ -87,15 +87,15 @@
       - name: Install Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.10"
       - name: Prepare environment
         run: pip3 install hatch
       - name: Build docs
-        run: hatch run build
+        run: hatch run docs-build
       - name: Publush to Github Pages
         uses: JamesIves/github-pages-deploy-action@v4
         with:
           branch: site
           folder: site
           clean: true
```

### Comparing `dplib_py-0.6.0/data/package-full.json` & `dplib_py-0.7.0/data/package-full.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/schema-full.json` & `dplib_py-0.7.0/data/schema-full.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/schema-types.json` & `dplib_py-0.7.0/data/schema-types.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/cassettes/test_check_package_custom_profile.yaml` & `dplib_py-0.7.0/data/cassettes/test_check_package_custom_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/cassettes/test_dialect_profile.yaml` & `dplib_py-0.7.0/data/cassettes/test_dialect_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/cassettes/test_package_profile.yaml` & `dplib_py-0.7.0/data/cassettes/test_package_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/cassettes/test_resource_profile.yaml` & `dplib_py-0.7.0/data/cassettes/test_resource_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/cassettes/test_schema_profile.yaml` & `dplib_py-0.7.0/data/cassettes/test_schema_profile.yaml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/plugins/ckan/package.json` & `dplib_py-0.7.0/data/plugins/ckan/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/plugins/datacite/package.json` & `dplib_py-0.7.0/data/plugins/datacite/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/plugins/dcat/package.xml` & `dplib_py-0.7.0/data/plugins/dcat/package.xml`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/plugins/github/package.json` & `dplib_py-0.7.0/data/plugins/github/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/data/plugins/zenodo/package.json` & `dplib_py-0.7.0/data/plugins/zenodo/package.json`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/contributing.md` & `dplib_py-0.7.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/converting-metadata.md` & `dplib_py-0.7.0/docs/converting-metadata.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/index.md` & `dplib_py-0.7.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/validating-metadata.md` & `dplib_py-0.7.0/docs/validating-metadata.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/working-with-models.md` & `dplib_py-0.7.0/docs/working-with-models.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/assets/favicon-shaddow.png` & `dplib_py-0.7.0/docs/assets/favicon-shaddow.png`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/assets/favicon.ico` & `dplib_py-0.7.0/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/assets/logo-dark.svg` & `dplib_py-0.7.0/docs/assets/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/assets/logo-light.svg` & `dplib_py-0.7.0/docs/assets/logo-light.svg`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/models/package.md` & `dplib_py-0.7.0/docs/models/package.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/models/resource.md` & `dplib_py-0.7.0/docs/models/resource.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/plugins/ckan.md` & `dplib_py-0.7.0/docs/plugins/ckan.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/plugins/cli.md` & `dplib_py-0.7.0/docs/plugins/cli.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/plugins/datacite.md` & `dplib_py-0.7.0/docs/plugins/datacite.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/plugins/dcat.md` & `dplib_py-0.7.0/docs/plugins/dcat.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/plugins/github.md` & `dplib_py-0.7.0/docs/plugins/github.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/plugins/pandas.md` & `dplib_py-0.7.0/docs/plugins/pandas.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/plugins/polars.md` & `dplib_py-0.7.0/docs/plugins/polars.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/plugins/sql.md` & `dplib_py-0.7.0/docs/plugins/sql.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/docs/plugins/zenodo.md` & `dplib_py-0.7.0/docs/plugins/zenodo.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/model.py` & `dplib_py-0.7.0/dplib/system/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from __future__ import annotations
 
 import pprint
 import warnings
-from functools import cached_property
 from typing import Optional
 
 from pydantic import BaseModel
 from typing_extensions import Self
 
-from . import types
-from .error import Error
-from .helpers.data import clean_data, dump_data, load_data
-from .helpers.file import read_file, write_file
-from .helpers.path import ensure_basepath, infer_format
+from .. import types
+from ..error import Error
+from ..helpers.data import clean_data, dump_data, load_data
+from ..helpers.file import read_file, write_file
+from ..helpers.path import ensure_basepath, infer_format
 
 
 class Model(BaseModel, extra="allow", validate_assignment=True):
     def __str__(self) -> str:
         return repr(self)
 
     def __repr__(self) -> str:
         return pprint.pformat(self.to_dict(), sort_dicts=False)
 
-    @cached_property
-    def custom(self) -> types.IDict:
+    @property
+    def custom(self) -> types.IData:
         assert self.model_extra is not None
         return self.model_extra
 
     # Converters
 
     def to_path(self, path: str, *, format: Optional[str] = None):
         if not format:
@@ -59,15 +58,15 @@
 
     def to_dict(self):
         data = self.model_dump(mode="json", exclude_none=True, exclude_defaults=True)
         clean_data(data)
         return data
 
     @classmethod
-    def from_dict(cls, data: types.IDict, *, basepath: Optional[str] = None) -> Self:
+    def from_dict(cls, data: types.IData, *, basepath: Optional[str] = None) -> Self:
         if basepath and cls.model_fields.get("basepath"):
             data["basepath"] = basepath
         return cls(**data)
 
 
 # Although pydantic@2 moved all the model methods to the "model_" namespace
 # the "schema" method is still in the root namespace
```

### Comparing `dplib_py-0.6.0/dplib/__spec__/test_model.py` & `dplib_py-0.7.0/dplib/system/__spec__/test_model.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/actions/dialect/check.py` & `dplib_py-0.7.0/dplib/actions/dialect/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ... import types
 from ...errors.metadata import MetadataError
 from ...models import Dialect
 from ..metadata.check import check_metadata
 
 
-def check_dialect(dialect: Union[str, types.IDict, Dialect]) -> List[MetadataError]:
+def check_dialect(dialect: Union[str, types.IData, Dialect]) -> List[MetadataError]:
     """Check the validity of a Table Dialect descriptor
 
     This validates the descriptor against the JSON Schema profiles to ensure
     conformity with Data Package standard and Data Package extensions.
 
     Parameters:
         dialect: The Table Dialect descriptor
```

### Comparing `dplib_py-0.6.0/dplib/actions/metadata/convert.py` & `dplib_py-0.7.0/dplib/actions/metadata/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from importlib import import_module
 from typing import Literal, Optional, Type, Union, cast
 
-from ...model import Model
 from ...models import Package, Resource
+from ...system import Model
 
 
 def convert_metadata(
     path: str,
     *,
     type: IType,
     format: Optional[str] = None,
```

### Comparing `dplib_py-0.6.0/dplib/actions/package/check.py` & `dplib_py-0.7.0/dplib/actions/package/check.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ...errors.metadata import MetadataError
 from ...helpers.data import read_data
 from ...helpers.path import infer_basepath
 from ...models import Package
 from ..metadata.check import check_metadata
 
 
-def check_package(package: Union[str, types.IDict, Package]) -> List[MetadataError]:
+def check_package(package: Union[str, types.IData, Package]) -> List[MetadataError]:
     """Check the validity of a Data Package descriptor
 
     This validates the descriptor against the JSON Schema profiles to ensure
     conformity with Data Package standard and Data Package extensions.
 
     Parameters:
         package: The Data Package descriptor
@@ -26,17 +26,19 @@
     if isinstance(package, str):
         basepath = infer_basepath(package)
         package = read_data(package)
     if isinstance(package, Package):
         basepath = package.basepath
         package = package.to_dict()
 
-    # Dereference resources[].dialect/schema
+    # Validate (including nested descriptors)
+    errors = check_metadata(package, type="package")
     resources = package.get("resources", [])
     if isinstance(resources, list):
         for resource in resources:  # type: ignore
-            for name in ["dialect", "schema"]:
-                value = resource.get(name)  # type: ignore
-                if value and isinstance(value, str):
-                    resource[name] = read_data(value, basepath=basepath)
+            for type in ["dialect", "schema"]:
+                value = resource.get(type)  # type: ignore
+                if isinstance(value, str):
+                    metadata = read_data(value, basepath=basepath)
+                    errors.extend(check_metadata(metadata, type=type))  # type: ignore
 
-    return check_metadata(package, type="package")
+    return errors
```

### Comparing `dplib_py-0.6.0/dplib/actions/package/convert.py` & `dplib_py-0.7.0/dplib/actions/package/convert.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from ...model import Model
+from ...system import Model
 from ..metadata.convert import INotation, convert_metadata
 
 
 def convert_package(
     path: str,
     *,
     format: Optional[str] = None,
```

### Comparing `dplib_py-0.6.0/dplib/actions/package/__spec__/test_check.py` & `dplib_py-0.7.0/dplib/actions/__spec__/test_package_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import pytest
 
 from dplib.actions.package.check import check_package
 from dplib.models import Package
 
+# TODO: move to corresponding action folder
+# For some reason pytest colelction failed if we used folders in Python3.11/12
+
 
 def test_check_package():
     errors = check_package("data/package.json")
     assert len(errors) == 0
 
 
 def test_check_package_invalid():
@@ -19,17 +22,16 @@
     assert error.full_message == "[/name] 1 is not of type 'string'"
 
 
 def test_check_package_invalid_dereferencing():
     errors = check_package("data/package-invalid-dereferencing.json")
     assert len(errors) == 1
     error = errors[0]
-    assert (
-        error.full_message == "[/resources/0/dialect/delimiter] 1 is not of type 'string'"
-    )
+    # TODO: extend error path so it shows the full path from the package root
+    assert error.full_message == "[/delimiter] 1 is not of type 'string'"
 
 
 @pytest.mark.vcr
 def test_check_package_custom_profile():
     errors = check_package("data/package-custom-profile.json")
     assert len(errors) == 1
     error = errors[0]
```

### Comparing `dplib_py-0.6.0/dplib/actions/resource/check.py` & `dplib_py-0.7.0/dplib/actions/resource/check.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ...errors.metadata import MetadataError
 from ...helpers.data import read_data
 from ...helpers.path import infer_basepath
 from ...models import Resource
 from ..metadata.check import check_metadata
 
 
-def check_resource(resource: Union[str, types.IDict, Resource]) -> List[MetadataError]:
+def check_resource(resource: Union[str, types.IData, Resource]) -> List[MetadataError]:
     """Check the validity of a Data Resource descriptor
 
     This validates the descriptor against the JSON Schema profiles to ensure
     conformity with Data Package standard and Data Package extensions.
 
     Parameters:
         resource: The Data Resource descriptor
@@ -26,14 +26,16 @@
     if isinstance(resource, str):
         basepath = infer_basepath(resource)
         resource = read_data(resource)
     if isinstance(resource, Resource):
         basepath = resource.basepath
         resource = resource.to_dict()
 
-    # Dereference dialect/schema
-    for name in ["dialect", "schema"]:
-        value = resource.get(name)
-        if value and isinstance(value, str):
-            resource[name] = read_data(value, basepath=basepath)
+    # Validate (including nested descriptors)
+    errors = check_metadata(resource, type="resource")
+    for type in ["dialect", "schema"]:
+        value = resource.get(type)
+        if isinstance(value, str):
+            metadata = read_data(value, basepath=basepath)
+            errors.extend(check_metadata(metadata, type=type))  # type: ignore
 
-    return check_metadata(resource, type="resource")
+    return errors
```

### Comparing `dplib_py-0.6.0/dplib/actions/resource/convert.py` & `dplib_py-0.7.0/dplib/actions/resource/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from ...model import Model
+from ...system import Model
 from ..metadata.convert import INotation, convert_metadata
 
 
 def convert_resource(
     path: str,
     *,
     format: Optional[str] = None,
```

### Comparing `dplib_py-0.6.0/dplib/actions/resource/__spec__/test_check.py` & `dplib_py-0.7.0/dplib/actions/__spec__/test_resource_check.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from dplib.actions.resource.check import check_resource
 from dplib.models import Resource
 
+# TODO: move to corresponding action folder
+# For some reason pytest colelction failed if we used folders in Python3.11/12
+
 
 def test_check_resource():
     errors = check_resource("data/resource.json")
     assert len(errors) == 0
 
 
 def test_check_resource_invalid():
@@ -17,14 +20,15 @@
     assert error.full_message == "[/name] 1 is not of type 'string'"
 
 
 def test_check_resource_invalid_dereferencing():
     errors = check_resource("data/resource-invalid-dereferencing.json")
     assert len(errors) == 1
     error = errors[0]
-    assert error.full_message == "[/dialect/delimiter] 1 is not of type 'string'"
+    # TODO: extend error path so it shows the full path from the resource root
+    assert error.full_message == "[/delimiter] 1 is not of type 'string'"
 
 
 def test_check_resource_from_model():
     resource = Resource(name="name", path="path")
     errors = check_resource(resource)
     assert len(errors) == 0
```

### Comparing `dplib_py-0.6.0/dplib/actions/schema/check.py` & `dplib_py-0.7.0/dplib/actions/schema/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ... import types
 from ...errors.metadata import MetadataError
 from ...models import Schema
 from ..metadata.check import check_metadata
 
 
-def check_schema(schema: Union[str, types.IDict, Schema]) -> List[MetadataError]:
+def check_schema(schema: Union[str, types.IData, Schema]) -> List[MetadataError]:
     """Check the validity of a Table Schema descriptor
 
     This validates the descriptor against the JSON Schema profiles to ensure
     conformity with Data Package standard and Data Package extensions.
 
     Parameters:
         schema: The Table Schema descriptor
```

### Comparing `dplib_py-0.6.0/dplib/actions/schema/__spec__/test_check.py` & `dplib_py-0.7.0/dplib/actions/__spec__/test_schema_check.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from dplib.actions.schema.check import check_schema
 from dplib.models import Schema
 
+# TODO: move to corresponding action folder
+# For some reason pytest colelction failed if we used folders in Python3.11/12
+
 
 def test_check_schema():
     errors = check_schema("data/schema.json")
     assert len(errors) == 0
 
 
 def test_check_schema_invalid():
```

### Comparing `dplib_py-0.6.0/dplib/errors/metadata.py` & `dplib_py-0.7.0/dplib/errors/metadata.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/helpers/data.py` & `dplib_py-0.7.0/dplib/helpers/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,54 +8,54 @@
 from ..error import Error
 from .file import read_file, write_file
 from .path import infer_format
 
 
 def read_data(
     path: str, *, format: Optional[str] = None, basepath: Optional[str] = None
-) -> types.IDict:
+) -> types.IData:
     if not format:
         format = infer_format(path, raise_missing=True)
     text = read_file(path, basepath=basepath)
     data = load_data(text, format=format)
     return data
 
 
-def write_data(path: str, data: types.IDict, *, format: Optional[str] = None):
+def write_data(path: str, data: types.IData, *, format: Optional[str] = None):
     if not format:
         format = infer_format(path, raise_missing=True)
     text = dump_data(data, format=format)
     write_file(path, text)
 
 
-def load_data(text: str, *, format: str) -> types.IDict:
+def load_data(text: str, *, format: str) -> types.IData:
     try:
         if format == "json":
             return json.loads(text)
         elif format == "yaml":
             yaml = import_module("yaml")
             return yaml.safe_load(text)
     except Exception:
         raise Error(f'Cannot load "{format}" data from text: {text}')
     raise Error(f"Cannot load data from text with format: {format}")
 
 
-def dump_data(data: types.IDict, *, format: str) -> str:
+def dump_data(data: types.IData, *, format: str) -> str:
     try:
         if format == "json":
             return json.dumps(data, indent=2)
         elif format == "yaml":
             yaml = import_module("yaml")
             return yaml.dump(data)
     except Exception:
         raise Error(f'Cannot dump "{format}" text from data: {data}')
     raise Error(f"Cannot dump data to text with format: {format}")
 
 
-def clean_data(data: types.IDict):
+def clean_data(data: types.IData):
     for key, value in list(data.items()):
         if isinstance(value, dict):
             clean_data(value)  # type: ignore
         elif isinstance(value, list):
             for item in value:  # type: ignore
                 if isinstance(item, dict):
                     clean_data(item)  # type: ignore
```

### Comparing `dplib_py-0.6.0/dplib/helpers/file.py` & `dplib_py-0.7.0/dplib/helpers/file.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/helpers/path.py` & `dplib_py-0.7.0/dplib/helpers/path.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/models/dialect/__spec__/test_dialect.py` & `dplib_py-0.7.0/dplib/models/dialect/__spec__/test_dialect.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from dplib.models import Dialect
 
 
 def test_dialect_from_path():
     dialect = Dialect.from_path("data/dialect.json")
     assert dialect.delimiter == ";"
-    assert dialect.get_delimiter() == ";"
 
 
 def test_dialect_from_path_full():
     dialect = Dialect.from_path("data/dialect-full.json")
     assert dialect.delimiter == ";"
     assert dialect.lineTerminator == "\r\n"
     assert dialect.quoteChar == "'"
@@ -21,19 +20,21 @@
     assert dialect.skipInitialSpace is True
     assert dialect.header is False
     assert dialect.commentChar == "#"
 
 
 def test_dialect_defaults():
     dialect = Dialect()
-    assert dialect.get_delimiter() == ","
-    assert dialect.get_line_terminator() == "\r\n"
-    assert dialect.get_quote_char() == '"'
-    assert dialect.get_double_quote() is True
-    assert dialect.get_header() is True
+    assert dialect.header is True
+    assert dialect.headerJoin == " "
+    assert dialect.delimiter == ","
+    assert dialect.lineTerminator == "\r\n"
+    assert dialect.quoteChar == '"'
+    assert dialect.doubleQuote is True
+    assert dialect.sheetNumber == 1
 
 
 def test_dialect_from_text():
     text = '{"delimiter": ";"}'
     dialect = Dialect.from_text(text, format="json")
     assert dialect.delimiter == ";"
 
@@ -50,15 +51,7 @@
         Dialect.from_dict(data)
 
 
 def test_dialect_set_proprty_invalid():
     dialect = Dialect()
     with pytest.raises(ValidationError):
         dialect.delimiter = 1  # type: ignore
-
-
-@pytest.mark.vcr
-def test_dialect_profile():
-    dialect = Dialect.from_path("data/dialect-full.json")
-    profile = dialect.get_profile()
-    assert profile
-    assert profile.jsonSchema.get("title") == "CSV Dialect"
```

### Comparing `dplib_py-0.6.0/dplib/models/package/package.py` & `dplib_py-0.7.0/dplib/models/package/package.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 import pydantic
 
-from ...model import Model
+from ... import settings
+from ...system import Model
 from ..contributor import Contributor
 from ..license import License
-from ..profile import Profile
 from ..resource import Resource
 from ..source import Source
 
 
 class Package(Model):
     """Data Package model"""
 
+    profile: str = pydantic.Field(
+        default=settings.PROFILE_CURRENT_PACKAGE,
+        alias="$schema",
+    )
+    """A profile URL"""
+
     basepath: Optional[str] = pydantic.Field(default=None, exclude=True)
     """
     Basepath of the package.
     All the resources are relative to this path.
     """
 
     resources: List[Resource] = []
@@ -35,19 +41,14 @@
     name: Optional[str] = None
     """
     A short url-usable (and preferably human-readable) name of the package.
     This MUST be lower-case and contain only alphanumeric characters
     along with ”.”, ”_” or ”-” characters.
     """
 
-    profile: Optional[str] = None
-    """
-    An URL identifying the profile of this descriptor as per the profiles specification.
-    """
-
     title: Optional[str] = None
     """
     A string providing a title or one sentence description for this package
     """
 
     description: Optional[str] = None
     """
@@ -101,23 +102,14 @@
 
     def model_post_init(self, _):
         for resource in self.resources:
             resource.basepath = self.basepath
 
     # Getters
 
-    def get_profile(self) -> Optional[Profile]:
-        """Get the resovled profile of the package
-
-        Returns:
-            The resolved profile of the package
-        """
-        if self.profile:
-            return Profile.from_path(self.profile)
-
     def get_resource(
         self, *, name: Optional[str] = None, path: Optional[str] = None
     ) -> Optional[Resource]:
         """Get a resource by name or path
 
         Parameters:
             name: The name of the resource
```

### Comparing `dplib_py-0.6.0/dplib/models/package/__spec__/test_package.py` & `dplib_py-0.7.0/dplib/models/package/__spec__/test_package.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,22 +47,14 @@
 
 def test_package_set_proprty_invalid():
     package = Package()
     with pytest.raises(ValidationError):
         package.name = 1  # type: ignore
 
 
-@pytest.mark.vcr
-def test_package_profile():
-    package = Package.from_path("data/package-full.json")
-    profile = package.get_profile()
-    assert profile
-    assert profile.jsonSchema.get("title") == "Data Package"
-
-
 def test_package_get_resource_by_name():
     package = Package.from_path("data/package.json")
     resource = package.get_resource(name="name")
     assert resource
     assert resource.name == "name"
     assert resource.path == "table.csv"
 
@@ -106,7 +98,13 @@
     package.dereference()
     resource = package.get_resource(name="name")
     assert resource
     assert isinstance(resource.dialect, Dialect)
     assert resource.dialect.delimiter == ";"
     assert isinstance(resource.schema, Schema)
     assert len(resource.schema.fields) == 2
+
+
+def test_package_contributors_role_v1():
+    package = Package.from_dict({"contributors": [{"role": "author"}]})
+    assert package.contributors[0].custom == {}
+    assert package.contributors[0].roles == ["author"]
```

### Comparing `dplib_py-0.6.0/dplib/models/resource/hash.py` & `dplib_py-0.7.0/dplib/models/resource/hash.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/models/resource/resource.py` & `dplib_py-0.7.0/dplib/models/resource/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from __future__ import annotations
 
 from typing import Any, List, Optional, Union
 
 import pydantic
 
-from ... import types
+from ... import settings, types
 from ...helpers.file import join_basepath
-from ...model import Model
+from ...system import Model
 from ..contributor import Contributor
 from ..dialect import Dialect
 from ..license import License
-from ..profile import Profile
 from ..schema import Schema
 from ..source import Source
 from .hash import Hash
 
 
 class Resource(Model):
     """Data Resource model"""
 
+    profile: str = pydantic.Field(
+        default=settings.PROFILE_CURRENT_RESOURCE,
+        alias="$schema",
+    )
+    """A profile URL"""
+
     basepath: Optional[str] = pydantic.Field(default=None, exclude=True)
     """
     Basepath of the resource.
     The data path and dialect/schema will be relative to this basepath.
     """
 
     name: Optional[str] = None
@@ -43,19 +48,14 @@
 
     data: Optional[Any] = None
     """
     Resource data rather than being stored in external files can be shipped inline
     on a Resource using the data property.
     """
 
-    profile: Optional[str] = None
-    """
-    An URL identifying the profile of this descriptor as per the profiles specification.
-    """
-
     dialect: Optional[Union[Dialect, str]] = None
     """
     A dialect property MAY be provided to specify Table Dialect
     """
 
     schema: Optional[Union[Schema, str]] = None  # type: ignore
     """
@@ -125,31 +125,22 @@
 
         Returns:
             The full path of the resource
         """
         if self.path and isinstance(self.path, str):
             return join_basepath(self.path, self.basepath)
 
-    def get_source(self) -> Optional[Union[str, types.IDict]]:
+    def get_source(self) -> Optional[Union[str, types.IData]]:
         """Get the source of the resource
 
         Returns:
             Data or full path
         """
         return self.data if self.data is not None else self.get_fullpath()
 
-    def get_profile(self) -> Optional[Profile]:
-        """Get the resovled profile of the resource
-
-        Returns:
-            The resolved profile of the resource
-        """
-        if self.profile:
-            return Profile.from_path(self.profile)
-
     def get_dialect(self) -> Optional[Dialect]:
         """Get the resolved dialect of the resource
 
         Returns:
             The resolved dialect of the resource
         """
         if self.dialect:
@@ -183,7 +174,23 @@
         """Dereference the package
         It will dereference all the resource's dialects and schemas
         """
         if isinstance(self.dialect, str):
             self.dialect = Dialect.from_path(self.dialect, basepath=self.basepath)
         if isinstance(self.schema, str):
             self.schema = Schema.from_path(self.schema, basepath=self.basepath)  # type: ignore
+
+    # Compat
+
+    @pydantic.model_validator(mode="before")
+    @classmethod
+    def compat(cls, data: types.IData):
+        if not isinstance(data, dict):  # type: ignore
+            return data
+
+        # resource.url
+        if not data.get("path"):
+            url = data.pop("url", None)
+            if url:
+                data["path"] = url
+
+        return data
```

### Comparing `dplib_py-0.6.0/dplib/models/resource/__spec__/test_resource.py` & `dplib_py-0.7.0/dplib/models/resource/__spec__/test_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,22 +51,14 @@
 
 def test_resource_set_proprty_invalid():
     resource = Resource()
     with pytest.raises(ValidationError):
         resource.name = 1  # type: ignore
 
 
-@pytest.mark.vcr
-def test_resource_profile():
-    resource = Resource.from_path("data/resource-full.json")
-    profile = resource.get_profile()
-    assert profile
-    assert profile.jsonSchema.get("title") == "Tabular Data Resource"
-
-
 def test_resource_get_fullpath():
     resource = Resource.from_path("data/resource.json")
     fullpath = resource.get_fullpath()
     assert fullpath == str(Path("data/table.csv"))
 
 
 def test_resource_get_fullpath_with_basepath():
@@ -118,7 +110,13 @@
 def test_resource_dereference():
     resource = Resource.from_path("data/resource-full.json")
     resource.dereference()
     assert isinstance(resource.dialect, Dialect)
     assert resource.dialect.delimiter == ";"
     assert isinstance(resource.schema, Schema)
     assert len(resource.schema.fields) == 2
+
+
+def test_resource_contributors_role_v1():
+    resource = Resource.from_dict({"contributors": [{"role": "author"}]})
+    assert resource.contributors[0].custom == {}
+    assert resource.contributors[0].roles == ["author"]
```

### Comparing `dplib_py-0.6.0/dplib/models/schema/schema.py` & `dplib_py-0.7.0/dplib/models/schema/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,78 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from ...model import Model
-from ..profile import Profile
-from .field import Field
+import pydantic
+
+from ... import settings, types
+from ...system import Model
+from ..field import IField
 from .foreignKey import ForeignKey
+from .types import IFieldsMatch
 
 
 class Schema(Model):
     """Table Schema model"""
 
-    profile: Optional[str] = None
-    """
-    An URL identifying the profile of this descriptor as per the profiles specification.
-    """
+    profile: str = pydantic.Field(
+        default=settings.PROFILE_CURRENT_SCHEMA,
+        alias="$schema",
+    )
+    """A profile URL"""
 
     title: Optional[str] = None
     """
     A string providing a title or one sentence description for this schema
     """
 
     description: Optional[str] = None
     """
     A description of the schema. The description MUST be markdown formatted —
     this also allows for simple plain text as plain text is itself valid markdown.
     """
 
-    fields: List[Field] = []
+    fields: List[IField] = []
     """
     List of fields in the table schema
     """
 
+    fieldsMatch: Optional[IFieldsMatch] = "exact"
+    """
+    The way Table Schema fields are mapped onto the data source fields
+    are defined by the fieldsMatch property.
+    """
+
     missingValues: List[str] = [""]
     """
     A list of field values to consider as null values
     """
 
     primaryKey: List[str] = []
     """
     A primary key is a field or set of fields that uniquely identifies
     each row in the table.
     """
 
+    uniqueKeys: List[List[str]] = []
+    """
+    A unique key is a field or a set of fields that are required
+    to have unique logical values in each row in the table.
+    """
+
     foreignKeys: List[ForeignKey] = []
     """
     A foreign key is a reference where values in a field (or fields)
     on the table (‘resource’ in data package terminology) described by this Table Schema
     connect to values a field (or fields) on this or a separate table (resource).
     """
 
     # Getters
 
-    def get_profile(self) -> Optional[Profile]:
-        """Get the resovled profile of the schema
-
-        Returns:
-            The resolved profile of the schema
-        """
-        if self.profile:
-            return Profile.from_path(self.profile)
-
-    def get_field(self, *, name: Optional[str] = None) -> Optional[Field]:
+    def get_field(self, *, name: Optional[str] = None) -> Optional[IField]:
         """Get a field by name
 
         Parameters:
             name: The name of the field to get
 
         Returns:
             The field with the given name if found
@@ -89,19 +96,34 @@
         """Get the types of the fields in the schema
 
         Returns:
             The types of the fields in the schema
         """
         types: List[str] = []
         for field in self.fields:
-            types.append(field.type)
+            types.append(field.type or "any")
         return types
 
     # Setters
 
-    def add_field(self, field: Field):
+    def add_field(self, field: IField):
         """Add a field to the schema
 
         Parameters:
             field: The field to add
         """
         self.fields.append(field)
+
+    # Compat
+
+    @pydantic.model_validator(mode="before")
+    @classmethod
+    def compat(cls, data: types.IData):
+        if not isinstance(data, dict):  # type: ignore
+            return data
+
+        # schema.primaryKey
+        primaryKey = data.get("primaryKey", None)
+        if isinstance(primaryKey, str):
+            data["primaryKey"] = [primaryKey]
+
+        return data
```

### Comparing `dplib_py-0.6.0/dplib/models/schema/__spec__/test_schema.py` & `dplib_py-0.7.0/dplib/models/schema/__spec__/test_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from pydantic import ValidationError
 
-from dplib.models import Field, Schema
+from dplib.models import IntegerField, Schema
 
 
 def test_schema_from_path():
     schema = Schema.from_path("data/schema.json")
     assert len(schema.fields) == 2
     assert schema.fields[0].name == "id"
     assert schema.fields[0].type == "integer"
@@ -48,25 +48,17 @@
 
 def test_schema_set_proprty_invalid():
     schema = Schema()
     with pytest.raises(ValidationError):
         schema.missingValues = 1  # type: ignore
 
 
-@pytest.mark.vcr
-def test_schema_profile():
-    schema = Schema.from_path("data/schema-full.json")
-    profile = schema.get_profile()
-    assert profile
-    assert profile.jsonSchema.get("title") == "Table Schema"
-
-
 def test_schema_add_field():
     schema = Schema()
-    schema.add_field(Field(name="id", type="integer"))
+    schema.add_field(IntegerField(name="id"))
     field = schema.get_field(name="id")
     assert field
     assert field.name == "id"
     assert field.type == "integer"
 
 
 def test_schema_get_field():
@@ -78,7 +70,20 @@
 
 
 def test_schema_to_dict():
     schema = Schema()
     assert schema.to_dict() == {}
     schema.missingValues.append("x")
     assert schema.to_dict() == {"missingValues": ["", "x"]}
+
+
+def test_schema_primary_key_v1():
+    schema = Schema.from_dict({"primaryKey": "name"})
+    assert schema.primaryKey == ["name"]
+
+
+def test_schema_foreign_keys_v1():
+    schema = Schema.from_dict(
+        {"foreignKeys": [{"fields": "name", "reference": {"fields": "name"}}]}
+    )
+    assert schema.foreignKeys[0].fields == ["name"]
+    assert schema.foreignKeys[0].reference.fields == ["name"]
```

### Comparing `dplib_py-0.6.0/dplib/plugins/ckan/models/package.py` & `dplib_py-0.7.0/dplib/plugins/ckan/models/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from dplib.model import Model
 from dplib.models import Contributor, License, Package
+from dplib.system import Model
 
 from .organization import CkanOrganization
 from .resource import CkanResource
 from .tag import CkanTag
 
 # References:
 # - https://demo.ckan.org/api/3/action/package_show?id=sample-dataset-1
@@ -69,25 +69,25 @@
 
         # License
         if self.license_id:
             license = License(name=self.license_id)
             if self.license_title:
                 license.title = self.license_title
             if self.license_url:
-                license.url = self.license_url
+                license.path = self.license_url
             package.licenses.append(license)
 
         # Contributors
         if self.author:
-            contributor = Contributor(title=self.author, role="author")
+            contributor = Contributor(title=self.author, roles=["author"])
             if self.author_email:
                 contributor.email = self.author_email
             package.contributors.append(contributor)
         if self.maintainer:
-            contributor = Contributor(title=self.maintainer, role="maintainer")
+            contributor = Contributor(title=self.maintainer, roles=["maintainer"])
             if self.maintainer_email:
                 contributor.email = self.maintainer_email
             package.contributors.append(contributor)
 
         # Resources
         for item in self.resources:
             resource = item.to_dp()
@@ -138,20 +138,21 @@
             if license.title:
                 ckan.license_title = license.title
             if license.path:
                 ckan.license_url = license.path
 
         # Contributors
         for contributor in package.contributors:
-            if contributor.role == "author":
-                ckan.author = contributor.title
-                ckan.author_email = contributor.email
-            elif contributor.role == "maintainer":
-                ckan.maintainer = contributor.title
-                ckan.maintainer_email = contributor.email
+            if contributor.roles:
+                if "author" in contributor.roles:
+                    ckan.author = contributor.title
+                    ckan.author_email = contributor.email
+                elif "maintainer" in contributor.roles:
+                    ckan.maintainer = contributor.title
+                    ckan.maintainer_email = contributor.email
 
         # Resources
         for resource in package.resources:
             item = CkanResource.from_dp(resource)
             if item:
                 ckan.resources.append(item)
```

### Comparing `dplib_py-0.6.0/dplib/plugins/ckan/models/resource.py` & `dplib_py-0.7.0/dplib/plugins/ckan/models/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from dplib.helpers.resource import slugify_name
-from dplib.model import Model
 from dplib.models import Resource
+from dplib.system import Model
 
 
 class CkanResource(Model):
     """CKAN Resource model"""
 
     name: str
     created: Optional[str] = None
```

### Comparing `dplib_py-0.6.0/dplib/plugins/ckan/models/__spec__/test_package.py` & `dplib_py-0.7.0/dplib/plugins/ckan/models/__spec__/test_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     assert package.licenses[0].name == "cc-by"
     assert len(package.resources) == 9
     assert len(package.keywords) == 8
     assert len(package.contributors) == 2
     assert package.resources[0].path == "sample-linked.csv"
     assert package.keywords[0] == "csv"
     assert package.contributors[0].title == "Test Author"
-    assert package.contributors[0].role == "author"
+    assert package.contributors[0].roles == ["author"]
     assert package.custom["ckan:id"] == "c322307a-b871-44fe-a602-32ee8437ff04"
 
 
 def test_ckan_package_from_dp():
     package = CkanPackage.from_dp(Package.from_path("data/package-full.json"))
     assert package.name == "name"
     assert package.name == "name"
```

### Comparing `dplib_py-0.6.0/dplib/plugins/cli/program.py` & `dplib_py-0.7.0/dplib/plugins/cli/program.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/cli/commands/main.py` & `dplib_py-0.7.0/dplib/plugins/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/cli/commands/package/convert.py` & `dplib_py-0.7.0/dplib/plugins/cli/commands/package/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/cli/commands/resource/convert.py` & `dplib_py-0.7.0/dplib/plugins/cli/commands/resource/convert.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/cli/helpers/check.py` & `dplib_py-0.7.0/dplib/plugins/cli/helpers/check.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/datacite/models/contributor.py` & `dplib_py-0.7.0/dplib/plugins/datacite/models/contributor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from dplib.model import Model
+from dplib.system import Model
 
 
 class DataciteContributorAffiliation(Model):
     name: Optional[str] = None
     affiliationIdentifier: Optional[str] = None
     affiliationIdentifierScheme: Optional[str] = None
```

### Comparing `dplib_py-0.6.0/dplib/plugins/datacite/models/package.py` & `dplib_py-0.7.0/dplib/plugins/datacite/models/package.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from dplib.model import Model
 from dplib.models import Contributor, License, Package
+from dplib.system import Model
 
 from .contributor import DataciteContributor, DataciteContributorAffiliation
 from .description import DataciteDescription
 from .identifier import DataciteIdentifier
 from .rights import DataciteRights
 from .subject import DataciteSubject
 from .title import DataciteTitle
@@ -76,16 +76,23 @@
         # Keywords
         for subject in self.subjects:
             package.keywords.append(subject.subject)
 
         # Contributors
         for type, items in [("creator", self.creators), ("other", self.contributors)]:
             for item in items:
-                contributor = Contributor(title=item.name)
-                contributor.role = type if type == "creator" else item.contributorType
+                contributor = Contributor(
+                    title=item.name,
+                    givenName=item.givenName,
+                    familyName=item.familyName,
+                )
+                if type == "creator":
+                    contributor.roles = [type]
+                elif item.contributorType:
+                    contributor.roles = [item.contributorType]
                 for affiliation in item.affiliation:
                     contributor.organization = affiliation.name
                     break
                 package.contributors.append(contributor)
 
         # Licenses
         for rights in self.rightsList:
@@ -142,19 +149,23 @@
 
         # Keywords
         for keyword in package.keywords:
             datacite.subjects.append(DataciteSubject(subject=keyword))
 
         # Contributors
         for contributor in package.contributors:
-            item = DataciteContributor(name=contributor.title)
+            item = DataciteContributor(
+                name=contributor.title,
+                givenName=contributor.givenName,
+                familyName=contributor.familyName,
+            )
             if contributor.organization:
                 org = DataciteContributorAffiliation(name=contributor.organization)
                 item.affiliation.append(org)
-            if contributor.role:
-                item.contributorType = contributor.role
             target = datacite.contributors
-            if contributor.role in ["author", "creator"]:
-                target = datacite.creators
+            if contributor.roles:
+                item.contributorType = contributor.roles[0]
+                if set(contributor.roles).intersection(["author", "creator"]):
+                    target = datacite.creators
             target.append(item)
 
         return datacite
```

### Comparing `dplib_py-0.6.0/dplib/plugins/datacite/models/__spec__/test_package.py` & `dplib_py-0.7.0/dplib/plugins/datacite/models/__spec__/test_package.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     assert package.publisher == "DataCite"
     assert package.publicationYear == "2014"
     assert package.schemaVersion == "http://datacite.org/schema/kernel-4"
     assert len(package.creators) == 1
     assert package.creators[0].name == "Miller, Elizabeth"
     assert len(package.contributors) == 1
     assert package.contributors[0].name == "Starr, Joan"
+    assert package.contributors[0].givenName == "Joan"
+    assert package.contributors[0].familyName == "Starr"
     assert len(package.descriptions) == 1
     assert package.descriptions[0].descriptionType == "Abstract"
     assert len(package.identifiers) == 2
     assert package.identifiers[0].identifierType == "DOI"
     assert len(package.rightsList) == 1
     assert package.rightsList[0].lang == "en-US"
     assert len(package.subjects) == 1
@@ -37,16 +39,20 @@
         package.homepage
         == "https://schema.datacite.org/meta/kernel-4.3/example/datacite-example-full-v4.3.xml"
     )
     assert package.version == "4.2"
     assert package.keywords == ["000 computer science"]
     assert len(package.contributors) == 2
     assert package.contributors[0].title == "Miller, Elizabeth"
+    assert package.contributors[0].givenName == "Elizabeth"
+    assert package.contributors[0].familyName == "Miller"
     assert package.contributors[1].title == "Starr, Joan"
-    assert package.contributors[1].role == "ProjectLeader"
+    assert package.contributors[1].givenName == "Joan"
+    assert package.contributors[1].familyName == "Starr"
+    assert package.contributors[1].roles == ["ProjectLeader"]
     assert len(package.licenses) == 1
     assert package.licenses[0].path == "http://creativecommons.org/publicdomain/zero/1.0"
 
 
 def test_datacite_package_from_dp():
     package = DatacitePackage.from_dp(Package.from_path("data/package-full.json"))
     assert package.version == "1.0"
@@ -69,14 +75,16 @@
         DatacitePackage.from_path("data/plugins/datacite/package.json").to_dp()
     )
     assert package.version == "4.2"
     assert len(package.creators) == 1
     assert package.creators[0].name == "Miller, Elizabeth"
     assert len(package.contributors) == 1
     assert package.contributors[0].name == "Starr, Joan"
+    assert package.contributors[0].givenName == "Joan"
+    assert package.contributors[0].familyName == "Starr"
     assert len(package.descriptions) == 1
     assert package.descriptions[0].descriptionType == "Abstract"
     assert len(package.identifiers) == 2
     assert package.identifiers[0].identifierType == "DOI"
     assert len(package.subjects) == 1
     assert package.subjects[0].subject == "000 computer science"
     assert len(package.titles) == 1
```

### Comparing `dplib_py-0.6.0/dplib/plugins/dcat/models/helpers.py` & `dplib_py-0.7.0/dplib/plugins/dcat/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/dcat/models/loaders.py` & `dplib_py-0.7.0/dplib/plugins/dcat/models/loaders.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/dcat/models/namespaces.py` & `dplib_py-0.7.0/dplib/plugins/dcat/models/namespaces.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/dcat/models/package.py` & `dplib_py-0.7.0/dplib/plugins/dcat/models/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Any, List, Optional
 
 from rdflib import BNode, Graph, URIRef
 
 from dplib.error import Error
-from dplib.model import Model
-from dplib.models import Package
+from dplib.models import Package, Source
+from dplib.system import Model
 
 from . import dumpers, loaders
 from . import namespaces as ns
 from .resource import DcatResource
 
 # References:
 # - https://www.w3.org/TR/vocab-dcat-2/
@@ -310,14 +310,19 @@
             if "T" in self.issued:
                 package.created = self.issued
 
         # Keywords
         for keyword in self.keywords:
             package.keywords.append(keyword)
 
+        # Sources
+        for source in self.sources:
+            source = Source(title=source)
+            package.sources.append(source)
+
         # Resources
         for distribution in self.distributions:
             resource = distribution.to_dp()
             if resource:
                 package.resources.append(resource)
 
         return package
@@ -358,14 +363,20 @@
         if package.created:
             dcat.issued = package.created
 
         # Keywords
         for keyword in package.keywords:
             dcat.keywords.append(keyword)
 
+        # Sources
+        for source in package.sources:
+            source = source.path or source.title
+            if source:
+                dcat.sources.append(source)
+
         # Resources
         for resource in package.resources:
             distribution = DcatResource.from_dp(resource)
             if distribution:
                 dcat.distributions.append(distribution)
 
         return dcat
```

### Comparing `dplib_py-0.6.0/dplib/plugins/dcat/models/resource.py` & `dplib_py-0.7.0/dplib/plugins/dcat/models/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 from rdflib import BNode, Graph
 
 from dplib.helpers.resource import slugify_name
-from dplib.model import Model
 from dplib.models import License, Resource
+from dplib.system import Model
 
 from . import dumpers, loaders
 from . import namespaces as ns
 from .types import ISubject
 
 
 class DcatResource(Model):
```

### Comparing `dplib_py-0.6.0/dplib/plugins/dcat/models/__spec__/test_package.py` & `dplib_py-0.7.0/dplib/plugins/dcat/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/github/models/package.py` & `dplib_py-0.7.0/dplib/plugins/github/models/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from dplib.model import Model
 from dplib.models import License, Package
+from dplib.system import Model
 
 from .license import GithubLicense
 from .owner import GithubOwner
 from .resource import GithubResource
 
 # References:
 # - https://docs.github.com/en/free-pro-team@latest/rest/repos/repos?apiVersion=2022-11-28#get-a-repository
@@ -65,15 +65,15 @@
         if self.license:
             license = License()
             if self.license.spdx_id:
                 license.name = self.license.spdx_id
             if self.license.name:
                 license.title = self.license.name
             if self.license.html_url:
-                license.url = self.license.html_url
+                license.path = self.license.html_url
             package.licenses.append(license)
 
         # Keywords
         for topic in self.topics:
             package.keywords.append(topic)
 
         # Resources
```

### Comparing `dplib_py-0.6.0/dplib/plugins/github/models/resource.py` & `dplib_py-0.7.0/dplib/plugins/github/models/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Literal, Optional
 
 from dplib.helpers.resource import slugify_name
-from dplib.model import Model
 from dplib.models import Resource
+from dplib.system import Model
 
 
 class GithubResource(Model):
     """Github Resource model"""
 
     name: str
     path: str
```

### Comparing `dplib_py-0.6.0/dplib/plugins/github/models/__spec__/test_package.py` & `dplib_py-0.7.0/dplib/plugins/github/models/__spec__/test_package.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/pandas/models/field.py` & `dplib_py-0.7.0/dplib/plugins/polars/models/field.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,121 @@
 from __future__ import annotations
 
-import datetime
-from typing import Any, Optional
+from typing import Any
 
-import isodate  # type: ignore
-import numpy as np
-import pandas as pd
-import pandas.core.dtypes.api as pdc
+import polars as pl
 
+from dplib import models
 from dplib.error import Error
-from dplib.model import Model
-from dplib.models import Field
+from dplib.system import Model
 
 
-class PandasField(Model, arbitrary_types_allowed=True):
-    """Pandas Field model"""
+class PolarsField(Model, arbitrary_types_allowed=True):
+    """Polars Field model"""
 
     name: str
     dtype: Any
-    dvalue: Optional[Any] = None
+    #  dtype: pl.PolarsDataType
 
     # Converters
 
-    def to_dp(self) -> Field:
+    def to_dp(self) -> models.IField:
         """Convert to Table Schema Field
 
         Returns:
             Table Schema Field
         """
-        field = Field(name=self.name)
 
         # Type
-        if pdc.is_bool_dtype(self.dtype):  # type: ignore
-            field.type = "boolean"
-        elif pdc.is_datetime64_any_dtype(self.dtype):  # type: ignore
-            field.type = "datetime"
-        elif pdc.is_integer_dtype(self.dtype):  # type: ignore
-            field.type = "integer"
-        elif pdc.is_numeric_dtype(self.dtype):  # type: ignore
-            field.type = "number"
-        elif self.dvalue is not None:
-            if isinstance(self.dvalue, (list, tuple)):  # type: ignore
-                field.type = "array"
-            elif isinstance(self.dvalue, datetime.datetime):
-                field.type = "datetime"
-            elif isinstance(self.dvalue, datetime.date):
-                field.type = "date"
-            elif isinstance(self.dvalue, isodate.Duration):  # type: ignore
-                field.type = "duration"
-            elif isinstance(self.dvalue, dict):
-                field.type = "object"
-            elif isinstance(self.dvalue, str):
-                field.type = "string"
-            elif isinstance(self.dvalue, datetime.time):
-                field.type = "time"
+        Field = models.Field
+        if self.dtype in ARRAY_TYPES:
+            Field = models.ArrayField
+        elif self.dtype in BOOLEAN_TYPES:
+            Field = models.BooleanField
+        elif self.dtype in DATE_TYPES:
+            Field = models.DateField
+        elif self.dtype in DATETIME_TYPES:
+            Field = models.DatetimeField
+        elif self.dtype in DURATION_TYPES:
+            Field = models.DurationField
+        elif self.dtype in INTEGER_TYPES:
+            Field = models.IntegerField
+        elif self.dtype in NUMBER_TYPES:
+            Field = models.NumberField
+        elif self.dtype in OBJECT_TYPES:
+            Field = models.ObjectField
+        elif self.dtype in STRING_TYPES:
+            Field = models.StringField
+        elif self.dtype in TIME_TYPES:
+            Field = models.TimeField
+
+        # Name
+        field = Field(name=self.name)
 
         return field
 
     @classmethod
-    def from_dp(cls, field: Field) -> PandasField:
-        """Create Pandas Field from Table Schema Field
+    def from_dp(cls, field: models.IField) -> PolarsField:
+        """Create Polars Field from Table Schema Field
 
         Parameters:
             field: Table Schema Field
 
         Returns:
-            Pandas Field
+            Polars Field
         """
         if not field.name:
-            raise Error(f"Field name is required to convert to pandas: {field}")
+            raise Error(f"Field name is required to convert to polars: {field}")
 
         # Type
-        dtype = np.dtype("O")
+        dtype = pl.Utf8
         if field.type == "array":
-            dtype = np.dtype(list)  # type: ignore
+            dtype = pl.List
         elif field.type == "boolean":
-            dtype = np.dtype(bool)
+            dtype = pl.Boolean
+        elif field.type == "date":
+            dtype = pl.Date
         elif field.type == "datetime":
-            dtype = pd.DatetimeTZDtype(tz="UTC")
-        elif field.type == "integer":
-            dtype = np.dtype(int)
+            dtype = pl.Datetime
+        elif field.type == "duration":
+            dtype = pl.Duration
         elif field.type == "geojson":
-            dtype = np.dtype(dict)
+            dtype = pl.Struct
+        elif field.type == "geopoint":
+            dtype = pl.List
+        elif field.type == "integer":
+            dtype = pl.Int64
         elif field.type == "number":
-            dtype = np.dtype(float)
+            dtype = pl.Decimal
         elif field.type == "object":
-            dtype = np.dtype(dict)
+            dtype = pl.Struct
         elif field.type == "string":
-            dtype = np.dtype(str)
+            dtype = pl.Utf8
+        elif field.type == "time":
+            dtype = pl.Time
         elif field.type == "year":
-            dtype = np.dtype(int)
-
-        return PandasField(name=field.name, dtype=dtype)
+            dtype = pl.Int8
+        elif field.type == "yearmonth":
+            dtype = pl.List
+
+        return PolarsField(name=field.name, dtype=dtype)
+
+
+ARRAY_TYPES = (pl.Array, pl.List)
+BOOLEAN_TYPES = (pl.Boolean,)
+DATE_TYPES = (pl.Date,)
+DATETIME_TYPES = (pl.Datetime,)
+DURATION_TYPES = (pl.Duration,)
+INTEGER_TYPES = (
+    pl.Int8,
+    pl.Int16,
+    pl.Int32,
+    pl.Int64,
+    pl.UInt8,
+    pl.UInt16,
+    pl.UInt32,
+    pl.UInt64,
+)
+NUMBER_TYPES = (pl.Float32, pl.Float64, pl.Decimal)
+STRING_TYPES = (pl.Utf8, pl.Categorical)
+OBJECT_TYPES = (pl.Struct,)
+TIME_TYPES = (pl.Time,)
```

### Comparing `dplib_py-0.6.0/dplib/plugins/pandas/models/schema.py` & `dplib_py-0.7.0/dplib/plugins/pandas/models/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Any, Dict, List
 
 import pandas as pd
 
-from dplib.model import Model
 from dplib.models import Schema
+from dplib.system import Model
 
 from .field import PandasField
 
 
 class PandasSchema(Model, arbitrary_types_allowed=True):
     """Pandas Schema model"""
```

### Comparing `dplib_py-0.6.0/dplib/plugins/polars/models/schema.py` & `dplib_py-0.7.0/dplib/plugins/polars/models/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Dict, List
 
 import polars as pl
 
-from dplib.model import Model
 from dplib.models import Schema
+from dplib.system import Model
 
 from .field import PolarsField
 
 
 class PolarsSchema(Model, arbitrary_types_allowed=True):
     """Polars Schema model"""
```

### Comparing `dplib_py-0.6.0/dplib/plugins/polars/models/__spec__/test_schema.py` & `dplib_py-0.7.0/dplib/plugins/polars/models/__spec__/test_schema.py`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/dplib/plugins/sql/models/field.py` & `dplib_py-0.7.0/dplib/plugins/sql/models/field.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,78 +6,81 @@
 
 import sqlalchemy as sa
 from sqlalchemy.dialects import mysql as ml
 from sqlalchemy.dialects import postgresql as pg
 from sqlalchemy.dialects import registry
 from sqlalchemy.schema import Column
 
-from dplib.model import Model
-from dplib.models import Field
+from dplib import models
+from dplib.system import Model
 
 from . import settings
 
 
 class SqlField(Model, arbitrary_types_allowed=True):
     """SQL Field model"""
 
     column: Column[Any]
 
     # Converters
 
-    def to_dp(self) -> Field:
+    def to_dp(self) -> models.IField:
         """Convert to Table Schema Field
 
         Returns:
             Table Schema Field
         """
-        field = Field(name=self.column.name)
-
         # Type
+        Field = models.Field
         if isinstance(self.column.type, ARRAY_TYPES):
-            field.type = "array"
+            Field = models.ArrayField
         elif isinstance(self.column.type, BOOLEAN_TYPES):
-            field.type = "boolean"
+            Field = models.BooleanField
         elif isinstance(self.column.type, DATE_TYPES):
-            field.type = "date"
+            Field = models.DateField
         elif isinstance(self.column.type, DATETIME_TYPES):
-            field.type = "datetime"
+            Field = models.DatetimeField
         elif isinstance(self.column.type, INTEGER_TYPES):
-            field.type = "integer"
+            Field = models.IntegerField
         elif isinstance(self.column.type, NUMBER_TYPES):
-            field.type = "number"
+            Field = models.NumberField
         elif isinstance(self.column.type, OBJECT_TYPES):
-            field.type = "object"
-        elif isinstance(self.column.type, TEXT_TYPES):
-            field.type = "string"
+            Field = models.ObjectField
+        elif isinstance(self.column.type, STRING_TYPES):
+            Field = models.StringField
         elif isinstance(self.column.type, TIME_TYPES):
-            field.type = "time"
+            Field = models.TimeField
+
+        # Name
+        field = Field(name=self.column.name)
 
         # Description
         if self.column.comment:
             field.description = self.column.comment
 
         # Constraints
         if not self.column.nullable:
             field.constraints.required = True
-        if isinstance(self.column.type, (sa.CHAR, sa.VARCHAR)):
-            if self.column.type.length:
-                field.constraints.maxLength = self.column.type.length
-        if isinstance(self.column.type, sa.CHAR):
-            if self.column.type.length:
-                field.constraints.minLength = self.column.type.length
         if isinstance(self.column.type, sa.Enum):
             if self.column.enums:
                 field.constraints.enum = self.column.enums
+        if isinstance(field, models.StringField):
+            if isinstance(self.column.type, (sa.CHAR, sa.VARCHAR)):
+                if self.column.type.length:
+                    field.constraints.maxLength = self.column.type.length
+            if isinstance(self.column.type, sa.CHAR):
+                if self.column.type.length:
+                    field.constraints.minLength = self.column.type.length
 
         return field
 
     @classmethod
     def from_dp(
         cls,
-        field: Field,
+        field: models.IField,
         *,
         dialect: str = settings.DEFAULT_DIALECT,
         table_name: Optional[str] = None,
     ) -> SqlField:
         """Create SQL Field from Table Schema Field
 
         Parameters:
@@ -85,15 +88,15 @@
             dialect: SQL dialect
             table_name: SQL table name
 
         Returns:
             SQL Field
         """
         Check = sa.CheckConstraint
-        checks: List[Check] = []
+        checks: List[sa.CheckConstraint] = []
         comment = field.description
         dialect_obj = registry.load(dialect)()
         nullable = not field.constraints.required
         quoted_name = dialect_obj.identifier_preparer.quote(field.name)
 
         # Type
         column_type = sa.Text
@@ -144,15 +147,15 @@
                 if dialect_obj.name == "sqlite":
                     checks.append(Check("LENGTH(%s) <= %s" % (quoted_name, max)))
             if min is not None:
                 if not isinstance(column_type, sa.CHAR) or dialect_obj.name == "sqlite":
                     checks.append(Check("LENGTH(%s) >= %s" % (quoted_name, min)))
 
         # Limit contstraints
-        if field.type in ["integer", "number"]:
+        if isinstance(field, (models.IntegerField, models.NumberField)):
             min = field.constraints.minimum
             max = field.constraints.maximum
             if min is not None:
                 checks.append(Check("%s >= %s" % (quoted_name, min)))
             if max is not None:
                 checks.append(Check("%s <= %s" % (quoted_name, max)))
 
@@ -189,9 +192,8 @@
 BOOLEAN_TYPES = (sa.Boolean,)
 DATE_TYPES = (sa.Date,)
 DATETIME_TYPES = (sa.DateTime,)
 INTEGER_TYPES = (sa.Integer,)
 NUMBER_TYPES = (sa.Float, sa.Numeric)  # type: ignore
 STRING_TYPES = (ml.BIT, ml.VARBINARY, ml.VARCHAR, pg.UUID, sa.Text, sa.VARCHAR)  # type: ignore
 OBJECT_TYPES = (pg.JSONB, pg.JSON)
-TEXT_TYPES = (sa.Text,)
 TIME_TYPES = (sa.Time,)
```

### Comparing `dplib_py-0.6.0/dplib/plugins/sql/models/schema.py` & `dplib_py-0.7.0/dplib/plugins/sql/models/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Any, Callable, List
 
 import sqlalchemy as sa
 from sqlalchemy.schema import Column, Constraint, Table
 
-from dplib.model import Model
 from dplib.models import ForeignKey, ForeignKeyReference, Schema
+from dplib.system import Model
 
 from . import settings
 from .field import SqlField
 
 
 class SqlSchema(Model, arbitrary_types_allowed=True):
     """SQL Schema model"""
```

### Comparing `dplib_py-0.6.0/dplib/plugins/sql/models/__spec__/test_schema.py` & `dplib_py-0.7.0/dplib/plugins/sql/models/__spec__/test_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sqlalchemy as sa
 from sqlalchemy.dialects import postgresql as pg
 
-from dplib.models import Field, Schema
+from dplib.models import Schema, StringField
 from dplib.plugins.sql.models import SqlSchema
 
 
 def test_sql_schema_from_dp():
     schema = SqlSchema.from_dp(
         Schema.from_path("data/schema-types.json"), table_name="test"
     )
@@ -89,14 +89,14 @@
         "time",
         "integer",
         "string",
     ]
 
 
 def test_sql_schema_from_dp_with_string_constraints():
-    field = Field(name="string", type="string")
+    field = StringField(name="string")
     field.constraints.minLength = 1
     field.constraints.enum = ["a", "b", "c"]
     field.constraints.pattern = "^[a-z]+$"
     schema = SqlSchema.from_dp(Schema(fields=[field]), table_name="test")
     assert len(schema.table.columns[0].constraints) == 2
     assert isinstance(schema.table.columns[0].type, sa.Enum)
```

### Comparing `dplib_py-0.6.0/dplib/plugins/zenodo/models/creator.py` & `dplib_py-0.7.0/dplib/plugins/zenodo/models/creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 import pydantic
 
-from dplib.model import Model
+from dplib.system import Model
 
 
 class ZenodoCreatorAffiliation(Model):
     name: str
 
 
 class ZenodoCreatorPersonOrOrg(Model):
```

### Comparing `dplib_py-0.6.0/dplib/plugins/zenodo/models/package.py` & `dplib_py-0.7.0/dplib/plugins/zenodo/models/package.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Dict, Optional
 
 import pydantic
 
-from dplib.model import Model
 from dplib.models import Contributor, Package
+from dplib.system import Model
 
 from .creator import ZenodoCreator, ZenodoCreatorAffiliation
 from .files import ZenodoFiles
 from .metadata import ZenodoMetadata
 from .pid import ZenodoPid
 from .resource import ZenodoResource
 from .subject import ZenodoSubject
@@ -72,17 +72,21 @@
         # Keywords
         for subject in self.metadata.subjects:
             package.keywords.append(subject.subject)
 
         # Contributors
         for creator in self.metadata.creators:
             if creator.person_or_org.name:
-                contributor = Contributor(title=creator.person_or_org.name)
+                contributor = Contributor(
+                    title=creator.person_or_org.name,
+                    givenName=creator.person_or_org.given_name,
+                    familyName=creator.person_or_org.family_name,
+                )
                 if creator.person_or_org.type:
-                    contributor.role = creator.person_or_org.type
+                    contributor.roles = [creator.person_or_org.type]
                 if creator.affiliations:
                     contributor.organization = creator.affiliations[0].name
                 package.contributors.append(contributor)
 
         return package
 
     @classmethod
@@ -120,14 +124,16 @@
             subject = ZenodoSubject(subject=keyword)
             zenodo.metadata.subjects.append(subject)
 
         # Contributors
         for contributor in package.contributors:
             creator = ZenodoCreator()
             creator.person_or_org.name = contributor.title
-            if contributor.role:
-                creator.person_or_org.type = contributor.role
+            creator.person_or_org.given_name = contributor.givenName
+            creator.person_or_org.family_name = contributor.familyName
+            if contributor.roles:
+                creator.person_or_org.type = contributor.roles[0]
             if contributor.organization:
                 affiliation = ZenodoCreatorAffiliation(name=contributor.organization)
                 creator.affiliations.append(affiliation)
 
         return zenodo
```

### Comparing `dplib_py-0.6.0/dplib/plugins/zenodo/models/resource.py` & `dplib_py-0.7.0/dplib/plugins/zenodo/models/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from dplib.helpers.resource import slugify_name
-from dplib.model import Model
 from dplib.models import Resource
+from dplib.system import Model
 
 
 class ZenodoResource(Model):
     """Zenodo Resource model"""
 
     key: str
     id: Optional[str] = None
```

### Comparing `dplib_py-0.6.0/dplib/plugins/zenodo/models/__spec__/test_package.py` & `dplib_py-0.7.0/dplib/plugins/zenodo/models/__spec__/test_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,17 @@
     assert package.description
     assert package.description.startswith("<p>This dataset contains pool-weir")
     assert package.homepage == "https://zenodo.org/api/records/5770714"
     assert package.version == "v1"
     assert package.created == "2021-12-10T05:47:07.709885+00:00"
     assert len(package.contributors) == 1
     assert package.contributors[0].title == "Fuentes-Pérez, Juan Francisco"
-    assert package.contributors[0].role == "personal"
+    assert package.contributors[0].givenName == "Juan Francisco"
+    assert package.contributors[0].familyName == "Fuentes-Pérez"
+    assert package.contributors[0].roles == ["personal"]
     assert (
         package.contributors[0].organization
         == "Department of Hydraulics and Hydrology, ETSIIAA, University of Valladolid, 34004 Palencia, Spain"
     )
     assert package.keywords == [
         "fishways",
         "hydraulics",
```

### Comparing `dplib_py-0.6.0/dplib/profiles/data-package.json` & `dplib_py-0.7.0/dplib/profiles/1.0/datapackage.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7497251678752795%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'description'": "'Tabular Data Package is a simple specification for data access and delivery of "*

 * *                  "tabular data.'",*

 * * "'properties'": "{'resources': {'title': 'Tabular Data Resources', 'items': {'title': 'Tabular "*

 * *                 "Data Resource', 'description': 'A Tabular Data Resource.', 'properties': "*

 * *                 "{'dialect': {'properties': {'csvddfVersion': OrderedDict([('title', 'CSV Dialect "*

 * *                 "schema […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "$schema": "http://json-schema.org/draft-04/schema#",
-    "description": "Data Package",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "description": "Tabular Data Package is a simple specification for data access and delivery of tabular data.",
     "properties": {
         "contributors": {
             "description": "The contributors to this descriptor.",
             "examples": [
                 "{\n  \"contributors\": [\n    {\n      \"title\": \"Joe Bloggs\"\n    }\n  ]\n}\n",
                 "{\n  \"contributors\": [\n    {\n      \"title\": \"Joe Bloggs\",\n      \"email\": \"joe@example.com\",\n      \"role\": \"author\"\n    }\n  ]\n}\n"
             ],
@@ -205,15 +205,15 @@
         },
         "resources": {
             "description": "An `array` of Tabular Data Resource objects, each compliant with the [Tabular Data Resource](/tabular-data-resource/) specification.",
             "examples": [
                 "{\n  \"resources\": [\n    {\n      \"name\": \"my-data\",\n      \"data\": [\n        \"data.csv\"\n      ],\n      \"schema\": \"tableschema.json\",\n      \"mediatype\": \"text/csv\"\n    }\n  ]\n}\n"
             ],
             "items": {
-                "description": "Data Resource.",
+                "description": "A Tabular Data Resource.",
                 "oneOf": [
                     {
                         "required": [
                             "name",
                             "data"
                         ]
                     },
@@ -273,14 +273,23 @@
                                 "description": "Specifies that any row beginning with this one-character string, without preceeding whitespace, causes the entire line to be ignored.",
                                 "examples": [
                                     "{\n  \"commentChar\": \"#\"\n}\n"
                                 ],
                                 "title": "Comment Character",
                                 "type": "string"
                             },
+                            "csvddfVersion": {
+                                "default": 1.2,
+                                "description": "A number to indicate the schema version of CSV Dialect. Version 1.0 was named CSV Dialect Description Format and used different field names.",
+                                "examples:": [
+                                    "{\n  \"csvddfVersion\": \"1.2\"\n}\n"
+                                ],
+                                "title": "CSV Dialect schema version",
+                                "type": "number"
+                            },
                             "delimiter": {
                                 "default": ",",
                                 "description": "A character sequence to use as the field separator.",
                                 "examples": [
                                     "{\n  \"delimiter\": \",\"\n}\n",
                                     "{\n  \"delimiter\": \";\"\n}\n"
                                 ],
@@ -348,14 +357,18 @@
                                     "{\n  \"skipInitialSpace\": true\n}\n"
                                 ],
                                 "title": "Skip Initial Space",
                                 "type": "boolean"
                             }
                         },
                         "propertyOrder": 50,
+                        "required": [
+                            "delimiter",
+                            "doubleQuote"
+                        ],
                         "title": "CSV Dialect",
                         "type": [
                             "string",
                             "object"
                         ]
                     },
                     "encoding": {
@@ -2269,20 +2282,20 @@
                             "{\n  \"title\": \"My Package Title\"\n}\n"
                         ],
                         "propertyOrder": 50,
                         "title": "Title",
                         "type": "string"
                     }
                 },
-                "title": "Data Resource",
+                "title": "Tabular Data Resource",
                 "type": "object"
             },
             "minItems": 1,
             "propertyOrder": 120,
-            "title": "Data Resources",
+            "title": "Tabular Data Resources",
             "type": "array"
         },
         "sources": {
             "description": "The raw sources for this resource.",
             "examples": [
                 "{\n  \"sources\": [\n    {\n      \"title\": \"World Bank and OECD\",\n      \"path\": \"http://data.worldbank.org/indicator/NY.GDP.MKTP.CD\"\n    }\n  ]\n}\n"
             ],
@@ -2341,10 +2354,10 @@
             "title": "Title",
             "type": "string"
         }
     },
     "required": [
         "resources"
     ],
-    "title": "Data Package",
+    "title": "Tabular Data Package",
     "type": "object"
 }
```

### Comparing `dplib_py-0.6.0/dplib/profiles/data-resource.json` & `dplib_py-0.7.0/dplib/profiles/1.0/dataresource.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7491742198773449%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'description'": "'A Tabular Data Resource.'",*

 * * "'properties'": "{'profile': {delete: ['default']}, 'dialect': {'title': 'CSV Dialect', "*

 * *                 "'description': 'The CSV dialect descriptor.', 'properties': {'csvddfVersion': "*

 * *                 "OrderedDict([('title', 'CSV Dialect schema version'), ('description', 'A number "*

 * *                 'to indicate the schema version of CSV Dialect. Version 1.0 was named CSV Dialect '*

 * *                […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "$schema": "http://json-schema.org/draft-04/schema#",
-    "description": "A Data Resource.",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "description": "A Tabular Data Resource.",
     "oneOf": [
         {
             "required": [
                 "name",
                 "data"
             ]
         },
@@ -40,15 +40,15 @@
             ],
             "format": "textarea",
             "propertyOrder": 60,
             "title": "Description",
             "type": "string"
         },
         "dialect": {
-            "description": "Table Dialect",
+            "description": "The CSV dialect descriptor.",
             "examples": [
                 "{\n  \"dialect\": {\n    \"delimiter\": \";\"\n  }\n}\n",
                 "{\n  \"dialect\": {\n    \"delimiter\": \"\\t\",\n    \"quoteChar\": \"'\",\n    \"commentChar\": \"#\"\n  }\n}\n"
             ],
             "properties": {
                 "caseSensitiveHeader": {
                     "context": "Use of case in source CSV files is not always an intentional decision. For example, should \"CAT\" and \"Cat\" be considered to have the same meaning.",
@@ -64,14 +64,23 @@
                     "description": "Specifies that any row beginning with this one-character string, without preceeding whitespace, causes the entire line to be ignored.",
                     "examples": [
                         "{\n  \"commentChar\": \"#\"\n}\n"
                     ],
                     "title": "Comment Character",
                     "type": "string"
                 },
+                "csvddfVersion": {
+                    "default": 1.2,
+                    "description": "A number to indicate the schema version of CSV Dialect. Version 1.0 was named CSV Dialect Description Format and used different field names.",
+                    "examples:": [
+                        "{\n  \"csvddfVersion\": \"1.2\"\n}\n"
+                    ],
+                    "title": "CSV Dialect schema version",
+                    "type": "number"
+                },
                 "delimiter": {
                     "default": ",",
                     "description": "A character sequence to use as the field separator.",
                     "examples": [
                         "{\n  \"delimiter\": \",\"\n}\n",
                         "{\n  \"delimiter\": \";\"\n}\n"
                     ],
@@ -139,15 +148,15 @@
                         "{\n  \"skipInitialSpace\": true\n}\n"
                     ],
                     "title": "Skip Initial Space",
                     "type": "boolean"
                 }
             },
             "propertyOrder": 50,
-            "title": "Table Dialect",
+            "title": "CSV Dialect",
             "type": [
                 "string",
                 "object"
             ]
         },
         "encoding": {
             "default": "utf-8",
@@ -314,15 +323,14 @@
                 }
             ],
             "propertyOrder": 30,
             "title": "Path"
         },
         "profile": {
             "context": "Every Package and Resource descriptor has a profile. The default profile, if none is declared, is `data-package` for Package and `data-resource` for Resource.",
-            "default": "data-resource",
             "description": "The profile of this descriptor.",
             "examples": [
                 "{\n  \"profile\": \"tabular-data-package\"\n}\n",
                 "{\n  \"profile\": \"http://example.com/my-profiles-json-schema.json\"\n}\n"
             ],
             "propertyOrder": 10,
             "title": "Profile",
@@ -2061,10 +2069,10 @@
                 "{\n  \"title\": \"My Package Title\"\n}\n"
             ],
             "propertyOrder": 50,
             "title": "Title",
             "type": "string"
         }
     },
-    "title": "Data Resource",
+    "title": "Tabular Data Resource",
     "type": "object"
 }
```

### Comparing `dplib_py-0.6.0/dplib/profiles/table-dialect.json` & `dplib_py-0.7.0/dplib/profiles/1.0/tabledialect.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5757575757575758%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'description'": "'The CSV dialect descriptor.'",*

 * * "'properties'": "{'csvddfVersion': OrderedDict([('title', 'CSV Dialect schema version'), "*

 * *                 "('description', 'A number to indicate the schema version of CSV Dialect. Version "*

 * *                 "1.0 was named CSV Dialect Description Format and used different field names.'), "*

 * *                 "('type', 'number'), ('default', 1.2), ('examples:', ['{\\n  "*

 * *                 '"csvddfVers […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "$schema": "http://json-schema.org/draft-04/schema#",
-    "description": "Table Dialect",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "description": "The CSV dialect descriptor.",
     "examples": [
         "{\n  \"dialect\": {\n    \"delimiter\": \";\"\n  }\n}\n",
         "{\n  \"dialect\": {\n    \"delimiter\": \"\\t\",\n    \"quoteChar\": \"'\",\n    \"commentChar\": \"#\"\n  }\n}\n"
     ],
     "properties": {
         "caseSensitiveHeader": {
             "context": "Use of case in source CSV files is not always an intentional decision. For example, should \"CAT\" and \"Cat\" be considered to have the same meaning.",
@@ -20,14 +20,23 @@
             "description": "Specifies that any row beginning with this one-character string, without preceeding whitespace, causes the entire line to be ignored.",
             "examples": [
                 "{\n  \"commentChar\": \"#\"\n}\n"
             ],
             "title": "Comment Character",
             "type": "string"
         },
+        "csvddfVersion": {
+            "default": 1.2,
+            "description": "A number to indicate the schema version of CSV Dialect. Version 1.0 was named CSV Dialect Description Format and used different field names.",
+            "examples:": [
+                "{\n  \"csvddfVersion\": \"1.2\"\n}\n"
+            ],
+            "title": "CSV Dialect schema version",
+            "type": "number"
+        },
         "delimiter": {
             "default": ",",
             "description": "A character sequence to use as the field separator.",
             "examples": [
                 "{\n  \"delimiter\": \",\"\n}\n",
                 "{\n  \"delimiter\": \";\"\n}\n"
             ],
@@ -94,12 +103,9 @@
             "examples": [
                 "{\n  \"skipInitialSpace\": true\n}\n"
             ],
             "title": "Skip Initial Space",
             "type": "boolean"
         }
     },
-    "title": "Table Dialect",
-    "type": [
-        "object"
-    ]
+    "title": "CSV Dialect"
 }
```

### Comparing `dplib_py-0.6.0/dplib/profiles/table-schema.json` & `dplib_py-0.7.0/dplib/profiles/1.0/tableschema.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7857142857142857%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'", 'delete': "['type']"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$schema": "http://json-schema.org/draft-04/schema#",
+    "$schema": "http://json-schema.org/draft-07/schema#",
     "description": "A Table Schema for this resource, compliant with the [Table Schema](/tableschema/) specification.",
     "examples": [
         "{\n  \"schema\": {\n    \"fields\": [\n      {\n        \"name\": \"first_name\",\n        \"type\": \"string\"\n        \"constraints\": {\n          \"required\": true\n        }\n      },\n      {\n        \"name\": \"age\",\n        \"type\": \"integer\"\n      },\n    ],\n    \"primaryKey\": [\n      \"name\"\n    ]\n  }\n}\n"
     ],
     "properties": {
         "fields": {
             "description": "An `array` of Table Schema Field objects.",
@@ -1664,13 +1664,9 @@
                 }
             ]
         }
     },
     "required": [
         "fields"
     ],
-    "title": "Table Schema",
-    "type": [
-        "string",
-        "object"
-    ]
+    "title": "Table Schema"
 }
```

### Comparing `dplib_py-0.6.0/.gitignore` & `dplib_py-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/LICENSE.md` & `dplib_py-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dplib_py-0.6.0/pyproject.toml` & `dplib_py-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,54 +24,53 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "pyyaml>=5.0",
     "pydantic>=2.0",
     "jsonpath>=0.80",
     "jsonschema>=3.0",
     "python-slugify>=6.0",
     "fsspec[http]>=2023.1.0",
     "typing-extensions>=4.0",
 ]
 
 [project.optional-dependencies]
-cli = ["typer[all]>=0.9", "rich>=10.0"]
+cli = ["typer>=0.12", "rich>=10.0"]
 dcat = ["rdflib>=6.0"]
 pandas = ["pandas>=1.0", "pandas-stubs>=1.0", "numpy>=1.0", "isodate>=0.6"]
 polars = ["polars-lts-cpu>=0.10"]
 sql = ["sqlalchemy>=1.4"]
 dev = [
     "moto",
     "ruff",
     "httpx",
     "hatch",
-    "isort",
-    "black",
     "yattag",
     "neovim",
     "pytest",
     "mkdocs",
     "pyright",
     "ipython",
     "pytest-cov",
     "pytest-vcr",
     "pytest-mock",
     "pytest-only",
     "oauth2client",
     "requests-mock",
     "pytest-dotenv",
     "pytest-timeout",
-    "pytest-lazy-fixture",
+    "pytest-lazy-fixtures",
     "mkdocstrings[python]",
     "mkdocs-material",
 ]
 
 [project.scripts]
 dp = "dplib.plugins.cli.__main__:program"
 
@@ -87,80 +86,77 @@
   "dplib-py[cli,dcat,sql,pandas,polars,dev]",
 ]
 
 [tool.hatch.envs.default.scripts]
 coverage = [
   "sensible-browser coverage/index.html",
 ]
-build = [
+docs = [
+  "mkdocs serve",
+]
+docs-build = [
   "mkdocs build",
 ]
 format = [
-  "ruff dplib --fix",
-  "isort dplib",
-  "black dplib",
+  "ruff check --fix",
+  "ruff format dplib",
 ]
 lint = [
-  "ruff dplib",
-  "isort dplib --check",
-  "black dplib --check",
+  "ruff check dplib",
 ]
 release = [
   """
   VERSION=$(hatch run version)
   git checkout main && git pull origin && git fetch -p
   git log --pretty=format:"%C(yellow)%h%Creset %s%Cgreen%d" --reverse -20
   echo "\nReleasing v$VERSION in 10 seconds. Press <CTRL+C> to abort\n" && sleep 10
   hatch run test && git commit -a -m "v$VERSION" && git tag -a "v$VERSION" -m "v$VERSION"
   git push --follow-tags
   """
 ]
-serve = [
-  "mkdocs serve",
-]
 spec = [
   "pytest --cov dplib --cov-report term-missing --cov-report html:coverage --cov-fail-under 0 --timeout=300",
 ]
 test = [
-  "hatch run lint",
-  "hatch run type",
-  "hatch run spec",
+  "lint",
+  "type",
+  "spec",
 ]
 type = [
   "pyright dplib",
 ]
 version = [
   "hatch --no-color version"
 ]
 
 [[tool.hatch.envs.ci.matrix]]
-python = ["3.8", "3.9", "3.10"]
+python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.ci.scripts]
-test = [
-  "hatch run lint",
+spec = [
   "pytest --cov dplib --cov-report term-missing --cov-report xml --cov-fail-under 0 --timeout=300 --ci",
 ]
+test = [
+  "lint",
+  "type",
+  "spec",
+]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
-[tool.black]
-line-length = 90
-
-[tool.isort]
-profile = "black"
-multi_line_output = 9
-
 [tool.ruff]
 line-length = 90
+
+[tool.ruff.lint]
 ignore = ["E501", "E731", "F405"]
+extend-select = ["I"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
 
 [tool.pytest.ini_options]
 testpaths = ["dplib"]
 env_files = [".env"]
 markers = [
     "ci: integrational tests (select with '--ci')",
```

### Comparing `dplib_py-0.6.0/PKG-INFO` & `dplib_py-0.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dplib-py
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python implementation of the Data Package standard
 Project-URL: homepage, https://github.com/frictionlessdata/dplib-py
 Author-email: Open Knowledge Foundation <info@okfn.org>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: data package,data validation,json schema,json table schema,open data,tabular data package
 Classifier: Development Status :: 4 - Beta
@@ -13,45 +13,44 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: fsspec[http]>=2023.1.0
 Requires-Dist: jsonpath>=0.80
 Requires-Dist: jsonschema>=3.0
 Requires-Dist: pydantic>=2.0
 Requires-Dist: python-slugify>=6.0
 Requires-Dist: pyyaml>=5.0
 Requires-Dist: typing-extensions>=4.0
 Provides-Extra: cli
 Requires-Dist: rich>=10.0; extra == 'cli'
-Requires-Dist: typer[all]>=0.9; extra == 'cli'
+Requires-Dist: typer>=0.12; extra == 'cli'
 Provides-Extra: dcat
 Requires-Dist: rdflib>=6.0; extra == 'dcat'
 Provides-Extra: dev
-Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: httpx; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
-Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mkdocs; extra == 'dev'
 Requires-Dist: mkdocs-material; extra == 'dev'
 Requires-Dist: mkdocstrings[python]; extra == 'dev'
 Requires-Dist: moto; extra == 'dev'
 Requires-Dist: neovim; extra == 'dev'
 Requires-Dist: oauth2client; extra == 'dev'
 Requires-Dist: pyright; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-dotenv; extra == 'dev'
-Requires-Dist: pytest-lazy-fixture; extra == 'dev'
+Requires-Dist: pytest-lazy-fixtures; extra == 'dev'
 Requires-Dist: pytest-mock; extra == 'dev'
 Requires-Dist: pytest-only; extra == 'dev'
 Requires-Dist: pytest-timeout; extra == 'dev'
 Requires-Dist: pytest-vcr; extra == 'dev'
 Requires-Dist: requests-mock; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: yattag; extra == 'dev'
@@ -69,18 +68,19 @@
 # Data Package Library
 
 [![Build](https://img.shields.io/github/actions/workflow/status/frictionlessdata/dplib-py/general.yaml?branch=main)](https://github.com/frictionlessdata/dplib-py/actions)
 [![Coverage](https://img.shields.io/codecov/c/github/frictionlessdata/dplib-py/main)](https://codecov.io/gh/frictionlessdata/dplib-py)
 [![Codebase](https://img.shields.io/badge/codebase-github-brightgreen)](https://github.com/frictionlessdata/dplib-py)
 [![Release](https://img.shields.io/pypi/v/dplib-py.svg)](https://pypi.python.org/pypi/dplib-py)
 
-Python implementation of the Data Package standard and various tools for working with data.
+Python implementation of the Data Package standard and various tools for working with data. For more information, please visit the [documentation portal](https://frictionlessdata.github.io/dplib-py).
 
 ## Purpose
 
 The Data Package Library is a lightweight Data Package Standard implementation in Python providing Pydantic data models and various metadata converters. At the moment, the main purpose of this library is to be used as an underlying component of Data Package based integrations.
 
-## Documentation
+## Funding
 
-Please visit the documentation portal:
+This project is funded through [NGI0 Entrust](https://nlnet.nl/entrust), a fund established by [NLnet](https://nlnet.nl) with financial support from the European Commission's [Next Generation Internet](https://ngi.eu) program. Learn more at the [NLnet project page](https://nlnet.nl/project/FrictionlessStandards/).
 
-- https://frictionlessdata.github.io/dplib-py/
+[<img src="https://nlnet.nl/logo/banner.png" alt="NLnet foundation logo" width="20%" />](https://nlnet.nl)
+[<img src="https://nlnet.nl/image/logos/NGI0_tag.svg" alt="NGI Zero Logo" width="20%" />](https://nlnet.nl/entrust)
```

