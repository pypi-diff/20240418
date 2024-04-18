# Comparing `tmp/shepherd_data-2023.9.9.tar.gz` & `tmp/shepherd_data-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_data-2023.9.9.tar", last modified: Sat Sep 30 12:20:33 2023, max compression
+gzip compressed data, was "shepherd_data-2024.4.1.tar", last modified: Thu Apr 18 13:25:13 2024, max compression
```

## Comparing `shepherd_data-2023.9.9.tar` & `shepherd_data-2024.4.1.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:33.534760 shepherd_data-2023.9.9/
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2023-09-30 12:20:33.534760 shepherd_data-2023.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2023-09-30 12:20:33.534760 shepherd_data-2023.9.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:33.530760 shepherd_data-2023.9.9/shepherd_data/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/shepherd_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/shepherd_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/shepherd_data/debug_resampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/shepherd_data/ivonne.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/shepherd_data/mppt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16853 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/shepherd_data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:33.534760 shepherd_data-2023.9.9/shepherd_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2023-09-30 12:20:33.000000 shepherd_data-2023.9.9/shepherd_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2023-09-30 12:20:33.000000 shepherd_data-2023.9.9/shepherd_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-30 12:20:33.000000 shepherd_data-2023.9.9/shepherd_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-09-30 12:20:33.000000 shepherd_data-2023.9.9/shepherd_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-09-30 12:20:33.000000 shepherd_data-2023.9.9/shepherd_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-09-30 12:20:33.000000 shepherd_data-2023.9.9/shepherd_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-30 12:20:33.000000 shepherd_data-2023.9.9/shepherd_data.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:20:33.530760 shepherd_data-2023.9.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/tests/test_cli_downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/tests/test_cli_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/tests/test_cli_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/tests/test_cli_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/tests/test_ivonne.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-09-30 12:19:59.000000 shepherd_data-2023.9.9/tests/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:13.168982 shepherd_data-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-18 13:25:13.168982 shepherd_data-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:25:13.168982 shepherd_data-2024.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:13.164982 shepherd_data-2024.4.1/shepherd_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/debug_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/mppt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/shepherd_data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:13.168982 shepherd_data-2024.4.1/shepherd_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 13:25:13.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:25:12.000000 shepherd_data-2024.4.1/shepherd_data.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:25:13.164982 shepherd_data-2024.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_cli_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_cli_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_cli_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_cli_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 13:24:56.000000 shepherd_data-2024.4.1/tests/test_reader.py
```

### Comparing `shepherd_data-2023.9.9/shepherd_data/cli.py` & `shepherd_data-2024.4.1/shepherd_data/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-"""
-Command definitions for CLI
-"""
+"""Command definitions for CLI"""
+
 import logging
 import os
 import sys
+from contextlib import suppress
 from datetime import datetime
 from pathlib import Path
 from typing import List
 from typing import Optional
 
 import click
 
 from shepherd_core import get_verbose_level
 from shepherd_core import increase_verbose_level
+from shepherd_core import local_tz
 from shepherd_core.commons import samplerate_sps_default
 
 from . import Reader
 from . import Writer
 from . import __version__
 
 logger = logging.getLogger("SHPData.cli")
 
 
 def path_to_flist(data_path: Path) -> List[Path]:
-    """every path gets transformed to a list of paths
+    """Every path gets transformed to a list of paths
     - if directory: list of files inside
     - if existing file: list with 1 element
     - or else: empty list
     """
     data_path = Path(data_path).resolve()
     h5files = []
     if data_path.is_file() and data_path.suffix.lower() == ".h5":
         h5files.append(data_path)
     elif data_path.is_dir():
         flist = os.listdir(data_path)
         for file in flist:
             fpath = data_path / str(file)
-            if not fpath.is_file() or ".h5" != fpath.suffix.lower():
+            if not fpath.is_file() or fpath.suffix.lower() != ".h5":
                 continue
             h5files.append(fpath)
     return h5files
 
 
 @click.group(context_settings={"help_option_names": ["-h", "--help"], "obj": {}})
 @click.option(
@@ -51,15 +52,15 @@
 )
 @click.option(
     "--version",
     is_flag=True,
     help="Prints version-info at start (combinable with -v)",
 )
 @click.pass_context  # TODO: is the ctx-type correct?
-def cli(ctx: click.Context, verbose: bool, version: bool) -> None:
+def cli(ctx: click.Context, verbose: bool, version: bool) -> None:  # noqa: FBT001
     """Shepherd: Synchronized Energy Harvesting Emulator and Recorder"""
     if verbose:
         increase_verbose_level(3)
     if version:
         logger.info("Shepherd-Data v%s", __version__)
         logger.debug("Python v%s", sys.version)
         logger.debug("Click v%s", click.__version__)
@@ -73,20 +74,23 @@
     """Validates a file or directory containing shepherd-recordings"""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()  # TODO: should be stored and passed in ctx
     valid_dir = True
     for file in files:
         logger.info("Validating '%s' ...", file.name)
         valid_file = True
-        with Reader(file, verbose=verbose_level > 2) as shpr:
-            valid_file &= shpr.is_valid()
-            valid_file &= shpr.check_timediffs()
-            valid_dir &= valid_file
-            if not valid_file:
-                logger.error(" -> File '%s' was NOT valid", file.name)
+        try:
+            with Reader(file, verbose=verbose_level > 2) as shpr:
+                valid_file &= shpr.is_valid()
+                valid_file &= shpr.check_timediffs()
+                valid_dir &= valid_file
+                if not valid_file:
+                    logger.error(" -> File '%s' was NOT valid", file.name)
+        except TypeError as _xpc:
+            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
     sys.exit(int(not valid_dir))
 
 
 @cli.command(short_help="Extracts recorded IVSamples and stores it to csv")
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 @click.option(
     "--ds-factor",
@@ -107,42 +111,44 @@
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     if not isinstance(ds_factor, (float, int)) or ds_factor < 1:
         ds_factor = 1000
         logger.info("DS-Factor was invalid was reset to 1'000")
     for file in files:
         logger.info("Extracting IV-Samples from '%s' ...", file.name)
-        with Reader(file, verbose=verbose_level > 2) as shpr:
-            # will create a downsampled h5-file (if not existing) and then saving to csv
-            ds_file = file.with_suffix(f".downsampled_x{round(ds_factor)}.h5")
-            if not ds_file.exists():
-                logger.info("Downsampling '%s' by factor x%f ...", file.name, ds_factor)
-                with Writer(
-                    ds_file,
-                    mode=shpr.get_mode(),
-                    datatype=shpr.get_datatype(),
-                    window_samples=shpr.get_window_samples(),
-                    cal_data=shpr.get_calibration_data(),
-                    verbose=verbose_level > 2,
-                ) as shpw:
-                    shpw["ds_factor"] = ds_factor
-                    shpw.store_hostname(shpr.get_hostname())
-                    shpw.store_config(shpr.get_config())
-                    shpr.downsample(
-                        shpr.ds_time, shpw.ds_time, ds_factor=ds_factor, is_time=True
-                    )
-                    shpr.downsample(
-                        shpr.ds_voltage, shpw.ds_voltage, ds_factor=ds_factor
-                    )
-                    shpr.downsample(
-                        shpr.ds_current, shpw.ds_current, ds_factor=ds_factor
-                    )
-
-            with Reader(ds_file, verbose=verbose_level > 2) as shpd:
-                shpd.save_csv(shpd["data"], separator)
+        try:
+            with Reader(file, verbose=verbose_level > 2) as shpr:
+                # will create a downsampled h5-file (if not existing) and then saving to csv
+                ds_file = file.with_suffix(f".downsampled_x{round(ds_factor)}.h5")
+                if not ds_file.exists():
+                    logger.info("Downsampling '%s' by factor x%f ...", file.name, ds_factor)
+                    with Writer(
+                        ds_file,
+                        mode=shpr.get_mode(),
+                        datatype=shpr.get_datatype(),
+                        window_samples=shpr.get_window_samples(),
+                        cal_data=shpr.get_calibration_data(),
+                        verbose=verbose_level > 2,
+                    ) as shpw:
+                        shpw["ds_factor"] = ds_factor
+                        shpw.store_hostname(shpr.get_hostname())
+                        shpw.store_config(shpr.get_config())
+                        shpr.downsample(
+                            shpr.ds_time,
+                            shpw.ds_time,
+                            ds_factor=ds_factor,
+                            is_time=True,
+                        )
+                        shpr.downsample(shpr.ds_voltage, shpw.ds_voltage, ds_factor=ds_factor)
+                        shpr.downsample(shpr.ds_current, shpw.ds_current, ds_factor=ds_factor)
+
+                with Reader(ds_file, verbose=verbose_level > 2) as shpd:
+                    shpd.save_csv(shpd["data"], separator)
+        except TypeError as _xpc:
+            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
 
 
 @cli.command(
     short_help="Extracts metadata and logs from file or directory containing shepherd-recordings"
 )
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 @click.option(
@@ -154,84 +160,89 @@
 )
 def extract_meta(in_data: Path, separator: str) -> None:
     """Extracts metadata and logs from file or directory containing shepherd-recordings"""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     for file in files:
         logger.info("Extracting metadata & logs from '%s' ...", file.name)
-        with Reader(file, verbose=verbose_level > 2) as shpr:
-            elements = shpr.save_metadata()
-            # TODO: add default exports (user-centric) and allow specifying --all or specific ones
-            # TODO: could also be combined with other extractors (just have one)
-            if "sysutil" in elements:
-                shpr.save_csv(shpr["sysutil"], separator)
-            if "timesync" in elements:
-                shpr.save_csv(shpr["timesync"], separator)
-
-            if "shepherd-log" in elements:
-                shpr.save_log(shpr["shepherd-log"])
-            if "dmesg" in elements:
-                shpr.save_log(shpr["dmesg"])
-            if "exceptions" in elements:
-                shpr.save_log(shpr["exceptions"])
-            if "uart" in elements:
-                shpr.save_log(shpr["uart"])
+        # TODO: add default exports (user-centric) and allow specifying --all or specific ones
+        # TODO: could also be combined with other extractors (just have one)
+        # TODO remove deprecated: timesync; "shepherd-log", "dmesg", "exceptions"
+        try:
+            with Reader(file, verbose=verbose_level > 2) as shpr:
+                shpr.save_metadata()
+                for element in ["ptp", "sysutil", "timesync"]:
+                    if element in shpr.h5file:
+                        shpr.save_csv(shpr[element], separator)
+                logs_depr = ["shepherd-log", "dmesg", "exceptions"]
+                logs = ["sheep", "kernel", "phc2sys", "uart"]
+                for element in logs + logs_depr:
+                    if element in shpr.h5file:
+                        shpr.save_log(shpr[element])
+                        # TODO: allow omitting timestamp,
+                        #       also test if segmented uart is correctly written
+                        shpr.warn_logs(element, show=True)
+        except TypeError as _xpc:
+            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
 
 
 @cli.command(
     short_help="Extracts uart from gpio-trace in file or directory containing shepherd-recordings"
 )
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 def extract_uart(in_data: Path) -> None:
     """Extracts uart from gpio-trace in file or directory containing shepherd-recordings"""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     for file in files:
         logger.info("Extracting uart from gpio-trace from from '%s' ...", file.name)
-        with Reader(file, verbose=verbose_level > 2) as shpr:
-            # TODO: move into separate fn OR add to h5-file and use .save_log(), ALSO TEST
-            lines = shpr.gpio_to_uart()
-            # TODO: could also add parameter to get symbols instead of lines
-            log_path = Path(file).with_suffix(".uart_from_wf.log")
-            if log_path.exists():
-                logger.warning("%s already exists, will skip", log_path)
-                continue
+        try:
+            with Reader(file, verbose=verbose_level > 2) as shpr:
+                # TODO: move into separate fn OR add to h5-file and use .save_log(), ALSO TEST
+                lines = shpr.gpio_to_uart()
+                # TODO: could also add parameter to get symbols instead of lines
+                log_path = Path(file).with_suffix(".uart_from_wf.log")
+                if log_path.exists():
+                    logger.info("File already exists, will skip '%s'", log_path.name)
+                    continue
 
-            with open(log_path, "w") as log_file:
-                for line in lines:
-                    try:
-                        timestamp = datetime.utcfromtimestamp(float(line[0]))
-                        log_file.write(timestamp.strftime("%Y-%m-%d %H:%M:%S.%f") + ":")
-                        log_file.write(f"\t{str.encode(line[1])}")
-                        log_file.write("\n")
-                    except TypeError:
-                        continue
+                with log_path.open("w") as log_file:
+                    for line in lines:
+                        with suppress(TypeError):
+                            timestamp = datetime.fromtimestamp(float(line[0]), tz=local_tz())
+                            log_file.write(timestamp.strftime("%Y-%m-%d %H:%M:%S.%f") + ":")
+                            # TODO: allow to skip Timestamp and export raw text
+                            log_file.write(f"\t{str.encode(line[1])}")
+                            log_file.write("\n")
+        except TypeError as _xpc:
+            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
 
 
-@cli.command(
-    short_help="Extracts gpio-trace from file or directory containing shepherd-recordings"
-)
+@cli.command(short_help="Extracts gpio-trace from file or directory containing shepherd-recordings")
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 @click.option(
     "--separator",
     "-s",
     default=";",
     type=click.STRING,
     help="Set an individual csv-separator",
 )
 def extract_gpio(in_data: Path, separator: str) -> None:
     """Extracts uart from gpio-trace in file or directory containing shepherd-recordings"""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     for file in files:
         logger.info("Extracting gpio-trace from from '%s' ...", file.name)
-        with Reader(file, verbose=verbose_level > 2) as shpr:
-            wfs = shpr.gpio_to_waveforms()
-            for name, wf in wfs.items():
-                shpr.waveform_to_csv(name, wf, separator)
+        try:
+            with Reader(file, verbose=verbose_level > 2) as shpr:
+                wfs = shpr.gpio_to_waveforms()
+                for name, wf in wfs.items():
+                    shpr.waveform_to_csv(name, wf, separator)
+        except TypeError as _xpc:
+            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
 
 
 @cli.command(
     short_help="Creates an array of downsampling-files from "
     "file or directory containing shepherd-recordings"
 )
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
@@ -245,63 +256,62 @@
 )
 @click.option(
     "--sample-rate",
     "-r",
     type=click.INT,
     help="Alternative Input to determine a downsample-factor (Choose One)",
 )
-def downsample(
-    in_data: Path, ds_factor: Optional[float], sample_rate: Optional[int]
-) -> None:
+def downsample(in_data: Path, ds_factor: Optional[float], sample_rate: Optional[int]) -> None:
     """Creates an array of downsampling-files from file
