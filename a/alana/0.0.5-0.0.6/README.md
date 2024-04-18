# Comparing `tmp/alana-0.0.5.tar.gz` & `tmp/alana-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alana-0.0.5.tar", last modified: Sun Apr 14 23:19:13 2024, max compression
+gzip compressed data, was "alana-0.0.6.tar", last modified: Thu Apr 18 03:37:05 2024, max compression
```

## Comparing `alana-0.0.5.tar` & `alana-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:19:13.013280 alana-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 23:19:09.000000 alana-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-14 23:19:13.013280 alana-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:19:13.013280 alana-0.0.5/alana/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-14 23:19:09.000000 alana-0.0.5/alana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-14 23:19:09.000000 alana-0.0.5/alana/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-14 23:19:09.000000 alana-0.0.5/alana/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)    23390 2024-04-14 23:19:09.000000 alana-0.0.5/alana/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:19:13.013280 alana-0.0.5/alana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-14 23:19:13.000000 alana-0.0.5/alana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-14 23:19:13.000000 alana-0.0.5/alana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:19:13.000000 alana-0.0.5/alana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 23:19:13.000000 alana-0.0.5/alana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 23:19:13.000000 alana-0.0.5/alana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 23:19:13.013280 alana-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-14 23:19:09.000000 alana-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:37:05.047818 alana-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 03:36:58.000000 alana-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-18 03:37:05.047818 alana-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:37:05.047818 alana-0.0.6/alana/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-18 03:36:58.000000 alana-0.0.6/alana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-18 03:36:58.000000 alana-0.0.6/alana/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-18 03:36:58.000000 alana-0.0.6/alana/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-18 03:36:58.000000 alana-0.0.6/alana/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22371 2024-04-18 03:36:58.000000 alana-0.0.6/alana/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 03:37:05.047818 alana-0.0.6/alana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-18 03:37:05.000000 alana-0.0.6/alana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 03:37:05.000000 alana-0.0.6/alana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 03:37:05.000000 alana-0.0.6/alana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 03:37:05.000000 alana-0.0.6/alana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 03:37:05.000000 alana-0.0.6/alana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 03:37:05.047818 alana-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-18 03:36:58.000000 alana-0.0.6/setup.py
```

### Comparing `alana-0.0.5/LICENSE` & `alana-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alana-0.0.5/PKG-INFO` & `alana-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alana
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.
 Home-page: https://github.com/alat-rights/alana-utilities
 Author: Alana
 Author-email: hi@alana.computer
 Keywords: LLM,utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alana-0.0.5/alana/color.py` & `alana-0.0.6/alana/color.py`

 * *Files identical despite different names*

### Comparing `alana-0.0.5/alana/globals.py` & `alana-0.0.6/alana/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'haiku' : 'claude-3-haiku-20240307',
     'claude-3-haiku-0307' : 'claude-3-haiku-20240307',
     'claude-2.1' : 'claude-2.1',
     'claude-2.0' : 'claude-2.0',
     'claude-instant-1.2' : 'claude-instant-1.2'
 }
 
