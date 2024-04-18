# Comparing `tmp/dtscalibration-3.0.2.tar.gz` & `tmp/dtscalibration-3.0.3.tar.gz`

## Comparing `dtscalibration-3.0.2.tar` & `dtscalibration-3.0.3.tar`

### file list

```diff
@@ -1,139 +1,139 @@
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/.bumpversion.cfg
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/.git-blame-ignore-revs
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/.readthedocs.yml
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/.zenodo.json
--rw-r--r--   0        0        0    12650 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/CHANGELOG.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/CITATION.cff
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/authors.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/changelog.rst
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/contributing.rst
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/index.rst
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/learn_by_examples.rst
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/readme.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/01Load_xml_measurement_files.ipynb
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/03Define_sections.ipynb
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/04Calculate_variance_Stokes.ipynb
--rw-r--r--   0        0        0    10323 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/07Calibrate_single_ended.ipynb
--rw-r--r--   0        0        0    17432 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/08Calibrate_double_ended.ipynb
--rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/09Import_timeseries.ipynb
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/10Align_double_ended_measurements.ipynb
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/11Merge_single_measurements_into_double.ipynb
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/12Datastore_from_numpy_arrays.ipynb
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/13Fixed_parameter_calibration.ipynb
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/14Lossy_splices.ipynb
--rw-r--r--   0        0        0     7747 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/15Matching_sections.ipynb
--rw-r--r--   0        0        0    16460 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/16Averaging_temperatures.ipynb
--rw-r--r--   0        0        0     8040 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/17Temperature_uncertainty_single_ended.ipynb
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/A2Load_sensornet_files.ipynb
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/A3Load_ap_sensing_files.ipynb
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/notebooks/A4Load_sensortran_files.ipynb
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/docs/reference/index.rst
--rw-r--r--   0        0        0    63280 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/examples/Added uncertainty from fixing parameters.pdf
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/examples/README.md
--rw-r--r--   0        0        0   133564 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/examples/temperature_variance_from_stokes.pdf
--rw-r--r--   0        0        0  1407624 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/examples/conference presentations/EGU2019_poster_dtscalibration.pdf
--rw-r--r--   0        0        0  2086568 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/__init__.py
--rw-r--r--   0        0        0    80227 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/calibrate_utils.py
--rw-r--r--   0        0        0   118552 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/dts_accessor.py
--rw-r--r--   0        0        0    45661 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/dts_accessor_utils.py
--rw-r--r--   0        0        0    23501 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/plot.py
--rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/variance_helpers.py
--rw-r--r--   0        0        0    21807 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/variance_stokes.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/calibration/section_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/__init__.py
--rw-r--r--   0        0        0    12289 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/apsensing.py
--rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/sensornet.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/sensortran.py
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/silixa.py
--rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/src/dtscalibration/io/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/__init__.py
--rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/test_averaging.py
--rw-r--r--   0        0        0    20532 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/test_datastore.py
--rw-r--r--   0        0        0    78659 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/test_dtscalibration.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/test_examples.py
--rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/test_variance_stokes.py
--rw-r--r--   0        0        0   677982 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml
--rw-r--r--   0        0        0   678035 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml
--rw-r--r--   0        0        0   678009 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/docs_notebooks/01Not_working.ipynb
--rwxr-xr-x   0        0        0   171342 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921112245510.xml
--rwxr-xr-x   0        0        0   171341 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921112746818.xml
--rwxr-xr-x   0        0        0   171310 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921113248085.xml
--rwxr-xr-x   0        0        0   129624 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014052498.xml
--rwxr-xr-x   0        0        0   129585 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014057119.xml
--rwxr-xr-x   0        0        0   129431 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014101652.xml
--rwxr-xr-x   0        0        0   129452 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014106243.xml
--rwxr-xr-x   0        0        0   129559 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014110917.xml
--rwxr-xr-x   0        0        0   129482 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014115480.xml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_ended2/info.txt
--rw-r--r--   0        0        0   436539 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml
--rw-r--r--   0        0        0   436736 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml
--rw-r--r--   0        0        0   436525 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml
--rw-r--r--   0        0        0   436669 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml
--rw-r--r--   0        0        0   436527 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml
--rw-r--r--   0        0        0   436478 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml
--rw-r--r--   0        0        0   436371 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml
--rw-r--r--   0        0        0   436475 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml
--rw-r--r--   0        0        0   436421 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml
--rw-r--r--   0        0        0   436359 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml
--rw-r--r--   0        0        0   436400 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml
--rw-r--r--   0        0        0   436238 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml
--rwxr-xr-x   0        0        0    20057 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv
--rwxr-xr-x   0        0        0    20028 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv
--rwxr-xr-x   0        0        0    20086 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv
--rw-r--r--   0        0        0    47136 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf
--rw-r--r--   0        0        0    47126 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf
--rw-r--r--   0        0        0    47113 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf
--rw-r--r--   0        0        0    47107 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf
--rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf
--rw-r--r--   0        0        0    64983 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf
--rw-r--r--   0        0        0    65031 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf
--rw-r--r--   0        0        0    65017 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf
--rw-r--r--   0        0        0    65058 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf
--rw-r--r--   0        0        0    65029 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf
--rw-r--r--   0        0        0    65043 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf
--rw-r--r--   0        0        0    65018 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf
--rw-r--r--   0        0        0    48160 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf
--rw-r--r--   0        0        0    48206 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf
--rw-r--r--   0        0        0    48196 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf
--rw-r--r--   0        0        0    48174 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf
--rw-r--r--   0        0        0    48163 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf
--rw-r--r--   0        0        0   126331 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf
--rw-r--r--   0        0        0   126323 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf
--rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat
--rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat
--rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat
--rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat
--rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat
--rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat
--rw-r--r--   0        0        0   164764 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060301031.xml
--rw-r--r--   0        0        0   164730 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060342281.xml
--rw-r--r--   0        0        0   164757 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060423515.xml
--rw-r--r--   0        0        0   164679 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060504750.xml
--rw-r--r--   0        0        0   164785 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060545968.xml
--rw-r--r--   0        0        0   164691 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060627218.xml
--rw-r--r--   0        0        0   164784 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060708453.xml
--rw-r--r--   0        0        0   215137 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml
--rw-r--r--   0        0        0   215082 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml
--rw-r--r--   0        0        0   215091 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml
--rw-r--r--   0        0        0   215114 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml
--rw-r--r--   0        0        0   215119 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml
--rw-r--r--   0        0        0   286652 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml
--rwxr-xr-x   0        0        0    88932 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132202074.xml
--rwxr-xr-x   0        0        0    88936 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132232903.xml
--rwxr-xr-x   0        0        0    88888 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132303723.xml
--rw-r--r--   0        0        0   166974 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/zipped data/double_ended.zip
--rw-r--r--   0        0        0   255063 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/zipped data/double_ended2.zip
--rw-r--r--   0        0        0  1508174 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/zipped data/double_single_ended.zip
--rw-r--r--   0        0        0   260862 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/zipped data/silixa_v4.5.zip
--rw-r--r--   0        0        0    78779 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/tests/data/zipped data/single_ended.zip
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/.gitignore
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/AUTHORS.rst
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/LICENSE
--rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/README.rst
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 dtscalibration-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/.bumpversion.cfg
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/.readthedocs.yml
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/.zenodo.json
+-rw-r--r--   0        0        0    13015 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/CHANGELOG.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/CITATION.cff
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/authors.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/changelog.rst
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/contributing.rst
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/index.rst
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/learn_by_examples.rst
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/readme.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/01Load_xml_measurement_files.ipynb
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/03Define_sections.ipynb
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/04Calculate_variance_Stokes.ipynb
+-rw-r--r--   0        0        0    10323 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/07Calibrate_single_ended.ipynb
+-rw-r--r--   0        0        0    17432 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/08Calibrate_double_ended.ipynb
+-rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/09Import_timeseries.ipynb
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/10Align_double_ended_measurements.ipynb
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/11Merge_single_measurements_into_double.ipynb
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/12Datastore_from_numpy_arrays.ipynb
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/13Fixed_parameter_calibration.ipynb
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/14Lossy_splices.ipynb
+-rw-r--r--   0        0        0     7747 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/15Matching_sections.ipynb
+-rw-r--r--   0        0        0    16460 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/16Averaging_temperatures.ipynb
+-rw-r--r--   0        0        0     8040 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/17Temperature_uncertainty_single_ended.ipynb
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/A2Load_sensornet_files.ipynb
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/A3Load_ap_sensing_files.ipynb
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/notebooks/A4Load_sensortran_files.ipynb
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/docs/reference/index.rst
+-rw-r--r--   0        0        0    63280 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/examples/Added uncertainty from fixing parameters.pdf
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/examples/README.md
+-rw-r--r--   0        0        0   133564 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/examples/temperature_variance_from_stokes.pdf
+-rw-r--r--   0        0        0  1407624 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/examples/conference presentations/EGU2019_poster_dtscalibration.pdf
+-rw-r--r--   0        0        0  2086568 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/__init__.py
+-rw-r--r--   0        0        0    80227 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/calibrate_utils.py
+-rw-r--r--   0        0        0   118552 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/dts_accessor.py
+-rw-r--r--   0        0        0    45903 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/dts_accessor_utils.py
+-rw-r--r--   0        0        0    23501 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/plot.py
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/variance_helpers.py
+-rw-r--r--   0        0        0    21807 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/variance_stokes.py
+-rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/calibration/section_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/io/__init__.py
+-rw-r--r--   0        0        0    12289 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/io/apsensing.py
+-rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/io/sensornet.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/io/sensortran.py
+-rw-r--r--   0        0        0    25250 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/io/silixa.py
+-rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/src/dtscalibration/io/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/test_averaging.py
+-rw-r--r--   0        0        0    20532 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/test_datastore.py
+-rw-r--r--   0        0        0    78659 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/test_dtscalibration.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/test_examples.py
+-rw-r--r--   0        0        0    28356 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/test_variance_stokes.py
+-rw-r--r--   0        0        0   677982 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml
+-rw-r--r--   0        0        0   678035 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml
+-rw-r--r--   0        0        0   678009 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/docs_notebooks/01Not_working.ipynb
+-rwxr-xr-x   0        0        0   171342 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_ended/channel 1_20170921112245510.xml
+-rwxr-xr-x   0        0        0   171341 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_ended/channel 1_20170921112746818.xml
+-rwxr-xr-x   0        0        0   171310 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_ended/channel 1_20170921113248085.xml
+-rwxr-xr-x   0        0        0   129624 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014052498.xml
+-rwxr-xr-x   0        0        0   129585 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014057119.xml
+-rwxr-xr-x   0        0        0   129431 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014101652.xml
+-rwxr-xr-x   0        0        0   129452 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014106243.xml
+-rwxr-xr-x   0        0        0   129559 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014110917.xml
+-rwxr-xr-x   0        0        0   129482 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014115480.xml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_ended2/info.txt
+-rw-r--r--   0        0        0   436539 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml
+-rw-r--r--   0        0        0   436736 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml
+-rw-r--r--   0        0        0   436525 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml
+-rw-r--r--   0        0        0   436669 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml
+-rw-r--r--   0        0        0   436527 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml
+-rw-r--r--   0        0        0   436478 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml
+-rw-r--r--   0        0        0   436371 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml
+-rw-r--r--   0        0        0   436475 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml
+-rw-r--r--   0        0        0   436421 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml
+-rw-r--r--   0        0        0   436359 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml
+-rw-r--r--   0        0        0   436400 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml
+-rw-r--r--   0        0        0   436238 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml
+-rwxr-xr-x   0        0        0    20057 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv
+-rwxr-xr-x   0        0        0    20028 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv
+-rwxr-xr-x   0        0        0    20086 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv
+-rw-r--r--   0        0        0    47136 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf
+-rw-r--r--   0        0        0    47126 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf
+-rw-r--r--   0        0        0    47113 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf
+-rw-r--r--   0        0        0    47107 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf
+-rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf
+-rw-r--r--   0        0        0    64983 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf
+-rw-r--r--   0        0        0    65031 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf
+-rw-r--r--   0        0        0    65017 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf
+-rw-r--r--   0        0        0    65058 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf
+-rw-r--r--   0        0        0    65029 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf
+-rw-r--r--   0        0        0    65043 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf
+-rw-r--r--   0        0        0    65018 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf
+-rw-r--r--   0        0        0    48160 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf
+-rw-r--r--   0        0        0    48206 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf
+-rw-r--r--   0        0        0    48196 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf
+-rw-r--r--   0        0        0    48174 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf
+-rw-r--r--   0        0        0    48163 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf
+-rw-r--r--   0        0        0   126331 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf
+-rw-r--r--   0        0        0   126323 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat
+-rw-r--r--   0        0        0   164764 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060301031.xml
+-rw-r--r--   0        0        0   164730 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060342281.xml
+-rw-r--r--   0        0        0   164757 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060423515.xml
+-rw-r--r--   0        0        0   164679 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060504750.xml
+-rw-r--r--   0        0        0   164785 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060545968.xml
+-rw-r--r--   0        0        0   164691 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060627218.xml
+-rw-r--r--   0        0        0   164784 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060708453.xml
+-rw-r--r--   0        0        0   215137 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml
+-rw-r--r--   0        0        0   215082 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml
+-rw-r--r--   0        0        0   215091 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml
+-rw-r--r--   0        0        0   215114 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml
+-rw-r--r--   0        0        0   215119 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml
+-rw-r--r--   0        0        0   286652 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml
+-rwxr-xr-x   0        0        0    88932 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/single_ended/channel 2_20180504132202074.xml
+-rwxr-xr-x   0        0        0    88936 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/single_ended/channel 2_20180504132232903.xml
+-rwxr-xr-x   0        0        0    88888 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/single_ended/channel 2_20180504132303723.xml
+-rw-r--r--   0        0        0   166974 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/zipped data/double_ended.zip
+-rw-r--r--   0        0        0   255063 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/zipped data/double_ended2.zip
+-rw-r--r--   0        0        0  1508174 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/zipped data/double_single_ended.zip
+-rw-r--r--   0        0        0   260862 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/zipped data/silixa_v4.5.zip
+-rw-r--r--   0        0        0    78779 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/tests/data/zipped data/single_ended.zip
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/.gitignore
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/AUTHORS.rst
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/LICENSE
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/README.rst
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 dtscalibration-3.0.3/PKG-INFO
```

