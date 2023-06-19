# Comparing `tmp/promptimize-0.2.2.tar.gz` & `tmp/promptimize-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptimize-0.2.2.tar", last modified: Tue Apr 25 16:55:17 2023, max compression
+gzip compressed data, was "promptimize-0.2.3.tar", last modified: Mon Jun 19 19:56:56 2023, max compression
```

## Comparing `promptimize-0.2.2.tar` & `promptimize-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.940752 promptimize-0.2.2/
--rw-r--r--   0 max        (501) staff       (20)       56 2023-04-07 20:39:22.000000 promptimize-0.2.2/.gitignore
--rw-r--r--   0 max        (501) staff       (20)       57 2023-04-08 19:15:24.000000 promptimize-0.2.2/.mypy.ini
--rw-r--r--   0 max        (501) staff       (20)     2058 2023-04-25 01:37:21.000000 promptimize-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 max        (501) staff       (20)    11358 2023-04-08 19:28:50.000000 promptimize-0.2.2/LICENSE
--rw-r--r--   0 max        (501) staff       (20)    13056 2023-04-25 16:55:17.940003 promptimize-0.2.2/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)    10594 2023-04-25 16:53:54.000000 promptimize-0.2.2/README.md
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.927226 promptimize-0.2.2/docs/
--rw-r--r--   0 max        (501) staff       (20)      685 2023-04-08 20:12:24.000000 promptimize-0.2.2/docs/Makefile
--rwxr-xr-x   0 max        (501) staff       (20)      565 2023-04-25 01:09:25.000000 promptimize-0.2.2/docs/publish.sh
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.929436 promptimize-0.2.2/docs/source/
--rw-r--r--   0 max        (501) staff       (20)     8144 2023-04-20 19:39:26.000000 promptimize-0.2.2/docs/source/README.md
--rw-r--r--   0 max        (501) staff       (20)     1268 2023-04-20 01:56:57.000000 promptimize-0.2.2/docs/source/conf.py
--rw-r--r--   0 max        (501) staff       (20)      111 2023-04-20 02:07:39.000000 promptimize-0.2.2/docs/source/index.rst
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.930704 promptimize-0.2.2/examples/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.931418 promptimize-0.2.2/examples/__pycache__/
--rw-r--r--   0 max        (501) staff       (20)     2557 2023-04-05 07:54:58.000000 promptimize-0.2.2/examples/__pycache__/use_cases.cpython-38.pyc
--rw-r--r--   0 max        (501) staff       (20)     2937 2023-04-25 00:36:26.000000 promptimize-0.2.2/examples/readme_examples.py
--rw-r--r--   0 max        (501) staff       (20)      892 2023-04-20 19:54:23.000000 promptimize-0.2.2/examples/readme_hello_world.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.936206 promptimize-0.2.2/promptimize/
--rw-r--r--   0 max        (501) staff       (20)       40 2023-04-25 01:13:35.000000 promptimize-0.2.2/promptimize/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     3556 2023-04-25 01:15:16.000000 promptimize-0.2.2/promptimize/cli.py
--rw-r--r--   0 max        (501) staff       (20)     1843 2023-04-25 01:16:34.000000 promptimize-0.2.2/promptimize/crawler.py
--rw-r--r--   0 max        (501) staff       (20)     4192 2023-04-25 01:20:03.000000 promptimize-0.2.2/promptimize/evals.py
--rw-r--r--   0 max        (501) staff       (20)     7673 2023-04-25 16:45:38.000000 promptimize-0.2.2/promptimize/prompt_cases.py
--rw-r--r--   0 max        (501) staff       (20)     3181 2023-04-25 16:49:57.000000 promptimize-0.2.2/promptimize/reports.py
--rw-r--r--   0 max        (501) staff       (20)      200 2023-04-05 07:16:13.000000 promptimize-0.2.2/promptimize/simple_jinja.py
--rw-r--r--   0 max        (501) staff       (20)     5910 2023-04-25 01:25:06.000000 promptimize-0.2.2/promptimize/suite.py
--rw-r--r--   0 max        (501) staff       (20)     9068 2023-04-25 01:25:49.000000 promptimize-0.2.2/promptimize/utils.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 16:55:17.938893 promptimize-0.2.2/promptimize.egg-info/
--rw-r--r--   0 max        (501) staff       (20)    13056 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      743 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       71 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/entry_points.txt
--rw-r--r--   0 max        (501) staff       (20)       65 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)       12 2023-04-25 16:55:17.000000 promptimize-0.2.2/promptimize.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)       31 2023-04-25 01:19:56.000000 promptimize-0.2.2/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)       97 2023-04-25 01:11:21.000000 promptimize-0.2.2/requirements-dev.txt
--rw-r--r--   0 max        (501) staff       (20)       65 2023-04-19 00:07:38.000000 promptimize-0.2.2/requirements.txt
--rw-r--r--   0 max        (501) staff       (20)       38 2023-04-25 16:55:17.941028 promptimize-0.2.2/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)      899 2023-04-25 16:54:48.000000 promptimize-0.2.2/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-19 19:56:56.731049 promptimize-0.2.3/
+-rw-r--r--   0 max        (501) staff       (20)       56 2023-04-07 20:39:22.000000 promptimize-0.2.3/.gitignore
+-rw-r--r--   0 max        (501) staff       (20)       57 2023-04-08 19:15:24.000000 promptimize-0.2.3/.mypy.ini
+-rw-r--r--   0 max        (501) staff       (20)     2043 2023-06-19 19:49:29.000000 promptimize-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 max        (501) staff       (20)    11358 2023-04-08 19:28:50.000000 promptimize-0.2.3/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)    10929 2023-06-19 19:56:56.730550 promptimize-0.2.3/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)    10592 2023-06-19 19:23:02.000000 promptimize-0.2.3/README.md
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-19 19:56:56.719740 promptimize-0.2.3/docs/
+-rw-r--r--   0 max        (501) staff       (20)      685 2023-04-08 20:12:24.000000 promptimize-0.2.3/docs/Makefile
+-rwxr-xr-x   0 max        (501) staff       (20)      565 2023-04-25 01:09:25.000000 promptimize-0.2.3/docs/publish.sh
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-19 19:56:56.721315 promptimize-0.2.3/docs/source/
+-rw-r--r--   0 max        (501) staff       (20)     8152 2023-06-19 19:19:49.000000 promptimize-0.2.3/docs/source/README.md
+-rw-r--r--   0 max        (501) staff       (20)     1283 2023-06-19 19:19:06.000000 promptimize-0.2.3/docs/source/conf.py
+-rw-r--r--   0 max        (501) staff       (20)      111 2023-04-20 02:07:39.000000 promptimize-0.2.3/docs/source/index.rst
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-19 19:56:56.722423 promptimize-0.2.3/examples/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-19 19:56:56.723033 promptimize-0.2.3/examples/__pycache__/
+-rw-r--r--   0 max        (501) staff       (20)     2557 2023-04-05 07:54:58.000000 promptimize-0.2.3/examples/__pycache__/use_cases.cpython-38.pyc
+-rw-r--r--   0 max        (501) staff       (20)     2976 2023-06-19 19:51:16.000000 promptimize-0.2.3/examples/readme_examples.py
+-rw-r--r--   0 max        (501) staff       (20)      892 2023-04-20 19:54:23.000000 promptimize-0.2.3/examples/readme_hello_world.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-19 19:56:56.726811 promptimize-0.2.3/promptimize/
+-rw-r--r--   0 max        (501) staff       (20)       40 2023-04-25 01:13:35.000000 promptimize-0.2.3/promptimize/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     3561 2023-04-26 15:35:02.000000 promptimize-0.2.3/promptimize/cli.py
+-rw-r--r--   0 max        (501) staff       (20)     1843 2023-04-25 01:16:34.000000 promptimize-0.2.3/promptimize/crawler.py
+-rw-r--r--   0 max        (501) staff       (20)     4394 2023-04-28 03:57:19.000000 promptimize-0.2.3/promptimize/evals.py
+-rw-r--r--   0 max        (501) staff       (20)     8147 2023-05-05 17:03:30.000000 promptimize-0.2.3/promptimize/prompt_cases.py
+-rw-r--r--   0 max        (501) staff       (20)     3181 2023-04-25 16:49:57.000000 promptimize-0.2.3/promptimize/reports.py
+-rw-r--r--   0 max        (501) staff       (20)      200 2023-04-05 07:16:13.000000 promptimize-0.2.3/promptimize/simple_jinja.py
+-rw-r--r--   0 max        (501) staff       (20)     6597 2023-06-19 19:49:29.000000 promptimize-0.2.3/promptimize/suite.py
+-rw-r--r--   0 max        (501) staff       (20)     9068 2023-04-25 01:25:49.000000 promptimize-0.2.3/promptimize/utils.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-19 19:56:56.729821 promptimize-0.2.3/promptimize.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)    10929 2023-06-19 19:56:56.000000 promptimize-0.2.3/promptimize.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      743 2023-06-19 19:56:56.000000 promptimize-0.2.3/promptimize.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-06-19 19:56:56.000000 promptimize-0.2.3/promptimize.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       71 2023-06-19 19:56:56.000000 promptimize-0.2.3/promptimize.egg-info/entry_points.txt
+-rw-r--r--   0 max        (501) staff       (20)       79 2023-06-19 19:56:56.000000 promptimize-0.2.3/promptimize.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)       12 2023-06-19 19:56:56.000000 promptimize-0.2.3/promptimize.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)       31 2023-04-25 01:19:56.000000 promptimize-0.2.3/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)       97 2023-04-25 01:11:21.000000 promptimize-0.2.3/requirements-dev.txt
+-rw-r--r--   0 max        (501) staff       (20)       79 2023-06-19 19:20:26.000000 promptimize-0.2.3/requirements.txt
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-06-19 19:56:56.731182 promptimize-0.2.3/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)      899 2023-06-19 19:54:46.000000 promptimize-0.2.3/setup.py
```

### Comparing `promptimize-0.2.2/.pre-commit-config.yaml` & `promptimize-0.2.3/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -17,32 +17,31 @@
 repos:
   #- repo: https://github.com/pre-commit/mirrors-mypy
   #  rev: v0.941
   #  hooks:
   #    - id: mypy
   #      additional_dependencies: [types-all]
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.2.0
+    rev: v4.4.0
     hooks:
