# Comparing `tmp/python_flux-1.0.6.tar.gz` & `tmp/python_flux-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.0.6.tar", max compression
+gzip compressed data, was "python_flux-1.0.7.tar", max compression
```

## Comparing `python_flux-1.0.6.tar` & `python_flux-1.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6515 2024-04-17 03:02:32.796113 python_flux-1.0.6/README.rst
--rw-r--r--   0        0        0      741 2024-04-17 02:42:41.927336 python_flux-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.6/python_flux/__init__.py
--rw-r--r--   0        0        0    15929 2024-04-17 03:02:42.202543 python_flux-1.0.6/python_flux/flux.py
--rw-r--r--   0        0        0      768 2024-04-17 01:57:13.061985 python_flux-1.0.6/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1596 2024-04-14 04:36:37.930223 python_flux-1.0.6/python_flux/producers.py
--rw-r--r--   0        0        0     1348 2024-04-17 01:56:35.567056 python_flux-1.0.6/python_flux/subscribers.py
--rw-r--r--   0        0        0     7246 1970-01-01 00:00:00.000000 python_flux-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6725 2024-04-18 05:33:58.138883 python_flux-1.0.7/README.rst
+-rw-r--r--   0        0        0      741 2024-04-18 05:33:57.671021 python_flux-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.7/python_flux/__init__.py
+-rw-r--r--   0        0        0    16352 2024-04-18 05:33:57.671955 python_flux-1.0.7/python_flux/flux.py
+-rw-r--r--   0        0        0      758 2024-04-18 05:33:57.672479 python_flux-1.0.7/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1596 2024-04-14 04:36:37.930223 python_flux-1.0.7/python_flux/producers.py
+-rw-r--r--   0        0        0     1641 2024-04-18 05:33:57.673160 python_flux-1.0.7/python_flux/subscribers.py
+-rw-r--r--   0        0        0     7456 1970-01-01 00:00:00.000000 python_flux-1.0.7/PKG-INFO
```

### Comparing `python_flux-1.0.6/README.rst` & `python_flux-1.0.7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 Permite modificar el valor de un flujo.
 
 Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo y se substituirá en el mismo por lo obtenido de la función.
 
 -  **map_function**: función(valor, contexto) desde donde se obtendrá el valor a sustituir.
 
 
-map_context(map_context_function):
-----------------------------------
+map_context(map_context_function)
+---------------------------------
 
 Permite modificar el contexto de un flujo.
 
 Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo y retornará un nuevo contexto que sustituirá al actual
 
 -  **map_context_function**: función(valor, contexto) desde donde se obtendrá el contexto a subsituir.
 
@@ -85,22 +85,24 @@
 Corta la ejecución del flujo luego de n segundos de procesamiento.
 
 La ejecución se cortará si al momento de evaluar este paso el tiempo transcurrido fue superior al configurado.
 
 -  **n**: Cantidad de segundos que el stream procesa elementos.
 
 
-log(message=lambda v, c: str(v), level=logging.INFO)
-----------------------------------------------------
+log(build_log_message, build_error_message, level)
+--------------------------------------------------
 
 Recibe una función(valor, contexto) que retorna un mensaje de texto que será logueado con el nivel de log indicado en level.
 
 El logueo se hace de forma asincrónica y no afecta al flujo.
 
--  **message**: Función que dado un valor y contexto retorna un mensaje a loguear.
+-  **build_log_message**: Función que dado un valor y contexto retorna un mensaje a loguear
+
+-  **build_error_message**: Función que dada una excepción y el contexto retorna el mensaje a loguear como ERROR
 
 -  **level**: Nivel de logueo que se usará
 
 
 on_error_resume(resume=fu.default_error_resume, exceptions=[Exception])
 -----------------------------------------------------------------------
 En caso de error, este paso ejecuta la función resume que debe retornar un valor a partir del error recibido por parámetro.
@@ -109,31 +111,32 @@
 
 -  **exceptions**: Lista de excepciones para los que se aplica la función resume.
 
 
 on_error_retry(retries=3, delay_ms=lambda i: 0, exceptions=[Exception])
 -----------------------------------------------------------------------
 
