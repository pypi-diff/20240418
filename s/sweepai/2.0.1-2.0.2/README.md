# Comparing `tmp/sweepai-2.0.1.tar.gz` & `tmp/sweepai-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-2.0.1.tar", last modified: Mon Apr 15 19:29:17 2024, max compression
+gzip compressed data, was "sweepai-2.0.2.tar", last modified: Thu Apr 18 19:11:04 2024, max compression
```

## Comparing `sweepai-2.0.1.tar` & `sweepai-2.0.2.tar`

### file list

```diff
@@ -1,128 +1,138 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.151241 sweepai-2.0.1/
--rw-r--r--   0 root         (0) root         (0)     2615 2024-04-10 22:25:21.000000 sweepai-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10746 2024-04-15 19:29:17.151241 sweepai-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6058 2024-04-05 22:26:32.000000 sweepai-2.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)     2041 2024-04-15 19:29:01.000000 sweepai-2.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 19:29:17.151241 sweepai-2.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.135241 sweepai-2.0.1/sweepai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.139241 sweepai-2.0.1/sweepai/agents/
--rw-r--r--   0 root         (0) root         (0)     1185 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/agent_utils.py
--rw-r--r--   0 root         (0) root         (0)     4691 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/assistant_functions.py
--rw-r--r--   0 root         (0) root         (0)     3525 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/agents/assistant_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     4052 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/assistant_wrapper_test.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/complete_code.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/complete_code_test.py
--rw-r--r--   0 root         (0) root         (0)     2448 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/distill_issue.py
--rw-r--r--   0 root         (0) root         (0)    43756 2024-04-15 19:13:53.000000 sweepai-2.0.1/sweepai/agents/modify.py
--rw-r--r--   0 root         (0) root         (0)    23096 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/agents/modify_bot.py
--rw-r--r--   0 root         (0) root         (0)     3515 2024-04-10 19:41:10.000000 sweepai-2.0.1/sweepai/agents/modify_file.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/pr_description_bot.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/agents/prune_modify_snippets.py
--rw-r--r--   0 root         (0) root         (0)    52254 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/api.py
--rw-r--r--   0 root         (0) root         (0)      753 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/api_test.py
--rw-r--r--   0 root         (0) root         (0)    13441 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/cli.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/cli_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.139241 sweepai-2.0.1/sweepai/config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12573 2024-04-09 21:46:59.000000 sweepai-2.0.1/sweepai/config/client.py
--rw-r--r--   0 root         (0) root         (0)     9845 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/config/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.143241 sweepai-2.0.1/sweepai/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19770 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/core/chat.py
--rw-r--r--   0 root         (0) root         (0)    47834 2024-04-14 04:26:32.000000 sweepai-2.0.1/sweepai/core/context_pruning.py
--rw-r--r--   0 root         (0) root         (0)    17807 2024-04-14 22:35:21.000000 sweepai-2.0.1/sweepai/core/entities.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/core/external_searcher.py
--rw-r--r--   0 root         (0) root         (0)    10786 2024-04-04 06:39:36.000000 sweepai-2.0.1/sweepai/core/lexical_search.py
--rw-r--r--   0 root         (0) root         (0)     5826 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/core/post_merge.py
--rw-r--r--   0 root         (0) root         (0)     4345 2024-04-04 06:39:36.000000 sweepai-2.0.1/sweepai/core/pr_reader.py
--rw-r--r--   0 root         (0) root         (0)    45522 2024-04-15 19:07:15.000000 sweepai-2.0.1/sweepai/core/prompts.py
--rw-r--r--   0 root         (0) root         (0)    33698 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/core/reflection_utils.py
--rw-r--r--   0 root         (0) root         (0)     5413 2024-04-09 21:46:59.000000 sweepai-2.0.1/sweepai/core/repo_parsing_utils.py
--rw-r--r--   0 root         (0) root         (0)    33362 2024-04-14 04:26:32.000000 sweepai-2.0.1/sweepai/core/sweep_bot.py
--rw-r--r--   0 root         (0) root         (0)     5758 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/core/update_prompts.py
--rw-r--r--   0 root         (0) root         (0)    10156 2024-04-07 23:48:23.000000 sweepai-2.0.1/sweepai/core/vector_db.py
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/global_threads.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.143241 sweepai-2.0.1/sweepai/handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15508 2024-04-07 00:49:31.000000 sweepai-2.0.1/sweepai/handlers/create_pr.py
--rw-r--r--   0 root         (0) root         (0)     5670 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/on_button_click.py
--rw-r--r--   0 root         (0) root         (0)     1569 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/on_button_click_test.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-04-09 21:46:59.000000 sweepai-2.0.1/sweepai/handlers/on_check_suite.py
--rw-r--r--   0 root         (0) root         (0)    18999 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/handlers/on_comment.py
--rw-r--r--   0 root         (0) root         (0)     3159 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/handlers/on_jira_ticket.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/on_merge.py
--rw-r--r--   0 root         (0) root         (0)    13160 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/on_merge_conflict.py
--rw-r--r--   0 root         (0) root         (0)      722 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/on_review.py
--rw-r--r--   0 root         (0) root         (0)    79755 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/handlers/on_ticket.py
--rw-r--r--   0 root         (0) root         (0)     5168 2024-04-07 00:49:31.000000 sweepai-2.0.1/sweepai/handlers/pr_utils.py
--rw-r--r--   0 root         (0) root         (0)    10042 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/stack_pr.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/handlers/stack_pr_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.143241 sweepai-2.0.1/sweepai/logn/
--rw-r--r--   0 root         (0) root         (0)       44 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/logn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7204 2024-04-11 00:23:29.000000 sweepai-2.0.1/sweepai/logn/cache.py
--rw-r--r--   0 root         (0) root         (0)    11758 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/logn/logn.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/logn/trace_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.151241 sweepai-2.0.1/sweepai/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3235 2024-04-09 21:46:59.000000 sweepai-2.0.1/sweepai/utils/anthropic_client.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/autoimport.py
--rw-r--r--   0 root         (0) root         (0)     3047 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/buttons.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/buttons_test.py
--rw-r--r--   0 root         (0) root         (0)     7850 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/chat_logger.py
--rw-r--r--   0 root         (0) root         (0)     7882 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/code_tree.py
--rw-r--r--   0 root         (0) root         (0)      716 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/code_tree_test.py
--rw-r--r--   0 root         (0) root         (0)      616 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/comment_utils.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/comment_utils_test.py
--rw-r--r--   0 root         (0) root         (0)     6757 2024-04-05 22:26:32.000000 sweepai-2.0.1/sweepai/utils/convert_openai_anthropic.py
--rw-r--r--   0 root         (0) root         (0)    13400 2024-04-12 22:10:10.000000 sweepai-2.0.1/sweepai/utils/diff.py
--rw-r--r--   0 root         (0) root         (0)     2902 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/diff_test.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)      392 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/docker_utils_test.py
--rw-r--r--   0 root         (0) root         (0)     2637 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/event_logger.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     7115 2024-04-14 03:11:57.000000 sweepai-2.0.1/sweepai/utils/fuzzy_diff.py
--rw-r--r--   0 root         (0) root         (0)     2709 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/fuzzy_diff_test.py
--rw-r--r--   0 root         (0) root         (0)    24360 2024-04-11 19:33:18.000000 sweepai-2.0.1/sweepai/utils/github_utils.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/github_utils_test.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/hash.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/html_extractor.py
--rw-r--r--   0 root         (0) root         (0)     4633 2024-04-15 19:07:17.000000 sweepai-2.0.1/sweepai/utils/modify_utils.py
--rw-r--r--   0 root         (0) root         (0)     5888 2024-04-09 00:20:22.000000 sweepai-2.0.1/sweepai/utils/multi_query.py
--rw-r--r--   0 root         (0) root         (0)    34644 2024-04-12 22:10:10.000000 sweepai-2.0.1/sweepai/utils/openai_listwise_reranker.py
--rw-r--r--   0 root         (0) root         (0)    11201 2024-04-10 19:41:10.000000 sweepai-2.0.1/sweepai/utils/openai_proxy.py
--rw-r--r--   0 root         (0) root         (0)     4220 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/openai_proxy_test.py
--rw-r--r--   0 root         (0) root         (0)     1422 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/patch_utils.py
--rw-r--r--   0 root         (0) root         (0)     9641 2024-03-28 21:42:33.000000 sweepai-2.0.1/sweepai/utils/progress.py
--rw-r--r--   0 root         (0) root         (0)      384 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/progress_test.py
--rw-r--r--   0 root         (0) root         (0)     7557 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/utils/prompt_constructor.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/regex_utils.py
--rw-r--r--   0 root         (0) root         (0)      841 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/safe_pqueue.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/scorer.py
--rw-r--r--   0 root         (0) root         (0)      791 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/scorer_test.py
--rw-r--r--   0 root         (0) root         (0)    13788 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/search_and_replace.py
--rw-r--r--   0 root         (0) root         (0)     2101 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/search_and_replace_test.py
--rw-r--r--   0 root         (0) root         (0)     4991 2024-04-05 22:26:32.000000 sweepai-2.0.1/sweepai/utils/str_utils.py
--rw-r--r--   0 root         (0) root         (0)    15481 2024-04-14 04:26:32.000000 sweepai-2.0.1/sweepai/utils/ticket_utils.py
--rw-r--r--   0 root         (0) root         (0)      606 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/timer.py
--rw-r--r--   0 root         (0) root         (0)     7346 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/tree_utils.py
--rw-r--r--   0 root         (0) root         (0)     2963 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/user_settings.py
--rw-r--r--   0 root         (0) root         (0)    23680 2024-04-15 19:07:15.000000 sweepai-2.0.1/sweepai/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)      586 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/utils/utils_test.py
--rw-r--r--   0 root         (0) root         (0)     3989 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/watch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.151241 sweepai-2.0.1/sweepai/web/
--rw-r--r--   0 root         (0) root         (0)     1864 2024-04-08 20:37:50.000000 sweepai-2.0.1/sweepai/web/event_utils.py
--rw-r--r--   0 root         (0) root         (0)     4588 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/web/events.py
--rw-r--r--   0 root         (0) root         (0)     1945 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/web/health.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-03-26 02:10:48.000000 sweepai-2.0.1/sweepai/web/health_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.151241 sweepai-2.0.1/sweepai.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10746 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3315 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      728 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-15 19:29:17.000000 sweepai-2.0.1/sweepai.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 19:29:17.151241 sweepai-2.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)      573 2024-04-07 00:49:31.000000 sweepai-2.0.1/tests/test_gha_extraction.py
--rw-r--r--   0 root         (0) root         (0)      381 2024-04-08 20:37:50.000000 sweepai-2.0.1/tests/test_jira_ticket.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-03-26 02:10:48.000000 sweepai-2.0.1/tests/test_watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)     2615 2024-04-14 06:06:44.000000 sweepai-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10788 2024-04-18 19:11:04.181913 sweepai-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6058 2024-04-14 06:06:44.000000 sweepai-2.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     2073 2024-04-18 19:10:54.000000 sweepai-2.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 19:11:04.181913 sweepai-2.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.161913 sweepai-2.0.2/sweepai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.165913 sweepai-2.0.2/sweepai/agents/
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/agent_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/assistant_functions.py
+-rw-r--r--   0 root         (0) root         (0)     3525 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/assistant_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/assistant_wrapper_test.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/agents/complete_code.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/agents/complete_code_test.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/distill_issue.py
+-rw-r--r--   0 root         (0) root         (0)    43177 2024-04-18 18:59:36.000000 sweepai-2.0.2/sweepai/agents/modify.py
+-rw-r--r--   0 root         (0) root         (0)    23096 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/modify_bot.py
+-rw-r--r--   0 root         (0) root         (0)     3515 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/modify_file.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/agents/pr_description_bot.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/agents/prune_modify_snippets.py
+-rw-r--r--   0 root         (0) root         (0)    52254 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/api.py
+-rw-r--r--   0 root         (0) root         (0)      753 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/api_test.py
+-rw-r--r--   0 root         (0) root         (0)    13441 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/cli_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.165913 sweepai-2.0.2/sweepai/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12573 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/config/client.py
+-rw-r--r--   0 root         (0) root         (0)     9845 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/config/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.169913 sweepai-2.0.2/sweepai/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19734 2024-04-18 17:51:40.000000 sweepai-2.0.2/sweepai/core/chat.py
+-rw-r--r--   0 root         (0) root         (0)    49580 2024-04-16 16:51:35.000000 sweepai-2.0.2/sweepai/core/context_pruning.py
+-rw-r--r--   0 root         (0) root         (0)    17807 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/entities.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/external_searcher.py
+-rw-r--r--   0 root         (0) root         (0)    10786 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/lexical_search.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/post_merge.py
+-rw-r--r--   0 root         (0) root         (0)     4345 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/pr_reader.py
+-rw-r--r--   0 root         (0) root         (0)    45655 2024-04-18 06:45:17.000000 sweepai-2.0.2/sweepai/core/prompts.py
+-rw-r--r--   0 root         (0) root         (0)    33698 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/reflection_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/repo_parsing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    34537 2024-04-18 06:40:48.000000 sweepai-2.0.2/sweepai/core/sweep_bot.py
+-rw-r--r--   0 root         (0) root         (0)     5758 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/core/update_prompts.py
+-rw-r--r--   0 root         (0) root         (0)    10156 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/core/vector_db.py
+-rw-r--r--   0 root         (0) root         (0)       19 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/global_threads.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.173913 sweepai-2.0.2/sweepai/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15508 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/create_pr.py
+-rw-r--r--   0 root         (0) root         (0)     5670 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/on_button_click.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/on_button_click_test.py
+-rw-r--r--   0 root         (0) root         (0)     5711 2024-04-18 19:10:06.000000 sweepai-2.0.2/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0 root         (0) root         (0)    18999 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/on_comment.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/on_jira_ticket.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/on_merge.py
+-rw-r--r--   0 root         (0) root         (0)    13160 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/on_merge_conflict.py
+-rw-r--r--   0 root         (0) root         (0)      722 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/on_review.py
+-rw-r--r--   0 root         (0) root         (0)    79750 2024-04-18 06:40:48.000000 sweepai-2.0.2/sweepai/handlers/on_ticket.py
+-rw-r--r--   0 root         (0) root         (0)     5168 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/pr_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10042 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/handlers/stack_pr.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/handlers/stack_pr_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.173913 sweepai-2.0.2/sweepai/logn/
+-rw-r--r--   0 root         (0) root         (0)       44 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/logn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2024-04-17 00:16:26.000000 sweepai-2.0.2/sweepai/logn/cache.py
+-rw-r--r--   0 root         (0) root         (0)    11758 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/logn/logn.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/logn/trace_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/sweepai/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3235 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/anthropic_client.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/autoimport.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/buttons.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/buttons_test.py
+-rw-r--r--   0 root         (0) root         (0)     7850 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/chat_logger.py
+-rw-r--r--   0 root         (0) root         (0)     7882 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/code_tree.py
+-rw-r--r--   0 root         (0) root         (0)      716 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/code_tree_test.py
+-rw-r--r--   0 root         (0) root         (0)      616 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/comment_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/comment_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     6761 2024-04-16 22:36:43.000000 sweepai-2.0.2/sweepai/utils/convert_openai_anthropic.py
+-rw-r--r--   0 root         (0) root         (0)    13400 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/diff.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/diff_test.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)      392 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/docker_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/event_logger.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7115 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/fuzzy_diff.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/fuzzy_diff_test.py
+-rw-r--r--   0 root         (0) root         (0)    24360 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/github_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/github_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/hash.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/html_extractor.py
+-rw-r--r--   0 root         (0) root         (0)     4955 2024-04-16 18:54:57.000000 sweepai-2.0.2/sweepai/utils/modify_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5888 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/multi_query.py
+-rw-r--r--   0 root         (0) root         (0)    34644 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/openai_listwise_reranker.py
+-rw-r--r--   0 root         (0) root         (0)    11201 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/openai_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     4220 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/openai_proxy_test.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/patch_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9641 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/progress.py
+-rw-r--r--   0 root         (0) root         (0)      384 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/progress_test.py
+-rw-r--r--   0 root         (0) root         (0)     7557 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/regex_utils.py
+-rw-r--r--   0 root         (0) root         (0)      841 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/safe_pqueue.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/scorer.py
+-rw-r--r--   0 root         (0) root         (0)      791 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/scorer_test.py
+-rw-r--r--   0 root         (0) root         (0)    13788 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/search_and_replace.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/search_and_replace_test.py
+-rw-r--r--   0 root         (0) root         (0)     4991 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/str_utils.py
+-rw-r--r--   0 root         (0) root         (0)    17916 2024-04-17 23:25:00.000000 sweepai-2.0.2/sweepai/utils/ticket_utils.py
+-rw-r--r--   0 root         (0) root         (0)      606 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/timer.py
+-rw-r--r--   0 root         (0) root         (0)     7346 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/tree_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/utils/user_settings.py
+-rw-r--r--   0 root         (0) root         (0)    23680 2024-04-16 16:48:05.000000 sweepai-2.0.2/sweepai/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)      586 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/utils/utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/sweepai/web/
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-14 06:06:44.000000 sweepai-2.0.2/sweepai/web/event_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2024-03-03 05:40:09.000000 sweepai-2.0.2/sweepai/web/events.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/web/health.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-02-26 23:28:50.000000 sweepai-2.0.2/sweepai/web/health_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/sweepai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10788 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3561 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      755 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-04-18 19:11:04.000000 sweepai-2.0.2/sweepai.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)      573 2024-04-14 06:06:44.000000 sweepai-2.0.2/tests/test_gha_extraction.py
+-rw-r--r--   0 root         (0) root         (0)      381 2024-04-14 06:06:44.000000 sweepai-2.0.2/tests/test_jira_ticket.py
+-rw-r--r--   0 root         (0) root         (0)     3487 2024-04-18 19:10:06.000000 sweepai-2.0.2/tests/test_run_gha.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-02-26 23:28:50.000000 sweepai-2.0.2/tests/test_watch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.161913 sweepai-2.0.2/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/vendor/tree-sitter-go/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.161913 sweepai-2.0.2/vendor/tree-sitter-go/bindings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.161913 sweepai-2.0.2/vendor/tree-sitter-go/bindings/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:11:04.181913 sweepai-2.0.2/vendor/tree-sitter-go/bindings/python/tree_sitter_go/
+-rw-r--r--   0 root         (0) root         (0)       85 2024-04-11 22:16:11.000000 sweepai-2.0.2/vendor/tree-sitter-go/bindings/python/tree_sitter_go/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-11 22:16:11.000000 sweepai-2.0.2/vendor/tree-sitter-go/bindings/python/tree_sitter_go/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 22:16:11.000000 sweepai-2.0.2/vendor/tree-sitter-go/bindings/python/tree_sitter_go/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1503 2024-04-11 22:16:11.000000 sweepai-2.0.2/vendor/tree-sitter-go/setup.py
```

### Comparing `sweepai-2.0.1/LICENSE` & `sweepai-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/PKG-INFO` & `sweepai-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 2.0.1
+Version: 2.0.2
 Summary: Sweep fixes GitHub issues
 Author-email: Kevin Lu <kevin@sweep.dev>, William Zeng <william@sweep.dev>, Martin Ye <martin@sweep.dev>
 License: Sweep Enterprise Edition (EE) license (the “EE License”)
         Copyright (c) 2024-present Sweep AI, Inc.
         
         With regard to the Sweep Software:
         
