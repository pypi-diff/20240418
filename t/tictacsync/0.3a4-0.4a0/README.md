# Comparing `tmp/tictacsync-0.3a4.tar.gz` & `tmp/tictacsync-0.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictacsync-0.3a4.tar", last modified: Thu Apr 11 00:00:48 2024, max compression
+gzip compressed data, was "tictacsync-0.4a0.tar", last modified: Thu Apr 18 16:08:29 2024, max compression
```

## Comparing `tictacsync-0.3a4.tar` & `tictacsync-0.4a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-11 00:00:48.361852 tictacsync-0.3a4/
--rwxr-xr-x   0 lutzray    (501) staff       (20)     1068 2021-11-05 23:38:28.000000 tictacsync-0.3a4/LICENSE
--rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-11 00:00:48.361395 tictacsync-0.3a4/PKG-INFO
--rw-rw-r--   0 lutzray    (501) staff       (20)     4170 2024-03-26 23:09:32.000000 tictacsync-0.3a4/README.md
--rw-r--r--   0 lutzray    (501) staff       (20)       38 2024-04-11 00:00:48.362011 tictacsync-0.3a4/setup.cfg
--rw-r--r--   0 lutzray    (501) staff       (20)     1790 2024-04-11 00:00:22.000000 tictacsync-0.3a4/setup.py
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-11 00:00:48.354502 tictacsync-0.3a4/tictacsync/
--rw-rw-r--   0 lutzray    (501) staff       (20)        0 2022-01-08 15:24:31.000000 tictacsync-0.3a4/tictacsync/__init__.py
--rw-r--r--   0 lutzray    (501) staff       (20)    27616 2024-04-10 23:52:37.000000 tictacsync-0.3a4/tictacsync/device_scanner.py
--rw-r--r--   0 lutzray    (501) staff       (20)    11393 2024-04-10 23:36:02.000000 tictacsync-0.3a4/tictacsync/entry.py
--rw-r--r--   0 lutzray    (501) staff       (20)     7279 2024-03-24 12:15:34.000000 tictacsync-0.3a4/tictacsync/multi2polywav.py
--rw-r--r--   0 lutzray    (501) staff       (20)     4885 2024-03-27 22:40:38.000000 tictacsync-0.3a4/tictacsync/remergemix.py
--rw-r--r--   0 lutzray    (501) staff       (20)    47608 2024-04-06 15:04:38.000000 tictacsync-0.3a4/tictacsync/timeline.py
--rw-r--r--   0 lutzray    (501) staff       (20)    76810 2024-04-02 15:13:47.000000 tictacsync-0.3a4/tictacsync/yaltc.py
-drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-11 00:00:48.360900 tictacsync-0.3a4/tictacsync.egg-info/
--rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/PKG-INFO
--rw-r--r--   0 lutzray    (501) staff       (20)      433 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/SOURCES.txt
--rw-r--r--   0 lutzray    (501) staff       (20)        1 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/dependency_links.txt
--rw-r--r--   0 lutzray    (501) staff       (20)      139 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/entry_points.txt
--rw-r--r--   0 lutzray    (501) staff       (20)        1 2022-01-31 00:58:06.000000 tictacsync-0.3a4/tictacsync.egg-info/not-zip-safe
--rw-r--r--   0 lutzray    (501) staff       (20)      132 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/requires.txt
--rw-r--r--   0 lutzray    (501) staff       (20)       11 2024-04-11 00:00:48.000000 tictacsync-0.3a4/tictacsync.egg-info/top_level.txt
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-18 16:08:29.820608 tictacsync-0.4a0/
+-rwxr-xr-x   0 lutzray    (501) staff       (20)     1068 2021-11-05 23:38:28.000000 tictacsync-0.4a0/LICENSE
+-rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-18 16:08:29.820223 tictacsync-0.4a0/PKG-INFO
+-rw-rw-r--   0 lutzray    (501) staff       (20)     4170 2024-03-26 23:09:32.000000 tictacsync-0.4a0/README.md
+-rw-r--r--   0 lutzray    (501) staff       (20)       38 2024-04-18 16:08:29.820741 tictacsync-0.4a0/setup.cfg
+-rw-r--r--   0 lutzray    (501) staff       (20)     1789 2024-04-18 16:07:57.000000 tictacsync-0.4a0/setup.py
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-18 16:08:29.815693 tictacsync-0.4a0/tictacsync/
+-rw-rw-r--   0 lutzray    (501) staff       (20)        0 2022-01-08 15:24:31.000000 tictacsync-0.4a0/tictacsync/__init__.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    27339 2024-04-12 00:39:24.000000 tictacsync-0.4a0/tictacsync/device_scanner.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    11386 2024-04-18 15:36:05.000000 tictacsync-0.4a0/tictacsync/entry.py
+-rw-r--r--   0 lutzray    (501) staff       (20)     7279 2024-03-24 12:15:34.000000 tictacsync-0.4a0/tictacsync/multi2polywav.py
+-rw-r--r--   0 lutzray    (501) staff       (20)     4885 2024-03-27 22:40:38.000000 tictacsync-0.4a0/tictacsync/remergemix.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    56225 2024-04-18 15:35:51.000000 tictacsync-0.4a0/tictacsync/timeline.py
+-rw-r--r--   0 lutzray    (501) staff       (20)    78490 2024-04-12 00:34:48.000000 tictacsync-0.4a0/tictacsync/yaltc.py
+drwxr-xr-x   0 lutzray    (501) staff       (20)        0 2024-04-18 16:08:29.819738 tictacsync-0.4a0/tictacsync.egg-info/
+-rw-r--r--   0 lutzray    (501) staff       (20)     5023 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/PKG-INFO
+-rw-r--r--   0 lutzray    (501) staff       (20)      433 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/SOURCES.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)        1 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/dependency_links.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)      139 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/entry_points.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)        1 2022-01-31 00:58:06.000000 tictacsync-0.4a0/tictacsync.egg-info/not-zip-safe
+-rw-r--r--   0 lutzray    (501) staff       (20)      132 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/requires.txt
+-rw-r--r--   0 lutzray    (501) staff       (20)       11 2024-04-18 16:08:29.000000 tictacsync-0.4a0/tictacsync.egg-info/top_level.txt
```

### Comparing `tictacsync-0.3a4/LICENSE` & `tictacsync-0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a4/PKG-INFO` & `tictacsync-0.4a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictacsync
-Version: 0.3a4
+Version: 0.4a0
 Summary: command for syncing audio video recordings
 Home-page: https://tictacsync.org/
 Author: Raymond Lutz
 Author-email: lutzrayblog@mac.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tictacsync-0.3a4/README.md` & `tictacsync-0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a4/setup.py` & `tictacsync-0.4a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     entry_points = {
         "console_scripts": [
         'tictacsync = tictacsync.entry:main',
         'remergemix = tictacsync.remergemix:main',
         'multi2polywav = tictacsync.multi2polywav:main',
         ]
         },
-    version = '0.3a4',
+    version = '0.4a',
     description = "command for syncing audio video recordings",
     long_description_content_type='text/markdown',
     long_description = long_descr,
     include_package_data=True,
     zip_safe=False,
     author = "Raymond Lutz",
     author_email = "lutzrayblog@mac.com",
```

### Comparing `tictacsync-0.3a4/tictacsync/device_scanner.py` & `tictacsync-0.4a0/tictacsync/device_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 @dataclass
 class Device:
     UID: int
     folder: Path
     name: str
     dev_type: str # CAM or REC
     n_chan: int
+    ttc: int
     tracks: Tracks
     def __hash__(self):
         return self.UID
     def __eq__(self, other):
         return self.UID == other
 
 @dataclass
@@ -111,15 +112,15 @@
         n = audio_str['channels']
         # pprint(ffmpeg.probe(p))
     else:
         n = sox.file_info.channels(_pathname(p)) # eg 2
     logger.debug('for file %s dev_UID established %s'%(p.name, dev_UID))
     return Media(p,
         Device(UID=dev_UID, folder=p.parent, name=dev_name, dev_type=dt,
-                n_chan=n, tracks=None))
+                n_chan=n, ttc=None, tracks=None))
 
 def get_device_ffprobe_UID(file):
     """
     Tries to find an unique hash integer identifying the device that produced
     the file based on the string inside ffprobe metadata  without any
     reference to date nor length nor time. Find out with ffprobe the type
     of device: CAM or REC for videocamera or audio recorder.
@@ -338,40 +339,30 @@
             logger.debug('parsed tracks %s'%tracks)
             ntracks = 2*len(tracks.stereomics)
             ntracks += len(tracks.mix)
             ntracks += len(tracks.unused)
             ntracks += len(tracks.others)
             ntracks += 1 # for ttc track
             logger.debug(' n chan: %i n tracks file: %i'%(nchan, ntracks))
-            # if ntracks != nchan:
-            #     print('\nError parsing %s content'%tracks_file)
-            #     print('incoherent number of tracks, %i vs %i quitting\n'%
-            #                                         (nchan, ntracks))
-                # sys.exit(1)
+            if ntracks != nchan:
+                print('\nError parsing %s content'%tracks_file)
+                print('incoherent number of tracks, %i vs %i quitting\n'%
+                                                    (nchan, ntracks))
+                sys.exit(1)
             err_msg = tracks.error_msg
             if  err_msg != None:
                 print('Error, quitting: in file %s, %s'%(tracks_file, err_msg))
                 raise Exception
             else:
+                logger.debug('tracks object%s'%tracks)
                 return tracks
         else:
             logger.debug('no tracks.txt file found')
             return None
 
-    # def _use_folder_as_device_name(self):
-    #     """
-    #     For each media in self.found_media_files replace existing Device.name by
-    #     folder name.
-
-    #     Returns nothing
-    #     """
-    #     for m in self.found_media_files:
-    #         m.device.name = m.path.parent.name
-    #     logger.debug(self.found_media_files)
-
     def _check_folders_have_same_device(self):
         """
         Since input_structure == 'folder_is_device,
         checks for files in self.found_media_files for structure as following.
 
         Warns user and quit program for:
           A- folders with mix of video and audio
```

### Comparing `tictacsync-0.3a4/tictacsync/entry.py` & `tictacsync-0.4a0/tictacsync/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,18 +122,18 @@
                     help='terse output')
     args = parser.parse_args()
     if args.verbose_output:
         logger.add(sys.stderr, level="DEBUG")
     # logger.add(sys.stdout, filter="__main__")
     # logger.add(sys.stdout, filter="device_scanner")
     # logger.add(sys.stdout, filter="yaltc") _extract_sound_to_merge
-    # logger.add(sys.stdout, filter=lambda r: r["function"] == "scan_media_and_build_devices_UID")
-    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_sox_multi2mono")
-    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_get_mix")
-    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_sox_mix")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_get_tracks_from_file")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_get_device_mix")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_sox_mono2stereo")
+    # logger.add(sys.stdout, filter=lambda r: r["function"] == "_sox_mix_files")
     top_dir = args.directory[0]
     if os.path.isfile(top_dir):
         file = top_dir
         process_single(file, args)
     if not os.path.isdir(top_dir):
         print('%s is not a directory or doesnt exist.'%top_dir)
         sys.exit(1)
@@ -230,15 +230,15 @@
     #     print('\nMerging for more than 2 devices is not implemented yet, quitting...')
     #     sys.exit(1)
     if len(recordings_with_time) < 2:
         if not args.terse:
             print('\nNothing to sync, exiting.\n')
         sys.exit(1)
     matcher = timeline.Matcher(recordings_with_time)
-    matcher.scan_audio_for_each_ref_rec()
+    matcher.scan_audio_for_each_videoclip()
     if not matcher.video_mergers:
         if not args.terse:
             print('\nNothing to sync, bye.\n')
         sys.exit(1)
     asked_ISOs = args.write_ISOs
     if asked_ISOs and scanner.input_structure != 'folder_is_device':
         print('Warning, can\'t write ISOs without structured folders: [gold1]--isos[/gold1] option ignored.\n')
@@ -259,19 +259,19 @@
     if not args.terse:
         print("\n")
     # find out where files were wrtitten
     a_stitcher = matcher.video_mergers[0]
     print('\nWrote output in folder [gold1]%s[/gold1]'%(
             a_stitcher.synced_clip_dir))
     for stitcher in matcher.video_mergers:
-        print('[gold1]%s[/gold1]'%stitcher.ref_recording.AVpath.name, end='')
+        print('[gold1]%s[/gold1]'%stitcher.videoclip.AVpath.name, end='')
         for audio in stitcher.get_matched_audio_recs():
             print(' + [gold1]%s[/gold1]'%audio.AVpath.name, end='')
-        new_file = stitcher.ref_recording.final_synced_file.parts
-        print(' became [gold1]%s[/gold1]'%stitcher.ref_recording.final_synced_file.name)
+        new_file = stitcher.videoclip.final_synced_file.parts
+        print(' became [gold1]%s[/gold1]'%stitcher.videoclip.final_synced_file.name)
         # matcher._build_otio_tracks_for_cam()
     matcher.shrink_gaps_between_takes()
     sys.exit(0)
     
 if __name__ == '__main__':
     main()
```

### Comparing `tictacsync-0.3a4/tictacsync/multi2polywav.py` & `tictacsync-0.4a0/tictacsync/multi2polywav.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a4/tictacsync/remergemix.py` & `tictacsync-0.4a0/tictacsync/remergemix.py`

 * *Files identical despite different names*

### Comparing `tictacsync-0.3a4/tictacsync/timeline.py` & `tictacsync-0.4a0/tictacsync/timeline.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 DEL_TEMP = False
 DB_OSX_NORM = -6 #dB
 OUT_DIR_DEFAULT = 'SyncedMedia'
 
 # utility for accessing pathnames
 def _pathname(tempfile_or_path) -> str:
     if isinstance(tempfile_or_path, str):
-        return tempfile_or_path
+        return tempfile_or_path ################################################
     if isinstance(tempfile_or_path, yaltc.Recording):
-        return str(tempfile_or_path.AVpath)
+        return str(tempfile_or_path.AVpath) ####################################
     if isinstance(tempfile_or_path, Path):
-        return str(tempfile_or_path)
+        return str(tempfile_or_path) ###########################################
     if isinstance(tempfile_or_path, tempfile._TemporaryFileWrapper):
-        return tempfile_or_path.name
+        return tempfile_or_path.name ###########################################
     else:
         raise Exception('%s should be Path or tempfile...'%tempfile_or_path)
 
 # utility for printing groupby results
 def print_grby(grby):
     for key, keylist in grby:
         print('\ngrouped by %s:'%key)
@@ -58,37 +58,32 @@
     mix_dict = {1:[channel]}
     logger.debug('sox args %s %s %s'%(source, dest, mix_dict))    
     sox_transform.remix(mix_dict)
     logger.debug('sox transform %s'%str(sox_transform))
     status = sox_transform.build(str(source), str(dest))
     logger.debug('sox status %s'%status)
 
-def _sox_keep(audio_file, kept_channels) -> tempfile.NamedTemporaryFile:
+def _sox_keep(audio_file, kept_channels: list) -> tempfile.NamedTemporaryFile:
     """
     Returns a NamedTemporaryFile containing the selected kept_channels
 
