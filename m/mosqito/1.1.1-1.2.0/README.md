# Comparing `tmp/mosqito-1.1.1.tar.gz` & `tmp/mosqito-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosqito-1.1.1.tar", last modified: Wed Feb  7 11:05:37 2024, max compression
+gzip compressed data, was "mosqito-1.2.0.tar", last modified: Thu Apr 18 19:08:35 2024, max compression
```

## Comparing `mosqito-1.1.1.tar` & `mosqito-1.2.0.tar`

### file list

```diff
@@ -1,149 +1,174 @@
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.825008 mosqito-1.1.1/
--rw-rw-rw-   0        0        0    11558 2024-02-07 11:04:08.000000 mosqito-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       89 2024-02-07 11:04:08.000000 mosqito-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6371 2024-02-07 11:05:37.825008 mosqito-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5831 2024-02-07 11:04:08.000000 mosqito-1.1.1/README.md
--rw-rw-rw-   0        0        0    15006 2024-02-07 11:04:08.000000 mosqito-1.1.1/logo.png
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.182522 mosqito-1.1.1/mosqito/
--rw-rw-rw-   0        0        0     2636 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.238245 mosqito-1.1.1/mosqito/sound_level_meter/
--rw-rw-rw-   0        0        0      300 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/__init__.py
--rw-rw-rw-   0        0        0     2690 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/freq_band_synthesis.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.336739 mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/__init__.py
--rw-rw-rw-   0        0        0     2337 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_center_freq.py
--rw-rw-rw-   0        0        0     2152 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_filter_bandwidth.py
--rw-rw-rw-   0        0        0     1110 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_getFrequencies.py
--rw-rw-rw-   0        0        0     1296 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_n_oct_freq_filter.py
--rw-rw-rw-   0        0        0     2027 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_n_oct_time_filter.py
--rw-rw-rw-   0        0        0      813 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_nominal_frequency.py
--rw-rw-rw-   0        0        0     2053 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/noct_spectrum.py
--rw-rw-rw-   0        0        0     2786 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/noct_synthesis.py
--rw-rw-rw-   0        0        0     1875 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sound_level_meter/spectrum.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.340725 mosqito-1.1.1/mosqito/sq_metrics/
--rw-rw-rw-   0        0        0     2104 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.348679 mosqito-1.1.1/mosqito/sq_metrics/loudness/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.431264 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/__init__.py
--rw-rw-rw-   0        0        0      838 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_auditory_filters_centre_freq.py
--rw-rw-rw-   0        0        0     1290 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_ear_filter_design.py
--rw-rw-rw-   0        0        0     3206 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_gammatone.py
--rw-rw-rw-   0        0        0      836 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_ecma_data.py
--rw-rw-rw-   0        0        0      919 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_nonlinearity.py
--rw-rw-rw-   0        0        0     3686 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_rectified_band_pass_signals.py
--rw-rw-rw-   0        0        0     3182 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/loudness_ecma.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.486983 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/__init__.py
--rw-rw-rw-   0        0        0    14672 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/_calc_slopes.py
--rw-rw-rw-   0        0        0     1252 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/_get_rns_index.py
--rw-rw-rw-   0        0        0     7753 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/_main_loudness.py
--rw-rw-rw-   0        0        0     2510 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst.py
--rw-rw-rw-   0        0        0     5026 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_freq.py
--rw-rw-rw-   0        0        0     2408 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_perseg.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.520805 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/__init__.py
--rw-rw-rw-   0        0        0     1718 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/_lowpass_intp.py
--rw-rw-rw-   0        0        0     6174 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/_nonlinear_decay.py
--rw-rw-rw-   0        0        0      998 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/_square_and_smooth.py
--rw-rw-rw-   0        0        0     1026 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/_temporal_weighting.py
--rw-rw-rw-   0        0        0     9834 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/_third_octave_levels.py
--rw-rw-rw-   0        0        0     2896 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/loudness_zwtv.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.540702 mosqito-1.1.1/mosqito/sq_metrics/loudness/utils/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/utils/__init__.py
--rw-rw-rw-   0        0        0     2569 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/utils/equal_loudness_contours.py
--rw-rw-rw-   0        0        0      949 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/utils/phone2spl.py
--rw-rw-rw-   0        0        0      984 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/utils/sone2phone.py
--rw-rw-rw-   0        0        0      744 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/loudness/utils/sone_to_phon.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.544683 mosqito-1.1.1/mosqito/sq_metrics/roughness/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/roughness/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.582493 mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/
--rw-rw-rw-   0        0        0     5052 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/_H_weighting.py
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/__init__.py
--rw-rw-rw-   0        0        0     1323 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/_ear_filter_coeff.py
--rw-rw-rw-   0        0        0      853 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/_gzi_weighting.py
--rw-rw-rw-   0        0        0     6971 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/_roughness_dw_main_calc.py
--rw-rw-rw-   0        0        0     2745 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw.py
--rw-rw-rw-   0        0        0     2951 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw_freq.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.587467 mosqito-1.1.1/mosqito/sq_metrics/sharpness/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/sharpness/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.618308 mosqito-1.1.1/mosqito/sq_metrics/sharpness/sharpness_din/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/sharpness/sharpness_din/__init__.py
--rw-rw-rw-   0        0        0     2147 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/sharpness/sharpness_din/_weighting_fastl.py
--rw-rw-rw-   0        0        0     4196 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_freq.py
--rw-rw-rw-   0        0        0     2200 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_from_loudness.py
--rw-rw-rw-   0        0        0     1879 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_perseg.py
--rw-rw-rw-   0        0        0     1451 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_st.py
--rw-rw-rw-   0        0        0     2021 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_tv.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.621292 mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.654877 mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/__init__.py
--rw-rw-rw-   0        0        0    10696 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_band_procedure_data.py
--rw-rw-rw-   0        0        0     4765 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_main_sii.py
--rw-rw-rw-   0        0        0     7741 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_speech_data.py
--rw-rw-rw-   0        0        0     4735 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi.py
--rw-rw-rw-   0        0        0     5012 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_freq.py
--rw-rw-rw-   0        0        0     4372 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_level.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.661843 mosqito-1.1.1/mosqito/sq_metrics/tonality/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.681741 mosqito-1.1.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/__init__.py
--rw-rw-rw-   0        0        0     8331 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/_pr_main_calc.py
--rw-rw-rw-   0        0        0     1644 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_freq.py
--rw-rw-rw-   0        0        0     1432 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_st.py
--rw-rw-rw-   0        0        0     3000 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_tv.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.723525 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/
--rw-rw-rw-   0        0        0     1388 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_LTH.py
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/__init__.py
--rw-rw-rw-   0        0        0     1566 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_critical_band.py
--rw-rw-rw-   0        0        0     2304 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_find_highest_tone.py
--rw-rw-rw-   0        0        0     2251 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_peak_level.py
--rw-rw-rw-   0        0        0     6198 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_screening_for_tones.py
--rw-rw-rw-   0        0        0     3614 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_spectrum_smoothing.py
--rw-rw-rw-   0        0        0     9759 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_tnr_main_calc.py
--rw-rw-rw-   0        0        0     1654 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_freq.py
--rw-rw-rw-   0        0        0     1465 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_st.py
--rw-rw-rw-   0        0        0     3075 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_tv.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.756358 mosqito-1.1.1/mosqito/utils/
--rw-rw-rw-   0        0        0     5385 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/utils/LTQ.py
--rw-rw-rw-   0        0        0      212 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/utils/__init__.py
--rw-rw-rw-   0        0        0     6507 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/utils/conversion.py
--rw-rw-rw-   0        0        0     2106 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/utils/isoclose.py
--rw-rw-rw-   0        0        0     2852 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/utils/load.py
--rw-rw-rw-   0        0        0     1266 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/utils/sine_wave_generator.py
--rw-rw-rw-   0        0        0     1725 2024-02-07 11:04:08.000000 mosqito-1.1.1/mosqito/utils/time_segmentation.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.224309 mosqito-1.1.1/mosqito.egg-info/
--rw-rw-rw-   0        0        0     6371 2024-02-07 11:05:36.000000 mosqito-1.1.1/mosqito.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6103 2024-02-07 11:05:36.000000 mosqito-1.1.1/mosqito.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-07 11:05:36.000000 mosqito-1.1.1/mosqito.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-02-07 11:05:36.000000 mosqito-1.1.1/mosqito.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-02-07 11:05:36.000000 mosqito-1.1.1/mosqito.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       21 2024-02-07 11:04:08.000000 mosqito-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0       86 2024-02-07 11:05:37.826998 mosqito-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1482 2024-02-07 11:04:08.000000 mosqito-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:36.781263 mosqito-1.1.1/tests/
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.762329 mosqito-1.1.1/tests/output/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/output/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.767308 mosqito-1.1.1/tests/sq_metrics/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.783227 mosqito-1.1.1/tests/sq_metrics/loudness/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/loudness/__init__.py
--rw-rw-rw-   0        0        0     1442 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/loudness/test_loudness_ecma.py
--rw-rw-rw-   0        0        0     6693 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/loudness/test_loudness_zwst.py
--rw-rw-rw-   0        0        0     1915 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/loudness/test_loudness_zwtv.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.793175 mosqito-1.1.1/tests/sq_metrics/roughness/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/roughness/__init__.py
--rw-rw-rw-   0        0        0     2167 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/roughness/signals_test_generation.py
--rw-rw-rw-   0        0        0     3700 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/roughness/test_roughness_dw.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.800136 mosqito-1.1.1/tests/sq_metrics/sharpness/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/sharpness/__init__.py
--rw-rw-rw-   0        0        0     6884 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/sharpness/test_sharpness_din.py
-drwxrwxrwx   0        0        0        0 2024-02-07 11:05:37.822024 mosqito-1.1.1/tests/sq_metrics/tonality/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/tonality/__init__.py
--rw-rw-rw-   0        0        0     1871 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/tonality/test_pr_ecma_freq.py
--rw-rw-rw-   0        0        0     1408 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/tonality/test_pr_ecma_st.py
--rw-rw-rw-   0        0        0     1475 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/tonality/test_pr_ecma_tv.py
--rw-rw-rw-   0        0        0     1845 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/tonality/test_tnr_ecma_freq.py
--rw-rw-rw-   0        0        0     1447 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/tonality/test_tnr_ecma_st.py
--rw-rw-rw-   0        0        0     1459 2024-02-07 11:04:08.000000 mosqito-1.1.1/tests/sq_metrics/tonality/test_tnr_ecma_tv.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.471934 mosqito-1.2.0/
+-rw-rw-rw-   0        0        0    11558 2024-02-07 11:04:08.000000 mosqito-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       89 2024-02-07 11:04:08.000000 mosqito-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1446 2024-04-18 19:08:35.470936 mosqito-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      840 2024-04-18 15:23:21.000000 mosqito-1.2.0/README.md
+-rw-rw-rw-   0        0        0    15006 2024-02-07 11:04:08.000000 mosqito-1.2.0/logo.png
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.047148 mosqito-1.2.0/mosqito/
+-rw-rw-rw-   0        0        0     3545 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.075150 mosqito-1.2.0/mosqito/sound_level_meter/
+-rw-rw-rw-   0        0        0      798 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/__init__.py
+-rw-rw-rw-   0        0        0     2946 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/comp_spectrum.py
+-rw-rw-rw-   0        0        0     2765 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/freq_band_synthesis.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.110152 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/__init__.py
+-rw-rw-rw-   0        0        0     2350 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_center_freq.py
+-rw-rw-rw-   0        0        0     2153 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_filter_bandwidth.py
+-rw-rw-rw-   0        0        0     1121 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_getFrequencies.py
+-rw-rw-rw-   0        0        0     1308 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_n_oct_freq_filter.py
+-rw-rw-rw-   0        0        0     2031 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_n_oct_time_filter.py
+-rw-rw-rw-   0        0        0      813 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_nominal_frequency.py
+-rw-rw-rw-   0        0        0     3119 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/noct_spectrum.py
+-rw-rw-rw-   0        0        0     3660 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/noct_synthesis.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.112152 mosqito-1.2.0/mosqito/sq_metrics/
+-rw-rw-rw-   0        0        0     2760 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.115156 mosqito-1.2.0/mosqito/sq_metrics/loudness/
+-rw-rw-rw-   0        0        0     1252 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.145236 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/__init__.py
+-rw-rw-rw-   0        0        0      837 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_auditory_filters_centre_freq.py
+-rw-rw-rw-   0        0        0     5570 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_band_pass_signals.py
+-rw-rw-rw-   0        0        0     1395 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_ear_filter_design.py
+-rw-rw-rw-   0        0        0     2259 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_ecma_time_segmentation.py
+-rw-rw-rw-   0        0        0     1977 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_gammatone.py
+-rw-rw-rw-   0        0        0      838 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_ecma_data.py
+-rw-rw-rw-   0        0        0     2481 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_from_bandpass.py
+-rw-rw-rw-   0        0        0      996 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_nonlinearity.py
+-rw-rw-rw-   0        0        0     1118 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_preprocessing.py
+-rw-rw-rw-   0        0        0     4769 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/loudness_ecma.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.178238 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/__init__.py
+-rw-rw-rw-   0        0        0    14615 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_calc_slopes.py
+-rw-rw-rw-   0        0        0     1270 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_get_rns_index.py
+-rw-rw-rw-   0        0        0     7678 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_main_loudness.py
+-rw-rw-rw-   0        0        0     4097 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst.py
+-rw-rw-rw-   0        0        0     7209 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_freq.py
+-rw-rw-rw-   0        0        0     4309 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_perseg.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.201239 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/__init__.py
+-rw-rw-rw-   0        0        0     1657 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_lowpass_intp.py
+-rw-rw-rw-   0        0        0     6284 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_nonlinear_decay.py
+-rw-rw-rw-   0        0        0      925 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_square_and_smooth.py
+-rw-rw-rw-   0        0        0      950 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_temporal_weighting.py
+-rw-rw-rw-   0        0        0     9700 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_third_octave_levels.py
+-rw-rw-rw-   0        0        0     4690 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/loudness_zwtv.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.217240 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/__init__.py
+-rw-rw-rw-   0        0        0     3505 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/equal_loudness_contours.py
+-rw-rw-rw-   0        0        0      913 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/phone2spl.py
+-rw-rw-rw-   0        0        0      929 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/sone2phone.py
+-rw-rw-rw-   0        0        0      681 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/sone_to_phon.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.219241 mosqito-1.2.0/mosqito/sq_metrics/roughness/
+-rw-rw-rw-   0        0        0      782 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.241243 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/
+-rw-rw-rw-   0        0        0     4959 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_H_weighting.py
+-rw-rw-rw-   0        0        0      276 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/__init__.py
+-rw-rw-rw-   0        0        0     1291 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_ear_filter_coeff.py
+-rw-rw-rw-   0        0        0      820 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_gzi_weighting.py
+-rw-rw-rw-   0        0        0     6966 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_roughness_dw_main_calc.py
+-rw-rw-rw-   0        0        0     3964 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw.py
+-rw-rw-rw-   0        0        0     5370 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw_freq.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.273919 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/
+-rw-rw-rw-   0        0        0      216 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/__init__.py
+-rw-rw-rw-   0        0        0     2303 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_estimate_fund_mod_rate.py
+-rw-rw-rw-   0        0        0     1090 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_interpolation_50.py
+-rw-rw-rw-   0        0        0     1779 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_lowpass_filter.py
+-rw-rw-rw-   0        0        0     1516 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_noise_reduction.py
+-rw-rw-rw-   0        0        0     1588 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_non_linear_transform.py
+-rw-rw-rw-   0        0        0     2454 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_peak_picking.py
+-rw-rw-rw-   0        0        0     2655 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_refinement.py
+-rw-rw-rw-   0        0        0      432 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_von_hann_window.py
+-rw-rw-rw-   0        0        0     4009 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_weighting.py
+-rw-rw-rw-   0        0        0     8364 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/roughness_ecma.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.278923 mosqito-1.2.0/mosqito/sq_metrics/sharpness/
+-rw-rw-rw-   0        0        0     1112 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.297920 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/
+-rw-rw-rw-   0        0        0      484 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/__init__.py
+-rw-rw-rw-   0        0        0     2148 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/_weighting_fastl.py
+-rw-rw-rw-   0        0        0     6708 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_freq.py
+-rw-rw-rw-   0        0        0     4454 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_from_loudness.py
+-rw-rw-rw-   0        0        0     3935 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_perseg.py
+-rw-rw-rw-   0        0        0     3858 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_st.py
+-rw-rw-rw-   0        0        0     4102 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_tv.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.299920 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/
+-rw-rw-rw-   0        0        0      778 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.317923 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/__init__.py
+-rw-rw-rw-   0        0        0    11748 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_band_procedure_data.py
+-rw-rw-rw-   0        0        0     5730 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_main_sii.py
+-rw-rw-rw-   0        0        0     9141 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_speech_data.py
+-rw-rw-rw-   0        0        0     6062 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi.py
+-rw-rw-rw-   0        0        0     6244 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_freq.py
+-rw-rw-rw-   0        0        0     5779 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_level.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.319923 mosqito-1.2.0/mosqito/sq_metrics/tonality/
+-rw-rw-rw-   0        0        0     1371 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.333923 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/__init__.py
+-rw-rw-rw-   0        0        0     8281 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/_pr_main_calc.py
+-rw-rw-rw-   0        0        0     5737 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_freq.py
+-rw-rw-rw-   0        0        0     5849 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_perseg.py
+-rw-rw-rw-   0        0        0     5188 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_st.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.364926 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/
+-rw-rw-rw-   0        0        0     1318 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_LTH.py
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/__init__.py
+-rw-rw-rw-   0        0        0     1532 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_critical_band.py
+-rw-rw-rw-   0        0        0     2253 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_find_highest_tone.py
+-rw-rw-rw-   0        0        0     2156 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_peak_level.py
+-rw-rw-rw-   0        0        0     6128 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_screening_for_tones.py
+-rw-rw-rw-   0        0        0     3570 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_spectrum_smoothing.py
+-rw-rw-rw-   0        0        0     9680 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_tnr_main_calc.py
+-rw-rw-rw-   0        0        0     5718 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_freq.py
+-rw-rw-rw-   0        0        0     5879 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_perseg.py
+-rw-rw-rw-   0        0        0     5226 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_st.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.386928 mosqito-1.2.0/mosqito/utils/
+-rw-rw-rw-   0        0        0     5315 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/LTQ.py
+-rw-rw-rw-   0        0        0     1793 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/utils/__init__.py
+-rw-rw-rw-   0        0        0     3693 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/utils/am_noise_generator.py
+-rw-rw-rw-   0        0        0     4067 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/utils/am_sine_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.401928 mosqito-1.2.0/mosqito/utils/conversion/
+-rw-rw-rw-   0        0        0        0 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/__init__.py
+-rw-rw-rw-   0        0        0      671 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/amp2db.py
+-rw-rw-rw-   0        0        0     1781 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/bark2freq.py
+-rw-rw-rw-   0        0        0      531 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/db2amp.py
+-rw-rw-rw-   0        0        0     1789 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/freq2bark.py
+-rw-rw-rw-   0        0        0     3619 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/spectrum2dBA.py
+-rw-rw-rw-   0        0        0     4265 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/utils/fm_sine_generator.py
+-rw-rw-rw-   0        0        0     2251 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/isoclose.py
+-rw-rw-rw-   0        0        0     2901 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/load.py
+-rw-rw-rw-   0        0        0     1963 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/utils/sine_wave_generator.py
+-rw-rw-rw-   0        0        0     1735 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/time_segmentation.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.468934 mosqito-1.2.0/mosqito.egg-info/
+-rw-rw-rw-   0        0        0     1446 2024-04-18 19:08:34.000000 mosqito-1.2.0/mosqito.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7348 2024-04-18 19:08:34.000000 mosqito-1.2.0/mosqito.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 19:08:34.000000 mosqito-1.2.0/mosqito.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-18 19:08:34.000000 mosqito-1.2.0/mosqito.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-18 19:08:34.000000 mosqito-1.2.0/mosqito.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       21 2024-02-07 11:04:08.000000 mosqito-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2024-04-18 19:08:35.474944 mosqito-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1495 2024-03-28 15:18:23.000000 mosqito-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.005145 mosqito-1.2.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.405930 mosqito-1.2.0/tests/output/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/output/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.407931 mosqito-1.2.0/tests/sq_metrics/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/sq_metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.416933 mosqito-1.2.0/tests/sq_metrics/loudness/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/sq_metrics/loudness/__init__.py
+-rw-rw-rw-   0        0        0     1205 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_ecma.py
+-rw-rw-rw-   0        0        0     6728 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_zwst.py
+-rw-rw-rw-   0        0        0     1913 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_zwtv.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.426930 mosqito-1.2.0/tests/sq_metrics/roughness/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/sq_metrics/roughness/__init__.py
+-rw-rw-rw-   0        0        0     4743 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/roughness/signals_test_generation.py
+-rw-rw-rw-   0        0        0     3834 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/roughness/test_roughness_dw.py
+-rw-rw-rw-   0        0        0     2280 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/roughness/test_roughness_ecma.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.435931 mosqito-1.2.0/tests/sq_metrics/sharpness/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/sq_metrics/sharpness/__init__.py
+-rw-rw-rw-   0        0        0     6885 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/sharpness/test_sharpness_din.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.463935 mosqito-1.2.0/tests/sq_metrics/tonality/
+-rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/sq_metrics/tonality/__init__.py
+-rw-rw-rw-   0        0        0     1837 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_freq.py
+-rw-rw-rw-   0        0        0     1310 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_st.py
+-rw-rw-rw-   0        0        0     1399 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_tv.py
+-rw-rw-rw-   0        0        0     1819 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_freq.py
+-rw-rw-rw-   0        0        0     1411 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_st.py
+-rw-rw-rw-   0        0        0     1502 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_tv.py
```

### Comparing `mosqito-1.1.1/LICENSE` & `mosqito-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosqito-1.1.1/logo.png` & `mosqito-1.2.0/logo.png`

 * *Files identical despite different names*

### Comparing `mosqito-1.1.1/mosqito/__init__.py` & `mosqito-1.2.0/mosqito/sq_metrics/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,66 @@
-from mosqito.sound_level_meter.noct_spectrum.noct_spectrum import noct_spectrum
-from mosqito.sound_level_meter.noct_spectrum.noct_synthesis import noct_synthesis
-from mosqito.sound_level_meter.spectrum import spectrum
+"""This module includes functions to compute the main sound quality metrics :
+
+   
+
+.. toctree::
+   :maxdepth: 2
+   
+   Loudness </source/reference/mosqito.sq_metrics.loudness>
+   Sharpness </source/reference/mosqito.sq_metrics.sharpness>
+   Roughness </source/reference/mosqito.sq_metrics.roughness>
+   Tonality </source/reference/mosqito.sq_metrics.tonality>
+   Speech Intelligibility </source/reference/mosqito.sq_metrics.speech_intelligibility>
+
+"""
+
+__all__ = ["sq_metrics"]
 
 from mosqito.sq_metrics.loudness.loudness_ecma.loudness_ecma import loudness_ecma
 from mosqito.sq_metrics.loudness.loudness_zwst.loudness_zwst import loudness_zwst
-from mosqito.sq_metrics.loudness.loudness_zwst.loudness_zwst_freq import loudness_zwst_freq
-from mosqito.sq_metrics.loudness.loudness_zwst.loudness_zwst_perseg import loudness_zwst_perseg
+from mosqito.sq_metrics.loudness.loudness_zwst.loudness_zwst_freq import (
+    loudness_zwst_freq,
+)
+from mosqito.sq_metrics.loudness.loudness_zwst.loudness_zwst_perseg import (
+    loudness_zwst_perseg,
+)
 
 from mosqito.sq_metrics.loudness.loudness_zwtv.loudness_zwtv import loudness_zwtv
-
-from mosqito.sq_metrics.loudness.utils.equal_loudness_contours import equal_loudness_contours
+from mosqito.sq_metrics.loudness.utils.equal_loudness_contours import (
+    equal_loudness_contours,
+)
 
 from mosqito.sq_metrics.tonality.prominence_ratio_ecma.pr_ecma_st import pr_ecma_st
-from mosqito.sq_metrics.tonality.prominence_ratio_ecma.pr_ecma_tv import pr_ecma_tv
+from mosqito.sq_metrics.tonality.prominence_ratio_ecma.pr_ecma_perseg import (
+    pr_ecma_perseg,
+)
 from mosqito.sq_metrics.tonality.prominence_ratio_ecma.pr_ecma_freq import pr_ecma_freq
 
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma.tnr_ecma_st import tnr_ecma_st
-from mosqito.sq_metrics.tonality.tone_to_noise_ecma.tnr_ecma_tv import tnr_ecma_tv
+from mosqito.sq_metrics.tonality.tone_to_noise_ecma.tnr_ecma_perseg import (
+    tnr_ecma_perseg,
+)
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma.tnr_ecma_freq import tnr_ecma_freq
 
 from mosqito.sq_metrics.roughness.roughness_dw.roughness_dw import roughness_dw
 from mosqito.sq_metrics.roughness.roughness_dw.roughness_dw_freq import roughness_dw_freq
-
+from mosqito.sq_metrics.roughness.roughness_ecma.roughness_ecma import roughness_ecma
 
 from mosqito.sq_metrics.sharpness.sharpness_din.sharpness_din_st import sharpness_din_st
 from mosqito.sq_metrics.sharpness.sharpness_din.sharpness_din_tv import sharpness_din_tv
-from mosqito.sq_metrics.sharpness.sharpness_din.sharpness_din_from_loudness import sharpness_din_from_loudness
-from mosqito.sq_metrics.sharpness.sharpness_din.sharpness_din_perseg import sharpness_din_perseg
-from mosqito.sq_metrics.sharpness.sharpness_din.sharpness_din_freq import sharpness_din_freq
+from mosqito.sq_metrics.sharpness.sharpness_din.sharpness_din_from_loudness import (
+    sharpness_din_from_loudness,
+)
+from mosqito.sq_metrics.sharpness.sharpness_din.sharpness_din_perseg import (
+    sharpness_din_perseg,
+)
+from mosqito.sq_metrics.sharpness.sharpness_din.sharpness_din_freq import (
+    sharpness_din_freq,
+)
 
+from mosqito.sq_metrics.loudness.utils.sone_to_phon import sone_to_phon
 from mosqito.sq_metrics.speech_intelligibility.sii_ansi.sii_ansi import sii_ansi
 from mosqito.sq_metrics.speech_intelligibility.sii_ansi.sii_ansi_freq import sii_ansi_freq
-from mosqito.sq_metrics.speech_intelligibility.sii_ansi.sii_ansi_level import sii_ansi_level
 
-from mosqito.sq_metrics.loudness.utils.sone_to_phon import sone_to_phon
-from mosqito.utils.isoclose import isoclose
-from mosqito.utils.load import load
-from mosqito.utils.sine_wave_generator import sine_wave_generator
-from mosqito.utils.time_segmentation import time_segmentation
-
-# Colors and linestyles
-COLORS = [
-    "#69c3c5",
-    "#ffd788",
-    "#ff8b88",
-    "#7894cf",
-    "#228080",
-    "#a8e2e2"
-]
+from mosqito.sq_metrics.speech_intelligibility.sii_ansi.sii_ansi_level import (
+    sii_ansi_level,
+)
```

### Comparing `mosqito-1.1.1/mosqito/sound_level_meter/freq_band_synthesis.py` & `mosqito-1.2.0/mosqito/sound_level_meter/freq_band_synthesis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 # -*- coding: utf-8 -*-
 
 # Standard library import
-from numpy import array, concatenate, zeros, log10, power, argmin, split, arange, interp, iscomplex
+from numpy import (
+    array,
+    concatenate,
+    zeros,
+    log10,
+    power,
+    argmin,
+    split,
+    arange,
+    interp,
+    iscomplex,
+)
+
 
 def freq_band_synthesis(spectrum, freqs, fmin, fmax):
     """Adapt input spectrum to frequency band levels
-    
+
     Convert the input spectrum to frequency band spectrum
     between "fmin" and "fmax".
-    
+
     Parameters
     ----------
     spectrum : numpy.ndarray
         One-sided spectrum of the signal in [dB], size (nperseg, nseg).
     freqs : list
         List of input frequency , size (nperseg) or (nperseg, nseg).
     fmin : float
@@ -32,43 +44,41 @@
     -------
     spec : numpy.ndarray
         Third octave band spectrum of signal sig [dB re.2e-5 Pa], size (nbands, nseg).
     fpref : numpy.ndarray
         Corresponding preferred third octave band center frequencies, size (nbands).
     """
     if iscomplex(spectrum).any():
-        raise ValueError('Input spectrum must be in dB, no complex value allowed.')
-    
-    if (fmin.min() < freqs.min()):
-        print("[WARNING] Input spectrum minimum frequency if higher than fmin. Empty values will be filled with 0.")
+        raise ValueError("Input spectrum must be in dB, no complex value allowed.")
+
+    if fmin.min() < freqs.min():
+        print(
+            "[WARNING] Input spectrum minimum frequency if higher than fmin. Empty values will be filled with 0."
+        )
         df = freqs[1] - freqs[0]
-        spectrum = interp(arange(fmin.min(),fmax.max()+df, df), freqs, spectrum)
-        freqs = arange(fmin.min(),fmax.max()+df, df)
+        spectrum = interp(arange(fmin.min(), fmax.max() + df, df), freqs, spectrum)
+        freqs = arange(fmin.min(), fmax.max() + df, df)
 
-    if (fmax.max() > freqs.max()):
-        print("[WARNING] Input spectrum maximum frequency if lower than fmax. Empty values will be filled with 0.")
+    if fmax.max() > freqs.max():
+        print(
+            "[WARNING] Input spectrum maximum frequency if lower than fmax. Empty values will be filled with 0."
+        )
         df = freqs[1] - freqs[0]
-        spectrum = interp(arange(fmin.min(),fmax.max()+df, df), freqs, spectrum)
-        freqs = arange(fmin.min(),fmax.max()+df, df)
-    
+        spectrum = interp(arange(fmin.min(), fmax.max() + df, df), freqs, spectrum)
+        freqs = arange(fmin.min(), fmax.max() + df, df)
+
     # Find the lower and upper index of each band
-    idx_low = argmin(abs(freqs[:,None] - fmin), axis=0)
-    idx_up = argmin(abs(freqs[:,None] - fmax), axis=0)
+    idx_low = argmin(abs(freqs[:, None] - fmin), axis=0)
+    idx_up = argmin(abs(freqs[:, None] - fmax), axis=0)
     idx = concatenate((idx_low, [idx_up[-1]]))
-    
+
     # Split the given spectrum in several bands
     bands = array(split(spectrum, idx), dtype=object)[1:-1]
-    
+
     # Compute the bands level
     band_spectrum = zeros((len(bands)))
     i = 0
     for s in bands:
-        band_spectrum[i] = 10*log10(sum(power(10,s/10)))      
+        band_spectrum[i] = 10 * log10(sum(power(10, s / 10)))
         i += 1
 
-    return band_spectrum, (fmin+fmax)/2
-
-
-        
-
-
-
+    return band_spectrum, (fmin + fmax) / 2
```

### Comparing `mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_center_freq.py` & `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_center_freq.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import numpy as np
+from numpy import array, log10, where, arange, round
 
 from mosqito.sound_level_meter.noct_spectrum._nominal_frequency import (
     NOMINAL_OCTAVE_CENTER_FREQUENCIES,
     NOMINAL_THIRD_OCTAVE_CENTER_FREQUENCIES,
 )
 
 
@@ -44,19 +44,19 @@
     elif G == 10:
         U = 10 ** (3 * b / 10)  # ANSI eq4
     else:
         raise ValueError(
             """ERROR: Only base 2 and base 10 are allowed for nth
             octave center frequency definition"""
         )
-    [kmin, kmax] = np.round(
-        np.log10(np.array([fmin, fmax]) / fr) / np.log10(U), 0)
+    [kmin, kmax] = round(
+        log10(array([fmin, fmax]) / fr) / log10(U), 0)
 
     # Band numbers such that f_exact = fr for k=0
-    k = np.arange(kmin, kmax + 1).astype(int)
+    k = arange(kmin, kmax + 1).astype(int)
 
     # compute ANSI eq1
     f_exact = fr * U ** k
 
     ####
     # get normalized frequencies
     ####
@@ -64,16 +64,16 @@
     f_nom = f_exact.copy()
 
     if n == 1:
         freq = NOMINAL_OCTAVE_CENTER_FREQUENCIES
     elif n == 3:
         freq = NOMINAL_THIRD_OCTAVE_CENTER_FREQUENCIES
     if n == 1 or n == 3:
-        i_ref = np.where(freq == fr)[0][0]
-        ind = np.where((k >= -i_ref) & (k < (len(freq) - i_ref)))
+        i_ref = where(freq == fr)[0][0]
+        ind = where((k >= -i_ref) & (k < (len(freq) - i_ref)))
         f_nom = freq[k[ind] + i_ref]
 
     # TODO
     # Manage other values of n
     # Manage band outside the known bands
 
     return f_exact, f_nom
