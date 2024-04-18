# Comparing `tmp/cloai-0.0.1a9.tar.gz` & `tmp/cloai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloai-0.0.1a9.tar", max compression
+gzip compressed data, was "cloai-0.1.0.tar", max compression
```

## Comparing `cloai-0.0.1a9.tar` & `cloai-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    26526 2023-12-21 17:51:54.141512 cloai-0.0.1a9/LICENSE
--rw-r--r--   0        0        0     1604 2023-12-21 17:51:54.141512 cloai-0.0.1a9/README.md
--rw-r--r--   0        0        0     2591 2023-12-21 17:51:54.141512 cloai-0.0.1a9/pyproject.toml
--rw-r--r--   0        0        0       49 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/__init__.py
--rw-r--r--   0        0        0      395 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/__main__.py
--rw-r--r--   0        0        0       46 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/cli/__init__.py
--rw-r--r--   0        0        0     8751 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/cli/commands.py
--rw-r--r--   0        0        0    11269 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/cli/parser.py
--rw-r--r--   0        0        0       41 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/core/__init__.py
--rw-r--r--   0        0        0     1987 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/core/config.py
--rw-r--r--   0        0        0      790 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/core/exceptions.py
--rw-r--r--   0        0        0     3579 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/core/utils.py
--rw-r--r--   0        0        0     4818 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/openai_api.py
--rw-r--r--   0        0        0     2073 2023-12-21 17:51:54.141512 cloai-0.0.1a9/src/cloai/prompts.yaml
--rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 cloai-0.0.1a9/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-04-18 18:53:28.738753 cloai-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1820 2024-04-18 18:53:28.738753 cloai-0.1.0/README.md
+-rw-r--r--   0        0        0     2728 2024-04-18 18:53:28.738753 cloai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/__init__.py
+-rw-r--r--   0        0        0      396 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/__main__.py
+-rw-r--r--   0        0        0       46 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/cli/__init__.py
+-rw-r--r--   0        0        0     9882 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/cli/commands.py
+-rw-r--r--   0        0        0    13199 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/cli/parser.py
+-rw-r--r--   0        0        0     2119 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/cli/prompts.py
+-rw-r--r--   0        0        0       41 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/core/__init__.py
+-rw-r--r--   0        0        0     3053 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/core/config.py
+-rw-r--r--   0        0        0      791 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/core/exceptions.py
+-rw-r--r--   0        0        0     4602 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/core/utils.py
+-rw-r--r--   0        0        0     7956 2024-04-18 18:53:28.738753 cloai-0.1.0/src/cloai/openai_api.py
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 cloai-0.1.0/PKG-INFO
```

### Comparing `cloai-0.0.1a9/LICENSE` & `cloai-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloai-0.0.1a9/README.md` & `cloai-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-# cloai
+# CLI OpenAI
 
-cloai is a Python command-line interface for interacting with the OpenAI API. It provides a set of commands to interact with various OpenAI services such as Speech-to-Text (STT), Text-to-Speech (TTS), and Image Generation.
+CLI OpenAI (cloai) is a command-line interface for interacting with the OpenAI API. It provides a set of commands to interact with various OpenAI services such as GPT, Speech-to-Text (STT), Text-to-Speech (TTS), and Image Generation.
 
 ## Installation
 
 To install cloai, you can use the following command:
 
 ```sh
-poetry add git+https://github.com/cmi-dair/cloai
+pip install cloai
 ```
 
 ## Usage
 
 Before running cloai, make sure the environment variable `OPENAI_API_KEY` is set to your OpenAI API key.
 
 To use the CLI, run `cloai --help` in your terminal. This will display a list of available commands and their descriptions.
 
 Here is a brief overview of the main commands:
 
+- `cloai gpt --help`: Shows the usages of the GPT command. The GPT command is used to generate text with OpenAI's GPT models. As there are several usage
+  options, the help command is the best way to learn how to use it.
+
+- `cloai dalle <prompt>`: Generates images with OpenAI's DALL-E. The `prompt` argument is the text prompt to generate the image from.
+
 - `cloai stt <filename>`: Transcribes audio files with OpenAI's STT models. The `filename` argument is the file to transcribe. It can be any format that ffmpeg supports. Use the `--clip` option to clip the file if it is too large.
 
 - `cloai tts <text>`: Generates audio files with OpenAI's Text to Speech models. The `text` argument is the text to convert to speech.
 
-- `cloai image <prompt>`: Generates images with OpenAI's DALL-E. The `prompt` argument is the text prompt to generate the image from.
-
 Each command has additional options that can be viewed by running `cloai <command> --help`.
 
 ## Contributing
 
 Contributions are welcome! Please see the [contributing guidelines](CONTRIBUTING.md) for more information.
 
 ## License
 
 cloai is licensed under the terms of the [L-GPLv2.1 license](LICENSE).
 
 ## Support
 