-En caso de error, este paso intenta ejecutar nuevamente el flujo
-**retries** cantidad de veces.
+En caso de error, este paso intenta ejecutar nuevamente el flujo **retries** cantidad de veces.
 
 Esto lo hace sólo para las excepciones indicadas por **exceptions** y los reintentos tienen un delay dado por la función **delay_ms** que recibe el número de reintento que es y espera obtener los ms de delay que se deben aplicar.
 
 -  **retries**: Cantidad de reintentos a aplicar
 
 -  **delay_ms**: función(int) que retorna dado el número de reintento en el que se está cuantos: ms de delay se deben aplicar.
 
 -  **exceptions**: Lista de excepciones para los que se aplica el método resume.
 
 
-subscribe(context={})
----------------------
+subscribe(skip_error, context)
+------------------------------
 
 Crea un objeto iterable a partir del flujo. Si se itera sobre este objeto se obtendrán los valores del flujo.
 
+-  **skip_error**: Ignora errores al obtener los valores desde el flujo
+
 -  **context**: Contexto inicial para el flujo
 
 -  **return**: Objeto iterable
 
 
 foreach(on_success=fu.default_success, on_error=fu.default_error, context={})
 -----------------------------------------------------------------------------
```

### Comparing `python_flux-1.0.6/pyproject.toml` & `python_flux-1.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "1.0.6"
+version = "1.0.7"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `python_flux-1.0.6/python_flux/flux.py` & `python_flux-1.0.7/python_flux/flux.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import threading
 import types
 import time
 from datetime import timedelta, datetime
 from functools import partial
 from jsonmerge import merge
 from python_flux.flux_utilis import FluxUtils as fu
-from python_flux.subscribers import SSubscribe, SForeach
+from python_flux.subscribers import SSubscribe
 
 
 class Flux(object):
 
     def filter(self, predicate, on_mismatch=fu.default_action):
         """
         Permite filtrar un flujo perimtiendo continuar a aquellos valores que cumplen con el
@@ -88,34 +88,38 @@
         La ejecición se cortará si al momento de evaluar este paso el tiempo transcurrido fue superior
         al configurado.
 
         :param n: Cantidad de segundos que el stream procesará elementos.
         """
         return FTakeDuringTimeDelta(n, self)
 
-    def log(self, message=lambda v, c: str(v), level=logging.INFO):
+    def log(self, build_log_message=lambda v, c: str(v), build_error_message=lambda e, c: str(v), level=logging.INFO):
         """
         Recibe una función(valor, contexto) que retorna un mensaje de texto que será logueado con el
         nivel de log indicado en level.
         El logueo se hace de forma asincrónica y no afecta al flujo.
 
-        :param message: Función que dado un valor y contexto retorna un mensaje a loguear.
+        :param build_log_message: Función que dado un valor y contexto retorna un mensaje a loguear
+        :param build_error_message: Función que dada una excepción y el contexto retorna el mensaje a loguear como ERROR
         :param level: Nivel de logueo que se usará
         """
         def log_function(l, msg, v, c):
-            if l is logging.ERROR:
-                logging.error(msg(v, c))
-            elif l is logging.WARNING or l is logging.WARN:
-                logging.warning(msg(v, c))
+            message = msg(v, c)
+            if l is logging.WARNING or l is logging.WARN:
+                logging.warning(message)
             elif l is logging.INFO:
-                logging.info(msg(v, c))
+                logging.info(message)
             elif l is logging.DEBUG:
-                logging.debug(msg(v, c))
+                logging.debug(message)
 
-        return FDoOnNext(partial(log_function, level, message), self)
+        def log_error(msg, e, c):
+            message = msg(e, c)
+            logging.error(message)
+
+        return FDoOnNext(partial(log_function, level, build_log_message), partial(log_error, build_error_message), True, self)
 
     def on_error_resume(self, resume=fu.default_error_resume, exceptions=[Exception]):
         """
         En caso de error, este paso ejecuta la función resume que debe retornar un valor
         a partir del error recibido por parámetro.
 
         :param resume: función(ex, contexto) Debe retornar el valor a substituir en el flujo.
@@ -133,65 +137,65 @@
         :param retries: Cantidad de reintentos a aplicar
         :param delay_ms: función(int) que retorna dado el número de reintento en el que se está cuantos
                   ms de delay se deben aplicar.
         :param exceptions: Lista de excepciones para los que se aplica el resume.
         """
         return FOnErrorRetry(retries, exceptions, delay_ms, self)
 
-    def subscribe(self, context={}):
+    def subscribe(self, context={}, skip_error=False):
         """
         Crea un objeto iterable a partir del flujo. Si se itera sobre este objeto se obtendrán
         los valores del flujo.
+        :param skip_error: Ignora errores al obtener los valores desde el flujo
         :param context: Contexto inicial para el flujo
         :return: Objeto iterable
         """
-        return SSubscribe(context, self)
+        return SSubscribe(skip_error, context, self)
 
     def foreach(self, on_success=fu.default_success, on_error=fu.default_error, on_finish=fu.default_finish, context={}):
         """
         Itera sobre los elementos del flujo e invoca a funciones on_success y on_error dependiendo
         el estado del flujo.
         :param on_success: función(valor, contexto) se invoca si el flujo procesa correctamente un valor
         :param on_error:  función(ex, contexto) se invoca si hay un error en el flujo.
                           Esto no corta el procesamiento a menos que se lance una excepción en el método
         :param on_finish: función(contexto) se invoca al finalizar el flujo
         :param context: Contexto inicial para el flujo
         """
-        flux = self.subscribe(context)
+        flux = self.subscribe(context, True)
         while True:
             try:
                 value = next(flux)
                 fu.try_or(partial(on_success), value, context)
             except StopIteration:
+                fu.try_or(partial(on_finish), context)
                 return
             except Exception as ex:
                 _, e = fu.try_or(partial(on_error), ex, context)
-                if e is not None:
-                    raise e
 
     def to_list(self, context={}):
         """
         Itera sobre los elementos del flujo y los retorna todos dentro de una lista.
         :param context: contexto inicial para el flujo
         :return: Lista de elementos
         """
-        return list(iter(SSubscribe(context, self)))
+        return list(iter(SSubscribe(True, context, self)))
 
     def collect(self, init=lambda c: {}, reduce=lambda v, a: a, context={}):
         """
-        Permite resumir en un sólo objeto el procesamiento de todos los elementos del flujo.
+        Permite agrupar en un sólo objeto el resultado del procesamiento de todos los elementos del flujo.
         Se inicializa un acumulador a través de la función init(contexto) y luego para cada elemento del flujo
         se invoca la función reduce(valor, acumulador) que procesa el valor y retorna un nuevo valor del acumulador.
         :param init: función(contexto) Retorna valor inicial del acumulador
         :param reduce: funcón(valor, acumulador) Dados el nuevo valor y el acumulador retorna un nuevo valor de acumulador.
         :param context: Contexto inicial para el flujo
         :return: Acumulador
         """
         acum = init(context)
-        flux = self.subscribe(context)
+        flux = self.subscribe(False, context)
         while True:
             try:
                 value = next(flux)
                 acum = reduce(value, acum)
             except StopIteration:
                 return
             except Exception as ex:
@@ -364,15 +368,15 @@
     def next(self, context):
         value, e, ctx = super(FOnErrorResume, self).next(context)
         if e is None:
             return value, e, ctx
         if isinstance(e, StopIteration):
             return None, e, ctx
         if any([isinstance(e, ex) for ex in self.exceptions]):
-            v, e = fu.try_or(partial(self.on_error_resume), e, ctx)
+            v, e = fu.try_or(partial(self.on_error_resume), e, value, ctx)
             if e is not None:
                 return value, e, ctx
             value = v
         return value, None, ctx
 
 
 class FOnErrorRetry(Stream):
```