```

### Comparing `mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_filter_bandwidth.py` & `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_filter_bandwidth.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 # Standard library imports
-import numpy as np
+from numpy import pi, sin, sqrt
 
 
 def _filter_bandwidth(fc, n=3, N=3):
     """Define nth octave filter bandwidth
 
     The filter bandwidth is designed according to the Order-N
     specification of the ANSI S1.1-1986 standard. Default
@@ -51,16 +51,16 @@
     # ANSI S1.1-1986.
     b = 1 / n
     f1 = fc / (2 ** (b / 2))  # ANSI eq5
     f2 = fc * (2 ** (b / 2))  # ANSI eq6
     # Reference bandwidth quotient
     qr = fc / (f2 - f1)  # ANSI eq7 & 8
     # Design bandwidth quotient
-    qd = (np.pi / 2 / N) / (np.sin(np.pi / 2 / N)) * qr  # ANSI eq9
+    qd = (pi / 2 / N) / (sin(pi / 2 / N)) * qr  # ANSI eq9
     # Ratio of the upper and lower band-edge frequencies to the mid-band frequency
-    alpha = (1 + np.sqrt(1 + 4 * qd ** 2)) / 2 / qd
+    alpha = (1 + sqrt(1 + 4 * qd ** 2)) / 2 / qd
 
     return alpha, f1, f2
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_getFrequencies.py` & `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_getFrequencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import numpy as np
+from numpy import array, empty, append
 
 
 def _getFrequencies(fstart, fend, b, G=10, fr=1000):
     """
     Calculate octave filter specifications
     :param fstart: start frequency
     :param fend: end frequency
     :param b: number of bands pr octave
     :param G: base
     :param fr: reference frequency
     :return: filter specification dict
     """
 
     # frequency matrix
-    freqs = np.empty((0, 3))
+    freqs = empty((0, 3))
 
     if G == 10:
         G = 10 ** (3 / 10)  # Base ten
     elif G == 2:
         G = 2
     else:
         print("The base system is not permitted. G must be 10 or 2")
@@ -31,10 +31,10 @@
             fm = (G ** ((2 * x - 59) / (2 * b))) * (fr)
         else:  # odd
             fm = (G ** ((x - 30) / b)) * (fr)
         # Bandedge frequencies
         f1 = (G ** (-1 / (2 * b))) * (fm)
         f2 = (G ** (1 / (2 * b))) * (fm)
         if f2 >= fstart:
-            freqs = np.append(freqs, np.array([[f1, fm, f2]]), axis=0)
+            freqs = append(freqs, array([[f1, fm, f2]]), axis=0)
         x += 1
     return {"f": freqs, "b": b, "G": G}
```

### Comparing `mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_n_oct_freq_filter.py` & `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_n_oct_freq_filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 
 # Standard library imports
-import numpy as np
+from numpy import multiply, sqrt, sum, abs
 from scipy.signal import butter, sosfreqz
 
 def _n_oct_freq_filter(spectrum, fs, fc, alpha, n=3):  
     """ n-th octave filtering in frequency domain
 
     Designs a digital 1/3-octave filter with center frequency fc for
     sampling frequency fs. 
@@ -35,13 +35,13 @@
     w1 = fc / (fs  / 2) / alpha
     w2 = fc / (fs  / 2) * alpha
 
     # Define filter coefficient
     sos = butter(n, [w1, w2], "bandpass", analog=False, output ='sos')  
     # Get FRF and apply it
     w, h = sosfreqz(sos, worN=len(spectrum))
-    spec_filt = np.multiply(h, spectrum.T).T
+    spec_filt = multiply(h, spectrum.T).T
     
     # Compute overall rms level
-    level = np.sqrt(np.sum(np.abs(spec_filt) ** 2, axis=0)) 
+    level = sqrt(sum(abs(spec_filt) ** 2, axis=0)) 
         
     return level
```

### Comparing `mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_n_oct_time_filter.py` & `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_n_oct_time_filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 # Standard library imports
-import numpy as np
+from numpy import sqrt, mean
 from scipy.signal import decimate, butter, sosfilt
 
 
 def _n_oct_time_filter(sig, fs, fc, alpha, N=3):
     """Design of a nth octave filter set
 
     Designs a digital 1/3-octave filter with center frequency fc for
@@ -61,14 +61,14 @@
     # define filter coefficient
     sos = butter(int(N), (w1, w2), "bandpass", analog=False, output='sos')
 
     # filter signal
     sig_filt = sosfilt(sos, sig, axis=0)
 
     # Compute overall rms level
-    level = np.sqrt(np.mean(sig_filt ** 2, axis=0))
+    level = sqrt(mean(sig_filt ** 2, axis=0))
 
     return level
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/_nominal_frequency.py` & `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_nominal_frequency.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.1.1/mosqito/sound_level_meter/noct_spectrum/noct_synthesis.py` & `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/noct_synthesis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,100 @@
 # -*- coding: utf-8 -*-
 
 # Standard library import
-import numpy as np
+from numpy import asarray, delete, array, where
 
 # Local application imports
 from mosqito.sound_level_meter.noct_spectrum._center_freq import _center_freq
 from mosqito.sound_level_meter.noct_spectrum._filter_bandwidth import _filter_bandwidth
 from mosqito.sound_level_meter.noct_spectrum._n_oct_freq_filter import _n_oct_freq_filter
 
-
 def noct_synthesis(spectrum, freqs, fmin, fmax, n=3, G=10, fr=1000):
     """Adapt input spectrum to nth-octave band spectrum
-    
-    Convert the input spectrum to third-octave band spectrum
-    between "fc_min" and "fc_max".
+                
+    This function the input spectrum to n-th octave band levels.
+                       
     Parameters
     ----------
-    spectrum : numpy.ndarray
-        amplitude rms of the one-sided spectrum of the signal, size (nperseg, nseg).
+    spectrum : array_like
+        RMS amplitude one-sided spectrum, size (nperseg, nseg).
     freqs : list
         List of input frequency , size (nperseg) or (nperseg, nseg).
     fmin : float
-        Min frequency band [Hz].
+        Minimum frequency band [Hz].
     fmax : float
-        Max frequency band [Hz].
+        Maximum frequency band [Hz].
     n : int
-        Number of bands pr octave.
+        Number of bands per octave.
     G : int
         System for specifying the exact geometric mean frequencies.
         Can be base 2 or base 10.
     fr : int
         Reference frequency. Shall be set to 1 kHz for audible frequency
         range, to 1 Hz for infrasonic range (f < 20 Hz) and to 1 MHz for
         ultrasonic range (f > 31.5 kHz).
-    Outputs
+
+    Returns
     -------
     spec : numpy.ndarray
-        Third octave band spectrum of signal sig [dB re.2e-5 Pa], size (nbands, nseg).
+        nth-octave octave band spectrum of signal sig [dB re.2e-5 Pa], size (nbands, nseg).
     fpref : numpy.ndarray
-        Corresponding preferred third octave band center frequencies, size (nbands).
+        Corresponding preferred nth-octave octave band center frequencies, size (nbands).
+
+    See Also
+    --------
+    .comp_spectrum : Spectrum computation from a time signal
+    .noct_spectrum : N-th octave band spectrum computation from a time signal
+
+    Examples
+    --------
+    .. plot::
+       :include-source:
+
+        >>> from mosqito.sound_level_meter import comp_spectrum, noct_synthesis
+        >>> from mosqito.utils import amp2db
+        >>> import matplotlib.pyplot as plt
+        >>> import numpy as np
+        >>> f=1000
+        >>> fs=48000
+        >>> d=0.2
+        >>> dB=60
+        >>> time = np.arange(0, d, 1/fs)
+        >>> stimulus = np.sin(2 * np.pi * f * time) + 0.5 * np.sin(6 * np.pi * f * time)
+        >>> rms = np.sqrt(np.mean(np.power(stimulus, 2)))
+        >>> ampl = 0.00002 * np.power(10, dB / 20) / rms
+        >>> stimulus = stimulus * ampl
+        >>> spec, freqs = comp_spectrum(stimulus, fs, db=False)
+        >>> spec_3, freq_axis = noct_synthesis(spec, freqs, fmin=90, fmax=14000)
+        >>> spec_3db = amp2db(spec_3, ref=2e-5)
+        >>> plt.step(freq_axis, spec_3db)
+        >>> plt.xlabel("Center frequency [Hz]")
+        >>> plt.ylabel("Amplitude [dB]")
+
     """
-    
+
     # Deduce sampling frequency
-    fs = np.mean(freqs[1:] - freqs[:-1]) * 2 * len(spectrum)
+    fs = freqs.max() * 2
+
+    # Sampling frequency shall be equal to 48 kHz (as per ISO 532)
+    if round(fs) != 48000:
+        raise ValueError("""ERROR: Sampling frequency shall be equal to 48 kHz""")
 
     # Get filters center frequencies
     fc_vec, fpref = _center_freq(fmin=fmin, fmax=fmax, n=n, G=G, fr=fr)
-    
+
     # Compute the filters bandwidth
     alpha_vec, f_low, f_high = _filter_bandwidth(fc_vec, n=n)
-    
+
     # Delete ends frequencies to prevent aliasing
-    idx = np.asarray(np.where(f_high > fs / 2))
+    idx = asarray(where(f_high > fs / 2))
     if any(idx[0]):
-        fc_vec = np.delete(fc_vec, idx)
-        f_low = np.delete(f_low, idx)
-        f_high = np.delete(f_high, idx)
-
-    # Number of nth bands
-    nband = len(fc_vec)
-    
-    # Results array initialization
-    if len(spectrum.shape) > 1:
-        nseg = spectrum.shape[1]
-        spec = np.zeros((nband, nseg))
-        # If only one axis is given, it is used for all the spectra
-        if len(freqs.shape) == 1:
-            freqs = np.tile(freqs, (nseg, 1)).T
-    else:
-        nseg = 1
-        spec = np.zeros((nband))
+        fc_vec = delete(fc_vec, idx)
+        f_low = delete(f_low, idx)
+        f_high = delete(f_high, idx)
 
     # Calculation of the rms level of the signal in each band
     spec = []
     for fc, alpha in zip(fc_vec, alpha_vec):
         spec.append(_n_oct_freq_filter(spectrum, fs, fc, alpha))
 
-    return np.array(spec), fpref
+    return array(spec), fpref
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_auditory_filters_centre_freq.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_auditory_filters_centre_freq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from numpy import arange
-from numpy import sinh
+from numpy import arange, sinh
 
 
 def _auditory_filters_centre_freq():
     """
     Auditory filter bank center frequencies generation
 
     This function generates the Auditory filter bank center frequencies according
-    to ECMA-418-2 section 5.1.3.1 equation 6
+    to ECMA-418-2, 2nd Ed (2022), Section 5.1.4.1, equation 9
 
     Parameters
     ----------
 
     Returns
     -------
     centre_freq: ndarray
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_ear_filter_design.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_ear_filter_design.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # -*- coding: utf-8 -*-
 from numpy import column_stack
 
 
 def _ear_filter_design():
-    """Return second-order filter coefficients of outer and middle/inner ear filter according to
-    ECMA-418-2:2020 section 5.1.2.
+    """Return second-order filter coefficients of outer and middle/inner ear
+    filter according to ECMA-418-2, 2nd Ed. (2022), Section 5.1.3.
 
     Parameters
     ----------
 
     Returns
     -------
     sos : array_like
         Array of second-order filter coefficients. Each row corresponds to a
         second-order section, with the first three columns providing the numerator
         coefficients and the last three providing the denominator coefficients.
 
     """
 
-    # Filer coefficients (ECMA-418-2:2020, Table 1)
+    # Filer coefficients (ECMA-418-2, 2nd Ed (2022) Table 1)
     filter_a = [
-        [1.0, -1.9253, 0.9380],
-        [1.0, -1.8061, 0.8354],
-        [1.0, -1.7636, 0.7832],
-        [1.0, -1.4347, 0.7276],
-        [1.0, -0.3661, -0.2841],
-        [1.0, -1.7960, 0.8058],
-        [1.0, -1.9124, 0.9142],
-        [1.0, 0.1623, 0.2842],
+        [1.0, -1.925299, 0.938014],
+        [1.0, -1.806088, 0.835382],
+        [1.0, -1.763632, 0.783160],
+        [1.0, -1.434650, 0.727599],
+        [1.0, -0.366092, -0.284120],
+        [1.0, -1.796003, 0.805838],
+        [1.0, -1.912434, 0.914161],
+        [1.0, 0.162320, 0.284244],
     ]
+
     filter_b = [
-        [1.0159, -1.9253, 0.9221],
-        [0.9589, -1.8061, 0.8764],
-        [0.9614, -1.7636, 0.8218],
-        [2.2258, -1.4347, -0.4982],
-        [0.4717, -0.3661, 0.2441],
-        [0.1153, 0.0000, -0.1153],
-        [0.9880, -1.9124, 0.9261],
-        [1.9522, 0.1623, -0.6680],
+        [1.015896, -1.925299, 0.922118],
+        [0.958943, -1.806088, 0.876439],
+        [0.961372, -1.763632, 0.821788],
+        [2.225804, -1.434650, -0.498204],
+        [0.471735, -0.366092, 0.244145],
+        [0.115267, 0.000000, -0.115267],
+        [0.988029, -1.912434, 0.926132],
+        [1.952238, 0.162320, -0.667994],
     ]
+
     sos_ear = column_stack((filter_b, filter_a))
 
     return sos_ear
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_ecma_data.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_ecma_data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,8 @@
     0.0237,
     0.0263,
     0.0296,
     0.0339,
     0.0398,
     0.0485,
     0.0622,
-]
+]
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_nonlinearity.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_nonlinearity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,40 @@
-import numpy as np
+# Standard library import
+from numpy import array, ones
 
 
 def _nonlinearity(p):
     """Apply the compressive nonlinearity of the auditory system to the
-    rectified band pass signal rms values according to ECMA 418-2 section 5.1.7
+    rectified band pass signal rms values according to Equation (23) in
+    ECMA 418-2, 2nd Ed (2022), section 5.1.8.
 
     Parameters
     ----------
     p: numpy.array
         RMS value of the rectified band pass signal blocks
 
     Returns
     -------
     a_prime: numpy.array
         Specific Loudness [sone_HMS per Bark].
 
     """
     p_0 = 2e-5
-    # c_N: In sones/bark
-    c_N = 0.0217406
+
+    # c_N: In sone_HMS/bark
+    c_N = 0.0211668
+
     alpha = 1.50
-    v_i = np.array(
-        [1.0, 0.6602, 0.0864, 0.6384, 0.0328, 0.4068, 0.2082, 0.3994, 0.6434]
-    )
-    thresh = np.array([15.0, 25.0, 35.0, 45.0, 55.0, 65.0, 75.0, 85.0])
+
+    v_i = array([1.0, 0.6602, 0.0864, 0.6384, 0.0328, 0.4068, 0.2082, 0.3994, 0.6434])
+
+    thresh = array([0.0, 15.0, 25.0, 35.0, 45.0, 55.0, 65.0, 75.0, 85.0])
+
     p_ti = p_0 * 10 ** (thresh / 20)
 
-    a_prime = np.ones(p.shape)
-    for i in range(8):
-        a_prime *= (1 + (p / p_ti[i]) ** alpha) ** ((v_i[i + 1] - v_i[i]) / alpha)
+    a_prime = ones(p.shape)
+    for i in range(1, 9):
+        a_prime *= (1 + (p / p_ti[i]) ** alpha) ** ((v_i[i] - v_i[i - 1]) / alpha)
+
     a_prime *= c_N * p / p_0
 
-    return a_prime
+    return a_prime
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/_rectified_band_pass_signals.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_band_pass_signals.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,16 +9,78 @@
 from mosqito.sq_metrics.loudness.loudness_ecma._auditory_filters_centre_freq import (
     _auditory_filters_centre_freq,
 )
 from mosqito.sq_metrics.loudness.loudness_ecma._gammatone import _gammatone
 from mosqito.utils import time_segmentation
 
 
-def _rectified_band_pass_signals(sig, sb=2048, sh=1024):
-    """Compute the rectified band-pass signals as per Clause 5.1.2 to 5.1.5 of
+def _band_pass_signals(sig, sb, sh):
+    """Compute the band-pass signals as per Clause 5.1.2 to 5.1.5 of
+    ECMA-418-2:2020
+
+    Calculation of the rectified band-pass signals along the 53 critical band rates
+    scale. Each band pass signal is segmented into time blocks according to sb and sh
+
+    Parameters
+    ----------
+    signal: numpy.array
+        'Pa', time signal values. The sampling frequency of the signal must be 48000 Hz.
+    sb: int or list of int
+        block size.
+    sh: int or list of int
+        Hop size.
+    Returns
+    -------
+    block_array_rect: list of numpy.array
+        rectified band-pass signals
+    """
+
+    if isinstance(sb, int):
+        sb = sb * np.ones(53, dtype=int)
+    elif len(sb) != 53:
+        raise ValueError("ERROR: len(sb) shall be either 1 or 53")
+    if isinstance(sh, int):
+        sh = sh * np.ones(53, dtype=int)
+    elif len(sh) != 53:
+        raise ValueError("ERROR: len(sh) shall be either 1 or 53")
+
+    # OUTER AND MIDDLE EAR FILTERING (5.1.2)
+
+    sos_ear = _ear_filter_design()
+    signal_filtered = sp_signal.sosfilt(sos_ear, sig, axis=0)
+
+    # AUDITORY FILTERING BANK (5.1.3)
+
+    # Order of the Outer and Middle ear filter
+    filter_order_k = 5
+    # Sampling frequency
+    fs = 48000.00
+    # Auditory filters centre frequencies
+    centre_freq = _auditory_filters_centre_freq()
+
+    block_bandpass_signals = []
+    for band_number in range(53):
+        bm_mod, am_mod = _gammatone(centre_freq[band_number], k=filter_order_k, fs=fs)
+
+        band_pass_signal = (
+            2.0
+            * (
+                sp_signal.lfilter(
+                    bm_mod,
+                    am_mod,
+                    signal_filtered,
+                    axis=0,
+                )
+            ).real
+        )
+        block_bandpass_signals.append(band_pass_signal)
+    return block_bandpass_signals
+
+def _rectified_band_pass_signals(sig, sb, sh):
+    """Compute the band-pass signals as per Clause 5.1.2 to 5.1.5 of
     ECMA-418-2:2020
 
     Calculation of the rectified band-pass signals along the 53 critical band rates
     scale. Each band pass signal is segmented into time blocks according to sb and sh
 
     Parameters
     ----------
@@ -81,19 +143,19 @@
         # signal array "band_pass_signal_hr" into blocks. "sb_array" is the block size which changes depending on the
         # "band_number" in which we are processing the signal. "sh_array" is the step size, the time shift to the next
         # block.
 
         block_array, _ = time_segmentation(
             band_pass_signal, fs, sb[band_number], sh[band_number], is_ecma=True
         )
-        block_array = block_array.T
-
+    
+        
         # RECTIFICATION (5.1.5)
 
         # This part acts as the activation of the auditory nerves when the basilar membrane vibrates in a certain
         # direction. In order to rectify the signal we are using "np.clip" which establish a minimum and a maximum value
         # for the signal. "a_min" is set to 0 float, while "a_max" is set to "None" in order to consider the positive
         # value of the signal.
 
-        block_array_rect.append(np.clip(block_array, a_min=0.00, a_max=None))
+        block_array_rect.append(np.clip(block_array.T, a_min=0.00, a_max=None))
 
     return block_array_rect
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_ecma/loudness_ecma.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_from_bandpass.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,50 @@
 # -*- coding: utf-8 -*-
-"""
-@author: Daniel Jiménez-Caminero Costa
-"""
+from numpy import sqrt, mean, array, linspace
 import numpy as np
 
 # Project Imports
-from mosqito.sq_metrics.loudness.loudness_ecma._rectified_band_pass_signals import (
-    _rectified_band_pass_signals,
-)
 from mosqito.sq_metrics.loudness.loudness_ecma._nonlinearity import _nonlinearity
 
 # Data import
 # Threshold in quiet
 from mosqito.sq_metrics.loudness.loudness_ecma._loudness_ecma_data import ltq_z
 
 
-def loudness_ecma(signal, sb=2048, sh=1024):
+def _loudness_from_bandpass(block_array, rectify=True):
     """Calculation of the specific and total loudness according to ECMA-418-2 section 5
 
     Parameters
     ----------
-    signal: numpy.array
+    block_array: numpy.array
         time signal values in 'Pa'. The sampling frequency of the signal must be 48000 Hz.
-    sb: int or list of int
-        block size.
-    sh: int or list of int
-        Hop size.
+        time-segmented + gammatone filtered
 
     Returns
     -------
     n_specific: list of numpy.array
         Specific Loudness [sone_HMS per Bark]. Each of the 53 element of the list corresponds to the time-dependant
         specific loudness for a given bark band. Can be a ragged array if a different sb/sh are used for each band.
 
     bark_axis: numpy.array
         Bark axis
 
     """
-
-    # TODO: return time axis (list or list of list)
-
-    # Computaton of rectified band-pass signals
-    # (section 5.1.2 to 5.1.5 of the standard)
-    block_array_rect = _rectified_band_pass_signals(signal, sb, sh)
-
-    # # sb and sh for Tonality
-    # z = np.linspace(0.5, 26.5, num=53, endpoint=True)
-    # sb = np.ones(53, dtype="int")
-    # sh = np.ones(53, dtype="int")
-    # sb[z <= 1.5] = 8192
-    # sh[z <= 1.5] = 2048
-    # sb[np.all([z >= 2, z <= 8], axis=0)] = 4096
-    # sh[np.all([z >= 2, z <= 8], axis=0)] = 1024
-    # sb[np.all([z >= 8.5, z <= 12.5], axis=0)] = 2048
-    # sh[np.all([z >= 8.5, z <= 12.5], axis=0)] = 512
-    # sb[z >= 13] = 1024
-    # sh[z >= 13] = 256
-
+    # Rectification (5.1.6)
+    if rectify==True:
+        block_array_rect = np.clip(block_array, a_min=0.00, a_max=None)
+    else:
+        block_array_rect = block_array
     n_specific = []
     for band_number in range(53):
         # ROOT-MEAN-SQUARE (section 5.1.6)
         # After the segmentation of the signal into blocks, root-mean square values of each block are calculated
         # according to Formula 17.
-        rms_block_value = np.sqrt(
-            2 * np.mean(np.array(block_array_rect[band_number]) ** 2, axis=1)
+        rms_block_value = sqrt(
+            2 * mean(array(block_array_rect[band_number]) ** 2, axis=1)
         )
 
         # NON-LINEARITY (section 5.1.7)
         # This section covers the other part of the calculations needed to consider the non-linear transformation
         # of sound pressure to specific loudness that does the the auditory system. After this point, the
         # computation is done equally to every block in which we have divided our signal.
         a_prime = _nonlinearity(rms_block_value)
@@ -75,9 +52,10 @@
         # SPECIFIC LOUDNESS CONSIDERING THE THRESHOLD IN QUIET (section 5.1.8)
         # The next calculation helps us obtain the result for the specific loudness - specific loudness with
         # consideration of the lower threshold of hearing.
         a_prime[a_prime < ltq_z[band_number]] = ltq_z[band_number]
         N_prime = a_prime - ltq_z[band_number]
         n_specific.append(N_prime)
 
-    bark_axis = np.linspace(0.5, 26.5, num=53, endpoint=True)
+    bark_axis = linspace(0.5, 26.5, num=53, endpoint=True)
+    
     return n_specific, bark_axis
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/_calc_slopes.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_calc_slopes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
 # Standard library imports
-import numpy as np
+from numpy import array, append, tile, ones, copy, int32, zeros, arange, roll, logical_not, divide, maximum, minimum, multiply, logical_and, logical_xor, floor, round
 
 from mosqito.sq_metrics.loudness.loudness_zwst._get_rns_index import _get_rns_index
 
 
 def _calc_slopes(nm):
     """"""
     # Upper limits of approximated critical bands in terms of critical
     # band rate
-    zup = np.array(
+    zup = array(
         [
             0.9,
             1.8,
             2.8,
             3.5,
             4.4,
             5.4,
@@ -34,15 +34,15 @@
             23.6,
             24,
         ]
     )
     # Range of specific loudness for the determination of the steepness
     # of the upper slopes in the specific loudness - critical band rate
     # pattern
-    rns = np.array(
+    rns = array(
         [
             21.5,
             18,
             15.1,
             11.5,
             9,
             6.1,
@@ -59,15 +59,15 @@
             0.035,
             0,
         ]
     )
     # Steepness of the upper slopes in the specific loudness = Critical
     # band rate pattern for the ranges 'rns' as a function of the number
     # of the critical band
-    usl = np.array(
+    usl = array(
         [
             (13, 8.2, 6.3, 5.5, 5.5, 5.5, 5.5, 5.5),
             (9, 7.5, 6, 5.1, 4.5, 4.5, 4.5, 4.5),
             (7.8, 6.7, 5.6, 4.9, 4.4, 3.9, 3.9, 3.9),
             (6.2, 5.4, 4.6, 4.0, 3.5, 3.2, 3.2, 3.2),
             (4.5, 3.8, 3.6, 3.2, 2.9, 2.7, 2.7, 2.7),
             (3.7, 3.0, 2.8, 2.35, 2.2, 2.2, 2.2, 2.2),
@@ -84,104 +84,103 @@
             (0.09, 0.08, 0.07, 0.06, 0.06, 0.06, 0.06, 0.05),
             (0.06, 0.05, 0.03, 0.02, 0.02, 0.02, 0.02, 0.02),
         ]
     )
 
     # From Ernesto Avedillo 13/feb/2022
     # Considering the original routine if ig > 7:ig = 7 until ig = 21 so I can append the last column until usl.shape = (18,21)
-    usl_reshaped = np.append(usl, np.tile(
-        usl[:, 7], 13).reshape(13, 18).T, axis=1)
+    usl_reshaped = append(usl, tile(usl[:, 7], 13).reshape(13, 18).T, axis=1)
 
     # For test, in case nm has only 1 col.
     len_1_nm = False
     if len(nm.shape) == 1:
         len_1_nm = True
-        nm = np.append(nm, nm).reshape(2, 21).T
+        nm = append(nm, nm).reshape(2, 21).T
 
     # Start values
     data_length = nm.shape[1]
     nm_wide = nm.shape[0]
     spec_length = 240
     dec_compare = 8
     # Working array variables
-    n2_array_specific = np.ones((spec_length, data_length))
-    z2_array_specific = np.ones((spec_length, data_length))
-    usl_array_specific = np.ones((spec_length, data_length))
-    dz_array_specific = np.ones((spec_length, data_length))
-    rns_values_specific = np.ones((spec_length, data_length))
+    n2_array_specific = ones((spec_length, data_length))
+    z2_array_specific = ones((spec_length, data_length))
+    usl_array_specific = ones((spec_length, data_length))
+    dz_array_specific = ones((spec_length, data_length))
+    rns_values_specific = ones((spec_length, data_length))
     # Create a zup vector called zup_ea to define the position in the N_spezific array.
-    zup_ea = (np.copy(zup) * 10).astype(np.int32)
-    zup_ea = np.append(zup_ea, 0)
+    zup_ea = (copy(zup) * 10).astype(int32)
+    zup_ea = append(zup_ea, 0)
 
     # Create a complete array of ZUP vectors with shape nm elements in a row
-    zup_array_ea = (np.ones((nm_wide, data_length)).T * zup).T
+    zup_array_ea = (ones((nm_wide, data_length)).T * zup).T
     # crearte an array of z values 0.1 increase
 
     # Prepare the array N_specific for output
     # For all cases where nm[:,col-1] < nm[:,col]
-    N_specific = np.zeros((spec_length, data_length))
+    N_specific = zeros((spec_length, data_length))
     # I save the first values for first raws defined in zup_ea
     # N_specific[:zup_ea[0],:] = np.multiply(N_specific[:zup_ea[0],:] , nm[1])
     # I complete the rest of the matrix extending the array 21  to 240
-    for i in np.arange(nm_wide - 1):
-        N_specific[zup_ea[i - 1]: zup_ea[i], :] = nm[i]
+    for i in arange(nm_wide - 1):
+        N_specific[zup_ea[i - 1] : zup_ea[i], :] = nm[i]
 
-    N = np.zeros(data_length)
+    N = zeros(data_length)
 
     # nm_aux = np.copy(nm)
     # nm_aux [0] = nm[1]
 
     # obtain the rns indexes for each value of the nm matrix.
     # rns_ind = _get_rns_index (nm, rns ,equal_too = True )
     rns_ind = _get_rns_index(nm, rns)
     # save in an array the values corresponding to this index
     rns_values = rns[rns_ind]
 
     # search usl_array for each nm cell
-    usl_array_ind = np.array(
-        [rns_ind.T, np.ones((zup.shape[0], data_length)).T * np.arange(21)], dtype=int
+    usl_array_ind = array(
+        [rns_ind.T, ones((zup.shape[0], data_length)).T * arange(21)], dtype=int
     ).transpose(1, 2, 0)
     usl_array = usl_reshaped[usl_array_ind[:, :, 0], usl_array_ind[:, :, 1]].T
     # create a 240 x nm shape[1] array to save the dz values equal to z2-z1
-    dz = np.zeros((nm_wide, data_length))
-    dz = zup_array_ea - np.roll(zup_array_ea, 1, axis=0)
+    dz = zeros((nm_wide, data_length))
+    dz = zup_array_ea - roll(zup_array_ea, 1, axis=0)
 
     dz[0, :] = zup[1]
     dz[1, :] = zup[1]
 
-    for i in np.arange(nm_wide):
-        n2_array_specific[zup_ea[i - 1]: zup_ea[i], :] = nm[i]
-        dz_array_specific[zup_ea[i - 1]: zup_ea[i], :] = dz[i]
-        z2_array_specific[zup_ea[i - 1]: zup_ea[i], :] = zup_array_ea[i]
-        usl_array_specific[zup_ea[i - 1]: zup_ea[i], :] = usl_array[i]
-        rns_values_specific[zup_ea[i - 1]: zup_ea[i], :] = rns_values[i]
+    for i in arange(nm_wide):
+        n2_array_specific[zup_ea[i - 1] : zup_ea[i], :] = nm[i]
+        dz_array_specific[zup_ea[i - 1] : zup_ea[i], :] = dz[i]
+        z2_array_specific[zup_ea[i - 1] : zup_ea[i], :] = zup_array_ea[i]
+        usl_array_specific[zup_ea[i - 1] : zup_ea[i], :] = usl_array[i]
+        rns_values_specific[zup_ea[i - 1] : zup_ea[i], :] = rns_values[i]
 
     j = 1
-    n1_aux = np.zeros(data_length)
-    z1_aux = np.zeros(data_length)
+    n1_aux = zeros(data_length)
+    z1_aux = zeros(data_length)
 
-    for i in np.arange(nm_wide):
+    for i in arange(nm_wide):
         # for all cases where nm[i-1]>nm[i]
         j = zup_ea[i - 1]
         indexes = _get_rns_index(n2_array_specific[j - 1], rns)
         rns_values_specific[j] = rns[indexes]
         usl_array_specific[j] = usl_reshaped[indexes, i - 1]
 
-        mask_n1_bigger_nm = np.round(n2_array_specific[j - 1], dec_compare) > np.round(
+        mask_n1_bigger_nm = round(n2_array_specific[j - 1], dec_compare) > round(
             nm[i], dec_compare
         )
         # For all n1 <= nm[i] calculate (N = N + n2 * (z2 - z1))
-        N[np.logical_not(mask_n1_bigger_nm)] += (
+        N[logical_not(mask_n1_bigger_nm)] += (
             n2_array_specific[j] * (z2_array_specific[j] - z1_aux)
-        )[np.logical_not(mask_n1_bigger_nm)]
-        n1_aux[np.logical_not(mask_n1_bigger_nm)] = np.copy(n2_array_specific[j])[
-            np.logical_not(mask_n1_bigger_nm)
+        )[logical_not(mask_n1_bigger_nm)]
+        n1_aux[logical_not(mask_n1_bigger_nm)] = copy(n2_array_specific[j])[
+            logical_not(mask_n1_bigger_nm)
         ]
-        z1_aux[np.logical_not(mask_n1_bigger_nm)] = np.copy(z2_array_specific[j])[
-            np.logical_not(mask_n1_bigger_nm)
+        z1_aux[logical_not(mask_n1_bigger_nm)] = copy(z2_array_specific[j])[
+            logical_not(mask_n1_bigger_nm)
         ]
 
         if mask_n1_bigger_nm.sum() > 0:
             # For all n1 > nm[i] calculate z2,dz n2.
             # This routine
             # n2 = rns[j]
             # if n2 < nm[i]:
@@ -194,38 +193,38 @@
             #     n2 = n1 - dz * usl[j, ig]
             # Can be subtituted by
             # max_rns_nm = max(rns[j],nm[i])
             # z2_ea = min((n1-max_rns_nm)/usl[j,ig]+z1,zup[i])
             # dz_ea = z2_ea - z1
             # n2_ea = n1 - dz_ea * usl[j,ig]
 
-            Max_rns_nm_Array = np.maximum(rns_values_specific[j - 1], nm[i])
-            z2_array_specific[j, mask_n1_bigger_nm] = np.minimum(
-                np.divide(n1_aux - Max_rns_nm_Array,
+            Max_rns_nm_Array = maximum(rns_values_specific[j - 1], nm[i])
+            z2_array_specific[j, mask_n1_bigger_nm] = minimum(
+                divide(n1_aux - Max_rns_nm_Array,
                           usl_array_specific[j]) + z1_aux,
                 zup[i],
             )[mask_n1_bigger_nm]
             dz_array_specific[j, mask_n1_bigger_nm] = (z2_array_specific[j] - z1_aux)[
                 mask_n1_bigger_nm
             ]
             n2_array_specific[j, mask_n1_bigger_nm] = (
                 n1_aux -
-                np.multiply(dz_array_specific[j], usl_array_specific[j])
+                multiply(dz_array_specific[j], usl_array_specific[j])
             )[mask_n1_bigger_nm]
 
             # Calculate N for all n1 > nm[i]
 
             N[mask_n1_bigger_nm] += (
                 dz_array_specific[j] * (n1_aux + n2_array_specific[j]) / 2
             )[mask_n1_bigger_nm]
 
             # get value of z
-            z_array = np.ones(data_length) * zup[i - 1] + 0.1
+            z_array = ones(data_length) * zup[i - 1] + 0.1
 
-            for j in np.arange(zup_ea[i - 1], zup_ea[i]):
+            for j in arange(zup_ea[i - 1], zup_ea[i]):
 
                 # Save values from previous calculation (only after second loop)
                 if j != zup_ea[i - 1]:
                     z2_array_specific[j, mask_n1_bigger_nm] = z2_array_specific[
                         j - 1, mask_n1_bigger_nm
                     ]
                     n2_array_specific[j, mask_n1_bigger_nm] = n2_array_specific[
@@ -238,18 +237,18 @@
                         j - 1, mask_n1_bigger_nm
                     ]
                     rns_values_specific[j, mask_n1_bigger_nm] = rns_values_specific[
                         j - 1, mask_n1_bigger_nm
                     ]
 
                 # Sometimes a second loop is necesary if z > z2
-                mask_z_bigger_z2 = np.logical_and(
+                mask_z_bigger_z2 = logical_and(
                     mask_n1_bigger_nm,
-                    np.round(z2_array_specific[j], dec_compare)
-                    <= np.round(z_array, dec_compare),
+                    round(z2_array_specific[j], dec_compare)
+                    <= round(z_array, dec_compare),
                 )
                 if mask_z_bigger_z2.sum() > 0:
                     indexes = _get_rns_index(
                         n2_array_specific[j,
                                           mask_z_bigger_z2], rns, equal_too=True
                     )
                     rns_values_specific[j, mask_z_bigger_z2] = rns[indexes]
@@ -261,98 +260,98 @@
                                                                  mask_z_bigger_z2]
                     z1_aux[mask_z_bigger_z2] = z2_array_specific[j,
                                                                  mask_z_bigger_z2]
 
                     # Vuelvo al inicio del loop y reviso de nuevo que n2 sea menor que nm
                     # Vuelvo a calcular mask_n1_bigger_nm
                     # Para los valores de n1_aux<=nm[i]
-                    mask_z_bigger_z2_1 = np.logical_and(
+                    mask_z_bigger_z2_1 = logical_and(
                         mask_z_bigger_z2,
-                        np.round(n1_aux, dec_compare) <= np.round(
+                        round(n1_aux, dec_compare) <= round(
                             nm[i], dec_compare),
                     )
                     n2_array_specific[j, mask_z_bigger_z2_1] = nm[i,
                                                                   mask_z_bigger_z2_1]
                     z2_array_specific[j, mask_z_bigger_z2_1] = zup[i]
                     dz_array_specific[j, mask_z_bigger_z2_1] = (
                         z2_array_specific[j] - z1_aux
                     )[mask_z_bigger_z2_1]
                     # Recalculate N
                     N[mask_z_bigger_z2_1] += (
                         n2_array_specific[j] * (z2_array_specific[j] - z1_aux)
                     )[mask_z_bigger_z2_1]
 
                     # For Values n1_aux>nm[i] after second loop
-                    mask_z_bigger_z2_2 = np.logical_and(
+                    mask_z_bigger_z2_2 = logical_and(
                         mask_z_bigger_z2,
-                        np.round(n1_aux, dec_compare) > np.round(
+                        round(n1_aux, dec_compare) > round(
                             nm[i], dec_compare),
                     )
-                    Max_rns_nm_Array = np.maximum(
+                    Max_rns_nm_Array = maximum(
                         rns_values_specific[j], nm[i])
-                    z2_array_specific[j, mask_z_bigger_z2_2] = np.minimum(
-                        np.divide(n1_aux - Max_rns_nm_Array,
+                    z2_array_specific[j, mask_z_bigger_z2_2] = minimum(
+                        divide(n1_aux - Max_rns_nm_Array,
                                   usl_array_specific[j])
                         + z1_aux,
                         zup[i],
                     )[mask_z_bigger_z2_2]
                     dz_array_specific[j, mask_z_bigger_z2_2] = (
                         z2_array_specific[j] - z1_aux
                     )[mask_z_bigger_z2_2]
                     n2_array_specific[j, mask_z_bigger_z2_2] = (
                         n1_aux
-                        - np.multiply(dz_array_specific[j], usl_array_specific[j])
+                        - multiply(dz_array_specific[j], usl_array_specific[j])
                     )[mask_z_bigger_z2_2]
                     # Recalculate N
                     N[mask_z_bigger_z2_2] += (
                         dz_array_specific[j] *
                         (n1_aux + n2_array_specific[j]) / 2
                     )[mask_z_bigger_z2_2]
                     N_specific[j, mask_z_bigger_z2_2] = (
-                        n1_aux - np.multiply((z_array - z1_aux),
+                        n1_aux - multiply((z_array - z1_aux),
                                              usl_array_specific[j])
                     )[mask_z_bigger_z2_2]
 
                     # For the rest of the values  Where z < z2 calculate N_Specific
-                    mask_z_rest = np.logical_xor(
+                    mask_z_rest = logical_xor(
                         mask_z_bigger_z2, mask_n1_bigger_nm)
                     N_specific[j, mask_z_rest] = (
-                        n1_aux - np.multiply((z_array - z1_aux),
+                        n1_aux - multiply((z_array - z1_aux),
                                              usl_array_specific[j])
                     )[mask_z_rest]
                     z_array += 0.1
 
                     # Generate a new mask for n1 > nm[i]
-                    mask_n1_bigger_nm = np.logical_xor(
+                    mask_n1_bigger_nm = logical_xor(
                         mask_n1_bigger_nm, mask_z_bigger_z2_1
                     )
 
                 else:
                     N_specific[j, mask_n1_bigger_nm] = (
-                        n1_aux - np.multiply((z_array - z1_aux),
+                        n1_aux - multiply((z_array - z1_aux),
                                              usl_array_specific[j])
                     )[mask_n1_bigger_nm]
                     z_array += 0.1
 
-                z1_aux = np.copy(z2_array_specific[j])
-                n1_aux = np.copy(n2_array_specific[j])
+                z1_aux = copy(z2_array_specific[j])
+                n1_aux = copy(n2_array_specific[j])
 
                 if mask_n1_bigger_nm.sum() == 0:
                     break
-            z1_aux = np.copy(z2_array_specific[zup_ea[i] - 1])
-            n1_aux = np.copy(n2_array_specific[zup_ea[i] - 1])
+            z1_aux = copy(z2_array_specific[zup_ea[i] - 1])
+            n1_aux = copy(n2_array_specific[zup_ea[i] - 1])
 
             indexes = _get_rns_index(
                 n2_array_specific[j, mask_z_bigger_z2], rns, equal_too=True
             )
             rns_values_specific[j, mask_z_bigger_z2] = rns[indexes]
             usl_array_specific[j,
                                mask_z_bigger_z2] = usl_reshaped[indexes, i - 1]
 
     N[N < 0] = 0
-    N[N <= 16] = np.floor(N[N <= 16] * 1000 + 0.5) / 1000
-    N[N > 16] = np.floor(N[N > 16] * 100 + 0.5) / 100
+    N[N <= 16] = floor(N[N <= 16] * 1000 + 0.5) / 1000
+    N[N > 16] = floor(N[N > 16] * 100 + 0.5) / 100
     if len_1_nm:
         N = N[0]
         N_specific = N_specific[:, 0]
 
     return N, N_specific
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/_get_rns_index.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_get_rns_index.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import numpy as np
-
+# Standard library import
+from numpy import round, tile, ones
 
 def _get_rns_index(array_nm, vector_rns, equal_too=False):
     """Function that returns the index in the array vector_rns for each value of srray _nm
 
     Parameters
     ----------
     array_nm : numpy.ndarray, values of the matrix toget the indexes