@@ -36,17 +36,18 @@
 Requires-Dist: rich==13.7.1
 Requires-Dist: fastapi==0.110.0
 Requires-Dist: prometheus-fastapi-instrumentator==7.0.0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: openai==1.13.3
 Requires-Dist: backoff==2.2.1
-Requires-Dist: pymongo==4.6.2
+Requires-Dist: pymongo==4.6.3
 Requires-Dist: gitpython==3.1.42
 Requires-Dist: tree-sitter==0.21.0
+Requires-Dist: tree-sitter-python==0.21.0
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: rapidfuzz==3.6.2
 Requires-Dist: importmagic==0.1.7
 Requires-Dist: hatchet-sdk==0.18.0
 Requires-Dist: pyflakes==3.2.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: networkx==3.2.1
```

### Comparing `sweepai-2.0.1/README.md` & `sweepai-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/pyproject.toml` & `sweepai-2.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Community = "https://discord.gg/sweep"
 Documentation = "https://docs.sweep.dev"
 Homepage = "https://sweep.dev"
 "Bug Tracker" = "https://github.com/sweepai/sweep/issues"
 
 [project]
 name = "sweepai"
-version = "2.0.1"
+version = "2.0.2"
 description = "Sweep fixes GitHub issues"
 authors = [
     {name = "Kevin Lu", email = "kevin@sweep.dev"},
     {name = "William Zeng", email = "william@sweep.dev"},
     {name = "Martin Ye", email = "martin@sweep.dev"},
 ]
 readme = "README.md"
@@ -41,17 +41,18 @@
   "rich==13.7.1",
   "fastapi==0.110.0",
   "prometheus-fastapi-instrumentator==7.0.0",
   "pyyaml==6.0.1",
   "python-dotenv==1.0.1",
   "openai==1.13.3",
   "backoff==2.2.1",
