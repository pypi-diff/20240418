# Comparing `tmp/RsCMPX_NiotMeas-4.0.186.tar.gz` & `tmp/RsCMPX_NiotMeas-5.0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RsCMPX_NiotMeas-4.0.186.tar", last modified: Mon Sep  4 10:18:02 2023, max compression
+gzip compressed data, was "dist\RsCMPX_NiotMeas-5.0.70.tar", last modified: Thu Apr 18 15:40:04 2024, max compression
```

## Comparing `RsCMPX_NiotMeas-4.0.186.tar` & `RsCMPX_NiotMeas-5.0.70.tar`

### file list

```diff
@@ -1,353 +1,342 @@
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.306340 RsCMPX_NiotMeas-4.0.186/
--rw-rw-rw-   0        0        0     2795 2023-09-04 10:18:02.305365 RsCMPX_NiotMeas-4.0.186/PKG-INFO
--rw-rw-rw-   0        0        0     1396 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/README.rst
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.592877 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.619228 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/CustomFiles/
--rw-rw-rw-   0        0        0       90 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/CustomFiles/__init__.py
--rw-rw-rw-   0        0        0     3725 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/CustomFiles/events.py
--rw-rw-rw-   0        0        0     4916 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/CustomFiles/reliability.py
--rw-rw-rw-   0        0        0    21864 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/CustomFiles/utilities.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.623133 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.626060 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.630941 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.641676 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.661198 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.669982 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/
--rw-rw-rw-   0        0        0     2431 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/Gsm.py
--rw-rw-rw-   0        0        0     2447 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/Utra.py
--rw-rw-rw-   0        0        0     1214 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/__init__.py
--rw-rw-rw-   0        0        0     2334 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/EvMagnitude.py
--rw-rw-rw-   0        0        0     2806 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/FreqError.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.674860 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Ibe/
--rw-rw-rw-   0        0        0     2831 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Ibe/IqOffset.py
--rw-rw-rw-   0        0        0     3452 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Ibe/__init__.py
--rw-rw-rw-   0        0        0     3110 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/IqOffset.py
--rw-rw-rw-   0        0        0     2236 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Merror.py
--rw-rw-rw-   0        0        0     3028 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Pdynamics.py
--rw-rw-rw-   0        0        0     2444 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Perror.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.680717 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/SeMask/
--rw-rw-rw-   0        0        0     4056 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/SeMask/Limit.py
--rw-rw-rw-   0        0        0     2104 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/SeMask/__init__.py
--rw-rw-rw-   0        0        0     3798 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.687549 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/
--rw-rw-rw-   0        0        0     2488 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Lrange.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.703165 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/
--rw-rw-rw-   0        0        0     4245 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Aclr.py
--rw-rw-rw-   0        0        0     2181 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Cidx.py
--rw-rw-rw-   0        0        0     4420 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Modulation.py
--rw-rw-rw-   0        0        0     3076 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SeMask.py
--rw-rw-rw-   0        0        0     6089 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Setup.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.707070 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SingleCmw/
--rw-rw-rw-   0        0        0     2175 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SingleCmw/Connector.py
--rw-rw-rw-   0        0        0     1069 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SingleCmw/__init__.py
--rw-rw-rw-   0        0        0     3081 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/__init__.py
--rw-rw-rw-   0        0        0     1536 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/SingleCmw.py
--rw-rw-rw-   0        0        0     6665 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.709997 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.714878 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/EePeriods/
--rw-rw-rw-   0        0        0     3151 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/EePeriods/Npusch.py
--rw-rw-rw-   0        0        0     1043 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/EePeriods/__init__.py
--rw-rw-rw-   0        0        0     2212 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/__init__.py
--rw-rw-rw-   0        0        0     1442 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Pdynamics.py
--rw-rw-rw-   0        0        0    22168 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Result.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.720734 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Scount/
--rw-rw-rw-   0        0        0     2828 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Scount/Spectrum.py
--rw-rw-rw-   0        0        0     3381 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Scount/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.726589 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.731470 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/Aclr/
--rw-rw-rw-   0        0        0     2237 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/Aclr/Enable.py
--rw-rw-rw-   0        0        0     1018 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/Aclr/__init__.py
--rw-rw-rw-   0        0        0     1463 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/SeMask.py
--rw-rw-rw-   0        0        0     1256 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/__init__.py
--rw-rw-rw-   0        0        0     2663 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Subcarrier.py
--rw-rw-rw-   0        0        0    21317 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.739277 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.752942 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/
--rw-rw-rw-   0        0        0     2302 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/EvMagnitude.py
--rw-rw-rw-   0        0        0     2204 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Merror.py
--rw-rw-rw-   0        0        0     2984 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Pdynamics.py
--rw-rw-rw-   0        0        0     2412 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Perror.py
--rw-rw-rw-   0        0        0     2838 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.754894 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.759776 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/EwLength/
--rw-rw-rw-   0        0        0     3427 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/EwLength/Pformat.py
--rw-rw-rw-   0        0        0     2116 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/EwLength/__init__.py
--rw-rw-rw-   0        0        0     2258 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/__init__.py
--rw-rw-rw-   0        0        0    16597 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Result.py
--rw-rw-rw-   0        0        0     2683 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Scount.py
--rw-rw-rw-   0        0        0    11283 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/__init__.py
--rw-rw-rw-   0        0        0     7131 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/RfSettings.py
--rw-rw-rw-   0        0        0     2423 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/__init__.py
--rw-rw-rw-   0        0        0     1052 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.761725 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.764654 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.773438 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/
--rw-rw-rw-   0        0        0     4481 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/Average.py
--rw-rw-rw-   0        0        0     4217 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/Current.py
--rw-rw-rw-   0        0        0     1266 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.784174 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/
--rw-rw-rw-   0        0        0     2092 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Average.py
--rw-rw-rw-   0        0        0     2092 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Current.py
--rw-rw-rw-   0        0        0     2092 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Maximum.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.795886 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/
--rw-rw-rw-   0        0        0     2128 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Average.py
--rw-rw-rw-   0        0        0     2128 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Current.py
--rw-rw-rw-   0        0        0     2128 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Maximum.py
--rw-rw-rw-   0        0        0     1512 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/__init__.py
--rw-rw-rw-   0        0        0     1766 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.798815 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.805646 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/
--rw-rw-rw-   0        0        0     2041 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Average.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.810526 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Current/
--rw-rw-rw-   0        0        0     1905 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Current/ScIndex.py
--rw-rw-rw-   0        0        0     2686 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Current/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.817359 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Extreme/
--rw-rw-rw-   0        0        0     1905 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Extreme/ScIndex.py
--rw-rw-rw-   0        0        0     2686 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Extreme/__init__.py
--rw-rw-rw-   0        0        0     2063 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/StandardDev.py
--rw-rw-rw-   0        0        0     1798 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/__init__.py
--rw-rw-rw-   0        0        0     1064 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.823215 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.826142 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.834927 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/
--rw-rw-rw-   0        0        0     2796 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/Average.py
--rw-rw-rw-   0        0        0     2796 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/Current.py
--rw-rw-rw-   0        0        0     1270 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.837854 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.845663 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/
--rw-rw-rw-   0        0        0     2527 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Average.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.850542 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Current/
--rw-rw-rw-   0        0        0     2370 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Current/ScIndex.py
--rw-rw-rw-   0        0        0     3173 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Current/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.856398 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Extreme/
--rw-rw-rw-   0        0        0     2370 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Extreme/ScIndex.py
--rw-rw-rw-   0        0        0     3173 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Extreme/__init__.py
--rw-rw-rw-   0        0        0     2549 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/StandardDev.py
--rw-rw-rw-   0        0        0     1802 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.868111 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/
--rw-rw-rw-   0        0        0     4050 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Average.py
--rw-rw-rw-   0        0        0     4050 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Current.py
--rw-rw-rw-   0        0        0     4404 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Extreme.py
--rw-rw-rw-   0        0        0     4072 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/StandardDev.py
--rw-rw-rw-   0        0        0     1820 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.880800 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/
--rw-rw-rw-   0        0        0     2333 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Average.py
--rw-rw-rw-   0        0        0     2333 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Current.py
--rw-rw-rw-   0        0        0     2461 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Extreme.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.886655 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/
--rw-rw-rw-   0        0        0     3819 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/All.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.895439 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/
--rw-rw-rw-   0        0        0     3064 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/Negativ.py
--rw-rw-rw-   0        0        0     3047 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/Positiv.py
--rw-rw-rw-   0        0        0     1289 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.904223 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/
--rw-rw-rw-   0        0        0     3070 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/Negativ.py
--rw-rw-rw-   0        0        0     3053 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/Positiv.py
--rw-rw-rw-   0        0        0     1289 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.913008 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/
--rw-rw-rw-   0        0        0     3064 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/Negativ.py
--rw-rw-rw-   0        0        0     3047 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/Positiv.py
--rw-rw-rw-   0        0        0     1289 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/__init__.py
--rw-rw-rw-   0        0        0     1738 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/__init__.py
--rw-rw-rw-   0        0        0     2355 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/StandardDev.py
--rw-rw-rw-   0        0        0     2037 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/__init__.py
--rw-rw-rw-   0        0        0     2670 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/__init__.py
--rw-rw-rw-   0        0        0     1679 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Sreliability.py
--rw-rw-rw-   0        0        0     1317 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.922767 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/
--rw-rw-rw-   0        0        0     2130 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Average.py
--rw-rw-rw-   0        0        0     2130 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Current.py
--rw-rw-rw-   0        0        0     2130 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Maximum.py
--rw-rw-rw-   0        0        0     1520 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.935456 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/
--rw-rw-rw-   0        0        0     8411 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Average.py
--rw-rw-rw-   0        0        0     8411 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Current.py
--rw-rw-rw-   0        0        0     9198 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Extreme.py
--rw-rw-rw-   0        0        0     4624 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/StandardDev.py
--rw-rw-rw-   0        0        0     1817 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.952049 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/
--rw-rw-rw-   0        0        0     5056 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Average.py
--rw-rw-rw-   0        0        0     5056 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Current.py
--rw-rw-rw-   0        0        0     5056 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Maximum.py
--rw-rw-rw-   0        0        0     5056 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Minimum.py
--rw-rw-rw-   0        0        0     3102 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/StandardDev.py
--rw-rw-rw-   0        0        0     2056 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.962785 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/
--rw-rw-rw-   0        0        0     2122 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Average.py
--rw-rw-rw-   0        0        0     2122 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Current.py
--rw-rw-rw-   0        0        0     2122 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Maximum.py
--rw-rw-rw-   0        0        0     1520 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.975472 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/
--rw-rw-rw-   0        0        0     4378 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Average.py
--rw-rw-rw-   0        0        0     4378 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Current.py
--rw-rw-rw-   0        0        0     4588 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Extreme.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.980352 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/
--rw-rw-rw-   0        0        0     3405 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/All.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.988161 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/
--rw-rw-rw-   0        0        0     2580 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/Negativ.py
--rw-rw-rw-   0        0        0     2563 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/Positiv.py
--rw-rw-rw-   0        0        0     1285 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.995970 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/
--rw-rw-rw-   0        0        0     2586 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/Negativ.py
--rw-rw-rw-   0        0        0     2569 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/Positiv.py
--rw-rw-rw-   0        0        0     1285 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.004753 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/
--rw-rw-rw-   0        0        0     2580 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/Negativ.py
--rw-rw-rw-   0        0        0     2563 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/Positiv.py
--rw-rw-rw-   0        0        0     1285 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/__init__.py
--rw-rw-rw-   0        0        0     2731 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/StandardDev.py
--rw-rw-rw-   0        0        0     2033 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.009632 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/State/
--rw-rw-rw-   0        0        0     2099 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/State/All.py
--rw-rw-rw-   0        0        0     2746 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/State/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.023296 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.032082 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/
--rw-rw-rw-   0        0        0     2598 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/Average.py
--rw-rw-rw-   0        0        0     2598 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/Current.py
--rw-rw-rw-   0        0        0     1268 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.042817 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/
--rw-rw-rw-   0        0        0     1906 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Average.py
--rw-rw-rw-   0        0        0     1906 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Current.py
--rw-rw-rw-   0        0        0     1906 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Maximum.py
--rw-rw-rw-   0        0        0     1537 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/__init__.py
--rw-rw-rw-   0        0        0     2085 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Iemissions.py
--rw-rw-rw-   0        0        0     1738 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Iq.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.052577 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/
--rw-rw-rw-   0        0        0     2360 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Average.py
--rw-rw-rw-   0        0        0     2360 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Current.py
--rw-rw-rw-   0        0        0     2360 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Maximum.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.064289 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/
--rw-rw-rw-   0        0        0     2384 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Average.py
--rw-rw-rw-   0        0        0     2384 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Current.py
--rw-rw-rw-   0        0        0     2384 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Maximum.py
--rw-rw-rw-   0        0        0     1514 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/__init__.py
--rw-rw-rw-   0        0        0     1758 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/__init__.py
--rw-rw-rw-   0        0        0     2025 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pmonitor.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.075025 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/
--rw-rw-rw-   0        0        0     2302 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Average.py
--rw-rw-rw-   0        0        0     2302 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Current.py
--rw-rw-rw-   0        0        0     2302 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Maximum.py
--rw-rw-rw-   0        0        0     1522 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/__init__.py
--rw-rw-rw-   0        0        0     2484 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/__init__.py
--rw-rw-rw-   0        0        0     7156 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.078929 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.093570 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/
--rw-rw-rw-   0        0        0     8825 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Average.py
--rw-rw-rw-   0        0        0     8825 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Current.py
--rw-rw-rw-   0        0        0     9406 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Extreme.py
--rw-rw-rw-   0        0        0     6387 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Preamble.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.098450 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/ScsGroup/
--rw-rw-rw-   0        0        0     3532 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/ScsGroup/Preamble.py
--rw-rw-rw-   0        0        0     2592 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/ScsGroup/__init__.py
--rw-rw-rw-   0        0        0     4833 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/StandardDev.py
--rw-rw-rw-   0        0        0     2321 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.115042 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/
--rw-rw-rw-   0        0        0     4982 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Average.py
--rw-rw-rw-   0        0        0     4982 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Current.py
--rw-rw-rw-   0        0        0     4982 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Maximum.py
--rw-rw-rw-   0        0        0     4982 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Minimum.py
--rw-rw-rw-   0        0        0     3057 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/StandardDev.py
--rw-rw-rw-   0        0        0     2056 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.120898 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/State/
--rw-rw-rw-   0        0        0     2083 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/State/All.py
--rw-rw-rw-   0        0        0     2730 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/State/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.131635 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/
--rw-rw-rw-   0        0        0     1937 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/EvPreamble.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.141394 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/
--rw-rw-rw-   0        0        0     2144 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Average.py
--rw-rw-rw-   0        0        0     2144 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Current.py
--rw-rw-rw-   0        0        0     2144 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Maximum.py
--rw-rw-rw-   0        0        0     1507 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/__init__.py
--rw-rw-rw-   0        0        0     1708 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Iq.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.151154 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/
--rw-rw-rw-   0        0        0     2166 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Average.py
--rw-rw-rw-   0        0        0     2166 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Current.py
--rw-rw-rw-   0        0        0     2166 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Maximum.py
--rw-rw-rw-   0        0        0     1522 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.160915 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/
--rw-rw-rw-   0        0        0     2390 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Average.py
--rw-rw-rw-   0        0        0     2390 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Current.py
--rw-rw-rw-   0        0        0     2390 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Maximum.py
--rw-rw-rw-   0        0        0     1537 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.172626 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/
--rw-rw-rw-   0        0        0     2154 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Average.py
--rw-rw-rw-   0        0        0     2154 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Current.py
--rw-rw-rw-   0        0        0     2154 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Maximum.py
--rw-rw-rw-   0        0        0     1522 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/__init__.py
--rw-rw-rw-   0        0        0     1945 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/PvPreamble.py
--rw-rw-rw-   0        0        0     2468 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/__init__.py
--rw-rw-rw-   0        0        0     5330 2023-09-04 10:17:58.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-09-04 10:17:57.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.174579 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Route/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.177506 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Route/NiotMeas/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.188243 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Route/NiotMeas/Scenario/
--rw-rw-rw-   0        0        0     2146 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Route/NiotMeas/Scenario/CombinedSignalPath.py
--rw-rw-rw-   0        0        0      889 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Route/NiotMeas/Scenario/MaProtocol.py
--rw-rw-rw-   0        0        0     2303 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Route/NiotMeas/Scenario/Salone.py
--rw-rw-rw-   0        0        0     2130 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Route/NiotMeas/Scenario/__init__.py
--rw-rw-rw-   0        0        0     2426 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Route/NiotMeas/__init__.py
--rw-rw-rw-   0        0        0     1031 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Route/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.190196 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Sense/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.195074 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/
--rw-rw-rw-   0        0        0      850 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/MultiEval.py
--rw-rw-rw-   0        0        0     1056 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/__init__.py
--rw-rw-rw-   0        0        0     1031 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Sense/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.198003 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.199955 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.207763 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/
--rw-rw-rw-   0        0        0     1043 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     2467 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/ListPy.py
--rw-rw-rw-   0        0        0     8424 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.212643 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/Prach/
--rw-rw-rw-   0        0        0     1023 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/Prach/Catalog.py
--rw-rw-rw-   0        0        0     6866 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/Prach/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/__init__.py
--rw-rw-rw-   0        0        0     1042 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:02.302436 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/
--rw-rw-rw-   0        0        0      586 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgLinkedEventArgs.py
--rw-rw-rw-   0        0        0     4165 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgSingle.py
--rw-rw-rw-   0        0        0     1116 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgSingleList.py
--rw-rw-rw-   0        0        0     1145 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgSingleSuppressed.py
--rw-rw-rw-   0        0        0     9097 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgStringComposer.py
--rw-rw-rw-   0        0        0     5751 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgStruct.py
--rw-rw-rw-   0        0        0     3439 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgStructList.py
--rw-rw-rw-   0        0        0     2546 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgStructStringParser.py
--rw-rw-rw-   0        0        0     5238 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/CommandsGroup.py
--rw-rw-rw-   0        0        0    25317 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/Conversions.py
--rw-rw-rw-   0        0        0     3775 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ConverterFromScpiString.py
--rw-rw-rw-   0        0        0     4768 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ConverterToScpiString.py
--rw-rw-rw-   0        0        0    12939 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/Core.py
--rw-rw-rw-   0        0        0     1386 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/GlobalData.py
--rw-rw-rw-   0        0        0    59853 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/Instrument.py
--rw-rw-rw-   0        0        0     4785 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/InstrumentErrors.py
--rw-rw-rw-   0        0        0     2225 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/InstrumentOptions.py
--rw-rw-rw-   0        0        0    13241 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/InstrumentSettings.py
--rw-rw-rw-   0        0        0     3518 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/InternalLinker.py
--rw-rw-rw-   0        0        0     4390 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/IoTransferEventArgs.py
--rw-rw-rw-   0        0        0     4289 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/RepeatedCapability.py
--rw-rw-rw-   0        0        0     4745 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ScpiEnums.py
--rw-rw-rw-   0        0        0    35058 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ScpiLogger.py
--rw-rw-rw-   0        0        0     5098 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/StreamReader.py
--rw-rw-rw-   0        0        0     5856 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/StreamWriter.py
--rw-rw-rw-   0        0        0     1114 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/StructBase.py
--rw-rw-rw-   0        0        0     3608 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/Types.py
--rw-rw-rw-   0        0        0     5498 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/Utilities.py
--rw-rw-rw-   0        0        0     5632 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/VisaPluginSocketIo.py
--rw-rw-rw-   0        0        0    50075 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/VisaSession.py
--rw-rw-rw-   0        0        0     7361 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/VisaSessionSim.py
--rw-rw-rw-   0        0        0       29 2023-07-13 05:46:50.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/__init__.py
--rw-rw-rw-   0        0        0    12888 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/RsCMPX_NiotMeas.py
--rw-rw-rw-   0        0        0      943 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/__init__.py
--rw-rw-rw-   0        0        0     7110 2023-09-04 10:17:56.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/enums.py
--rw-rw-rw-   0        0        0    29398 2023-09-04 10:17:55.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/repcap.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:18:01.606542 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas.egg-info/
--rw-rw-rw-   0        0        0     2795 2023-09-04 10:18:01.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19018 2023-09-04 10:18:01.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-04 10:18:01.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-09-04 10:18:01.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-09-04 10:18:01.000000 RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-04 10:18:02.306340 RsCMPX_NiotMeas-4.0.186/setup.cfg
--rw-rw-rw-   0        0        0     1497 2023-09-04 10:17:59.000000 RsCMPX_NiotMeas-4.0.186/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.929853 RsCMPX_NiotMeas-5.0.70/
+-rw-rw-rw-   0        0        0     2864 2024-04-18 15:40:04.914450 RsCMPX_NiotMeas-5.0.70/PKG-INFO
+-rw-rw-rw-   0        0        0     1439 2024-04-18 15:40:02.000000 RsCMPX_NiotMeas-5.0.70/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.041093 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.065862 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/CustomFiles/
+-rw-rw-rw-   0        0        0       90 2024-04-18 15:40:02.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/CustomFiles/__init__.py
+-rw-rw-rw-   0        0        0     3725 2024-04-18 15:40:02.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/CustomFiles/events.py
+-rw-rw-rw-   0        0        0     4916 2024-04-18 15:40:02.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/CustomFiles/reliability.py
+-rw-rw-rw-   0        0        0    21864 2024-04-18 15:40:02.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/CustomFiles/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.065862 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.075857 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.075857 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.104566 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.114603 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.129567 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/
+-rw-rw-rw-   0        0        0     2431 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/Gsm.py
+-rw-rw-rw-   0        0        0     2447 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/Utra.py
+-rw-rw-rw-   0        0        0     1214 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/__init__.py
+-rw-rw-rw-   0        0        0     2334 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/EvMagnitude.py
+-rw-rw-rw-   0        0        0     2806 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/FreqError.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.139561 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Ibe/
+-rw-rw-rw-   0        0        0     2831 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Ibe/IqOffset.py
+-rw-rw-rw-   0        0        0     3452 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Ibe/__init__.py
+-rw-rw-rw-   0        0        0     3110 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/IqOffset.py
+-rw-rw-rw-   0        0        0     2236 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Merror.py
+-rw-rw-rw-   0        0        0     3028 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Pdynamics.py
+-rw-rw-rw-   0        0        0     2444 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Perror.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.139561 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/SeMask/
+-rw-rw-rw-   0        0        0     4056 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/SeMask/Limit.py
+-rw-rw-rw-   0        0        0     2104 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/SeMask/__init__.py
+-rw-rw-rw-   0        0        0     3798 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.149553 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/
+-rw-rw-rw-   0        0        0     2488 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Lrange.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.169544 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/
+-rw-rw-rw-   0        0        0     4245 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Aclr.py
+-rw-rw-rw-   0        0        0     2181 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Cidx.py
+-rw-rw-rw-   0        0        0     4420 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Modulation.py
+-rw-rw-rw-   0        0        0     3076 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SeMask.py
+-rw-rw-rw-   0        0        0     6102 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.169544 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SingleCmw/
+-rw-rw-rw-   0        0        0     2175 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SingleCmw/Connector.py
+-rw-rw-rw-   0        0        0     1069 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SingleCmw/__init__.py
+-rw-rw-rw-   0        0        0     3081 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/__init__.py
+-rw-rw-rw-   0        0        0     1536 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/SingleCmw.py
+-rw-rw-rw-   0        0        0     6665 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.179540 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.179540 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/EePeriods/
+-rw-rw-rw-   0        0        0     3151 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/EePeriods/Npusch.py
+-rw-rw-rw-   0        0        0     1043 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/EePeriods/__init__.py
+-rw-rw-rw-   0        0        0     2212 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/__init__.py
+-rw-rw-rw-   0        0        0     1442 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Pdynamics.py
+-rw-rw-rw-   0        0        0    22168 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Result.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.189532 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Scount/
+-rw-rw-rw-   0        0        0     2828 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Scount/Spectrum.py
+-rw-rw-rw-   0        0        0     3381 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Scount/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.196038 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.196038 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/Aclr/
+-rw-rw-rw-   0        0        0     2237 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/Aclr/Enable.py
+-rw-rw-rw-   0        0        0     1018 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/Aclr/__init__.py
+-rw-rw-rw-   0        0        0     1463 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/SeMask.py
+-rw-rw-rw-   0        0        0     1256 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/__init__.py
+-rw-rw-rw-   0        0        0     2663 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Subcarrier.py
+-rw-rw-rw-   0        0        0    21309 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.213048 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.263163 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/
+-rw-rw-rw-   0        0        0     2302 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/EvMagnitude.py
+-rw-rw-rw-   0        0        0     2204 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Merror.py
+-rw-rw-rw-   0        0        0     2984 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Pdynamics.py
+-rw-rw-rw-   0        0        0     2412 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Perror.py
+-rw-rw-rw-   0        0        0     2838 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.263163 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.277531 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/EwLength/
+-rw-rw-rw-   0        0        0     3427 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/EwLength/Pformat.py
+-rw-rw-rw-   0        0        0     2116 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/EwLength/__init__.py
+-rw-rw-rw-   0        0        0     2258 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/__init__.py
+-rw-rw-rw-   0        0        0    16597 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Result.py
+-rw-rw-rw-   0        0        0     2683 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Scount.py
+-rw-rw-rw-   0        0        0    11275 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/__init__.py
+-rw-rw-rw-   0        0        0     7183 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/RfSettings.py
+-rw-rw-rw-   0        0        0     2423 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.281521 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.292019 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.308031 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/
+-rw-rw-rw-   0        0        0     4481 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/Average.py
+-rw-rw-rw-   0        0        0     4217 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/Current.py
+-rw-rw-rw-   0        0        0     1266 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.318028 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/
+-rw-rw-rw-   0        0        0     2092 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Average.py
+-rw-rw-rw-   0        0        0     2092 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Current.py
+-rw-rw-rw-   0        0        0     2092 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Maximum.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.329534 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/
+-rw-rw-rw-   0        0        0     2128 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Average.py
+-rw-rw-rw-   0        0        0     2128 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Current.py
+-rw-rw-rw-   0        0        0     2128 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     1512 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/__init__.py
+-rw-rw-rw-   0        0        0     1766 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.339534 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.346048 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/
+-rw-rw-rw-   0        0        0     2041 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Average.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.349604 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Current/
+-rw-rw-rw-   0        0        0     1905 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Current/ScIndex.py
+-rw-rw-rw-   0        0        0     2686 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Current/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.359557 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Extreme/
+-rw-rw-rw-   0        0        0     1905 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Extreme/ScIndex.py
+-rw-rw-rw-   0        0        0     2686 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Extreme/__init__.py
+-rw-rw-rw-   0        0        0     2063 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/StandardDev.py
+-rw-rw-rw-   0        0        0     1798 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/__init__.py
+-rw-rw-rw-   0        0        0     1064 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.359557 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.369552 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.379437 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/
+-rw-rw-rw-   0        0        0     2796 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/Average.py
+-rw-rw-rw-   0        0        0     2796 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/Current.py
+-rw-rw-rw-   0        0        0     1270 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.379437 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.396448 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/
+-rw-rw-rw-   0        0        0     2527 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Average.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.406446 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Current/
+-rw-rw-rw-   0        0        0     2370 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Current/ScIndex.py
+-rw-rw-rw-   0        0        0     3173 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Current/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.412952 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Extreme/
+-rw-rw-rw-   0        0        0     2370 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Extreme/ScIndex.py
+-rw-rw-rw-   0        0        0     3173 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Extreme/__init__.py
+-rw-rw-rw-   0        0        0     2549 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/StandardDev.py
+-rw-rw-rw-   0        0        0     1802 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/__init__.py
+-rw-rw-rw-   0        0        0     1068 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.429460 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/
+-rw-rw-rw-   0        0        0     4050 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Average.py
+-rw-rw-rw-   0        0        0     4050 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Current.py
+-rw-rw-rw-   0        0        0     4404 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Extreme.py
+-rw-rw-rw-   0        0        0     4072 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/StandardDev.py
+-rw-rw-rw-   0        0        0     1820 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.449503 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/
+-rw-rw-rw-   0        0        0     2333 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Average.py
+-rw-rw-rw-   0        0        0     2333 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Current.py
+-rw-rw-rw-   0        0        0     2461 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Extreme.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.449503 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/
+-rw-rw-rw-   0        0        0     3819 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/All.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.465288 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/
+-rw-rw-rw-   0        0        0     3064 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/Negativ.py
+-rw-rw-rw-   0        0        0     3047 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/Positiv.py
+-rw-rw-rw-   0        0        0     1289 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.467007 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/
+-rw-rw-rw-   0        0        0     3070 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/Negativ.py
+-rw-rw-rw-   0        0        0     3053 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/Positiv.py
+-rw-rw-rw-   0        0        0     1289 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.477003 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/
+-rw-rw-rw-   0        0        0     3064 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/Negativ.py
+-rw-rw-rw-   0        0        0     3047 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/Positiv.py
+-rw-rw-rw-   0        0        0     1289 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/__init__.py
+-rw-rw-rw-   0        0        0     1738 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/__init__.py
+-rw-rw-rw-   0        0        0     2355 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/StandardDev.py
+-rw-rw-rw-   0        0        0     2037 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/__init__.py
+-rw-rw-rw-   0        0        0     2670 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/__init__.py
+-rw-rw-rw-   0        0        0     1679 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Sreliability.py
+-rw-rw-rw-   0        0        0     1317 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.486997 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/
+-rw-rw-rw-   0        0        0     2130 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Average.py
+-rw-rw-rw-   0        0        0     2130 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Current.py
+-rw-rw-rw-   0        0        0     2130 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Maximum.py
+-rw-rw-rw-   0        0        0     1520 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.497696 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/
+-rw-rw-rw-   0        0        0     8411 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Average.py
+-rw-rw-rw-   0        0        0     8411 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Current.py
+-rw-rw-rw-   0        0        0     9198 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Extreme.py
+-rw-rw-rw-   0        0        0     4624 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/StandardDev.py
+-rw-rw-rw-   0        0        0     1817 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.532752 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/
+-rw-rw-rw-   0        0        0     5056 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Average.py
+-rw-rw-rw-   0        0        0     5056 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Current.py
+-rw-rw-rw-   0        0        0     5056 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Maximum.py
+-rw-rw-rw-   0        0        0     5056 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Minimum.py
+-rw-rw-rw-   0        0        0     3102 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/StandardDev.py
+-rw-rw-rw-   0        0        0     2056 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.543724 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/
+-rw-rw-rw-   0        0        0     2122 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Average.py
+-rw-rw-rw-   0        0        0     2122 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Current.py
+-rw-rw-rw-   0        0        0     2122 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Maximum.py
+-rw-rw-rw-   0        0        0     1520 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.563000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/
+-rw-rw-rw-   0        0        0     4378 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Average.py
+-rw-rw-rw-   0        0        0     4378 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Current.py
+-rw-rw-rw-   0        0        0     4588 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Extreme.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.565035 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/
+-rw-rw-rw-   0        0        0     3405 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/All.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.565035 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/
+-rw-rw-rw-   0        0        0     2580 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/Negativ.py
+-rw-rw-rw-   0        0        0     2563 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/Positiv.py
+-rw-rw-rw-   0        0        0     1285 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.579813 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/
+-rw-rw-rw-   0        0        0     2586 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/Negativ.py
+-rw-rw-rw-   0        0        0     2569 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/Positiv.py
+-rw-rw-rw-   0        0        0     1285 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.589814 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/
+-rw-rw-rw-   0        0        0     2580 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/Negativ.py
+-rw-rw-rw-   0        0        0     2563 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/Positiv.py
+-rw-rw-rw-   0        0        0     1285 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/__init__.py
+-rw-rw-rw-   0        0        0     1734 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/__init__.py
+-rw-rw-rw-   0        0        0     2731 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/StandardDev.py
+-rw-rw-rw-   0        0        0     2033 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.596319 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/State/
+-rw-rw-rw-   0        0        0     2099 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/State/All.py
+-rw-rw-rw-   0        0        0     2746 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/State/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.606319 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.613063 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/
+-rw-rw-rw-   0        0        0     2598 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/Average.py
+-rw-rw-rw-   0        0        0     2598 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/Current.py
+-rw-rw-rw-   0        0        0     1268 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.623063 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/
+-rw-rw-rw-   0        0        0     1906 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Average.py
+-rw-rw-rw-   0        0        0     1906 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Current.py
+-rw-rw-rw-   0        0        0     1906 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Maximum.py
+-rw-rw-rw-   0        0        0     1537 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/__init__.py
+-rw-rw-rw-   0        0        0     2085 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Iemissions.py
+-rw-rw-rw-   0        0        0     1738 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Iq.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.639568 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/
+-rw-rw-rw-   0        0        0     2360 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Average.py
+-rw-rw-rw-   0        0        0     2360 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Current.py
+-rw-rw-rw-   0        0        0     2360 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Maximum.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.650100 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/
+-rw-rw-rw-   0        0        0     2384 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Average.py
+-rw-rw-rw-   0        0        0     2384 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Current.py
+-rw-rw-rw-   0        0        0     2384 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Maximum.py
+-rw-rw-rw-   0        0        0     1514 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/__init__.py
+-rw-rw-rw-   0        0        0     1758 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/__init__.py
+-rw-rw-rw-   0        0        0     2025 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pmonitor.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.660071 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/
+-rw-rw-rw-   0        0        0     2302 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Average.py
+-rw-rw-rw-   0        0        0     2302 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Current.py
+-rw-rw-rw-   0        0        0     2302 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Maximum.py
+-rw-rw-rw-   0        0        0     1522 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/__init__.py
+-rw-rw-rw-   0        0        0     2484 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/__init__.py
+-rw-rw-rw-   0        0        0     7152 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.676118 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.696399 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/
+-rw-rw-rw-   0        0        0     8825 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Average.py
+-rw-rw-rw-   0        0        0     8825 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Current.py
+-rw-rw-rw-   0        0        0     9406 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Extreme.py
+-rw-rw-rw-   0        0        0     6387 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Preamble.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.699507 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/ScsGroup/
+-rw-rw-rw-   0        0        0     3532 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/ScsGroup/Preamble.py
+-rw-rw-rw-   0        0        0     2592 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/ScsGroup/__init__.py
+-rw-rw-rw-   0        0        0     4833 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/StandardDev.py
+-rw-rw-rw-   0        0        0     2321 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.719495 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/
+-rw-rw-rw-   0        0        0     4982 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Average.py
+-rw-rw-rw-   0        0        0     4982 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Current.py
+-rw-rw-rw-   0        0        0     4982 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Maximum.py
+-rw-rw-rw-   0        0        0     4982 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Minimum.py
+-rw-rw-rw-   0        0        0     3057 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/StandardDev.py
+-rw-rw-rw-   0        0        0     2056 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.735118 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/State/
+-rw-rw-rw-   0        0        0     2083 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/State/All.py
+-rw-rw-rw-   0        0        0     2730 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/State/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.744092 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/
+-rw-rw-rw-   0        0        0     1937 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/EvPreamble.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.758373 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/
+-rw-rw-rw-   0        0        0     2144 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Average.py
+-rw-rw-rw-   0        0        0     2144 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Current.py
+-rw-rw-rw-   0        0        0     2144 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Maximum.py
+-rw-rw-rw-   0        0        0     1507 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/__init__.py
+-rw-rw-rw-   0        0        0     1708 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Iq.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.764418 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/
+-rw-rw-rw-   0        0        0     2166 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Average.py
+-rw-rw-rw-   0        0        0     2166 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Current.py
+-rw-rw-rw-   0        0        0     2166 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Maximum.py
+-rw-rw-rw-   0        0        0     1522 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.774413 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/
+-rw-rw-rw-   0        0        0     2390 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Average.py
+-rw-rw-rw-   0        0        0     2390 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Current.py
+-rw-rw-rw-   0        0        0     2390 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Maximum.py
+-rw-rw-rw-   0        0        0     1537 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.794402 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/
+-rw-rw-rw-   0        0        0     2154 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Average.py
+-rw-rw-rw-   0        0        0     2154 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Current.py
+-rw-rw-rw-   0        0        0     2154 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Maximum.py
+-rw-rw-rw-   0        0        0     1522 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/__init__.py
+-rw-rw-rw-   0        0        0     1945 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/PvPreamble.py
+-rw-rw-rw-   0        0        0     2468 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/__init__.py
+-rw-rw-rw-   0        0        0     5326 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/__init__.py
+-rw-rw-rw-   0        0        0     1285 2024-04-18 15:40:00.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.794402 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Sense/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.804398 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/
+-rw-rw-rw-   0        0        0      850 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/MultiEval.py
+-rw-rw-rw-   0        0        0     1056 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/__init__.py
+-rw-rw-rw-   0        0        0     1031 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Sense/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.804398 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.812904 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.822903 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/
+-rw-rw-rw-   0        0        0     2467 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/ListPy.py
+-rw-rw-rw-   0        0        0     6711 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     4920 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/Prach.py
+-rw-rw-rw-   0        0        0     1285 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/__init__.py
+-rw-rw-rw-   0        0        0     1042 2024-04-18 15:40:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.914450 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/
+-rw-rw-rw-   0        0        0      586 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgLinkedEventArgs.py
+-rw-rw-rw-   0        0        0     4165 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgSingle.py
+-rw-rw-rw-   0        0        0     1116 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgSingleList.py
+-rw-rw-rw-   0        0        0     1145 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgSingleSuppressed.py
+-rw-rw-rw-   0        0        0     9097 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgStringComposer.py
+-rw-rw-rw-   0        0        0     5751 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgStruct.py
+-rw-rw-rw-   0        0        0     3439 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgStructList.py
+-rw-rw-rw-   0        0        0     2546 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgStructStringParser.py
+-rw-rw-rw-   0        0        0     5238 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/CommandsGroup.py
+-rw-rw-rw-   0        0        0    25419 2024-04-03 11:15:31.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Conversions.py
+-rw-rw-rw-   0        0        0     3775 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ConverterFromScpiString.py
+-rw-rw-rw-   0        0        0     4768 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ConverterToScpiString.py
+-rw-rw-rw-   0        0        0    14213 2024-04-03 11:15:31.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Core.py
+-rw-rw-rw-   0        0        0     1386 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/GlobalData.py
+-rw-rw-rw-   0        0        0    60862 2024-04-03 11:15:31.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Instrument.py
+-rw-rw-rw-   0        0        0     4785 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/InstrumentErrors.py
+-rw-rw-rw-   0        0        0     2225 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/InstrumentOptions.py
+-rw-rw-rw-   0        0        0    16156 2024-04-03 11:15:31.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/InstrumentSettings.py
+-rw-rw-rw-   0        0        0     3518 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/InternalLinker.py
+-rw-rw-rw-   0        0        0     4390 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/IoTransferEventArgs.py
+-rw-rw-rw-   0        0        0      387 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Properties.py
+-rw-rw-rw-   0        0        0     4289 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/RepeatedCapability.py
+-rw-rw-rw-   0        0        0     4745 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ScpiEnums.py
+-rw-rw-rw-   0        0        0    35525 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ScpiLogger.py
+-rw-rw-rw-   0        0        0     5098 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/StreamReader.py
+-rw-rw-rw-   0        0        0     5856 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/StreamWriter.py
+-rw-rw-rw-   0        0        0     1114 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/StructBase.py
+-rw-rw-rw-   0        0        0     3608 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Types.py
+-rw-rw-rw-   0        0        0     5498 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Utilities.py
+-rw-rw-rw-   0        0        0     5716 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/VisaPluginSocketIo.py
+-rw-rw-rw-   0        0        0    51976 2024-04-03 11:15:31.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/VisaSession.py
+-rw-rw-rw-   0        0        0     7512 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/VisaSessionSim.py
+-rw-rw-rw-   0        0        0       29 2024-02-28 16:27:53.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/__init__.py
+-rw-rw-rw-   0        0        0    12822 2024-04-18 15:40:02.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/RsCMPX_NiotMeas.py
+-rw-rw-rw-   0        0        0      941 2024-04-18 15:40:02.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/__init__.py
+-rw-rw-rw-   0        0        0     4607 2024-04-18 15:39:59.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/enums.py
+-rw-rw-rw-   0        0        0    29398 2024-04-18 15:39:57.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/repcap.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:40:04.055763 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas.egg-info/
+-rw-rw-rw-   0        0        0     2864 2024-04-18 15:40:03.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18521 2024-04-18 15:40:03.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 15:40:03.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-18 15:40:03.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-18 15:40:03.000000 RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 15:40:04.929853 RsCMPX_NiotMeas-5.0.70/setup.cfg
+-rw-rw-rw-   0        0        0     1496 2024-04-18 15:40:02.000000 RsCMPX_NiotMeas-5.0.70/setup.py
```

### Comparing `RsCMPX_NiotMeas-4.0.186/PKG-INFO` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: RsCMPX_NiotMeas
-Version: 4.0.186
+Name: RsCMPX-NiotMeas
+Version: 5.0.70
 Summary: CMP180 Narrowband IoT Measurement Remote-control module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 License: MIT
 Description: ==================================
          RsCMPX_NiotMeas
         ==================================
@@ -44,15 +44,18 @@
         
         Examples: https://github.com/Rohde-Schwarz/Examples/
         
         
         Version history
         ----------------
         
-        	Latest release notes summary: Fixed documentation
+        	Latest release notes summary: Update for FW 5.0.70
+        
+        	Version 5.0.70
+        		- Update for FW 5.0.70
         
         	Version 4.0.186
         		- Fixed documentation
         
         	Version 4.0.185
         		- First released version for FW 4.0.185
```

