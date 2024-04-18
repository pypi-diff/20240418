# Comparing `tmp/gnosisai-0.1-py3-none-any.whl.zip` & `tmp/gnosisai-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18305 bytes, number of entries: 46
+Zip file size: 22174 bytes, number of entries: 58
 -rw-r--r--  2.0 unx     2825 b- defN 24-Apr-18 06:07 gnosisai/README.md
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 02:14 gnosisai/__init__.py
 -rw-r--r--  2.0 unx     2327 b- defN 24-Apr-17 02:14 gnosisai/builder.py
 -rw-r--r--  2.0 unx      320 b- defN 24-Apr-18 07:28 gnosisai/correspond_file_path.yaml
 -rw-r--r--  2.0 unx     2458 b- defN 24-Apr-18 07:30 gnosisai/main.py
--rw-r--r--  2.0 unx       46 b- defN 24-Apr-18 08:35 gnosisai/requirements.txt
+-rw-r--r--  2.0 unx       41 b- defN 24-Apr-18 08:37 gnosisai/requirements.txt
 -rw-r--r--  2.0 unx      258 b- defN 24-Apr-17 02:14 gnosisai/vars.yaml
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 02:14 gnosisai/template/__init__.py
 -rw-r--r--  2.0 unx      363 b- defN 24-Apr-17 02:14 gnosisai/template/requirements.txt
 -rw-r--r--  2.0 unx      774 b- defN 24-Apr-17 02:14 gnosisai/template/run.sh
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 02:14 gnosisai/template/manifests/.gitkeep
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 02:14 gnosisai/template/models/.gitkeep
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 02:14 gnosisai/template/src/__init__.py
@@ -24,25 +24,37 @@
 -rw-r--r--  2.0 unx      622 b- defN 24-Apr-17 02:14 gnosisai/template_files/Dockerfile.j2
 -rw-r--r--  2.0 unx     1234 b- defN 24-Apr-17 02:14 gnosisai/template_files/deployment.yml.j2
 -rw-r--r--  2.0 unx      241 b- defN 24-Apr-17 02:14 gnosisai/template_files/docker-compose.yml.j2
 -rw-r--r--  2.0 unx      751 b- defN 24-Apr-17 02:14 gnosisai/template_files/makefile.j2
 -rw-r--r--  2.0 unx       58 b- defN 24-Apr-17 02:14 gnosisai/template_files/namespace.yml.j2
 -rw-r--r--  2.0 unx     2113 b- defN 24-Apr-17 02:14 gnosisai/template_files/prediction.py.j2
 -rw-r--r--  2.0 unx     1846 b- defN 24-Apr-17 02:14 gnosisai/template_files/routers.py.j2
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:35 ss/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:35 ss/src/__init__.py
+-rw-r--r--  2.0 unx      959 b- defN 24-Apr-18 08:35 ss/src/configurations.py
+-rw-r--r--  2.0 unx      610 b- defN 24-Apr-18 08:35 ss/src/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:35 ss/src/app/__init__.py
+-rw-r--r--  2.0 unx      381 b- defN 24-Apr-18 08:35 ss/src/app/app.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:35 ss/src/app/routers/__init__.py
+-rw-r--r--  2.0 unx     1817 b- defN 24-Apr-18 08:35 ss/src/app/routers/routers.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:35 ss/src/ml/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-Apr-18 08:35 ss/src/ml/prediction.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:35 ss/src/utils/__init__.py
+-rw-r--r--  2.0 unx      574 b- defN 24-Apr-18 08:35 ss/src/utils/profiler.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:31 sss/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:31 sss/src/__init__.py
 -rw-r--r--  2.0 unx      959 b- defN 24-Apr-18 08:31 sss/src/configurations.py
 -rw-r--r--  2.0 unx      610 b- defN 24-Apr-18 08:31 sss/src/constants.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:31 sss/src/app/__init__.py
 -rw-r--r--  2.0 unx      381 b- defN 24-Apr-18 08:31 sss/src/app/app.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:31 sss/src/app/routers/__init__.py
 -rw-r--r--  2.0 unx     1817 b- defN 24-Apr-18 08:31 sss/src/app/routers/routers.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:31 sss/src/ml/__init__.py
 -rw-r--r--  2.0 unx     2119 b- defN 24-Apr-18 08:31 sss/src/ml/prediction.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:31 sss/src/utils/__init__.py
 -rw-r--r--  2.0 unx      574 b- defN 24-Apr-18 08:31 sss/src/utils/profiler.py