-    or directory containing shepherd-recordings"""
+    or directory containing shepherd-recordings
+    """
     if ds_factor is None and sample_rate is not None and sample_rate >= 1:
         ds_factor = int(samplerate_sps_default / sample_rate)
         # TODO: shouldn't current sps be based on file rather than default?
     if isinstance(ds_factor, (float, int)) and ds_factor >= 1:
         ds_list = [ds_factor]
     else:
         ds_list = [5, 25, 100, 500, 2_500, 10_000, 50_000, 250_000, 1_000_000]
 
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     for file in files:
-        with Reader(file, verbose=verbose_level > 2) as shpr:
-            for _factor in ds_list:
-                if shpr.ds_time.shape[0] / _factor < 1000:
-                    logger.warning(
-                        "will skip downsampling for %s because resulting sample-size is too small",
-                        file.name,
-                    )
-                    break
-                ds_file = file.with_suffix(f".downsampled_x{round(_factor)}.h5")
-                if ds_file.exists():
-                    continue
-                logger.info("Downsampling '%s' by factor x%f ...", file.name, _factor)
-                with Writer(
-                    ds_file,
-                    mode=shpr.get_mode(),
-                    datatype=shpr.get_datatype(),
-                    window_samples=shpr.get_window_samples(),
-                    cal_data=shpr.get_calibration_data(),
-                    verbose=verbose_level > 2,
-                ) as shpw:
-                    shpw["ds_factor"] = _factor
-                    shpw.store_hostname(shpr.get_hostname())
-                    shpw.store_config(shpr.get_config())
-                    shpr.downsample(
-                        shpr.ds_time, shpw.ds_time, ds_factor=_factor, is_time=True
-                    )
-                    shpr.downsample(shpr.ds_voltage, shpw.ds_voltage, ds_factor=_factor)
-                    shpr.downsample(shpr.ds_current, shpw.ds_current, ds_factor=_factor)
+        try:
+            with Reader(file, verbose=verbose_level > 2) as shpr:
+                for _factor in ds_list:
+                    if shpr.ds_voltage.shape[0] / _factor < 1000:
+                        logger.warning(
+                            "will skip downsampling for %s because "
+                            "resulting sample-size is too small",
+                            file.name,
+                        )
+                        break
+                    ds_file = file.with_suffix(f".downsampled_x{round(_factor)}.h5")
+                    if ds_file.exists():
+                        continue
+                    logger.info("Downsampling '%s' by factor x%f ...", file.name, _factor)
+                    with Writer(
+                        ds_file,
+                        mode=shpr.get_mode(),
+                        datatype=shpr.get_datatype(),
+                        window_samples=shpr.get_window_samples(),
+                        cal_data=shpr.get_calibration_data(),
+                        verbose=verbose_level > 2,
+                    ) as shpw:
+                        shpw["ds_factor"] = _factor
+                        shpw.store_hostname(shpr.get_hostname())
+                        shpw.store_config(shpr.get_config())
+                        shpr.downsample(shpr.ds_time, shpw.ds_time, ds_factor=_factor, is_time=True)
+                        shpr.downsample(shpr.ds_voltage, shpw.ds_voltage, ds_factor=_factor)
+                        shpr.downsample(shpr.ds_current, shpw.ds_current, ds_factor=_factor)
+        except TypeError as _xpc:
+            logger.error("ERROR: will skip file, caught exception: %s", _xpc)
 
 
-@cli.command(
-    short_help="Plots IV-trace from file or directory containing shepherd-recordings"
-)
+@cli.command(short_help="Plots IV-trace from file or directory containing shepherd-recordings")
 @click.argument("in_data", type=click.Path(exists=True, resolve_path=True))
 @click.option(
     "--start",
     "-s",
     default=None,
     type=click.FLOAT,
     help="Start of plot in seconds, will be 0 if omitted",
@@ -335,28 +345,31 @@
 )
 def plot(
     in_data: Path,
     start: Optional[float],
     end: Optional[float],
     width: int,
     height: int,
-    multiplot: bool,
+    multiplot: bool,  # noqa: FBT001
 ) -> None:
     """Plots IV-trace from file or directory containing shepherd-recordings"""
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
     multiplot = multiplot and len(files) > 1
     data = []
     for file in files:
         logger.info("Generating plot for '%s' ...", file.name)
-        with Reader(file, verbose=verbose_level > 2) as shpr:
-            if multiplot:
-                data.append(shpr.generate_plot_data(start, end, relative_ts=True))
-            else:
-                shpr.plot_to_file(start, end, width, height)
+        try:
+            with Reader(file, verbose=verbose_level > 2) as shpr:
+                if multiplot:
+                    data.append(shpr.generate_plot_data(start, end, relative_timestamp=True))
+                else:
+                    shpr.plot_to_file(start, end, width, height)
+        except TypeError as _xpc:
+            logger.exception("ERROR: will skip file, caught exception: %s", _xpc)
     if multiplot:
         logger.info("Got %d datasets to plot", len(data))
         mpl_path = Reader.multiplot_to_file(data, in_data, width, height)
         if mpl_path:
             logger.info("Plot generated and saved to '%s'", mpl_path.name)
         else:
             logger.info("Plot not generated, path was already in use.")
```

### Comparing `shepherd_data-2023.9.9/shepherd_data/debug_resampler.py` & `shepherd_data-2024.4.1/shepherd_data/debug_resampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,13 +20,11 @@
     with shpd.Writer(
         out_file,
         mode=shpr.get_mode(),
         datatype=shpr.get_datatype(),
         window_samples=shpr.get_window_samples(),
         cal_data=shpr.get_calibration_data(),
     ) as shpw:
-        shpr.resample(
-            shpr.ds_time, shpw.ds_time, samplerate_dst=samplerate_sps, is_time=True
-        )
+        shpr.resample(shpr.ds_time, shpw.ds_time, samplerate_dst=samplerate_sps, is_time=True)
         shpr.resample(shpr.ds_voltage, shpw.ds_voltage, samplerate_dst=samplerate_sps)
         shpr.resample(shpr.ds_current, shpw.ds_current, samplerate_dst=samplerate_sps)
         shpw.save_metadata()
```

### Comparing `shepherd_data-2023.9.9/shepherd_data/ivonne.py` & `shepherd_data-2024.4.1/shepherd_data/ivonne.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,55 @@
-"""
-prototype of a file-reader with various converters
+"""prototype of a file-reader with various converters
 to generate valid shepherd-data for emulation
 
 """
+
 import errno
 import logging
 import math
 import os
-import pickle  # noqa: S403
+import pickle
 from pathlib import Path
+from types import TracebackType
 from typing import Optional
+from typing import Type
 
 import numpy as np
 import pandas as pd
 from tqdm import trange
+from typing_extensions import Self
 
 from . import Writer
 from .mppt import MPPTracker
 from .mppt import OptimalTracker
 from .mppt import iv_model
 
 
-def get_voc(coeffs: pd.DataFrame):
+def get_voc(coeffs: pd.DataFrame):  # noqa: ANN201
     """Open-circuit voltage of IV curve with given coefficients."""
     return np.log(coeffs["a"] / coeffs["b"] + 1) / coeffs["c"]
 
 
-def get_isc(coeffs: pd.DataFrame):
+def get_isc(coeffs: pd.DataFrame):  # noqa: ANN201
     """Short-circuit current of IV curve with given coefficients."""
     return coeffs["a"]
 
 
 class Reader:
-    """container for converters to shepherd-data"""
+    """Container for converters that bridge the gap to shepherds data-files."""
 
     _logger: logging.Logger = logging.getLogger("SHPData.IVonne.Reader")
 
     def __init__(
         self,
         file_path: Path,
         samplerate_sps: Optional[int] = None,
+        *,
         verbose: bool = True,
-    ):
+    ) -> None:
         self._logger.setLevel(logging.INFO if verbose else logging.WARNING)
 
         self.file_path = Path(file_path).resolve()
         self.samplerate_sps: int = 50
         if samplerate_sps is not None:
             self.samplerate_sps = samplerate_sps
 
@@ -54,35 +58,39 @@
 
         self.runtime_s: float = 0
         self.file_size: int = 0
         self.data_rate: float = 0
 
         self._df: Optional[pd.DataFrame] = None
 
-    def __enter__(self):
+    def __enter__(self) -> Self:
         if not self.file_path.exists():
-            raise FileNotFoundError(
-                errno.ENOENT, os.strerror(errno.ENOENT), self.file_path.name
-            )
-        with open(self.file_path, "rb") as ifr:
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), self.file_path.name)
+        with self.file_path.open("rb") as ifr:
             self._df = pickle.load(ifr)  # noqa: S301
         self._refresh_file_stats()
-        self._logger.info(
+        self._logger.debug(
             "Reading data from '%s'\n"
             "\t- runtime = %d s\n"
             "\t- size = %.3f KiB\n"
             "\t- rate = %.3f KiB/s",
-            self.file_path,
+            self.file_path.name,
             self.runtime_s,
             self.file_size / 2**10,
             self.data_rate / 2**10,
         )
         return self
 
-    def __exit__(self, *exc):  # type: ignore
+    def __exit__(
+        self,
+        typ: Optional[Type[BaseException]] = None,
+        exc: Optional[BaseException] = None,
+        tb: Optional[TracebackType] = None,
+        extra_arg: int = 0,
+    ) -> None:
         pass
 
     def _refresh_file_stats(self) -> None:
         if self._df is None:
             raise RuntimeError("IVonne Context was not entered - file not open!")
         self.runtime_s = round(self._df.shape[0] / self.samplerate_sps, 3)
         self.file_size = self.file_path.stat().st_size
@@ -91,53 +99,48 @@
     def convert_2_ivcurves(
         self,
         shp_output: Path,
         v_max: float = 5.0,
         pts_per_curve: int = 1000,
         duration_s: Optional[float] = None,
     ) -> None:
-        """Transforms previously recorded parameters to shepherd hdf database with IV curves.
-        Shepherd should work with IV 'surfaces', where we have a stream of IV curves
+        """Transform recorded parameters to shepherd hdf database with IV curves.
+
+        Shepherd works with IV 'surfaces', which is a stream of IV curves.
 
         :param shp_output: Path where the resulting hdf file shall be stored
         :param v_max: Maximum voltage supported by shepherd
         :param pts_per_curve: Number of sampling points of the prototype curve
         :param duration_s: time to stop in seconds, counted from beginning
         """
         if self._df is None:
             raise RuntimeError("IVonne Context was not entered - file not open!")
         if isinstance(duration_s, (float, int)) and self.runtime_s > duration_s:
             self._logger.info("  -> gets trimmed to %f s", duration_s)
