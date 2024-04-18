# Comparing `tmp/ffmpeg_media_type-0.0.9.tar.gz` & `tmp/ffmpeg_media_type-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_media_type-0.0.9.tar", max compression
+gzip compressed data, was "ffmpeg_media_type-1.0.0.tar", max compression
```

## Comparing `ffmpeg_media_type-0.0.9.tar` & `ffmpeg_media_type-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,424 @@
--rw-r--r--   0        0        0     1066 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/LICENSE
--rw-r--r--   0        0        0     4904 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/README.md
--rw-r--r--   0        0        0     1589 2023-10-17 04:08:52.482603 ffmpeg_media_type-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      186 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/__init__.py
--rw-r--r--   0        0        0      763 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/conftest.py
--rw-r--r--   0        0        0        0 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/__init__.py
--rw-r--r--   0        0        0    89367 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-3.2.json
--rw-r--r--   0        0        0    91003 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-3.3.json
--rw-r--r--   0        0        0    92339 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-3.4.json
--rw-r--r--   0        0        0    94852 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.0.json
--rw-r--r--   0        0        0    95951 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.1.json
--rw-r--r--   0        0        0    97292 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.2.json
--rw-r--r--   0        0        0   100111 2023-10-17 04:08:31.966319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.3.json
--rw-r--r--   0        0        0   106316 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-4.4.json
--rw-r--r--   0        0        0   107177 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-5.0.json
--rw-r--r--   0        0        0   109161 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-5.1.json
--rw-r--r--   0        0        0   120284 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/data/ffmpeg-6.0.json
--rw-r--r--   0        0        0       47 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/exceptions.py
--rw-r--r--   0        0        0     3689 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/info.py
--rw-r--r--   0        0        0      378 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/main.py
--rw-r--r--   0        0        0        0 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/py.typed
--rw-r--r--   0        0        0        0 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/__init__.py
--rw-r--r--   0        0        0     6977 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/ffmpeg.py
--rw-r--r--   0        0        0      514 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/shell.py
--rw-r--r--   0        0        0     2977 2023-10-17 04:08:31.970319 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/table.py
--rw-r--r--   0        0        0     1790 2023-10-17 04:08:32.074320 ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/utils/wiki_ext.py
--rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 ffmpeg_media_type-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4904 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/README.md
+-rw-r--r--   0        0        0     1664 2024-04-18 00:36:22.717750 ffmpeg_media_type-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      234 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/3dostr.json
+-rw-r--r--   0        0        0      216 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/3g2.json
+-rw-r--r--   0        0        0      214 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/3gp.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/4xm.json
+-rw-r--r--   0        0        0      214 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/a64.json
+-rw-r--r--   0        0        0      203 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/aa.json
+-rw-r--r--   0        0        0      218 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/aac.json
+-rw-r--r--   0        0        0      189 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/aax.json
+-rw-r--r--   0        0        0      203 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ac3.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ac4.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ace.json
+-rw-r--r--   0        0        0      195 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/acm.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/act.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/adf.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/adp.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ads.json
+-rw-r--r--   0        0        0      235 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/adts.json
+-rw-r--r--   0        0        0      197 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/adx.json
+-rw-r--r--   0        0        0      197 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/aea.json
+-rw-r--r--   0        0        0      185 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/afc.json
+-rw-r--r--   0        0        0      236 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/aiff.json
+-rw-r--r--   0        0        0      189 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/aix.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/alaw.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/alias_pix.json
+-rw-r--r--   0        0        0      216 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/alp.json
+-rw-r--r--   0        0        0      204 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/amr.json
+-rw-r--r--   0        0        0      189 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/amrnb.json
+-rw-r--r--   0        0        0      189 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/amrwb.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/amv.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/anm.json
+-rw-r--r--   0        0        0      191 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/apac.json
+-rw-r--r--   0        0        0      185 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/apc.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ape.json
+-rw-r--r--   0        0        0      214 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/apm.json
+-rw-r--r--   0        0        0      230 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/apng.json
+-rw-r--r--   0        0        0      239 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/aptx.json
+-rw-r--r--   0        0        0      250 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/aptx_hd.json
+-rw-r--r--   0        0        0      203 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/aqtitle.json
+-rw-r--r--   0        0        0      209 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/argo_asf.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/argo_brp.json
+-rw-r--r--   0        0        0      213 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/argo_cvg.json
+-rw-r--r--   0        0        0      263 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/asf.json
+-rw-r--r--   0        0        0      219 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/asf_o.json
+-rw-r--r--   0        0        0      271 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/asf_stream.json
+-rw-r--r--   0        0        0      229 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ass.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ast.json
+-rw-r--r--   0        0        0      205 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/au.json
+-rw-r--r--   0        0        0      221 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/audiotoolbox.json
+-rw-r--r--   0        0        0      193 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/av1.json
+-rw-r--r--   0        0        0      211 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/avfoundation.json
+-rw-r--r--   0        0        0      233 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/avi.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/avif.json
+-rw-r--r--   0        0        0      242 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/avm2.json
+-rw-r--r--   0        0        0      209 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/avr.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/avs.json
+-rw-r--r--   0        0        0      222 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/avs2.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/avs3.json
+-rw-r--r--   0        0        0      207 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/bethsoftvid.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/bfi.json
+-rw-r--r--   0        0        0      221 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/bfstm.json
+-rw-r--r--   0        0        0      188 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/bin.json
+-rw-r--r--   0        0        0      182 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/bink.json
+-rw-r--r--   0        0        0      196 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/binka.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/bit.json
+-rw-r--r--   0        0        0      203 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/bitpacked.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/bmp_pipe.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/bmv.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/boa.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/bonk.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/brender_pix.json
+-rw-r--r--   0        0        0      218 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/brstm.json
+-rw-r--r--   0        0        0      190 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/c93.json
+-rw-r--r--   0        0        0      230 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/caf.json
+-rw-r--r--   0        0        0      235 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/cavsvideo.json
+-rw-r--r--   0        0        0      193 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/cdg.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/cdxl.json
+-rw-r--r--   0        0        0      190 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/cine.json
+-rw-r--r--   0        0        0      205 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/codec2.json
+-rw-r--r--   0        0        0      204 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/codec2raw.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/concat.json
+-rw-r--r--   0        0        0      205 2024-04-18 00:36:04.713919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/crc.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/cri_pipe.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dash.json
+-rw-r--r--   0        0        0      185 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/data.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/daud.json
+-rw-r--r--   0        0        0      195 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dcstr.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dds_pipe.json
+-rw-r--r--   0        0        0      193 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/derf.json
+-rw-r--r--   0        0        0      193 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dfa.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dfpwm.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dhav.json
+-rw-r--r--   0        0        0      204 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dirac.json
+-rw-r--r--   0        0        0      221 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dnxhd.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dpx_pipe.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dsf.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dsicin.json
+-rw-r--r--   0        0        0      211 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dss.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dts.json
+-rw-r--r--   0        0        0      196 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dtshd.json
+-rw-r--r--   0        0        0      220 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dv.json
+-rw-r--r--   0        0        0      190 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dvbsub.json
+-rw-r--r--   0        0        0      186 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dvbtxt.json
+-rw-r--r--   0        0        0      224 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dvd.json
+-rw-r--r--   0        0        0      180 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/dxa.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ea.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ea_cdata.json
+-rw-r--r--   0        0        0      216 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/eac3.json
+-rw-r--r--   0        0        0      214 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/epaf.json
+-rw-r--r--   0        0        0      197 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/evc.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/exr_pipe.json
+-rw-r--r--   0        0        0      223 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/f32be.json
+-rw-r--r--   0        0        0      226 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/f32le.json
+-rw-r--r--   0        0        0      225 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/f4v.json
+-rw-r--r--   0        0        0      223 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/f64be.json
+-rw-r--r--   0        0        0      226 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/f64le.json
+-rw-r--r--   0        0        0      214 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ffmetadata.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/fifo.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/fifo_test.json
+-rw-r--r--   0        0        0      224 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/film_cpk.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/filmstrip.json
+-rw-r--r--   0        0        0      218 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/fits.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/flac.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/flic.json
+-rw-r--r--   0        0        0      216 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/flv.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/framecrc.json
+-rw-r--r--   0        0        0      222 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/framehash.json
+-rw-r--r--   0        0        0      220 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/framemd5.json
+-rw-r--r--   0        0        0      190 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/frm.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/fsb.json
+-rw-r--r--   0        0        0      211 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/fwse.json
+-rw-r--r--   0        0        0      219 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/g722.json
+-rw-r--r--   0        0        0      228 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/g723_1.json
+-rw-r--r--   0        0        0      228 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/g726.json
+-rw-r--r--   0        0        0      236 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/g726le.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/g729.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/gdv.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/gem_pipe.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/genh.json
+-rw-r--r--   0        0        0      237 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/gif.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/gif_pipe.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/gsm.json
+-rw-r--r--   0        0        0      229 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/gxf.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/h261.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/h263.json
+-rw-r--r--   0        0        0      224 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/h264.json
+-rw-r--r--   0        0        0      207 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/hash.json
+-rw-r--r--   0        0        0      189 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/hca.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/hcom.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/hdr_pipe.json
+-rw-r--r--   0        0        0      193 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/hds.json
+-rw-r--r--   0        0        0      216 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/hevc.json
+-rw-r--r--   0        0        0      214 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/hls.json
+-rw-r--r--   0        0        0      188 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/hnm.json
+-rw-r--r--   0        0        0      214 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ico.json
+-rw-r--r--   0        0        0      191 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/idcin.json
+-rw-r--r--   0        0        0      195 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/idf.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/iff.json
+-rw-r--r--   0        0        0      194 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ifv.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ilbc.json
+-rw-r--r--   0        0        0      495 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/image2.json
+-rw-r--r--   0        0        0      209 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/image2pipe.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/imf.json
+-rw-r--r--   0        0        0      207 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ingenient.json
+-rw-r--r--   0        0        0      194 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ipmovie.json
+-rw-r--r--   0        0        0      244 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ipod.json
+-rw-r--r--   0        0        0      195 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ipu.json
+-rw-r--r--   0        0        0      232 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ircam.json
+-rw-r--r--   0        0        0      236 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ismv.json
+-rw-r--r--   0        0        0      187 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/iss.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/iv8.json
+-rw-r--r--   0        0        0      191 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ivf.json
+-rw-r--r--   0        0        0      212 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ivr.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/j2k_pipe.json
+-rw-r--r--   0        0        0      228 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/jacosub.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/jpeg_pipe.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/jpegls_pipe.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/jpegxl_anim.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/jpegxl_pipe.json
+-rw-r--r--   0        0        0      194 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/jv.json
+-rw-r--r--   0        0        0      193 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/kux.json
+-rw-r--r--   0        0        0      227 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/kvag.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/laf.json
+-rw-r--r--   0        0        0      219 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/latm.json
+-rw-r--r--   0        0        0      211 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/lavfi.json
+-rw-r--r--   0        0        0      214 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/live_flv.json
+-rw-r--r--   0        0        0      188 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/lmlm4.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/loas.json
+-rw-r--r--   0        0        0      191 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/lrc.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/luodat.json
+-rw-r--r--   0        0        0      185 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/lvf.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/lxf.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/m4v.json
+-rw-r--r--   0        0        0      237 2024-04-18 00:36:04.717919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/matroska,webm.json
+-rw-r--r--   0        0        0      221 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/matroska.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mca.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mcc.json
+-rw-r--r--   0        0        0      205 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/md5.json
+-rw-r--r--   0        0        0      212 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mgsts.json
+-rw-r--r--   0        0        0      225 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/microdvd.json
+-rw-r--r--   0        0        0      233 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mjpeg.json
+-rw-r--r--   0        0        0      209 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mjpeg_2000.json
+-rw-r--r--   0        0        0      256 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mkvtimestamp_v2.json
+-rw-r--r--   0        0        0      191 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mlp.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mlv.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mm.json
+-rw-r--r--   0        0        0      219 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mmf.json
+-rw-r--r--   0        0        0      197 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mods.json
+-rw-r--r--   0        0        0      203 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/moflex.json
+-rw-r--r--   0        0        0      304 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mov,mp4,m4a,3gp,3g2,mj2.json
+-rw-r--r--   0        0        0      204 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mov.json
+-rw-r--r--   0        0        0      233 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mp2.json
+-rw-r--r--   0        0        0      242 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mp3.json
+-rw-r--r--   0        0        0      218 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mp4.json
+-rw-r--r--   0        0        0      190 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpc.json
+-rw-r--r--   0        0        0      190 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpc8.json
+-rw-r--r--   0        0        0      249 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpeg.json
+-rw-r--r--   0        0        0      240 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpeg1video.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpeg2video.json
+-rw-r--r--   0        0        0      261 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpegts.json
+-rw-r--r--   0        0        0      220 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpegtsraw.json
+-rw-r--r--   0        0        0      197 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpegvideo.json
+-rw-r--r--   0        0        0      234 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpjpeg.json
+-rw-r--r--   0        0        0      205 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpl2.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mpsub.json
+-rw-r--r--   0        0        0      194 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/msf.json
+-rw-r--r--   0        0        0      203 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/msnwctcp.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/msp.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mtaf.json
+-rw-r--r--   0        0        0      180 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mtv.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mulaw.json
+-rw-r--r--   0        0        0      196 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/musx.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mv.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mvi.json
+-rw-r--r--   0        0        0      245 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mxf.json
+-rw-r--r--   0        0        0      258 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mxf_d10.json
+-rw-r--r--   0        0        0      273 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mxf_opatom.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/mxg.json
+-rw-r--r--   0        0        0      193 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/nc.json
+-rw-r--r--   0        0        0      225 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/nistsphere.json
+-rw-r--r--   0        0        0      209 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/nsp.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/nsv.json
+-rw-r--r--   0        0        0      216 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/null.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/nut.json
+-rw-r--r--   0        0        0      188 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/nuv.json
+-rw-r--r--   0        0        0      204 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/obu.json
+-rw-r--r--   0        0        0      204 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/oga.json
+-rw-r--r--   0        0        0      211 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ogg.json
+-rw-r--r--   0        0        0      212 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ogv.json
+-rw-r--r--   0        0        0      229 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/oma.json
+-rw-r--r--   0        0        0      205 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/opus.json
+-rw-r--r--   0        0        0      189 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/osq.json
+-rw-r--r--   0        0        0      213 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/paf.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pam_pipe.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pbm_pipe.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pcx_pipe.json
+-rw-r--r--   0        0        0      196 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pdv.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pfm_pipe.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pgm_pipe.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pgmyuv_pipe.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pgx_pipe.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/phm_pipe.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/photocd_pipe.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pictor_pipe.json
+-rw-r--r--   0        0        0      226 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pjs.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pmp.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/png_pipe.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pp_bnk.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ppm_pipe.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/psd_pipe.json
+-rw-r--r--   0        0        0      220 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/psp.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/psxstr.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pva.json
+-rw-r--r--   0        0        0      209 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/pvf.json
+-rw-r--r--   0        0        0      180 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/qcp.json
+-rw-r--r--   0        0        0      204 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/qdraw_pipe.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/qoi_pipe.json
+-rw-r--r--   0        0        0      188 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/r3d.json
+-rw-r--r--   0        0        0      225 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/rawvideo.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/realtext.json
+-rw-r--r--   0        0        0      195 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/redspark.json
+-rw-r--r--   0        0        0      196 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/rka.json
+-rw-r--r--   0        0        0      180 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/rl2.json
+-rw-r--r--   0        0        0      216 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/rm.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/roq.json
+-rw-r--r--   0        0        0      190 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/rpl.json
+-rw-r--r--   0        0        0      194 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/rsd.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/rso.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/rtp.json
+-rw-r--r--   0        0        0      216 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/rtp_mpegts.json
+-rw-r--r--   0        0        0      196 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/rtsp.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/s16be.json
+-rw-r--r--   0        0        0      222 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/s16le.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/s24be.json
+-rw-r--r--   0        0        0      218 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/s24le.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/s32be.json
+-rw-r--r--   0        0        0      218 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/s32le.json
+-rw-r--r--   0        0        0      189 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/s337m.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/s8.json
+-rw-r--r--   0        0        0      211 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sami.json
+-rw-r--r--   0        0        0      194 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sap.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.721919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sbc.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sbg.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/scc.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/scd.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sdl,sdl2.json
+-rw-r--r--   0        0        0      193 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sdns.json
+-rw-r--r--   0        0        0      180 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sdp.json
+-rw-r--r--   0        0        0      188 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sdr2.json
+-rw-r--r--   0        0        0      207 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sds.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sdx.json
+-rw-r--r--   0        0        0      188 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/segment.json
+-rw-r--r--   0        0        0      247 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ser.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sga.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sgi_pipe.json
+-rw-r--r--   0        0        0      193 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/shn.json
+-rw-r--r--   0        0        0      207 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/siff.json
+-rw-r--r--   0        0        0      217 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/simbiosis_imx.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sln.json
+-rw-r--r--   0        0        0      213 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/smjpeg.json
+-rw-r--r--   0        0        0      184 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/smk.json
+-rw-r--r--   0        0        0      218 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/smoothstreaming.json
+-rw-r--r--   0        0        0      194 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/smush.json
+-rw-r--r--   0        0        0      187 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sol.json
+-rw-r--r--   0        0        0      217 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sox.json
+-rw-r--r--   0        0        0      223 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/spdif.json
+-rw-r--r--   0        0        0      205 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/spx.json
+-rw-r--r--   0        0        0      216 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/srt.json
+-rw-r--r--   0        0        0      204 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/stl.json
+-rw-r--r--   0        0        0      220 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/stream_segment,ssegment.json
+-rw-r--r--   0        0        0      224 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/streamhash.json
+-rw-r--r--   0        0        0      213 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/subviewer.json
+-rw-r--r--   0        0        0      217 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/subviewer1.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sunrast_pipe.json
+-rw-r--r--   0        0        0      244 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/sup.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/svag.json
+-rw-r--r--   0        0        0      222 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/svcd.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/svg_pipe.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/svs.json
+-rw-r--r--   0        0        0      238 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/swf.json
+-rw-r--r--   0        0        0      189 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/tak.json
+-rw-r--r--   0        0        0      203 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/tedcaptions.json
+-rw-r--r--   0        0        0      195 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/tee.json
+-rw-r--r--   0        0        0      180 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/thp.json
+-rw-r--r--   0        0        0      203 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/tiertexseq.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/tiff_pipe.json
+-rw-r--r--   0        0        0      189 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/tmv.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/truehd.json
+-rw-r--r--   0        0        0      211 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/tta.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ttml.json
+-rw-r--r--   0        0        0      245 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/tty.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/txd.json
+-rw-r--r--   0        0        0      190 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/ty.json
+-rw-r--r--   0        0        0      217 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/u16be.json
+-rw-r--r--   0        0        0      224 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/u16le.json
+-rw-r--r--   0        0        0      217 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/u24be.json
+-rw-r--r--   0        0        0      220 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/u24le.json
+-rw-r--r--   0        0        0      217 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/u32be.json
+-rw-r--r--   0        0        0      220 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/u32le.json
+-rw-r--r--   0        0        0      203 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/u8.json
+-rw-r--r--   0        0        0      230 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/uncodedframecrc.json
+-rw-r--r--   0        0        0      189 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/usm.json
+-rw-r--r--   0        0        0      209 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/v210.json
+-rw-r--r--   0        0        0      211 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/v210x.json
+-rw-r--r--   0        0        0      194 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vag.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vbn_pipe.json
+-rw-r--r--   0        0        0      198 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vc1.json
+-rw-r--r--   0        0        0      208 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vc1test.json
+-rw-r--r--   0        0        0      242 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vcd.json
+-rw-r--r--   0        0        0      204 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vidc.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vividas.json
+-rw-r--r--   0        0        0      187 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vivo.json
+-rw-r--r--   0        0        0      187 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vmd.json
+-rw-r--r--   0        0        0      220 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vob.json
+-rw-r--r--   0        0        0      207 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vobsub.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/voc.json
+-rw-r--r--   0        0        0      194 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vpk.json
+-rw-r--r--   0        0        0      203 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vplayer.json
+-rw-r--r--   0        0        0      251 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vqf.json
+-rw-r--r--   0        0        0      218 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/vvc.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/w64.json
+-rw-r--r--   0        0        0      194 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/wady.json
+-rw-r--r--   0        0        0      228 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/wav.json
+-rw-r--r--   0        0        0      201 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/wavarc.json
+-rw-r--r--   0        0        0      206 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/wc3movie.json
+-rw-r--r--   0        0        0      205 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/webm.json
+-rw-r--r--   0        0        0      215 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/webm_chunk.json
+-rw-r--r--   0        0        0      229 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/webm_dash_manifest.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/webp.json
+-rw-r--r--   0        0        0      202 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/webp_pipe.json
+-rw-r--r--   0        0        0      207 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/webvtt.json
+-rw-r--r--   0        0        0      217 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/wsaud.json
+-rw-r--r--   0        0        0      212 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/wsd.json
+-rw-r--r--   0        0        0      199 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/wsvqa.json
+-rw-r--r--   0        0        0      218 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/wtv.json
+-rw-r--r--   0        0        0      212 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/wv.json
+-rw-r--r--   0        0        0      190 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/wve.json
+-rw-r--r--   0        0        0      210 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/x11grab.json
+-rw-r--r--   0        0        0      184 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/xa.json
+-rw-r--r--   0        0        0      205 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/xbin.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/xbm_pipe.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/xmd.json
+-rw-r--r--   0        0        0      195 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/xmv.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/xpm_pipe.json
+-rw-r--r--   0        0        0      197 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/xvag.json
+-rw-r--r--   0        0        0      200 2024-04-18 00:36:04.725919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/xwd_pipe.json
+-rw-r--r--   0        0        0      192 2024-04-18 00:36:04.729919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/xwma.json
+-rw-r--r--   0        0        0      195 2024-04-18 00:36:04.729919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/yop.json
+-rw-r--r--   0        0        0      218 2024-04-18 00:36:04.729919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/cache/yuv4mpegpipe.json
+-rw-r--r--   0        0        0      101 2024-04-18 00:36:04.729919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/exceptions.py
+-rw-r--r--   0        0        0     3412 2024-04-18 00:36:04.729919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/info.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:36:04.729919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/py.typed
+-rw-r--r--   0        0        0     3387 2024-04-18 00:36:04.729919 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/schema.py
+-rw-r--r--   0        0        0        0 2024-04-18 00:36:04.833918 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2024-04-18 00:36:04.833918 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/utils/cache.py
+-rw-r--r--   0        0        0      909 2024-04-18 00:36:04.833918 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/utils/ffprobe.py
+-rw-r--r--   0        0        0     4858 2024-04-18 00:36:04.833918 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/utils/hotfix_webp.py
+-rw-r--r--   0        0        0     1008 2024-04-18 00:36:04.833918 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/utils/loader.py
+-rw-r--r--   0        0        0     1130 2024-04-18 00:36:04.833918 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/utils/shell.py
+-rw-r--r--   0        0        0     1275 2024-04-18 00:36:04.833918 ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/utils/thumbnail.py
+-rw-r--r--   0        0        0     5866 1970-01-01 00:00:00.000000 ffmpeg_media_type-1.0.0/PKG-INFO
```

### Comparing `ffmpeg_media_type-0.0.9/LICENSE` & `ffmpeg_media_type-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.9/README.md` & `ffmpeg_media_type-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.9/pyproject.toml` & `ffmpeg_media_type-1.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 [tool.poetry]
 name = "ffmpeg-media-type"
