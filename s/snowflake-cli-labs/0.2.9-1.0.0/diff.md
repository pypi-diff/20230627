# Comparing `tmp/snowflake_cli_labs-0.2.9.tar.gz` & `tmp/snowflake_cli_labs-1.0.0.tar.gz`

## Comparing `snowflake_cli_labs-0.2.9.tar` & `snowflake_cli_labs-1.0.0.tar`

### file list

```diff
@@ -1,80 +1,151 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/LEGAL.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/requirements-dev.txt
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/requirements.txt
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/snowcli.spec
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tox.ini
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/docs/images/coverage_5.png
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/__init__.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/config.py
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/snow_connector.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/snowsql_config.py
--rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/utils.py
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/__init__.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/connection.py
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/function.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/package.py
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/render.py
--rw-r--r--   0        0        0    20029 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/snowpark_shared.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/sql.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/stage.py
--rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/streamlit.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/warehouse.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure_coverage/__init__.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure_coverage/clear.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure_coverage/report.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/python_templates/environment.yml.jinja
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/python_templates/snowpark_coverage.py.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/call_procedure.sql
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/create_function.sql
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/create_procedure.sql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/create_stage.sql
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/create_streamlit.sql
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/describe_function.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/describe_procedure.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/describe_streamlit.sql
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/drop_function.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/drop_procedure.sql
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/drop_stage.sql
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/drop_streamlit.sql
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/execute_function.sql
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/get_stage.sql
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/get_streamlit_url.sql
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/list_functions.sql
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/list_procedures.sql
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/list_stage.sql
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/list_stages.sql
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/list_streamlits.sql
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/put_stage.sql
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/remove_from_stage.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/set_procedure_comment.sql
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/share_streamlit.sql
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/show_warehouses.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_function/.gitignore
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_function/app.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_function/app.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_function/requirements.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_procedure/.gitignore
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_procedure/app.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_procedure/app.toml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_procedure/local_connection.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_procedure/requirements.txt
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/conftest.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/test_main.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/test_render.py
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/test_snow_connector.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/test_sql.py
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/__snapshots__/test_snow_connector.ambr
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/LICENSE
--rw-r--r--   0        0        0    11607 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/README.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/pyproject.toml
--rw-r--r--   0        0        0    12603 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/LEGAL.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/snowcli.spec
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tox.ini
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/docs/images/coverage_5.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/__init__.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/config.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/connection_params.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/exception.py
+-rw-r--r--   0        0        0    25360 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/snow_connector.py
+-rw-r--r--   0        0        0    22751 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/utils.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/__init__.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/connection.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/loggers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/registry.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/render.py
+-rw-r--r--   0        0        0    19073 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark_shared.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/sql.py
+-rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/stage.py
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/streamlit.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/warehouse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/common/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/common/alias.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/common/flags.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/common/snow_cli_global_context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/main/__init__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/main/snow_cli_main_typer.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/__init__.py
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/cp.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/function.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/jobs.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/package.py
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/registry.py
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/services.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure_coverage/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure_coverage/clear.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure_coverage/report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/output/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/output/formats.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/output/printing.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/python_templates/environment.yml.jinja
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/python_templates/snowpark_coverage.py.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/call_procedure.sql
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/create_function.sql
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/create_procedure.sql
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/create_stage.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/create_streamlit.sql
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/describe_function.sql
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/describe_procedure.sql
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/describe_streamlit.sql
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/drop_function.sql
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/drop_procedure.sql
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/drop_stage.sql
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/drop_streamlit.sql
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/execute_function.sql
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/get_stage.sql
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/get_streamlit_url.sql
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/list_functions.sql
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/list_procedures.sql
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/list_stage.sql
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/list_stages.sql
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/list_streamlits.sql
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/put_stage.sql
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/remove_from_stage.sql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/set_env.sql
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/set_procedure_comment.sql
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/share_streamlit.sql
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/show_warehouses.sql
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/compute_pool/create_compute_pool.sql
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/compute_pool/drop_compute_pool.sql
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/compute_pool/list_compute_pools.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/compute_pool/stop_compute_pools.sql
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/jobs/create_job.sql
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/jobs/desc_job.sql
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/jobs/drop_job.sql
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/jobs/logs_job.sql
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/jobs/status_job.sql
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/create_service.sql
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/desc_service.sql
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/drop_service.sql
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/list_service.sql
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/logs_service.sql
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/snowcli/sql/snowservices/services/status_service.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_function/.gitignore
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_function/app.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_function/config.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_function/requirements.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_procedure/.gitignore
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_procedure/app.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_procedure/config.toml
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_procedure/local_connection.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/src/templates/default_procedure/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test.toml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_config.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_connection.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_main.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_render.py
+-rw-r--r--   0        0        0    25290 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_snow_connector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_spec.yaml
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_sql.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_stage.py
+-rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/__snapshots__/test_connection.ambr
+-rw-r--r--   0        0        0    12070 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/__snapshots__/test_snow_connector.ambr
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/config/env_variables_config
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/output/test_printing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/anaconda_channel_data.json
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/test_data.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/test_streamlit_requirements.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/test_data/local_packages/.packages/zendesk/file.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/testing_utils/__init__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests/testing_utils/result_assertions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/conftest.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/snowflake_connector.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/test_warehouse.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/config/connection_configs.toml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/tests_integration/config/test.toml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/README.md
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 snowflake_cli_labs-1.0.0/PKG-INFO
```

### Comparing `snowflake_cli_labs-0.2.9/.pre-commit-config.yaml` & `snowflake_cli_labs-1.0.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         exclude: .github/repo_meta.yaml
       - id: debug-statements
       - id: check-ast
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.217"
     hooks:
       - id: ruff
-        args: [--fix, --exclude, "**/tests/"]
+        args: [--fix, --exclude, "**/tests/", --line-length, "88", --select, "N"]
   - repo: https://github.com/psf/black
     rev: 22.12.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.990
     hooks:
```

### Comparing `snowflake_cli_labs-0.2.9/snowcli.spec` & `snowflake_cli_labs-1.0.0/snowcli.spec`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.9/docs/images/coverage_1.png` & `snowflake_cli_labs-1.0.0/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.9/docs/images/coverage_2.png` & `snowflake_cli_labs-1.0.0/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.9/docs/images/coverage_3.png` & `snowflake_cli_labs-1.0.0/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.9/docs/images/coverage_4.png` & `snowflake_cli_labs-1.0.0/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.9/docs/images/coverage_5.png` & `snowflake_cli_labs-1.0.0/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/utils.py` & `snowflake_cli_labs-1.0.0/src/snowcli/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,165 +1,204 @@
 from __future__ import annotations
+from dataclasses import dataclass
 
 import glob
 import json
+import logging
 import os
 import pathlib
 import re
 import shutil
 import subprocess
 import warnings
 import zipfile
 from pathlib import Path
-from typing import List, Literal, Optional
+from typing import Dict, List, Literal, Optional
 
 import click
 import requests
 import requirements
+from requirements.requirement import Requirement
 import typer
 from jinja2 import Environment, FileSystemLoader
-from rich import box, print
-from rich.table import Table
-from snowflake.connector.cursor import SnowflakeCursor
 
-from snowcli.config import AppConfig
+from snowcli.config import cli_config
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 YesNoAskOptions = ["yes", "no", "ask"]
 YesNoAskOptionsType = Literal["yes", "no", "ask"]
 
 PIP_PATH = os.environ.get("SNOWCLI_PIP_PATH", "pip")
 
 templates_path = os.path.join(Path(__file__).parent, "python_templates")
 
+log = logging.getLogger(__name__)
 
+
+# TODO: add typing to all functions
 def yes_no_ask_callback(value: str):
     """
     A typer callback to handle yes/no/ask parameters
     """
     if value not in YesNoAskOptions:
         raise typer.BadParameter(
             f"Valid values: {YesNoAskOptions}. You provided: {value}",
         )
     return value
 
 
-def getDeployNames(database, schema, name) -> dict:
+def get_deploy_names(database, schema, name) -> dict:
     stage = f"{database}.{schema}.deployments"
     path = f"/{name.lower()}/app.zip"
     directory = f"/{name.lower()}"
     return {
         "stage": stage,
         "path": path,
         "full_path": f"@{stage}{path}",
         "directory": directory,
     }
 
 
 # create a temporary directory, copy the file_path to it and rename to app.zip
 
 
-def prepareAppZip(file_path, temp_dir) -> str:
+def prepare_app_zip(file_path, temp_dir) -> str:
     # get filename from file path (e.g. app.zip from /path/to/app.zip)
+    # TODO: think if no file exceptions are handled correctly
     file_name = os.path.basename(file_path)
     temp_path = temp_dir + "/" + file_name
     shutil.copy(file_path, temp_path)
     return temp_path
 
 
-def parseRequirements(requirements_file: str = "requirements.txt") -> list[str]:
+@dataclass
+class SplitRequirements:
+    """A dataclass to hold the results of parsing requirements files and dividing them into
+    snowflake-supported vs other packages.
+    """
+
+    snowflake: List[Requirement]
+    other: List[Requirement]
+
+
+def parse_requirements(
+    requirements_file: str = "requirements.txt",
+) -> List[Requirement]:
     """Reads and parses a python requirements.txt file.
 
     Args:
         requirements_file (str, optional): The name of the file.
         Defaults to 'requirements.txt'.
 
     Returns:
         list[str]: A flat list of package names, without versions
     """
-    reqs = []
+    reqs: List[Requirement] = []
     if os.path.exists(requirements_file):
         with open(requirements_file, encoding="utf-8") as f:
             for req in requirements.parse(f):
-                reqs.append(req.name)
+                reqs.append(req)
     else:
-        click.echo(f"No {requirements_file} found")
+        log.info(f"No {requirements_file} found")
 
-    return reqs
+    return deduplicate_and_sort_reqs(reqs)
+
+
+def deduplicate_and_sort_reqs(packages: List[Requirement]) -> List[Requirement]:
+    """
+    Deduplicates a list of requirements, keeping the first occurrence of each package.
+    """
+    seen = set()
+    deduped: List[Requirement] = []
+    for package in packages:
+        if package.name not in seen:
+            deduped.append(package)
+            seen.add(package.name)
+    # sort by package name
+    deduped.sort(key=lambda x: x.name)
+    return deduped
 
 
 # parse JSON from https://repo.anaconda.com/pkgs/snowflake/channeldata.json and
 # return a list of packages that exist in packages with the .packages json
 # response from https://repo.anaconda.com/pkgs/snowflake/channeldata.json
-# CURRENTLY DOES NOT SUPPORT PINNING TO VERSIONS
-
-
-def parseAnacondaPackages(packages: list[str]) -> dict:
+def parse_anaconda_packages(packages: List[Requirement]) -> SplitRequirements:
+    """
+    Checks if a list of packages are available in the Snowflake Anaconda channel.
+    Returns a dict with two keys: 'snowflake' and 'other'.
+    Each key contains a list of Requirement objects.
+    """
     url = "https://repo.anaconda.com/pkgs/snowflake/channeldata.json"
     response = requests.get(url)
-    snowflakePackages = []
-    otherPackages = []
+    snowflake_packages: List[Requirement] = []
+    other_packages: List[Requirement] = []
     if response.status_code == 200:
         channel_data = response.json()
         for package in packages:
             # pip package names are case insensitive,
             # Anaconda package names are lowercased
-            if package.lower() in channel_data["packages"]:
-                snowflakePackages.append(
-                    f"{package}",
-                )
+            if package.name.lower() in channel_data["packages"]:
+                snowflake_packages.append(package)
             else:
-                click.echo(
-                    f'"{package}" not found in Snowflake anaconda channel...',
+                log.info(
+                    f"'{package.name}' not found in Snowflake anaconda channel...",
                 )
-                otherPackages.append(package)
-        # As at April 2023, streamlit appears unavailable in the Snowflake Anaconda channel
-        # but actually works if specified in the environment
-        if "streamlit" in otherPackages:
-            otherPackages.remove("streamlit")
-        return {"snowflake": snowflakePackages, "other": otherPackages}
+                if package.name.lower() == "streamlit":
+                    # As at April 2023, streamlit appears unavailable in the Snowflake Anaconda channel
+                    # but actually works if specified in the environment
+                    log.info(
+                        f"'{package.name}' is not available in the Snowflake anaconda channel "
+                        "but is supported in the environment.yml file",
+                    )
+                else:
+                    other_packages.append(package)
+        return SplitRequirements(snowflake=snowflake_packages, other=other_packages)
     else:
-        click.echo(f"Error: {response.status_code}")
-        return {}
+        log.error(f"Error reading Anaconda channel data: {response.status_code}")
+        raise typer.Abort()
 
 
-def generateStreamlitEnvironmentFile(
+def generate_streamlit_environment_file(
     excluded_anaconda_deps: Optional[List[str]],
+    requirements_file: str = "requirements.snowflake.txt",
 ) -> Optional[Path]:
     """Creates an environment.yml file for streamlit deployment, if a Snowflake
     requirements file exists.
     The file path is returned if it was generated, otherwise None is returned.
     """
-    if os.path.exists("requirements.snowflake.txt"):
-        # for each line in requirements.snowflake.txt, prepend '- ' to the line and prepare it for interpolation into the template
-        with open("requirements.snowflake.txt", "r", encoding="utf-8") as f:
-            requirements = f.read().split("\n")
+    if os.path.exists(requirements_file):
+        snowflake_requirements = parse_requirements(requirements_file)
+
         # remove explicitly excluded anaconda dependencies
         if excluded_anaconda_deps is not None:
-            print(f"""Excluded dependencies: {','.join(excluded_anaconda_deps)}""")
-            requirements = [
-                line for line in requirements if line not in excluded_anaconda_deps
+            log.info(f"Excluded dependencies: {','.join(excluded_anaconda_deps)}")
+            snowflake_requirements = [
+                r
+                for r in snowflake_requirements
+                if r.name not in excluded_anaconda_deps
             ]
-        # remove duplicates, remove comments, remove snowflake-connector-python
-        requirements = [
-            f"- {line}"
-            for line in sorted(list(set(requirements)))
-            if len(line) > 0 and line[0] != "#" and line != "snowflake-connector-python"
+        # remove snowflake-connector-python
+        requirement_yaml_lines = [
+            # unsure if streamlit supports versioned requirements,
+            # following PrPr docs convention for now
+            f"- {req.name}"
+            for req in snowflake_requirements
+            if req.name != "snowflake-connector-python"
         ]
-        dependencies_list = "\n".join(requirements)
+        dependencies_list = "\n".join(requirement_yaml_lines)
         environment = Environment(loader=FileSystemLoader(templates_path))
         template = environment.get_template("environment.yml.jinja")
         with open("environment.yml", "w", encoding="utf-8") as f:
             f.write(template.render(dependencies=dependencies_list))
         return Path("environment.yml")
     return None
 
 
-def generateStreamlitPackageWrapper(
+def generate_streamlit_package_wrapper(
     stage_name: str, main_module: str, extract_zip: bool
 ) -> Path:
     """Uses a jinja template to generate a streamlit wrapper.
     The wrapper will add app.zip to the path and import the app module.
     """
     environment = Environment(loader=FileSystemLoader(templates_path))
     template = environment.get_template("streamlit_app_launcher.py.jinja")
@@ -172,28 +211,37 @@
         }
     )
     with open(target_file, "w", encoding="utf-8") as output_file:
         output_file.write(content)
     return target_file
 
 
-def getDownloadedPackageNames() -> dict[str, list[str]]:
+@dataclass
+class RequirementWithFiles:
+    """A dataclass to hold a requirement and the path to the
+    downloaded files/folders that belong to it"""
+
+    requirement: Requirement
+    files: List[str]
+
+
+def get_downloaded_packages() -> Dict[str, RequirementWithFiles]:
     """Returns a dict of official package names mapped to the files/folders
     that belong to it under the .packages directory.
 
     Returns:
         dict[str:List[str]]: a dict of package folder names to package name
     """
     metadata_files = glob.glob(".packages/*dist-info/METADATA")
     packages_full_path = os.path.abspath(".packages")
-    return_dict = {}
+    return_dict: Dict[str, RequirementWithFiles] = {}
     for metadata_file in metadata_files:
         parent_folder = os.path.dirname(metadata_file)
-        package_name = getPackageNameFromMetadata(metadata_file)
-        if package_name is not None:
+        package = get_package_name_from_metadata(metadata_file)
+        if package is not None:
             # since we found a package name, we can now look at the RECORD
             # file (a sibling of METADATA) to determine which files and
             # folders that belong to it
             record_file_path = os.path.join(parent_folder, "RECORD")
             if os.path.exists(record_file_path):
                 # the RECORD file contains a list of files included in the
                 # package, get the unique root folder names and delete them
@@ -218,19 +266,21 @@
                         # We'll ignore those by asserting that the full
                         # packages path exists in the full path of each item.
                         if (
                             os.path.exists(record_entry_full_path)
                             and packages_full_path in record_entry_full_path
                         ):
                             included_record_entries.append(record_entry)
-                    return_dict[package_name] = included_record_entries
+                    return_dict[package.name] = RequirementWithFiles(
+                        requirement=package, files=included_record_entries
+                    )
     return return_dict
 
 
-def getPackageNameFromMetadata(metadata_file_path: str) -> str | None:
+def get_package_name_from_metadata(metadata_file_path: str) -> Requirement | None:
     """Loads a METADATA file from the dist-info directory of an installed
     Python package, finds the name of the package.
     This is found on a line containing "Name: my_package".
 
     Args:
         metadata_file_path (str): The path to the METADATA file
 
@@ -238,18 +288,23 @@
         str: the name of the package.
     """
     with open(metadata_file_path, encoding="utf-8") as metadata_file:
         contents = metadata_file.read()
         results = re.search("^Name: (.*)$", contents, flags=re.MULTILINE)
         if results is None:
             return None
-        return results.group(1)
+        requirement_line = results.group(1)
+        results = re.search("^Version: (.*)$", contents, flags=re.MULTILINE)
+        if results is not None:
+            version = results.group(1)
+            requirement_line += f"=={version}"
+        return Requirement.parse(requirement_line)
 
 
-def generateSnowparkCoverageWrapper(
+def generate_snowpark_coverage_wrapper(
     target_file: str,
     proc_name: str,
     proc_signature: str,
     handler_module: str,
     handler_function: str,
     coverage_reports_stage: str,
     coverage_reports_stage_path: str,
@@ -280,115 +335,133 @@
             "coverage_reports_stage_path": coverage_reports_stage_path,
         }
     )
     with open(target_file, "w", encoding="utf-8") as output_file:
         output_file.write(content)
 
 
-def addFileToExistingZip(zip_file: str, other_file: str):
+def add_file_to_existing_zip(zip_file: str, other_file: str):
     """Adds another file to an existing zip file
 
     Args:
         zip_file (str): The existing zip file
         other_file (str): The new file to add
     """
     with zipfile.ZipFile(zip_file, mode="a") as myzip:
         myzip.write(other_file, os.path.basename(other_file))
 
 
-def installPackages(
+def install_packages(
     file_name: str | None,
     perform_anaconda_check: bool = True,
     package_native_libraries: YesNoAskOptionsType = "ask",
     package_name: str | None = None,
-) -> tuple[bool, dict[str, list[str]] | None]:
+) -> tuple[bool, SplitRequirements | None]:
+    """
+    Install packages from a requirements.txt file or a single package name,
+    into a local folder named '.packages'.
+    If a requirements.txt file is provided, they will be installed using pip.
+    If a package name is provided, it will be installed using pip.
+    Returns a tuple of:
+    1) a boolean indicating whether the installation was successful
+    2) a SplitRequirements object containing any installed dependencies
+    which are available on the Snowflake anaconda channel. These will have
+    been deleted from the local packages folder.
+    """
     pip_install_result = None
     second_chance_results = None
     if file_name is not None:
         try:
             process = subprocess.Popen(
                 [PIP_PATH, "install", "-t", ".packages/", "-r", file_name],
                 stdout=subprocess.PIPE,
                 universal_newlines=True,
             )
             for line in process.stdout:  # type: ignore
-                click.echo(line.strip())
+                log.info(line.strip())
             process.wait()
             pip_install_result = process.returncode
         except FileNotFoundError:
-            click.echo(
-                "\n\npip not found. Please install pip and try again.\nHINT: you can also set the environment variable 'SNOWCLI_PIP_PATH' to the path of pip.",
-                err=True,
+            log.error(
+                "pip not found. Please install pip and try again. "
+                "HINT: you can also set the environment variable 'SNOWCLI_PIP_PATH' to the path of pip.",
             )
             return False, None
     if package_name is not None:
         try:
             process = subprocess.Popen(
                 [PIP_PATH, "install", "-t", ".packages/", package_name],
                 stdout=subprocess.PIPE,
                 universal_newlines=True,
             )
             for line in process.stdout:  # type: ignore
-                click.echo(line.strip())
+                log.info(line.strip())
             process.wait()
             pip_install_result = process.returncode
         except FileNotFoundError:
-            click.echo(
-                "\n\npip not found. Please install pip and try again.\nHINT: you can also set the environment variable 'SNOWCLI_PIP_PATH' to the path of pip.",
-                err=True,
+            log.error(
+                "pip not found. Please install pip and try again. "
+                "HINT: you can also set the environment variable 'SNOWCLI_PIP_PATH' to the path of pip.",
             )
             return False, None
 
     if pip_install_result is not None and pip_install_result != 0:
-        print(
-            f"pip failed with return code {pip_install_result}. \n\nThis may happen when attempting to install a package that isn't compatible with the host architecture - and generally means it has native libraries."
+        log.info(
+            f"pip failed with return code {pip_install_result}. "
+            "This may happen when attempting to install a package "
+            "that isn't compatible with the host architecture - "
+            "and generally means it has native libraries."
         )
         return False, None
     if perform_anaconda_check:
-        click.echo("Checking for dependencies available in Anaconda...")
+        log.info("Checking for dependencies available in Anaconda...")
         # it's not over just yet. a non-Anaconda package may have brought in
         # a package available on Anaconda.
         # use each folder's METADATA file to determine its real name
-        downloaded_packages = getDownloadedPackageNames()
-        click.echo(f"Downloaded packages: {downloaded_packages.values()}")
+        downloaded_packages_dict = get_downloaded_packages()
+        log.info(f"Downloaded packages: {downloaded_packages_dict.keys()}")
         # look for all the downloaded packages on the Anaconda channel
-        second_chance_results = parseAnacondaPackages(
-            list(downloaded_packages.keys()),
+        downloaded_package_requirements = [
+            r.requirement for r in downloaded_packages_dict.values()
+        ]
+        second_chance_results = parse_anaconda_packages(
+            downloaded_package_requirements,
         )
-        second_chance_snowflake_packages = second_chance_results["snowflake"]
+        second_chance_snowflake_packages = second_chance_results.snowflake
         if len(second_chance_snowflake_packages) > 0:
-            click.echo(
-                f"""Good news! The following package dependencies can be
-                imported directly from Anaconda, and will be excluded from
-                the zip: {second_chance_snowflake_packages}""",
+            log.info(
+                "Good news! The following package dependencies can be "
+                "imported directly from Anaconda, and will be excluded from "
+                f"the zip: {second_chance_snowflake_packages}"
             )
         else:
-            click.echo(
-                "None of the package dependencies were found on Anaconda",
-            )
+            log.info("None of the package dependencies were found on Anaconda")
+        second_chance_snowflake_package_names = [
+            p.name for p in second_chance_snowflake_packages
+        ]
         downloaded_packages_not_needed = {
             k: v
-            for k, v in downloaded_packages.items()
-            if k in second_chance_snowflake_packages
+            for k, v in downloaded_packages_dict.items()
+            if k in second_chance_snowflake_package_names
         }
         for package, items in downloaded_packages_not_needed.items():
-            click.echo(f"Package {package}: deleting {items}")
-            for item in items:
+            log.info(f"Package {package}: deleting {len(items.files)} files")
+            for item in items.files:
                 item_path = os.path.join(".packages", item)
                 if os.path.exists(item_path):
                     if os.path.isdir(item_path):
                         shutil.rmtree(item_path)
                     else:
                         os.remove(item_path)
 
-    click.echo("Checking to see if packages have native libaries...\n")
+    log.info("Checking to see if packages have native libraries...")
     # use glob to see if any files in packages have a .so extension
     if glob.glob(".packages/**/*.so"):
         for path in glob.glob(".packages/**/*.so"):
-            click.echo(f"Potential native library: {path}")
+            log.info(f"Potential native library: {path}")
         continue_installation = (
             click.confirm(
                 "\n\nWARNING! Some packages appear to have native libraries!\n"
                 "Continue with package installation?",
                 default=False,
             )
             if package_native_libraries == "ask"
@@ -396,21 +469,23 @@
         )
         if continue_installation:
             return True, second_chance_results
         else:
             shutil.rmtree(".packages")
             return False, second_chance_results
     else:
-        click.echo(
-            "No non-supported native libraries found in packages (Good news!)..."
-        )
+        log.info("No non-supported native libraries found in packages (Good news!)...")
         return True, second_chance_results
 
 
-def recursiveZipPackagesDir(pack_dir: str, dest_zip: str) -> bool:
+def recursive_zip_packages_dir(pack_dir: str, dest_zip: str) -> bool:
+    # TODO:
+    # 1. why this is -> bool
+    # 2. Reformat it to with open...
+    # 3. Reformat it to get list od dirs and then iterate through it, adding files to zip
     # create a zip file object
     zipf = zipfile.ZipFile(dest_zip, "w", zipfile.ZIP_DEFLATED, allowZip64=True)
 
     # for every file in the relative path pack_dir, add it to the zip file
     for file in pathlib.Path(pack_dir).glob("**/*"):
         zipf.write(file, arcname=os.path.relpath(file, pack_dir))
 
@@ -436,15 +511,15 @@
                         zipf.write(file, arcname=os.path.relpath(file, directory))
 
     # close the zip file object
     zipf.close()
     return True
 
 
-def standardZipDir(dest_zip: str) -> bool:
+def standard_zip_dir(dest_zip: str) -> bool:
     zipf = zipfile.ZipFile(dest_zip, "w", zipfile.ZIP_DEFLATED, allowZip64=True)
     for file in pathlib.Path(".").glob("*"):
         if not file.match(".*"):
             zipf.write(os.path.relpath(file))
 
     if os.getenv("SNOWCLI_INCLUDE_PATHS") is not None:
         for dir_path in os.getenv("SNOWCLI_INCLUDE_PATHS", "").split(":"):
@@ -459,113 +534,52 @@
                         zipf.write(file, arcname=os.path.relpath(file, directory))
 
     # close the zip file object
     zipf.close()
     return True
 
 
-def getSnowflakePackages() -> list[str]:
+def get_snowflake_packages() -> list[str]:
     if os.path.exists("requirements.snowflake.txt"):
         with open("requirements.snowflake.txt", encoding="utf-8") as f:
             return [line.strip() for line in f]
     else:
         return []
 
 
-def getSnowflakePackagesDelta(anaconda_packages) -> list[str]:
-    updatedPackageList = []
+def get_snowflake_packages_delta(anaconda_packages) -> list[str]:
+    updated_package_list = []
     if os.path.exists("requirements.snowflake.txt"):
         with open("requirements.snowflake.txt", encoding="utf-8") as f:
             # for each line, check if it exists in anaconda_packages. If it
             # doesn't, add it to the return string
             for line in f:
                 if line.strip() not in anaconda_packages:
-                    updatedPackageList.append(line.strip())
-        return updatedPackageList
+                    updated_package_list.append(line.strip())
+        return updated_package_list
     else:
-        return updatedPackageList
+        return updated_package_list
 
 
-def convertResourceDetailsToDict(function_details: list[tuple]) -> dict:
+def convert_resource_details_to_dict(function_details: list[tuple]) -> dict:
     function_dict = {}
     json_properties = ["packages", "installed_packages"]
     for function in function_details:
         if function[0] in json_properties:
             function_dict[function[0]] = json.loads(
                 function[1].replace("'", '"'),
             )
         else:
             function_dict[function[0]] = function[1]
     return function_dict
 
 
-def print_db_cursor(
-    cursor, only_cols=[], show_header: bool = True, show_border: bool = True
-):
-    if cursor.description:
-        if any(only_cols):
-            cols = [
-                (index, col[0])
-                for (index, col) in enumerate(
-                    cursor.description,
-                )
-                if col[0] in only_cols
-            ]
-        else:
-            cols = [(index, col[0]) for (index, col) in enumerate(cursor.description)]
-
-        box_val = box.HEAVY_HEAD if show_border else None
-
-        table = Table(
-            *[col[1] for col in cols],
-            show_header=show_header,
-            box=box_val,
-            border_style=None,
-        )
-        for row in cursor.fetchall():
-            filtered_row = [str(row[col_index]) for (col_index, _) in cols]
-            try:
-                table.add_row(*filtered_row)
-            except Exception as e:
-                print(type(e))
-                print(e.args)
-                print(e)
-        print(table)
-
-
-def print_list_tuples(lt: SnowflakeCursor):
-    table = Table("Key", "Value")
-    for item in lt:
-        if item[0] == "imports":
-            table.add_row(item[0], item[1].strip("[]"))
-        else:
-            table.add_row(item[0], item[1])
-    print(table)
-
-
-def conf_callback(ctx: typer.Context, param: typer.CallbackParam, value: str):
-    if value:
-        try:
-            app_config = AppConfig().config
-
-            # Initialize the default map
-            ctx.default_map = ctx.default_map or {}
-            # if app_config has key 'default'
-            config_section = os.getenv("SNOWCLI_CONFIG_SECTION", "default")
-            if config_section in app_config:
-                ctx.default_map.update(
-                    app_config.get(config_section),
-                )  # type: ignore
-            if value in app_config:
-                # TODO: Merge the config dict into default_map
-                # type: ignore
-                ctx.default_map.update(app_config.get(value))
-        except Exception as ex:
-            raise typer.BadParameter(str(ex))
-    return value
+def check_for_connection(connection_name: str):
+    cli_config.get_connection(connection_name=connection_name)
+    return connection_name
 
 
 def generate_deploy_stage_name(name: str, input_parameters: str) -> str:
     return name + input_parameters.replace("(", "",).replace(")", "",).replace(
         " ",
         "_",
     ).replace(
```

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/cli/__init__.py` & `snowflake_cli_labs-1.0.0/src/snowcli/cli/stage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,168 +1,189 @@
 from __future__ import annotations
 