### Comparing `RsCMPX_NiotMeas-4.0.186/README.rst` & `RsCMPX_NiotMeas-5.0.70/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 Examples: https://github.com/Rohde-Schwarz/Examples/
 
 
 Version history
 ----------------
 
-	Latest release notes summary: Fixed documentation
+	Latest release notes summary: Update for FW 5.0.70
+
+	Version 5.0.70
+		- Update for FW 5.0.70
 
 	Version 4.0.186
 		- Fixed documentation
 
 	Version 4.0.185
 		- First released version for FW 4.0.185
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/CustomFiles/events.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/CustomFiles/events.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/CustomFiles/reliability.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/CustomFiles/reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/CustomFiles/utilities.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/CustomFiles/utilities.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/Gsm.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/Gsm.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/Utra.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/Utra.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Aclr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/EvMagnitude.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/EvMagnitude.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/FreqError.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/FreqError.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Ibe/IqOffset.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Ibe/IqOffset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Ibe/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Ibe/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/IqOffset.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/IqOffset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Merror.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Merror.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Pdynamics.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Pdynamics.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Perror.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/Perror.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/SeMask/Limit.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/SeMask/Limit.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/SeMask/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/SeMask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Limit/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Lrange.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Lrange.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Aclr.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Aclr.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Cidx.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Cidx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Modulation.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Modulation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SeMask.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SeMask.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Setup.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("setup", core, parent)
 
 	# noinspection PyTypeChecker
 	class SetupStruct(StructBase):
 		"""Structure for setting input parameters. Fields: \n
 			- Segment_Length: int: Number of slots in the segment
-			- Level: float: Expected nominal power in the segment. The range can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+			- Level: float: Expected nominal power in the segment. The range can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the specifications document.
 			- Band: enums.Band: No parameter help available
 			- Frequency: float: Carrier center frequency used in the segment
 			- Npusch_Format: enums.NpuschFormat: Format of the NPUSCH.
 			- Nof_Subcarrier: int: Number of subcarriers per resource unit The allowed values have dependencies, see 'Resource unit allocation'.
 			- Start_Sc: int: Offset of the first allocated subcarrier from the edge of the transmission bandwidth For a subcarrier spacing of 3.75 kHz / 15 kHz, n equals 48 / 12.
 			- Nof_Ru_S: enums.NofRsrcUnits: Number of resource units allocated for the NPUSCH
 			- Nof_Repetitions: enums.NofRepetitionsList: Number of NPUSCH repetitions: 1, 2, 4, ..., 512, 1024, 2048
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SingleCmw/Connector.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SingleCmw/Connector.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SingleCmw/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/SingleCmw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/Segment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/SingleCmw.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/SingleCmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/EePeriods/Npusch.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/EePeriods/Npusch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/EePeriods/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/EePeriods/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Pdynamics.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Pdynamics.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Result.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Result.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Scount/Spectrum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Scount/Spectrum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Scount/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Scount/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/Aclr/Enable.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/Aclr/Enable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/Aclr/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/Aclr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/SeMask.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/SeMask.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Subcarrier.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/Subcarrier.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/MultiEval/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,24 +206,24 @@
 		"""
 		param = Conversions.enum_scalar_to_str(stop_condition, enums.StopCondition)
 		self._core.io.write(f'CONFigure:NIOT:MEASurement<Instance>:MEValuation:SCONdition {param}')
 
 	def get_mo_exception(self) -> bool:
 		"""SCPI: CONFigure:NIOT:MEASurement<Instance>:MEValuation:MOEXception \n
 		Snippet: value: bool = driver.configure.niotMeas.multiEval.get_mo_exception() \n
-		Specifies whether measurement results that the R&S CMP180 identifies as faulty or inaccurate are rejected. \n
+		Specifies whether measurement results that the CMP180 identifies as faulty or inaccurate are rejected. \n
 			:return: meas_on_exception: OFF: Faulty results are rejected ON: Results are never rejected
 		"""
 		response = self._core.io.query_str('CONFigure:NIOT:MEASurement<Instance>:MEValuation:MOEXception?')
 		return Conversions.str_to_bool(response)
 
 	def set_mo_exception(self, meas_on_exception: bool) -> None:
 		"""SCPI: CONFigure:NIOT:MEASurement<Instance>:MEValuation:MOEXception \n
 		Snippet: driver.configure.niotMeas.multiEval.set_mo_exception(meas_on_exception = False) \n
-		Specifies whether measurement results that the R&S CMP180 identifies as faulty or inaccurate are rejected. \n
+		Specifies whether measurement results that the CMP180 identifies as faulty or inaccurate are rejected. \n
 			:param meas_on_exception: OFF: Faulty results are rejected ON: Results are never rejected
 		"""
 		param = Conversions.bool_to_str(meas_on_exception)
 		self._core.io.write(f'CONFigure:NIOT:MEASurement<Instance>:MEValuation:MOEXception {param}')
 
 	# noinspection PyTypeChecker
 	def get_cprefix(self) -> enums.CyclicPrefix:
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/EvMagnitude.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/EvMagnitude.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Merror.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Merror.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Pdynamics.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Pdynamics.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Perror.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/Perror.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Limit/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/EwLength/Pformat.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/EwLength/Pformat.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/EwLength/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/EwLength/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Result.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Result.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Scount.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/Scount.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/Prach/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,24 +117,24 @@
 		"""
 		param = Conversions.enum_scalar_to_str(stop_condition, enums.StopCondition)
 		self._core.io.write(f'CONFigure:NIOT:MEASurement<Instance>:PRACh:SCONdition {param}')
 
 	def get_mo_exception(self) -> bool:
 		"""SCPI: CONFigure:NIOT:MEASurement<Instance>:PRACh:MOEXception \n
 		Snippet: value: bool = driver.configure.niotMeas.prach.get_mo_exception() \n