-    if len(kept_channels) == 1 then it's a mono mix on the specified track
-    if len(kept_channels) == 2 then it's a stereo mix on the specified tracks
+    Channels numbers in kept_channels are not ZBIDXed as per SOX format
     """
-
-
-
-
     audio_file = _pathname(audio_file)
     nchan = sox.file_info.channels(audio_file)
     logger.debug('in file of %i chan, have to keep %s'%
         (nchan, kept_channels))
     all_channels = range(1, nchan + 1) # from 1 to nchan included
     # Building dict according to pysox.remix format.
     # https://pysox.readthedocs.io/en/latest/api.html#sox.transform.Transformer.remix
     # eg:   {1: [3], 2: [4]} to keep channels 3 & 4    
     kept_channels = [[n] for n in kept_channels]
     sox_remix_dict = dict(zip(all_channels, kept_channels))
-    output_fh = tempfile.NamedTemporaryFile(suffix='.wav', delete=DEL_TEMP)
-    out_file = _pathname(output_fh)
+    output_tempfile = tempfile.NamedTemporaryFile(suffix='.wav', delete=DEL_TEMP)
+    out_file = _pathname(output_tempfile)
     logger.debug('sox in and out files: %s %s'%(audio_file, out_file))
     # sox_transform.set_output_format(channels=1)
     sox_transform = sox.Transformer()
     sox_transform.remix(sox_remix_dict)
     logger.debug('sox remix transform: %s'%sox_transform)
     logger.debug('sox remix dict: %s'%sox_remix_dict)
     status = sox_transform.build(audio_file, out_file, return_output=True )
@@ -99,16 +94,15 @@
     logger.debug('remixed input_file ffprobe:\n%s'%(stdout +
         stderr).decode('utf-8'))
     p = Popen('ffprobe %s -hide_banner'%out_file,
         shell=True, stdout=PIPE, stderr=PIPE)
     stdout, stderr = p.communicate()
     logger.debug('remixed out_file ffprobe:\n%s'%(stdout +
         stderr).decode('utf-8'))
-    return output_fh
-
+    return output_tempfile
 
 def _split_channels(multi_chan_audio:Path) -> list:
     nchan = sox.file_info.channels(_pathname(multi_chan_audio))
     source = _pathname(multi_chan_audio)
     paths = []
     for i in range(nchan):
         out_fh = tempfile.NamedTemporaryFile(suffix='.wav',
@@ -128,15 +122,15 @@
     """
     Combines (stacks) files referred by the list of Path into a new temporary
     files passed on return each files are stacked in a different channel, so
     len(paths) == n_channels
     """
     if len(paths) == 1: # one device only, nothing to stack
         logger.debug('one device only, nothing to stack')
-        return paths[0]
+        return paths[0] ########################################################
     out_file_handle = tempfile.NamedTemporaryFile(suffix='.wav',
         delete=DEL_TEMP)
     filenames = [_pathname(p) for p in paths]
     out_file_name = _pathname(out_file_handle)
     logger.debug('combining files: %s into %s'%(
         filenames,
         out_file_name))
@@ -154,128 +148,208 @@
         _pathname(out_file_handle))
     nchan = sox.file_info.channels(
         _pathname(out_file_handle)) 
     logger.debug('merged file duration %f s with %i channels '%
         (merged_duration, nchan))
     return out_file_handle
 
-def _sox_multi2mono(multichan_tmpfl) -> tempfile.NamedTemporaryFile:
-    # return a mono mix down
+def _sox_multi2stereo(multichan_tmpfl, stereo_trxs) -> tempfile.NamedTemporaryFile:
+
+    """
+    This mixes down all the tracks in multichan_tmpfl to a stereo wav file. Any
+    mono tracks are panned 50-50 (mono tracks are those not present in argument
+    stereo_trxs)
+
+    Args:
+        multichan_tmpfl : tempfile.NamedTemporaryFile
+            contains the edited and synced audio, almost ready to be merged
+            with the concurrent video file
+        stereo_trxs : list of pairs of integers
+            each pairs identifies a left-right tracks, 1st track in
+            multichan_tmpfl is index 1 (sox is not ZBIDX)
+    Returns:
+        the tempfile.NamedTemporaryFile of a stereo wav file
+        containing the audio to be merged with the video
+    """
     n_chan_input = sox.file_info.channels(_pathname(multichan_tmpfl))
     logger.debug('n chan input: %s'%n_chan_input)
     if n_chan_input == 1: # nothing to mix down
-        return multichan_tmpfl
-    mono_tpfl = tempfile.NamedTemporaryFile(suffix='.wav',
+        return multichan_tmpfl #################################################
+    stereo_tempfile = tempfile.NamedTemporaryFile(suffix='.wav',
                     delete=DEL_TEMP)
     tfm = sox.Transformer()
     tfm.channels(1)
-    status = tfm.build(_pathname(multichan_tmpfl),_pathname(mono_tpfl))
+    status = tfm.build(_pathname(multichan_tmpfl),_pathname(stereo_tempfile))
+    logger.debug('n chan ouput: %s'%
+                sox.file_info.channels(_pathname(stereo_tempfile)))
+    logger.debug('sox.build status for _sox_multi2stereo(): %s'%status)
+    if status != True:
+        print('Error, sox did not normalize file in _sox_multi2stereo()')
+        sys.exit(1)
+    return stereo_tempfile
+
+def _sox_mix_channels(multichan_tmpfl, stereo_pairs=[]) -> tempfile.NamedTemporaryFile:
+    """
+    Returns a mix down of the multichannel wav file. If stereo_pairs list is
+    empty, a mono mix is done with all the channel present in multichan_tmpfl.
+    If stereo_pairs contains one or more elements, a stereo mix is returned with
+    the specified Left-Right pairs and all other mono tracks (panned 50-50)
+
+    Note: stereo_pairs numbers are not ZBIDXed
+    """
+    n_chan_input = sox.file_info.channels(_pathname(multichan_tmpfl))
+    logger.debug('n chan input: %s'%n_chan_input)
+    if n_chan_input == 1: # nothing to mix down
+        return multichan_tmpfl #################################################
+    if stereo_pairs == []:
+        # all mono
+        mono_tpfl = tempfile.NamedTemporaryFile(suffix='.wav',
+                        delete=DEL_TEMP)
+        tfm = sox.Transformer()
+        tfm.channels(1)
+        status = tfm.build(_pathname(multichan_tmpfl),_pathname(mono_tpfl))
+        logger.debug('number of chan in ouput: %s'%
+                    sox.file_info.channels(_pathname(mono_tpfl)))
+        logger.debug('sox.build status for _sox_mix_channels(): %s'%status)
+        if status != True:
+            print('Error, sox did not normalize file in _sox_mix_channels()')
+            sys.exit(1)
+        return mono_tpfl
+    else:
+        # stereo tracks present, so stereo output
+        logger.debug('stereo tracks present %s, so stereo output'%stereo_pairs)
+        stereo_files = [_sox_keep(pair) for pair in stereo_pairs]
+    #### ???
+    return 
+
+def _sox_mono2stereo(temp_file) -> tempfile.NamedTemporaryFile:
+    # upgrade a mono file to stereo panning 50-50
+    stereo_tempfile = tempfile.NamedTemporaryFile(suffix='.wav',
+                    delete=DEL_TEMP)
+    tfm = sox.Transformer()
+    tfm.channels(2)
+    status = tfm.build(_pathname(temp_file),_pathname(stereo_tempfile))
     logger.debug('n chan ouput: %s'%
-                sox.file_info.channels(_pathname(mono_tpfl)))
-    logger.debug('sox.build status for _sox_multi2mono(): %s'%status)
+                sox.file_info.channels(_pathname(stereo_tempfile)))
+    logger.debug('sox.build status for _sox_mono2stereo(): %s'%status)
     if status != True:
-        print('Error, sox did not normalize file in _sox_multi2mono()')
+        print('Error, sox did not normalize file in _sox_mono2stereo()')
         sys.exit(1)
-    return mono_tpfl
+    return stereo_tempfile
 
 
-def _sox_mix(paths:list) -> tempfile.NamedTemporaryFile:
+def _sox_mix_files(temp_files_to_mix:list) -> tempfile.NamedTemporaryFile:
     """