-  "pymongo==4.6.2",
+  "pymongo==4.6.3",
   "gitpython==3.1.42",
   "tree-sitter==0.21.0",
+  "tree-sitter-python==0.21.0",
   "tree-sitter-languages==1.10.2",
   "rapidfuzz==3.6.2",
   "importmagic==0.1.7",
   "hatchet-sdk==0.18.0",
   "pyflakes==3.2.0",
   "beautifulsoup4==4.12.3",
   "networkx==3.2.1",
```

### Comparing `sweepai-2.0.1/sweepai/agents/agent_utils.py` & `sweepai-2.0.2/sweepai/agents/agent_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/agents/assistant_functions.py` & `sweepai-2.0.2/sweepai/agents/assistant_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/agents/assistant_wrapper.py` & `sweepai-2.0.2/sweepai/agents/assistant_wrapper.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/agents/assistant_wrapper_test.py` & `sweepai-2.0.2/sweepai/agents/assistant_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/agents/complete_code.py` & `sweepai-2.0.2/sweepai/agents/complete_code.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/agents/complete_code_test.py` & `sweepai-2.0.2/sweepai/agents/complete_code_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/agents/distill_issue.py` & `sweepai-2.0.2/sweepai/agents/distill_issue.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/agents/modify.py` & `sweepai-2.0.2/sweepai/agents/modify.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from rapidfuzz import fuzz, process
 
 from loguru import logger
 from tqdm import tqdm
 from sweepai.core.chat import ChatGPT, parse_function_calls_for_openai
 from sweepai.core.entities import FileChangeRequest, Message
-from sweepai.core.reflection_utils import ModifyEvaluatorAgent
 from sweepai.utils.chat_logger import ChatLogger
 from sweepai.utils.convert_openai_anthropic import AnthropicFunctionCall
 from sweepai.utils.diff import generate_diff
 from sweepai.utils.github_utils import ClonedRepo
 from sweepai.utils.modify_utils import manual_code_check
 from sweepai.utils.utils import get_check_results
 
@@ -131,24 +130,24 @@
 Explain why creating this new file is necessary to complete the task and how it integrates with the existing codebase structure.
 </description>
 </parameter>
 </parameters>
 </tool_description>
 
 <tool_description>
-<tool_name>submit_result</tool_name>
+<tool_name>submit_task</tool_name>
 <description>
-Indicate that the task is complete and all requirements have been met. Provide the final code changes or solution.
+Indicate that the current task is complete.
 </description>
 <parameters>
 <parameter>
 <name>justification</name>
 <type>str</type>
 <description>
-Summarize the code changes made and explain how they fulfill the user's original request. Provide the complete, modified code if applicable.
+Summarize the code changes made and explain how they fulfill the user's original request.
 </description>
 </parameter>
 </parameters>
 </tool_description>"""
 
 instructions = """You are an expert software developer tasked with editing code to fulfill the user's request. Your goal is to make the necessary changes to the codebase while following best practices and respecting existing conventions. 
 
@@ -195,26 +194,31 @@
 <param_name>param_value</param_name>
 </parameters>
 </invoke>
 </function_call>
 
 Here is an example:
 
-<function_call>
-<invoke>
-<tool_name>analyze_problem_and_propose_plan</tool_name>
+<tool_description>
+<tool_name>submit_task</tool_name>
+<description>
+Indicate that the current task is complete.
+</description>
 <parameters>
-<problem_analysis>The problem analysis goes here</problem_analysis>
-<proposed_plan>The proposed plan goes here</proposed_plan>
+<parameter>
+<name>justification</name>
+<type>str</type>
+<description>
+Summarize the code changes made and explain how they fulfill the user's original request.
+</description>
+</parameter>
 </parameters>
-</invoke>
-</function_call>
+</tool_description>
 
-If you are really done, call the submit_result function.
-"""
+If the current task is complete, call the submit_task function."""
 
 NO_TOOL_CALL_PROMPT_OPENAI = """FAILURE
 No function calls were made or your last function call was incorrectly formatted. The correct syntax for function calling is this:
 
 <function_call>
 <tool_name>
 <parameter1>
@@ -241,21 +245,49 @@
 </original_code>
 <new_code>
 new code line here
 </new_code>
 </make_change>
 </function_call>
 
-If you are really done, call the submit_result function.
+If the current task is complete, call the submit_task function.
 """
 
+self_review_prompt = """First, review and critique the change(s) you have made. Perform the following:
+
+1. Analyze code patch and indicate:
+   - Purpose and impact of each change
+   - Check for potential errors: 
+     - Logic errors
+     - Unhandled edge cases
+     - Missing imports
+     - Incomplete changes
+     - Undefined variables/functions
+     - Usage of nullable attributes
+     - Non-functional code
+   - Alignment with plan and requirements
+2. Perform critical contextual analysis:
+   - Break down changes 
+   - Explain reasoning
+   - Identify logic issues, edge cases, plan deviations
+   - Consider all scenarios and pitfalls
+   - Consider backwards compatibility and future-proofing
+   - Suggest fixes for problems
+3. Be extremely critical. Do not overlook ANY issues.
+
+Limit the scope of the critique to the current task, which is:
+
+{current_task}
+
+Determine if the changes are correct and complete. If you are satisfied with the changes, call the submit_task function to move onto the next task. If you would like to continue making changes, call make_changes."""
+
 tool_call_parameters = {
     "make_change": ["justification", "file_name", "original_code", "new_code"],
     "create_file": ["justification", "file_name", "file_path", "contents"],
-    "submit_result": ["justification"],
+    "submit_task": ["justification"],
 }
 
 def english_join(items: list[str]) -> str:
     if len(items) == 0:
         return ""
     if len(items) == 1:
         return items[0]
@@ -356,15 +388,15 @@
     current_fcr_index = 0
     for current_fcr_index, fcr in enumerate(fcrs):
         if not fcr.is_completed:
             break
     combined_request_unformatted = "{relevant_files}# Plan of Code Changes\n\nIn order to solve the user's request you will need to modify or create {files_to_modify_list}.{completed_prompt} Here are the instructions for the edits you need to make:\n\n<files_to_change>\n{files_to_modify}\n</files_to_change>"
     completed_prompt = "" if current_fcr_index == 0 else f" You have already completed {current_fcr_index} of the {len(fcrs)} required changes."
     if modify_files_dict:
-        combined_request_unformatted += "\nThe above files reflect the latest updates you have already made. READ THROUGH THEM CAREFULLY TO FIGURE OUT WHAT YOUR NEXT STEPS ARE. Call the make_change, create_file or submit_result tools."
+        combined_request_unformatted += "\nThe above files reflect the latest updates you have already made. READ THROUGH THEM CAREFULLY TO FIGURE OUT WHAT YOUR NEXT STEPS ARE. Call the make_change, create_file or submit_task tools."
     files_to_modify_string = ""
 
     files_to_modify_messages = {fcr.filename: "" for fcr in fcrs}
     for i, fcr in enumerate(fcrs):
         # first add the instructions to the user message
         if i < current_fcr_index: # already done
             files_to_modify_messages[fcr.filename] += f"\n\nYou have already {fcr.change_type} {fcr.filename}, where the specific instructions were to:\n\n{fcr.instructions}"
@@ -636,25 +668,33 @@
     chat_logger_messages: list[dict[str, str]] | None = None,
     use_openai: bool = False,
 ) :
     # iterate through modify_files_dict and generate diffs
     llm_response = ""
     tool_name = function_call.function_name
     tool_call = function_call.function_parameters
-    if tool_name == "submit_result":
-        changes_made = False
+    if tool_name == "submit_task":
         changes_made = generate_diffs(modify_files_dict)
         if changes_made:
             llm_response = "DONE"
         else:
             llm_state["done_counter"] += 1
             if llm_state["done_counter"] > 3:
                 llm_response = "DONE"
             else:
                 llm_response = "ERROR\n\nNo changes were made. Please continue working on your task."
+
+        for fcr in llm_state["fcrs"]:
+            if not fcr.is_completed:
+                fcr.is_completed = True
+                llm_response = f"SUCCESS\n\nThe current task is complete. Please move on to the next task. {llm_state['current_task']}"
+                break
+
+        if all([fcr.is_completed for fcr in llm_state["fcrs"]]):
+            llm_response = "DONE"
     elif tool_name == "no_tool_call":
         if use_openai:
             llm_response = NO_TOOL_CALL_PROMPT_OPENAI
         else:
             llm_response = NO_TOOL_CALL_PROMPT
     elif tool_name == "make_change":
         error_message = ""
@@ -680,14 +720,17 @@
                 if new_code == original_code:
                     error_message += "The new_code and original_code are the same. Are you CERTAIN this change needs to be made? If you are certain this change needs to be made, MAKE SURE that the new_code and original_code are NOT the same."
                     break
                 if not original_code:
                     error_message = "The original_code is empty. Make sure that the original_code is not empty and that it is a valid section of code that you are trying to replace."
                 # get the latest contents of the file
                 file_contents = get_latest_contents(file_name, cloned_repo, modify_files_dict)
+                # if the file is not in modify_files_dict, add it
+                if file_name not in modify_files_dict:
+                    modify_files_dict[file_name] = {"contents": file_contents, "original_contents": file_contents}
                 warning_message = ""
                 
                 # handle special case where there are \r\n characters in the current chunk as this will cause search and replace to ALWAYS fail
                 if "\r\n" in file_contents:
                     # replace in current chunk
                     file_contents = file_contents.replace("\r\n", "\n")
                 # check to see that the original_code is in the new_code by trying all possible indentations
@@ -755,50 +798,19 @@
             ) + f"{warning_message}\n\nYou can continue to make changes to the file {file_name} and call the make_change tool again, or handle the rest of the plan. REMEMBER to add all necessary imports at the top of the file, if the import is not already there!"
             # set contents
             if file_name not in modify_files_dict:
                 modify_files_dict[file_name] = {
                     "contents": file_contents,
                     "original_contents": file_contents,
                 }