-            df_elements_n = min(
-                self._df.shape[0], int(duration_s * self.samplerate_sps)
-            )
+            df_elements_n = min(self._df.shape[0], int(duration_s * self.samplerate_sps))
         else:
             df_elements_n = self._df.shape[0]
 
         if shp_output.exists():
-            self._logger.warning("%s already exists, will skip", shp_output.name)
+            self._logger.info("File already exists, will skip '%s'", shp_output.name)
             return
 
         v_proto = np.linspace(0, v_max, pts_per_curve)
 
-        with Writer(
-            shp_output, datatype="ivcurve", window_samples=pts_per_curve
-        ) as sfw:
+        with Writer(shp_output, datatype="ivcurve", window_samples=pts_per_curve) as sfw:
             sfw.store_hostname("IVonne")
             curve_interval_us = round(sfw.sample_interval_ns * pts_per_curve / 1000)
             up_factor = self.sample_interval_ns // sfw.sample_interval_ns
             max_elements = math.ceil(sfw.max_elements // up_factor)
             job_iter = trange(0, df_elements_n, max_elements, desc="generate ivcurves")
 
             for idx in job_iter:
                 idx_top = min(idx + max_elements, df_elements_n)
                 df_slice = self._df.iloc[idx : idx_top + 1].copy()
-                df_slice["timestamp"] = pd.TimedeltaIndex(
-                    data=df_slice["time"], unit="s"
-                )
+                df_slice["timestamp"] = pd.to_timedelta(df_slice["time"], unit="s")
                 df_slice = df_slice.set_index("timestamp")
                 # warning: .interpolate does crash in debug-mode with typeError
                 df_slice = (
                     df_slice.resample(f"{curve_interval_us}us")
                     .interpolate(method="cubic")
                     .iloc[:-1]
                 )
@@ -158,43 +161,43 @@
     def convert_2_ivsamples(
         self,
         shp_output: Path,
         v_max: float = 5.0,
         duration_s: Optional[float] = None,
         tracker: Optional[MPPTracker] = None,
     ) -> None:
-        """Transforms shepherd IV curves to shepherd IV traces.
+        """Transform shepherd IV curves to shepherd IV samples / traces.
 
         For the 'buck' and 'buck-boost' modes, shepherd takes voltage and current traces.
         These can be recorded with shepherd or generated from existing IV curves by, for
         example, maximum power point tracking. This function takes a shepherd IV curve
         file and applies the specified MPPT algorithm to extract the corresponding
         voltage and current traces.
 
-        TODO:
+        Todo:
+        ----
             - allow to use harvester-model in shepherd-code
             - generalize and put it into main code
 
         :param shp_output: Path where the resulting hdf file shall be stored
         :param v_max: Maximum voltage supported by shepherd
         :param duration_s: time to stop in seconds, counted from beginning
         :param tracker: VOC or OPT
+
         """
         if self._df is None:
             raise RuntimeError("IVonne Context was not entered - file not open!")
         if isinstance(duration_s, (float, int)) and self.runtime_s > duration_s:
             self._logger.info("  -> gets trimmed to %f s", duration_s)
-            df_elements_n = min(
-                self._df.shape[0], int(duration_s * self.samplerate_sps)
-            )
+            df_elements_n = min(self._df.shape[0], int(duration_s * self.samplerate_sps))
         else:
             df_elements_n = self._df.shape[0]
 
         if shp_output.exists():
-            self._logger.warning("%s already exists, will skip", shp_output.name)
+            self._logger.info("File already exists, will skip '%s'", shp_output.name)
             return
 
         if tracker is None:
             tracker = OptimalTracker(
                 v_max,
             )
 
@@ -209,56 +212,48 @@
                 # select (max_elements + 1) elements, so upsampling is without gaps
                 # -> drop a sample at the end
                 idx_top = min(idx + max_elements, df_elements_n)
                 df_slice = self._df.iloc[idx : idx_top + 1].copy()
                 df_slice.loc[:, "voc"] = get_voc(df_slice)
                 df_slice.loc[df_slice["voc"] >= v_max, "voc"] = v_max
                 df_slice = tracker.process(df_slice)
-                df_slice["timestamp"] = pd.TimedeltaIndex(
-                    data=df_slice["time"], unit="s"
-                )
-                df_slice = df_slice[["time", "v", "i", "timestamp"]].set_index(
-                    "timestamp"
-                )
+                df_slice["timestamp"] = pd.to_timedelta(df_slice["time"], unit="s")
+                df_slice = df_slice[["time", "v", "i", "timestamp"]].set_index("timestamp")
                 # warning: .interpolate does crash in debug-mode with typeError
                 df_slice = (
-                    df_slice.resample(f"{interval_us}us")
-                    .interpolate(method="cubic")
-                    .iloc[:-1]
+                    df_slice.resample(f"{interval_us}us").interpolate(method="cubic").iloc[:-1]
                 )
                 sfw.append_iv_data_si(
                     df_slice["time"].to_numpy(),
                     df_slice["v"].to_numpy(),
                     df_slice["i"].to_numpy(),
                 )
 
     def upsample_2_isc_voc(
         self,
         shp_output: Path,
         v_max: float = 5.0,
         duration_s: Optional[float] = None,
     ) -> None:
-        """Transforms ivonne-parameters to upsampled version for shepherd
+        """Transform ivonne-parameters to up-sampled versions for shepherd.
 
         :param shp_output: Path where the resulting hdf file shall be stored
         :param v_max: Maximum voltage supported by shepherd
         :param duration_s: time to stop in seconds, counted from beginning
         """
         if self._df is None:
             raise RuntimeError("IVonne Context was not entered - file not open!")
         if isinstance(duration_s, (float, int)) and self.runtime_s > duration_s:
             self._logger.info("  -> gets trimmed to %f s", duration_s)
-            df_elements_n = min(
-                self._df.shape[0], int(duration_s * self.samplerate_sps)
-            )
+            df_elements_n = min(self._df.shape[0], int(duration_s * self.samplerate_sps))
         else:
             df_elements_n = self._df.shape[0]
 
         if shp_output.exists():
-            self._logger.warning("%s already exists, will skip", shp_output.name)
+            self._logger.info("File already exists, will skip '%s'", shp_output.name)
             return
 
         with Writer(shp_output, datatype="isc_voc") as sfw:
             sfw.store_hostname("IVonne")
             interval_us = round(sfw.sample_interval_ns / 1000)
             up_factor = self.sample_interval_ns // sfw.sample_interval_ns
             max_elements = math.ceil(sfw.max_elements // up_factor)
@@ -268,24 +263,18 @@
                 # select (max_elements + 1) elements, so upsampling is without gaps
                 # -> drop a sample at the end
                 idx_top = min(idx + max_elements, df_elements_n)
                 df_slice = self._df.iloc[idx : idx_top + 1].copy()
                 df_slice.loc[:, "voc"] = get_voc(df_slice)
                 df_slice.loc[df_slice["voc"] >= v_max, "voc"] = v_max
                 df_slice.loc[:, "isc"] = get_isc(df_slice)
-                df_slice["timestamp"] = pd.TimedeltaIndex(
-                    data=df_slice["time"], unit="s"
-                )
-                df_slice = df_slice[["time", "voc", "isc", "timestamp"]].set_index(
-                    "timestamp"
-                )
+                df_slice["timestamp"] = pd.to_timedelta(df_slice["time"], unit="s")
+                df_slice = df_slice[["time", "voc", "isc", "timestamp"]].set_index("timestamp")
                 # warning: .interpolate does crash in debug-mode with typeError
                 df_slice = (
-                    df_slice.resample(f"{interval_us}us")
-                    .interpolate(method="cubic")
-                    .iloc[:-1]
+                    df_slice.resample(f"{interval_us}us").interpolate(method="cubic").iloc[:-1]
                 )
                 sfw.append_iv_data_si(
                     df_slice["time"].to_numpy(),
                     df_slice["voc"].to_numpy(),
                     df_slice["isc"].to_numpy(),
                 )
```

### Comparing `shepherd_data-2023.9.9/shepherd_data/mppt.py` & `shepherd_data-2024.4.1/shepherd_data/mppt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,109 +1,112 @@
+"""Harvesters, simple and fast approach.
+
+Might be exchanged by shepherds py-model of pru-harvesters.
 """
-Harvesters, simple and fast approach.
-Might be exchanged by shepherds py-model of pru-harvesters
-"""
+
 import numpy as np
 import pandas as pd
 
 from shepherd_core import Calc_t
 
 
 def iv_model(voltages: Calc_t, coeffs: pd.Series) -> Calc_t:
-    """Simple diode based model of a solar panel IV curve.
+    """Calculate simple diode based model (equivalent circuit diagram) of a solar panel IV curve.
 
-    Args:
-        :param voltages: Load voltage of the solar panel
-        :param coeffs: three generic coefficients
-
-    Returns:
-        Solar current at given load voltage
+    :param voltages: Load voltage of the solar panel
+    :param coeffs: three generic coefficients
+    :return: Solar current at given load voltage
     """
     currents = float(coeffs["a"]) - float(coeffs["b"]) * (
         np.exp(float(coeffs["c"]) * voltages) - 1.0
     )
     if isinstance(currents, np.ndarray):
         currents[currents < 0.0] = 0.0
     else:
         currents = max(0.0, currents)
 
     return currents
 
 
-def find_oc(v_arr: np.ndarray, i_arr: np.ndarray, ratio: float = 0.05):
+def find_oc(v_arr: np.ndarray, i_arr: np.ndarray, ratio: float = 0.05) -> np.ndarray:
     """Approximates opencircuit voltage.
 
     Searches last current value that is above a certain ratio of the short-circuit
     current.
     """
     return v_arr[np.argmax(i_arr < i_arr[0] * ratio)]
 
 
 class MPPTracker:
-    """Prototype
+    """Prototype for a MPPT-class.
 
     :param v_max: Maximum voltage supported by shepherd
     :param pts_per_curve: resolution of internal ivcurve
     """
 
-    def __init__(self, v_max: float = 5.0, pts_per_curve: int = 1000):
+    def __init__(self, v_max: float = 5.0, pts_per_curve: int = 1000) -> None:
         self.pts_per_curve: int = pts_per_curve
         self.v_max: float = v_max
         self.v_proto: np.ndarray = np.linspace(0, v_max, pts_per_curve)
 
     def process(self, coeffs: pd.DataFrame) -> pd.DataFrame:
-        """apply harvesting model to input data
+        """Apply harvesting model to input data.
 
         :param coeffs: ivonne coefficients
-        :return:
+        :return: ivsample-data
         """
-        return pd.DataFrame()
 
 
 class OpenCircuitTracker(MPPTracker):
-    """Open-circuit based MPPT
+    """Open-circuit (-voltage) based MPPT.
 
     :param v_max: Maximum voltage supported by shepherd
     :param pts_per_curve: resolution of internal ivcurve
     :param ratio:  (float) Ratio of open-circuit voltage to track
     """
 
-    def __init__(
-        self, v_max: float = 5.0, pts_per_curve: int = 1000, ratio: float = 0.8
-    ):
+    def __init__(self, v_max: float = 5.0, pts_per_curve: int = 1000, ratio: float = 0.8) -> None:
         super().__init__(v_max, pts_per_curve)
         self.ratio = ratio
 
     def process(self, coeffs: pd.DataFrame) -> pd.DataFrame:
+        """Apply harvesting model to input data.
+
+        :param coeffs: ivonne coefficients
+        :return: ivsample-data
+        """
         coeffs["icurve"] = coeffs.apply(lambda x: iv_model(self.v_proto, x), axis=1)
         if "voc" not in coeffs.columns:
-            coeffs["voc"] = coeffs.apply(
-                lambda x: find_oc(self.v_proto, x["ivcurve"]), axis=1
-            )
+            coeffs["voc"] = coeffs.apply(lambda x: find_oc(self.v_proto, x["ivcurve"]), axis=1)
         coeffs["rvoc_pos"] = coeffs.apply(
             lambda x: np.argmax(self.v_proto[self.v_proto < self.ratio * x["voc"]]),
             axis=1,
         )
         coeffs["i"] = coeffs.apply(lambda x: x["icurve"][x["rvoc_pos"]], axis=1)
         coeffs["v"] = coeffs.apply(lambda x: self.v_proto[x["rvoc_pos"]], axis=1)
         return coeffs
 
 
 class OptimalTracker(MPPTracker):
-    """Optimal MPPT
+    """Optimal MPPT by looking at the whole curve.
 
     Calculates optimal harvesting voltage for every time and corresponding IV curve.
 
     :param v_max: Maximum voltage supported by shepherd
     :param pts_per_curve: resolution of internal ivcurve
     """
 
-    def __init__(self, v_max: float = 5.0, pts_per_curve: int = 1000):
+    def __init__(self, v_max: float = 5.0, pts_per_curve: int = 1000) -> None:
         super().__init__(v_max, pts_per_curve)
 
     def process(self, coeffs: pd.DataFrame) -> pd.DataFrame:
+        """Apply harvesting model to input data.
+
+        :param coeffs: ivonne coefficients
+        :return: ivsample-data
+        """
         coeffs["icurve"] = coeffs.apply(lambda x: iv_model(self.v_proto, x), axis=1)
         coeffs["pcurve"] = coeffs.apply(lambda x: self.v_proto * x["icurve"], axis=1)
         coeffs["max_pos"] = coeffs.apply(lambda x: np.argmax(x["pcurve"]), axis=1)
         coeffs["i"] = coeffs.apply(lambda x: x["icurve"][x["max_pos"]], axis=1)
         coeffs["v"] = coeffs.apply(lambda x: self.v_proto[x["max_pos"]], axis=1)
         return coeffs
```

### Comparing `shepherd_data-2023.9.9/shepherd_data/reader.py` & `shepherd_data-2024.4.1/shepherd_data/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,137 +1,175 @@
-"""
-Reader-Baseclass
-"""
+"""Reader-Baseclass for opening shepherds hdf5-files."""
+
 import math
 from datetime import datetime
 from pathlib import Path
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import h5py
 import numpy as np
 from matplotlib import pyplot as plt
 from tqdm import trange
 
 from shepherd_core import Reader as CoreReader
+from shepherd_core import local_tz
 from shepherd_core.logger import logger
 
-# import samplerate  # TODO: just a test-fn for now
+# import samplerate  # noqa: ERA001, TODO: just a test-fn for now
 
 
 class Reader(CoreReader):
     """Sequentially Reads shepherd-data from HDF5 file.
 
     Args:
+    ----
         file_path: Path of hdf5 file containing shepherd data with iv-samples, iv-curves or isc&voc
         verbose: more info during usage, 'None' skips the setter
+
     """
 
-    def __init__(self, file_path: Optional[Path], verbose: Optional[bool] = True):
-        super().__init__(file_path, verbose)
+    def __init__(
+        self,
+        file_path: Optional[Path],
+        *,
+        verbose: Optional[bool] = True,
+    ) -> None:
+        super().__init__(file_path, verbose=verbose)
 
     def save_csv(self, h5_group: h5py.Group, separator: str = ";") -> int:
-        """extract numerical data via csv
+        """Extract numerical data from group and store it into csv.
 
         :param h5_group: can be external and should probably be downsampled
         :param separator: used between columns
         :return: number of processed entries
         """
         if h5_group["time"].shape[0] < 1:
             self._logger.warning("%s is empty, no csv generated", h5_group.name)
             return 0
         if not isinstance(self.file_path, Path):
             return 0
         csv_path = self.file_path.with_suffix(f".{h5_group.name.strip('/')}.csv")
         if csv_path.exists():
-            self._logger.warning("%s already exists, will skip", csv_path)
+            self._logger.info("File already exists, will skip '%s'", csv_path.name)
             return 0
-        datasets = [
-            key if isinstance(h5_group[key], h5py.Dataset) else []
-            for key in h5_group.keys()
-        ]
+        datasets = [key if isinstance(h5_group[key], h5py.Dataset) else [] for key in h5_group]
         datasets.remove("time")
-        datasets = ["time"] + datasets
+        datasets = ["time", *datasets]
         separator = separator.strip().ljust(2)
-        header = [
-            h5_group[key].attrs["description"].replace(", ", separator)
-            for key in datasets
-        ]
+        header = [h5_group[key].attrs["description"].replace(", ", separator) for key in datasets]
         header = separator.join(header)
-        with open(csv_path, "w", encoding="utf-8-sig") as csv_file:
-            self._logger.info(
-                "CSV-Generator will save '%s' to '%s'", h5_group.name, csv_path.name
-            )
+        with csv_path.open("w", encoding="utf-8-sig") as csv_file:
+            self._logger.info("CSV-Generator will save '%s' to '%s'", h5_group.name, csv_path.name)
             csv_file.write(header + "\n")
             for idx, time_ns in enumerate(h5_group["time"][:]):
-                timestamp = datetime.utcfromtimestamp(time_ns / 1e9)
+                timestamp = datetime.fromtimestamp(time_ns / 1e9, tz=local_tz())
                 csv_file.write(timestamp.strftime("%Y-%m-%d %H:%M:%S.%f"))
                 for key in datasets[1:]:
                     values = h5_group[key][idx]
                     if isinstance(values, np.ndarray):
                         values = separator.join([str(value) for value in values])
                     csv_file.write(f"{separator}{values}")
                 csv_file.write("\n")
         return h5_group["time"][:].shape[0]
 
-    def save_log(self, h5_group: h5py.Group) -> int:
-        """save dataset in group as log, optimal for logged dmesg and exceptions
+    def save_log(self, h5_group: h5py.Group, *, add_timestamp: bool = True) -> int:
+        """Save dataset from group as log, optimal for logged 'dmesg' and console-output.
 
         :param h5_group: can be external
+        :param add_timestamp: can be external
         :return: number of processed entries
         """
         if h5_group["time"].shape[0] < 1:
             self._logger.warning("%s is empty, no log generated", h5_group.name)
             return 0
         if not isinstance(self.file_path, Path):
             return 0
         log_path = self.file_path.with_suffix(f".{h5_group.name.strip('/')}.log")
         if log_path.exists():
-            self._logger.warning("%s already exists, will skip", log_path)
+            self._logger.info("File already exists, will skip '%s'", log_path.name)
             return 0
-        datasets = [
-            key if isinstance(h5_group[key], h5py.Dataset) else []
-            for key in h5_group.keys()
-        ]
+        datasets = [key if isinstance(h5_group[key], h5py.Dataset) else [] for key in h5_group]
         datasets.remove("time")
-        with open(log_path, "w", encoding="utf-8-sig") as log_file:
-            self._logger.info(
-                "Log-Generator will save '%s' to '%s'", h5_group.name, log_path.name
-            )
+        with log_path.open("w", encoding="utf-8-sig") as log_file:
+            self._logger.info("Log-Generator will save '%s' to '%s'", h5_group.name, log_path.name)
             for idx, time_ns in enumerate(h5_group["time"][:]):
-                timestamp = datetime.utcfromtimestamp(time_ns / 1e9)
-                log_file.write(timestamp.strftime("%Y-%m-%d %H:%M:%S.%f") + ":")
+                if add_timestamp:
+                    timestamp = datetime.fromtimestamp(time_ns / 1e9, local_tz())
+                    # ⤷ TODO: these .fromtimestamp would benefit from included TZ
+                    log_file.write(timestamp.strftime("%Y-%m-%d %H:%M:%S.%f") + ":")
                 for key in datasets:
                     try:
                         message = str(h5_group[key][idx])
                     except OSError:
                         message = "[[[ extractor - faulty element ]]]"
                     log_file.write(f"\t{message}")
                 log_file.write("\n")
         return h5_group["time"].shape[0]
 
+    def warn_logs(
+        self,
+        group_name: str = "sheep",
+        min_level: int = 30,
+        limit: int = 10,
+        *,
+        show: bool = True,
+    ) -> int:
+        """Print warning messages from log in data-group."""
+        _count = self.count_errors_in_log(group_name, min_level)
+        if _count < 1:
+            return 0
+        if not show:
+            return _count
+        self._logger.warning(
+            "%s caught %d messages with level>=%d -> first %d are:",
+            self.get_hostname(),
+            _count,
+            min_level,
+            limit,
+        )
+        for idx, time_ns in enumerate(self.h5file[group_name]["time"][:]):
+            _level = self.h5file[group_name]["level"][idx]
+            if _level < min_level:
+                continue
+            _msg = self.h5file[group_name]["message"][idx]
+            _timestamp = datetime.fromtimestamp(time_ns / 1e9, local_tz())
+            if _level < 30:
+                self._logger.info("    %s: %s", _timestamp, _msg)
+            elif _level < 40:
+                self._logger.warning("    %s: %s", _timestamp, _msg)
+            else:
+                self._logger.error("    %s: %s", _timestamp, _msg)
+            limit -= 1
+            if limit < 1:
+                break
+        return _count
+
     def downsample(
         self,
-        data_src: h5py.Dataset,
+        data_src: Union[h5py.Dataset, np.ndarray],
         data_dst: Union[None, h5py.Dataset, np.ndarray],
         start_n: int = 0,
         end_n: Optional[int] = None,
         ds_factor: float = 5,
+        *,
         is_time: bool = False,
     ) -> Union[h5py.Dataset, np.ndarray]:
-        """Warning: only valid for IV-Stream, not IV-Curves
+        """Sample down iv-data.
+
+        Warning: only valid for IV-Stream, not IV-Curves
 
         :param data_src: a h5-dataset to digest, can be external
         :param data_dst: can be a dataset, numpy-array or None (will be created internally then)
         :param start_n: start-sample
         :param end_n: ending-sample (not included)
-        :param ds_factor: downsampling-factor
-        :param is_time: time is not really downsamples, but just decimated
-        :return: downsampled h5-dataset or numpy-array
+        :param ds_factor: sampling-factor
+        :param is_time: time is not really down-sampled, but decimated
+        :return: resampled h5-dataset or numpy-array
         """
         from scipy import signal  # here due to massive delay
 
         if self.get_datatype() == "ivcurve":
             self._logger.warning("Downsampling-Function was not written for IVCurves")
         ds_factor = max(1, math.floor(ds_factor))
 
@@ -170,53 +208,47 @@
         for _iter in trange(
             0,
             iterations,
             desc=f"downsampling {data_src.name}",
             leave=False,
             disable=iterations < 8,
         ):
-            slice_ds = data_src[
-                start_n + _iter * iblock_len : start_n + (_iter + 1) * iblock_len
-            ]
+            slice_ds = data_src[start_n + _iter * iblock_len : start_n + (_iter + 1) * iblock_len]
             if not is_time and ds_factor > 1:
                 slice_ds, f_state = signal.sosfilt(filter_, slice_ds, zi=f_state)
             slice_ds = slice_ds[::ds_factor]
             slice_len = min(dest_len - _iter * oblock_len, oblock_len)
-            data_dst[_iter * oblock_len : (_iter + 1) * oblock_len] = slice_ds[
-                :slice_len
-            ]
+            data_dst[_iter * oblock_len : (_iter + 1) * oblock_len] = slice_ds[:slice_len]
         if isinstance(data_dst, np.ndarray):
-            data_dst.resize(
-                (oblock_len * (iterations - 1) + slice_len,), refcheck=False
-            )
+            data_dst.resize((oblock_len * (iterations - 1) + slice_len,), refcheck=False)
         else:
             data_dst.resize((oblock_len * (iterations - 1) + slice_len,))
         return data_dst
 
     def resample(
         self,
-        data_src: h5py.Dataset,
+        data_src: Union[h5py.Dataset, np.ndarray],
         data_dst: Union[None, h5py.Dataset, np.ndarray],
         start_n: int = 0,
         end_n: Optional[int] = None,
         samplerate_dst: float = 1000,
+        *,
         is_time: bool = False,
     ) -> Union[h5py.Dataset, np.ndarray]:
+        """Up- or down-sample the original trace-data.
+
+        :param data_src: original iv-data
+        :param data_dst: resampled iv-traces
+        :param start_n: start index of the source
+        :param end_n: end index of the source
+        :param samplerate_dst: desired sampling rate
+        :param is_time: time-array is handled differently than IV-Samples
+        :return: resampled iv-data
         """
-        :param data_src:
-        :param data_dst:
-        :param start_n:
-        :param end_n:
-        :param samplerate_dst:
-        :param is_time:
-        :return:
-        """
-        self._logger.error(
-            "Resampling is still under construction - do not use for now!"
-        )
+        self._logger.error("Resampling is still under construction - do not use for now!")
         if self.get_datatype() == "ivcurve":
             self._logger.warning("Resampling-Function was not written for IVCurves")
 
         if isinstance(end_n, (int, float)):
             _end_n = min(data_src.shape[0], round(end_n))
         else:
             _end_n = data_src.shape[0]
@@ -282,34 +314,34 @@
                 #                                 samplerate_dst, filter="kaiser_fast")
                 slice_out_nxt = slice_out_now + slice_out_ds.shape[0]
                 # print(f"@{i}: got {slice_out_ds.shape[0]}")  # noqa: E800
                 data_dst[slice_out_now:slice_out_nxt] = slice_out_ds
                 slice_out_now = slice_out_nxt
             resampler.reset()
             """
-            pass
 
         if isinstance(data_dst, np.ndarray):
             data_dst.resize((slice_out_now,), refcheck=False)
         else:
             data_dst.resize((slice_out_now,))
 
         return data_dst
 
     def generate_plot_data(
         self,
         start_s: Optional[float] = None,
         end_s: Optional[float] = None,
-        relative_ts: bool = True,
+        *,
+        relative_timestamp: bool = True,
     ) -> Dict:
-        """provides down-sampled iv-data that can be feed into plot_to_file()
+        """Provide down-sampled iv-data that can be fed into plot_to_file().
 
         :param start_s: time in seconds, relative to start of recording
         :param end_s: time in seconds, relative to start of recording
-        :param relative_ts: treat
+        :param relative_timestamp: treat
         :return: down-sampled size of ~ self.max_elements
         """
         if self.get_datatype() == "ivcurve":
             self._logger.warning("Plot-Function was not written for IVCurves")
         if not isinstance(start_s, (float, int)):
             start_s = 0
         if not isinstance(end_s, (float, int)):
@@ -327,43 +359,37 @@
                     start_sample,
                     end_sample,
                     ds_factor,
                     is_time=True,
                 )
             ).astype(float),
             "voltage": self._cal.voltage.raw_to_si(
-                self.downsample(
-                    self.ds_voltage, None, start_sample, end_sample, ds_factor
-                )
+                self.downsample(self.ds_voltage, None, start_sample, end_sample, ds_factor)
             ),
             "current": self._cal.current.raw_to_si(
-                self.downsample(
-                    self.ds_current, None, start_sample, end_sample, ds_factor
-                )
+                self.downsample(self.ds_current, None, start_sample, end_sample, ds_factor)
             ),
             "start_s": start_s,
             "end_s": end_s,
         }