-    mix files referred by the list of Path into a new temporary files passed on return
+    Mix files referred by the list of Path into a new temporary files passed on
+    return. If one of the files is stereo, upgrade each mono file to a panned
+    50-50 stereo file before mixing.
     """
     def _sox_norm(tempf):
         normed_tempfile = tempfile.NamedTemporaryFile(suffix='.wav',
                         delete=DEL_TEMP)
         tfm = sox.Transformer()
         tfm.norm(DB_OSX_NORM)
         status = tfm.build(_pathname(tempf),_pathname(normed_tempfile))
         logger.debug('sox.build status for norm(): %s'%status)
         if status != True:
-            print('Error, sox did not normalize file in _sox_mix()')
+            print('Error, sox did not normalize file in _sox_mix_files()')
             sys.exit(1)
         return normed_tempfile
-    paths = [_sox_norm(p) for p in paths]
-    cbn = sox.Combiner()
-    N = len(paths)
+    N = len(temp_files_to_mix)
     if N == 1: # nothing to mix
         logger.debug('one file: nothing to mix')
-        return paths[0]
+        return temp_files_to_mix[0] ########################################################
+    cbn = sox.Combiner()
     cbn.set_input_format(file_type=['wav']*N)
-    filenames = [_pathname(p) for p in paths]
-    logger.debug('%i files to mix %s'%(N, filenames))
-    logger.debug('nchan for each file %s'%[sox.file_info.channels(f) for
-                                    f in filenames])
+    # check if stereo files are present
+    max_n_chan = max([sox.file_info.channels(f) for f
+                                in [_pathname(p) for p in temp_files_to_mix]])
+    logger.debug('max_n_chan %s'%max_n_chan)
+    if max_n_chan == 2:
+        # upgrade all mono to stereo
+        stereo_tempfiles = [p for p in temp_files_to_mix
+            if sox.file_info.channels(_pathname(p)) == 2 ]
+        mono_tempfiles = [p for p in temp_files_to_mix
+            if sox.file_info.channels(_pathname(p)) == 1 ]
+        logger.debug('there are %i mono files and %i stereo files'%
+            (len(stereo_tempfiles), len(mono_tempfiles)))
+        new_stereo = [_sox_mono2stereo(tmpfl) for tmpfl
+                            in mono_tempfiles]
+        stereo_tempfiles += new_stereo
+        files_to_mix = [_pathname(tempfl) for tempfl in stereo_tempfiles]
+    else:
+        # all mono
+        files_to_mix = [_pathname(tempfl) for tempfl in temp_files_to_mix]
     mixed_tempf = tempfile.NamedTemporaryFile(suffix='.wav',delete=DEL_TEMP)
-    status = cbn.build(filenames,
+    status = cbn.build(files_to_mix,
                 _pathname(mixed_tempf),
                 combine_type='mix',
                 input_volumes=[1/N]*N)
     logger.debug('sox.build status for mix: %s'%status)
     if status != True:
-        print('Error, sox did not mix files in _sox_mix()')
+        print('Error, sox did not mix files in _sox_mix_files()')
         sys.exit(1)
     normed_tempfile = tempfile.NamedTemporaryFile(suffix='.wav',delete=DEL_TEMP)
     tfm = sox.Transformer()
     tfm.norm(DB_OSX_NORM)
     status = tfm.build(_pathname(mixed_tempf),_pathname(normed_tempfile))
     logger.debug('sox.build status for norm(): %s'%status)
     if status != True:
-        print('Error, sox did not normalize file in _sox_mix()')
+        print('Error, sox did not normalize file in _sox_mix_files()')
         sys.exit(1)
     return normed_tempfile
 
-
 class AudioStitcherVideoMerger:
     """
     Typically each found video is associated with an AudioStitcherVideoMerger
     instance. AudioStitcherVideoMerger does the actual audio-video file
-    processing of merging self.ref_recording (gen. a video) with all audio
+    processing of merging self.videoclip (gen. a video) with all audio
     files in  self.edited_audio as determined by the Matcher
     object (it instanciates and manages AudioStitcherVideoMerger objects).
 
     All audio file edits are done using pysox and video+audio merging with
     ffmpeg. When necessary, clock drift is corrected for all overlapping audio
     devices to match the precise clock value of the ref recording (to a few
     ppm), using sox tempo transform.
 
-    N.B.: A audio_stitch doesn't extend beyond the corresponding ref_recording
+    N.B.: A audio_stitch doesn't extend beyond the corresponding videoclip
     video start and end times: it is not a audio montage for the whole movie
     project.
 
 
     Attributes:
 
-        ref_recording : a Recording instance
-            The video (or designated main sound) audio files are synced to
+        videoclip : a Recording instance
+            The video to which audio files are synced
 
         edited_audio : dict as {Recording : path}
             keys are elements of matched_audio_recordings of class Recording
             and the value stores the Pathlib path of the eventual edited
             audio (trimmed , padded or time stretched). Before building the
             audio_montage, path points to the initial
             Recording.valid_sound
 
         synced_clip_dir : Path
             where synced clips are written
 
     """
 
-    def __init__(self, reference_recording):
-        self.ref_recording = reference_recording
+    def __init__(self, video_clip):
+        self.videoclip = video_clip
         # self.matched_audio_recordings = []
         self.edited_audio = {}
         logger.debug('instantiating AudioStitcherVideoMerger for %s'%
-                            reference_recording)
+                            video_clip)
 
     def add_matched_audio(self, audio_rec):
         """
         Populates self.edited_audio, a dict as {Recording : path}
 
         AudioStitcherVideoMerger.add_matched_audio() is called
-        within Matcher.scan_audio_for_each_ref_rec()
+        within Matcher.scan_audio_for_each_videoclip()
 
         Returns nothing, fills self.edited_audio dict with
         matched audio.
 
         """
         self.edited_audio[audio_rec] = audio_rec.valid_sound
         """
@@ -286,15 +360,15 @@
         audio_rec.valid_sound doesn't need to be reinitialized since
         it stays unchanged)
         """
         return
 
     def get_matched_audio_recs(self):
         """
-        Returns audio recordings that overlap self.ref_recording.
+        Returns audio recordings that overlap self.videoclip.
         Simply keys of self.edited_audio dict
         """
         return list(self.edited_audio.keys())
 
     def _get_audio_devices(self):
         devices = set([r.device for r in self.get_matched_audio_recs()])
         logger.debug('get_matched_audio_recs: %s'%
@@ -311,22 +385,22 @@
     def _dedrift_rec(self, rec):
         # first_audio_p = rec.AVpath
         initial_duration = sox.file_info.duration(
             _pathname(rec.valid_sound))
         sox_transform = sox.Transformer()
         # tempo_scale_factor = rec.device_relative_speed
         tempo_scale_factor = rec.device_relative_speed
-        reC_dev = rec.device.name
-        reF_dev = self.ref_recording.device.name
+        audio_dev = rec.device.name
+        video_dev = self.videoclip.device.name
         if tempo_scale_factor > 1:
             print('[gold1]%s[/gold1] clock too fast relative to [gold1]%s[/gold1] so file is too long by a %f factor\n'%
-                (reC_dev, reF_dev, tempo_scale_factor))
+                (audio_dev, video_dev, tempo_scale_factor))
         else:
             print('[gold1]%s[/gold1] clock too slow relative to [gold1]%s[/gold1] so file is too short by a %f factor\n'%
-                (reC_dev, reF_dev, tempo_scale_factor))
+                (audio_dev, video_dev, tempo_scale_factor))
         sox_transform.tempo(tempo_scale_factor)
         # scaled_file = self._get_soxed_file(rec, sox_transform)
         logger.debug('sox_transform %s'%sox_transform.effects)
         self._edit_audio_file(rec, sox_transform)
         scaled_file_name = _pathname(self.edited_audio[rec])
         new_duration = sox.file_info.duration(scaled_file_name)
         # goal_duration = rec.get_corrected_duration()
@@ -343,29 +417,29 @@
         recordings = self._get_all_recordings_for(device)
         # [TODO here] Check if all unidentified device files are not
         # overlapping because they are considered produced by the same
         # device. If some overlap then necessarily they're from different
         # ones. List the files and warn the user there is a risk of error if
         # they're not from the same device.
 
-        logger.debug('%i audio files for reference rec %s:'%(len(recordings),
-            self.ref_recording))
+        logger.debug('%i audio files for videoclip %s:'%(len(recordings),
+            self.videoclip))
         for r in recordings:
             logger.debug('  %s'%r)
-        speeds = numpy.array([rec.get_speed_ratio(self.ref_recording)
+        speeds = numpy.array([rec.get_speed_ratio(self.videoclip)
                                     for rec in recordings])
         mean_speed = numpy.mean(speeds)
         for r in recordings:
             r.device_relative_speed = mean_speed
             # r.device_relative_speed = 0.9
             logger.debug('set device_relative_speed for %s'%r)
             logger.debug(' value: %f'%r.device_relative_speed)
-            r.set_time_position_to(self.ref_recording)
+            r.set_time_position_to(self.videoclip)
             logger.debug('time_position for %s: %fs relative to %s'%(r,
-                r.time_position, self.ref_recording))
+                r.time_position, self.videoclip))
         # st_dev_speeds just to check for anomalous situation
         st_dev_speeds = numpy.std(speeds)
         logger.debug('mean speed for %s: %.6f std dev: %.0e'%(device,
                                                     mean_speed,
                                                     st_dev_speeds))
         if st_dev_speeds > 1.0e-5:
             logger.error('too much variation for device speeds')
@@ -423,44 +497,44 @@
             self._pad_file(rec, pad_duration)
             # new_file = rec.edited_version
             new_file = self.edited_audio[rec]
             growing_file = self._concatenate_audio_files(growing_file, new_file)
         end_time = sox.file_info.duration(growing_file.name)
         logger.debug('total edited audio duration  %.2f s'%end_time)
         logger.debug('video duration  %.2f s'%
-            self.ref_recording.get_duration())
+            self.videoclip.get_duration())
         return growing_file
 
     def _pad_or_trim_first_audio(self, first_rec):
         """
         TODO: check if first_rec is a Recording or tempfile (maybe a tempfile if dedrifted)
         NO: will change tempo after trimming/padding
 
         Store (into Recording.edited_audio dict) the handle  of the sox processed
-        first recording, padded or chopped according to AudioStitcherVideoMerger.ref_recording
+        first recording, padded or chopped according to AudioStitcherVideoMerger.videoclip
         starting time. Length of the written file can differ from length of the
         submitted Recording object if drift is corrected with sox tempo
         transform, so check it with sox.file_info.duration()
         """
         logger.debug(' editing %s'%first_rec)
         audio_start  = first_rec.get_start_time()
-        ref_start = self.ref_recording.get_start_time()
-        if ref_start < audio_start: # padding
+        video_start = self.videoclip.get_start_time()
+        if video_start < audio_start: # padding
             logger.debug('padding')
-            pad_duration  = (audio_start-ref_start).total_seconds()
+            pad_duration  = (audio_start-video_start).total_seconds()
             """padding first_file:
                     ┏━━━━━━━━━━━━━━━┓
                     ┗━━━━━━━━━━━━━━━┛ref
                       ┏━━━━━━┓
                     ┣━┻━━━━━━┛
             """
             self._pad_file(first_rec, pad_duration)
         else:
             logger.debug('trimming')
-            length = (ref_start-audio_start).total_seconds()
+            length = (video_start-audio_start).total_seconds()
             """chopping first_file:
                     ┏━━━━━━━━━━━━━━━┓
                     ┗━━━━━━━━━━━━━━━┛ref
                   ┏━╋━━━━┓
                   ┗━┻━━━━┛
             """
             self._chop_file(first_rec, length)
@@ -501,15 +575,15 @@
         Apply the specified sox_transform onto the audio_rec and update
         self.edited_audio dict with the result (with audio_rec as the key)
         """
         output_fh = tempfile.NamedTemporaryFile(suffix='.wav', delete=DEL_TEMP)
         logger.debug('transform: %s'%sox_transform.effects)
         recording_fh = self.edited_audio[audio_rec]
         logger.debug('for recording %s, matching %s'%(audio_rec,
-                                                self.ref_recording))
+                                                self.videoclip))
         input_file = _pathname(recording_fh)
         logger.debug('AudioStitcherVideoMerger.edited_audio[audio_rec]: %s'%
                                                     input_file)
         out_file = _pathname(output_fh)
         logger.debug('sox in and out files: %s %s'%(input_file, out_file))
         status = sox_transform.build(input_file, out_file, return_output=True )
         logger.debug('sox.build exit code %s'%str(status))
@@ -547,15 +621,15 @@
             """            
             Changes the length of audio contained in audio_tempfile so it is the
             same as video length associated with this AudioStitcherVideoMerger.
             Returns a tempfile.NamedTemporaryFile with the new audio
             """         
             sox_transform = sox.Transformer()
             audio_length = sox.file_info.duration(_pathname(audio_tempfile))