--rw-r--r--  2.0 unx       94 b- defN 24-Apr-18 08:35 gnosisai-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 08:35 gnosisai-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 24-Apr-18 08:35 gnosisai-0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-18 08:35 gnosisai-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3891 b- defN 24-Apr-18 08:35 gnosisai-0.1.dist-info/RECORD
-46 files, 31211 bytes uncompressed, 11997 bytes compressed:  61.6%
+-rw-r--r--  2.0 unx      116 b- defN 24-Apr-18 08:41 gnosisai-0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 08:41 gnosisai-0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 24-Apr-18 08:41 gnosisai-0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-18 08:41 gnosisai-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4819 b- defN 24-Apr-18 08:41 gnosisai-0.2.dist-info/RECORD
+58 files, 38619 bytes uncompressed, 14424 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -81,14 +81,50 @@
 
 Filename: gnosisai/template_files/prediction.py.j2
 Comment: 
 
 Filename: gnosisai/template_files/routers.py.j2
 Comment: 
 
+Filename: ss/__init__.py
+Comment: 
+
+Filename: ss/src/__init__.py
+Comment: 
+
+Filename: ss/src/configurations.py
+Comment: 
+
+Filename: ss/src/constants.py
+Comment: 
+
+Filename: ss/src/app/__init__.py
+Comment: 
+
+Filename: ss/src/app/app.py
+Comment: 
+
+Filename: ss/src/app/routers/__init__.py
+Comment: 
+
+Filename: ss/src/app/routers/routers.py
+Comment: 
+
+Filename: ss/src/ml/__init__.py
+Comment: 
+
+Filename: ss/src/ml/prediction.py
+Comment: 
+
+Filename: ss/src/utils/__init__.py
+Comment: 
+
+Filename: ss/src/utils/profiler.py
+Comment: 
+
 Filename: sss/__init__.py
 Comment: 
 
 Filename: sss/src/__init__.py
 Comment: 
 
 Filename: sss/src/configurations.py
@@ -117,23 +153,23 @@
 
 Filename: sss/src/utils/__init__.py
 Comment: 
 
 Filename: sss/src/utils/profiler.py
 Comment: 
 
-Filename: gnosisai-0.1.dist-info/METADATA
+Filename: gnosisai-0.2.dist-info/METADATA
 Comment: 
 
-Filename: gnosisai-0.1.dist-info/WHEEL
+Filename: gnosisai-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: gnosisai-0.1.dist-info/entry_points.txt
+Filename: gnosisai-0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: gnosisai-0.1.dist-info/top_level.txt
+Filename: gnosisai-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: gnosisai-0.1.dist-info/RECORD
+Filename: gnosisai-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gnosisai/requirements.txt

```diff
@@ -1,4 +1,3 @@
 click>=7.1.2
 Jinja2>=2.11.2
-PyYAML>=5.3.1
-yaml
+PyYAML>=5.3.1
```

## Comparing `gnosisai-0.1.dist-info/RECORD` & `gnosisai-0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 gnosisai/README.md,sha256=EOGkTR5mXh3Y56gCMZPOv6_YMjikvvBANTuewhsNm88,2825
 gnosisai/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gnosisai/builder.py,sha256=ED6F4n2QUISyvSyEONrU1umTENJp0Q4Kq35Y9GvP8uw,2327
 gnosisai/correspond_file_path.yaml,sha256=02k2BxFaKgd_ra_ByPF3kjbAD72_thxHmxCmSV5-a8w,320
 gnosisai/main.py,sha256=zOTeMo5NNrqhqhA8ckn2Rp-JBB_gw2z38mKFWCkn4iA,2458