-		Specifies whether measurement results that the R&S CMP180 identifies as faulty or inaccurate are rejected. \n
+		Specifies whether measurement results that the CMP180 identifies as faulty or inaccurate are rejected. \n
 			:return: meas_on_exception: OFF: Faulty results are rejected ON: Results are never rejected
 		"""
 		response = self._core.io.query_str('CONFigure:NIOT:MEASurement<Instance>:PRACh:MOEXception?')
 		return Conversions.str_to_bool(response)
 
 	def set_mo_exception(self, meas_on_exception: bool) -> None:
 		"""SCPI: CONFigure:NIOT:MEASurement<Instance>:PRACh:MOEXception \n
 		Snippet: driver.configure.niotMeas.prach.set_mo_exception(meas_on_exception = False) \n
-		Specifies whether measurement results that the R&S CMP180 identifies as faulty or inaccurate are rejected. \n
+		Specifies whether measurement results that the CMP180 identifies as faulty or inaccurate are rejected. \n
 			:param meas_on_exception: OFF: Faulty results are rejected ON: Results are never rejected
 		"""
 		param = Conversions.bool_to_str(meas_on_exception)
 		self._core.io.write(f'CONFigure:NIOT:MEASurement<Instance>:PRACh:MOEXception {param}')
 
 	def get_pformat(self) -> int:
 		"""SCPI: CONFigure:NIOT:MEASurement<Instance>:PRACh:PFORmat \n
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/RfSettings.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/RfSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,45 +30,45 @@
 		self._core.io.write(f'CONFigure:NIOT:MEASurement<Instance>:RFSettings:EATTenuation {param}')
 
 	def get_umargin(self) -> float:
 		"""SCPI: CONFigure:NIOT:MEASurement<Instance>:RFSettings:UMARgin \n
 		Snippet: value: float = driver.configure.niotMeas.rfSettings.get_umargin() \n
 		Sets the margin that the measurement adds to the expected nominal power to determine the reference power. The reference
 		power minus the external input attenuation must be within the power range of the selected input connector. Refer to the
-		data sheet. \n
+		specifications document. \n
 			:return: user_margin: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:NIOT:MEASurement<Instance>:RFSettings:UMARgin?')
 		return Conversions.str_to_float(response)
 
 	def set_umargin(self, user_margin: float) -> None:
 		"""SCPI: CONFigure:NIOT:MEASurement<Instance>:RFSettings:UMARgin \n
 		Snippet: driver.configure.niotMeas.rfSettings.set_umargin(user_margin = 1.0) \n
 		Sets the margin that the measurement adds to the expected nominal power to determine the reference power. The reference
 		power minus the external input attenuation must be within the power range of the selected input connector. Refer to the