-            video_length = self.ref_recording.get_duration()
+            video_length = self.videoclip.get_duration()
             if audio_length > video_length:
                 # trim audio
                 sox_transform.trim(0, video_length)
             else:
                 # pad audio
                 sox_transform.pad(0, video_length - audio_length)
             out_tf = tempfile.NamedTemporaryFile(suffix='.wav',
@@ -566,17 +640,17 @@
             logger.debug('sox in and out files: %s %s'%(input_file, out_file))
             status = sox_transform.build(input_file, out_file,
                                                 return_output=True )
             logger.debug('sox.build exit code %s'%str(status))
             logger.debug('audio duration  %.2f s'%
                 sox.file_info.duration(_pathname(out_tf)))
             logger.debug('video duration  %.2f s'%
-                self.ref_recording.get_duration())
+                self.videoclip.get_duration())
             return out_tf
-        synced_clip_file = self.ref_recording.final_synced_file
+        synced_clip_file = self.videoclip.final_synced_file
         synced_clip_dir = synced_clip_file.parent
         # build ISOs subfolders structure, see comment string below
         video_stem_WO_suffix = synced_clip_file.stem
         # video_stem_WO_suffix = synced_clip_file.stem.split('.')[0]
         # OUT_DIR_DEFAULT, D2 = ISOsDIR.split('/')
         ISOdir = synced_clip_dir/(video_stem_WO_suffix + '.ISO')
         os.makedirs(ISOdir, exist_ok=True)
@@ -587,168 +661,247 @@
         # logger.debug('will split audio to %s'%(ISOdir))
         for name, mono_tmpfl in edited_audio_all_devices:
              # pad(start_duration: float = 0.0, end_duration: float = 0.0)[source]
             destination = ISOdir/('%s.wav'%name)
             mono_tmpfl_trimpad = _fit_length(mono_tmpfl)
             shutil.copy(_pathname(mono_tmpfl_trimpad), destination)
             logger.debug('destination:%s'%destination)
-        # # mixNnormed = _sox_mix(tempfiles)
+        # # mixNnormed = _sox_mix_files(tempfiles)
         # # print('516', _pathname(mixNnormed))
         # os.remove(ISO_multi_chan)
 
