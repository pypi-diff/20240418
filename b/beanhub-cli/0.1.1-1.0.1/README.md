# Comparing `tmp/beanhub_cli-0.1.1.tar.gz` & `tmp/beanhub_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_cli-0.1.1.tar", max compression
+gzip compressed data, was "beanhub_cli-1.0.1.tar", max compression
```

## Comparing `beanhub_cli-0.1.1.tar` & `beanhub_cli-1.0.1.tar`

### file list

```diff
@@ -1,201 +1,201 @@
--rw-r--r--   0        0        0     1072 2023-10-08 22:46:39.180327 beanhub_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0     3363 2023-10-08 22:46:39.180327 beanhub_cli-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/__init__.py
--rw-r--r--   0        0        0      884 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/aliase.py
--rw-r--r--   0        0        0      915 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/cli.py
--rw-r--r--   0        0        0      735 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/environment.py
--rw-r--r--   0        0        0     2867 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/format.py
--rw-r--r--   0        0        0        0 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/forms/__init__.py
--rw-r--r--   0        0        0        0 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/forms/app/__init__.py
--rw-r--r--   0        0        0      119 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/forms/app/constants.py
--rw-r--r--   0        0        0      745 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/forms/app/data/sample_forms_doc.yaml
--rw-r--r--   0        0        0     4298 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/forms/app/deps.py
--rw-r--r--   0        0        0      934 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/forms/app/helpers.py
--rw-r--r--   0        0        0     1007 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/forms/app/main.py
--rw-r--r--   0        0        0     5739 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/forms/app/routes.py
--rw-r--r--   0        0        0      861 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/forms/app/settings.py
--rw-r--r--   0        0        0   242711 2023-10-08 22:46:39.184327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/js/beanhub-web-react-0.1.6.js
--rw-r--r--   0        0        0   569147 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/js/beanhub-web-react-0.1.6.js.map
--rw-r--r--   0        0        0    11360 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/LICENSE
--rw-r--r--   0        0        0    17192 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.css
--rw-r--r--   0        0        0    18548 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.css.map
--rw-r--r--   0        0        0    15733 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.min.css
--rw-r--r--   0        0        0    58136 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/js/bootstrap-datepicker.js
--rw-r--r--   0        0        0    33871 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/js/bootstrap-datepicker.min.js
--rw-r--r--   0        0        0      636 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker-en-CA.min.js
--rw-r--r--   0        0        0      778 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar-DZ.min.js
--rw-r--r--   0        0        0      704 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar-tn.min.js
--rw-r--r--   0        0        0      714 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar.min.js
--rw-r--r--   0        0        0      531 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.az.min.js
--rw-r--r--   0        0        0      615 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bg.min.js
--rw-r--r--   0        0        0      562 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bm.min.js
--rw-r--r--   0        0        0     1210 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bn.min.js
--rw-r--r--   0        0        0      510 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.br.min.js
--rw-r--r--   0        0        0      475 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bs.min.js
--rw-r--r--   0        0        0      525 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ca.min.js
--rw-r--r--   0        0        0      536 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.cs.min.js
--rw-r--r--   0        0        0      433 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.cy.min.js
--rw-r--r--   0        0        0      514 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.da.min.js
--rw-r--r--   0        0        0      510 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.de.min.js
--rw-r--r--   0        0        0      764 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.el.min.js
--rw-r--r--   0        0        0      517 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-AU.min.js
--rw-r--r--   0        0        0      518 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-CA.min.js
--rw-r--r--   0        0        0      518 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-GB.min.js
--rw-r--r--   0        0        0      518 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-IE.min.js
--rw-r--r--   0        0        0      517 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-NZ.min.js
--rw-r--r--   0        0        0      516 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-US.min.js
--rw-r--r--   0        0        0      517 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-ZA.min.js
--rw-r--r--   0        0        0      515 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.eo.min.js
--rw-r--r--   0        0        0      513 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.es.min.js
--rw-r--r--   0        0        0      537 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.et.min.js
--rw-r--r--   0        0        0      528 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.eu.min.js
--rw-r--r--   0        0        0      670 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fa.min.js
--rw-r--r--   0        0        0      551 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fi.min.js
--rw-r--r--   0        0        0      488 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fo.min.js
--rw-r--r--   0        0        0      512 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fr-CH.min.js
--rw-r--r--   0        0        0      536 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fr.min.js
--rw-r--r--   0        0        0      489 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.gl.min.js
--rw-r--r--   0        0        0      563 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.he.min.js
--rw-r--r--   0        0        0      944 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hi.min.js
--rw-r--r--   0        0        0      462 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hr.min.js
--rw-r--r--   0        0        0      541 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hu.min.js
--rw-r--r--   0        0        0      757 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hy.min.js
--rw-r--r--   0        0        0      505 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.id.min.js
--rw-r--r--   0        0        0      496 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.is.min.js
--rw-r--r--   0        0        0      506 2023-10-08 22:46:39.188327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.it-CH.min.js
--rw-r--r--   0        0        0      525 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.it.min.js
--rw-r--r--   0        0        0      502 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ja.min.js
--rw-r--r--   0        0        0      970 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ka.min.js
--rw-r--r--   0        0        0     1076 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kh.min.js
--rw-r--r--   0        0        0      649 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kk.min.js
--rw-r--r--   0        0        0      945 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.km.min.js
--rw-r--r--   0        0        0      532 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ko.min.js
--rw-r--r--   0        0        0      575 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kr.min.js
--rw-r--r--   0        0        0      565 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.lt.min.js
--rw-r--r--   0        0        0      526 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.lv.min.js
--rw-r--r--   0        0        0      493 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.me.min.js
--rw-r--r--   0        0        0      657 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mk.min.js
--rw-r--r--   0        0        0      638 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mn.min.js
--rw-r--r--   0        0        0      990 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mr.min.js
--rw-r--r--   0        0        0      448 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ms.min.js
--rw-r--r--   0        0        0      522 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.nl-BE.min.js
--rw-r--r--   0        0        0      513 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.nl.min.js
--rw-r--r--   0        0        0      515 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.no.min.js
--rw-r--r--   0        0        0      515 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.oc.min.js
--rw-r--r--   0        0        0      552 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.pl.min.js
--rw-r--r--   0        0        0      504 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.pt-BR.min.js
--rw-r--r--   0        0        0      498 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.pt.min.js
--rw-r--r--   0        0        0      505 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ro.min.js
--rw-r--r--   0        0        0      662 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.rs-latin.min.js
--rw-r--r--   0        0        0      817 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.rs.min.js
--rw-r--r--   0        0        0      731 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ru.min.js
--rw-r--r--   0        0        0      988 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.si.min.js
--rw-r--r--   0        0        0      497 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sk.min.js
--rw-r--r--   0        0        0      455 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sl.min.js
--rw-r--r--   0        0        0      518 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sq.min.js
--rw-r--r--   0        0        0      478 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sr-latin.min.js
--rw-r--r--   0        0        0      651 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sr.min.js
--rw-r--r--   0        0        0      492 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sv.min.js
--rw-r--r--   0        0        0      431 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sw.min.js
--rw-r--r--   0        0        0      934 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ta.min.js
--rw-r--r--   0        0        0      700 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.tg.min.js
--rw-r--r--   0        0        0      833 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.th.min.js
--rw-r--r--   0        0        0      530 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.tk.min.js
--rw-r--r--   0        0        0      495 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.tr.min.js
--rw-r--r--   0        0        0      723 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uk.min.js
--rw-r--r--   0        0        0      703 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uz-cyrl.min.js
--rw-r--r--   0        0        0      516 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uz-latn.min.js
--rw-r--r--   0        0        0      551 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.vi.min.js
--rw-r--r--   0        0        0      613 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.zh-CN.min.js
--rw-r--r--   0        0        0      607 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.zh-TW.min.js
--rw-r--r--   0        0        0     7427 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/LICENSE.txt
--rw-r--r--   0        0        0   102217 2023-10-08 22:46:39.192327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/css/all.min.css
--rw-r--r--   0        0        0   189684 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   109808 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    63348 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    24488 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   394668 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150020 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10172 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4568 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0     1124 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/LICENSE.md
--rw-r--r--   0        0        0    18931 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/css/select2.css
--rw-r--r--   0        0        0    16264 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/css/select2.min.css
--rw-r--r--   0        0        0      870 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/af.js
--rw-r--r--   0        0        0      909 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ar.js
--rw-r--r--   0        0        0      725 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/az.js
--rw-r--r--   0        0        0      972 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bg.js
--rw-r--r--   0        0        0     1295 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bn.js
--rw-r--r--   0        0        0      969 2023-10-08 22:46:39.196327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bs.js
--rw-r--r--   0        0        0      904 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ca.js
--rw-r--r--   0        0        0     1296 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/cs.js
--rw-r--r--   0        0        0      832 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/da.js
--rw-r--r--   0        0        0      870 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/de.js
--rw-r--r--   0        0        0     1021 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/dsb.js
--rw-r--r--   0        0        0     1186 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/el.js
--rw-r--r--   0        0        0      925 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/en.js
--rw-r--r--   0        0        0      871 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/eo.js
--rw-r--r--   0        0        0      926 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/es.js
--rw-r--r--   0        0        0      805 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/et.js
--rw-r--r--   0        0        0      872 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/eu.js
--rw-r--r--   0        0        0     1027 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fa.js
--rw-r--r--   0        0        0      807 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fi.js
--rw-r--r--   0        0        0      981 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fr.js
--rw-r--r--   0        0        0      928 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/gl.js
--rw-r--r--   0        0        0      988 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/he.js
--rw-r--r--   0        0        0     1179 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hi.js
--rw-r--r--   0        0        0      856 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hr.js
--rw-r--r--   0        0        0     1022 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hsb.js
--rw-r--r--   0        0        0      923 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hu.js
--rw-r--r--   0        0        0     1032 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hy.js
--rw-r--r--   0        0        0      772 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/id.js
--rw-r--r--   0        0        0      811 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/is.js
--rw-r--r--   0        0        0      901 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/it.js
--rw-r--r--   0        0        0      866 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ja.js
--rw-r--r--   0        0        0     1199 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ka.js
--rw-r--r--   0        0        0     1092 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/km.js
--rw-r--r--   0        0        0      859 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ko.js
--rw-r--r--   0        0        0      948 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/lt.js
--rw-r--r--   0        0        0      904 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/lv.js
--rw-r--r--   0        0        0     1042 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/mk.js
--rw-r--r--   0        0        0      815 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ms.js
--rw-r--r--   0        0        0      782 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/nb.js
--rw-r--r--   0        0        0     1361 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ne.js
--rw-r--r--   0        0        0      908 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/nl.js
--rw-r--r--   0        0        0     1381 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pa.js
--rw-r--r--   0        0        0      951 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pl.js
--rw-r--r--   0        0        0     1053 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ps.js
--rw-r--r--   0        0        0      880 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pt-BR.js
--rw-r--r--   0        0        0      882 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pt.js
--rw-r--r--   0        0        0      942 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ro.js
--rw-r--r--   0        0        0     1175 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ru.js
--rw-r--r--   0        0        0     1310 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sk.js
--rw-r--r--   0        0        0      929 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sl.js
--rw-r--r--   0        0        0      907 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sq.js
--rw-r--r--   0        0        0     1113 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sr-Cyrl.js
--rw-r--r--   0        0        0      984 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sr.js
--rw-r--r--   0        0        0      790 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sv.js
--rw-r--r--   0        0        0     1360 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/te.js
--rw-r--r--   0        0        0     1078 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/th.js
--rw-r--r--   0        0        0      775 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/tk.js
--rw-r--r--   0        0        0      779 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/tr.js
--rw-r--r--   0        0        0     1160 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/uk.js
--rw-r--r--   0        0        0      800 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/vi.js
--rw-r--r--   0        0        0      772 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/zh-CN.js
--rw-r--r--   0        0        0      711 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/zh-TW.js
--rw-r--r--   0        0        0   167106 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.full.js
--rw-r--r--   0        0        0    76775 2023-10-08 22:46:39.200327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.full.min.js
--rw-r--r--   0        0        0   156955 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.js
--rw-r--r--   0        0        0    73170 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.min.js
--rw-r--r--   0        0        0     1954 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/errors.html
--rw-r--r--   0        0        0      614 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/flash_messages.html
--rw-r--r--   0        0        0      522 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/footer.html
--rw-r--r--   0        0        0     2404 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/form.html
--rw-r--r--   0        0        0     4726 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/home.html
--rw-r--r--   0        0        0     1935 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/layout.html
--rw-r--r--   0        0        0      215 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/cli.py
--rw-r--r--   0        0        0     4992 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/main.py
--rw-r--r--   0        0        0     2842 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/forms/validator.py
--rw-r--r--   0        0        0      146 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/beanhub_cli/main.py
--rw-r--r--   0        0        0      792 2023-10-08 22:46:39.204327 beanhub_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 beanhub_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-18 07:41:33.494393 beanhub_cli-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3330 2024-04-18 07:41:33.494393 beanhub_cli-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-18 07:41:33.494393 beanhub_cli-1.0.1/beanhub_cli/__init__.py
+-rw-r--r--   0        0        0      884 2024-04-18 07:41:33.494393 beanhub_cli-1.0.1/beanhub_cli/aliase.py
+-rw-r--r--   0        0        0      915 2024-04-18 07:41:33.494393 beanhub_cli-1.0.1/beanhub_cli/cli.py
+-rw-r--r--   0        0        0      735 2024-04-18 07:41:33.494393 beanhub_cli-1.0.1/beanhub_cli/environment.py
+-rw-r--r--   0        0        0     2867 2024-04-18 07:41:33.494393 beanhub_cli-1.0.1/beanhub_cli/format.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:41:33.494393 beanhub_cli-1.0.1/beanhub_cli/forms/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:41:33.494393 beanhub_cli-1.0.1/beanhub_cli/forms/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-04-18 07:41:33.498393 beanhub_cli-1.0.1/beanhub_cli/forms/app/constants.py
+-rw-r--r--   0        0        0      745 2024-04-18 07:41:33.498393 beanhub_cli-1.0.1/beanhub_cli/forms/app/data/sample_forms_doc.yaml
+-rw-r--r--   0        0        0     4298 2024-04-18 07:41:33.498393 beanhub_cli-1.0.1/beanhub_cli/forms/app/deps.py
+-rw-r--r--   0        0        0      934 2024-04-18 07:41:33.498393 beanhub_cli-1.0.1/beanhub_cli/forms/app/helpers.py
+-rw-r--r--   0        0        0     1007 2024-04-18 07:41:33.498393 beanhub_cli-1.0.1/beanhub_cli/forms/app/main.py
+-rw-r--r--   0        0        0     5739 2024-04-18 07:41:33.498393 beanhub_cli-1.0.1/beanhub_cli/forms/app/routes.py
+-rw-r--r--   0        0        0      861 2024-04-18 07:41:33.498393 beanhub_cli-1.0.1/beanhub_cli/forms/app/settings.py
+-rw-r--r--   0        0        0   242711 2024-04-18 07:41:33.498393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/js/beanhub-web-react-0.1.6.js
+-rw-r--r--   0        0        0   569147 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/js/beanhub-web-react-0.1.6.js.map
+-rw-r--r--   0        0        0    11360 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/LICENSE
+-rw-r--r--   0        0        0    17192 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.css
+-rw-r--r--   0        0        0    18548 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.css.map
+-rw-r--r--   0        0        0    15733 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.min.css
+-rw-r--r--   0        0        0    58136 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/js/bootstrap-datepicker.js
+-rw-r--r--   0        0        0    33871 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/js/bootstrap-datepicker.min.js
+-rw-r--r--   0        0        0      636 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker-en-CA.min.js
+-rw-r--r--   0        0        0      778 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar-DZ.min.js
+-rw-r--r--   0        0        0      704 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar-tn.min.js
+-rw-r--r--   0        0        0      714 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar.min.js
+-rw-r--r--   0        0        0      531 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.az.min.js
+-rw-r--r--   0        0        0      615 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bg.min.js
+-rw-r--r--   0        0        0      562 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bm.min.js
+-rw-r--r--   0        0        0     1210 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bn.min.js
+-rw-r--r--   0        0        0      510 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.br.min.js
+-rw-r--r--   0        0        0      475 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bs.min.js
+-rw-r--r--   0        0        0      525 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ca.min.js
+-rw-r--r--   0        0        0      536 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.cs.min.js
+-rw-r--r--   0        0        0      433 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.cy.min.js
+-rw-r--r--   0        0        0      514 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.da.min.js
+-rw-r--r--   0        0        0      510 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.de.min.js
+-rw-r--r--   0        0        0      764 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.el.min.js
+-rw-r--r--   0        0        0      517 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-AU.min.js
+-rw-r--r--   0        0        0      518 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-CA.min.js
+-rw-r--r--   0        0        0      518 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-GB.min.js
+-rw-r--r--   0        0        0      518 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-IE.min.js
+-rw-r--r--   0        0        0      517 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-NZ.min.js
+-rw-r--r--   0        0        0      516 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-US.min.js
+-rw-r--r--   0        0        0      517 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-ZA.min.js
+-rw-r--r--   0        0        0      515 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.eo.min.js
+-rw-r--r--   0        0        0      513 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.es.min.js
+-rw-r--r--   0        0        0      537 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.et.min.js
+-rw-r--r--   0        0        0      528 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.eu.min.js
+-rw-r--r--   0        0        0      670 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fa.min.js
+-rw-r--r--   0        0        0      551 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fi.min.js
+-rw-r--r--   0        0        0      488 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fo.min.js
+-rw-r--r--   0        0        0      512 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fr-CH.min.js
+-rw-r--r--   0        0        0      536 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fr.min.js
+-rw-r--r--   0        0        0      489 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.gl.min.js
+-rw-r--r--   0        0        0      563 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.he.min.js
+-rw-r--r--   0        0        0      944 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hi.min.js
+-rw-r--r--   0        0        0      462 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hr.min.js
+-rw-r--r--   0        0        0      541 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hu.min.js
+-rw-r--r--   0        0        0      757 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hy.min.js
+-rw-r--r--   0        0        0      505 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.id.min.js
+-rw-r--r--   0        0        0      496 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.is.min.js
+-rw-r--r--   0        0        0      506 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.it-CH.min.js
+-rw-r--r--   0        0        0      525 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.it.min.js
+-rw-r--r--   0        0        0      502 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ja.min.js
+-rw-r--r--   0        0        0      970 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ka.min.js
+-rw-r--r--   0        0        0     1076 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kh.min.js
+-rw-r--r--   0        0        0      649 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kk.min.js
+-rw-r--r--   0        0        0      945 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.km.min.js
+-rw-r--r--   0        0        0      532 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ko.min.js
+-rw-r--r--   0        0        0      575 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kr.min.js
+-rw-r--r--   0        0        0      565 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.lt.min.js
+-rw-r--r--   0        0        0      526 2024-04-18 07:41:33.502393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.lv.min.js
+-rw-r--r--   0        0        0      493 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.me.min.js
+-rw-r--r--   0        0        0      657 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mk.min.js
+-rw-r--r--   0        0        0      638 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mn.min.js
+-rw-r--r--   0        0        0      990 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mr.min.js
+-rw-r--r--   0        0        0      448 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ms.min.js
+-rw-r--r--   0        0        0      522 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.nl-BE.min.js
+-rw-r--r--   0        0        0      513 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.nl.min.js
+-rw-r--r--   0        0        0      515 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.no.min.js
+-rw-r--r--   0        0        0      515 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.oc.min.js
+-rw-r--r--   0        0        0      552 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.pl.min.js
+-rw-r--r--   0        0        0      504 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.pt-BR.min.js
+-rw-r--r--   0        0        0      498 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.pt.min.js
+-rw-r--r--   0        0        0      505 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ro.min.js
+-rw-r--r--   0        0        0      662 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.rs-latin.min.js
+-rw-r--r--   0        0        0      817 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.rs.min.js
+-rw-r--r--   0        0        0      731 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ru.min.js
+-rw-r--r--   0        0        0      988 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.si.min.js
+-rw-r--r--   0        0        0      497 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sk.min.js
+-rw-r--r--   0        0        0      455 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sl.min.js
+-rw-r--r--   0        0        0      518 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sq.min.js
+-rw-r--r--   0        0        0      478 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sr-latin.min.js
+-rw-r--r--   0        0        0      651 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sr.min.js
+-rw-r--r--   0        0        0      492 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sv.min.js
+-rw-r--r--   0        0        0      431 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sw.min.js
+-rw-r--r--   0        0        0      934 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ta.min.js
+-rw-r--r--   0        0        0      700 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.tg.min.js
+-rw-r--r--   0        0        0      833 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.th.min.js
+-rw-r--r--   0        0        0      530 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.tk.min.js
+-rw-r--r--   0        0        0      495 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.tr.min.js
+-rw-r--r--   0        0        0      723 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uk.min.js
+-rw-r--r--   0        0        0      703 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uz-cyrl.min.js
+-rw-r--r--   0        0        0      516 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uz-latn.min.js
+-rw-r--r--   0        0        0      551 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.vi.min.js
+-rw-r--r--   0        0        0      613 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.zh-CN.min.js
+-rw-r--r--   0        0        0      607 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.zh-TW.min.js
+-rw-r--r--   0        0        0     7427 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/LICENSE.txt
+-rw-r--r--   0        0        0   102217 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/css/all.min.css
+-rw-r--r--   0        0        0   189684 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   109808 2024-04-18 07:41:33.506393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    63348 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    24488 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   394668 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150020 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10172 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4568 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0     1124 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/LICENSE.md
+-rw-r--r--   0        0        0    18931 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/css/select2.css
+-rw-r--r--   0        0        0    16264 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/css/select2.min.css
+-rw-r--r--   0        0        0      870 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/af.js
+-rw-r--r--   0        0        0      909 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ar.js
+-rw-r--r--   0        0        0      725 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/az.js
+-rw-r--r--   0        0        0      972 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bg.js
+-rw-r--r--   0        0        0     1295 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bn.js
+-rw-r--r--   0        0        0      969 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bs.js
+-rw-r--r--   0        0        0      904 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ca.js
+-rw-r--r--   0        0        0     1296 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/cs.js
+-rw-r--r--   0        0        0      832 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/da.js
+-rw-r--r--   0        0        0      870 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/de.js
+-rw-r--r--   0        0        0     1021 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/dsb.js
+-rw-r--r--   0        0        0     1186 2024-04-18 07:41:33.510393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/el.js
+-rw-r--r--   0        0        0      925 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/en.js
+-rw-r--r--   0        0        0      871 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/eo.js
+-rw-r--r--   0        0        0      926 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/es.js
+-rw-r--r--   0        0        0      805 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/et.js
+-rw-r--r--   0        0        0      872 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/eu.js
+-rw-r--r--   0        0        0     1027 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fa.js
+-rw-r--r--   0        0        0      807 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fi.js
+-rw-r--r--   0        0        0      981 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fr.js
+-rw-r--r--   0        0        0      928 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/gl.js
+-rw-r--r--   0        0        0      988 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/he.js
+-rw-r--r--   0        0        0     1179 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hi.js
+-rw-r--r--   0        0        0      856 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hr.js
+-rw-r--r--   0        0        0     1022 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hsb.js
+-rw-r--r--   0        0        0      923 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hu.js
+-rw-r--r--   0        0        0     1032 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hy.js
+-rw-r--r--   0        0        0      772 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/id.js
+-rw-r--r--   0        0        0      811 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/is.js
+-rw-r--r--   0        0        0      901 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/it.js
+-rw-r--r--   0        0        0      866 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ja.js
+-rw-r--r--   0        0        0     1199 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ka.js
+-rw-r--r--   0        0        0     1092 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/km.js
+-rw-r--r--   0        0        0      859 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ko.js
+-rw-r--r--   0        0        0      948 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/lt.js
+-rw-r--r--   0        0        0      904 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/lv.js
+-rw-r--r--   0        0        0     1042 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/mk.js
+-rw-r--r--   0        0        0      815 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ms.js
+-rw-r--r--   0        0        0      782 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/nb.js
+-rw-r--r--   0        0        0     1361 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ne.js
+-rw-r--r--   0        0        0      908 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/nl.js
+-rw-r--r--   0        0        0     1381 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pa.js
+-rw-r--r--   0        0        0      951 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pl.js
+-rw-r--r--   0        0        0     1053 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ps.js
+-rw-r--r--   0        0        0      880 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pt-BR.js
+-rw-r--r--   0        0        0      882 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pt.js
+-rw-r--r--   0        0        0      942 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ro.js
+-rw-r--r--   0        0        0     1175 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ru.js
+-rw-r--r--   0        0        0     1310 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sk.js
+-rw-r--r--   0        0        0      929 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sl.js
+-rw-r--r--   0        0        0      907 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sq.js
+-rw-r--r--   0        0        0     1113 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sr-Cyrl.js
+-rw-r--r--   0        0        0      984 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sr.js
+-rw-r--r--   0        0        0      790 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sv.js
+-rw-r--r--   0        0        0     1360 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/te.js
+-rw-r--r--   0        0        0     1078 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/th.js
+-rw-r--r--   0        0        0      775 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/tk.js
+-rw-r--r--   0        0        0      779 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/tr.js
+-rw-r--r--   0        0        0     1160 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/uk.js
+-rw-r--r--   0        0        0      800 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/vi.js
+-rw-r--r--   0        0        0      772 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/zh-CN.js
+-rw-r--r--   0        0        0      711 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/zh-TW.js
+-rw-r--r--   0        0        0   167106 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.full.js
+-rw-r--r--   0        0        0    76775 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.full.min.js
+-rw-r--r--   0        0        0   156955 2024-04-18 07:41:33.514393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.js
+-rw-r--r--   0        0        0    73170 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.min.js
+-rw-r--r--   0        0        0     1954 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/errors.html
+-rw-r--r--   0        0        0      614 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/flash_messages.html
+-rw-r--r--   0        0        0      522 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/footer.html
+-rw-r--r--   0        0        0     2404 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/form.html
+-rw-r--r--   0        0        0     4726 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/home.html
+-rw-r--r--   0        0        0     1935 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/layout.html
+-rw-r--r--   0        0        0      215 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/forms/cli.py
+-rw-r--r--   0        0        0     4992 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/forms/main.py
+-rw-r--r--   0        0        0     2842 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/forms/validator.py
+-rw-r--r--   0        0        0      146 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/beanhub_cli/main.py
+-rw-r--r--   0        0        0      792 2024-04-18 07:41:33.518393 beanhub_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4290 1970-01-01 00:00:00.000000 beanhub_cli-1.0.1/PKG-INFO
```

### Comparing `beanhub_cli-0.1.1/LICENSE` & `beanhub_cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/README.md` & `beanhub_cli-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - **Formatter** - Advanced Beancount file formatter based on top of [beancount-black](https://github.com/LaunchPlatform/beancount-black)
 - **Basic Beancount file manipulations** - Effortless Beancount account name renaming and other basic manipulations (coming soon)
 - **Doesn't require a BeanHub account** - While some features in the future will require a BeanHub repository to operate, but we make most of them usable even without a BeanHub account
 
 ## Screenshots
 
 <p align="center">
-  <a href="https://beanhub.io"><img src="https://github.com/LaunchPlatform/beanhub-cli/raw/master/assets/forms-screenshot.png?raw=true" alt="BeanHub Forms Screenshot" /></a>
+  <img src="https://github.com/LaunchPlatform/beanhub-cli/raw/master/assets/forms-screenshot.png?raw=true" alt="BeanHub Forms Screenshot" />
 </p>
 
 # Sponsor
 
 <p align="center">
   <a href="https://beanhub.io"><img src="https://github.com/LaunchPlatform/beanhub-cli/raw/master/assets/beanhub.svg?raw=true" alt="BeanHub logo" /></a>
 </p>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 input-with-beanhub-custom-forms/) web app locally to try out your forms -
 **Formatter** - Advanced Beancount file formatter based on top of [beancount-
 black](https://github.com/LaunchPlatform/beancount-black) - **Basic Beancount
 file manipulations** - Effortless Beancount account name renaming and other
 basic manipulations (coming soon) - **Doesn't require a BeanHub account** -
 While some features in the future will require a BeanHub repository to operate,
 but we make most of them usable even without a BeanHub account ## Screenshots
-                          _[_B_e_a_n_H_u_b_ _F_o_r_m_s_ _S_c_r_e_e_n_s_h_o_t_]
+                          [BeanHub Forms Screenshot]
 # Sponsor
                                 _[_B_e_a_n_H_u_b_ _l_o_g_o_]
 A modern accounting book service based on the most popular open source version
 control system [Git](https://git-scm.com/) and text-based double entry
 accounting book software [Beancount](https://beancount.github.io/docs/
 index.html). ## Install ```bash pip install beanhub-cli ``` ## Usage ###
 BeanHub Forms web app To make it much easier for BeanHub users to test their
```

### Comparing `beanhub_cli-0.1.1/beanhub_cli/aliase.py` & `beanhub_cli-1.0.1/beanhub_cli/aliase.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/cli.py` & `beanhub_cli-1.0.1/beanhub_cli/cli.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/environment.py` & `beanhub_cli-1.0.1/beanhub_cli/environment.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/format.py` & `beanhub_cli-1.0.1/beanhub_cli/format.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/data/sample_forms_doc.yaml` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/data/sample_forms_doc.yaml`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/deps.py` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/deps.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/helpers.py` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/helpers.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/main.py` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/main.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/routes.py` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/routes.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/settings.py` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/settings.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/js/beanhub-web-react-0.1.6.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/js/beanhub-web-react-0.1.6.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/js/beanhub-web-react-0.1.6.js.map` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/js/beanhub-web-react-0.1.6.js.map`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/LICENSE` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.css` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.css`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.css.map` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.css.map`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.min.css` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/css/bootstrap-datepicker.min.css`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/js/bootstrap-datepicker.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/js/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/js/bootstrap-datepicker.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/js/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker-en-CA.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker-en-CA.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar-DZ.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar-DZ.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar-tn.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar-tn.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ar.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.az.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.az.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bg.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bg.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bm.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bm.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bn.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.bn.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ca.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ca.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.cs.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.cs.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.da.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.da.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.el.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.el.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-AU.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-AU.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-CA.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-CA.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-GB.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-GB.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-IE.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-IE.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-NZ.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-NZ.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-US.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-US.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-ZA.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.en-ZA.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.eo.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.eo.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.es.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.es.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.et.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.et.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.eu.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.eu.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fa.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fa.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fi.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fi.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fr-CH.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fr-CH.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fr.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.fr.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.he.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.he.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hi.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hi.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hu.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hu.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hy.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.hy.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.it.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.it.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ka.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ka.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kh.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kh.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kk.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kk.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.km.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.km.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ko.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ko.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kr.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.kr.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.lt.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.lt.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.lv.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.lv.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mk.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mk.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mn.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mn.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mr.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.mr.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.nl-BE.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.nl-BE.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.nl.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.nl.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.no.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.no.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.oc.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.oc.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.pl.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.pl.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.rs-latin.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.rs-latin.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.rs.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.rs.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ru.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ru.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.si.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.si.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sq.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sq.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sr.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.sr.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ta.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.ta.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.tg.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.tg.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.th.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.th.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.tk.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.tk.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uk.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uk.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uz-cyrl.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uz-cyrl.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uz-latn.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.uz-latn.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.vi.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.vi.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.zh-CN.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.zh-CN.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.zh-TW.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/bootstrap-datepicker/locales/bootstrap-datepicker.zh-TW.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/LICENSE.txt` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/css/all.min.css` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/css/all.min.css`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-brands-400.ttf` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-brands-400.woff2` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-regular-400.ttf` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-regular-400.woff2` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-solid-900.ttf` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-solid-900.woff2` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-v4compatibility.ttf` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-v4compatibility.woff2` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/fontawesome6/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/LICENSE.md` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/css/select2.css` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/css/select2.css`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/css/select2.min.css` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/af.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/af.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ar.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/az.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/az.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bg.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bn.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bs.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ca.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/cs.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/da.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/da.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/de.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/de.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/dsb.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/el.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/el.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/en.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/en.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/eo.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/eo.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/es.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/es.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/et.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/et.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/eu.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fa.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fi.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fr.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/gl.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/he.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/he.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hi.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hr.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hsb.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hu.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hy.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/id.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/id.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/is.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/is.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/it.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/it.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ja.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ka.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/km.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/km.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ko.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/lt.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/lv.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/mk.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ms.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/nb.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ne.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/nl.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pa.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pa.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pl.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ps.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pt-BR.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pt.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ro.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ru.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sk.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sl.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sq.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sr-Cyrl.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sr.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sv.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/te.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/te.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/th.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/th.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/tk.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/tr.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/uk.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/vi.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/zh-CN.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/zh-TW.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.full.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.full.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.min.js` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/static/vendor/select2/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/errors.html` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/errors.html`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/flash_messages.html` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/flash_messages.html`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/footer.html` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/footer.html`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/form.html` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/form.html`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/home.html` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/home.html`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/app/templates/layout.html` & `beanhub_cli-1.0.1/beanhub_cli/forms/app/templates/layout.html`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/main.py` & `beanhub_cli-1.0.1/beanhub_cli/forms/main.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/beanhub_cli/forms/validator.py` & `beanhub_cli-1.0.1/beanhub_cli/forms/validator.py`

 * *Files identical despite different names*

### Comparing `beanhub_cli-0.1.1/pyproject.toml` & `beanhub_cli-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-cli"
-version = "0.1.1"
+version = "1.0.1"
 description = "Command line tools for BeanHub"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 bh = "beanhub_cli.main:cli"
@@ -12,15 +12,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^2.4.0"
 starlette-wtf = "^0.4.3"
 fastapi = ">= 0.98.0, <1.0.0"
 jinja2 = ">=3.1.2, <4.0.0"
 pyyaml = "^6.0.1"
-beancount-black = "^0.2.1"
+beancount-black = "^1.0.0"
 click = "^8.1.7"
 uvicorn = "^0.23.2"
 beanhub-forms = "^0.1.3"
 pydantic-settings = "^2.0.3"
 rich = "^13.6.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `beanhub_cli-0.1.1/PKG-INFO` & `beanhub_cli-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: beanhub-cli
-Version: 0.1.1
+Version: 1.0.1
 Summary: Command line tools for BeanHub
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beancount-black (>=0.2.1,<0.3.0)
+Requires-Dist: beancount-black (>=1.0.0,<2.0.0)
 Requires-Dist: beanhub-forms (>=0.1.3,<0.2.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: fastapi (>=0.98.0,<1.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic (>=2.4.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
@@ -33,15 +33,15 @@
 - **Formatter** - Advanced Beancount file formatter based on top of [beancount-black](https://github.com/LaunchPlatform/beancount-black)
 - **Basic Beancount file manipulations** - Effortless Beancount account name renaming and other basic manipulations (coming soon)
 - **Doesn't require a BeanHub account** - While some features in the future will require a BeanHub repository to operate, but we make most of them usable even without a BeanHub account
 
 ## Screenshots
 
 <p align="center">
-  <a href="https://beanhub.io"><img src="https://github.com/LaunchPlatform/beanhub-cli/raw/master/assets/forms-screenshot.png?raw=true" alt="BeanHub Forms Screenshot" /></a>
+  <img src="https://github.com/LaunchPlatform/beanhub-cli/raw/master/assets/forms-screenshot.png?raw=true" alt="BeanHub Forms Screenshot" />
 </p>
 
 # Sponsor
 
 <p align="center">
   <a href="https://beanhub.io"><img src="https://github.com/LaunchPlatform/beanhub-cli/raw/master/assets/beanhub.svg?raw=true" alt="BeanHub logo" /></a>
 </p>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: beanhub-cli Version: 0.1.1 Summary: Command line
+Metadata-Version: 2.1 Name: beanhub-cli Version: 1.0.1 Summary: Command line
 tools for BeanHub License: MIT Author: Fang-Pen Lin Author-email:
 fangpen@launchplatform.com Requires-Python: >=3.9,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beancount-black (>=0.2.1,<0.3.0) Requires-Dist: beanhub-forms
+Requires-Dist: beancount-black (>=1.0.0,<2.0.0) Requires-Dist: beanhub-forms
 (>=0.1.3,<0.2.0) Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist: fastapi
 (>=0.98.0,<1.0.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0) Requires-Dist:
 pydantic (>=2.4.0,<3.0.0) Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: rich (>=13.6.0,<14.0.0)
 Requires-Dist: starlette-wtf (>=0.4.3,<0.5.0) Requires-Dist: uvicorn
 (>=0.23.2,<0.24.0) Description-Content-Type: text/markdown # beanhub-cli [!
 [CircleCI](https://dl.circleci.com/status-badge/img/gh/LaunchPlatform/beanhub-
@@ -19,15 +19,15 @@
 custom-forms/) web app locally to try out your forms - **Formatter** - Advanced
 Beancount file formatter based on top of [beancount-black](https://github.com/
 LaunchPlatform/beancount-black) - **Basic Beancount file manipulations** -
 Effortless Beancount account name renaming and other basic manipulations
 (coming soon) - **Doesn't require a BeanHub account** - While some features in
 the future will require a BeanHub repository to operate, but we make most of
 them usable even without a BeanHub account ## Screenshots
-                          _[_B_e_a_n_H_u_b_ _F_o_r_m_s_ _S_c_r_e_e_n_s_h_o_t_]
+                          [BeanHub Forms Screenshot]
 # Sponsor
                                 _[_B_e_a_n_H_u_b_ _l_o_g_o_]
 A modern accounting book service based on the most popular open source version
 control system [Git](https://git-scm.com/) and text-based double entry
 accounting book software [Beancount](https://beancount.github.io/docs/
 index.html). ## Install ```bash pip install beanhub-cli ``` ## Usage ###
 BeanHub Forms web app To make it much easier for BeanHub users to test their
```
