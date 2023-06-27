# Comparing `tmp/ConfigArgParse-1.5.3.tar.gz` & `tmp/ConfigArgParse-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ConfigArgParse-1.5.3.tar", last modified: Sun Oct  3 00:17:14 2021, max compression
+gzip compressed data, was "ConfigArgParse-1.5.5.tar", last modified: Tue Jun 27 20:26:56 2023, max compression
```

## Comparing `ConfigArgParse-1.5.3.tar` & `ConfigArgParse-1.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-10-03 00:17:14.000000 ConfigArgParse-1.5.3/
--rw-r--r--   0 root         (0) staff       (20)    22350 2021-10-03 00:17:14.000000 ConfigArgParse-1.5.3/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1070 2018-02-04 17:57:28.000000 ConfigArgParse-1.5.3/LICENSE
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-10-03 00:17:14.000000 ConfigArgParse-1.5.3/tests/
--rw-r--r--   0 root         (0) staff       (20)       46 2018-02-04 17:57:28.000000 ConfigArgParse-1.5.3/tests/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      140 2019-12-08 16:37:48.000000 ConfigArgParse-1.5.3/tests/__init__.pyc
--rw-r--r--   0 root         (0) staff       (20)    69819 2021-10-03 00:15:57.000000 ConfigArgParse-1.5.3/tests/test_configargparse.py
--rw-r--r--   0 root         (0) staff       (20)       51 2018-02-04 17:57:28.000000 ConfigArgParse-1.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)    49875 2021-10-03 00:15:57.000000 ConfigArgParse-1.5.3/configargparse.py
--rw-r--r--   0 root         (0) staff       (20)     3895 2021-10-03 00:16:57.000000 ConfigArgParse-1.5.3/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-10-03 00:17:14.000000 ConfigArgParse-1.5.3/ConfigArgParse.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    22350 2021-10-03 00:17:14.000000 ConfigArgParse-1.5.3/ConfigArgParse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      312 2021-10-03 00:17:14.000000 ConfigArgParse-1.5.3/ConfigArgParse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       42 2021-10-03 00:17:14.000000 ConfigArgParse-1.5.3/ConfigArgParse.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       15 2021-10-03 00:17:14.000000 ConfigArgParse-1.5.3/ConfigArgParse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2021-10-03 00:17:14.000000 ConfigArgParse-1.5.3/ConfigArgParse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2021-10-03 00:17:14.000000 ConfigArgParse-1.5.3/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)    17283 2021-08-05 23:14:22.000000 ConfigArgParse-1.5.3/README.rst
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-27 20:26:56.870567 ConfigArgParse-1.5.5/
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-27 20:26:56.866836 ConfigArgParse-1.5.5/ConfigArgParse.egg-info/
+-rw-r--r--   0 weisburd   (502) staff       (20)    23633 2023-06-27 20:26:56.000000 ConfigArgParse-1.5.5/ConfigArgParse.egg-info/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)      312 2023-06-27 20:26:56.000000 ConfigArgParse-1.5.5/ConfigArgParse.egg-info/SOURCES.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)        1 2023-06-27 20:26:56.000000 ConfigArgParse-1.5.5/ConfigArgParse.egg-info/dependency_links.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)       42 2023-06-27 20:26:56.000000 ConfigArgParse-1.5.5/ConfigArgParse.egg-info/requires.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)       15 2023-06-27 20:26:56.000000 ConfigArgParse-1.5.5/ConfigArgParse.egg-info/top_level.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)     1070 2018-02-04 17:57:28.000000 ConfigArgParse-1.5.5/LICENSE
+-rw-r--r--   0 weisburd   (502) staff       (20)       51 2018-02-04 17:57:28.000000 ConfigArgParse-1.5.5/MANIFEST.in
+-rw-r--r--   0 weisburd   (502) staff       (20)    23633 2023-06-27 20:26:56.870182 ConfigArgParse-1.5.5/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)    22375 2023-06-27 20:24:25.000000 ConfigArgParse-1.5.5/README.rst
+-rw-r--r--   0 weisburd   (502) staff       (20)    64519 2023-06-27 19:47:23.000000 ConfigArgParse-1.5.5/configargparse.py
+-rw-r--r--   0 weisburd   (502) staff       (20)       38 2023-06-27 20:26:56.870681 ConfigArgParse-1.5.5/setup.cfg
+-rw-r--r--   0 weisburd   (502) staff       (20)     4015 2023-06-27 20:20:39.000000 ConfigArgParse-1.5.5/setup.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-27 20:26:56.868768 ConfigArgParse-1.5.5/tests/
+-rw-r--r--   0 weisburd   (502) staff       (20)       46 2018-02-04 17:57:28.000000 ConfigArgParse-1.5.5/tests/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)      140 2019-12-08 16:37:48.000000 ConfigArgParse-1.5.5/tests/__init__.pyc
+-rw-r--r--   0 weisburd   (502) staff       (20)    70874 2023-06-27 19:58:08.000000 ConfigArgParse-1.5.5/tests/test_configargparse.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ConfigArgParse-1.5.3/PKG-INFO` & `ConfigArgParse-1.5.5/ConfigArgParse.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,491 +1,14 @@
 Metadata-Version: 2.1
 Name: ConfigArgParse
-Version: 1.5.3
+Version: 1.5.5
 Summary: A drop-in replacement for argparse that allows options to also be set via config files and/or environment variables.
 Home-page: https://github.com/bw2/ConfigArgParse
 License: MIT