-gnosisai/requirements.txt,sha256=WLFKXBOmxmfVWYpApBKFijRm-Ce42tBHxIMAcm5wY7Y,46
+gnosisai/requirements.txt,sha256=8UKN98mO-GiXQfL-IyvlL1AquvkzUFuuKlLLGb7s9Ko,41
 gnosisai/vars.yaml,sha256=fH6zw0Jf60SmuUMmJsnj4t5cC8EUSp-Ojz7mg8Yy3-A,258
 gnosisai/template/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gnosisai/template/requirements.txt,sha256=lSJTK6p233gWm-LBeET7VV8yQ7P01uyHYKhiwSHaq7k,363
 gnosisai/template/run.sh,sha256=Tc5xHmly7TTxZ0hzAxRaOhR4BwkmTgIwp5v3-G91hIs,774
 gnosisai/template/manifests/.gitkeep,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gnosisai/template/models/.gitkeep,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gnosisai/template/src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -23,24 +23,36 @@
 gnosisai/template_files/Dockerfile.j2,sha256=RKRzaw1f4_OH0mcgtzYQR5itWNpBLH8oSaaUsy7kVOA,622
 gnosisai/template_files/deployment.yml.j2,sha256=8RwMmXe4lR9SOR0mSAnbvNGHdc0WjiyrRueEiSy1Lu0,1234
 gnosisai/template_files/docker-compose.yml.j2,sha256=VSMUHQBa17gVetF_HKgDwXgxcH2zFy4TkZZH7BqcIZ0,241
 gnosisai/template_files/makefile.j2,sha256=6Sn4irTug_4qzByCZeX1Wnwjr2D0vvRlA0ImfNRCRIk,751
 gnosisai/template_files/namespace.yml.j2,sha256=2Vps62kd6WFpmghOJ3G8FrzG-j2Gp6oniLSZ-ToaMvk,58
 gnosisai/template_files/prediction.py.j2,sha256=aPXWkCIRhBwgdU_wkiQgeab22sahcAwJZ0XobEeWGew,2113
 gnosisai/template_files/routers.py.j2,sha256=H6vJ8xXhXYDiKJW1xOsIaCkd-DVBNrgTIzSX5hAbUZs,1846
+ss/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ss/src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ss/src/configurations.py,sha256=_EFv13vLeVa_lEWnmttJIS2n9F8jrRZ3XoPV30MWKH4,959
+ss/src/constants.py,sha256=5I21xdxmxO5yTHb14K9T6NHX-8dTHV7rgtIFpyLKNbs,610
+ss/src/app/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ss/src/app/app.py,sha256=gQlVl1ulhh4mdPA2wWOXXUmSEAFl7vVbupRjMydC3f4,381
+ss/src/app/routers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ss/src/app/routers/routers.py,sha256=oaEUNwlElxYANfS64AddM9QeBQmPqhy0IQn88pnzc6Y,1817
+ss/src/ml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ss/src/ml/prediction.py,sha256=9mwi0Mljt2c7zsl4q_OarPlQpQlM2Wb_CAqGCmHQ6ts,2119
+ss/src/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ss/src/utils/profiler.py,sha256=7alVQiO2w5z5gMzlSw7ilMYzS0NCF4sJwhH9dC04U6c,574
 sss/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sss/src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sss/src/configurations.py,sha256=_EFv13vLeVa_lEWnmttJIS2n9F8jrRZ3XoPV30MWKH4,959
 sss/src/constants.py,sha256=5I21xdxmxO5yTHb14K9T6NHX-8dTHV7rgtIFpyLKNbs,610
 sss/src/app/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sss/src/app/app.py,sha256=gQlVl1ulhh4mdPA2wWOXXUmSEAFl7vVbupRjMydC3f4,381
 sss/src/app/routers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sss/src/app/routers/routers.py,sha256=oaEUNwlElxYANfS64AddM9QeBQmPqhy0IQn88pnzc6Y,1817
 sss/src/ml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sss/src/ml/prediction.py,sha256=9mwi0Mljt2c7zsl4q_OarPlQpQlM2Wb_CAqGCmHQ6ts,2119
 sss/src/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sss/src/utils/profiler.py,sha256=7alVQiO2w5z5gMzlSw7ilMYzS0NCF4sJwhH9dC04U6c,574
-gnosisai-0.1.dist-info/METADATA,sha256=-Xrk0XVYWBqSMpfWeWRXAoHiJokjIXPalCUQj-Q6GOs,94
-gnosisai-0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-gnosisai-0.1.dist-info/entry_points.txt,sha256=5k2OVN2B57sW4NpnFnEPfZNSHLH2QhcHS59W2epgiLE,47
-gnosisai-0.1.dist-info/top_level.txt,sha256=qutUd-UXxcVZXuYI-_FOIZMK0zREDEUPY4LcQUQ8OS8,13
-gnosisai-0.1.dist-info/RECORD,,
+gnosisai-0.2.dist-info/METADATA,sha256=AHz5Pco8vO_oUpvuy-PizglNfRvTmWxtwvIW6lPojeE,116
+gnosisai-0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+gnosisai-0.2.dist-info/entry_points.txt,sha256=5k2OVN2B57sW4NpnFnEPfZNSHLH2QhcHS59W2epgiLE,47
+gnosisai-0.2.dist-info/top_level.txt,sha256=XSgbQKL6qxQLjalKYi0GvIaMhoDsyiHAb85S5OLEfaM,16
+gnosisai-0.2.dist-info/RECORD,,
```

