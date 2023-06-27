# Comparing `tmp/aicodebot-0.5.3.tar.gz` & `tmp/aicodebot-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.5.3.tar", last modified: Tue Jun 27 05:35:57 2023, max compression
+gzip compressed data, was "aicodebot-0.5.4.tar", last modified: Tue Jun 27 15:13:26 2023, max compression
```

## Comparing `aicodebot-0.5.3.tar` & `aicodebot-0.5.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:35:57.833034 aicodebot-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 05:35:35.000000 aicodebot-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-27 05:35:57.833034 aicodebot-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-06-27 05:35:35.000000 aicodebot-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:35:57.833034 aicodebot-0.5.3/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:35:57.833034 aicodebot-0.5.3/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/fun_fact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-27 05:35:35.000000 aicodebot-0.5.3/aicodebot/prompts/review.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 05:35:57.833034 aicodebot-0.5.3/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 05:35:57.000000 aicodebot-0.5.3/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-27 05:35:35.000000 aicodebot-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 05:35:57.833034 aicodebot-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-27 05:35:35.000000 aicodebot-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:26.957495 aicodebot-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 15:13:04.000000 aicodebot-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-06-27 15:13:26.957495 aicodebot-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-27 15:13:04.000000 aicodebot-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:26.957495 aicodebot-0.5.4/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 15:13:04.000000 aicodebot-0.5.4/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-27 15:13:04.000000 aicodebot-0.5.4/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-06-27 15:13:04.000000 aicodebot-0.5.4/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-27 15:13:04.000000 aicodebot-0.5.4/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:26.957495 aicodebot-0.5.4/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:04.000000 aicodebot-0.5.4/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 15:13:04.000000 aicodebot-0.5.4/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-27 15:13:04.000000 aicodebot-0.5.4/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-27 15:13:04.000000 aicodebot-0.5.4/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-27 15:13:04.000000 aicodebot-0.5.4/aicodebot/prompts/fun_fact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-27 15:13:04.000000 aicodebot-0.5.4/aicodebot/prompts/review.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:26.957495 aicodebot-0.5.4/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-06-27 15:13:26.000000 aicodebot-0.5.4/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 15:13:26.000000 aicodebot-0.5.4/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:13:26.000000 aicodebot-0.5.4/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 15:13:26.000000 aicodebot-0.5.4/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 15:13:26.000000 aicodebot-0.5.4/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 15:13:26.000000 aicodebot-0.5.4/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-27 15:13:04.000000 aicodebot-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:13:26.957495 aicodebot-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-27 15:13:04.000000 aicodebot-0.5.4/setup.py
```

### Comparing `aicodebot-0.5.3/LICENSE` & `aicodebot-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.3/PKG-INFO` & `aicodebot-0.5.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.5.3
+Version: 0.5.4
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -17,25 +17,27 @@
 
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
-⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow.
+There are lot of ways to use AICodeBot that we have planned. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-⚠️ It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features. ⬇
 
-We're working on it and it's getting better all the time.
+⚠️ It uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+
+We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](CONTRIBUTING.md) for more.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
-It's also not a "build a website for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, it's built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
+It's also not a "build a website for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it
 
 ### AI-Assisted Git Commit
 
 `aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. It will also commit the changes for you once everything checks out.
 
@@ -47,63 +49,80 @@
 
 `aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It also suggests best practices for code improvement.
 
 ## Getting Started
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
 
-To install the command line interface, run `pip install aicodebot`. You'll also need to set up an OpenAI API key, which you can get for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
-
-Follow the steps below to set up AICodeBot on your machine:
+To install AICodeBot, run:
 
 `pip install aicodebot`
 
-Note:
+And then run `aicodebot --help` to get started.
+
+```bash
+Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  -V, --version  Show the version and exit.
+  -h, --help     Show this message and exit.
+
+Commands:
+  alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
+  commit     Generate a commit message based on your changes.
+  debug      Run a command and debug the output.
+  fun-fact   Get a fun fact about programming and artificial intelligence.
+  review     Do a code review, with [un]staged changes, or a specified...
+  ```
+
+### Open AI key setup
+
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
+Pro tip: You can also set the `OPENAI_API_KEY` environment variable to your API key, and it will use that instead of prompting you.
+
 ## Roadmap of Upcoming Features
 
 ### Code Workflow Improvements
 
