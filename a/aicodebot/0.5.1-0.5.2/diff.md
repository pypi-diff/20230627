# Comparing `tmp/aicodebot-0.5.1.tar.gz` & `tmp/aicodebot-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.5.1.tar", last modified: Tue Jun 27 03:26:10 2023, max compression
+gzip compressed data, was "aicodebot-0.5.2.tar", last modified: Tue Jun 27 05:09:21 2023, max compression
```

## Comparing `aicodebot-0.5.1.tar` & `aicodebot-0.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:26:10.322542 aicodebot-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 03:25:46.000000 aicodebot-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-06-27 03:26:10.322542 aicodebot-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-06-27 03:25:46.000000 aicodebot-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:26:10.318541 aicodebot-0.5.1/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 03:25:46.000000 aicodebot-0.5.1/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 03:25:46.000000 aicodebot-0.5.1/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-06-27 03:25:46.000000 aicodebot-0.5.1/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-27 03:25:46.000000 aicodebot-0.5.1/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:26:10.318541 aicodebot-0.5.1/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 03:25:46.000000 aicodebot-0.5.1/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-27 03:25:46.000000 aicodebot-0.5.1/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-27 03:25:46.000000 aicodebot-0.5.1/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-27 03:25:46.000000 aicodebot-0.5.1/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-27 03:25:46.000000 aicodebot-0.5.1/aicodebot/prompts/fun_fact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-27 03:25:46.000000 aicodebot-0.5.1/aicodebot/prompts/review.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 03:26:10.318541 aicodebot-0.5.1/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-06-27 03:26:10.000000 aicodebot-0.5.1/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 03:26:10.000000 aicodebot-0.5.1/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 03:26:10.000000 aicodebot-0.5.1/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 03:26:10.000000 aicodebot-0.5.1/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 03:26:10.000000 aicodebot-0.5.1/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 03:26:10.000000 aicodebot-0.5.1/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-27 03:25:46.000000 aicodebot-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 03:26:10.322542 aicodebot-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-27 03:25:46.000000 aicodebot-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:21.727999 aicodebot-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 05:08:57.000000 aicodebot-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-27 05:09:21.727999 aicodebot-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-27 05:08:57.000000 aicodebot-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:21.727999 aicodebot-0.5.2/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:21.727999 aicodebot-0.5.2/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/fun_fact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-27 05:08:57.000000 aicodebot-0.5.2/aicodebot/prompts/review.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:09:21.727999 aicodebot-0.5.2/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 05:09:21.000000 aicodebot-0.5.2/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-27 05:08:57.000000 aicodebot-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:09:21.727999 aicodebot-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-27 05:08:57.000000 aicodebot-0.5.2/setup.py
```

### Comparing `aicodebot-0.5.1/LICENSE` & `aicodebot-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.1/PKG-INFO` & `aicodebot-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.5.1
+Version: 0.5.2
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
 ⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow.
 