-    def _get_mix(self, device, multichan_tmpfl) -> tempfile.NamedTemporaryFile:
-        """        
-        If device has an associated Tracks description that declares a (mono or
-        stereo) mix track, returns a tmpfl containing the corresponding
-        tracks. If not, mix all the tracks with sox.
-
-        If no L-R tracks are declared in tracks.txt, a mono mix is returned;
-        If some
-        micL micR or mixL mixR
+    def _get_device_mix(self, device, multichan_tmpfl) -> tempfile.NamedTemporaryFile:
+        """
+        Build or get a mix from edited and joined audio for a given device
+
+        Returns a mix for merging with video clip. The way the mix is obtained
+        (or created) depends if a tracks.txt for the device  was submitted and
+        depends on its content. There are 4 cases (explained later):
+
+        #1 no mix (or no tracks.txt), all mono
+        #2 no mix, one or more stereo mics
+        #3 mono mix declared
+        #4 stereo mix declared
+
+        In details:
+
+        If no device tracks.txt file declared a mix track (or if tracks.txt is
+        absent), a mix is done programmatically. Two possibilities:
+
+            #1- no stereo pairs were declared: a global mono mix is returned.
+            #2- one or more stereo pair mics were used and declared (micL, micR):
+            a global stereo mix is returned with mono tracks panned 50-50
+
+        If device has an associated Tracks description AND it declares a(mono or
+        stereo) mix track, this fct returns a tempfile containing the
+        corresponding tracks, simpley extarcting them from multichan_tmpfl
+        (thos covers cases #3 and #4)
+
+        Args:
+            device : device_scanner.Device dataclass
+                the device that recorded the audio found in multichan_tmpfl
+            multichan_tmpfl : tempfile.NamedTemporaryFile
+                contains the edited and synced audio, almost ready to be merged
+                with the concurrent video file (after mix down)
+
+        Returns:
+            the tempfile.NamedTemporaryFile of a stereo or mono wav file
+            containing the audio to be merged with the video in
+            self.videoclip
+
 
         """
-        if device.tracks is None:
-            logger.debug('no tracks.txt, mixing all')
-            return _sox_multi2mono(multichan_tmpfl)
-        mix_tracks = device.tracks.mix
-        if mix_tracks == []:
-            logger.debug('tracks.txt present but no mix trx, mixing all')
-            return _sox_multi2mono(multichan_tmpfl)
-        # if here, mix exists
-        logger.debug('%s has mix %s'%(device.name, mix_tracks))
         logger.debug('device %s'%device)
-        if 'ttc' in device.tracks.rawtrx:
-            sox_TTC_chan = device.tracks.rawtrx.index('ttc')
-        elif 'tc' in device.tracks.rawtrx:
-            sox_TTC_chan = device.tracks.rawtrx.index('tc')
-        else:
-            print('Error: no tc or ttc tag in track.txt')
+        if device.n_chan == 2:
+            # tracks.txt or not,
+            # it's stereo, ie audio + TTC, so remove TTC and return
+            kept_channel = (device.ttc + 1)%2 # 1 -> 0 and 0 -> 1
+            logger.debug('no tracks.txt, keeping one chan %i'%kept_channel)
+            return _sox_keep(multichan_tmpfl, [kept_channel + 1]) #-------------
+        # it's multitrack (more than 2 channels)
+        if device.tracks is None:
+            # multitrack but no mix done on location, so do mono mix with all
+            all_channels = list(range(device.n_chan))
+            logger.debug('multitrack but no tracks.txt, mixing %s except TTC at %i'%
+                (all_channels, device.ttc))
+            all_channels.remove(device.ttc)
+            sox_kept_channels = [i + 1 for i in all_channels] # sox indexing
+            logger.debug('mixing channels: %s (sox #)'%sox_kept_channels)
+            kept_audio = _sox_keep(multichan_tmpfl, sox_kept_channels)
+            return _sox_mix_channels(kept_audio) #------------------------------
+        # user wrote a tracks.txt metadata file, check it
+        if device.tracks.mix == [] and device.tracks.stereomics == []:
+            # it's multitrac and no mix done on location, so do a mono mix with
+            # all, but here remove '0' and TTC tracks from mix
+            all_channels = list(range(1, device.n_chan + 1)) # sox not ZBIDX
+            to_remove = device.tracks.unused + [device.ttc+1]# unused is sox idx
+            logger.debug('multitrack but no tracks.txt, mixing %s except # %s (sox #)'%
+                (all_channels, to_remove))
+            sox_kept_channels = [i for i in all_channels
+                                            if i not in to_remove]
+            logger.debug('mixing channels: %s (sox #)'%sox_kept_channels)
+            kept_audio = _sox_keep(multichan_tmpfl, sox_kept_channels)
+            return _sox_mix_channels(kept_audio) #------------------------------
+        if device.tracks.mix != []:
+            # Mix were done on location, no and we only have to extracted it
+            # from the recording. If mono mix, device.tracks.mix has one element;
+            # if stereo mix, device.tracks.mix is a pair of number:
+            logger.debug('%s has mix %s'%(device.name, device.tracks.mix))
+            logger.debug('device %s'%device)
+            # just checking coherency
+            if 'ttc' in device.tracks.rawtrx:
+                trx_TTC_chan = device.tracks.rawtrx.index('ttc')
+            elif 'tc' in device.tracks.rawtrx:
+                trx_TTC_chan = device.tracks.rawtrx.index('tc')
+            else:
+                print('Error: no tc or ttc tag in track.txt')
+                sys.exit(1)
+            logger.debug('TTC chan %i, dev ttc %i'%(trx_TTC_chan, device.ttc))
+            if trx_TTC_chan != device.ttc:
+                print('Error: ttc channel # incoherency in track.txt')
+                sys.exit(1)
+            # coherency check done, extract mix track (or tracks if stereo)
+            mix_kind = 'mono' if len(device.tracks.mix) == 1 else 'stereo'
+            logger.debug('%s mix declared on channel %s (sox #)'%
+                    (mix_kind, device.tracks.mix))
+            return _sox_keep(multichan_tmpfl, device.tracks.mix) #--------------
+        # if here, all cases have been covered except tracks.txt AND no mix AND
+        # stereo mic(s) so first a coherency check, and then proceed
+        if device.tracks.stereomics == []:
+            print('Error, no stereo mic?, check tracks.txt. Quitting')
             sys.exit(1)
-        sox_TTC_chan += 1 # sox Not ZBIDX
-        logger.debug('TTC chan %i'%sox_TTC_chan)
-        # redo indexing since tracks.txt numbers refere to complete
-        # files and here audio file had TTC and muted channels
-        # removed:
-        if len(mix_tracks) == 2: # two tracks to shift
-            mixL_chan, mixR_chan = mix_tracks
-            # shifting left chan if necessary
-            shift = 0
-            if mixL_chan > sox_TTC_chan:
-                shift += 1
-            for unused_tr in device.tracks.unused:
-                if mixL_chan > unused_tr:
-                    shift += 1
-            mixL_chan -= shift
-            # shifting right chan if necessary
-            shift = 0
-            if mixR_chan > sox_TTC_chan:
-                shift += 1
-            for unused_tr in device.tracks.unused:
-                if mixR_chan > unused_tr:
-                    shift += 1
-            mixR_chan -= shift
-            mix_tracks = [mixL_chan, mixR_chan]
-        else: # mono, one track to shift
-            monomix_chan = mix_tracks[0]
-            shift = 0
-            if monomix_chan > sox_TTC_chan:
-                shift += 1
-            for unused_tr in device.tracks.unused:
-                if monomix_chan > unused_tr:
-                    shift += 1
-            monomix_chan -= shift
-            mix_tracks = [monomix_chan]
-        logger.debug('new mix_tracks: %s'%mix_tracks)
-        return _sox_keep(multichan_tmpfl, mix_tracks)
-            
+        logger.debug('processing stereo pair(s) %s'%device.tracks.stereomics)
+        stereo_mic_idx_pairs = [pair for name, pair in device.tracks.stereomics]
+        logger.debug('stereo pairs idxs %s'%stereo_mic_idx_pairs)
+        mic_stereo_files = [_sox_keep(multichan_tmpfl, pair) for pair
+                                                    in stereo_mic_idx_pairs]
+        # flatten list of tuples of channels being stereo mics
+        stereo_mic_idx_flat = [item for sublist in stereo_mic_idx_pairs
+                                                    for item in sublist]
+        logger.debug('stereo_mic_idx_flat %s'%stereo_mic_idx_flat)
+        mono_tracks = [i for i in range(1, device.n_chan + 1)
+                                if i not in stereo_mic_idx_flat]
+        # remove TTC track number
+        mono_tracks.remove(device.ttc + 1)
+        logger.debug('mono_tracks %s'%mono_tracks)
+        mono_files = [_sox_keep(multichan_tmpfl, [chan]) for chan
+                                                    in mono_tracks]
+        new_stereo_files = [_sox_mono2stereo(f) for f in mono_files]
+        stereo_files = mic_stereo_files + new_stereo_files
+        return _sox_mix_files(stereo_files)
 
     def build_audio_and_write_video(self, top_dir, output_dir,
                                     write_multicam_structure,
                                     asked_ISOs):
         """
         top_dir: Path, directory where media were looked for
 
         output_dir: str for optional folder specified as CLI argument, if
         value is None, fall back to OUT_DIR_DEFAULT
 
         write_multicam_structure: True if needs to write multicam folders
 
         asked_ISOs: bool flag specified as CLI argument
 
-        For each audio devices found overlapping self.ref_recording: pad, trim
+        For each audio devices found overlapping self.videoclip: pad, trim
         or stretch audio files by calling _get_concatenated_audiofile_for(), and
         put them in merged_audio_files_by_device. More than one audio recorder
         can be used for a shot: that's why merged_audio_files_by_device is a
         list
 
         Returns nothing
 
         Sets AudioStitcherVideoMerger.final_synced_file on completion
         """
         logger.debug(' fct args: top_dir: %s; output_dir: %s; write_multicam_structure: %s; asked_ISOs: %s;'%
             (top_dir, output_dir, write_multicam_structure, asked_ISOs))
-        logger.debug('device for rec %s: %s'%(self.ref_recording,
-            self.ref_recording.device))
+        logger.debug('device for rec %s: %s'%(self.videoclip,
+            self.videoclip.device))
         # suppose the user called tictacsync with 'mondayPM' as top folder to
         # scan for dailies (and 'somefolder' for output):
         if output_dir == None:
             synced_clip_dir = Path(top_dir)/OUT_DIR_DEFAULT # = mondayPM/SyncedMedia
         else:
             synced_clip_dir = Path(output_dir)/Path(top_dir).name # = somefolder/mondayPM
         if write_multicam_structure:
-            device_name = self.ref_recording.device.name
+            device_name = self.videoclip.device.name
             synced_clip_dir = synced_clip_dir/device_name # = synced_clip_dir/ZOOM
         self.synced_clip_dir = synced_clip_dir
         os.makedirs(synced_clip_dir, exist_ok=True)
         logger.debug('synced_clip_dir is: %s'%synced_clip_dir)
         synced_clip_file = synced_clip_dir/\
-            Path(self.ref_recording.new_rec_name).name
+            Path(self.videoclip.new_rec_name).name
         logger.debug('editing files for %s'%synced_clip_file)
-        self.ref_recording.final_synced_file = synced_clip_file # relative
+        self.videoclip.final_synced_file = synced_clip_file # relative
         # collecting edited audio by device, in (Device, tempfile) pairs:
         merged_audio_files_by_device = [
                             (d, self._get_concatenated_audiofile_for(d)) 
                             for d in self._get_audio_devices()]
         if len(merged_audio_files_by_device) == 0:
             # no audio file overlaps for this clip
-            return
+            return #############################################################
         if len(merged_audio_files_by_device) == 1:
             # only one audio recorder was used, pick singleton in list
             dev, concatenate_audio_file = merged_audio_files_by_device[0]
             logger.debug('one audio device only: %s'%dev)
             # check if this sole recorder is stereo
             if dev.n_chan == 2:
-                # stereo minus TTC chan = mono, check consistency:
+                # consistency check
                 nchan_sox = sox.file_info.channels(
                     _pathname(concatenate_audio_file))
-                logger.debug('nchan_sox: %i mono?'%nchan_sox)
-                if not nchan_sox == 1:
+                logger.debug('Two chan only, nchan_sox: %i dev.n_chan %i'%
+                                (nchan_sox, dev.n_chan))
+                if not nchan_sox == 2:
                     raise Exception('Error in channel processing')
                 # all OK, merge and return
-                logger.debug('simply mono to merge')
-                self.ref_recording.synced_audio = concatenate_audio_file
+                logger.debug('simply mono to merge, TTC on chan %i'%
+                            dev.ttc)
+                # only 2 channels so keep the channel OTHER than TTC
+                if dev.ttc == 1:
+                    # keep channel 0, but + 1 because of sox indexing
+                    sox_kept_channel = 1 
+                else:
+                    # dev.ttc == 0 so keep ch 1, but + 1 (sox indexing)
+                    sox_kept_channel = 2
+                self.videoclip.synced_audio = \
+                        _sox_keep(concatenate_audio_file, [sox_kept_channel])
                 self._merge_audio_and_video()
-                return
-        # if still here, either multitracks and/or multi recorders so check if a
-        # mix has been done on location and identified as is in atracks.txt
-        # file. Split audio channels in mono wav tempfiles at the same time
+                return #########################################################
+        #
+        # if not returned yet from fct, either multitracks and/or multi
+        # recorders so check if a mix has been done on location and identified
+        # as is in atracks.txt file. Split audio channels in mono wav tempfiles
+        # at the same time
         #
         multiple_recorders = len(merged_audio_files_by_device) > 1
         logger.debug('multiple_recorder: %s'%multiple_recorders)
-        # dev_mixes_mix contains all audio recorders if many
-        mixes = [self._get_mix(device, multi_chan_audio)
+        # the device_mixes list contains all audio recorders if many. If only
+        # one audiorecorder was used (most of the cases) len(device_mixes) is 1
+        device_mixes = [self._get_device_mix(device, multi_chan_audio)
                 for device, multi_chan_audio
                 in merged_audio_files_by_device]
-        logger.debug('there are %i dev mixes'%len(mixes))
-        logger.debug('mixes %s'%mixes)
-        dev_mixes_mix = _sox_mix(mixes)
-        logger.debug('will merge with %s'%(_pathname(dev_mixes_mix)))
-        self.ref_recording.synced_audio = dev_mixes_mix
-        logger.debug('dev_mixes_mix n chan: %i'%
-            sox.file_info.channels(_pathname(dev_mixes_mix)))
+
+
+
+        # If multiple audio recorders were used and one of
+        # them has mixL and mixR tracks, two possibilities:
+
+        #     A- others have mixL mixR too: mix of device_mixes are done (and none mix
+        #     tracks are ignored but copied in the ISOs folder if asked)
+        #     B- others don't have mixL-mixR: all tracks from them are panned
+        #     50-50 and stereo-mixed
+
+
+        logger.debug('there are %i dev device_mixes'%len(device_mixes))
+        logger.debug('device_mixes %s'%device_mixes)
+        mix_of_device_mixes = _sox_mix_files(device_mixes)
+        logger.debug('will merge with %s'%(_pathname(mix_of_device_mixes)))
+        self.videoclip.synced_audio = mix_of_device_mixes
+        logger.debug('mix_of_device_mixes n chan: %i'%
+            sox.file_info.channels(_pathname(mix_of_device_mixes)))
         self._merge_audio_and_video()
         # devices_and_monofiles is list of (device, [monofiles])
         # [(dev1, multichan1), (dev2, multichan2)] in
         # merged_audio_files_by_device -> 
         # [(dev1, [mono1_ch1, mono1_ch2]), (dev2, [mono2_ch1, mono2_ch2)]] in 
         # devices_and_monofiles:
         if asked_ISOs:
@@ -759,20 +912,21 @@
                 pprint.pformat(devices_and_monofiles))
             def _trnm(dev, idx): # used in the list comprehension just below
                 # generates track name for later if asked_ISOs
                 # idx is from 0 to nchan-1 for this device
                 if dev.tracks == None:
                     tag = 'chan%s'%str(idx+1).zfill(2)
                 else:
-                    audio_tags = [tag for tag in dev.tracks.rawtrx
-                        if tag not in ['ttc','0','tc']]
-                    tag = audio_tags[idx]
+                    # audio_tags = [tag for tag in dev.tracks.rawtrx
+                    #     if tag not in ['ttc','0','tc']]
+                    tag = dev.tracks.rawtrx[idx]
                 if multiple_recorders:
                     tag += '_' + dev.name
-                return tag
+                logger.debug('tag %s'%tag)
+                return tag #####################################################
             # replace device, idx pair with track name (+ device name if many)
             # loop over devices than loop over tracks
             names_audio_tempfiles = []
             for dev, mono_tmpfiles_list in devices_and_monofiles:
                 for idx, monotf in enumerate(mono_tmpfiles_list):
                     names_audio_tempfiles.append((_trnm(dev, idx), monotf))
             logger.debug('names_audio_tempfiles %s'%names_audio_tempfiles)
@@ -800,33 +954,32 @@
         video_extension = video_path.suffix
         silenced_opts = ["-loglevel", "quiet", "-nostats", "-hide_banner"]
         file_handle = tempfile.NamedTemporaryFile(suffix=video_extension,
             delete=DEL_TEMP)
         out1 = in1.output(file_handle.name, map='0:v', vcodec='copy')
         ffmpeg.run([out1.global_args(*silenced_opts)], overwrite_output=True)
         return file_handle
-        # os.path.split audio channels if more than one
 
     def _merge_audio_and_video(self):
         """      
-        Calls ffmpeg to join video in self.ref_recording.AVpath to
-        audio in self.ref_recording.synced_audio
+        Calls ffmpeg to join video in self.videoclip.AVpath to
+        audio in self.videoclip.synced_audio
 
-        On entry, ref_recording.final_synced_file is a Path to an non existing
-        file (contrarily to ref_recording.synced_audio).
-        On exit, self.ref_recording.final_synced_file points to the final synced
+        On entry, videoclip.final_synced_file is a Path to an non existing
+        file (contrarily to videoclip.synced_audio).
+        On exit, self.videoclip.final_synced_file points to the final synced
         video file.
 
         Returns nothing.
         """
-        synced_clip_file = self.ref_recording.final_synced_file
-        video_path = self.ref_recording.AVpath
-        timecode = self.ref_recording.get_timecode()
-        # self.ref_recording.synced_audio = audio_path
-        audio_path = self.ref_recording.synced_audio
+        synced_clip_file = self.videoclip.final_synced_file
+        video_path = self.videoclip.AVpath
+        timecode = self.videoclip.get_timecode()
+        # self.videoclip.synced_audio = audio_path
+        audio_path = self.videoclip.synced_audio
         vid_only_handle = self._keep_VIDEO_only(video_path)
         a_n = _pathname(audio_path)
         v_n = str(vid_only_handle.name)
         out_n = str(synced_clip_file)
         logger.debug('Merging: \n\t %s + %s = %s\n'%(
                         audio_path,
                         video_path,
@@ -872,36 +1025,26 @@
     """
     Matcher looks for any video in self.recordings and for each one finds out
     all audio recordings (again in self.recordings) that time overlap
     (or against any designated 'main sound', see below). It then spawns
     AudioStitcherVideoMerger objects that do the actual file manipulations. Each video
     (and main sound) will have its AudioStitcherVideoMerger instance.
 
-    All videos are de facto reference recording and matching audio files are
-    looked up for each one of them.
-
     The Matcher doesn't keep neither set any editing information in itself: the
     in and out time values (UTC times) used are those kept inside each Recording
     instances.
 
-    [NOT YET IMPLEMENTED]: When shooting is done with multiple audio recorders,
-    ONE audio device can be designated as 'main sound' and used as reference
-    recording; then all audio tracks are synced together against this main
-    sound audio file, keeping the TicTacCode track alongside for syncing against
-    their video counterpart(in a second pass and after a mixdown editing).
-    [/NOT YET IMPLEMENTED]
-
     Attributes:
 
         recordings : list of Recording instances
             all the scanned recordings with valid TicTacCode, set in __init__()
 
         video_mergers : list
             of AudioStitcherVideoMerger Class instances, built by
-            scan_audio_for_each_ref_rec(); each video has a corresponding
+            scan_audio_for_each_videoclip(); each video has a corresponding
             AudioStitcherVideoMerger object. An audio_stitch doesn't extend
             beyond the corresponding video start and end times.
 
     """
 
     def __init__(self, recordings_list):
         """        
@@ -925,54 +1068,54 @@
             rec_extension = rec.AVpath.suffix
             rel_path_new_name = '%s%s'%(rec.AVpath.stem, rec_extension)
             rec.new_rec_name = Path(rel_path_new_name)
             logger.debug('for %s new name: %s'%(
                 _pathname(rec.AVpath),
                 _pathname(rec.new_rec_name)))
 
-    def scan_audio_for_each_ref_rec(self):
+    def scan_audio_for_each_videoclip(self):
         """
         For each video (and for the Main Sound) in self.recordings, this finds
         any audio that has overlapping times and instantiates a
         AudioStitcherVideoMerger object.
 
         V1 checked against A1, A2, A3, A4
         V2 checked against A1, A2, A3, A4
         V3 checked against    ...
         Main Sound checked against A1, A2, A3, A4
         """
-        refeference_recordings = [r for r in self.recordings if r.is_video()
+        video_recordings = [r for r in self.recordings if r.is_video()
                                                             or r.is_reference]
         audio_recs = [r for r in self.recordings if r.is_audio()
                                                 and not r.is_reference]
         if not audio_recs:
             print('\nNo audio recording found, syncing of videos only not implemented yet, exiting...\n')
             sys.exit(1)
-        for ref_rec in refeference_recordings:
-            reference_tag = 'video' if ref_rec.is_video() else 'audio'
+        for videoclip in video_recordings:
+            reference_tag = 'video' if videoclip.is_video() else 'audio'
             logger.debug('Looking for overlaps with %s %s'%(
                             reference_tag,
-                            ref_rec))
-            audio_stitch = AudioStitcherVideoMerger(ref_rec)
+                            videoclip))
+            audio_stitch = AudioStitcherVideoMerger(videoclip)
             for audio in audio_recs:
-                if self._does_overlap(ref_rec, audio):
+                if self._does_overlap(videoclip, audio):
                     audio_stitch.add_matched_audio(audio)
                     logger.debug('recording %s overlaps,'%(audio))
                     # print('  recording [gold1]%s[/gold1] overlaps,'%(audio))
             if len(audio_stitch.get_matched_audio_recs()) > 0:
                 self.video_mergers.append(audio_stitch)
             else:
                 logger.debug('\n  nothing\n')
-                print('No overlap found for %s'%ref_rec.AVpath.name)
+                print('No overlap found for %s'%videoclip.AVpath.name)
                 del audio_stitch
         logger.debug('%i video_mergers created'%len(self.video_mergers))
 
-    def _does_overlap(self, ref_rec, audio_rec):
+    def _does_overlap(self, videoclip, audio_rec):
         A1, A2 = audio_rec.get_start_time(), audio_rec.get_end_time()
-        R1, R2 = ref_rec.get_start_time(), ref_rec.get_end_time()
+        R1, R2 = videoclip.get_start_time(), videoclip.get_end_time()
         no_overlap = (A2 < R1) or (A1 > R2)
         return not no_overlap
 
     def shrink_gaps_between_takes(self, with_gap=CLUSTER_GAP):
         """
         for single cam shootings this simply sets the gap between takes,
         tweaking each vid timecode metadata to distribute them next to each
@@ -986,19 +1129,19 @@
         or
         1111111111111    222222 (cam A)
           1111111     22222 (cam B)
 
         Returns nothing, changes are done in the video files metadata
         (each referenced by Recording.final_synced_file)
         """
-        vids = [m.ref_recording for m in self.video_mergers]
+        vids = [m.videoclip for m in self.video_mergers]
         logger.debug('vids %s'%vids)
         if len(vids) == 1:
             logger.debug('just one take, no gap to shrink')
-            return
+            return #############################################################
         # INs_and_OUTs contains (time, direction, video) for each video,
         # where direction is 'in|out' and video an instance of Recording
         INs_and_OUTs = [(vid.get_start_time(), 'in', vid) for vid in vids]
         for vid in vids:
             INs_and_OUTs.append((vid.get_end_time(), 'out', vid))
         INs_and_OUTs = sorted(INs_and_OUTs, key=lambda vtuple: vtuple[0])
         logger.debug('INs_and_OUTs: %s'%INs_and_OUTs)
```

### Comparing `tictacsync-0.3a4/tictacsync/yaltc.py` & `tictacsync-0.4a0/tictacsync/yaltc.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,34 +67,34 @@
 
 BPF_LOW_FRQ, BPF_HIGH_FRQ = (0.5*F1, 2*F2)
 
 
 # utility for accessing pathnames
 def _pathname(tempfile_or_path):
     if isinstance(tempfile_or_path, type('')):
-        return tempfile_or_path
+        return tempfile_or_path ################################################
     if isinstance(tempfile_or_path, Path):
-        return str(tempfile_or_path)
+        return str(tempfile_or_path) ###########################################
     if isinstance(tempfile_or_path, tempfile._TemporaryFileWrapper):
-        return tempfile_or_path.name
+        return tempfile_or_path.name ###########################################
     else:
         raise Exception('%s should be Path or tempfile... is %s'%(
             tempfile_or_path,
             type(tempfile_or_path)))
 
 def to_precision(x,p):
     """
     returns a string representation of x formatted with a precision of p
 
     Based on the webkit javascript implementation taken from here:
     https://code.google.com/p/webkit-mirror/source/browse/JavaScriptCore/kjs/number_object.cpp
     """
     x = float(x)
     if x == 0.:
-        return "0." + "0"*(p-1)
+        return "0." + "0"*(p-1) ################################################
     out = []
     if x < 0:
         out.append("-")
         x = -x
     e = int(math.log10(x))
     tens = math.pow(10, e - p + 1)
     n = math.floor(x/tens)
@@ -239,15 +239,15 @@
         relative to extract beginning
         """
         # if self.detected_pulse_position:
         #     logger.debug('returning detected value')
         #     return self.detected_pulse_position
         if self.estimated_pulse_position:
             logger.debug('returning cached estimated value')
-            return self.estimated_pulse_position
+            return self.estimated_pulse_position ###############################
         _, silence_center_x = self._fit_triangular_signal_to_convoluted_env()
         # symbol_width_samples = 1e-3*SYMBOL_LENGTH
         self.estimated_pulse_position = silence_center_x + int(0.5*(
             0.5 - 1e-3*SYMBOL_LENGTH)*self.samplerate)
         logger.debug('returning estimated value from silence mid position')
         return self.estimated_pulse_position
 
@@ -390,16 +390,17 @@
                         self.sound_extract_position,
                         cached_value,
                         abs_tol=0.1)):
             logger.debug('yes, fit values cached:')
             v1 = self.cached_convolution_fit['chi_square']
             v2 = self.cached_convolution_fit['minimum position']
             v2_file = v2 + self.sound_extract_position
-            logger.debug('cached chi_sq: %s minimum position in file: %s'%(v1, v2_file))
-            return (v1, v2)
+            logger.debug('cached chi_sq: %s minimum position in file: %s'%
+                (v1, v2_file))
+            return (v1, v2) ####################################################
                 # cached!
         x_shifted, convolution = self._get_square_convolution()
         # see numpy.convolve(..., mode='valid')
         x = np.arange(len(convolution))
         trig_params = lmfit.Parameters()
         trig_params.add(
             'A', value=1, min=0, max=2
@@ -415,26 +416,27 @@
         def trig_wave(pars, x, signal_data=None):
             # looking for phase sx with a sin of 1 sec period and 0<y<1.0
             A = pars['A']
             p = pars['period']
             mp = pars['min_position']
             model = 2*A*arcsin(abs(sin((x - mp)*2*pi/p)))/pi
             if signal_data is None:
-                return model
+                return model ###################################################
             return model - signal_data
         fit_trig = lmfit.minimize(
                             trig_wave, trig_params,
                             args=(x,), kws={'signal_data': convolution}
                             )
         chi_square = fit_trig.chisqr
         shift = x_shifted[0] # convolution is shorter than sound envelope
         min_position = int(fit_trig.params['min_position'].value) + shift
         logger.debug('chi_square %.1f minimum convolution position %i in file'%
                      (chi_square, min_position + self.sound_extract_position))
-        self.cached_convolution_fit['sound_extract_position'] = self.sound_extract_position
+        self.cached_convolution_fit['sound_extract_position'] = \
+                                                self.sound_extract_position
         self.cached_convolution_fit['chi_square'] = chi_square
         self.cached_convolution_fit['minimum position'] = min_position
 
         return chi_square, min_position + shift
 
     def extract_seems_TicTacCode(self):
         """margin
@@ -461,16 +463,17 @@
         left_window_boundary : int
             left indice.
         right_window_boundary : int
             right indice.
 
         """
         if self.silent_zone_indices:
-            return self.silent_zone_indices
-        _, silence_center_position = self._fit_triangular_signal_to_convoluted_env()
+            return self.silent_zone_indices ####################################
+        _, silence_center_position = \
+            self._fit_triangular_signal_to_convoluted_env()
         srate = self.samplerate
         half_window = int(SAFE_SILENCE_WINDOW_WIDTH * 1e-3 * srate/2)
         left_window_boundary = silence_center_position - half_window
         right_window_boundary = silence_center_position + half_window
         # margin = 0.75 * srate
         values = np.array([left_window_boundary, right_window_boundary,
                     silence_center_position])
@@ -707,15 +710,15 @@
 
     def _get_BFSK_symbols_boundaries(self):
         # returns indices of start of each slice and boundaries
         pulse_position = self._get_pulse_position()
         boundaries_OK, left_boundary, right_boundary = \
                 self._get_BFSK_word_boundaries()
         if left_boundary is None:
-            return None, None, None
+            return None, None, None ############################################
         symbol_width_samples = \
                 float(right_boundary - left_boundary)/N_SYMBOLS_SAMD21
         symbol_positions = symbol_width_samples * \
                 np.arange(float(0), float(N_SYMBOLS_SAMD21 + 1)) + \
                 pulse_position
         int_symb_positions = symbol_positions.round().astype(int)
         logger.debug('%i symbol positions %s samples in file'%
@@ -907,15 +910,15 @@
             return filtered_data
         sample_rate = self.samplerate
         times = np.arange(len(data))/sample_rate
         return _bandpass(data, [BPF_LOW_FRQ, BPF_HIGH_FRQ], sample_rate)
 
     def get_time_in_sound_extract(self, plots):
         if self.sound_extract is None:
-            return None
+            return None ########################################################
         if plots:
             self.make_silence_analysis_plot()
         pulse_position = self._detect_sync_pulse_position()
         pulse_pos_in_file = pulse_position + self.sound_extract_position
         pulse_position_sec = pulse_pos_in_file/self.samplerate
         logger.debug('found sync pulse at sample %i in file'%pulse_pos_in_file)
         symbols_indices, word_lft, word_rght = \
@@ -924,15 +927,15 @@
             title = 'Bit slicing at %s, %.2f s'%(pulse_pos_in_file,
                     pulse_position_sec)
             # self.make_silence_analysis_plot()
             logger.debug('calling _plot_slices()')
             self._plot_slices(pulse_position, symbols_indices, word_lft,
                                 word_rght, title)
         if symbols_indices is None:
-            return None
+            return None ########################################################
         sliced_data = self._slice_sound_extract(symbols_indices)
         frequencies = [self._get_main_frequency(data_slice)
                             for data_slice
                             in sliced_data
                             ]
         logger.debug('frequencies = %s'%frequencies)
         sr = self.samplerate
@@ -946,15 +949,15 @@
         for i, bit in enumerate(bits):
             if bit == None:
                 logger.warning('cant decode frequency %i for bit at %i-%i'%(
                                 corrected_freq[i],
                                 symbols_indices[i],
                                 symbols_indices[i+1]))
         if None in bits:
-            return None
+            return None ########################################################
         bits_string = ''.join(bits)
         logger.debug('bits = %s'%bits_string)
         time_values = self._values_from_bits(bits_string)
         time_values['pulse at'] = (pulse_position +
                                     self.sound_extract_position -
                                     SAMD21_LATENCY*1e-6*self.samplerate)
         time_values['clock source'] = 'GPS' \
@@ -1007,33 +1010,34 @@
             in multi recorders set-ups, user decides if a sound-only recording
             is the time reference for all other audio recordings. By
             default any video recording is the time reference for other audio,
             so this attribute is only relevant to sound recordings and is
             implicitly True for each video recordings (but not set)
 
         device_relative_speed : float
+
             the ratio of the recording device clock speed relative to the
-            reference_rec clock device, in order to correct clock drift with
-            pysox tempo transform. If value < 1.0 then the recording is slower
-            than reference_rec. Updated by each AudioStitcherVideoMerger
-            instance so the value can change depending on the reference
-            recording (video or main sound). A mean is calculated for all
+            video recorder clock device, in order to correct clock drift with
+            pysox tempo transform. If value < 1.0 then the recording is
+            slower than video recorder. Updated by each
+            AudioStitcherVideoMerger instance so the value can change
+            depending on the video recording . A mean is calculated for all
             recordings of the same device in
             AudioStitcherVideoMerger._get_concatenated_audiofile_for()
 
         time_position : float
             The time (in seconds) at which the recording starts relative to the
-            reference recording. Updated by each AudioStitcherVideoMerger
-            instance so the value can change depending on the reference
+            video recording. Updated by each AudioStitcherVideoMerger
+            instance so the value can change depending on the video
             recording (a video or main sound).
 
         final_synced_file : a pathlib.Path
             contains the path of the merged video file after the call to
             AudioStitcher.build_audio_and_write_video if the Recording is a
-            reference recording, relative to the working directory
+            video recording, relative to the working directory
             
         synced_audio : pathlib.Path
             contains the path of audio only of self.final_synced_file. Absolute
             path to tempfile.
 
         in_cam_audio_sync_error : int
             in cam audio sync error, read in the camera folder. Negative value
@@ -1164,18 +1168,18 @@
         float
             recording duration in seconds.
 
         """
         if self.valid_sound:
             val = sox.file_info.duration(_pathname(self.valid_sound))
             logger.debug('duration of valid_sound %f'%val)