### Comparing `dtscalibration-3.0.2/.zenodo.json` & `dtscalibration-3.0.3/.zenodo.json`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/CHANGELOG.rst` & `dtscalibration-3.0.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 
 Changelog
 =========
 
+3.0.3 (2024-04-18)
+---
+
+Fixed 
+
+* Improved error message when some variables cannot be shifted by the suggest_shift_double_ended function.
+
+Changed:
+
+* [dev] Moved to Ruff instead of isort for import sorting
+
+
+3.0.2 (2024-04-13)
+---
+
+Fixed
+
+* Bumpversion configuration was incorrect since v3.0.0. Therefore the 3.0.1 release failed. This is a re-release of 3.0.1:
+
 3.0.1 (2024-04-13)
 ---
 
 Fixed
 
 * Oryx v4 double ended could have the backward measurements incorrectly cut off during loading.
```

### Comparing `dtscalibration-3.0.2/CITATION.cff` & `dtscalibration-3.0.3/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,9 @@
   - calibration
   - Python
 cff-version: "1.0.3"
 doi: "10.5281/zenodo.1410097"
 license: "BSD-3-Clause"
 repository-code: "https://github.com/dtscalibration/python-dts-calibration"
 title: "Python distributed temperature sensing calibration"
-version: "v3.0.2"
+version: "v3.0.3"
 url: "https://python-dts-calibration.readthedocs.io"
