# Comparing `tmp/soundtools-0.2.0.2.tar.gz` & `tmp/soundtools-0.2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.2.0.2.tar", last modified: Mon Apr 15 02:23:29 2024, max compression
+gzip compressed data, was "soundtools-0.2.0.3.tar", last modified: Thu Apr 18 19:28:47 2024, max compression
```

## Comparing `soundtools-0.2.0.2.tar` & `soundtools-0.2.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 02:23:29.634908 soundtools-0.2.0.2/
--rw-rw-rw-   0        0        0      709 2024-04-15 02:23:29.634733 soundtools-0.2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 02:23:29.634908 soundtools-0.2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      797 2024-04-15 02:23:19.000000 soundtools-0.2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:23:29.632233 soundtools-0.2.0.2/soundtools/
--rw-rw-rw-   0        0        0      399 2024-04-15 02:22:44.000000 soundtools-0.2.0.2/soundtools/__init__.py
--rw-rw-rw-   0        0        0    35969 2024-04-15 02:22:55.000000 soundtools-0.2.0.2/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:23:29.633231 soundtools-0.2.0.2/soundtools.egg-info/
--rw-rw-rw-   0        0        0      709 2024-04-15 02:23:29.000000 soundtools-0.2.0.2/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-15 02:23:29.000000 soundtools-0.2.0.2/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 02:23:29.000000 soundtools-0.2.0.2/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-15 02:23:29.000000 soundtools-0.2.0.2/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 19:28:47.272583 soundtools-0.2.0.3/
+-rw-rw-rw-   0        0        0      701 2024-04-18 19:28:47.243954 soundtools-0.2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 19:28:47.272583 soundtools-0.2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-04-18 19:28:21.000000 soundtools-0.2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:28:47.240954 soundtools-0.2.0.3/soundtools/
+-rw-rw-rw-   0        0        0      399 2024-04-18 19:27:17.000000 soundtools-0.2.0.3/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    36660 2024-04-18 19:27:25.000000 soundtools-0.2.0.3/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:28:47.243954 soundtools-0.2.0.3/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-04-18 19:28:47.000000 soundtools-0.2.0.3/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-18 19:28:47.000000 soundtools-0.2.0.3/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 19:28:47.000000 soundtools-0.2.0.3/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-18 19:28:47.000000 soundtools-0.2.0.3/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.2.0.2/PKG-INFO` & `soundtools-0.2.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.0.2
+Version: 0.2.0.3
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
-### made by Mohammad Erfan Karami
+made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-### version: 0.2.0.2
+version: 0.2.0.3
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

### Comparing `soundtools-0.2.0.2/setup.py` & `soundtools-0.2.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 setup(
 name='soundtools',
-version='0.2.0.2',
+version='0.2.0.3',
 description="used to work with sounds waves",