-If you encounter any issues or have any questions, please report them on our [issues page](https://github.com/cmi-dair/cloai/issues).
+If you encounter any issues or have any questions, please report them on our [issues page](https://github.com/childmindresearch/cloai/issues).
```

### Comparing `cloai-0.0.1a9/pyproject.toml` & `cloai-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cloai"
-version = "0.0.1a9"
+version = "0.1.0"
 description = "A CLI for OpenAI's API"
 authors = ["Reinder Vos de Wael <reinder.vosdewael@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "cloai", from = "src"}]
 
 [tool.poetry.dependencies]
-python = ">3.8, <4.0"
+python = ">3.10, <4.0"
 pydantic-settings = "^2.1.0"
 pydantic = "^2.5.2"
 ffmpeg-python = "^0.2.0"
 openai = "^1.6.0"
 requests = "^2.31.0"
-pyyaml = "^6.0.1"
 python-docx = "^1.1.0"
-pypdf = "^3.17.3"
+pypdf = ">=3.17.3,<5.0.0"
+aiohttp = "^3.9.3"
+aiofiles = "^23.2.1"
+instructor = ">=0.5.2,<1.3.0"
+aiocsv = "^1.2.5"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.3"
+pytest = ">=7.4.3,<9.0.0"
 mypy = "^1.8.0"
-pre-commit = {version = "^3.6.0", python = ">=3.9"}
-pytest-cov = "^4.1.0"
-ruff = "^0.1.7"
+pre-commit = "^3.6.0"
+pytest-cov = ">=4.1,<6.0"
+ruff = ">=0.1.7,<0.4.0"
 pytest-mock = "^3.12.0"
 pytest-asyncio = "^0.23.2"
 types-requests = "^2.31.0.10"
 tox = "^4.11.4"
 tox-poetry-installer = "1.0.0b1"
 types-pyyaml = "^6.0.12.12"
 pytest-dotenv = "^0.5.2"
+aioresponses = "^0.7.6"
+types-aiofiles = "^23.2.0.20240106"
 
 [tool.poetry.group.docs.dependencies]
 pdoc = "^14.2.0"
 
 [tool.poetry.scripts]
 cloai = 'cloai.__main__:main'
 
@@ -102,30 +107,30 @@
   "ANN102",  # cls should never be type annotated.
   "B008"  # Allow function call in arguments; this is common in FastAPI.
 ]
 fixable = ["ALL"]
 unfixable = []
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-[tool.ruff.format]
-quote-style = "double"
-indent-style = "space"
-skip-magic-trailing-comma = false
-line-ending = "auto"
-
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/**/*.py" = [
   "S101",  # Allow assets
   "ARG",  # Unused arguments are common in tests (fixtures).
   "FBT",  # Allow positional booleans
   "SLF001",  # Allow private member access.
   "INP001"  # No need for namespace packages in tests.
 ]
 "src/**/models.py" = [
   "A003"  # Allow id as a field name.
 ]
 "src/**/schemas.py" = [
   "A003"  # Allow id as a field name.
 ]
+
+[tool.ruff.format]
+quote-style = "double"
+indent-style = "space"
+skip-magic-trailing-comma = false
+line-ending = "auto"
```

### Comparing `cloai-0.0.1a9/src/cloai/cli/commands.py` & `cloai-0.1.0/src/cloai/cli/commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Contains the core business logic of the OpenAI CLI."""
-from __future__ import annotations
 
 import asyncio
 import logging
 import pathlib
 import tempfile
 from typing import Literal
 
+import aiofiles
 import ffmpeg
-import yaml
 
 from cloai import openai_api
+from cloai.cli import prompts
 from cloai.core import config, exceptions, utils
 
 settings = config.get_settings()
 logger = logging.getLogger(settings.LOGGER_NAME)
-PROMPT_FILE = settings.PROMPT_FILE
 MAX_FILE_SIZE = 24_500_000  # Max size is 25MB, but we leave some room for error.
 
 
 class ChatCompletion:
     """A class for running the Chat Completion model.
 
     Attributes:
@@ -151,71 +150,73 @@
 
         Returns:
             The determined system prompt as a string.
         """
         if system_prompt_file:
             return self._read_file(system_prompt_file)
         if system_preset:
-            with PROMPT_FILE.open() as file:
-                prompts = yaml.safe_load(file)
-                return prompts["system"][system_preset]
+            return getattr(prompts.Prompts, system_preset)
         if system_prompt:
             return system_prompt
         msg = "No system prompt provided."
         raise exceptions.LoggedValueError(msg)
 
 
 async def speech_to_text(
     filename: pathlib.Path,
     model: str,
     *,
     clip: bool = False,
+    language: config.WhisperLanguages = config.WhisperLanguages.ENGLISH,
 ) -> str:
     """Transcribes audio files with OpenAI's TTS models.
 
     Args:
         filename: The file to transcribe. Can be any format that ffmpeg supports.
         model: The transcription model to use.
-        voice: The voice to use.
         clip: Whether to clip the file if it is too large, defaults to False.
+        language: The language used in the audio file.
     """
     logger.debug("Transcribing audio.")
     with tempfile.TemporaryDirectory() as temp_dir:
         temp_file = pathlib.Path(temp_dir) / "temp.mp3"
         ffmpeg.input(filename).output(str(temp_file)).overwrite_output().run()
 
         if clip:
             files = list(utils.clip_audio(temp_file, temp_dir, MAX_FILE_SIZE))
         else:
             files = [temp_file]
 
         stt = openai_api.SpeechToText()
-        transcription_promises = [stt.run(filename, model=model) for filename in files]
+        transcription_promises = [
+            stt.run(filename, model=model, language=language) for filename in files
+        ]
         transcriptions = await asyncio.gather(*transcription_promises)
 
         return " ".join(transcriptions)
 
 
 async def text_to_speech(
     text: str,
     output_file: str,
-    model: str,
+    model: Literal["tts-1", "tts-1-hd"],
     voice: Literal["alloy", "echo", "fable", "onyx", "nova", "shimmer"],
 ) -> None:
     """Converts text to speech with OpenAI's TTS models.
 
     Args:
         text: The text to convert to speech.
         output_file: The name of the output file.
         model: The model to use.
         voice: The voice to use.
     """
     logger.debug("Converting text to speech.")
     tts = openai_api.TextToSpeech()
-    await tts.run(text, output_file, model=model, voice=voice)
+    audio_bytes = await tts.run(text, model=model, voice=voice)
+    await utils.save_file(output_file, audio_bytes)
 
 
 async def image_generation(  # noqa: PLR0913
     prompt: str,
     output_base_name: str,
     model: str,
     size: Literal["256x256", "512x512", "1024x1024", "1792x1024", "1024x1792"] | None,
@@ -250,13 +251,51 @@
             size=size,
             quality=quality,
             n=1,
         )
         for _ in range(n)
     ]
     urls = [url[0] for url in await asyncio.gather(*url_promises)]
-    for index, url in enumerate(urls):
-        if url is None:
-            logger.warning("Image %s failed to generate, skipping.", index)
-            continue
-        file = pathlib.Path(f"{output_base_name}_{index}.png")
-        utils.download_file(file, url)
+    if all(url is None for url in urls):
+        msg = "No images were generated."
+        raise exceptions.OpenAIError(msg)
+    urls_not_none = [url for url in urls if url is not None]
+
+    await asyncio.gather(
+        *[
+            utils.download_file(f"{output_base_name}_{index}.png", url)
+            for index, url in enumerate(urls_not_none)
+        ],
+    )
+
+
+async def get_embedding(
+    text_file: pathlib.Path,
+    output_file: pathlib.Path,
+    model: Literal[
+        "text-embedding-3-small",
+        "text-embedding-3-large",
+    ] = "text-embedding-3-large",
+    *,
+    keep_new_lines: bool = False,
+) -> None:
+    """Get the embedding using OpenAI's Embedding models.
+
+    Args:
+        text_file: the text file to embed.
+        model: the name of the Embedding model to use,
+        defaults to text-embedding-3-large.
+        output_file: the name of the CSV output file.
+        keep_new_lines: Whether to keep or remove line breaks,
+        defaults to False.
+    """
+    async with aiofiles.open(text_file, mode="r") as file:
+        text = await file.read()
+
+    get_embedding = openai_api.Embedding()
+
+    embedding = await get_embedding.run(
+        text=text,
+        model=model,
+        keep_new_lines=keep_new_lines,
+    )
+    await utils.save_csv(output_file, embedding)
```

### Comparing `cloai-0.0.1a9/src/cloai/cli/parser.py` & `cloai-0.1.0/src/cloai/cli/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Command line interface for the OpenAI API."""
-from __future__ import annotations
 
 import argparse
 import pathlib
 import sys
 
 from cloai.cli import commands
 from cloai.core import config, exceptions
 
 logger = config.get_logger()
 
 
 PARSER_DEFAULTS = {
-    "epilog": "Please report issues at https://github.com/cmi-dair/cloai.",
+    "epilog": "Please report issues at https://github.com/childmindresearch/cloai.",
     "formatter_class": argparse.ArgumentDefaultsHelpFormatter,
 }
 
 
 async def parse_args() -> None:
     """Parse command line arguments and execute the corresponding command."""
     parser = create_parser()
@@ -68,14 +67,15 @@
     )
 
     subparsers = parser.add_subparsers(dest="command")
     _add_chat_completion_parser(subparsers)
     _add_stt_parser(subparsers)
     _add_tts_parser(subparsers)
     _add_image_generation_parser(subparsers)