### Comparing `python_flux-1.0.6/python_flux/flux_utilis.py` & `python_flux-1.0.7/python_flux/flux_utilis.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,13 +24,13 @@
         raise e
 
     @staticmethod
     def default_finish(context):
         pass
 
     @staticmethod
-    def try_or(statement, value, ctx) -> (object, Exception):
+    def try_or(statement, *args) -> (object, Exception):
         try:
-            v = statement(value, ctx)
+            v = statement(*args)
             return v, None
         except Exception as ex:
             return None, ex
```

### Comparing `python_flux-1.0.6/python_flux/producers.py` & `python_flux-1.0.7/python_flux/producers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.6/python_flux/subscribers.py` & `python_flux-1.0.7/python_flux/subscribers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 from functools import partial
 
 from jsonmerge import merge
 from python_flux.flux_utilis import FluxUtils as fu
 
 
 class SSubscribe(object):
-    def __init__(self, ctx, f):
+    def __init__(self, skip_error, ctx, f):
         if type(ctx) == dict:
             self.context = ctx
         else:
             self.context = ctx()
         self.flux = f
+        self.skip_error = skip_error
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        self.flux.prepare_next()
-        value, e, ctx = self.flux.next(self.context)
-        if e is not None:
-            raise e
-        self.context = merge(self.context, ctx)
-        return value
+        while True:
+            self.flux.prepare_next()
+            value, e, ctx = self.flux.next(self.context)
+            if isinstance(e, StopIteration):
+                raise e
+            if e is not None and self.skip_error:
+                self.context = merge(self.context, ctx)
+                continue
+            if e is not None:
+                raise e
+            self.context = merge(self.context, ctx)
+            return value
 
 
 class SForeach(object):
     def __init__(self, on_success, on_error, on_finish, ctx, f):
         self.on_success = on_success
         self.on_error = on_error
         self.on_finish = on_finish