-        if relative_ts:
+        if relative_timestamp:
             data["time"] = data["time"] - self._cal.time.raw_to_si(self.ds_time[0])
         return data
 
     @staticmethod
-    def assemble_plot(
-        data: Union[dict, list], width: int = 20, height: int = 10
-    ) -> plt.Figure:
-        """
-        TODO: add power (if wanted)
+    def assemble_plot(data: Union[dict, list], width: int = 20, height: int = 10) -> plt.Figure:
+        """Create the actual figure.
 
         :param data: plottable / down-sampled iv-data with some meta-data
                 -> created with generate_plot_data()
         :param width: plot-width
         :param height: plot-height
-        :return:
+        :return: figure
         """
+        # TODO: add power (if wanted)
         if isinstance(data, dict):
             data = [data]
         fig, axes = plt.subplots(2, 1, sharex="all")
         fig.suptitle("Voltage and current")
         for date in data:
             axes[0].plot(date["time"], date["voltage"], label=date["name"])
             axes[1].plot(date["time"], date["current"] * 10**6, label=date["name"])
@@ -380,59 +406,56 @@
     def plot_to_file(
         self,
         start_s: Optional[float] = None,
         end_s: Optional[float] = None,
         width: int = 20,
         height: int = 10,
     ) -> None:
-        """creates (down-sampled) IV-Plot
-            -> omitting start- and end-time will use the whole duration
+        """Create (down-sampled) IV-Plots.
+
+        Omitting start- and end-time will use the whole trace (full duration).
 
         :param start_s: time in seconds, relative to start of recording, optional
         :param end_s: time in seconds, relative to start of recording, optional
         :param width: plot-width
         :param height: plot-height
         """
         if not isinstance(self.file_path, Path):
             return
 
         data = [self.generate_plot_data(start_s, end_s)]
 
         start_str = f"{data[0]['start_s']:.3f}".replace(".", "s")
         end_str = f"{data[0]['end_s']:.3f}".replace(".", "s")