-import pkgutil
-import sys
-from collections.abc import Container
 from pathlib import Path
 
 import typer
-from rich import print
 
-from .. import __about__
-from ..config import AppConfig
-from ..snowsql_config import SnowsqlConfig
-from . import (
-    connection,
-    function,
-    package,
-    procedure,
-    render,
-    sql,
-    stage,
-    streamlit,
-    warehouse,
+from snowcli import config
+from snowcli.cli.common.flags import DEFAULT_CONTEXT_SETTINGS, ConnectionOption
+from snowcli.config import connect_to_snowflake
+from snowcli.output.printing import print_db_cursor
+
+app = typer.Typer(
+    name="stage",
+    context_settings=DEFAULT_CONTEXT_SETTINGS,
+    help="Manage stages",
 )
 
-app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
 
+@app.command("list")
+def stage_list(
+    environment: str = ConnectionOption,
+    name=typer.Argument(None, help="Name of stage"),
+):
+    """
+    List stage contents
+    """
+    conn = connect_to_snowflake(connection_name=environment)
 
-def version_callback(value: bool):
-    if value:
-        typer.echo(f"SnowCLI Version: {__about__.VERSION}")
-        raise typer.Exit()
-
-
-@app.command()
-def login(
-    snowsql_config_path: Path = typer.Option(
-        "~/.snowsql/config",
-        "--config",
-        "-c",
-        prompt="Path to Snowsql config",
-        help="snowsql config file",
-    ),
-    snowsql_connection_name: str = typer.Option(
-        ...,
-        "--connection",
-        "-C",
-        prompt="Connection name (for entry in snowsql config)",
-        help="connection name from snowsql config file",
+    if config.is_auth():
+        if name:
+            results = conn.list_stage(
+                database=conn.ctx.database,
+                schema=conn.ctx.schema,
+                role=conn.ctx.role,
+                warehouse=conn.ctx.warehouse,
+                name=name,
+            )
+            print_db_cursor(results)
+        else:
+            results = conn.list_stages(
+                database=conn.ctx.database,
+                schema=conn.ctx.schema,
+                role=conn.ctx.role,
+                warehouse=conn.ctx.warehouse,
+            )
+            print_db_cursor(results)
+
+
+@app.command("get")
+def stage_get(
+    environment: str = ConnectionOption,
+    name: str = typer.Argument(..., help="Stage name"),
+    path: Path = typer.Argument(
+        Path.cwd(),
+        exists=False,
+        file_okay=True,
+        dir_okay=True,
+        writable=True,
+        resolve_path=True,
+        help="Directory location to store downloaded files",
     ),
 ):
     """
-    Select a Snowflake connection to use with SnowCLI.
+    Download files from a stage to a local client
     """
-    if not snowsql_config_path.expanduser().exists():
-        print(f"Path to snowsql config does not exist: {snowsql_config_path}")
-        raise typer.Abort()
-
-    cfg_snowsql = SnowsqlConfig(snowsql_config_path)
-    if f"connections.{snowsql_connection_name}" not in cfg_snowsql.config:
-        print(
-            "Connection not found in "
-            f"{snowsql_config_path}: {snowsql_connection_name}. ",
-            "You can add with `snow connection add`.",
+    conn = connect_to_snowflake(connection_name=environment)
+
+    if config.is_auth():
+        results = conn.get_stage(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            name=name,
+            path=str(path),
         )
-        raise typer.Abort()
+        print_db_cursor(results)
 
-    cfg = AppConfig()
-    cfg.config["snowsql_config_path"] = str(snowsql_config_path.expanduser())
-    cfg.config["snowsql_connection_name"] = snowsql_connection_name
-    cfg.save()
-    print(
-        "Using connection name " f"{snowsql_connection_name} in {snowsql_config_path}",
-    )
-    print(f"Wrote {cfg.path}")
-
-
-@app.command()
-def configure(
-    environment: str = typer.Option(
-        "dev",
-        "-e",
-        "--environment",
-        help="Name of environment (e.g. dev, prod, staging)",
-    ),
-    database: str = typer.Option(
-        ...,
-        "--database",
-        prompt="Snowflake database",
-        help="Snowflake database",
-    ),
-    schema: str = typer.Option(
-        ...,
-        "--schema",
-        prompt="Snowflake schema",
-        help="Snowflake schema",
-    ),
-    role: str = typer.Option(
-        ...,
-        "--role",
-        prompt="Snowflake role",
-        help="Snowflake role",
-    ),
-    warehouse: str = typer.Option(
+
+@app.command("put")
+def stage_put(
+    environment: str = ConnectionOption,
+    path: Path = typer.Argument(
         ...,
-        "--warehouse",
-        prompt="Snowflake warehouse",
-        help="Snowflake warehouse",
+        exists=True,
+        file_okay=True,
+        dir_okay=True,
+        writable=True,
+        resolve_path=True,
+        help="File or directory to upload to stage",
+    ),
+    name: str = typer.Argument(..., help="Stage name"),
+    overwrite: bool = typer.Option(
+        False,
+        help="Overwrite existing files in stage",
+    ),
+    parallel: int = typer.Option(
+        4,
+        help="Number of parallel threads to use for upload",
     ),
 ):
     """
-    Configure an environment to use with your Snowflake connection.
-    """
-    print(f"Configuring environment #{environment}...")
-    cfg = AppConfig()
-    if environment in cfg.config and not typer.confirm(
-        "Environment {environment} already exists. Overwrite?",
-    ):
-        print("Cancelling...")
-        raise typer.Abort()
-
-    cfg.config[environment] = {}
-    cfg.config[environment]["database"] = database
-    cfg.config[environment]["schema"] = schema
-    cfg.config[environment]["role"] = role
-    cfg.config[environment]["warehouse"] = warehouse
-    cfg.save()
-    print(f"Wrote environment {environment} to {cfg.path}")
-
-
-@app.callback()
-def default(
-    version: bool = typer.Option(
-        None,
-        "--version",
-        callback=version_callback,
-        is_eager=True,
-    ),
-) -> None:
-    """
-    SnowCLI - A CLI for Snowflake
+    Upload files to a stage from a local client
     """
+    conn = connect_to_snowflake(connection_name=environment)
 
+    if config.is_auth():
+        filepath = str(path)
+        if path.is_dir():
+            filepath = str(path) + "/*"
+
+        results = conn.put_stage(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            name=name,
+            path=str(filepath),
+            overwrite=overwrite,
+            parallel=parallel,
+        )
+        print_db_cursor(results)
 
-MODULE_IGNORE_SET = frozenset(("procedure_coverage",))
 
+@app.command("create")
+def stage_create(
+    environment: str = ConnectionOption,
+    name: str = typer.Argument(..., help="Stage name"),
+):
+    """
+    Create stage if not exists
+    """
+    conn = connect_to_snowflake(connection_name=environment)
 
-def register_cli_typers(ignore_container: Container[str] = MODULE_IGNORE_SET) -> None:
-    for _, name, _ in pkgutil.walk_packages(__path__):
-        if name not in ignore_container:
-            cli_app = __import__(f"{__name__}.{name}", fromlist=["_trash"])
-            try:
-                app.add_typer(cli_app.app, name=name)
-            except AttributeError:
-                # Ignore modules that don't define app global
-                pass
+    if config.is_auth():
+        results = conn.create_stage(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            name=name,
+        )
+        print_db_cursor(results)
 
 
-register_cli_typers()
+@app.command("drop")
+def stage_drop(
+    environment: str = ConnectionOption,
+    name: str = typer.Argument(..., help="Stage name"),
+):
+    """
+    Drop stage
+    """
+    conn = connect_to_snowflake(connection_name=environment)
 
-app.command("sql")(sql.execute_sql)
+    if config.is_auth():
+        results = conn.drop_stage(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            name=name,
+        )
+        print_db_cursor(results)
 
 
-if __name__ == "__main__":
-    app()
+@app.command("remove")
+def stage_remove(
+    environment: str = ConnectionOption,
+    stage_name: str = typer.Argument(..., help="Stage name"),
+    file_name: str = typer.Argument(..., help="File name"),
+):
+    """
+    Remove file from stage
+    """
+
+    conn = connect_to_snowflake(connection_name=environment)
 
-if getattr(sys, "frozen", False):
-    app(sys.argv[1:])
+    if config.is_auth():
+        config.connect_to_snowflake()
+        results = conn.remove_from_stage(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            name=stage_name,
+            path=file_name,
+        )
+        print_db_cursor(results)
```

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/cli/function.py` & `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/function.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,55 @@
-#!/usr/bin/env python
 from __future__ import annotations
 
 import os
 from pathlib import Path
 from shutil import copytree
 
 import pkg_resources
 import typer
 
+from snowcli.cli.common.flags import DEFAULT_CONTEXT_SETTINGS, ConnectionOption
 from snowcli.cli.snowpark_shared import (
     CheckAnacondaForPyPiDependancies,
     PackageNativeLibrariesOption,
     PyPiDownloadOption,
     snowpark_create,
     snowpark_describe,
     snowpark_drop,
     snowpark_execute,
     snowpark_list,
     snowpark_package,
     snowpark_update,
 )
-from snowcli.utils import conf_callback
 
-app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
-EnvironmentOption = typer.Option(
-    "dev",
-    help="Environment name",
-    callback=conf_callback,
-    is_eager=True,
+app = typer.Typer(
+    name="function",
+    context_settings=DEFAULT_CONTEXT_SETTINGS,
+    help="Manage user defined functions",
+)
+
+HandlerOption = typer.Option(
+    ...,
+    "--handler",
+    "-h",
+    help="Handler",
+)
+
+InputParametersOption = typer.Option(
+    ...,
+    "--input-parameters",
+    "-i",
+    help="Input parameters - such as (message string, count int)",
+)
+
+ReturnTypeOption = typer.Option(
+    ...,
+    "--return-type",
+    "-r",
+    help="Return type",
 )
 
 
 @app.command("init")
 def function_init():
     """
     Initialize this directory with a sample set of files to create a function.
@@ -44,15 +62,15 @@
         f"{os.getcwd()}",
         dirs_exist_ok=True,
     )
 
 
 @app.command("create")
 def function_create(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     pypi_download: str = PyPiDownloadOption,
     package_native_libraries: str = PackageNativeLibrariesOption,
     check_anaconda_for_pypi_deps: bool = CheckAnacondaForPyPiDependancies,
     name: str = typer.Option(
         ...,
         "--name",
         "-n",
@@ -61,32 +79,17 @@
     file: Path = typer.Option(
         "app.zip",
         "--file",
         "-f",
         help="Path to the file or folder to deploy",
         exists=False,
     ),
-    handler: str = typer.Option(
-        ...,
-        "--handler",
-        "-h",
-        help="Handler",
-    ),
-    input_parameters: str = typer.Option(
-        ...,
-        "--input-parameters",
-        "-i",
-        help="Input parameters - such as (message string, count int)",
-    ),
-    return_type: str = typer.Option(
-        ...,
-        "--return-type",
-        "-r",
-        help="Return type",
-    ),
+    handler: str = HandlerOption,
+    input_parameters: str = InputParametersOption,
+    return_type: str = ReturnTypeOption,
     overwrite: bool = typer.Option(
         False,
         "--overwrite",
         "-o",
         help="Replace if existing function",
     ),
 ):
@@ -105,44 +108,29 @@
         return_type=return_type,
         overwrite=overwrite,
     )
 
 
 @app.command("update")
 def function_update(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     pypi_download: str = PyPiDownloadOption,
     check_anaconda_for_pypi_deps: bool = CheckAnacondaForPyPiDependancies,
     package_native_libraries: str = PackageNativeLibrariesOption,
     name: str = typer.Option(..., "--name", "-n", help="Name of the function"),
     file: Path = typer.Option(
         "app.zip",
         "--file",
         "-f",
         help="Path to the file to update",
         exists=False,
     ),
-    handler: str = typer.Option(
-        ...,
-        "--handler",
-        "-h",
-        help="Handler",
-    ),
-    input_parameters: str = typer.Option(
-        ...,
-        "--input-parameters",
-        "-i",
-        help="Input parameters - such as (message string, count int)",
-    ),
-    return_type: str = typer.Option(
-        ...,
-        "--return-type",
-        "-r",
-        help="Return type",
-    ),
+    handler: str = HandlerOption,
+    input_parameters: str = InputParametersOption,
+    return_type: str = ReturnTypeOption,
     replace: bool = typer.Option(
         False,
         "--replace-always",
         "-a",
         help="Replace function, even if no detected changes to metadata",
     ),
 ):
@@ -174,35 +162,30 @@
         check_anaconda_for_pypi_deps,
         package_native_libraries,  # type: ignore[arg-type]
     )
 
 
 @app.command("execute")
 def function_execute(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     function: str = typer.Option(
         ...,
         "--function",
         "-f",
         help="Function with inputs. E.g. 'hello(int, string)'",
     ),
 ):
     snowpark_execute(type="function", environment=environment, select=function)
 
 
 @app.command("describe")
 def function_describe(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     name: str = typer.Option("", "--name", "-n", help="Name of the function"),
-    input_parameters: str = typer.Option(
-        "",
-        "--input-parameters",
-        "-i",
-        help="Input parameters - such as (message string, count int)",
-    ),
+    input_parameters: str = InputParametersOption,
     function: str = typer.Option(
         "",
         "--function",
         "-f",
         help="Function signature with inputs. E.g. 'hello(int, string)'",
     ),
 ):
@@ -213,35 +196,30 @@
         input_parameters=input_parameters,
         signature=function,
     )
 
 
 @app.command("list")
 def function_list(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     like: str = typer.Option(
         "%%",
         "--like",
         "-l",
         help='Filter functions by name - e.g. "hello%"',
     ),
 ):
     snowpark_list("function", environment, like=like)
 
 
 @app.command("drop")
 def function_drop(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     name: str = typer.Option("", "--name", "-n", help="Name of the function"),
-    input_parameters: str = typer.Option(
-        "",
-        "--input-parameters",
-        "-i",
-        help="Input parameters - such as (message string, count int)",
-    ),
+    input_parameters: str = InputParametersOption,
     signature: str = typer.Option(
         "",
         "--procedure",
         "-p",
         help="Function signature with inputs. E.g. 'hello(int, string)'",
     ),
 ):
```

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/cli/package.py` & `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/package.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-#!/usr/bin/env python
 from __future__ import annotations
 
 import os
 import tempfile
 from pathlib import Path
 from shutil import rmtree
 
 import click
+import logging
 import typer
+from requirements.requirement import Requirement
 
 from snowcli import config, utils
-from snowcli.config import AppConfig
+from snowcli.cli.common.flags import DEFAULT_CONTEXT_SETTINGS, ConnectionOption
+from snowcli.config import connect_to_snowflake
 
 app = typer.Typer(
-    context_settings={"help_option_names": ["-h", "--help"]},
+    name="package",
+    context_settings=DEFAULT_CONTEXT_SETTINGS,
     help="Manage custom Python packages for Snowpark",
 )
-EnvironmentOption = typer.Option("dev", help="Environment name")
+log = logging.getLogger(__name__)
 
 
 @app.command("lookup")
 def package_lookup(
     name: str = typer.Argument(
         ...,
         help="Name of the package",
@@ -32,41 +35,41 @@
         help="Install packages that are not available on the Snowflake anaconda channel",
     ),
     _run_nested: bool = False,
 ):
     """
     Check to see if a package is available on the Snowflake anaconda channel.
     """
-    packageResponse = utils.parseAnacondaPackages([name])
+    package_response = utils.parse_anaconda_packages([Requirement.parse(name)])
     ## if list has any items
 
-    if len(packageResponse["snowflake"]) > 0:
-        click.echo(f"Package {name} is available on the Snowflake anaconda channel.")
+    if len(package_response.snowflake) > 0:
+        log.info(f"Package {name} is available on the Snowflake anaconda channel.")
         if _run_nested:
-            click.echo(
-                f"No need to create a package. Just include in your `packages` declaration."
+            log.info(
+                "No need to create a package. Just include in your `packages` declaration."
             )
     else:
         if not install_packages:
             install_packages = click.confirm(
                 "The package is not in Anaconda. Do you want to try to see if it's supported as a custom package (requires pip)?",
                 default=True,
             )
         if install_packages:
             packages_string = None
-            status, results = utils.installPackages(
+            status, results = utils.install_packages(
                 perform_anaconda_check=True, package_name=name, file_name=None
             )
-            if status and results is not None and len(results["snowflake"]) > 0:
-                packages_string = f"The package {name} is supported, but does depend on the following Snowflake supported native libraries you should include the following in your packages: {results['snowflake']}"
+            if status and results is not None and len(results.snowflake) > 0:
+                packages_string = f"The package {name} is supported, but does depend on the following Snowflake supported native libraries you should include the following in your packages: {results.snowflake}"
             # if .packages subfolder exists, delete it
             if not _run_nested and os.path.exists(".packages"):
                 rmtree(".packages")
             if packages_string is not None:
-                click.echo("\n\n" + packages_string)
+                log.info(packages_string)
             if _run_nested and packages_string is not None:
                 return packages_string
 
 
 @app.command("create")
 def package_create(
     name: str = typer.Argument(
@@ -81,21 +84,21 @@
     ),
 ):
     """
     Create a python package as a zip file that can be uploaded to a stage and imported for a Snowpark python app.
     """
     results_string = package_lookup(name, install_packages, _run_nested=True)
     if os.path.exists(".packages"):
-        utils.recursiveZipPackagesDir(".packages", name + ".zip")
+        utils.recursive_zip_packages_dir(".packages", name + ".zip")
         rmtree(".packages")
-        click.echo(
-            f"\n\nPackage {name}.zip created. You can now upload it to a stage (`snow package upload -f {name}.zip -s packages`) and reference it in your procedure or function."
+        log.info(
+            f"Package {name}.zip created. You can now upload it to a stage (`snow package upload -f {name}.zip -s packages`) and reference it in your procedure or function."
         )
         if results_string is not None:
-            click.echo("\n" + results_string)
+            log.info(results_string)
 
 
 @app.command("upload")
 def package_upload(
     file: Path = typer.Option(
         ...,
         "--file",
@@ -111,38 +114,32 @@
     ),
     overwrite: bool = typer.Option(
         False,
         "--overwrite",
         "-o",
         help="Overwrite the file if it already exists",
     ),
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
 ):
     """
     Upload a python package zip file to a Snowflake stage so it can be referenced in the imports of a procedure or function.
     """
-    env_conf = AppConfig().config.get(environment)
-    if env_conf is None:
-        click.echo(
-            f"The {environment} environment is not configured in app.toml "
-            "yet, please run `snow configure` first before continuing.",
-        )
-        raise typer.Abort()
-    if config.isAuth():
-        config.connectToSnowflake()
+    conn = connect_to_snowflake(connection_name=environment)
+    if config.is_auth():
         click.echo(f"Uploading {file} to Snowflake @{stage}/{file}...")
         with tempfile.TemporaryDirectory() as temp_dir:
-            temp_app_zip_path = utils.prepareAppZip(file, temp_dir)
-            deploy_response = config.snowflake_connection.uploadFileToStage(
+            temp_app_zip_path = utils.prepare_app_zip(file, temp_dir)
+            deploy_response = conn.upload_file_to_stage(
                 file_path=temp_app_zip_path,
                 destination_stage=stage,
                 path="/",
-                database=env_conf["database"],
-                schema=env_conf["schema"],
+                database=conn.ctx.database,
+                schema=conn.ctx.schema,
                 overwrite=overwrite,
-                role=env_conf["role"],
+                role=conn.ctx.role,
+                warehouse=conn.ctx.warehouse,
             )
-        click.echo(f"Package {file} {deploy_response[6]} to Snowflake @{stage}/{file}.")
+        log.info(f"Package {file} {deploy_response[6]} to Snowflake @{stage}/{file}.")
         if deploy_response[6] == "SKIPPED":
-            click.echo(
+            log.info(
                 "Package already exists on stage. Consider using --overwrite to overwrite the file."
             )
```

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure.py` & `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-#!/usr/bin/env python
 from __future__ import annotations
 
 import os
 from pathlib import Path
 from shutil import copytree
 
 import pkg_resources
 import typer
 
+from snowcli.cli.common.flags import DEFAULT_CONTEXT_SETTINGS, ConnectionOption
+from snowcli.cli.snowpark.procedure_coverage import app as procedure_coverage_app
 from snowcli.cli.snowpark_shared import (
     CheckAnacondaForPyPiDependancies,
     PackageNativeLibrariesOption,
     PyPiDownloadOption,
     snowpark_create,
     snowpark_describe,
     snowpark_drop,
     snowpark_execute,
     snowpark_list,
     snowpark_package,
     snowpark_update,
 )
-from snowcli.utils import conf_callback
+from snowcli.utils import check_for_connection
 
-from . import procedure_coverage
-
-app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
-EnvironmentOption = typer.Option(
-    "dev",
-    help="Environment name",
-    callback=conf_callback,
-    is_eager=True,
+app = typer.Typer(
+    name="procedure",
+    context_settings=DEFAULT_CONTEXT_SETTINGS,
+    help="Manage stored procedures",
 )
-app.add_typer(procedure_coverage.app, name="coverage")
+app.add_typer(procedure_coverage_app)
 
 
 @app.command("init")
 def procedure_init():
     """
     Initialize this directory with a sample set of files to create a procedure.
     """
@@ -47,15 +44,15 @@
         f"{os.getcwd()}",
         dirs_exist_ok=True,
     )
 
 
 @app.command("create")
 def procedure_create(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     pypi_download: str = PyPiDownloadOption,
     check_anaconda_for_pypi_deps: bool = CheckAnacondaForPyPiDependancies,
     package_native_libraries: str = PackageNativeLibrariesOption,
     name: str = typer.Option(
         ...,
         "--name",
         "-n",
@@ -120,15 +117,15 @@
         execute_as_caller,
         install_coverage_wrapper,
     )
 
 
 @app.command("update")
 def procedure_update(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     pypi_download: str = PyPiDownloadOption,
     check_anaconda_for_pypi_deps: bool = CheckAnacondaForPyPiDependancies,
     package_native_libraries: str = PackageNativeLibrariesOption,
     name: str = typer.Option(
         ...,
         "--name",
         "-n",
@@ -172,15 +169,19 @@
     ),
     install_coverage_wrapper: bool = typer.Option(
         False,
         "--install-coverage-wrapper",
         help="Wraps the procedure with a code coverage measurement tool, so that a coverage report can be later retrieved.",
     ),
 ):
-    (pypi_download, check_anaconda_for_pypi_deps, package_native_libraries)
+    snowpark_package(
+        pypi_download,  # type: ignore[arg-type]
+        check_anaconda_for_pypi_deps,
+        package_native_libraries,  # type: ignore[arg-type]
+    )
     snowpark_update(
         "procedure",
         environment,
         name,
         file,
         handler,
         input_parameters,
@@ -202,28 +203,28 @@
         check_anaconda_for_pypi_deps,
         package_native_libraries,  # type: ignore[arg-type]
     )
 
 
 @app.command("execute")
 def procedure_execute(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     select: str = typer.Option(
         ...,
         "--procedure",
         "-p",
         help="Procedure with inputs. E.g. 'hello(int, string)'. Must exactly match those provided when creating the procedure.",
     ),
 ):
     snowpark_execute("procedure", environment, select)
 
 
 @app.command("describe")
 def procedure_describe(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     name: str = typer.Option("", "--name", "-n", help="Name of the procedure"),
     input_parameters: str = typer.Option(
         "",
         "--input-parameters",
         "-i",
         help="Input parameters - such as (message string, count int)",
     ),
@@ -241,28 +242,28 @@
         input_parameters,
         signature,
     )
 
 
 @app.command("list")
 def procedure_list(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     like: str = typer.Option(
         "%%",
         "--like",
         "-l",
         help='Filter procedures by name - e.g. "hello%"',
     ),
 ):
     snowpark_list("procedure", environment, like=like)
 
 
 @app.command("drop")
 def procedure_drop(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     name: str = typer.Option("", "--name", "-n", help="Name of the procedure"),
     input_parameters: str = typer.Option(
         "",
         "--input-parameters",
         "-i",
         help="Input parameters - such as (message string, count int)",
     ),
```

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/cli/render.py` & `snowflake_cli_labs-1.0.0/src/snowcli/cli/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-#!/usr/bin/env python
 from __future__ import annotations
 
 import json
 from pathlib import Path
 from textwrap import dedent
 from typing import List, Optional
 
 import jinja2
 import typer
 
-app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
+from snowcli.cli.common.flags import DEFAULT_CONTEXT_SETTINGS
+
+app = typer.Typer(context_settings=DEFAULT_CONTEXT_SETTINGS, hidden=True)
 
 
 def read_file_content(file_name: str):
     return Path(file_name).read_text()
 
 
 @jinja2.pass_environment  # type: ignore
```

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/cli/stage.py` & `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/services.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,166 +1,188 @@
-#!/usr/bin/env python
-from __future__ import annotations
-
-from pathlib import Path
+import sys
 
 import typer
-
 from snowcli import config
-from snowcli.config import AppConfig
-from snowcli.utils import print_db_cursor
+from snowcli.cli import DEFAULT_CONTEXT_SETTINGS
+from typing import TextIO
+from typing_extensions import Annotated
+
+from snowcli.cli.common.flags import ConnectionOption
+from snowcli.config import connect_to_snowflake
+from snowcli.output.printing import print_db_cursor
+
+app = typer.Typer(
+    context_settings=DEFAULT_CONTEXT_SETTINGS, name="services", help="Manage services"
+)
+
+
+if not sys.stdout.closed and sys.stdout.isatty():
+    GREEN = "\033[32m"
+    BLUE = "\033[34m"
+    ORANGE = "\033[38:2:238:76:44m"
+    GRAY = "\033[2m"
+    ENDC = "\033[0m"
+else:
+    GREEN = ""
+    ORANGE = ""
+    BLUE = ""
+    GRAY = ""
+    ENDC = ""
+
+
+@app.command()
+def create(
+    environment: str = ConnectionOption,
+    name: str = typer.Option(..., "--name", "-n", help="Job Name"),
+    compute_pool: str = typer.Option(..., "--compute_pool", "-c", help="Compute Pool"),
+    spec_path: str = typer.Option(..., "--spec_path", "-s", help="Spec Path"),
+    num_instances: Annotated[
+        int, typer.Option("--num_instances", "-num", help="Number of instances")
+    ] = 1,
+    stage: str = typer.Option("SOURCE_STAGE", "--stage", "-l", help="Stage name"),
+):
+    """
+    Create service
+    """
+    conn = connect_to_snowflake(connection_name=environment)
 
-app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
-EnvironmentOption = typer.Option("dev", help="Environment name")
+    if config.is_auth():
+        results = conn.create_service(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            name=name,
+            compute_pool=compute_pool,
+            num_instances=num_instances,
+            spec_path=spec_path,
+            stage=stage,
+        )
+        print_db_cursor(results)
 
 
-@app.command("list")
-def stage_list(
-    environment: str = EnvironmentOption,
-    name=typer.Argument(None, help="Name of stage"),
+@app.command()
+def desc(
+    environment: str = ConnectionOption,
+    name: str = typer.Argument(..., help="Service Name"),
 ):
     """
-    List stage contents
+    Desc Service
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
-        if name:
-            results = config.snowflake_connection.listStage(
-                database=env_conf.get("database"),
-                schema=env_conf.get("schema"),
-                role=env_conf.get("role"),
-                warehouse=env_conf.get("warehouse"),
-                name=name,
-            )
-            print_db_cursor(results)
-        else:
-            results = config.snowflake_connection.listStages(
-                database=env_conf.get("database"),
-                schema=env_conf.get("schema"),
-                role=env_conf.get("role"),
-                warehouse=env_conf.get("warehouse"),
-            )
-            print_db_cursor(results)
-
-
-@app.command("get")
-def stage_get(
-    environment: str = EnvironmentOption,
-    name: str = typer.Argument(..., help="Stage name"),
-    path: Path = typer.Argument(
-        Path("."),
-        exists=False,
-        file_okay=True,
-        dir_okay=True,
-        writable=True,
-        resolve_path=True,
-        help="Directory location to store downloaded files",
+    if config.is_auth():
+        results = conn.desc_service(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
+            name=name,
+        )
+        print_db_cursor(results)
+
+
+def _prefix_line(prefix: str, line: str) -> str:
+    """
+    _prefix_line ensure the prefix is still present even when dealing with return characters
+    """
+    if "\r" in line:
+        line = line.replace("\r", f"\r{prefix}")
+    if "\n" in line[:-1]:
+        line = line[:-1].replace("\n", f"\n{prefix}") + line[-1:]
+    if not line.startswith("\r"):
+        line = f"{prefix}{line}"
+    return line
+
+
+def print_log_lines(file: TextIO, name, id, logs):
+    prefix = f"{GREEN}{name}/{id}{ENDC} "
+    logs = logs[0:-1]
+    for log in logs:
+        print(_prefix_line(prefix, log + "\n"), file=file, end="", flush=True)
+
+
+@app.command()
+def logs(
+    environment: str = ConnectionOption,
+    name: str = typer.Argument(..., help="Service Name"),
+    container_name: str = typer.Option(
+        ..., "--container_name", "-c", help="Container Name"
     ),
 ):
     """
-    Download files from a stage to a local client
+    Logs Service
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
-        results = config.snowflake_connection.getStage(
-            database=env_conf.get("database"),
-            schema=env_conf.get("schema"),
-            role=env_conf.get("role"),
-            warehouse=env_conf.get("warehouse"),
+    if config.is_auth():
+        results = conn.logs_service(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
             name=name,
-            path=str(path),
+            instance_id="0",
+            container_name=container_name,
         )
-        print_db_cursor(results)
+        cursor = results.fetchone()
+        logs = next(iter(cursor)).split("\n")
+        print_log_lines(sys.stdout, name, "0", logs)
 
 
-@app.command("put")
-def stage_put(
-    environment: str = EnvironmentOption,
-    path: Path = typer.Argument(
-        ...,
-        exists=True,
-        file_okay=True,
-        dir_okay=True,
-        writable=True,
-        resolve_path=True,
-        help="File or directory to upload to stage",
-    ),
-    name: str = typer.Argument(..., help="Stage name"),
-    overwrite: bool = typer.Option(
-        False,
-        help="Overwrite existing files in stage",
-    ),
-    parallel: int = typer.Option(
-        4,
-        help="Number of parallel threads to use for upload",
-    ),
+@app.command()
+def status(
+    environment: str = ConnectionOption,
+    name: str = typer.Argument(..., help="Service Name"),
 ):
     """
-    Upload files to a stage from a local client
+    Logs Service
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
-        filepath = str(path)
-        if path.is_dir():
-            filepath = str(path) + "/*"
-
-        results = config.snowflake_connection.putStage(
-            database=env_conf.get("database"),
-            schema=env_conf.get("schema"),
-            role=env_conf.get("role"),
-            warehouse=env_conf.get("warehouse"),
+    if config.is_auth():
+        results = conn.status_service(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
             name=name,
-            path=str(filepath),
-            overwrite=overwrite,
-            parallel=parallel,
         )
         print_db_cursor(results)
 
 
-@app.command("create")
-def stage_create(
-    environment: str = EnvironmentOption,
-    name: str = typer.Argument(..., help="Stage name"),
-):
+@app.command()
+def list(environment: str = ConnectionOption):
     """
-    Create stage if not exists
+    List Service
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
-        results = config.snowflake_connection.createStage(
-            database=env_conf.get("database"),
-            schema=env_conf.get("schema"),
-            role=env_conf.get("role"),
-            warehouse=env_conf.get("warehouse"),
-            name=name,
+    if config.is_auth():
+        results = conn.list_service(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
         )
         print_db_cursor(results)
 
 
-@app.command("drop")
-def stage_drop(
-    environment: str = EnvironmentOption,
-    name: str = typer.Argument(..., help="Stage name"),
+@app.command()
+def drop(
+    environment: str = ConnectionOption,
+    name: str = typer.Argument(..., help="Service Name"),
 ):
     """
-    Drop stage
+    Drop Service
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
-        results = config.snowflake_connection.dropStage(
-            database=env_conf.get("database"),
-            schema=env_conf.get("schema"),
-            role=env_conf.get("role"),
-            warehouse=env_conf.get("warehouse"),
+    if config.is_auth():
+        results = conn.drop_service(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
             name=name,
         )
         print_db_cursor(results)
```

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/cli/streamlit.py` & `snowflake_cli_labs-1.0.0/src/snowcli/cli/streamlit.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,104 +1,93 @@
-#!/usr/bin/env python
 from __future__ import annotations
 
+import logging
+import typer
 from pathlib import Path
 from typing import List, Optional
 
-import typer
-from rich import print
-
 from snowcli import config
-from snowcli.config import AppConfig
+from snowcli.cli.common.flags import DEFAULT_CONTEXT_SETTINGS, ConnectionOption
+from snowcli.config import connect_to_snowflake
+from snowcli.output.printing import print_db_cursor
 from snowcli.utils import (
-    generateStreamlitEnvironmentFile,
-    generateStreamlitPackageWrapper,
-    print_db_cursor,
+    generate_streamlit_environment_file,
+    generate_streamlit_package_wrapper,
 )
-
-app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
-EnvironmentOption = typer.Option("dev", help="Environment name")
-
 from snowcli.cli.snowpark_shared import (
     CheckAnacondaForPyPiDependancies,
     PackageNativeLibrariesOption,
     PyPiDownloadOption,
     snowpark_package,
 )
 
+app = typer.Typer(
+    context_settings=DEFAULT_CONTEXT_SETTINGS,
+    help="Manage Streamlit in Snowflake",
+)
+log = logging.getLogger(__name__)
+
 
 def get_standard_stage_name(name: str) -> str:
     # Handle embedded stages
     if name.startswith("snow://"):
         return name
 
     return f"@{name}"
 
 
 @app.command("list")
 def streamlit_list(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     only_cols: List[str] = typer.Option(list, help="Only show these columns"),
-    show_header: bool = typer.Option(
-        True,
-        help="Show column headers",
-    ),
-    show_border: bool = typer.Option(
-        True,
-        help="Show column borders",
-    ),
 ):
     """
     List streamlit apps.
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
-        results = config.snowflake_connection.listStreamlits(
-            database=env_conf.get("database"),
-            schema=env_conf.get("schema"),
-            role=env_conf.get("role"),
-            warehouse=env_conf.get("warehouse"),
+    if config.is_auth():
+        results = conn.list_streamlits(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
         )
 
         print_db_cursor(
             results,
-            only_cols=only_cols,
-            show_header=show_header,
-            show_border=show_border,
+            columns=only_cols,
         )
 
 
 @app.command("describe")
 def streamlit_describe(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Name of streamlit to be deployed."),
 ):
     """
     Describe a streamlit app.
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
-        description, url = config.snowflake_connection.describeStreamlit(
+    if config.is_auth():
+        description, url = conn.describe_streamlit(
             name,
-            database=env_conf.get("database"),
-            schema=env_conf.get("schema"),
-            role=env_conf.get("role"),
-            warehouse=env_conf.get("warehouse"),
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
         )
         print_db_cursor(description)
         print_db_cursor(url)
 
 
 @app.command("create")
 def streamlit_create(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Name of streamlit to be created."),
     file: Path = typer.Option(
         "streamlit_app.py",
         exists=True,
         readable=True,
         file_okay=True,
         help="Path to streamlit file",
@@ -112,93 +101,88 @@
         help="Set this flag to package all code and dependencies into a zip file. "
         + "This should be considered a temporary workaround until native support is available.",
     ),
 ):
     """
     Create a streamlit app named NAME.
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
+    if config.is_auth():
         if from_stage:
             if "." in from_stage:
                 full_stage_name = from_stage
             else:
-                full_stage_name = (
-                    f"{env_conf.get('database')}.{env_conf.get('schema')}.{from_stage}"
-                )
+                full_stage_name = f"{conn.ctx.database}.{conn.ctx.schema}.{from_stage}"
             standard_page_name = get_standard_stage_name(full_stage_name)
             from_stage_command = f"FROM {standard_page_name}"
         else:
             from_stage_command = ""
 
-        results = config.snowflake_connection.createStreamlit(
-            database=env_conf.get("database"),
-            schema=env_conf.get("schema"),
-            role=env_conf.get("role"),
-            warehouse=env_conf.get("warehouse"),
+        results = conn.create_streamlit(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
             name=name,
             file="streamlit_app_launcher.py" if use_packaging_workaround else file.name,
             from_stage_command=from_stage_command,
         )
         print_db_cursor(results)
 
 
 @app.command("share")
 def streamlit_share(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Name of streamlit to be shared."),
     to_role: str = typer.Argument(
         ..., help="Role that streamlit should be shared with."
     ),
 ):
     """
     Create a streamlit app named NAME.
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
-        results = config.snowflake_connection.shareStreamlit(
-            database=env_conf.get("database"),
-            schema=env_conf.get("schema"),
-            role=env_conf.get("role"),
-            warehouse=env_conf.get("warehouse"),
+    if config.is_auth():
+        results = conn.share_streamlit(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
             name=name,
             to_role=to_role,
         )
         print_db_cursor(results)
 
 
 @app.command("drop")
 def streamlit_drop(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Name of streamlit to be deleted."),
 ):
     """
     Create a streamlit app named NAME.
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
-        results = config.snowflake_connection.dropStreamlit(
-            database=env_conf.get("database"),
-            schema=env_conf.get("schema"),
-            role=env_conf.get("role"),
-            warehouse=env_conf.get("warehouse"),
+    if config.is_auth():
+        results = conn.drop_streamlit(
+            database=conn.ctx.database,
+            schema=conn.ctx.schema,
+            role=conn.ctx.role,
+            warehouse=conn.ctx.warehouse,
             name=name,
         )
         print_db_cursor(results)
 
 
 @app.command("deploy")
 def streamlit_deploy(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     name: str = typer.Argument(..., help="Name of streamlit to be deployed."),
     file: Path = typer.Option(
         "streamlit_app.py",
         exists=True,
         readable=True,
         file_okay=True,
         help="Path to streamlit file",
@@ -229,109 +213,114 @@
         + "Provide a comma-separated list of package names to exclude them from "
         + "environment.yml (noting the risk of runtime errors).",
     ),
 ):
     """
     Deploy streamlit with NAME.
     """
-    env_conf = AppConfig().config.get(environment)
+    conn = connect_to_snowflake(connection_name=environment)
 
-    if config.isAuth():
-        config.connectToSnowflake()
-        schema = env_conf.get("schema")
-        role = env_conf.get("role")
-        database = env_conf.get("database")
+    if config.is_auth():
+        schema = conn.ctx.schema
+        role = conn.ctx.role
+        database = conn.ctx.database
+        warehouse = conn.ctx.warehouse
+        # THIS WORKAROUND HAS NOT BEEN TESTETD WITH THE NEW STREAMLIT SYNTAX
         if use_packaging_workaround:
-            # package an app.zip file, same as the other snowpark package commands
+            # package an app.zip file, same as the other snowpark_containers_cmds package commands
             snowpark_package(
                 pypi_download,  # type: ignore[arg-type]
                 check_anaconda_for_pypi_deps,
                 package_native_libraries,  # type: ignore[arg-type]
             )
             # upload the resulting app.zip file
-            config.snowflake_connection.uploadFileToStage(
+            conn.upload_file_to_stage(
                 "app.zip",
                 f"{name}_stage",
                 "/",
-                role,
-                database,
-                schema,
+                role=role,
+                database=database,
+                schema=schema,
+                warehouse=warehouse,
                 overwrite=True,
+                create_stage=False,
             )
             main_module = str(file).replace(".py", "")
-            file = generateStreamlitPackageWrapper(
+            file = generate_streamlit_package_wrapper(
                 stage_name=f"{name}_stage",
                 main_module=main_module,
                 extract_zip=packaging_workaround_includes_content,
             )
             # upload the wrapper file
-            config.snowflake_connection.uploadFileToStage(
+            conn.upload_file_to_stage(
                 str(file),
                 f"{name}_stage",
                 "/",
-                role,
-                database,
-                schema,
+                role=role,
+                database=database,
+                schema=schema,
+                warehouse=warehouse,
                 overwrite=True,
+                create_stage=False,
             )
             # if the packaging process generated an environment.snowflake.txt
             # file, convert it into an environment.yml file
             excluded_anaconda_deps_list: Optional[List[str]] = None
             if excluded_anaconda_deps is not None:
                 excluded_anaconda_deps_list = excluded_anaconda_deps.split(",")
-            env_file = generateStreamlitEnvironmentFile(excluded_anaconda_deps_list)
+            env_file = generate_streamlit_environment_file(excluded_anaconda_deps_list)
             if env_file:
-                config.snowflake_connection.uploadFileToStage(
+                conn.upload_file_to_stage(
                     str(env_file),
                     f"{name}_stage",
                     "/",
-                    role,
-                    database,
-                    schema,
+                    role=role,
+                    database=database,
+                    schema=schema,
+                    warehouse=warehouse,
                     overwrite=True,
+                    create_stage=False,
                 )
 
-        base_url = config.snowflake_connection.deployStreamlit(
+        base_url = conn.deploy_streamlit(
             name=name,
             file_path=str(file),
             stage_path="/",
             role=role,
             database=database,
             schema=schema,
+            warehouse=warehouse,
             overwrite=True,
         )
 
         def get_url() -> str:
             try:
-                host = config.snowflake_connection.connection_config["host"]
+                host = conn.ctx.host
             except KeyError:
                 return base_url
 
             host_parts = host.split(".")
 
             if len(host_parts) != 6:
-                print(
-                    f"""The connection host ({host}) was missing or not in
-                    the expected format
-                    (<account>.<deployment>.snowflakecomputing.com)"""
+                log.error(
+                    f"The connection host ({host}) was missing or not in "
+                    "the expected format "
+                    "(<account>.<deployment>.snowflakecomputing.com)"
                 )
                 raise typer.Exit()
             else:
                 account_name = host_parts[0]
                 deployment = ".".join(host_parts[1:4])
 
-            snowflake_host = env_conf.get(
-                "snowflake_host",
-                "app.snowflake.com",
-            )
+            snowflake_host = conn.ctx.host or "app.snowflake.com"
             uppercased_dsn = f"{database}.{schema}.{name}".upper()
             return (
                 f"https://{snowflake_host}/{deployment}/{account_name}/"
                 f"#/streamlit-apps/{uppercased_dsn}"
             )
 
         url = get_url()
 
         if open_:
             typer.launch(url)
         else:
-            print(url)
+            log.info(url)
```

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure_coverage/report.py` & `snowflake_cli_labs-1.0.0/src/snowcli/cli/snowpark/procedure_coverage/report.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,38 @@
+import logging
 import os
 import tempfile
 from enum import Enum
 
 import coverage
 import snowflake.connector
 import typer
 
 from snowcli import config, utils
-from snowcli.config import AppConfig
-from snowcli.utils import conf_callback, generate_deploy_stage_name, print_db_cursor
+from snowcli.config import connect_to_snowflake
+from snowcli.utils import generate_deploy_stage_name
 
-from . import app
+from snowcli.cli.snowpark.procedure_coverage import app
+from snowcli.cli.common.flags import ConnectionOption
 
-EnvironmentOption = typer.Option(
-    "dev",
-    help="Environment name",
-    callback=conf_callback,
-    is_eager=True,
-)
+log = logging.getLogger(__name__)
 
 
 class ReportOutputOptions(str, Enum):
     html = "html"
     json = "json"
     lcov = "lcov"
 
 
 @app.command(
     "report",
     help="Generate a code coverage report by downloading and combining reports from the stage",
 )
 def procedure_coverage_report(
-    environment: str = EnvironmentOption,
+    environment: str = ConnectionOption,
     name: str = typer.Option(
         ...,
         "--name",
         "-n",
         help="Name of the procedure",
     ),
     input_parameters: str = typer.Option(
@@ -52,26 +49,19 @@
     ),
     store_as_comment: bool = typer.Option(
         False,
         "--store-as-comment",
         help="In addition to the local report, saves the percentage coverage (a decimal value) as a comment on the stored procedure so that a coverage threshold can be easily checked for a number of procedures.",
     ),
 ):
-    env_conf = AppConfig().config.get(environment)
-    if env_conf is None:
-        print(
-            f"The {environment} environment is not configured in app.toml "
-            "yet, please run `snow configure -e dev` first before continuing.",
-        )
-        raise typer.Abort()
-    if config.isAuth():
-        config.connectToSnowflake()
-        deploy_dict = utils.getDeployNames(
-            env_conf["database"],
-            env_conf["schema"],
+    conn = connect_to_snowflake(connection_name=environment)
+    if config.is_auth():
+        deploy_dict = utils.get_deploy_names(
+            conn.ctx.database,
+            conn.ctx.schema,
             generate_deploy_stage_name(
                 name,
                 input_parameters,
             ),
         )
         coverage_file = ".coverage"
         # the coverage databases will include paths like "/home/udf/132735964617982/app.zip/app.py", where they ran on Snowflake
@@ -88,59 +78,65 @@
 
         combined_coverage = coverage.Coverage(data_file=coverage_file)
         with tempfile.TemporaryDirectory() as temp_dir:
             stage_name = deploy_dict["stage"]
             stage_path = deploy_dict["directory"]
             report_files = f"{stage_name}{stage_path}/coverage/"
             try:
-                results = config.snowflake_connection.getStage(
-                    database=env_conf.get("database"),
-                    schema=env_conf.get("schema"),
-                    role=env_conf.get("role"),
-                    warehouse=env_conf.get("warehouse"),
+                results = conn.get_stage(
+                    database=conn.ctx.database,
+                    schema=conn.ctx.schema,
+                    role=conn.ctx.role,
+                    warehouse=conn.ctx.warehouse,
                     name=report_files,
                     path=str(temp_dir),
                 ).fetchall()
             except snowflake.connector.errors.DatabaseError as database_error:
                 if database_error.errno == 253006:
                     results = []
             if len(results) == 0:
-                print(
-                    "No code coverage reports were found on the stage. Please ensure that you've invoked the procedure at least once and that you provided the correct inputs"
+                log.error(
+                    "No code coverage reports were found on the stage. "
+                    "Please ensure that you've invoked the procedure at least once "
+                    "and that you provided the correct inputs"
                 )
                 raise typer.Abort()
             else:
-                print(f"Combining data from {len(results)} reports")
+                log.info(f"Combining data from {len(results)} reports")
             combined_coverage.combine(
                 # the tuple contains the columns: | file ┃ size ┃ status ┃ message |
                 data_paths=[
                     os.path.join(temp_dir, os.path.basename(result[0]))
                     for result in results
                 ]
             )
         if output_format == ReportOutputOptions.html:
             coverage_percentage = combined_coverage.html_report()
-            print(
+            log.info(
                 "Your HTML code coverage report is now available under the 'htmlcov' folder (htmlcov/index.html)."
             )
         elif output_format == ReportOutputOptions.json:
             coverage_percentage = combined_coverage.json_report()
-            print("Your JSON code coverage report is now available in 'coverage.json'.")
+            log.info(
+                "Your JSON code coverage report is now available in 'coverage.json'."
+            )
         elif output_format == ReportOutputOptions.lcov:
             coverage_percentage = combined_coverage.lcov_report()
-            print("Your lcov code coverage report is now available in 'coverage.lcov'.")
+            log.info(
+                "Your lcov code coverage report is now available in 'coverage.lcov'."
+            )
         else:
-            print(f"Unknown output format '{output_format}'")
+            log.error(f"Unknown output format '{output_format}'")
         if store_as_comment:
-            print(
+            log.info(
                 f"Storing total coverage value of {str(coverage_percentage)} as a procedure comment."
             )
-            config.snowflake_connection.setProcedureComment(
-                env_conf["database"],
-                env_conf["schema"],
-                env_conf["role"],
-                env_conf["warehouse"],
+            conn.set_procedure_comment(
+                conn.ctx.database,
+                conn.ctx.schema,
+                conn.ctx.role,
+                conn.ctx.warehouse,
                 name=name,
-                inputParameters=input_parameters,
+                input_parameters=input_parameters,
                 show_exceptions=True,
                 comment=str(coverage_percentage),
             )
```

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/python_templates/snowpark_coverage.py.jinja` & `snowflake_cli_labs-1.0.0/src/snowcli/python_templates/snowpark_coverage.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.9/src/snowcli/python_templates/streamlit_app_launcher.py.jinja` & `snowflake_cli_labs-1.0.0/src/snowcli/python_templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.9/src/templates/default_procedure/local_connection.py` & `snowflake_cli_labs-1.0.0/src/templates/default_procedure/local_connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         session_config_dict = {
             k.replace("name", ""): v.strip('"') for k, v in session_config.items()
         }
         session_config_dict.update(app_config.get(environment))  # type: ignore
         return session_config_dict
     except Exception:
         raise Exception(
-            "Error creating snowpark session - be sure you've logged into "
+            "Error creating snowpark_containers_cmds session - be sure you've logged into "
             "the SnowCLI and have a valid app.toml file",
         )
```

### Comparing `snowflake_cli_labs-0.2.9/tests/test_render.py` & `snowflake_cli_labs-1.0.0/tests/test_render.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                             "name": "APP.PYTHON_HELLO",
                             "signature": [
                                 {"name": "arg1", "type": "STRING"},
                             ],
                             "returns": "STRING",
                             "language": "PYTHON",
                             "runtime_version": "3.8",
-                            "packages": "snowflake-snowpark-python",
+                            "packages": "snowflake-snowpark_containers_cmds-python",
                             "imports": [
                                 "/module.zip",
                             ],
                             "handler": "module.procedures.python_hello",
                             "grants": [{"role": "APP_ROLE", "grant": "USAGE"}],
                         }
                     ]
@@ -98,15 +98,15 @@
         == """\
 CREATE OR REPLACE PROCEDURE APP.PYTHON_HELLO(    
 ARG1 STRING
 )
 RETURNS STRING
 LANGUAGE PYTHON
 RUNTIME_VERSION = '3.8'
-PACKAGES = ('snowflake-snowpark-python')
+PACKAGES = ('snowflake-snowpark_containers_cmds-python')
 IMPORTS = ('/module.zip')
 HANDLER = 'module.procedures.python_hello'
 ;
 GRANT USAGE ON PROCEDURE APP.PYTHON_HELLO(STRING)
 TO DATABASE ROLE APP_ROLE;
 
 """
```

### Comparing `snowflake_cli_labs-0.2.9/tests/test_snow_connector.py` & `snowflake_cli_labs-1.0.0/tests/test_snow_connector.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,81 @@
 import textwrap
+from pathlib import Path
 from unittest import mock
 
 import pytest
+
 from snowcli.snow_connector import SnowflakeConnector
 
 
 # Used as a solution to syrupy having some problems with comparing multilines string
-class custom_str(str):
+class CustomStr(str):
     def __repr__(self):
         return str(self)
 
 
+MOCK_CONNECTION = {
+    "database": "databaseValue",
+    "schema": "schemaValue",
+    "role": "roleValue",
+    "warehouse": "warehouseValue",
+}
+
+
+@pytest.mark.parametrize(
+    "cmd,expected",
+    [
+        (["sql", "-q", "foo"], "SNOWCLI.SQL"),
+        (["warehouse", "status"], "SNOWCLI.WAREHOUSE.STATUS"),
+    ],
+)
+@mock.patch("snowcli.snow_connector.snowflake.connector.connect")
+def test_command_context_is_passed_to_snowflake_connection(
+    mock_conn, runner, cmd, expected
+):
+    mock_conn.return_value.execute_stream.return_value = (mock.MagicMock(),)
+    result = runner.invoke_with_config(cmd)
+    assert result.exit_code == 0, result.output
+    kwargs = mock_conn.call_args_list[-1][-1]
+    assert "application" in kwargs
+    assert kwargs["application"] == expected
+
+
 @mock.patch("snowflake.connector")
-def test_createFunction(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_create_function(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.createFunction(
+    connector.create_function(
         name="nameValue",
-        inputParameters="(string a, variant b)",
-        returnType="returnTypeValue",
+        input_parameters="(string a, variant b)",
+        return_type="returnTypeValue",
         handler="handlerValue",
         imports="import1, import2",
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         overwrite=True,
         packages=["aaa", "bbb"],
     )
     query_io, *_ = connector.ctx.execute_stream.call_args.args
     query_str = query_io.getvalue()
-    print(custom_str(query_str))
-    assert custom_str(query_str) == snapshot
+    assert CustomStr(query_str) == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_createProcedure(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_create_procedure(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.createProcedure(
+    connector.create_procedure(
         name="nameValue",
-        inputParameters="(string a, variant b)",
-        returnType="returnTypeValue",
+        input_parameters="(string a, variant b)",
+        return_type="returnTypeValue",
         handler="handlerValue",
         imports="import1, import2",
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         overwrite=True,
@@ -59,470 +83,707 @@
         execute_as_caller=True,
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_executeFunction(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_execute_function(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.executeFunction(
+    connector.execute_function(
         function="functionValue",
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_executeProcedure(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_execute_procedure(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.executeProcedure(
+    connector.execute_procedure(
         procedure="procedureValue",
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_describeFunction(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_describe_function(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.describeFunction(
+    connector.describe_function(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         signature="signatureValue",
         name="nameValue",
-        inputParameters="(string a, variant b)",
+        input_parameters="(string a, variant b)",
         show_exceptions="show_exceptionsValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_describeProcedure(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_describe_procedure(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.describeProcedure(
+    connector.describe_procedure(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         signature="signatureValue",
         name="nameValue",
-        inputParameters="(string a, variant b)",
+        input_parameters="(string a, variant b)",
         show_exceptions="show_exceptionsValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_listFunctions(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_list_functions(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.listFunctions(
+    connector.list_functions(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         like="likeValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_listStages(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_list_stages(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.listStages(
+    connector.list_stages(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         like="likeValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
-@pytest.mark.parametrize(
-    "stage_name", [("namedStageValue"), ("snow://embeddedStageValue")]
-)
+@pytest.mark.parametrize("stage_name", ["namedStageValue", "snow://embeddedStageValue"])
 @mock.patch("snowflake.connector")
-def test_listStage(_, snapshot, stage_name):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_list_stage(_, snapshot, stage_name):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.listStage(
+    connector.list_stage(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name=stage_name,
         like="likeValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
-@pytest.mark.parametrize(
-    "stage_name", [("namedStageValue"), ("snow://embeddedStageValue")]
-)
+@pytest.mark.parametrize("stage_name", ["namedStageValue", "snow://embeddedStageValue"])
 @mock.patch("snowflake.connector")
-def test_getStage(_, snapshot, stage_name):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_get_stage(_, snapshot, stage_name):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.getStage(
+    connector.get_stage(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name=stage_name,
         path="pathValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_setProcedureComment(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_set_procedure_comment(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.setProcedureComment(
+    connector.set_procedure_comment(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         signature="signatureValue",
         name="nameValue",
-        inputParameters="(string a, variant b)",
+        input_parameters="(string a, variant b)",
         show_exceptions="show_exceptionsValue",
         comment="commentValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
-@pytest.mark.parametrize(
-    "stage_name", [("namedStageValue"), ("snow://embeddedStageValue")]
-)
+@pytest.mark.parametrize("stage_name", ["namedStageValue", "snow://embeddedStageValue"])
 @mock.patch("snowflake.connector")
-def test_putStage(_, snapshot, stage_name):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_put_stage(_, snapshot, stage_name):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.putStage(
+    connector.put_stage(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name=stage_name,
         path="pathValue",
         overwrite=True,
-        parallel="parallelValue",
+        parallel=42,
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert textwrap.dedent(query.getvalue()) == snapshot
 
 
-@pytest.mark.parametrize(
-    "stage_name", [("namedStageValue"), ("snow://embeddedStageValue")]
-)
+@pytest.mark.parametrize("stage_name", ["namedStageValue", "snow://embeddedStageValue"])
 @mock.patch("snowflake.connector")
-def test_removeFromStage(_, snapshot, stage_name):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_remove_from_stage(_, snapshot, stage_name):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.removeFromStage(
+    connector.remove_from_stage(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name=stage_name,
         path="/pathValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_createStage(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_create_stage(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.createStage(
+    connector.create_stage(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name="nameValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_dropStage(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_drop_stage(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.dropStage(
+    connector.drop_stage(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name="nameValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_listProcedures(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_list_procedures(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.listProcedures(
+    connector.list_procedures(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         like="likeValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_dropFunction(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_drop_function(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.dropFunction(
+    connector.drop_function(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         signature="signatureValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_dropProcedure(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_drop_procedure(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.dropProcedure(
+    connector.drop_procedure(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         signature="signatureValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_listStreamlits(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_list_streamlits(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.listStreamlits(
+    connector.list_streamlits(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_showWarehouses(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_show_warehouses(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.showWarehouses(
+    connector.show_warehouses(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         like="likeValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_createStreamlit(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_create_streamlit(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.createStreamlit(
+    connector.create_streamlit(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name="nameValue",
         file="fileValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_createStreamlitFromStage(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_create_streamlit_from_stage(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.createStreamlit(
+    connector.create_streamlit(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name="nameValue",
         file="fileValue",
         from_stage_command="FROM @stageValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_shareStreamlit(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_share_streamlit(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.shareStreamlit(
+    connector.share_streamlit(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name="nameValue",
         to_role="to_roleValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_dropStreamlit(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_drop_streamlit(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.dropStreamlit(
+    connector.drop_streamlit(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name="nameValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
-def test_deployStreamlit(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
-    )
+def test_deploy_streamlit(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (mock.MagicMock(),)
-    connector.uploadFileToStage = mock.MagicMock()
+    connector.upload_file_to_stage = mock.MagicMock()
 
-    connector.deployStreamlit(
+    connector.deploy_streamlit(
         name="nameValue",
         file_path="file_pathValue",
         stage_path="stage_pathValue",
         role="roleValue",
         database="databaseValue",
         schema="schemaValue",
+        warehouse="warehouseValue",
         overwrite=True,
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
+@pytest.mark.parametrize(
+    "create_stage",
+    [True, False],
+)
+@pytest.mark.parametrize("stage_name", ["namedStageValue", "snow://embeddedStageValue"])
 @mock.patch("snowflake.connector")
-def test_describeStreamlit(_, snapshot):
-    connector = SnowflakeConnector(
-        connection_name="foo", snowsql_config=mock.MagicMock()
+def test_upload_file_to_stage(_, snapshot, create_stage, stage_name):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.upload_file_to_stage(
+        file_path="file_pathValue",
+        destination_stage=stage_name,
+        path="pathValue",
+        role="roleValue",
+        database="databaseValue",
+        schema="schemaValue",
+        warehouse="warehouseValue",
+        overwrite="overwriteValue",
+        create_stage=create_stage,
     )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_describe_streamlit(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
     connector.ctx.execute_stream.return_value = (None, None)
 
-    connector.describeStreamlit(
+    connector.describe_streamlit(
         name="nameValue",
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_create_cp(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.create_compute_pool(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        name="nameValue",
+        num_instances=42,
+        instance_family="instance_familyValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_list_cp(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.list_compute_pools(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_drop_cp(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.drop_compute_pool(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        name="nameValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_stop_cp(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.stop_compute_pool(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        name="nameValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowcli.snow_connector.hashlib.md5")
+@mock.patch("snowcli.snow_connector.open")
+@mock.patch("snowflake.connector")
+def test_job_service(_, __, mock_md5, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+    mock_md5.return_value.hexdigest.return_value = "4231"
+
+    connector.create_job(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        compute_pool="compute_poolValue",
+        spec_path="test_spec.yaml",
+        stage="stageValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_desc_job(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.desc_job(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        id="idValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_logs_job(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.logs_job(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        id="idValue",
+        container_name="container_nameValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_status_job(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.status_job(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        id="idValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_drop_job(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.drop_job(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        id="idValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowcli.cli.snowpark.registry.connect_to_snowflake")
+def test_registry_get_token(mock_conn, runner):
+    mock_conn.return_value.ctx._rest._token_request.return_value = {
+        "data": {
+            "sessionToken": "token1234",
+            "validityInSecondsST": 42,
+        }
+    }
+    result = runner.invoke(["snowpark", "registry", "token"])
+    assert result.exit_code == 0, result.output
+    assert result.stdout == '{"token": "token1234", "expires_in": 42}'
+
+
+@mock.patch("snowcli.snow_connector.hashlib.md5")
+@mock.patch("snowcli.snow_connector.open")
+@mock.patch("snowflake.connector")
+def test_create_service(_, __, mock_md5, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+    mock_md5.return_value.hexdigest.return_value = "4231"
+    connector.create_service(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        name="nameValue",
+        compute_pool="compute_poolValue",
+        num_instances=42,
+        spec_path="test_spec.yaml",
+        stage="stageValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_desc_services(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.desc_service(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        name="nameValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_logs_services(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.logs_service(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        name="nameValue",
+        instance_id="0",
+        container_name="container_nameValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_status_services(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.status_service(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        name="nameValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_list_services(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.list_service(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
+def test_drop_services(_, snapshot):
+    connector = SnowflakeConnector(connection_parameters=MOCK_CONNECTION)
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.drop_service(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        name="nameValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
```

### Comparing `snowflake_cli_labs-0.2.9/tests/test_sql.py` & `snowflake_cli_labs-1.0.0/tests/test_sql.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,107 @@
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from unittest import mock
 
-CONFIG_MOCK = "snowcli.cli.sql.config"
+from tests.testing_utils.result_assertions import assert_that_result_is_usage_error
 
+MOCK_CONNECTION = "snowcli.cli.sql.config.connect_to_snowflake"
 
-@mock.patch(CONFIG_MOCK)
-def test_sql_execute_query(mock_config, runner):
+
+@mock.patch(MOCK_CONNECTION)
+def test_sql_execute_query(mock_conn, runner):
     result = runner.invoke(["sql", "-q", "query"])
 
     assert result.exit_code == 0
-    mock_config.snowflake_connection.ctx.execute_string.assert_called_once_with(
+    mock_conn.return_value.ctx.execute_string.assert_called_once_with(
         sql_text="query", remove_comments=True, cursor_class=mock.ANY
     )
 
 
-@mock.patch(CONFIG_MOCK)
-def test_sql_execute_file(mock_config, runner):
+@mock.patch(MOCK_CONNECTION)
+def test_sql_execute_file(mock_conn, runner):
     with NamedTemporaryFile("r") as tmp_file:
         Path(tmp_file.name).write_text("query from file")
         result = runner.invoke(["sql", "-f", tmp_file.name])
 
     assert result.exit_code == 0
-    mock_config.snowflake_connection.ctx.execute_string.assert_called_once_with(
+    mock_conn.return_value.ctx.execute_string.assert_called_once_with(
         sql_text="query from file", remove_comments=True, cursor_class=mock.ANY
     )
 
 
-@mock.patch(CONFIG_MOCK)
-def test_sql_execute_from_stdin(mock_config, runner):
+@mock.patch(MOCK_CONNECTION)
+def test_sql_execute_from_stdin(mock_conn, runner):
     result = runner.invoke(["sql"], input="query from input")
 
     assert result.exit_code == 0
-    mock_config.snowflake_connection.ctx.execute_string.assert_called_once_with(
+    mock_conn.return_value.ctx.execute_string.assert_called_once_with(
         sql_text="query from input", remove_comments=True, cursor_class=mock.ANY
     )
 
 
-def test_sql_execute_from_stdin_with_other_query_source(runner):
-    with NamedTemporaryFile("r") as tmp_file:
-        result = runner.invoke(["sql", "-f", tmp_file.name], input="query from input")
+def test_sql_fails_if_no_query_file_or_stdin(runner):
+    result = runner.invoke(["sql"])
 
-    assert result.exit_code == 1
-    assert "Can't use stdin input together with query or filename" in str(result)
+    assert_that_result_is_usage_error(
+        result, "Provide either query or filename argument"
+    )
 
 
-def test_sql_execute_fails_if_no_query_file_or_stdin(runner):
-    result = runner.invoke(
-        ["sql"],
-    )
+def test_sql_fails_for_both_stdin_and_other_query_source(runner):
+    with NamedTemporaryFile("r") as tmp_file:
+        result = runner.invoke(["sql", "-f", tmp_file.name], input="query from input")
 
-    assert result.exit_code == 1
-    assert "Provide either query or filename argument" in str(result)
+    assert_that_result_is_usage_error(
+        result, "Can't use stdin input together with query or filename"
+    )
 
 
 def test_sql_fails_for_both_query_and_file(runner):
     with NamedTemporaryFile("r") as tmp_file:
         result = runner.invoke(["sql", "-f", tmp_file.name, "-q", "query"])
 
-    assert result.exit_code == 1
-    assert "Both query and file provided" in str(result)
+    assert_that_result_is_usage_error(result, "Both query and file provided")
+
+
+@mock.patch("snowcli.cli.sql.config.is_auth")
+def test_sql_fails_if_user_not_authenticated(mock_is_auth, runner):
+    mock_is_auth.return_value = False
+    result = runner.invoke(["sql", "-q", "select 1"])
+
+    assert_that_result_is_usage_error(result, "Not authenticated")
 
 
-@mock.patch("snowcli.config.AppConfig")
 @mock.patch("snowflake.connector.connect")
-@mock.patch("snowcli.cli.sql.config.isAuth")
-def test_sql_overrides_connection_configuration(_, mock_conn, mock_app_config, runner):
-    with NamedTemporaryFile() as tmp:
-        Path(tmp.name).write_text("[connections.fooConn]")
-
-        mock_app_config.return_value.config = {"snowsql_config_path": tmp.name}
-        result = runner.invoke(
-            [
-                "sql",
-                "-q",
-                "select 1",
-                "--connection",
-                "fooConn",
-                "--accountname",
-                "accountnameValue",
-                "--username",
-                "usernameValue",
-                "--dbname",
-                "dbnameValue",
-                "--schemaname",
-                "schemanameValue",
-                "--rolename",
-                "rolenameValue",
-                "--warehouse",
-                "warehouseValue",
-            ]
-        )
+@mock.patch("snowcli.config.cli_config")
+def test_sql_overrides_connection_configuration(mock_config, mock_conn, runner):
+    mock_config.get_connection.return_value = {}
+    result = runner.invoke(
+        [
+            "sql",
+            "-q",
+            "select 1",
+            "--accountname",
+            "accountnameValue",
+            "--username",
+            "usernameValue",
+            "--dbname",
+            "dbnameValue",
+            "--schemaname",
+            "schemanameValue",
+            "--rolename",
+            "rolenameValue",
+            "--warehouse",
+            "warehouseValue",
+        ]
+    )
 
     assert result.exit_code == 0
     mock_conn.assert_called_once_with(
+        application="SNOWCLI.SQL",
         account="accountnameValue",
         user="usernameValue",
         warehouse="warehouseValue",
-        role="rolenameValue",
         database="dbnameValue",
         schema="schemanameValue",
-        application="SNOWCLI",
+        role="rolenameValue",
     )
```

### Comparing `snowflake_cli_labs-0.2.9/tests/__snapshots__/test_snow_connector.ambr` & `snowflake_cli_labs-1.0.0/tests/__snapshots__/test_snow_connector.ambr`

 * *Files 21% similar despite different names*

```diff
@@ -1,316 +1,540 @@
 # serializer version: 1
-# name: test_createFunction
+# name: test_create_cp
   '''
+  use role roleValue;
+  use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
+  
+  CREATE COMPUTE POOL nameValue
+    MIN_NODES = 42
+    MAX_NODES = 42
+    INSTANCE_FAMILY = instance_familyValue;
+  '''
+# ---
+# name: test_create_function
+  '''
+  use role roleValue;
   use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
   CREATE OR REPLACE  FUNCTION nameValue(string a, variant b)
            RETURNS returnTypeValue
            LANGUAGE PYTHON
            RUNTIME_VERSION=3.8
            IMPORTS=('import1, import2')
            HANDLER='handlerValue'
            PACKAGES=('aaa','bbb');
   describe function nameValue(a, b);
   '''
 # ---
-# name: test_createProcedure
+# name: test_create_procedure
   '''
+  use role roleValue;
+  use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
-  use warehouse warehouseValue;
-  
   CREATE OR REPLACE  PROCEDURE nameValue(string a, variant b)
            RETURNS returnTypeValue
            LANGUAGE PYTHON
            RUNTIME_VERSION=3.8
            IMPORTS=('import1, import2')
            HANDLER='handlerValue'
            PACKAGES=('aaa','bbb')
            EXECUTE AS CALLER;
   
   
   describe PROCEDURE nameValue(a, b);
   '''
 # ---
-# name: test_createStage
+# name: test_create_service
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
-  create stage if not exists nameValue;
+  CREATE STAGE IF NOT EXISTS stageValue;
+  
+  put file://test_spec.yaml @stageValue/services/4231 auto_compress=false OVERWRITE = TRUE;
+  
+  CREATE SERVICE IF NOT EXISTS nameValue
+    MIN_INSTANCES = 42
+    MAX_INSTANCES = 42
+    COMPUTE_POOL =  compute_poolValue
+    spec=@stageValue/services/4231/test_spec.yaml;
   '''
 # ---
-# name: test_createStreamlit
+# name: test_create_stage
   '''
   use role roleValue;
+  use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
-  use warehouse warehouseValue;
   
+  create stage if not exists nameValue;
+  '''
+# ---
+# name: test_create_streamlit
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
   create streamlit nameValue
     
     MAIN_FILE = 'fileValue'
     QUERY_WAREHOUSE = warehouseValue;
   
   show streamlits;
   describe streamlit nameValue;
   
   alter streamlit nameValue checkout;
   '''
 # ---
-# name: test_createStreamlitFromStage
+# name: test_create_streamlit_from_stage
   '''
   use role roleValue;
+  use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
-  use warehouse warehouseValue;
-  
   create streamlit nameValue
     FROM @stageValue
     MAIN_FILE = 'fileValue'
     QUERY_WAREHOUSE = warehouseValue;
   
   show streamlits;
   describe streamlit nameValue;
   
   alter streamlit nameValue checkout;
   '''
 # ---
-# name: test_deployStreamlit
+# name: test_deploy_streamlit
   '''
+  use role roleValue;
+  
   use database databaseValue;
   use schema schemaValue;
-  use role roleValue;
   
   CALL SYSTEM$GENERATE_STREAMLIT_URL_FROM_NAME('nameValue');
   '''
 # ---
-# name: test_describeFunction
+# name: test_desc_job
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  desc service idValue;
+  '''
+# ---
+# name: test_desc_services
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  desc service nameValue;
+  '''
+# ---
+# name: test_describe_function
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   desc FUNCTION signatureValue;
   '''
 # ---
-# name: test_describeProcedure
+# name: test_describe_procedure
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   desc PROCEDURE signatureValue;
   '''
 # ---
-# name: test_describeStreamlit
+# name: test_describe_streamlit
   '''
+  use role roleValue;
+  
   use database databaseValue;
   use schema schemaValue;
-  use role roleValue;
   
   CALL SYSTEM$GENERATE_STREAMLIT_URL_FROM_NAME('nameValue');
   '''
 # ---
-# name: test_dropFunction
+# name: test_drop_cp
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  drop compute pool nameValue;
+  '''
+# ---
+# name: test_drop_function
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   drop function signatureValue;
   '''
 # ---
-# name: test_dropProcedure
+# name: test_drop_job
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  call SYSTEM$CANCEL_JOB('idValue');
+  '''
+# ---
+# name: test_drop_procedure
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   drop procedure signatureValue;
   '''
 # ---
-# name: test_dropStage
+# name: test_drop_services
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
-  drop stage nameValue;
+  DROP SERVICE nameValue;
   '''
 # ---
-# name: test_dropStreamlit
+# name: test_drop_stage
   '''
   use role roleValue;
+  use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
+  
+  drop stage nameValue;
+  '''
+# ---
+# name: test_drop_streamlit
+  '''
+  use role roleValue;
   use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
   drop streamlit "nameValue";
   '''
 # ---
-# name: test_executeFunction
+# name: test_execute_function
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   select functionValue;
   '''
 # ---
-# name: test_executeProcedure
+# name: test_execute_procedure
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   call procedureValue;
   '''
 # ---
-# name: test_getStage[namedStageValue]
+# name: test_get_stage[namedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
   get @namedStageValue file://pathValue/
   '''
 # ---
-# name: test_getStage[snow://embeddedStageValue]
+# name: test_get_stage[snow://embeddedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
   get snow://embeddedStageValue file://pathValue/
   '''
 # ---
-# name: test_listFunctions
+# name: test_job_service
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  CREATE STAGE IF NOT EXISTS stageValue;
+  
+  put file://test_spec.yaml @stageValue/jobs/4231 auto_compress=false OVERWRITE = TRUE;
+  
+  EXECUTE SERVICE
+    COMPUTE_POOL =  compute_poolValue
+    spec=@stageValue/jobs/4231/test_spec.yaml;
+  '''
+# ---
+# name: test_list_cp
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  show compute pools;
+  '''
+# ---
+# name: test_list_functions
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   show user functions like 'likeValue';
   select "name", "created_on", "arguments", "language" from table(result_scan(last_query_id()));
   '''
 # ---
-# name: test_listProcedures
+# name: test_list_procedures
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   show user procedures like 'likeValue';
   select "name", "created_on", "arguments" from table(result_scan(last_query_id()));
   '''
 # ---
-# name: test_listStage[namedStageValue]
+# name: test_list_services
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  show services;
+  '''
+# ---
+# name: test_list_stage[namedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   ls @namedStageValue;
   '''
 # ---
-# name: test_listStage[snow://embeddedStageValue]
+# name: test_list_stage[snow://embeddedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   ls snow://embeddedStageValue;
   '''
 # ---
-# name: test_listStages
+# name: test_list_stages
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   show stages;
   '''
 # ---
-# name: test_listStreamlits
+# name: test_list_streamlits
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   show streamlits;
   '''
 # ---
-# name: test_putStage[namedStageValue]
+# name: test_logs_job
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  call SYSTEM$GET_JOB_LOGS('idValue', 'container_nameValue');
+  '''
+# ---
+# name: test_logs_services
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
-  put file://pathValue @namedStageValue auto_compress=false parallel=parallelValue overwrite=True;
+  call SYSTEM$GET_SERVICE_LOGS('nameValue', '0', 'container_nameValue');
   '''
 # ---
-# name: test_putStage[snow://embeddedStageValue]
+# name: test_put_stage[namedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
-  put file://pathValue snow://embeddedStageValue auto_compress=false parallel=parallelValue overwrite=True;
+  
+  
+  put file://pathValue @namedStageValue auto_compress=false parallel=42 overwrite=True;
   '''
 # ---
-# name: test_removeFromStage[namedStageValue]
+# name: test_put_stage[snow://embeddedStageValue]
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  
+  
+  put file://pathValue snow://embeddedStageValue auto_compress=false parallel=42 overwrite=True;
+  '''
+# ---
+# name: test_remove_from_stage[namedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
   remove @namedStageValue/pathValue
   '''
 # ---
-# name: test_removeFromStage[snow://embeddedStageValue]
+# name: test_remove_from_stage[snow://embeddedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
   remove snow://embeddedStageValue/pathValue
   '''
 # ---
-# name: test_setProcedureComment
+# name: test_set_procedure_comment
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   alter PROCEDURE signatureValue SET COMMENT = $$commentValue$$;
   '''
 # ---
-# name: test_shareStreamlit
+# name: test_share_streamlit
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
   grant usage on streamlit nameValue to role to_roleValue;
   '''
 # ---
-# name: test_showWarehouses
+# name: test_show_warehouses
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   show warehouses;
   '''
 # ---
+# name: test_status_job
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  CALL SYSTEM$GET_JOB_STATUS('idValue');
+  '''
+# ---
+# name: test_status_services
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  CALL SYSTEM$GET_SERVICE_STATUS('nameValue');
+  '''
+# ---
+# name: test_stop_cp
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  alter compute pool nameValue stop all services;
+  '''
+# ---
+# name: test_upload_file_to_stage[namedStageValue-False]
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  
+  
+  put file://file_pathValue @namedStageValuepathValue auto_compress=false parallel=4 overwrite=overwriteValue;
+  '''
+# ---
+# name: test_upload_file_to_stage[namedStageValue-True]
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  
+  create stage if not exists namedStageValue comment='deployments managed by snowcli';
+  
+  
+  put file://file_pathValue @namedStageValuepathValue auto_compress=false parallel=4 overwrite=overwriteValue;
+  '''
+# ---
+# name: test_upload_file_to_stage[snow://embeddedStageValue-False]
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  
+  
+  put file://file_pathValue snow://embeddedStageValuepathValue auto_compress=false parallel=4 overwrite=overwriteValue;
+  '''
+# ---
+# name: test_upload_file_to_stage[snow://embeddedStageValue-True]
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  
+  create stage if not exists snow://embeddedStageValue comment='deployments managed by snowcli';
+  
+  
+  put file://file_pathValue snow://embeddedStageValuepathValue auto_compress=false parallel=4 overwrite=overwriteValue;
+  '''
+# ---
```

### Comparing `snowflake_cli_labs-0.2.9/LICENSE` & `snowflake_cli_labs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.9/pyproject.toml` & `snowflake_cli_labs-1.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -8,35 +8,44 @@
 license = "Apache-2.0"
 license_files = ["LICENSE"]
 dynamic = ["version"]
 requires-python = ">=3.8"
 description = "Snowflake CLI"
 readme = "README.md"
 dependencies = [
-  "coverage",
-  "jinja2",
-  "pyyaml",
-  "requirements-parser",
-  "rich",
-  "snowflake-connector-python[secure-local-storage]",
-  "toml",
-  "typer"
+  "coverage==7.2.7",
+  "jinja2==3.1.2",
+  "rich==13.4.2",
+  "requests==2.28.1",
+  "requirements-parser==0.5.0",
+#  "snowflake-connector-python==3.0.4",
+  "snowflake-connector-python-nightly==2023.6.24",
+  "tomlkit==0.11.8",
+  "typer==0.9.0",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: SQL",
   "Topic :: Database"
 ]
 
+[project.optional-dependencies]
+dev = [
+  "pre-commit==3.3.3",
+  "pytest==7.4.0",
+  "syrupy==4.0.4",
+  "tox==4.6.3",
+]
+
 [project.urls]
 "Source code" = "https://github.com/Snowflake-Labs/snowcli"
 "Bug Tracker" = "https://github.com/Snowflake-Labs/snowcli/issues"
 
 [project.scripts]
 snow = "snowcli.cli:app"
 
@@ -53,7 +62,13 @@
 
 [tool.ruff]
 line-length = 88
 select = [
     # isort
     "I001"
 ]
+
+[tool.pytest.ini_options]
+addopts = "-m 'not integration'"
+markers = [
+  "integration: mark test as integration test",
+]
```