-		data sheet. \n
+		specifications document. \n
 			:param user_margin: No help available
 		"""
 		param = Conversions.decimal_value_to_str(user_margin)
 		self._core.io.write(f'CONFigure:NIOT:MEASurement<Instance>:RFSettings:UMARgin {param}')
 
 	def get_envelope_power(self) -> float:
 		"""SCPI: CONFigure:NIOT:MEASurement<Instance>:RFSettings:ENPower \n
 		Snippet: value: float = driver.configure.niotMeas.rfSettings.get_envelope_power() \n
 		Sets the expected nominal power of the measured RF signal. \n
-			:return: exp_nom_pow: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+			:return: exp_nom_pow: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the specifications document.
 		"""
 		response = self._core.io.query_str('CONFigure:NIOT:MEASurement<Instance>:RFSettings:ENPower?')
 		return Conversions.str_to_float(response)
 
 	def set_envelope_power(self, exp_nom_pow: float) -> None:
 		"""SCPI: CONFigure:NIOT:MEASurement<Instance>:RFSettings:ENPower \n
 		Snippet: driver.configure.niotMeas.rfSettings.set_envelope_power(exp_nom_pow = 1.0) \n
 		Sets the expected nominal power of the measured RF signal. \n
-			:param exp_nom_pow: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+			:param exp_nom_pow: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the specifications document.
 		"""
 		param = Conversions.decimal_value_to_str(exp_nom_pow)
 		self._core.io.write(f'CONFigure:NIOT:MEASurement<Instance>:RFSettings:ENPower {param}')
 
 	def get_frequency(self) -> float:
 		"""SCPI: CONFigure:NIOT:MEASurement<Instance>:RFSettings:FREQuency \n
 		Snippet: value: float = driver.configure.niotMeas.rfSettings.get_frequency() \n
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/NiotMeas/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Configure/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Configure/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Aclr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/EvMagnitude/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Current/ScIndex.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Current/ScIndex.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Current/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Current/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Extreme/ScIndex.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Extreme/ScIndex.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Extreme/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/Extreme/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/StandardDev.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/Margin/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/InbandEmission/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Aclr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Current/ScIndex.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Current/ScIndex.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Current/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Current/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Extreme/ScIndex.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Extreme/ScIndex.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Extreme/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/Extreme/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/StandardDev.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/Margin/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/InbandEmission/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Extreme.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/StandardDev.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Extreme.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/All.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/Negativ.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/Negativ.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/Positiv.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/Positiv.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Average/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/Negativ.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/Negativ.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/Positiv.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/Positiv.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Current/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/Negativ.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/Negativ.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/Positiv.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/Positiv.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/Minimum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/Margin/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/StandardDev.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/SeMask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Segment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Sreliability.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/Sreliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Merror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Extreme.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/StandardDev.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Minimum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/StandardDev.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Pdynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Perror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Extreme.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/All.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/Negativ.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/Negativ.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/Positiv.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/Positiv.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Average/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/Negativ.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/Negativ.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/Positiv.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/Positiv.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Current/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/Negativ.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/Negativ.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/Positiv.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/Positiv.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/Minimum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/Margin/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/StandardDev.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/SeMask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/State/All.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/State/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Aclr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/EvmSymbol/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Iemissions.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Iemissions.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Iq.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Iq.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/Post/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pdynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pmonitor.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/Pmonitor.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/SeMask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/Trace/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/MultiEval/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,49 +97,49 @@
 			from .ListPy import ListPyCls
 			self._listPy = ListPyCls(self._core, self._cmd_group)
 		return self._listPy
 
 	def initiate(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: INITiate:NIOT:MEASurement<Instance>:MEValuation \n
 		Snippet: driver.niotMeas.multiEval.initiate() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'INITiate:NIOT:MEASurement<Instance>:MEValuation', opc_timeout_ms)
 
 	def stop(self) -> None:
 		"""SCPI: STOP:NIOT:MEASurement<Instance>:MEValuation \n
 		Snippet: driver.niotMeas.multiEval.stop() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 		"""
 		self._core.io.write(f'STOP:NIOT:MEASurement<Instance>:MEValuation')
 
 	def stop_with_opc(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: STOP:NIOT:MEASurement<Instance>:MEValuation \n
 		Snippet: driver.niotMeas.multiEval.stop_with_opc() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 		Same as stop, but waits for the operation to complete before continuing further. Use the RsCMPX_NiotMeas.utilities.opc_timeout_set() to set the timeout value. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'STOP:NIOT:MEASurement<Instance>:MEValuation', opc_timeout_ms)
 
 	def abort(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: ABORt:NIOT:MEASurement<Instance>:MEValuation \n
 		Snippet: driver.niotMeas.multiEval.abort() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'ABORt:NIOT:MEASurement<Instance>:MEValuation', opc_timeout_ms)
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Extreme.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Preamble.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/Preamble.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/ScsGroup/Preamble.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/ScsGroup/Preamble.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/ScsGroup/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/ScsGroup/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/StandardDev.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Minimum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/StandardDev.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Pdynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/State/All.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/State/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/EvPreamble.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/EvPreamble.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Evm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Iq.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Iq.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Merror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Average.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Current.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Maximum.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/PvPreamble.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/PvPreamble.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,49 +41,49 @@
 			from .Pdynamics import PdynamicsCls
 			self._pdynamics = PdynamicsCls(self._core, self._cmd_group)
 		return self._pdynamics
 
 	def initiate(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: INITiate:NIOT:MEASurement<Instance>:PRACh \n
 		Snippet: driver.niotMeas.prach.initiate() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'INITiate:NIOT:MEASurement<Instance>:PRACh', opc_timeout_ms)
 
 	def stop(self) -> None:
 		"""SCPI: STOP:NIOT:MEASurement<Instance>:PRACh \n
 		Snippet: driver.niotMeas.prach.stop() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 		"""
 		self._core.io.write(f'STOP:NIOT:MEASurement<Instance>:PRACh')
 
 	def stop_with_opc(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: STOP:NIOT:MEASurement<Instance>:PRACh \n
 		Snippet: driver.niotMeas.prach.stop_with_opc() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 		Same as stop, but waits for the operation to complete before continuing further. Use the RsCMPX_NiotMeas.utilities.opc_timeout_set() to set the timeout value. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'STOP:NIOT:MEASurement<Instance>:PRACh', opc_timeout_ms)
 
 	def abort(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: ABORt:NIOT:MEASurement<Instance>:PRACh \n
 		Snippet: driver.niotMeas.prach.abort() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'ABORt:NIOT:MEASurement<Instance>:PRACh', opc_timeout_ms)
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/NiotMeas/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/NiotMeas/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Route/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Sense/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class RouteCls:
-	"""Route commands group definition. 5 total commands, 1 Subgroups, 0 group commands"""
+class SenseCls:
+	"""Sense commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("route", core, parent)
+		self._cmd_group = CommandsGroup("sense", core, parent)
 
 	@property
 	def niotMeas(self):
-		"""niotMeas commands group. 1 Sub-classes, 1 commands."""
+		"""niotMeas commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_niotMeas'):
 			from .NiotMeas import NiotMeasCls
 			self._niotMeas = NiotMeasCls(self._core, self._cmd_group)
 		return self._niotMeas
 
-	def clone(self) -> 'RouteCls':
+	def clone(self) -> 'SenseCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = RouteCls(self._core, self._cmd_group.parent)
+		new_group = SenseCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/MultiEval.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/MultiEval.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Sense/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class SenseCls:
-	"""Sense commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
+class NiotMeasCls:
+	"""NiotMeas commands group definition. 10 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("sense", core, parent)
+		self._cmd_group = CommandsGroup("niotMeas", core, parent)
 
 	@property
-	def niotMeas(self):
-		"""niotMeas commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_niotMeas'):
-			from .NiotMeas import NiotMeasCls
-			self._niotMeas = NiotMeasCls(self._core, self._cmd_group)
-		return self._niotMeas
+	def multiEval(self):
+		"""multiEval commands group. 1 Sub-classes, 5 commands."""
+		if not hasattr(self, '_multiEval'):
+			from .MultiEval import MultiEvalCls
+			self._multiEval = MultiEvalCls(self._core, self._cmd_group)
+		return self._multiEval
 
-	def clone(self) -> 'SenseCls':
+	@property
+	def prach(self):
+		"""prach commands group. 0 Sub-classes, 4 commands."""
+		if not hasattr(self, '_prach'):
+			from .Prach import PrachCls
+			self._prach = PrachCls(self._core, self._cmd_group)
+		return self._prach
+
+	def clone(self) -> 'NiotMeasCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = SenseCls(self._core, self._cmd_group.parent)
+		new_group = NiotMeasCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/ListPy.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/ListPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,29 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
-from .....Internal.Utilities import trim_str_response
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class MultiEvalCls:
-	"""MultiEval commands group definition. 8 total commands, 2 Subgroups, 6 group commands"""
+	"""MultiEval commands group definition. 6 total commands, 1 Subgroups, 5 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("multiEval", core, parent)
 
 	@property