@@ -16,21 +16,21 @@
     indexes :  numpy.ndarray
         Array of indexes
     """
 
     if len(array_nm.shape) == 1:
         (wide,) = array_nm.shape
         (deep,) = vector_rns.shape
-        array_aux = np.round(np.tile(array_nm, [deep, 1]), 8)
-        rns_array = np.round(np.ones([wide, deep]) * vector_rns, 8).T
+        array_aux = round(tile(array_nm, [deep, 1]), 8)
+        rns_array = round(ones([wide, deep]) * vector_rns, 8).T
     else:
         wide, length = array_nm.shape
         (deep,) = vector_rns.shape
-        array_aux = np.round(np.tile(array_nm, [deep, 1, 1]), 8)
-        rns_array = np.round((np.ones([wide, length, deep]) * vector_rns), 8).transpose(
+        array_aux = round(tile(array_nm, [deep, 1, 1]), 8)
+        rns_array = round((ones([wide, length, deep]) * vector_rns), 8).transpose(
             2, 0, 1
         )
         # indexes = (array_aux < rns_array).sum(axis=0)
         # indexes[indexes==18] = 17
     if equal_too:
         indexes = (array_aux <= rns_array).sum(axis=0)
     else:
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/_main_loudness.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_main_loudness.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # -*- coding: utf-8 -*-
-"""
-@date Created on Thur Apr 30 2020
-@author martin_g for Eomys
-"""
 
 # Standard library imports
-import numpy as np
+from numpy import max, array, newaxis, arange, multiply, ones, logical_xor, power, zeros, log10, copy, append, squeeze
 
 
 def _main_loudness(spec_third, field_type):
     """Calculate core loudness
 
     The code is based on BASIC program published in "Program for
-    calculating loudness according to DIN 45631 (ISO 532B)", E.Zwicker
+    calculating loudness according to DIN 45631 (ISO 532-1:2017)", E.Zwicker
     and H.Fastl, J.A.S.J (E) 12, 1 (1991).
     It also corresponds to the following functions of the C program
     published with ISO 532-1:2017:
     - corr_third_octave_intensities
     - f_calc_lcbs
     - f_calc_core_loudness
     - f_corr_loudness
@@ -35,49 +31,49 @@
         Core loudness
     """
     # Ref. ISO 532-1:2017 paragraph A.3
     # The table A.3 giving the weights of the 1/3 band levels for
     # center freq. below 300 Hz is only specified for levels up to 120 dB
     # If one of the first 11 bands (from 25 to 250 Hz) exceed 120 dB the
     # Zwicker method cannot be applied.
-    if np.max(spec_third[0:11]) > 120.0:
+    if max(spec_third[0:11]) > 120.0:
         raise ValueError(
             "1/3 octave band value exceed 120 dB, for which "
             + "the Zwicker method is no longer valid."
         )
     #
     # Date tables definition (variable names and description according to
     # Zwicker:1991)
     # Ranges of 1/3 octave band levels for correction at low frequencies
     # according to equal loudness contours
-    rap = np.array([45, 55, 65, 71, 80, 90, 100, 120])
+    rap = array([45, 55, 65, 71, 80, 90, 100, 120])
     # Reduction of 1/3 octave band levels at low frequencies according to
     # equal loudness contours within the eight ranges defined by RAP
-    dll = np.array(
+    dll = array(
         [
             (-32, -24, -16, -10, -5, 0, -7, -3, 0, -2, 0),
             (-29, -22, -15, -10, -4, 0, -7, -2, 0, -2, 0),
             (-27, -19, -14, -9, -4, 0, -6, -2, 0, -2, 0),
             (-25, -17, -12, -9, -3, 0, -5, -2, 0, -2, 0),
             (-23, -16, -11, -7, -3, 0, -4, -1, 0, -1, 0),
             (-20, -14, -10, -6, -3, 0, -4, -1, 0, -1, 0),
             (-18, -12, -9, -6, -2, 0, -3, -1, 0, -1, 0),
             (-15, -10, -8, -4, -2, 0, -3, -1, 0, -1, 0),
         ]
     )
     # Critical band level at absolute threshold without taking into
     # account the transmission characteristics of the ear
-    ltq = np.array([30, 18, 12, 8, 7, 6, 5, 4, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3])
+    ltq = array([30, 18, 12, 8, 7, 6, 5, 4, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3])
     # Correction of levels according to the transmission characteristics
     # of the ear
-    a0 = np.array(
+    a0 = array(
         [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, -0.5, -1.6, -3.2, -5.4, -5.6, -4, -1.5, 2, 5, 12]
     )
     # Level difference between free and diffuse sound fields
-    ddf = np.array(
+    ddf = array(
         [
             0,
             0,
             0.5,
             0.9,
             1.2,
             1.6,
@@ -95,15 +91,15 @@
             4,
             4.3,
             4,
         ]
     )
     # Adaptation of 1/3 oct. band levels to the corresponding critical
     # band level
-    dcb = np.array(
+    dcb = array(
         [
             -0.25,
             -0.6,
             -0.8,
             -0.8,
             -0.5,
             0,
@@ -126,111 +122,111 @@
     #
     # Correction of 1/3 oct. band levels according to equal loudness
     # contours 'xp' and calculation of the intensities for 1/3 oct.
     # bands up to 315 Hz
 
     # 1-dimensional array to 2-dimensional array with size (nfreq, 1)
     if spec_third.ndim == 1:
-        spec_third = spec_third[:, np.newaxis]
+        spec_third = spec_third[:, newaxis]
 
     spec_third_aux = spec_third[: dll.shape[1], :]
     # spec_third_aux[:, -1] = 0
 
     # Convert rap, dll in 3 dimensional array
     # 1. generate the array shape
-    base_mat = np.ones((dll.shape[0], dll.shape[1], spec_third_aux.shape[1]))
+    base_mat = ones((dll.shape[0], dll.shape[1], spec_third_aux.shape[1]))
     # 2. start saving data in rap and DLL array
-    rap_mat = np.array(
-        [base_mat[:, i, :].T * rap for i in np.arange(dll.shape[1])]
+    rap_mat = array(
+        [base_mat[:, i, :].T * rap for i in arange(dll.shape[1])]
     ).transpose(2, 0, 1)
-    dll_mat = np.array(
-        [np.multiply(base_mat[:, :, i], dll) for i in np.arange(spec_third.shape[1])]
+    dll_mat = array(
+        [multiply(base_mat[:, :, i], dll) for i in arange(spec_third.shape[1])]
     ).transpose(1, 2, 0)
-    spec_third_aux_mat = np.array(
+    spec_third_aux_mat = array(
         [
-            np.multiply(base_mat[i, :, :], spec_third_aux)
-            for i in np.arange(dll.shape[0])
+            multiply(base_mat[i, :, :], spec_third_aux)
+            for i in arange(dll.shape[0])
         ]
     )
     # create the the array rap-dll
     rap_dll_mat = rap_mat - dll_mat
 
     # This part substitutes the while loop.
     # create the mask to operate
     logic_mat = spec_third_aux_mat > rap_dll_mat
     dll_result = dll_mat[0, :, :]
     dll_result[logic_mat[0, :, :]] = 0
-    for i in np.arange(1, dll_mat.shape[0] - 1):
-        mask = np.logical_xor(logic_mat[i - 1, :, :], logic_mat[i, :, :])
+    for i in arange(1, dll_mat.shape[0] - 1):
+        mask = logical_xor(logic_mat[i - 1, :, :], logic_mat[i, :, :])
         dll_result[mask] = dll_mat[i, mask]
 
     xp = dll_result + spec_third_aux
-    ti = np.power(10, (xp / 10))
+    ti = power(10, (xp / 10))
 
     # Determination of levels LCB(1), LCB(2) and LCB(3) within the
     # first three critical bands
 
-    gi = np.zeros([3, dll_result.shape[1]])
+    gi = zeros([3, dll_result.shape[1]])
     gi[0, :] = ti[0:6, :].sum(axis=0)
     gi[1, :] = ti[6:9, :].sum(axis=0)
     gi[2, :] = ti[9:11, :].sum(axis=0)
 
     logic_gi = gi > 0
-    lcb = np.zeros([3, dll_result.shape[1]])
-    lcb[logic_gi] = 10 * np.log10(gi[logic_gi])
+    lcb = zeros([3, dll_result.shape[1]])
+    lcb[logic_gi] = 10 * log10(gi[logic_gi])
 
     # Calculation of main loudness
     s = 0.25
-    nm = np.zeros([20, spec_third_aux.shape[1]])
-    le = np.copy(spec_third[8:, :])
+    nm = zeros([20, spec_third_aux.shape[1]])
+    le = copy(spec_third[8:, :])
     # le = le.reshape((20))
     le[0:3, :] = lcb
-    a0_mat = np.ones(a0.shape[0] * spec_third.shape[1]).reshape(
+    a0_mat = ones(a0.shape[0] * spec_third.shape[1]).reshape(
         a0.shape[0], spec_third.shape[1]
     )
     a0_mat = (a0_mat.T * a0).T
     le = le - a0_mat
 
     if field_type == "diffuse":
-        ddf_mat = np.ones(ddf.shape[0] * spec_third.shape[1]).reshape(
+        ddf_mat = ones(ddf.shape[0] * spec_third.shape[1]).reshape(
             ddf.shape[0], spec_third.shape[1]
         )
         ddf_mat = (ddf_mat.T * ddf).T
         le += ddf_mat
 
-    ltq_mat = np.ones(ltq.shape[0] * spec_third.shape[1]).reshape(
+    ltq_mat = ones(ltq.shape[0] * spec_third.shape[1]).reshape(
         ltq.shape[0], spec_third.shape[1]
     )
     ltq_mat = (ltq_mat.T * ltq).T
     i = le > ltq_mat
-    dcb_mat = np.ones(dcb.shape[0] * spec_third.shape[1]).reshape(
+    dcb_mat = ones(dcb.shape[0] * spec_third.shape[1]).reshape(
         dcb.shape[0], spec_third.shape[1]
     )
     dcb_mat = (dcb_mat.T * dcb).T
     le[i] -= dcb_mat[i]
 
-    mp1 = 0.0635 * np.power(10, 0.025 * ltq_mat)
+    mp1 = 0.0635 * power(10, 0.025 * ltq_mat)
     mp1[i == False] = 0
-    mp2 = np.power(1 - s + s * np.power(10, 0.1 * (le - ltq_mat)), 0.25) - 1
+    mp2 = power(1 - s + s * power(10, 0.1 * (le - ltq_mat)), 0.25) - 1
     mp2[i == False] = 0
 
-    nm = np.multiply(mp1, mp2)
+    nm = multiply(mp1, mp2)
 
     nm[i == False] = 0
     nm[nm < 0] = 0
     current_shape = nm.shape
-    nm = np.append(nm, np.zeros(current_shape[1])).reshape(
+    nm = append(nm, zeros(current_shape[1])).reshape(
         current_shape[0] + 1, current_shape[1]
     )
     #
     # Correction of specific loudness in the lowest critical band
     # taking into account the dependance of absolute threshold
     # within this critical band
     korry = 0.4 + 0.32 * nm[0] ** 0.2
     nm[0, korry <= 1] *= korry[korry <= 1]
     # nm[:, -1] = 0
     # if spec_third.ndim == 1 or spec_third.shape[1] == 1:
     #     # This is only for test_loudness_zwicker_3oct because only one array of one col is given and this routine needs 2 or more
     #     # This line is only also for testing test_loudness_zwicker_wav(), only in case one col in spec third is given.
     #     nm = nm[:, 1]
 
-    return np.squeeze(nm)
+    return squeeze(nm)
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,62 +3,108 @@
 # Third party imports
 import numpy as np
 
 # Local application imports
 from mosqito.sound_level_meter import noct_spectrum
 from mosqito.sq_metrics.loudness.loudness_zwst._main_loudness import _main_loudness
 from mosqito.sq_metrics.loudness.loudness_zwst._calc_slopes import _calc_slopes
-from mosqito.utils.conversion import amp2db
+from mosqito.utils import amp2db
 
 
 def loudness_zwst(signal, fs, field_type="free"):
-    """Zwicker-loudness calculation for stationary signals
+    """
+    Compute the loudness value from a time signal
 
-    Calculates the acoustic loudness according to Zwicker method for
-    stationary signals.
-    Normatice reference:
-        ISO 532:1975 (method B)
-        DIN 45631:1991
-        ISO 532-1:2017 (method 1)
-    The code is based on BASIC program published in "Program for
-    calculating loudness according to DIN 45631 (ISO 532B)", E.Zwicker
-    and H.Fastl, J.A.S.J (E) 12, 1 (1991).
-    Note that due to normative continuity, as defined in the
-    preceeding standards, the method is in accordance with
-    ISO 226:1987 equal loudness contours (instead of ISO 226:2003)
+    This function computes the acoustic loudness according to Zwicker method for
+    stationary signals (ISO.532-1:2017).
 
     Parameters
     ----------
     signal : numpy.array
-        Signal time values [Pa]
+        Signal time values [Pa], dim (nperseg, nseg).
     fs : float
         Sampling frequency [Hz]
     field_type : str
         Type of soundfield corresponding to spec_third ("free" by
         default or "diffuse").
 
-    Outputs
+    Returns
+    -------
+    N : float or array_like
+        Overall loudness array in [sones], size (Ntime,).
+    N_specific : array_like
+        Specific loudness array [sones/bark], size (Nbark, Ntime).
+    bark_axis: array_like
+        Bark axis array, size (Nbark,).
+
+    Warning
     -------
-    N : float or numpy.array
-        The overall loudness array [sones], size (Ntime,).
-    N_specific : numpy.ndarray
-        The specific loudness array [sones/bark], size (Nbark, Ntime).
-    bark_axis: numpy.array
-        The Bark axis array, size (Nbark,).
+    The sampling frequency of the signal must be >= 48 kHz to fulfill requirements.
+    If the provided signal doesn't meet the requirements, it will be resampled.
+
+    See Also
+    --------
+    .loudness_zwst_perseg : Loudness computation by time-segment
+    .loudness_zwst_freq : Loudness computation from a sound spectrum
+    .loudness_zwtv : Loudness computation for a non-stationary time signal
+
+    Notes
+    -----
+    The total loudness :math:`N` of the signal is computed as the integral of the specific loudness :math:`N'` measured in sone/bark, over the Bark scale.
+    The values of specific loudness are evaluated from third octave band levels as function of critical band rate :math:`z` in Bark.
+
+    .. math::
+        N=\\int_{0}^{24Bark}N'(z)\\textup{dz}
+
+    Due to normative continuity, the method is in accordance with ISO 226:1987 equal loudness contours
+    instead of ISO 226:2003, as defined in the following standards:
+        * ISO 532:1975 (method B)
+        * DIN 45631:1991
+        * ISO 532-1:2017 (method 1)
+
+    References
+    ----------
+    :cite:empty:`L_zw-ZF91`
+    :cite:empty:`L_zw-ISO.532-1:2017`
+    
+    .. bibliography::
+        :keyprefix: L_zw-
+
+    Examples
+    --------
+    .. plot::
+       :include-source:
+
+       >>> from mosqito.sq_metrics import loudness_zwst
+       >>> import matplotlib.pyplot as plt
+       >>> import numpy as np
+       >>> f=1000
+       >>> fs=48000
+       >>> d=0.2
+       >>> dB=60
+       >>> time = np.arange(0, d, 1/fs)
+       >>> stimulus = 0.5 * (1 + np.sin(2 * np.pi * f * time))
+       >>> rms = np.sqrt(np.mean(np.power(stimulus, 2)))
+       >>> ampl = 0.00002 * np.power(10, dB / 20) / rms
+       >>> stimulus = stimulus * ampl
+       >>> N, N_spec, bark_axis = loudness_zwst(stimulus, fs)
+       >>> plt.plot(bark_axis, N_spec)
+       >>> plt.xlabel("Frequency band [Bark]")
+       >>> plt.ylabel("Specific loudness [Sone/Bark]")
+       >>> plt.title("Loudness = " + f"{N:.2f}" + " [Sone]")
     """
 
     if fs < 48000:
         print(
             "[Warning] Signal resampled to 48 kHz to allow calculation. To fulfill the standard requirements fs should be >=48 kHz."
         )
         from scipy.signal import resample
 
         signal = resample(signal, int(48000 * len(signal) / fs))
         fs = 48000
-
     # Compute third octave band spectrum
     spec_third, _ = noct_spectrum(signal, fs, fmin=24, fmax=12600)
 
     # Compute dB values
     spec_third = amp2db(spec_third, ref=2e-5)
 
     # Compute main loudness
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/_lowpass_intp.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_lowpass_intp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # -*- coding: utf-8 -*-
-"""
-@date Created on Fri May 22 2020
-@author martin_g for Eomys
-"""
 
 # Standard library imports
 import math
-import numpy as np
-#Needed for the loudness_zwicker_lowpass_intp_ea function
+from numpy import copy, roll, zeros, shape, arange
+
+# Needed for the loudness_zwicker_lowpass_intp_ea function
 from scipy import signal
 
 
 def _lowpass_intp(loudness, tau, sample_rate):
     """1st order low-pass with linear interpolation of signal for
     increased precision
 
@@ -25,37 +22,37 @@
         Louness signal sampling frequency
 
     Outputs
     -------
     filt_loudness : numpy.ndarray
         Filtered loudness
     """
-    filt_loudness = np.zeros(np.shape(loudness))
+    filt_loudness = zeros(shape(loudness))
     # Factor for virtual upsampling/inner iterations
     lp_iter = 24
 
-    num_samples = np.shape(loudness)[0]
+    num_samples = shape(loudness)[0]
     a1 = math.exp(-1 / (sample_rate * lp_iter * tau))
     b0 = 1 - a1
     y1 = 0
 
-    delta = np.copy(loudness)
-    delta = np.roll(delta,-1)
+    delta = copy(loudness)
+    delta = roll(delta,-1)
     delta [-1] = 0
     delta = (delta - loudness) /  lp_iter
-    ui_delta = np.zeros(loudness.shape[0]*lp_iter).reshape(loudness.shape[0],lp_iter)
+    ui_delta = zeros(loudness.shape[0]*lp_iter).reshape(loudness.shape[0],lp_iter)
     ui_delta [:,0] = loudness  
     
-    #Create the array complete of deltas to apply the filter.
-    for i_in in np.arange(1, lp_iter):
-        ui_delta [:,i_in] = delta + ui_delta [:,i_in-1]  
-    
+    # Create the array complete of deltas to apply the filter.
+    for i_in in arange(1, lp_iter):
+        ui_delta[:, i_in] = delta + ui_delta[:, i_in - 1]
+
     # Rechape into a vector.
-    ui_delta = ui_delta.reshape(lp_iter*num_samples)
+    ui_delta = ui_delta.reshape(lp_iter * num_samples)
 
     # Apply the filter.
-    ui_delta = signal.lfilter([b0], [1,-a1], ui_delta, axis=- 1, zi=None)
-    
+    ui_delta = signal.lfilter([b0], [1, -a1], ui_delta, axis=-1, zi=None)
+
     # Reshape again to recover the first col.
-    ui_delta = ui_delta.reshape(loudness.shape[0],lp_iter)
-    filt_loudness = ui_delta[:,0]
+    ui_delta = ui_delta.reshape(loudness.shape[0], lp_iter)
+    filt_loudness = ui_delta[:, 0]
     return filt_loudness
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/_nonlinear_decay.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_nonlinear_decay.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 # -*- coding: utf-8 -*-
-"""
-@date Created on Fri May 22 2020
-@author martin_g for Eomys
-"""
 
-# Standard library imports
-import math
 
-# Third party import
-import numpy as np
+# Standard library imports
+from math import sqrt, exp
+from numpy import copy, roll, zeros, arange, logical_and, logical_not
 
 
 def _nl_loudness(core_loudness):
     """Simulate the nonlinear temporal decay of the hearing system
 
     Parameters
     ----------
@@ -22,63 +17,62 @@
     Outputs
     -------
     nl_loudness :  numpy.ndarray
         Loudness with non linear temporal decay
     """
     # Initialization
     sample_rate = 2000
-    nl_loudness = np.copy(core_loudness)
+    nl_loudness = copy(core_loudness)
     # Factor for virtual upsampling/inner iterations
     nl_iter = 24
     # Time constants for non_linear temporal decay
     t_short = 0.005
     t_long = 0.015
     t_var = 0.075
     # Initializes constants B and states of capacitors C1 and C2
     delta_t = 1 / (sample_rate * nl_iter)
     P = (t_var + t_long) / (t_var * t_short)
     Q = 1 / (t_short * t_var)
-    lambda_1 = -P / 2 + math.sqrt(P * P / 4 - Q)
-    lambda_2 = -P / 2 - math.sqrt(P * P / 4 - Q)
+    lambda_1 = -P / 2 + sqrt(P * P / 4 - Q)
+    lambda_2 = -P / 2 - sqrt(P * P / 4 - Q)
     den = t_var * (lambda_1 - lambda_2)
-    e1 = math.exp(lambda_1 * delta_t)
-    e2 = math.exp(lambda_2 * delta_t)
+    e1 = exp(lambda_1 * delta_t)
+    e2 = exp(lambda_2 * delta_t)
     B = [
         (e1 - e2) / den,
         ((t_var * lambda_2 + 1) * e1 - (t_var * lambda_1 + 1) * e2) / den,
         ((t_var * lambda_1 + 1) * e1 - (t_var * lambda_2 + 1) * e2) / den,
         (t_var * lambda_1 + 1) * (t_var * lambda_2 + 1) * (e1 - e2) / den,
-        math.exp(-delta_t / t_long),
-        math.exp(-delta_t / t_var),
+        exp(-delta_t / t_long),
+        exp(-delta_t / t_var),
     ]
     nl_lp = {"B": B}
-    #nl_lp["uo_last"] = 0
-    #nl_lp["u2_last"] = 0
+    # nl_lp["uo_last"] = 0
+    # nl_lp["u2_last"] = 0
 
-    delta = np.copy(core_loudness,)
-    delta = np.roll(delta, -1, axis=1)
+    delta = copy(core_loudness,)
+    delta = roll(delta, -1, axis=1)
     delta[:, -1] = 0
     delta = (delta - nl_loudness)/nl_iter