```

### Comparing `python_flux-1.0.6/PKG-INFO` & `python_flux-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.0.6
+Version: 1.0.7
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
 Permite modificar el valor de un flujo.
 
 Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo y se substituirá en el mismo por lo obtenido de la función.
 
 -  **map_function**: función(valor, contexto) desde donde se obtendrá el valor a sustituir.
 
 
-map_context(map_context_function):
-----------------------------------
+map_context(map_context_function)
+---------------------------------
 
 Permite modificar el contexto de un flujo.
 
 Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo y retornará un nuevo contexto que sustituirá al actual
 
 -  **map_context_function**: función(valor, contexto) desde donde se obtendrá el contexto a subsituir.
 
@@ -103,22 +103,24 @@
 Corta la ejecución del flujo luego de n segundos de procesamiento.
 
 La ejecución se cortará si al momento de evaluar este paso el tiempo transcurrido fue superior al configurado.
 
 -  **n**: Cantidad de segundos que el stream procesa elementos.
 
 
-log(message=lambda v, c: str(v), level=logging.INFO)
-----------------------------------------------------
+log(build_log_message, build_error_message, level)
+--------------------------------------------------
 
 Recibe una función(valor, contexto) que retorna un mensaje de texto que será logueado con el nivel de log indicado en level.
 
 El logueo se hace de forma asincrónica y no afecta al flujo.
 
--  **message**: Función que dado un valor y contexto retorna un mensaje a loguear.
+-  **build_log_message**: Función que dado un valor y contexto retorna un mensaje a loguear
+
+-  **build_error_message**: Función que dada una excepción y el contexto retorna el mensaje a loguear como ERROR
 
 -  **level**: Nivel de logueo que se usará
 
 
 on_error_resume(resume=fu.default_error_resume, exceptions=[Exception])
 -----------------------------------------------------------------------
 En caso de error, este paso ejecuta la función resume que debe retornar un valor a partir del error recibido por parámetro.
@@ -127,31 +129,32 @@
 
 -  **exceptions**: Lista de excepciones para los que se aplica la función resume.
 
 
 on_error_retry(retries=3, delay_ms=lambda i: 0, exceptions=[Exception])
 -----------------------------------------------------------------------
 
-En caso de error, este paso intenta ejecutar nuevamente el flujo
-**retries** cantidad de veces.
+En caso de error, este paso intenta ejecutar nuevamente el flujo **retries** cantidad de veces.
 
 Esto lo hace sólo para las excepciones indicadas por **exceptions** y los reintentos tienen un delay dado por la función **delay_ms** que recibe el número de reintento que es y espera obtener los ms de delay que se deben aplicar.
 
 -  **retries**: Cantidad de reintentos a aplicar
 
 -  **delay_ms**: función(int) que retorna dado el número de reintento en el que se está cuantos: ms de delay se deben aplicar.
 
 -  **exceptions**: Lista de excepciones para los que se aplica el método resume.
 
 
-subscribe(context={})
----------------------
+subscribe(skip_error, context)
+------------------------------
 
 Crea un objeto iterable a partir del flujo. Si se itera sobre este objeto se obtendrán los valores del flujo.
 
+-  **skip_error**: Ignora errores al obtener los valores desde el flujo
+
 -  **context**: Contexto inicial para el flujo
 
 -  **return**: Objeto iterable
 
 
 foreach(on_success=fu.default_success, on_error=fu.default_error, context={})
 -----------------------------------------------------------------------------
```