-            return val
+            return val #########################################################
         else:
             if self.probe is None:
-                return 0
+                return 0 #######################################################
             try:
                 probed_duration = float(self.probe['format']['duration'])
             except:
                 logger.error('oups, cant find duration from ffprobe')
                 raise Exception('stopping here')
             logger.debug('ffprobed duration is: %f sec'%probed_duration)
             return probed_duration # duration in s
@@ -1288,15 +1292,15 @@
         Returns
         -------
         TYPE
             DESCRIPTION.
 
         """
         if t1 == None or t2 == None:
-            return False
+            return False #######################################################
         logger.debug('t1 : %s t2: %s'%(t1, t2))
         datetime_1 = self._get_timedate_from_dict(t1)
         datetime_2 = self._get_timedate_from_dict(t2)
         # if datetime_2 < datetime_1:
         #     return False
         sample_position_1 = t1['pulse at']
         sample_position_2 = t2['pulse at']
@@ -1330,27 +1334,27 @@
                                 delta_seconds_whole)
         logger.debug('delta samples between pulse %i'%
                                 delta_samples_whole)
         logger.debug('true sample rate = %s Hz'%
                                 to_precision(true_samplerate, 8))
         return true_samplerate
 
-    def set_time_position_to(self, reference_recording):
+    def set_time_position_to(self, video_clip):
         """
         Sets self.time_position, the time (in seconds) at which the recording
-        starts relative to the reference recording. Updated by each AudioStitcherVideoMerger
-        instance so the value can change depending on the reference
+        starts relative to the video recording. Updated by each AudioStitcherVideoMerger
+        instance so the value can change depending on the video
         recording (a video or main sound).
 
         called by timeline.AudioStitcher._get_concatenated_audiofile_for()
         
         """
-        ref_start_time = reference_recording.get_start_time()
+        video_start_time = video_clip.get_start_time()
         self.time_position = (self.get_start_time()
-                                            - ref_start_time).total_seconds()
+                                            - video_start_time).total_seconds()
 
     def get_Dt_with(self, later_recording):
         """
         Returns delta time in seconds
         """
         if not later_recording:
             return 0
@@ -1362,22 +1366,22 @@
         """
         Try to decode a TicTacCode_channel at start AND finish;
         if successful, returns a datetime.datetime instance;
         if not returns None.
         If successful AND self is audio, sets self.valid_sound
         """
         if self.start_time is not None:
-            return self.start_time
+            return self.start_time #############################################
         cached_times = {}
         def find_time(t_sec, plots=False):
             time_k = int(t_sec)
             # if cached_times.has_key(time_k):
             if CACHING and time_k in cached_times:
                 logger.debug('cache hit _find_time_around() for t=%s s'%time_k)
-                return cached_times[time_k]
+                return cached_times[time_k] ####################################
             else:
                 logger.debug('_find_time_around() for t=%s s not cached'%time_k)
                 new_t = self._find_time_around(t_sec, plots)
                 cached_times[time_k] = new_t
                 return new_t
         for i, pair in enumerate(TRIAL_TIMES):
             near_beg, near_end = pair
@@ -1387,15 +1391,15 @@
                                     len(TRIAL_TIMES), near_beg))
             if i > 1:
                 logger.warning('More than one trial: #%i/%i'%(i+1,
                                         len(TRIAL_TIMES)))
             # time_around_beginning = self._find_time_around(near_beg)
             time_around_beginning = find_time(near_beg, plots)
             if self.TicTacCode_channel is None:
-                return None
+                return None ####################################################
             logger.debug('Trial #%i, end at %f'%(i+1, near_end))
             # time_around_end = self._find_time_around(near_end)
             time_around_end = find_time(near_end, plots)
             logger.debug('trial result, time_around_beginning:\n   %s'%
                     (time_around_beginning))
             logger.debug('trial result, time_around_end:\n   %s'%
                     (time_around_end))
@@ -1403,19 +1407,19 @@
                     time_around_beginning,
                     time_around_end)
             logger.debug('_two_times_are_coherent: %s'%coherence) 
             if coherence:
                 break
         if not coherence:
             logger.warning('found times are incoherent')
-            return None
+            return None ########################################################
         if None in [time_around_beginning, time_around_end]:
             logger.warning('didnt find any time in file')
             self.start_time = None
-            return None
+            return None ########################################################
         true_sr = self._compute_true_samplerate(
                         time_around_beginning,
                         time_around_end)
         # self.true_samplerate = to_precision(true_sr,8)
         self.true_samplerate = true_sr
         first_pulse_position = time_around_beginning['pulse at']
         delay_from_start = timedelta(
@@ -1424,140 +1428,142 @@
                                     time_around_beginning)
         in_cam_correction = timedelta(seconds=self.in_cam_audio_sync_arror/1000)
         start_UTC = first_time_date - delay_from_start + in_cam_correction
         logger.debug('recording started at %s'%start_UTC)
         self.start_time = start_UTC
         self.sync_position = time_around_beginning['pulse at']
         if self.is_audio():
-            self.valid_sound = self._strip_TTC_and_Null()
+            # self.valid_sound = self._strip_TTC_and_Null() # why now? :-)
+            self.valid_sound = self.AVpath
         return start_UTC
 
-    def _strip_TTC_and_Null(self) -> tempfile.NamedTemporaryFile:
-        """        
-        TTC is stripped from original audio and a tempfile.NamedTemporaryFile is
-        returned. If the original audio is stereo, this is simply the audio
-        without the TicTacCode channel, so this fct returns a mono wav
-        tempfile. But if the original audio is multitrack, two possibilities:
-
-            A- there's a track.txt file declaring null channels (with '0' tags)
-            then those tracks are excluded too (a check is done those tracks
-            have low signal and warns the user otherwise) 
-
-            B- it's a multitrack recording but without track declaration
-            (no track.txt was found in the device folder): all the tracks are
-            returned into a multiwav tempfile (except TTC).
-
-        Notes:
-            'track.txt' is defined in device_scanner.TRACKSFN 
-
-            Beware of track indexing: sox starts indexing tracks at 1 but code
-            here uses zero based indexing.
-        """
-        tracks_file = self.device.folder/device_scanner.TRACKSFN
-        input_file = _pathname(self.AVpath)
-        # n_channels = sox.file_info.channels(input_file) # eg 2
-        n_channels = self.device.n_chan
-        sox_TicTacCode_channel = self.TicTacCode_channel + 1 # sox channels start at 1
-        if n_channels == 2:
-            logger.debug('stereo, so only excluding TTC (ZB idx) %i'%
-                    self.TicTacCode_channel)
-            return self._sox_strip(input_file, [self.TicTacCode_channel])
-        # First a check is done if the ttc tracks concur: the track detected
-        # by the Decoder class, stored in Recording.TicTacCode_channel VS the
-        # track declared by the user, Tracks.ttc (see device_scanner.py). If
-        # not, warn the user and exit.
-        trax = self.device.tracks # a Tracks dataclass instance, if any
-        logger.debug('trax %s'%trax)
-        if trax == None: #TO DO: mix or mixL, mixR or do mixdown
-            return self._sox_strip(input_file, [self.TicTacCode_channel])
-        else:
-            logger.debug('ttc channel declared for the device: %i, ttc detected: %i, non zero base indexing'%
-                        (trax.ttc, sox_TicTacCode_channel))
-        if trax.ttc != sox_TicTacCode_channel: # warn and quit
-            print('Error: TicTacCode channel detected is [gold1]%i[/gold1]'%
-                sox_TicTacCode_channel, end=' ')
-            print('and the file [gold1]%s[/gold1] specifies channel [gold1]%i[/gold1],'%
-                (tracks_file, trax.ttc))
-            print('Please correct the discrepancy and rerun. Quitting.')
-            sys.exit(1)
-        track_is_declared_audio = [ tag not in ['ttc','0','tc']
-                                    for tag in trax.rawtrx]
-        logger.debug('from tracks_file %s'%tracks_file)
-        logger.debug('track_is_declared_audio (not ttc or 0): %s'%
-                                                track_is_declared_audio)
-        # Now find out which files are silent, ie those with sox stats "RMS lev
-        # db" value inferior to DB_RMS_SILENCE_SOX (typ -50 -60 dbFS) from the
-        # sox "stat" command. Ex output belwow:
-        #
-        # sox input.wav -n channels stats -w 0.01
-        #
-        #              Overall     Ch1       Ch2       Ch3       Ch4  
-        # DC offset  -0.000047 -0.000047 -0.000047 -0.000016 -0.000031
-        # Min level  -0.060913 -0.060913 -0.048523 -0.036438 -0.002777
-        # Max level   0.050201  0.050201  0.048767  0.039032  0.002838
-        # Pk lev dB     -24.31    -24.31    -26.24    -28.17    -50.94
-        # RMS lev dB    -40.33    -55.29    -53.70    -34.41    -59.75 <- this line
-        # RMS Pk dB     -28.39    -28.39    -30.90    -31.20    -55.79
-        # RMS Tr dB     -97.42    -79.66    -75.87    -97.42    -96.09
-        # Crest factor       -     35.41     23.61      2.05      2.76
-        # Flat factor     6.93      0.00      0.00      0.97     10.63
-        # Pk count        10.2         2         2        17        20
-        # Bit-depth      12/16     12/16     12/16     12/16      8/16
-        # Num samples    11.2M
-        # Length s     232.780
-        # Scale max   1.000000
-        # Window s       0.010
-        args = ['sox', input_file, '-n', 'channels', 'stats', '-w', '0.01']
-        _, _, stat_output = sox.core.sox(args)
-        logger.debug('sox stat output: \n%s'%stat_output)
-        sox_RMS_lev_dB = stat_output.split('\n')[5].split()[4:]
-        logger.debug('Rec %s'%self)
-        logger.debug('Sox RMS %s, n_channels: %i'%(sox_RMS_lev_dB, n_channels))
-        # valid audio is non silent and not ttc
-        track_is_active = [float(db) > DB_RMS_SILENCE_SOX
-            if idx + 1 != sox_TicTacCode_channel else False
-            for idx, db in enumerate(sox_RMS_lev_dB)]
-        logger.debug('track_is_active %s'%track_is_active)
-        # Stored in self.device.tracks and as declared by the user, a track is
-        # either:
-        #
-        # - an active track (because a name was given to it)
-        # - the ttc track (as identified by the user)
-        # - a muted track (declared by a "0" in tracks.txt)
-        #
-        # the following checks active tracks are effectively non silent and
-        # muted tracks are effectively silent (warn the user if not but
-        # proceed, giving priority to status declared in the tracks.txt file.
-        # eg a non silent track will be discarded if the user tagged it with
-        # a "0")
-        declared_and_detected_are_same = all([a==b for a,b
-            in zip(track_is_declared_audio, track_is_active)])
-        logger.debug('declared_and_detected_are_same: %s'%
-                                declared_and_detected_are_same)
-        if not declared_and_detected_are_same:
-            print('Warning, the file [gold1]%s[/gold1] specifies channel usage'%
-                (tracks_file))
-            print('and some muted tracks are not silent (or the inverse, see below),')
-            print('will proceed but if it\'s an error do necessary corrections and rerun.\n')
-            table = Table(title="Tracks status")
-            table.add_column("track #", justify="center", style='gold1')
-            table.add_column("RMS Level", justify="center", style='gold1')
-            table.add_column("Declared", justify="center", style='gold1')
-            for n in range(n_channels):
-                table.add_row(str(n+1), '%.0f dBFS'%float(sox_RMS_lev_dB[n]),
-                    trax.rawtrx[n])
-            console = Console()
-            console.print(table)
-        if trax:
-            excluded_channels = [i for i in range(n_channels)
-                if not track_is_declared_audio[i]]
-        else:
-            excluded_channels = [self.TicTacCode_channel]
-        logger.debug('excluded_channels %s (ZB idx)'%excluded_channels)
-        return self._sox_strip(input_file, excluded_channels)
+    # def _strip_TTC_and_Null(self) -> tempfile.NamedTemporaryFile:
+    #     """        
+    #     TTC is stripped from original audio and a tempfile.NamedTemporaryFile is
+    #     returned. If the original audio is stereo, this is simply the audio
+    #     without the TicTacCode channel, so this fct returns a mono wav
+    #     tempfile. But if the original audio is multitrack, two possibilities:
+
+    #         A- there's a track.txt file declaring null channels (with '0' tags)
+    #         then those tracks are excluded too (a check is done those tracks
+    #         have low signal and warns the user otherwise) 
+
+    #         B- it's a multitrack recording but without track declaration
+    #         (no track.txt was found in the device folder): all the tracks are
+    #         returned into a multiwav tempfile (except TTC).
+
+    #     Notes:
+    #         'track.txt' is defined in device_scanner.TRACKSFN 
+
+    #         Beware of track indexing: sox starts indexing tracks at 1 but code
+    #         here uses zero based indexing.
+    #     """
+    #     tracks_file = self.device.folder/device_scanner.TRACKSFN
+    #     input_file = _pathname(self.AVpath)
+    #     # n_channels = sox.file_info.channels(input_file) # eg 2
+    #     n_channels = self.device.n_chan
+    #     sox_TicTacCode_channel = self.TicTacCode_channel + 1 # sox start at 1
+    #     if n_channels == 2:
+    #         logger.debug('stereo, so only excluding TTC (ZB idx) %i'%
+    #                 self.TicTacCode_channel)
+    #         return self._sox_strip(input_file, [self.TicTacCode_channel]) ######
+    #     #
+    #     # First a check is done if the ttc tracks concur: the track detected
+    #     # by the Decoder class, stored in Recording.TicTacCode_channel VS the
+    #     # track declared by the user, Tracks.ttc (see device_scanner.py). If
+    #     # not, warn the user and exit.
+    #     trax = self.device.tracks # a Tracks dataclass instance, if any
+    #     logger.debug('trax %s'%trax)
+    #     if trax == None:
+    #         return self._sox_strip(input_file, [self.TicTacCode_channel]) ######
+    #     else:
+    #         logger.debug('ttc channel declared for the device: %i, ttc detected: %i, non zero base indexing'%
+    #                     (trax.ttc, sox_TicTacCode_channel))
+    #     if trax.ttc != sox_TicTacCode_channel: # warn and quit
+    #         print('Error: TicTacCode channel detected is [gold1]%i[/gold1]'%
+    #             sox_TicTacCode_channel, end=' ')
+    #         print('and the file [gold1]%s[/gold1] specifies channel [gold1]%i[/gold1],'%
+    #             (tracks_file, trax.ttc))
+    #         print('Please correct the discrepancy and rerun. Quitting.')
+    #         sys.exit(1)
+    #     track_is_declared_audio = [ tag not in ['ttc','0','tc']
+    #                                 for tag in trax.rawtrx]
+    #     logger.debug('from tracks_file %s'%tracks_file)
+    #     logger.debug('track_is_declared_audio (not ttc or 0): %s'%
+    #                                             track_is_declared_audio)
+    #     # Now find out which files are silent, ie those with sox stats "RMS lev
+    #     # db" value inferior to DB_RMS_SILENCE_SOX (typ -50 -60 dbFS) from the
+    #     # sox "stat" command. Ex output belwow:
+    #     #
+    #     # sox input.wav -n channels stats -w 0.01
+    #     #
+    #     #              Overall     Ch1       Ch2       Ch3       Ch4  
+    #     # DC offset  -0.000047 -0.000047 -0.000047 -0.000016 -0.000031
+    #     # Min level  -0.060913 -0.060913 -0.048523 -0.036438 -0.002777
+    #     # Max level   0.050201  0.050201  0.048767  0.039032  0.002838
+    #     # Pk lev dB     -24.31    -24.31    -26.24    -28.17    -50.94
+    #     # RMS lev dB    -40.33    -55.29    -53.70    -34.41    -59.75 <- this line
+    #     # RMS Pk dB     -28.39    -28.39    -30.90    -31.20    -55.79
+    #     # RMS Tr dB     -97.42    -79.66    -75.87    -97.42    -96.09
+    #     # Crest factor       -     35.41     23.61      2.05      2.76
+    #     # Flat factor     6.93      0.00      0.00      0.97     10.63
+    #     # Pk count        10.2         2         2        17        20
+    #     # Bit-depth      12/16     12/16     12/16     12/16      8/16
+    #     # Num samples    11.2M
+    #     # Length s     232.780
+    #     # Scale max   1.000000
+    #     # Window s       0.010
+    #     args = ['sox', input_file, '-n', 'channels', 'stats', '-w', '0.01']
+    #     _, _, stat_output = sox.core.sox(args)
+    #     logger.debug('sox stat output: \n%s'%stat_output)
+    #     sox_RMS_lev_dB = stat_output.split('\n')[5].split()[4:]
+    #     logger.debug('Rec %s'%self)
+    #     logger.debug('Sox RMS %s, n_channels: %i'%(sox_RMS_lev_dB, n_channels))
+    #     # valid audio is non silent and not ttc
+    #     track_is_active = [float(db) > DB_RMS_SILENCE_SOX
+    #         if idx + 1 != sox_TicTacCode_channel else False
+    #         for idx, db in enumerate(sox_RMS_lev_dB)]
+    #     logger.debug('track_is_active %s'%track_is_active)
+    #     # Stored in self.device.tracks and as declared by the user, a track is
+    #     # either:
+    #     #
+    #     # - an active track (because a name was given to it)
+    #     # - the ttc track (as identified by the user)
+    #     # - a muted track (declared by a "0" in tracks.txt)
+    #     #
+    #     # the following checks active tracks are effectively non silent and
+    #     # muted tracks are effectively silent (warn the user if not but
+    #     # proceed, giving priority to status declared in the tracks.txt file.
+    #     # eg a non silent track will be discarded if the user tagged it with
+    #     # a "0")
+    #     declared_and_detected_are_same = all([a==b for a,b
+    #         in zip(track_is_declared_audio, track_is_active)])
+    #     logger.debug('declared_and_detected_are_same: %s'%
+    #                             declared_and_detected_are_same)
+    #     if not declared_and_detected_are_same:
+    #         print('Warning, the file [gold1]%s[/gold1] specifies channel usage'%
+    #             (tracks_file))
+    #         print('and some muted tracks are not silent (or the inverse, see below),')
+    #         print('will proceed but if it\'s an error do necessary corrections and rerun.\n')
+    #         table = Table(title="Tracks status")
+    #         table.add_column("track #", justify="center", style='gold1')
+    #         table.add_column("RMS Level", justify="center", style='gold1')
+    #         table.add_column("Declared", justify="center", style='gold1')
+    #         for n in range(n_channels):
+    #             table.add_row(str(n+1), '%.0f dBFS'%float(sox_RMS_lev_dB[n]),
+    #                 trax.rawtrx[n])
+    #         console = Console()
+    #         console.print(table)
+    #     if trax:
+    #         excluded_channels = [i for i in range(n_channels)
+    #             if not track_is_declared_audio[i]]
+    #     else:
+    #         excluded_channels = [self.TicTacCode_channel]
+    #     logger.debug('excluded_channels %s (ZB idx)'%excluded_channels)
+    #     return self._sox_strip(input_file, excluded_channels)
 
 
 
     def _sox_strip(self, audio_file, excluded_channels) -> tempfile.NamedTemporaryFile:
         # building dict according to pysox.remix format.
         # https://pysox.readthedocs.io/en/latest/api.html#sox.transform.Transformer.remix
         # eg: 4 channels with TicTacCode_channel at #2 