-    ui_delta = np.zeros(core_loudness.size*nl_iter).reshape(
+    ui_delta = zeros(core_loudness.size*nl_iter).reshape(
         core_loudness.shape[0], core_loudness.shape[1], nl_iter)
     ui_delta[:, :, 0] = core_loudness
 
-    for i_in in np.arange(1, nl_iter):
-        ui_delta[:, :, i_in] = ui_delta[:, :, i_in-1] + delta
+    for i_in in arange(1, nl_iter):
+        ui_delta[:, :, i_in] = ui_delta[:, :, i_in - 1] + delta
 
-    ui_delta = ui_delta.reshape(
-        core_loudness.shape[0], core_loudness.shape[1]*nl_iter)
-    uo_mat = np.copy(ui_delta,)
+    ui_delta = ui_delta.reshape(core_loudness.shape[0], core_loudness.shape[1] * nl_iter)
+    uo_mat = copy(ui_delta,)
     # create u2_mat (equivalent to u2 last) and fill the first col.
-    u2_mat = np.zeros(uo_mat.shape[0]*uo_mat.shape[1]
+    u2_mat = zeros(uo_mat.shape[0]*uo_mat.shape[1]
                       ).reshape(uo_mat.shape[0], uo_mat.shape[1])
     mask = core_loudness[:, 0] >= 1e-5
-    u2_mat[mask, 0] = core_loudness[mask, 0]*(1 - nl_lp["B"][5])
+    u2_mat[mask, 0] = core_loudness[mask, 0] * (1 - nl_lp["B"][5])
 
-    '''
+    """
     Truth Table for u2 & uo
     u2 = nl_lp["uo_last"] * nl_lp["B"][0] - nl_lp["u2_last"] * nl_lp["B"][1]
     u2' = (nl_lp["u2_last"] - ui) * nl_lp["B"][5] + ui
     ui < uo(j-1) | uo(j-1) > u2(j-1) | uo < ui  |u2 > uo  |uo' < ui  |abs(ui -  uo(j-1)) < 1e-5 | ui > u2(j-1) | uo                                      |  u2
     ---------------------------------------------------------------
         Truth           Truth           Truth      Truth       --             --                                 ui                                       ui
         Truth           Truth           False      Truth       --             --                                 uo=f(uo(j-1),u2(j-1),B(2),B(3))          uo=f(uo(j-1),u2(j-1),B(2),B(3))
@@ -87,39 +81,52 @@
         Truth           False                                  Truth                                             ui                                       ui
         Truth           False                                  False                                             uo=f(uo(j-1),B(4)                        uo=f(uo(j-1),B(4) 
         False                                                                Truth                  Truth        ui                                       u2=f(u2(j-1),B(5),ui(j)
         False                                                                Truth                  False        ui                                       ui
         False                                                                False                  Truth        ui                                       u2=f(u2(j-1),B(5),ui(j)
         False                                                                False                  False        ui                                       u2=f(u2(j-1),B(5),ui(j)
  
-    '''
-    for col in np.arange(core_loudness.shape[1]*nl_iter):
+    """
+    for col in arange(core_loudness.shape[1]*nl_iter):
         uo2 = uo_mat[:, col-1] * nl_lp["B"][2] - \
             u2_mat[:, col-1] * nl_lp["B"][3]
-        mask = np.logical_and(
-            uo_mat[:, col-1] > u2_mat[:, col-1], uo2 >= ui_delta[:, col])
+        mask = logical_and(
+            uo_mat[:, col - 1] > u2_mat[:, col - 1], uo2 >= ui_delta[:, col]
+        )
         uo_mat[mask, col] = uo2[mask]  # in case uo higher than ui
 
         uo2 = uo_mat[:, col-1] * nl_lp["B"][4]
-        mask = np.logical_and(uo_mat[:, col-1] <=
+        mask = logical_and(uo_mat[:, col-1] <=
                               u2_mat[:, col-1], uo2 >= ui_delta[:, col])
         uo_mat[mask, col] = uo2[mask]  # in case uo_2 higher than ui
 
         u2_mat[:, col] = uo_mat[:, col]  # higher than uo
-        u22 = uo_mat[:, col-1] * nl_lp["B"][0] - \
-            u2_mat[:, col-1] * nl_lp["B"][1]
-        mask = np.logical_and(np.logical_and(
-            ui_delta[:, col] < uo_mat[:, col-1], uo_mat[:, col-1] > u2_mat[:, col-1]), u22 <= uo_mat[:, col])
+        u22 = uo_mat[:, col - 1] * nl_lp["B"][0] - u2_mat[:, col - 1] * nl_lp["B"][1]
+        mask = logical_and(
+            logical_and(
+                ui_delta[:, col] < uo_mat[:, col - 1],
+                uo_mat[:, col - 1] > u2_mat[:, col - 1],
+            ),
+            u22 <= uo_mat[:, col],
+        )
         u2_mat[mask, col] = u22[mask]  # in case u22 lower than uo_last
 
-        u2_2 = (u2_mat[:, col-1] - ui_delta[:, col]) * \
-            nl_lp["B"][5] + ui_delta[:, col]
-        mask = np.logical_and(ui_delta[:, col] >= uo_mat[:, col-1], np.logical_not(np.logical_and(
-            abs(ui_delta[:, col] - uo_mat[:, col-1]) < 1e-5,  uo_mat[:, col] <= u2_mat[:, col-1])))
+        u2_2 = (u2_mat[:, col - 1] - ui_delta[:, col]) * nl_lp["B"][5] + ui_delta[
+            :, col
+        ]
+        mask = logical_and(
+            ui_delta[:, col] >= uo_mat[:, col - 1],
+            logical_not(
+                logical_and(
+                    abs(ui_delta[:, col] - uo_mat[:, col - 1]) < 1e-5,
+                    uo_mat[:, col] <= u2_mat[:, col - 1],
+                )
+            ),
+        )
         u2_mat[mask, col] = u2_2[mask]  # lower than ui
 
     nl_loudness = uo_mat.reshape(
-        core_loudness.shape[0], core_loudness.shape[1], nl_iter)[:, :, 0]
-    uo_mat = uo_mat.reshape(
-        core_loudness.shape[0], core_loudness.shape[1]*nl_iter)
+        core_loudness.shape[0], core_loudness.shape[1], nl_iter
+    )[:, :, 0]
+    uo_mat = uo_mat.reshape(core_loudness.shape[0], core_loudness.shape[1] * nl_iter)
 
     return nl_loudness
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/_square_and_smooth.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_square_and_smooth.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # -*- coding: utf-8 -*-
-"""
-@date Created on Fri May 22 2020
-@author martin_g for Eomys
-"""
 
 # Standard library imports
 import numpy as np
-from scipy import signal
+from scipy.signal import lfilter
 
 
 def _square_and_smooth(sig, center_freq, fs):
     """3rd order low-pass filtering (See ISO 532-1 section 6.3)
 
     Parameters
     ----------
@@ -28,15 +24,15 @@
     """
     # Frequency dependent time constant
     if center_freq <= 1000:
         tau = 2 / (3 * center_freq)
     else:
         tau = 2 / (3 * 1000)
     # Squaring
-    sig = sig ** 2
+    sig = sig**2
     # Three smoothing low-pass filters
     a1 = np.exp(-1 / (fs * tau))
     b0 = 1 - a1
     # zi = signal.lfilter_zi([b0], [1 -a1])
     for i in range(3):
-        sig = signal.lfilter([b0], [1, -a1], sig)
+        sig = lfilter([b0], [1, -a1], sig)
     return sig
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/_temporal_weighting.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_temporal_weighting.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 # -*- coding: utf-8 -*-
-"""
-@date Created on Fri May 22 2020
-@author martin_g for Eomys
-"""
 
 # Local application import
 from mosqito.sq_metrics.loudness.loudness_zwtv._lowpass_intp import (
     _lowpass_intp,
 )
 
 
@@ -25,15 +21,15 @@
 
     Outputs
     -------
     loudness : numpy.ndarray
         Filtered loudness
     """
     sample_rate = 2000
-    tau = 3.5 * 10 ** -3
+    tau = 3.5 * 10**-3
     filt_loudness_1 = _lowpass_intp(loudness, tau, sample_rate)
-    tau = 70 * 10 ** -3
+    tau = 70 * 10**-3
     filt_loudness_2 = _lowpass_intp(loudness, tau, sample_rate)
 
     loudness = 0.47 * filt_loudness_1 + 0.53 * filt_loudness_2
 
     return loudness
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/_third_octave_levels.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_third_octave_levels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # -*- coding: utf-8 -*-
-"""
-@date Created on Fri May 22 2020
-@author martin_g for Eomys
-"""
 
 # Third party imports
-import numpy as np
-from scipy import signal
+from numpy import linspace, empty, array, log10
+from scipy.signal import sosfilt
 
 # Local application imports
 from mosqito.sq_metrics.loudness.loudness_zwtv._square_and_smooth import (
     _square_and_smooth,
 )
 
 
@@ -33,28 +29,26 @@
         Set of time signals filtered per third octave bands
     """
     # Sampling frequency shall be equal to 48 kHz (as per ISO 532)
     if fs != 48000:
         raise ValueError("""ERROR: Sampling frequency shall be equal to 48 kHz""")
     # Constants
     n_level_band = 28
-    n_filter_coeff = 6
     dec_factor = int(fs / 2000)
     # Initialisation
-    coeff = np.zeros(n_filter_coeff)
     # Filter coefficients of one-third-octave-band filters (reference
     # table)
     # ISO 532-1 Table A.1
-    third_octave_filter_ref = np.array(
+    third_octave_filter_ref = array(
         [[1, 2, 1, 1, -2, 1], [1, 0, -1, 1, -2, 1], [1, -2, 1, 1, -2, 1]]
     )
     # Filter coefficients of one-third-octave-band filters (difference to
     # reference table for 28 one-third-octave-band filters)
     # ISO 532-1 Table A.2
-    third_octave_filter = np.array(
+    third_octave_filter = array(
         [
             [
                 [0, 0, 0, 0, -6.70260e-004, 6.59453e-004],
                 [0, 0, 0, 0, -3.75071e-004, 3.61926e-004],
                 [0, 0, 0, 0, -3.06523e-004, 2.97634e-004],
             ],
             [
@@ -192,15 +186,15 @@
                 [0, 0, 0, 0, -2.19464e000, 2.76470e-001],
                 [0, 0, 0, 0, -1.90231e000, 1.47304e-001],
             ],
         ]
     )
     # Filter gain values
     # ISO 532-1 Table A.2
-    filter_gain = np.array(
+    filter_gain = array(
         [
             4.30764e-011,
             8.59340e-011,
             1.71424e-010,
             3.41944e-010,
             6.82035e-010,
             1.36026e-009,
@@ -258,28 +252,28 @@
         6300,
         8000,
         10000,
         12500,
     ]
 
     n_time = len(sig[::dec_factor])
-    time_axis = np.linspace(0, len(sig) / fs, num=n_time)
+    time_axis = linspace(0, len(sig) / fs, num=n_time)
 
-    third_octave_level = np.zeros((n_level_band, n_time))
+    third_octave_level = empty((n_level_band, n_time))
     for i_bands in range(n_level_band):
-        
+
         # Initialisation
-        tiny_value = 10 ** -12
-        i_ref = 4 * 10 ** -10
+        tiny_value = 10**-12
+        i_ref = 4 * 10**-10
         # 2nd order fltering (See ISO 532-1 section 6.3 and A.2)
         coeff = third_octave_filter_ref - third_octave_filter[i_bands, :, :]
-        sig_filt = filter_gain[i_bands] * signal.sosfilt(coeff, sig)
+        sig_filt = filter_gain[i_bands] * sosfilt(coeff, sig)
         # Calculate center frequency of filter
         center_freq = 10 ** ((i_bands - 16) / 10) * 1000
         # Squaring and smoothing of filtered signal
         sig_filt = _square_and_smooth(sig_filt, center_freq, 48000)
         # SPL calculation and decimation
-        third_octave_level[i_bands, :] = 10 * np.log10(
+        third_octave_level[i_bands, :] = 10 * log10(
             (sig_filt[::dec_factor] + tiny_value) / i_ref
         )
 
     return third_octave_level, time_axis, freq
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/loudness_zwtv/loudness_zwtv.py` & `mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_zwtv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,64 @@
 # -*- coding: utf-8 -*-
 
-# Standard library imports
-import numpy as np
+# Third party imports
+import pytest
+
+# Local application imports
+from mosqito.sq_metrics import loudness_zwtv
+from mosqito.utils import load
+from validations.sq_metrics.loudness_zwtv.validation_loudness_zwtv import (
+    _check_compliance,
+)
+
+
+@pytest.mark.loudness_zwtv  # to skip or run only loudness zwicker time-varying tests
+def test_loudness_zwtv():
+    """Test function for the script loudness_zwicker_time
+
+    Test function for the script loudness_zwtv with
+    .wav file as input. The input file is provided by ISO 532-1 annex
+    B4 and B5, the compliance is assessed according to section 6.1 of the
+    standard. One .png compliance plot is generated.
 
-# Local applications imports
-from mosqito.sq_metrics.loudness.loudness_zwst._main_loudness import _main_loudness
-from mosqito.sq_metrics.loudness.loudness_zwst._calc_slopes import _calc_slopes
-from mosqito.sq_metrics.loudness.loudness_zwtv._nonlinear_decay import _nl_loudness
-from mosqito.sq_metrics.loudness.loudness_zwtv._temporal_weighting import _temporal_weighting
-from mosqito.sq_metrics.loudness.loudness_zwtv._third_octave_levels import _third_octave_levels
-
-
-def loudness_zwtv(signal, fs, field_type='free'):
-    """Calculate Zwicker-loudness for time-varying signals
-    Calculate the acoustic loudness according to Zwicker method for
-    time-varying signals.
-    Normatice reference:
-        DIN 45631/A1:2010
-        ISO 532-1:2017 (method 2)
-    The code is based on C program source code published alongside
-    with ISO 532-1 standard.
-    Note that for reasons of normative continuity, as defined in the
-    preceeding standards, the method is in accordance with
-    ISO 226:1987 equal loudness contours (instead of ISO 226:2003)
     Parameters
     ----------
-    signal : numpy.array
-        A time signal values [Pa].
-    fs : integer
-        Sampling frequency.
-    field_type : str
-        Type of soundfield corresponding to signal ("free" by or "diffuse").
-        
+    None
+
     Outputs
     -------
-    N : float
-        Calculated loudness [sones], size (Ntime,).
-    N_specific : numpy.ndarray
-        Specific loudness [sones/bark], size (Nbark, Ntime).
-    bark_axis : numpy.ndarray
-        Corresponding bark axis, size (Nbark,).
-    time_axis : numpy.ndarray
-        Time axis, size (Ntime,).
-
-    """        
-
-    if fs < 48000:
-        print("[Warning] Signal resampled to 48 kHz to allow calculation. To fulfill the standard requirements fs should be >=48 kHz."
-             )
-        from scipy.signal import resample
-        signal = resample(signal, int(48000 * len(signal) / fs))
-        fs = 48000
-
-
-    # Compute third octave band spectrum vs. time
-    spec_third, time_axis, _ = _third_octave_levels(signal, fs)
-
-    # Calculate core loudness (vectorized version)
-    core_loudness = _main_loudness(spec_third, field_type)
-
-    #
-    # Nonlinearity
-    core_loudness = _nl_loudness(core_loudness)
-    #
-    # Calculation of specific loudness
-    loudness, spec_loudness = _calc_slopes(core_loudness)
-
-    # temporal weigthing
-    filt_loudness = _temporal_weighting(loudness)
-    #
-    # Decimation from temporal resolution 0.5 ms to 2ms and return
-    dec_factor = 4
-    N = filt_loudness[::dec_factor]
-    N_spec = spec_loudness[:, ::dec_factor]
-    time_axis = time_axis[::dec_factor]
-    #
-    # Build bark axis
-    bark_axis = np.linspace(0.1, 24, int(24 / 0.1))
-
-    return N, N_spec, bark_axis, time_axis
+    None
+    """
+    # Test signal as input for time-varying loudness
+    # (from ISO 532-1 annex B4)
+    signal = {
+        "data_file": "tests/input/Test signal 10 (tone pulse 1 kHz 10 ms 70 dB).wav",
+        "xls": "tests/input/Results and tests for synthetic signals (time varying loudness).xlsx",
+        "tab": "Test signal 10",
+        "N_specif_bark": 8.5,
+        "field": "free",
+    }
+
+    # Load signal and compute third octave band spectrum
+    sig, fs = load(signal["data_file"], wav_calib=2 * 2**0.5)
+
+    # Compute Loudness
+    N, N_spec, bark_axis, time_axis = loudness_zwtv(sig, fs, field_type=signal["field"])
+    loudness = {
+        "name": "Loudness",
+        "values": N,
+        "specific values": N_spec,
+        "freqs": bark_axis,
+    }
+
+    # Check axis dimensions
+    assert len(N) == len(time_axis)
+    assert N_spec.shape[1] == len(time_axis)
+    assert N_spec.shape[0] == len(bark_axis)
+
+    # Check ISO 532-1 compliance
+    assert _check_compliance(loudness, signal, "./tests/output/")
+
+
+# test de la fonction
+if __name__ == "__main__":
+    test_loudness_zwtv()
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/utils/phone2spl.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/phone2spl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # -*- coding: utf-8 -*-
-"""
-@author: Daniel Jiménez-Caminero Costa
-"""
-
-import numpy as np
+from numpy import log10
 
 
 def phone2spl(phones, tf, af, lu):
-    """ Conversion from phones to Sound Pressure Level (dB SPL), based on the standard ISO/FDIS 226:2003.
+    """Conversion from phones to Sound Pressure Level (dB SPL), based on the standard ISO/FDIS 226:2003.
 
     Parameters
     ----------
     phones: float
         Logarithmic unit of loudness ('phon' = Ln).
 
     tf: float
@@ -26,13 +22,15 @@
     Returns
     -------
     spl: float
         Sound pressure level ('dB SPL').
 
     """
     # "Af" is argument of the dB SPL conversion formula
-    Af = (4.47 * (10 ** (-3))) * ((10 ** (0.025 * phones)) - 1.15) + ((0.4 * (10 ** (((tf + lu) / 10) - 9))) ** af)
+    Af = (4.47 * (10 ** (-3))) * ((10 ** (0.025 * phones)) - 1.15) + (
+        (0.4 * (10 ** (((tf + lu) / 10) - 9))) ** af
+    )
 
     # Result of the phone value converted to dB SPL value
-    spl = ((10. / af) * np.log10(Af)) - lu + 94
+    spl = ((10. / af) * log10(Af)) - lu + 94
 
     return spl
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/utils/sone2phone.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/sone2phone.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # -*- coding: utf-8 -*-
-"""
-@author: Daniel Jiménez-Caminero Costa
-"""
-
-import numpy as np
+from numpy import log10
 
 
 def sone2phone(sones):
-    """ Conversion between sones and phones, based on the work done by Hugo Fastl and Eberhard Zwicker in the article
+    """Conversion between sones and phones, based on the work done by Hugo Fastl and Eberhard Zwicker in the article
     "Psychoacoustics: Facts and Models".
 
     Parameters
     ----------
     sones: float
         One of the units in which loudness is measured. 1 sone equals to 40 phones. The conversion from sones to phones
         is not linear.
@@ -22,12 +18,12 @@
         Logarithmic unit of loudness (phon = Ln). The dB SPL values of the signal at 1 kHz have the same value in
         phons. For example, 50 db SPL @ 1 kHz corresponds to 50 phones. The rest of the frequencies does not have
         the same co-relation between each other.
 
     """
 
     if sones >= 1:
-        phons = 40 + ((10 * np.log10(sones)) / np.log10(2))
+        phons = 40 + ((10 * log10(sones)) / log10(2))
 
     else:
         phons = 40 * ((sones + 0.0005) ** 0.35)
     return phons
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/loudness/utils/sone_to_phon.py` & `mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/sone_to_phon.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 # -*- coding: utf-8 -*-
-"""
-@date Created on Fri Feb 28 2020
-@author martin_g for Eomys
-"""
 
 # Standard library imports
-import math
+from math import log2
 
 
 def sone_to_phon(sone):
     """Calculate Loudness level [phons] from Loudness [sones]
 
     The code is based on BASIC program published in "Program for
-    calculating loudness according to DIN 45631 (ISO 532B)", E.Zwicker
+    calculating loudness according to DIN 45631 (ISO 532-1:2017)", E.Zwicker
     and H.Fastl, J.A.S.J (E) 12, 1 (1991).
 
     Parameters
     ----------
     N : float
         Loudness [sones]
 
     Outputs
     -------
     LN : float
         Loudness level [phons]
     """
 
     if sone < 1:
-        phon = 40 * sone ** 0.35
+        phon = 40 * sone**0.35
         if phon < 3:
             phon = 3
     else:
-        phon = 10 * math.log2(sone) + 40
+        phon = 10 * log2(sone) + 40
     return phon
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/_H_weighting.py` & `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_H_weighting.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Fri Oct  2 11:38:13 2020
 
-@author: pc
-"""
 # Standard library import
-import numpy as np
-import math
+from numpy import zeros, array, arange, interp
+from math import floor
 
 
 def _H_weighting(n, fs):
     """Weighting functions Hi definition for each 1-bark-wide interval i
 
     The code is based on the article "Psychoacoustical roughness:
     implementation of an optimized model" by Daniel and Weber in 1997.
@@ -39,35 +35,35 @@
     -------
     H : numpy.array
         47 weighting functions Hi
 
     """
     cut = 2
     # freq_axis = np.concatenate((np.arange(0,int(n/2),1)*fs/n,np.zeros((int(n/2)))))
-    H = np.zeros((47, n))
+    H = zeros((47, n))
 
     # H2, H16 and H42 are given
 
-    H2_x = np.array([0, 17, 23, 25, 32, 37, 48, 67, 90, 114, 171, 206, 247, 294, 358])
-    H2_y = np.array(
+    H2_x = array([0, 17, 23, 25, 32, 37, 48, 67, 90, 114, 171, 206, 247, 294, 358])
+    H2_y = array(
         [0, 0.8, 0.95, 0.975, 1, 0.975, 0.9, 0.8, 0.7, 0.6, 0.4, 0.3, 0.2, 0.1, 0]
     )
-    last = math.floor((358 / fs) * n)
-    j = np.arange(cut, last)
+    last = floor((358 / fs) * n)
+    j = arange(cut, last)
     freq = j * fs / n
-    H[1, j] = np.interp(freq[j - cut], H2_x, H2_y)
+    H[1, j] = interp(freq[j - cut], H2_x, H2_y)
 
-    H5_x = np.array([0, 32, 43, 56, 69, 92, 120, 142, 165, 231, 277, 331, 397, 502])
-    H5_y = np.array([0, 0.8, 0.95, 1, 0.975, 0.9, 0.8, 0.7, 0.6, 0.4, 0.3, 0.2, 0.1, 0])
-    last = math.floor((502 / fs) * n)
-    j = np.arange(cut, last)
+    H5_x = array([0, 32, 43, 56, 69, 92, 120, 142, 165, 231, 277, 331, 397, 502])
+    H5_y = array([0, 0.8, 0.95, 1, 0.975, 0.9, 0.8, 0.7, 0.6, 0.4, 0.3, 0.2, 0.1, 0])
+    last = floor((502 / fs) * n)
+    j = arange(cut, last)
     freq = j * fs / n
-    H[4, j] = np.interp(freq[j - cut], H5_x, H5_y)
+    H[4, j] = interp(freq[j - cut], H5_x, H5_y)
 
-    H16_x = np.array(
+    H16_x = array(
         [
             0,
             23.5,
             34,
             47,
             56,
             63,
@@ -83,15 +79,15 @@
             290,
             348,
             415,
             500,
             645,
         ]
     )
-    H16_y = np.array(
+    H16_y = array(
         [
             0,
             0.4,
             0.6,
             0.8,
             0.9,
             0.95,
@@ -107,21 +103,21 @@
             0.4,
             0.3,
             0.2,
             0.1,
             0,
         ]
     )
-    last = math.floor((502 / fs) * n)
-    j = np.arange(cut, last)
+    last = floor((502 / fs) * n)
+    j = arange(cut, last)
     freq = j * fs / n
 
-    H[15, j] = np.interp(freq[j - cut], H16_x, H16_y)
+    H[15, j] = interp(freq[j - cut], H16_x, H16_y)
 
-    H21_x = np.array(
+    H21_x = array(
         [
             0,
             19,
             44,
             52.5,
             58,
             75,
@@ -135,15 +131,15 @@
             290,
             348,
             415,
             500,
             645,
         ]
     )
-    H21_y = np.array(
+    H21_y = array(
         [
             0,
             0.4,
             0.8,
             0.9,
             0.95,
             1,
@@ -157,17 +153,17 @@
             0.4,
             0.3,
             0.2,
             0.1,
             0,
         ]
     )
-    H[20, j] = np.interp(freq[j - cut], H21_x, H21_y)
+    H[20, j] = interp(freq[j - cut], H21_x, H21_y)
 
-    H42_x = np.array(
+    H42_x = array(
         [
             0,
             15,
             41,
             49,
             53,
             64,
@@ -182,15 +178,15 @@
             290,
             348,
             415,
             500,
             645,
         ]
     )
-    H42_y = np.array(
+    H42_y = array(
         [
             0,
             0.4,
             0.8,
             0.9,
             0.965,
             0.99,
@@ -205,15 +201,15 @@
             0.4,
             0.3,
             0.2,
             0.1,
             0,
         ]
     )
-    H[41, j] = np.interp(freq[j - cut], H42_x, H42_y)
+    H[41, j] = interp(freq[j - cut], H42_x, H42_y)
 
     # According to the article we have :
 
     H[0, :] = H[2, :] = H[3, :] = H[1, :]
     for i in range(5, 15):
         H[i, :] = H[4, :]
     for i in range(16, 20):
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/_ear_filter_coeff.py` & `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_ear_filter_coeff.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Nov  9 10:11:27 2020
 
-@author: pc
-"""
-
-import numpy as np
+# Standard library import
+from numpy import interp
 
 
 def _ear_filter_coeff(bark_axis):
     """Zwicker coefficient for the transmission between outer and inner ear
 
     See E. Zwicker, H. Fastl: Psychoacoustics. Springer,Berlin, Heidelberg, 1990.
     The coefficients are linearly interpolated from the values given in figure 8.18
@@ -71,10 +67,10 @@
         -11.3,
         -20,
         -40,
         -130,
         -999,
     ]
 
-    a0tab = np.interp(bark_axis, xp, yp)
+    a0tab = interp(bark_axis, xp, yp)
 
     return a0tab
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/_gzi_weighting.py` & `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_gzi_weighting.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Fri Nov  6 10:29:02 2020
-
-@author: wantysal
-"""
-
-import numpy as np
 
+# Standard library import
+from numpy import array, arange, interp
 
 def _gzi_weighting(center_freq):
-    """ Weighting function for the specific roughness given by Aures """
+    """Weighting function for the specific roughness given by Aures"""
 
-    gr_x = np.arange(0, 25, 1)
-    gr_y = np.array(
+    gr_x = arange(0, 25, 1)
+    gr_y = array(
         [
             0.15,
             0.26,
             0.38,
             0.47,
             0.54,
             0.65,
@@ -38,10 +33,10 @@
             0.30,
             0.30,
             0.30,
             0.30,
         ]
     )
 
-    gzi = np.interp(center_freq, gr_x, gr_y)
+    gzi = interp(center_freq, gr_x, gr_y)
 
     return gzi
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/_roughness_dw_main_calc.py` & `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_roughness_dw_main_calc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 
 # Standard imports
-import numpy as np
+from numpy import concatenate, zeros, arange, where, interp, mean, real, corrcoef, power, sqrt, abs, empty
 from numpy.fft import fft, ifft
 import math
 
 # Local imports
 from mosqito.utils.LTQ import LTQ
 from mosqito.sq_metrics.roughness.roughness_dw._ear_filter_coeff import (
     _ear_filter_coeff,
 )
-from mosqito.utils.conversion import freq2bark, db2amp, amp2db, bark2freq
+from mosqito.utils import freq2bark, db2amp, amp2db, bark2freq
+
 
 def _roughness_dw_main_calc(spec, freq_axis, fs, gzi, hWeight):
     """
     Daniel and Weber roughness main calculation
 
     Parameters
     ----------
@@ -37,90 +38,92 @@
     """
     if len(spec) != len(freq_axis):
         raise ValueError(
             "spectrum and frequency axis should have the same number of points !"
         )
 
     # convert spectrum to 2-sided
-    spec = np.concatenate((spec, spec[len(spec)::-1]))
+    spec = concatenate((spec, spec[len(spec)::-1]))
 
     n = len(spec)
     # Frequency axis in Bark
     bark_axis = freq2bark(freq_axis)
     # Highest frequency
-    nZ = np.arange(1, n//2 + 1, 1)
+    nZ = arange(1, n//2 + 1, 1)
 
     # Calculate Zwicker a0 factor (transfer characteristic of the outer and inner ear)
-    a0 = np.zeros((n))
+    a0 = zeros((n))
     a0[nZ - 1] = db2amp(_ear_filter_coeff(bark_axis), ref=1)
     spec = a0 * spec
 
     # Conversion of the spec into dB
-    module = np.abs(spec[0:n//2])
+    module = abs(spec[0:n//2])
     spec_dB = amp2db(module, ref=2e-5)
-    
+
     # Find the audible components within the spec
     threshold = LTQ(bark_axis, reference="roughness")
-    audible_index = np.where(spec_dB > threshold)[0]
+    audible_index = where(spec_dB > threshold)[0]
     # Number of audible frequencies
     n_aud = len(audible_index)
 
     # --------------------------------- stage 1 ------------------------------------
     # ----------------Creation of the specific excitations functions----------------
 
     # Terhardt's slopes definition
     # lower slope [dB/Bark]
     s1 = -27
-    s2 = np.zeros((n_aud))
+    s2 = zeros((n_aud))
     # upper slope [dB/Bark]
-    for k in np.arange(0, n_aud, 1):
+    for k in arange(0, n_aud, 1):
         s2[k] = min(
-            -24 - (230 / freq_axis[audible_index[k]]) + (0.2 * spec_dB[audible_index[k]]),
+            -24
+            - (230 / freq_axis[audible_index[k]])
+            + (0.2 * spec_dB[audible_index[k]]),
             0,
         )
 
     # The excitation pattern are calculated for 47 overlapping 1-bark-wide channels
     n_channel = 47
     # Channels number
-    zi = np.arange(1, n_channel + 1) / 2
+    zi = arange(1, n_channel + 1) / 2
     # Center frequencies for each channel
     zb = bark2freq(zi) * n / fs
     # Minimum excitation level
-    minExcitDB = np.interp(zb, nZ, threshold)
-    
-    ch_low = np.zeros((n_aud))
-    ch_high = np.zeros((n_aud))
-    for i in np.arange(0, n_aud):
+    minExcitDB = interp(zb, nZ, threshold)
+
+    ch_low = zeros((n_aud))
+    ch_high = zeros((n_aud))
+    for i in arange(0, n_aud):
         # Lower limit of the channel corresponding to each component
         ch_low[i] = math.floor(2 * bark_axis[audible_index[i]]) - 1
         # Higher limit
         ch_high[i] = math.ceil(2 * bark_axis[audible_index[i]]) - 1
 
     # Creation of the excitation pattern
-    slopes = np.zeros((n_aud, n_channel))
-    for k in np.arange(0, n_aud):
+    slopes = zeros((n_aud, n_channel))
+    for k in arange(0, n_aud):
         levDB = spec_dB[audible_index[k]]
         b = bark_axis[audible_index[k]]
-        for j in np.arange(0, int(ch_low[k] + 1)):
+        for j in arange(0, int(ch_low[k] + 1)):
             sl = (s1 * (b - ((j + 1) * 0.5))) + levDB
             if sl > minExcitDB[j]:
                 slopes[k, j] = db2amp(sl, ref=0.00002)
-        for j in np.arange(int(ch_high[k]), n_channel):
+        for j in arange(int(ch_high[k]), n_channel):
             sl = (s2[k] * (((j + 1) * 0.5) - b)) + levDB
             if sl > minExcitDB[j]:
                 slopes[k, j] = db2amp(sl, ref=0.00002)
 
     # Initialization
-    hBP = np.zeros((n_channel, n))
-    mod_depth = np.zeros((n_channel))
+    hBP = zeros((n_channel, n))
+    mod_depth = zeros((n_channel))
 
     # Definition of the excitation amplitude
-    for i in np.arange(0, n_channel, 1):
-        exc = np.zeros((n), dtype=complex)
-        for j in np.arange(0, n_aud, 1):
+    for i in arange(0, n_channel, 1):
+        exc = zeros((n), dtype=complex)
+        for j in arange(0, n_aud, 1):
             ind = audible_index[j]
             # the component belongs to the bark window
             if ch_low[j] == i:
                 ampl = 1
             elif ch_high[j] == i:
                 ampl = 1
             # the component is higher than the bark window
@@ -130,64 +133,61 @@
             else:
                 ampl = slopes[j, i - 1] / module[ind]
 
             # reconstruction of the spec
             exc[ind] = ampl * spec[ind]
 
         # The temporal specific excitation functions are obtained by IFFT
-        temporal_excitation = np.abs(n * np.real(ifft(exc)))
+        temporal_excitation = abs(n * real(ifft(exc)))
         # ------------------------------- stage 2 --------------------------------------
         # ---------------------modulation depth calculation-----------------------------
 
         # The fluctuations of the envelope are contained in the low frequency part
         # of the spec of specific excitations in absolute value
-        h0 = np.mean(temporal_excitation)
+        h0 = mean(temporal_excitation)
         envelope_spec = fft(temporal_excitation - h0)
 
         # This spec is weighted to model the low-frequency  bandpass
         # characteristic of the roughness on modulation frequency
         envelope_spec = envelope_spec * hWeight[i, :]
         # The time functions of the bandpass filtered envelopes hBPi(t)
         # are calculated via inverse Fourier transform :
-        hBP[i, :] = 2 * np.real(ifft(envelope_spec))
+        hBP[i, :] = 2 * real(ifft(envelope_spec))
 
         # Modulation depth estimation is given by envelope RMS values
         # and excitation functions time average :
-        hBPrms = np.sqrt(np.mean(np.power(hBP[i, :], 2)))
+        hBPrms = sqrt(mean(power(hBP[i, :], 2)))
         if h0 > 0:
             mod_depth[i] = hBPrms / h0
             if mod_depth[i] > 1:
                 mod_depth[i] = 1
         else:
             mod_depth[i] = 0
     # ------------------------------- stage 3 --------------------------------------
     # ----------------roughness calculation with cross correlation------------------
 
     # Crosscorrelation coefficients between the envelopes of the channels
     # i and i+2 with dz= 1 bark
-    ki = np.zeros((47))
+    ki = zeros((47))
 
     for i in range(0, 45):
         if hBP[i].all() != 0 and hBP[i + 2].all() != 0:
-            ki[i] = np.corrcoef(hBP[i, :], hBP[i + 2, :])[0, 1]
+            ki[i] = corrcoef(hBP[i, :], hBP[i + 2, :])[0, 1]
 
     # Specific roughness calculation with gzi the modulation depth weighting
     # function given by Aures
-    R_spec = np.zeros((47))
+    R_spec = empty((47))
 
     R_spec[0] = gzi[0] * pow(mod_depth[0] * ki[0], 2)
     R_spec[1] = gzi[1] * pow(mod_depth[1] * ki[1], 2)
-    for i in np.arange(2, 45):
+    for i in arange(2, 45):
         R_spec[i] = gzi[i] * pow(mod_depth[i] * ki[i] * ki[i - 2], 2)
     R_spec[45] = gzi[45] * pow(mod_depth[45] * ki[43], 2)
     R_spec[46] = gzi[46] * pow(mod_depth[46] * ki[44], 2)
 
     # Total roughness calculation with calibration factor of 0.25 given in the article
     # to produce a roughness of 1 asper for a 1-kHz, 60dB tone with carrier frequency
     # of 70 Hz and a modulation depth of 1
 
     R = 0.25 * sum(R_spec)
 
     return R, R_spec, zi
-
-
-
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw.py` & `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,93 @@
 # -*- coding: utf-8 -*-
 
 # Standard imports
-import numpy as np
+from numpy import arange, empty
 
 # Local imports
 from mosqito.utils.time_segmentation import time_segmentation
-from mosqito.sound_level_meter.spectrum import spectrum
+from mosqito.sound_level_meter.comp_spectrum import comp_spectrum
 from mosqito.sq_metrics.roughness.roughness_dw._roughness_dw_main_calc import (
     _roughness_dw_main_calc,
 )
 from mosqito.sq_metrics.roughness.roughness_dw._gzi_weighting import _gzi_weighting
 from mosqito.sq_metrics.roughness.roughness_dw._H_weighting import _H_weighting
 
 
 def roughness_dw(signal, fs, overlap=0.5):
-    """Roughness calculation of a signal sampled at 48kHz.
+    """
+    Computes the roughness according to Daniel and Weber method
+    from a time signal
 
-    The code is based on the algorithm described in "Psychoacoustical roughness:
-    implementation of an optimized model" by Daniel and Weber in 1997.
-    The roughness model consists of a parallel processing structure that is made up
-    of successive stages and calculates intermediate specific roughnesses R_spec,
-    which are summed up to determine the total roughness R.
+    This function computes the global and specific roughness values
+    of a signal sampled at 48 kHz.
 
     Parameters
     ----------
-    signal :numpy.array
-        A time signal [Pa]
+    signal : array_like or DataTime object
+        Input time signal in Pa
     fs : float
         Sampling frequency [Hz]
     overlap : float
         Overlapping coefficient for the time windows of 200ms
 
-    Outputs
+    Returns
     -------
     R : numpy.array
-        Roughness [asper].
+        Roughness value in [asper]
     R_spec : numpy.array
-        Specific roughness over bark axis.
+        Specific roughness over bark axis
     bark_axis : numpy.array
-        Frequency axis [bark].
+        Frequency axis in [bark]
     time : numpy.array
-        Time axis [s].
+        Time axis in [s]
+
+    See Also
+    --------
+    .roughness_dw_freq : Roughness computation from a sound spectrum
+
+    Notes
+    -----
+    The model consists of a parallel processing structure made up
+    of successive stages to calculate intermediate specific roughnesses :math:`R'`,
+    which are summed up to determine the total roughness :math:`R`:
+
+    .. math::
+        R=0.25\\sum_{i=1}^{47}R'_{i}
+
+    References
+    ----------
+    :cite:empty:`R-roughnessDW`
+
+    .. bibliography::
+        :keyprefix: R-
 
+    Examples
+    --------
+    .. plot::
+       :include-source:
+
+       >>> from mosqito.sq_metrics import roughness_dw
+       >>> import matplotlib.pyplot as plt
+       >>> import numpy as np
+       >>> fc=1000
+       >>> fmod=70
+       >>> fs=44100
+       >>> d=0.2
+       >>> dB=60
+       >>> time = np.arange(0, d, 1/fs)
+       >>> stimulus = (0.5 * (1 + np.sin(2 * np.pi * fmod * time))* np.sin(2 * np.pi * fc * time))
+       >>> rms = np.sqrt(np.mean(np.power(stimulus, 2)))
+       >>> ampl = 0.00002 * np.power(10, dB / 20) / rms
+       >>> stimulus = stimulus * ampl
+       >>> R, R_specific, bark, time = roughness_dw(stimulus, fs=44100, overlap=0)
+       >>> plt.plot(bark, R_specific)
+       >>> plt.xlabel("Bark axis [Bark]")
+       >>> plt.ylabel("Specific roughness [Asper/Bark]")
+       >>> plt.title("Roughness = " + f"{R[0]:.2f}" + " [Asper]")
     """
 
     # Number of points within each frame according to the time resolution of 200ms
     nperseg = int(0.2 * fs)
     # Overlapping segment length
     noverlap = int(overlap * nperseg)
     # reshaping of the signal according to the overlap and time proportions
@@ -53,27 +95,27 @@
         signal, fs, nperseg=nperseg, noverlap=noverlap, is_ecma=False
     )
     if len(sig.shape) == 1:
         nseg = 1
     else:
         nseg = sig.shape[1]
 
-    spec, _ = spectrum(sig, fs, nfft="default", window="blackman", db=False)
+    spec, _ = comp_spectrum(sig, fs, nfft="default", window="blackman", db=False)
 
     # Frequency axis in Hertz
-    freq_axis = np.arange(1, nperseg // 2 + 1, 1) * (fs / nperseg)
+    freq_axis = arange(1, nperseg // 2 + 1, 1) * (fs / nperseg)
 
     # Initialization of the weighting functions H and g
     hWeight = _H_weighting(nperseg, fs)
     # Aures modulation depth weighting function
-    gzi = _gzi_weighting(np.arange(1, 48, 1) / 2)
+    gzi = _gzi_weighting(arange(1, 48, 1) / 2)
 
-    R = np.zeros((nseg))
-    R_spec = np.zeros((47, nseg))
     if len(spec.shape) > 1:
+        R = empty((nseg))
+        R_spec = empty((47, nseg))
         for i in range(nseg):
             R[i], R_spec[:, i], bark_axis = _roughness_dw_main_calc(
                 spec[:, i], freq_axis, fs, gzi, hWeight
             )
     else:
         R, R_spec, bark_axis = _roughness_dw_main_calc(
             spec, freq_axis, fs, gzi, hWeight
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/sharpness/sharpness_din/_weighting_fastl.py` & `mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/_weighting_fastl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import numpy as np
+from numpy import array
 
 # Zwicker and Fastl weighting function
-x = np.array(
+x = array(
     [
         0.0985854,
         14.826764,
         15.364039,
         15.863559,
         16.297388,
         16.533346,
@@ -53,15 +53,15 @@
         23.38871,
         23.5416,
         23.6848,
         23.932978,
     ]
 )
 
-y = np.array(
+y = array(
     [
         0.9783246,
         0.99701804,
         1.0092967,
         1.0169811,
         1.0438102,
         1.0713409,
@@ -107,8 +107,8 @@
         3.147401,
         3.2980514,
         3.429891,
         3.5806417,
         3.7125149,
         3.9385738,
     ]
-)
+)
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_band_procedure_data.py` & `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_band_procedure_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from numpy import array
 
+
 def _get_critical_band_data():
-    """ See § 3.4 of the standard ANSI S3.5. """
+    """See § 3.4 of the standard ANSI S3.5."""
     CENTER_FREQUENCIES = array(
         [
             150,
             250,
             350,
             450,
             570,
@@ -20,15 +21,15 @@
             2500,
             2900,
             3400,
             4000,
             4800,
             5800,
             7000,
-            8500
+            8500,
         ]
     )
 
     LOWER_FREQUENCIES = array(
         [
             100,
             200,
@@ -46,15 +47,15 @@
             2320,
             2700,
             3150,
             3700,
             4400,
             5300,
             6400,
-            7700
+            7700,
         ]
     )
 
     UPPER_FREQUENCIES = array(
         [
             200,
             300,
@@ -72,18 +73,18 @@
             2700,
             3150,
             3700,
             4400,
             5300,
             6400,
             7700,
-            9500
+            9500,
         ]
     )
-    
+
     IMPORTANCE = array(
         [
             0.0103,
             0.0261,
             0.0419,
             0.0577,
             0.0577,
@@ -98,18 +99,18 @@
             0.0577,
             0.0577,
             0.0577,
             0.0577,
             0.0460,
             0.0343,
             0.0226,
-            0.0110
+            0.0110,
         ]
     )
-    
+
     STANDARD_SPEECH_SPECTRUM_NORMAL = array(
         [
             31.44,
             34.75,
             34.14,
             34.58,
             33.17,
@@ -124,15 +125,15 @@
             13.80,
             12.21,
             11.09,
             9.33,
             5.84,
             3.47,
             1.78,
-            -0.14
+            -0.14,
         ]
     )
 
     REFERENCE_INTERNAL_NOISE_SPECTRUM = array(
         [
             1.50,
             -3.90,
@@ -150,131 +151,139 @@
             -21.20,
             -23.20,
             -24.90,
             -25.90,
             -24.20,
             -19.00,
             -11.70,
-            -6.00
+            -6.00,
         ]
     )
 
     FREEFIELD2EARDRUM_TRANSFER_FUNCTION = array(
         [
-        0.60,
-        1.00,
-        1.40,
-        1.40,
-        1.90,
-        2.80,
-        3.00,
-        2.60,
-        2.60,
-        3.60,
-        6.10,
-        10.50,
-        13.80,
-        16.80,
-        15.80,
-        14.90,
-        14.30,
-        12.40,
-        7.90,
-        4.30,
-        0.50
-        ]
+            0.60,
+            1.00,
+            1.40,
+            1.40,
+            1.90,
+            2.80,
+            3.00,
+            2.60,
+            2.60,
+            3.60,
+            6.10,
+            10.50,
+            13.80,
+            16.80,
+            15.80,
+            14.90,
+            14.30,
+            12.40,
+            7.90,
+            4.30,
+            0.50,
+        ]
+    )
+    return (
+        CENTER_FREQUENCIES,
+        LOWER_FREQUENCIES,
+        UPPER_FREQUENCIES,
+        IMPORTANCE,
+        REFERENCE_INTERNAL_NOISE_SPECTRUM,
+        STANDARD_SPEECH_SPECTRUM_NORMAL,
     )
-    return CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, IMPORTANCE, REFERENCE_INTERNAL_NOISE_SPECTRUM, STANDARD_SPEECH_SPECTRUM_NORMAL
+
 
 def _get_equal_critical_band_data():
     CENTER_FREQUENCIES = array(
         [
-        350,
-        450,
-        570,
-        700,
-        840,
-        1000,
-        1170,
-        1370,
-        1600,
-        1850,
-        2150,
-        2500,
-        2900,
-        3400,
-        4000,
-        4800,
-        5800,
+            350,
+            450,
+            570,
+            700,
+            840,
+            1000,
+            1170,
+            1370,
+            1600,
+            1850,
+            2150,
+            2500,
+            2900,
+            3400,
+            4000,
+            4800,
+            5800,
         ]
     )
 
     LOWER_FREQUENCIES = array(
         [
-        300,
-        400,
-        510,
-        630,
-        770,
-        920,
-        1080,
-        1270,
-        1480,
-        1720,
-        2000,
-        2320,
-        2700,
-        3150,
-        3700,
-        4400,
-        5300,
+            300,
+            400,
+            510,
+            630,
+            770,
+            920,
+            1080,
+            1270,
+            1480,
+            1720,
+            2000,
+            2320,
+            2700,
+            3150,
+            3700,
+            4400,
+            5300,
         ]
     )
 
     UPPER_FREQUENCIES = array(
         [
-        400,
-        510,
-        630,
-        770,
-        920,
-        1080,
-        1270,
-        1480,
-        1720,
-        2000,
-        2320,
-        2700,
-        3150,
-        3700,
-        4400,
-        5300,
-        6400
+            400,
+            510,
+            630,
+            770,
+            920,
+            1080,
+            1270,
+            1480,
+            1720,
+            2000,
+            2320,
+            2700,
+            3150,
+            3700,
+            4400,
+            5300,
+            6400,
         ]
     )
 
     IMPORTANCE = array(
         [
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
-        0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
+            0.0588,
         ]
     )
 
     STANDARD_SPEECH_SPECTRUM_NORMAL = array(
         [
             34.14,
             34.58,
@@ -292,15 +301,14 @@
             11.09,
             9.33,
             5.84,
             3.47,
         ]
     )
 
-
     REFERENCE_INTERNAL_NOISE_SPECTRUM = array(
         [
             -7.20,
             -8.90,
             -10.30,
             -11.40,
             -12.00,
@@ -317,303 +325,294 @@
             -24.20,
             -19.00,
         ]
     )
 
     FREEFIELD2EARDRUM_TRANSFER_FUNCTION = array(
         [
-        1.40,
-        1.40,
-        1.90,
-        2.80,
-        3.00,
-        2.60,
-        2.60,
-        3.60,
-        6.10,
-        10.50,
-        13.80,
-        16.80,
-        15.80,
-        14.90,
-        14.30,
-        12.40,
-        7.90,
+            1.40,
+            1.40,
+            1.90,
+            2.80,
+            3.00,
+            2.60,
+            2.60,
+            3.60,
+            6.10,
+            10.50,
+            13.80,
+            16.80,
+            15.80,
+            14.90,
+            14.30,
+            12.40,
+            7.90,
         ]
     )
-    return CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, IMPORTANCE, REFERENCE_INTERNAL_NOISE_SPECTRUM, STANDARD_SPEECH_SPECTRUM_NORMAL
+    return (
+        CENTER_FREQUENCIES,
+        LOWER_FREQUENCIES,
+        UPPER_FREQUENCIES,
+        IMPORTANCE,
+        REFERENCE_INTERNAL_NOISE_SPECTRUM,
+        STANDARD_SPEECH_SPECTRUM_NORMAL,
+    )
+
 
 def _get_octave_band_data():
     CENTER_FREQUENCIES = array(
         [
-        250,
-        500,
-        1000,
-        2000,
-        4000,
-        8000,
+            250,
+            500,
+            1000,
+            2000,
+            4000,
+            8000,
         ]
     )
 
     LOWER_FREQUENCIES = array(
         [
-        177,
-        355,
-        710,
-        1420,
-        2840,
-        5680,
+            177,
+            355,
+            710,
+            1420,
+            2840,
+            5680,
         ]
     )
 
     UPPER_FREQUENCIES = array(
         [
-        355,
-        710,
-        1420,
-        2840,
-        5680,
-        11360,
+            355,
+            710,
+            1420,
+            2840,
+            5680,
+            11360,
         ]
     )
 
     BANDWIDTH_ADJUSTEMENT = array(
         [
-        22.48,
-        25.48,
-        28.48,
-        31.48,
-        34.48,
-        37.48,
-        ]
-    )    
-
-
-    IMPORTANCE = array(
-        [
-        0.0617,
-        0.1671,
-        0.2373,
-        0.2648,
-        0.2142,
-        0.0549
+            22.48,
+            25.48,
+            28.48,
+            31.48,
+            34.48,
+            37.48,
         ]
     )
 
-    STANDARD_SPEECH_SPECTRUM_NORMAL = array(
-        [
-        34.75,
-        34.27,
-        25.01,
-        17.32,
-        9.33,
-        1.13
-        ]
-    )
+    IMPORTANCE = array([0.0617, 0.1671, 0.2373, 0.2648, 0.2142, 0.0549])
+
+    STANDARD_SPEECH_SPECTRUM_NORMAL = array([34.75, 34.27, 25.01, 17.32, 9.33, 1.13])
 
     REFERENCE_INTERNAL_NOISE_SPECTRUM = array(
-        [
-        -3.90,
-        -9.70,
-        -12.50,
-        -17.70,
-        -25.90,
-        -7.10
-        ]
+        [-3.90, -9.70, -12.50, -17.70, -25.90, -7.10]
     )
 
-    FREEFIELD2EARDRUM_TRANSFER_FUNCTION = array(
-        [
-        1.00,
-        1.80,
-        2.60,
-        12.00,
-        14.30,
-        1.80
-        ]
+    FREEFIELD2EARDRUM_TRANSFER_FUNCTION = array([1.00, 1.80, 2.60, 12.00, 14.30, 1.80])
+    return (
+        CENTER_FREQUENCIES,
+        LOWER_FREQUENCIES,
+        UPPER_FREQUENCIES,
+        BANDWIDTH_ADJUSTEMENT,
+        IMPORTANCE,
+        REFERENCE_INTERNAL_NOISE_SPECTRUM,
+        STANDARD_SPEECH_SPECTRUM_NORMAL,
     )
-    return CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, BANDWIDTH_ADJUSTEMENT, IMPORTANCE, REFERENCE_INTERNAL_NOISE_SPECTRUM, STANDARD_SPEECH_SPECTRUM_NORMAL
+
 
 def _get_third_octave_band_data():
     CENTER_FREQUENCIES = array(
         [
-        160,
-        200,
-        250,
-        315,
-        400,
-        500,
-        630,
-        800,
-        1000,
-        1250,
-        1600,
-        2000,
-        2500,
-        3150,
-        4000,
-        5000,
-        6300,
-        8000
+            160,
+            200,
+            250,
+            315,
+            400,
+            500,
+            630,
+            800,
+            1000,
+            1250,
+            1600,
+            2000,
+            2500,
+            3150,
+            4000,
+            5000,
+            6300,
+            8000,
         ]
-        )
+    )
 
     LOWER_FREQUENCIES = array(
         [
-        141,
-        178,
-        224,
-        282,
-        355,
-        447,
-        562,
-        708,
-        891,
-        1122,
-        1413,
-        1778,
-        2239,
-        2818,
-        3548,
-        4467,
-        5623,
-        7079,
+            141,
+            178,
+            224,
+            282,
+            355,
+            447,
+            562,
+            708,
+            891,
+            1122,
+            1413,
+            1778,
+            2239,
+            2818,
+            3548,
+            4467,
+            5623,
+            7079,
         ]
-        )
+    )
 
     UPPER_FREQUENCIES = array(
         [
-        178,
-        224,
-        282,
-        355,
-        447,
-        562,
-        708,
-        891,
-        1122,
-        1413,
-        1778,
-        2239,
-        2818,
-        3548,
-        4467,
-        5623,
-        7079,
-        8913,
+            178,
+            224,
+            282,
+            355,
+            447,
+            562,
+            708,
+            891,
+            1122,
+            1413,
+            1778,
+            2239,
+            2818,
+            3548,
+            4467,
+            5623,
+            7079,
+            8913,
         ]
-        )
+    )
 
     BANDWIDTH_ADJUSTEMENT = array(
         [
-        15.65,
-        16.65,
-        17.65,
-        18.65,
-        19.65,
-        20.65,
-        21.65,
-        22.65,
-        23.65,
-        24.65,
-        25.65,
-        26.65,
-        27.65,
-        28.65,
-        29.65,
-        30.65,
-        31.65,
-        32.65,
+            15.65,
+            16.65,
+            17.65,
+            18.65,
+            19.65,
+            20.65,
+            21.65,
+            22.65,
+            23.65,
+            24.65,
+            25.65,
+            26.65,
+            27.65,
+            28.65,
+            29.65,
+            30.65,
+            31.65,
+            32.65,
         ]
-    )    
+    )
 
     IMPORTANCE = array(
         [
-        0.0083,
-        0.0095,
-        0.0150,
-        0.0289,
-        0.0440,
-        0.0578,
-        0.0653,
-        0.0711,
-        0.0818,
-        0.0844,
-        0.0882,
-        0.0898,
-        0.0868,
-        0.0844,
-        0.0771,
-        0.0527,
-        0.0364,
-        0.0185,
+            0.0083,
+            0.0095,
+            0.0150,
+            0.0289,
+            0.0440,
+            0.0578,
+            0.0653,
+            0.0711,
+            0.0818,
+            0.0844,
+            0.0882,
+            0.0898,
+            0.0868,
+            0.0844,
+            0.0771,
+            0.0527,
+            0.0364,
+            0.0185,
         ]
     )
 
-    STANDARD_SPEECH_SPECTRUM_NORMAL = array (
-        [
-        32.41,
-        34.48,
-        34.75,
-        33.98,
-        34.59,
-        34.27,
-        32.06,
-        28.30,
-        25.01,
-        23.00,
-        20.15,
-        17.32,
-        13.18,
-        11.55,
-        9.33,
-        5.31,
-        2.59,
-        1.13    ]
+    STANDARD_SPEECH_SPECTRUM_NORMAL = array(
+        [
+            32.41,
+            34.48,
+            34.75,
+            33.98,
+            34.59,
+            34.27,
+            32.06,
+            28.30,
+            25.01,
+            23.00,
+            20.15,
+            17.32,
+            13.18,
+            11.55,
+            9.33,
+            5.31,
+            2.59,
+            1.13,
+        ]
     )
 
     REFERENCE_INTERNAL_NOISE_SPECTRUM = array(
         [
-        0.60,
-        -1.70,
-        -3.90,
-        -6.10,
-        -8.20,
-        -9.70,
-        -10.80,
-        -11.90,
-        -12.50,
-        -13.50,
-        -15.40,
-        -17.70,
-        -21.20,
-        -24.20,
-        -25.90,
-        -23.60,
-        -15.80,
-        -7.10
+            0.60,
+            -1.70,
+            -3.90,
+            -6.10,
+            -8.20,
+            -9.70,
+            -10.80,
+            -11.90,
+            -12.50,
+            -13.50,
+            -15.40,
+            -17.70,
+            -21.20,
+            -24.20,
+            -25.90,
+            -23.60,
+            -15.80,
+            -7.10,
         ]
     )
 
     FREEFIELD2EARDRUM_TRANSFER_FUNCTION = array(
         [
-        0.00,
-        0.50,
-        1.00,
-        1.40,
-        1.50,
-        1.80,
-        2.40,
-        3.10,
-        2.60,
-        3.00,
-        6.10,
-        12.00,
-        16.80,
-        15.00,
-        14.30,
-        10.70,
-        6.40,
-        1.80,
-        ]
+            0.00,
+            0.50,
+            1.00,
+            1.40,
+            1.50,
+            1.80,
+            2.40,
+            3.10,
+            2.60,
+            3.00,
+            6.10,
+            12.00,
+            16.80,
+            15.00,
+            14.30,
+            10.70,
+            6.40,
+            1.80,
+        ]
+    )
+    return (
+        CENTER_FREQUENCIES,
+        LOWER_FREQUENCIES,
+        UPPER_FREQUENCIES,
+        BANDWIDTH_ADJUSTEMENT,
+        IMPORTANCE,
+        REFERENCE_INTERNAL_NOISE_SPECTRUM,
+        STANDARD_SPEECH_SPECTRUM_NORMAL,
     )
-    return CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, BANDWIDTH_ADJUSTEMENT, IMPORTANCE, REFERENCE_INTERNAL_NOISE_SPECTRUM, STANDARD_SPEECH_SPECTRUM_NORMAL
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_main_sii.py` & `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_main_sii.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # -*- coding: utf-8 -*-
 
 
 from numpy import array, zeros, log10, maximum, where, sum
 
-from mosqito.sq_metrics.speech_intelligibility.sii_ansi._band_procedure_data import _get_critical_band_data, _get_equal_critical_band_data, _get_octave_band_data, _get_third_octave_band_data
-from mosqito.sq_metrics.speech_intelligibility.sii_ansi._speech_data import _get_critical_band_speech_data, _get_equal_critical_band_speech_data, _get_octave_band_speech_data, _get_third_octave_band_speech_data
+from mosqito.sq_metrics.speech_intelligibility.sii_ansi._band_procedure_data import (
+    _get_critical_band_data,
+    _get_equal_critical_band_data,
+    _get_octave_band_data,
+    _get_third_octave_band_data,
+)
+from mosqito.sq_metrics.speech_intelligibility.sii_ansi._speech_data import (
+    _get_critical_band_speech_data,
+    _get_equal_critical_band_speech_data,
+    _get_octave_band_speech_data,
+    _get_third_octave_band_speech_data,
+)
 from mosqito.utils.LTQ import LTQ
-from mosqito.utils.conversion import freq2bark
+from mosqito.utils import freq2bark
 
 
 def _main_sii(method, speech_spectrum, noise_spectrum, threshold):
     """Calculate core speech intelligibility index
 
     This function computes SII values based on ANSI S3.5 standard.
 
@@ -21,91 +31,144 @@
     speech_spectrum : array_like
         Speech spectrum [dB ref. 2e-5 Pa] with same size as the chosen method frequency axis.
     noise_spectrum : array_like
         Noise spectrum [dB ref. 2e-5 Pa] with same size as the chosen method frequency axis.
     threshold : array_like or 'zwicker'
         Threshold of hearing [dB ref. 2e-5 Pa] with same size as the chosen method frequency axis, or 'zwicker' to use the standard threshold.
         Default to None sets the threshold to zeros on each frequency band.
-        
+
     Returns
     -------
     sii: numpy.ndarray
         Overall SII value.
     specific_sii: numpy.ndarray
         Specific SII values along the frequency axis.
     freq_axis: numpy.ndarray
         Frequency axis corresponding to the chosen method.
     """
-    
-    if (method!='critical') & (method!='equally_critical') & (method!='third_octave') & (method!='octave'):
-        raise ValueError('Method should be within {"critical", "equally_critical", "third_octave", "octave"}.')
-    
+
+    if (
+        (method != "critical")
+        & (method != "equally_critical")
+        & (method != "third_octave")
+        & (method != "octave")
+    ):
+        raise ValueError(
+            'Method should be within {"critical", "equally_critical", "third_octave", "octave"}.'
+        )
+
     # Get band data according to the chosen method
-    if method == 'critical':
-        CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, IMPORTANCE, REFERENCE_INTERNAL_NOISE_SPECTRUM, STANDARD_SPEECH_SPECTRUM_NORMAL = _get_critical_band_data()
-    elif method == 'equally_critical':
-        CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, IMPORTANCE, REFERENCE_INTERNAL_NOISE_SPECTRUM, STANDARD_SPEECH_SPECTRUM_NORMAL = _get_equal_critical_band_data()
-    elif method == 'third_octave':
-        CENTER_FREQUENCIES, _, _, _, IMPORTANCE, REFERENCE_INTERNAL_NOISE_SPECTRUM, STANDARD_SPEECH_SPECTRUM_NORMAL = _get_third_octave_band_data()
-    elif method == 'octave':
-        CENTER_FREQUENCIES, _, _, _, IMPORTANCE, REFERENCE_INTERNAL_NOISE_SPECTRUM, STANDARD_SPEECH_SPECTRUM_NORMAL = _get_octave_band_data()
+    if method == "critical":
+        (
+            CENTER_FREQUENCIES,
+            LOWER_FREQUENCIES,
+            UPPER_FREQUENCIES,
+            IMPORTANCE,
+            REFERENCE_INTERNAL_NOISE_SPECTRUM,
+            STANDARD_SPEECH_SPECTRUM_NORMAL,
+        ) = _get_critical_band_data()
+    elif method == "equally_critical":
+        (
+            CENTER_FREQUENCIES,
+            LOWER_FREQUENCIES,
+            UPPER_FREQUENCIES,
+            IMPORTANCE,
+            REFERENCE_INTERNAL_NOISE_SPECTRUM,
+            STANDARD_SPEECH_SPECTRUM_NORMAL,
+        ) = _get_equal_critical_band_data()
+    elif method == "third_octave":
+        (
+            CENTER_FREQUENCIES,
+            _,
+            _,
+            _,
+            IMPORTANCE,
+            REFERENCE_INTERNAL_NOISE_SPECTRUM,
+            STANDARD_SPEECH_SPECTRUM_NORMAL,
+        ) = _get_third_octave_band_data()
+    elif method == "octave":
+        (
+            CENTER_FREQUENCIES,
+            _,
+            _,
+            _,
+            IMPORTANCE,
+            REFERENCE_INTERNAL_NOISE_SPECTRUM,
+            STANDARD_SPEECH_SPECTRUM_NORMAL,
+        ) = _get_octave_band_data()
     nbands = len(CENTER_FREQUENCIES)
-    
+
     if threshold is None:
         T = zeros((nbands))
-    elif threshold == 'zwicker':
+    elif threshold == "zwicker":
         T = LTQ(freq2bark(CENTER_FREQUENCIES))
     else:
         T = array(threshold)
-        
+
     # dB bandwidth adjustement
-    if (method == 'critical_bands') or (method == 'equal_critical_bands'):
+    if (method == "critical_bands") or (method == "equal_critical_bands"):
         noise_spectrum -= 10 * log10(UPPER_FREQUENCIES - LOWER_FREQUENCIES)
 
     # STEP 3
-    if method == 'octave':
+    if method == "octave":
         Z = noise_spectrum
     else:
         V = speech_spectrum - 24
         B = maximum(noise_spectrum, V)
-        if method == 'third_octave':
-            C = -80 + 0.6 * (B + 10*log10(CENTER_FREQUENCIES)-6.353)
+        if method == "third_octave":
+            C = -80 + 0.6 * (B + 10 * log10(CENTER_FREQUENCIES) - 6.353)
             Z = zeros((nbands))
-            for i in range(nbands): 
+            for i in range(nbands):
                 s = 0
                 for k in range(i):
-                    s += 10**(0.1*(B[k] + 3.32 * C[k] * log10(0.89 * CENTER_FREQUENCIES[i] / CENTER_FREQUENCIES[k])))
-                Z[i] = 10 * log10(10**(0.1*noise_spectrum[i]) + s)
+                    s += 10 ** (
+                        0.1
+                        * (
+                            B[k]
+                            + 3.32
+                            * C[k]
+                            * log10(
+                                0.89 * CENTER_FREQUENCIES[i] / CENTER_FREQUENCIES[k]
+                            )
+                        )
+                    )
+                Z[i] = 10 * log10(10 ** (0.1 * noise_spectrum[i]) + s)
         else:
-            C = -80 + 0.6 * (B + 10*log10(UPPER_FREQUENCIES - LOWER_FREQUENCIES))
+            C = -80 + 0.6 * (B + 10 * log10(UPPER_FREQUENCIES - LOWER_FREQUENCIES))
             Z = zeros((nbands))
-            for i in range(nbands): 
+            for i in range(nbands):
                 s = 0
-                for k in range(i-1):
-                    s += 10**(0.1*(B[k] + 3.32 * C[k] * log10(CENTER_FREQUENCIES[i] / CENTER_FREQUENCIES[k])))                    
-                Z[i] = 10 * log10(10**(0.1*noise_spectrum[i]) + s)
+                for k in range(i - 1):
+                    s += 10 ** (
+                        0.1
+                        * (
+                            B[k]
+                            + 3.32
+                            * C[k]
+                            * log10(CENTER_FREQUENCIES[i] / CENTER_FREQUENCIES[k])
+                        )
+                    )
+                Z[i] = 10 * log10(10 ** (0.1 * noise_spectrum[i]) + s)
         # 4.3.2.4
         Z[0] = B[0]
-    
+
     # STEP 4
     X = REFERENCE_INTERNAL_NOISE_SPECTRUM + T
-    
+
     # STEP 5
     D = maximum(Z, X)
-    
+
     # STEP 6
-    L = 1 - (speech_spectrum - STANDARD_SPEECH_SPECTRUM_NORMAL -10)/160
-    L[where(L>1)] = 1
-    
+    L = 1 - (speech_spectrum - STANDARD_SPEECH_SPECTRUM_NORMAL - 10) / 160
+    L[where(L > 1)] = 1
+
     # STEP 7
-    K = (speech_spectrum - D + 15)/30
-    K[where(K>1)] = 1
-    K[where(K<0)] = 0
+    K = (speech_spectrum - D + 15) / 30
+    K[where(K > 1)] = 1
+    K[where(K < 0)] = 0
     A = L * K
-    
+
     # STEP 8
     SII = sum(IMPORTANCE * A)
     SII_specific = IMPORTANCE * A
-    
-    return SII, SII_specific, CENTER_FREQUENCIES
-
 
+    return SII, SII_specific, CENTER_FREQUENCIES
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_speech_data.py` & `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_speech_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,383 +1,365 @@
 from numpy import array
 
+
 def _get_critical_band_speech_data(speech_level):
-    """ See § 3.4 of the standard ANSI S3.5. """
-    
+    """See § 3.4 of the standard ANSI S3.5."""
+
     if speech_level == "normal":
         SPEECH_SPECTRUM = array(
-        [
-            31.44,
-            34.75,
-            34.14,
-            34.58,
-            33.17,
-            30.64,
-            27.59,
-            25.01,
-            23.52,
-            22.28,
-            20.15,
-            18.29,
-            16.37,
-            13.80,
-            12.21,
-            11.09,
-            9.33,
-            5.84,
-            3.47,
-            1.78,
-            -0.14
-        ])
+            [
+                31.44,
+                34.75,
+                34.14,
+                34.58,
+                33.17,
+                30.64,
+                27.59,
+                25.01,
+                23.52,
+                22.28,
+                20.15,
+                18.29,
+                16.37,
+                13.80,
+                12.21,
+                11.09,
+                9.33,
+                5.84,
+                3.47,
+                1.78,
+                -0.14,
+            ]
+        )
         SPEECH_LEVEL = 62.35
     elif speech_level == "raised":
         SPEECH_SPECTRUM = array(
             [
-            34.06,
-            38.98,
-            38.62,
-            39.84,
-            39.44,
-            37.99,
-            35.85,
-            33.86,
-            32.56,
-            30.91,
-            28.58,
-            26.37,
-            24.34,
-            22.35,
-            21.04,
-            19.56,
-            16.78,
-            12.14,
-            9.04,
-            6.36,
-            3.44
-            ])
+                34.06,
+                38.98,
+                38.62,
+                39.84,
+                39.44,
+                37.99,
+                35.85,
+                33.86,
+                32.56,
+                30.91,
+                28.58,
+                26.37,
+                24.34,
+                22.35,
+                21.04,
+                19.56,
+                16.78,
+                12.14,
+                9.04,
+                6.36,
+                3.44,
+            ]
+        )
         SPEECH_LEVEL = 68.34
     elif speech_level == "loud":
 
         SPEECH_SPECTRUM = array(
             [
-            34.21,
-            41.55,
-            43.68,
-            44.08,
-            45.34,
-            45.22,
-            43.60,
-            42.16,
-            41.07,
-            39.68,
-            37.70,
-            35.62,
-            33.17,
-            30.98,
-            29.01,
-            27.71,
-            25.41,
-            19.20,
-            15.37,
-            12.61,
-            9.62
-            ])
+                34.21,
+                41.55,
+                43.68,
+                44.08,
+                45.34,
+                45.22,
+                43.60,
+                42.16,
+                41.07,
+                39.68,
+                37.70,
+                35.62,
+                33.17,
+                30.98,
+                29.01,
+                27.71,
+                25.41,
+                19.20,
+                15.37,
+                12.61,
+                9.62,
+            ]
+        )
         SPEECH_LEVEL = 74.85
     elif speech_level == "shout":
         SPEECH_SPECTRUM = array(
-        [
-        28.69,
-        42.50,
-        47.14,
-        48.46,
-        50.17,
-        51.68,
-        51.43,
-        51.31,
-        49.40,
-        49.03,
-        47.65,
-        45.47,
-        43.13,
-        40.80,
-        39.15,
-        37.30,
-        34.41,
-        29.01,
-        25.17,
-        22.08,
-        18.76
-        ])
+            [
+                28.69,
+                42.50,
+                47.14,
+                48.46,
+                50.17,
+                51.68,
+                51.43,
+                51.31,
+                49.40,
+                49.03,
+                47.65,
+                45.47,
+                43.13,
+                40.80,
+                39.15,
+                37.30,
+                34.41,
+                29.01,
+                25.17,
+                22.08,
+                18.76,
+            ]
+        )
         SPEECH_LEVEL = 82.30
     else:
-        raise ValueError("Error: available speech levels are {'normal', 'raised', 'loud', 'shout'}")
+        raise ValueError(
+            "Error: available speech levels are {'normal', 'raised', 'loud', 'shout'}"
+        )
 
     return SPEECH_SPECTRUM, SPEECH_LEVEL
 
+
 def _get_equal_critical_band_speech_data(speech_level):
     if speech_level == "normal":
         SPEECH_SPECTRUM = array(
-        [
-            34.14,
-            34.58,
-            33.17,
-            30.64,
-            27.59,
-            25.01,
-            23.52,
-            22.28,
-            20.15,
-            18.29,
-            16.37,
-            13.80,
-            12.21,
-            11.09,
-            9.33,
-            5.84,
-            3.47,
-        ]
-    )
+            [
+                34.14,
+                34.58,
+                33.17,
+                30.64,
+                27.59,
+                25.01,
+                23.52,
+                22.28,
+                20.15,
+                18.29,
+                16.37,
+                13.80,
+                12.21,
+                11.09,
+                9.33,
+                5.84,
+                3.47,
+            ]
+        )
         SPEECH_LEVEL = 62.35
     elif speech_level == "raised":
         SPEECH_SPECTRUM = array(
-        [
-        38.62,
-        39.84,
-        39.44,
-        37.99,
-        35.85,
-        33.86,
-        32.56,
-        30.91,
-        28.58,
-        26.37,
-        24.34,
-        22.35,
-        21.04,
-        19.56,
-        16.78,
-        12.14,
-        9.04,
-        ]
-    )
+            [
+                38.62,
+                39.84,
+                39.44,
+                37.99,
+                35.85,
+                33.86,
+                32.56,
+                30.91,
+                28.58,
+                26.37,
+                24.34,
+                22.35,
+                21.04,
+                19.56,
+                16.78,
+                12.14,
+                9.04,
+            ]
+        )
         SPEECH_LEVEL = 68.34
     elif speech_level == "loud":
         SPEECH_SPECTRUM = array(
-        [
-        43.68,
-        44.08,
-        45.34,
-        45.22,
-        43.60,
-        42.16,
-        41.07,
-        39.68,
-        37.70,
-        35.62,
-        33.17,
-        30.98,
-        29.01,
-        27.71,
-        25.41,
-        19.20,
-        15.37,
-        ]
-    )
+            [
+                43.68,
+                44.08,
+                45.34,
+                45.22,
+                43.60,
+                42.16,
+                41.07,
+                39.68,
+                37.70,
+                35.62,
+                33.17,
+                30.98,
+                29.01,
+                27.71,
+                25.41,
+                19.20,
+                15.37,
+            ]
+        )
         SPEECH_LEVEL = 74.85
     elif speech_level == "shout":
         SPEECH_SPECTRUM = array(
-        [
-        47.14,
-        48.46,
-        50.17,
-        51.68,
-        51.43,
-        51.31,
-        49.40,
-        49.03,
-        47.65,
-        45.47,
-        43.13,
-        40.80,
-        39.15,
-        37.30,
-        34.41,
-        29.01,
-        25.17,
-        ]
-    )
+            [
+                47.14,
+                48.46,
+                50.17,
+                51.68,
+                51.43,
+                51.31,
+                49.40,
+                49.03,
+                47.65,
+                45.47,
+                43.13,
+                40.80,
+                39.15,
+                37.30,
+                34.41,
+                29.01,
+                25.17,
+            ]
+        )
         SPEECH_LEVEL = 82.30
     else:
-        raise ValueError("Error: Available speech levels are {'normal', 'raised', 'loud', 'shout'}")
+        raise ValueError(
+            "Error: Available speech levels are {'normal', 'raised', 'loud', 'shout'}"
+        )
 
     return SPEECH_SPECTRUM, SPEECH_LEVEL
 
+
 def _get_octave_band_speech_data(speech_level):
 
     if speech_level == "normal":
-        SPEECH_SPECTRUM = array(
-        [
-        34.75,
-        34.27,
-        25.01,
-        17.32,
-        9.33,
-        1.13
-        ]
-    )
+        SPEECH_SPECTRUM = array([34.75, 34.27, 25.01, 17.32, 9.33, 1.13])
         SPEECH_LEVEL = 62.35
     elif speech_level == "raised":
-        SPEECH_SPECTRUM = array(
-        [
-        38.98,
-        40.15,
-        33.86,
-        25.32,
-        16.78,
-        5.07
-        ]
-    )
+        SPEECH_SPECTRUM = array([38.98, 40.15, 33.86, 25.32, 16.78, 5.07])
 
         SPEECH_LEVEL = 68.34
     elif speech_level == "loud":
-        SPEECH_SPECTRUM = array(
-        [
-        41.55,
-        44.85,
-        42.16,
-        34.39,
-        25.41,
-        11.39
-        ]
-    )
+        SPEECH_SPECTRUM = array([41.55, 44.85, 42.16, 34.39, 25.41, 11.39])
         SPEECH_LEVEL = 74.85
     elif speech_level == "shout":