-long_description="""### made by Mohammad Erfan Karami
+long_description="""made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-### version: 0.2.0.2
+version: 0.2.0.3
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves""",
 author='Mohammad Erfan Karami',
```

### Comparing `soundtools-0.2.0.2/soundtools/soundtools.py` & `soundtools-0.2.0.3/soundtools/soundtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """### made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-### version: 0.2.0.2
+### version: 0.2.0.3
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves"""
 
@@ -80,16 +80,15 @@
                 name = f"{wave_type}|{freq}|{dur}"
                 if name in self.existed_notes.keys():
                     wave = vol * np.array(self.existed_notes[name], dtype=self.dtype)
                     return wave
                 
                 temp = func(self, freq, dur, self.max_amp)
                 result: SoundBuffer = func(self, freq, dur, vol)
-                result[result > self.max_amp] = self.max_amp
-                result[result < self.min_amp] = self.min_amp
+                result = self._fix_amp(result)
                 self.existed_notes[name] = self.array_to_tuple(temp)
                 
                 return result
             return wrapper
         return decorator
 
     @cache_wave("sine")
@@ -236,44 +235,50 @@
         buf += vol*0.9 * np.sin(pi_2_samples_num * freq*2 / self.default_sample_rate)
         buf += vol * np.sin(pi_2_samples_num * freq*4 / self.default_sample_rate)
         buf += vol*0.6 * np.sin(pi_2_samples_num * freq*6 / self.default_sample_rate)
         buf += vol*0.7 * np.sin(pi_2_samples_num * freq*16 / self.default_sample_rate)
         buf += vol*0.5 * np.sin(pi_2_samples_num * freq*20 / self.default_sample_rate)
         buf += vol*0.3 * np.sin(pi_2_samples_num * freq*24 / self.default_sample_rate)
 
-        wave = (buf/7).astype(self.dtype)
+        wave = (buf/7*0.4247).astype(self.dtype)
         return wave
     
     @cache_wave("marimb")
     def marimba(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a "not even close to marimba" sound based on the given frequency, duration and amplitude or volume\n
         warning!: very annoying sound"""
         
         pi_2_samples_num = self.tau * np.arange(self.default_sample_rate * dur)
         buf = vol * np.sin(pi_2_samples_num * freq / self.default_sample_rate)
         buf += vol*0.75 * np.sin(pi_2_samples_num * freq*10 / self.default_sample_rate)
         buf += vol/2 * np.sin(pi_2_samples_num * freq*20 / self.default_sample_rate)
         buf += vol/4 * np.sin(pi_2_samples_num * freq*30 / self.default_sample_rate)
         
         wave = (buf/4).astype(self.dtype)
-        return wave
+        return self.fade_out(wave, wave.size)
     
     @cache_wave("tst")
     def test(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         buf = np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
         for h in range(1, 1000):
             f = freq*h
             if f > 20000:
                 break
             buf += (-1)**h * (np.sin(self.tau * np.arange(self.default_sample_rate * dur) * f / self.default_sample_rate)/h)
         
         wave = (vol * (0.5 - self.rev_pi*buf)).astype(self.dtype)
         return wave
     
     
+    def _fix_amp(self, wave: SoundBuffer) -> SoundBuffer:
+        wave[wave > self.max_amp] = self.max_amp
+        wave[wave < self.min_amp] = self.min_amp
+        return wave
+    
+    
     def _generate_fade_buffer(self, fade_len:int = 1500, dtype: Dtype|None=None) -> SoundBuffer:
         dtype = self.dtype if not dtype else dtype
         return ((1 - np.cos(np.linspace(0, np.pi, fade_len))) * 0.5).astype(dtype)
     
     
     def fade_in(self, buffer: SoundBuffer, fadein_len:int = 1500) -> SoundBuffer:
         fadein = self._generate_fade_buffer(fadein_len, buffer.dtype)
@@ -717,14 +722,32 @@
         
         self.input_stream.stop_stream()
         
         buf = np.frombuffer(total_frames, self.input_dtype)
         return buf
     
     
+    def add_buffers(a: SoundBuffer, b: SoundBuffer) -> SoundBuffer:
+        s = a.size if a.size < b.size else b.size
+        return a[:s] + b[:s]
+    
+    
+    def add_multiple_buffers(*buffers: SoundBuffer):
+        s: int = buffers[0].size
+        for buffer in buffers[1:]:
+            if buffer.size < s:
+                s = buffer.size
+        
+        s_bufs: SoundBuffer = buffers[0][:s]
+        
+        for buffer in buffers[1:]:
+            s_bufs += buffer
+            
+        return s_bufs / len(buffers)
+    
     # creates a note buffer and plays it
     def play(self, note:str|float|int, wave_type: Wave, duration:str|float=0, volume:float=0) -> None:
         """generates then plays a note with the given arguments"""
         buf: bytes = self.generate_note_buffer(note, wave_type, duration, volume).tobytes()
     
         self.play_buffer(buf)
```

### Comparing `soundtools-0.2.0.2/soundtools.egg-info/PKG-INFO` & `soundtools-0.2.0.3/soundtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.0.2
+Version: 0.2.0.3
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
-### made by Mohammad Erfan Karami
+made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-### version: 0.2.0.2
+version: 0.2.0.3
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