-	def catalog(self):
-		"""catalog commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_catalog'):
-			from .Catalog import CatalogCls
-			self._catalog = CatalogCls(self._core, self._cmd_group)
-		return self._catalog
-
-	@property
 	def listPy(self):
 		"""listPy commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_listPy'):
 			from .ListPy import ListPyCls
 			self._listPy = ListPyCls(self._core, self._cmd_group)
 		return self._listPy
 
-	def get_source(self) -> str:
-		"""SCPI: TRIGger:NIOT:MEASurement<Instance>:MEValuation:SOURce \n
-		Snippet: value: str = driver.trigger.niotMeas.multiEval.get_source() \n
-		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
-		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
-		:CATalog:SOURce?. \n
-			:return: source:
-				- 'Free Run (No Sync) ': Free run without synchronization
-				- 'IF Power': Power trigger (received RF power) """
-		response = self._core.io.query_str('TRIGger:NIOT:MEASurement<Instance>:MEValuation:SOURce?')
-		return trim_str_response(response)
-
-	def set_source(self, source: str) -> None:
-		"""SCPI: TRIGger:NIOT:MEASurement<Instance>:MEValuation:SOURce \n
-		Snippet: driver.trigger.niotMeas.multiEval.set_source(source = '1') \n
-		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
-		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
-		:CATalog:SOURce?. \n
-			:param source:
-				- 'Free Run (No Sync) ': Free run without synchronization
-				- 'IF Power': Power trigger (received RF power) """
-		param = Conversions.value_to_quoted_str(source)
-		self._core.io.write(f'TRIGger:NIOT:MEASurement<Instance>:MEValuation:SOURce {param}')
-
 	def get_threshold(self) -> float or bool:
 		"""SCPI: TRIGger:NIOT:MEASurement<Instance>:MEValuation:THReshold \n
 		Snippet: value: float or bool = driver.trigger.niotMeas.multiEval.get_threshold() \n
 		Defines the trigger threshold for power trigger sources. \n
 			:return: trig_threshold: (float or boolean) No help available
 		"""
 		response = self._core.io.query_str('TRIGger:NIOT:MEASurement<Instance>:MEValuation:THReshold?')
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Implementations/Trigger/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class NiotMeasCls:
-	"""NiotMeas commands group definition. 14 total commands, 2 Subgroups, 0 group commands"""
+class TriggerCls:
+	"""Trigger commands group definition. 10 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("niotMeas", core, parent)
+		self._cmd_group = CommandsGroup("trigger", core, parent)
 
 	@property
-	def multiEval(self):
-		"""multiEval commands group. 2 Sub-classes, 6 commands."""
-		if not hasattr(self, '_multiEval'):
-			from .MultiEval import MultiEvalCls
-			self._multiEval = MultiEvalCls(self._core, self._cmd_group)
-		return self._multiEval
+	def niotMeas(self):
+		"""niotMeas commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_niotMeas'):
+			from .NiotMeas import NiotMeasCls
+			self._niotMeas = NiotMeasCls(self._core, self._cmd_group)
+		return self._niotMeas
 
-	@property
-	def prach(self):
-		"""prach commands group. 1 Sub-classes, 5 commands."""
-		if not hasattr(self, '_prach'):
-			from .Prach import PrachCls
-			self._prach = PrachCls(self._core, self._cmd_group)
-		return self._prach
-
-	def clone(self) -> 'NiotMeasCls':
+	def clone(self) -> 'TriggerCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = NiotMeasCls(self._core, self._cmd_group.parent)
+		new_group = TriggerCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgLinkedEventArgs.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgLinkedEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgSingle.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgSingle.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgSingleList.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgSingleList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgSingleSuppressed.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgSingleSuppressed.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgStringComposer.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgStringComposer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgStruct.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgStruct.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgStructList.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgStructList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ArgStructStringParser.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ArgStructStringParser.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/CommandsGroup.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/CommandsGroup.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/Conversions.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import math
 import struct
 import sys
 from enum import Enum
 from typing import List, Tuple
 from .ScpiEnums import ScpiEnum, enum_spec_prefixes, enum_spec_strings
+from .Properties import Properties
 from datetime import datetime
 
 from . import Utilities
 from .InstrumentErrors import RsInstrException
 
 
 class BinFloatFormat(Enum):
@@ -198,19 +199,20 @@
 
 
 number_plus_inf_lookup = frozenset(['Inf', 'INF', 'INFINITY', '+Inf', '+INF', '+inf', '+INFINITY', '+Infinity', '+infinity'])
 number_minus_inf_lookup = frozenset(['-Inf', '-INF', '-inf', '-INFINITY', '-Infinity', '-infinity'])
 number_nan_lookup = frozenset(['Nan', 'NAN', 'nan', 'NaN', 'NAV', 'NaV', 'NCAP', 'INV', 'NONE', 'none', 'None', 'DTX', 'UND', 'und'])
 number_max_lookup = frozenset(['OFL', 'ofl', 'Ofl'])
 number_min_lookup = frozenset(['UFL', 'ufl', 'Ufl'])
-number_si_suffix = {'pHz': 1E-12, 'MHz': 1E+6, 'kHz': 1E+3, 'GHz': 1E+9, 'mHz': 1E-3, 'uHz': 1E-6, 'µHz': 1E-6, 'THz': 1E+12, 'nHz': 1E-9, 'ns': 1E-9, 'fW': 1E-15,
-					'pW': 1E-12, 'nW': 1E-9, 'uW': 1E-6, 'µW': 1E-6, 'mW': 1E-3, 'kW': 1E3, 'MW': 1E6, 'GW': 1E9, 'MV': 1E+6, 'MA': 1E+6, 'ps': 1E-12, 'fs': 1E-15,
-					'km': 1E+3, 'kV': 1E+3, 'kA': 1E+3, 'pF': 1E-2, 'Hz': 1.0, 'mm': 1E-3, 'mA': 1E-3, 'mF': 1E-3, 'mV': 1E-3, 'pV': 1E-12, 'nF': 1E-9, 'nA': 1E-9,
-					'nV': 1E-9, 'nm': 1E-9, 'pm': 1E-12, 'us': 1E-6, 'µs': 1E-6, 'uF': 1E-6, 'µF': 1E-6, 'ms': 1E-3, 'uA': 1E-6, 'µA': 1E-6, 'uV': 1E-6, 'µV': 1E-6,
-					'um': 1E-6, 'µm': 1E-6, 'pA': 1E-12, 'V': 1, 'W': 1, 'A': 1, 'F': 1, 's': 1, 'm': 1}
+number_si_suffix = {
+	'pHz': 1E-12, 'MHz': 1E+6, 'kHz': 1E+3, 'GHz': 1E+9, 'mHz': 1E-3, 'uHz': 1E-6, 'µHz': 1E-6, 'THz': 1E+12, 'nHz': 1E-9, 'ns': 1E-9, 'fW': 1E-15,
+	'pW': 1E-12, 'nW': 1E-9, 'uW': 1E-6, 'µW': 1E-6, 'mW': 1E-3, 'kW': 1E3, 'MW': 1E6, 'GW': 1E9, 'MV': 1E+6, 'MA': 1E+6, 'ps': 1E-12, 'fs': 1E-15,
+	'km': 1E+3, 'kV': 1E+3, 'kA': 1E+3, 'pF': 1E-2, 'Hz': 1.0, 'mm': 1E-3, 'mA': 1E-3, 'mF': 1E-3, 'mV': 1E-3, 'pV': 1E-12, 'nF': 1E-9, 'nA': 1E-9,
+	'nV': 1E-9, 'nm': 1E-9, 'pm': 1E-12, 'us': 1E-6, 'µs': 1E-6, 'uF': 1E-6, 'µF': 1E-6, 'ms': 1E-3, 'uA': 1E-6, 'µA': 1E-6, 'uV': 1E-6, 'µV': 1E-6,
+	'um': 1E-6, 'µm': 1E-6, 'pA': 1E-12, 'V': 1, 'W': 1, 'A': 1, 'F': 1, 's': 1, 'm': 1}
 int_neg_inf = -(sys.maxsize - 1)
 
 
 def strip_si_suffix(string: str) -> Tuple[bool, str, float]:
 	"""Tries to find defined suffixes in the text and returns the stripped text and the multiplier as double number.
 	If no known suffix is detected, the method returns false, strippedText=text, multiplier=1.0
 	Example: text='123 MHz' strippedText='123' multiplier=1E6"""
@@ -362,15 +364,15 @@
 	else:
 		raise RsInstrException(f"bool_to_str: unsupported variable type '{type(value)}', value '{value}'. Only boolean values are supported.")
 
 
 def str_enclose_by_quotes(string: str) -> str:
 	"""Returns string enclosed by single quotes."""
 	assert_string_data(string)
-	return "'" + string + "'"
+	return Properties.scpi_quotes + string + Properties.scpi_quotes
 
 
 def list_to_csv_str(value: List, delimiter: str = ',') -> str:
 	"""Converts list of elements to strings separated by commas.
 	Element types can differ on an individual basis.
 	Supported element types:
 	- int
@@ -480,15 +482,15 @@
 	"""Converts scalar value to string enclosed by single quotes.
 	Supported element types:
 	- int
 	- bool
 	- float
 	- string
 	- enum"""
-	return f"'{value_to_str(x)}'"
+	return Properties.scpi_quotes + value_to_str(x) + Properties.scpi_quotes
 
 
 def str_to_float_list(string: str) -> List[float]:
 	"""Converts string with comma-separated values to list of Floats."""
 	assert_string_data(string)
 	if not string:
 		return []
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ConverterFromScpiString.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ConverterFromScpiString.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ConverterToScpiString.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ConverterToScpiString.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/Core.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Core.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,40 @@
 from typing import Callable
 
 from . import InstrumentOptions as Options
 from .ArgSingle import ArgSingle
 from .ArgSingleList import ArgSingleList
 from .Conversions import BinFloatFormat, BinIntFormat
 from .Instrument import Instrument
-from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode
+from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode, OpcSyncQueryMechanism
 from .ScpiLogger import LoggingMode
 from .InstrumentErrors import RsInstrException
+from .Properties import Properties
 
 
 class Core(object):
 	"""Main driver component. Provides: \n
 		- Main core constructor
 		- 'io' interface for all the write / query operations
 		- Command parameters string composer for single arguments...
 		- Link handlers adding / changing / deleting
 
 		Version history:
 
+		1.70.0 (27.02.2024)
+			- Added settings profile 'XK41' for R&S Software Defined Radios.
+			- Added settings 'FirstCmds' where you can send the defined commands right after the init. Send more commands in a row with ';;' separator.
+			- Added settings 'EachCmdPrefix' - this prefix is added to each command sent to the instrument. Supported values are also 'lf', 'cr', 'tab'
+
+		1.60.0 (31.01.2024)
+			- Added Properties script for global properties.
+			- Added Properties.scpi_quotes, string option settings token: 'ScpiQuotes'. Example: ScpiQuotes=double. Default: Single
+			- Fixed VisaPluginSocketIo read() method for cases where the session is lost. The method now generates exception in that case.
+			- Added settings 'OpcSyncQueryMechanism' with values: Standard, AlsoCheckMav, ClsOnlyCheckMavErrQueue, OnlyCheckMavErrQueue
+
 		1.54.0 (27.06.2023)
 			- Added new options profile for ATS chambers.
 			- Added settings boolean token EachCmdAsQuery. Example: EachCmdAsQuery=True. Default: False
 
 		1.53.0 (18.10.2022)
 			- Improved mode where the instrument works with a session from another object.
 			- Silently ignoring invalid *IDN? string.