@@ -1627,21 +1633,21 @@
         true = self.true_samplerate
         if true > nominal:
             ppm = (true/nominal - 1) * 1e6
         else:
             ppm = - (nominal/true - 1) * 1e6
         return int(ppm)
 
-    def get_speed_ratio(self, ref_recording):
+    def get_speed_ratio(self, videoclip):
         nominal = self.get_samplerate()
         true = self.true_samplerate
         ratio = true/nominal
-        nominal_ref = ref_recording.get_samplerate()
-        true_ref = ref_recording.true_samplerate
-        ratio_ref = true_ref/nominal_ref
+        nominal_vid = videoclip.get_samplerate()
+        true_ref = videoclip.true_samplerate
+        ratio_ref = true_ref/nominal_vid
         return ratio/ratio_ref
 
     def get_samplerate(self):
         # return int samplerate (nominal)
         string = self._ffprobe_audio_stream()['sample_rate']
         return eval(string) # eg eval(24000/1001)
 
@@ -1684,28 +1690,28 @@
             logger.error(e)
             logger.error(e.stderr)
         os.remove(_pathname(video_path))
         shutil.copy(_pathname(file_handle), _pathname(video_path))
 
     def has_audio(self):
         if not self.probe:
-            return False
+            return False #######################################################
         streams = self.probe['streams']
         codecs = [stream['codec_type'] for stream in streams]
         return 'audio' in codecs
 
     def get_audio_channels_nbr(self):
         if not self.has_audio():
-            return 0
+            return 0 ###########################################################
         audio_str = self._ffprobe_audio_stream()
         return audio_str['channels']
 
     def is_video(self):
         if not self.probe:
-            return False
+            return False #######################################################
         streams = self.probe['streams']
         codecs = [stream['codec_type'] for stream in streams]
         return 'video' in codecs
 
     def is_audio(self):
         return not self.is_video()
 
@@ -1738,15 +1744,15 @@
         path = self.AVpath
         decoder = self.decoder
         if decoder:
             decoder.clear_decoder()
         # decoder.cached_convolution_fit['is clean'] = False
         if not self.has_audio():
             self.TicTacCode_channel = None
-            return
+            return #############################################################
         logger.debug('will read around %.2f sec'%time_where)
         dryrun = (ffmpeg
             .input(str(path), ss=time_where, t=chunk_length)
             .output('pipe:', format='s16le', acodec='pcm_s16le')
             .get_args())
         dryrun = ' '.join(dryrun)
         logger.debug('using ffmpeg-python built args to pipe wav file into numpy array:\nffmpeg %s'%dryrun)
@@ -1771,26 +1777,28 @@
             decoder.set_sound_extract_and_sr(
                     chan_dat,
                     self.get_samplerate(),
                     sound_extract_position
                     )
             if decoder.extract_seems_TicTacCode():
                 self.TicTacCode_channel = i_chan
+                self.device.ttc = i_chan
                 logger.debug('find TicTacCode channel, chan #%i'%
                                 self.TicTacCode_channel)
-                return self
+                return self ####################################################
         # end of loop: none found
         self.TicTacCode_channel = None
         logger.warning('found no TicTacCode channel')
         return self
     
     def seems_to_have_TicTacCode_at_beginning(self):
         if self.probe is None:
-            return False
-        self._read_sound_find_TicTacCode(TRIAL_TIMES[0][0], SOUND_EXTRACT_LENGTH)
+            return False #######################################################
+        self._read_sound_find_TicTacCode(TRIAL_TIMES[0][0],
+            SOUND_EXTRACT_LENGTH)
         return self.TicTacCode_channel is not None
 
     def does_overlap_with_time(self, time):
         A1, A2 = self.get_start_time(), self.get_end_time()
         # R1, R2 = rec.get_start_time(), rec.get_end_time()
         # no_overlap = (A2 < R1) or (A1 > R2)
         return time >= A1 and time <= A2
```

### Comparing `tictacsync-0.3a4/tictacsync.egg-info/PKG-INFO` & `tictacsync-0.4a0/tictacsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tictacsync
-Version: 0.3a4
+Version: 0.4a0
 Summary: command for syncing audio video recordings
 Home-page: https://tictacsync.org/
 Author: Raymond Lutz
 Author-email: lutzrayblog@mac.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