-- [X] **Assisted Git Commit**: Automatically generate a commit message.
+- [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
 - [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
-- [X] **Code Review**: Provides feedback on potential issues in cod, such as style violations, potential bugs, and performance issues. It could also suggest best practices for code improvement. Eventually: FIX the code automatically and notify the team.
-- [ ] **Fix the Build**: Check the CI/CD pipeline, figure out what is broken, and fix the build.
+- [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
 - [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
 - [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 - [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
-- [ ] **Error Detection**: Detects errors in code and suggests potential fixes.
 - [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
-- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions)
+- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
 - [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repo.
-- [ ] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
-- [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to @aicodebot
+- [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
+- [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
 
 ### User Interfaces
 
 - [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
+- [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate gif.
 - [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
 - [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
 - [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
 - [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository Management
 
 - [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
 - [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
 - [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
 - [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
 
 ### Fun
 
-- [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming.
-- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity.
-- [ ] **Telling Jokes**: Tells programming jokes. :smiley:
+- [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
+- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
+- [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
 - [ ] **Supportive Encouragement**: High fives and kudos for a job well done
-- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs. We've gotta figure out how to teach LLMs about humor.
+- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Development / Contributing
 
 ### The Stack
 
@@ -128,56 +147,8 @@
 
 ## Alignment ❤️ + 🤖
 
 Technology itself is amoral, it just imbues the values of the engineers who create it. We believe that AI should be built in a way that aligns with humanity, and we're building aicodebot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
 
 ## Contributing
 
-We'd love your help! If you're interested in contributing, here's how to get started.
-
-1. Clone the repository
-
-```bash
-git clone git@github.com:novara-ai/aicodebot.git
-```
-
-2. Set up a virtual environment (I recommend using [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/))
-
-```bash
-mkvirtualenv --python=`which python3` aicodebot
-```
-
-3. Install the dependencies:
-
-```bash
-pip install -r requirements/requirements-dev.txt
-```
-
-4. Use aicodebot to build aicodebot 😎
-
-### Testing
-
-Install the test dependencies with
-`pip install -r requirements/requirements-test.txt`
-
-We use `pytest` for testing. It will skip some tests if OPENAI_API_KEY is not set.
-
-### Coding Principles
-
-Borrowed from the [zen of python](http://c2.com/cgi/wiki?PythonPhilosophy), with a couple of changes.
-
-```text
-1. **Readability is the number 1 code quality metric**.
-2. Beautiful is better than ugly.
-3. Explicit is better than implicit.
-4. Simple is better than complex.
-5. Complex is better than complicated.
-6. Flat is better than nested.
-7. Sparse is better than dense.
-8. Special cases aren't special enough to break the rules.
-    * Although practicality beats purity.
-9. Errors should never pass silently.
-    * Unless explicitly silenced.
-10. In the face of ambiguity, refuse the temptation to guess.
-11. There should be one -- and preferably only one -- obvious way to do it.
-12. Now is better than never.
-```
+We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING.md](CONTRIBUTING.md) for more details.
```

### Comparing `aicodebot-0.5.3/README.md` & `aicodebot-0.5.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
-⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow.
+There are lot of ways to use AICodeBot that we have planned. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-⚠️ It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features. ⬇
 
-We're working on it and it's getting better all the time.
+⚠️ It uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+
+We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](CONTRIBUTING.md) for more.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
-It's also not a "build a website for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, it's built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
+It's also not a "build a website for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it
 
 ### AI-Assisted Git Commit
 
 `aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. It will also commit the changes for you once everything checks out.
 
@@ -30,63 +32,80 @@
 
 `aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It also suggests best practices for code improvement.
 
 ## Getting Started
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
 
-To install the command line interface, run `pip install aicodebot`. You'll also need to set up an OpenAI API key, which you can get for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
-
-Follow the steps below to set up AICodeBot on your machine:
+To install AICodeBot, run:
 
 `pip install aicodebot`
 
-Note:
+And then run `aicodebot --help` to get started.
+
+```bash
+Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  -V, --version  Show the version and exit.
+  -h, --help     Show this message and exit.
+
+Commands:
+  alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
+  commit     Generate a commit message based on your changes.
+  debug      Run a command and debug the output.
+  fun-fact   Get a fun fact about programming and artificial intelligence.
+  review     Do a code review, with [un]staged changes, or a specified...
+  ```
+
+### Open AI key setup
+
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
+Pro tip: You can also set the `OPENAI_API_KEY` environment variable to your API key, and it will use that instead of prompting you.
+
 ## Roadmap of Upcoming Features
 
 ### Code Workflow Improvements
 
-- [X] **Assisted Git Commit**: Automatically generate a commit message.
+- [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
 - [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
-- [X] **Code Review**: Provides feedback on potential issues in cod, such as style violations, potential bugs, and performance issues. It could also suggest best practices for code improvement. Eventually: FIX the code automatically and notify the team.
-- [ ] **Fix the Build**: Check the CI/CD pipeline, figure out what is broken, and fix the build.
+- [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
 - [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
 - [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 - [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
-- [ ] **Error Detection**: Detects errors in code and suggests potential fixes.
 - [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
-- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions)
+- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
 - [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repo.
-- [ ] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
-- [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to @aicodebot
+- [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
+- [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
 
 ### User Interfaces
 
 - [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
+- [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate gif.
 - [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
 - [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
 - [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
 - [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository Management
 
 - [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
 - [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
 - [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
 - [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
 
 ### Fun
 
-- [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming.
-- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity.
-- [ ] **Telling Jokes**: Tells programming jokes. :smiley:
+- [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
+- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
+- [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
 - [ ] **Supportive Encouragement**: High fives and kudos for a job well done
-- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs. We've gotta figure out how to teach LLMs about humor.
+- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Development / Contributing
 
 ### The Stack
 
@@ -111,56 +130,8 @@
 
 ## Alignment ❤️ + 🤖
 
 Technology itself is amoral, it just imbues the values of the engineers who create it. We believe that AI should be built in a way that aligns with humanity, and we're building aicodebot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
 
 ## Contributing
 
-We'd love your help! If you're interested in contributing, here's how to get started.
-
-1. Clone the repository
-
-```bash
-git clone git@github.com:novara-ai/aicodebot.git
-```
-
-2. Set up a virtual environment (I recommend using [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/))
-
-```bash
-mkvirtualenv --python=`which python3` aicodebot
-```
-
-3. Install the dependencies:
-
-```bash
-pip install -r requirements/requirements-dev.txt
-```
-
-4. Use aicodebot to build aicodebot 😎
-
-### Testing
-
-Install the test dependencies with
-`pip install -r requirements/requirements-test.txt`
-
-We use `pytest` for testing. It will skip some tests if OPENAI_API_KEY is not set.
-
-### Coding Principles
-
-Borrowed from the [zen of python](http://c2.com/cgi/wiki?PythonPhilosophy), with a couple of changes.
-
-```text
-1. **Readability is the number 1 code quality metric**.
-2. Beautiful is better than ugly.
-3. Explicit is better than implicit.
-4. Simple is better than complex.
-5. Complex is better than complicated.
-6. Flat is better than nested.
-7. Sparse is better than dense.
-8. Special cases aren't special enough to break the rules.
-    * Although practicality beats purity.
-9. Errors should never pass silently.
-    * Unless explicitly silenced.
-10. In the face of ambiguity, refuse the temptation to guess.
-11. There should be one -- and preferably only one -- obvious way to do it.
-12. Now is better than never.
-```
+We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING.md](CONTRIBUTING.md) for more details.
```

### Comparing `aicodebot-0.5.3/aicodebot/cli.py` & `aicodebot-0.5.4/aicodebot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     if verbose:
         console.print(f"Diff context token size: {prompt_token_size}")
 
     if prompt_token_size + response_token_size > 16_000:
         # Bigger models coming soon
         console.print("The diff context is too large to review. 😞")
         sys.exit(1)
-    elif prompt_token_size + response_token_size > 4_000:
+    elif prompt_token_size + response_token_size > 3_500:  # It's actually 4k, but we want a buffer
         model = "gpt-3.5-turbo-16k"  # supports 16k tokens but is a bit slower and more expensive
     else:
         model = DEFAULT_MODEL  # gpt-3.5-turbo supports 4k tokens
 
     # Set up the language model
     llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose)
 
@@ -227,15 +227,15 @@
     if verbose:
         console.print(f"Prompt token size: {prompt_token_size}")
 
     if prompt_token_size + response_token_size > 16_000:
         # Bigger models coming soon
         console.print("The diff context is too large to review. 😞")
         sys.exit(1)
-    elif prompt_token_size + response_token_size > 4_000:
+    elif prompt_token_size + response_token_size > 3_500:  # It's actually 4k, but we want a buffer
         model = "gpt-3.5-turbo-16k"  # supports 16k tokens but is a bit slower and more expensive
     else:
         model = DEFAULT_MODEL  # gpt-3.5-turbo supports 4k tokens
 
     # Set up the language model
     llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose)
```

### Comparing `aicodebot-0.5.3/aicodebot/helpers.py` & `aicodebot-0.5.4/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.3/aicodebot/prompts/alignment.yaml` & `aicodebot-0.5.4/aicodebot/prompts/alignment.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.3/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.5.4/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.3/aicodebot/prompts/review.yaml` & `aicodebot-0.5.4/aicodebot/prompts/review.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.3/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.5.4/aicodebot.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.5.3
+Version: 0.5.4
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -17,25 +17,27 @@
 
 # AI Code Bot 🤖
 
 ## Your AI-powered coding companion
 
 AICodeBot is a coding assistant designed to make your coding life easier. With capabilities to perform code reviews, manage dependencies, and even suggest improvements, think of it as your AI version of a pair programmer - a team member that accelerates the pace of development and helps you write better code.
 
-⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow.
+There are lot of ways to use AICodeBot that we have planned. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/) that you can use to generate commit messages, debug code, and review code. In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-⚠️ It uses OpenAI's ChatGPT large language model, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+⚠️ Status: This project is in its infancy with very limited features, but it already improves the software development workflow, and has a healthy Roadmap of features. ⬇
 
-We're working on it and it's getting better all the time.
+⚠️ It uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes it does dumb things, which is why we have you confirm before it does anything permanent.
+
+We're using AICodeBot to build AICodeBot, and it's getting better all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](CONTRIBUTING.md) for more.
 
 ### What it's not
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
-It's also not a "build a website for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, it's built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
+It's also not a "build a website for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that, Instead, AICodeBot is built to work with existing code bases and help you improve them at the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it
 
 ### AI-Assisted Git Commit
 
 `aicodebot commit` will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. It will also commit the changes for you once everything checks out.
 
@@ -47,63 +49,80 @@
 
 `aicodebot review` will run a code review on your code and suggest improvements. By default it will look at [un]staged changes, and you can also supply a specific commit hash to review. It also suggests best practices for code improvement.
 
 ## Getting Started
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
 
-To install the command line interface, run `pip install aicodebot`. You'll also need to set up an OpenAI API key, which you can get for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
-
-Follow the steps below to set up AICodeBot on your machine:
+To install AICodeBot, run:
 
 `pip install aicodebot`
 
-Note:
+And then run `aicodebot --help` to get started.
+
+```bash
+Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  -V, --version  Show the version and exit.
+  -h, --help     Show this message and exit.
+
+Commands:
+  alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
+  commit     Generate a commit message based on your changes.
+  debug      Run a command and debug the output.
+  fun-fact   Get a fun fact about programming and artificial intelligence.
+  review     Do a code review, with [un]staged changes, or a specified...
+  ```
+
+### Open AI key setup
+
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
+Pro tip: You can also set the `OPENAI_API_KEY` environment variable to your API key, and it will use that instead of prompting you.
+
 ## Roadmap of Upcoming Features
 
 ### Code Workflow Improvements
 
-- [X] **Assisted Git Commit**: Automatically generate a commit message.
+- [X] **Assisted Git Commit**: Automatically generate a commit message based on the changes you've made
 - [X] **Assisted Debugging**: Run a command with aicodebot and it captures the log message and tries to figure out what's going on from the error message.  Eventually, it could also suggest fixes for the error and make the changes for you. Try it out with `aicodebot debug $command`
-- [X] **Code Review**: Provides feedback on potential issues in cod, such as style violations, potential bugs, and performance issues. It could also suggest best practices for code improvement. Eventually: FIX the code automatically and notify the team.
-- [ ] **Fix the Build**: Check the CI/CD pipeline, figure out what is broken, and fix the build.
+- [X] **Code Review**: Provides feedback on potential issues in code,  and suggests improvements to make it better.
 - [ ] **Dependency Management**: Updating dependencies to their latest versions with pull requests that run tests.
 - [ ] **Documentation Generation**: Generates comprehensive documentation for code, including docstrings, README files, and wiki pages.
 - [ ] **Performance Optimization Suggestions**: Suggests potential performance optimizations for code.
-- [ ] **Error Detection**: Detects errors in code and suggests potential fixes.
 - [ ] **Test Generation**: Generates unit tests for code, improve test coverage.
-- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions)
+- [ ] **Integration with CI/CD pipelines**: Integrates with CI/CD pipelines to automate tasks like code review, testing, and deployment (via GitHub Actions). Eventually: Fix the build automatically when there are small errors.
 - [ ] **Rubber Ducky Chat Bot**: Helps developers think through design issues by providing a conversational interface to discuss and solve problems, using data from the current repo.
-- [ ] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
-- [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to @aicodebot
+- [X] **Linting/Formatting**: Checks code for linting errors and automatically fixes them where possible (via pre-commit)
+- [ ] **Handle GitHub Issues**: Handles basic tasks that you assign to [@aicodebot](https://pypi.org/project/aicodebot/)
 
 ### User Interfaces
 
 - [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
+- [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate gif.
 - [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories.
 - [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
 - [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
 - [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository Management
 
 - [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
 - [ ] **Handle Stale Issues**: Automatically detects and handles stale issues on GitHub by nudging the responsible parties.
 - [ ] **Triage Incoming Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary.
 - [ ] **Rate the complexity of PRs**: Rates the complexity of pull requests and assigns them to developers based on their skill level and context
 
 ### Fun
 
-- [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming.
-- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity.
-- [ ] **Telling Jokes**: Tells programming jokes. :smiley:
+- [X] **Fun Facts**: Provides fun facts about programming or AI. It could also share interesting news or articles related to AI and programming. Try it out with `aicodebot fun-fact`.
+- [X] **Alignment**: Gives a heart-centered inspirational message about how we can build AI in a way that aligns with humanity. Try it out with `aicodebot alignment`.
+- [ ] **Telling Jokes**: We've gotta figure out how to teach LLMs about humor. :)
 - [ ] **Supportive Encouragement**: High fives and kudos for a job well done
-- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs. We've gotta figure out how to teach LLMs about humor.
+- [ ] **GIF Reactions**: Reacts to messages with relevant and fun gifs.
 
 <img src="https://camo.githubusercontent.com/6fc1e79b4aa226b24a756c4c8e20e5b049301a930449a7321d3e45f516e61601/68747470733a2f2f74656e6f722e636f6d2f766965772f6b746f2d6b6f756e6f746f72692d6b6f756e6f746f7269746f6b656e2d6c626f772d73746f726b686f6c646572732d6769662d32353637363438332e676966" width="25%">
 
 ## Development / Contributing
 
 ### The Stack
 
@@ -128,56 +147,8 @@
 
 ## Alignment ❤️ + 🤖
 
 Technology itself is amoral, it just imbues the values of the engineers who create it. We believe that AI should be built in a way that aligns with humanity, and we're building aicodebot to help us do just that. We're building from a heart-centered space, and contributing to the healthy intersection of AI and humanity.
 
 ## Contributing
 
-We'd love your help! If you're interested in contributing, here's how to get started.
-
-1. Clone the repository
-
-```bash
-git clone git@github.com:novara-ai/aicodebot.git
-```
-
-2. Set up a virtual environment (I recommend using [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/))
-
-```bash
-mkvirtualenv --python=`which python3` aicodebot
-```
-
-3. Install the dependencies:
-
-```bash
-pip install -r requirements/requirements-dev.txt
-```
-
-4. Use aicodebot to build aicodebot 😎
-
-### Testing
-
-Install the test dependencies with
-`pip install -r requirements/requirements-test.txt`
-
-We use `pytest` for testing. It will skip some tests if OPENAI_API_KEY is not set.
-
-### Coding Principles
-
-Borrowed from the [zen of python](http://c2.com/cgi/wiki?PythonPhilosophy), with a couple of changes.
-
-```text
-1. **Readability is the number 1 code quality metric**.
-2. Beautiful is better than ugly.
-3. Explicit is better than implicit.
-4. Simple is better than complex.
-5. Complex is better than complicated.
-6. Flat is better than nested.
-7. Sparse is better than dense.
-8. Special cases aren't special enough to break the rules.
-    * Although practicality beats purity.
-9. Errors should never pass silently.
-    * Unless explicitly silenced.
-10. In the face of ambiguity, refuse the temptation to guess.
-11. There should be one -- and preferably only one -- obvious way to do it.
-12. Now is better than never.
-```
+We'd love your help! If you're interested in contributing, here's how to get started. See [CONTRIBUTING.md](CONTRIBUTING.md) for more details.
```

### Comparing `aicodebot-0.5.3/aicodebot.egg-info/SOURCES.txt` & `aicodebot-0.5.4/aicodebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.3/pyproject.toml` & `aicodebot-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.5.3/setup.py` & `aicodebot-0.5.4/setup.py`

 * *Files identical despite different names*