@@ -175,15 +187,15 @@
 			reset: bool = False,
 			driver_options: str = None,
 			user_options: str = None,
 			direct_session: object = None):
 		"""Initializes new driver session. For cleaner code, use the class methods: \n
 		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
 
-		self.core_version = '1.54.0'
+		self.core_version = '1.55.0'
 		self.resource_name = resource_name
 
 		# Typical settings for the Core
 		self._instrumentSettings = InstrumentSettings(
 			InstrViClearMode.execute_on_all,  # Instrument viClear mode
 			False,  # Full model name. True: SMW200A, False: SMW
 			0,  # Delay by each write
@@ -193,15 +205,17 @@
 			30000,  # OPC timeout
 			10000,  # VISA timeout
 			60000,  # Self-test timeout
 			Options.ParseMode.Auto,  # *OPT? response parsing mode
 			BinFloatFormat.Single_4bytes,  # Format for parsing of binary float numbers
 			BinIntFormat.Integer32_4bytes,  # Format for parsing of binary integer numbers
 			False,  # OPC query after each setting
-			LoggingMode.Off  # Logging mode
+			LoggingMode.Off,
+			OpcSyncQueryMechanism.only_check_mav_err_queue
+			# Logging mode
 		)
 
 		self._instrumentSettings.apply_option_settings(driver_options)
 		self._instrumentSettings.apply_option_settings(user_options)
 
 		self.simulating = self._instrumentSettings.simulating
 		self.supported_idn_patterns = self._instrumentSettings.supported_idn_patterns
@@ -212,14 +226,15 @@
 		self.io = Instrument(self.resource_name, self.simulating, self._instrumentSettings, handle)
 		self.io.query_instr_status = True
 		# Update the resource name if it changed, for example because of the direct session
 		self.resource_name = self.io.resource_name
 		self.allow_reconnect = self.io.allow_reconnect
 
 		self._apply_settings_to_instrument(self._instrumentSettings)
+		self._apply_global_properties(self._instrumentSettings)
 		self.io.set_simulating_cmds()
 
 		if id_query:
 			self.io.fits_idn_pattern(self.supported_idn_patterns, self.supported_instr_models)
 
 		if reset:
 			self.io.reset()
@@ -275,14 +290,20 @@
 	def _apply_settings_to_instrument(self, settings: InstrumentSettings) -> None:
 		"""Applies settings relevant for the Instrument from the InstrumentSettings structure."""
 		if settings.instrument_status_check is not None:
 			self.io.query_instr_status = settings.instrument_status_check
 		if self.simulating and settings.instrument_simulation_idn_string is not None:
 			self.io.idn_string = settings.instrument_simulation_idn_string
 
+	@staticmethod
+	def _apply_global_properties(settings: InstrumentSettings) -> None:
+		"""Applies settings valid for the entire module. All are available in the module 'Properties'."""
+		if settings.scpi_quotes is not None:
+			Properties.scpi_quotes = settings.scpi_quotes
+
 	def compose_cmd_arg_param(
 			self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None) -> str:
 		"""Composes command parameter string based on the single argument definition."""
 		return self._args_single_list.compose_cmd_string(arg1, arg2, arg3, arg4, arg5, arg6)
 
 	def get_last_sent_cmd(self) -> str:
 		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/GlobalData.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/GlobalData.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/Instrument.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,21 +86,34 @@
 
 			self._set_session(VisaSession(resource_name, self._settings, direct_session))
 			self._init_logger(self._session.resource_name)
 			self._log_start_segment(direct_start_time)
 
 			self._lock = self._session.get_lock()
 			with self._lock:
-				self._session.clear_before_read()
-				self.idn_string = Utilities.trim_str_response(self._session.query_str(self._session.cmd_idn)).strip()
+				self.idn_string = ''
+				if len(self._session.cmd_idn) > 0:
+					self._session.clear_before_read()
+					resp = Utilities.trim_str_response(self._session.query_str(self._session.cmd_idn)).strip()
+					if settings.idn_custom_parse:
+						sr = settings.idn_custom_parse.split('->')
+						search = sr[0]
+						replace = sr[1]
+						resp = re.sub(search, replace, resp)
+					self.idn_string = resp
+				else:
+					self.idn_string = "Rohde&Schwarz,DefaultDevice,100001,1.00"
+
 				# NRP-Z session coercing
 				if self._session.is_rsnrp_session():
 					self._settings.instr_options_parse_mode = InstrumentOptions.ParseMode.Skip
 					self.stb_in_error_check = False
+
 				self.instr_options_parse_mode = self._settings.instr_options_parse_mode
+
 			self._log_info('Session init', f"Device{dir_str} '{self.resource_name}' IDN: {self.idn_string}")
 
 		except RsInstrException as e:
 			if not self.logger:
 				self._assure_logger_exists()
 				self._log_start_segment(direct_start_time)
 			self._log_error('Session init error', e.args[0], self._start_time, datetime.now())
@@ -385,14 +398,24 @@
 		self._session.visa_timeout = value
 
 	@property
 	def data_chunk_size(self) -> int:
 		"""Returns max chunk size of one data block."""
 		return self._session.data_chunk_size
 
+	@property
+	def opc_sync_query_mechanism(self) -> InstrumentSettings.OpcSyncQueryMechanism:
+		"""Returns the current setting of the OPC-Sync query mechanism."""
+		return self._session.opc_sync_query_mechanism
+
+	@opc_sync_query_mechanism.setter
+	def opc_sync_query_mechanism(self, mechanism: InstrumentSettings.OpcSyncQueryMechanism) -> None:
+		"""Sets the current setting of the OPC-Sync query mechanism."""
+		self._session.opc_sync_query_mechanism = mechanism
+
 	@data_chunk_size.setter
 	def data_chunk_size(self, chunk_size: int) -> None:
 		"""Sets the maximum size of one block transferred during write/read operations."""
 		self._session.data_chunk_size = int(chunk_size)
 
 	# noinspection PyMethodMayBeStatic
 	def _sim_cached_value_found(self, value) -> bool:
@@ -435,15 +458,16 @@
 		if items_count >= 4:
 			self.firmware_version = Utilities.trim_str_response(items[3].strip())
 
 	def fits_idn_pattern(self, patterns: List[str], supported_models: List[str]) -> None:
 		"""Throws exception if the current instrument model does not fit  any of the patterns.
 		The supported_models argument is only used for exception messages"""
 		matches = False
-		assert self._idn_string, f'*IDN? was not assigned yet.'
+		if not self._idn_string:
+			return
 		for x in patterns:
 			matches = re.search(x, self.idn_string, re.IGNORECASE)
 			if matches:
 				break
 		if not matches:
 			message = f"Instrument is not supported.\n*IDN? string: '{self.idn_string}'"
 			if len(supported_models) > 0:
@@ -723,15 +747,16 @@
 			try:
 				self._log_start_segment()
 				query = self._replace_global_repcaps(query)
 				self.start_send_read_event(query, True)
 				self._call_pre_query_handler(query, block_callback)
 				response = self._session.query_str_with_opc(query, timeout, log_info)
 				self.end_send_read_event()
-				self._session.query_and_clear_esr()
+				if self._session.clear_status_after_query_with_opc():
+					self._session.query_and_clear_esr()
 				self._log_info(log_info, f'{query} {response}')
 				self.check_status()
 			except RsInstrException as e:
 				self._log_exception(e, log_info)
 				raise
 			finally:
 				self._log_end_segment()
@@ -818,15 +843,16 @@
 
 					self._log_start_segment()
 					query = self._replace_global_repcaps(query)
 					self.start_send_read_event(query, True)
 					self._call_pre_query_handler(query, False)
 					self._session.query_bin_block_with_opc(query, stream, True, timeout)
 					self.end_send_read_event()
-					self._session.query_and_clear_esr()
+					if self._session.clear_status_after_query_with_opc():
+						self._session.query_and_clear_esr()
 					add_str = 'target file' if append is False else 'appended to target file'
 					self._log_info(log_info, f'Query {query} - written {size_to_kb_mb_string(stream.written_len, True)}, {add_str} {file_path}')
 					self.check_status()
 				except RsInstrException as e:
 					self._log_exception(e, log_info)
 					raise
 				finally:
@@ -1047,15 +1073,16 @@
 					return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
 				if stream.binary:
 					result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
 					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result)
 				else:
 					result = Conv.str_to_float_list(stream.content)
 					self._log_info_list(f'{log_info}, received ascii format list', result)
-				self._session.query_and_clear_esr()
+				if self._session.clear_status_after_query_with_opc():
+					self._session.query_and_clear_esr()
 				self.check_status()
 				return result
 			except RsInstrException as e:
 				self._log_exception(e, log_info)
 				raise
 			finally:
 				self._log_end_segment()
@@ -1130,15 +1157,16 @@
 					return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
 				if stream.binary:
 					result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
 					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result)
 				else:
 					result = Conv.str_to_int_list(stream.content)
 					self._log_info_list(f'{log_info}, received ascii format list', result)
-				self._session.query_and_clear_esr()
+				if self._session.clear_status_after_query_with_opc():
+					self._session.query_and_clear_esr()
 				self.check_status()
 				return result
 			except RsInstrException as e:
 				self._log_exception(e, log_info)
 				raise
 			finally:
 				self._log_end_segment()
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/InstrumentErrors.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/InstrumentErrors.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/InstrumentOptions.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/InstrumentOptions.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/InstrumentSettings.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/InstrumentSettings.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,22 @@
 	"""Mode that is used for OPC-sync commands/queries"""
 	stb_poll = 1
 	stb_poll_slow = 2
 	stb_poll_superslow = 3
 	opc_query = 4
 
 
+class OpcSyncQueryMechanism(Enum):
+	"""Mechanism to use when querying with OPC."""
+	standard = 0  # Sends the command with ;*OPC at the end, and waits for the ESB or ERRQ bits.
+	also_check_mav = 1  # Same as Standard, but for queries additionally ends the OPC-waiting queue on MAV bit set to 1.
+	cls_only_check_mav_err_queue = 2  # ClearBeforeRead, does not send the ;*OPC as the command suffix. In the wait loop, checks the MAV and ERRQ.
+	only_check_mav_err_queue = 3  # Same as above, but skips the ClearBeforeRead()
+
+
 class InstrumentSettings(object):
 	"""Defines settings of the instrument session."""
 
 	def __init__(
 			self,
 			viclear_exe_mode: InstrViClearMode,
 			idn_model_full_name: bool,
@@ -45,29 +53,32 @@
 			opc_timeout: int,
 			visa_timeout: int,
 			self_test_timeout: int,
 			instr_options_parse_mode: Opts.ParseMode,
 			bin_float_numbers_format: Conv.BinFloatFormat,
 			bin_int_numbers_format: Conv.BinIntFormat,
 			opc_query_after_write: bool,
-			logging_mode: LoggingMode):
+			logging_mode: LoggingMode,
+			opc_query_sync_mechanism: OpcSyncQueryMechanism):
 
 		self.viclear_exe_mode = viclear_exe_mode
 		self.idn_model_full_name = idn_model_full_name
 		self.write_delay = write_delay
 		self.read_delay = read_delay
 		self.io_segment_size = io_segment_size
 		self.opc_wait_mode = opc_wait_mode
 		self.opc_timeout = opc_timeout
 		self.visa_timeout = visa_timeout
 		self.selftest_timeout = self_test_timeout
 		self.instr_options_parse_mode = instr_options_parse_mode
 		self.bin_float_numbers_format = bin_float_numbers_format
 		self.bin_int_numbers_format = bin_int_numbers_format
 		self.opc_query_after_write = opc_query_after_write
+		self.opc_query_after_write = opc_query_after_write
+		self.opc_query_sync_mechanism = opc_query_sync_mechanism
 
 		self.logging_mode = logging_mode
 		self.logging_name = None
 		self.log_to_global_target = False
 		self.log_to_console = False
 		self.log_to_udp = False
 		self.log_udp_port = 49200
@@ -75,16 +86,20 @@
 		self.assure_write_with_tc = False
 		self.term_char = '\n'
 		self.encoding = 'charmap'
 		self.add_term_char_to_write_bin_block = False
 		self.open_timeout = 0
 		self.exclusive_lock = False
 		self.vxi_capable = True
+		self.scpi_quotes: str or None = None
 
 		self.cmd_idn = '*IDN?'
+		self.first_cmds = ''
+		self.idn_custom_parse = ''
+		self.each_cmd_prefix = ''
 		self.cmd_reset = '*RST'
 		self.skip_status_system_setting = False
 		self.skip_clear_status = False
 		self.stb_in_error_check = True
 		self.each_cmd_as_query = False
 		self.instr_status_check = False
 		self.disable_opc_query = False
@@ -173,14 +188,15 @@
 		if value:
 			self.write_delay = Conv.str_to_int(value)
 
 		value = self._get_driversetup_item('ReadDelay')
 		if value is not None:
 			self.read_delay = Conv.str_to_int(value)
 
+		# OpcWaitMode
 		value = self._get_driversetup_item('OpcWaitMode')
 		if value:
 			value = value.upper()
 			if value == 'STBPOLLING':
 				self.opc_wait_mode = WaitForOpcMode.stb_poll
 			elif value == 'STBPOLLINGSLOW':
 				self.opc_wait_mode = WaitForOpcMode.stb_poll_slow
@@ -205,28 +221,39 @@
 		if value:
 			self.exclusive_lock = Conv.str_to_bool(value)
 
 		value = self._get_driversetup_item('VxiCapable')
 		if value:
 			self.vxi_capable = Conv.str_to_bool(value)
 
+		# ScpiQuotes
+		value = self._get_driversetup_item('ScpiQuotes')
+		if value:
+			if value.lower() == 'single':
+				self.scpi_quotes = "'"
+			elif value.lower() == 'double':
+				self.scpi_quotes = '"'
+			else:
+				self.scpi_quotes = value
+
 		# Obsolete, use the AssureWriteWithTermChar
 		value = self._get_driversetup_item('AssureWriteWithLf')
 		if not value:
 			value = self._get_driversetup_item('AssureWriteWithTermChar')
 		if value:
 			self.assure_write_with_tc = Conv.str_to_bool(value)
 
 		# Obsolete, use the DataChunkSize
 		value = self._get_driversetup_item('IoSegmentSize')
 		if not value:
 			value = self._get_driversetup_item('DataChunkSize')
 		if value:
 			self.io_segment_size = Conv.str_to_int(value)
 
+		# TerminationCharacter
 		value = self._get_driversetup_item('TerminationCharacter')
 		if value:
 			val_lc = value.lower()
 			if value == '\\r' or val_lc == 'cr':
 				self.term_char = '\r'
 			elif value == '\\n' or val_lc == 'lf':
 				self.term_char = '\n'
@@ -247,26 +274,40 @@
 		if value:
 			self.opc_timeout = Conv.str_to_int(value)
 
 		value = self._get_driversetup_item('VisaTimeout')
 		if value:
 			self.visa_timeout = Conv.str_to_int(value)
 
+		# ViClearExeMode
 		value = self._get_driversetup_item('ViClearExeMode')
 		if value:
 			enum_value = Conv.str_to_simple_scalar_enum(value, InstrViClearMode, case_sensitive=False, ignore_underscores=True)
 			if enum_value is None:
 				try:
 					enum_value = InstrViClearMode(Conv.str_to_int(value))
 				except ValueError:
 					raise ValueError(
 						f"Unknown value in InitWithOptions string DriverSetup key 'ViClearExeMode'. Value '{value}' is not recognized. "
 						f"Valid values: ExecuteOnAll, Disabled, IgnoreError or integer bit-wise value.")
 			self.viclear_exe_mode = enum_value
 
+		# OpcSyncQueryMechanism
+		value = self._get_driversetup_item('OpcSyncQueryMechanism')
+		if value:
+			enum_value = Conv.str_to_simple_scalar_enum(value, OpcSyncQueryMechanism, case_sensitive=False, ignore_underscores=True)
+			if enum_value is None:
+				try:
+					enum_value = OpcSyncQueryMechanism(Conv.str_to_int(value))
+				except ValueError:
+					raise ValueError(
+						f"Unknown value in InitWithOptions string DriverSetup key 'OpcSyncQueryMechanism'. Value '{value}' is not recognized. "
+						f"Valid values: Standard, AlsoCheckMav, ClsOnlyCheckMavErrQueue, OnlyCheckMavErrQueue.")
+			self.opc_query_sync_mechanism = enum_value
+
 		value = self._get_driversetup_item('OpcQueryAfterWrite')
 		if value:
 			self.opc_query_after_write = Conv.str_to_bool(value)
 
 		value = self._get_driversetup_item('StbInErrorCheck')
 		if value:
 			self.stb_in_error_check = Conv.str_to_bool(value)
@@ -275,14 +316,15 @@
 		if value:
 			self.each_cmd_as_query = Conv.str_to_bool(value)
 
 		value = self._get_driversetup_item('DisableOpcQuery')
 		if value:
 			self.disable_opc_query = Conv.str_to_bool(value)
 
+		# LoggingMode
 		value = self._get_driversetup_item('LoggingMode')
 		if value:
 			enum_value = Conv.str_to_simple_scalar_enum(value, LoggingMode, case_sensitive=False)
 			if not enum_value:
 				raise ValueError(
 					f"Unknown value in InitWithOptions string 'options', key 'LoggingMode'. Value '{value}' is not recognized. "
 					f"Valid values: {', '.join([x.name for x in LoggingMode])}")
@@ -308,28 +350,29 @@
 		value = self._get_driversetup_item('LoggingUdpPort')
 		if value:
 			self.log_udp_port = Conv.str_to_int(value)
 
 		# Others
 		value = self._get_driversetup_item('CmdIdn')
 		if value:
-			self.cmd_idn = value
+			self.cmd_idn = '' if value.lower() == '<none>' else value
 
 		value = self._get_driversetup_item('CmdReset')
 		if value:
 			self.cmd_reset = value
 
 		value = self._get_driversetup_item('SkipStatusSystemSettings')
 		if value:
 			self.skip_status_system_setting = Conv.str_to_bool(value)
 
 		value = self._get_driversetup_item('SkipClearStatus')
 		if value:
 			self.skip_clear_status = Conv.str_to_bool(value)
 
+		# QueryOpt
 		value = self._get_driversetup_item('QueryOpt')
 		if value:
 			enum_value = Conv.str_to_simple_scalar_enum(value, Opts.ParseMode, case_sensitive=False)
 			if not enum_value:
 				raise ValueError(
 					f"Unknown value in InitWithOptions string 'options', key 'QueryOpt'. Value '{value}' is not recognized. "
 					f"Valid values: {', '.join([x.name for x in Opts.ParseMode])}")
@@ -354,15 +397,15 @@
 		if value:
 			self.supported_instr_models = [*map(trim_str_response, value.split('/'))]
 
 		value = self._get_driversetup_item('SupportedIdnPatterns')
 		if value:
 			self.supported_idn_patterns = [*map(trim_str_response, value.split('/'))]
 
-		# Profile has the ultimate priority.
+		# Profiles
 		value = self._get_driversetup_item('Profile')
 		if value:
 			val_low = value.lower()
 
 			if val_low == 'hm8123':
 				self.term_char = '\r'
 				self.assure_write_with_tc = True
@@ -398,9 +441,44 @@
 				self.skip_status_system_setting = True
 				self.skip_clear_status = True
 				self.disable_opc_query = True
 				self.instrument_status_check = False
 				self.stb_in_error_check = False
 				self.each_cmd_as_query = True
 
+			elif val_low == 'xk41':
+				self.assure_write_with_tc = True
+				self.skip_status_system_setting = True
+				self.skip_clear_status = True
+				self.disable_opc_query = True
+				self.instrument_status_check = False
+				self.stb_in_error_check = False
+				self.each_cmd_prefix = '\n'
+				self.first_cmds = '<q>M:REMOTE SENTER1'
+				self.cmd_idn = 'M:GR GVER'
+				self.idn_custom_parse = 'gVER"([^"]+)"->Rohde&Schwarz,M3SR,100000,\\1'
+				self.term_char = '\r'
+				self.each_cmd_as_query = True
+
 			else:
-				raise ValueError(f"Unknown value in InitWithOptions string 'options', key 'Profile', value '{value}'. Valid values (case-insensitive): HM8123, CMQ, Minimal, ATS")
+				raise ValueError(f"Unknown value in InitWithOptions string 'options', key 'Profile', value '{value}'. Valid values (case-insensitive): HM8123, CMQ, Minimal, XK41, ATS")
+
+			# Following values can still be overwritten on top of the profiles
+			value = self._get_driversetup_item('FirstCmds')
+			if value:
+				self.first_cmds = value
+
+			value = self._get_driversetup_item('IdnCustomParse')
+			if value:
+				self.idn_custom_parse = value
+
+			value = self._get_driversetup_item('EachCmdPrefix')
+			if value:
+				val_lc = value.lower()
+				if value == '\\r' or val_lc == 'cr':
+					self.each_cmd_prefix = '\r'
+				elif value == '\\n' or val_lc == 'lf':
+					self.each_cmd_prefix = '\n'
+				elif value == '\\t' or val_lc == 'tab':
+					self.each_cmd_prefix = '\t'
+				else:
+					self.each_cmd_prefix = value
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/InternalLinker.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/InternalLinker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/IoTransferEventArgs.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/IoTransferEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/RepeatedCapability.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/RepeatedCapability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ScpiEnums.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ScpiEnums.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/ScpiLogger.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/ScpiLogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,15 @@
 
     def __init__(self, resource_name: str, encoding: str = 'charmap'):
         if resource_name is None:
             raise RsInstrException('resource_name cannot be None')
         self._orig_resource_name = resource_name
         self._global_mode: bool = False
         self._default_mode: LoggingMode = LoggingMode.Off
+        self._last_logging_mode: LoggingMode = LoggingMode.On
         self._mode: LoggingMode = self._default_mode
         self._log_target_local = None
         self._cached = CachedEntries()
         self._timestamp_reference_time_local: datetime or None = None
         self._format_string: str = ''
         self._line_divider: str = '\n'
         self._target_auto_flushing = True
@@ -366,14 +367,25 @@
             # logging is ON. Check the internal log entries and flush them to the target
             self._flush_cached_entries()
         self._mode = value
         if self._mode == LoggingMode.Off and self.get_logging_target():
             # Logging was switched off, flush the entries on the target
             self.flush()
 
+    def start(self) -> None:
+        """Starts the logging with the last defined LoggingMode. Default is LoggingMode.On"""
+        self.mode = self._last_logging_mode
+
+    def stop(self) -> None:
+        """Stops the logging. This is the same as: mode = LoggingMode.Off"""
+        if self.mode is not LoggingMode.Off:
+            self._last_logging_mode = self.mode
+
+        self.mode = LoggingMode.Off
+
     @property
     def log_status_check_ok(self) -> bool:
         """Sets / returns the current status of status checking OK.
         If True (default), the log contains logging of the status checking 'Status check: OK'.
         If False, the 'Status check: OK' is skipped - the log is more compact.
         Errors will still be logged."""
         return self._log_status_check_ok
@@ -469,15 +481,15 @@
             return self._default_mode
         else:
             return value
 
     @property
     def default_mode(self) -> LoggingMode:
         """Sets / returns the default logging mode.
