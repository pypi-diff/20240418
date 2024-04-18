# Comparing `tmp/miniagents-0.0.4.tar.gz` & `tmp/miniagents-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniagents-0.0.4.tar", max compression
+gzip compressed data, was "miniagents-0.0.5.tar", max compression
```

## Comparing `miniagents-0.0.4.tar` & `miniagents-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.4/LICENSE
--rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.4/miniagents/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.4/miniagents/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.4/miniagents/ext/llms/__init__.py
--rw-r--r--   0        0        0     3749 2024-04-10 07:17:04.828930 miniagents-0.0.4/miniagents/ext/llms/anthropic.py
--rw-r--r--   0        0        0     5545 2024-04-10 07:17:04.829863 miniagents-0.0.4/miniagents/miniagents.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.4/miniagents/promisegraph/__init__.py
--rw-r--r--   0        0        0      563 2024-04-02 17:38:48.000619 miniagents-0.0.4/miniagents/promisegraph/errors.py
--rw-r--r--   0        0        0     2228 2024-03-27 07:32:21.726518 miniagents-0.0.4/miniagents/promisegraph/node.py
--rw-r--r--   0        0        0    17291 2024-04-10 07:17:04.830362 miniagents-0.0.4/miniagents/promisegraph/promise.py
--rw-r--r--   0        0        0      337 2024-04-10 07:17:04.830846 miniagents-0.0.4/miniagents/promisegraph/sentinels.py
--rw-r--r--   0        0        0     1838 2024-04-10 07:17:04.831287 miniagents-0.0.4/miniagents/promisegraph/sequence.py
--rw-r--r--   0        0        0     1972 2024-04-10 07:17:04.831723 miniagents-0.0.4/miniagents/promisegraph/typing.py
--rw-r--r--   0        0        0      694 2024-04-05 18:27:53.768905 miniagents-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.5/LICENSE
+-rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.5/miniagents/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.5/miniagents/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.5/miniagents/ext/llms/__init__.py
+-rw-r--r--   0        0        0     4364 2024-04-18 21:45:37.115573 miniagents-0.0.5/miniagents/ext/llms/anthropic.py
+-rw-r--r--   0        0        0    19743 2024-04-18 21:45:37.116519 miniagents-0.0.5/miniagents/miniagents.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.5/miniagents/promisegraph/__init__.py
+-rw-r--r--   0        0        0      563 2024-04-02 17:38:48.000619 miniagents-0.0.5/miniagents/promisegraph/errors.py
+-rw-r--r--   0        0        0     3603 2024-04-18 21:45:37.116977 miniagents-0.0.5/miniagents/promisegraph/node.py
+-rw-r--r--   0        0        0    18727 2024-04-18 21:45:37.117862 miniagents-0.0.5/miniagents/promisegraph/promise.py
+-rw-r--r--   0        0        0      453 2024-04-18 21:45:37.118627 miniagents-0.0.5/miniagents/promisegraph/sentinels.py
+-rw-r--r--   0        0        0     1888 2024-04-16 00:22:57.814833 miniagents-0.0.5/miniagents/promisegraph/sequence.py
+-rw-r--r--   0        0        0     2219 2024-04-16 00:22:57.815527 miniagents-0.0.5/miniagents/promisegraph/typing.py
+-rw-r--r--   0        0        0      694 2024-04-10 07:26:59.741695 miniagents-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.5/PKG-INFO
```

### Comparing `miniagents-0.0.4/LICENSE` & `miniagents-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.4/miniagents/ext/llms/anthropic.py` & `miniagents-0.0.5/miniagents/ext/llms/anthropic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,81 @@
 """
 This module integrates Anthropic language models with MiniAgents.
 """
 
 import typing
-from typing import AsyncIterator, Any, Optional, Union
+from functools import partial
+from typing import AsyncIterator, Any, Optional
 
-from miniagents.miniagents import MessagePromise, MessageType, MessageSequence, Message
-from miniagents.promisegraph.promise import PromiseContext
-from miniagents.promisegraph.sentinels import Sentinel, DEFAULT
+from miniagents.miniagents import (
+    MessagePromise,
+    Message,
+    miniagent,
+    MiniAgent,
+    MiniAgents,
+    InteractionContext,
+)
+from miniagents.promisegraph.node import Node
 
 if typing.TYPE_CHECKING:
     import anthropic as anthropic_original
 
 
