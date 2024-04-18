# Comparing `tmp/collective.volto.formsupport-2.7.0.tar.gz` & `tmp/collective.volto.formsupport-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.volto.formsupport-2.7.0.tar", last modified: Mon Apr  3 07:07:32 2023, max compression
+gzip compressed data, was "collective.volto.formsupport-3.0.1.tar", last modified: Thu Apr 18 08:04:53 2024, max compression
```

## Comparing `collective.volto.formsupport-2.7.0.tar` & `collective.volto.formsupport-3.0.1.tar`

### file list

```diff
@@ -1,115 +1,140 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.070009 collective.volto.formsupport-2.7.0/
--rw-r--r--   0 cekk       (501) staff       (20)     2479 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)      109 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      679 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      117 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)    15956 2023-04-03 07:07:32.070258 collective.volto.formsupport-2.7.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     8827 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.049517 collective.volto.formsupport-2.7.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7947 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)      107 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)       42 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      543 2023-04-03 07:07:32.070907 collective.volto.formsupport-2.7.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2991 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.042698 collective.volto.formsupport-2.7.0/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.049762 collective.volto.formsupport-2.7.0/src/collective/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.052051 collective.volto.formsupport-2.7.0/src/collective/volto/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.054487 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/
--rw-r--r--   0 cekk       (501) staff       (20)      198 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.055264 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      781 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/browser/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.055559 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/browser/overrides/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/browser/overrides/.gitkeep
--rw-r--r--   0 cekk       (501) staff       (20)      637 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/browser/send_mail_template.pt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.055775 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/browser/static/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/browser/static/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.057549 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/
--rw-r--r--   0 cekk       (501) staff       (20)      288 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1648 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     2221 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/hcaptcha.py
--rw-r--r--   0 cekk       (501) staff       (20)     1467 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/honeypot.py
--rw-r--r--   0 cekk       (501) staff       (20)     2346 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/norobots.py
--rw-r--r--   0 cekk       (501) staff       (20)     2087 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/recaptcha.py
--rw-r--r--   0 cekk       (501) staff       (20)      597 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/vocabularies.py
--rw-r--r--   0 cekk       (501) staff       (20)     1543 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.058334 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/datamanager/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/datamanager/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3531 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/datamanager/catalog.py
--rw-r--r--   0 cekk       (501) staff       (20)      610 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/datamanager/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1030 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.059575 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3315 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/collective.volto.formsupport.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.044210 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.060323 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1443 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.mo
--rw-r--r--   0 cekk       (501) staff       (20)     3759 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.044448 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/pt_BR/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.060909 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1499 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.mo
--rw-r--r--   0 cekk       (501) staff       (20)     3794 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.po
--rw-r--r--   0 cekk       (501) staff       (20)     1778 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      521 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      260 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.044983 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.062012 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      209 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      195 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/profiles/default/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.062294 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/profiles/default/registry/
--rw-r--r--   0 cekk       (501) staff       (20)      186 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/profiles/default/registry/main.xml
--rw-r--r--   0 cekk       (501) staff       (20)      118 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.062644 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      138 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.063178 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      230 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.063985 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/serializer/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/serializer/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1963 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/serializer/blocks.py
--rw-r--r--   0 cekk       (501) staff       (20)      416 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/serializer/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.064490 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      192 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.065864 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/form_data/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/form_data/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      529 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/form_data/clear.py
--rw-r--r--   0 cekk       (501) staff       (20)     1049 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/form_data/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     3450 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/form_data/csv.py
--rw-r--r--   0 cekk       (501) staff       (20)     2570 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/form_data/form_data.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.066659 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/submit_form/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/submit_form/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      424 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/submit_form/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)    12002 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/submit_form/post.py
--rw-r--r--   0 cekk       (501) staff       (20)      628 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     2669 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.069739 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)    74429 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/file.pdf
--rw-r--r--   0 cekk       (501) staff       (20)    14321 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_captcha.py
--rw-r--r--   0 cekk       (501) staff       (20)     4306 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_event.py
--rw-r--r--   0 cekk       (501) staff       (20)     9637 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_honeypot.py
--rw-r--r--   0 cekk       (501) staff       (20)    16806 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_send_action_form.py
--rw-r--r--   0 cekk       (501) staff       (20)     8923 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_serialize_block.py
--rw-r--r--   0 cekk       (501) staff       (20)     2628 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)     8745 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_store_action_form.py
--rw-r--r--   0 cekk       (501) staff       (20)     6216 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/upgrades.py
--rw-r--r--   0 cekk       (501) staff       (20)      668 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/upgrades.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1090 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/utils.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-03 07:07:32.051805 collective.volto.formsupport-2.7.0/src/collective.volto.formsupport.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)    15956 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective.volto.formsupport.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     4512 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective.volto.formsupport.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective.volto.formsupport.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      153 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective.volto.formsupport.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       28 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective.volto.formsupport.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective.volto.formsupport.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      473 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective.volto.formsupport.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2023-04-03 07:07:31.000000 collective.volto.formsupport-2.7.0/src/collective.volto.formsupport.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.666070 collective.volto.formsupport-3.0.1/
+-rw-r--r--   0 cekk       (501) staff       (20)     3927 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      109 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      679 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      117 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)    18224 2024-04-18 08:04:53.666143 collective.volto.formsupport-3.0.1/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)    12962 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/constraints_plone52.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       62 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/constraints_plone60.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.656347 collective.volto.formsupport-3.0.1/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7947 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)      107 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       29 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      334 2024-04-18 08:04:53.666377 collective.volto.formsupport-3.0.1/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     3118 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.652823 collective.volto.formsupport-3.0.1/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.656467 collective.volto.formsupport-3.0.1/src/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.657472 collective.volto.formsupport-3.0.1/src/collective/volto/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.658457 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/
+-rw-r--r--   0 cekk       (501) staff       (20)      197 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.658970 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1233 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      452 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/email_confirm_view.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.659078 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/overrides/.gitkeep
+-rw-r--r--   0 cekk       (501) staff       (20)      655 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/send_mail_template.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1061 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/send_mail_template_table.pt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.659171 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/static/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.659264 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)     9564 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/templates/email_confirm_view.pt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.659999 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/
+-rw-r--r--   0 cekk       (501) staff       (20)      288 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1626 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2224 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/hcaptcha.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1469 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/honeypot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2271 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/norobots.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2089 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/recaptcha.py
+-rw-r--r--   0 cekk       (501) staff       (20)      564 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/vocabularies.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1548 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.660334 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3832 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/catalog.py
+-rw-r--r--   0 cekk       (501) staff       (20)      595 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1030 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.660887 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5016 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/collective.volto.formsupport.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.653514 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/de/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.661122 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/de/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1654 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     5637 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.653635 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/es/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.661348 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/es/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     2375 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     6167 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.653745 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.661580 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     3102 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     6160 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.653852 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.661810 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1499 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     5495 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1778 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      521 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      273 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.654095 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.662245 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      209 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      195 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.662357 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)      186 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/registry/main.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.662469 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      138 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.662670 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      272 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.662969 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/deserializer/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/deserializer/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1301 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/deserializer/blocks.py
+-rw-r--r--   0 cekk       (501) staff       (20)      426 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/deserializer/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.663277 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/serializer/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/serializer/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1900 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/serializer/blocks.py
+-rw-r--r--   0 cekk       (501) staff       (20)      449 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/serializer/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.663476 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      233 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.663994 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      942 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/clear.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1118 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3451 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/csv.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3930 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/form_data.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.664318 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/submit_form/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/submit_form/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      443 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/submit_form/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)    18588 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/submit_form/post.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.664646 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      689 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2801 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/email.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.664845 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/scripts/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/scripts/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2538 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/scripts/cleansing.py
+-rw-r--r--   0 cekk       (501) staff       (20)      628 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2827 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.665948 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)    74429 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/file.pdf
+-rw-r--r--   0 cekk       (501) staff       (20)    16091 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_captcha.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2439 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_deserialize_block.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4504 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_event.py
+-rw-r--r--   0 cekk       (501) staff       (20)    11327 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_honeypot.py
+-rw-r--r--   0 cekk       (501) staff       (20)    46978 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_send_action_form.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8854 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_serialize_block.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3207 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)    11064 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_store_action_form.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8193 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)      940 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/upgrades.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1695 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/utils.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-18 08:04:53.657369 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)    18224 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     5683 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      214 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       28 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      493 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2024-04-18 08:04:53.000000 collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/top_level.txt
```

### Comparing `collective.volto.formsupport-2.7.0/DEVELOP.rst` & `collective.volto.formsupport-3.0.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-2.7.0/LICENSE.GPL` & `collective.volto.formsupport-3.0.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-2.7.0/LICENSE.rst` & `collective.volto.formsupport-3.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-2.7.0/docs/conf.py` & `collective.volto.formsupport-3.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-2.7.0/setup.py` & `collective.volto.formsupport-3.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.volto.formsupport",
-    version="2.7.0",
+    version="3.0.1",
     description="Add support for customizable forms in Volto",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -48,17 +48,19 @@
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.6",
     install_requires=[
         "setuptools",
         "z3c.jbot",
         "plone.api>=1.8.4",
-        "plone.restapi",
+        "plone.restapi>=8.36.0",
         "plone.app.dexterity",
         "souper.plone",
+        "click",
+        "pyotp",
     ],
     extras_require={
         "hcaptcha": [
             "plone.formwidget.hcaptcha>=1.0.1",
         ],
         "recaptcha": [
             "plone.formwidget.recaptcha",
@@ -85,9 +87,10 @@
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     [console_scripts]
     update_locale = collective.volto.formsupport.locales.update:update_locale
+    formsupport_data_cleansing = collective.volto.formsupport.scripts.cleansing:main
     """,
 )
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/browser/send_mail_template.pt` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/browser/send_mail_template.pt`

 * *Files 23% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 00000090: 6765 7428 2770 6172 616d 6574 6572 7327  get('parameters'
 000000a0: 2c20 7b7d 293b 0a20 2020 2020 2020 2020  , {});.         
 000000b0: 2020 2075 726c 2070 7974 686f 6e3a 6f70     url python:op
 000000c0: 7469 6f6e 732e 6765 7428 2775 726c 272c  tions.get('url',
 000000d0: 2027 2729 3b0a 2020 2020 2020 2020 2020   '');.          
 000000e0: 2020 7469 746c 6520 7079 7468 6f6e 3a6f    title python:o
 000000f0: 7074 696f 6e73 2e67 6574 2827 7469 746c  ptions.get('titl
-00000100: 6527 2c20 2727 293b 223e 0a20 203c 7020  e', '');">.  <p 
-00000110: 6931 386e 3a74 7261 6e73 6c61 7465 3d22  i18n:translate="
-00000120: 7365 6e64 5f6d 6169 6c5f 7465 7874 223e  send_mail_text">
-00000130: 0a20 2020 2041 206e 6577 2066 6f72 6d20  .    A new form 
-00000140: 6861 7320 6265 656e 2073 7562 6d69 7474  has been submitt
-00000150: 6564 2066 726f 6d20 3c73 7472 6f6e 6720  ed from <strong 
-00000160: 6931 386e 3a6e 616d 653d 2275 726c 223e  i18n:name="url">
-00000170: 247b 7469 746c 657d 3c2f 7374 726f 6e67  ${title}</strong
-00000180: 3e3a 0a20 203c 2f70 3e0a 2020 3c75 6c3e  >:.  </p>.  <ul>
-00000190: 0a20 2020 203c 7461 6c3a 6669 656c 6420  .    <tal:field 
-000001a0: 7265 7065 6174 3d22 6669 656c 6420 7061  repeat="field pa
-000001b0: 7261 6d65 7465 7273 223e 0a20 2020 2020  rameters">.     
-000001c0: 203c 6c69 2074 616c 3a64 6566 696e 653d   <li tal:define=
-000001d0: 2276 616c 7565 2066 6965 6c64 2f76 616c  "value field/val
-000001e0: 7565 7c6e 6f74 6869 6e67 3b0a 2020 2020  ue|nothing;.    
-000001f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000200: 2020 6c61 6265 6c20 6669 656c 642f 6c61    label field/la
-00000210: 6265 6c7c 6e6f 7468 696e 6722 3e0a 2020  bel|nothing">.  
-00000220: 2020 2020 2020 2020 3c73 7472 6f6e 673e          <strong>
-00000230: 247b 6c61 6265 6c7d 3a3c 2f73 7472 6f6e  ${label}:</stron
-00000240: 673e 2024 7b76 616c 7565 7d0a 2020 2020  g> ${value}.    
-00000250: 2020 3c2f 6c69 3e0a 2020 2020 3c2f 7461    </li>.    </ta
-00000260: 6c3a 6669 656c 643e 0a20 203c 2f75 6c3e  l:field>.  </ul>
-00000270: 0a3c 2f74 616c 3a72 6f6f 743e 0a         .</tal:root>.
+00000100: 6527 2c20 2727 293b 223e 0a20 203c 756c  e', '');">.  <ul
+00000110: 3e0a 2020 2020 3c74 616c 3a66 6965 6c64  >.    <tal:field
+00000120: 2072 6570 6561 743d 2266 6965 6c64 2070   repeat="field p
+00000130: 6172 616d 6574 6572 7322 3e0a 2020 2020  arameters">.    
+00000140: 2020 3c6c 6920 7461 6c3a 6465 6669 6e65    <li tal:define
+00000150: 3d22 7661 6c75 6520 6669 656c 642f 7661  ="value field/va
+00000160: 6c75 657c 6e6f 7468 696e 673b 0a20 2020  lue|nothing;.   
+00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000180: 2020 206c 6162 656c 2066 6965 6c64 2f6c     label field/l
+00000190: 6162 656c 7c6e 6f74 6869 6e67 223e 0a20  abel|nothing">. 
+000001a0: 2020 2020 2020 2020 203c 7374 726f 6e67           <strong
+000001b0: 3e24 7b6c 6162 656c 7d3a 3c2f 7374 726f  >${label}:</stro
+000001c0: 6e67 3e20 247b 7661 6c75 657d 0a20 2020  ng> ${value}.   
+000001d0: 2020 203c 2f6c 693e 0a20 2020 203c 2f74     </li>.    </t
+000001e0: 616c 3a66 6965 6c64 3e0a 2020 3c2f 756c  al:field>.  </ul
+000001f0: 3e0a 2020 3c70 2069 3138 6e3a 7472 616e  >.  <p i18n:tran
+00000200: 736c 6174 653d 2273 656e 645f 6d61 696c  slate="send_mail
+00000210: 5f74 6578 7422 3e0a 2020 2020 4120 6e65  _text">.    A ne
+00000220: 7720 666f 726d 2068 6173 2062 6565 6e20  w form has been 
+00000230: 7375 626d 6974 7465 6420 6672 6f6d 203c  submitted from <
+00000240: 6120 6872 6566 3d22 247b 7572 6c7d 223e  a href="${url}">
+00000250: 3c73 7472 6f6e 6720 6931 386e 3a6e 616d  <strong i18n:nam
+00000260: 653d 2275 726c 223e 247b 7572 6c7d 3c2f  e="url">${url}</
+00000270: 7374 726f 6e67 3e3c 2f61 3e0a 2020 3c2f  strong></a>.  </
+00000280: 703e 0a3c 2f74 616c 3a72 6f6f 743e 0a    p>.</tal:root>.
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/configure.zcml` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/configure.zcml`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:zcml="http://namespaces.zope.org/zcml">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
 
-    <adapter
-        zcml:condition="installed plone.formwidget.hcaptcha"
-        factory=".hcaptcha.HCaptchaSupport"
-        provides="..interfaces.ICaptchaSupport"
-        for="* zope.publisher.interfaces.browser.IBrowserRequest"
-        name="hcaptcha"
-        />
-
-    <adapter
-        zcml:condition="installed plone.formwidget.hcaptcha"
-        factory=".hcaptcha.HCaptchaInvisibleSupport"
-        provides="..interfaces.ICaptchaSupport"
-        for="* zope.publisher.interfaces.browser.IBrowserRequest"
-        name="hcaptcha_invisible"
-        />
-
-    <adapter
-        zcml:condition="installed plone.formwidget.recaptcha"
-        factory=".recaptcha.RecaptchaSupport"
-        provides="..interfaces.ICaptchaSupport"
-        for="* zope.publisher.interfaces.browser.IBrowserRequest"
-        name="recaptcha"
-        />
-
-    <adapter
-        zcml:condition="installed collective.z3cform.norobots"
-        factory=".norobots.NoRobotsSupport"
-        provides="..interfaces.ICaptchaSupport"
-        for="* zope.publisher.interfaces.browser.IBrowserRequest"
-        name="norobots-captcha"
-        />
-    
-    <adapter
-        zcml:condition="installed collective.honeypot"
-        factory=".honeypot.HoneypotSupport"
-        provides="..interfaces.ICaptchaSupport"
-        for="* zope.publisher.interfaces.browser.IBrowserRequest"
-        name="honeypot"
-        />
-
-    <utility
-        name="collective.volto.formsupport.captcha.providers"
-        component=".vocabularies.captcha_providers_vocabulary_factory"
-        />
+  <adapter
+      factory=".hcaptcha.HCaptchaSupport"
+      provides="..interfaces.ICaptchaSupport"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest"
+      name="hcaptcha"
+      zcml:condition="installed plone.formwidget.hcaptcha"
+      />
+
+  <adapter
+      factory=".hcaptcha.HCaptchaInvisibleSupport"
+      provides="..interfaces.ICaptchaSupport"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest"
+      name="hcaptcha_invisible"
+      zcml:condition="installed plone.formwidget.hcaptcha"
+      />
+
+  <adapter
+      factory=".recaptcha.RecaptchaSupport"
+      provides="..interfaces.ICaptchaSupport"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest"
+      name="recaptcha"
+      zcml:condition="installed plone.formwidget.recaptcha"
+      />
+
+  <adapter
+      factory=".norobots.NoRobotsSupport"
+      provides="..interfaces.ICaptchaSupport"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest"
+      name="norobots-captcha"
+      zcml:condition="installed collective.z3cform.norobots"
+      />
+
+  <adapter
+      factory=".honeypot.HoneypotSupport"
+      provides="..interfaces.ICaptchaSupport"
+      for="*
+           zope.publisher.interfaces.browser.IBrowserRequest"
+      name="honeypot"
+      zcml:condition="installed collective.honeypot"
+      />
+
+  <utility
+      name="collective.volto.formsupport.captcha.providers"
+      component=".vocabularies.captcha_providers_vocabulary_factory"
+      />
 
 </configure>
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/hcaptcha.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/hcaptcha.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from . import CaptchaSupport
-from collective.volto.formsupport import _
 from plone.formwidget.hcaptcha.interfaces import IHCaptchaSettings
 from plone.formwidget.hcaptcha.nohcaptcha import submit
+
 # from plone.formwidget.hcaptcha.validator import WrongCaptchaCode
 from plone.registry.interfaces import IRegistry
 from zExceptions import BadRequest
 from zope.component import queryUtility
 from zope.i18n import translate
 
+from collective.volto.formsupport import _
+
+from . import CaptchaSupport
+
 
 class HCaptchaSupport(CaptchaSupport):
     name = _("HCaptcha")
 
     def __init__(self, context, request):
         super().__init__(context, request)
         registry = queryUtility(IRegistry)
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/honeypot.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/honeypot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from . import CaptchaSupport
 from collective.honeypot.config import HONEYPOT_FIELD
 from collective.honeypot.utils import found_honeypot
-from collective.volto.formsupport import _
 from plone.restapi.deserializer import json_body
 from zExceptions import BadRequest
 from zope.i18n import translate
 
+from collective.volto.formsupport import _
+
+from . import CaptchaSupport
+
 
 class HoneypotSupport(CaptchaSupport):
     name = _("Honeypot Support")
 
     def isEnabled(self):
         """
         Honeypot is enabled with env vars
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/norobots.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/norobots.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from . import CaptchaSupport
-from collective.volto.formsupport import _
-from collective.z3cform.norobots.browser.interfaces import (
-    INorobotsWidgetSettings,
-)
+import json
+
+from collective.z3cform.norobots.browser.interfaces import INorobotsWidgetSettings
 from plone import api
 from plone.registry.interfaces import IRegistry
 from zExceptions import BadRequest
 from zope.component import queryUtility
 from zope.i18n import translate
 
-import json
+from collective.volto.formsupport import _
+
+from . import CaptchaSupport
 
 
 class NoRobotsSupport(CaptchaSupport):
     name = _("NoRobots ReCaptcha Support")
 
     def __init__(self, context, request):
         super().__init__(context, request)
         registry = queryUtility(IRegistry)
-        self.settings = registry.forInterface(
-            INorobotsWidgetSettings, check=False
-        )
+        self.settings = registry.forInterface(INorobotsWidgetSettings, check=False)
 
     def isEnabled(self):
         return self.settings and self.settings.questions
 
     def serialize(self):
         if not self.settings.questions:
             raise ValueError(
@@ -62,13 +60,11 @@
         value = json_token.get("value")
         id = json_token.get("id")
         id_check = json_token.get("id_check")
 
         if not view.verify(input=value, question_id=id, id_check=id_check):
             raise BadRequest(
                 translate(
-                    _(
-                        "The code you entered was wrong, please enter the new one."
-                    ),
+                    _("The code you entered was wrong, please enter the new one."),
                     context=self.request,
                 )
             )
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/recaptcha.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/recaptcha.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from . import CaptchaSupport
-from collective.volto.formsupport import _
 from plone.formwidget.recaptcha.interfaces import IReCaptchaSettings
 from plone.formwidget.recaptcha.norecaptcha import submit
 from plone.registry.interfaces import IRegistry
 from zExceptions import BadRequest
 from zope.component import queryUtility
 from zope.i18n import translate
 
+from collective.volto.formsupport import _
+
+from . import CaptchaSupport
+
 
 class RecaptchaSupport(CaptchaSupport):
     name = _("Google ReCaptcha")
 
     def __init__(self, context, request):
         super().__init__(context, request)
         registry = queryUtility(IRegistry)
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/captcha/vocabularies.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/captcha/vocabularies.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from ..interfaces import ICaptchaSupport
 from zope.component import getAdapters
 from zope.interface import provider
 from zope.schema.interfaces import IVocabularyFactory
-from zope.schema.vocabulary import SimpleTerm
-from zope.schema.vocabulary import SimpleVocabulary
+from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
+
+from ..interfaces import ICaptchaSupport
 
 
 @provider(IVocabularyFactory)
 def captcha_providers_vocabulary_factory(context):
     terms = []
     for name, adapter in getAdapters((context, context.REQUEST), ICaptchaSupport):
         if adapter.isEnabled():
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/configure.zcml` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/configure.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:plone="http://namespaces.plone.org/plone"
-    i18n_domain="collective.volto.formsupport">
+    i18n_domain="collective.volto.formsupport"
+    >
 
   <i18n:registerTranslations directory="locales" />
 
   <!--
     Be careful if you use general includeDependencies, it can have side effects!
     Better import explicit packages or configurations ;)
   -->
@@ -22,26 +23,26 @@
 
   <include file="permissions.zcml" />
   <include file="upgrades.zcml" />
 
   <genericsetup:registerProfile
       name="default"
       title="Volto: Form support"
-      directory="profiles/default"
       description="Installs the collective.volto.formsupport add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/default"
       post_handler=".setuphandlers.post_install"
       />
 
   <genericsetup:registerProfile
       name="uninstall"
       title="Volto: Form support (uninstall)"
-      directory="profiles/uninstall"
       description="Uninstalls the collective.volto.formsupport add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/uninstall"
       post_handler=".setuphandlers.uninstall"
       />
 
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="collective.volto.formsupport-hiddenprofiles"
       />
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/datamanager/catalog.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/catalog.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 
-from collective.volto.formsupport import logger
-from collective.volto.formsupport.interfaces import IFormDataStore
-from collective.volto.formsupport.utils import get_blocks
 from copy import deepcopy
 from datetime import datetime
+
 from plone.dexterity.interfaces import IDexterityContent
 from plone.restapi.deserializer import json_body
 from repoze.catalog.catalog import Catalog
 from repoze.catalog.indexes.field import CatalogFieldIndex
 from souper.interfaces import ICatalogFactory
-from souper.soup import get_soup
-from souper.soup import NodeAttributeIndexer
-from souper.soup import Record
+from souper.soup import NodeAttributeIndexer, Record, get_soup
 from zope.component import adapter
-from zope.interface import implementer
-from zope.interface import Interface
+from zope.interface import Interface, implementer
+
+from collective.volto.formsupport import logger
+from collective.volto.formsupport.interfaces import IFormDataStore
+from collective.volto.formsupport.utils import get_blocks
 
 
 @implementer(ICatalogFactory)
 class FormDataSoupCatalogFactory(object):
     def __call__(self, context):
         #  do not set any index here..maybe on each form
         catalog = Catalog()
@@ -56,27 +55,38 @@
             if id != self.block_id:
                 continue
             block_type = block.get("@type", "")
             if block_type == "form":
                 form_block = deepcopy(block)
         if not form_block:
             return {}
-        return form_block.get("subblocks", [])
+
+        subblocks = form_block.get("subblocks", [])
+
+        # Add the 'custom_field_id' field back in as this isn't stored with each subblock
+        for index, field in enumerate(subblocks):
+            if form_block.get(field["field_id"]):
+                subblocks[index]["custom_field_id"] = form_block.get(field["field_id"])
+
+        return subblocks
 
     def add(self, data):
         form_fields = self.get_form_fields()
         if not form_fields:
             logger.error(
                 'Block with id {} and type "form" not found in context: {}.'.format(
                     self.block_id, self.context.absolute_url()
                 )
             )
             return None
 
-        fields = {x["field_id"]: x.get("label", x["field_id"]) for x in form_fields}
+        fields = {
+            x["field_id"]: x.get("custom_field_id", x.get("label", x["field_id"]))
+            for x in form_fields
+        }
         record = Record()
         fields_labels = {}
         fields_order = []
         for field_data in data:
             field_id = field_data.get("field_id", "")
             value = field_data.get("value", "")
             if field_id in fields:
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/datamanager/configure.zcml` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/datamanager/configure.zcml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:plone="http://namespaces.plone.org/plone"
-    i18n_domain="collective.volto.formsupport">
+    i18n_domain="collective.volto.formsupport"
+    >
 
-    <!-- Enable each Dexterity content to be a soup root -->
-    <class class="plone.dexterity.content.DexterityContent">
-        <implements interface="souper.plone.interfaces.ISoupRoot" />
-    </class>
+  <!-- Enable each Dexterity content to be a soup root -->
+  <class class="plone.dexterity.content.DexterityContent">
+    <implements interface="souper.plone.interfaces.ISoupRoot" />
+  </class>
 
-    <!-- register the catalog -->
-    <utility
-        provides="souper.interfaces.ICatalogFactory"
-        factory=".catalog.FormDataSoupCatalogFactory"
-        name="form_data"
-    />
+  <!-- register the catalog -->
+  <utility
+      factory=".catalog.FormDataSoupCatalogFactory"
+      provides="souper.interfaces.ICatalogFactory"
+      name="form_data"
+      />
 
-    <adapter factory=".catalog.FormDataStore" />
+  <adapter factory=".catalog.FormDataStore" />
 </configure>
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/interfaces.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/README.rst` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/collective.volto.formsupport.pot` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/collective.volto.formsupport.pot`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,157 @@
 #--- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 #SOME DESCRIPTIVE TITLE.
 #FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-09-20 08:23+0000\n"
+"POT-Creation-Date: 2024-04-17 10:34+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: collective.volto.formsupport\n"
 
-#: collective/volto/formsupport/captcha/recaptcha.py:12
+#: collective/volto/formsupport/restapi/services/validation/email.py:55
+msgid "Email confirmation code"
+msgstr ""
+
+#: collective/volto/formsupport/captcha/recaptcha.py:14
 msgid "Google ReCaptcha"
 msgstr ""
 
-#: collective/volto/formsupport/captcha/hcaptcha.py:13
+#: collective/volto/formsupport/captcha/hcaptcha.py:16
 msgid "HCaptcha"
 msgstr ""
 
-#: collective/volto/formsupport/captcha/hcaptcha.py:62
+#: collective/volto/formsupport/captcha/hcaptcha.py:65
 msgid "HCaptcha Invisible"
 msgstr ""
 
-#: collective/volto/formsupport/configure.zcml:33
+#: collective/volto/formsupport/captcha/honeypot.py:13
+msgid "Honeypot Support"
+msgstr ""
+
+#: collective/volto/formsupport/configure.zcml:34
 msgid "Installs the collective.volto.formsupport add-on."
 msgstr ""
 
-#: collective/volto/formsupport/captcha/hcaptcha.py:43
-#: collective/volto/formsupport/captcha/norobots.py:53
-#: collective/volto/formsupport/captcha/recaptcha.py:42
+#: collective/volto/formsupport/captcha/hcaptcha.py:46
+#: collective/volto/formsupport/captcha/norobots.py:51
+#: collective/volto/formsupport/captcha/recaptcha.py:44
 msgid "No captcha token provided."
 msgstr ""
 
 #: collective/volto/formsupport/captcha/norobots.py:16
 msgid "NoRobots ReCaptcha Support"
 msgstr ""
 
-#: collective/volto/formsupport/captcha/hcaptcha.py:55
-#: collective/volto/formsupport/captcha/norobots.py:69
-#: collective/volto/formsupport/captcha/recaptcha.py:54
+#: collective/volto/formsupport/restapi/services/validation/email.py:98
+msgid "OTP is wrong"
+msgstr ""
+
+#: collective/volto/formsupport/captcha/hcaptcha.py:58
+#: collective/volto/formsupport/captcha/norobots.py:67
+#: collective/volto/formsupport/captcha/recaptcha.py:56
 msgid "The code you entered was wrong, please enter the new one."
 msgstr ""
 
-#: collective/volto/formsupport/configure.zcml:42
+#: collective/volto/formsupport/restapi/services/validation/email.py:68
+msgid "The email field is missing"
+msgstr ""
+
+#: collective/volto/formsupport/browser/templates/email_confirm_view.pt:367
+msgid "The form on ${page} was compiled with this email address, if it was not you, ignore the message."
+msgstr ""
+
+#: collective/volto/formsupport/restapi/services/validation/email.py:92
+msgid "The otp field is missing"
+msgstr ""
+
+#: collective/volto/formsupport/restapi/services/validation/email.py:71
+msgid "The provided email address is not valid"
+msgstr ""
+
+#: collective/volto/formsupport/restapi/services/validation/email.py:74
+msgid "The uid field is missing"
+msgstr ""
+
+#: collective/volto/formsupport/configure.zcml:43
 msgid "Uninstalls the collective.volto.formsupport add-on."
 msgstr ""
 
-#: collective/volto/formsupport/configure.zcml:33
+#: collective/volto/formsupport/configure.zcml:34
 msgid "Volto: Form support"
 msgstr ""
 
-#: collective/volto/formsupport/configure.zcml:42
+#: collective/volto/formsupport/configure.zcml:43
 msgid "Volto: Form support (uninstall)"
 msgstr ""
 
+#: collective/volto/formsupport/browser/templates/email_confirm_view.pt:353
+msgid "Your code to validate the email address:"
+msgstr ""
+
 #. Default: "Attachments too big. You uploaded ${uploaded_str}, but limit is ${max} MB. Try to compress files."
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:152
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:213
 msgid "attachments_too_big"
 msgstr ""
 
 #. Default: "Block with @type \"form\" and id \"$block\" not found in this context: $context"
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:93
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:128
 msgid "block_form_not_found_label"
 msgstr ""
 
 #. Default: "Empty form data."
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:119
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:154
 msgid "empty_form_data"
 msgstr ""
 
+#. Default: "Error submitting form."
+#: collective/volto/formsupport/captcha/honeypot.py:30
+msgid "honeypot_error"
+msgstr ""
+
 #. Default: "Unable to send confirm email. Please retry later or contact site administator."
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:66
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:75
 msgid "mail_send_exception"
 msgstr ""
 
 #. Default: "You need to set at least one form action between \"send\" and \"store\"."
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:108
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:143
 msgid "missing_action"
 msgstr ""
 
 #. Default: "Missing block_id"
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:86
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:121
 msgid "missing_blockid_label"
 msgstr ""
 
-#. Default: "A new form has been submitted from ${url}:"
-#: collective/volto/formsupport/browser/send_mail_template.pt:7
+#. Default: "A new form has been submitted from <a href=\"${url}\">${url}</a>"
+#: collective/volto/formsupport/browser/send_mail_template.pt:15
 msgid "send_mail_text"
 msgstr ""
 
+#. Default: "Form submission data for ${title}"
+#: collective/volto/formsupport/browser/send_mail_template_table.pt:12
+msgid "send_mail_text_table"
+msgstr ""
+
 #. Default: "Missing required field: subject or from."
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:230
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:320
 msgid "send_required_field_missing"
 msgstr ""
+
+#. Default: "Email not valid in \"${field}\" field."
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:185
+msgid "wrong_email"
+msgstr ""
+
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:244
+msgid "{email}'s OTP is wrong"
+msgstr ""
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.po` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.po`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,156 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-09-20 08:23+0000\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
+"Project-Id-Version: \n"
+"POT-Creation-Date: 2024-04-17 10:34+0000\n"
+"PO-Revision-Date: 2021-05-11 18:49-0300\n"
+"Last-Translator: Érico Andrei <ericof@plone.org>, 2021\n"
+"Language-Team: Portuguese (https://www.transifex.com/plone/teams/14552/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0\n"
-"Language-Code: en\n"
-"Language-Name: English\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"Language-Code: pt-br\n"
+"Language-Name: Português do Brasil\n"
 "Preferred-Encodings: utf-8 latin1\n"
-"Domain: DOMAIN\n"
+"Domain: collective.volto.formsupport\n"
+"Language: pt_BR\n"
+"X-Generator: Poedit 2.4.3\n"
 
-#: collective/volto/formsupport/captcha/recaptcha.py:12
+#: collective/volto/formsupport/restapi/services/validation/email.py:55
+msgid "Email confirmation code"
+msgstr ""
+
+#: collective/volto/formsupport/captcha/recaptcha.py:14
 msgid "Google ReCaptcha"
 msgstr ""
 
-#: collective/volto/formsupport/captcha/hcaptcha.py:13
+#: collective/volto/formsupport/captcha/hcaptcha.py:16
 msgid "HCaptcha"
 msgstr ""
 
-#: collective/volto/formsupport/captcha/hcaptcha.py:62
+#: collective/volto/formsupport/captcha/hcaptcha.py:65
 msgid "HCaptcha Invisible"
 msgstr ""
 
-#: collective/volto/formsupport/configure.zcml:33
-msgid "Installs the collective.volto.formsupport add-on."
+#: collective/volto/formsupport/captcha/honeypot.py:13
+msgid "Honeypot Support"
 msgstr ""
 
-#: collective/volto/formsupport/captcha/hcaptcha.py:43
-#: collective/volto/formsupport/captcha/norobots.py:53
-#: collective/volto/formsupport/captcha/recaptcha.py:42
+#: collective/volto/formsupport/configure.zcml:34
+msgid "Installs the collective.volto.formsupport add-on."
+msgstr "Instala o complemento collective.volto.formsupport."
+
+#: collective/volto/formsupport/captcha/hcaptcha.py:46
+#: collective/volto/formsupport/captcha/norobots.py:51
+#: collective/volto/formsupport/captcha/recaptcha.py:44
 msgid "No captcha token provided."
-msgstr "Nessun token captcha fornito."
+msgstr ""
 
 #: collective/volto/formsupport/captcha/norobots.py:16
 msgid "NoRobots ReCaptcha Support"
 msgstr ""
 
-#: collective/volto/formsupport/captcha/hcaptcha.py:55
-#: collective/volto/formsupport/captcha/norobots.py:69
-#: collective/volto/formsupport/captcha/recaptcha.py:54
+#: collective/volto/formsupport/restapi/services/validation/email.py:98
+msgid "OTP is wrong"
+msgstr ""
+
+#: collective/volto/formsupport/captcha/hcaptcha.py:58
+#: collective/volto/formsupport/captcha/norobots.py:67
+#: collective/volto/formsupport/captcha/recaptcha.py:56
 msgid "The code you entered was wrong, please enter the new one."
-msgstr "Il codice che hai inserito è sbagliato, per favore prova con un altro."
+msgstr ""
 
-#: collective/volto/formsupport/configure.zcml:42
-msgid "Uninstalls the collective.volto.formsupport add-on."
+#: collective/volto/formsupport/restapi/services/validation/email.py:68
+msgid "The email field is missing"
 msgstr ""
 
-#: collective/volto/formsupport/configure.zcml:33
-msgid "Volto: Form support"
+#: collective/volto/formsupport/browser/templates/email_confirm_view.pt:367
+msgid "The form on ${page} was compiled with this email address, if it was not you, ignore the message."
+msgstr ""
+
+#: collective/volto/formsupport/restapi/services/validation/email.py:92
+msgid "The otp field is missing"
+msgstr ""
+
+#: collective/volto/formsupport/restapi/services/validation/email.py:71
+msgid "The provided email address is not valid"
+msgstr ""
+
+#: collective/volto/formsupport/restapi/services/validation/email.py:74
+msgid "The uid field is missing"
 msgstr ""
 
-#: collective/volto/formsupport/configure.zcml:42
+#: collective/volto/formsupport/configure.zcml:43
+msgid "Uninstalls the collective.volto.formsupport add-on."
+msgstr "Desinstala o complemento collective.volto.formsupport."
+
+#: collective/volto/formsupport/configure.zcml:34
+msgid "Volto: Form support"
+msgstr "Volto: Suporte a formulários"
+
+#: collective/volto/formsupport/configure.zcml:43
 msgid "Volto: Form support (uninstall)"
+msgstr "Volto: Suporte a formulários (Desinstalar)"
+
+#: collective/volto/formsupport/browser/templates/email_confirm_view.pt:353
+msgid "Your code to validate the email address:"
 msgstr ""
 
 #. Default: "Attachments too big. You uploaded ${uploaded_str}, but limit is ${max} MB. Try to compress files."
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:152
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:213
 msgid "attachments_too_big"
-msgstr "Allegati troppo grandi. Hai caricato ${uploaded_str}, ma il limite è di ${max} MB. Prova a comprimerli."
+msgstr ""
 
 #. Default: "Block with @type \"form\" and id \"$block\" not found in this context: $context"
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:93
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:128
 msgid "block_form_not_found_label"
-msgstr "Blocco con @type \"form\" e id \"$block\" non trovato nel contesto: $context"
+msgstr "Bloco com @type \"form\" e id \"${block}\" não encontrado no contexto: $context."
 
 #. Default: "Empty form data."
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:119
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:154
 msgid "empty_form_data"
-msgstr "Form senza dati."
+msgstr "Formulário sem dados."
+
+#. Default: "Error submitting form."
+#: collective/volto/formsupport/captcha/honeypot.py:30
+msgid "honeypot_error"
+msgstr ""
 
 #. Default: "Unable to send confirm email. Please retry later or contact site administator."
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:66
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:75
 msgid "mail_send_exception"
-msgstr "Impossibile inviare la mail di conferma. Per favore riprova più tardi o contatta l'amministratore del sito."
+msgstr ""
 
 #. Default: "You need to set at least one form action between \"send\" and \"store\"."
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:108
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:143
 msgid "missing_action"
-msgstr "Devi selezionare almeno un'azione tra \"salva\" e \"invia\"."
+msgstr "Você deve selecionar pelo menos uma ação entre \"salvar\" e \"enviar\"."
 
 #. Default: "Missing block_id"
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:86
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:121
 msgid "missing_blockid_label"
-msgstr "Campo block_id mancante."
+msgstr "Campo  block_id não informado"
 
-#. Default: "A new form has been submitted from ${url}:"
-#: collective/volto/formsupport/browser/send_mail_template.pt:7
+#. Default: "A new form has been submitted from <a href=\"${url}\">${url}</a>"
+#: collective/volto/formsupport/browser/send_mail_template.pt:15
 msgid "send_mail_text"
-msgstr "Un nuovo form è stato compilato da ${url}:"
+msgstr "Um novo formulário foi preenchido em ${url}:"
+
+#. Default: "Form submission data for ${title}"
+#: collective/volto/formsupport/browser/send_mail_template_table.pt:12
+msgid "send_mail_text_table"
+msgstr ""
 
 #. Default: "Missing required field: subject or from."
-#: collective/volto/formsupport/restapi/services/submit_form/post.py:230
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:320
 msgid "send_required_field_missing"
-msgstr "Campo obbligatorio mancante: subject o from."
+msgstr "Campo obrigatório não presente: Assunto ou remetente."
+
+#. Default: "Email not valid in \"${field}\" field."
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:185
+msgid "wrong_email"
+msgstr ""
+
+#: collective/volto/formsupport/restapi/services/submit_form/post.py:244
+msgid "{email}'s OTP is wrong"
+msgstr ""
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.mo` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
-"POT-Creation-Date: 2022-09-20 08:23+0000\n"
+"POT-Creation-Date: 2024-04-17 10:34+0000\n"
 "PO-Revision-Date: 2021-05-11 18:49-0300\n"
 "Last-Translator: Érico Andrei <ericof@plone.org>, 2021\n"
 "Language-Team: Portuguese (https://www.transifex.com/plone/teams/14552/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/update.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/update.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import os
-import pkg_resources
 import subprocess
 
+import pkg_resources
 
 domain = "collective.volto.formsupport"
 os.chdir(pkg_resources.resource_filename(domain, ""))
 os.chdir("../../../../")
 target_path = "src/collective/volto/formsupport/"
 locale_path = target_path + "locales/"
 i18ndude = "./bin/i18ndude"
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/locales/update.sh` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/serializer/blocks.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/serializer/blocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # -*- coding: utf-8 -*-
-from collective.volto.formsupport.interfaces import ICaptchaSupport
-from collective.volto.formsupport.interfaces import ICollectiveVoltoFormsupportLayer
+import os
+
 from plone import api
 from plone.restapi.behaviors import IBlocks
 from plone.restapi.interfaces import IBlockFieldSerializationTransformer
 from Products.CMFPlone.interfaces import IPloneSiteRoot
-from zope.component import adapter
-from zope.component import getMultiAdapter
+from zope.component import adapter, getMultiAdapter
 from zope.interface import implementer
 
-import os
+from collective.volto.formsupport.interfaces import (
+    ICaptchaSupport,
+    ICollectiveVoltoFormsupportLayer,
+)
 
 
 class FormSerializer(object):
     """ """
 
     order = 200  # after standard ones
     block_type = "form"
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/form_data/configure.zcml` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/configure.zcml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:plone="http://namespaces.plone.org/plone"
-    xmlns:zcml="http://namespaces.zope.org/zcml">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
 
   <plone:service
-    method="GET"
-    name="@form-data"
-    for="plone.restapi.behaviors.IBlocks"
-    factory=".form_data.FormDataGet"
-    permission="cmf.ModifyPortalContent"
-    layer="collective.volto.formsupport.interfaces.ICollectiveVoltoFormsupportLayer"
-    />
-  <adapter factory=".form_data.FormData" name="form-data"/>
+      method="GET"
+      factory=".form_data.FormDataGet"
+      for="plone.restapi.behaviors.IBlocks"
+      permission="cmf.ModifyPortalContent"
+      layer="collective.volto.formsupport.interfaces.ICollectiveVoltoFormsupportLayer"
+      name="@form-data"
+      />
+  <adapter
+      factory=".form_data.FormData"
+      name="form-data"
+      />
 
   <plone:service
-    method="GET"
-    name="@form-data-clear"
-    for="plone.restapi.behaviors.IBlocks"
-    factory=".clear.FormDataClear"
-    permission="cmf.ModifyPortalContent"
-    layer="collective.volto.formsupport.interfaces.ICollectiveVoltoFormsupportLayer"
-    />
+      method="DELETE"
+      factory=".clear.FormDataClear"
+      for="plone.restapi.behaviors.IBlocks"
+      permission="cmf.ModifyPortalContent"
+      layer="collective.volto.formsupport.interfaces.ICollectiveVoltoFormsupportLayer"
+      name="@form-data-clear"
+      />
 
   <plone:service
-    method="GET"
-    name="@form-data-export"
-    for="plone.restapi.behaviors.IBlocks"
-    factory=".csv.FormDataExportGet"
-    permission="cmf.ModifyPortalContent"
-    layer="collective.volto.formsupport.interfaces.ICollectiveVoltoFormsupportLayer"
-    />
+      method="GET"
+      factory=".csv.FormDataExportGet"
+      for="plone.restapi.behaviors.IBlocks"
+      permission="cmf.ModifyPortalContent"
+      layer="collective.volto.formsupport.interfaces.ICollectiveVoltoFormsupportLayer"
+      name="@form-data-export"
+      />
 
 </configure>
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/form_data/csv.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/form_data/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
-from collective.volto.formsupport.interfaces import IFormDataStore
+import csv
+
+import six
 from plone.restapi.serializer.converters import json_compatible
 from plone.restapi.services import Service
 from six import StringIO
 from zope.component import getMultiAdapter
 
-import csv
-import six
+from collective.volto.formsupport.interfaces import IFormDataStore
 
 SKIP_ATTRS = ["block_id", "fields_labels", "fields_order"]
 
 
 class FormDataExportGet(Service):
     def __init__(self, context, request):
         super().__init__(context, request)
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/restapi/services/form_data/form_data.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/restapi/services/validation/email.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,98 @@
 # -*- coding: utf-8 -*-
 
-from collective.volto.formsupport.interfaces import IFormDataStore
-from collective.volto.formsupport.utils import get_blocks
+import logging
+import os
+from email import policy
+from email.message import EmailMessage
+from email.utils import parseaddr
+
 from plone import api
-from plone.memoize import view
-from plone.restapi.interfaces import IExpandableElement
-from plone.restapi.serializer.converters import json_compatible
+from plone.restapi.deserializer import json_body
 from plone.restapi.services import Service
-from zope.component import adapter
-from zope.component import getMultiAdapter
-from zope.interface import implementer
-from zope.interface import Interface
-
-import json
-import six
-
-
-@implementer(IExpandableElement)
-@adapter(Interface, Interface)
-class FormData(object):
-    def __init__(self, context, request):
-        self.context = context
-        self.request = request
-
-    def __call__(self, expand=False):
-        if not self.show_component():
-            return {}
-
-        result = {
-            "form_data": {"@id": "{}/@form-data".format(self.context.absolute_url())}
-        }
-        if not expand:
-            return result
-
-        store = getMultiAdapter((self.context, self.request), IFormDataStore)
-        data = store.search()
-        items = [self.expand_records(x) for x in data]
-        data = {
-            "@id": "{}/@form-data".format(self.context.absolute_url()),
-            "items": items,
-            "items_total": len(items),
-        }
-
-        result["form_data"] = data
-        return result
-
-    @property
-    @view.memoize
-    def form_block(self):
-        blocks = get_blocks(self.context)
-
-        if isinstance(blocks, six.text_type):
-            blocks = json.loads(blocks)
-        if not blocks:
-            return {}
-        for block in blocks.values():
-            if block.get("@type", "") == "form" and block.get("store", False):
-                return block
-        return {}
-
-    def show_component(self):
-        if not api.user.has_permission("Modify portal content", obj=self.context):
-            return False
-        return self.form_block and True or False
-
-    def expand_records(self, record):
-        fields_labels = record.attrs.get("fields_labels", {})
-        data = {}
-        for k, v in record.attrs.items():
-            if k in ["fields_labels", "fields_order"]:
-                continue
-            data[k] = {
-                "value": json_compatible(v),
-                "label": fields_labels.get(k, k),
-            }
-        data["id"] = record.intid
+from zExceptions import BadRequest
+
+from collective.volto.formsupport import _
+from collective.volto.formsupport.utils import (
+    generate_email_token,
+    validate_email_token,
+)
+
+CTE = os.environ.get("MAIL_CONTENT_TRANSFER_ENCODING", None)
+
+logger = logging.getLogger(__name__)
+
+
+class ValidateEmailMessage(Service):
+    def reply(self):
+        data = self.validate()
+
+        self.send_token(generate_email_token(data["uid"], data["email"]), data["email"])
+
+        return self.reply_no_content()
+
+    def send_token(self, token, email):
+        """
+        Send token to recipient
+        """
+        portal_transforms = api.portal.get_tool(name="portal_transforms")
+        mail_view = api.content.get_view(
+            context=self.context, name="email-confirm-view"
+        )
+
+        content = mail_view(token=token)
+        mfrom = api.portal.get_registry_record("plone.email_from_address")
+        host = api.portal.get_tool("MailHost")
+        msg = EmailMessage(policy=policy.SMTP)
+
+        msg.set_content(
+            portal_transforms.convertTo("text/plain", content, mimetype="text/html")
+            .getData()
+            .strip(),
+            cte=CTE,
+        )
+        msg.add_alternative(content, subtype="html", cte=CTE)
+
+        msg["Subject"] = api.portal.translate(_("Email confirmation code"))
+        msg["From"] = mfrom
+        msg["To"] = email
+
+        try:
+            host.send(msg, charset="utf-8")
+        except Exception as e:
+            logger.error(f"The email confirmation message was not send due to {e}")
+
+    def validate(self):
+        data = json_body(self.request)
+
+        if "email" not in data:
+            raise BadRequest(_("The email field is missing"))
+
+        if "@" not in parseaddr(data["email"])[1]:
+            raise BadRequest(_("The provided email address is not valid"))
+
+        if "uid" not in data:
+            raise BadRequest(_("The uid field is missing"))
+
         return data
 
 
-class FormDataGet(Service):
+class ValidateEmailToken(Service):
     def reply(self):
-        form_data = FormData(self.context, self.request)
-        return form_data(expand=True).get("form_data", {})
+        self.validate()
+
+        return self.reply_no_content()
+
+    def validate(self):
+        data = json_body(self.request)
+
+        if "email" not in data:
+            raise BadRequest(_("The email field is missing"))
+
+        if "otp" not in data:
+            raise BadRequest(_("The otp field is missing"))
+
+        if "uid" not in data:
+            raise BadRequest(_("The uid field is missing"))
+
+        if not validate_email_token(data["uid"], data["email"], data["otp"]):
+            raise BadRequest(_("OTP is wrong"))
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/setuphandlers.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/testing.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
+import collective.honeypot
+import collective.MockMailHost
+import plone.restapi
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
-from plone.app.testing import applyProfile
-from plone.app.testing import FunctionalTesting
-from plone.app.testing import IntegrationTesting
-from plone.app.testing import PloneSandboxLayer
-from plone.app.testing import quickInstallProduct
+from plone.app.testing import (
+    FunctionalTesting,
+    IntegrationTesting,
+    PloneSandboxLayer,
+    applyProfile,
+    quickInstallProduct,
+)
 from plone.restapi.testing import PloneRestApiDXLayer
 from plone.testing import z2
 
-import collective.MockMailHost
 import collective.volto.formsupport
-import collective.honeypot
-import plone.restapi
 
 
 class VoltoFormsupportLayer(PloneSandboxLayer):
-
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
         # The z3c.autoinclude feature is disabled in the Plone fixture base
         # layer.
         import plone.restapi
@@ -27,14 +28,22 @@
         self.loadZCML(package=plone.restapi)
         self.loadZCML(package=collective.volto.formsupport)
 
     def setUpPloneSite(self, portal):
         applyProfile(portal, "plone.restapi:blocks")
         applyProfile(portal, "collective.volto.formsupport:default")
 
+        # Mock the validate email tocken function
+        def validate_email_token_mock(*args, **kwargs):
+            return True
+
+        from collective.volto.formsupport import utils
+
+        utils.validate_email_token = validate_email_token_mock
+
 
 VOLTO_FORMSUPPORT_FIXTURE = VoltoFormsupportLayer()
 
 
 VOLTO_FORMSUPPORT_INTEGRATION_TESTING = IntegrationTesting(
     bases=(VOLTO_FORMSUPPORT_FIXTURE,),
     name="VoltoFormsupportLayer:IntegrationTesting",
@@ -44,15 +53,14 @@
 VOLTO_FORMSUPPORT_FUNCTIONAL_TESTING = FunctionalTesting(
     bases=(VOLTO_FORMSUPPORT_FIXTURE,),
     name="VoltoFormsupportLayer:FunctionalTesting",
 )
 
 
 class VoltoFormsupportRestApiLayer(PloneRestApiDXLayer):
-
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         super(VoltoFormsupportRestApiLayer, self).setUpZope(app, configurationContext)
         self.loadZCML(package=collective.MockMailHost)
         self.loadZCML(package=plone.restapi)
         self.loadZCML(package=collective.honeypot)
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/file.pdf` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_captcha.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_captcha.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # -*- coding: utf-8 -*-
-from collective.volto.formsupport.testing import (  # noqa: E501,
-    VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING,
-)
+import json
+import unittest
 from hashlib import md5
+from unittest.mock import Mock, patch
+
+import transaction
+from collective.z3cform.norobots.browser.interfaces import INorobotsWidgetSettings
 from plone import api
-from plone.app.testing import setRoles
-from plone.app.testing import SITE_OWNER_NAME
-from plone.app.testing import SITE_OWNER_PASSWORD
-from plone.app.testing import TEST_USER_ID
+from plone.app.testing import (
+    SITE_OWNER_NAME,
+    SITE_OWNER_PASSWORD,
+    TEST_USER_ID,
+    setRoles,
+)
 from plone.formwidget.hcaptcha.interfaces import IHCaptchaSettings
 from plone.formwidget.recaptcha.interfaces import IReCaptchaSettings
-from collective.z3cform.norobots.browser.interfaces import INorobotsWidgetSettings
 from plone.registry.interfaces import IRegistry
 from plone.restapi.testing import RelativeSession
 from Products.MailHost.interfaces import IMailHost
-from unittest.mock import Mock
-from unittest.mock import patch
 from zope.component import getUtility
 
-import json
-import transaction
-import unittest
+from collective.volto.formsupport.testing import (  # noqa: E501,
+    VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING,
+)
 
 
 class TestCaptcha(unittest.TestCase):
-
     layer = VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -81,31 +82,39 @@
     def test_recaptcha_no_settings(self):
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "recaptcha",
             },
         }
         self.registry.registerInterface(IReCaptchaSettings)
         transaction.commit()
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                 ],
                 "block_id": "form-id",
             },
         )
         transaction.commit()
         self.assertEqual(response.status_code, 500)
         self.assertEqual(
@@ -122,31 +131,39 @@
 
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "recaptcha",
             },
         }
         transaction.commit()
 
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                 ],
                 "block_id": "form-id",
             },
         )
         transaction.commit()
         self.assertEqual(response.status_code, 400)
         self.assertEqual(response.json()["message"], "No captcha token provided.")
@@ -154,15 +171,19 @@
         with patch(
             "collective.volto.formsupport.captcha.recaptcha.submit"
         ) as mock_submit:
             mock_submit.return_value = Mock(is_valid=False)
             response = self.submit_form(
                 data={
                     "data": [
-                        {"label": "Message", "value": "just want to say hi"},
+                        {
+                            "field_id": "message",
+                            "label": "Message",
+                            "value": "just want to say hi",
+                        },
                     ],
                     "block_id": "form-id",
                     "captcha": {"token": "12345"},
                 },
             )
             transaction.commit()
             mock_submit.assert_called_once_with("12345", "private", "127.0.0.1")
@@ -175,23 +196,27 @@
         with patch(
             "collective.volto.formsupport.captcha.recaptcha.submit"
         ) as mock_submit:
             mock_submit.return_value = Mock(is_valid=True)
             response = self.submit_form(
                 data={
                     "data": [
-                        {"label": "Message", "value": "just want to say hi"},
+                        {
+                            "field_id": "message",
+                            "label": "Message",
+                            "value": "just want to say hi",
+                        },
                     ],
                     "block_id": "form-id",
                     "captcha": {"token": "12345"},
                 },
             )
             transaction.commit()
             mock_submit.assert_called_once_with("12345", "private", "127.0.0.1")
-            self.assertEqual(response.status_code, 204)
+            self.assertEqual(response.status_code, 200)
 
     def test_hcaptcha(
         self,
     ):
         self.registry.registerInterface(IHCaptchaSettings)
         settings = self.registry.forInterface(IHCaptchaSettings)
         settings.public_key = "public"
@@ -199,31 +224,39 @@
 
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "hcaptcha",
             },
         }
         transaction.commit()
 
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                 ],
                 "block_id": "form-id",
             },
         )
         transaction.commit()
         self.assertEqual(response.status_code, 400)
         self.assertEqual(response.json()["message"], "No captcha token provided.")
@@ -231,15 +264,19 @@
         with patch(
             "collective.volto.formsupport.captcha.hcaptcha.submit"
         ) as mock_submit:
             mock_submit.return_value = Mock(is_valid=False)
             response = self.submit_form(
                 data={
                     "data": [
-                        {"label": "Message", "value": "just want to say hi"},
+                        {
+                            "field_id": "message",
+                            "label": "Message",
+                            "value": "just want to say hi",
+                        },
                     ],
                     "block_id": "form-id",
                     "captcha": {"token": "12345"},
                 },
             )
             transaction.commit()
             mock_submit.assert_called_once_with("12345", "private", "127.0.0.1")
@@ -252,23 +289,27 @@
         with patch(
             "collective.volto.formsupport.captcha.hcaptcha.submit"
         ) as mock_submit:
             mock_submit.return_value = Mock(is_valid=True)
             response = self.submit_form(
                 data={
                     "data": [
-                        {"label": "Message", "value": "just want to say hi"},
+                        {
+                            "field_id": "message",
+                            "label": "Message",
+                            "value": "just want to say hi",
+                        },
                     ],
                     "block_id": "form-id",
                     "captcha": {"token": "12345"},
                 },
             )
             transaction.commit()
             mock_submit.assert_called_once_with("12345", "private", "127.0.0.1")
-            self.assertEqual(response.status_code, 204)
+            self.assertEqual(response.status_code, 200)
 
     def test_get_vocabulary(self):
         response = self.api_session.get(
             "/@vocabularies/collective.volto.formsupport.captcha.providers"
         )
         self.assertEqual(response.status_code, 200)
         data = response.json()
@@ -320,21 +361,25 @@
 
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "norobots-captcha",
             },
         }
         transaction.commit()
 
         captcha_token = json.dumps(
@@ -346,42 +391,50 @@
                 ).hexdigest(),
             }
         )
 
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                 ],
                 "block_id": "form-id",
                 "captcha": {"provider": "norobots-captcha", "token": captcha_token},
             },
         )
-        self.assertEqual(response.status_code, 204)
+        self.assertEqual(response.status_code, 200)
 
     def test_norobots_wrong_captcha(self):
         """test that using norobots and a wrong answer, the captcha is not passed"""
         self.registry.registerInterface(INorobotsWidgetSettings)
         settings = self.registry.forInterface(INorobotsWidgetSettings)
         settings.questions = ("Write five using cipers::5", "How much is 10 + 4::14")
         transaction.commit()
 
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "norobots-captcha",
             },
         }
         transaction.commit()
 
         captcha_token = json.dumps(
@@ -393,15 +446,19 @@
                 ).hexdigest(),
             }
         )
 
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                 ],
                 "block_id": "form-id",
                 "captcha": {"provider": "norobots-captcha", "token": captcha_token},
             },
         )
 
         self.assertEqual(response.status_code, 400)
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_event.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_event.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # -*- coding: utf-8 -*-
-from collective.volto.formsupport.testing import (  # noqa: E501,
-    VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING,
-)
+import unittest
+
+import transaction
 from plone import api
-from plone.app.testing import setRoles
-from plone.app.testing import SITE_OWNER_NAME
-from plone.app.testing import SITE_OWNER_PASSWORD
-from plone.app.testing import TEST_USER_ID
+from plone.app.testing import (
+    SITE_OWNER_NAME,
+    SITE_OWNER_PASSWORD,
+    TEST_USER_ID,
+    setRoles,
+)
 from plone.registry.interfaces import IRegistry
 from plone.restapi.testing import RelativeSession
 from Products.MailHost.interfaces import IMailHost
 from zope.component import getUtility
 from zope.configuration import xmlconfig
 
-import transaction
-import unittest
+from collective.volto.formsupport.testing import (  # noqa: E501,
+    VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING,
+)
 
 
 def event_handler(event):
     event.data["data"].append(
         {"label": "Reply", "value": "hello"},
     )
 
 
 class TestEvent(unittest.TestCase):
-
     layer = VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         xmlconfig.string(
             """
             <configure xmlns="http://namespaces.zope.org/zope">
                 <subscriber
@@ -87,44 +89,51 @@
         )
         # transaction.commit()
         return response
 
     def test_trigger_event(
         self,
     ):
-
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
             },
         }
         transaction.commit()
 
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                 ],
                 "block_id": "form-id",
             },
         )
         transaction.commit()
 
-        self.assertEqual(response.status_code, 204)
+        self.assertEqual(response.status_code, 200)
         self.assertEqual(len(self.mailhost.messages), 1)
         msg = self.mailhost.messages[0]
         if isinstance(msg, bytes) and bytes is not str:
             # Python 3 with Products.MailHost 4.10+
             msg = msg.decode("utf-8")
         self.assertIn("To: site_addr@plone.com", msg)
         self.assertNotIn("To: smith@doe.com", msg)
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_honeypot.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_honeypot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # -*- coding: utf-8 -*-
-from collective.volto.formsupport.testing import (  # noqa: E501,
-    VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING,
-)
+import json
+import unittest
+
+import transaction
 from plone import api
-from plone.app.testing import setRoles
-from plone.app.testing import SITE_OWNER_NAME
-from plone.app.testing import SITE_OWNER_PASSWORD
-from plone.app.testing import TEST_USER_ID
+from plone.app.testing import (
+    SITE_OWNER_NAME,
+    SITE_OWNER_PASSWORD,
+    TEST_USER_ID,
+    setRoles,
+)
 from plone.registry.interfaces import IRegistry
 from plone.restapi.testing import RelativeSession
 from Products.MailHost.interfaces import IMailHost
 from zope.component import getUtility
 
-import transaction
-import unittest
-import json
+from collective.volto.formsupport.testing import (  # noqa: E501,
+    VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING,
+)
 
 
 class TestHoneypot(unittest.TestCase):
-
     layer = VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -68,104 +70,129 @@
         response = self.api_session.post(
             url,
             json=data,
         )
         return response
 
     def test_honeypot_installed_but_field_not_in_form(self):
-
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "honeypot",
             },
         }
         transaction.commit()
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                 ],
                 "block_id": "form-id",
             },
         )
 
         self.assertEqual(response.status_code, 400)
         self.assertEqual(
             response.json()["message"],
             "Error submitting form.",
         )
 
     def test_honeypot_field_in_form_empty_pass_validation(self):
-
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "honeypot",
             },
         }
         transaction.commit()
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                     {"label": "protected_1", "value": ""},
                 ],
                 "block_id": "form-id",
             },
         )
-        self.assertEqual(response.status_code, 204)
+        self.assertEqual(response.status_code, 200)
 
     def test_honeypot_field_in_form_compiled_fail_validation(self):
-
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
+                    {
+                        "field_id": "protected_1",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "honeypot",
             },
         }
         transaction.commit()
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
-                    {"label": "protected_1", "value": "foo"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
+                    {"field_id": "protected_1", "label": "protected_1", "value": "foo"},
                 ],
                 "block_id": "form-id",
             },
         )
 
         self.assertEqual(response.status_code, 400)
         self.assertEqual(
@@ -179,70 +206,86 @@
         """
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "honeypot",
             },
         }
         transaction.commit()
         captcha_token = json.dumps({"id": "protected_1", "value": "foo"})
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                 ],
                 "block_id": "form-id",
                 "captcha": {
                     "provider": "honey",
                     "token": captcha_token,
                     "value": "",
                 },
             },
         )
 
-        self.assertEqual(response.status_code, 204)
+        self.assertEqual(response.status_code, 200)
 
     def test_form_submitted_from_volto_invalid_because_missing_value(self):
         """
         when you compile the form from volto, the honey field value is passed into captcha value
         """
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "honeypot",
             },
         }
         transaction.commit()
         captcha_token = json.dumps({"id": "protected_1", "value": "foo"})
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                 ],
                 "block_id": "form-id",
                 "captcha": {
                     "provider": "honey",
                     "token": captcha_token,
                 },
             },
@@ -260,31 +303,39 @@
         """
         self.document.blocks = {
             "text-id": {"@type": "text"},
             "form-id": {
                 "@type": "form",
                 "default_subject": "block subject",
                 "default_from": "john@doe.com",
-                "send": True,
+                "send": ["recipient"],
                 "subblocks": [
                     {
                         "field_id": "contact",
                         "field_type": "from",
                         "use_as_bcc": True,
                     },
+                    {
+                        "field_id": "message",
+                        "field_type": "text",
+                    },
                 ],
                 "captcha": "honeypot",
             },
         }
         transaction.commit()
         captcha_token = json.dumps({"id": "protected_1", "value": "foo"})
         response = self.submit_form(
             data={
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
                 ],
                 "block_id": "form-id",
                 "captcha": {
                     "provider": "honey",
                     "token": captcha_token,
                     "value": "i'm a bot",
                 },
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_serialize_block.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_serialize_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
-from collective.volto.formsupport.testing import (  # noqa: E501,
-    VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING,
-)
+import os
+import unittest
+
+import transaction
 from plone import api
-from plone.app.testing import setRoles
-from plone.app.testing import SITE_OWNER_NAME
-from plone.app.testing import SITE_OWNER_PASSWORD
-from plone.app.testing import TEST_USER_ID
+from plone.app.testing import (
+    SITE_OWNER_NAME,
+    SITE_OWNER_PASSWORD,
+    TEST_USER_ID,
+    setRoles,
+)
 from plone.formwidget.hcaptcha.interfaces import IHCaptchaSettings
 from plone.formwidget.recaptcha.interfaces import IReCaptchaSettings
 from plone.registry.interfaces import IRegistry
 from plone.restapi.testing import RelativeSession
 from zope.component import getUtility
 
-import transaction
-import unittest
-import os
+from collective.volto.formsupport.testing import (  # noqa: E501,
+    VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING,
+)
 
 
 class TestBlockSerialization(unittest.TestCase):
-
     layer = VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -70,15 +72,14 @@
         self.assertNotEqual(res["blocks"]["form-id"], self.document.blocks["form-id"])
         self.assertNotIn("default_from", res["blocks"]["form-id"].keys())
         self.assertNotIn("default_foo", res["blocks"]["form-id"].keys())
         self.assertIn("subblocks", res["blocks"]["form-id"].keys())
 
 
 class TestBlockSerializationRecaptcha(unittest.TestCase):
-
     layer = VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -127,15 +128,14 @@
         self.assertEqual(
             res["blocks"]["form-id"]["captcha_props"],
             {"provider": "recaptcha", "public_key": "public"},
         )
 
 
 class TestBlockSerializationHCaptcha(unittest.TestCase):
-
     layer = VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -184,15 +184,14 @@
         self.assertEqual(
             res["blocks"]["form-id"]["captcha_props"],
             {"provider": "hcaptcha", "public_key": "public"},
         )
 
 
 class TestBlockSerializationAttachmentsLimit(unittest.TestCase):
-
     layer = VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_setup.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 """Setup tests for this package."""
+import unittest
+
+from plone import api
+from plone.app.testing import TEST_USER_ID, setRoles
+
 from collective.volto.formsupport.testing import (  # noqa: E501,
     VOLTO_FORMSUPPORT_INTEGRATION_TESTING,
 )
-from plone import api
-from plone.app.testing import setRoles
-from plone.app.testing import TEST_USER_ID
-
-import unittest
-
 
 try:
     from Products.CMFPlone.utils import get_installer
 except ImportError:
     get_installer = None
 
 
@@ -27,50 +26,64 @@
         if get_installer:
             self.installer = get_installer(self.portal, self.layer["request"])
         else:
             self.installer = api.portal.get_tool("portal_quickinstaller")
 
     def test_product_installed(self):
         """Test if collective.volto.formsupport is installed."""
-        self.assertTrue(
-            self.installer.isProductInstalled("collective.volto.formsupport")
-        )
+        if hasattr(self.installer, "isProductInstalled"):
+            self.assertTrue(
+                self.installer.isProductInstalled("collective.volto.formsupport")
+            )
+        else:  # plone 6
+            self.assertTrue(
+                self.installer.is_product_installed("collective.volto.formsupport")
+            )
 
     def test_browserlayer(self):
         """Test that ICollectiveVoltoFormsupportLayer is registered."""
+        from plone.browserlayer import utils
+
         from collective.volto.formsupport.interfaces import (
             ICollectiveVoltoFormsupportLayer,
         )
-        from plone.browserlayer import utils
 
         self.assertIn(ICollectiveVoltoFormsupportLayer, utils.registered_layers())
 
 
 class TestUninstall(unittest.TestCase):
-
     layer = VOLTO_FORMSUPPORT_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         if get_installer:
             self.installer = get_installer(self.portal, self.layer["request"])
         else:
             self.installer = api.portal.get_tool("portal_quickinstaller")
         roles_before = api.user.get_roles(TEST_USER_ID)
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
-        self.installer.uninstallProducts(["collective.volto.formsupport"])
+        if hasattr(self.installer, "uninstallProducts"):
+            self.installer.uninstallProducts(["collective.volto.formsupport"])
+        else:  # plone6
+            self.installer.uninstall_product("collective.volto.formsupport")
         setRoles(self.portal, TEST_USER_ID, roles_before)
 
     def test_product_uninstalled(self):
         """Test if collective.volto.formsupport is cleanly uninstalled."""
-        self.assertFalse(
-            self.installer.isProductInstalled("collective.volto.formsupport")
-        )
+        if hasattr(self.installer, "isProductInstalled"):
+            self.assertFalse(
+                self.installer.isProductInstalled("collective.volto.formsupport")
+            )
+        else:  # plone 6
+            self.assertFalse(
+                self.installer.is_product_installed("collective.volto.formsupport")
+            )
 
     def test_browserlayer_removed(self):
         """Test that ICollectiveVoltoFormsupportLayer is removed."""
+        from plone.browserlayer import utils
+
         from collective.volto.formsupport.interfaces import (
             ICollectiveVoltoFormsupportLayer,
         )
-        from plone.browserlayer import utils
 
         self.assertNotIn(ICollectiveVoltoFormsupportLayer, utils.registered_layers())
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/tests/test_store_action_form.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/tests/test_store_action_form.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
-from collective.volto.formsupport.testing import (  # noqa: E501,
-    VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING,
-)
+import csv
+import unittest
 from datetime import datetime
 from io import StringIO
+
+import transaction
 from plone import api
-from plone.app.testing import setRoles
-from plone.app.testing import SITE_OWNER_NAME
-from plone.app.testing import SITE_OWNER_PASSWORD
-from plone.app.testing import TEST_USER_ID
+from plone.app.testing import (
+    SITE_OWNER_NAME,
+    SITE_OWNER_PASSWORD,
+    TEST_USER_ID,
+    setRoles,
+)
 from plone.restapi.testing import RelativeSession
 from Products.MailHost.interfaces import IMailHost
 from zope.component import getUtility
 
-import csv
-import transaction
-import unittest
-
+from collective.volto.formsupport.testing import (  # noqa: E501,
+    VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING,
+)
 
-class TestMailSend(unittest.TestCase):
 
+class TestMailStore(unittest.TestCase):
     layer = VOLTO_FORMSUPPORT_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -77,39 +79,45 @@
     def export_csv(self):
         url = "{}/@form-data-export".format(self.document_url)
         response = self.api_session.get(url)
         return response
 
     def clear_data(self):
         url = "{}/@form-data-clear".format(self.document_url)
-        response = self.api_session.get(url)
-        # transaction.commit()
+        response = self.api_session.delete(url)
         return response
 
     def test_unable_to_store_data(self):
         """form schema not defined, unable to store data"""
         self.document.blocks = {
-            "form-id": {"@type": "form", "store": True},
+            "form-id": {
+                "@type": "form",
+                "store": True,
+            },
         }
         transaction.commit()
 
         response = self.submit_form(
             data={
                 "from": "john@doe.com",
                 "data": [
-                    {"label": "Message", "value": "just want to say hi"},
-                    {"label": "Name", "value": "John"},
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "value": "just want to say hi",
+                    },
+                    {"field_id": "name", "label": "Name", "value": "John"},
                 ],
                 "subject": "test subject",
                 "block_id": "form-id",
             },
         )
         transaction.commit()
         self.assertEqual(response.status_code, 400)
-        self.assertEqual(response.json()["message"], "Unable to store data")
+        self.assertEqual(response.json()["message"], "Empty form data.")
         response = self.export_csv()
 
     def test_store_data(self):
         self.document.blocks = {
             "form-id": {
                 "@type": "form",
                 "store": True,
@@ -138,21 +146,21 @@
                     {"field_id": "foo", "value": "skip this"},
                 ],
                 "subject": "test subject",
                 "block_id": "form-id",
             },
         )
         transaction.commit()
-        self.assertEqual(response.status_code, 204)
+        self.assertEqual(response.status_code, 200)
         response = self.export_data()
         data = response.json()
         self.assertEqual(len(data["items"]), 1)
         self.assertEqual(
             sorted(data["items"][0].keys()),
-            ["block_id", "date", "id", "message", "name"],
+            ["__expired", "block_id", "date", "id", "message", "name"],
         )
         self.assertEqual(
             data["items"][0]["message"],
             {"label": "Message", "value": "just want to say hi"},
         )
         self.assertEqual(data["items"][0]["name"], {"label": "Name", "value": "John"})
         response = self.submit_form(
@@ -163,25 +171,25 @@
                     {"field_id": "name", "value": "Sally"},
                 ],
                 "subject": "test subject",
                 "block_id": "form-id",
             },
         )
         transaction.commit()
-        self.assertEqual(response.status_code, 204)
+        self.assertEqual(response.status_code, 200)
         response = self.export_data()
         data = response.json()
         self.assertEqual(len(data["items"]), 2)
         self.assertEqual(
             sorted(data["items"][0].keys()),
-            ["block_id", "date", "id", "message", "name"],
+            ["__expired", "block_id", "date", "id", "message", "name"],
         )
         self.assertEqual(
             sorted(data["items"][1].keys()),
-            ["block_id", "date", "id", "message", "name"],
+            ["__expired", "block_id", "date", "id", "message", "name"],
         )
         sorted_data = sorted(data["items"], key=lambda x: x["name"]["value"])
         self.assertEqual(sorted_data[0]["name"]["value"], "John")
         self.assertEqual(sorted_data[0]["message"]["value"], "just want to say hi")
         self.assertEqual(sorted_data[1]["name"]["value"], "Sally")
         self.assertEqual(sorted_data[1]["message"]["value"], "bye")
 
@@ -234,20 +242,80 @@
                     {"field_id": "name", "value": "Sally"},
                 ],
                 "subject": "test subject",
                 "block_id": "form-id",
             },
         )
 
-        self.assertEqual(response.status_code, 204)
+        self.assertEqual(response.status_code, 200)
         response = self.export_csv()
         data = [*csv.reader(StringIO(response.text), delimiter=",")]
         self.assertEqual(len(data), 3)
         self.assertEqual(data[0], ["Message", "Name", "date"])
         sorted_data = sorted(data[1:])
         self.assertEqual(sorted_data[0][:-1], ["bye", "Sally"])
         self.assertEqual(sorted_data[1][:-1], ["just want to say hi", "John"])
 
         # check date column. Skip seconds because can change during test
-        now = datetime.utcnow().strftime("%Y-%m-%dT%H:%M")
+        now = datetime.now().strftime("%Y-%m-%dT%H:%M")
+        self.assertTrue(sorted_data[0][-1].startswith(now))
+        self.assertTrue(sorted_data[1][-1].startswith(now))
+
+    def test_data_id_mapping(self):
+        self.document.blocks = {
+            "form-id": {
+                "@type": "form",
+                "store": True,
+                "test-field": "renamed-field",
+                "subblocks": [
+                    {
+                        "field_id": "message",
+                        "label": "Message",
+                        "field_type": "text",
+                    },
+                    {
+                        "field_id": "test-field",
+                        "label": "Test field",
+                        "field_type": "text",
+                    },
+                ],
+            },
+        }
+        transaction.commit()
+        response = self.submit_form(
+            data={
+                "from": "john@doe.com",
+                "data": [
+                    {"field_id": "message", "value": "just want to say hi"},
+                    {"field_id": "test-field", "value": "John"},
+                ],
+                "subject": "test subject",
+                "block_id": "form-id",
+            },
+        )
+
+        response = self.submit_form(
+            data={
+                "from": "sally@doe.com",
+                "data": [
+                    {"field_id": "message", "value": "bye"},
+                    {"field_id": "test-field", "value": "Sally"},
+                ],
+                "subject": "test subject",
+                "block_id": "form-id",
+            },
+        )
+
+        self.assertEqual(response.status_code, 200)
+        response = self.export_csv()
+        data = [*csv.reader(StringIO(response.text), delimiter=",")]
+        self.assertEqual(len(data), 3)
+        # Check that 'test-field' got renamed
+        self.assertEqual(data[0], ["Message", "renamed-field", "date"])
+        sorted_data = sorted(data[1:])
+        self.assertEqual(sorted_data[0][:-1], ["bye", "Sally"])
+        self.assertEqual(sorted_data[1][:-1], ["just want to say hi", "John"])
+
+        # check date column. Skip seconds because can change during test
+        now = datetime.now().strftime("%Y-%m-%dT%H:%M")
         self.assertTrue(sorted_data[0][-1].startswith(now))
         self.assertTrue(sorted_data[1][-1].startswith(now))
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/upgrades.py` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/upgrades.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,68 @@
 # -*- coding: utf-8 -*-
-from Acquisition import aq_base
 from copy import deepcopy
+
+from Acquisition import aq_base
 from plone import api
 from plone.dexterity.utils import iterSchemata
-from zope.schema import getFields
-from collective.volto.formsupport.interfaces import IFormDataStore
-from zope.component import getMultiAdapter
-from zope.globalrequest import getRequest
-from souper.soup import Record
-from zope.component import getUtility
 from plone.i18n.normalizer.interfaces import IIDNormalizer
+from souper.soup import Record
+from zope.component import getMultiAdapter, getUtility
+from zope.globalrequest import getRequest
+from zope.schema import getFields
 
+from collective.volto.formsupport.interfaces import IFormDataStore
 
 try:
     from collective.volto.blocksfield.field import BlocksField
 
     HAS_BLOCKSFIELD = True
 except ImportError:
     HAS_BLOCKSFIELD = False
 
-from collective.volto.formsupport import logger
-
 import json
 
+from collective.volto.formsupport import logger
 
 DEFAULT_PROFILE = "profile-collective.volto.formsupport:default"
 
 
+def _has_block_form(block_data):
+    for block in block_data.values():
+        if block.get("@type", "") == "form":
+            return True
+    return False
+
+
+def _get_all_content_with_blocks():
+    content = []
+
+    portal = api.portal.get()
+    portal_blocks = getattr(portal, "blocks", "")
+    if portal_blocks:
+        if _has_block_form(portal_blocks):
+            content.append(portal)
+
+    pc = api.portal.get_tool(name="portal_catalog")
+    brains = pc()
+    total = len(brains)
+
+    for i, brain in enumerate(brains):
+        if i % 100 == 0:
+            logger.info("Progress: {}/{}".format(i + 1, total))
+        item = brain.getObject()
+        for schema in iterSchemata(item.aq_base):
+            for name, field in getFields(schema).items():
+                if name == "blocks":
+                    if _has_block_form(getattr(item, "blocks", {})):
+                        content.append(item)
+
+    return content
+
+
 def to_1100(context):  # noqa: C901 # pragma: no cover
     logger.info("### START CONVERSION FORM BLOCKS ###")
 
     def fix_block(blocks, url):
         for block in blocks.values():
             if block.get("@type", "") != "form":
                 continue
@@ -162,7 +194,40 @@
                     if blocks:
                         res = fix_data(blocks, item)
                         if res:
                             fixed_contents.append(brain.getPath())
     logger.info("Fixed {} contents:".format(len(fixed_contents)))
     for path in fixed_contents:
         logger.info("- {}".format(path))
+
+
+def to_1300(context):  # noqa: C901 # pragma: no cover
+    def update_send_from_bool_to_list_for_content(item):
+        blocks = (
+            item.blocks
+        )  # We've already checked we've a form block so no need to guard here
+
+        for block in blocks.values():
+            if block.get("@type", "") != "form":
+                continue
+            send = block.get("send")
+            if isinstance(send, bool):
+                new_send_value = ["recipient"] if block.get("send") else []
+                block["send"] = new_send_value
+                logger.info(
+                    "[CONVERTED] - {} form send value from {} to {}".format(
+                        item, send, new_send_value
+                    )
+                )
+
+        item.blocks = blocks
+
+    logger.info("### START UPGRADE SEND FROM STRING TO ARRAY ###")
+
+    content = _get_all_content_with_blocks()
+
+    for item in content:
+        update_send_from_bool_to_list_for_content(item)
+
+    logger.info("### FINISHED UPGRADE SEND FROM STRING TO ARRAY ###")
+
+    # self.block.get("send")
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective/volto/formsupport/upgrades.zcml` & `collective.volto.formsupport-3.0.1/src/collective/volto/formsupport/upgrades.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 <configure
-  xmlns="http://namespaces.zope.org/zope"
-  xmlns:genericsetup="http://namespaces.zope.org/genericsetup">
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    >
 
   <genericsetup:upgradeSteps
-    source="1000"
-    destination="1100"
-    profile="collective.volto.formsupport:default">
+      profile="collective.volto.formsupport:default"
+      source="1000"
+      destination="1100"
+      >
     <genericsetup:upgradeStep
         title="Convert field types"
         handler=".upgrades.to_1100"
         />
   </genericsetup:upgradeSteps>
   <genericsetup:upgradeSteps
-    source="1100"
-    destination="1200"
-    profile="collective.volto.formsupport:default">
+      profile="collective.volto.formsupport:default"
+      source="1100"
+      destination="1200"
+      >
     <genericsetup:upgradeStep
         title="Store fieldid in records"
         handler=".upgrades.to_1200"
         />
   </genericsetup:upgradeSteps>
+
+  <genericsetup:upgradeStep
+      title="Convert send from a bool into a list of who to send to"
+      profile="collective.volto.formsupport:default"
+      source="*"
+      destination="1300"
+      handler=".upgrades.to_1300"
+      />
+
 </configure>
```

### Comparing `collective.volto.formsupport-2.7.0/src/collective.volto.formsupport.egg-info/SOURCES.txt` & `collective.volto.formsupport-3.0.1/src/collective.volto.formsupport.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 DEVELOP.rst
 LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 constraints.txt
 constraints_plone52.txt
+constraints_plone60.txt
 requirements.txt
 setup.cfg
 setup.py
 docs/conf.py
 docs/index.rst
 src/collective/__init__.py
 src/collective.volto.formsupport.egg-info/PKG-INFO
@@ -29,17 +30,20 @@
 src/collective/volto/formsupport/setuphandlers.py
 src/collective/volto/formsupport/testing.py
 src/collective/volto/formsupport/upgrades.py
 src/collective/volto/formsupport/upgrades.zcml
 src/collective/volto/formsupport/utils.py
 src/collective/volto/formsupport/browser/__init__.py
 src/collective/volto/formsupport/browser/configure.zcml
+src/collective/volto/formsupport/browser/email_confirm_view.py
 src/collective/volto/formsupport/browser/send_mail_template.pt
+src/collective/volto/formsupport/browser/send_mail_template_table.pt
 src/collective/volto/formsupport/browser/overrides/.gitkeep
 src/collective/volto/formsupport/browser/static/.gitkeep
+src/collective/volto/formsupport/browser/templates/email_confirm_view.pt
 src/collective/volto/formsupport/captcha/__init__.py
 src/collective/volto/formsupport/captcha/configure.zcml
 src/collective/volto/formsupport/captcha/hcaptcha.py
 src/collective/volto/formsupport/captcha/honeypot.py
 src/collective/volto/formsupport/captcha/norobots.py
 src/collective/volto/formsupport/captcha/recaptcha.py
 src/collective/volto/formsupport/captcha/vocabularies.py
@@ -47,41 +51,54 @@
 src/collective/volto/formsupport/datamanager/catalog.py
 src/collective/volto/formsupport/datamanager/configure.zcml
 src/collective/volto/formsupport/locales/README.rst
 src/collective/volto/formsupport/locales/__init__.py
 src/collective/volto/formsupport/locales/collective.volto.formsupport.pot
 src/collective/volto/formsupport/locales/update.py
 src/collective/volto/formsupport/locales/update.sh
+src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.mo
+src/collective/volto/formsupport/locales/de/LC_MESSAGES/collective.volto.formsupport.po
+src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.mo
+src/collective/volto/formsupport/locales/es/LC_MESSAGES/collective.volto.formsupport.po
 src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.mo
 src/collective/volto/formsupport/locales/it/LC_MESSAGES/collective.volto.formsupport.po
 src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.mo
 src/collective/volto/formsupport/locales/pt_BR/LC_MESSAGES/collective.volto.formsupport.po
 src/collective/volto/formsupport/profiles/default/browserlayer.xml
 src/collective/volto/formsupport/profiles/default/catalog.xml
 src/collective/volto/formsupport/profiles/default/metadata.xml
 src/collective/volto/formsupport/profiles/default/rolemap.xml
 src/collective/volto/formsupport/profiles/default/registry/main.xml
 src/collective/volto/formsupport/profiles/uninstall/browserlayer.xml
 src/collective/volto/formsupport/restapi/__init__.py
 src/collective/volto/formsupport/restapi/configure.zcml
+src/collective/volto/formsupport/restapi/deserializer/__init__.py
+src/collective/volto/formsupport/restapi/deserializer/blocks.py
+src/collective/volto/formsupport/restapi/deserializer/configure.zcml
 src/collective/volto/formsupport/restapi/serializer/__init__.py
 src/collective/volto/formsupport/restapi/serializer/blocks.py
 src/collective/volto/formsupport/restapi/serializer/configure.zcml
 src/collective/volto/formsupport/restapi/services/__init__.py
 src/collective/volto/formsupport/restapi/services/configure.zcml
 src/collective/volto/formsupport/restapi/services/form_data/__init__.py
 src/collective/volto/formsupport/restapi/services/form_data/clear.py
 src/collective/volto/formsupport/restapi/services/form_data/configure.zcml
 src/collective/volto/formsupport/restapi/services/form_data/csv.py
 src/collective/volto/formsupport/restapi/services/form_data/form_data.py
 src/collective/volto/formsupport/restapi/services/submit_form/__init__.py
 src/collective/volto/formsupport/restapi/services/submit_form/configure.zcml
 src/collective/volto/formsupport/restapi/services/submit_form/post.py
+src/collective/volto/formsupport/restapi/services/validation/__init__.py
+src/collective/volto/formsupport/restapi/services/validation/configure.zcml
+src/collective/volto/formsupport/restapi/services/validation/email.py
+src/collective/volto/formsupport/scripts/__init__.py
+src/collective/volto/formsupport/scripts/cleansing.py
 src/collective/volto/formsupport/tests/__init__.py
 src/collective/volto/formsupport/tests/file.pdf
 src/collective/volto/formsupport/tests/test_captcha.py
+src/collective/volto/formsupport/tests/test_deserialize_block.py
 src/collective/volto/formsupport/tests/test_event.py
 src/collective/volto/formsupport/tests/test_honeypot.py
 src/collective/volto/formsupport/tests/test_send_action_form.py
 src/collective/volto/formsupport/tests/test_serialize_block.py
 src/collective/volto/formsupport/tests/test_setup.py
 src/collective/volto/formsupport/tests/test_store_action_form.py
```