```

### Comparing `dtscalibration-3.0.2/CONTRIBUTING.rst` & `dtscalibration-3.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/conf.py` & `dtscalibration-3.0.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 source_suffix = [".rst", ".md"]
 master_doc = "index"
 project = "dtscalibration"
 year = str(date.today().year)
 author = "Bas des Tombe and Bart Schilperoort"
 copyright = f"{year}, {author}"
-version = release = "3.0.2"
+version = release = "3.0.3"
 
 pygments_style = "trac"
 templates_path = [".", sphinx_autosummary_accessors.templates_path]
 extlinks = {
     "issue": (
         "https://github.com/dtscalibration/python-dts-calibration/issues" "/%s",
         "#",
```

### Comparing `dtscalibration-3.0.2/docs/learn_by_examples.rst` & `dtscalibration-3.0.3/docs/learn_by_examples.rst`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/01Load_xml_measurement_files.ipynb` & `dtscalibration-3.0.3/docs/notebooks/01Load_xml_measurement_files.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/03Define_sections.ipynb` & `dtscalibration-3.0.3/docs/notebooks/03Define_sections.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/04Calculate_variance_Stokes.ipynb` & `dtscalibration-3.0.3/docs/notebooks/04Calculate_variance_Stokes.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/07Calibrate_single_ended.ipynb` & `dtscalibration-3.0.3/docs/notebooks/07Calibrate_single_ended.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/08Calibrate_double_ended.ipynb` & `dtscalibration-3.0.3/docs/notebooks/08Calibrate_double_ended.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/09Import_timeseries.ipynb` & `dtscalibration-3.0.3/docs/notebooks/09Import_timeseries.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/10Align_double_ended_measurements.ipynb` & `dtscalibration-3.0.3/docs/notebooks/10Align_double_ended_measurements.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/11Merge_single_measurements_into_double.ipynb` & `dtscalibration-3.0.3/docs/notebooks/11Merge_single_measurements_into_double.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/12Datastore_from_numpy_arrays.ipynb` & `dtscalibration-3.0.3/docs/notebooks/12Datastore_from_numpy_arrays.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/13Fixed_parameter_calibration.ipynb` & `dtscalibration-3.0.3/docs/notebooks/13Fixed_parameter_calibration.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/14Lossy_splices.ipynb` & `dtscalibration-3.0.3/docs/notebooks/14Lossy_splices.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/15Matching_sections.ipynb` & `dtscalibration-3.0.3/docs/notebooks/15Matching_sections.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/16Averaging_temperatures.ipynb` & `dtscalibration-3.0.3/docs/notebooks/16Averaging_temperatures.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/17Temperature_uncertainty_single_ended.ipynb` & `dtscalibration-3.0.3/docs/notebooks/17Temperature_uncertainty_single_ended.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/A2Load_sensornet_files.ipynb` & `dtscalibration-3.0.3/docs/notebooks/A2Load_sensornet_files.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/A3Load_ap_sensing_files.ipynb` & `dtscalibration-3.0.3/docs/notebooks/A3Load_ap_sensing_files.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/notebooks/A4Load_sensortran_files.ipynb` & `dtscalibration-3.0.3/docs/notebooks/A4Load_sensortran_files.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/docs/reference/index.rst` & `dtscalibration-3.0.3/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/examples/Added uncertainty from fixing parameters.pdf` & `dtscalibration-3.0.3/examples/Added uncertainty from fixing parameters.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/examples/temperature_variance_from_stokes.pdf` & `dtscalibration-3.0.3/examples/temperature_variance_from_stokes.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/examples/conference presentations/EGU2019_poster_dtscalibration.pdf` & `dtscalibration-3.0.3/examples/conference presentations/EGU2019_poster_dtscalibration.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf` & `dtscalibration-3.0.3/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/__init__.py` & `dtscalibration-3.0.3/src/dtscalibration/__init__.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/calibrate_utils.py` & `dtscalibration-3.0.3/src/dtscalibration/calibrate_utils.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/dts_accessor.py` & `dtscalibration-3.0.3/src/dtscalibration/dts_accessor.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/dts_accessor_utils.py` & `dtscalibration-3.0.3/src/dtscalibration/dts_accessor_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -952,15 +952,20 @@
     new_data = (("st", st), ("ast", ast), ("rst", rst), ("rast", rast))
 
     for k, v in new_data:
         d2_data[k] = xr.DataArray(data=v, dims=ds[k].dims, attrs=ds[k].attrs)
 
     not_included = [k for k in ds.data_vars if k not in d2_data]
     if not_included and verbose:
-        print("I dont know what to do with the following data", not_included)
+        msg = (
+            "The following variables could not be shifted and are not included in the "
+            f"new dataset: {not_included}. You can silence this warning with the "
+            "keyword argument `verbose=False`."
+        )
+        warnings.warn(msg, UserWarning)
 
     return xr.Dataset(data_vars=d2_data, coords=d2_coords, attrs=ds.attrs)
 
 
 def suggest_cable_shift_double_ended(
     ds: xr.Dataset,
     irange: npt.NDArray[np.int_],
@@ -1058,15 +1063,15 @@
     if plot_result:
         if fig_kwargs is None:
             fig_kwargs = {}
 
         f, (ax0, ax1) = plt.subplots(2, 1, sharex=False, **fig_kwargs)
         f.suptitle(f"best shift is {ishift1} or {ishift2}")
 
-        dt = ds.isel(time=0)
+        dt = ds.isel(time=0)[["st", "ast", "rst", "rast", "x"]]
         x = dt["x"].data
         y = dt["st"].data
         ax0.plot(x, y, label="ST original")
         y = dt["rst"].data
         ax0.plot(x, y, label="REV-ST original")
 
         dtsh1 = shift_double_ended(dt, ishift1)
```

### Comparing `dtscalibration-3.0.2/src/dtscalibration/plot.py` & `dtscalibration-3.0.3/src/dtscalibration/plot.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/variance_helpers.py` & `dtscalibration-3.0.3/src/dtscalibration/variance_helpers.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/variance_stokes.py` & `dtscalibration-3.0.3/src/dtscalibration/variance_stokes.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/calibration/section_utils.py` & `dtscalibration-3.0.3/src/dtscalibration/calibration/section_utils.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/io/apsensing.py` & `dtscalibration-3.0.3/src/dtscalibration/io/apsensing.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/io/sensornet.py` & `dtscalibration-3.0.3/src/dtscalibration/io/sensornet.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/io/sensortran.py` & `dtscalibration-3.0.3/src/dtscalibration/io/sensortran.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/src/dtscalibration/io/silixa.py` & `dtscalibration-3.0.3/src/dtscalibration/io/silixa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import warnings
 from pathlib import Path
 from xml.etree import ElementTree
 
 import dask
 import dask.array as da
 import numpy as np
 import pandas as pd
@@ -93,15 +94,19 @@
         )
 
     else:
         raise NotImplementedError(
             "Silixa xml version " + f"{xml_version} not implemented"
         )
 
-    ds = xr.Dataset(data_vars=data_vars, coords=coords, attrs=attrs, **kwargs)
+    with warnings.catch_warnings():
+        warnings.filterwarnings(
+            "ignore", message="Converting non-nanosecond precision timedelta"
+        )
+        ds = xr.Dataset(data_vars=data_vars, coords=coords, attrs=attrs, **kwargs)
     return ds
 
 
 def silixa_xml_version_check(filepathlist):
     """Function which tests which version of xml files have to be read.
 
     Parameters
```

### Comparing `dtscalibration-3.0.2/src/dtscalibration/io/utils.py` & `dtscalibration-3.0.3/src/dtscalibration/io/utils.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/test_averaging.py` & `dtscalibration-3.0.3/tests/test_averaging.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/test_datastore.py` & `dtscalibration-3.0.3/tests/test_datastore.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/test_dtscalibration.py` & `dtscalibration-3.0.3/tests/test_dtscalibration.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/test_examples.py` & `dtscalibration-3.0.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/test_variance_stokes.py` & `dtscalibration-3.0.3/tests/test_variance_stokes.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml` & `dtscalibration-3.0.3/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml` & `dtscalibration-3.0.3/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml` & `dtscalibration-3.0.3/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/docs_notebooks/01Not_working.ipynb` & `dtscalibration-3.0.3/tests/data/docs_notebooks/01Not_working.ipynb`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921112245510.xml` & `dtscalibration-3.0.3/tests/data/double_ended/channel 1_20170921112245510.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921112746818.xml` & `dtscalibration-3.0.3/tests/data/double_ended/channel 1_20170921112746818.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_ended/channel 1_20170921113248085.xml` & `dtscalibration-3.0.3/tests/data/double_ended/channel 1_20170921113248085.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014052498.xml` & `dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014052498.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014057119.xml` & `dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014057119.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014101652.xml` & `dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014101652.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014106243.xml` & `dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014106243.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014110917.xml` & `dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014110917.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_ended2/channel 1_20180328014115480.xml` & `dtscalibration-3.0.3/tests/data/double_ended2/channel 1_20180328014115480.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml` & `dtscalibration-3.0.3/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv` & `dtscalibration-3.0.3/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv` & `dtscalibration-3.0.3/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv` & `dtscalibration-3.0.3/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf` & `dtscalibration-3.0.3/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat` & `dtscalibration-3.0.3/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat` & `dtscalibration-3.0.3/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat` & `dtscalibration-3.0.3/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat` & `dtscalibration-3.0.3/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat` & `dtscalibration-3.0.3/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat` & `dtscalibration-3.0.3/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060301031.xml` & `dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060301031.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060342281.xml` & `dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060342281.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060423515.xml` & `dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060423515.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060504750.xml` & `dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060504750.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060545968.xml` & `dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060545968.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060627218.xml` & `dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060627218.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v4.5/channel 3_20151002060708453.xml` & `dtscalibration-3.0.3/tests/data/silixa_v4.5/channel 3_20151002060708453.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml` & `dtscalibration-3.0.3/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml` & `dtscalibration-3.0.3/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml` & `dtscalibration-3.0.3/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml` & `dtscalibration-3.0.3/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml` & `dtscalibration-3.0.3/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml` & `dtscalibration-3.0.3/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132202074.xml` & `dtscalibration-3.0.3/tests/data/single_ended/channel 2_20180504132202074.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132232903.xml` & `dtscalibration-3.0.3/tests/data/single_ended/channel 2_20180504132232903.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/single_ended/channel 2_20180504132303723.xml` & `dtscalibration-3.0.3/tests/data/single_ended/channel 2_20180504132303723.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/zipped data/double_ended.zip` & `dtscalibration-3.0.3/tests/data/zipped data/double_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/zipped data/double_ended2.zip` & `dtscalibration-3.0.3/tests/data/zipped data/double_ended2.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/zipped data/double_single_ended.zip` & `dtscalibration-3.0.3/tests/data/zipped data/double_single_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/zipped data/silixa_v4.5.zip` & `dtscalibration-3.0.3/tests/data/zipped data/silixa_v4.5.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/tests/data/zipped data/single_ended.zip` & `dtscalibration-3.0.3/tests/data/zipped data/single_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/.gitignore` & `dtscalibration-3.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/LICENSE` & `dtscalibration-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dtscalibration-3.0.2/README.rst` & `dtscalibration-3.0.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     :target: https://github.com/dtscalibration/python-dts-calibration/actions/workflows/build.yml
     :alt: Test Status
 
 .. |version| image:: https://img.shields.io/pypi/v/dtscalibration.svg
     :alt: PyPI Package latest release
     :target: https://pypi.python.org/pypi/dtscalibration
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v3.0.2.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v3.0.3.svg
     :alt: Commits since latest release
     :target: https://github.com/dtscalibration/python-dts-calibration/compare/v1.1.1...main
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/dtscalibration.svg
     :alt: PyPI Wheel
     :target: https://pypi.python.org/pypi/dtscalibration
 
@@ -49,16 +49,15 @@
    :alt: Interactively run the example notebooks online
    :target: https://mybinder.org/v2/gh/dtscalibration/python-dts-calibration/main?labpath=docs%2Fnotebooks
 
 .. end-badges
 
 A Python package to load Distributed Temperature Sensing files, perform a calibration, and plot the result. A detailed description of the calibration procedure can be found at https://doi.org/10.3390/s20082235 .
 
-* Free software: BSD 3-Clause License
-
+Do you have questions, ideas or just want to say hi? Please leave a message on the ` discussions page <https://github.com/dtscalibration/python-dts-calibration/discussions>`_!
 
 Installation
 ============
 
 .. code-block:: zsh
 
     pip install dtscalibration
@@ -74,17 +73,17 @@
 DTS measures temperature by calibrating backscatter measurements to sections with a known temperature. DTS devices provide a simple interface to perform a limited calibration. Re-calibrating your measurements with this Python package gives you better temperature estimates and additional options.
 
 * Advanced calibration routine
    * Supports `single <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/07Calibrate_single_ended.ipynb>`_- and `double-ended <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/08Calibrate_double_ended.ipynb>`_ setups
    * Compute uncertainty of the calibrated temperature
    * All measurements are used to estimate parameter values that are constant over time.
    * Weighted least-squares calibration
-   * `Fixing parameters to a previously determined value <../main/examples/notebooks/13Fixed_parameter_calibration.ipynb>`_
-   * `(Asymmetric) step loss correction <../main/examples/notebooks/14Lossy_splices.ipynb>`_ so that fiber connectors can be used instead of welds/splices.
-   * `Matching temperature sections <../main/examples/notebooks/15Matching_sections.ipynb>`_ to support J-configurations
+   * `Fixing parameters to a previously determined value <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/13Fixed_parameter_calibration.ipynb>`_
+   * `(Asymmetric) step loss correction <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/14Lossy_splices.ipynb>`_ so that fiber connectors can be used instead of welds/splices.
+   * `Matching temperature sections <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/15Matching_sections.ipynb>`_ to support J-configurations
 * Dynamic reference section definition
 * Tools for merging and aligning double-ended setups
 * Data formats of most manufacturers are supported
 
 Devices currently supported
 ===========================
 * Silixa Ltd.: **Ultima** & **XT-DTS** .xml files *(up to version 8.1)*
```

### Comparing `dtscalibration-3.0.2/pyproject.toml` & `dtscalibration-3.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 packages = ["src/dtscalibration"]
 
 [tool.hatch.publish.index]
 disable = true  # Requires confirmation when publishing to pypi.
 
 [project]
 name = "dtscalibration"
-version = "3.0.2"
+version = "3.0.3"
 description = "Load Distributed Temperature Sensing (DTS) files, calibrate the temperature and estimate its uncertainty."
 readme = "README.rst"
 license = "BSD-3-Clause"
 requires-python = ">=3.9, <3.12"
 authors = [
   {name = "Bas des Tombe, Bart Schilperoort"},
 ]
@@ -67,15 +67,14 @@
 ]
 
 [project.optional-dependencies]
 dev = [
     "hatch",
     "bump2version",
     "ruff",
-    "isort",
     "black[jupyter]",   # for formatting
     "mypy",             # for type checking
     "types-PyYAML",     # for pyyaml types
     "types-xmltodict",  # for xmltodict types
     "pandas-stubs",     # for pandas types
     "pytest",
     "pytest-cov",       # for coverage
@@ -104,18 +103,17 @@
 [tool.hatch.envs.default]
 features = ["dev"]
 
 [tool.hatch.envs.default.scripts]
 lint = [
   "ruff check src/ tests/ examples/",
   "black --check docs/notebooks",
-  "isort --check-only --diff src/ tests/ examples/",
   "mypy src/",
 ]
-format = ["isort src/ tests/ examples/", "ruff check src/ tests/ examples/ --fix", "ruff format src/ tests/ examples/", "black docs/notebooks", "lint",]
+format = ["ruff check src/ tests/ examples/ --fix", "ruff format src/ tests/ examples/", "black docs/notebooks", "lint",]
 test = ["pytest ./src/ ./tests/",]
 fast-test = ["pytest ./tests/ -m \"not slow\"",]
 coverage = [
   "pytest --cov --cov-report term --cov-report xml --cov-branch --junitxml=xunit-result.xml tests/",
 ]
 
 [tool.hatch.envs.docs]
@@ -149,31 +147,28 @@
   # "D",  # pydocstyle
   # "C90",  # mccabe complexity
   # "N",  # PEP8-naming
   "UP",  # pyupgrade (upgrade syntax to current syntax)
   "PLE",  # Pylint error https://github.com/charliermarsh/ruff#error-ple
   # "PLR",  # Pylint refactor (e.g. too-many-arguments)
   "PLW",  # Pylint warning (useless-else-on-loop)
-  # "I",  # isort
+  "I",  # isort
   "SIM",  # flake8-simplify
 
 ]
 extend-select = [
   #"D401",  # First line should be in imperative mood
   "D400",  # First line should end in a period.
   "D404",  # First word of the docstring should not be "This"
   "TID252",  # No relative imports (not pep8 compliant)
 ]
 ignore = [
   "PLR2004",  # magic value used in comparson
   "E501",  # Line too long (want to have fixed
 ]
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["E", "F", "UP", "PLE", "D"]
-unfixable = []
 line-length = 88
 exclude = ["docs", "build"]
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 # Minimum supported Python version
 target-version = "py39"
 
@@ -182,25 +177,18 @@
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.mccabe]
 max-complexity = 10
 
-[tool.ruff.lint.isort]
+[tool.ruff.isort]
+known-first-party = ["dtscalibration"]
 force-single-line = true
 
-[tool.isort]
-py_version=39
-force_single_line = true
-known_first_party = ["dtscalibration"]
-skip = [".gitignore", ".tox", "docs", ".venv"]
-src_paths = ["src", "tests"]
-line_length = 120
-
 [tool.black]
 line-length = 88
 target-version = ['py39', 'py310', 'py311']
 extend-exclude = ".venv"
 
 [tool.mypy]
 ignore_missing_imports = true  # Preferably false, but matplotlib, scipy and statsmodels are missing typing stubs
```

### Comparing `dtscalibration-3.0.2/PKG-INFO` & `dtscalibration-3.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dtscalibration
-Version: 3.0.2
+Version: 3.0.3
 Summary: Load Distributed Temperature Sensing (DTS) files, calibrate the temperature and estimate its uncertainty.
 Author: Bas des Tombe, Bart Schilperoort
 Maintainer: Bas des Tombe, Bart Schilperoort
 License-Expression: BSD-3-Clause
 License-File: AUTHORS.rst
 License-File: LICENSE
 Keywords: DTS,calibration,confidence intervals,distributed temperature sensing
@@ -34,15 +34,14 @@
 Requires-Dist: statsmodels
 Requires-Dist: xarray[parallel]
 Requires-Dist: xmltodict
 Provides-Extra: dev
 Requires-Dist: black[jupyter]; extra == 'dev'
 Requires-Dist: bump2version; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
-Requires-Dist: isort; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: nbformat; extra == 'dev'
 Requires-Dist: pandas-stubs; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-xdist; extra == 'dev'
@@ -93,15 +92,15 @@
     :target: https://github.com/dtscalibration/python-dts-calibration/actions/workflows/build.yml
     :alt: Test Status
 
 .. |version| image:: https://img.shields.io/pypi/v/dtscalibration.svg
     :alt: PyPI Package latest release
     :target: https://pypi.python.org/pypi/dtscalibration
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v3.0.2.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v3.0.3.svg
     :alt: Commits since latest release
     :target: https://github.com/dtscalibration/python-dts-calibration/compare/v1.1.1...main
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/dtscalibration.svg
     :alt: PyPI Wheel
     :target: https://pypi.python.org/pypi/dtscalibration
 
@@ -117,16 +116,15 @@
    :alt: Interactively run the example notebooks online
    :target: https://mybinder.org/v2/gh/dtscalibration/python-dts-calibration/main?labpath=docs%2Fnotebooks
 
 .. end-badges
 
 A Python package to load Distributed Temperature Sensing files, perform a calibration, and plot the result. A detailed description of the calibration procedure can be found at https://doi.org/10.3390/s20082235 .
 
-* Free software: BSD 3-Clause License
-
+Do you have questions, ideas or just want to say hi? Please leave a message on the ` discussions page <https://github.com/dtscalibration/python-dts-calibration/discussions>`_!
 
 Installation
 ============
 
 .. code-block:: zsh
 
     pip install dtscalibration
@@ -142,17 +140,17 @@
 DTS measures temperature by calibrating backscatter measurements to sections with a known temperature. DTS devices provide a simple interface to perform a limited calibration. Re-calibrating your measurements with this Python package gives you better temperature estimates and additional options.
 
 * Advanced calibration routine
    * Supports `single <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/07Calibrate_single_ended.ipynb>`_- and `double-ended <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/08Calibrate_double_ended.ipynb>`_ setups
    * Compute uncertainty of the calibrated temperature
    * All measurements are used to estimate parameter values that are constant over time.
    * Weighted least-squares calibration
-   * `Fixing parameters to a previously determined value <../main/examples/notebooks/13Fixed_parameter_calibration.ipynb>`_
-   * `(Asymmetric) step loss correction <../main/examples/notebooks/14Lossy_splices.ipynb>`_ so that fiber connectors can be used instead of welds/splices.
-   * `Matching temperature sections <../main/examples/notebooks/15Matching_sections.ipynb>`_ to support J-configurations
+   * `Fixing parameters to a previously determined value <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/13Fixed_parameter_calibration.ipynb>`_
+   * `(Asymmetric) step loss correction <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/14Lossy_splices.ipynb>`_ so that fiber connectors can be used instead of welds/splices.
+   * `Matching temperature sections <https://github.com/dtscalibration/python-dts-calibration/blob/main/docs/notebooks/15Matching_sections.ipynb>`_ to support J-configurations
 * Dynamic reference section definition
 * Tools for merging and aligning double-ended setups
 * Data formats of most manufacturers are supported
 
 Devices currently supported
 ===========================
 * Silixa Ltd.: **Ultima** & **XT-DTS** .xml files *(up to version 8.1)*
```