-def anthropic(
-    messages: MessageType,
-    schedule_immediately: Union[bool, Sentinel] = DEFAULT,
-    stream: Union[bool, Sentinel] = DEFAULT,
+class AnthropicMessage(Message):
+    """
+    A message generated by an Anthropic model.
+    """
+
+    anthropic: Node
+
+
+def create_anthropic_agent(
     async_client: Optional["anthropic_original.AsyncAnthropic"] = None,
-    **kwargs,
-) -> MessagePromise:
+    assistant_reply_metadata: Optional[dict[str, Any]] = None,
+    **mini_agent_kwargs,
+) -> MiniAgent:
     """
-    Run text generation with Anthropic.
+    Create an MiniAgent for Anthropic models (see MiniAgent class definition and docstring for usage details).
     """
     if not async_client:
         # pylint: disable=import-outside-toplevel
         # noinspection PyShadowingNames
         import anthropic as anthropic_original
 
-        # TODO Oleksandr: instantiate the client only once (but still don't import `anthropic` at the module level)
         async_client = anthropic_original.AsyncAnthropic()
 
-    if stream is DEFAULT:
-        stream = PromiseContext().stream_llm_tokens_by_default
+    return miniagent(
+        partial(_anthropic_func, async_client=async_client, global_reply_metadata=assistant_reply_metadata),
+        alias="ANTHROPIC_AGENT",
+        **mini_agent_kwargs,
+    )
+
+
+async def _anthropic_func(
+    ctx: InteractionContext,
+    async_client: "anthropic_original.AsyncAnthropic",
+    global_reply_metadata: Optional[dict[str, Any]],
+    reply_metadata: Optional[dict[str, Any]] = None,
+    stream: Optional[bool] = None,
+    **kwargs,
+) -> None:
+    """
+    Run text generation with Anthropic.
+    """
+    global_reply_metadata = global_reply_metadata or {}
+    reply_metadata = reply_metadata or {}
+    if stream is None:
+        stream = MiniAgents.get_current().stream_llm_tokens_by_default
 
     async def message_token_producer(metadata_so_far: dict[str, Any]) -> AsyncIterator[str]:
-        collected_messages = await MessageSequence.acollect_messages(messages)
+        metadata_so_far.update(global_reply_metadata)
+        metadata_so_far.update(reply_metadata)
+        collected_messages = await ctx.messages.acollect_messages()
         message_dicts = [_message_to_anthropic_dict(msg) for msg in collected_messages]
 
-        metadata_so_far["agent_call"] = {
-            "anthropic": {
-                "message_hash_keys": tuple(msg.hash_key for msg in collected_messages),
-                "stream": stream,
-                **kwargs,
-            },
-        }
-
         if stream:
             # pylint: disable=not-async-context-manager
             async with async_client.messages.stream(messages=message_dicts, **kwargs) as response:
                 async for token in response.text_stream:
                     yield token
                 anthropic_final_message = await response.get_final_message()
             # # TODO Oleksandr: if PromptLayer support is needed, but `text_stream` is still not supported by
@@ -69,24 +95,27 @@
                     f"exactly one TextBlock was expected from Anthropic, "
                     f"but {len(anthropic_final_message.content)} were returned instead"
                 )
             yield anthropic_final_message.content[0].text  # yield the whole text as one "piece"
 
         metadata_so_far["anthropic"] = anthropic_final_message.model_dump(exclude={"content"})
 