-⚠️  It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+⚠️ It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
 
 We're working on it and it's getting better all the time.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the [Alignment](#alignment) section below for more on that.
 
@@ -106,15 +106,15 @@
 ## Development / Contributing
 
 ### The Stack
 
 #### Test and Build
 
 [![GitHub Build](https://github.com/novara-ai/aicodebot/actions/workflows/build.yml/badge.svg)](https://github.com/novara-ai/aicodebot/actions?query=build)
-[![CodeCov](https://codecov.io/gh/novara-ai/aicodebot/branch/main/graph/badge.svg)](https://codecov.io/gh/novara_ai/aicodebot)
+[![CodeCov](https://codecov.io/gh/novara-ai/aicodebot/branch/main/graph/badge.svg)](https://codecov.io/gh/novara-ai/aicodebot)
 [![Pytest](https://img.shields.io/badge/%F0%9F%A7%AA-Pytest-blue)](https://docs.pytest.org/en/stable/contents.html)
 
 #### Code Quality
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

### Comparing `aicodebot-0.5.1/README.md` & `aicodebot-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
 ⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow.
 
-⚠️  It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+⚠️ It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
 
 We're working on it and it's getting better all the time.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the [Alignment](#alignment) section below for more on that.
 
@@ -89,15 +89,15 @@
 ## Development / Contributing
 
 ### The Stack
 
 #### Test and Build
 
 [![GitHub Build](https://github.com/novara-ai/aicodebot/actions/workflows/build.yml/badge.svg)](https://github.com/novara-ai/aicodebot/actions?query=build)
-[![CodeCov](https://codecov.io/gh/novara-ai/aicodebot/branch/main/graph/badge.svg)](https://codecov.io/gh/novara_ai/aicodebot)
+[![CodeCov](https://codecov.io/gh/novara-ai/aicodebot/branch/main/graph/badge.svg)](https://codecov.io/gh/novara-ai/aicodebot)
 [![Pytest](https://img.shields.io/badge/%F0%9F%A7%AA-Pytest-blue)](https://docs.pytest.org/en/stable/contents.html)
 
 #### Code Quality
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

### Comparing `aicodebot-0.5.1/aicodebot/cli.py` & `aicodebot-0.5.2/aicodebot/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,103 +1,86 @@
 from aicodebot import version as aicodebot_version
 from aicodebot.helpers import exec_and_get_output, get_token_length, git_diff_context
 from dotenv import load_dotenv
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
-from langchain.llms import OpenAI
 from langchain.prompts import load_prompt
 from pathlib import Path
 from rich.console import Console
 from rich.style import Style
 import click, datetime, openai, os, random, subprocess, sys, tempfile, webbrowser
 
-console = Console()
-bot_style = Style(color="#30D5C8")
-DEFAULT_MAX_TOKENS = 1024
-
-
-def setup_environment():
-    # Load environment variables from the config file
-    config_file = Path(Path.home() / ".aicodebot")
-    load_dotenv(config_file)
-
-    if os.getenv("OPENAI_API_KEY"):
-        openai.api_key = os.getenv("OPENAI_API_KEY")
-        return True
-
-    openai_api_key_url = "https://platform.openai.com/account/api-keys"
-
-    console.print(
-        "[bold red]The OPENAI_API_KEY environment variable is not set.[/bold red]\n"
-        f"Let's fix that for you by creating a config file at {config_file}"
-    )
-
-    if click.confirm("Do you want me to open the OpenAI API keys page for you in a browser?"):
-        webbrowser.open(openai_api_key_url)
+# ----------------------------- Default settings ----------------------------- #
 
-    if click.confirm(f"Do you want me to create the {config_file} file for you?"):
-        api_key = click.prompt("Please enter your OpenAI API key")
+DEFAULT_MAX_TOKENS = 1024
+DEFAULT_TEMPERATURE = 0.1
+DEFAULT_MODEL = "gpt-3.5-turbo"  # Can't wait to use GPT-4, as the results are much better. On the waitlist.
+DEFAULT_SPINNER = "point"
 
-        # Copy .env.template to .env and insert the API key
-        template_file = Path(__file__).parent / ".aicodebot.template"
-        with Path.open(template_file, "r") as template, Path.open(config_file, "w") as env:
-            for line in template:
-                if line.startswith("OPENAI_API_KEY="):
-                    env.write(f"OPENAI_API_KEY={api_key}\n")
-                else:
-                    env.write(line)
+# ----------------------- Setup for rich console output ---------------------- #
+console = Console()
+bot_style = Style(color="#30D5C8")
 
-        console.print(f"[bold green]Created {config_file} with your OpenAI API key. You're all set![/bold green]")
-        sys.exit(0)
 
-    raise click.ClickException("Please set an API key in the OPENAI_API_KEY environment variable or in a .env file.")
+# -------------------------- Top level command group ------------------------- #
 
 
 @click.group()
 @click.version_option(aicodebot_version, "--version", "-V")
 @click.help_option("--help", "-h")
 def cli():
     pass
 
 
+# ---------------------------------------------------------------------------- #
+#                                   Commands                                   #
+# ---------------------------------------------------------------------------- #
+
+# Commands are defined as functions with the @click decorator.
+# The function name is the command name, and the docstring is the help text.
+# Keep the commands in alphabetical order.
+
+
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 def alignment(verbose):
     """Get a message about Heart-Centered AI Alignment ❤ + 🤖."""
     setup_environment()
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "alignment.yaml")
 
     # Set up the language model
-    llm = OpenAI(temperature=1, max_tokens=DEFAULT_MAX_TOKENS)
+    llm = ChatOpenAI(
+        model=DEFAULT_MODEL, temperature=DEFAULT_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose
+    )
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
-    with console.status("Thinking", spinner="point"):
+    with console.status("Generating an inspirational message", spinner=DEFAULT_SPINNER):
         response = chain.run({})
         console.print(response, style=bot_style)
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 @click.option("-t", "--response-token-size", type=int, default=250)
 @click.option("-y", "--yes", is_flag=True, default=False, help="Don't ask for confirmation before committing.")
 @click.option("--skip-pre-commit", is_flag=True, help="Skip running pre-commit (otherwise run it if it is found).")
 def commit(verbose, response_token_size, yes, skip_pre_commit):
-    """Generate a git commit message and commit changes after you approve."""
+    """Generate a commit message based on your changes."""
     setup_environment()
 
     # Check if pre-commit is installed and .pre-commit-config.yaml exists
     if not skip_pre_commit and Path(".pre-commit-config.yaml").exists():
         console.print("Running pre-commit checks...")
         result = subprocess.run(["pre-commit", "run", "--all-files"])
         if result.returncode != 0:
-            console.print("Pre-commit checks failed. Please fix the issues and try again.")
+            console.print("🛑 Pre-commit checks failed. Please fix the issues and try again.")
             return
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "commit_message.yaml")
 
     # Get the changes from git
     staged_files = exec_and_get_output(["git", "diff", "--name-only", "--cached"])
@@ -109,162 +92,206 @@
     else:
         # The list of files to be committed is the same as the list of staged files
         files = staged_files
 
     diff_context = git_diff_context()
 
     if not diff_context:
-        console.print("No changes to commit.")
+        console.print("No changes to commit. 🤷")
         sys.exit(0)
 
     # Check the size of the diff context and adjust accordingly
-    diff_context_token_size = get_token_length(diff_context)
+    prompt_token_size = get_token_length(diff_context) + get_token_length(prompt.template)
     if verbose:
-        console.print(f"Diff context token size: {diff_context_token_size}")
+        console.print(f"Diff context token size: {prompt_token_size}")
 
-    if diff_context_token_size + response_token_size > 16_000:
-        console.print("The diff context is too large to review. Bigger models coming soon.")
+    if prompt_token_size + response_token_size > 16_000:
+        # Bigger models coming soon
+        console.print("The diff context is too large to review. 😞")
         sys.exit(1)
-    elif diff_context_token_size + response_token_size > 4_000:
+    elif prompt_token_size + response_token_size > 4_000:
         model = "gpt-3.5-turbo-16k"  # supports 16k tokens but is a bit slower and more expensive
     else:
-        model = "gpt-3.5-turbo"  # supports 4k tokens
+        model = DEFAULT_MODEL  # gpt-3.5-turbo supports 4k tokens
 
     # Set up the language model
-    llm = ChatOpenAI(temperature=0.1, model=model, max_tokens=response_token_size)
+    llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose)
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
     console.print("The following files will be committed:\n" + files)
-    with console.status("Thinking", spinner="point"):
+    with console.status("Generating the commit message", spinner=DEFAULT_SPINNER):
         response = chain.run(diff_context)
 
     # Write the commit message to a temporary file
     with tempfile.NamedTemporaryFile(mode="w", delete=False) as temp:
         temp.write(str(response).strip())
         temp_file_name = temp.name
 
     # Open the temporary file in the user's editor
     editor = os.getenv("EDITOR", "vim")
     subprocess.call([editor, temp_file_name])  # noqa: S603
 
     # Ask the user if they want to commit the changes
-    if yes or click.confirm("Do you want to commit the changes?"):
+    if yes or click.confirm("Are you ready to commit the changes?"):
         # Commit the changes using the temporary file for the commit message
         exec_and_get_output(["git", "commit", "-F", temp_file_name])
         console.print(f"✅ {len(files.splitlines())} files committed.")
 
     # Delete the temporary file
     Path.unlink(temp_file_name)
 
 
 @cli.command(context_settings={"ignore_unknown_options": True})
 @click.argument("command", nargs=-1)
 @click.option("-v", "--verbose", count=True)
 def debug(command, verbose):
-    """Run a command and get debugging advice if it fails."""
+    """Run a command and debug the output."""
     setup_environment()
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "debug.yaml")
 
     # Set up the language model
-    llm = OpenAI(temperature=0.1, max_tokens=DEFAULT_MAX_TOKENS)
+    llm = ChatOpenAI(
+        model=DEFAULT_MODEL, temperature=DEFAULT_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose
+    )
 
     # Set up the chain
     chat_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
     command_str = " ".join(command)
 
     # Run the command and capture its output
-    console.print(f"Running:\n{command_str}")
+    console.print(f"Executing the command:\n{command_str}")
     process = subprocess.run(command_str, shell=True, capture_output=True, text=True)  # noqa: S602
 
     # Print the output of the command
     output = f"Standard Output:\n{process.stdout}\nStandard Error:\n{process.stderr}"
-    console.print(f"Output:\n{output}")
+    console.print(output)
 
     # Print a message about the exit status
     if process.returncode == 0:
         console.print("✅ The command completed successfully.")
     else:
         console.print(f"The command exited with status {process.returncode}.")
 
     # If the command failed, send its output to ChatGPT for analysis
     if process.returncode != 0:
         error_output = process.stderr
-        with console.status("Thinking", spinner="point"):
+        with console.status("Debugging", spinner=DEFAULT_SPINNER):
             response = chat_chain.run(error_output)
             console.print(response, style=bot_style)
         sys.exit(process.returncode)
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 def fun_fact(verbose):
-    """Tell me something interesting about programming or AI."""
+    """Get a fun fact about programming and artificial intelligence."""
     setup_environment()
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "fun_fact.yaml")
 
     # Set up the language model
-    llm = ChatOpenAI(temperature=1, max_tokens=DEFAULT_MAX_TOKENS)
+    llm = ChatOpenAI(model=DEFAULT_MODEL, temperature=0.9, max_tokens=250, verbose=verbose)
 
     # Set up the chain
     chat_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
-    with console.status("Thinking", spinner="point"):
+    with console.status("Fetching a fun fact", spinner=DEFAULT_SPINNER):
         # Select a random year so that we get a different answer each time
         year = random.randint(1942, datetime.datetime.utcnow().year)
         response = chat_chain.run(f"programming and artificial intelligence in the year {year}")
         console.print(response, style=bot_style)
 
 
 @cli.command
 @click.option("-c", "--commit", help="The commit hash to review.")
 @click.option("-v", "--verbose", count=True)
 def review(commit, verbose):
-    """Use AI to do a code review, with [un]staged changes, or a specified commit."""
+    """Do a code review, with [un]staged changes, or a specified commit."""
     setup_environment()
 
     diff_context = git_diff_context(commit)
     if not diff_context:
-        console.print("No changes to commit.")
+        console.print("No changes detected for review. 🤷")
         sys.exit(0)
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "review.yaml")
 
     # Check the size of the diff context and adjust accordingly
     response_token_size = DEFAULT_MAX_TOKENS / 2
-    diff_context_token_size = get_token_length(diff_context)
+    prompt_token_size = get_token_length(diff_context) + get_token_length(prompt.template)
     if verbose:
-        console.print(f"Diff context token size: {diff_context_token_size}")
+        console.print(f"Prompt token size: {prompt_token_size}")
 
-    if diff_context_token_size + response_token_size > 16_000:
-        console.print("The diff context is too large to review. Bigger models coming soon.")
+    if prompt_token_size + response_token_size > 16_000:
+        # Bigger models coming soon
+        console.print("The diff context is too large to review. 😞")
         sys.exit(1)
-    elif diff_context_token_size + response_token_size > 4_000:
+    elif prompt_token_size + response_token_size > 4_000:
         model = "gpt-3.5-turbo-16k"  # supports 16k tokens but is a bit slower and more expensive
     else:
-        model = "gpt-3.5-turbo"  # supports 4k tokens
+        model = DEFAULT_MODEL  # gpt-3.5-turbo supports 4k tokens
 
     # Set up the language model
-    llm = ChatOpenAI(temperature=0.1, model=model, max_tokens=response_token_size)
+    llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose)
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
-    with console.status("Reviewing", spinner="point"):
+    with console.status("Reviewing code", spinner=DEFAULT_SPINNER):
         response = chain.run(diff_context)
         console.print(response, style=bot_style)
 
 
-@cli.command()
-def version():
-    """Print the version number."""
-    console.print(f"AICodeBot version {aicodebot_version}")
+# ------------------------------- End Commands ------------------------------- #
+
+
+def setup_environment():
+    # Load environment variables from the config file
+    config_file = Path(Path.home() / ".aicodebot")
+    load_dotenv(config_file)
+
+    if os.getenv("OPENAI_API_KEY"):
+        openai.api_key = os.getenv("OPENAI_API_KEY")
+        return True
+
+    openai_api_key_url = "https://platform.openai.com/account/api-keys"
+
+    console.print(
+        "[bold red]The OPENAI_API_KEY environment variable is not set.[/bold red]\n"
+        f"The OpenAI API key is required to use aicodebot. You can get one for free on the OpenAI website.\n"
+        f"Let's create a config file for you at {config_file}"
+    )
+
+    if click.confirm("Open the OpenAI API keys page for you in a browser?"):
+        webbrowser.open(openai_api_key_url)
+
+    if click.confirm(f"Create the {config_file} file for you?"):
+        api_key = click.prompt("Please enter your OpenAI API key")
+
+        # Copy .env.template to .env and insert the API key
+        template_file = Path(__file__).parent / ".aicodebot.template"
+        with Path.open(template_file, "r") as template, Path.open(config_file, "w") as env:
+            for line in template:
+                if line.startswith("OPENAI_API_KEY="):
+                    env.write(f"OPENAI_API_KEY={api_key}\n")
+                else:
+                    env.write(line)
+
+        console.print(
+            f"[bold green]Created {config_file} with your OpenAI API key.[/bold green] "
+            "Now, please re-run aicodebot and let's get started!"
+        )
+        sys.exit(0)
+
+    raise click.ClickException(
+        "🛑 Please set an API key in the OPENAI_API_KEY environment variable or in a .aicodebot file."
+    )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `aicodebot-0.5.1/aicodebot/helpers.py` & `aicodebot-0.5.2/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.1/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.5.2/aicodebot/prompts/commit_message.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# LLM Prompt for the commit command prompts the AI to generate a commit message for the supplied diff context
 _type: prompt
 template_format: f-string
 input_variables: ["diff_context"]
 template: |
     You are an expert software engineer. I need you to generate a commit message for a change in a git repository.
     Here's the diff context:
```

### Comparing `aicodebot-0.5.1/aicodebot/prompts/review.yaml` & `aicodebot-0.5.2/aicodebot/prompts/review.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,31 @@
+# LLM Prompt for the review command that prompts the AI to do a code review for the supplied diff context
 _type: prompt
 template_format: f-string
 input_variables: ["diff_context"]
 template: |
-    You are an expert code reviewer.
+    You are an expert code reviewer, and I want you to review a change in a git repository.
+
     You know how to give constructive feedback.
-    You know how to give feedback that is actionable.
-    You know how to give feedback that is kind.
-    You know how to give feedback that is specific.
+    You know how to give feedback that is actionable, kind, and specific
     Contextually appropriate emojis are encouraged, but not required.
 
     DO NOT give comments that discuss formatting, as those will be handled with pre-commit with the black and isort hooks.
     DO NOT respond with line numbers, use function names or file names instead (you're going to be wrong about the line numbers anyway).
 
-    Review this code change.  The relevant diff context is as follows, between the BEGIN DIFF and END DIFF markers:
+    Here's the diff context:
 
     BEGIN DIFF
     {diff_context}
     END DIFF
 
-    The main focus is to tell the author how they could make the code better.
+    Remember:
+    - Lines starting with "-" are being removed.
+    - Lines starting with "+" are being added.
+    - Lines starting with " " are unchanged.
+
+    Consider the file names for context (e.g., "README.md" is a markdown file, "*.py" is a Python file).
+    Understand the difference between code and comments. Comment lines start with ##, #, or //.
+
+    The main focus is to tell me how I could make the code better.
 
     If the changes look good overall and don't require any feedback, then just respond with "LGTM" (looks good to me).
```

### Comparing `aicodebot-0.5.1/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.5.2/aicodebot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.5.1
+Version: 0.5.2
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
 ⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow.
 
-⚠️  It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+⚠️ It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
 
 We're working on it and it's getting better all the time.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the [Alignment](#alignment) section below for more on that.
 
@@ -106,15 +106,15 @@
 ## Development / Contributing
 
 ### The Stack
 
 #### Test and Build
 
 [![GitHub Build](https://github.com/novara-ai/aicodebot/actions/workflows/build.yml/badge.svg)](https://github.com/novara-ai/aicodebot/actions?query=build)
-[![CodeCov](https://codecov.io/gh/novara-ai/aicodebot/branch/main/graph/badge.svg)](https://codecov.io/gh/novara_ai/aicodebot)
+[![CodeCov](https://codecov.io/gh/novara-ai/aicodebot/branch/main/graph/badge.svg)](https://codecov.io/gh/novara-ai/aicodebot)
 [![Pytest](https://img.shields.io/badge/%F0%9F%A7%AA-Pytest-blue)](https://docs.pytest.org/en/stable/contents.html)
 
 #### Code Quality
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

### Comparing `aicodebot-0.5.1/aicodebot.egg-info/SOURCES.txt` & `aicodebot-0.5.2/aicodebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.1/pyproject.toml` & `aicodebot-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.1/setup.py` & `aicodebot-0.5.2/setup.py`

 * *Files identical despite different names*