-        You can recall the default mode by calling the logger.mode = LoggingMode.Default
+        You can recall the default mode by calling the logger.mode = LoggingMode.Default.
 
         :Data Type: LoggingMode
         """
         return self._default_mode
 
     @default_mode.setter
     def default_mode(self, value: LoggingMode) -> None:
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/StreamReader.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/StreamReader.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/StreamWriter.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/StreamWriter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/StructBase.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/StructBase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/Types.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Types.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/Utilities.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/Utilities.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/VisaPluginSocketIo.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/VisaPluginSocketIo.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,16 @@
 
 		try:
 			while True:
 				to_read_len = chunk_size - read_len
 				if to_read_len <= 0:
 					break
 				data = session.recv(to_read_len)
+				if not data:
+					raise pyvisa.VisaIOError(pyvisa.constants.VI_ERROR_CONN_LOST)
 				chunk += data
 				read_len += len(data)
 
 				if self._socket_io.read_termination is not None:
 					# Read termination character is ON, look for it and stop the reading if found
 					term_char = self._socket_io.read_termination.encode()
 					if term_char in data:
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/VisaSession.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/VisaSession.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from typing import List, Tuple, Callable, AnyStr
 import os.path
 import re
 import threading
 
 # noinspection PyPackageRequirements
 import pyvisa
+from pyvisa.errors import StatusCode
 
 from .VisaPluginSocketIo import ResourceManager, SocketIo
 from . import InstrumentSettings, InstrumentErrors, Conversions as Conv
-from .InstrumentSettings import WaitForOpcMode, InstrViClearMode as ViClearMode
+from .InstrumentSettings import WaitForOpcMode, OpcSyncQueryMechanism, InstrViClearMode as ViClearMode
 from .StreamReader import StreamReader
 from .StreamWriter import StreamWriter
 from .Utilities import size_to_kb_mb_string, calculate_chunks_count
 import platform
 import struct
 
 
@@ -74,14 +75,16 @@
 		self.visa_library_name = None
 		self.resource_name = resource_name  # might be changed later if direct_session is used
 		self.encoding = settings.encoding  # default encoder between bytes and string
 		self.cmd_idn = settings.cmd_idn
 		self.skip_status_system_setting = settings.skip_status_system_setting
 		self.skip_clear_status = settings.skip_clear_status
 		self.stb_in_error_check = settings.stb_in_error_check
+		self.opc_sync_query_mechanism = settings.opc_query_sync_mechanism
+		self.each_cmd_prefix = settings.each_cmd_prefix
 
 		# Implemented for interface compatibility with VisaSessionSim
 		self.cached_to_stream = False
 
 		# Event handlers
 		# noinspection PyTypeChecker
 		self.on_read_chunk_handler: Callable = None
@@ -189,14 +192,27 @@
 		# Must call the VISA viClear() before any communication with the instrument
 		self.clear()
 
 		# Further steps are for NRP-Z session not valid
 		if self.is_rsnrp_session():
 			return
 
+		# First commands, can be more than one, separated by ';;'
+		if settings.first_cmds:
+			cmds = settings.first_cmds.split(';;')
+			for cmd in cmds:
+				if cmd.startswith('<w>'):
+					self.write(cmd[3:])
+				elif cmd.startswith('<q>'):
+					_ = self._query_str_no_events(cmd[3:])
+				elif '?' in cmd:
+					_ = self._query_str_no_events(cmd)
+				else:
+					self.write(cmd)
+
 		# Clear instrument status
 		if self.skip_clear_status is False:
 			self.write('*CLS')
 			if self.vxi_capable:
 				stb = self._read_stb()
 				if stb & StatusByte.message_available:
 					self._flush_junk_data()
@@ -328,15 +344,15 @@
 	@data_chunk_size.setter
 	def data_chunk_size(self, chunk_size: int) -> None:
 		"""Sets the maximum size of one block transferred during write/read operations."""
 		self._data_chunk_size = int(chunk_size)
 		self._session.chunk_size = int(chunk_size)
 
 	def _resolve_opc_timeout(self, timeout: int) -> int:
-		"""Resolves entered timeout value - if the input value is less than 1, it is replaces with opc_timeout."""
+		"""Resolves entered timeout value - if the input value is less than 1, it is replaced with opc_timeout."""
 		if timeout is None or timeout < 1:
 			return self.opc_timeout
 		else:
 			return timeout
 
 	def _set_regs_ese_sre(self, mode: WaitForOpcMode) -> WaitForOpcMode:
 		"""Based on the WaitForOpcMode, it sets the ESE and SRE register masks.
@@ -364,41 +380,60 @@
 			current_value = int(self._query_str_no_events('*SRE?'))
 			mask = current_value | mask.value
 		# Also affect the _opc_wait_mode:
 		# If the mask has event_status_byte == false, and the _opc_wait_mode is service_request, set it to stb_poll
 		# If the mask has event_status_byte == true, do not change anything
 		self.write(f'*SRE {mask.value}')
 
-	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int, end_mask: StatusByte) -> StatusByte:
+	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int) -> StatusByte:
 		"""Reads Status Byte Register and ends if the ESB bit (5) is set to 1.
 		Also works with the SOCKET and SERIAL interface by sending *STB? query.
 		In that case however, command cannot be a query.
 		Returns the last read Status Byte value."""
 		timeout_secs = timeout / 1000
-		self.clear_before_read()
+		end_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
 		if command.endswith(self._term_char):
 			command = command.rstrip(self._term_char)
-		self.write(command + ';*OPC')
-		# Use catch to return the VISA Timeout back
+
+		if is_query is True:
+			if self.opc_sync_query_mechanism == OpcSyncQueryMechanism.standard or self.opc_sync_query_mechanism == OpcSyncQueryMechanism.also_check_mav:
+				self.clear_before_read()
+				self.write(command + ';*OPC')
+				if self.opc_sync_query_mechanism == OpcSyncQueryMechanism.also_check_mav:
+					end_mask |= StatusByte.message_available
+
+			elif self.opc_sync_query_mechanism == OpcSyncQueryMechanism.only_check_mav_err_queue:
+				self.write(command)
+				end_mask = StatusByte.error_queue_not_empty | StatusByte.message_available
+
+			elif self.opc_sync_query_mechanism == OpcSyncQueryMechanism.cls_only_check_mav_err_queue:
+				self.clear_before_read()
+				self.write(command)
+				end_mask = StatusByte.error_queue_not_empty | StatusByte.message_available
+		else:
+			self.clear_before_read()
+			self.write(command + ';*OPC')
+
 		start = time.time()
 		# STB polling loop
 		while True:
 			stb = self._read_stb()
 			elapsed = self._polling_delay(start)
 			if elapsed > timeout_secs:
 				self._narrow_down_opc_tout_error(command, is_query, timeout)
 			if end_mask & stb:
 				break
 		return stb
 
-	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int, end_mask: StatusByte) -> StatusByte:
+	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int) -> StatusByte:
 		"""Queries Status Byte Register (*STB?) and ends if the ESB bit (5) is set to 1.
 			The command must not be a query. Also works with the SOCKET and SERIAL interface.
 			Returns the last read Status Byte value."""
 		timeout_secs = timeout / 1000
+		end_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
 		self.clear_before_read()
 		if command.endswith(self._term_char):
 			command = command.rstrip(self._term_char)
 		self.write(command + ';*OPC')
 		start = time.time()
 		# STB polling loop
 		while True:
@@ -658,16 +693,17 @@
 		- sending the *IDN? query"""
 		if self._session is None:
 			return False
 		# noinspection PyBroadException
 		try:
 			old_tout = self.visa_timeout
 			self.visa_timeout = 2000
-			self.write(self.cmd_idn)
-			_ = self._read_str_no_events()
+			if len(self.cmd_idn) > 0:
+				self.write(self.cmd_idn)
+				_ = self._read_str_no_events()
 			self.visa_timeout = old_tout
 			return True
 		except Exception:
 			return False
 
 	def _write_and_wait_for_opc(self, command: str, is_query: bool, timeout: int) -> StatusByte:
 		"""Internal method to synchronise a command with OPC timeout.
@@ -683,21 +719,18 @@
 
 		if self._opc_wait_mode == WaitForOpcMode.opc_query:
 			if is_query:
 				raise RsInstrException('Sending a query with OpcQuery synchronization is not possible')
 			stb = self._write_and_query_opc(command, timeout)
 		else:
 			# STB polling
-			end_stb_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
-			if is_query:
-				end_stb_mask |= StatusByte.message_available
 			if self.vxi_capable:
-				stb = self._write_and_poll_stb_vxi(command, is_query, timeout, end_stb_mask)
+				stb = self._write_and_poll_stb_vxi(command, is_query, timeout)
 			else:
-				stb = self._write_and_poll_stb_non_vxi(command, timeout, end_stb_mask)
+				stb = self._write_and_poll_stb_non_vxi(command, timeout)
 
 		return stb
 
 	def _write_and_query_opc(self, cmd: str, timeout: int) -> StatusByte:
 		"""Internal method to write a command followed by query_opc().
 		Used for opc-synchronization if the mode is set to WaitForOpcMode.opc_query or the session is not-vxi.
 		Timeout value 0 means the OPC timeout is used."""