+    _add_embedding_parser(subparsers)
     return parser
 
 
 async def run_command(args: argparse.Namespace) -> str | bytes | None:
     """Executes the specified command based on the provided arguments.
 
     Args:
@@ -116,15 +116,24 @@
         )
         return None
     if args.command == "whisper":
         return await commands.speech_to_text(
             filename=args.filename,
             model=args.model,
             clip=args.clip,
+            language=config.WhisperLanguages[args.language],
         )
+    if args.command == "embedding":
+        await commands.get_embedding(
+            text_file=args.text_file,
+            output_file=args.output_file,
+            model=args.model,
+            keep_new_lines=args.keep_new_lines,
+        )
+        return None
     msg = f"Unknown command {args.command}."
     raise exceptions.InvalidArgumentError(msg)
 
 
 def _add_chat_completion_parser(
     subparsers: argparse._SubParsersAction,
 ) -> None:
@@ -141,15 +150,15 @@
         description="Completes text with OpenAI's GPT models.",
         help="Completes text with OpenAI's GPT models.",
         **PARSER_DEFAULTS,  # type: ignore[arg-type]
     )
 
     user_group = chat_parser.add_argument_group(
         "User Prompts",
-        """The prompts povided by the user. One must be provided and these
+        """The prompts provided by the user. One must be provided and these
         arguments are mutually exclusive.""",
     )
     user_group_exclusive = user_group.add_mutually_exclusive_group(required=True)
     user_group_exclusive.add_argument(
         "-p",
         "--user-prompt",
         help="The user prompt to complete.",
@@ -231,14 +240,21 @@
         "-m",
         "--model",
         help=("The transcription model to use."),
         type=lambda x: x.lower(),
         choices=["whisper-1"],
         default="whisper-1",
     )