-DEFAULT_MODEL = "opus"
+DEFAULT_MODEL = "claude-3-opus-20240229"
 
 SYSTEM: Dict[Literal["few_shot", "gen_prompt", "pretty_print"], str] = {}
 
 SYSTEM.update({"few_shot" : """You are a prompt engineering assistant tasked with generating few-shot examples given a task.
 
 Your user would like to accomplish a specific task. His/her description of the task will be enclosed in <description/> XML tags.
```

### Comparing `alana-0.0.5/alana/prompt.py` & `alana-0.0.6/alana/prompt.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,44 +24,45 @@
         raise ValueError("No '>' or '<' allowed in get_xml tag name!")
     if content == "":
         red(var="`remove_xml`: Empty string provided as `content`.") # TODO: Improve error logging
     pattern: str = rf"<{tag}>.*?</{tag}>" # NOTE: Removed group matching, so can't use `get_xml_pattern`
     output: str = re.sub(pattern=pattern, repl=repl, string=content, flags=re.DOTALL)
     return output
 
-def respond(user: str, messages: Optional[List[MessageParam]] = None) -> List[MessageParam]:
+def respond(content: str, messages: Optional[List[MessageParam]] = None, role: Literal["user", "assistant"] = "user") -> List[MessageParam]:
     """Append a user message to messages list.
     
     Args:
-        user (str): The newest user message content.
+        content (str): The newest message content.
         messages (Optional[List[MessageParam]]): A list of `anthropic.types.MessageParam` objects. The last MessageParam should be from assistant. If `messages` is None, we will populate it with exactly one MessageParam based on `user`.
+        role (Literal["user", "assistant"]): Corresponding source for the message!
     
     Returns:
         List[MessageParam]
     """
     if messages is None:
         messages = []
     messages.append(MessageParam(
-        role='user',
-        content=user,
+        role=role,
+        content=content,
     ))
     return messages
 
-def gen(user: Optional[str] = None, system: str = "", messages: Optional[List[MessageParam]] = None, append: bool = True, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens = 1024, temperature=0.3, loud=True, **kwargs) -> str:
+def gen(user: Optional[str] = None, system: str = "", messages: Optional[List[MessageParam]] = None, append: bool = True, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens = 1024, temperature=1.0, loud=True, **kwargs: Any) -> str:
     """Generate a response from Claude. Returns the text content (`str`) of Claude's response. If you want the Message object instead, use `gen_msg`.
     
     Args:
         user (Optional[str], optional): The user's message content. Defaults to None.
         system (str, optional): The system message for Claude. Defaults to "".
         messages (Optional[List[MessageParam]], optional): A list of `anthropic.types.MessageParam`. Defaults to None.
         append (bool, optional): Whether to append the generated response (as an `anthropic.types.MessageParam`) to `messages`. Defaults to True.
         model (str, optional): The name of the model to use. Defaults to globals.DEFAULT_MODEL.
         api_key (Optional[str], optional): The API key to use for authentication. Defaults to None (if None, uses os.environ["ANTHROPIC_API_KEY]).
         max_tokens (int, optional): The maximum number of tokens to generate in the response. Defaults to 1024.
-        temperature (float, optional): The temperature value for controlling the randomness of the generated response. Defaults to 0.3.
+        temperature (float, optional): The temperature value for controlling the randomness of the generated response.
         loud (bool, optional): Whether to print verbose output. Defaults to True.
         **kwargs: Additional keyword arguments to pass to the underlying generation function.
 
     Raises:
         ValueError: If no prompt is provided (both `user` and `messages` are None).
         ValueError: If the last message in `messages` is from the user and `user` is also provided.
         ValueError: If Claude does not provide a response.
@@ -84,15 +85,15 @@
     """
     if user is None and messages is None:
         raise ValueError("No prompt provided! `user` and `messages` are both None.")
 
     if messages is None:
         assert user is not None  # To be stricter, type(user) == str
         messages=[
-            MessageParam(role="user", content=user), # type: ignore
+            MessageParam(role="user", content=user),
         ]
     elif user is not None:
         assert messages is not None  # To be stricter, messages is List[MessageParam]
         if len(messages) >= 1 and messages[-1]["role"] == "user":
             raise ValueError("`gen`: Bad request! Roles must be alternating. Last message in `messages` is from user, but `user` provided.")
         messages.append(
             MessageParam(role="user", content=user)  # TODO: Check that non-alternating roles are ok (e.g. user, assistant, assistant)
@@ -101,38 +102,39 @@
     output: Message = gen_msg(system=system, messages=messages, model=model, api_key=api_key, max_tokens=max_tokens, loud=loud, temperature=temperature, **kwargs)
 
     if len(output.content) == 0:
         raise ValueError(f"Claude did not provide a response. Stop reason: {output.stop_reason}. Full API response: {output}")
     
     if append == True:
         if messages[-1]["role"] == "assistant":  # NOTE: Anthropic API does not allow non-alternating roles (raises Err400). Let's enforce this.
+            # NOTE: messages[-1]["content"] is assistant output, so should be `str`, since Anthropic API (as of Apr 16 2024) only supports text output!
             existing_assistant_content: str = messages[-1]["content"] # type: ignore
             assistant_content: str = existing_assistant_content + output.content[0].text
             messages.pop()
         else:
             assistant_content: str = output.content[0].text
         
         messages.append(
             MessageParam(
                 role="assistant",
                 content=assistant_content
             )
         )
     return output.content[0].text
 
-def gen_msg(messages: List[MessageParam], system: str = "", model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens = 1024, temperature=0.3, loud=True, **kwargs) -> Message:
+def gen_msg(messages: List[MessageParam], system: str = "", model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens = 1024, temperature=1.0, loud=True, **kwargs: Any) -> Message:
     """Generate a response from Claude using the Anthropic API.
 
     Args:
         messages (List[MessageParam]): A list of `anthropic.types.MessageParam`s representing the conversation history.
         system (str, optional): The system message to set the context for Claude. Defaults to "".
         model (str, optional): The name of the model to use. Defaults to globals.DEFAULT_MODEL.
         api_key (Optional[str], optional): The API key to use for authentication. Defaults to None.
         max_tokens (int, optional): The maximum number of tokens to generate in the response. Defaults to 1024.
-        temperature (float, optional): The temperature value for controlling the randomness of the generated response. Defaults to 0.3.
+        temperature (float, optional): The temperature value for controlling the randomness of the generated response.
         loud (bool, optional): Whether to print verbose output. Defaults to True.
         **kwargs: Additional keyword arguments to pass to the Anthropic API.
 
     Returns:
         Message: The Message object produced by the Anthropic API, containing the generated response.
 
     Notes:
@@ -176,24 +178,24 @@
         **kwargs
     )
     if loud:
         yellow(var=message)
 
     return message
 
-def gen_examples_list(instruction: str, n_examples: int = 5, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens: int = 1024, temperature=0.3, **kwargs) -> List[str]:
+def gen_examples_list(instruction: str, n_examples: int = 5, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens: int = 1024, temperature=1.0, **kwargs: Any) -> List[str]:
     """Uses Claude to generate a Python list of few-shot examples for a given natural language instruction.
 
     Args:
         instruction (str): The natural language instruction for which to generate examples.
         n_examples (int, optional): The number of examples to ask Claude to generate. Defaults to 5.
         model (str, optional): The name of the model to use. Defaults to `globals.DEFAULT_MODEL`.
         api_key (Optional[str], optional): The API key to use for authentication. Defaults to None.
         max_tokens (int, optional): The maximum number of tokens to generate in the response. Defaults to 1024.
-        temperature (float, optional): The temperature value for controlling the randomness of the generated response. Defaults to 0.3.
+        temperature (float, optional): The temperature value for controlling the randomness of the generated response.
         **kwargs: Additional keyword arguments to pass to the `gen` function (`gen` passes kwargs to the Anthropic API).
 
     Returns:
         List[str]: A Python list of generated few-shot examples.
 
     Notes:
         - The function constructs a system message using the `globals.SYSTEM["few_shot"]` template and the provided `n_examples`.
@@ -212,29 +214,29 @@
             "In a world where magic was a part of everyday life, a brave knight named Eldric embarked on a quest to retrieve a powerful artifact...",
             "Deep in the enchanted forest, a group of talking animals gathered around a wise old oak tree to discuss a pressing matter..."
         ]
     """
     system: str = globals.SYSTEM["few_shot"].format(n_examples=n_examples)
     user: str = globals.USER["few_shot"].format(instruction=instruction)
     if n_examples < 1:
-        red(var="Too few examples provided! Trying anyway...")
+        red(var="Too few examples requested! Trying anyway...")
 
     model_output: str = gen(user=user, system=system, model=model, api_key=api_key, max_tokens=max_tokens, temperature=temperature, **kwargs)
     return get_xml(tag='example', content=model_output)
 
-def gen_examples(instruction: str, n_examples: int = 5, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens: int = 1024, temperature=0.3, **kwargs) -> str:
+def gen_examples(instruction: str, n_examples: int = 5, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens: int = 1024, temperature=1.0, **kwargs: Any) -> str:
     """Generate a formatted string containing few-shot examples for a given natural language instruction. Uses `gen_examples_list`.
 
     Args:
         instruction (str): The natural language instruction for which to generate examples.
         n_examples (int, optional): The number of examples to generate. Defaults to 5.
         model (str, optional): The name of the model to use. Defaults to globals.DEFAULT_MODEL.
         api_key (Optional[str], optional): The API key to use for authentication. Defaults to None.
         max_tokens (int, optional): The maximum number of tokens to generate in the response. Defaults to 1024.
-        temperature (float, optional): The temperature value for controlling the randomness of the generated response. Defaults to 0.3.
+        temperature (float, optional): The temperature value for controlling the randomness of the generated response.
         **kwargs: Additional keyword arguments to pass to the `gen_examples_list` function (passed to Anthropic API).
 
     Returns:
         str: A formatted string containing the generated few-shot examples, enclosed in XML-like tags.
 
     Notes:
         - The function calls the `gen_examples_list` function to generate a list of few-shot examples based on the provided `instruction`, `n_examples`, `model`, `api_key`, `max_tokens`, `temperature`, and any additional keyword arguments.
@@ -251,23 +253,24 @@
         <example>Deep in the enchanted forest, a group of talking animals gathered around a wise old oak tree to discuss a pressing matter...</example>
         </examples>
     """
     examples: List[str] = gen_examples_list(instruction=instruction, n_examples=n_examples, model=model, api_key=api_key, max_tokens=max_tokens, temperature=temperature, **kwargs)
     formatted_examples: str = "\n<examples>\n<example>" + '</example>\n<example>'.join(examples) + "</example>\n</examples>"
     return formatted_examples
 
-def gen_prompt(instruction: str, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens: int = 1024, temperature=0.3, **kwargs) -> Dict[Literal["system", "user", "full"], Union[str, List]]:
+def gen_prompt(instruction: str, messages: Optional[List[MessageParam]] = None, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens: int = 1024, temperature=1.0, **kwargs: Any) -> Dict[Literal["system", "user", "full"], Union[str, List]]:
     """Meta-prompter! Generate a prompt given an arbitrary instruction.
     
     Args:
         instruction (str): The arbitrary instruction for which to generate a prompt.
+        messages (Optional[List[MessageParam]]): !!!!EXPERIMENTAL!!!! A list wherein to receive a 2-turn prompt generation thread! STRONGLY RECOMMEND TO BE EMPTY.
         model (str, optional): The name of the model to use. Defaults to globals.DEFAULT_MODEL.
         api_key (Optional[str], optional): The API key to use for authentication. Defaults to None.
         max_tokens (int, optional): The maximum number of tokens to generate in the response. Defaults to 1024.
-        temperature (float, optional): The temperature value for controlling the randomness of the generated response. Defaults to 0.3.
+        temperature (float, optional): The temperature value for controlling the randomness of the generated response.
         **kwargs: Additional keyword arguments to pass to the `gen` function.
 
     Returns:
         Dict[Literal["system", "user", "full"], Union[str, List]]: A dictionary containing the generated prompts.
             - "system" (Union[str, List[str]]): The generated system prompt(s).
             - "user" (Union[str, List[str]]): The generated user prompt(s).
             - "full" (str): The full generated output, including both system and user prompts.
@@ -295,24 +298,29 @@
         <user_prompt>
         Write a story about a robot learning to love.
         </user_prompt>
     """
     meta_system_prompt: str = globals.SYSTEM["gen_prompt"]
     meta_prompt: str = globals.USER["gen_prompt"].format(instruction=instruction)
 
-    full_output: str = gen(user=meta_prompt, system=meta_system_prompt, model=model, api_key=api_key, max_tokens=max_tokens, temperature=temperature, **kwargs)
+    if messages is not None:
+        yellow(var="`alana.prompt.gen_prompt`: Please note that `messages` support in `gen_prompt` is experimental!")
+    if messages is not None and len(messages) > 0:
+        red("`alana.prompt.gen_prompt`: Non-empty `messages` received! In `gen_prompt`, it's STRONGLY recommended to pass in an empty list for `messages`.")
+
+    full_output: str = gen(user=meta_prompt, messages=messages, system=meta_system_prompt, model=model, api_key=api_key, max_tokens=max_tokens, temperature=temperature, **kwargs)
     system_prompt: Union[List[str], str] = get_xml(tag="system_prompt", content=full_output)
     if len(system_prompt) >= 1:
         system_prompt = system_prompt[0]
     user_prompt: Union[List[str], str] = get_xml(tag="user_prompt", content=full_output)
     if len(user_prompt) == 1:  # TODO: Find a saner way to handle this. E.g. delegate to a formatter model.
         user_prompt = user_prompt[0]
     return {"system": system_prompt, "user": user_prompt, "full": full_output}
 
-def pretty_print(var: Any, loud: bool = True, model: str = "sonnet") -> str:
+def pretty_print(var: Any, loud: bool = True, model: str = "sonnet", **kwargs) -> str:
     """Pretty-print an arbitrary variable. By default, uses Sonnet (not globals.DEFAULT_MODEL).
 
     Args:
         var (Any): The variable to pretty-print.
         loud (bool, optional): Whether to print the pretty-printed output. Defaults to True.
         model (str, optional): The name of the model to use. Defaults to "sonnet".
 
@@ -345,45 +353,16 @@
             "age": 30,
             "city": "New York"
         }
     """
     system = globals.SYSTEM["pretty_print"]
     user = globals.USER["pretty_print"].format(var=f'{var}')
 
-    string: str = gen(user=user, system=system, model=model)
+    string: str = gen(user=user, system=system, model=model, loud=False, **kwargs) # NOTE: We just don't log pretty print model outputs
     pretty: Union[List[str], str] = get_xml(tag="pretty", content=string)
     if len(pretty) == 0:
         raise ValueError("`pretty_print`: XML parsing error! Number of <pretty/> tags is 0.")
     else:
         pretty = pretty[-1]
     if loud:
         print(pretty)
     return pretty
-
-# Aliases!
-def grab(tag: str, content: str) -> List[str]:
-    """Alias for get_xml"""
-    return get_xml(tag=tag, content=content)
-
-def xml(tag: str, content: str) -> List[str]:
-    """Alias for get_xml"""
-    return get_xml(tag=tag, content=content)
-
-def rm_xml(tag: str, content: str) -> str:
-    """Alias for remove_xml"""
-    return rm_xml(tag=tag, content=content)
-
-def n_shot_list(instruction: str, n_examples: int = 5, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens: int = 1024, temperature=0.3, **kwargs) -> List[str]:
-    """Alias for gen_examples_list"""
-    return gen_examples_list(instruction=instruction, n_examples=n_examples, model=model, api_key=api_key, max_tokens=max_tokens, temperature=temperature, **kwargs)
-
-def n_shot(instruction: str, n_examples: int = 5, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens: int = 1024, temperature=0.3, **kwargs) -> str:
-    """Alias for gen_examples"""
-    return gen_examples(instruction=instruction, n_examples=n_examples, model=model, api_key=api_key, max_tokens=max_tokens, temperature=temperature, **kwargs)
-
-def few_shot_list(instruction: str, n_examples: int = 5, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens: int = 1024, temperature=0.3, **kwargs) -> List[str]:
-    """Alias for gen_examples_list"""
-    return gen_examples_list(instruction=instruction, n_examples=n_examples, model=model, api_key=api_key, max_tokens=max_tokens, temperature=temperature, **kwargs)
-
-def few_shot(instruction: str, n_examples: int = 5, model: str = globals.DEFAULT_MODEL, api_key: Optional[str] = None, max_tokens: int = 1024, temperature=0.3, **kwargs) -> str:
-    """Alias for gen_examples"""
-    return gen_examples(instruction=instruction, n_examples=n_examples, model=model, api_key=api_key, max_tokens=max_tokens, temperature=temperature, **kwargs)
```

### Comparing `alana-0.0.5/alana.egg-info/PKG-INFO` & `alana-0.0.6/alana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alana
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.
 Home-page: https://github.com/alat-rights/alana-utilities
 Author: Alana
 Author-email: hi@alana.computer
 Keywords: LLM,utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alana-0.0.5/setup.py` & `alana-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
    name='alana',
-   version='0.0.5',  # Update the version number as needed
+   version='0.0.6',  # Update the version number as needed
    author='Alana',
    author_email='hi@alana.computer',
    description='Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.',
    long_description="""
 🎵 Note: I have been making new releases frequently. Make sure your package is up-to-date!
 
 ⚠️ Warning: This library is in active early development! No guarantees are made for backward compatibility. The library is NOT production-ready.
@@ -88,8 +88,8 @@
    ],
    keywords='LLM, utilities',  # Add relevant keywords
    python_requires='>=3.6',
    install_requires=[
       'anthropic',
       'colorama',
    ],
-)
+)
```