@@ -711,21 +744,33 @@
 			self.write(cmd)
 			self.query_opc()
 		finally:
 			if old_tout != timeout:
 				self.visa_timeout = old_tout
 		return self._query_stb()
 
+	def clear_status_after_query_with_opc(self) -> bool:
+		"""Returns true, if the opc-sync queries require status clearing afterward."""
+		if self.vxi_capable is False or self._opc_wait_mode is WaitForOpcMode.opc_query:
+			return False
+		if self.opc_sync_query_mechanism == InstrumentSettings.OpcSyncQueryMechanism.standard:
+			return True
+		if self.opc_sync_query_mechanism == InstrumentSettings.OpcSyncQueryMechanism.also_check_mav:
+			return True
+		return False
+
 	def write(self, cmd: str) -> None:
 		"""Writes command to the instrument."""
 		if self.write_delay > 0:
 			time.sleep(self.write_delay / 1000)
 		add_tc = False
 		if self._assure_write_with_tc and not cmd.endswith(self._term_char):
 			add_tc = True
+		if self.each_cmd_prefix:
+			cmd = self.each_cmd_prefix + cmd
 		cmd_bytes = cmd.encode(self.encoding)
 		if add_tc:
 			cmd_bytes += self._term_char.encode(self.encoding)
 		self._session.write_raw(cmd_bytes)
 
 	def _read_unknown_len(self, stream: StreamWriter, allow_chunk_events: bool, prepend_data: AnyStr = None) -> None:
 		"""Reads data of unknown length to the provided WriteStream.
@@ -788,20 +833,23 @@
 		"""Queries the instrument and reads the response as string.
 		The length of the string is not limited. The response is then trimmed for trailing LF.
 		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
 		response = ''
 		self.write(query)
 		try:
 			response = self._read_str_no_events()
-		except pyvisa.VisaIOError:
+		except pyvisa.VisaIOError as e:
 			context = f"Query '{query.rstrip(self._term_char)}'"
-			if allow_tout_error_narrow_down:
-				self._narrow_down_io_tout_error(context + ' - ')
+			if e.error_code == StatusCode.error_timeout:
+				if allow_tout_error_narrow_down:
+					self._narrow_down_io_tout_error(context + ' - ')
+				else:
+					raise InstrumentErrors.TimeoutException(context)
 			else:
-				raise InstrumentErrors.TimeoutException(context)
+				raise InstrumentErrors.RsInstrException(context)
 		return response
 
 	def _query_str_no_events_timed(self, query: str, timeout: int, suppress_read_tout: bool = False) -> str:
 		"""Queries the instrument and reads the response as string.
 		The entered timeout sets the VISA timeout just for this call. You can suppress the timeout error.
 		The length of the string is not limited. The response is then trimmed for trailing LF.
 		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/Internal/VisaSessionSim.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/Internal/VisaSessionSim.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,18 @@
 		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
 		return
 
 	def clear(self) -> None:
 		"""Perform VISA viClear conditionally based on the instrument settings."""
 		return
 
+	def clear_status_after_query_with_opc(self) -> bool:
+		"""Returns true, if the opc-sync queries require status clearing afterward."""
+		return False
+
 	def write(self, cmd: str) -> None:
 		"""Writes command to the instrument."""
 		self._last_cmd = cmd
 		self._update_cmd_vals_cache(cmd)
 		return
 
 	def query_str(self, query: str) -> str:
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/RsCMPX_NiotMeas.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/RsCMPX_NiotMeas.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from datetime import datetime, timedelta
 from . import repcap
 from .Internal.RepeatedCapability import RepeatedCapability
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class RsCMPX_NiotMeas:
-	"""319 total commands, 5 Subgroups, 0 group commands"""
-	_driver_options = "SupportedInstrModels = CMW/CMP/CMX, SupportedIdnPatterns = CMW/CMP/CMX, SimulationIdnString = 'Rohde&Schwarz,CMP180,100001,4.0.186.0003'"
+	"""310 total commands, 4 Subgroups, 0 group commands"""
+	_driver_options = "SupportedInstrModels = CMW/CMP/CMX, SupportedIdnPatterns = CMW/CMP/CMX, SimulationIdnString = 'Rohde&Schwarz,CMP180,100001,5.0.70.0005'"
 	_global_logging_relative_timestamp: ClassVar[datetime] = None
 	_global_logging_target_stream: ClassVar = None
 
 	def __init__(self, resource_name: str, id_query: bool = True, reset: bool = False, options: str = None, direct_session: object = None):
 		"""Initializes new RsCMPX_NiotMeas session. \n
 		Parameter options tokens examples:
 			- ``Simulate=True`` - starts the session in simulation mode. Default: ``False``
@@ -31,27 +31,28 @@
 			- ``TerminationCharacter = "\\r"`` - Sets the termination character for reading. Default: ``\\n`` (LineFeed or LF)
 			- ``DataChunkSize = 10E3`` - Maximum size of one write/read segment. If transferred data is bigger, it is split to more segments. Default: ``1E6`` bytes
 			- ``OpcTimeout = 10000`` - same as driver.utilities.opc_timeout = 10000. Default: ``30000ms``
 			- ``VisaTimeout = 5000`` - same as driver.utilities.visa_timeout = 5000. Default: ``10000ms``
 			- ``ViClearExeMode = Disabled`` - viClear() execution mode. Default: ``execute_on_all``
 			- ``OpcQueryAfterWrite = True`` - same as driver.utilities.opc_query_after_write = True. Default: ``False``
 			- ``StbInErrorCheck = False`` - if true, the driver checks errors with *STB? If false, it uses SYST:ERR?. Default: ``True``
+			- ``ScpiQuotes = double'. - for SCPI commands, you can define how strings are quoted. With single or double quotes. Possible values: single | double | {char}. Default: ``single``
 			- ``LoggingMode = On`` - Sets the logging status right from the start. Default: ``Off``
 			- ``LoggingName = 'MyDevice'`` - Sets the name to represent the session in the log entries. Default: ``'resource_name'``
 			- ``LogToGlobalTarget = True`` - Sets the logging target to the class-property previously set with RsCMPX_NiotMeas.set_global_logging_target() Default: ``False``
 			- ``LoggingToConsole = True`` - Immediately starts logging to the console. Default: False
 			- ``LoggingToUdp = True`` - Immediately starts logging to the UDP port. Default: False
 			- ``LoggingUdpPort = 49200`` - UDP port to log to. Default: 49200
 		:param resource_name: VISA resource name, e.g. 'TCPIP::192.168.2.1::INSTR'
 		:param id_query: if True, the instrument's model name is verified against the models supported by the driver and eventually throws an exception.
 		:param reset: Resets the instrument (sends *RST command) and clears its status sybsystem.
 		:param options: string tokens alternating the driver settings.
 		:param direct_session: Another driver object or pyVisa object to reuse the session instead of opening a new session."""
 		self._core = Core(resource_name, id_query, reset, RsCMPX_NiotMeas._driver_options, options, direct_session)
-		self._core.driver_version = '4.0.186.0003'
+		self._core.driver_version = '5.0.70.0005'
 		self._options = options
 		self._add_all_global_repcaps()
 		self._custom_properties_init()
 		self.utilities.default_instrument_setup()
 		# noinspection PyTypeChecker
 		self._cmd_group = CommandsGroup("ROOT", self._core, None)
 
@@ -123,25 +124,25 @@
 		self._core.io.reset_time_statistics()
 
 	@staticmethod
 	def assert_minimum_version(min_version: str) -> None:
 		"""Asserts that the driver version fulfills the minimum required version you have entered.
 		This way you make sure your installed driver is of the entered version or newer."""
 		min_version_list = min_version.split('.')
-		curr_version_list = '4.0.186.0003'.split('.')
+		curr_version_list = '5.0.70.0005'.split('.')
 		count_min = len(min_version_list)
 		count_curr = len(curr_version_list)
 		count = count_min if count_min < count_curr else count_curr
 		for i in range(count):
 			minimum = int(min_version_list[i])
 			curr = int(curr_version_list[i])
 			if curr > minimum:
 				break
 			if curr < minimum:
-				raise RsInstrException(f"Assertion for minimum RsCMPX_NiotMeas version failed. Current version: '4.0.186.0003', minimum required version: '{min_version}'")
+				raise RsInstrException(f"Assertion for minimum RsCMPX_NiotMeas version failed. Current version: '5.0.70.0005', minimum required version: '{min_version}'")
 
 	@staticmethod
 	def list_resources(expression: str = '?*::INSTR', visa_select: str = None) -> List[str]:
 		"""Finds all the resources defined by the expression
 			- '?*' - matches all the available instruments
 			- 'USB::?*' - matches all the USB instruments
 			- 'TCPIP::192?*' - matches all the LAN instruments with the IP address starting with 192
@@ -187,22 +188,14 @@
 	def _sync_to_custom_properties(self, cloned: 'RsCMPX_NiotMeas') -> None:
 		"""Synchronises the state of all the custom properties to the entered object."""
 		cloned.utilities.sync_from(self.utilities)
 		cloned.events.sync_from(self.events)
 		cloned.reliability.sync_from(self.reliability)
 
 	@property
-	def route(self):
-		"""route commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_route'):
-			from .Implementations.Route import RouteCls
-			self._route = RouteCls(self._core, self._cmd_group)
-		return self._route
-
-	@property
 	def configure(self):
 		"""configure commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_configure'):
 			from .Implementations.Configure import ConfigureCls
 			self._configure = ConfigureCls(self._core, self._cmd_group)
 		return self._configure
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/__init__.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """RsCMPX_NiotMeas instrument driver
-	:version: 4.0.186.3
+	:version: 5.0.70.5
 	:copyright: 2023 by Rohde & Schwarz GMBH & Co. KG
 	:license: MIT, see LICENSE for more details.
 """
 
-__version__ = '4.0.186.3'
+__version__ = '5.0.70.5'
 
 # Main class
 from RsCMPX_NiotMeas.RsCMPX_NiotMeas import RsCMPX_NiotMeas
 
 # Bin data format
 from RsCMPX_NiotMeas.Internal.Conversions import BinIntFormat, BinFloatFormat
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas/repcap.py` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas/repcap.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas.egg-info/PKG-INFO` & `RsCMPX_NiotMeas-5.0.70/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: RsCMPX-NiotMeas
-Version: 4.0.186
+Name: RsCMPX_NiotMeas
+Version: 5.0.70
 Summary: CMP180 Narrowband IoT Measurement Remote-control module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 License: MIT
 Description: ==================================
          RsCMPX_NiotMeas
         ==================================
@@ -44,15 +44,18 @@
         
         Examples: https://github.com/Rohde-Schwarz/Examples/
         
         
         Version history
         ----------------
         
-        	Latest release notes summary: Fixed documentation
+        	Latest release notes summary: Update for FW 5.0.70
+        
+        	Version 5.0.70
+        		- Update for FW 5.0.70
         
         	Version 4.0.186
         		- Fixed documentation
         
         	Version 4.0.185
         		- First released version for FW 4.0.185
```

### Comparing `RsCMPX_NiotMeas-4.0.186/RsCMPX_NiotMeas.egg-info/SOURCES.txt` & `RsCMPX_NiotMeas-5.0.70/RsCMPX_NiotMeas.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -215,30 +215,22 @@
 RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Current.py
 RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/Maximum.py
 RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Pdynamics/__init__.py
 RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Average.py
 RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Current.py
 RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/Maximum.py
 RsCMPX_NiotMeas/Implementations/NiotMeas/Prach/Trace/Perror/__init__.py
-RsCMPX_NiotMeas/Implementations/Route/__init__.py
-RsCMPX_NiotMeas/Implementations/Route/NiotMeas/__init__.py
-RsCMPX_NiotMeas/Implementations/Route/NiotMeas/Scenario/CombinedSignalPath.py
-RsCMPX_NiotMeas/Implementations/Route/NiotMeas/Scenario/MaProtocol.py
-RsCMPX_NiotMeas/Implementations/Route/NiotMeas/Scenario/Salone.py
-RsCMPX_NiotMeas/Implementations/Route/NiotMeas/Scenario/__init__.py
 RsCMPX_NiotMeas/Implementations/Sense/__init__.py
 RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/MultiEval.py
 RsCMPX_NiotMeas/Implementations/Sense/NiotMeas/__init__.py
 RsCMPX_NiotMeas/Implementations/Trigger/__init__.py
+RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/Prach.py
 RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/__init__.py
-RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/Catalog.py
 RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/ListPy.py
 RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/MultiEval/__init__.py
-RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/Prach/Catalog.py
-RsCMPX_NiotMeas/Implementations/Trigger/NiotMeas/Prach/__init__.py
 RsCMPX_NiotMeas/Internal/ArgLinkedEventArgs.py
 RsCMPX_NiotMeas/Internal/ArgSingle.py
 RsCMPX_NiotMeas/Internal/ArgSingleList.py
 RsCMPX_NiotMeas/Internal/ArgSingleSuppressed.py
 RsCMPX_NiotMeas/Internal/ArgStringComposer.py
 RsCMPX_NiotMeas/Internal/ArgStruct.py
 RsCMPX_NiotMeas/Internal/ArgStructList.py
@@ -251,14 +243,15 @@
 RsCMPX_NiotMeas/Internal/GlobalData.py
 RsCMPX_NiotMeas/Internal/Instrument.py
 RsCMPX_NiotMeas/Internal/InstrumentErrors.py
 RsCMPX_NiotMeas/Internal/InstrumentOptions.py
 RsCMPX_NiotMeas/Internal/InstrumentSettings.py
 RsCMPX_NiotMeas/Internal/InternalLinker.py
 RsCMPX_NiotMeas/Internal/IoTransferEventArgs.py
+RsCMPX_NiotMeas/Internal/Properties.py
 RsCMPX_NiotMeas/Internal/RepeatedCapability.py
 RsCMPX_NiotMeas/Internal/ScpiEnums.py
 RsCMPX_NiotMeas/Internal/ScpiLogger.py
 RsCMPX_NiotMeas/Internal/StreamReader.py
 RsCMPX_NiotMeas/Internal/StreamWriter.py
 RsCMPX_NiotMeas/Internal/StructBase.py
 RsCMPX_NiotMeas/Internal/Types.py
```

### Comparing `RsCMPX_NiotMeas-4.0.186/setup.py` & `RsCMPX_NiotMeas-5.0.70/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.rst").read_text()
 
 # This call to setup() does all the work
 setup(
     name="RsCMPX_NiotMeas",
-    version="4.0.186",
+    version="5.0.70",
     description="CMP180 Narrowband IoT Measurement Remote-control module",
     long_description=README,
     long_description_content_type="text/x-rst",
     author="Rohde & Schwarz GmbH & Co. KG",
     copyright="Copyright © Rohde & Schwarz GmbH & Co. KG 2022",
     license="MIT",
     classifiers=['License :: OSI Approved :: MIT License',
```