+    stt_parser.add_argument(
+        "--language",
+        help="The language of the audio file.",
+        type=lambda x: x.upper(),
+        choices=[language.name for language in config.WhisperLanguages],
+        default="ENGLISH",
+    )
 
 
 def _add_tts_parser(
     subparsers: argparse._SubParsersAction,
 ) -> None:
     """Get the argument parser for the "tts" command.
 
@@ -331,14 +347,57 @@
         "--number",
         help="The number of images to generate.",
         type=_positive_int,
         default=1,
     )
 
 
+def _add_embedding_parser(
+    subparsers: argparse._SubParsersAction,
+) -> None:
+    """Get the argument parser for the "embedding" command.
+
+    Args:
+        subparsers: The subparsers object to add the "embedding" command to.
+
+    Returns:
+        argparse.ArgumentParser: The argument parser for the "embedding" command.
+    """
+    embedding_parser = subparsers.add_parser(
+        "embedding",
+        description="Generates embedding with OpenAI's Text Embedding models.",
+        help="Generates embedding with OpenAI's Text Embedding models.",
+        **PARSER_DEFAULTS,  # type: ignore[arg-type]
+    )
+    embedding_parser.add_argument(
+        "text_file",
+        help="The text file to generate an embedding from.",
+        type=pathlib.Path,
+    )
+    embedding_parser.add_argument(
+        "output_file",
+        help="The name of the CSV output file.",
+        type=pathlib.Path,
+    )
+    embedding_parser.add_argument(
+        "-m",
+        "--model",
+        help=("The model to use."),
+        choices=["text-embedding-3-small", "text-embedding-3-large"],
+        default="text-embedding-3-large",
+    )
+    embedding_parser.add_argument(
+        "--keep-new-lines",
+        dest="keep_new_lines",
+        help=("Keeps line breaks in text if specified."),
+        action=argparse.BooleanOptionalAction,
+        default=False,
+    )
+
+
 def _arg_validation(args: argparse.Namespace) -> argparse.Namespace:
     """Validate the parsed arguments.
 
     Validation across arguments is not possible with the built-in argparse
     validation. This function performs validation across arguments.
 
     Args:
```

### Comparing `cloai-0.0.1a9/src/cloai/core/exceptions.py` & `cloai-0.1.0/src/cloai/core/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom exceptions."""
+
 from cloai.core import config
 
 logger = config.get_logger()
 
 
 class LoggedException(BaseException):
     """Base class for exceptions that log their message."""
```

### Comparing `cloai-0.0.1a9/src/cloai/core/utils.py` & `cloai-0.1.0/src/cloai/core/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """Utility functions for cloai."""
-from __future__ import annotations
 
 import math
 import pathlib
 import uuid
-from typing import TYPE_CHECKING
+from collections.abc import Generator
 
+import aiocsv
+import aiofiles
+import aiohttp
 import docx
 import ffmpeg
 import pypdf
-import requests
 
 from cloai.core import config
 
-if TYPE_CHECKING:
-    from collections.abc import Generator
-
 logger = config.get_logger()
 
 
 def clip_audio(
     filename: str | pathlib.Path,
     out_dir: str | pathlib.Path,
     target_size: int,
 ) -> Generator[pathlib.Path, None, None]:
     """Clips the file to the maximum size.
 
     Args:
+    ----
         filename: The file to clip.
         out_dir: The directory to save the clipped files to.
         target_size: The target size of the clipped files.
+
     """
     logger.warning(
         "File too large. Clipping may lead to inaccurate results around the clips.",
     )
 
     file_size = get_file_size(filename)
     n_files = (file_size // target_size) + 1
@@ -56,61 +56,102 @@
     stream.run()
 
     files = list(pathlib.Path(out_dir).glob(f"*{uuid_id}*.mp3"))
     files.sort()
     yield from files
 
 
-def download_file(filename: str | pathlib.Path, url: str) -> None:
+async def save_file(filename: str | pathlib.Path, content: bytes) -> None:
+    """Saves content to a file asynchronously.
+
+    Args:
+    ----
+        filename: The name of the file to save the content to.
+        content: The content to save to the file.
+
+    """
+    async with aiofiles.open(filename, "wb") as file:
+        await file.write(content)
+
+
+async def save_csv(filename: str | pathlib.Path, content: list[float]) -> None:
+    """Saves content to a csv file asynchronously.
+
+    Args:
+    ----
+        filename: The name of the file to save the content to.
+        content: The content to save to the file.
+
+    """
+    async with aiofiles.open(filename, "w") as file:
+        writer = aiocsv.AsyncWriter(file)
+        await writer.writerow(content)
+
+
+async def download_file(filename: str | pathlib.Path, url: str) -> None:
     """Downloads a file from a URL.
 
     Args:
+    ----
         filename: The name of the file to download.
         url: The URL to download the file from.