-            next_step, feedback = ModifyEvaluatorAgent().evaluate_patch(
-                problem_statement=llm_state["request"],
-                patch = generate_diff(file_contents, new_file_contents, n=10),
-                changed_files=modify_files_dict,
-                new_file_contents=new_file_contents,
-                current_plan=llm_state["plan"],
-                current_task=llm_state["current_task"],
-                previous_attempt=llm_state["previous_attempt"],
-                file_name=file_name,
-                warning_message=warning_message,
-                chat_logger_messages=chat_logger_messages,
-            )
-
-            if next_step == "COMPLETE":
-                # Sets first fcr that is not completed to completed
-                for fcr in llm_state["fcrs"]:
-                    if not fcr.is_completed:
-                        fcr.is_completed = True
-                        break
-                llm_state["plan"] = render_plan(llm_state["fcrs"])
-                llm_state["current_task"] = render_current_task(llm_state["fcrs"])
-                llm_response = f"{success_message}"
-                modify_files_dict[file_name]["original_contents"] = file_contents if "original_contents" not in modify_files_dict[file_name] else modify_files_dict[file_name]["original_contents"]
-                modify_files_dict[file_name]['contents'] = new_file_contents
-                llm_state["previous_attempt"] = ""
-            elif next_step == "CONTINUE":
-                # guard modify files
-                llm_response = f"SUCCESS\n\nThe changes have been applied. However, we need to fix a few more things before moving to the next task of the plan. Here is the feedback from the user:\n\n```\n{generate_diff(file_contents, new_file_contents)}\n```\n{feedback}"
-                modify_files_dict[file_name]["original_contents"] = file_contents if "original_contents" not in modify_files_dict[file_name] else modify_files_dict[file_name]["original_contents"]
-                modify_files_dict[file_name]['contents'] = new_file_contents
-                previous_attempt = f"<previous_attempt>\nThe contractor previously made this change:\n\n```diff\n{generate_diff(file_contents, new_file_contents)}\n```\n\nAnd you accepted with the following feedback:\n{feedback}\n</previous_attempt>"
-                llm_state["previous_attempt"] = previous_attempt
+            if warning_message:
+                llm_response = f"SUCCESS\n\nThe following changes have been applied:\n\n```diff\n{generate_diff(file_contents, new_file_contents)}\n```\nThe code changes also yield the following warnings:\n```\n{warning_message}\n```\n\n{self_review_prompt.format(current_task=llm_state['current_task'])}"
             else:
-                previous_attempt = f"<previous_attempt>\nThe contractor previously attempted at making this change:\n\n```diff\n{generate_diff(file_contents, new_file_contents)}\n```\n\nAnd you rejected it with the following feedback:\n{feedback}\n</previous_attempt>"
-                llm_state["previous_attempt"] = previous_attempt
-                llm_response = f"Changes Rejected with ERROR:\n\n{feedback}"
+                llm_response = f"SUCCESS\n\nThe following changes have been applied:\n\n```diff\n{generate_diff(file_contents, new_file_contents)}\n```\n{self_review_prompt.format(current_task=llm_state['current_task'])}"
+            modify_files_dict[file_name]['contents'] = new_file_contents
     elif tool_name == "create_file":
         error_message = ""
         success_message = ""
         for key in tool_call_parameters[tool_name]:
             if key not in tool_call:
                 error_message += f"No {key} was provided in the {tool_name} tool call. Call the tool again but this time provide the {key}.\n"
         if not error_message:
```

### Comparing `sweepai-2.0.1/sweepai/agents/modify_bot.py` & `sweepai-2.0.2/sweepai/agents/modify_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/agents/modify_file.py` & `sweepai-2.0.2/sweepai/agents/modify_file.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/agents/pr_description_bot.py` & `sweepai-2.0.2/sweepai/agents/pr_description_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/agents/prune_modify_snippets.py` & `sweepai-2.0.2/sweepai/agents/prune_modify_snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/api.py` & `sweepai-2.0.2/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/api_test.py` & `sweepai-2.0.2/sweepai/api_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/cli.py` & `sweepai-2.0.2/sweepai/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/cli_test.py` & `sweepai-2.0.2/sweepai/cli_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/config/client.py` & `sweepai-2.0.2/sweepai/config/client.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/config/server.py` & `sweepai-2.0.2/sweepai/config/server.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/core/chat.py` & `sweepai-2.0.2/sweepai/core/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,27 +145,27 @@
     "submit_result": ["justification"],
 }
 
 # returns a dictionary of the tool call parameters, assumes correct
 def parse_function_call_parameters(tool_call_contents: str, parameters: list[str]) -> dict[str, Any]:
     tool_args = {}
     for param in parameters:
-        param_regex = rf'<{param}>\s*(?P<{param}>.*?)\s*<\/{param}>'
+        param_regex = rf'<{param}>(?P<{param}>.*?)<\/{param}>'
         match = re.search(param_regex, tool_call_contents, re.DOTALL)
         if match:
             param_contents = match.group(param)
             tool_args[param] = param_contents
     return tool_args
 
 # parse llm response for tool calls in xml format
 def parse_function_calls_for_openai(response_contents: str) -> list[dict[str, str]]:
     tool_calls = []
     # first get all tool calls
     for tool_name in tool_call_parameters.keys():
-        tool_call_regex = rf'<{tool_name}>\s*(?P<function_call>.*?)\s*<\/{tool_name}>'
+        tool_call_regex = rf'<{tool_name}>(?P<function_call>.*?)<\/{tool_name}>'
         tool_call_matches = re.finditer(tool_call_regex, response_contents, re.DOTALL)
         # now we extract its parameters
         for tool_call_match in tool_call_matches:
             tool_call_contents = tool_call_match.group("function_call")
             # get parameters based off of tool name
             parameters = tool_call_parameters[tool_name]
             tool_call = { "tool": tool_name, 
@@ -415,15 +415,15 @@
                     system_message: str = system_message, 
                     model: str = model,
                     use_openai: bool = use_openai,
                 ) -> str: # add system message and model to cache
                     if use_openai:
                         client = OpenAI()
                     else:
-                        if ANTHROPIC_AVAILABLE and "opus" not in model:
+                        if ANTHROPIC_AVAILABLE:
                             if "anthropic" not in model:
                                 model = f"anthropic.{model}-v1:0"
                                 self.model = f"anthropic.{self.model}-v1:0"
                             client = AnthropicBedrock(
                                 aws_access_key=AWS_ACCESS_KEY,
                                 aws_secret_key=AWS_SECRET_KEY,
                                 aws_region=AWS_REGION,
```

### Comparing `sweepai-2.0.1/sweepai/core/context_pruning.py` & `sweepai-2.0.2/sweepai/core/context_pruning.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,15 +374,15 @@
             else:
                 line = line.strip()
                 current_node = line
                 if current_node:
                     G.add_node(current_node)
     return G
 
-@file_cache(ignore_params=["rcm", "G"])
+# @file_cache(ignore_params=["rcm", "G"])
 def graph_retrieval(formatted_query: str, top_k_paths: list[str], rcm: RepoContextManager, G: nx.DiGraph):
     # TODO: tune these params
     top_paths_cutoff = 25
     num_rerank = 30
     selected_paths = rcm.top_snippet_paths[:10]
     top_k_paths = top_k_paths[:top_paths_cutoff]
 
@@ -440,37 +440,36 @@
         return distilled_file_path_list
     except Exception as e:
         logger.error(e)
         return []
 
 # @file_cache(ignore_params=["repo_context_manager", "override_import_graph"]) # can't cache this because rcm is stateful
 def integrate_graph_retrieval(formatted_query: str, repo_context_manager: RepoContextManager, override_import_graph: nx.DiGraph = None):
-    num_graph_retrievals = 25
     repo_context_manager, import_graph = parse_query_for_files(formatted_query, repo_context_manager)
     if override_import_graph:
         import_graph = override_import_graph
-    if import_graph:
-        # Graph retrieval can fail and return [] if the graph is not found or pagerank does not converge
-        # Happens especially when graph has multiple components
-        graph_retrieved_files = graph_retrieval(formatted_query, sorted(repo_context_manager.top_snippet_paths), repo_context_manager, import_graph) # sort input for caching
-        if graph_retrieved_files:
-            sorted_snippets = sorted(
-                repo_context_manager.snippets,
-                key=lambda snippet: repo_context_manager.snippet_scores[snippet.denotation],
-                reverse=True,
-            )
-            snippets = []
-            for file_path in graph_retrieved_files:
-                for snippet in sorted_snippets[50 - num_graph_retrievals:]:
-                    if snippet.file_path == file_path:
-                        snippets.append(snippet)
-                        break
-            graph_retrieved_files = graph_retrieved_files[:num_graph_retrievals]
-            repo_context_manager.read_only_snippets = snippets[:len(graph_retrieved_files)]
-            repo_context_manager.current_top_snippets = repo_context_manager.current_top_snippets[:50 - num_graph_retrievals]
+    # if import_graph:
+    #     # Graph retrieval can fail and return [] if the graph is not found or pagerank does not converge
+    #     # Happens especially when graph has multiple components
+    #     graph_retrieved_files = graph_retrieval(formatted_query, sorted(repo_context_manager.top_snippet_paths), repo_context_manager, import_graph) # sort input for caching
+    #     if graph_retrieved_files:
+    #         sorted_snippets = sorted(
+    #             repo_context_manager.snippets,
+    #             key=lambda snippet: repo_context_manager.snippet_scores[snippet.denotation],
+    #             reverse=True,
+    #         )
+    #         snippets = []
+    #         for file_path in graph_retrieved_files:
+    #             for snippet in sorted_snippets[50 - num_graph_retrievals:]:
+    #                 if snippet.file_path == file_path:
+    #                     snippets.append(snippet)
+    #                     break
+    #         graph_retrieved_files = graph_retrieved_files[:num_graph_retrievals]
+    #         repo_context_manager.read_only_snippets = snippets[:len(graph_retrieved_files)]
+    #         repo_context_manager.current_top_snippets = repo_context_manager.current_top_snippets[:50 - num_graph_retrievals]
     return repo_context_manager, import_graph
 
 # add import trees for any relevant_file_paths (code files that appear in query)
 def build_import_trees(
     rcm: RepoContextManager,
     import_graph: nx.DiGraph,
     override_import_graph: nx.DiGraph = None,
@@ -523,14 +522,64 @@
                 rcm.boost_snippets_to_top(code_snippets)
             except Exception as e:
                 logger.error(
                     f"Tried to add code file found in query but recieved error: {e}, skipping and continuing to next one."
                 )
     return rcm
 
+def generate_import_graph_text(graph):
+  # Create a dictionary to store the import relationships
+  import_dict = {}
+
+  # Iterate over each node (file) in the graph
+  for node in graph.nodes():
+    # Get the files imported by the current file
+    imported_files = list(graph.successors(node))
+
+    # Add the import relationships to the dictionary
+    if imported_files:
+      import_dict[node] = imported_files
+    else:
+      import_dict[node] = []
+
+  # Generate the text-based representation
+  final_text = ""
+  visited_files = set()
+  for file, imported_files in sorted(import_dict.items(), key=lambda x: x[0]):
+    if file not in visited_files:
+      final_text += generate_file_imports(graph, file, visited_files, "")
+      final_text += "\n"
+
+  # Add files that are not importing any other files
+  non_importing_files = [
+      file for file, imported_files in import_dict.items()
+      if not imported_files and file not in visited_files
+  ]
+  if non_importing_files:
+    final_text += "\n".join(non_importing_files)
+
+  return final_text
+
+
+def generate_file_imports(graph,
+                          file,
+                          visited_files,
+                          last_successor,
+                          indent_level=0):
+  # if you just added this file as a successor, you don't need to add it again
+  visited_files.add(file)
+  text = "  " * indent_level + f"{file}\n" if file != last_successor else ""
+
+  for imported_file in graph.successors(file):
+    text += "  " * (indent_level + 1) + f"──> {imported_file}\n"
+    if imported_file not in visited_files:
+      text += generate_file_imports(graph, imported_file, visited_files,
+                                    imported_file, indent_level + 2)
+
+  return text
 
 # fetch all files mentioned in the user query
 def parse_query_for_files(
     query: str, rcm: RepoContextManager
 ) -> tuple[RepoContextManager, nx.DiGraph]:
     # use cloned_repo to attempt to find any files names that appear in the query
     repo_full_name = rcm.cloned_repo.repo_full_name
```

### Comparing `sweepai-2.0.1/sweepai/core/entities.py` & `sweepai-2.0.2/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/core/external_searcher.py` & `sweepai-2.0.2/sweepai/core/external_searcher.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/core/lexical_search.py` & `sweepai-2.0.2/sweepai/core/lexical_search.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/core/post_merge.py` & `sweepai-2.0.2/sweepai/core/post_merge.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/core/pr_reader.py` & `sweepai-2.0.2/sweepai/core/pr_reader.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/core/prompts.py` & `sweepai-2.0.2/sweepai/core/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,176 +175,105 @@
 
 cot_retrieval_prompt = """
 Gather information to solve the problem. Use "finish" when you feel like you have sufficient information.
 """
 
 files_to_change_abstract_prompt = """Write an abstract minimum plan to address this issue in the least amount of change possible. Try to originate the root causes of this issue. Be clear and concise. 1 paragraph."""
 
-files_to_change_system_prompt = """You are a brilliant and meticulous engineer assigned to plan code changes to solve the following Github issue using the snippets provided from the codebase. You have the utmost care for the plan that you write, so you ensure that all the relevant modules in the file are identified. Take into account the current repository's language, frameworks, and dependencies, as well as the existing modules such as helper functions, utility operations and backend services."""
+files_to_change_system_prompt = """You are an AI assistant helping an intern update code to resolve a GitHub issue. The user will provide code snippets, a description of the issue, and relevant parts of the codebase.
 
-files_to_change_system_prompt = """You are a brilliant and meticulous engineer assigned to plan code changes to solve the following Github issue using the snippets provided from the codebase. You have the utmost care for the plan that you write, so you ensure that all the relevant modules in the file are identified. Take into account the current repository's language, frameworks, and dependencies, as well as the existing modules such as helper functions, utility operations and backend services."""
+Your role is to analyze the issue and codebase, then provide a clear, step-by-step plan the intern can follow to make the necessary code changes to resolve the issue. Reference specific files, functions, variables and code snippets in your plan.
 
-files_to_change_system_prompt = """\
-You are a brilliant and meticulous engineer assigned to plan code changes to solve the following Github issue. You have the utmost care for the plan that you write, so you do not make mistakes and every function and class will be fully implemented. Take into account the current repository's language, frameworks, and dependencies."""
+Do not write out the full code changes, but rather give detailed natural language instructions and explanations the intern can follow to update the code themselves. Organize the steps logically and break them into small, manageable tasks.
 
+Prioritize using existing code and functions to make efficient and maintainable changes, while minimizing new code. Ensure your suggestions fully resolve the issue."""
 
-# put more emphasis on modify
-# TODO: lots of improvements and cleanup needed here
-files_to_change_prompt = """# Task: 
-Analyze the provided code snippets, repository, and GitHub issue to understand the requested change. Propose a complete plan for an intern to fully resolve the user's issue, utilizing the relevant code snippets and utility modules provided. Because the intern is unfamiliar with the codebase, provide clear and detailed instructions for updating the code logic.
+files_to_change_prompt = """Your job is to write a high quality, detailed, step-by-step plan for an intern to help resolve a user's GitHub issue.
 
-You are provided with relevent_snippets, which contain code snippets you may need to modify or import and read_only_snippets, which contain code snippets of utility functions, services and type definitions you likely do not need to modify.
+You will analyze the provided code snippets, repository, and GitHub issue to understand the requested change. Create a step-by-step plan for an intern to fully resolve the user's GitHub issue. The plan should utilize the relevant code snippets and utility modules provided. Give detailed instructions for updating the code logic, as the intern is unfamiliar with the codebase.
 
 Guidelines:
-* Always include the full file path (e.g. src/utils/strings/regex_utils.py instead of just strings/regex_utils.py or regex_utils.py) and reference the provided snippets.
-* Provide clear, natural language instructions for updating the code logic and specify necessary imports.
-* Be specific and direct in your instructions, avoiding vague terms like "identify" or "ensure." Instead, use actionable phrases like "add", "locate" or "change."
-* Include relevant type definitions, interfaces, and schemas to provide a clear understanding of the entities and their relationships.
-* Avoid using line numbers; instead, reference the locations of the changes using surrounding code or function headers as context.
-* When modifying code, provide detailed instructions and the actual code changes required. Write all code changes in the diff format. Do not leave comments or placeholders for the user to fill in.
+- Always include the full file path and reference the provided snippets 
+- Provide clear instructions for updating the code, specifying necessary imports
+- Be specific and direct, using phrases like "add", "change", "remove" instead of vague terms
+- Reference relevant type definitions, interfaces, and schemas 
+- Avoid line numbers and instead reference code locations using surrounding code or function names
+- Ensure your plan is complete and covers all necessary changes to fully resolve the issue
+- Suggest high-quality, safe, maintainable, efficient and backwards compatible changes
+- Prioritize using existing code and utility methods to minimize writing new code
+- Break the task into small steps, with each <create> or <modify> section for each logical code block worth of change. Use multiple <modify> blocks for the same file if there are multiple distinct changes to make in that file.
 
 Please use the following XML format for your response:
 
 # Issue Analysis:
 <issue_analysis>
 * Identify the root cause of the issue by referencing specific code entities in the relevant files.
-* Outline a plan that completely resolves the user's request, referencing provided code snippets, entity names, and necessary files/directories.
+* Outline ALL changes that need to occur for the user's request to be resolved, by referencing provided code snippets, entity names, and necessary files/directories.
 
 List ALL files we should modify to resolve the issue:
 - File path 1: Outline of instructions for modifying the file
     - First change to make in the file
     - Second change to make in the file
 - File path 2: Outline of instructions for modifying the file
     - First change to make in the file
     - Second change to make in the file
 [additional files as needed]
 
-List ALL relevant utility modules from the provided set and specify where they can be used, including:
+List ALL relevant read-only utility modules from the provided set and specify where they can be used. These are not files you need to make changes to but files you need to read while making changes in other files, including:
 - Type definitions, interfaces, and schemas
 - Helper functions
 - Frontend components
 - Database services
 - API endpoints
 [additional relevant modules as needed]
 
 * For each <create> or <modify> section in your plan, explain its purpose and how it contributes to resolving the issue.
-* Topologically sort the plan so that changes in low-level modules, such as DB query logic, are made before changes in high-level modules, such as API endpoints.
 [additional analysis as needed]
 </issue_analysis>
 
-# Plan:
-<plan>
-<create file="file_path_1" relevant_files="space-separated list of files containing ALL modules to use when creating file_path_1">
-* Natural language instructions for creating the new file to solve the issue.
-* Reference necessary imports and entity names.
-* Include relevant type definitions, interfaces, and schemas.
-* Provide the actual code to be added, with detailed explanations.
-</create>
-
-[additional creates as needed]
-
-<modify file="file_path_2" relevant_files="space-separated list of files containing ALL modules to use while modifying file_path_2">
-* Detailed natural language instructions for modifying the file to solve the issue.
-* Reference the locations of the changes using surrounding code or function headers, not line numbers.
-* Include relevant type definitions, interfaces, and schemas.
-* Each file should be modified at most once. If multiple changes are needed, separate them into different <modify> blocks.
-</modify>
-
-[additional modifies as needed]
-</plan>
-
-Here's an example of an excellent issue analysis and plan:
+Format:
 <issue_analysis>
-The root cause of the issue is that the searchProducts method in the ProductService class (product_service.py) does not properly handle searching for products by category, price range, and keyword simultaneously. It should return products that match all the provided criteria.
-
-To completely resolve the user's request, we need to:
-
-Modify the searchProducts method in product_service.py to:
-Add optional parameters for category_id, min_price, max_price, and keyword
-Update the database query to filter products based on the provided criteria
-Update the search_products endpoint in app.py to:
-Extract the new search parameters from the request
-Pass the parameters to the searchProducts method
-Update the ProductSchema in schemas/product_schema.py to include the category_id field
-Relevant files to modify:
-
-src/services/product_service.py - Update searchProducts to handle category, price range, and keyword filtering
-src/app.py - Update search_products endpoint to extract new parameters and pass them to searchProducts
-src/schemas/product_schema.py - Add category_id field to ProductSchema
-Relevant utility modules:
-"""
-
-# TODO: Fix relevant files block
-
-files_to_change_prompt = """# Task: 
-Critically analyze the provided code snippets, repository, and GitHub issue to understand the requested change. Propose a complete plan for an intern to fully resolve the user's issue, utilizing the relevant code snippets and utility modules provided. Because the intern is unfamiliar with the codebase, provide clear and detailed instructions for updating the code logic.
-
-You are provided with relevent_snippets, which contain code snippets you may need to modify or import and read_only_snippets, which contain code snippets of utility functions, services and type definitions you likely do not need to modify.
+Identify the root cause of the issue referencing specific code in the relevant files. Outline ALL changes needed to resolve the user's request, referencing provided code snippets, entity names, and necessary files/directories. 
 
-Guidelines:
-* Always include the full file path and reference the provided snippets.
-* Provide clear, natural language instructions for updating the code logic and specify necessary imports.
-* Be specific and direct in your instructions, avoiding vague terms like "identify" or "ensure." Instead, use actionable phrases like "add", "locate" or "change."
-* Include relevant type definitions, interfaces, and schemas in the relevant_files to provide a clear understanding of the entities and their relationships.
-* Avoid using line numbers; instead, reference the locations of the changes using surrounding code or function headers as context.
-* Be certain that your plan is complete and covers all the necessary changes to fully resolve the issue.
-* Suggest high-quality changes that are completely safe, maintainable, efficient and backwards compatible.
-* Divide the task into smaller steps, where each <create> or <modify> section corresponds to one small code block of change. You may have multiple <modify> blocks for the same file.
-
-Please use the following XML format for your response:
-
-# Issue Analysis:
-<issue_analysis>
-* Identify the root cause of the issue by referencing specific code entities in the relevant files.
-* Outline ALL changes that need to occur for the user's request to be resolved, by referencing provided code snippets, entity names, and necessary files/directories.
-
-List ALL files we should modify to resolve the issue:
-- File path 1: Outline of instructions for modifying the file
-    - First change to make in the file
-    - Second change to make in the file
-- File path 2: Outline of instructions for modifying the file
-    - First change to make in the file
-    - Second change to make in the file
-[additional files as needed]
-
-List ALL relevant read-only utility modules from the provided set and specify where they can be used. These are not files you need to make changes to but files you need to read while making changes in other files, including:
-- Type definitions, interfaces, and schemas
-- Helper functions
+List ALL files to modify:
+- File path 1: Outline of changes 
+- File path 2: Outline of changes
+[additional files]
+
+List ALL relevant read-only utility modules to reference:
+- Type definitions, interfaces, schemas
+- Helper functions 
 - Frontend components
-- Database services
+- Database services 
 - API endpoints
-[additional relevant modules as needed]
+[additional modules]
 
-* For each <create> or <modify> section in your plan, explain its purpose and how it contributes to resolving the issue.
-[additional analysis as needed]
+For each <create> or <modify> in the plan, explain its purpose for resolving the issue.
+[additional analysis]
 </issue_analysis>
 
-# Plan:
-<plan>
+<plan>  
 <create file="file_path_1">
-* Natural language instructions for creating the new file to solve the issue.
-* Reference necessary imports and entity names.
-* Include references to relevant type definitions, interfaces, and schemas.
+Instructions for creating the new file. Reference imports and entity names. Include relevant type definitions, interfaces, schemas.
 </create>
+[additional creates]
 
-[additional creates as needed]
+<modify file="file_path_2"> 
+Instructions for modifying one section of the file. Reference change locations using surrounding code or functions, not line numbers. Include relevant type definitions, interfaces, schemas. Describe code changes without writing code.
+</modify>
 
 <modify file="file_path_2">
-* Detailed natural language instructions for modifying the file to solve the issue.
-* Reference the locations of the changes using surrounding code or function headers, not line numbers.
-* Include references to relevant type definitions, interfaces, and schemas.
-* Describe code changes, but do not write the actual code.
-* You may modify the same file multiple times. Each <modify> block should contain a single block of code changes from one small section of the file.
+Instructions for modifying a different section of the same file. Use multiple <modify> blocks for the same file to separate distinct changes.
 </modify>
 
-[additional modifies as needed]
+[additional modifies as needed, for the same file or different files]
 </plan>
 
 <relevant_modules>
-[List of all relevant files to use or read while making changes, such as type definitions, interfaces, and schemas, one per line]
+[List of all relevant files to reference while making changes, one per line] 
 </relevant_modules>
 
 Here's an example of an excellent issue analysis and plan:
 
 <issue_analysis>
 The root cause of the issue is that the `createPost` method in the `PostService` class (post_service.py) does not validate that the user submitting the post has a non-deleted account. It should check the `user.deleted` property and raise an exception if the user's account is deleted.
 
@@ -415,14 +344,101 @@
 </plan>
 
 <relevant_modules>
 src/entities/user.py
 src/entities/post.py
 </relevant_modules>"""
 
+plan_selection_prompt = """Critique the pros and cons of each plan based on the following guidelines, prioritizing thoroughness and correctness over potential performance overhead: 
+- Correctness: The code change should fully address the original issue or requirement without introducing new bugs, security vulnerabilities, or performance problems. Follow defensive programming practices, such as avoiding implicit assumptions, validating inputs, and handling edge cases. Consider the potential impact on all relevant data structures and ensure the solution maintains data integrity and consistency. Thoroughness is a top priority. 
+- Backwards Compatibility: When possible, avoid breaking changes to public APIs, data formats, or behaviors that existing code depends on. 
+- Clarity: The code change should be readable, well-structured, and easy for other developers to understand and maintain. Follow existing conventions and style guides, and include documentation and comments for complex or non-obvious logic. 
+- Simplicity: Strive for a solution that is as simple as possible while still being complete and correct. Favor straightforward and easily understandable code. Performance overhead should not be a factor in evaluating simplicity. 
+- Integration: Assess how well the change fits with the overall architecture and design of the system. Avoid tightly coupling components or introducing new dependencies that could complicate future development or deployment. After evaluating the plans against these criteria, select the one that provides the most thorough and correct solution within the specific context and constraints of the project. Prioritize long-term maintainability and architectural integrity.
+
+Respond using the following XML format:
+
+<final_plan>
+[Insert the final plan here, including any modifications or improvements based on the feedback and dialogue. Explain how the plan aligns with the guidelines and why it was chosen over the alternatives.]
+</final_plan>
+
+Here is an example response format:
+
+<final_plan>
+<modify file="example.py">
+[Example instructions here]
+</modify>
+...
+<modify file="anotherexamplefile.py">
+[More example instructions here]
+</modify>
+[Your explanation of why this plan was chosen and how it aligns with the guidelines and any modications made to this plan]
+</final_plan>"""
+
+context_files_to_change_prompt = """Your job is to write a high quality, detailed, step-by-step plan for an intern to help resolve a user's GitHub issue.
+
+You will analyze the provided code snippets, repository, and GitHub issue to understand the requested change. Create a step-by-step plan for an intern to fully resolve the user's GitHub issue. The plan should utilize the relevant code snippets and utility modules provided. Give detailed instructions for updating the code logic, as the intern is unfamiliar with the codebase.
+
+Guidelines:
+- Always include the full file path and reference the provided snippets 
+- Provide clear instructions for updating the code, specifying necessary imports
+- Be specific and direct, using phrases like "add", "change", "remove" instead of vague terms
+- Reference relevant type definitions, interfaces, and schemas 
+- Avoid line numbers and instead reference code locations using surrounding code or function names
+- Ensure your plan is complete and covers all necessary changes to fully resolve the issue
+- Suggest high-quality, safe, maintainable, efficient and backwards compatible changes
+- Prioritize using existing code and utility methods to minimize writing new code
+- Break the task into small steps, with each <create> or <modify> section for each logical code block worth of change. Use multiple <modify> blocks for the same file if there are multiple distinct changes to make in that file.
+
+Please use the following XML format for your response:
+
+# Issue Analysis:
+<issue_analysis>
+Identify the root cause of the issue referencing specific code in the relevant files. Outline ALL changes needed to resolve the user's request, referencing provided code snippets, entity names, and necessary files/directories. 
+
+List ALL files to modify:
+- File path 1: Outline of changes 
+- File path 2: Outline of changes
+[additional files]
+
+List ALL relevant read-only utility modules to reference:
+- Type definitions, interfaces, schemas
+- Helper functions 
+- Frontend components
+- Database services 
+- API endpoints
+[additional modules]
+
+For each <create> or <modify> in the plan, explain its purpose for resolving the issue.
+[additional analysis]
+</issue_analysis>
+
+<plan number="#">
+<create file="file_path_1">
+Instructions for creating the new file. Reference imports and entity names. Include relevant type definitions, interfaces, schemas.
+</create>
+[additional creates]
+
+<modify file="file_path_2"> 
+Instructions for modifying one section of the file. Reference change locations using surrounding code or functions, not line numbers. Include relevant type definitions, interfaces, schemas. Describe code changes without writing code.
+</modify>
+
+<modify file="file_path_2">
+Instructions for modifying a different section of the same file. Use multiple <modify> blocks for the same file to separate distinct changes.
+</modify>
+
+[additional modifies as needed, for the same file or different files]
+</plan>
+
+<relevant_modules>
+[List of all relevant files to reference while making changes, one per line] 
+</relevant_modules>
+
+Generate three diverse plans to address the user issue based off of your issue analysis. The best plan will be chosen later."""
+
 extract_files_to_change_prompt = """\
 # Task:
 Create a plan that resolves the user's query and ONLY the user's query under "Issue Title" and "Issue Description", providing your response in the below format:
 <contextual_request_analysis>
 Review each function of each relevant_snippet and analyze the user request to determine if this change should use the refactor or unit test tools.
 The refactor tool performs code transformations in a single file without making other logical changes. Determine the function(s) that are too long and should have it's individual parts extracted.
 The unit test tool creates or edits unit tests for a given file. Determine all functions that should be unit tested.
```

### Comparing `sweepai-2.0.1/sweepai/core/reflection_utils.py` & `sweepai-2.0.2/sweepai/core/reflection_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/core/repo_parsing_utils.py` & `sweepai-2.0.2/sweepai/core/repo_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/core/sweep_bot.py` & `sweepai-2.0.2/sweepai/core/sweep_bot.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,34 +4,37 @@
 import traceback
 from typing import Dict, Generator
 
 from github.ContentFile import ContentFile
 from github.GithubException import GithubException, UnknownObjectException
 from github.Repository import Repository
 from loguru import logger
+from networkx import Graph
 from pydantic import BaseModel
 
 from sweepai.agents.modify_file import modify_file
 from sweepai.config.client import SweepConfig, get_blocked_dirs, get_branch_name_config
 from sweepai.config.server import DEFAULT_GPT4_32K_MODEL, DEFAULT_GPT35_MODEL
 from sweepai.core.chat import ChatGPT
+from sweepai.core.context_pruning import generate_import_graph_text
 from sweepai.core.entities import (
     AssistantRaisedException,
     FileChangeRequest,
     MaxTokensExceeded,
     Message,
     NoFilesException,
     ProposedIssue,
     PullRequest,
     RegexMatchError,
     SandboxResponse,
     Snippet,
 )
 from sweepai.core.prompts import (
     files_to_change_prompt,
+    context_files_to_change_prompt,
     pull_request_prompt,
     subissues_prompt,
     files_to_change_system_prompt
 )
 from sweepai.utils.chat_logger import ChatLogger, discord_log_error
 from sweepai.utils.progress import (
     AssistantAPIMessage,
@@ -185,17 +188,19 @@
     raise Exception("Budget number of chars too low!")
 
 def get_files_to_change(
     relevant_snippets: list[Snippet],
     read_only_snippets: list[Snippet],
     problem_statement,
     repo_name,
+    import_graph: Graph | None = None,
     pr_diffs: str = "",
     chat_logger: ChatLogger = None,
-    seed: int = 0
+    seed: int = 0,
+    context: bool = False,
 ) -> tuple[list[FileChangeRequest], str]:
     file_change_requests: list[FileChangeRequest] = []
     messages: list[Message] = []
     messages.append(
         Message(role="system", content=files_to_change_system_prompt, key="system")
     )
     messages.append(
@@ -212,20 +217,22 @@
     interleaved_snippets = []
     for i in range(max(len(relevant_snippets), len(read_only_snippets))):
         if i < len(relevant_snippets):
             interleaved_snippets.append(relevant_snippets[i])
         if i < len(read_only_snippets):
             interleaved_snippets.append(read_only_snippets[i])
 
+    interleaved_snippets = relevant_snippets
+
     max_snippets = get_max_snippets(interleaved_snippets)
     relevant_snippets = [snippet for snippet in max_snippets if any(snippet.file_path == relevant_snippet.file_path for relevant_snippet in relevant_snippets)]
     read_only_snippets = [snippet for snippet in max_snippets if not any(snippet.file_path == relevant_snippet.file_path for relevant_snippet in relevant_snippets)]
 
-    relevant_snippet_template = '<snippet index="{i}">\n<source>\n{snippet_denotation}\n</source>\n<snippet_content>\n{content}\n</snippet_content>\n</snippet>'
-    read_only_snippet_template = '<read_only_snippet index="{i}">\n<source>\n{snippet_denotation}\n</source>\n<snippet_content>\n{content}\n</snippet_content>\n</read_only_snippet>'
+    relevant_snippet_template = '<snippet index="{i}">\n<snippet_path>\n{snippet_denotation}\n</snippet_path>\n<source>\n{content}\n</source>\n</snippet>'
+    read_only_snippet_template = '<read_only_snippet index="{i}">\n<snippet_path>\n{snippet_denotation}\n</snippet_path>\n<source>\n{content}\n</source>\n</read_only_snippet>'
     # attach all relevant snippets
     joined_relevant_snippets = "\n".join(
         relevant_snippet_template.format(
             i=i,
             snippet_denotation=snippet.denotation,
             content=snippet.expand(300).get_snippet(add_lines=False),
         ) for i, snippet in enumerate(relevant_snippets)
@@ -249,49 +256,67 @@
     messages.append(
         Message(
             role="user",
             content=read_only_snippets_message,
             key="relevant_snippets",
         )
     )
+
+    if import_graph:
+        sub_graph = import_graph.subgraph(
+            [snippet.file_path for snippet in relevant_snippets + read_only_snippets]
+        )
+        import_graph = generate_import_graph_text(sub_graph).strip("\n")
+        # serialize the graph so LLM can read it
+        graph_text = f"<graph_text>\nThis represents the file-to-file import graph, where each file is listed along with its imported files using arrows (──>) to show the directionality of the imports. Indentation is used to indicate the hierarchy of imports, and files that are not importing any other files are listed separately at the bottom.\n{import_graph}\n</graph_text>"
+
+        messages.append(
+            Message(
+                role="user",
+                content=graph_text,
+                key="graph_text",
+            )
+        )
+
     messages.append(
         Message(
             role="user",
             content=f"# Repo & Issue Metadata\nRepo: {repo_name}\nIssue: {problem_statement}",
         )
     )
     if pr_diffs:
         messages.append(
             Message(role="user", content=pr_diffs, key="pr_diffs")
         )
     try:
         print("messages")
         for message in messages:
             print(message.content + "\n\n")
-        joint_message = "\n\n".join(message.content for message in messages[1:-1])
+        joint_message = "\n\n".join(message.content for message in messages[1:])
         print("messages", joint_message)
         chat_gpt = ChatGPT(
             messages=[
                 Message(
                     role="system",
                     content=files_to_change_system_prompt,
                 ),
             ],
         )
         MODEL = "claude-3-opus-20240229"
         files_to_change_response = chat_gpt.chat_anthropic(
-            content=joint_message + "\n\n" + files_to_change_prompt,
+            content=joint_message + "\n\n" + (files_to_change_prompt if not context else context_files_to_change_prompt),
             model=MODEL,
             temperature=0.1
         )
         if chat_logger:
             chat_logger.add_chat(
                 {
                     "model": MODEL,
                     "messages": [{"role": message.role, "content": message.content} for message in chat_gpt.messages],
+                    "output": files_to_change_response,
                 })
         print("files_to_change_response", files_to_change_response)
         relevant_modules = []
         pattern = re.compile(r"<relevant_modules>(.*?)</relevant_modules>", re.DOTALL)
         relevant_modules_match = pattern.search(files_to_change_response)
         if relevant_modules_match:
             relevant_modules = [relevant_module.strip() for relevant_module in relevant_modules_match.group(1).split("\n") if relevant_module.strip()]
```

### Comparing `sweepai-2.0.1/sweepai/core/update_prompts.py` & `sweepai-2.0.2/sweepai/core/update_prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/core/vector_db.py` & `sweepai-2.0.2/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/create_pr.py` & `sweepai-2.0.2/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/on_button_click.py` & `sweepai-2.0.2/sweepai/handlers/on_button_click.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/on_button_click_test.py` & `sweepai-2.0.2/sweepai/handlers/on_button_click_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/on_check_suite.py` & `sweepai-2.0.2/sweepai/handlers/on_check_suite.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         file
         for file in zipfile.namelist()
         if file.startswith(dir) and not file.endswith("/")
     ]
 
 
 @file_cache()
-def download_logs(repo_full_name: str, run_id: int, installation_id: int):
+def download_logs(repo_full_name: str, run_id: int, installation_id: int, get_errors_only=True):
     token = get_token(installation_id)
     headers = {
         "Accept": "application/vnd.github+json",
         "Authorization": f"Bearer {token}",
         "X-GitHub-Api-Version": "2022-11-28",
     }
     response = requests.get(
@@ -53,14 +53,16 @@
         for file in zip_file.namelist():
             if file.endswith(".txt"):
                 with zip_file.open(file) as f:
                     logs = f.read().decode("utf-8")
                     last_line = logs.splitlines()[-1]
                     if "##[error]" in last_line:
                         logs_str += logs
+                    elif not get_errors_only: # get all logs
+                        logs_str += logs
     return logs_str
 
 gha_prompt = """\
 The below command yielded the following errors:
 <command>
 {command_line}
 </command>
```

### Comparing `sweepai-2.0.1/sweepai/handlers/on_comment.py` & `sweepai-2.0.2/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/on_jira_ticket.py` & `sweepai-2.0.2/sweepai/handlers/on_jira_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/on_merge.py` & `sweepai-2.0.2/sweepai/handlers/on_merge.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/on_merge_conflict.py` & `sweepai-2.0.2/sweepai/handlers/on_merge_conflict.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/on_review.py` & `sweepai-2.0.2/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/on_ticket.py` & `sweepai-2.0.2/sweepai/handlers/on_ticket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1377,16 +1377,16 @@
 
                 # create draft pr, then convert to regular pr later
                 pr: GithubPullRequest = repo.create_pull(
                     title=pr_changes.title,
                     body=pr_actions_message + pr_changes.body,
                     head=pr_changes.pr_head,
                     base=overrided_branch_name or SweepConfig.get_branch(repo),
-                    # TODO: reenable it later
-                    draft=True,
+                    # removed draft PR
+                    draft=False,
                 )
 
                 try:
                     pr.add_to_assignees(username)
                 except Exception as e:
                     logger.error(
                         f"Failed to add assignee {username}: {e}, probably a bot."
@@ -1904,8 +1904,8 @@
         + (purchase_message if not is_paying_user else "")
     )
     payment_message_start = (
         f"{user_type}: I'm using {model_name}. You have {gpt_tickets_left_message}{daily_message}. (tracking ID: <code>{tracking_id}</code>)"
         + (purchase_message if not is_paying_user else "")
     )
 
-    return payment_message, payment_message_start
+    return payment_message, payment_message_start
```

### Comparing `sweepai-2.0.1/sweepai/handlers/pr_utils.py` & `sweepai-2.0.2/sweepai/handlers/pr_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/stack_pr.py` & `sweepai-2.0.2/sweepai/handlers/stack_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/handlers/stack_pr_test.py` & `sweepai-2.0.2/sweepai/handlers/stack_pr_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/logn/cache.py` & `sweepai-2.0.2/sweepai/logn/cache.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/logn/logn.py` & `sweepai-2.0.2/sweepai/logn/logn.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/anthropic_client.py` & `sweepai-2.0.2/sweepai/utils/anthropic_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/autoimport.py` & `sweepai-2.0.2/sweepai/utils/autoimport.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/buttons.py` & `sweepai-2.0.2/sweepai/utils/buttons.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/buttons_test.py` & `sweepai-2.0.2/sweepai/utils/buttons_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/chat_logger.py` & `sweepai-2.0.2/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/code_tree.py` & `sweepai-2.0.2/sweepai/utils/code_tree.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/code_tree_test.py` & `sweepai-2.0.2/sweepai/utils/code_tree_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/comment_utils.py` & `sweepai-2.0.2/sweepai/utils/comment_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/comment_utils_test.py` & `sweepai-2.0.2/sweepai/utils/comment_utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/convert_openai_anthropic.py` & `sweepai-2.0.2/sweepai/utils/convert_openai_anthropic.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
             # Extract parameters within the parameters section
             parameter_matches = re.findall(parameter_pattern, parameters_section, re.DOTALL)
             function_parameters = {}
             for param in parameter_matches:
                 parameter_name = param[0]
                 parameter_value = param[1]
-                function_parameters[parameter_name] = parameter_value.strip()
+                function_parameters[parameter_name] = parameter_value.strip("\n")
 
             if function_name and function_parameters != {}:
                 function_calls.append(AnthropicFunctionCall(function_name, function_parameters))
 
         return function_calls
 
 def mock_function_calls_to_string(function_calls: list[AnthropicFunctionCall]) -> str:
```

### Comparing `sweepai-2.0.1/sweepai/utils/diff.py` & `sweepai-2.0.2/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/diff_test.py` & `sweepai-2.0.2/sweepai/utils/diff_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/docker_utils.py` & `sweepai-2.0.2/sweepai/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/event_logger.py` & `sweepai-2.0.2/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/fuzzy_diff.py` & `sweepai-2.0.2/sweepai/utils/fuzzy_diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/fuzzy_diff_test.py` & `sweepai-2.0.2/sweepai/utils/fuzzy_diff_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/github_utils.py` & `sweepai-2.0.2/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/github_utils_test.py` & `sweepai-2.0.2/sweepai/utils/github_utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/html_extractor.py` & `sweepai-2.0.2/sweepai/utils/html_extractor.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/modify_utils.py` & `sweepai-2.0.2/sweepai/utils/modify_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,25 +60,31 @@
         # only continue if it is unique, this will then later fail the uniqueness check
         if file_contents.count(new_code) > 1:
             return 0, False
         if new_code in file_contents:
             # now check how many leading whitespaces there are
             for line in file_lines:
                 if new_code in line:
+                    # unless the code is at the start of the line
+                    if line.startswith(new_code):
+                        return 0, False
                     return len(line)-len(line.lstrip()), False
         else:
             # now try rstrip if initially the code is not there
             new_code = new_code.rstrip()
             if file_contents.count(new_code) > 1: # uniqueness check
                 return 0, False
             if new_code in file_contents:
                # now check how many leading whitespaces there are
                 for line in file_lines:
                     if new_code in line:
-                        return len(line)-len(line.lstrip()), False
+                        # unless the code is at the start of the line
+                        if line.startswith(new_code):
+                            return 0, True
+                        return len(line)-len(line.lstrip()), True
         return -1, False
                 
     # assume one indent is two spaces and check max 10 indents
     for indent in range(0, 40, 2):
         new_code_lines = [f"{' ' * indent}{line}" for line in code_lines]
         new_code = "\n".join(new_code_lines)
         if new_code in file_contents:
```

### Comparing `sweepai-2.0.1/sweepai/utils/multi_query.py` & `sweepai-2.0.2/sweepai/utils/multi_query.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/openai_listwise_reranker.py` & `sweepai-2.0.2/sweepai/utils/openai_listwise_reranker.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/openai_proxy.py` & `sweepai-2.0.2/sweepai/utils/openai_proxy.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/openai_proxy_test.py` & `sweepai-2.0.2/sweepai/utils/openai_proxy_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/patch_utils.py` & `sweepai-2.0.2/sweepai/utils/patch_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/progress.py` & `sweepai-2.0.2/sweepai/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/prompt_constructor.py` & `sweepai-2.0.2/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/regex_utils.py` & `sweepai-2.0.2/sweepai/utils/regex_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/safe_pqueue.py` & `sweepai-2.0.2/sweepai/utils/safe_pqueue.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/scorer.py` & `sweepai-2.0.2/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/scorer_test.py` & `sweepai-2.0.2/sweepai/utils/scorer_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/search_and_replace.py` & `sweepai-2.0.2/sweepai/utils/search_and_replace.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/search_and_replace_test.py` & `sweepai-2.0.2/sweepai/utils/search_and_replace_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/str_utils.py` & `sweepai-2.0.2/sweepai/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/ticket_utils.py` & `sweepai-2.0.2/sweepai/utils/ticket_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from collections import defaultdict
 import traceback
 from time import time
 
 import cohere
 from loguru import logger
 from tqdm import tqdm
+import networkx as nx
 
 from sweepai.config.client import SweepConfig, get_blocked_dirs
 from sweepai.config.server import COHERE_API_KEY
-from sweepai.core.context_pruning import RepoContextManager, get_relevant_context, integrate_graph_retrieval
+from sweepai.core.context_pruning import RepoContextManager, add_relevant_files_to_top_snippets, build_import_trees, integrate_graph_retrieval
 from sweepai.core.entities import Snippet
 from sweepai.core.lexical_search import (
     compute_vector_search_scores,
     prepare_lexical_search_index,
     search_index,
 )
+from sweepai.core.sweep_bot import get_files_to_change
 from sweepai.logn.cache import file_cache
 from sweepai.utils.chat_logger import discord_log_error
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import ClonedRepo
 from sweepai.utils.multi_query import generate_multi_queries
 from sweepai.utils.openai_listwise_reranker import listwise_rerank_snippets
 from sweepai.utils.progress import TicketProgress
@@ -267,15 +269,15 @@
             key=lambda snippet: content_to_lexical_score[snippet.denotation],
             reverse=True,
         )[:k]
     if ticket_progress:
         ticket_progress.search_progress.retrieved_snippets = ranked_snippets
         ticket_progress.save()
     # you can use snippet.denotation and snippet.get_snippet()
-    if not skip_reranking:
+    if not skip_reranking and not skip_pointwise_reranking:
         ranked_snippets[:NUM_SNIPPETS_TO_RERANK] = listwise_rerank_snippets(queries[0], ranked_snippets[:NUM_SNIPPETS_TO_RERANK])
     snippet_paths = [snippet.file_path for snippet in ranked_snippets]
     prefixes = []
     for snippet_path in snippet_paths:
         snippet_depth = len(snippet_path.split("/"))
         for idx in range(snippet_depth):  # heuristic
             if idx > snippet_depth // 2:
@@ -307,14 +309,79 @@
         queries = [query, *generate_multi_queries(query)]
     else:
         queries = [query]
     return multi_prep_snippets(
         cloned_repo, queries, ticket_progress, k, skip_reranking
     )
 
+def get_relevant_context(
+    query: str,
+    repo_context_manager: RepoContextManager,
+    seed: int = None,
+    import_graph: nx.DiGraph = None,
+    chat_logger = None,
+) -> RepoContextManager:
+    logger.info("Seed: " + str(seed))
+    repo_context_manager = build_import_trees(
+        repo_context_manager,
+        import_graph,
+    )
+    repo_context_manager = add_relevant_files_to_top_snippets(repo_context_manager)
+    repo_context_manager.dir_obj.add_relevant_files(
+        repo_context_manager.relevant_file_paths
+    )
+    fcrs, plan = get_files_to_change(
+        relevant_snippets=repo_context_manager.current_top_snippets,
+        read_only_snippets=repo_context_manager.snippets,
+        problem_statement=query,
+        repo_name=repo_context_manager.cloned_repo.repo_full_name,
+        import_graph=import_graph,
+        chat_logger=chat_logger,
+        seed=seed,
+        context=True
+    )
+    repo_context_manager.current_top_snippets = []
+    repo_context_manager.read_only_snippets = []
+    visited_paths = set()
+    for fcr in fcrs:
+        if fcr.filename in visited_paths:
+            continue
+        visited_paths.add(fcr.filename)
+        try:
+            content = repo_context_manager.cloned_repo.get_file_contents(fcr.filename)
+        except FileNotFoundError:
+            continue
+        snippet = Snippet(
+            file_path=fcr.filename,
+            start=0,
+            end=len(content.split("\n")),
+            content=content,
+        )
+        repo_context_manager.current_top_snippets.append(snippet)
+    repo_context_manager.read_only_snippets = []
+    if fcrs:
+        for file_path in fcrs[0].relevant_files:
+            if file_path in visited_paths:
+                continue
+            visited_paths.add(file_path)
+            try:
+                content = repo_context_manager.cloned_repo.get_file_contents(file_path)
+            except FileNotFoundError:
+                continue
+            snippet = Snippet(
+                file_path=file_path,
+                start=0,
+                end=len(content.split("\n")),
+                content=content,
+            )
+            repo_context_manager.read_only_snippets.append(snippet)
+    else:
+        raise Exception("No file change requests created.")
+    return repo_context_manager
+
 def fetch_relevant_files(
     cloned_repo,
     title,
     summary,
     replies_text,
     username,
     metadata,
```

### Comparing `sweepai-2.0.1/sweepai/utils/timer.py` & `sweepai-2.0.2/sweepai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/tree_utils.py` & `sweepai-2.0.2/sweepai/utils/tree_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/user_settings.py` & `sweepai-2.0.2/sweepai/utils/user_settings.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/utils.py` & `sweepai-2.0.2/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/utils/utils_test.py` & `sweepai-2.0.2/sweepai/utils/utils_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/watch.py` & `sweepai-2.0.2/sweepai/watch.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/web/event_utils.py` & `sweepai-2.0.2/sweepai/web/event_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/web/events.py` & `sweepai-2.0.2/sweepai/web/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/web/health.py` & `sweepai-2.0.2/sweepai/web/health.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai/web/health_test.py` & `sweepai-2.0.2/sweepai/web/health_test.py`

 * *Files identical despite different names*

### Comparing `sweepai-2.0.1/sweepai.egg-info/PKG-INFO` & `sweepai-2.0.2/sweepai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 2.0.1
+Version: 2.0.2
 Summary: Sweep fixes GitHub issues
 Author-email: Kevin Lu <kevin@sweep.dev>, William Zeng <william@sweep.dev>, Martin Ye <martin@sweep.dev>
 License: Sweep Enterprise Edition (EE) license (the “EE License”)
         Copyright (c) 2024-present Sweep AI, Inc.
         
         With regard to the Sweep Software:
         
@@ -36,17 +36,18 @@
 Requires-Dist: rich==13.7.1
 Requires-Dist: fastapi==0.110.0
 Requires-Dist: prometheus-fastapi-instrumentator==7.0.0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: openai==1.13.3
 Requires-Dist: backoff==2.2.1
-Requires-Dist: pymongo==4.6.2
+Requires-Dist: pymongo==4.6.3
 Requires-Dist: gitpython==3.1.42
 Requires-Dist: tree-sitter==0.21.0
+Requires-Dist: tree-sitter-python==0.21.0
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: rapidfuzz==3.6.2
 Requires-Dist: importmagic==0.1.7
 Requires-Dist: hatchet-sdk==0.18.0
 Requires-Dist: pyflakes==3.2.0
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: networkx==3.2.1
```

### Comparing `sweepai-2.0.1/sweepai.egg-info/SOURCES.txt` & `sweepai-2.0.2/sweepai.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -108,8 +108,13 @@
 sweepai/utils/utils_test.py
 sweepai/web/event_utils.py
 sweepai/web/events.py
 sweepai/web/health.py
 sweepai/web/health_test.py
 tests/test_gha_extraction.py
 tests/test_jira_ticket.py
-tests/test_watch.py
+tests/test_run_gha.py
+tests/test_watch.py
+vendor/tree-sitter-go/setup.py
+vendor/tree-sitter-go/bindings/python/tree_sitter_go/__init__.py
+vendor/tree-sitter-go/bindings/python/tree_sitter_go/__init__.pyi
+vendor/tree-sitter-go/bindings/python/tree_sitter_go/py.typed
```

### Comparing `sweepai-2.0.1/sweepai.egg-info/requires.txt` & `sweepai-2.0.2/sweepai.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 rich==13.7.1
 fastapi==0.110.0
 prometheus-fastapi-instrumentator==7.0.0
 pyyaml==6.0.1
 python-dotenv==1.0.1
 openai==1.13.3
 backoff==2.2.1
-pymongo==4.6.2
+pymongo==4.6.3
 gitpython==3.1.42
 tree-sitter==0.21.0
+tree-sitter-python==0.21.0
 tree-sitter-languages==1.10.2
 rapidfuzz==3.6.2
 importmagic==0.1.7
 hatchet-sdk==0.18.0
 pyflakes==3.2.0
 beautifulsoup4==4.12.3
 networkx==3.2.1
```

### Comparing `sweepai-2.0.1/tests/test_gha_extraction.py` & `sweepai-2.0.2/tests/test_gha_extraction.py`

 * *Files identical despite different names*