-        SPEECH_SPECTRUM = array(
-        [
-        42.50,
-        49.24,
-        51.31,
-        44.32,
-        34.41,
-        20.72
-        ]
-    )
+        SPEECH_SPECTRUM = array([42.50, 49.24, 51.31, 44.32, 34.41, 20.72])
         SPEECH_LEVEL = 82.30
     else:
-        raise ValueError("Error: Available speech levels are {'normal', 'raised', 'loud', 'shout'}")
+        raise ValueError(
+            "Error: Available speech levels are {'normal', 'raised', 'loud', 'shout'}"
+        )
 
     return SPEECH_SPECTRUM, SPEECH_LEVEL
 
+
 def _get_third_octave_band_speech_data(speech_level):
     if speech_level == "normal":
         SPEECH_SPECTRUM = array(
-        [
-        32.41,
-        34.48,
-        34.75,
-        33.98,
-        34.59,
-        34.27,
-        32.06,
-        28.30,
-        25.01,
-        23.00,
-        20.15,
-        17.32,
-        13.18,
-        11.55,
-        9.33,
-        5.31,
-        2.59,
-        1.13    ]
-    )
+            [
+                32.41,
+                34.48,
+                34.75,
+                33.98,
+                34.59,
+                34.27,
+                32.06,
+                28.30,
+                25.01,
+                23.00,
+                20.15,
+                17.32,
+                13.18,
+                11.55,
+                9.33,
+                5.31,
+                2.59,
+                1.13,
+            ]
+        )
         SPEECH_LEVEL = 62.35
     elif speech_level == "raised":
         SPEECH_SPECTRUM = array(
-        [
-        33.81,
-        33.92,
-        38.98,
-        38.57,
-        39.11,
-        40.15,
-        38.78,
-        36.37,
-        33.86,
-        31.89,
-        28.58,
-        25.32,
-        22.35,
-        20.15,
-        16.78,
-        11.47,
-        7.67,
-        5.07
-        ]
-    )
+            [
+                33.81,
+                33.92,
+                38.98,
+                38.57,
+                39.11,
+                40.15,
+                38.78,
+                36.37,
+                33.86,
+                31.89,
+                28.58,
+                25.32,
+                22.35,
+                20.15,
+                16.78,
+                11.47,
+                7.67,
+                5.07,
+            ]
+        )
         SPEECH_LEVEL = 68.34
     elif speech_level == "loud":
         SPEECH_SPECTRUM = array(
-        [
-        35.29,
-        37.76,
-        41.55,
-        43.78,
-        43.40,
-        44.85,
-        45.55,
-        44.05,
-        42.16,
-        40.53,
-        37.70,
-        34.39,
-        30.98,
-        28.21,
-        25.41,
-        18.35,
-        13.87,
-        11.39,
-        ]
-    )
+            [
+                35.29,
+                37.76,
+                41.55,
+                43.78,
+                43.40,
+                44.85,
+                45.55,
+                44.05,
+                42.16,
+                40.53,
+                37.70,
+                34.39,
+                30.98,
+                28.21,
+                25.41,
+                18.35,
+                13.87,
+                11.39,
+            ]
+        )
         SPEECH_LEVEL = 74.85
     elif speech_level == "shout":
         SPEECH_SPECTRUM = array(
-        [
-        30.77,
-        36.65,
-        42.50,
-        46.51,
-        47.40,
-        49.24,
-        51.21,
-        51.44,
-        51.31,
-        49.63,
-        47.65,
-        44.32,
-        40.80,
-        38.13,
-        34.41,
-        28.24,
-        23.45,
-        20.72,
-        ]
-    )
+            [
+                30.77,
+                36.65,
+                42.50,
+                46.51,
+                47.40,
+                49.24,
+                51.21,
+                51.44,
+                51.31,
+                49.63,
+                47.65,
+                44.32,
+                40.80,
+                38.13,
+                34.41,
+                28.24,
+                23.45,
+                20.72,
+            ]
+        )
         SPEECH_LEVEL = 82.30
     else:
-        raise ValueError("Error: Available speech levels are {'normal', 'raised', 'loud', 'shout'}")
-    
+        raise ValueError(
+            "Error: Available speech levels are {'normal', 'raised', 'loud', 'shout'}"
+        )
+
     return SPEECH_SPECTRUM, SPEECH_LEVEL
 
+
 if __name__ == "__main__":
-    
+
     speech_level = "normal"
     speech_spectrum, _ = _get_critical_band_speech_data(speech_level)
     print(len(speech_spectrum))
     speech_spectrum, _ = _get_equal_critical_band_speech_data(speech_level)
     print(len(speech_spectrum))
     speech_spectrum, _ = _get_third_octave_band_speech_data(speech_level)
     print(len(speech_spectrum))
     speech_spectrum, _ = _get_octave_band_speech_data(speech_level)
     print(len(speech_spectrum))
-    
-    print('done')
+
+    print("done")
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi.py` & `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_freq.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,168 @@
 # -*- coding: utf-8 -*-
 
-from numpy import array, zeros
-
-from mosqito.sq_metrics.speech_intelligibility.sii_ansi._band_procedure_data import _get_critical_band_data, _get_equal_critical_band_data, _get_octave_band_data, _get_third_octave_band_data
-from mosqito.sq_metrics.speech_intelligibility.sii_ansi._speech_data import _get_critical_band_speech_data, _get_equal_critical_band_speech_data, _get_octave_band_speech_data, _get_third_octave_band_speech_data
+from mosqito.sq_metrics.speech_intelligibility.sii_ansi._band_procedure_data import (
+    _get_critical_band_data,
+    _get_equal_critical_band_data,
+    _get_octave_band_data,
+    _get_third_octave_band_data,
+)
+from mosqito.sq_metrics.speech_intelligibility.sii_ansi._speech_data import (
+    _get_critical_band_speech_data,
+    _get_equal_critical_band_speech_data,
+    _get_octave_band_speech_data,
+    _get_third_octave_band_speech_data,
+)
 from mosqito.sq_metrics.speech_intelligibility.sii_ansi._main_sii import _main_sii
-from mosqito.sound_level_meter.spectrum import spectrum
+
 from mosqito.sound_level_meter.freq_band_synthesis import freq_band_synthesis
 
 
-def sii_ansi(noise, fs, method, speech_level, threshold=None):
+def sii_ansi_freq(spectrum, freqs, method, speech_level, threshold=None):
     """Calculate speech intelligibility index
 
-    This function computes SII values for a noise time signal according to ANSI S3.5 standard.
+    This function computes SII values for a noise spectrum in dB according to ANSI S3.5 standard.
 
     Parameters
     ----------
-    noise : array_like
-        Noise time signal in [Pa].
-    fs: float
-        Sampling frequency of the input noise signal.
+    spectrum : array_like
+        Noise spectrum [dB ref. 2e-5 Pa].
+    freqs: array_like
+        Frequency axis [Hz] of the spectrum.
     method: {"critical", "equally_critical", "third_octave", "octave"}
         Type of frequency band to be used for the calculation. See § 3.4 of the standard.
     speech_level : {'normal', 'raised', 'loud', 'shout'}
         Speech level to assess, the corresponding speech spectrum defined in the standard is used for calculation.
     threshold : array_like or 'zwicker'
         Threshold of hearing [dB ref. 2e-5 Pa] with same size as the chosen method frequency axis, or 'zwicker' to use the standard threshold.
         Default to None sets the threshold to zeros on each frequency band.
-        
+
     Returns
     -------
     sii: numpy.ndarray
         Overall SII value.
     specific_sii: numpy.ndarray
         Specific SII values along the frequency axis.
     freq_axis: numpy.ndarray
         Frequency axis corresponding to the chosen method.
-        
+
+    See also
+    --------
+    .sii_ansi : Speech intelligibility with a time signal as background noise
+    .sii_ansi_level : Speech intelligibility with an overall SPL level as background noise
+
+    Warning
+    -------
+    Input spectrum must be provided in dB.
+    
+    Notes
+    -----
+    The Speech Intelligibility Index :math:`SII` of the signal is computed as the sum of the speech-to-noise ratio :math:`A` weighted by an importance function :math:`I`, 
+    over the :math:`n` frequency bands. 
+    
+    .. math::
+        SII=\\sum_{i=1}^{n}A_{i}I_{i}
+    
+    The number of frequency bands considered depends on the chosen method:
+      * "critical": 21 critical bands corresponding to the Bark scale
+      * "equally_critical": 17 equally contributing critical bands
+      * "third-octave": 18 third-octave bands
+      * "octave": 6 octave bands
+
+    
+    References
+    ----------
+    :cite:empty:`SII-ANSI.S3.5:2017`
+    
+    .. bibliography::
+        :keyprefix: SII-
+
     Examples
     --------
     .. plot::
        :include-source:
 
-        >>> from mosqito.sq_metrics.speech_intelligibility import sii
+        >>> from mosqito.sq_metrics import sii_ansi_freq
+        >>> from mosqito.sound_level_meter.comp_spectrum import comp_spectrum
         >>> import matplotlib.pyplot as plt
         >>> import numpy as np
         >>> fs=48000
         >>> d=0.2
-        >>> dB=90
+        >>> dB=60
         >>> time = np.arange(0, d, 1/fs)
         >>> f = 50
         >>> stimulus = np.sin(2 * np.pi * f * time) * np.sin(np.pi * f * time) + np.sin(10 * np.pi * f * time) + np.sin(100 * np.pi * f * time)
         >>> rms = np.sqrt(np.mean(np.power(stimulus, 2)))
         >>> ampl = 0.00002 * np.power(10, dB / 20) / rms
         >>> stimulus = stimulus * ampl
-        >>> SII, SII_spec, freq_axis = sii(stimulus, fs, method='critical', speech_level='normal')
+        >>> spec, freqs = comp_spectrum(stimulus, fs, db=True)
+        >>> SII, SII_spec, freq_axis = sii_ansi_freq(spec, freqs, method='critical', speech_level='normal')
         >>> plt.plot(freq_axis, SII_spec)
         >>> plt.xlabel("Frequency [Hz]")
         >>> plt.ylabel("Specific value ")
-        >>> plt.title("Speech Intelligibility Index = " + f"{SII:.2f}")   
-        
+        >>> plt.title("Speech Intelligibility Index = " + f"{SII:.2f}")
+
     """
-    
-    if (method!='critical') & (method!='equally_critical') & (method!='third_octave') & (method!='octave'):
-        raise ValueError('Method should be within {"critical", "equally_critical", "third_octave", "octave"}.')
-        
-    if (speech_level!='normal') & (speech_level!='raised') & (speech_level!='loud') & (speech_level!='shout'):
-        raise ValueError('Speech level should be within {"normal", "raised", "loud", "shout"} to use the corresponding standard data.')
-    
+
+    if (
+        (method != "critical")
+        & (method != "equally_critical")
+        & (method != "third_octave")
+        & (method != "octave")
+    ):
+        raise ValueError(
+            'Method should be within {"critical", "equally_critical", "third_octave", "octave"}.'
+        )
+
+    if (
+        (speech_level != "normal")
+        & (speech_level != "raised")
+        & (speech_level != "loud")
+        & (speech_level != "shout")
+    ):
+        raise ValueError(
+            'Speech level should be within {"normal", "raised", "loud", "shout"} to use the corresponding standard data.'
+        )
+
     # Get standard speech spectrum
-    if method == 'critical':
+    if method == "critical":
         speech_spectrum, speech_level = _get_critical_band_speech_data(speech_level)
-        CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, _, _, _ = _get_critical_band_data()
-    elif method == 'equally_critical':
-        speech_spectrum, speech_level = _get_equal_critical_band_speech_data(speech_level)
-        CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, _, _, _ = _get_equal_critical_band_data()
-    elif method == 'third_octave':
+        CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, _, _, _ = (
+            _get_critical_band_data()
+        )
+    elif method == "equally_critical":
+        speech_spectrum, speech_level = _get_equal_critical_band_speech_data(
+            speech_level
+        )
+        CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, _, _, _ = (
+            _get_equal_critical_band_data()
+        )
+    elif method == "third_octave":
         speech_spectrum, speech_level = _get_third_octave_band_speech_data(speech_level)
-        CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, _, _, _, _ = _get_third_octave_band_data()
-    elif method == 'octave':
+        CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, _, _, _, _ = (
+            _get_third_octave_band_data()
+        )
+    elif method == "octave":
         speech_spectrum, speech_level = _get_octave_band_speech_data(speech_level)
-        CENTER_FREQUENCIES, LOWER_FREQUENCIES, UPPER_FREQUENCIES, _, _, _, _, = _get_octave_band_data()
-    
-    # Compute noise spectrum in dB
-    spec, freqs = spectrum(noise, fs, nfft="default", window="blackman", db=True)
-    noise_spectrum, _ = freq_band_synthesis(spec, freqs, LOWER_FREQUENCIES, UPPER_FREQUENCIES)
-                
-    SII, SII_specific, freq_axis = _main_sii(method, speech_spectrum, noise_spectrum, threshold)    
-    
+        (
+            CENTER_FREQUENCIES,
+            LOWER_FREQUENCIES,
+            UPPER_FREQUENCIES,
+            _,
+            _,
+            _,
+            _,
+        ) = _get_octave_band_data()
+    nbands = len(speech_spectrum)
+
+    if (len(spectrum) != nbands) or (freqs != CENTER_FREQUENCIES).any():
+        noise_spectrum, _ = freq_band_synthesis(
+            spectrum, freqs, LOWER_FREQUENCIES, UPPER_FREQUENCIES
+        )
+    else:
+        noise_spectrum = spectrum
+
+    SII, SII_specific, freq_axis = _main_sii(
+        method, speech_spectrum, noise_spectrum, threshold
+    )
+
     return SII, SII_specific, freq_axis
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_level.py` & `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_level.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,146 @@
 # -*- coding: utf-8 -*-
 
 from numpy import ones, log10, power
 
-from mosqito.sq_metrics.speech_intelligibility.sii_ansi._band_procedure_data import _get_critical_band_data, _get_equal_critical_band_data, _get_octave_band_data, _get_third_octave_band_data
-from mosqito.sq_metrics.speech_intelligibility.sii_ansi._speech_data import _get_critical_band_speech_data, _get_equal_critical_band_speech_data, _get_octave_band_speech_data, _get_third_octave_band_speech_data
+from mosqito.sq_metrics.speech_intelligibility.sii_ansi._band_procedure_data import (
+    _get_critical_band_data,
+    _get_equal_critical_band_data,
+    _get_octave_band_data,
+    _get_third_octave_band_data,
+)
+from mosqito.sq_metrics.speech_intelligibility.sii_ansi._speech_data import (
+    _get_critical_band_speech_data,
+    _get_equal_critical_band_speech_data,
+    _get_octave_band_speech_data,
+    _get_third_octave_band_speech_data,
+)
 from mosqito.sq_metrics.speech_intelligibility.sii_ansi._main_sii import _main_sii
 
 
 def sii_ansi_level(noise_level, method, speech_level, threshold=None):
     """Calculate speech intelligibility index
 
     This function computes SII values for an overall noise level in dB according to ANSI S3.5 standard.
     This value is used to create a uniform noise spectrum, with the same deduced level on each frequency band.
 
     Parameters
     ----------
     noise_level : float
-        Overall noise level in [dB ref. 2e-5 Pa]. 
+        Overall noise level in [dB ref. 2e-5 Pa].
     method: {"critical", "equally_critical", "third_octave", "octave"}
         Type of frequency band to be used for the calculation. See § 3.4 of the standard.
     speech_level : {'normal', 'raised', 'loud', 'shout'}
         Speech level to assess, the corresponding speech spectrum defined in the standard is used for calculation.
     threshold : array_like or 'zwicker'
         Threshold of hearing [dB ref. 2e-5 Pa] with same size as the chosen method frequency axis, or 'zwicker' to use the standard threshold.
         Default to None sets the threshold to zeros on each frequency band.
-                
+
     Returns
     -------
     sii: numpy.ndarray
         Overall SII value.
     specific_sii: numpy.ndarray
         Specific SII values along the frequency axis.
     freq_axis: numpy.ndarray
         Frequency axis corresponding to the chosen method.
+
+    See also
+    --------
+    .sii_ansi : Speech intelligibility with a time signal as background noise
+    .sii_ansi_freq : Speech intelligibility with a frequency spectrum as background noise
+    
+    Notes
+    ------
+    The input dB level corresponds to the overall sound pressure level. It is used to create a full uniform spectrum with the following sound level on each of the N bands: 
+    
+    .. math::
+            L_{band}=10\\log_{10}\\left( \\frac{10^{\\frac{L_{overall}}{10}}}{N} \\right)
+        
+    The Speech Intelligibility Index :math:`SII` of the signal is computed as the sum of the speech-to-noise ratio :math:`A` weighted by an importance function :math:`I`, 
+    over the :math:`n` frequency bands. 
+    
+    .. math::
+        SII=\\sum_{i=1}^{n}A_{i}I_{i}
+    
+    The number of frequency bands considered depends on the chosen method:
+      * "critical": 21 critical bands corresponding to the Bark scale
+      * "equally_critical": 17 equally contributing critical bands
+      * "third-octave": 18 third-octave bands
+      * "octave": 6 octave bands
+        
+        
+    References
+    ----------
+    :cite:empty:`SII-ANSI.S3.5:2017`
+    
+    .. bibliography::
+        :keyprefix: SII-
         
     Examples
     --------
     .. plot::
        :include-source:
-       
+
         >>> import matplotlib.pyplot as plt
         >>> import numpy as np
-        >>> from mosqito.sq_metrics.speech_intelligibility import sii_level
+        >>> from mosqito.sq_metrics.speech_intelligibility import sii_ansi_level
         >>> fs=48000
         >>> d=0.2
         >>> dB=90
         >>> time = np.arange(0, d, 1/fs)
         >>> f = 50
         >>> stimulus = np.sin(2 * np.pi * f * time) * np.sin(np.pi * f * time) + np.sin(10 * np.pi * f * time) + np.sin(100 * np.pi * f * time)
         >>> rms = np.sqrt(np.mean(np.power(stimulus, 2)))
         >>> ampl = 0.00002 * np.power(10, dB / 20) / rms
         >>> stimulus = stimulus * ampl
         >>> speech_level = 'raised'
-        >>> SII, SII_spec, freq_axis = sii_level(60, method='critical', speech_level=speech_level, threshold='zwicker')
+        >>> SII, SII_spec, freq_axis = sii_ansi_level(60, method='critical', speech_level=speech_level, threshold='zwicker')
         >>> plt.plot(freq_axis, SII_spec)
         >>> plt.xlabel("Frequency [Hz]")
         >>> plt.ylabel("Specific value ")
-        >>> plt.title("Speech Intelligibility Index = " + f"{SII:.2f} \n Speech level: " + speech_level)   
-
+        >>> plt.title("Speech Intelligibility Index = " + f"{SII:.2f}")
     """
-    
-    if (method!='critical') & (method!='equally_critical') & (method!='third_octave') & (method!='octave'):
-        raise ValueError('Method should be within {"critical", "equally_critical", "third_octave", "octave"}.')
-        
-    if (speech_level!='normal') & (speech_level!='raised') & (speech_level!='loud') & (speech_level!='shout'):
-        raise ValueError('Speech level should be within {"normal", "raised", "loud", "shout"} to use the corresponding standard data.')
-    
+
+    if (
+        (method != "critical")
+        & (method != "equally_critical")
+        & (method != "third_octave")
+        & (method != "octave")
+    ):
+        raise ValueError(
+            'Method should be within {"critical", "equally_critical", "third_octave", "octave"}.'
+        )
+
+    if (
+        (speech_level != "normal")
+        & (speech_level != "raised")
+        & (speech_level != "loud")
+        & (speech_level != "shout")
+    ):
+        raise ValueError(
+            'Speech level should be within {"normal", "raised", "loud", "shout"} to use the corresponding standard data.'
+        )
+
     # Get standard speech spectrum
-    if method == 'critical':
+    if method == "critical":
         speech_spectrum, speech_level = _get_critical_band_speech_data(speech_level)
-    elif method == 'equally_critical':
-        speech_spectrum, speech_level = _get_equal_critical_band_speech_data(speech_level)
-    elif method == 'third_octave':
+    elif method == "equally_critical":
+        speech_spectrum, speech_level = _get_equal_critical_band_speech_data(
+            speech_level
+        )
+    elif method == "third_octave":
         speech_spectrum, speech_level = _get_third_octave_band_speech_data(speech_level)
-    elif method == 'octave':
+    elif method == "octave":
         speech_spectrum, speech_level = _get_octave_band_speech_data(speech_level)
     nbands = len(speech_spectrum)
-    
+
     # Create noise spectrum as uniform spectrum from overall level
-    band_level = 10 * log10(power(10, noise_level/10)/nbands)
+    band_level = 10 * log10(power(10, noise_level / 10) / nbands)
     noise_spectrum = ones((nbands)) * band_level
-        
+
     # Compute SII
-    SII, SII_specific, freq_axis = _main_sii(method, speech_spectrum, noise_spectrum, threshold)    
-    
-    return SII, SII_specific, freq_axis
+    SII, SII_specific, freq_axis = _main_sii(
+        method, speech_spectrum, noise_spectrum, threshold
+    )
 
+    return SII, SII_specific, freq_axis
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/_pr_main_calc.py` & `mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/_pr_main_calc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # -*- coding: utf-8 -*-
-
-import numpy as np
+from numpy import asarray, where, append, empty, array, argmin, log10, power, delete, abs
 
 # from scipy.signal import welch, periodogram
 
 # Local functions imports
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma._critical_band import (
     _critical_band,
     _lower_critical_band,
     _upper_critical_band,
 )
-from mosqito.sq_metrics.tonality.tone_to_noise_ecma._screening_for_tones import _screening_for_tones
-from mosqito.sq_metrics.tonality.tone_to_noise_ecma._find_highest_tone import _find_highest_tone
+from mosqito.sq_metrics.tonality.tone_to_noise_ecma._screening_for_tones import (
+    _screening_for_tones,
+)
+from mosqito.sq_metrics.tonality.tone_to_noise_ecma._find_highest_tone import (
+    _find_highest_tone,
+)
 
 
 def _pr_main_calc(spectrum_db, freq_axis):
     """
         Calculation of the tone-to noise ratio according to the method described
         in ECMA 74, annex D.
         The method to find the tonal candidates is the one described by Wade Bray
         in 'Methods for automating prominent tone evaluation and for considerin
         variations with time or other reference quantities'
         The total value calculated, T-PR, is calculated according to ECMA TR/108
 
     Parameters
     ----------
     spectrum_db : array
-        Spectrum values in dB [nperseg x nseg]
+        Spectrum values in dB (nperseg x nseg)
     freq_axis : array
-        frequency axis corresponding to the spectrum [nperseg x nseg]
+        frequency axis corresponding to the spectrum (nperseg x nseg)
 
     Output
     ------
     tones_freqs : array of float
         Frequency list of the tones [number of tones x nseg]
     pr : array of float
         TNR value calculated for each tone [number of tones x nseg]
@@ -43,39 +46,40 @@
     """
 
     #### Spectrum creation #######################################################
 
     if len(spectrum_db.shape) == 1:
         nseg = 1
         # Frequency axis of interest
-        freq_index = np.where((freq_axis > 89.1) & (freq_axis < 11200))[0]
+        freq_index = where((freq_axis > 89.1) & (freq_axis < 11200))[0]
         freqs = freq_axis[freq_index]
         spec_db = spectrum_db[freq_index]
 
     elif (len(spectrum_db.shape) > 1) & (len(freq_axis.shape) > 1):
         nseg = spectrum_db.shape[1]
-        freqs = [[]for i in range(nseg)]
-        spec_db = [[]for i in range(nseg)]
+        freqs = [[] for i in range(nseg)]
+        spec_db = [[] for i in range(nseg)]
         for i in range(nseg):
             # Frequency axis of interest
-            freq_index_rows = np.where(
-                (freq_axis[:, i] > 89.1) & (freq_axis[:, i] < 11200))[0]
-            freqs[i] = np.append(freqs[i], freq_axis[freq_index_rows, i])
-            spec_db[i] = np.append(spec_db[i], spectrum_db[freq_index_rows, i])
-        freqs = np.asarray(freqs)
-        spec_db = np.asarray(spec_db)
+            freq_index_rows = where(
+                (freq_axis[:, i] > 89.1) & (freq_axis[:, i] < 11200)
+            )[0]
+            freqs[i] = append(freqs[i], freq_axis[freq_index_rows, i])
+            spec_db[i] = append(spec_db[i], spectrum_db[freq_index_rows, i])
+        freqs = asarray(freqs)
+        spec_db = asarray(spec_db)
 
     elif (len(spectrum_db.shape) > 1) & (len(freq_axis.shape) == 1):
         # Frequency axis of interest
-        freq_index = np.where((freq_axis > 89.1) & (freq_axis < 11200))[0]
+        freq_index = where((freq_axis > 89.1) & (freq_axis < 11200))[0]
         # Initialization
         nfreqs = len(freq_index)
         nseg = spectrum_db.shape[1]
-        freqs = np.zeros((nseg, nfreqs))
-        spec_db = np.zeros((nseg, nfreqs))
+        freqs = empty((nseg, nfreqs))
+        spec_db = empty((nseg, nfreqs))
         for i in range(nseg):
             freqs[i, :] = freq_axis[freq_index]
             spec_db[i, :] = spectrum_db[freq_index, i]
 
     #### Screening to find the potential tonal components ########################
 
     peak_index = _screening_for_tones(freqs, spec_db, "smoothed", 90, 11200)
@@ -85,22 +89,22 @@
     # Initialization of the results lists
     if nseg == 1:
         PR = []
         t_pr = []
         tones_freqs = []
         prominence = []
     else:
-        PR = [[]for i in range(nseg)]
-        t_pr = [[]for i in range(nseg)]
-        tones_freqs = [[]for i in range(nseg)]
-        prominence = [[]for i in range(nseg)]
+        PR = [[] for i in range(nseg)]
+        t_pr = [[] for i in range(nseg)]
+        tones_freqs = [[] for i in range(nseg)]
+        prominence = [[] for i in range(nseg)]
 
     for i in range(nseg):
 
-        pr = np.array([], dtype=object)
+        pr = array([], dtype=object)
 
         if nseg == 1:
             peaks = peak_index
             spec = spec_db
             fr = freqs
 
         elif nseg > 1:
@@ -120,67 +124,67 @@
                     fr, spec, peaks.astype(int), nb_tones, ind
                 )
 
             ft = fr[ind]
 
             # Level of the middle critical band
             f1, f2 = _critical_band(ft)
-            low_limit_idx = np.argmin(np.abs(fr - f1))
-            high_limit_idx = np.argmin(np.abs(fr - f2))
+            low_limit_idx = argmin(abs(fr - f1))
+            high_limit_idx = argmin(abs(fr - f2))
 
             spec_sum = sum(10 ** (spec[low_limit_idx:high_limit_idx] / 10))
             if spec_sum != 0:
-                Lm = 10 * np.log10(spec_sum)
+                Lm = 10 * log10(spec_sum)
             else:
                 Lm = 0
 
             # Level of the lower critical band
             f1, f2 = _lower_critical_band(ft)
-            low_limit = np.argmin(np.abs(fr - f1))
-            high_limit = np.argmin(np.abs(fr - f2))
+            low_limit = argmin(abs(fr - f1))
+            high_limit = argmin(abs(fr - f2))
 
             spec_sum = sum(10 ** (spec[low_limit:high_limit] / 10))
             if spec_sum != 0:
-                Ll = 10 * np.log10(spec_sum)
+                Ll = 10 * log10(spec_sum)
             else:
                 Ll = 0
 
             delta_f = f2 - f1
 
             # Level of the upper critical band
             f1, f2 = _upper_critical_band(ft)
-            low_limit = np.argmin(np.abs(fr - f1))
-            high_limit = np.argmin(np.abs(fr - f2))
+            low_limit = argmin(abs(fr - f1))
+            high_limit = argmin(abs(fr - f2))
 
             spec_sum = sum(10 ** (spec[low_limit:high_limit] / 10))
             if spec_sum != 0:
-                Lu = 10 * np.log10(spec_sum)
+                Lu = 10 * log10(spec_sum)
             else:
                 Lu = 0
 
             if ft <= 171.4:
-                delta = 10 * np.log10(10 ** (0.1 * Lm)) - 10 * np.log10(
+                delta = 10 * log10(10 ** (0.1 * Lm)) - 10 * log10(
                     ((100 / delta_f) * 10 ** (0.1 * Ll) + 10 ** (0.1 * Lu)) * 0.5
                 )
 
             elif ft > 171.4:
-                delta = 10 * np.log10(10 ** (0.1 * Lm)) - 10 * np.log10(
+                delta = 10 * log10(10 ** (0.1 * Lm)) - 10 * log10(
                     (10 ** (0.1 * Ll) + 10 ** (0.1 * Lu)) * 0.5
                 )
 
             if delta > 0:
                 if nseg > 1:
-                    tones_freqs[i] = np.append(tones_freqs[i], ft)
+                    tones_freqs[i] = append(tones_freqs[i], ft)
                 elif nseg == 1:
-                    tones_freqs = np.append(tones_freqs, ft)
-                pr = np.append(pr, delta)
+                    tones_freqs = append(tones_freqs, ft)
+                pr = append(pr, delta)
 
                 # Prominent discrete tone criteria
                 if ft >= 89.1 and ft <= 1000:
-                    if delta >= 9 + 10 * np.log10(1000 / ft):
+                    if delta >= 9 + 10 * log10(1000 / ft):
                         if nseg > 1:
                             prominence[i].append(True)
 
                         elif nseg == 1:
                             prominence.append(True)
                     else:
                         if nseg > 1:
@@ -201,31 +205,30 @@
                             prominence[i].append(False)
 
                         elif nseg == 1:
                             prominence.append(False)
 
             # suppression from the list of tones of all the candidates belonging to the
             # same critical band
-            sup = np.where((peaks >= low_limit_idx) & (peaks <= high_limit_idx))[0]
-            peaks = np.delete(peaks, sup)
+            sup = where((peaks >= low_limit_idx) & (peaks <= high_limit_idx))[0]
+            peaks = delete(peaks, sup)
             nb_tones -= len(sup)
 
         if nseg > 1:
-            if sum(np.power(10, (pr[prominence[i]] / 10))) != 0:
-                t_pr[i] = 10 * \
-                    np.log10(sum(np.power(10, (pr[prominence[i]] / 10))))
+            if sum(power(10, (pr[prominence[i]] / 10))) != 0:
+                t_pr[i] = 10 * log10(sum(power(10, (pr[prominence[i]] / 10))))
             else:
                 t_pr[i] = 0
-            PR[i] = np.append(PR[i], pr)
+            PR[i] = append(PR[i], pr)
 
         elif nseg == 1:
-            if sum(np.power(10, (pr[prominence] / 10))) != 0:
-                t_pr = np.append(
-                    t_pr, 10 * np.log10(sum(np.power(10, (pr[prominence] / 10)))))
+            if sum(power(10, (pr[prominence] / 10))) != 0:
+                t_pr = append(
+                    t_pr, 10 * log10(sum(power(10, (pr[prominence] / 10)))))
             else:
                 t_pr = 0
-            PR = np.append(PR, pr)
+            PR = append(PR, pr)
 
-    tones_freqs = np.asarray(tones_freqs, dtype=object)
-    prominence = np.asarray(prominence, dtype=object)
+    tones_freqs = asarray(tones_freqs, dtype=object)
+    prominence = asarray(prominence, dtype=object)
 
     return tones_freqs, PR, prominence, t_pr
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_freq.py` & `mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_freq.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 # -*- coding: utf-8 -*-
 
+# Optional package import
+try:
+    import pytest
+except ImportError:
+    raise RuntimeError("In order to perform the tests you need the 'pytest' package.")
 # External import
 import numpy as np
 
-# Local imports
-from mosqito.sq_metrics.tonality.prominence_ratio_ecma._pr_main_calc import _pr_main_calc
-from mosqito.utils.conversion import amp2db
+# Local application imports
+from mosqito.utils import load
+from mosqito.sound_level_meter.comp_spectrum import comp_spectrum
+from mosqito.sq_metrics import pr_ecma_freq
 
 
-def pr_ecma_freq(spectrum, freqs, prominence=True):
-    """Computation of prominence ratio according to ECMA-74, annex D.10
-    for an amplitude or complex frequency spectrum.
-        The T-PR value is calculated according to ECMA-TR/108
+@pytest.mark.pr_freq  # to skip or run PR test
+def test_pr_ecma_freq():
+    """Test function for the prominence ratio calculation of an audio signal
+
+    Validation function for the "pr_ecma_freq" function with complex spectrum array
+    as input. The input signal was generated using audacity, and then the spectrum is computed using mosqito.
 
     Parameters
     ----------
-    spectrum :numpy.array
-        An amplitude or complex frequency spectrum [nperseg x nseg].
-    freqs : np.array
-        Frequency axis [nperseg x nseg] or [nperseg]. 
-    prominence : boolean
-        If True, the algorithm only returns the prominent tones, if False it returns all tones detected.
-        Default is True.
-
-    Output
-    ------
-    t_pr : array of float
-        Global PR value.
-    pr : array of float
-        PR values for each detected tone.
-    promi : array of bool
-        Prominence criterion for each detected tone.    
-    tones_freqs : array of float
-        Frequency list of the detected tones.
+    None
+
+    Outputs
+    -------
+    None
     """
-    
+    # Test signal as input for prominence ratio calculation
+    # signals generated using audacity : white noise + tones at 200 and 2000 Hz
+
+    signal = {
+        "is_stationary": True,
+        "data_file": "tests/input/white_noise_442_1768_Hz_stationary.wav",
+    }
+
+    # Load signal
+    audio, fs = load(signal["data_file"], wav_calib=0.01)
+    # convert to frequency domain
+    spec, freqs = comp_spectrum(audio, fs, window='hanning', db=False)
+
+    # Compute tone-to-noise ratio
+    # 1D input
+    # Compute tone-to-noise ratio
+    t_pr, pr, promi, freq = pr_ecma_freq(spec, freqs=freqs, prominence=False)
+
+    # 2D spectrum, 1D freq axis
+    spec = np.tile(spec, (4, 1)).T
+
+    t_pr, pr, promi, freq = pr_ecma_freq(spec, freqs=freqs, prominence=False)
+
+    # 2D spectrum, 2D freq axis
+    freqs = np.tile(freqs, (4, 1)).T
+    t_pr, pr, promi, freq = pr_ecma_freq(spec, freqs=freqs, prominence=False)
 
-    if len(spectrum) != len(freqs) :
-        raise ValueError('Input spectrum and frequency axis must have the same size')
 
-    # Compute spectrum dB values
-    spectrum_db = amp2db(np.abs(spectrum), ref=2e-5)
-                  
-    # Compute PR values
-    tones_freqs, pr, prom, t_pr = _pr_main_calc(spectrum_db, freqs)
- 
-    if prominence == False:
-        return t_pr, pr, prom, tones_freqs  
-    else:
-        return t_pr, pr[prom], prom[prom], tones_freqs[prom]
+if __name__ == "__main__":
+    test_pr_ecma_freq()
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_critical_band.py` & `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_critical_band.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Fri Dec 11 09:04:04 2020
 
-@author: pc
-"""
-import numpy as np
+# Standard library imports
+from numpy import power, sqrt
 
 
 def _critical_band(f0):
     """Analytical definition of the critical band centered on f0
     according to ECMA-74 annex D.8"""
 
-    delta_fc = 25 + 75 * np.power(1 + 1.4 * np.power(f0 / 1000, 2), 0.69)
+    delta_fc = 25 + 75 * power(1 + 1.4 * power(f0 / 1000, 2), 0.69)
 
     if f0 < 500:
         f1 = f0 - delta_fc / 2
         f2 = f0 + delta_fc / 2
 
     elif f0 >= 500:
-        f1 = -1 * delta_fc / 2 + np.sqrt(delta_fc ** 2 + 4 * f0 ** 2) / 2
+        f1 = -1 * delta_fc / 2 + sqrt(delta_fc ** 2 + 4 * f0 ** 2) / 2
         f2 = f1 + delta_fc
 
     return f1, f2
 
 
 def _lower_critical_band(f0):
     """Analytical definition of the critical band immediately below and contiguous
@@ -40,15 +37,15 @@
         c1 = 1.001
         c2 = -6.9e-05
     elif f0 > 1600:
         c0 = 6.8
         c1 = 0.806
         c2 = -8.2e-06
 
-    f1 = c0 + c1 * f0 + c2 * f0 ** 2
+    f1 = c0 + c1 * f0 + c2 * f0**2
 
     return f1, f2
 
 
 def _upper_critical_band(f0):
     """Analytical definition of the critical band immediately above and contiguous
     with the critical band centered on f0 according to ECMA-74 annex D.10
@@ -61,10 +58,10 @@
         c1 = 1.035
         c2 = 7.7e-05
     elif f0 > 1600:
         c0 = 3.3
         c1 = 1.215
         c2 = 2.16e-05
 
-    f2 = c0 + c1 * f0 + c2 * f0 ** 2
+    f2 = c0 + c1 * f0 + c2 * f0**2
 
     return f1, f2
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_find_highest_tone.py` & `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_find_highest_tone.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Wed Dec 16 20:23:01 2020
 
-@author: Salomé
-"""
 # Standard library imports
-import numpy as np
+from numpy import argmin, argsort, delete, where, abs
 
 # Mosqito functions import
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma._critical_band import _critical_band
 
 
 def _find_highest_tone(freqs, spec_db, index, nb_tones, ind):
     """
@@ -41,32 +37,32 @@
     nb_tones : integer
         number of candidate tones non examinated updated
     """
 
     f = freqs[ind]
     # critical band centered on f
     f1, f2 = _critical_band(f)
-    low_limit_idx = np.argmin(np.abs(freqs - f1))
-    high_limit_idx = np.argmin(np.abs(freqs - f2))
+    low_limit_idx = argmin(abs(freqs - f1))
+    high_limit_idx = argmin(abs(freqs - f2))
 
     # Other tones in the critical band centered on f tones
     multiple_idx = index[index > low_limit_idx]
     multiple_idx = multiple_idx[multiple_idx < high_limit_idx]
 
     if len(multiple_idx) > 1:
-        sort_spec = np.argsort(-1 * spec_db[multiple_idx])
+        sort_spec = argsort(-1 * spec_db[multiple_idx])
 
         # highest tones in the critical band
         ind_p = multiple_idx[sort_spec[0]]
         ind_s = multiple_idx[sort_spec[1]]
 
         # suppression of the lower values
         for s in sort_spec[2:]:
-            sup = np.where(index == multiple_idx[s])[0]
-            index = np.delete(index, sup)
+            sup = where(index == multiple_idx[s])[0]
+            index = delete(index, sup)
             nb_tones -= 1
 
         if ind_p != ind:
             # screening to find the highest value in the critical band centered on fp
             ind_p, ind_s, index, nb_tones = _find_highest_tone(
                 freqs, spec_db, index, nb_tones, ind_p
             )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_peak_level.py` & `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_peak_level.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Tue Dec 22 10:26:48 2020
 
-@author: wantysal
-"""
 # Standard library import
-import numpy as np
+from numpy import abs, log10
 
 
 def _peak_level(freqs, spec, peak_index):
     """
         Correct the level of the peak present at peak_index
 
         This kind of error in peak levels is due to spectrum resolution
@@ -35,46 +31,46 @@
     # initial level
     Li = spec[peak_index]
     # modified level
     L = spec[peak_index]
 
     # Screen the right points of the peak
     temp = peak_index + 1
-    
+
     if temp != len(spec):
         Ltemp = Li
         # As long as the level decreases,
-        while Ltemp - np.abs(spec[temp]) > 0:
+        while Ltemp - abs(spec[temp]) > 0:
             # if the level of the point is close enough of the peak point,
             if Li - spec[temp] < 10:
                 Ltemp = spec[temp]
                 # its level is summed up with the peak's one
-                L = 10 * np.log10(10 ** (L / 10) + 10 ** (spec[temp] / 10))
-                
+                L = 10 * log10(10 ** (L / 10) + 10 ** (spec[temp] / 10))
+
                 temp += 1
                 if temp == len(spec):
                     temp -= 1
                     Ltemp = -1
             else:
                 Ltemp = -1
 
     # Screen the left points of the peak
     temp = peak_index - 1
-    
+
     if temp != -1:
         Ltemp = Li
         # As long as the level decreases,
-        while Ltemp - np.abs(spec[temp]) > 0:
+        while Ltemp - abs(spec[temp]) > 0:
             # if the level of the point is close enough of the peak point,
             if Li - spec[temp] < 10:
                 Ltemp = spec[temp]
                 # its level is summed up with the peak's one
-                L = 10 * np.log10(10 ** (L / 10) + 10 ** (spec[temp] / 10))
-    
+                L = 10 * log10(10 ** (L / 10) + 10 ** (spec[temp] / 10))
+
                 temp -= 1
-                if temp <0:
+                if temp < 0:
                     temp += 1
                     Ltemp = -1
             else:
                 Ltemp = -1
 
     return L
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_screening_for_tones.py` & `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_screening_for_tones.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Wed Dec 16 20:23:01 2020
 
-@author: wantysal
-"""
 # Standard library imports
-import numpy as np
+from numpy import arange, diff, sign, where, delete, asarray, append
 
 # Mosqito functions import
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma._spectrum_smoothing import _spectrum_smoothing
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma._LTH import _LTH
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma._critical_band import _critical_band
 
 
@@ -54,15 +50,15 @@
     # Creation of the smoothed spectrum
     smooth_spec = _spectrum_smoothing(freqs, spec_db.T, 24, low_freq, high_freq, freqs).T
     
     
     n = spec_db.shape[0]
     if len(spec_db.shape)>1:
         m = spec_db.shape[1] 
-        stop = np.arange(1,n+1) * m -1
+        stop = arange(1,n+1) * m -1
         
     else:
         m = spec_db.shape[0]
         n = 1
         stop = [m]
     
     
@@ -70,49 +66,49 @@
     spec_db = spec_db.ravel()
     freqs = freqs.ravel()
  
     if method == "smoothed":
 
         # Criteria 1 : the level of the spectral line is higher than the level of
         # the two neighboring lines
-        maxima = (np.diff(np.sign(np.diff(spec_db))) < 0).nonzero()[0] + 1
+        maxima = (diff(sign(diff(spec_db))) < 0).nonzero()[0] + 1
 
         # Criteria 2 : the level of the spectral line exceeds the corresponding lines
         # of the 1/24 octave smoothed spectrum by at least 6 dB
-        indexx = np.where(spec_db[maxima] > smooth_spec[maxima] + 6)[0]
+        indexx = where(spec_db[maxima] > smooth_spec[maxima] + 6)[0]
 
         # Criteria 3 : the level of the spectral line exceeds the threshold of hearing
         threshold = _LTH(freqs)
-        audible = np.where(spec_db[maxima][indexx] > threshold[maxima][indexx] + 10)[0]
+        audible = where(spec_db[maxima][indexx] > threshold[maxima][indexx] + 10)[0]
 
-        index = np.arange(0, len(spec_db))[maxima][indexx][audible]
+        index = arange(0, len(spec_db))[maxima][indexx][audible]
 
     if method == "not-smoothed":
         # Criteria 1 : the level of the spectral line is higher than the level of
         # the two neighboring lines
         maxima = (
-            np.diff(np.sign(np.diff(spec_db[3 : len(spec_db) - 3]))) < 0
+            diff(sign(diff(spec_db[3 : len(spec_db) - 3]))) < 0
         ).nonzero()[
             0
         ] + 1  # local max
 
         # Criteria 2 : the level of the spectral line is at least 7 dB higher than its
         # +/- 2,3 neighbors
-        indexx = np.where(
+        indexx = where(
             (spec_db[maxima] > (spec_db[maxima + 2] + 7))
             & (spec_db[maxima] > (spec_db[maxima - 2] + 7))
             & (spec_db[maxima] > (spec_db[maxima + 3] + 7))
             & (spec_db[maxima] > (spec_db[maxima - 3] + 7))
         )[0]
 
         # Criteria 3 : the level of the spectral line exceeds the threshold of hearing
         threshold = _LTH(freqs)
-        audible = np.where(spec_db[maxima][indexx] > threshold[maxima][indexx] + 10)[0]
+        audible = where(spec_db[maxima][indexx] > threshold[maxima][indexx] + 10)[0]
 
-        index = np.arange(0, len(spec_db))[maxima][indexx][audible]
+        index = arange(0, len(spec_db))[maxima][indexx][audible]
 
     ###############################################################################
     # Check of the tones width : a candidate is discarded if its width is greater
     # than half the critical bandwidth
 
     if n == 1:
         tones = []
@@ -159,19 +155,19 @@
         cb_width = f2 - f1
 
         # Tonal width
         t_width = freqs[high_limit] - freqs[low_limit]
 
         if t_width < cb_width:
             if n>1:
-                tones[block] = np.append(tones[block], peak_index - block*m)
+                tones[block] = append(tones[block], peak_index - block*m)
             else:
-                tones = np.append(tones, peak_index )
+                tones = append(tones, peak_index )
 
         # All the candidates already screened are deleted from the list
-        sup = np.where(index <= high_limit)[0]
-        index = np.delete(index, sup)
+        sup = where(index <= high_limit)[0]
+        index = delete(index, sup)
     
-    tones = np.asarray(tones, dtype=object)
+    tones = asarray(tones, dtype=object)
 
 
     return tones
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_spectrum_smoothing.py` & `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_spectrum_smoothing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Dec 21 16:44:36 2020
 
-@author: wantysal
-"""
 # Standard library import
-import numpy as np
+from numpy import arange, zeros, where, delete, argmin, mean, log10, squeeze, abs, empty
 
 # Local import
 from mosqito.sound_level_meter.noct_spectrum._getFrequencies import _getFrequencies
 
 
 def _spectrum_smoothing(freqs_in, spec, noct, low_freq, high_freq, freqs_out):
     """
@@ -38,61 +34,61 @@
     """
     nperseg = spec.shape[0]
     if len(spec.shape) > 1:
         nseg = spec.shape[1]
     else:
         nseg = 1
     spec = spec.ravel()
-    stop = np.arange(1, nseg + 1) * nperseg
+    stop = arange(1, nseg + 1) * nperseg
     freqs_in = freqs_in.ravel()
 
     # n-th octave bands filter
     filter_freqs = _getFrequencies(low_freq, high_freq, noct, G=10, fr=1000)["f"]
     filter_freqs[len(filter_freqs) - 1, 2] = high_freq
     filter_freqs[0, 0] = low_freq
 
     # Smoothed spectrum creation
     nb_bands = filter_freqs.shape[0]
-    smoothed_spectrum = np.zeros((nb_bands, nseg))
+    smoothed_spectrum = zeros((nb_bands, nseg))
     i = 0
     # Each band is considered individually until all of them have been treated
     while nb_bands > 0:
         # Find the index of the spectral components within the frequency bin
-        bin_index = np.where((freqs_in >= filter_freqs[i, 0]) & (freqs_in <= filter_freqs[i, 2]))[0]
+        bin_index = where((freqs_in >= filter_freqs[i, 0]) & (freqs_in <= filter_freqs[i, 2]))[0]
 
         # If the frequency bin is empty, it is deleted from the list
         if len(bin_index) == 0:
-            smoothed_spectrum = np.delete(smoothed_spectrum, i, axis=0)
-            filter_freqs = np.delete(filter_freqs, i, axis=0)
+            smoothed_spectrum = delete(smoothed_spectrum, i, axis=0)
+            filter_freqs = delete(filter_freqs, i, axis=0)
             nb_bands -= 1
 
         else:
             # The spectral components within the frequency bin are averaged on an energy basis
-            spec_sum = np.zeros((nseg))
+            spec_sum = empty((nseg))
             for j in range(nseg):
                 if len(bin_index[(bin_index < stop[j]) & (bin_index > (stop[j] - nperseg))])!= 0:
-                    spec_sum[j] = np.mean(10** (spec[bin_index[(bin_index < stop[j]) & (bin_index > (stop[j] - nperseg))]]/ 10))
+                    spec_sum[j] = mean(10** (spec[bin_index[(bin_index < stop[j]) & (bin_index > (stop[j] - nperseg))]]/ 10))
                 else:
                     spec_sum[j] = 1e-12
-            smoothed_spectrum[i, :] = 10 * np.log10(spec_sum)# / len(bin_index[(bin_index < stop[j]) & (bin_index > (stop[j] - m))]))
+            smoothed_spectrum[i, :] = 10 * log10(spec_sum)# / len(bin_index[(bin_index < stop[j]) & (bin_index > (stop[j] - m))]))
         nb_bands -= 1
         i += 1
     # Pose of the smoothed spectrum on the frequency-axis
-    low = np.zeros((filter_freqs.shape[0], nseg))
-    high = np.zeros((filter_freqs.shape[0], nseg))
+    low = empty((filter_freqs.shape[0], nseg))
+    high = empty((filter_freqs.shape[0], nseg))
 
     # Index of the lower and higher limit of each frequency bin into the original spectrum
     for i in range(len(filter_freqs)):
-        low[i,:] = np.argmin(np.abs(freqs_out - filter_freqs[i, 0]))
-        high[i,:] = np.argmin(np.abs(freqs_out - filter_freqs[i, 2]))
+        low[i,:] = argmin(abs(freqs_out - filter_freqs[i, 0]))
+        high[i,:] = argmin(abs(freqs_out - filter_freqs[i, 2]))
     low = low.astype(int)
     high = high.astype(int)
 
-    smooth_spec = np.zeros((nperseg, nseg))
+    smooth_spec = empty((nperseg, nseg))
     for i in range(nseg):
         for j in range(filter_freqs.shape[0]):
             smooth_spec[low[j,i] : high[j,i], i] = smoothed_spectrum[j,i]
     
     if smooth_spec.shape[1] == 1:
-        smooth_spec = np.squeeze(smooth_spec)
+        smooth_spec = squeeze(smooth_spec)
 
     return smooth_spec
```

### Comparing `mosqito-1.1.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_tnr_main_calc.py` & `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_tnr_main_calc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-import numpy as np
+from numpy import where, log10, delete, argmin, asarray, power, append, empty, array, abs
 
 # Local functions imports
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma._critical_band import _critical_band
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma._screening_for_tones import _screening_for_tones
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma._find_highest_tone import _find_highest_tone
 from mosqito.sq_metrics.tonality.tone_to_noise_ecma._peak_level import _peak_level
 
@@ -17,17 +17,17 @@
         in 'Methods for automating prominent tone evaluation and for considerin
         variations with time or other reference quantities'
         The total value calculated, T-TNR, is calculated according to ECMA TR/108
 
     Parameters
     ----------
     spectrum_db : array
-        spectrum values in dB [nperseg x nseg].
+        spectrum values in dB (nperseg x nseg).
     freq_axis : array
-        frequency axis corresponding to the spectrum [nperseg x nseg].
+        frequency axis corresponding to the spectrum (nperseg x nseg).
 
     Output
     ------
     tones_freqs : array of float
         frequency of the tones (n blocks x number of tones)
     tnr : array of float
         TNR value calculated for each tone (n blocks x number of tones)
@@ -39,38 +39,38 @@
 
     #### Spectrum creation #######################################################
 
 
     if len(spectrum_db.shape) == 1:
         nseg = 1
         # Frequency axis of interest
-        freq_index = np.where((freq_axis > 89.1) & (freq_axis < 11200))[0]
+        freq_index = where((freq_axis > 89.1) & (freq_axis < 11200))[0]
         freqs = freq_axis[freq_index]
         spec_db = spectrum_db[freq_index]
         
     elif (len(spectrum_db.shape) > 1) & (len(freq_axis.shape) > 1):
         nseg = spectrum_db.shape[1]
         freqs = [[]for i in range(nseg)]
         spec_db = [[]for i in range(nseg)]
         for i in range(nseg):
             # Frequency axis of interest
-            freq_index_rows = np.where((freq_axis[:,i] > 89.1) & (freq_axis[:,i] < 11200))[0]
-            freqs[i] = np.append(freqs[i],freq_axis[freq_index_rows,i])
-            spec_db[i] = np.append(spec_db[i],spectrum_db[freq_index_rows,i])
-        freqs = np.asarray(freqs)
-        spec_db = np.asarray(spec_db)
+            freq_index_rows = where((freq_axis[:,i] > 89.1) & (freq_axis[:,i] < 11200))[0]
+            freqs[i] = append(freqs[i],freq_axis[freq_index_rows,i])
+            spec_db[i] = append(spec_db[i],spectrum_db[freq_index_rows,i])
+        freqs = asarray(freqs)
+        spec_db = asarray(spec_db)
     
     elif (len(spectrum_db.shape) > 1) & (len(freq_axis.shape) == 1):
         # Frequency axis of interest
-        freq_index = np.where((freq_axis > 89.1) & (freq_axis < 11200))[0]
+        freq_index = where((freq_axis > 89.1) & (freq_axis < 11200))[0]
         # Initialization
         nfreqs = len(freq_index)    
         nseg = spectrum_db.shape[1]
-        freqs = np.zeros((nseg,nfreqs))
-        spec_db = np.zeros((nseg,nfreqs))
+        freqs = empty((nseg,nfreqs))
+        spec_db = empty((nseg,nfreqs))
         for i in range(nseg):
             freqs[i,:] = freq_axis[freq_index]
             spec_db[i,:] = spectrum_db[freq_index,i]
 
 
     #### Screening to find the potential tonal components ########################
 
@@ -89,15 +89,15 @@
         prominence = [[]for i in range(nseg)]
     
 
     #### Evaluation of each candidate ############################################
 
     for i in range(nseg):
         
-        tnr = np.array([], dtype=object)
+        tnr = array([], dtype=object)
         
         if nseg == 1:
             peaks = peak_index
             spec = spec_db
             fr = freqs
             frs = freq_axis
         elif nseg > 1:
@@ -124,88 +124,88 @@
     
             # multiple tones in a critical band
             if ind_s != None:
                 fp = fr[ind_p]
                 fs = fr[ind_s]
     
                 # proximity criterion
-                delta_f = 21 * 10 ** ((1.2 * (np.abs(np.log10(fp / 212))) ** 1.8))
-                if np.abs(fs - fp) < delta_f:
+                delta_f = 21 * 10 ** ((1.2 * (abs(log10(fp / 212))) ** 1.8))
+                if abs(fs - fp) < delta_f:
     
                     # tone SPL
                     Lp = _peak_level(fr, spec, ind_p)
                     Ls = _peak_level(fr, spec, ind_s)
     
-                    Lt = 10 * np.log10(((10 ** (Lp / 10) + 10 ** (Ls / 10))))
+                    Lt = 10 * log10(((10 ** (Lp / 10) + 10 ** (Ls / 10))))
     
                     # total SPL in the critical band
                     f1, f2 = _critical_band(fp)
-                    low_limit_idx = np.argmin(np.abs(fr - f1))
-                    high_limit_idx = np.argmin(np.abs(fr - f2))
+                    low_limit_idx = argmin(abs(fr - f1))
+                    high_limit_idx = argmin(abs(fr - f2))
     
                     spec_sum = sum(10 ** (spec[low_limit_idx:high_limit_idx] / 10))
-                    Ltot = 10 * np.log10(spec_sum)
+                    Ltot = 10 * log10(spec_sum)
     
                     # suppression of the second highest tone from the list of tones
-                    sup = np.where(peaks == ind_s)[0]
-                    peaks = np.delete(peaks, sup)
+                    sup = where(peaks == ind_s)[0]
+                    peaks = delete(peaks, sup)
                     nb_tones -= 1
     
                     delta_ft = 2 * (frs[1] - frs[0])
     
                 else:
                     # the two highest tones are not close enough to be considered as one
                     # tone SPL
                     Lt = spec[ind_p]
     
                     # total SPL in the critical band
                     f1, f2 = _critical_band(fr[ind_p])
-                    low_limit_idx = np.argmin(np.abs(fr - f1))
-                    high_limit_idx = np.argmin(np.abs(fr - f2))
+                    low_limit_idx = argmin(abs(fr - f1))
+                    high_limit_idx = argmin(abs(fr - f2))
     
                     spec_sum = sum(10 ** (spec[low_limit_idx:high_limit_idx] / 10))
-                    Ltot = 10 * np.log10(spec_sum)
+                    Ltot = 10 * log10(spec_sum)
     
                     delta_ft = fr[1] - fr[0]
     
             # single tone in a critical band
             else:
                 # tone SPL
                 Lt = _peak_level(fr, spec, ind_p)
     
                 # total SPL in the critical band
                 f1, f2 = _critical_band(fr[ind_p])
-                low_limit_idx = np.argmin(np.abs(fr - f1))
-                high_limit_idx = np.argmin(np.abs(fr - f2))
+                low_limit_idx = argmin(abs(fr - f1))
+                high_limit_idx = argmin(abs(fr - f2))
     
                 spec_sum = sum(10 ** (spec[low_limit_idx:high_limit_idx] / 10))
-                Ltot = 10 * np.log10(spec_sum)
+                Ltot = 10 * log10(spec_sum)
     
                 delta_ft = fr[1] - fr[0]
     
             # SPL of the masking noise
             delta_fc = f2 - f1
             delta_ftot = frs[high_limit_idx] - frs[low_limit_idx]
-            Ln = 10 * np.log10(10 ** (Ltot / 10) - 10 ** (Lt / 10)) + 10 * np.log10(
+            Ln = 10 * log10(10 ** (Ltot / 10) - 10 ** (Lt / 10)) + 10 * log10(
                 delta_fc / (delta_ftot - delta_ft)
             )
     
             # Tone-to-noise ratio
             f = fr[ind_p]
             delta_t = Lt - Ln
             if delta_t > 0:
                 if nseg > 1:
-                    tones_freqs[i] = np.append(tones_freqs[i], f)
+                    tones_freqs[i] = append(tones_freqs[i], f)
                 elif nseg == 1:
-                    tones_freqs = np.append(tones_freqs, f)
-                tnr = np.append(tnr, delta_t)
+                    tones_freqs = append(tones_freqs, f)
+                tnr = append(tnr, delta_t)
     
                 # Prominence criteria
                 if f >= 89.1 and f < 1000:
-                    if delta_t >= 8 + 8.33 * np.log10(1000 / f):
+                    if delta_t >= 8 + 8.33 * log10(1000 / f):
                         if nseg > 1:
                             prominence[i].append(True)                        
                         elif nseg == 1:
                             prominence.append(True)
                     else:
                         if nseg > 1:
                             prominence[i].append(False)
@@ -223,32 +223,32 @@
                         if nseg > 1:
                             prominence[i].append(False)
                         
                         elif nseg == 1:
                             prominence.append(False)
     
             # suppression from the list of tones
-            sup = np.where(peaks == ind_p)[0]
-            peaks = np.delete(peaks, sup)
+            sup = where(peaks == ind_p)[0]
+            peaks = delete(peaks, sup)
             nb_tones -= 1
     
 
         if nseg > 1:
-            if sum(np.power(10, (tnr[prominence[i]] / 10))) != 0:
-                t_tnr[i] = 10 * np.log10(sum(np.power(10, (tnr[prominence[i]] / 10))))
+            if sum(power(10, (tnr[prominence[i]] / 10))) != 0:
+                t_tnr[i] = 10 * log10(sum(power(10, (tnr[prominence[i]] / 10))))
             else:
                 t_tnr[i] =  0
-            TNR[i] = np.append(TNR[i], tnr)               
+            TNR[i] = append(TNR[i], tnr)               
                     
                     
         elif nseg == 1:
-            if sum(np.power(10, (tnr[prominence] / 10))) != 0:
-                t_tnr = np.append(t_tnr,10 * np.log10(sum(np.power(10, (tnr[prominence] / 10)))))
+            if sum(power(10, (tnr[prominence] / 10))) != 0:
+                t_tnr = append(t_tnr,10 * log10(sum(power(10, (tnr[prominence] / 10)))))
             else:
                 t_tnr =  0
-            TNR = np.append(TNR, tnr)
+            TNR = append(TNR, tnr)
         
-    tones_freqs = np.asarray(tones_freqs, dtype=object)
-    prominence = np.asarray(prominence, dtype=object)
+    tones_freqs = asarray(tones_freqs, dtype=object)
+    prominence = asarray(prominence, dtype=object)
 
     
     return tones_freqs, TNR , prominence, t_tnr
```

### Comparing `mosqito-1.1.1/mosqito/utils/LTQ.py` & `mosqito-1.2.0/mosqito/utils/LTQ.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Thu Nov  5 17:32:06 2020
 
-@author: wantysal
-"""
-
-import numpy as np
+from numpy import array, interp
 
 
 def LTQ(bark_axis, reference="zwicker"):
     """Calculate the level threshold in quiet over bark_axis
 
     Linear interpolation from the data given in E. Zwicker, H. Fastl:
     Psychoacoustics. Springer, Berlin, Heidelberg, 1990. (figure 2.1)
     SPL is given for a free-field condition relative to 2 × 10−5 Pa
     (Threshold for roughness is slightly different)
 
     Parameters
     ----------
     bark_axis: numpy.array
-        frequency axis in bark to compute the threshold
+        Frequency axis in bark to compute the threshold
     reference: str()
         'zwicker' or 'roughness'
     """
 
     # Make list of minimum excitation (Hearing Treshold)
 
     if reference == "zwicker":
-        HTres_x = np.array(
+        HTres_x = array(
             [
                 2.40445500e-04,
                 2.97265560e-04,
                 3.83444580e-04,
                 4.87665300e-04,
                 6.38024300e-04,
                 8.26911900e-04,
@@ -79,15 +74,15 @@
                 2.31538743e01,
                 2.32710993e01,
                 2.33580350e01,
                 2.34824357e01,
             ]
         )
 
-        HTres_y = np.array(
+        HTres_y = array(
             [
                 73.28456,
                 69.49444,
                 65.17124,
                 61.262524,
                 57.471996,
                 53.918324,
@@ -136,15 +131,15 @@
                 65.02121,
                 75.87385,
                 89.63695,
             ]
         )
 
     if reference == "roughness":
-        HTres_x = np.array(
+        HTres_x = array(
             [
                 0,
                 0.01,
                 0.17,
                 0.8,
                 1,
                 1.5,
@@ -168,15 +163,15 @@
                 23,
                 24,
                 24.5,
                 25,
             ]
         )
 
-        HTres_y = np.array(
+        HTres_y = array(
             [
                 130,
                 70,
                 60,
                 30,
                 25,
                 20,
@@ -200,10 +195,10 @@
                 15,
                 48,
                 60,
                 130,
             ]
         )
 
-    threshold = np.interp(bark_axis, HTres_x, HTres_y)
+    threshold = interp(bark_axis, HTres_x, HTres_y)
 
     return threshold
```

### Comparing `mosqito-1.1.1/mosqito/utils/isoclose.py` & `mosqito-1.2.0/mosqito/utils/isoclose.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,61 +3,67 @@
 try:
     import matplotlib.pyplot as plt
 except ImportError:
     raise RuntimeError(
         "In order to perform this validation you need the 'matplotlib' package."
     )
 
-import numpy as np
+from numpy import amin, amax, arange, abs
 
-
-def isoclose(actual, desired, rtol=1e-7, atol=0, is_plot=False, tol_label=None, xaxis=None):
+def isoclose(
+    actual, desired, rtol=1e-7, atol=0, is_plot=False, tol_label=None, xaxis=None
+):
     """
     Check if two arrays are equal up to desired tolerance.
 
-    The test is inspired from section 5.1 of ISO 532-1. It compares 
+    The test is inspired from section 5.1 of ISO 532-1. It compares
     ``actual`` to ``desired +/- min(atol, rtol * abs(desired))``.
 
     Parameters
     ----------
     actual : array_like
         Array obtained.
     desired : array_like
         Array desired.
     rtol : float, optional
         Relative tolerance.
+        Default to 1e-7
     atol : float, optional
         Absolute tolerance.
+        Default to 0
     is_plot : bool, optional
-        To generate a "compliance" plot
+        To generate a "compliance" plot.
+        Default to False
     tol_label: str
         Label for the tolerance curves
+        Default to None
     xaxis : array_like, optional
-        x axis for the "compliance" plot
+        x axis for the "compliance" plot.
+        Default to None
 
-    Output
+    Returns
     ------
     is_isoclose: bool
         False if actual and desired are not equal up to specified tolerance.
 
     """
 
     # Tolerances
-    range_pos = np.amin(
+    range_pos = amin(
         [desired * (1 - abs(rtol)), desired - abs(atol)], axis=0)
-    range_neg = np.amax(
+    range_neg = amax(
         [desired * (1 + abs(rtol)), desired + abs(atol)], axis=0)
 
     # Test for ISO 532-1 comformance (section 5.1)
     is_isoclose = (actual >= range_pos).all() and (actual <= range_neg).all()
 
     if is_plot:
         # Define xaxis
         if xaxis is None:
-            xaxis = np.arange(actual.shape[0])
+            xaxis = arange(actual.shape[0])
 
         # Plot desired range
         plt.plot(
             xaxis,
             range_neg,
             color="tab:red",
             linestyle="solid",
```

### Comparing `mosqito-1.1.1/mosqito/utils/load.py` & `mosqito-1.2.0/mosqito/utils/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Nov 16 08:59:34 2020
-
-@author: wantysal
-"""
 
 # Standard library imports
-import numpy as np
+from numpy import int16, int32
 from scipy.io import wavfile, loadmat
 from scipy.signal import resample
 import pyuff
 
 
 def load(file, wav_calib=None, mat_signal="", mat_fs=""):
-    """Extract the signal and its time axis from .wav or .uff file,
-    resample the signal to 48 kHz, and affects its sampling frequency
+    """
+    Signal loading
+    
+    This function extracts the signal and its time axis from .wav or .uff file,
+    resamples the signal to 48 kHz, and affects its sampling frequency
     and time signal values.
 
     Parameters
     ----------
     file : string
-        string path to the signal file
+        String path to the signal file.
     wav_calib : float, optional
         Wav file calibration factor [Pa/FS]. Level of the signal in Pa_peak
         corresponding to the full scale of the .wav file. If None, a
-        calibration factor of 1 is considered. Default to None.
+        calibration factor of 1 is considered. 
+        Default to None
     mat_signal : string
-        in case of a .mat file, name of the signal variable
+        In case of a .mat file, name of the signal variable.
+        Default to ""
     mat_fs : string
-        in case of a .mat file, name of the sampling frequency variable
-
-    Outputs
+        In case of a .mat file, name of the sampling frequency variable.
+        Default to ""
+        
+    Returns
     -------
     signal : numpy.array
         time signal values
     fs : integer
         sampling frequency
     """
 
@@ -47,19 +48,19 @@
             signal = signal[:, 0]
             print("[Info] Multichannel signal loaded. Keeping only first channel")
 
         # calibration factor for the signal to be in Pa
         if wav_calib is None:
             wav_calib = 1
             print("[Info] A calibration of 1 Pa/FS is considered")
-        if isinstance(signal[0], np.int16):
+        if isinstance(signal[0], int16):
             signal = wav_calib * signal / (2**15 - 1)
-        elif isinstance(signal[0], np.int32):
+        elif isinstance(signal[0], int32):
             signal = wav_calib * signal / (2**31 - 1)
-        elif isinstance(signal[0], np.float):
+        elif isinstance(signal[0], float):
             signal = wav_calib * signal
 
     # load the .uff file content
     elif file[-3:].lower() == "uff" or file[-3:].lower() == "unv":
         uff_file = pyuff.UFF(file)
         data = uff_file.read_sets()
```

### Comparing `mosqito-1.1.1/mosqito/utils/time_segmentation.py` & `mosqito-1.2.0/mosqito/utils/time_segmentation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-import numpy as np
+from numpy import zeros, hstack, array, mean, linspace
 
 
 def time_segmentation(sig, fs, nperseg=2048, noverlap=None, is_ecma=False):
     """Function used for the segmentation of a time signal into
     smaller parts of audio (blocks).
 
     Parameters
@@ -31,27 +31,27 @@
     time: numpy.array
         The time axis corresponding to the segmented
         signal, size (nseg,)
     """
 
     if noverlap is None:
         noverlap = int(nperseg / 2)
-        
+
     if noverlap == 0:
         noverlap = nperseg
 
     if is_ecma:
         # pad with zeros at the begining
-        sig = np.hstack((np.zeros(nperseg), sig))
+        sig = hstack((zeros(nperseg), sig))
 
     # build time axis for sig
-    time = np.linspace(0, (len(sig) - 1) / fs, num=len(sig))
+    time = linspace(0, (len(sig) - 1) / fs, num=len(sig))
 
     l = 0
     block_array = []
     time_array = []
     while l * noverlap <= len(sig) - nperseg:
         block_array.append(sig[l * noverlap : nperseg + l * noverlap])
-        time_array.append(np.mean(time[l * noverlap : nperseg + l * noverlap]))
+        time_array.append(mean(time[l * noverlap : nperseg + l * noverlap]))
         l += 1
 
-    return np.array(block_array).T, np.array(time_array)
+    return array(block_array).T, array(time_array)
```

### Comparing `mosqito-1.1.1/mosqito.egg-info/SOURCES.txt` & `mosqito-1.2.0/mosqito.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,34 +8,37 @@
 mosqito/__init__.py
 mosqito.egg-info/PKG-INFO
 mosqito.egg-info/SOURCES.txt
 mosqito.egg-info/dependency_links.txt
 mosqito.egg-info/requires.txt
 mosqito.egg-info/top_level.txt
 mosqito/sound_level_meter/__init__.py
+mosqito/sound_level_meter/comp_spectrum.py
 mosqito/sound_level_meter/freq_band_synthesis.py
-mosqito/sound_level_meter/spectrum.py
 mosqito/sound_level_meter/noct_spectrum/__init__.py
 mosqito/sound_level_meter/noct_spectrum/_center_freq.py
 mosqito/sound_level_meter/noct_spectrum/_filter_bandwidth.py
 mosqito/sound_level_meter/noct_spectrum/_getFrequencies.py
 mosqito/sound_level_meter/noct_spectrum/_n_oct_freq_filter.py
 mosqito/sound_level_meter/noct_spectrum/_n_oct_time_filter.py
 mosqito/sound_level_meter/noct_spectrum/_nominal_frequency.py
 mosqito/sound_level_meter/noct_spectrum/noct_spectrum.py
 mosqito/sound_level_meter/noct_spectrum/noct_synthesis.py
 mosqito/sq_metrics/__init__.py
 mosqito/sq_metrics/loudness/__init__.py
 mosqito/sq_metrics/loudness/loudness_ecma/__init__.py
 mosqito/sq_metrics/loudness/loudness_ecma/_auditory_filters_centre_freq.py
+mosqito/sq_metrics/loudness/loudness_ecma/_band_pass_signals.py
 mosqito/sq_metrics/loudness/loudness_ecma/_ear_filter_design.py
+mosqito/sq_metrics/loudness/loudness_ecma/_ecma_time_segmentation.py
 mosqito/sq_metrics/loudness/loudness_ecma/_gammatone.py
 mosqito/sq_metrics/loudness/loudness_ecma/_loudness_ecma_data.py
+mosqito/sq_metrics/loudness/loudness_ecma/_loudness_from_bandpass.py
 mosqito/sq_metrics/loudness/loudness_ecma/_nonlinearity.py
-mosqito/sq_metrics/loudness/loudness_ecma/_rectified_band_pass_signals.py
+mosqito/sq_metrics/loudness/loudness_ecma/_preprocessing.py
 mosqito/sq_metrics/loudness/loudness_ecma/loudness_ecma.py
 mosqito/sq_metrics/loudness/loudness_zwst/__init__.py
 mosqito/sq_metrics/loudness/loudness_zwst/_calc_slopes.py
 mosqito/sq_metrics/loudness/loudness_zwst/_get_rns_index.py
 mosqito/sq_metrics/loudness/loudness_zwst/_main_loudness.py
 mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst.py
 mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_freq.py
@@ -56,14 +59,25 @@
 mosqito/sq_metrics/roughness/roughness_dw/_H_weighting.py
 mosqito/sq_metrics/roughness/roughness_dw/__init__.py
 mosqito/sq_metrics/roughness/roughness_dw/_ear_filter_coeff.py
 mosqito/sq_metrics/roughness/roughness_dw/_gzi_weighting.py
 mosqito/sq_metrics/roughness/roughness_dw/_roughness_dw_main_calc.py
 mosqito/sq_metrics/roughness/roughness_dw/roughness_dw.py
 mosqito/sq_metrics/roughness/roughness_dw/roughness_dw_freq.py
+mosqito/sq_metrics/roughness/roughness_ecma/__init__.py
+mosqito/sq_metrics/roughness/roughness_ecma/_estimate_fund_mod_rate.py
+mosqito/sq_metrics/roughness/roughness_ecma/_interpolation_50.py
+mosqito/sq_metrics/roughness/roughness_ecma/_lowpass_filter.py
+mosqito/sq_metrics/roughness/roughness_ecma/_noise_reduction.py
+mosqito/sq_metrics/roughness/roughness_ecma/_non_linear_transform.py
+mosqito/sq_metrics/roughness/roughness_ecma/_peak_picking.py
+mosqito/sq_metrics/roughness/roughness_ecma/_refinement.py
+mosqito/sq_metrics/roughness/roughness_ecma/_von_hann_window.py
+mosqito/sq_metrics/roughness/roughness_ecma/_weighting.py
+mosqito/sq_metrics/roughness/roughness_ecma/roughness_ecma.py
 mosqito/sq_metrics/sharpness/__init__.py
 mosqito/sq_metrics/sharpness/sharpness_din/__init__.py
 mosqito/sq_metrics/sharpness/sharpness_din/_weighting_fastl.py
 mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_freq.py
 mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_from_loudness.py
 mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_perseg.py
 mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_st.py
@@ -76,43 +90,52 @@
 mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi.py
 mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_freq.py
 mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_level.py
 mosqito/sq_metrics/tonality/__init__.py
 mosqito/sq_metrics/tonality/prominence_ratio_ecma/__init__.py
 mosqito/sq_metrics/tonality/prominence_ratio_ecma/_pr_main_calc.py
 mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_freq.py
+mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_perseg.py
 mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_st.py
-mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_tv.py
 mosqito/sq_metrics/tonality/tone_to_noise_ecma/_LTH.py
 mosqito/sq_metrics/tonality/tone_to_noise_ecma/__init__.py
 mosqito/sq_metrics/tonality/tone_to_noise_ecma/_critical_band.py
 mosqito/sq_metrics/tonality/tone_to_noise_ecma/_find_highest_tone.py
 mosqito/sq_metrics/tonality/tone_to_noise_ecma/_peak_level.py
 mosqito/sq_metrics/tonality/tone_to_noise_ecma/_screening_for_tones.py
 mosqito/sq_metrics/tonality/tone_to_noise_ecma/_spectrum_smoothing.py
 mosqito/sq_metrics/tonality/tone_to_noise_ecma/_tnr_main_calc.py
 mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_freq.py
+mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_perseg.py
 mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_st.py
-mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_tv.py
 mosqito/utils/LTQ.py
 mosqito/utils/__init__.py
-mosqito/utils/conversion.py
+mosqito/utils/am_noise_generator.py
+mosqito/utils/am_sine_generator.py
+mosqito/utils/fm_sine_generator.py
 mosqito/utils/isoclose.py
 mosqito/utils/load.py
 mosqito/utils/sine_wave_generator.py
 mosqito/utils/time_segmentation.py
+mosqito/utils/conversion/__init__.py
+mosqito/utils/conversion/amp2db.py
+mosqito/utils/conversion/bark2freq.py
+mosqito/utils/conversion/db2amp.py
+mosqito/utils/conversion/freq2bark.py
+mosqito/utils/conversion/spectrum2dBA.py
 tests/output/__init__.py
 tests/sq_metrics/__init__.py
 tests/sq_metrics/loudness/__init__.py
 tests/sq_metrics/loudness/test_loudness_ecma.py
 tests/sq_metrics/loudness/test_loudness_zwst.py
 tests/sq_metrics/loudness/test_loudness_zwtv.py
 tests/sq_metrics/roughness/__init__.py
 tests/sq_metrics/roughness/signals_test_generation.py
 tests/sq_metrics/roughness/test_roughness_dw.py
+tests/sq_metrics/roughness/test_roughness_ecma.py
 tests/sq_metrics/sharpness/__init__.py
 tests/sq_metrics/sharpness/test_sharpness_din.py
 tests/sq_metrics/tonality/__init__.py
 tests/sq_metrics/tonality/test_pr_ecma_freq.py
 tests/sq_metrics/tonality/test_pr_ecma_st.py
 tests/sq_metrics/tonality/test_pr_ecma_tv.py
 tests/sq_metrics/tonality/test_tnr_ecma_freq.py
```

### Comparing `mosqito-1.1.1/setup.py` & `mosqito-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import setuptools
 
 # /!\ update before a release
-MoSQITo_VERSION = "1.1.1"
+from mosqito import __version__
+version = __version__
 
 # MoSQITo description
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 python_requires = ">= 3.5"
 
@@ -16,23 +17,23 @@
         requirements
     ).splitlines()  # remove endline in each element
 
 tests_require = ["pytest>=5.4.1", "pandas", "openpyxl", "matplotlib"]
 
 setuptools.setup(
     name="mosqito",
-    version=MoSQITo_VERSION,
+    version=version,
     author="MoSQITo Developers",
     author_email="martin.glesser@eomys.com",
     description="Modular Sound Quality Integrated Toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Eomys/MoSQITo",
     download_url="https://github.com/Eomys/MoSQITo/archive/v{}.tar.gz".format(
-        MoSQITo_VERSION
+        version
     ),
     packages=setuptools.find_packages(
         exclude=[
             "docs",
             "tutorials",
             "validations",
             "tests",
```

### Comparing `mosqito-1.1.1/tests/sq_metrics/loudness/test_loudness_ecma.py` & `mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_ecma.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,43 +11,38 @@
 
 # Local application imports
 from mosqito.utils.sine_wave_generator import (
     sine_wave_generator,
 )
 from mosqito.sq_metrics import loudness_ecma
 
-
 @pytest.mark.loudness_ecma  # to skip or run only loudness ecma tests
 def test_loudness_ecma():
     """Test function for the Loudness_ecma calculation"""
 
     # Generate a 1kHz / 80 dB test tone and compute loudness
     signal, _ = sine_wave_generator(
         fs=48000,
-        t=0.25,
-        spl_value=80,
+        d=0.25,
         freq=1000,
+        spl_level=80,
     )
-    n_specific, _ = loudness_ecma(signal)
-    n_specific = np.array(n_specific)
-    n_tot = np.sum(n_specific, axis=0)
-    n_tot_mean_1kHz = np.mean(n_tot[5:])
+    
+    n_1kHz, _, _, _, _ = loudness_ecma(signal, fs=48000)
 
     # Generate a 5kHz / 78.7 dB test tone and compute loudness
     signal, _ = sine_wave_generator(
         fs=48000,
-        t=0.25,
-        spl_value=78.73977248964925,
+        d=0.25,
         freq=5000,
+        spl_level=78.49095, 
     )
-    n_specific, _ = loudness_ecma(signal)
-    n_specific = np.array(n_specific)
-    n_tot = np.sum(n_specific, axis=0)
-    n_tot_mean_5kHz = np.mean(n_tot[5:])
+    n_5kHz, _, _, _, _ = loudness_ecma(signal, fs=48000)
 
     # Compare loudness
-    np.testing.assert_almost_equal(n_tot_mean_1kHz, n_tot_mean_5kHz)
-
+    
+    assert np.isclose(n_1kHz, n_5kHz)
+    
 
 # test de la fonction
 if __name__ == "__main__":
     test_loudness_ecma()
```

### Comparing `mosqito-1.1.1/tests/sq_metrics/loudness/test_loudness_zwst.py` & `mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_zwst.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 except ImportError:
     raise RuntimeError("In order to perform the tests you need the 'pytest' package.")
 
 import numpy as np
 from numpy.fft import fft, fftfreq
 
 # Local application imports
-from mosqito.utils import load, isoclose
+from mosqito.utils import load
+from mosqito.utils.isoclose import isoclose
 from mosqito.sq_metrics import loudness_zwst, loudness_zwst_freq, loudness_zwst_perseg
 from mosqito.sq_metrics.loudness.loudness_zwst._main_loudness import _main_loudness
 from mosqito.sq_metrics.loudness.loudness_zwst._calc_slopes import _calc_slopes
 from tests.input.Test_signal_1 import test_signal_1
 
 
 @pytest.fixture
```

### Comparing `mosqito-1.1.1/tests/sq_metrics/loudness/test_loudness_zwtv.py` & `mosqito-1.2.0/tests/sq_metrics/roughness/test_roughness_ecma.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,80 @@
 # -*- coding: utf-8 -*-
 
-# Third party imports
-import pytest
+# Optional package import
+try:
+    import pytest
+except ImportError:
+    raise RuntimeError("In order to perform the tests you need the 'pytest' package.")
+
+import numpy as np
+from scipy.fft import fft
 
 # Local application imports
-from mosqito.sq_metrics import loudness_zwtv
-from mosqito.utils import load
-from validations.sq_metrics.loudness_zwtv.validation_loudness_zwtv import (
-    _check_compliance,
-)
+from mosqito.sq_metrics import roughness_ecma, roughness_ecma
+from mosqito.utils.am_sine_generator import am_sine_generator
 
 
-@pytest.mark.loudness_zwtv  # to skip or run only loudness zwicker time-varying tests
-def test_loudness_zwtv():
-    """Test function for the script loudness_zwicker_time
-
-    Test function for the script loudness_zwtv with
-    .wav file as input. The input file is provided by ISO 532-1 annex
-    B4 and B5, the compliance is assessed according to section 6.1 of the
-    standard. One .png compliance plot is generated.
+@pytest.mark.roughness_ecma  # to skip or run only ECMA 418-2 roughness tests
+def test_roughness_ecma():
+    """Test function for the roughness calculation of a audio signal
+
+    Test function for the script "comp_roughness" method with signal array
+    as input. The input signals are chosen according to the article "Psychoacoustical
+    roughness: implementation of an optimized model" by Daniel and Weber in 1997.
+    The figure 3 is used to compare amplitude-modulated signals created according to
+    their carrier frequency and modulation frequency to the article results.
+    One .png compliance plot is generated.
 
     Parameters
     ----------
     None
 
     Outputs
     -------
     None
     """
-    # Test signal as input for time-varying loudness
-    # (from ISO 532-1 annex B4)
-    signal = {
-        "data_file": "tests/input/Test signal 10 (tone pulse 1 kHz 10 ms 70 dB).wav",
-        "xls": "tests/input/Results and tests for synthetic signals (time varying loudness).xlsx",
-        "tab": "Test signal 10",
-        "N_specif_bark": 8.5,
-        "field": "free",
-    }
-
-    # Load signal and compute third octave band spectrum
-    sig, fs = load(signal["data_file"], wav_calib=2 * 2 ** 0.5)
-
-    # Compute Loudness
-    N, N_spec, bark_axis, time_axis = loudness_zwtv(sig, fs, field_type=signal["field"])
-    loudness = {
-        "name": "Loudness",
-        "values": N,
-        "specific values": N_spec,
-        "freqs": bark_axis,
-    }
-
-    # Check axis dimensions
-    assert len(N) == len(time_axis)
-    assert N_spec.shape[1] == len(time_axis)
-    assert N_spec.shape[0] == len(bark_axis)
 
-    # Check ISO 532-1 compliance
-    assert _check_compliance(loudness, signal, "./tests/output/")
+    # Stimulus generation
+    fmod = 70
+    time = np.linspace(0,1,48000)
+    xmod = np.sin(2*np.pi*fmod*time)
+    stimulus, _ = am_sine_generator(xmod, fs=48000, fc=1000, spl_level=60)
+
+    # Roughness calculation
+    R, _, _, _, _ = roughness_ecma(stimulus, fs=48000)
+
+    # Check compliance
+    tst = check_compliance(R)
+
+    assert tst
+
+def check_compliance(R):
+    """Check the compliance of roughness calc. to Daniel and Weber article
+    "Psychoacoustical roughness: implementation of an optimized model", 1997.
+
+    Check the compliance of the input data R to figure 3 of the article
+    using the reference data described in the dictionary article_ref.
+
+    Parameter
+    ---------
+    R: numpy.array
+        Calculated roughnesses [asper]
+
+    Output
+    ------
+    tst : bool
+        Compliance to the reference data
+    """
+
+    # Reference value of 1 asper given by Zwicker and Fastl
+    ref = 1
+
+    # Test for comformance (0.1 asper tolerance)
+    tst = (R >= ref - 0.1).all() and (R <= ref + 0.1).all()
+
+    return tst
 
 
 # test de la fonction
 if __name__ == "__main__":
-    test_loudness_zwtv()
+    test_roughness_ecma()
```

### Comparing `mosqito-1.1.1/tests/sq_metrics/roughness/test_roughness_dw.py` & `mosqito-1.2.0/tests/sq_metrics/roughness/test_roughness_dw.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     raise RuntimeError("In order to perform the tests you need the 'pytest' package.")
 
 import numpy as np
 from scipy.fft import fft
 
 # Local application imports
 from mosqito.sq_metrics import roughness_dw, roughness_dw_freq
-from tests.sq_metrics.roughness.signals_test_generation import signal_test
-from mosqito.sound_level_meter.spectrum import spectrum
+from mosqito.utils.am_sine_generator import am_sine_generator
+from mosqito.sound_level_meter.comp_spectrum import comp_spectrum
 
 
 @pytest.mark.roughness_dw  # to skip or run only Daniel and Weber roughness tests
 def test_roughness_dw():
     """Test function for the roughness calculation of a audio signal
 
     Test function for the script "comp_roughness" method with signal array
@@ -32,15 +32,18 @@
 
     Outputs
     -------
     None
     """
 
     # Stimulus generation
-    stimulus, _ = signal_test(fc=1000, fmod=70, mdepth=1, fs=44100, d=0.2, dB=60)
+    fmod = 70
+    time = np.linspace(0,1,48000)
+    xmod = np.sin(2*np.pi*fmod*time)
+    stimulus, _ = am_sine_generator(xmod, fs=48000, fc=1000, spl_level=60)
 
     # Roughness calculation
     roughness, time, _, _ = roughness_dw(stimulus, fs=44100, overlap=0)
     R = {
         "name": "Roughness",
         "values": roughness,
         "time": time,
@@ -67,21 +70,23 @@
     ----------
     None
 
     Outputs
     -------
     None
     """
-    fs = 44100
-    # Stimulus generation
-    stimulus, _ = signal_test(fc=1000, fmod=70, mdepth=1, fs=fs, d=0.2, dB=60)
+    fs = 48000
+    fmod = 70
+    time = np.linspace(0,1,fs)
+    xmod = np.sin(2*np.pi*fmod*time)
+    stimulus, _ = am_sine_generator(xmod, fs=fs, fc=1000, spl_level=60)
 
     # conversion into frequency domain
     n = len(stimulus)
-    spec, freqs = spectrum(stimulus, fs, nfft="default", window="blackman", db=False)
+    spec, freqs = comp_spectrum(stimulus, fs, nfft="default", window="blackman", db=False)
 
     # Roughness calculation
     roughness, _, _ = roughness_dw_freq(spec, freqs)
     R = {
         "name": "Roughness",
         "values": roughness,
     }
```

### Comparing `mosqito-1.1.1/tests/sq_metrics/sharpness/test_sharpness_din.py` & `mosqito-1.2.0/tests/sq_metrics/sharpness/test_sharpness_din.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from mosqito.utils import load
 from mosqito.sq_metrics import (
     sharpness_din_st,
     sharpness_din_tv,
     sharpness_din_freq,
     sharpness_din_perseg,
 )
-from mosqito.sound_level_meter.spectrum import spectrum
+from mosqito.sound_level_meter.comp_spectrum import comp_spectrum
+
 
 @pytest.fixture
 def test_signal():
     # Input signal from DIN 45692_2009E
     sig, fs = load("tests/input/broadband_570.wav", wav_calib=1)
     sig_dict = {
         "signal": sig,
@@ -123,17 +124,15 @@
     sig = test_signal["signal"]
     fs = test_signal["fs"]
 
     # Compute sharpness
     sharpness, _ = sharpness_din_perseg(sig, fs, nperseg=2**14, weighting="aures")
     sharpness, _ = sharpness_din_perseg(sig, fs, nperseg=2**14, weighting="bismarck")
     sharpness, _ = sharpness_din_perseg(sig, fs, nperseg=2**14, weighting="fastl")
-    sharpness, time_axis = sharpness_din_perseg(
-        sig, fs, nperseg=2**14, weighting="din"
-    )
+    sharpness, time_axis = sharpness_din_perseg(sig, fs, nperseg=2**14, weighting="din")
 
     # Check that the value is within the desired values +/- 5%
     # as per DIN 45692_2009E (chapter 6)
     np.testing.assert_allclose(sharpness, test_signal["S_din"], rtol=0.05)
 
 
 @pytest.mark.sharpness_din
@@ -187,15 +186,15 @@
     # Input signal from DIN 45692_2009E
     signal = {"data_file": "tests/input/broadband_570.wav", "S": test_signal["S_din"]}
 
     # Input signal
     sig = test_signal["signal"]
     fs = test_signal["fs"]
     # Compute corresponding spectrum
-    spec, freqs = spectrum(sig, fs, nfft="default", window="blackman", db=False)
+    spec, freqs = comp_spectrum(sig, fs, nfft="default", window="blackman", db=False)
 
     # Compute sharpness
     sharpness = sharpness_din_freq(spec, freqs, weighting="din")
 
     assert check_compliance(sharpness, signal)
```

### Comparing `mosqito-1.1.1/tests/sq_metrics/tonality/test_pr_ecma_freq.py` & `mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_st.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,50 @@
 # -*- coding: utf-8 -*-
 
+
 # Optional package import
 try:
     import pytest
 except ImportError:
-    raise RuntimeError(
-        "In order to perform the tests you need the 'pytest' package."
-    )
-# External import
+    raise RuntimeError("In order to perform the tests you need the 'pytest' package.")
+
 import numpy as np
 
 # Local application imports
 from mosqito.utils import load
-from mosqito.sound_level_meter.spectrum import spectrum
-from mosqito.sq_metrics import pr_ecma_freq
+from mosqito.sq_metrics import tnr_ecma_st
+
 
-@pytest.mark.pr_freq  # to skip or run PR test
-def test_pr_ecma_freq():
+@pytest.mark.tnr_st  # to skip or run PR test
+def test_tnr_ecma_st():
     """Test function for the prominence ratio calculation of an audio signal
 
-    Validation function for the "pr_ecma_freq" function with complex spectrum array
-    as input. The input signal was generated using audacity, and then the spectrum is computed using mosqito.
+    Validation function for the "tnr_ecma_st" function with stationary signal array
+    as input. The input signal was generated using audacity.
 
     Parameters
     ----------
     None
 
     Outputs
     -------
     None
     """
-    # Test signal as input for prominence ratio calculation
-    # signals generated using audacity : white noise + tones at 200 and 2000 Hz
-
-
-    signal =         {
-            "is_stationary": True,
-            "data_file": "tests/input/white_noise_442_1768_Hz_stationary.wav"
-        }
+    # Test signal as input for tone to noise ratio calculation
+    # signals generated using audacity : white noise + tones at 442 and 1768 Hz
 
+    signal = {
+        "tones freq": [442, 1768],
+        "data_file": "tests/input/white_noise_442_1768_Hz_stationary.wav",
+    }
 
     # Load signal
     audio, fs = load(signal["data_file"], wav_calib=0.01)
-    # convert to frequency domain
-    spec, freqs = spectrum(audio, fs, window='hanning', db=False)
-
-    # Compute tone-to-noise ratio
-    # 1D input
     # Compute tone-to-noise ratio
-    t_pr, pr, promi, freq = pr_ecma_freq(spec, freqs=freqs, prominence=False )
+    t_tnr, tnr, prom, freq = tnr_ecma_st(audio, fs, prominence=True)
+    np.testing.assert_almost_equal(t_tnr, 32.7142766)
+    np.testing.assert_almost_equal(freq.astype(np.int32), [442, 1768])
+    assert np.count_nonzero(prom == True) == 2
 
-    # 2D spectrum, 1D freq axis
-    spec = np.tile(spec, (4,1)).T
-    
-    t_pr, pr, promi, freq = pr_ecma_freq(spec, freqs=freqs, prominence=False )
-
-    # 2D spectrum, 2D freq axis
-    freqs = np.tile(freqs,(4,1)).T
-    t_pr, pr, promi, freq = pr_ecma_freq(spec, freqs=freqs, prominence=False )
-        
-if __name__ == "__main__":
-    test_pr_ecma_freq()
 
+if __name__ == "__main__":
+    test_tnr_ecma_st()
```

### Comparing `mosqito-1.1.1/tests/sq_metrics/tonality/test_pr_ecma_st.py` & `mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_st.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 # -*- coding: utf-8 -*-
 
 # Optional package import
 try:
     import pytest
 except ImportError:
-    raise RuntimeError(
-        "In order to perform the tests you need the 'pytest' package."
-    )
+    raise RuntimeError("In order to perform the tests you need the 'pytest' package.")
 
 import numpy as np
+
 # Local application imports
 from mosqito.utils import load
 from mosqito.sq_metrics import pr_ecma_st
 
 
 @pytest.mark.pr_st  # to skip or run PR test
 def test_pr_ecma_st():
     """Test function for the prominence ratio calculation of an audio signal
 
-    Validation function for the Audio_signal class "tone_to_noise_ecma" method with signal array
-    as input. The input signals are generated using audacity.
+    Validation function for the function pr_ecma_st. The input signals were generated using audacity.
 
     Parameters
     ----------
     None
 
     Outputs
     -------
     None
     """
     # Test signal as input for prominence ratio calculation
     # signals generated using audacity : white noise + tones at 442 and 1768 Hz
 
-    signal = {
-            "data_file": "tests/input/white_noise_442_1768_Hz_stationary.wav"
-        }
+    signal = {"data_file": "tests/input/white_noise_442_1768_Hz_stationary.wav"}
 
     # Load signal
     audio, fs = load(signal["data_file"], wav_calib=0.01)
 
     # Compute tone-to-noise ratio
     t_pr, pr, prom, freq = pr_ecma_st(audio, fs, prominence=True)
     np.testing.assert_almost_equal(t_pr, 32.20980078537321)
     np.testing.assert_almost_equal(freq.astype(np.int32), [442, 1768])
     assert np.count_nonzero(prom == True) == 2
 
 
 if __name__ == "__main__":
     test_pr_ecma_st()
-
```

### Comparing `mosqito-1.1.1/tests/sq_metrics/tonality/test_pr_ecma_tv.py` & `mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_tv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 # -*- coding: utf-8 -*-
 
 # Optional package import
 try:
     import pytest
 except ImportError:
-    raise RuntimeError(
-        "In order to perform the tests you need the 'pytest' package."
-    )
+    raise RuntimeError("In order to perform the tests you need the 'pytest' package.")
 
 import numpy as np
+
 # Local application imports
 from mosqito.utils import load
-from mosqito.sq_metrics import pr_ecma_tv
+from mosqito.sq_metrics import pr_ecma_perseg
 
 
 @pytest.mark.pr_tv  # to skip or run PR test
-def test_pr_ecma_tv():
+def test_pr_ecma_perseg():
     """Test function for the prominence ratio calculation of an audio signal
 
-    Validation function for the Audio_signal class "tone_to_noise_ecma" method with signal array
-    as input. The input signals are generated using audacity.
+    Validation function for the function pr_ecma_perseg. The input signals were generated using audacity.
 
     Parameters
     ----------
     None
 
     Outputs
     -------
     None
     """
     # Test signal as input for prominence ratio calculation
     # signals generated using audacity : white noise + tones at 442 and 1768 Hz
 
-    signal = {
-            "data_file": "tests/input/white_noise_442_1768_Hz_varying.wav"
-        }
+    signal = {"data_file": "tests/input/white_noise_442_1768_Hz_varying.wav"}
 
     # Load signal
     audio, fs = load(signal["data_file"], wav_calib=0.01)
 
     # Compute tone-to-noise ratio
-    t_pr, pr, prom, freq, time = pr_ecma_tv(audio, fs, prominence=True)
+    t_pr, pr, prom, freq, time = pr_ecma_perseg(audio, fs, prominence=True)
     np.testing.assert_almost_equal(max(t_pr), 34.02082433185258)
-    assert pr[np.argmin(np.abs(freq-442)),:].all() != np.nan
-    assert pr[np.argmin(np.abs(freq-1768)),2:3].all() != np.nan
+    assert pr[np.argmin(np.abs(freq - 442)), :].all() != np.nan
+    assert pr[np.argmin(np.abs(freq - 1768)), 2:3].all() != np.nan
     assert np.count_nonzero(prom == True) == 8
 
 
-
 if __name__ == "__main__":
-    test_pr_ecma_tv()
-
-
+    test_pr_ecma_perseg()
```

### Comparing `mosqito-1.1.1/tests/sq_metrics/tonality/test_tnr_ecma_freq.py` & `mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_freq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 
 # Optional package import
 try:
     import pytest
 except ImportError:
-    raise RuntimeError(
-        "In order to perform the tests you need the 'pytest' package."
-    )
+    raise RuntimeError("In order to perform the tests you need the 'pytest' package.")
 
 # External import
 import numpy as np
 
 # Local application imports
 from mosqito.utils import load
-from mosqito.sound_level_meter.spectrum import spectrum
+from mosqito.sound_level_meter.comp_spectrum import comp_spectrum
 from mosqito.sq_metrics import tnr_ecma_freq
 
+
 @pytest.mark.tnr_freq  # to skip or run TNR test
 def test_tnr_ecma_freq():
     """Test function for the prominence ratio calculation of an audio signal
 
     Validation function for the "tnr_ecma_freq" function with complex spectrum array
     as input. The input signal was generated using audacity, and then the spectrum is computed using mosqito.
 
@@ -30,35 +29,33 @@
     Outputs
     -------
     None
     """
     # Test signal as input for prominence ratio calculation
     # signals generated using audacity : white noise + tones at 200 and 2000 Hz
 
-
-    signal =     {
-            "is_stationary": True,
-            "data_file": "tests/input/white_noise_442_1768_Hz_stationary.wav"
-        }
-    
+    signal = {
+        "is_stationary": True,
+        "data_file": "tests/input/white_noise_442_1768_Hz_stationary.wav",
+    }
 
     # Load signal
     audio, fs = load(signal["data_file"], wav_calib=0.01)
     # convert to frequency domain
-    spec, freqs = spectrum(audio, fs, window='hanning', db=False)
+    spec, freqs = comp_spectrum(audio, fs, window='hanning', db=False)
 
     # 1D input
     # Compute tone-to-noise ratio
-    t_tnr, tnr, promi, freq = tnr_ecma_freq(spec, freqs=freqs, prominence=False )
+    t_tnr, tnr, promi, freq = tnr_ecma_freq(spec, freqs=freqs, prominence=False)
 
     # 2D spectrum, 1D freq axis
-    spec = np.tile(spec, (4,1)).T
-    
-    t_tnr, tnr, promi, freq = tnr_ecma_freq(spec, freqs=freqs, prominence=False )
+    spec = np.tile(spec, (4, 1)).T
+
+    t_tnr, tnr, promi, freq = tnr_ecma_freq(spec, freqs=freqs, prominence=False)
 
     # 2D spectrum, 2D freq axis
-    freqs = np.tile(freqs,(4,1)).T
-    t_tnr, tnr, promi, freq = tnr_ecma_freq(spec, freqs=freqs, prominence=False )
+    freqs = np.tile(freqs, (4, 1)).T
+    t_tnr, tnr, promi, freq = tnr_ecma_freq(spec, freqs=freqs, prominence=False)
 
 
 if __name__ == "__main__":
     test_tnr_ecma_freq()
```

### Comparing `mosqito-1.1.1/tests/sq_metrics/tonality/test_tnr_ecma_st.py` & `mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_tv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 # -*- coding: utf-8 -*-
-
-
 # Optional package import
 try:
     import pytest
 except ImportError:
-    raise RuntimeError(
-        "In order to perform the tests you need the 'pytest' package."
-    )
+    raise RuntimeError("In order to perform the tests you need the 'pytest' package.")
 
 import numpy as np
+
 # Local application imports
 from mosqito.utils import load
-from mosqito.sq_metrics import tnr_ecma_st
+from mosqito.sq_metrics import tnr_ecma_perseg
 
 
-@pytest.mark.tnr_st  # to skip or run PR test
-def test_tnr_ecma_st():
+@pytest.mark.tnr_tv  # to skip or run TNR test
+def test_tnr_ecma_perseg():
     """Test function for the prominence ratio calculation of an audio signal
 
-    Validation function for the "tnr_ecma_st" function with stationary signal array
+    Validation function for the "tnr_ecma_perseg" function with time-varying signal array
     as input. The input signal was generated using audacity.
 
     Parameters
     ----------
     None
 
     Outputs
     -------
     None
     """
-    # Test signal as input for tone to noise ratio calculation
+    # Test signal as input for prominence ratio calculation
     # signals generated using audacity : white noise + tones at 442 and 1768 Hz
 
-    signal =  {
-            "tones freq": [442, 1768],
-            "data_file": "tests/input/white_noise_442_1768_Hz_stationary.wav"
-        }
+    signal = {
+        "freq": [442, 1768],
+        "data_file": "tests/input/white_noise_442_1768_Hz_varying.wav",
+    }
 
     # Load signal
     audio, fs = load(signal["data_file"], wav_calib=0.01)
+
     # Compute tone-to-noise ratio
-    t_tnr, tnr, prom, freq = tnr_ecma_st(audio, fs, prominence=True)
-    np.testing.assert_almost_equal(t_tnr, 32.7142766)
-    np.testing.assert_almost_equal(freq.astype(np.int32), [442, 1768])
-    assert np.count_nonzero(prom == True) == 2
-        
-if __name__ == "__main__":
-    test_tnr_ecma_st()
+    t_tnr, tnr, prom, freq, time = tnr_ecma_perseg(audio, fs, prominence=True)
+    np.testing.assert_almost_equal(max(t_tnr), 34.710964273840155)
+    assert tnr[np.argmin(np.abs(freq - 442)), :].all() != np.nan
+    assert tnr[np.argmin(np.abs(freq - 1768)), 2:3].all() != np.nan
+    assert np.count_nonzero(prom == True) == 8
 
 
+if __name__ == "__main__":
+    test_tnr_ecma_perseg()
```