-      - id: check-docstring-first
       - id: check-added-large-files
         exclude: \.(geojson)$
       - id: check-yaml
         exclude: ^helm/superset/templates/
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
         args: ["--markdown-linebreak-ext=md"]
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.4.1 # Use the sha or tag you want to point at
+    rev: v3.0.0-alpha.9-for-vscode # Use the sha or tag you want to point at
     hooks:
       - id: prettier
         args: ["--ignore-path=./superset-frontend/.prettierignore"]
         files: "superset-frontend"
   # blacklist unsafe functions like make_url (see #19526)
   - repo: https://github.com/skorokithakis/blacklist-pre-commit-hook
     rev: e2f070289d8eddcaec0b580d3bde29437e7c8221
```

### Comparing `promptimize-0.2.2/LICENSE` & `promptimize-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.2/PKG-INFO` & `promptimize-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,278 +1,281 @@
 Metadata-Version: 2.1
 Name: promptimize
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python toolkit to generate and evaluate prompts for GPT at scale
 Home-page: UNKNOWN
 Author: Maxime Beauchemin
 Author-email: maximebeauchemin@gmail.com
 License: Apache License, Version 2.0
-Description: # 💡 ¡promptimize! 💡
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        [![PyPI version](https://badge.fury.io/py/promptimize.svg)](https://badge.fury.io/py/promptimize)
-        
-        <img src="https://user-images.githubusercontent.com/487433/229948453-36cbc2d1-e71f-4e87-9111-ab428bc96f4c.png" width=300/>
-        
-        Promptimize is a prompt engineering **evaluation** and **testing** toolkit.
-        
-        It accelerates and provides structure around prompt engineering at scale
-        with confidence, bringing some of the ideas behind test-driven
-        development (TDD) to engineering prompts.
-        
-        With promptimize, you can:
-        
-        - Define your "prompt cases" (think "test cases" but specific to evaluating
-          prompts) as code and associate them with evaluation functions
-        - Generate prompt variations dynamically
-        - Execute and rank prompts test suites across different
-          engines/models/temperature/settings and compare results, brining
-          the hyperparameter tuning mindset to prompt engineering
-        - Get reports on your prompts' performance as you iterate. Answer question
-          around how different prompt suites are performing against one-another.
-          Which individual cases or categories of cases improved? regressed?
-        - Minimize API calls! only re-assess what changed as you change it
-        - Perform human if and where needed, introspected failed cases, overriding
-          false negatives
-        
-        In essence, promptimize provides a programmatic way to execute and fine-tune
-        your prompts and evaluation functions in Python, allowing you to iterate
-        quickly and with confidence.
-        
-        ## Hello world - the simplest prompt examples
-        [more examples on GitHub](https://github.com/preset-io/promptimize/tree/main/examples)
-        ```python
-        # Brining some "prompt generator" classes - note that you can derive and extend those
-        from promptimize.prompts import SimplePrompt
-        
-        # Bringing some useful eval function that help evaluating and scoring responses
-        # eval functions have a handle on the prompt object and are expected
-        # to return a score between 0 and 1
-        from promptimize import evals
-        
-        # Promptimize will scan the target folder and find all Prompt objects
-        # and derivatives that are in the python modules
-        simple_prompts = [
-        
-            # Prompting "hello there" and making sure there's "hi" or "hello"
-            # somewhere in the answer
-            PromptCase("hello there!", lambda x: evals.any_word(x, ["hi", "hello"])),
-            PromptCase(
-                "name the top 50 guitar players!", lambda x: evals.all_words(x, ["frank zappa"])
-            ),
-        ]
-        ```
-        
-        ### The CLI's `run` command
-        ```
-        $ promptimize run --help
-        Usage: promptimize run [OPTIONS] PATH
-        
-          run some prompts
-        
-        Options:
-          -v, --verbose             Trigger more verbose output
-          -f, --force               Force run, do not skip
-          -h, --human               Human review, allowing a human to review and force
-                                    pass/fail each prompt case
-          -r, --repair              Only re-run previously failed
-          -x, --dry-run             DRY run, don't call the API
-          --shuffle                 Shuffle the prompts in a random order
-          -s, --style [json|yaml]   json or yaml formatting
-          -m, --max-tokens INTEGER  max_tokens passed to the model
-          -l, --limit INTEGER       limit how many prompt cases to run in a single
-                                    batch
-          -t, --temperature FLOAT   max_tokens passed to the model
-          -e, --engine TEXT         model as accepted by the openai API
-          -k, --key TEXT            The keys to run
-          -o, --output PATH
-          -s, --silent
-        ```
-        
-        Let's run those examples and produce a report `./report.yaml`
-        ```
-        $ promptimize run examples/ --output ./report.yaml
-        ```
-        
-        ```yaml
-        💡 ¡promptimize! 💡
-        # ----------------------------------------
-        # (1/2) [RUN] prompt: prompt-115868ef
-        # ----------------------------------------
-        key: prompt-115868ef
-        user_input: hello there!
-        prompt_hash: 115868ef
-        response: Hi there! How are you doing today?
-        execution:
-          api_call_duration_ms: 883.8047981262207
-          run_at: '2023-04-25T02:21:40.443077'
-          score: 1.0
-        
-        # ----------------------------------------
-        # (2/2) [RUN] prompt: prompt-5c085656
-        # ----------------------------------------
-        key: prompt-5c085656
-        user_input: name the top 10 guitar players!
-        prompt_hash: 5c085656
-        response: |-
-          1. Jimi Hendrix
-          2. Eric Clapton
-          {{ ... }}
-          11. Carlos Santana
-        weight: 2
-        execution:
-          api_call_duration_ms: 2558.135747909546
-          run_at: '2023-04-25T02:21:43.007529'
-          score: 0.0
-        
-        # ----------------------------------------
-        # Suite summary
-        # ----------------------------------------
-        suite_score: 0.3333333333333333
-        git_info:
-          sha: 2cf28498ba0f
-          branch: main
-          dirty: true
-        ```
-        
-        ## Problem + POV
-        
-        Thousands of product builders are currently trying to figure out how to
-        bring the power of AI into the products and experiences they are building.
-        The probabilistic (often semi-random, sometimes hectic) nature of LLMs
-        makes this a challenge.
-        
-        Prompt engineering is a huge piece of the puzzle in terms of how to do this
-        right, especially given the complexity, risks, and drawbacks around
-        model tuning.
-        
-        We believe product builders need to tame AI through proper, rigorous
-        **prompt engineering**. This allows making the probabilistic nature of
-        AI more deterministic, or somewhat predictable, and allows builders to apply
-        a hyperparameter tuning-type mindset and approach to prompt engineering.
-        
-        Any prompt-generator logic that's going to be let loose in the wild inside
-        a product should be thoroughly tested and evaluated with "prompt cases" that
-        cover the breath of what people may do in a product.
-        
-        In short, Promptimize allows you to test prompts at industrial scale,
-        so that you can confidently use them in the products you are building.
-        
-        ## Information Architecture
-        
-        - **Prompt:** A Prompt instance is a certain test case, a single prompt
-          with an associated set of evaluation functions to rate its success.
-        - **Evaluation:** An evaluation function that reads the response and returns
-          a success rate between `0` and `1`.
-        - **Suite:** A Suite is a collection of Prompt; it's able to run things,
-          accumulate results, and print reports about its collection of use cases.
-        - **Report**: a report is the compiled results of running a certain prompt
-          `Suite` or set of suites. Reports can be consumed, compared, and expanded.
-        
-        ## Principles
-        
-        - **Configuration as code:** All prompt cases, suites, and evaluations are
-          defined as code, which makes it easy to dynamically generate all sorts
-          of use cases and suites.
-        - **Expressive**: a clean DSL that's to-the-point -> user prompt + assertions.
-          the actually prompt creation logic lives in the derivative class of `PromptCase`,
-          so that we can have clean, dense files that contain nice `Suite`s
-        - **Support the iteration mindset:** making it easy for people to try things,
-          get suggestions from the AI, adapt, compare, and push forward
-        - **Extensibility:** the toolkit is designed to be extremely hackable and
-          extensible. Hooks, extensions, high API surface.
-        - **AI-powered:** the framework offers ways to expand your suites based
-          on the examples that exists. Use AI to generate more prompt cases!
-        
-        
-        ## Interesting features / facts
-        
-        Listing out a few features you should know about that you can start using as your
-        suites of prompts become larger / more complex
-        
-        * evaluation functions are assumed to return a value between 0 and 1.
-          contrarily to unit tests, prompt cases aren't boolean
-        * prompts can be assigned a `weight` (default 1) this enables you to define
-          which prompts are more important than others for reporting purposes and suite evaluation
-        * prompts can be assigned a `category`, this can be used in the reporting.
-          That helps understanding which categories are performing better than
-          others, or are most affected by iterations
-        * The `Prompt` class `pre_run` and `post_run` hooks if you want to do
-          post-processing for instance. An example of that would be if you do a prompt
-          that expects GPT to generate code, and you'd like actually say run that code
-          and test it. In our SQL implementation, we run the SQL against the database
-          for instance and get a pandas dataframe back, and allow doing assertions
-          on the dataframe itself
-        
-        
-        
-        ## Getting started
-        
-        To install the Promptimize package, use the following command:
-        ```bash
-        pip install promptimize
-        ```
-        
-        First you'll need an openai API key, let's set it as an env var
-        ```bash
-        export OPENAI_API_KEY=sk-{{ REDACTED }}
-        ```
-        
-        Find the examples executed below
-        [here](https://github.com/preset-io/promptimize/blob/main/examples/readme_examples.py)
-        
-        ```bash
-        # Clone the repo
-        git clone git@github.com:preset-io/promptimize.git
-        cd promptimize
-        
-        # NOTE: CLI is `promptimize`, but `p9e` is a shorter synonym, can be used interchangibly
-        # First let's run some of the examples
-        p9e run ./examples
-        
-        # Now the same but with verbose output
-        p9e run ./examples --verbose --output ./report.yaml
-        
-        ```
-        ## Langchain
-        
-        How does promptimize relate to `langchain`?
-        
-        We think langchain is amazing and promptimize uses langchain under the
-        hood to interact with openai, and has integration with langchain
-        (see `LangchainPromptCase`, and the upcoming `LangchainChainPromptCase`
-        and `LangchainAgntPromptCase`)
-        While you don't have to use
-        langchain, and could use promptimize on top of any python prompt generation
-        whether it'd be another library or some home grown thing.
-        
-        
-        ## Context
-        
-        <img src="https://user-images.githubusercontent.com/487433/230508578-456a7040-1184-433a-a555-dceb7c28c32c.png" width="75" title="Max"/>
-        
-        Where is `promptimize` coming from!? I'm (Maxime Beauchemin) a startup
-        founder at <a href="www.preset.io">Preset</a> working on brining AI to BI
-        (data exploration,
-        and visualization). At Preset, we use `promptimize` to generate
-        complex SQL based on natural language, and to suggest charts to users. We
-        derive the `SimpleQuery` class to make it fitted to our specific use
-        cases in our own prompt engineering repo. It's not my first open source project
-        as the creator of
-        [Apache Superset](https://github.com/apache/superset/) and
-        [Apache Airflow](https://github.com/apache/airflow/)
-        
-        
-        ## Contribute
-        
-        This project is in its super early stages as of `0.2.0`, and contributions,
-        contributors, and maintainers are highly encouraged. While it's a great time
-        to onboard and influence the direction of the project, things are still
-        evolving quickly. To get involved, open a GitHub issue
-        or submit a pull request!
-        
-        ## Links
-        * [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/introducing-promptimize/)
-        * [Preset Blog](https://preset.io/blog/)
-        * [Promptimize DOCS](https://preset-io.github.io/promptimize/)
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# 💡 ¡promptimize! 💡
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![PyPI version](https://badge.fury.io/py/promptimize.svg)](https://badge.fury.io/py/promptimize)
+
+<img src="https://user-images.githubusercontent.com/487433/229948453-36cbc2d1-e71f-4e87-9111-ab428bc96f4c.png" width=300/>
+
+Promptimize is a prompt engineering **evaluation** and **testing** toolkit.
+
+It accelerates and provides structure around prompt engineering at scale
+with confidence, bringing some of the ideas behind test-driven
+development (TDD) to engineering prompts.
+
+With promptimize, you can:
+
+- Define your "prompt cases" (think "test cases" but specific to evaluating
+  prompts) as code and associate them with evaluation functions
+- Generate prompt variations dynamically
+- Execute and rank prompts test suites across different
+  engines/models/temperature/settings and compare results, brining
+  the hyperparameter tuning mindset to prompt engineering
+- Get reports on your prompts' performance as you iterate. Answer question
+  around how different prompt suites are performing against one-another.
+  Which individual cases or categories of cases improved? regressed?
+- Minimize API calls! only re-assess what changed as you change it
+- Perform human if and where needed, introspected failed cases, overriding
+  false negatives
+
+In essence, promptimize provides a programmatic way to execute and fine-tune
+your prompts and evaluation functions in Python, allowing you to iterate
+quickly and with confidence.
+
+## Hello world - the simplest prompt examples
+[more examples on GitHub](https://github.com/preset-io/promptimize/tree/main/examples)
+```python
+# Brining some "prompt generator" classes - note that you can derive and extend those
+from promptimize.prompts import PromptCase
+
+# Bringing some useful eval function that help evaluating and scoring responses
+# eval functions have a handle on the prompt object and are expected
+# to return a score between 0 and 1
+from promptimize import evals
+
+# Promptimize will scan the target folder and find all Prompt objects
+# and derivatives that are in the python modules
+simple_prompts = [
+
+    # Prompting "hello there" and making sure there's "hi" or "hello"
+    # somewhere in the answer
+    PromptCase("hello there!", lambda x: evals.any_word(x, ["hi", "hello"])),
+    PromptCase(
+        "name the top 50 guitar players!", lambda x: evals.all_words(x, ["frank zappa"])
+    ),
+]
+```
+
+### The CLI's `run` command
+```
+$ promptimize run --help
+Usage: promptimize run [OPTIONS] PATH
+
+  run some prompts
+
+Options:
+  -v, --verbose             Trigger more verbose output
+  -f, --force               Force run, do not skip
+  -h, --human               Human review, allowing a human to review and force
+                            pass/fail each prompt case
+  -r, --repair              Only re-run previously failed
+  -x, --dry-run             DRY run, don't call the API
+  --shuffle                 Shuffle the prompts in a random order
+  -s, --style [json|yaml]   json or yaml formatting
+  -m, --max-tokens INTEGER  max_tokens passed to the model
+  -l, --limit INTEGER       limit how many prompt cases to run in a single
+                            batch
+  -t, --temperature FLOAT   max_tokens passed to the model
+  -e, --engine TEXT         model as accepted by the openai API
+  -k, --key TEXT            The keys to run
+  -o, --output PATH
+  -s, --silent
+```
+
+Let's run those examples and produce a report `./report.yaml`
+```
+$ promptimize run examples/ --output ./report.yaml
+```
+
+```yaml
+💡 ¡promptimize! 💡
+# ----------------------------------------
+# (1/2) [RUN] prompt: prompt-115868ef
+# ----------------------------------------
+key: prompt-115868ef
+user_input: hello there!
+prompt_hash: 115868ef
+response: Hi there! How are you doing today?
+execution:
+  api_call_duration_ms: 883.8047981262207
+  run_at: '2023-04-25T02:21:40.443077'
+  score: 1.0
+
+# ----------------------------------------
+# (2/2) [RUN] prompt: prompt-5c085656
+# ----------------------------------------
+key: prompt-5c085656
+user_input: name the top 10 guitar players!
+prompt_hash: 5c085656
+response: |-
+  1. Jimi Hendrix
+  2. Eric Clapton
+  {{ ... }}
+  11. Carlos Santana
+weight: 2
+execution:
+  api_call_duration_ms: 2558.135747909546
+  run_at: '2023-04-25T02:21:43.007529'
+  score: 0.0
+
+# ----------------------------------------
+# Suite summary
+# ----------------------------------------
+suite_score: 0.3333333333333333
+git_info:
+  sha: 2cf28498ba0f
+  branch: main
+  dirty: true
+```
+
+## Problem + POV
+
+Thousands of product builders are currently trying to figure out how to
+bring the power of AI into the products and experiences they are building.
+The probabilistic (often semi-random, sometimes hectic) nature of LLMs
+makes this a challenge.
+
+Prompt engineering is a huge piece of the puzzle in terms of how to do this
+right, especially given the complexity, risks, and drawbacks around
+model tuning.
+
+We believe product builders need to tame AI through proper, rigorous
+**prompt engineering**. This allows making the probabilistic nature of
+AI more deterministic, or somewhat predictable, and allows builders to apply
+a hyperparameter tuning-type mindset and approach to prompt engineering.
+
+Any prompt-generator logic that's going to be let loose in the wild inside
+a product should be thoroughly tested and evaluated with "prompt cases" that
+cover the breath of what people may do in a product.
+
+In short, Promptimize allows you to test prompts at industrial scale,
+so that you can confidently use them in the products you are building.
+
+## Information Architecture
+
+- **Prompt:** A Prompt instance is a certain test case, a single prompt
+  with an associated set of evaluation functions to rate its success.
+- **Evaluation:** An evaluation function that reads the response and returns
+  a success rate between `0` and `1`.
+- **Suite:** A Suite is a collection of Prompt; it's able to run things,
+  accumulate results, and print reports about its collection of use cases.
+- **Report**: a report is the compiled results of running a certain prompt
+  `Suite` or set of suites. Reports can be consumed, compared, and expanded.
+
+## Principles
+
+- **Configuration as code:** All prompt cases, suites, and evaluations are
+  defined as code, which makes it easy to dynamically generate all sorts
+  of use cases and suites.
+- **Expressive**: a clean DSL that's to-the-point -> user prompt + assertions.
+  the actually prompt creation logic lives in the derivative class of `PromptCase`,
+  so that we can have clean, dense files that contain nice `Suite`s
+- **Support the iteration mindset:** making it easy for people to try things,
+  get suggestions from the AI, adapt, compare, and push forward
+- **Extensibility:** the toolkit is designed to be extremely hackable and
+  extensible. Hooks, extensions, high API surface.
+- **AI-powered:** the framework offers ways to expand your suites based
+  on the examples that exists. Use AI to generate more prompt cases!
+
+
+## Interesting features / facts
+
+Listing out a few features you should know about that you can start using as your
+suites of prompts become larger / more complex
+
+* evaluation functions are assumed to return a value between 0 and 1.
+  contrarily to unit tests, prompt cases aren't boolean
+* prompts can be assigned a `weight` (default 1) this enables you to define
+  which prompts are more important than others for reporting purposes and suite evaluation
+* prompts can be assigned a `category`, this can be used in the reporting.
+  That helps understanding which categories are performing better than
+  others, or are most affected by iterations
+* The `Prompt` class `pre_run` and `post_run` hooks if you want to do
+  post-processing for instance. An example of that would be if you do a prompt
+  that expects GPT to generate code, and you'd like actually say run that code
+  and test it. In our SQL implementation, we run the SQL against the database
+  for instance and get a pandas dataframe back, and allow doing assertions
+  on the dataframe itself
+
+
+
+## Getting started
+
+To install the Promptimize package, use the following command:
+```bash
+pip install promptimize
+```
+
+First you'll need an openai API key, let's set it as an env var
+```bash
+export OPENAI_API_KEY=sk-{{ REDACTED }}
+```
+
+Find the examples executed below
+[here](https://github.com/preset-io/promptimize/blob/main/examples/readme_examples.py)
+
+```bash
+# Clone the repo
+git clone git@github.com:preset-io/promptimize.git
+cd promptimize
+
+# NOTE: CLI is `promptimize`, but `p9e` is a shorter synonym, can be used interchangibly
+# First let's run some of the examples
+p9e run ./examples
+
+# Now the same but with verbose output
+p9e run ./examples --verbose --output ./report.yaml
+
+```
+## Langchain
+
+How does promptimize relate to `langchain`?
+
+We think langchain is amazing and promptimize uses langchain under the
+hood to interact with openai, and has integration with langchain
+(see `LangchainPromptCase`, and the upcoming `LangchainChainPromptCase`
+and `LangchainAgntPromptCase`)
+While you don't have to use
+langchain, and could use promptimize on top of any python prompt generation
+whether it'd be another library or some home grown thing.
+
+
+## Context
+
+<img src="https://user-images.githubusercontent.com/487433/230508578-456a7040-1184-433a-a555-dceb7c28c32c.png" width="75" title="Max"/>
+
+Where is `promptimize` coming from!? I'm (Maxime Beauchemin) a startup
+founder at <a href="www.preset.io">Preset</a> working on brining AI to BI
+(data exploration,
+and visualization). At Preset, we use `promptimize` to generate
+complex SQL based on natural language, and to suggest charts to users. We
+derive the `SimpleQuery` class to make it fitted to our specific use
+cases in our own prompt engineering repo. It's not my first open source project
+as the creator of
+[Apache Superset](https://github.com/apache/superset/) and
+[Apache Airflow](https://github.com/apache/airflow/)
+
+
+## Contribute
+
+This project is in its super early stages as of `0.2.0`, and contributions,
+contributors, and maintainers are highly encouraged. While it's a great time
+to onboard and influence the direction of the project, things are still
+evolving quickly. To get involved, open a GitHub issue
+or submit a pull request!
+
+## Links
+* [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/introducing-promptimize/)
+* [Preset Blog](https://preset.io/blog/)
+* [Promptimize DOCS](https://preset-io.github.io/promptimize/)
+
+
```

### Comparing `promptimize-0.2.2/README.md` & `promptimize-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 your prompts and evaluation functions in Python, allowing you to iterate
 quickly and with confidence.
 
 ## Hello world - the simplest prompt examples
 [more examples on GitHub](https://github.com/preset-io/promptimize/tree/main/examples)
 ```python
 # Brining some "prompt generator" classes - note that you can derive and extend those
-from promptimize.prompts import SimplePrompt
+from promptimize.prompts import PromptCase
 
 # Bringing some useful eval function that help evaluating and scoring responses
 # eval functions have a handle on the prompt object and are expected
 # to return a score between 0 and 1
 from promptimize import evals
 
 # Promptimize will scan the target folder and find all Prompt objects
```

### Comparing `promptimize-0.2.2/docs/Makefile` & `promptimize-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.2/docs/publish.sh` & `promptimize-0.2.3/docs/publish.sh`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.2/docs/source/README.md` & `promptimize-0.2.3/docs/source/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -144,18 +144,18 @@
 
 ```python
 ```
 ```bash
 # NOTE: CLI is `promptimize`, but `p9e` is a shorter synonym, can be used interchangibly
 
 # First let's run some of the examples
-p9e ./examples
+p9e run ./examples
 
 # Now the same but with verbose output
-p9e ./examples --verbose
+p9e run ./examples --verbose
 
 ```
 ## Langchain?
 
 How does promptimize relate to `langchain`?
 
 We think langchain is amazing and promptimize uses langchain under the
```

### Comparing `promptimize-0.2.2/docs/source/conf.py` & `promptimize-0.2.3/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,12 @@
 exclude_patterns: List = []
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "alabaster"
-html_logo = "https://user-images.githubusercontent.com/487433/229948453-36cbc2d1-e71f-4e87-9111-ab428bc96f4c.png"
+html_logo = (
+    "https://user-images.githubusercontent.com/"
+    "487433/229948453-36cbc2d1-e71f-4e87-9111-ab428bc96f4c.png"
+)
 html_static_path = ["_static"]
```

### Comparing `promptimize-0.2.2/examples/__pycache__/use_cases.cpython-38.pyc` & `promptimize-0.2.3/examples/__pycache__/use_cases.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.2/examples/readme_examples.py` & `promptimize-0.2.3/examples/readme_examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 
 # Generating a few SQL prompts
 sql_prompts = [
     SqlPrompt(
         # you can pass a unique key that can we used to reference a prompt
         key="sql-top-10-inc",
         # the user input that'll be added in place of {{ input }} in the template above
-        user_input="give me the top 10 countries with the highest net increase of population over the past 25 years?",
+        user_input=(
+            "give me the top 10 countries with the highest net increase "
+            "of population over the past 25 years?"
+        ),
         # the dialect template parameter, overriding the default set above
         dialect="BigQuery",
         # a simple validation function making sure the SQL starts with SELECT
         evaluators=lambda x: 1 if x.response.strip().startswith("SELECT") else 0,
     ),
 ]
```

### Comparing `promptimize-0.2.2/examples/readme_hello_world.py` & `promptimize-0.2.3/examples/readme_hello_world.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.2/promptimize/cli.py` & `promptimize-0.2.3/promptimize/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     help="limit how many prompt cases to run in a single batch",
 )
 @click.option(
     "--temperature",
     "-t",
     type=click.FLOAT,
     default=0.5,
-    help="max_tokens passed to the model",
+    help="the temperature passed to the model",
 )
 @click.option(
     "--engine",
     "-e",
     type=click.STRING,
     default="text-davinci-003",
     help="model as accepted by the openai API",
```

### Comparing `promptimize-0.2.2/promptimize/crawler.py` & `promptimize-0.2.3/promptimize/crawler.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.2/promptimize/evals.py` & `promptimize-0.2.3/promptimize/evals.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,7 +104,19 @@
     1
     >>> all_words("This is an Example string.", ["example", "test"], case_sensitive=True)
     0
     >>> all_words("This is an Example string.", ["example", "notfound"])
     0
     """
     return _common_word_search(response, words, case_sensitive, match_type="all")
+
+
+base_all = all
+base_any = any
+
+
+def all(iteratable):
+    return 1 if base_all([i == 1 for i in iteratable]) else 0
+
+
+def any(iteratable):
+    return 1 if base_any([i == 1 for i in iteratable]) else 0
```

### Comparing `promptimize-0.2.2/promptimize/prompt_cases.py` & `promptimize-0.2.3/promptimize/prompt_cases.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from typing import Any, Callable, List, Optional, Union
 
 from langchain.llms import OpenAI
+from langchain.callbacks import get_openai_callback
 
 from box import Box
 
 from promptimize import utils
 from promptimize.simple_jinja import process_template
 
 
@@ -67,15 +68,23 @@
     def get_prompt_executor(self):
         model_name = os.environ.get("OPENAI_MODEL") or "text-davinci-003"
         openai_api_key = os.environ.get("OPENAI_API_KEY")
         self.prompt_executor_kwargs = {"model_name": model_name}
         return OpenAI(model_name=model_name, openai_api_key=openai_api_key)
 
     def execute_prompt(self, prompt_str):
-        self.response = self.prompt_executor(prompt_str)
+        with get_openai_callback() as cb:
+            self.response = self.prompt_executor(prompt_str)
+        self.execution.openai = Box()
+        oai = self.execution.openai
+        oai.total_tokens = cb.total_tokens
+        oai.prompt_tokens = cb.prompt_tokens
+        oai.completion_tokens = cb.completion_tokens
+        oai.total_cost = cb.total_cost
+
         return self.response
 
     def pre_run(self):
         pass
 
     def post_run(self):
         pass
@@ -106,14 +115,16 @@
             "prompt_hash": self.prompt_hash,
             "prompt": self.prompt,
             "category": self.category,
             "response": self.response,
             "weight": self.weight,
             "execution": self.execution.to_dict(),
         }
+        if hasattr(self, "error"):
+            d["error"] = self.error
         return d
 
     def print(self, verbose=False, style="yaml"):
         style = style or "yaml"
         output = self.to_dict(verbose)
         if not verbose:
             for attr in self.verbose_attrs:
@@ -129,14 +140,15 @@
             result = evaluator(self)
             if not (utils.is_numeric(result) and 0 <= result <= 1):
                 raise Exception("Value should be between 0 and 1")
             test_results.append(result)
 
         if len(test_results):
             self.execution.score = sum(test_results) / len(test_results)
+            self.execution.results = test_results
         self.was_tested = True
 
     @property
     def prompt_hash(self):
         if self._prompt_hash:
             return self._prompt_hash
         return utils.short_hash(hash(self))
```

### Comparing `promptimize-0.2.2/promptimize/reports.py` & `promptimize-0.2.3/promptimize/reports.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.2/promptimize/suite.py` & `promptimize-0.2.3/promptimize/suite.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     Attributes:
         name (Optional[str]): The name of the suite.
         prompts (Dict[str, Prompt]): Dictionary of prompts to be tested,
             keyed by the prompt key.
         last_run_completion_create_kwargs (Dict[str, Any]): Keyword arguments
             used in the last run for completion creation.
+        efective_prompts (List): List of prompts values that finally will be tested.
     """
 
     def __init__(
         self,
         prompts: List["BasePromptCase"],
         name: Optional[str] = None,
     ) -> None:
@@ -43,14 +44,15 @@
         Args:
             prompts (List[Prompt]): List of prompts to be tested.
             name (Optional[str]): The name of the suite. Defaults to None.
         """
         self.name = name
         self.prompts = {o.key: o for o in prompts}
         self.last_run_completion_create_kwargs: dict = {}
+        self.effective_prompts = list(self.prompts.values())
 
     def execute(  # noqa
         self,
         verbose: bool = False,
         style: str = "yaml",
         silent: bool = False,
         report=None,
@@ -66,26 +68,22 @@
         Execute the suite with the given settings.
 
         Args:
             verbose (bool): If True, print verbose output. Defaults to False.
             style (str): Output style for serialization. Defaults to "yaml".
             silent (bool): If True, suppress output. Defaults to False.
         """
-        prompts = list(self.prompts.values())
-        if keys:
-            prompts = [p for p in prompts if p.key in keys]
-        if repair and report:
-            failed_keys = report.failed_keys
-            prompts = [p for p in prompts if p.key in failed_keys]
-
-        if shuffle:
-            random.shuffle(prompts)
-
-        if limit:
-            prompts = prompts[:limit]
+        self.reload_effective_prompts(
+            report=report,
+            keys=keys,
+            repair=repair,
+            shuffle=shuffle,
+            limit=limit,
+        )
+        prompts = self.effective_prompts
 
         for i, prompt in enumerate(prompts):
             should_run = force or self.should_prompt_execute(prompt, report)
             progress = f"({i+1}/{len(prompts)})"
             if not silent:
                 if should_run:
                     separated_section(f"# {progress} [RUN] prompt: {prompt.key}", fg="cyan")
@@ -121,14 +119,35 @@
                     break
 
         # `self.last_run_completion_create_kwargs = completion_create_kwargs
         if not silent:
             separated_section("# Suite summary", fg="cyan")
             click.echo(utils.serialize_object(self._serialize_run_summary(), style))
 
+    def reload_effective_prompts(
+        self,
+        report=None,
+        keys: list = None,
+        repair: bool = False,
+        shuffle: bool = False,
+        limit: int = 0,
+    ):
+        self.effective_prompts = list(self.prompts.values())
+        if keys:
+            self.effective_prompts = [p for p in self.effective_prompts if p.key in keys]
+        if repair and report:
+            failed_keys = report.failed_keys
+            self.effective_prompts = [p for p in self.effective_prompts if p.key in failed_keys]
+
+        if shuffle:
+            random.shuffle(self.effective_prompts)
+
+        if limit:
+            self.effective_prompts = self.effective_prompts[:limit]
+
     def should_prompt_execute(self, prompt, report):
         if not report or not report.prompts:
             return True
         report_prompt = report.prompts.get(prompt.key)
         if not report_prompt:
             return True
         else:
@@ -153,15 +172,15 @@
             Dict[str, Union[Optional[float], Dict[str, Any]]]: Serialized run summary of the suite.
         """
         prompts = self.prompts.values()
         tested = [p for p in prompts if p.was_tested and p.execution.score is not None]
         suite_score = None
         if len(tested) > 0:
             total_weight = sum([p.weight for p in tested])
-            suite_score = sum([p.execution.score for p in tested]) / total_weight
+            suite_score = sum([p.execution.score * p.weight for p in tested]) / total_weight
         d = {
             "suite_score": suite_score,
             "git_info": utils.get_git_info(),
         }
 
         return d
```

### Comparing `promptimize-0.2.2/promptimize/utils.py` & `promptimize-0.2.3/promptimize/utils.py`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.2/promptimize.egg-info/PKG-INFO` & `promptimize-0.2.3/promptimize.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,278 +1,281 @@
 Metadata-Version: 2.1
 Name: promptimize
-Version: 0.2.2
+Version: 0.2.3
 Summary: A python toolkit to generate and evaluate prompts for GPT at scale
 Home-page: UNKNOWN
 Author: Maxime Beauchemin
 Author-email: maximebeauchemin@gmail.com
 License: Apache License, Version 2.0
-Description: # 💡 ¡promptimize! 💡
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        [![PyPI version](https://badge.fury.io/py/promptimize.svg)](https://badge.fury.io/py/promptimize)
-        
-        <img src="https://user-images.githubusercontent.com/487433/229948453-36cbc2d1-e71f-4e87-9111-ab428bc96f4c.png" width=300/>
-        
-        Promptimize is a prompt engineering **evaluation** and **testing** toolkit.
-        
-        It accelerates and provides structure around prompt engineering at scale
-        with confidence, bringing some of the ideas behind test-driven
-        development (TDD) to engineering prompts.
-        
-        With promptimize, you can:
-        
-        - Define your "prompt cases" (think "test cases" but specific to evaluating
-          prompts) as code and associate them with evaluation functions
-        - Generate prompt variations dynamically
-        - Execute and rank prompts test suites across different
-          engines/models/temperature/settings and compare results, brining
-          the hyperparameter tuning mindset to prompt engineering
-        - Get reports on your prompts' performance as you iterate. Answer question
-          around how different prompt suites are performing against one-another.
-          Which individual cases or categories of cases improved? regressed?
-        - Minimize API calls! only re-assess what changed as you change it
-        - Perform human if and where needed, introspected failed cases, overriding
-          false negatives
-        
-        In essence, promptimize provides a programmatic way to execute and fine-tune
-        your prompts and evaluation functions in Python, allowing you to iterate
-        quickly and with confidence.
-        
-        ## Hello world - the simplest prompt examples
-        [more examples on GitHub](https://github.com/preset-io/promptimize/tree/main/examples)
-        ```python
-        # Brining some "prompt generator" classes - note that you can derive and extend those
-        from promptimize.prompts import SimplePrompt
-        
-        # Bringing some useful eval function that help evaluating and scoring responses
-        # eval functions have a handle on the prompt object and are expected
-        # to return a score between 0 and 1
-        from promptimize import evals
-        
-        # Promptimize will scan the target folder and find all Prompt objects
-        # and derivatives that are in the python modules
-        simple_prompts = [
-        
-            # Prompting "hello there" and making sure there's "hi" or "hello"
-            # somewhere in the answer
-            PromptCase("hello there!", lambda x: evals.any_word(x, ["hi", "hello"])),
-            PromptCase(
-                "name the top 50 guitar players!", lambda x: evals.all_words(x, ["frank zappa"])
-            ),
-        ]
-        ```
-        
-        ### The CLI's `run` command
-        ```
-        $ promptimize run --help
-        Usage: promptimize run [OPTIONS] PATH
-        
-          run some prompts
-        
-        Options:
-          -v, --verbose             Trigger more verbose output
-          -f, --force               Force run, do not skip
-          -h, --human               Human review, allowing a human to review and force
-                                    pass/fail each prompt case
-          -r, --repair              Only re-run previously failed
-          -x, --dry-run             DRY run, don't call the API
-          --shuffle                 Shuffle the prompts in a random order
-          -s, --style [json|yaml]   json or yaml formatting
-          -m, --max-tokens INTEGER  max_tokens passed to the model
-          -l, --limit INTEGER       limit how many prompt cases to run in a single
-                                    batch
-          -t, --temperature FLOAT   max_tokens passed to the model
-          -e, --engine TEXT         model as accepted by the openai API
-          -k, --key TEXT            The keys to run
-          -o, --output PATH
-          -s, --silent
-        ```
-        
-        Let's run those examples and produce a report `./report.yaml`
-        ```
-        $ promptimize run examples/ --output ./report.yaml
-        ```
-        
-        ```yaml
-        💡 ¡promptimize! 💡
-        # ----------------------------------------
-        # (1/2) [RUN] prompt: prompt-115868ef
-        # ----------------------------------------
-        key: prompt-115868ef
-        user_input: hello there!
-        prompt_hash: 115868ef
-        response: Hi there! How are you doing today?
-        execution:
-          api_call_duration_ms: 883.8047981262207
-          run_at: '2023-04-25T02:21:40.443077'
-          score: 1.0
-        
-        # ----------------------------------------
-        # (2/2) [RUN] prompt: prompt-5c085656
-        # ----------------------------------------
-        key: prompt-5c085656
-        user_input: name the top 10 guitar players!
-        prompt_hash: 5c085656
-        response: |-
-          1. Jimi Hendrix
-          2. Eric Clapton
-          {{ ... }}
-          11. Carlos Santana
-        weight: 2
-        execution:
-          api_call_duration_ms: 2558.135747909546
-          run_at: '2023-04-25T02:21:43.007529'
-          score: 0.0
-        
-        # ----------------------------------------
-        # Suite summary
-        # ----------------------------------------
-        suite_score: 0.3333333333333333
-        git_info:
-          sha: 2cf28498ba0f
-          branch: main
-          dirty: true
-        ```
-        
-        ## Problem + POV
-        
-        Thousands of product builders are currently trying to figure out how to
-        bring the power of AI into the products and experiences they are building.
-        The probabilistic (often semi-random, sometimes hectic) nature of LLMs
-        makes this a challenge.
-        
-        Prompt engineering is a huge piece of the puzzle in terms of how to do this
-        right, especially given the complexity, risks, and drawbacks around
-        model tuning.
-        
-        We believe product builders need to tame AI through proper, rigorous
-        **prompt engineering**. This allows making the probabilistic nature of
-        AI more deterministic, or somewhat predictable, and allows builders to apply
-        a hyperparameter tuning-type mindset and approach to prompt engineering.
-        
-        Any prompt-generator logic that's going to be let loose in the wild inside
-        a product should be thoroughly tested and evaluated with "prompt cases" that
-        cover the breath of what people may do in a product.
-        
-        In short, Promptimize allows you to test prompts at industrial scale,
-        so that you can confidently use them in the products you are building.
-        
-        ## Information Architecture
-        
-        - **Prompt:** A Prompt instance is a certain test case, a single prompt
-          with an associated set of evaluation functions to rate its success.
-        - **Evaluation:** An evaluation function that reads the response and returns
-          a success rate between `0` and `1`.
-        - **Suite:** A Suite is a collection of Prompt; it's able to run things,
-          accumulate results, and print reports about its collection of use cases.
-        - **Report**: a report is the compiled results of running a certain prompt
-          `Suite` or set of suites. Reports can be consumed, compared, and expanded.
-        
-        ## Principles
-        
-        - **Configuration as code:** All prompt cases, suites, and evaluations are
-          defined as code, which makes it easy to dynamically generate all sorts
-          of use cases and suites.
-        - **Expressive**: a clean DSL that's to-the-point -> user prompt + assertions.
-          the actually prompt creation logic lives in the derivative class of `PromptCase`,
-          so that we can have clean, dense files that contain nice `Suite`s
-        - **Support the iteration mindset:** making it easy for people to try things,
-          get suggestions from the AI, adapt, compare, and push forward
-        - **Extensibility:** the toolkit is designed to be extremely hackable and
-          extensible. Hooks, extensions, high API surface.
-        - **AI-powered:** the framework offers ways to expand your suites based
-          on the examples that exists. Use AI to generate more prompt cases!
-        
-        
-        ## Interesting features / facts
-        
-        Listing out a few features you should know about that you can start using as your
-        suites of prompts become larger / more complex
-        
-        * evaluation functions are assumed to return a value between 0 and 1.
-          contrarily to unit tests, prompt cases aren't boolean
-        * prompts can be assigned a `weight` (default 1) this enables you to define
-          which prompts are more important than others for reporting purposes and suite evaluation
-        * prompts can be assigned a `category`, this can be used in the reporting.
-          That helps understanding which categories are performing better than
-          others, or are most affected by iterations
-        * The `Prompt` class `pre_run` and `post_run` hooks if you want to do
-          post-processing for instance. An example of that would be if you do a prompt
-          that expects GPT to generate code, and you'd like actually say run that code
-          and test it. In our SQL implementation, we run the SQL against the database
-          for instance and get a pandas dataframe back, and allow doing assertions
-          on the dataframe itself
-        
-        
-        
-        ## Getting started
-        
-        To install the Promptimize package, use the following command:
-        ```bash
-        pip install promptimize
-        ```
-        
-        First you'll need an openai API key, let's set it as an env var
-        ```bash
-        export OPENAI_API_KEY=sk-{{ REDACTED }}
-        ```
-        
-        Find the examples executed below
-        [here](https://github.com/preset-io/promptimize/blob/main/examples/readme_examples.py)
-        
-        ```bash
-        # Clone the repo
-        git clone git@github.com:preset-io/promptimize.git
-        cd promptimize
-        
-        # NOTE: CLI is `promptimize`, but `p9e` is a shorter synonym, can be used interchangibly
-        # First let's run some of the examples
-        p9e run ./examples
-        
-        # Now the same but with verbose output
-        p9e run ./examples --verbose --output ./report.yaml
-        
-        ```
-        ## Langchain
-        
-        How does promptimize relate to `langchain`?
-        
-        We think langchain is amazing and promptimize uses langchain under the
-        hood to interact with openai, and has integration with langchain
-        (see `LangchainPromptCase`, and the upcoming `LangchainChainPromptCase`
-        and `LangchainAgntPromptCase`)
-        While you don't have to use
-        langchain, and could use promptimize on top of any python prompt generation
-        whether it'd be another library or some home grown thing.
-        
-        
-        ## Context
-        
-        <img src="https://user-images.githubusercontent.com/487433/230508578-456a7040-1184-433a-a555-dceb7c28c32c.png" width="75" title="Max"/>
-        
-        Where is `promptimize` coming from!? I'm (Maxime Beauchemin) a startup
-        founder at <a href="www.preset.io">Preset</a> working on brining AI to BI
-        (data exploration,
-        and visualization). At Preset, we use `promptimize` to generate
-        complex SQL based on natural language, and to suggest charts to users. We
-        derive the `SimpleQuery` class to make it fitted to our specific use
-        cases in our own prompt engineering repo. It's not my first open source project
-        as the creator of
-        [Apache Superset](https://github.com/apache/superset/) and
-        [Apache Airflow](https://github.com/apache/airflow/)
-        
-        
-        ## Contribute
-        
-        This project is in its super early stages as of `0.2.0`, and contributions,
-        contributors, and maintainers are highly encouraged. While it's a great time
-        to onboard and influence the direction of the project, things are still
-        evolving quickly. To get involved, open a GitHub issue
-        or submit a pull request!
-        
-        ## Links
-        * [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/introducing-promptimize/)
-        * [Preset Blog](https://preset.io/blog/)
-        * [Promptimize DOCS](https://preset-io.github.io/promptimize/)
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# 💡 ¡promptimize! 💡
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![PyPI version](https://badge.fury.io/py/promptimize.svg)](https://badge.fury.io/py/promptimize)
+
+<img src="https://user-images.githubusercontent.com/487433/229948453-36cbc2d1-e71f-4e87-9111-ab428bc96f4c.png" width=300/>
+
+Promptimize is a prompt engineering **evaluation** and **testing** toolkit.
+
+It accelerates and provides structure around prompt engineering at scale
+with confidence, bringing some of the ideas behind test-driven
+development (TDD) to engineering prompts.
+
+With promptimize, you can:
+
+- Define your "prompt cases" (think "test cases" but specific to evaluating
+  prompts) as code and associate them with evaluation functions
+- Generate prompt variations dynamically
+- Execute and rank prompts test suites across different
+  engines/models/temperature/settings and compare results, brining
+  the hyperparameter tuning mindset to prompt engineering
+- Get reports on your prompts' performance as you iterate. Answer question
+  around how different prompt suites are performing against one-another.
+  Which individual cases or categories of cases improved? regressed?
+- Minimize API calls! only re-assess what changed as you change it
+- Perform human if and where needed, introspected failed cases, overriding
+  false negatives
+
+In essence, promptimize provides a programmatic way to execute and fine-tune
+your prompts and evaluation functions in Python, allowing you to iterate
+quickly and with confidence.
+
+## Hello world - the simplest prompt examples
+[more examples on GitHub](https://github.com/preset-io/promptimize/tree/main/examples)
+```python
+# Brining some "prompt generator" classes - note that you can derive and extend those
+from promptimize.prompts import PromptCase
+
+# Bringing some useful eval function that help evaluating and scoring responses
+# eval functions have a handle on the prompt object and are expected
+# to return a score between 0 and 1
+from promptimize import evals
+
+# Promptimize will scan the target folder and find all Prompt objects
+# and derivatives that are in the python modules
+simple_prompts = [
+
+    # Prompting "hello there" and making sure there's "hi" or "hello"
+    # somewhere in the answer
+    PromptCase("hello there!", lambda x: evals.any_word(x, ["hi", "hello"])),
+    PromptCase(
+        "name the top 50 guitar players!", lambda x: evals.all_words(x, ["frank zappa"])
+    ),
+]
+```
+
+### The CLI's `run` command
+```
+$ promptimize run --help
+Usage: promptimize run [OPTIONS] PATH
+
+  run some prompts
+
+Options:
+  -v, --verbose             Trigger more verbose output
+  -f, --force               Force run, do not skip
+  -h, --human               Human review, allowing a human to review and force
+                            pass/fail each prompt case
+  -r, --repair              Only re-run previously failed
+  -x, --dry-run             DRY run, don't call the API
+  --shuffle                 Shuffle the prompts in a random order
+  -s, --style [json|yaml]   json or yaml formatting
+  -m, --max-tokens INTEGER  max_tokens passed to the model
+  -l, --limit INTEGER       limit how many prompt cases to run in a single
+                            batch
+  -t, --temperature FLOAT   max_tokens passed to the model
+  -e, --engine TEXT         model as accepted by the openai API
+  -k, --key TEXT            The keys to run
+  -o, --output PATH
+  -s, --silent
+```
+
+Let's run those examples and produce a report `./report.yaml`
+```
+$ promptimize run examples/ --output ./report.yaml
+```
+
+```yaml
+💡 ¡promptimize! 💡
+# ----------------------------------------
+# (1/2) [RUN] prompt: prompt-115868ef
+# ----------------------------------------
+key: prompt-115868ef
+user_input: hello there!
+prompt_hash: 115868ef
+response: Hi there! How are you doing today?
+execution:
+  api_call_duration_ms: 883.8047981262207
+  run_at: '2023-04-25T02:21:40.443077'
+  score: 1.0
+
+# ----------------------------------------
+# (2/2) [RUN] prompt: prompt-5c085656
+# ----------------------------------------
+key: prompt-5c085656
+user_input: name the top 10 guitar players!
+prompt_hash: 5c085656
+response: |-
+  1. Jimi Hendrix
+  2. Eric Clapton
+  {{ ... }}
+  11. Carlos Santana
+weight: 2
+execution:
+  api_call_duration_ms: 2558.135747909546
+  run_at: '2023-04-25T02:21:43.007529'
+  score: 0.0
+
+# ----------------------------------------
+# Suite summary
+# ----------------------------------------
+suite_score: 0.3333333333333333
+git_info:
+  sha: 2cf28498ba0f
+  branch: main
+  dirty: true
+```
+
+## Problem + POV
+
+Thousands of product builders are currently trying to figure out how to
+bring the power of AI into the products and experiences they are building.
+The probabilistic (often semi-random, sometimes hectic) nature of LLMs
+makes this a challenge.
+
+Prompt engineering is a huge piece of the puzzle in terms of how to do this
+right, especially given the complexity, risks, and drawbacks around
+model tuning.
+
+We believe product builders need to tame AI through proper, rigorous
+**prompt engineering**. This allows making the probabilistic nature of
+AI more deterministic, or somewhat predictable, and allows builders to apply
+a hyperparameter tuning-type mindset and approach to prompt engineering.
+
+Any prompt-generator logic that's going to be let loose in the wild inside
+a product should be thoroughly tested and evaluated with "prompt cases" that
+cover the breath of what people may do in a product.
+
+In short, Promptimize allows you to test prompts at industrial scale,
+so that you can confidently use them in the products you are building.
+
+## Information Architecture
+
+- **Prompt:** A Prompt instance is a certain test case, a single prompt
+  with an associated set of evaluation functions to rate its success.
+- **Evaluation:** An evaluation function that reads the response and returns
+  a success rate between `0` and `1`.
+- **Suite:** A Suite is a collection of Prompt; it's able to run things,
+  accumulate results, and print reports about its collection of use cases.
+- **Report**: a report is the compiled results of running a certain prompt
+  `Suite` or set of suites. Reports can be consumed, compared, and expanded.
+
+## Principles
+
+- **Configuration as code:** All prompt cases, suites, and evaluations are
+  defined as code, which makes it easy to dynamically generate all sorts
+  of use cases and suites.
+- **Expressive**: a clean DSL that's to-the-point -> user prompt + assertions.
+  the actually prompt creation logic lives in the derivative class of `PromptCase`,
+  so that we can have clean, dense files that contain nice `Suite`s
+- **Support the iteration mindset:** making it easy for people to try things,
+  get suggestions from the AI, adapt, compare, and push forward
+- **Extensibility:** the toolkit is designed to be extremely hackable and
+  extensible. Hooks, extensions, high API surface.
+- **AI-powered:** the framework offers ways to expand your suites based
+  on the examples that exists. Use AI to generate more prompt cases!
+
+
+## Interesting features / facts
+
+Listing out a few features you should know about that you can start using as your
+suites of prompts become larger / more complex
+
+* evaluation functions are assumed to return a value between 0 and 1.
+  contrarily to unit tests, prompt cases aren't boolean
+* prompts can be assigned a `weight` (default 1) this enables you to define
+  which prompts are more important than others for reporting purposes and suite evaluation
+* prompts can be assigned a `category`, this can be used in the reporting.
+  That helps understanding which categories are performing better than
+  others, or are most affected by iterations
+* The `Prompt` class `pre_run` and `post_run` hooks if you want to do
+  post-processing for instance. An example of that would be if you do a prompt
+  that expects GPT to generate code, and you'd like actually say run that code
+  and test it. In our SQL implementation, we run the SQL against the database
+  for instance and get a pandas dataframe back, and allow doing assertions
+  on the dataframe itself
+
+
+
+## Getting started
+
+To install the Promptimize package, use the following command:
+```bash
+pip install promptimize
+```
+
+First you'll need an openai API key, let's set it as an env var
+```bash
+export OPENAI_API_KEY=sk-{{ REDACTED }}
+```
+
+Find the examples executed below
+[here](https://github.com/preset-io/promptimize/blob/main/examples/readme_examples.py)
+
+```bash
+# Clone the repo
+git clone git@github.com:preset-io/promptimize.git
+cd promptimize
+
+# NOTE: CLI is `promptimize`, but `p9e` is a shorter synonym, can be used interchangibly
+# First let's run some of the examples
+p9e run ./examples
+
+# Now the same but with verbose output
+p9e run ./examples --verbose --output ./report.yaml
+
+```
+## Langchain
+
+How does promptimize relate to `langchain`?
+
+We think langchain is amazing and promptimize uses langchain under the
+hood to interact with openai, and has integration with langchain
+(see `LangchainPromptCase`, and the upcoming `LangchainChainPromptCase`
+and `LangchainAgntPromptCase`)
+While you don't have to use
+langchain, and could use promptimize on top of any python prompt generation
+whether it'd be another library or some home grown thing.
+
+
+## Context
+
+<img src="https://user-images.githubusercontent.com/487433/230508578-456a7040-1184-433a-a555-dceb7c28c32c.png" width="75" title="Max"/>
+
+Where is `promptimize` coming from!? I'm (Maxime Beauchemin) a startup
+founder at <a href="www.preset.io">Preset</a> working on brining AI to BI
+(data exploration,
+and visualization). At Preset, we use `promptimize` to generate
+complex SQL based on natural language, and to suggest charts to users. We
+derive the `SimpleQuery` class to make it fitted to our specific use
+cases in our own prompt engineering repo. It's not my first open source project
+as the creator of
+[Apache Superset](https://github.com/apache/superset/) and
+[Apache Airflow](https://github.com/apache/airflow/)
+
+
+## Contribute
+
+This project is in its super early stages as of `0.2.0`, and contributions,
+contributors, and maintainers are highly encouraged. While it's a great time
+to onboard and influence the direction of the project, things are still
+evolving quickly. To get involved, open a GitHub issue
+or submit a pull request!
+
+## Links
+* [Blog - Mastering AI-Powered Product Development: Introducing Promptimize for Test-Driven Prompt Engineering](https://preset.io/blog/introducing-promptimize/)
+* [Preset Blog](https://preset.io/blog/)
+* [Promptimize DOCS](https://preset-io.github.io/promptimize/)
+
+
```

### Comparing `promptimize-0.2.2/promptimize.egg-info/SOURCES.txt` & `promptimize-0.2.3/promptimize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptimize-0.2.2/setup.py` & `promptimize-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the contents of the README.md file
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="promptimize",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "promptimize=promptimize:cli",
             "p9e=promptimize:cli",
```