-version = "0.0.9"
+version = "1.0.0"
 description = "ffmpeg-media-type is a Python library that utilizes FFmpeg to extract crucial details from media files, such as duration, width, and height. With seamless integration of 100% typehint support, it offers a user-friendly interface for easy access to media file information."
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "ffmpeg_media_type", from = "src" }]
-include = ["ffmpeg_media_type/py.typed", "ffmpeg_media_type/data/*.json"]
-exclude = ["**/tests"]
+include = ["ffmpeg_media_type/py.typed", "ffmpeg_media_type/cache/*.json"]
+exclude = ["**/tests", "**/test_data", "**/conftest.py"]
 keywords = ["ffmpeg", "ffprobe", "video", "image", "audio", "media", "mimetype", "mp4", "mp3", "mov", "webm"]
 classifiers = [
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
     ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pydantic = "*"
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 requests = "^2.31.0"
 beautifulsoup4 = "^4.12.2"
 prospector = "^1.10.2"
 bandit = "^1.7.5"
 pre-commit = "^3.3.3"
 mypy = "^1.4.1"
 typer = "^0.9.0"
-
-[tool.poetry.group.test.dependencies]
 syrupy = "^4.0.5"
 pytest = "^7.4.0"
 pytest-vcr = "^1.0.2"
 pytest-cov = "^4.1.0"
 
+[tool.poetry.scripts]
+rebuild = "scripts.main:app"
+
+
 [tool.poetry-dynamic-versioning]
 enable = false
 pattern = "default-unprefixed"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `ffmpeg_media_type-0.0.9/src/ffmpeg_media_type/info.py` & `ffmpeg_media_type-1.0.0/src/ffmpeg_media_type/info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,135 +1,121 @@
 import os
-from typing import Literal
 from urllib.parse import urlparse
 
-from pydantic import BaseModel
+from .schema import FFMpegSupport, MediaInfo
+from .utils.cache import load
+from .utils.ffprobe import ffprobe
+from .utils.thumbnail import generate_thumbnail
+
+
+def extract_file_extension_from_uri(uri: str) -> str:
+    """
+    Extract the file extension from a URI.
+
+    Args:
+        uri: the URI to extract the file extension from
+
+    Returns:
+        the file extension
+    """
 
-from .utils.ffmpeg import FFProbeInfo, ffprobe, get_ffmpeg, load_cache
-from .utils.shell import call
-
-
-class MediaInfo(BaseModel):
-    type: Literal["image", "video", "audio"]
-
-    width: int | None = None
-    height: int | None = None
-    duration: float | None = None
-
-    format: str | None = None
-    size: int | None = None
-    suggest_ext: str | None = None
-
-
-def generate_thumbnail(video_path: str, thumbnail_path: str, time_offset: float = 0) -> str:
-    ffmpeg_cmd = get_ffmpeg() + [
-        "-y",  # Overwrite output file if it exists
-        "-i",
-        video_path,  # Input video path
-        "-ss",
-        str(time_offset),  # Time offset (seek to the specified position)
-        "-vframes",
-        "1",  # Number of frames to output
-        "-vf",
-        "scale=320:-1",  # Thumbnail size (width: 320, height: proportional)
-        "-q:v",
-        "2",  # Quality (2 - high, 5 - low)
-        thumbnail_path,  # Output thumbnail path
-    ]
-
-    call(ffmpeg_cmd)
-
-    return thumbnail_path
-
-
-def _extract_file_extension(uri: str) -> str:
     parsed_uri = urlparse(uri)
     path = parsed_uri.path
     filename = os.path.basename(path)
     _, extension = os.path.splitext(filename)
     return extension[1:].lower()
 
 
-_KNOWN_CODEC_EXTS = {
-    "png_pipe": ["png"],
-    "svg_pipe": ["svg"],
-    "tiff_pipe": ["tiff", "tif"],
-    "bmp_pipe": ["bmp"],
-    "gif_pipe": ["gif"],
-    "jpeg_pipe": ["jpeg", "jpg"],
-    "webp_pipe": ["webp"],
-    "mjpeg": ["jpg", "jpeg", "mjpeg"],
+KNOWN_CODEC_EXTS = {
+    "png_pipe": ("png",),
+    "svg_pipe": ("svg",),
+    "tiff_pipe": ("tiff", "tif"),
+    "bmp_pipe": ("bmp",),
+    "gif_pipe": ("gif",),
+    "jpeg_pipe": ("jpeg", "jpg"),
+    "webp_pipe": ("webp",),
+    "mjpeg": ("jpg", "jpeg", "mjpeg"),
 }
+"""
+Dictionary mapping codec names to common file extensions.
+"""
 
 
-def _guess_media_info(
-    uri: str,
-    info: FFProbeInfo,
-) -> MediaInfo:
-    infos = load_cache()
-    current_ext = _extract_file_extension(uri)
+def detect(uri: str) -> MediaInfo:
+    """
+    Detect the media type of a file.
+
+    Args:
+        uri: the URI of the file
+
+    Returns:
+        the media type information
+
+    Raises:
+        FfmpegMediaTypeError: If the ffmpeg command fails.
+    """
+    info = ffprobe(uri)
+    current_ext = extract_file_extension_from_uri(uri)
 
     format_name = info.format.format_name
     duration = info.format.duration
 
     # NOTE: handle ffmpeg's image compatibility
     if format_name == "image2":
         format_name = info.streams[0].codec_name
 
     # NOTE: detect file extension
-    if format_name in _KNOWN_CODEC_EXTS:
-        common_exts = _KNOWN_CODEC_EXTS[format_name]
-    elif format_name in infos:
-        common_exts = infos[format_name].common_exts
+    if format_name in KNOWN_CODEC_EXTS:
+        common_exts = KNOWN_CODEC_EXTS[format_name]
+    elif support_info := load(FFMpegSupport, format_name):
+        common_exts = support_info.common_exts
     else:
-        common_exts = []
+        common_exts = ()
 
     if current_ext in common_exts:
         suggest_ext = current_ext
     elif common_exts:
         suggest_ext = common_exts[0]
     else:
         suggest_ext = None
 
     # NOTE: we classify gif as image
     if not duration or format_name in ("gif", "mjpeg"):
         return MediaInfo(
             type="image",
             width=info.streams[0].width or 0,
             height=info.streams[0].height or 0,
-            duration=duration or 0,
+            duration=float(duration) if duration is not None else None,
             format=format_name,
-            size=info.format.size,
+            size=int(info.format.size) if info.format.size is not None else None,
             suggest_ext=suggest_ext,
         )
 
     for stream in info.streams:
         # NOTE: if there is at least one video stream, the media is video
         if stream.codec_type == "video" and format_name not in ("mp3",):
             width = stream.width
             height = stream.height
 
             return MediaInfo(
                 type="video",
                 width=width or 0,
                 height=height or 0,
-                duration=duration or 0,
+                duration=float(duration) if duration is not None else None,
                 format=format_name,
-                size=info.format.size,
+                size=int(info.format.size) if info.format.size is not None else None,
                 suggest_ext=suggest_ext,
             )
 
     # NOTE: if there is no video stream, the media is audio
     return MediaInfo(
         type="audio",
         width=0,
         height=0,
-        duration=duration or 0,
+        duration=float(duration) if duration is not None else None,
         format=format_name,
-        size=info.format.size,
+        size=int(info.format.size) if info.format.size is not None else None,
         suggest_ext=suggest_ext,
     )
 
 
-def detect(uri: str) -> MediaInfo:
-    probe_info = ffprobe(uri)
-    return _guess_media_info(uri, probe_info)
+__all__ = ["detect", "generate_thumbnail"]
```

### Comparing `ffmpeg_media_type-0.0.9/PKG-INFO` & `ffmpeg_media_type-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ffmpeg-media-type
-Version: 0.0.9
+Version: 1.0.0
 Summary: ffmpeg-media-type is a Python library that utilizes FFmpeg to extract crucial details from media files, such as duration, width, and height. With seamless integration of 100% typehint support, it offers a user-friendly interface for easy access to media file information.
 Keywords: ffmpeg,ffprobe,video,image,audio,media,mimetype,mp4,mp3,mov,webm
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # ffmpeg-media-type
 
 `ffmpeg-media-type` is a Python library that utilizes FFmpeg to detect various media file information, such as duration, width, and height. This library provides an easy-to-use interface for extracting essential details from media files by leveraging the powerful capabilities of FFmpeg.
 
 [![CI](https://github.com/livingbio/ffmpeg-media-type/workflows/python-unittest/badge.svg?branch=main)](https://github.com/livingbio/ffmpeg-media-type/actions?query=workflow%3Apython-unittest++branch%3Amain++)
```