-        plot_path = self.file_path.resolve().with_suffix(
-            f".plot_{start_str}_to_{end_str}.png"
-        )
+        plot_path = self.file_path.resolve().with_suffix(f".plot_{start_str}_to_{end_str}.png")
         if plot_path.exists():
             self._logger.warning("Plot exists, will skip & not overwrite!")
             return
         self._logger.info("Plot generated, will be saved to '%s'", plot_path.name)
         fig = self.assemble_plot(data, width, height)
         plt.savefig(plot_path)
         plt.close(fig)
         plt.clf()
 
     @staticmethod
     def multiplot_to_file(
         data: list, plot_path: Path, width: int = 20, height: int = 10
     ) -> Optional[Path]:
-        """creates (down-sampled) IV-Multi-Plot
+        """Create (down-sampled) IV-Multi-Plots (of more than one trace).
 
         :param data: plottable / down-sampled iv-data with some meta-data
             -> created with generate_plot_data()
         :param plot_path: optional
         :param width: plot-width
         :param height: plot-height
         """
         start_str = f"{data[0]['start_s']:.3f}".replace(".", "s")
         end_str = f"{data[0]['end_s']:.3f}".replace(".", "s")
         plot_path = (
-            Path(plot_path)
-            .resolve()
-            .with_suffix(f".multiplot_{start_str}_to_{end_str}.png")
+            Path(plot_path).resolve().with_suffix(f".multiplot_{start_str}_to_{end_str}.png")
         )
         if plot_path.exists():
             logger.warning("Plot exists, will skip & not overwrite!")
             return None
         fig = Reader.assemble_plot(data, width, height)
         plt.savefig(plot_path)
         plt.close(fig)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shepherd_data-2023.9.9/tests/test_cli_downsample.py` & `shepherd_data-2024.4.1/tests/test_cli_downsample.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 from click.testing import CliRunner
 
 from shepherd_data.cli import cli
 
 
 def test_cli_downsample_file_full(data_h5: Path) -> None:
-    res = CliRunner().invoke(
-        cli, ["--verbose", "downsample", "--ds-factor", "10", str(data_h5)]
-    )
+    res = CliRunner().invoke(cli, ["--verbose", "downsample", "--ds-factor", "10", str(data_h5)])
     assert res.exit_code == 0
     assert data_h5.with_suffix(".downsampled_x10.h5").exists()
 
 
 def test_cli_downsample_file_short(data_h5: Path) -> None:
     res = CliRunner().invoke(cli, ["-v", "downsample", "-f", "20", str(data_h5)])
     assert res.exit_code == 0
@@ -34,17 +32,15 @@
         cli, ["--verbose", "downsample", "--ds-factor", "40", str(data_h5.parent)]
     )
     assert res.exit_code == 0
     assert data_h5.with_suffix(".downsampled_x40.h5").exists()
 
 
 def test_cli_downsample_rate_file_full(data_h5: Path) -> None:
-    res = CliRunner().invoke(
-        cli, ["--verbose", "downsample", "--sample-rate", "100", str(data_h5)]
-    )
+    res = CliRunner().invoke(cli, ["--verbose", "downsample", "--sample-rate", "100", str(data_h5)])
     assert res.exit_code == 0
     assert data_h5.with_suffix(".downsampled_x1000.h5").exists()
 
 
 def test_cli_downsample_rate_file_short(data_h5: Path) -> None:
     res = CliRunner().invoke(cli, ["-v", "downsample", "-r", "200", str(data_h5)])
     assert res.exit_code == 0
```

### Comparing `shepherd_data-2023.9.9/tests/test_cli_extract.py` & `shepherd_data-2024.4.1/tests/test_cli_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     )
     assert res.exit_code == 0
     assert data_h5.with_suffix(".downsampled_x100.h5").exists()
     assert data_h5.with_suffix(".downsampled_x100.data.csv").exists()
 
 
 def test_cli_extract_file_short(data_h5: Path) -> None:
-    res = CliRunner().invoke(
-        cli, ["-v", "extract", "-f", "200", "-s", ";", str(data_h5)]
-    )
+    res = CliRunner().invoke(cli, ["-v", "extract", "-f", "200", "-s", ";", str(data_h5)])
     assert res.exit_code == 0
     assert data_h5.with_suffix(".downsampled_x200.h5").exists()
     assert data_h5.with_suffix(".downsampled_x200.data.csv").exists()
 
 
 def test_cli_extract_file_min(data_h5: Path) -> None:
     res = CliRunner().invoke(cli, ["-v", "extract", str(data_h5)])
@@ -56,17 +54,15 @@
     )
     assert res.exit_code == 0
     assert data_h5.with_suffix(".downsampled_x2000.h5").exists()
     assert data_h5.with_suffix(".downsampled_x2000.data.csv").exists()
 
 
 def test_cli_extract_meta_file_full(data_h5: Path) -> None:
-    res = CliRunner().invoke(
-        cli, ["--verbose", "extract-meta", "--separator", ";", str(data_h5)]
-    )
+    res = CliRunner().invoke(cli, ["--verbose", "extract-meta", "--separator", ";", str(data_h5)])
     assert res.exit_code == 0
     # TODO: nothing to grab here, add in base-file, same for tests below
 
 
 def test_cli_extract_meta_file_short(data_h5: Path) -> None:
     res = CliRunner().invoke(cli, ["-v", "extract-meta", "-s", "-", str(data_h5)])
     assert res.exit_code == 0
```

### Comparing `shepherd_data-2023.9.9/tests/test_cli_plot.py` & `shepherd_data-2024.4.1/tests/test_cli_plot.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,30 +48,24 @@
     assert res.exit_code == 0
     assert data_h5.with_suffix(".plot_2s345_to_8s765.png").exists()
 
 
 def test_cli_plot_file_min(data_h5: Path) -> None:
     res = CliRunner().invoke(cli, ["-v", "plot", str(data_h5)])
     assert res.exit_code == 0
-    assert data_h5.with_suffix(
-        ".plot_0s000_to_10s000.png"
-    ).exists()  # full duration of file
+    assert data_h5.with_suffix(".plot_0s000_to_10s000.png").exists()  # full duration of file
 
 
 def test_cli_plot_dir_min(tmp_path: Path) -> None:
     file1_path = generate_h5_file(tmp_path, "hrv_file1.h5")
     file2_path = generate_h5_file(tmp_path, "hrv_file2.h5")
     res = CliRunner().invoke(cli, ["-v", "plot", str(tmp_path.resolve())])
     assert res.exit_code == 0
-    assert file1_path.with_suffix(
-        ".plot_0s000_to_10s000.png"
-    ).exists()  # full duration of file
-    assert file2_path.with_suffix(
-        ".plot_0s000_to_10s000.png"
-    ).exists()  # full duration of file
+    assert file1_path.with_suffix(".plot_0s000_to_10s000.png").exists()  # full duration of file
+    assert file2_path.with_suffix(".plot_0s000_to_10s000.png").exists()  # full duration of file
 
 
 def test_cli_multiplot_dir_full(tmp_path: Path) -> None:
     generate_h5_file(tmp_path, "hrv_file1.h5")
     generate_h5_file(tmp_path, "hrv_file2.h5")
     res = CliRunner().invoke(
         cli,
@@ -119,10 +113,8 @@
 
 
 def test_cli_multiplot_dir_min(tmp_path: Path) -> None:
     generate_h5_file(tmp_path, "hrv_file1.h5")
     generate_h5_file(tmp_path, "hrv_file2.h5")
     res = CliRunner().invoke(cli, ["-v", "plot", "-m", str(tmp_path)])
     assert res.exit_code == 0
-    assert tmp_path.with_suffix(
-        ".multiplot_0s000_to_10s000.png"
-    ).exists()  # full duration of file
+    assert tmp_path.with_suffix(".multiplot_0s000_to_10s000.png").exists()  # full duration of file
```

### Comparing `shepherd_data-2023.9.9/tests/test_ivonne.py` & `shepherd_data-2024.4.1/tests/test_ivonne.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 
 from shepherd_data import Reader
 from shepherd_data import ivonne
 from shepherd_data import mppt
 
 
-@pytest.fixture
+@pytest.fixture()
 def example_path() -> Path:
     here = Path(__file__).resolve().parent
     return here.parent / "examples"
 
 
 def test_convert_ivonne(tmp_path: Path, example_path: Path) -> None:
     input_file = "jogging_10m"
```