-Description: ConfigArgParse
-        --------------
-        
-        .. image:: https://img.shields.io/pypi/v/ConfigArgParse.svg?style=flat
-            :alt: PyPI version
-            :target: https://pypi.python.org/pypi/ConfigArgParse
-        
-        .. image:: https://img.shields.io/pypi/pyversions/ConfigArgParse.svg
-            :alt: Supported Python versions
-            :target: https://pypi.python.org/pypi/ConfigArgParse
-        
-        .. image:: https://travis-ci.org/bw2/ConfigArgParse.svg?branch=master
-            :alt: Travis CI build
-            :target: https://travis-ci.org/bw2/ConfigArgParse
-        
-        .. image:: https://img.shields.io/badge/-API_Documentation-blue
-            :alt: API Documentation
-            :target: https://bw2.github.io/ConfigArgParse/
-        
-        Overview
-        ~~~~~~~~
-        
-        Applications with more than a handful of user-settable options are best
-        configured through a combination of command line args, config files,
-        hard-coded defaults, and in some cases, environment variables.
-        
-        Python's command line parsing modules such as argparse have very limited
-        support for config files and environment variables, so this module
-        extends argparse to add these features.
-        
-        Available on PyPI: http://pypi.python.org/pypi/ConfigArgParse
-        
-        .. image:: https://travis-ci.org/bw2/ConfigArgParse.svg?branch=master
-            :target: https://travis-ci.org/bw2/ConfigArgParse
-        
-        Features
-        ~~~~~~~~
-        
-        -  command-line, config file, env var, and default settings can now be
-           defined, documented, and parsed in one go using a single API (if a
-           value is specified in more than one way then: command line >
-           environment variables > config file values > defaults)
-        -  config files can have .ini or .yaml style syntax (eg. key=value or
-           key: value)
-        -  user can provide a config file via a normal-looking command line arg
-           (eg. -c path/to/config.txt) rather than the argparse-style @config.txt
-        -  one or more default config file paths can be specified
-           (eg. ['/etc/bla.conf', '~/.my_config'] )
-        -  all argparse functionality is fully supported, so this module can
-           serve as a drop-in replacement (verified by argparse unittests).
-        -  env vars and config file keys & syntax are automatically documented
-           in the -h help message
-        -  new method :code:`print_values()` can report keys & values and where
-           they were set (eg. command line, env var, config file, or default).
-        -  lite-weight (no 3rd-party library dependencies except (optionally) PyYAML)
-        -  extensible (:code:`ConfigFileParser` can be subclassed to define a new
-           config file format)
-        -  unittested by running the unittests that came with argparse but on
-           configargparse, and using tox to test with Python 2.7 and Python 3+
-        
-        Example
-        ~~~~~~~
-        
-        *config_test.py*:
-        
-        Script that defines 4 options and a positional arg and then parses and prints the values. Also,
-        it prints out the help message as well as the string produced by :code:`format_values()` to show
-        what they look like.
-        
-        .. code:: py
-        
-           import configargparse
-        
-           p = configargparse.ArgParser(default_config_files=['/etc/app/conf.d/*.conf', '~/.my_settings'])
-           p.add('-c', '--my-config', required=True, is_config_file=True, help='config file path')
-           p.add('--genome', required=True, help='path to genome file')  # this option can be set in a config file because it starts with '--'
-           p.add('-v', help='verbose', action='store_true')
-           p.add('-d', '--dbsnp', help='known variants .vcf', env_var='DBSNP_PATH')  # this option can be set in a config file because it starts with '--'
-           p.add('vcf', nargs='+', help='variant file(s)')
-        
-           options = p.parse_args()
-        
-           print(options)
-           print("----------")
-           print(p.format_help())
-           print("----------")
-           print(p.format_values())    # useful for logging where different settings came from
-        
-        
-        *config.txt:*
-        
-        Since the script above set the config file as required=True, lets create a config file to give it:
-        
-        .. code:: py
-        
-            # settings for config_test.py
-            genome = HCMV     # cytomegalovirus genome
-            dbsnp = /data/dbsnp/variants.vcf
-        
-        
-        *command line:*
-        
-        Now run the script and pass it the config file:
-        
-        .. code:: bash
-        
-            DBSNP_PATH=/data/dbsnp/variants_v2.vcf python config_test.py --my-config config.txt f1.vcf f2.vcf
-        
-        *output:*
-        
-        Here is the result:
-        
-        .. code:: bash
-        
-            Namespace(dbsnp='/data/dbsnp/variants_v2.vcf', genome='HCMV', my_config='config.txt', v=False, vcf=['f1.vcf', 'f2.vcf'])
-            ----------
-            usage: config_test.py [-h] -c MY_CONFIG --genome GENOME [-v] [-d DBSNP]
-                                  vcf [vcf ...]
-            
-            Args that start with '--' (eg. --genome) can also be set in a config file
-            (/etc/app/conf.d/*.conf or ~/.my_settings or specified via -c). Config file
-            syntax allows: key=value, flag=true, stuff=[a,b,c] (for details, see syntax at
-            https://goo.gl/R74nmi). If an arg is specified in more than one place, then
-            commandline values override environment variables which override config file
-            values which override defaults.
-            
-            positional arguments:
-              vcf                   variant file(s)
-            
-            optional arguments:
-              -h, --help            show this help message and exit
-              -c MY_CONFIG, --my-config MY_CONFIG
-                                    config file path
-              --genome GENOME       path to genome file
-              -v                    verbose
-              -d DBSNP, --dbsnp DBSNP
-                                    known variants .vcf [env var: DBSNP_PATH]
-            
-            ----------
-            Command Line Args:   --my-config config.txt f1.vcf f2.vcf
-            Environment Variables:
-              DBSNP_PATH:        /data/dbsnp/variants_v2.vcf
-            Config File (config.txt):
-              genome:            HCMV
-        
-        Special Values
-        ~~~~~~~~~~~~~~
-        
-        Under the hood, configargparse handles environment variables and config file
-        values by converting them to their corresponding command line arg. For
-        example, "key = value" will be processed as if "--key value" was specified
-        on the command line.
-        
-        Also, the following special values (whether in a config file or an environment
-        variable) are handled in a special way to support booleans and lists:
-        
-        -  :code:`key = true` is handled as if "--key" was specified on the command line.
-           In your python code this key must be defined as a boolean flag
-           (eg. action="store_true" or similar).
-        
-        -  :code:`key = [value1, value2, ...]` is handled as if "--key value1 --key value2"
-           etc. was specified on the command line. In your python code this key must
-           be defined as a list (eg. action="append").
-        
-        Config File Syntax
-        ~~~~~~~~~~~~~~~~~~
-        
-        Only command line args that have a long version (eg. one that starts with '--')
-        can be set in a config file. For example, "--color" can be set by putting
-        "color=green" in a config file. The config file syntax depends on the constuctor
-        arg: :code:`config_file_parser_class` which can be set to one of the provided
-        classes: :code:`DefaultConfigFileParser`, :code:`YAMLConfigFileParser`,
-        :code:`ConfigparserConfigFileParser` or to your own subclass of the
-        :code:`ConfigFileParser` abstract class.
-        
-        *DefaultConfigFileParser*  - the full range of valid syntax is:
-        
-        .. code:: yaml
-        
-                # this is a comment
-                ; this is also a comment (.ini style)
-                ---            # lines that start with --- are ignored (yaml style)
-                -------------------
-                [section]      # .ini-style section names are treated as comments
-        
-                # how to specify a key-value pair (all of these are equivalent):
-                name value     # key is case sensitive: "Name" isn't "name"
-                name = value   # (.ini style)  (white space is ignored, so name = value same as name=value)
-                name: value    # (yaml style)
-                --name value   # (argparse style)
-        
-                # how to set a flag arg (eg. arg which has action="store_true")
-                --name
-                name
-                name = True    # "True" and "true" are the same
-        
-                # how to specify a list arg (eg. arg which has action="append")
-                fruit = [apple, orange, lemon]
-                indexes = [1, 12, 35 , 40]
-        
-        
-        *YAMLConfigFileParser*  - allows a subset of YAML syntax (http://goo.gl/VgT2DU)
-        
-        .. code:: yaml
-        
-                # a comment
-                name1: value
-                name2: true    # "True" and "true" are the same
-        
-                fruit: [apple, orange, lemon]
-                indexes: [1, 12, 35, 40]
-        
-        *ConfigparserConfigFileParser*  - allows a subset of python's configparser
-        module syntax (https://docs.python.org/3.7/library/configparser.html). In
-        particular the following configparser options are set:
-        
-        .. code:: py
-        
-                config = configparser.ArgParser(
-                    delimiters=("=",":"),
-                    allow_no_value=False,
-                    comment_prefixes=("#",";"),
-                    inline_comment_prefixes=("#",";"),
-                    strict=True,
-                    empty_lines_in_values=False,
-                )
-        
-        Once configparser parses the config file all section names are removed, thus all
-        keys must have unique names regardless of which INI section they are defined
-        under. Also, any keys which have python list syntax are converted to lists by
-        evaluating them as python code using ast.literal_eval
-        (https://docs.python.org/3/library/ast.html#ast.literal_eval). To facilitate
-        this all multi-line values are converted to single-line values. Thus multi-line
-        string values will have all new-lines converted to spaces. Note, since key-value
-        pairs that have python dictionary syntax are saved as single-line strings, even
-        if formatted across multiple lines in the config file, dictionaries can be read
-        in and converted to valid python dictionaries with PyYAML's safe_load. Example
-        given below:
-        
-        .. code:: py
-        
-                # inside your config file (e.g. config.ini)
-                [section1]  # INI sections treated as comments
-                system1_settings: { # start of multi-line dictionary
-                    'a':True,
-                    'b':[2, 4, 8, 16],
-                    'c':{'start':0, 'stop':1000},
-                    'd':'experiment 32 testing simulation with parameter a on'
-                    } # end of multi-line dictionary value
-        
-                .......
-        
-                # in your configargparse setup
-                import configargparse
-                import yaml
-        
-                parser = configargparse.ArgParser(
-                    config_file_parser_class=configargparse.ConfigparserConfigFileParser
-                )
-                parser.add_argument('--system1_settings', type=yaml.safe_load)
-                
-                args = parser.parse_args() # now args.system1 is a valid python dict
-        
-        
-        ArgParser Singletons
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        To make it easier to configure different modules in an application,
-        configargparse provides globally-available ArgumentParser instances
-        via configargparse.get_argument_parser('name') (similar to
-        logging.getLogger('name')).
-        
-        Here is an example of an application with a utils module that also
-        defines and retrieves its own command-line args.
-        
-        *main.py*
-        
-        .. code:: py
-        
-            import configargparse
-            import utils
-        
-            p = configargparse.get_argument_parser()
-            p.add_argument("-x", help="Main module setting")
-            p.add_argument("--m-setting", help="Main module setting")
-            options = p.parse_known_args()   # using p.parse_args() here may raise errors.
-        
-        *utils.py*
-        
-        .. code:: py
-        
-            import configargparse
-            p = configargparse.get_argument_parser()
-            p.add_argument("--utils-setting", help="Config-file-settable option for utils")
-        
-            if __name__ == "__main__":
-               options = p.parse_known_args()
-        
-        Help Formatters
-        ~~~~~~~~~~~~~~~
-        
-        :code:`ArgumentDefaultsRawHelpFormatter` is a new HelpFormatter that both adds
-        default values AND disables line-wrapping. It can be passed to the constructor:
-        :code:`ArgParser(.., formatter_class=ArgumentDefaultsRawHelpFormatter)`
-        
-        
-        Aliases
-        ~~~~~~~
-        
-        The configargparse.ArgumentParser API inherits its class and method
-        names from argparse and also provides the following shorter names for
-        convenience:
-        
-        -  p = configargparse.get_arg_parser()  # get global singleton instance
-        -  p = configargparse.get_parser()
-        -  p = configargparse.ArgParser()  # create a new instance
-        -  p = configargparse.Parser()
-        -  p.add_arg(..)
-        -  p.add(..)
-        -  options = p.parse(..)
-        
-        HelpFormatters:
-        
-        - RawFormatter = RawDescriptionHelpFormatter
-        - DefaultsFormatter = ArgumentDefaultsHelpFormatter
-        - DefaultsRawFormatter = ArgumentDefaultsRawHelpFormatter
-        
-        API Documentation
-        ~~~~~~~~~~~~~~~~~
-        
-        You can review the generated API Documentation for the ``configargparse`` module: `HERE <https://bw2.github.io/ConfigArgParse/>`_
-        
-        Design Notes
-        ~~~~~~~~~~~~
-        
-        Unit tests:
-        
-        tests/test_configargparse.py contains custom unittests for features
-        specific to this module (such as config file and env-var support), as
-        well as a hook to load and run argparse unittests (see the built-in
-        test.test_argparse module) but on configargparse in place of argparse.
-        This ensures that configargparse will work as a drop in replacement for
-        argparse in all usecases.
-        
-        Previously existing modules (PyPI search keywords: config argparse):
-        
-        -  argparse (built-in module Python v2.7+)
-        
-           -  Good:
-        
-              -  fully featured command line parsing
-              -  can read args from files using an easy to understand mechanism
-        
-           -  Bad:
-        
-              -  syntax for specifying config file path is unusual (eg.
-                 @file.txt)and not described in the user help message.
-              -  default config file syntax doesn't support comments and is
-                 unintuitive (eg. --namevalue)
-              -  no support for environment variables
-        
-        -  ConfArgParse v1.0.15
-           (https://pypi.python.org/pypi/ConfArgParse)
-        
-           -  Good:
-        
-              -  extends argparse with support for config files parsed by
-                 ConfigParser
-              -  clear documentation in README
-        
-           -  Bad:
-        
-              -  config file values are processed using
-                 ArgumentParser.set_defaults(..) which means "required" and
-                 "choices" are not handled as expected. For example, if you
-                 specify a required value in a config file, you still have to
-                 specify it again on the command line.
-              -  doesn't work with Python 3 yet
-              -  no unit tests, code not well documented
-        
-        -  appsettings v0.5 (https://pypi.python.org/pypi/appsettings)
-        
-           -  Good:
-        
-              -  supports config file (yaml format) and env_var parsing
-              -  supports config-file-only setting for specifying lists and
-                 dicts
-        
-           -  Bad:
-        
-              -  passes in config file and env settings via parse_args
-                 namespace param
-              -  tests not finished and don't work with Python 3 (import
-                 StringIO)
-        
-        -  argparse_config v0.5.1
-           (https://pypi.python.org/pypi/argparse_config)
-        
-           -  Good:
-        
-              -  similar features to ConfArgParse v1.0.15
-        
-           -  Bad:
-        
-              -  doesn't work with Python 3 (error during pip install)
-        
-        -  yconf v0.3.2 - (https://pypi.python.org/pypi/yconf) - features
-           and interface not that great
-        -  hieropt v0.3 - (https://pypi.python.org/pypi/hieropt) - doesn't
-           appear to be maintained, couldn't find documentation
-        
-        -  configurati v0.2.3 - (https://pypi.python.org/pypi/configurati)
-        
-           -  Good:
-        
-              -  JSON, YAML, or Python configuration files
-              -  handles rich data structures such as dictionaries
-              -  can group configuration names into sections (like .ini files)
-        
-           -  Bad:
-        
-              -  doesn't work with Python 3
-              -  2+ years since last release to PyPI
-              -  apparently unmaintained
-        
-        
-        Design choices:
-        
-        1. all options must be settable via command line. Having options that
-           can only be set using config files or env. vars adds complexity to
-           the API, and is not a useful enough feature since the developer can
-           split up options into sections and call a section "config file keys",
-           with command line args that are just "--" plus the config key.
-        2. config file and env. var settings should be processed by appending
-           them to the command line (another benefit of #1). This is an
-           easy-to-implement solution and implicitly takes care of checking that
-           all "required" args are provied, etc., plus the behavior should be
-           easy for users to understand.
-        3. configargparse shouldn't override argparse's
-           convert_arg_line_to_args method so that all argparse unit tests
-           can be run on configargparse.
-        4. in terms of what to allow for config file keys, the "dest" value of
-           an option can't serve as a valid config key because many options can
-           have the same dest. Instead, since multiple options can't use the
-           same long arg (eg. "--long-arg-x"), let the config key be either
-           "--long-arg-x" or "long-arg-x". This means the developer can allow
-           only a subset of the command-line args to be specified via config
-           file (eg. short args like -x would be excluded). Also, that way
-           config keys are automatically documented whenever the command line
-           args are documented in the help message.
-        5. don't force users to put config file settings in the right .ini
-           [sections]. This doesn't have a clear benefit since all options are
-           command-line settable, and so have a globally unique key anyway.
-           Enforcing sections just makes things harder for the user and adds
-           complexity to the implementation.
-        6. if necessary, config-file-only args can be added later by
-           implementing a separate add method and using the namespace arg as in
-           appsettings_v0.5
-        
-        Relevant sites:
-        
-        -  http://stackoverflow.com/questions/6133517/parse-config-file-environment-and-command-line-arguments-to-get-a-single-coll
-        -  http://tricksntweaks.blogspot.com/2013_05_01_archive.html
-        -  http://www.youtube.com/watch?v=vvCwqHgZJc8#t=35
-        
-        
-        .. |Travis CI Status for bw2/ConfigArgParse| image:: https://travis-ci.org/bw2/ConfigArgParse.svg?branch=master
-        
-        
-        Versioning
-        ~~~~~~~~~~
-        
-        This software follows `Semantic Versioning`_
-        
-        .. _Semantic Versioning: http://semver.org/
-        
 Keywords: options,argparse,ConfigArgParse,config,environment variables,envvars,ENV,environment,optparse,YAML,INI
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -494,9 +17,607 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
-Provides-Extra: test
 Provides-Extra: yaml
+Provides-Extra: test
+License-File: LICENSE
+
+ConfigArgParse
+--------------
+
+.. image:: https://img.shields.io/pypi/v/ConfigArgParse.svg?style=flat
+    :alt: PyPI version
+    :target: https://pypi.python.org/pypi/ConfigArgParse
+
+.. image:: https://img.shields.io/pypi/pyversions/ConfigArgParse.svg
+    :alt: Supported Python versions
+    :target: https://pypi.python.org/pypi/ConfigArgParse
+
+.. image:: https://img.shields.io/badge/-API_Documentation-blue
+    :alt: API Documentation
+    :target: https://bw2.github.io/ConfigArgParse/
+
+Overview
+~~~~~~~~
+
+Applications with more than a handful of user-settable options are best
+configured through a combination of command line args, config files,
+hard-coded defaults, and in some cases, environment variables.
+
+Python's command line parsing modules such as argparse have very limited
+support for config files and environment variables, so this module
+extends argparse to add these features.
+
+Available on PyPI: http://pypi.python.org/pypi/ConfigArgParse
+
+
+Features
+~~~~~~~~
+
+-  command-line, config file, env var, and default settings can now be
+   defined, documented, and parsed in one go using a single API (if a
+   value is specified in more than one way then: command line >
+   environment variables > config file values > defaults)
+-  config files can have .ini or .yaml style syntax (eg. key=value or
+   key: value)
+-  user can provide a config file via a normal-looking command line arg
+   (eg. -c path/to/config.txt) rather than the argparse-style @config.txt
+-  one or more default config file paths can be specified
+   (eg. ['/etc/bla.conf', '~/.my_config'] )
+-  all argparse functionality is fully supported, so this module can
+   serve as a drop-in replacement (verified by argparse unittests).
+-  env vars and config file keys & syntax are automatically documented
+   in the -h help message
+-  new method :code:`print_values()` can report keys & values and where
+   they were set (eg. command line, env var, config file, or default).
+-  lite-weight (no 3rd-party library dependencies except (optionally) PyYAML)
+-  extensible (:code:`ConfigFileParser` can be subclassed to define a new
+   config file format)
+-  unittested by running the unittests that came with argparse but on
+   configargparse, and using tox to test with Python 2.7 and Python 3+
+
+Example
+~~~~~~~
+
+*config_test.py*:
+
+Script that defines 4 options and a positional arg and then parses and prints the values. Also,
+it prints out the help message as well as the string produced by :code:`format_values()` to show
+what they look like.
+
+.. code:: py
+
+   import configargparse
+
+   p = configargparse.ArgParser(default_config_files=['/etc/app/conf.d/*.conf', '~/.my_settings'])
+   p.add('-c', '--my-config', required=True, is_config_file=True, help='config file path')
+   p.add('--genome', required=True, help='path to genome file')  # this option can be set in a config file because it starts with '--'
+   p.add('-v', help='verbose', action='store_true')
+   p.add('-d', '--dbsnp', help='known variants .vcf', env_var='DBSNP_PATH')  # this option can be set in a config file because it starts with '--'
+   p.add('vcf', nargs='+', help='variant file(s)')
+
+   options = p.parse_args()
+
+   print(options)
+   print("----------")
+   print(p.format_help())
+   print("----------")
+   print(p.format_values())    # useful for logging where different settings came from
+
+
+*config.txt:*
+
+Since the script above set the config file as required=True, lets create a config file to give it:
+
+.. code:: py
+
+    # settings for config_test.py
+    genome = HCMV     # cytomegalovirus genome
+    dbsnp = /data/dbsnp/variants.vcf
+
+
+*command line:*
+
+Now run the script and pass it the config file:
+
+.. code:: bash
+
+    DBSNP_PATH=/data/dbsnp/variants_v2.vcf python config_test.py --my-config config.txt f1.vcf f2.vcf
+
+*output:*
+
+Here is the result:
+
+.. code:: bash
+
+    Namespace(dbsnp='/data/dbsnp/variants_v2.vcf', genome='HCMV', my_config='config.txt', v=False, vcf=['f1.vcf', 'f2.vcf'])
+    ----------
+    usage: config_test.py [-h] -c MY_CONFIG --genome GENOME [-v] [-d DBSNP]
+                          vcf [vcf ...]
+    
+    Args that start with '--' (eg. --genome) can also be set in a config file
+    (/etc/app/conf.d/*.conf or ~/.my_settings or specified via -c). Config file
+    syntax allows: key=value, flag=true, stuff=[a,b,c] (for details, see syntax at
+    https://goo.gl/R74nmi). If an arg is specified in more than one place, then
+    commandline values override environment variables which override config file
+    values which override defaults.
+    
+    positional arguments:
+      vcf                   variant file(s)
+    
+    optional arguments:
+      -h, --help            show this help message and exit
+      -c MY_CONFIG, --my-config MY_CONFIG
+                            config file path
+      --genome GENOME       path to genome file
+      -v                    verbose
+      -d DBSNP, --dbsnp DBSNP
+                            known variants .vcf [env var: DBSNP_PATH]
+    
+    ----------
+    Command Line Args:   --my-config config.txt f1.vcf f2.vcf
+    Environment Variables:
+      DBSNP_PATH:        /data/dbsnp/variants_v2.vcf
+    Config File (config.txt):
+      genome:            HCMV
+
+Special Values
+~~~~~~~~~~~~~~
+
+Under the hood, configargparse handles environment variables and config file
+values by converting them to their corresponding command line arg. For
+example, "key = value" will be processed as if "--key value" was specified
+on the command line.
+
+Also, the following special values (whether in a config file or an environment
+variable) are handled in a special way to support booleans and lists:
+
+-  :code:`key = true` is handled as if "--key" was specified on the command line.
+   In your python code this key must be defined as a boolean flag
+   (eg. action="store_true" or similar).
+
+-  :code:`key = [value1, value2, ...]` is handled as if "--key value1 --key value2"
+   etc. was specified on the command line. In your python code this key must
+   be defined as a list (eg. action="append").
+
+Config File Syntax
+~~~~~~~~~~~~~~~~~~
+
+Only command line args that have a long version (eg. one that starts with '--')
+can be set in a config file. For example, "--color" can be set by putting
+"color=green" in a config file. The config file syntax depends on the constructor
+arg: :code:`config_file_parser_class` which can be set to one of the provided
+classes: :code:`DefaultConfigFileParser`, :code:`YAMLConfigFileParser`,
+:code:`ConfigparserConfigFileParser` or to your own subclass of the
+:code:`ConfigFileParser` abstract class.
+
+*DefaultConfigFileParser*  - the full range of valid syntax is:
+
+.. code:: yaml
+
+        # this is a comment
+        ; this is also a comment (.ini style)
+        ---            # lines that start with --- are ignored (yaml style)
+        -------------------
+        [section]      # .ini-style section names are treated as comments
+
+        # how to specify a key-value pair (all of these are equivalent):
+        name value     # key is case sensitive: "Name" isn't "name"
+        name = value   # (.ini style)  (white space is ignored, so name = value same as name=value)
+        name: value    # (yaml style)
+        --name value   # (argparse style)
+
+        # how to set a flag arg (eg. arg which has action="store_true")
+        --name
+        name
+        name = True    # "True" and "true" are the same
+
+        # how to specify a list arg (eg. arg which has action="append")
+        fruit = [apple, orange, lemon]
+        indexes = [1, 12, 35 , 40]
+
+
+*YAMLConfigFileParser*  - allows a subset of YAML syntax (http://goo.gl/VgT2DU)
+
+.. code:: yaml
+
+        # a comment
+        name1: value
+        name2: true    # "True" and "true" are the same
+
+        fruit: [apple, orange, lemon]
+        indexes: [1, 12, 35, 40]
+        colors:
+          - green
+          - red
+          - blue
+
+*ConfigparserConfigFileParser*  - allows a subset of python's configparser
+module syntax (https://docs.python.org/3.7/library/configparser.html). In
+particular the following configparser options are set:
+
+.. code:: py
+
+        config = configparser.ArgParser(
+            delimiters=("=",":"),
+            allow_no_value=False,
+            comment_prefixes=("#",";"),
+            inline_comment_prefixes=("#",";"),
+            strict=True,
+            empty_lines_in_values=False,
+        )
+
+Once configparser parses the config file all section names are removed, thus all
+keys must have unique names regardless of which INI section they are defined
+under. Also, any keys which have python list syntax are converted to lists by
+evaluating them as python code using ast.literal_eval
+(https://docs.python.org/3/library/ast.html#ast.literal_eval). To facilitate
+this all multi-line values are converted to single-line values. Thus multi-line
+string values will have all new-lines converted to spaces. Note, since key-value
+pairs that have python dictionary syntax are saved as single-line strings, even
+if formatted across multiple lines in the config file, dictionaries can be read
+in and converted to valid python dictionaries with PyYAML's safe_load. Example
+given below:
+
+.. code:: py
+
+        # inside your config file (e.g. config.ini)
+        [section1]  # INI sections treated as comments
+        system1_settings: { # start of multi-line dictionary
+            'a':True,
+            'b':[2, 4, 8, 16],
+            'c':{'start':0, 'stop':1000},
+            'd':'experiment 32 testing simulation with parameter a on'
+            } # end of multi-line dictionary value
+
+        .......
+
+        # in your configargparse setup
+        import configargparse
+        import yaml
+
+        parser = configargparse.ArgParser(
+            config_file_parser_class=configargparse.ConfigparserConfigFileParser
+        )
+        parser.add_argument('--system1_settings', type=yaml.safe_load)
+        
+        args = parser.parse_args() # now args.system1 is a valid python dict
+
+*IniConfigParser*  - INI parser with support for sections.
+
+This parser somewhat ressembles ``ConfigparserConfigFileParser``. It uses configparser and apply the same kind of processing to 
+values written with python list syntax. 
+
+With the following additions: 
+   - Must be created with argument to bind the parser to a list of sections.
+   - Does not convert multiline strings to single line.
+   - Optional support for converting multiline strings to list (if ``split_ml_text_to_list=True``). 
+   - Optional support for quoting strings in config file 
+      (useful when text must not be converted to list or when text 
+      should contain trailing whitespaces).
+
+This config parser can be used to integrate with ``setup.cfg`` files.
+
+Example::
+
+      # this is a comment
+      ; also a comment
+      [my_super_tool]
+      # how to specify a key-value pair
+      format-string: restructuredtext 
+      # white space are ignored, so name = value same as name=value
+      # this is why you can quote strings 
+      quoted-string = '\thello\tmom...  '
+      # how to set an arg which has action="store_true"
+      warnings-as-errors = true
+      # how to set an arg which has action="count" or type=int
+      verbosity = 1
+      # how to specify a list arg (eg. arg which has action="append")
+      repeatable-option = ["https://docs.python.org/3/objects.inv",
+                     "https://twistedmatrix.com/documents/current/api/objects.inv"]
+      # how to specify a multiline text:
+      multi-line-text = 
+         Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+         Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+         Maecenas quis dapibus leo, a pellentesque leo. 
+
+If you use ``IniConfigParser(sections, split_ml_text_to_list=True)``::
+
+      # the same rules are applicable with the following changes:
+      [my-software]
+      # how to specify a list arg (eg. arg which has action="append")
+      repeatable-option = # Just enter one value per line (the list literal format can also be used)
+         https://docs.python.org/3/objects.inv
+         https://twistedmatrix.com/documents/current/api/objects.inv
+      # how to specify a multiline text (you have to quote it):
+      multi-line-text = '''
+         Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+         Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+         Maecenas quis dapibus leo, a pellentesque leo. 
+         '''
+
+Usage:
+
+.. code:: py
+
+   import configargparse
+   parser = configargparse.ArgParser(
+            default_config_files=['setup.cfg', 'my_super_tool.ini'],
+            config_file_parser_class=configargparse.IniConfigParser(['tool:my_super_tool', 'my_super_tool']),
+        )
+   ...
+
+*TomlConfigParser*  - TOML parser with support for sections.
+
+`TOML <https://github.com/toml-lang/toml/blob/main/toml.md>`_ parser. This config parser can be used to integrate with ``pyproject.toml`` files.
+
+Example::
+
+   # this is a comment
+   [tool.my-software] # TOML section table.
+   # how to specify a key-value pair
+   format-string = "restructuredtext" # strings must be quoted
+   # how to set an arg which has action="store_true"
+   warnings-as-errors = true
+   # how to set an arg which has action="count" or type=int
+   verbosity = 1
+   # how to specify a list arg (eg. arg which has action="append")
+   repeatable-option = ["https://docs.python.org/3/objects.inv",
+                  "https://twistedmatrix.com/documents/current/api/objects.inv"]
+   # how to specify a multiline text:
+   multi-line-text = '''
+      Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+      Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+      Maecenas quis dapibus leo, a pellentesque leo. 
+      '''
+
+Usage:
+
+.. code:: py
+
+   import configargparse
+   parser = configargparse.ArgParser(
+            default_config_files=['pyproject.toml', 'my_super_tool.toml'],
+            config_file_parser_class=configargparse.TomlConfigParser(['tool.my_super_tool']),
+        )
+   ...
+
+*CompositeConfigParser*  - Create a config parser to understand multiple formats.
+
+This parser will successively try to parse the file with each parser, until it succeeds, 
+else fail showing all encountered error messages.
+
+The following code will make configargparse understand both TOML and INI formats. 
+Making it easy to integrate in both ``pyproject.toml`` and ``setup.cfg``.
+
+.. code:: py
+
+   import configargparse
+   my_tool_sections = ['tool.my_super_tool', 'tool:my_super_tool', 'my_super_tool']
+                    # pyproject.toml like section, setup.cfg like section, custom section
+   parser = configargparse.ArgParser(
+            default_config_files=['setup.cfg', 'my_super_tool.ini'],
+            config_file_parser_class=configargparse.CompositeConfigParser(
+               [configargparse.TomlConfigParser(my_tool_sections), 
+                configargparse.IniConfigParser(my_tool_sections, split_ml_text_to_list=True)]
+               ),
+        )
+   ...
+
+Note that it's required to put the TOML parser first because the INI syntax basically would accept anything whereas TOML. 
+
+ArgParser Singletons
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To make it easier to configure different modules in an application,
+configargparse provides globally-available ArgumentParser instances
+via configargparse.get_argument_parser('name') (similar to
+logging.getLogger('name')).
+
+Here is an example of an application with a utils module that also
+defines and retrieves its own command-line args.
+
+*main.py*
+
+.. code:: py
+
+    import configargparse
+    import utils
+
+    p = configargparse.get_argument_parser()
+    p.add_argument("-x", help="Main module setting")
+    p.add_argument("--m-setting", help="Main module setting")
+    options = p.parse_known_args()   # using p.parse_args() here may raise errors.
+
+*utils.py*
+
+.. code:: py
+
+    import configargparse
+    p = configargparse.get_argument_parser()
+    p.add_argument("--utils-setting", help="Config-file-settable option for utils")
+
+    if __name__ == "__main__":
+       options = p.parse_known_args()
+
+Help Formatters
+~~~~~~~~~~~~~~~
+
+:code:`ArgumentDefaultsRawHelpFormatter` is a new HelpFormatter that both adds
+default values AND disables line-wrapping. It can be passed to the constructor:
+:code:`ArgParser(.., formatter_class=ArgumentDefaultsRawHelpFormatter)`
+
+
+Aliases
+~~~~~~~
+
+The configargparse.ArgumentParser API inherits its class and method
+names from argparse and also provides the following shorter names for
+convenience:
+
+-  p = configargparse.get_arg_parser()  # get global singleton instance
+-  p = configargparse.get_parser()
+-  p = configargparse.ArgParser()  # create a new instance
+-  p = configargparse.Parser()
+-  p.add_arg(..)
+-  p.add(..)
+-  options = p.parse(..)
+
+HelpFormatters:
+
+- RawFormatter = RawDescriptionHelpFormatter
+- DefaultsFormatter = ArgumentDefaultsHelpFormatter
+- DefaultsRawFormatter = ArgumentDefaultsRawHelpFormatter
+
+API Documentation
+~~~~~~~~~~~~~~~~~
+
+You can review the generated API Documentation for the ``configargparse`` module: `HERE <https://bw2.github.io/ConfigArgParse/>`_
+
+Design Notes
+~~~~~~~~~~~~
+
+Unit tests:
+
+tests/test_configargparse.py contains custom unittests for features
+specific to this module (such as config file and env-var support), as
+well as a hook to load and run argparse unittests (see the built-in
+test.test_argparse module) but on configargparse in place of argparse.
+This ensures that configargparse will work as a drop in replacement for
+argparse in all usecases.
+
+Previously existing modules (PyPI search keywords: config argparse):
+
+-  argparse (built-in module Python v2.7+)
+
+   -  Good:
+
+      -  fully featured command line parsing
+      -  can read args from files using an easy to understand mechanism
+
+   -  Bad:
+
+      -  syntax for specifying config file path is unusual (eg.
+         @file.txt)and not described in the user help message.
+      -  default config file syntax doesn't support comments and is
+         unintuitive (eg. --namevalue)
+      -  no support for environment variables
+
+-  ConfArgParse v1.0.15
+   (https://pypi.python.org/pypi/ConfArgParse)
+
+   -  Good:
+
+      -  extends argparse with support for config files parsed by
+         ConfigParser
+      -  clear documentation in README
+
+   -  Bad:
+
+      -  config file values are processed using
+         ArgumentParser.set_defaults(..) which means "required" and
+         "choices" are not handled as expected. For example, if you
+         specify a required value in a config file, you still have to
+         specify it again on the command line.
+      -  doesn't work with Python 3 yet
+      -  no unit tests, code not well documented
+
+-  appsettings v0.5 (https://pypi.python.org/pypi/appsettings)
+
+   -  Good:
+
+      -  supports config file (yaml format) and env_var parsing
+      -  supports config-file-only setting for specifying lists and
+         dicts
+
+   -  Bad:
+
+      -  passes in config file and env settings via parse_args
+         namespace param
+      -  tests not finished and don't work with Python 3 (import
+         StringIO)
+
+-  argparse_config v0.5.1
+   (https://pypi.python.org/pypi/argparse_config)
+
+   -  Good:
+
+      -  similar features to ConfArgParse v1.0.15
+
+   -  Bad:
+
+      -  doesn't work with Python 3 (error during pip install)
+
+-  yconf v0.3.2 - (https://pypi.python.org/pypi/yconf) - features
+   and interface not that great
+-  hieropt v0.3 - (https://pypi.python.org/pypi/hieropt) - doesn't
+   appear to be maintained, couldn't find documentation
+
+-  configurati v0.2.3 - (https://pypi.python.org/pypi/configurati)
+
+   -  Good:
+
+      -  JSON, YAML, or Python configuration files
+      -  handles rich data structures such as dictionaries
+      -  can group configuration names into sections (like .ini files)
+
+   -  Bad:
+
+      -  doesn't work with Python 3
+      -  2+ years since last release to PyPI
+      -  apparently unmaintained
+
+
+Design choices:
+
+1. all options must be settable via command line. Having options that
+   can only be set using config files or env. vars adds complexity to
+   the API, and is not a useful enough feature since the developer can
+   split up options into sections and call a section "config file keys",
+   with command line args that are just "--" plus the config key.
+2. config file and env. var settings should be processed by appending
+   them to the command line (another benefit of #1). This is an
+   easy-to-implement solution and implicitly takes care of checking that
+   all "required" args are provided, etc., plus the behavior should be
+   easy for users to understand.
+3. configargparse shouldn't override argparse's
+   convert_arg_line_to_args method so that all argparse unit tests
+   can be run on configargparse.
+4. in terms of what to allow for config file keys, the "dest" value of
+   an option can't serve as a valid config key because many options can
+   have the same dest. Instead, since multiple options can't use the
+   same long arg (eg. "--long-arg-x"), let the config key be either
+   "--long-arg-x" or "long-arg-x". This means the developer can allow
+   only a subset of the command-line args to be specified via config
+   file (eg. short args like -x would be excluded). Also, that way
+   config keys are automatically documented whenever the command line
+   args are documented in the help message.
+5. > don't force users to put config file settings in the right .ini [sections].
+   This doesn't have a clear benefit since all options are command-line settable,
+   and so have a globally unique key anyway.
+   Enforcing sections just makes things harder for the user and adds complexity to the implementation.
+   NOTE: This design choice was preventing configargparse from integrating with common Python project
+   config files like setup.cfg or pyproject.toml,
+   so additional parser classes were added that parse only a subset of the values defined in INI or
+   TOML config files.
+6. if necessary, config-file-only args can be added later by
+   implementing a separate add method and using the namespace arg as in
+   appsettings_v0.5
+
+Relevant sites:
+
+-  http://stackoverflow.com/questions/6133517/parse-config-file-environment-and-command-line-arguments-to-get-a-single-coll
+-  http://tricksntweaks.blogspot.com/2013_05_01_archive.html
+-  http://www.youtube.com/watch?v=vvCwqHgZJc8#t=35
+
+
+
+Versioning
+~~~~~~~~~~
+
+This software follows `Semantic Versioning`_
+
+.. _Semantic Versioning: http://semver.org/
```

### Comparing `ConfigArgParse-1.5.3/LICENSE` & `ConfigArgParse-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ConfigArgParse-1.5.3/tests/test_configargparse.py` & `ConfigArgParse-1.5.5/tests/test_configargparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 
         self.assertRegex(self.format_values(),
             "Command Line Args:   file1.txt file2.txt --arg-x -y 3 --arg-z 100")
 
     def testBasicCase2(self, use_groups=False):
 
         ## Test command line, config file and env var values
-        default_config_file = tempfile.NamedTemporaryFile(mode="w", delete=True)
+        default_config_file = tempfile.NamedTemporaryFile(mode="w", delete=False)
         default_config_file.flush()
 
         p = self.initParser(default_config_files=['/etc/settings.ini',
                 '/home/jeff/.user_settings', default_config_file.name])
         p.add_arg('vcf', nargs='+', help='Variant file(s)')
         if not use_groups:
             self.add_arg('--genome', help='Path to genome file', required=True)
@@ -203,15 +203,15 @@
         self.assertParseArgsRaises("too few arg"
                                    if sys.version_info.major < 3 else
                                    "the following arguments are required: vcf, -g/--my-cfg-file",
                                    args="--genome hg19")
         self.assertParseArgsRaises("Unable to open config file: file.txt. Error: No such file or director", args="-g file.txt")
 
         # check values after setting args on command line
-        config_file2 = tempfile.NamedTemporaryFile(mode="w", delete=True)
+        config_file2 = tempfile.NamedTemporaryFile(mode="w", delete=False)
         config_file2.flush()
 
         ns = self.parse(args="--genome hg19 -g %s bla.vcf " % config_file2.name)
         self.assertEqual(ns.genome, "hg19")
         self.assertEqual(ns.verbose, False)
         self.assertIsNone(ns.dbsnp)
         self.assertEqual(ns.fmt, "BED")
@@ -343,15 +343,15 @@
 
         ns = self.parse("positional_value", config_file_contents="""arg = [Shell, someword, anotherword]""")
 
         self.assertEqual(ns.arg, ['Shell', 'someword', 'anotherword'])
         self.assertEqual(ns.a, "positional_value")
 
     def testMutuallyExclusiveArgs(self):
-        config_file = tempfile.NamedTemporaryFile(mode="w", delete=True)
+        config_file = tempfile.NamedTemporaryFile(mode="w", delete=False)
 
         p = self.parser
         g = p.add_argument_group(title="group1")
         g.add_arg('--genome', help='Path to genome file', required=True)
         g.add_arg('-v', dest='verbose', action='store_true')
 
         g = p.add_mutually_exclusive_group(required=True)
@@ -394,19 +394,19 @@
             'group1:\n'
             '  --genome GENOME       Path to genome file\n'
             '  -v\n\n'%OPTIONAL_ARGS_STRING +
             5*r'(.+\s*)')
         config_file.close()
 
     def testSubParsers(self):
-        config_file1 = tempfile.NamedTemporaryFile(mode="w", delete=True)
+        config_file1 = tempfile.NamedTemporaryFile(mode="w", delete=False)
         config_file1.write("--i = B")
         config_file1.flush()
 
-        config_file2 = tempfile.NamedTemporaryFile(mode="w", delete=True)
+        config_file2 = tempfile.NamedTemporaryFile(mode="w", delete=False)
         config_file2.write("p = 10")
         config_file2.flush()
 
         parser = configargparse.ArgumentParser(prog="myProg")
         subparsers = parser.add_subparsers(title="actions")
 
         parent_parser = configargparse.ArgumentParser(add_help=False)
@@ -623,15 +623,15 @@
         ns = self.parse("", env_vars = {"HEIGHT": "tall", "FLAG2": "no"})
         self.assertEqual(ns.y, True)
 
         # error should occur when flag arg is given a value
         self.initParser()
         self.add_arg("-v", "--verbose", env_var="VERBOSE", action="store_true")
         self.assertParseArgsRaises("Unexpected value for VERBOSE: 'bla'. "
-                                   "Expecting 'true', 'false', 'yes', 'no', '1' or '0'",
+                                   "Expecting 'true', 'false', 'yes', 'no', 'on', 'off', '1' or '0'",
             args="",
             env_vars={"VERBOSE" : "bla"})
         ns = self.parse("",
                         config_file_contents="verbose=true",
                         env_vars={"HEIGHT": "true"})
         self.assertEqual(ns.verbose, True)
         ns = self.parse("",
@@ -831,41 +831,41 @@
         self.assertRaises(ValueError, self.add_arg, 'c', action="store_false",
                           is_config_file=True)
 
         self.add_arg("-c", "--config", is_config_file=True)
         self.add_arg("--x", required=True)
 
         # verify parsing from config file
-        config_file = tempfile.NamedTemporaryFile(mode="w", delete=True)
+        config_file = tempfile.NamedTemporaryFile(mode="w", delete=False)
         config_file.write("x=bla")
         config_file.flush()
 
         ns = self.parse(args="-c %s" % config_file.name)
         self.assertEqual(ns.x, "bla")
 
     def testConstructor_ConfigFileArgs(self):
         # Test constructor args:
         #   args_for_setting_config_path
         #   config_arg_is_required
         #   config_arg_help_message
-        temp_cfg = tempfile.NamedTemporaryFile(mode="w", delete=True)
+        temp_cfg = tempfile.NamedTemporaryFile(mode="w", delete=False)
         temp_cfg.write("genome=hg19")
         temp_cfg.flush()
 
         self.initParser(args_for_setting_config_path=["-c", "--config"],
                         config_arg_is_required = True,
                         config_arg_help_message = "my config file",
                         default_config_files=[temp_cfg.name])
         self.add_arg('--genome', help='Path to genome file', required=True)
         self.assertParseArgsRaises("argument -c/--config is required"
                                    if sys.version_info.major < 3 else
                                    "arguments are required: -c/--config",
                                    args="")
 
-        temp_cfg2 = tempfile.NamedTemporaryFile(mode="w", delete=True)
+        temp_cfg2 = tempfile.NamedTemporaryFile(mode="w", delete=False)
         ns = self.parse("-c " + temp_cfg2.name)
         self.assertEqual(ns.genome, "hg19")
 
         # temp_cfg2 config file should override default config file values
         temp_cfg2.write("genome=hg20")
         temp_cfg2.flush()
         ns = self.parse("-c " + temp_cfg2.name)
@@ -898,15 +898,15 @@
         ns, args = self.parse_known(config_file_contents="arg1 = 3")
         self.assertEqual(getattr(ns, "arg1", ""), "")
 
     def test_AbbrevConfigFileArgs(self):
         """Tests that abbreviated values don't get pulled from config file.
 
         """
-        temp_cfg = tempfile.NamedTemporaryFile(mode="w", delete=True)
+        temp_cfg = tempfile.NamedTemporaryFile(mode="w", delete=False)
         temp_cfg.write("a2a = 0.5\n")
         temp_cfg.write("a3a = 0.5\n")
         temp_cfg.flush()
 
         self.initParser()
 
         self.add_arg('-c', '--config_file', required=False, is_config_file=True,
@@ -930,28 +930,27 @@
         self.add_arg('--arg1', help='Arg1 help text', required=True)
         self.add_arg('--flag', help='Flag help text', action="store_true")
 
         self.assertRegex(self.format_help(),
             r'usage: .* \[-h\] -c CONFIG_FILE\s+'
             r'\[-w CONFIG_OUTPUT_PATH\]\s* --arg1\s+ARG1\s*\[--flag\]\s*'
             '%s:\\s*'
-            '-h, --help \\s* show this help message and exit\n\\s*'
-            r'-c CONFIG_FILE, --config CONFIG_FILE\s+my config file\s*'
-            r'-w CONFIG_OUTPUT_PATH, --write-config CONFIG_OUTPUT_PATH\s*takes\s*'
-            r'the current command line args and writes them\s*'
-            r'out to a config file at the given path, then exits\s*'
-            r'--arg1 ARG1\s*Arg1 help text\s*'
-            r'--flag \s*Flag help text\s*'
-            'Args that start with \'--\' \\(eg. --arg1\\) can also be set in a '
-            r'config file\s*\(~/.myconfig or specified via -c\).\s*'
-            r'Config file syntax allows: key=value,\s*flag=true, stuff=\[a,b,c\] '
-            r'\(for details, see syntax at https://goo.gl/R74nmi\).\s*'
-            r'If an arg is specified in more than\s*one place, then '
-            r'commandline values\s*override config file values which override\s*'
-            r'defaults.'%OPTIONAL_ARGS_STRING
+            '-h, --help \\s* show this help message and exit '
+            r'-c CONFIG_FILE, --config CONFIG_FILE\s+my config file '
+            r'-w CONFIG_OUTPUT_PATH, --write-config CONFIG_OUTPUT_PATH takes '
+            r'the current command line args and writes them '
+            r'out to a config file at the given path, then exits '
+            r'--arg1 ARG1 Arg1 help text '
+            r'--flag Flag help text '
+            'Args that start with \'--\' can also be set in a '
+            r'config file \(~/.myconfig or specified via -c\). '
+            r'Config file syntax allows: key=value, flag=true, stuff=\[a,b,c\] '
+            r'\(for details, see syntax at https://goo.gl/R74nmi\). '
+            r'In general, command-line values override config file values '
+            r'which override defaults. '.replace(' ', '\s*') % OPTIONAL_ARGS_STRING
         )
 
     def test_FormatHelpProg(self):
         self.initParser('format_help_prog')
         self.assertRegex(self.format_help(), 'usage: format_help_prog .*')
 
     def test_FormatHelpProgLib(self):
@@ -970,15 +969,15 @@
         if s == "invalid": raise Exception("invalid name")
         return TestMisc.CustomClass(s)
 
     def testConstructor_WriteOutConfigFileArgs(self):
         # Test constructor args:
         #   args_for_writing_out_config_file
         #   write_out_config_file_arg_help_message
-        cfg_f = tempfile.NamedTemporaryFile(mode="w+", delete=True)
+        cfg_f = tempfile.NamedTemporaryFile(mode="w+", delete=False)
         self.initParser(args_for_writing_out_config_file=["-w"],
                         write_out_config_file_arg_help_message="write config")
 
 
         self.add_arg("-not-config-file-settable")
         self.add_arg("--config-file-settable-arg", type=int)
         self.add_arg("--config-file-settable-arg2", type=int, default=3)
@@ -1011,15 +1010,15 @@
             self.parse, args = command_line_args + " -w /")
         cfg_f.close()
 
     def testConstructor_WriteOutConfigFileArgs2(self):
         # Test constructor args:
         #   args_for_writing_out_config_file
         #   write_out_config_file_arg_help_message
-        cfg_f = tempfile.NamedTemporaryFile(mode="w+", delete=True)
+        cfg_f = tempfile.NamedTemporaryFile(mode="w+", delete=False)
         self.initParser(args_for_writing_out_config_file=["-w"],
                         write_out_config_file_arg_help_message="write config")
 
 
         self.add_arg("-not-config-file-settable")
         self.add_arg("-a", "--arg1", type=int, env_var="ARG1")
         self.add_arg("-b", "--arg2", type=int, default=3)
@@ -1062,15 +1061,15 @@
         There was a bug where the long version of the
         args_for_writing_out_config_file was being dumped into the resultant
         output config file
         """
         # Test constructor args:
         #   args_for_writing_out_config_file
         #   write_out_config_file_arg_help_message
-        cfg_f = tempfile.NamedTemporaryFile(mode="w+", delete=True)
+        cfg_f = tempfile.NamedTemporaryFile(mode="w+", delete=False)
         self.initParser(args_for_writing_out_config_file=["--write-config"],
                         write_out_config_file_arg_help_message="write config")
 
 
         self.add_arg("-not-config-file-settable")
         self.add_arg("--config-file-settable-arg", type=int)
         self.add_arg("--config-file-settable-arg2", type=int, default=3)
@@ -1483,15 +1482,39 @@
 
         # test serialize
         output_config_str = p.serialize(parsed_obj)
         self.assertEqual(input_config_str.getvalue(), output_config_str)
 
         self.assertDictEqual(parsed_obj, {'a': '3', 'list_arg': [1,2,3]})
 
-
+    def testYAMLConfigFileParser_w_ArgumentParser_parsed_values(self):
+        try:
+            import yaml
+        except:
+            raise AssertionError("WARNING: PyYAML not installed. "
+                            "Couldn't test YAMLConfigFileParser")
+            return
+        
+        parser = configargparse.ArgumentParser(config_file_parser_class=configargparse.YAMLConfigFileParser)
+        parser.add_argument('-c', '--config', is_config_file=True)
+        parser.add_argument('--verbosity', action='count')
+        parser.add_argument('--verbose', action='store_true')
+        parser.add_argument('--level', type=int)
+
+        config_lines = ["verbosity: 3", 
+                        "verbose: true", 
+                        "level: 35"]
+        config_str = "\n".join(config_lines)+"\n"
+        config_file = tempfile.gettempdir()+"/temp_YAMLConfigFileParser.cfg"
+        with open(config_file, 'w') as f:
+            f.write(config_str)
+        args = parser.parse_args(["--config=%s"%config_file])
+        assert args.verbosity == 3
+        assert args.verbose == True
+        assert args.level == 35
 
 ################################################################################
 # since configargparse should work as a drop-in replacement for argparse
 # in all situations, run argparse unittests on configargparse by modifying
 # their source code to use configargparse.ArgumentParser
 
 try:
```

### Comparing `ConfigArgParse-1.5.3/configargparse.py` & `ConfigArgParse-1.5.5/configargparse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 A drop-in replacement for `argparse` that allows options to also be set via config files and/or environment variables.
 
 :see: `configargparse.ArgumentParser`, `configargparse.add_argument`
 """
 import argparse
+import ast
+import csv
+import functools
 import json
 import glob
 import os
 import re
 import sys
 import types
 from collections import OrderedDict
@@ -86,15 +89,15 @@
         raise NotImplementedError("get_syntax_description(..) not implemented")
 
     def parse(self, stream):
         """Parses the keys and values from a config file.
 
         NOTE: For keys that were specified to configargparse as
         action="store_true" or "store_false", the config file value must be
-        one of: "yes", "no", "true", "false". Otherwise an error will be raised.
+        one of: "yes", "no", "on", "off", "true", "false". Otherwise an error will be raised.
 
         Args:
             stream (IO): A config file input stream (such as an open file object).
 
         Returns:
             OrderedDict: Items where the keys are strings and the
             values are either strings or lists (eg. to support config file
@@ -291,22 +294,29 @@
         on it unless this parser is used."""
         try:
             import yaml
         except ImportError:
             raise ConfigFileParserException("Could not import yaml. "
                 "It can be installed by running 'pip install PyYAML'")
 
-        return yaml
+        try:
+            from yaml import CSafeLoader as SafeLoader
+            from yaml import CDumper as Dumper
+        except ImportError:
+            from yaml import SafeLoader
+            from yaml import Dumper
+
+        return yaml, SafeLoader, Dumper
 
     def parse(self, stream):
         # see ConfigFileParser.parse docstring
-        yaml = self._load_yaml()
+        yaml, SafeLoader, _ = self._load_yaml()
 
         try:
-            parsed_obj = yaml.safe_load(stream)
+            parsed_obj = yaml.load(stream, Loader=SafeLoader)
         except Exception as e:
             raise ConfigFileParserException("Couldn't parse config file: %s" % e)
 
         if not isinstance(parsed_obj, dict):
             raise ConfigFileParserException("The config file doesn't appear to "
                 "contain 'key: value' pairs (aka. a YAML mapping). "
                 "yaml.load('%s') returned type '%s' instead of 'dict'." % (
@@ -323,20 +333,339 @@
 
         return result
 
     def serialize(self, items, default_flow_style=False):
         # see ConfigFileParser.serialize docstring
 
         # lazy-import so there's no dependency on yaml unless this class is used
-        yaml = self._load_yaml()
+        yaml, _, Dumper = self._load_yaml()
 
         # it looks like ordering can't be preserved: http://pyyaml.org/ticket/29
         items = dict(items)
-        return yaml.dump(items, default_flow_style=default_flow_style)
+        return yaml.dump(items, default_flow_style=default_flow_style, Dumper=Dumper)
+
+
+"""
+Provides `configargparse.ConfigFileParser` classes to parse ``TOML`` and ``INI`` files with **mandatory** support for sections.
+Useful to integrate configuration into project files like ``pyproject.toml`` or ``setup.cfg``.
+
+`TomlConfigParser` usage: 
+
+>>> TomlParser = TomlConfigParser(['tool.my_super_tool']) # Simple TOML parser.
+>>> parser = ArgumentParser(..., default_config_files=['./pyproject.toml'], config_file_parser_class=TomlParser)
+
+`IniConfigParser` works the same way (also it optionaly convert multiline strings to list with argument ``split_ml_text_to_list``).
+
+`CompositeConfigParser` usage:
+
+>>> MY_CONFIG_SECTIONS = ['tool.my_super_tool', 'tool:my_super_tool', 'my_super_tool']
+>>> TomlParser =  TomlConfigParser(MY_CONFIG_SECTIONS)
+>>> IniParser = IniConfigParser(MY_CONFIG_SECTIONS, split_ml_text_to_list=True)
+>>> MixedParser = CompositeConfigParser([TomlParser, IniParser]) # This parser supports both TOML and INI formats.
+>>> parser = ArgumentParser(..., default_config_files=['./pyproject.toml', 'setup.cfg', 'my_super_tool.ini'], config_file_parser_class=MixedParser)
+
+"""
+
+# I did not invented these regex, just put together some stuff from:
+# - https://stackoverflow.com/questions/11859442/how-to-match-string-in-quotes-using-regex
+# - and https://stackoverflow.com/a/41005190
+
+_QUOTED_STR_REGEX = re.compile(r'(^\"(?:\\.|[^\"\\])*\"$)|'
+                               r'(^\'(?:\\.|[^\'\\])*\'$)')
+
+_TRIPLE_QUOTED_STR_REGEX = re.compile(r'(^\"\"\"(\s+)?(([^\"]|\"([^\"]|\"[^\"]))*(\"\"?)?)?(\s+)?(?:\\.|[^\"\\])?\"\"\"$)|'
+                                                                                                 # Unescaped quotes at the end of a string generates 
+                                                                                                 # "SyntaxError: EOL while scanning string literal", 
+                                                                                                 # so we don't account for those kind of strings as quoted.
+                                      r'(^\'\'\'(\s+)?(([^\']|\'([^\']|\'[^\']))*(\'\'?)?)?(\s+)?(?:\\.|[^\'\\])?\'\'\'$)', flags=re.DOTALL)
+
+@functools.lru_cache(maxsize=256, typed=True)
+def is_quoted(text, triple=True):
+    """
+    Detect whether a string is a quoted representation. 
+
+    :param triple: Also match tripple quoted strings.
+    """
+    return bool(_QUOTED_STR_REGEX.match(text)) or \
+        (triple and bool(_TRIPLE_QUOTED_STR_REGEX.match(text)))
+
+def unquote_str(text, triple=True):
+    """
+    Unquote a maybe quoted string representation. 
+    If the string is not detected as being a quoted representation, it returns the same string as passed.
+    It supports all kinds of python quotes: ``\"\"\"``, ``'''``, ``"`` and ``'``.
+
+    :param triple: Also unquote tripple quoted strings.
+    @raises ValueError: If the string is detected as beeing quoted but literal_eval() fails to evaluate it as string.
+        This would be a bug in the regex. 
+    """
+    if is_quoted(text, triple=triple):
+        try:
+            s = ast.literal_eval(text)
+            assert isinstance(s, str)
+        except Exception as e:
+            raise ValueError(f"Error trying to unquote the quoted string: {text}: {e}") from e
+        return s
+    return text
+
+def parse_toml_section_name(section_name):
+    """
+    Parse a TOML section name to a sequence of strings.
 
+    The following names are all valid: 
+
+    .. python::
+
+        "a.b.c"            # this is best practice -> returns ("a", "b", "c")
+        " d.e.f "          # same as [d.e.f] -> returns ("d", "e", "f")
+        " g .  h  . i "    # same as [g.h.i] -> returns ("g", "h", "i")
+        ' j . "ʞ" . "l" '  # same as [j."ʞ"."l"], double or simple quotes here are supported. -> returns ("j", "ʞ", "l")
+    """
+    section = []
+    for row in csv.reader([section_name], delimiter='.'):
+        for a in row:
+            section.append(unquote_str(a.strip(), triple=False))
+    return tuple(section)
+
+def get_toml_section(data, section):
+    """
+    Given some TOML data (as loaded with `toml.load()`), returns the requested section of the data.
+    Returns ``None`` if the section is not found.
+    """
+    sections = parse_toml_section_name(section) if isinstance(section, str) else section
+    itemdata = data.get(sections[0])
+    if not itemdata:
+        return None
+    sections = sections[1:]
+    if sections:
+        return get_toml_section(itemdata, sections)
+    else:
+        if not isinstance(itemdata, dict):
+            return None
+        return itemdata
+
+class TomlConfigParser(ConfigFileParser):
+    """
+    Create a TOML parser bounded to the list of provided sections.
+
+    Example::
+        # this is a comment
+        [tool.my-software] # TOML section table.
+        # how to specify a key-value pair
+        format-string = "restructuredtext" # strings must be quoted
+        # how to set an arg which has action="store_true"
+        warnings-as-errors = true
+        # how to set an arg which has action="count" or type=int
+        verbosity = 1
+        # how to specify a list arg (eg. arg which has action="append")
+        repeatable-option = ["https://docs.python.org/3/objects.inv",
+                       "https://twistedmatrix.com/documents/current/api/objects.inv"]
+        # how to specify a multiline text:
+        multi-line-text = '''
+            Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+            Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+            Maecenas quis dapibus leo, a pellentesque leo. 
+            '''
+
+    Note that the config file fragment above is also valid for the `IniConfigParser` class and would be parsed the same manner. 
+    Thought, any valid TOML config file will not be necessarly parsable with `IniConfigParser` (INI files must be rigorously indented whereas TOML files).
+    
+    See the `TOML specification <>`_ for details. 
+    """
+
+    def __init__(self, sections):
+        """
+        :param sections: The section names bounded to the new parser.
+        """
+        super().__init__()
+        self.sections = sections
+    
+    def __call__(self):
+        return self
+
+    def parse(self, stream):
+        """Parses the keys and values from a TOML config file."""
+        # parse with configparser to allow multi-line values
+        import toml
+        try:
+            config = toml.load(stream)
+        except Exception as e:
+            raise ConfigFileParserException("Couldn't parse TOML file: %s" % e)
+
+        # convert to dict and filter based on section names
+        result = OrderedDict()
+
+        for section in self.sections:
+            data = get_toml_section(config, section)
+            if data:
+                # Seems a little weird, but anything that is not a list is converted to string, 
+                # It will be converted back to boolean, int or whatever after.
+                # Because config values are still passed to argparser for computation.
+                for key, value in data.items():
+                    if isinstance(value, list):
+                        result[key] = value
+                    elif value is None:
+                        pass
+                    else:
+                        result[key] = str(value)
+                break
+        
+        return result
+
+    def get_syntax_description(self):
+        return ("Config file syntax is Tom's Obvious, Minimal Language. "
+                "See https://github.com/toml-lang/toml/blob/v0.5.0/README.md for details.")
+
+class IniConfigParser(ConfigFileParser):
+    """
+    Create a INI parser bounded to the list of provided sections.
+    Optionaly convert multiline strings to list.
+
+    Example (if split_ml_text_to_list=False)::
+
+        # this is a comment
+        ; also a comment
+        [my-software]
+        # how to specify a key-value pair
+        format-string: restructuredtext 
+        # white space are ignored, so name = value same as name=value
+        # this is why you can quote strings 
+        quoted-string = '\thello\tmom...  '
+        # how to set an arg which has action="store_true"
+        warnings-as-errors = true
+        # how to set an arg which has action="count" or type=int
+        verbosity = 1
+        # how to specify a list arg (eg. arg which has action="append")
+        repeatable-option = ["https://docs.python.org/3/objects.inv",
+                       "https://twistedmatrix.com/documents/current/api/objects.inv"]
+        # how to specify a multiline text:
+        multi-line-text = 
+            Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+            Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+            Maecenas quis dapibus leo, a pellentesque leo. 
+    
+    Example (if split_ml_text_to_list=True)::
+
+        # the same rules are applicable with the following changes:
+        [my-software]
+        # how to specify a list arg (eg. arg which has action="append")
+        repeatable-option = # Just enter one value per line (the list literal format can also be used)
+            https://docs.python.org/3/objects.inv
+            https://twistedmatrix.com/documents/current/api/objects.inv
+        # how to specify a multiline text (you have to quote it):
+        multi-line-text = '''
+            Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+            Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+            Maecenas quis dapibus leo, a pellentesque leo. 
+            '''
+    """
+
+    def __init__(self, sections, split_ml_text_to_list):
+        """
+        :param sections: The section names bounded to the new parser.
+        :split_ml_text_to_list: Wether to convert multiline strings to list
+        """
+        super().__init__()
+        self.sections = sections
+        self.split_ml_text_to_list = split_ml_text_to_list
+
+    def __call__(self):
+        return self
+
+    def parse(self, stream):
+        """Parses the keys and values from an INI config file."""
+        # parse with configparser to allow multi-line values
+        import configparser
+        config = configparser.ConfigParser()
+        try:
+            config.read_string(stream.read())
+        except Exception as e:
+            raise ConfigFileParserException("Couldn't parse INI file: %s" % e)
+
+        # convert to dict and filter based on INI section names
+        result = OrderedDict()
+        for section in config.sections() + [configparser.DEFAULTSECT]:
+            if section not in self.sections:
+                continue
+            for k,v in config[section].items():
+                strip_v = v.strip()
+                if not strip_v:
+                    # ignores empty values, anyway allow_no_value=False by default so this should not happend.
+                    continue
+                # evaluate lists
+                if strip_v.startswith('[') and strip_v.endswith(']'):
+                    try:
+                        result[k] = ast.literal_eval(strip_v)
+                    except ValueError as e:
+                        # error evaluating object
+                        raise ConfigFileParserException("Error evaluating list: " + str(e) + ". Put quotes around your text if it's meant to be a string.") from e
+                else:
+                    if is_quoted(strip_v):
+                        # evaluate quoted string
+                        try:
+                            result[k] = unquote_str(strip_v)
+                        except ValueError as e:
+                            # error unquoting string
+                            raise ConfigFileParserException(str(e)) from e
+                    # split multi-line text into list of strings if split_ml_text_to_list is enabled.
+                    elif self.split_ml_text_to_list and '\n' in v.rstrip('\n'):
+                        try:
+                            result[k] = [unquote_str(i) for i in strip_v.split('\n') if i]
+                        except ValueError as e:
+                            # error unquoting string
+                            raise ConfigFileParserException(str(e)) from e
+                    else:
+                        result[k] = v
+        return result
+
+    def get_syntax_description(self):
+        msg = ("Uses configparser module to parse an INI file which allows multi-line values. "
+                "See https://docs.python.org/3/library/configparser.html for details. "
+                "This parser includes support for quoting strings literal as well as python list syntax evaluation. ")
+        if self.split_ml_text_to_list:
+            msg += ("Alternatively lists can be constructed with a plain multiline string, "
+                "each non-empty line will be converted to a list item.")
+        return msg
+
+class CompositeConfigParser(ConfigFileParser):
+    """
+    Createa a config parser composed by others `ConfigFileParser`s.  
+
+    The composite parser will successively try to parse the file with each parser, 
+    until it succeeds, else raise execption with all encountered errors. 
+    """
+
+    def __init__(self, config_parser_types):
+        super().__init__()
+        self.parsers = [p() for p in config_parser_types]
+
+    def __call__(self):
+        return self
+
+    def parse(self, stream):
+        errors = []
+        for p in self.parsers:
+            try:
+                return p.parse(stream) # type: ignore[no-any-return]
+            except Exception as e:
+                stream.seek(0)
+                errors.append(e)
+        raise ConfigFileParserException(
+                f"Error parsing config: {', '.join(repr(str(e)) for e in errors)}")
+    
+    def get_syntax_description(self) :
+        def guess_format_name(classname):
+            strip = classname.lower().strip('_').replace('parser', 
+                '').replace('config', '').replace('file', '')
+            return strip.upper() if strip else '??'
+        
+        msg = "Uses multiple config parser settings (in order): \n"
+        for i, parser in enumerate(self.parsers): 
+            msg += f"[{i+1}] {guess_format_name(parser.__class__.__name__)}: {parser.get_syntax_description()} \n"
+        return msg
 
 # used while parsing args to keep track of where they came from
 _COMMAND_LINE_SOURCE_KEY = "command_line"
 _ENV_VAR_SOURCE_KEY = "environment_variables"
 _CONFIG_FILE_SOURCE_KEY = "config_file"
 _DEFAULTS_SOURCE_KEY = "defaults"
 
@@ -584,15 +913,15 @@
             config_streams = self._open_config_files(args)
 
         # parse each config file
         for stream in reversed(config_streams):
             try:
                 config_items = self._config_file_parser.parse(stream)
             except ConfigFileParserException as e:
-                self.error(e)
+                self.error(str(e))
             finally:
                 if hasattr(stream, "close"):
                     stream.close()
 
             # add each config item to the commandline unless it's there already
             config_args = []
             nargs = False
@@ -667,16 +996,16 @@
         - "defaults"
         Each such key, will be mapped to another dictionary containing the options set via that method. Here the key
         will be the option name, and the value will be a 2-tuple of the form (`argparse.Action` obj, `str` value).
 
         Returns:
             dict[str, dict[str, tuple[argparse.Action, str]]]: source to settings dict
         """
-
-        return self._source_to_settings
+        # _source_to_settings is set in parse_know_args().
+        return self._source_to_settings # type:ignore[attribute-error]
 
 
     def write_config_file(self, parsed_namespace, output_file_paths, exit_after=False):
         """Write the given settings to output files.
 
         Args:
             parsed_namespace: namespace object created within parse_known_args()
@@ -788,35 +1117,36 @@
                 self.get_command_line_key_for_unknown_config_file_setting(key)
         else:
             if not is_boolean_optional_action(action):
                 command_line_key = action.option_strings[-1]
 
         # handle boolean value
         if action is not None and isinstance(action, ACTION_TYPES_THAT_DONT_NEED_A_VALUE):
-            if value.lower() in ("true", "yes", "1"):
+            assert isinstance(value, str), "config parser should convert anything that is not a list to string."
+            if value.lower() in ("true", "yes", "on", "1"):
                 if not is_boolean_optional_action(action):
                     args.append( command_line_key )
                 else:
                     # --foo
                     args.append(action.option_strings[0])
-            elif value.lower() in ("false", "no", "0"):
+            elif value.lower() in ("false", "no", "off", "0"):
                 # don't append when set to "false" / "no"
                 if not is_boolean_optional_action(action):
                     pass
                 else:
                     # --no-foo
                     args.append(action.option_strings[1])
             elif isinstance(action, argparse._CountAction):
                 for arg in args:
                     if any([arg.startswith(s) for s in action.option_strings]):
                         value = 0
                 args += [action.option_strings[0]] * int(value)
             else:
                 self.error("Unexpected value for %s: '%s'. Expecting 'true', "
-                           "'false', 'yes', 'no', '1' or '0'" % (key, value))
+                           "'false', 'yes', 'no', 'on', 'off', '1' or '0'" % (key, value))
         elif isinstance(value, list):
             accepts_list_and_has_nargs = action is not None and action.nargs is not None and (
                    isinstance(action, argparse._StoreAction) or isinstance(action, argparse._AppendAction)
             ) and (
                 action.nargs in ('+', '*') or (isinstance(action.nargs, int) and action.nargs > 1)
             )
 
@@ -949,15 +1279,15 @@
             _COMMAND_LINE_SOURCE_KEY: "Command Line Args: ",
             _ENV_VAR_SOURCE_KEY: "Environment Variables:\n",
             _CONFIG_FILE_SOURCE_KEY: "Config File (%s):\n",
             _DEFAULTS_SOURCE_KEY: "Defaults:\n"
         }
 
         r = StringIO()
-        for source, settings in self._source_to_settings.items():
+        for source, settings in self._source_to_settings.items(): #type:ignore[argument-error]
             source = source.split("|")
             source = source_key_to_display_value_map[source[0]] % tuple(source[1:])
             r.write(source)
             for key, (action, value) in settings.items():
                 if key:
                     r.write("  {:<19}{}\n".format(key+":", value))
                 else:
@@ -987,16 +1317,16 @@
                 self._actions if getattr(a, "is_config_file_arg", False)]
 
             if config_settable_args and (default_config_files or
                                          config_path_actions):
                 self._add_config_file_help = False  # prevent duplication
                 added_config_file_help = True
 
-                msg += ("Args that start with '%s' (eg. %s) can also be set in "
-                        "a config file") % (cc, config_settable_args[0][0])
+                msg += ("Args that start with '%s' can also be set in "
+                        "a config file") % cc
                 config_arg_string = " or ".join(a.option_strings[0]
                     for a in config_path_actions if a.option_strings)
                 if config_arg_string:
                     config_arg_string = "specified via " + config_arg_string
                 if default_config_files or config_arg_string:
                     msg += " (%s)." % " or ".join(tuple(default_config_files) +
                                                   tuple(filter(None, [config_arg_string])))
@@ -1018,16 +1348,15 @@
 
         if added_env_var_help or added_config_file_help:
             value_sources = ["defaults"]
             if added_config_file_help:
                 value_sources = ["config file values"] + value_sources
             if added_env_var_help:
                 value_sources = ["environment variables"] + value_sources
-            msg += (" If an arg is specified in more than one place, then "
-                "commandline values override %s.") % (
+            msg += " In general, command-line values override %s." % (
                 " which override ".join(value_sources))
 
         text_width = max(self._get_formatter()._width, 11)
         msg = textwrap.fill(msg, text_width)
 
         return (argparse.ArgumentParser.format_help(self)
               + ("\n{}\n".format(msg) if msg != "" else ""))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ConfigArgParse-1.5.3/setup.py` & `ConfigArgParse-1.5.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,17 @@
         logging.error("ERROR: while starting an HTTP server to serve "
                       "the coverage report: %s" % e)
 
 
 command = sys.argv[-1]
 if command == 'publish':
     os.system('rm -rf dist')    
-    os.system('python setup.py sdist')
+    os.system('python3 setup.py sdist')
     os.system('python3 setup.py bdist_wheel')
+    os.system('twine check dist/*')  # check for formatting or other issues that would cause twine upload to error out
     os.system('twine upload dist/*whl dist/*gz')
     sys.exit()
 elif command == "coverage":
     try:
         import coverage
     except:
         sys.exit("coverage.py not installed (pip install --user coverage)")
@@ -77,15 +78,15 @@
     'PyYAML',
     'pytest',
 ]
 
 
 setup(
     name='ConfigArgParse',
-    version="1.5.3",
+    version="1.5.5",
     description='A drop-in replacement for argparse that allows options to '
                 'also be set via config files and/or environment variables.',
     long_description=long_description,
     url='https://github.com/bw2/ConfigArgParse',
     py_modules=['configargparse'],
     include_package_data=True,
     license="MIT",
```

### Comparing `ConfigArgParse-1.5.3/ConfigArgParse.egg-info/PKG-INFO` & `ConfigArgParse-1.5.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,491 +1,14 @@
 Metadata-Version: 2.1
 Name: ConfigArgParse
-Version: 1.5.3
+Version: 1.5.5
 Summary: A drop-in replacement for argparse that allows options to also be set via config files and/or environment variables.
 Home-page: https://github.com/bw2/ConfigArgParse
 License: MIT
-Description: ConfigArgParse
-        --------------
-        
-        .. image:: https://img.shields.io/pypi/v/ConfigArgParse.svg?style=flat
-            :alt: PyPI version
-            :target: https://pypi.python.org/pypi/ConfigArgParse
-        
-        .. image:: https://img.shields.io/pypi/pyversions/ConfigArgParse.svg
-            :alt: Supported Python versions
-            :target: https://pypi.python.org/pypi/ConfigArgParse
-        
-        .. image:: https://travis-ci.org/bw2/ConfigArgParse.svg?branch=master
-            :alt: Travis CI build
-            :target: https://travis-ci.org/bw2/ConfigArgParse
-        
-        .. image:: https://img.shields.io/badge/-API_Documentation-blue
-            :alt: API Documentation
-            :target: https://bw2.github.io/ConfigArgParse/
-        
-        Overview
-        ~~~~~~~~
-        
-        Applications with more than a handful of user-settable options are best
-        configured through a combination of command line args, config files,
-        hard-coded defaults, and in some cases, environment variables.
-        
-        Python's command line parsing modules such as argparse have very limited
-        support for config files and environment variables, so this module
-        extends argparse to add these features.
-        
-        Available on PyPI: http://pypi.python.org/pypi/ConfigArgParse
-        
-        .. image:: https://travis-ci.org/bw2/ConfigArgParse.svg?branch=master
-            :target: https://travis-ci.org/bw2/ConfigArgParse
-        
-        Features
-        ~~~~~~~~
-        
-        -  command-line, config file, env var, and default settings can now be
-           defined, documented, and parsed in one go using a single API (if a
-           value is specified in more than one way then: command line >
-           environment variables > config file values > defaults)
-        -  config files can have .ini or .yaml style syntax (eg. key=value or
-           key: value)
-        -  user can provide a config file via a normal-looking command line arg
-           (eg. -c path/to/config.txt) rather than the argparse-style @config.txt
-        -  one or more default config file paths can be specified
-           (eg. ['/etc/bla.conf', '~/.my_config'] )
-        -  all argparse functionality is fully supported, so this module can
-           serve as a drop-in replacement (verified by argparse unittests).
-        -  env vars and config file keys & syntax are automatically documented
-           in the -h help message
-        -  new method :code:`print_values()` can report keys & values and where
-           they were set (eg. command line, env var, config file, or default).
-        -  lite-weight (no 3rd-party library dependencies except (optionally) PyYAML)
-        -  extensible (:code:`ConfigFileParser` can be subclassed to define a new
-           config file format)
-        -  unittested by running the unittests that came with argparse but on
-           configargparse, and using tox to test with Python 2.7 and Python 3+
-        
-        Example
-        ~~~~~~~
-        
-        *config_test.py*:
-        
-        Script that defines 4 options and a positional arg and then parses and prints the values. Also,
-        it prints out the help message as well as the string produced by :code:`format_values()` to show
-        what they look like.
-        
-        .. code:: py
-        
-           import configargparse
-        
-           p = configargparse.ArgParser(default_config_files=['/etc/app/conf.d/*.conf', '~/.my_settings'])
-           p.add('-c', '--my-config', required=True, is_config_file=True, help='config file path')
-           p.add('--genome', required=True, help='path to genome file')  # this option can be set in a config file because it starts with '--'
-           p.add('-v', help='verbose', action='store_true')
-           p.add('-d', '--dbsnp', help='known variants .vcf', env_var='DBSNP_PATH')  # this option can be set in a config file because it starts with '--'
-           p.add('vcf', nargs='+', help='variant file(s)')
-        
-           options = p.parse_args()
-        
-           print(options)
-           print("----------")
-           print(p.format_help())
-           print("----------")
-           print(p.format_values())    # useful for logging where different settings came from
-        
-        
-        *config.txt:*
-        
-        Since the script above set the config file as required=True, lets create a config file to give it:
-        
-        .. code:: py
-        
-            # settings for config_test.py
-            genome = HCMV     # cytomegalovirus genome
-            dbsnp = /data/dbsnp/variants.vcf
-        
-        
-        *command line:*
-        
-        Now run the script and pass it the config file:
-        
-        .. code:: bash
-        
-            DBSNP_PATH=/data/dbsnp/variants_v2.vcf python config_test.py --my-config config.txt f1.vcf f2.vcf
-        
-        *output:*
-        
-        Here is the result:
-        
-        .. code:: bash
-        
-            Namespace(dbsnp='/data/dbsnp/variants_v2.vcf', genome='HCMV', my_config='config.txt', v=False, vcf=['f1.vcf', 'f2.vcf'])
-            ----------
-            usage: config_test.py [-h] -c MY_CONFIG --genome GENOME [-v] [-d DBSNP]
-                                  vcf [vcf ...]
-            
-            Args that start with '--' (eg. --genome) can also be set in a config file
-            (/etc/app/conf.d/*.conf or ~/.my_settings or specified via -c). Config file
-            syntax allows: key=value, flag=true, stuff=[a,b,c] (for details, see syntax at
-            https://goo.gl/R74nmi). If an arg is specified in more than one place, then
-            commandline values override environment variables which override config file
-            values which override defaults.
-            
-            positional arguments:
-              vcf                   variant file(s)
-            
-            optional arguments:
-              -h, --help            show this help message and exit
-              -c MY_CONFIG, --my-config MY_CONFIG
-                                    config file path
-              --genome GENOME       path to genome file
-              -v                    verbose
-              -d DBSNP, --dbsnp DBSNP
-                                    known variants .vcf [env var: DBSNP_PATH]
-            
-            ----------
-            Command Line Args:   --my-config config.txt f1.vcf f2.vcf
-            Environment Variables:
-              DBSNP_PATH:        /data/dbsnp/variants_v2.vcf
-            Config File (config.txt):
-              genome:            HCMV
-        
-        Special Values
-        ~~~~~~~~~~~~~~
-        
-        Under the hood, configargparse handles environment variables and config file
-        values by converting them to their corresponding command line arg. For
-        example, "key = value" will be processed as if "--key value" was specified
-        on the command line.
-        
-        Also, the following special values (whether in a config file or an environment
-        variable) are handled in a special way to support booleans and lists:
-        
-        -  :code:`key = true` is handled as if "--key" was specified on the command line.
-           In your python code this key must be defined as a boolean flag
-           (eg. action="store_true" or similar).
-        
-        -  :code:`key = [value1, value2, ...]` is handled as if "--key value1 --key value2"
-           etc. was specified on the command line. In your python code this key must
-           be defined as a list (eg. action="append").
-        
-        Config File Syntax
-        ~~~~~~~~~~~~~~~~~~
-        
-        Only command line args that have a long version (eg. one that starts with '--')
-        can be set in a config file. For example, "--color" can be set by putting
-        "color=green" in a config file. The config file syntax depends on the constuctor
-        arg: :code:`config_file_parser_class` which can be set to one of the provided
-        classes: :code:`DefaultConfigFileParser`, :code:`YAMLConfigFileParser`,
-        :code:`ConfigparserConfigFileParser` or to your own subclass of the
-        :code:`ConfigFileParser` abstract class.
-        
-        *DefaultConfigFileParser*  - the full range of valid syntax is:
-        
-        .. code:: yaml
-        
-                # this is a comment
-                ; this is also a comment (.ini style)
-                ---            # lines that start with --- are ignored (yaml style)
-                -------------------
-                [section]      # .ini-style section names are treated as comments
-        
-                # how to specify a key-value pair (all of these are equivalent):
-                name value     # key is case sensitive: "Name" isn't "name"
-                name = value   # (.ini style)  (white space is ignored, so name = value same as name=value)
-                name: value    # (yaml style)
-                --name value   # (argparse style)
-        
-                # how to set a flag arg (eg. arg which has action="store_true")
-                --name
-                name
-                name = True    # "True" and "true" are the same
-        
-                # how to specify a list arg (eg. arg which has action="append")
-                fruit = [apple, orange, lemon]
-                indexes = [1, 12, 35 , 40]
-        
-        
-        *YAMLConfigFileParser*  - allows a subset of YAML syntax (http://goo.gl/VgT2DU)
-        
-        .. code:: yaml
-        
-                # a comment
-                name1: value
-                name2: true    # "True" and "true" are the same
-        
-                fruit: [apple, orange, lemon]
-                indexes: [1, 12, 35, 40]
-        
-        *ConfigparserConfigFileParser*  - allows a subset of python's configparser
-        module syntax (https://docs.python.org/3.7/library/configparser.html). In
-        particular the following configparser options are set:
-        
-        .. code:: py
-        
-                config = configparser.ArgParser(
-                    delimiters=("=",":"),
-                    allow_no_value=False,
-                    comment_prefixes=("#",";"),
-                    inline_comment_prefixes=("#",";"),
-                    strict=True,
-                    empty_lines_in_values=False,
-                )
-        
-        Once configparser parses the config file all section names are removed, thus all
-        keys must have unique names regardless of which INI section they are defined
-        under. Also, any keys which have python list syntax are converted to lists by
-        evaluating them as python code using ast.literal_eval
-        (https://docs.python.org/3/library/ast.html#ast.literal_eval). To facilitate
-        this all multi-line values are converted to single-line values. Thus multi-line
-        string values will have all new-lines converted to spaces. Note, since key-value
-        pairs that have python dictionary syntax are saved as single-line strings, even
-        if formatted across multiple lines in the config file, dictionaries can be read
-        in and converted to valid python dictionaries with PyYAML's safe_load. Example
-        given below:
-        
-        .. code:: py
-        
-                # inside your config file (e.g. config.ini)
-                [section1]  # INI sections treated as comments
-                system1_settings: { # start of multi-line dictionary
-                    'a':True,
-                    'b':[2, 4, 8, 16],
-                    'c':{'start':0, 'stop':1000},
-                    'd':'experiment 32 testing simulation with parameter a on'
-                    } # end of multi-line dictionary value
-        
-                .......
-        
-                # in your configargparse setup
-                import configargparse
-                import yaml
-        
-                parser = configargparse.ArgParser(
-                    config_file_parser_class=configargparse.ConfigparserConfigFileParser
-                )
-                parser.add_argument('--system1_settings', type=yaml.safe_load)
-                
-                args = parser.parse_args() # now args.system1 is a valid python dict
-        
-        
-        ArgParser Singletons
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        To make it easier to configure different modules in an application,
-        configargparse provides globally-available ArgumentParser instances
-        via configargparse.get_argument_parser('name') (similar to
-        logging.getLogger('name')).
-        
-        Here is an example of an application with a utils module that also
-        defines and retrieves its own command-line args.
-        
-        *main.py*
-        
-        .. code:: py
-        
-            import configargparse
-            import utils
-        
-            p = configargparse.get_argument_parser()
-            p.add_argument("-x", help="Main module setting")
-            p.add_argument("--m-setting", help="Main module setting")
-            options = p.parse_known_args()   # using p.parse_args() here may raise errors.
-        
-        *utils.py*
-        
-        .. code:: py
-        
-            import configargparse
-            p = configargparse.get_argument_parser()
-            p.add_argument("--utils-setting", help="Config-file-settable option for utils")
-        
-            if __name__ == "__main__":
-               options = p.parse_known_args()
-        
-        Help Formatters
-        ~~~~~~~~~~~~~~~
-        
-        :code:`ArgumentDefaultsRawHelpFormatter` is a new HelpFormatter that both adds
-        default values AND disables line-wrapping. It can be passed to the constructor:
-        :code:`ArgParser(.., formatter_class=ArgumentDefaultsRawHelpFormatter)`
-        
-        
-        Aliases
-        ~~~~~~~
-        
-        The configargparse.ArgumentParser API inherits its class and method
-        names from argparse and also provides the following shorter names for
-        convenience:
-        
-        -  p = configargparse.get_arg_parser()  # get global singleton instance
-        -  p = configargparse.get_parser()
-        -  p = configargparse.ArgParser()  # create a new instance
-        -  p = configargparse.Parser()
-        -  p.add_arg(..)
-        -  p.add(..)
-        -  options = p.parse(..)
-        
-        HelpFormatters:
-        
-        - RawFormatter = RawDescriptionHelpFormatter
-        - DefaultsFormatter = ArgumentDefaultsHelpFormatter
-        - DefaultsRawFormatter = ArgumentDefaultsRawHelpFormatter
-        
-        API Documentation
-        ~~~~~~~~~~~~~~~~~
-        
-        You can review the generated API Documentation for the ``configargparse`` module: `HERE <https://bw2.github.io/ConfigArgParse/>`_
-        
-        Design Notes
-        ~~~~~~~~~~~~
-        
-        Unit tests:
-        
-        tests/test_configargparse.py contains custom unittests for features
-        specific to this module (such as config file and env-var support), as
-        well as a hook to load and run argparse unittests (see the built-in
-        test.test_argparse module) but on configargparse in place of argparse.
-        This ensures that configargparse will work as a drop in replacement for
-        argparse in all usecases.
-        
-        Previously existing modules (PyPI search keywords: config argparse):
-        
-        -  argparse (built-in module Python v2.7+)
-        
-           -  Good:
-        
-              -  fully featured command line parsing
-              -  can read args from files using an easy to understand mechanism
-        
-           -  Bad:
-        
-              -  syntax for specifying config file path is unusual (eg.
-                 @file.txt)and not described in the user help message.
-              -  default config file syntax doesn't support comments and is
-                 unintuitive (eg. --namevalue)
-              -  no support for environment variables
-        
-        -  ConfArgParse v1.0.15
-           (https://pypi.python.org/pypi/ConfArgParse)
-        
-           -  Good:
-        
-              -  extends argparse with support for config files parsed by
-                 ConfigParser
-              -  clear documentation in README
-        
-           -  Bad:
-        
-              -  config file values are processed using
-                 ArgumentParser.set_defaults(..) which means "required" and
-                 "choices" are not handled as expected. For example, if you
-                 specify a required value in a config file, you still have to
-                 specify it again on the command line.
-              -  doesn't work with Python 3 yet
-              -  no unit tests, code not well documented
-        
-        -  appsettings v0.5 (https://pypi.python.org/pypi/appsettings)
-        
-           -  Good:
-        
-              -  supports config file (yaml format) and env_var parsing
-              -  supports config-file-only setting for specifying lists and
-                 dicts
-        
-           -  Bad:
-        
-              -  passes in config file and env settings via parse_args
-                 namespace param
-              -  tests not finished and don't work with Python 3 (import
-                 StringIO)
-        
-        -  argparse_config v0.5.1
-           (https://pypi.python.org/pypi/argparse_config)
-        
-           -  Good:
-        
-              -  similar features to ConfArgParse v1.0.15
-        
-           -  Bad:
-        
-              -  doesn't work with Python 3 (error during pip install)
-        
-        -  yconf v0.3.2 - (https://pypi.python.org/pypi/yconf) - features
-           and interface not that great
-        -  hieropt v0.3 - (https://pypi.python.org/pypi/hieropt) - doesn't
-           appear to be maintained, couldn't find documentation
-        
-        -  configurati v0.2.3 - (https://pypi.python.org/pypi/configurati)
-        
-           -  Good:
-        
-              -  JSON, YAML, or Python configuration files
-              -  handles rich data structures such as dictionaries
-              -  can group configuration names into sections (like .ini files)
-        
-           -  Bad:
-        
-              -  doesn't work with Python 3
-              -  2+ years since last release to PyPI
-              -  apparently unmaintained
-        
-        
-        Design choices:
-        
-        1. all options must be settable via command line. Having options that
-           can only be set using config files or env. vars adds complexity to
-           the API, and is not a useful enough feature since the developer can
-           split up options into sections and call a section "config file keys",
-           with command line args that are just "--" plus the config key.
-        2. config file and env. var settings should be processed by appending
-           them to the command line (another benefit of #1). This is an
-           easy-to-implement solution and implicitly takes care of checking that
-           all "required" args are provied, etc., plus the behavior should be
-           easy for users to understand.
-        3. configargparse shouldn't override argparse's
-           convert_arg_line_to_args method so that all argparse unit tests
-           can be run on configargparse.
-        4. in terms of what to allow for config file keys, the "dest" value of
-           an option can't serve as a valid config key because many options can
-           have the same dest. Instead, since multiple options can't use the
-           same long arg (eg. "--long-arg-x"), let the config key be either
-           "--long-arg-x" or "long-arg-x". This means the developer can allow
-           only a subset of the command-line args to be specified via config
-           file (eg. short args like -x would be excluded). Also, that way
-           config keys are automatically documented whenever the command line
-           args are documented in the help message.
-        5. don't force users to put config file settings in the right .ini
-           [sections]. This doesn't have a clear benefit since all options are
-           command-line settable, and so have a globally unique key anyway.
-           Enforcing sections just makes things harder for the user and adds
-           complexity to the implementation.
-        6. if necessary, config-file-only args can be added later by
-           implementing a separate add method and using the namespace arg as in
-           appsettings_v0.5
-        
-        Relevant sites:
-        
-        -  http://stackoverflow.com/questions/6133517/parse-config-file-environment-and-command-line-arguments-to-get-a-single-coll
-        -  http://tricksntweaks.blogspot.com/2013_05_01_archive.html
-        -  http://www.youtube.com/watch?v=vvCwqHgZJc8#t=35
-        
-        
-        .. |Travis CI Status for bw2/ConfigArgParse| image:: https://travis-ci.org/bw2/ConfigArgParse.svg?branch=master
-        
-        
-        Versioning
-        ~~~~~~~~~~
-        
-        This software follows `Semantic Versioning`_
-        
-        .. _Semantic Versioning: http://semver.org/
-        
 Keywords: options,argparse,ConfigArgParse,config,environment variables,envvars,ENV,environment,optparse,YAML,INI
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -494,9 +17,607 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
-Provides-Extra: test
 Provides-Extra: yaml
+Provides-Extra: test
+License-File: LICENSE
+
+ConfigArgParse
+--------------
+
+.. image:: https://img.shields.io/pypi/v/ConfigArgParse.svg?style=flat
+    :alt: PyPI version
+    :target: https://pypi.python.org/pypi/ConfigArgParse
+
+.. image:: https://img.shields.io/pypi/pyversions/ConfigArgParse.svg
+    :alt: Supported Python versions
+    :target: https://pypi.python.org/pypi/ConfigArgParse
+
+.. image:: https://img.shields.io/badge/-API_Documentation-blue
+    :alt: API Documentation
+    :target: https://bw2.github.io/ConfigArgParse/
+
+Overview
+~~~~~~~~
+
+Applications with more than a handful of user-settable options are best
+configured through a combination of command line args, config files,
+hard-coded defaults, and in some cases, environment variables.
+
+Python's command line parsing modules such as argparse have very limited
+support for config files and environment variables, so this module
+extends argparse to add these features.
+
+Available on PyPI: http://pypi.python.org/pypi/ConfigArgParse
+
+
+Features
+~~~~~~~~
+
+-  command-line, config file, env var, and default settings can now be
+   defined, documented, and parsed in one go using a single API (if a
+   value is specified in more than one way then: command line >
+   environment variables > config file values > defaults)
+-  config files can have .ini or .yaml style syntax (eg. key=value or
+   key: value)
+-  user can provide a config file via a normal-looking command line arg
+   (eg. -c path/to/config.txt) rather than the argparse-style @config.txt
+-  one or more default config file paths can be specified
+   (eg. ['/etc/bla.conf', '~/.my_config'] )
+-  all argparse functionality is fully supported, so this module can
+   serve as a drop-in replacement (verified by argparse unittests).
+-  env vars and config file keys & syntax are automatically documented
+   in the -h help message
+-  new method :code:`print_values()` can report keys & values and where
+   they were set (eg. command line, env var, config file, or default).
+-  lite-weight (no 3rd-party library dependencies except (optionally) PyYAML)
+-  extensible (:code:`ConfigFileParser` can be subclassed to define a new
+   config file format)
+-  unittested by running the unittests that came with argparse but on
+   configargparse, and using tox to test with Python 2.7 and Python 3+
+
+Example
+~~~~~~~
+
+*config_test.py*:
+
+Script that defines 4 options and a positional arg and then parses and prints the values. Also,
+it prints out the help message as well as the string produced by :code:`format_values()` to show
+what they look like.
+
+.. code:: py
+
+   import configargparse
+
+   p = configargparse.ArgParser(default_config_files=['/etc/app/conf.d/*.conf', '~/.my_settings'])
+   p.add('-c', '--my-config', required=True, is_config_file=True, help='config file path')
+   p.add('--genome', required=True, help='path to genome file')  # this option can be set in a config file because it starts with '--'
+   p.add('-v', help='verbose', action='store_true')
+   p.add('-d', '--dbsnp', help='known variants .vcf', env_var='DBSNP_PATH')  # this option can be set in a config file because it starts with '--'
+   p.add('vcf', nargs='+', help='variant file(s)')
+
+   options = p.parse_args()
+
+   print(options)
+   print("----------")
+   print(p.format_help())
+   print("----------")
+   print(p.format_values())    # useful for logging where different settings came from
+
+
+*config.txt:*
+
+Since the script above set the config file as required=True, lets create a config file to give it:
+
+.. code:: py
+
+    # settings for config_test.py
+    genome = HCMV     # cytomegalovirus genome
+    dbsnp = /data/dbsnp/variants.vcf
+
+
+*command line:*
+
+Now run the script and pass it the config file:
+
+.. code:: bash
+
+    DBSNP_PATH=/data/dbsnp/variants_v2.vcf python config_test.py --my-config config.txt f1.vcf f2.vcf
+
+*output:*
+
+Here is the result:
+
+.. code:: bash
+
+    Namespace(dbsnp='/data/dbsnp/variants_v2.vcf', genome='HCMV', my_config='config.txt', v=False, vcf=['f1.vcf', 'f2.vcf'])
+    ----------
+    usage: config_test.py [-h] -c MY_CONFIG --genome GENOME [-v] [-d DBSNP]
+                          vcf [vcf ...]
+    
+    Args that start with '--' (eg. --genome) can also be set in a config file
+    (/etc/app/conf.d/*.conf or ~/.my_settings or specified via -c). Config file
+    syntax allows: key=value, flag=true, stuff=[a,b,c] (for details, see syntax at
+    https://goo.gl/R74nmi). If an arg is specified in more than one place, then
+    commandline values override environment variables which override config file
+    values which override defaults.
+    
+    positional arguments:
+      vcf                   variant file(s)
+    
+    optional arguments:
+      -h, --help            show this help message and exit
+      -c MY_CONFIG, --my-config MY_CONFIG
+                            config file path
+      --genome GENOME       path to genome file
+      -v                    verbose
+      -d DBSNP, --dbsnp DBSNP
+                            known variants .vcf [env var: DBSNP_PATH]
+    
+    ----------
+    Command Line Args:   --my-config config.txt f1.vcf f2.vcf
+    Environment Variables:
+      DBSNP_PATH:        /data/dbsnp/variants_v2.vcf
+    Config File (config.txt):
+      genome:            HCMV
+
+Special Values
+~~~~~~~~~~~~~~
+
+Under the hood, configargparse handles environment variables and config file
+values by converting them to their corresponding command line arg. For
+example, "key = value" will be processed as if "--key value" was specified
+on the command line.
+
+Also, the following special values (whether in a config file or an environment
+variable) are handled in a special way to support booleans and lists:
+
+-  :code:`key = true` is handled as if "--key" was specified on the command line.
+   In your python code this key must be defined as a boolean flag
+   (eg. action="store_true" or similar).
+
+-  :code:`key = [value1, value2, ...]` is handled as if "--key value1 --key value2"
+   etc. was specified on the command line. In your python code this key must
+   be defined as a list (eg. action="append").
+
+Config File Syntax
+~~~~~~~~~~~~~~~~~~
+
+Only command line args that have a long version (eg. one that starts with '--')
+can be set in a config file. For example, "--color" can be set by putting
+"color=green" in a config file. The config file syntax depends on the constructor
+arg: :code:`config_file_parser_class` which can be set to one of the provided
+classes: :code:`DefaultConfigFileParser`, :code:`YAMLConfigFileParser`,
+:code:`ConfigparserConfigFileParser` or to your own subclass of the
+:code:`ConfigFileParser` abstract class.
+
+*DefaultConfigFileParser*  - the full range of valid syntax is:
+
+.. code:: yaml
+
+        # this is a comment
+        ; this is also a comment (.ini style)
+        ---            # lines that start with --- are ignored (yaml style)
+        -------------------
+        [section]      # .ini-style section names are treated as comments
+
+        # how to specify a key-value pair (all of these are equivalent):
+        name value     # key is case sensitive: "Name" isn't "name"
+        name = value   # (.ini style)  (white space is ignored, so name = value same as name=value)
+        name: value    # (yaml style)
+        --name value   # (argparse style)
+
+        # how to set a flag arg (eg. arg which has action="store_true")
+        --name
+        name
+        name = True    # "True" and "true" are the same
+
+        # how to specify a list arg (eg. arg which has action="append")
+        fruit = [apple, orange, lemon]
+        indexes = [1, 12, 35 , 40]
+
+
+*YAMLConfigFileParser*  - allows a subset of YAML syntax (http://goo.gl/VgT2DU)
+
+.. code:: yaml
+
+        # a comment
+        name1: value
+        name2: true    # "True" and "true" are the same
+
+        fruit: [apple, orange, lemon]
+        indexes: [1, 12, 35, 40]
+        colors:
+          - green
+          - red
+          - blue
+
+*ConfigparserConfigFileParser*  - allows a subset of python's configparser
+module syntax (https://docs.python.org/3.7/library/configparser.html). In
+particular the following configparser options are set:
+
+.. code:: py
+
+        config = configparser.ArgParser(
+            delimiters=("=",":"),
+            allow_no_value=False,
+            comment_prefixes=("#",";"),
+            inline_comment_prefixes=("#",";"),
+            strict=True,
+            empty_lines_in_values=False,
+        )
+
+Once configparser parses the config file all section names are removed, thus all
+keys must have unique names regardless of which INI section they are defined
+under. Also, any keys which have python list syntax are converted to lists by
+evaluating them as python code using ast.literal_eval
+(https://docs.python.org/3/library/ast.html#ast.literal_eval). To facilitate
+this all multi-line values are converted to single-line values. Thus multi-line
+string values will have all new-lines converted to spaces. Note, since key-value
+pairs that have python dictionary syntax are saved as single-line strings, even
+if formatted across multiple lines in the config file, dictionaries can be read
+in and converted to valid python dictionaries with PyYAML's safe_load. Example
+given below:
+
+.. code:: py
+
+        # inside your config file (e.g. config.ini)
+        [section1]  # INI sections treated as comments
+        system1_settings: { # start of multi-line dictionary
+            'a':True,
+            'b':[2, 4, 8, 16],
+            'c':{'start':0, 'stop':1000},
+            'd':'experiment 32 testing simulation with parameter a on'
+            } # end of multi-line dictionary value
+
+        .......
+
+        # in your configargparse setup
+        import configargparse
+        import yaml
+
+        parser = configargparse.ArgParser(
+            config_file_parser_class=configargparse.ConfigparserConfigFileParser
+        )
+        parser.add_argument('--system1_settings', type=yaml.safe_load)
+        
+        args = parser.parse_args() # now args.system1 is a valid python dict
+
+*IniConfigParser*  - INI parser with support for sections.
+
+This parser somewhat ressembles ``ConfigparserConfigFileParser``. It uses configparser and apply the same kind of processing to 
+values written with python list syntax. 
+
+With the following additions: 
+   - Must be created with argument to bind the parser to a list of sections.
+   - Does not convert multiline strings to single line.
+   - Optional support for converting multiline strings to list (if ``split_ml_text_to_list=True``). 
+   - Optional support for quoting strings in config file 
+      (useful when text must not be converted to list or when text 
+      should contain trailing whitespaces).
+
+This config parser can be used to integrate with ``setup.cfg`` files.
+
+Example::
+
+      # this is a comment
+      ; also a comment
+      [my_super_tool]
+      # how to specify a key-value pair
+      format-string: restructuredtext 
+      # white space are ignored, so name = value same as name=value
+      # this is why you can quote strings 
+      quoted-string = '\thello\tmom...  '
+      # how to set an arg which has action="store_true"
+      warnings-as-errors = true
+      # how to set an arg which has action="count" or type=int
+      verbosity = 1
+      # how to specify a list arg (eg. arg which has action="append")
+      repeatable-option = ["https://docs.python.org/3/objects.inv",
+                     "https://twistedmatrix.com/documents/current/api/objects.inv"]
+      # how to specify a multiline text:
+      multi-line-text = 
+         Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+         Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+         Maecenas quis dapibus leo, a pellentesque leo. 
+
+If you use ``IniConfigParser(sections, split_ml_text_to_list=True)``::
+
+      # the same rules are applicable with the following changes:
+      [my-software]
+      # how to specify a list arg (eg. arg which has action="append")
+      repeatable-option = # Just enter one value per line (the list literal format can also be used)
+         https://docs.python.org/3/objects.inv
+         https://twistedmatrix.com/documents/current/api/objects.inv
+      # how to specify a multiline text (you have to quote it):
+      multi-line-text = '''
+         Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+         Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+         Maecenas quis dapibus leo, a pellentesque leo. 
+         '''
+
+Usage:
+
+.. code:: py
+
+   import configargparse
+   parser = configargparse.ArgParser(
+            default_config_files=['setup.cfg', 'my_super_tool.ini'],
+            config_file_parser_class=configargparse.IniConfigParser(['tool:my_super_tool', 'my_super_tool']),
+        )
+   ...
+
+*TomlConfigParser*  - TOML parser with support for sections.
+
+`TOML <https://github.com/toml-lang/toml/blob/main/toml.md>`_ parser. This config parser can be used to integrate with ``pyproject.toml`` files.
+
+Example::
+
+   # this is a comment
+   [tool.my-software] # TOML section table.
+   # how to specify a key-value pair
+   format-string = "restructuredtext" # strings must be quoted
+   # how to set an arg which has action="store_true"
+   warnings-as-errors = true
+   # how to set an arg which has action="count" or type=int
+   verbosity = 1
+   # how to specify a list arg (eg. arg which has action="append")
+   repeatable-option = ["https://docs.python.org/3/objects.inv",
+                  "https://twistedmatrix.com/documents/current/api/objects.inv"]
+   # how to specify a multiline text:
+   multi-line-text = '''
+      Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+      Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+      Maecenas quis dapibus leo, a pellentesque leo. 
+      '''
+
+Usage:
+
+.. code:: py
+
+   import configargparse
+   parser = configargparse.ArgParser(
+            default_config_files=['pyproject.toml', 'my_super_tool.toml'],
+            config_file_parser_class=configargparse.TomlConfigParser(['tool.my_super_tool']),
+        )
+   ...
+
+*CompositeConfigParser*  - Create a config parser to understand multiple formats.
+
+This parser will successively try to parse the file with each parser, until it succeeds, 
+else fail showing all encountered error messages.
+
+The following code will make configargparse understand both TOML and INI formats. 
+Making it easy to integrate in both ``pyproject.toml`` and ``setup.cfg``.
+
+.. code:: py
+
+   import configargparse
+   my_tool_sections = ['tool.my_super_tool', 'tool:my_super_tool', 'my_super_tool']
+                    # pyproject.toml like section, setup.cfg like section, custom section
+   parser = configargparse.ArgParser(
+            default_config_files=['setup.cfg', 'my_super_tool.ini'],
+            config_file_parser_class=configargparse.CompositeConfigParser(
+               [configargparse.TomlConfigParser(my_tool_sections), 
+                configargparse.IniConfigParser(my_tool_sections, split_ml_text_to_list=True)]
+               ),
+        )
+   ...
+
+Note that it's required to put the TOML parser first because the INI syntax basically would accept anything whereas TOML. 
+
+ArgParser Singletons
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To make it easier to configure different modules in an application,
+configargparse provides globally-available ArgumentParser instances
+via configargparse.get_argument_parser('name') (similar to
+logging.getLogger('name')).
+
+Here is an example of an application with a utils module that also
+defines and retrieves its own command-line args.
+
+*main.py*
+
+.. code:: py
+
+    import configargparse
+    import utils
+
+    p = configargparse.get_argument_parser()
+    p.add_argument("-x", help="Main module setting")
+    p.add_argument("--m-setting", help="Main module setting")
+    options = p.parse_known_args()   # using p.parse_args() here may raise errors.
+
+*utils.py*
+
+.. code:: py
+
+    import configargparse
+    p = configargparse.get_argument_parser()
+    p.add_argument("--utils-setting", help="Config-file-settable option for utils")
+
+    if __name__ == "__main__":
+       options = p.parse_known_args()
+
+Help Formatters
+~~~~~~~~~~~~~~~
+
+:code:`ArgumentDefaultsRawHelpFormatter` is a new HelpFormatter that both adds
+default values AND disables line-wrapping. It can be passed to the constructor:
+:code:`ArgParser(.., formatter_class=ArgumentDefaultsRawHelpFormatter)`
+
+
+Aliases
+~~~~~~~
+
+The configargparse.ArgumentParser API inherits its class and method
+names from argparse and also provides the following shorter names for
+convenience:
+
+-  p = configargparse.get_arg_parser()  # get global singleton instance
+-  p = configargparse.get_parser()
+-  p = configargparse.ArgParser()  # create a new instance
+-  p = configargparse.Parser()
+-  p.add_arg(..)
+-  p.add(..)
+-  options = p.parse(..)
+
+HelpFormatters:
+
+- RawFormatter = RawDescriptionHelpFormatter
+- DefaultsFormatter = ArgumentDefaultsHelpFormatter
+- DefaultsRawFormatter = ArgumentDefaultsRawHelpFormatter
+
+API Documentation
+~~~~~~~~~~~~~~~~~
+
+You can review the generated API Documentation for the ``configargparse`` module: `HERE <https://bw2.github.io/ConfigArgParse/>`_
+
+Design Notes
+~~~~~~~~~~~~
+
+Unit tests:
+
+tests/test_configargparse.py contains custom unittests for features
+specific to this module (such as config file and env-var support), as
+well as a hook to load and run argparse unittests (see the built-in
+test.test_argparse module) but on configargparse in place of argparse.
+This ensures that configargparse will work as a drop in replacement for
+argparse in all usecases.
+
+Previously existing modules (PyPI search keywords: config argparse):
+
+-  argparse (built-in module Python v2.7+)
+
+   -  Good:
+
+      -  fully featured command line parsing
+      -  can read args from files using an easy to understand mechanism
+
+   -  Bad:
+
+      -  syntax for specifying config file path is unusual (eg.
+         @file.txt)and not described in the user help message.
+      -  default config file syntax doesn't support comments and is
+         unintuitive (eg. --namevalue)
+      -  no support for environment variables
+
+-  ConfArgParse v1.0.15
+   (https://pypi.python.org/pypi/ConfArgParse)
+
+   -  Good:
+
+      -  extends argparse with support for config files parsed by
+         ConfigParser
+      -  clear documentation in README
+
+   -  Bad:
+
+      -  config file values are processed using
+         ArgumentParser.set_defaults(..) which means "required" and
+         "choices" are not handled as expected. For example, if you
+         specify a required value in a config file, you still have to
+         specify it again on the command line.
+      -  doesn't work with Python 3 yet
+      -  no unit tests, code not well documented
+
+-  appsettings v0.5 (https://pypi.python.org/pypi/appsettings)
+
+   -  Good:
+
+      -  supports config file (yaml format) and env_var parsing
+      -  supports config-file-only setting for specifying lists and
+         dicts
+
+   -  Bad:
+
+      -  passes in config file and env settings via parse_args
+         namespace param
+      -  tests not finished and don't work with Python 3 (import
+         StringIO)
+
+-  argparse_config v0.5.1
+   (https://pypi.python.org/pypi/argparse_config)
+
+   -  Good:
+
+      -  similar features to ConfArgParse v1.0.15
+
+   -  Bad:
+
+      -  doesn't work with Python 3 (error during pip install)
+
+-  yconf v0.3.2 - (https://pypi.python.org/pypi/yconf) - features
+   and interface not that great
+-  hieropt v0.3 - (https://pypi.python.org/pypi/hieropt) - doesn't
+   appear to be maintained, couldn't find documentation
+
+-  configurati v0.2.3 - (https://pypi.python.org/pypi/configurati)
+
+   -  Good:
+
+      -  JSON, YAML, or Python configuration files
+      -  handles rich data structures such as dictionaries
+      -  can group configuration names into sections (like .ini files)
+
+   -  Bad:
+
+      -  doesn't work with Python 3
+      -  2+ years since last release to PyPI
+      -  apparently unmaintained
+
+
+Design choices:
+
+1. all options must be settable via command line. Having options that
+   can only be set using config files or env. vars adds complexity to
+   the API, and is not a useful enough feature since the developer can
+   split up options into sections and call a section "config file keys",
+   with command line args that are just "--" plus the config key.
+2. config file and env. var settings should be processed by appending
+   them to the command line (another benefit of #1). This is an
+   easy-to-implement solution and implicitly takes care of checking that
+   all "required" args are provided, etc., plus the behavior should be
+   easy for users to understand.
+3. configargparse shouldn't override argparse's
+   convert_arg_line_to_args method so that all argparse unit tests
+   can be run on configargparse.
+4. in terms of what to allow for config file keys, the "dest" value of
+   an option can't serve as a valid config key because many options can
+   have the same dest. Instead, since multiple options can't use the
+   same long arg (eg. "--long-arg-x"), let the config key be either
+   "--long-arg-x" or "long-arg-x". This means the developer can allow
+   only a subset of the command-line args to be specified via config
+   file (eg. short args like -x would be excluded). Also, that way
+   config keys are automatically documented whenever the command line
+   args are documented in the help message.
+5. > don't force users to put config file settings in the right .ini [sections].
+   This doesn't have a clear benefit since all options are command-line settable,
+   and so have a globally unique key anyway.
+   Enforcing sections just makes things harder for the user and adds complexity to the implementation.
+   NOTE: This design choice was preventing configargparse from integrating with common Python project
+   config files like setup.cfg or pyproject.toml,
+   so additional parser classes were added that parse only a subset of the values defined in INI or
+   TOML config files.
+6. if necessary, config-file-only args can be added later by
+   implementing a separate add method and using the namespace arg as in
+   appsettings_v0.5
+
+Relevant sites:
+
+-  http://stackoverflow.com/questions/6133517/parse-config-file-environment-and-command-line-arguments-to-get-a-single-coll
+-  http://tricksntweaks.blogspot.com/2013_05_01_archive.html
+-  http://www.youtube.com/watch?v=vvCwqHgZJc8#t=35
+
+
+
+Versioning
+~~~~~~~~~~
+
+This software follows `Semantic Versioning`_
+
+.. _Semantic Versioning: http://semver.org/
```

### Comparing `ConfigArgParse-1.5.3/README.rst` & `ConfigArgParse-1.5.5/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -5,18 +5,14 @@
     :alt: PyPI version
     :target: https://pypi.python.org/pypi/ConfigArgParse
 
 .. image:: https://img.shields.io/pypi/pyversions/ConfigArgParse.svg
     :alt: Supported Python versions
     :target: https://pypi.python.org/pypi/ConfigArgParse
 
-.. image:: https://travis-ci.org/bw2/ConfigArgParse.svg?branch=master
-    :alt: Travis CI build
-    :target: https://travis-ci.org/bw2/ConfigArgParse
-
 .. image:: https://img.shields.io/badge/-API_Documentation-blue
     :alt: API Documentation
     :target: https://bw2.github.io/ConfigArgParse/
 
 Overview
 ~~~~~~~~
 
@@ -26,16 +22,14 @@
 
 Python's command line parsing modules such as argparse have very limited
 support for config files and environment variables, so this module
 extends argparse to add these features.
 
 Available on PyPI: http://pypi.python.org/pypi/ConfigArgParse
 
-.. image:: https://travis-ci.org/bw2/ConfigArgParse.svg?branch=master
-    :target: https://travis-ci.org/bw2/ConfigArgParse
 
 Features
 ~~~~~~~~
 
 -  command-line, config file, env var, and default settings can now be
    defined, documented, and parsed in one go using a single API (if a
    value is specified in more than one way then: command line >
@@ -163,15 +157,15 @@
    be defined as a list (eg. action="append").
 
 Config File Syntax
 ~~~~~~~~~~~~~~~~~~
 
 Only command line args that have a long version (eg. one that starts with '--')
 can be set in a config file. For example, "--color" can be set by putting
-"color=green" in a config file. The config file syntax depends on the constuctor
+"color=green" in a config file. The config file syntax depends on the constructor
 arg: :code:`config_file_parser_class` which can be set to one of the provided
 classes: :code:`DefaultConfigFileParser`, :code:`YAMLConfigFileParser`,
 :code:`ConfigparserConfigFileParser` or to your own subclass of the
 :code:`ConfigFileParser` abstract class.
 
 *DefaultConfigFileParser*  - the full range of valid syntax is:
 
@@ -205,14 +199,18 @@
 
         # a comment
         name1: value
         name2: true    # "True" and "true" are the same
 
         fruit: [apple, orange, lemon]
         indexes: [1, 12, 35, 40]
+        colors:
+          - green
+          - red
+          - blue
 
 *ConfigparserConfigFileParser*  - allows a subset of python's configparser
 module syntax (https://docs.python.org/3.7/library/configparser.html). In
 particular the following configparser options are set:
 
 .. code:: py
 
@@ -257,14 +255,136 @@
         parser = configargparse.ArgParser(
             config_file_parser_class=configargparse.ConfigparserConfigFileParser
         )
         parser.add_argument('--system1_settings', type=yaml.safe_load)
         
         args = parser.parse_args() # now args.system1 is a valid python dict
 
+*IniConfigParser*  - INI parser with support for sections.
+
+This parser somewhat ressembles ``ConfigparserConfigFileParser``. It uses configparser and apply the same kind of processing to 
+values written with python list syntax. 
+
+With the following additions: 
+   - Must be created with argument to bind the parser to a list of sections.
+   - Does not convert multiline strings to single line.
+   - Optional support for converting multiline strings to list (if ``split_ml_text_to_list=True``). 
+   - Optional support for quoting strings in config file 
+      (useful when text must not be converted to list or when text 
+      should contain trailing whitespaces).
+
+This config parser can be used to integrate with ``setup.cfg`` files.
+
+Example::
+
+      # this is a comment
+      ; also a comment
+      [my_super_tool]
+      # how to specify a key-value pair
+      format-string: restructuredtext 
+      # white space are ignored, so name = value same as name=value
+      # this is why you can quote strings 
+      quoted-string = '\thello\tmom...  '
+      # how to set an arg which has action="store_true"
+      warnings-as-errors = true
+      # how to set an arg which has action="count" or type=int
+      verbosity = 1
+      # how to specify a list arg (eg. arg which has action="append")
+      repeatable-option = ["https://docs.python.org/3/objects.inv",
+                     "https://twistedmatrix.com/documents/current/api/objects.inv"]
+      # how to specify a multiline text:
+      multi-line-text = 
+         Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+         Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+         Maecenas quis dapibus leo, a pellentesque leo. 
+
+If you use ``IniConfigParser(sections, split_ml_text_to_list=True)``::
+
+      # the same rules are applicable with the following changes:
+      [my-software]
+      # how to specify a list arg (eg. arg which has action="append")
+      repeatable-option = # Just enter one value per line (the list literal format can also be used)
+         https://docs.python.org/3/objects.inv
+         https://twistedmatrix.com/documents/current/api/objects.inv
+      # how to specify a multiline text (you have to quote it):
+      multi-line-text = '''
+         Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+         Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+         Maecenas quis dapibus leo, a pellentesque leo. 
+         '''
+
+Usage:
+
+.. code:: py
+
+   import configargparse
+   parser = configargparse.ArgParser(
+            default_config_files=['setup.cfg', 'my_super_tool.ini'],
+            config_file_parser_class=configargparse.IniConfigParser(['tool:my_super_tool', 'my_super_tool']),
+        )
+   ...
+
+*TomlConfigParser*  - TOML parser with support for sections.
+
+`TOML <https://github.com/toml-lang/toml/blob/main/toml.md>`_ parser. This config parser can be used to integrate with ``pyproject.toml`` files.
+
+Example::
+
+   # this is a comment
+   [tool.my-software] # TOML section table.
+   # how to specify a key-value pair
+   format-string = "restructuredtext" # strings must be quoted
+   # how to set an arg which has action="store_true"
+   warnings-as-errors = true
+   # how to set an arg which has action="count" or type=int
+   verbosity = 1
+   # how to specify a list arg (eg. arg which has action="append")
+   repeatable-option = ["https://docs.python.org/3/objects.inv",
+                  "https://twistedmatrix.com/documents/current/api/objects.inv"]
+   # how to specify a multiline text:
+   multi-line-text = '''
+      Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
+      Vivamus tortor odio, dignissim non ornare non, laoreet quis nunc. 
+      Maecenas quis dapibus leo, a pellentesque leo. 
+      '''
+
+Usage:
+
+.. code:: py
+
+   import configargparse
+   parser = configargparse.ArgParser(
+            default_config_files=['pyproject.toml', 'my_super_tool.toml'],
+            config_file_parser_class=configargparse.TomlConfigParser(['tool.my_super_tool']),
+        )
+   ...
+
+*CompositeConfigParser*  - Create a config parser to understand multiple formats.
+
+This parser will successively try to parse the file with each parser, until it succeeds, 
+else fail showing all encountered error messages.
+
+The following code will make configargparse understand both TOML and INI formats. 
+Making it easy to integrate in both ``pyproject.toml`` and ``setup.cfg``.
+
+.. code:: py
+
+   import configargparse
+   my_tool_sections = ['tool.my_super_tool', 'tool:my_super_tool', 'my_super_tool']
+                    # pyproject.toml like section, setup.cfg like section, custom section
+   parser = configargparse.ArgParser(
+            default_config_files=['setup.cfg', 'my_super_tool.ini'],
+            config_file_parser_class=configargparse.CompositeConfigParser(
+               [configargparse.TomlConfigParser(my_tool_sections), 
+                configargparse.IniConfigParser(my_tool_sections, split_ml_text_to_list=True)]
+               ),
+        )
+   ...
+
+Note that it's required to put the TOML parser first because the INI syntax basically would accept anything whereas TOML. 
 
 ArgParser Singletons
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To make it easier to configure different modules in an application,
 configargparse provides globally-available ArgumentParser instances
 via configargparse.get_argument_parser('name') (similar to
@@ -430,46 +550,47 @@
    can only be set using config files or env. vars adds complexity to
    the API, and is not a useful enough feature since the developer can
    split up options into sections and call a section "config file keys",
    with command line args that are just "--" plus the config key.
 2. config file and env. var settings should be processed by appending
    them to the command line (another benefit of #1). This is an
    easy-to-implement solution and implicitly takes care of checking that
-   all "required" args are provied, etc., plus the behavior should be
+   all "required" args are provided, etc., plus the behavior should be
    easy for users to understand.
 3. configargparse shouldn't override argparse's
    convert_arg_line_to_args method so that all argparse unit tests
    can be run on configargparse.
 4. in terms of what to allow for config file keys, the "dest" value of
    an option can't serve as a valid config key because many options can
    have the same dest. Instead, since multiple options can't use the
    same long arg (eg. "--long-arg-x"), let the config key be either
    "--long-arg-x" or "long-arg-x". This means the developer can allow
    only a subset of the command-line args to be specified via config
    file (eg. short args like -x would be excluded). Also, that way
    config keys are automatically documented whenever the command line
    args are documented in the help message.
-5. don't force users to put config file settings in the right .ini
-   [sections]. This doesn't have a clear benefit since all options are
-   command-line settable, and so have a globally unique key anyway.
-   Enforcing sections just makes things harder for the user and adds
-   complexity to the implementation.
+5. > don't force users to put config file settings in the right .ini [sections].
+   This doesn't have a clear benefit since all options are command-line settable,
+   and so have a globally unique key anyway.
+   Enforcing sections just makes things harder for the user and adds complexity to the implementation.
+   NOTE: This design choice was preventing configargparse from integrating with common Python project
+   config files like setup.cfg or pyproject.toml,
+   so additional parser classes were added that parse only a subset of the values defined in INI or
+   TOML config files.
 6. if necessary, config-file-only args can be added later by
    implementing a separate add method and using the namespace arg as in
    appsettings_v0.5
 
 Relevant sites:
 
 -  http://stackoverflow.com/questions/6133517/parse-config-file-environment-and-command-line-arguments-to-get-a-single-coll
 -  http://tricksntweaks.blogspot.com/2013_05_01_archive.html
 -  http://www.youtube.com/watch?v=vvCwqHgZJc8#t=35
 
 
-.. |Travis CI Status for bw2/ConfigArgParse| image:: https://travis-ci.org/bw2/ConfigArgParse.svg?branch=master
-
 
 Versioning
 ~~~~~~~~~~
 
 This software follows `Semantic Versioning`_
 
 .. _Semantic Versioning: http://semver.org/
```