-    """
-    response = requests.get(url, timeout=10)
-    response.raise_for_status()
 
-    with pathlib.Path(filename).open("wb") as file:
-        file.write(response.content)
+    """
+    async with aiohttp.ClientSession() as session, session.get(url) as response:
+        response.raise_for_status()
+        async with aiofiles.open(filename, "wb") as file:
+            while True:
+                chunk = await response.content.read(1024)
+                if not chunk:
+                    break
+                await file.write(chunk)
 
 
 def get_audio_duration(filename: str | pathlib.Path) -> float:
     """Gets the duration of the audio file.
 
     Args:
+    ----
         filename: The name of the audio file.
 
     Returns:
+    -------
         float: The duration of the audio file.
+
     """
     probe = ffmpeg.probe(filename)
     return float(probe["format"]["duration"])
 
 
 def get_file_size(filename: str | pathlib.Path) -> int:
     """Gets the size of the file.
 
     Args:
+    ----
         filename: The name of the file.
 
     Returns:
+    -------
         int: The size of the file.
+
     """
     return pathlib.Path(filename).stat().st_size
 
 
 def pdf_to_str(file_path: str | pathlib.Path) -> str:
     """Convert a PDF file to text.
 
     Args:
+    ----
         file_path: The path to the PDF file.
 
     Returns:
+    -------
         str: The extracted text from the PDF file.
+
     """
     with pathlib.Path(file_path).open("rb") as file:
         reader = pypdf.PdfReader(file)
         return " ".join(
             [
                 reader.pages[page_num].extract_text()
                 for page_num in range(len(reader.pages))
@@ -118,27 +159,33 @@
         )
 
 
 def docx_to_str(file_path: str | pathlib.Path) -> str:
     """Convert a docx file to text.
 
     Args:
+    ----
         file_path: The path to the docx file.
 
     Returns:
+    -------
         str: The extracted text from the docx file.
+
     """
     document = docx.Document(file_path)
     return " ".join([paragraph.text for paragraph in document.paragraphs])
 
 
 def txt_to_str(file_path: str | pathlib.Path) -> str:
     """Convert a txt file to text.
 
     Args:
+    ----
         file_path: The path to the txt file.
 
     Returns:
+    -------
         str: The extracted text from the txt file.
+
     """
     with pathlib.Path(file_path).open() as file:
         return file.read()
```

### Comparing `cloai-0.0.1a9/src/cloai/openai_api.py` & `cloai-0.1.0/src/cloai/openai_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,136 +1,200 @@
 """This module contains interactions with OpenAI models."""
-from __future__ import annotations
 
 import abc
 import logging
 import pathlib
-from typing import Any, Literal, TypedDict
+from typing import Any, Literal, TypedDict, TypeVar
 
+import instructor
 import openai
+import pydantic
 
 from cloai.core import config, exceptions
 
 settings = config.get_settings()
 OPENAI_API_KEY = settings.OPENAI_API_KEY
 LOGGER_NAME = settings.LOGGER_NAME
 
 logger = logging.getLogger(LOGGER_NAME)
 
+T = TypeVar("T")
+
 
 class Message(TypedDict):
     """A message object."""
 
     role: Literal["assistant", "system", "user"]
     content: str
 
 
-class OpenAIBaseClass(abc.ABC):
+class OpenAIBaseClass(pydantic.BaseModel, abc.ABC):
     """An abstract base class for OpenAI models.
 
     This class initializes the OpenAI client and requires a run method to be
     implemented.
 
     Attributes:
+        api_key: The OpenAI API key.
         client: The OpenAI client used to interact with the model.
     """
 
-    def __init__(self) -> None:
-        """Initializes a new instance of the OpenAIBaseClass class."""
-        self.client = openai.OpenAI(api_key=OPENAI_API_KEY.get_secret_value())
+    model_config = pydantic.ConfigDict(
+        arbitrary_types_allowed=True,
+    )
+
+    api_key: pydantic.SecretStr | None = OPENAI_API_KEY
+    client: openai.AsyncOpenAI = pydantic.Field(init=False, default=None)
+
+    def model_post_init(self, __context: Any) -> None:  # noqa: ANN401
+        """Initializes a new instance of the OpenAIBaseClass class.
+
+        Args:
+            api_key: The OpenAI API key.
+        """
+        if self.api_key is None:
+            msg = "No OpenAI API key provided."
+            raise exceptions.OpenAIError(msg)
+        self.client = openai.AsyncOpenAI(api_key=self.api_key.get_secret_value())
 
     @abc.abstractmethod
     async def run(self, *_args: Any, **_kwargs: Any) -> Any:  # noqa: ANN401
         """Runs the model."""
         ...
 
 
 class ChatCompletion(OpenAIBaseClass):
     """A class for running the Chat Completion models."""
 
     async def run(
         self,
         user_prompt: str,
         system_prompt: str,
-        model: Literal["gpt-4", "gpt-3.5-turbo", "gpt-4-1106-preview"] = "gpt-4",
+        model: str = "gpt-4",
     ) -> str:
         """Runs the Chat Completion model.
 
         Args:
             user_prompt: The user's prompt.
             system_prompt: The system's prompt.
             model: The name of the Chat Completion model to use.
 
         Returns:
             The model's response.
         """
         system_message = Message(role="system", content=system_prompt)
         user_message = Message(role="user", content=user_prompt)
-        response = self.client.chat.completions.create(
+        response = await self.client.chat.completions.create(
             model=model,
             messages=[system_message, user_message],  # type: ignore[list-item]
         )
         if not response.choices[0].message.content:
             msg = "No response from OpenAI."
             raise exceptions.OpenAIError(msg)
         return response.choices[0].message.content
 
 
+class ChatCompletionInstructor(OpenAIBaseClass):
+    """A class for running the Chat Completion models using the instructor library.
+
+    This class is intended to only be exposed to the user through the Python interface.
+    """
+
+    def __init__(self) -> None:
+        """Patches the OpenAI library to use instructor."""
+        super().__init__()
+        self.client = instructor.patch(self.client)
+
+    async def run(  # noqa: PLR0913
+        self,
+        user_prompt: str,
+        system_prompt: str,
+        response_model: T,
+        model: str = "gpt-4",
+        max_retries: int = 1,
+    ) -> T:
+        """Runs the Chat Completion model.
+
+        Args:
+            user_prompt: The user's prompt.
+            system_prompt: The system's prompt.
+            response_model: The response model to return.
+            model: The name of the Chat Completion model to use.
+            max_retries: The maximum number of retries to attempt.
+
+        Returns:
+            The model's response.
+        """
+        system_message = Message(role="system", content=system_prompt)
+        user_message = Message(role="user", content=user_prompt)
+        return await self.client.chat.completions.create(  # type: ignore[call-overload]
+            model=model,
+            messages=[system_message, user_message],  # type: ignore[list-item]
+            response_model=response_model,
+            max_retries=max_retries,
+        )
+
+
 class TextToSpeech(OpenAIBaseClass):
     """A class for running the Text-To-Speech models."""
 
     async def run(
         self,
         text: str,
-        output_file: pathlib.Path | str,
-        model: str = "tts-1",
+        model: Literal["tts-1", "tts-1-hd"] = "tts-1",
         voice: Literal["alloy", "echo", "fable", "onyx", "nova", "shimmer"] = "onyx",
-    ) -> None:
+    ) -> bytes:
         """Runs the Text-To-Speech model.
 
         Args:
             text: The text to convert to speech.
             output_file: The name of the output file.
             model: The name of the Text-To-Speech model to use.
             voice: The voice to use.
 
         Returns:
             The model's response.
         """
-        response = self.client.audio.speech.create(
+        response = await self.client.audio.speech.create(
             model=model,
             voice=voice,
             input=text,
         )
-        response.stream_to_file(output_file)
+        return response.content
 
 
 class SpeechToText(OpenAIBaseClass):
     """A class for running the Speech-To-Text models."""
 
     async def run(
         self,
         audio_file: pathlib.Path | str,
         model: str = "whisper-1",
+        language: config.WhisperLanguages | str = config.WhisperLanguages.ENGLISH,
     ) -> str:
         """Runs the Speech-To-Text model.
 
         Args:
             audio_file: The audio to convert to text.
             model: The name of the Speech-To-Text model to use.
+            language: The language of the audio. Can be both provided through the
+                config.WhisperLanguages enum, which guarantees support, or as a string.
 
         Returns:
             The model's response.
         """
-        with pathlib.Path(audio_file).open("rb") as audio:
-            return self.client.audio.transcriptions.create(
-                model=model,
-                file=audio,
-                response_format="text",
-            )  # type: ignore[return-value] # response_format overrides output type.
+        if isinstance(language, config.WhisperLanguages):
+            language = language.value
+
+        return await self.client.audio.transcriptions.create(
+            model=model,
+            file=pathlib.Path(audio_file),
+            response_format="text",
+            language=language,
+        )  # type: ignore[return-value] # response_format overrides output type.
 
 
 class ImageGeneration(OpenAIBaseClass):
     """A class for running the Image Generation models."""
 
     async def run(  # noqa: PLR0913
         self,
@@ -149,16 +213,49 @@
             size: The size of the generated image.
             quality: The quality of the generated image.
             n: The number of images to generate.
 
         Returns:
             str: The image urls.
         """
-        response = self.client.images.generate(
+        response = await self.client.images.generate(
             model=model,
             prompt=prompt,
             size=size,
             quality=quality,
             n=n,
         )
 
         return [data.url for data in response.data]
+
+
+class Embedding(OpenAIBaseClass):
+    """A class for running the Embedding models."""
+
+    async def run(
+        self,
+        text: str,
+        model: Literal[
+            "text-embedding-3-small",
+            "text-embedding-3-large",
+        ] = "text-embedding-3-large",
+        *,
+        keep_new_lines: bool = False,
+    ) -> list[float]:
+        """Runs the Embedding model.
+
+        Args:
+            text: the string to embed.
+            model: the name of the Embedding model to use.
+            keep_new_lines: Whether to keep or remove line breaks,
+            defaults to False.
+
+        Returns:
+            The embedding (list of numbers)
+        """
+        if keep_new_lines is False:
+            text = text.replace("\n", " ")
+        response = await self.client.embeddings.create(
+            input=text,
+            model=model,
+        )
+        return response.data[0].embedding
```

### Comparing `cloai-0.0.1a9/src/cloai/prompts.yaml` & `cloai-0.1.0/src/cloai/cli/prompts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,43 @@
-system:
-  summary: >
-    You are SummaryGPT, designed to provide concise and accurate summaries of
-    user-provided texts across various topics. Your primary function is to
-    distill complex or lengthy content into clear, brief overviews, maintaining
-    the essence and style of the original text. You are adept at handling
-    diverse subject matter, ensuring that your summaries are informative,
-    well-written, and reflective of the tone and structure of the source
-    material. Your capability to adapt to different writing styles and contexts
-    makes you a versatile tool for users seeking quick understanding of any
-    text.
-  transcript: >
-    You are TranscriptGPT, specialized in refining and correcting transcripts
-    generated by Whisper speech-to-text models. When users provide you with
-    these initial transcriptions, your primary role is to meticulously review
-    and rectify any inaccuracies, ensuring the final text precisely mirrors the
-    spoken content. Your expertise lies in enhancing the clarity and accuracy of
-    these transcripts, making them true and reliable reflections of the original
-    audio. Your attention to detail and proficiency in understanding various
-    speech nuances make you an essential tool for producing error-free,
-    high-quality written records of spoken words.
-  simplify: >
-    Your task as SimplifyGPT is to transform complex texts into versions that
-    are easier to read and understand. When given a text, you should carefully
-    revise it to lower its reading level while preserving the original meaning
-    and key information. This involves simplifying vocabulary, shortening
-    sentences, and explaining any complex concepts in straightforward language.
-    Your goal is to make the content accessible to a broader audience, including
-    younger readers or those with limited proficiency in the language, without
-    losing the essence of the original text. Your ability to distill intricate
-    ideas into clear, simple language is crucial for enhancing comprehension and
-    accessibility.
+"""File for storing the default prompts."""
+
+import dataclasses
+
+
+@dataclasses.dataclass
+class Prompts:
+    """Stores default prompts."""
+
+    transcript = """
+You are TranscriptGPT, specialized in refining and correcting transcripts
+generated by Whisper speech-to-text models. When users provide you with
+these initial transcriptions, your primary role is to meticulously review
+and rectify any inaccuracies, ensuring the final text precisely mirrors the
+spoken content. Your expertise lies in enhancing the clarity and accuracy of
+these transcripts, making them true and reliable reflections of the original
+audio. Your attention to detail and proficiency in understanding various
+speech nuances make you an essential tool for producing error-free,
+high-quality written records of spoken words.
+"""
+    simplify = """
+Your task as SimplifyGPT is to transform complex texts into versions that
+are easier to read and understand. When given a text, you should carefully
+revise it to lower its reading level while preserving the original meaning
+and key information. This involves simplifying vocabulary, shortening
+sentences, and explaining any complex concepts in straightforward language.
+Your goal is to make the content accessible to a broader audience, including
+younger readers or those with limited proficiency in the language, without
+losing the essence of the original text. Your ability to distill intricate
+ideas into clear, simple language is crucial for enhancing comprehension and
+accessibility.
+"""
+    summary = """
+You are SummaryGPT, designed to provide concise and accurate summaries of
+user-provided texts across various topics. Your primary function is to
+distill complex or lengthy content into clear, brief overviews, maintaining
+the essence and style of the original text. You are adept at handling
+diverse subject matter, ensuring that your summaries are informative,
+well-written, and reflective of the tone and structure of the source
+material. Your capability to adapt to different writing styles and contexts
+makes you a versatile tool for users seeking quick understanding of any
+text.
+"""
```

### Comparing `cloai-0.0.1a9/PKG-INFO` & `cloai-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 Metadata-Version: 2.1
 Name: cloai
-Version: 0.0.1a9
+Version: 0.1.0
 Summary: A CLI for OpenAI's API
 License: LGPL-2.1
 Author: Reinder Vos de Wael
 Author-email: reinder.vosdewael@childmind.org
-Requires-Python: >3.8,<4.0
+Requires-Python: >3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiocsv (>=1.2.5,<2.0.0)
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
+Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
+Requires-Dist: instructor (>=0.5.2,<1.3.0)
 Requires-Dist: openai (>=1.6.0,<2.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
-Requires-Dist: pypdf (>=3.17.3,<4.0.0)
+Requires-Dist: pypdf (>=3.17.3,<5.0.0)
 Requires-Dist: python-docx (>=1.1.0,<2.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-# cloai
+# CLI OpenAI
 
-cloai is a Python command-line interface for interacting with the OpenAI API. It provides a set of commands to interact with various OpenAI services such as Speech-to-Text (STT), Text-to-Speech (TTS), and Image Generation.
+CLI OpenAI (cloai) is a command-line interface for interacting with the OpenAI API. It provides a set of commands to interact with various OpenAI services such as GPT, Speech-to-Text (STT), Text-to-Speech (TTS), and Image Generation.
 
 ## Installation
 
 To install cloai, you can use the following command:
 
 ```sh
-poetry add git+https://github.com/cmi-dair/cloai
+pip install cloai
 ```
 
 ## Usage
 
 Before running cloai, make sure the environment variable `OPENAI_API_KEY` is set to your OpenAI API key.
 
 To use the CLI, run `cloai --help` in your terminal. This will display a list of available commands and their descriptions.
 
 Here is a brief overview of the main commands:
 
+- `cloai gpt --help`: Shows the usages of the GPT command. The GPT command is used to generate text with OpenAI's GPT models. As there are several usage
+  options, the help command is the best way to learn how to use it.
+
+- `cloai dalle <prompt>`: Generates images with OpenAI's DALL-E. The `prompt` argument is the text prompt to generate the image from.
+
 - `cloai stt <filename>`: Transcribes audio files with OpenAI's STT models. The `filename` argument is the file to transcribe. It can be any format that ffmpeg supports. Use the `--clip` option to clip the file if it is too large.
 
 - `cloai tts <text>`: Generates audio files with OpenAI's Text to Speech models. The `text` argument is the text to convert to speech.
 
-- `cloai image <prompt>`: Generates images with OpenAI's DALL-E. The `prompt` argument is the text prompt to generate the image from.
-
 Each command has additional options that can be viewed by running `cloai <command> --help`.
 
 ## Contributing
 
 Contributions are welcome! Please see the [contributing guidelines](CONTRIBUTING.md) for more information.
 
 ## License
 
 cloai is licensed under the terms of the [L-GPLv2.1 license](LICENSE).
 
 ## Support
 
-If you encounter any issues or have any questions, please report them on our [issues page](https://github.com/cmi-dair/cloai/issues).
+If you encounter any issues or have any questions, please report them on our [issues page](https://github.com/childmindresearch/cloai/issues).
```