-    return MessagePromise(
-        message_token_producer=message_token_producer,
-        schedule_immediately=schedule_immediately,
+    ctx.reply(
+        MessagePromise(
+            schedule_immediately=True,  # TODO Oleksandr: should this be customizable ?
+            message_token_producer=message_token_producer,
+            message_class=AnthropicMessage,
+        )
     )
 
 
 def _message_to_anthropic_dict(message: Message) -> dict[str, Any]:
     # TODO Oleksandr: introduce a lambda function to derive roles from messages ?
     try:
         role = message.role
     except AttributeError:
         role = getattr(message, "anthropic_role", "user")
 
     return {
         "role": role,
-        "content": message.text,
+        "content": str(message),
     }
```

### Comparing `miniagents-0.0.4/miniagents/promisegraph/errors.py` & `miniagents-0.0.5/miniagents/promisegraph/errors.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.4/miniagents/promisegraph/promise.py` & `miniagents-0.0.5/miniagents/promisegraph/promise.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 from contextvars import ContextVar
 from types import TracebackType
 from typing import Generic, AsyncIterator, Union, Optional, Iterable, Awaitable, Any
 
 from miniagents.promisegraph.errors import AppendClosedError, AppendNotOpenError
 from miniagents.promisegraph.sentinels import Sentinel, NO_VALUE, FAILED, END_OF_QUEUE, DEFAULT
 from miniagents.promisegraph.typing import (
+    T,
     PIECE,
     WHOLE,
     StreamedPieceProducer,
     StreamedWholePackager,
     PromiseCollectedEventHandler,
+    PromiseFulfiller,
 )
 
 
 class PromiseContext:
     """
     This is the main class for managing the context of promises. It is a context manager that is used to configure
     default settings for promises and to handle the lifecycle of promises (attach `on_promise_collected` handlers).
@@ -29,52 +31,63 @@
 
     _current: ContextVar[Optional["PromiseContext"]] = ContextVar("PromiseContext._current", default=None)
 
     def __init__(
         self,
         schedule_immediately_by_default: bool = True,
         producer_capture_errors_by_default: bool = False,
-        stream_llm_tokens_by_default: bool = True,
         on_promise_collected: Union[PromiseCollectedEventHandler, Iterable[PromiseCollectedEventHandler]] = (),
     ) -> None:
         self.parent = self._current.get()
-        self.on_promise_collected: list[PromiseCollectedEventHandler] = (
+        self.on_promise_collected_handlers: list[PromiseCollectedEventHandler] = (
             [on_promise_collected] if callable(on_promise_collected) else list(on_promise_collected)
         )
         self.child_tasks: set[Task] = set()
 
         self.schedule_immediately_by_default = schedule_immediately_by_default
         self.producer_capture_errors_by_default = producer_capture_errors_by_default
-        # TODO Oleksandr: move this setting to a child class (MiniAgents ?)
-        self.stream_llm_tokens_by_default = stream_llm_tokens_by_default
 
         self._previous_ctx_token: Optional[contextvars.Token] = None
 
     @classmethod
     def get_current(cls) -> "PromiseContext":
         """
         Get the current context. If no context is currently active, raise an error.
         """
         current = cls._current.get()
         if not current:
             raise RuntimeError(
-                "No PromiseContext is currently active. Did you forget to do `async with PromiseContext():`?"
+                f"No {cls.__name__} is currently active. Did you forget to do `async with {cls.__name__}():`?"
+            )
+        if not isinstance(current, cls):
+            raise TypeError(
+                f"You seem to have done `async with {type(current).__name__}():` (or similar), "
+                f"but `async with {cls.__name__}():` is expected instead."
             )
         return current
 
+    def on_promise_collected(self, handler: PromiseCollectedEventHandler) -> PromiseCollectedEventHandler:
+        """
+        Add a handler to be called after a promise is collected.
+        """
+        self.on_promise_collected_handlers.append(handler)
+        return handler
+
     def schedule_task(self, awaitable: Awaitable) -> Task:
         """
         Schedule a task in the current context. "Scheduling" a task this way instead of just creating it with
         `asyncio.create_task()` allows the context to keep track of the child tasks and to wait for them to finish
         before finalizing the context.
         """
 
         async def awaitable_wrapper() -> Any:
             try:
                 return await awaitable
+                # TODO Oleksandr: memorize exceptions so they can be raised when PromiseContext is finalized ?
+                #  HUGE NO! that would be a memory leak
             finally:
                 self.child_tasks.remove(task)
 
         task = asyncio.create_task(awaitable_wrapper())
         self.child_tasks.add(task)
         return task
 
@@ -91,90 +104,142 @@
         return self
 
     async def afinalize(self) -> None:
         """
         Finalize the context (wait for all the child tasks to finish and reset the context). This method is called
         automatically at the end of the `async with` block.
         """
-        await asyncio.gather(
-            *self.child_tasks,
-            return_exceptions=True,  # this prevents waiting until the first exception and then giving up
-        )
+        while self.child_tasks:
+            await asyncio.gather(
+                *self.child_tasks,
+                return_exceptions=True,  # this prevents waiting until the first exception and then giving up
+            )  # TODO Oleksandr: log exceptions that `gather` may return ?
         self._current.reset(self._previous_ctx_token)
         self._previous_ctx_token = None
 
     async def __aenter__(self) -> "PromiseContext":
         return self.activate()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         await self.afinalize()
 
 
-class StreamedPromise(Generic[PIECE, WHOLE]):
+class Promise(Generic[T]):
+    """
+    TODO Oleksandr
+    """
+
+    def __init__(
+        self,
+        schedule_immediately: Union[bool, Sentinel] = DEFAULT,
+        fulfiller: Optional[PromiseFulfiller[T]] = None,
+        prefill_result: Union[Optional[T], Sentinel] = NO_VALUE,
+    ) -> None:
+        # TODO Oleksandr: raise an error if both prefilled_whole and packager are set (or both are not set)
+        promise_context = PromiseContext.get_current()
+
+        if schedule_immediately is DEFAULT:
+            schedule_immediately = promise_context.schedule_immediately_by_default
+
+        self.__fulfiller = fulfiller
+
+        if prefill_result is NO_VALUE:
+            # NO_VALUE is used because `None` is also a legitimate value
+            self._result: Union[T, Sentinel, BaseException] = NO_VALUE
+        else:
+            self._result = prefill_result
+            self._schedule_collected_event_handlers()
+
+        self._fulfiller_lock = asyncio.Lock()
+
+        if schedule_immediately and prefill_result is NO_VALUE:
+            promise_context.schedule_task(self.acollect())
+
+    async def acollect(self) -> T:
+        """
+        TODO Oleksandr: update this docstring
+        "Accumulates" all the pieces of the stream and returns the "whole" value. Will return the exact
+        same object (the exact same instance) if called multiple times on the same instance of `StreamedPromise`.
+        """
+        # TODO Oleksandr: put a deadlock prevention mechanism in place, i. e. find a way to disallow calling
+        #  `acollect()` from within the `fulfiller` function
+        if self._result is NO_VALUE:
+            async with self._fulfiller_lock:
+                if self._result is NO_VALUE:
+                    try:
+                        self._result = await self.__fulfiller(self)
+                    except BaseException as exc:  # pylint: disable=broad-except
+                        self._result = exc
+
+                    self._schedule_collected_event_handlers()
+
+        if isinstance(self._result, BaseException):
+            raise self._result
+        return self._result
+
+    def _schedule_collected_event_handlers(self):
+        promise_ctx = PromiseContext.get_current()
+        while promise_ctx:
+            for handler in promise_ctx.on_promise_collected_handlers:
+                promise_ctx.schedule_task(handler(self, self._result))
+            promise_ctx = promise_ctx.parent
+
+
+class StreamedPromise(Generic[PIECE, WHOLE], Promise[WHOLE]):
     """
     A StreamedPromise represents a promise of a whole value that can be streamed piece by piece.
 
     The StreamedPromise allows for "replaying" the stream of pieces without involving the producer
     for the pieces that have already been produced. This means that multiple consumers can iterate
     over the stream independently, and each consumer will receive all the pieces from the beginning,
     even if some pieces were produced before the consumer started iterating.
 
     :param producer: A callable that returns an async iterator yielding the pieces of the whole value.
     :param packager: A callable that takes an async iterable of pieces and returns the whole value
                      ("packages" the pieces).
     TODO Oleksandr: explain the `schedule_immediately` parameter
     """
 
-    # pylint: disable=too-many-instance-attributes,too-many-arguments
-
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         schedule_immediately: Union[bool, Sentinel] = DEFAULT,
         producer: Optional[StreamedPieceProducer[PIECE]] = None,
         packager: Optional[StreamedWholePackager[WHOLE]] = None,
-        prefill_pieces: Optional[Iterable[PIECE]] = NO_VALUE,
-        prefill_whole: Optional[WHOLE] = NO_VALUE,
+        prefill_pieces: Union[Optional[Iterable[PIECE]], Sentinel] = NO_VALUE,
+        prefill_whole: Union[Optional[WHOLE], Sentinel] = NO_VALUE,
     ) -> None:
-        # TODO Oleksandr: raise an error if both prefill_pieces/prefilled_whole and producer/packager are set
-        #  (or both are not set)
+        # TODO Oleksandr: raise an error if both prefill_pieces and producer are set (or both are not set)
+        promise_context = PromiseContext.get_current()
+
+        if schedule_immediately is DEFAULT:
+            schedule_immediately = promise_context.schedule_immediately_by_default
+
+        super().__init__(
+            schedule_immediately=schedule_immediately,
+            fulfiller=packager,
+            prefill_result=prefill_whole,
+        )
         self.__producer = producer
-        self.__packager = packager
 
         if prefill_pieces is NO_VALUE:
             self._pieces_so_far: list[Union[PIECE, BaseException]] = []
         else:
             self._pieces_so_far: list[Union[PIECE, BaseException]] = [*prefill_pieces, StopAsyncIteration()]
 
-        if prefill_whole is NO_VALUE:
-            # NO_VALUE is used because `None` is also a legitimate value for the "whole"
-            self._whole: Union[WHOLE, Sentinel, BaseException] = NO_VALUE
-        else:
-            self._whole = prefill_whole
-            self._schedule_collected_event_handlers()
-
         self._all_pieces_consumed = prefill_pieces is not NO_VALUE
         self._producer_lock = asyncio.Lock()
-        self._packager_lock = asyncio.Lock()
-
-        promise_context = PromiseContext.get_current()
-
-        if schedule_immediately is DEFAULT:
-            schedule_immediately = promise_context.schedule_immediately_by_default
 
         if schedule_immediately and prefill_pieces is NO_VALUE:
             # start producing pieces at the earliest task switch (put them in a queue for further consumption)
             self._queue = asyncio.Queue()
             promise_context.schedule_task(self._aproduce_the_stream())
         else:
             # each piece will be produced on demand (when the first consumer iterates over it and not earlier)
             self._queue = None
 
-        if schedule_immediately and prefill_whole is NO_VALUE:
-            promise_context.schedule_task(self.acollect())
-
         self._producer_iterator: Union[Optional[AsyncIterator[PIECE]], Sentinel] = None
 
     def __aiter__(self) -> AsyncIterator[PIECE]:
         """
         This allows to consume the stream piece by piece. Each new iterator returned by `__aiter__` will replay
         the stream from the beginning.
         """
@@ -183,42 +248,14 @@
     def __call__(self, *args, **kwargs) -> AsyncIterator[PIECE]:
         """
         This enables the `StreamedPromise` to be used as a piece producer for another `StreamedPromise`, effectively
         chaining them together.
         """
         return self.__aiter__()
 
-    async def acollect(self) -> WHOLE:
-        """
-        "Accumulates" all the pieces of the stream and returns the "whole" value. Will return the exact
-        same object (the exact same instance) if called multiple times on the same instance of `StreamedPromise`.
-        """
-        # TODO Oleksandr: put a deadlock prevention mechanism in place, i. e. find a way to disallow calling
-        #  `acollect()` from within the `packager` function
-        if self._whole is NO_VALUE:
-            async with self._packager_lock:
-                if self._whole is NO_VALUE:
-                    try:
-                        self._whole = await self.__packager(self)
-                    except BaseException as exc:  # pylint: disable=broad-except
-                        self._whole = exc
-
-                    self._schedule_collected_event_handlers()
-
-        if isinstance(self._whole, BaseException):
-            raise self._whole
-        return self._whole
-
-    def _schedule_collected_event_handlers(self):
-        promise_ctx = PromiseContext.get_current()
-        while promise_ctx:
-            for handler in promise_ctx.on_promise_collected:
-                promise_ctx.schedule_task(handler(self, self._whole))
-            promise_ctx = promise_ctx.parent
-
     async def _aproduce_the_stream(self) -> None:
         while True:
             piece = await self._aproducer_iterator_next()
             self._queue.put_nowait(piece)
             if isinstance(piece, StopAsyncIteration):
                 break
```

### Comparing `miniagents-0.0.4/miniagents/promisegraph/sequence.py` & `miniagents-0.0.5/miniagents/promisegraph/sequence.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 """
 The main class in this module is `FlatSequence`. See its docstring for more information.
 """
 
 from typing import Generic, AsyncIterator, Union
 
-from miniagents.promisegraph.promise import StreamedPromise, AppendProducer
+from miniagents.promisegraph.promise import StreamedPromise
 from miniagents.promisegraph.sentinels import Sentinel, DEFAULT
-from miniagents.promisegraph.typing import SequenceFlattener, IN, OUT
+from miniagents.promisegraph.typing import SequenceFlattener, IN, OUT, StreamedPieceProducer
 
 
 class FlatSequence(Generic[IN, OUT]):
     """
     TODO Oleksandr: produce a docstring for this class after you use it in the MiniAgents framework
     """
 
-    append_producer: AppendProducer[IN]
     sequence_promise: StreamedPromise[OUT, tuple[OUT, ...]]
 
     def __init__(
         self,
+        incoming_producer: StreamedPieceProducer[IN],
         flattener: SequenceFlattener[IN, OUT],
         schedule_immediately: Union[bool, Sentinel] = DEFAULT,
-        producer_capture_errors: Union[bool, Sentinel] = DEFAULT,
         sequence_promise_class: type[StreamedPromise[OUT, tuple[OUT, ...]]] = StreamedPromise[OUT, tuple[OUT, ...]],
     ) -> None:
         self.__flattener = flattener
         self._input_promise = StreamedPromise(
             producer=self._producer,
             packager=lambda _: None,
             schedule_immediately=False,
         )
+        # TODO Oleksandr: should I really pass `self` here ? it is not of type `StreamedPromiseBound`
+        self._incoming_producer_iterator = incoming_producer(self)
 
-        self.append_producer = AppendProducer(capture_errors=producer_capture_errors)
         self.sequence_promise = sequence_promise_class(
             producer=self._input_promise,
             packager=self._packager,
             schedule_immediately=schedule_immediately,
         )
 
     async def _producer(self, _) -> AsyncIterator[OUT]:
-        async for zero_or_more_items in self.append_producer:
+        async for zero_or_more_items in self._incoming_producer_iterator:
             async for item in self.__flattener(self, zero_or_more_items):
                 yield item
 
     async def _packager(self, _) -> tuple[OUT, ...]:
         return tuple([item async for item in self.sequence_promise])  # pylint: disable=consider-using-generator
```

### Comparing `miniagents-0.0.4/miniagents/promisegraph/typing.py` & `miniagents-0.0.5/miniagents/promisegraph/typing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 """
 Types for the PromiseGraph part of the library.
 """
 
 from typing import TypeVar, AsyncIterator, Protocol, Union, Any
 
+T = TypeVar("T")
 PIECE = TypeVar("PIECE")
 WHOLE = TypeVar("WHOLE")
 IN = TypeVar("IN")
 OUT = TypeVar("OUT")
+PromiseBound = TypeVar("PromiseBound", bound="Promise")
 StreamedPromiseBound = TypeVar("StreamedPromiseBound", bound="StreamedPromise")
 FlatSequenceBound = TypeVar("FlatSequenceBound", bound="FlatSequence")
 
 
+class PromiseFulfiller(Protocol[T]):
+    """
+    TODO Oleksandr: docstring
+    """
+
+    async def __call__(self, promise: PromiseBound) -> T: ...
+
+
 class StreamedPieceProducer(Protocol[PIECE]):
     """
     A protocol for piece producers. A piece producer is a function that takes a `StreamedPromise` instance as an
     argument and returns an async iterator of pieces.
     """
 
     def __call__(self, streamed_promise: StreamedPromiseBound) -> AsyncIterator[PIECE]: ...
@@ -28,20 +38,21 @@
     """
 
     async def __call__(self, streamed_promise: StreamedPromiseBound) -> WHOLE: ...
 
 
 class PromiseCollectedEventHandler(Protocol):
     """
+    TODO Oleksandr: update this docstring
     A protocol for StreamedPromise collection event handlers. A promise collection event is a function that is
     scheduled to be called after StreamedPromise.acollect() finishes collecting the promise. "Scheduled" means
     that the function is passed to the event loop for execution without blocking the current coroutine.
     """
 
-    async def __call__(self, streamed_promise: StreamedPromiseBound, whole: Any) -> None: ...
+    async def __call__(self, promise: PromiseBound, result: Any) -> None: ...
 
 
 class SequenceFlattener(Protocol[IN, OUT]):
     """
     A protocol for sequence flatteners. A sequence flattener is a function that takes a single object of type `IN`
     and asynchronously converts it into zero or more objects of type `OUT`. In other words, it "flattens" a single
     `IN` into zero or more instances of `OUT`.
```

### Comparing `miniagents-0.0.4/pyproject.toml` & `miniagents-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 119
 
 [tool.coverage.run]
 branch = true
 
 [tool.poetry]
 name = "miniagents"
-version = "0.0.4"
+version = "0.0.5"
 description = """\
 TODO Oleksandr\
 """
 authors = ["Oleksandr Tereshchenko <toporok@gmail.com>"]
 homepage = "https://github.com/teremterem/MiniAgents"
 readme = "README.md"
 license = "MIT"
```

### Comparing `miniagents-0.0.4/PKG-INFO` & `miniagents-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniagents
-Version: 0.0.4
+Version: 0.0.5
 Summary: TODO Oleksandr
 Home-page: https://github.com/teremterem/MiniAgents
 License: MIT
 Author: Oleksandr Tereshchenko
 Author-email: toporok@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

