# Comparing `tmp/fractal_server-1.3.0a9.tar.gz` & `tmp/fractal_server-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.3.0a9.tar", max compression
+gzip compressed data, was "fractal_server-1.3.1.tar", max compression
```

## Comparing `fractal_server-1.3.0a9.tar` & `fractal_server-1.3.1.tar`

### file list

```diff
@@ -1,107 +1,99 @@
--rw-r--r--   0        0        0     1576 2022-12-15 19:55:06.212112 fractal_server-1.3.0a9/LICENSE
--rw-r--r--   0        0        0     2100 2023-06-20 19:21:04.815875 fractal_server-1.3.0a9/README.md
--rw-r--r--   0        0        0       69 2022-12-15 19:55:06.216112 fractal_server-1.3.0a9/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-06-21 08:32:07.752695 fractal_server-1.3.0a9/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-12-15 19:55:06.216112 fractal_server-1.3.0a9/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      952 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     7616 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/_aux_functions.py
--rw-r--r--   0        0        0     7624 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/dataset.py
--rw-r--r--   0        0        0     4817 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0     8880 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    15912 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    12866 2023-06-21 08:31:20.096225 fractal_server-1.3.0a9/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     3081 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3412 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/job.py
--rw-r--r--   0        0        0      309 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     2355 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     2563 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1119 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     2535 2023-06-21 08:31:20.096225 fractal_server-1.3.0a9/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5205 2023-06-21 08:31:20.096225 fractal_server-1.3.0a9/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0    10102 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19523 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5464 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3245 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3839 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     4331 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19766 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    42200 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     7900 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0    11324 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-06-20 20:07:43.590964 fractal_server-1.3.0a9/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-06-20 20:09:45.855554 fractal_server-1.3.0a9/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0       57 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      425 2023-06-20 20:09:08.951386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-06-20 20:09:08.971386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1624 2023-06-20 20:09:08.951386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     4082 2023-06-20 20:09:08.975386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     3551 2023-06-20 20:09:08.975386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     1179 2023-06-20 20:09:08.983386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     2719 2023-06-20 20:09:08.983386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     3306 2023-06-20 20:09:08.991386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1216 2023-06-20 20:09:08.991386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     3896 2023-06-20 20:09:09.235387 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3479 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     2578 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0     2935 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-06-20 20:09:08.927385 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      620 2023-06-20 20:09:08.947386 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-06-20 20:09:09.247387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1255 2023-06-20 20:09:09.247387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1178 2023-06-20 20:09:09.251387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-06-20 20:09:09.251387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2806 2023-06-20 20:09:09.255387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1349 2023-06-20 20:09:09.259387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2685 2023-06-20 20:09:09.263387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2925 2023-06-20 20:09:09.263387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0     1420 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0      968 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12432 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/logger.py
--rw-r--r--   0        0        0     5935 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-12-15 19:55:06.216112 fractal_server-1.3.0a9/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-12-15 19:55:06.216112 fractal_server-1.3.0a9/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     8770 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0      746 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2022-12-15 19:55:06.216112 fractal_server-1.3.0a9/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    17581 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/utils.py
--rw-r--r--   0        0        0     2704 2023-06-21 08:32:07.752695 fractal_server-1.3.0a9/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 fractal_server-1.3.0a9/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-06-23 06:18:06.498772 fractal_server-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2100 2023-06-23 06:18:06.498772 fractal_server-1.3.1/README.md
+-rw-r--r--   0        0        0       69 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/.gitignore
+-rw-r--r--   0        0        0       22 2023-06-27 14:52:47.431576 fractal_server-1.3.1/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     1242 2023-06-27 14:23:44.473555 fractal_server-1.3.1/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     7622 2023-06-27 14:28:32.735643 fractal_server-1.3.1/fractal_server/app/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0     7624 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/api/v1/dataset.py
+-rw-r--r--   0        0        0     4990 2023-06-27 14:51:02.824508 fractal_server-1.3.1/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0     8880 2023-06-27 14:30:25.873556 fractal_server-1.3.1/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0     5516 2023-06-27 14:23:44.473555 fractal_server-1.3.1/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    10831 2023-06-27 14:23:44.473555 fractal_server-1.3.1/fractal_server/app/api/v1/task_collection.py
+-rw-r--r--   0        0        0     9246 2023-06-27 14:23:44.473555 fractal_server-1.3.1/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     5165 2023-06-27 14:23:44.473555 fractal_server-1.3.1/fractal_server/app/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     3081 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3412 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0      309 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     2355 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     2563 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1119 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     2535 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5205 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0    10102 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19523 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5464 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3245 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3839 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     4331 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19766 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    42200 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     7900 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0    11324 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-26 06:59:30.472776 fractal_server-1.3.1/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-26 06:59:32.128764 fractal_server-1.3.1/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       57 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-26 06:59:32.128764 fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-06-26 06:59:32.128764 fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1624 2023-06-26 06:59:32.128764 fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4082 2023-06-26 06:59:32.132763 fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     3551 2023-06-26 06:59:32.132763 fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     1179 2023-06-26 06:59:32.140764 fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     2719 2023-06-26 06:59:32.140764 fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     3306 2023-06-26 06:59:32.144764 fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1216 2023-06-26 06:59:32.148764 fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     3896 2023-06-26 06:59:32.152763 fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      139 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0     1420 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0      968 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-06-26 06:59:30.480776 fractal_server-1.3.1/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12432 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-06-27 14:30:25.873556 fractal_server-1.3.1/fractal_server/logger.py
+-rw-r--r--   0        0        0     5935 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     8770 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0      746 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    17581 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-06-23 06:18:06.502771 fractal_server-1.3.1/fractal_server/utils.py
+-rw-r--r--   0        0        0     2700 2023-06-27 14:52:47.431576 fractal_server-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3544 1970-01-01 00:00:00.000000 fractal_server-1.3.1/PKG-INFO
```

### Comparing `fractal_server-1.3.0a9/LICENSE` & `fractal_server-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/README.md` & `fractal_server-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/__main__.py` & `fractal_server-1.3.1/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/alembic.ini` & `fractal_server-1.3.1/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/api/__init__.py` & `fractal_server-1.3.1/fractal_server/app/api/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,24 +5,30 @@
 
 from ...config import get_settings
 from ...syringe import Inject
 from .v1.dataset import router as dataset_router
 from .v1.job import router as job_router
 from .v1.project import router as project_router
 from .v1.task import router as task_router
+from .v1.task_collection import router as taskcollection_router
 from .v1.workflow import router as workflow_router
+from .v1.workflowtask import router as workflowtask_router
 
 
 router_default = APIRouter()
 router_v1 = APIRouter()
 
 router_v1.include_router(project_router, prefix="/project", tags=["Projects"])
 router_v1.include_router(task_router, prefix="/task", tags=["Tasks"])
+router_v1.include_router(
+    taskcollection_router, prefix="/task", tags=["Task Collection"]
+)
 router_v1.include_router(dataset_router, tags=["Datasets"])
 router_v1.include_router(workflow_router, tags=["Workflows"])
+router_v1.include_router(workflowtask_router, tags=["Workflow Tasks"])
 router_v1.include_router(job_router, tags=["Jobs"])
 
 
 @router_default.get("/alive/")
 async def alive():
     settings = Inject(get_settings)
     return dict(
```

### Comparing `fractal_server-1.3.0a9/fractal_server/app/api/v1/_aux_functions.py` & `fractal_server-1.3.1/fractal_server/app/api/v1/_aux_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
 async def _get_job_check_owner(
     *,
     project_id: int,
     job_id: int,
     user_id: int,
     db: AsyncSession,
-) -> dict[str, Union[Dataset, Project]]:
+) -> dict[str, Union[ApplyWorkflow, Project]]:
     """
     Get a job and a project, after access control on the project
     """
     # Access control for project
     project = await _get_project_check_owner(
         project_id=project_id, user_id=user_id, db=db
     )
```

### Comparing `fractal_server-1.3.0a9/fractal_server/app/api/v1/dataset.py` & `fractal_server-1.3.1/fractal_server/app/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/api/v1/job.py` & `fractal_server-1.3.1/fractal_server/app/api/v1/job.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Optional
 from zipfile import ZIP_DEFLATED
 from zipfile import ZipFile
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
-from fastapi import Response
 from fastapi import status
 from fastapi.responses import StreamingResponse
 from sqlmodel import select
 
 from ....config import get_settings
 from ....syringe import Inject
 from ...db import AsyncSession
@@ -162,13 +161,17 @@
         project_id=project_id,
         job_id=job_id,
         user_id=user.id,
         db=db,
     )
     job = output["job"]
 
+    # Note: we are **not** marking the job as failed (by setting its `status`
+    # attribute) here, since this will be done by the runner backend as soon as
+    # it detects the shutdown-trigerring file and performs the actual shutdown.
+
     # Write shutdown file
     shutdown_file = Path(job.working_dir) / SHUTDOWN_FILENAME
     with shutdown_file.open("w") as f:
         f.write(f"Trigger executor shutdown for {job.id=}, {project_id=}.")
 
-    return Response(status_code=status.HTTP_200_OK)
+    return job
```

### Comparing `fractal_server-1.3.0a9/fractal_server/app/api/v1/project.py` & `fractal_server-1.3.1/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/api/v1/task.py` & `fractal_server-1.3.1/fractal_server/app/api/v1/task_collection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-import asyncio
 import json
-from copy import deepcopy  # noqa
 from pathlib import Path
 from shutil import copy as shell_copy
 from shutil import rmtree as shell_rmtree
 from tempfile import TemporaryDirectory
-from typing import Optional
 
 from fastapi import APIRouter
 from fastapi import BackgroundTasks
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
 from pydantic.error_wrappers import ValidationError
-from sqlmodel import select
 
 from ....common.schemas import StateRead
 from ....common.schemas import TaskCollectPip
 from ....common.schemas import TaskCollectStatus
 from ....common.schemas import TaskCreate
-from ....common.schemas import TaskRead
-from ....common.schemas import TaskUpdate
 from ....config import get_settings
 from ....logger import close_logger
 from ....logger import set_logger
 from ....syringe import Inject
 from ....tasks.collection import _TaskCollectPip
 from ....tasks.collection import create_package_dir_pip
 from ....tasks.collection import create_package_environment_pip
@@ -37,18 +31,16 @@
 from ....tasks.collection import inspect_package
 from ...db import AsyncSession
 from ...db import DBSyncSession
 from ...db import get_db
 from ...db import get_sync_db
 from ...models import State
 from ...models import Task
-from ...models import WorkflowTask
 from ...security import current_active_user
 from ...security import User
-from ._aux_functions import _get_task_check_owner
 
 router = APIRouter()
 
 logger = set_logger(__name__)
 
 
 async def _background_collect_pip(
@@ -323,163 +315,7 @@
     # not set; if so, we collect the current logs
     if verbose and not data.log:
         data.log = get_collection_log(data.venv_path)
         state.data = data.sanitised_dict()
     close_logger(logger)
     await db.close()
     return state
-
-
-@router.get("/", response_model=list[TaskRead])
-async def get_list_task(
-    user: User = Depends(current_active_user),
-    db: AsyncSession = Depends(get_db),
-) -> list[TaskRead]:
-    """
-    Get list of available tasks
-    """
-    stm = select(Task)
-    res = await db.execute(stm)
-    task_list = res.scalars().unique().fetchall()
-    await asyncio.gather(*[db.refresh(t) for t in task_list])
-    await db.close()
-    return task_list
-
-
-@router.get("/{task_id}", response_model=TaskRead)
-async def get_task(
-    task_id: int,
-    user: User = Depends(current_active_user),
-    db: AsyncSession = Depends(get_db),
-) -> TaskRead:
-    """
-    Get info on a specific task
-    """
-    task = await db.get(Task, task_id)
-    await db.close()
-    if not task:
-        raise HTTPException(
-            status_code=status.HTTP_404_NOT_FOUND, detail="Task not found"
-        )
-    return task
-
-
-@router.patch("/{task_id}", response_model=TaskRead)
-async def patch_task(
-    task_id: int,
-    task_update: TaskUpdate,
-    user: User = Depends(current_active_user),
-    db: AsyncSession = Depends(get_db),
-) -> Optional[TaskRead]:
-    """
-    Edit a specific task (restricted to superusers and task owner)
-    """
-
-    if task_update.source:
-        raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail="patch_task endpoint cannot set `source`",
-        )
-
-    # Retrieve task from database
-    db_task = await _get_task_check_owner(task_id=task_id, user=user, db=db)
-
-    update = task_update.dict(exclude_unset=True)
-    for key, value in update.items():
-        if isinstance(value, str):
-            setattr(db_task, key, value)
-        elif isinstance(value, dict):
-            if key == "args_schema":
-                setattr(db_task, key, value)
-            else:
-                current_dict = deepcopy(getattr(db_task, key))
-                current_dict.update(value)
-                setattr(db_task, key, current_dict)
-        else:
-            raise HTTPException(
-                status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-                detail=f"Invalid {type(value)=} for {key=}",
-            )
-
-    await db.commit()
-    await db.refresh(db_task)
-    await db.close()
-    return db_task
-
-
-@router.post("/", response_model=TaskRead, status_code=status.HTTP_201_CREATED)
-async def create_task(
-    task: TaskCreate,
-    user: User = Depends(current_active_user),
-    db: AsyncSession = Depends(get_db),
-) -> Optional[TaskRead]:
-    """
-    Create a new task
-    """
-    # Set task.owner attribute
-    if user.username:
-        owner = user.username
-    elif user.slurm_user:
-        owner = user.slurm_user
-    else:
-        raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail=(
-                "Cannot add a new task because current user does not "
-                "have `username` or `slurm_user` attributes."
-            ),
-        )
-
-    # Prepend owner to task.source
-    task.source = f"{owner}:{task.source}"
-
-    # Verify that source is not already in use (note: this check is only useful
-    # to provide a user-friendly error message, but `task.source` uniqueness is
-    # already guaranteed by a constraint in the table definition).
-    stm = select(Task).where(Task.source == task.source)
-    res = await db.execute(stm)
-    if res.scalars().all():
-        raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail=f'Task source "{task.source}" already in use',
-        )
-
-    # Add task
-    db_task = Task(**task.dict(), owner=owner)
-    db.add(db_task)
-    await db.commit()
-    await db.refresh(db_task)
-    await db.close()
-    return db_task
-
-
-@router.delete("/{task_id}", status_code=204)
-async def delete_task(
-    task_id: int,
-    user: User = Depends(current_active_user),
-    db: AsyncSession = Depends(get_db),
-) -> Response:
-    """
-    Delete a task
-    """
-
-    db_task = await _get_task_check_owner(task_id=task_id, user=user, db=db)
-
-    # Check that the Task is not in relationship with some WorkflowTask
-    stm = select(WorkflowTask).filter(WorkflowTask.task_id == task_id)
-    res = await db.execute(stm)
-    workflowtask_list = res.scalars().all()
-    if workflowtask_list:
-        raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail=(
-                f"Cannot remove Task {task_id} because it is currently "
-                "imported in Workflows "
-                f"{[x.workflow_id for x in workflowtask_list]}. "
-                "If you want to remove this task, then you should first remove"
-                " the workflows.",
-            ),
-        )
-
-    await db.delete(db_task)
-    await db.commit()
-    return Response(status_code=status.HTTP_204_NO_CONTENT)
```

### Comparing `fractal_server-1.3.0a9/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.3.1/fractal_server/app/api/v1/workflow.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # Marco Franzon <marco.franzon@exact-lab.it>
 # Tommaso Comparin <tommaso.comparin@exact-lab.it>
 #
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
-from copy import deepcopy
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
@@ -28,23 +27,20 @@
 from ...models import Task
 from ...models import Workflow
 from ...models import WorkflowCreate
 from ...models import WorkflowExport
 from ...models import WorkflowImport
 from ...models import WorkflowRead
 from ...models import WorkflowTaskCreate
-from ...models import WorkflowTaskRead
-from ...models import WorkflowTaskUpdate
 from ...models import WorkflowUpdate
 from ...security import current_active_user
 from ...security import User
 from ._aux_functions import _check_workflow_exists
 from ._aux_functions import _get_project_check_owner
 from ._aux_functions import _get_workflow_check_owner
-from ._aux_functions import _get_workflow_task_check_owner
 
 
 router = APIRouter()
 
 
 @router.get(
     "/project/{project_id}/workflow/",
@@ -305,127 +301,7 @@
                 **new_wf_task.dict(),
                 task_id=task_id,
                 db=db,
             )
 
     await db.close()
     return db_workflow
-
-
-@router.post(
-    "/project/{project_id}/workflow/{workflow_id}/wftask/",
-    response_model=WorkflowTaskRead,
-    status_code=status.HTTP_201_CREATED,
-)
-async def create_workflowtask(
-    project_id: int,
-    workflow_id: int,
-    task_id: int,
-    new_task: WorkflowTaskCreate,
-    user: User = Depends(current_active_user),
-    db: AsyncSession = Depends(get_db),
-) -> Optional[WorkflowTaskRead]:
-    """
-    Add a WorkflowTask to a Workflow
-    """
-
-    workflow = await _get_workflow_check_owner(
-        project_id=project_id, workflow_id=workflow_id, user_id=user.id, db=db
-    )
-    async with db:
-        workflow_task = await workflow.insert_task(
-            **new_task.dict(),
-            task_id=task_id,
-            db=db,
-        )
-
-    await db.close()
-    return workflow_task
-
-
-@router.patch(
-    "/project/{project_id}/workflow/{workflow_id}/wftask/{workflow_task_id}",
-    response_model=WorkflowTaskRead,
-)
-async def update_workflowtask(
-    project_id: int,
-    workflow_id: int,
-    workflow_task_id: int,
-    workflow_task_update: WorkflowTaskUpdate,
-    user: User = Depends(current_active_user),
-    db: AsyncSession = Depends(get_db),
-) -> Optional[WorkflowTaskRead]:
-    """
-    Edit a WorkflowTask of a Workflow
-    """
-
-    db_workflow_task, db_workflow = await _get_workflow_task_check_owner(
-        project_id=project_id,
-        workflow_task_id=workflow_task_id,
-        workflow_id=workflow_id,
-        user_id=user.id,
-        db=db,
-    )
-
-    for key, value in workflow_task_update.dict(exclude_unset=True).items():
-        if key == "args":
-
-            # Get default arguments via a Task property method
-            default_args = deepcopy(
-                db_workflow_task.task.default_args_from_args_schema
-            )
-            # Override default_args with args value items
-            actual_args = default_args.copy()
-            if value is not None:
-                for k, v in value.items():
-                    actual_args[k] = v
-            if not actual_args:
-                actual_args = None
-            setattr(db_workflow_task, key, actual_args)
-        elif key == "meta":
-            current_meta = deepcopy(db_workflow_task.meta) or {}
-            current_meta.update(value)
-            setattr(db_workflow_task, key, current_meta)
-        else:
-            raise HTTPException(
-                status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-                detail=f"patch_workflow_task endpoint cannot set {key=}",
-            )
-
-    await db.commit()
-    await db.refresh(db_workflow_task)
-    await db.close()
-
-    return db_workflow_task
-
-
-@router.delete(
-    "/project/{project_id}/workflow/{workflow_id}/wftask/{workflow_task_id}",
-    status_code=status.HTTP_204_NO_CONTENT,
-)
-async def delete_workflowtask(
-    project_id: int,
-    workflow_id: int,
-    workflow_task_id: int,
-    user: User = Depends(current_active_user),
-    db: AsyncSession = Depends(get_db),
-) -> Response:
-    """
-    Delete a WorkflowTask of a Workflow
-    """
-
-    db_workflow_task, db_workflow = await _get_workflow_task_check_owner(
-        project_id=project_id,
-        workflow_task_id=workflow_task_id,
-        workflow_id=workflow_id,
-        user_id=user.id,
-        db=db,
-    )
-
-    await db.delete(db_workflow_task)
-    await db.commit()
-
-    await db.refresh(db_workflow)
-    db_workflow.task_list.reorder()
-    await db.commit()
-
-    return Response(status_code=status.HTTP_204_NO_CONTENT)
```

### Comparing `fractal_server-1.3.0a9/fractal_server/app/db/__init__.py` & `fractal_server-1.3.1/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/models/job.py` & `fractal_server-1.3.1/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/models/project.py` & `fractal_server-1.3.1/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/models/security.py` & `fractal_server-1.3.1/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/models/state.py` & `fractal_server-1.3.1/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/models/task.py` & `fractal_server-1.3.1/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/models/workflow.py` & `fractal_server-1.3.1/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/__init__.py` & `fractal_server-1.3.1/fractal_server/app/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_common.py` & `fractal_server-1.3.1/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.3.1/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.3.1/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.3.1/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.3.1/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.3.1/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.3.1/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.3.1/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.3.1/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.3.1/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.3.1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.3.1/fractal_server/app/runner/_slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.3.1/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/runner/common.py` & `fractal_server-1.3.1/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/app/security/__init__.py` & `fractal_server-1.3.1/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.3.1/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.3.1/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/README.md` & `fractal_server-1.3.1/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/__init__.py` & `fractal_server-1.3.1/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 20:08:58 2023 UTC, .py size: 1616 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5a07 9264 5006 0000  o.......Z..dP...
+00000000: 6f0d 0d0a 0000 0000 5237 9964 5006 0000  o.......R7.dP...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6402 6501 6602 6403 6404  d.l.Z.d.e.f.d.d.
 00000040: 8404 5a02 640b 6402 6501 6406 6503 6604  ..Z.d.d.e.d.e.f.
 00000050: 6407 6408 8405 5a04 6402 6501 6602 6409  d.d...Z.d.e.f.d.
 00000060: 640a 8404 5a05 6401 5300 290c e900 0000  d...Z.d.S.).....
 00000070: 004e da09 6174 7472 6962 7574 6563 0100  .N..attributec..
```

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 20:08:58 2023 UTC, .py size: 1117 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5a07 9264 5d04 0000  o.......Z..d]...
+00000000: 6f0d 0d0a 0000 0000 5237 9964 5d04 0000  o.......R7.d]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c06 6d07 5a07 0100 6407 5a08 4700  d.l.m.Z...d.Z.G.
 00000070: 6408 6409 8400 6409 6504 8303 5a09 4700  d.d...d.e...Z.G.
@@ -39,64 +39,64 @@
 00000260: 6865 6d61 732f 6170 706c 7977 6f72 6b66  hemas/applyworkf
 00000270: 6c6f 772e 7079 7208 0000 0010 0000 0073  low.pyr........s
 00000280: 0600 0000 0a00 0401 1007 7208 0000 0063  ..........r....c
 00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000002a0: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
 000002b0: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
 000002c0: 0464 0183 0183 015a 0564 0453 0029 0572  .d.....Z.d.S.).r
-000002d0: 0900 0000 720b 0000 0054 2901 5a0b 616c  ....r....T).Z.al
+000002d0: 0900 0000 720b 0000 0054 2901 da0b 616c  ....r....T)...al
 000002e0: 6c6f 775f 7265 7573 654e 2906 720c 0000  low_reuseN).r...
 000002f0: 0072 0d00 0000 720e 0000 0072 0500 0000  .r....r....r....
-00000300: 7207 0000 005a 0c5f 776f 726b 6572 5f69  r....Z._worker_i
+00000300: 7207 0000 00da 0c5f 776f 726b 6572 5f69  r......_worker_i
 00000310: 6e69 7472 1200 0000 7212 0000 0072 1200  nitr....r....r..
 00000320: 0000 7213 0000 0072 0900 0000 1b00 0000  ..r....r........
 00000330: 7308 0000 0008 000a 0306 0108 ff72 0900  s............r..
 00000340: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
 00000350: 0000 0003 0000 0040 0000 0073 8e00 0000  .......@...s....
 00000360: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
 00000370: 3c00 6503 6504 6402 3c00 6503 6504 6403  <.e.e.d.<.e.e.d.
 00000380: 3c00 6503 6504 6404 3c00 6503 6504 6405  <.e.e.d.<.e.e.d.
 00000390: 3c00 6505 6504 6406 3c00 6506 6505 1900  <.e.e.d.<.e.e...
 000003a0: 6504 6407 3c00 6507 6504 6408 3c00 6506  e.d.<.e.e.d.<.e.
 000003b0: 6507 1900 6504 6409 3c00 6506 6508 6507  e...e.d.<.e.e.e.
 000003c0: 1900 1900 6504 640a 3c00 6506 6507 1900  ....e.d.<.e.e...
 000003d0: 6504 640b 3c00 6506 6507 1900 6504 640c  e.d.<.e.e...e.d.
 000003e0: 3c00 640d 640e 8400 5a09 640f 5300 2910  <.d.d...Z.d.S.).
-000003f0: 720a 0000 00da 0269 645a 0a70 726f 6a65  r......idZ.proje
-00000400: 6374 5f69 645a 0b77 6f72 6b66 6c6f 775f  ct_idZ.workflow_
-00000410: 6964 5a10 696e 7075 745f 6461 7461 7365  idZ.input_datase
-00000420: 745f 6964 5a11 6f75 7470 7574 5f64 6174  t_idZ.output_dat
+000003f0: 720a 0000 00da 0269 64da 0a70 726f 6a65  r......id..proje
+00000400: 6374 5f69 64da 0b77 6f72 6b66 6c6f 775f  ct_id..workflow_
+00000410: 6964 da10 696e 7075 745f 6461 7461 7365  id..input_datase
+00000420: 745f 6964 da11 6f75 7470 7574 5f64 6174  t_id..output_dat
 00000430: 6173 6574 5f69 64da 0f73 7461 7274 5f74  aset_id..start_t
 00000440: 696d 6573 7461 6d70 da0d 656e 645f 7469  imestamp..end_ti
 00000450: 6d65 7374 616d 70da 0673 7461 7475 73da  mestamp..status.
-00000460: 036c 6f67 da07 6869 7374 6f72 795a 0b77  .log..historyZ.w
-00000470: 6f72 6b69 6e67 5f64 6972 5a10 776f 726b  orking_dirZ.work
+00000460: 036c 6f67 da07 6869 7374 6f72 79da 0b77  .log..history..w
+00000470: 6f72 6b69 6e67 5f64 6972 da10 776f 726b  orking_dir..work
 00000480: 696e 675f 6469 725f 7573 6572 6301 0000  ing_dir_userc...
 00000490: 0000 0000 0000 0000 0002 0000 0003 0000  ................
 000004a0: 0043 0000 0073 2800 0000 7c00 a000 a100  .C...s(...|.....
 000004b0: 7d01 7401 7c00 6a02 8301 7c01 6401 3c00  }.t.|.j...|.d.<.
 000004c0: 7401 7c00 6a03 8301 7c01 6402 3c00 7c01  t.|.j...|.d.<.|.
-000004d0: 5300 2903 4e72 1500 0000 7216 0000 0029  S.).Nr....r....)
-000004e0: 04da 0464 6963 7472 1000 0000 7215 0000  ...dictr....r...
-000004f0: 0072 1600 0000 2902 da04 7365 6c66 da01  .r....)...self..
+000004d0: 5300 2903 4e72 1b00 0000 721c 0000 0029  S.).Nr....r....)
+000004e0: 04da 0464 6963 7472 1000 0000 721b 0000  ...dictr....r...
+000004f0: 0072 1c00 0000 2902 da04 7365 6c66 da01  .r....)...self..
 00000500: 6472 1200 0000 7212 0000 0072 1300 0000  dr....r....r....
 00000510: da0e 7361 6e69 7469 7365 645f 6469 6374  ..sanitised_dict
 00000520: 3100 0000 7308 0000 0008 010e 010e 0104  1...s...........
 00000530: 017a 2041 7070 6c79 576f 726b 666c 6f77  .z ApplyWorkflow
 00000540: 5265 6164 2e73 616e 6974 6973 6564 5f64  Read.sanitised_d
 00000550: 6963 744e 290a 720c 0000 0072 0d00 0000  ictN).r....r....
 00000560: 720e 0000 00da 0369 6e74 7211 0000 0072  r......intr....r
 00000570: 0200 0000 7203 0000 0072 1000 0000 da04  ....r....r......
-00000580: 6c69 7374 721d 0000 0072 1200 0000 7212  listr....r....r.
+00000580: 6c69 7374 7225 0000 0072 1200 0000 7212  listr%...r....r.
 00000590: 0000 0072 1200 0000 7213 0000 0072 0a00  ...r....r....r..
 000005a0: 0000 2300 0000 731c 0000 000a 0008 0108  ..#...s.........
 000005b0: 0108 0108 0108 0108 010c 0108 010c 0110  ................
 000005c0: 010c 010c 010c 0272 0a00 0000 4e29 0c72  .......r....N).r
 000005d0: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
-000005e0: 005a 0870 7964 616e 7469 6372 0400 0000  .Z.pydanticr....
+000005e0: 00da 0870 7964 616e 7469 6372 0400 0000  ...pydanticr....
 000005f0: 7205 0000 00da 0b5f 7661 6c69 6461 746f  r......_validato
 00000600: 7273 7207 0000 00da 075f 5f61 6c6c 5f5f  rsr......__all__
 00000610: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
 00000620: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
 00000630: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
 00000640: 0073 1200 0000 0c00 0c01 0c02 0c01 0c02  .s..............
 00000650: 0402 1007 100b 1408                      ........
```

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 20:08:58 2023 UTC, .py size: 3479 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5a07 9264 970d 0000  o.......Z..d....
+00000000: 6f0d 0d0a 0000 0000 5237 9964 970d 0000  o.......R7.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c04 6d06 5a06 0100 6400 6406 6c04  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c04 6d08 5a08  m.Z...d.d.l.m.Z.
@@ -78,25 +78,25 @@
 000004d0: 206e 6565 645f 6770 753d 5472 7565 292c   need_gpu=True),
 000004e0: 0a20 2020 2020 2020 2020 2020 2065 7463  .            etc
 000004f0: 2e0a 2020 2020 2020 2020 6172 6773 5f73  ..        args_s
 00000500: 6368 656d 613a 0a20 2020 2020 2020 2020  chema:.         
 00000510: 2020 204a 534f 4e20 5363 6865 6d61 2066     JSON Schema f
 00000520: 6f72 2074 6173 6b20 6172 6775 6d65 6e74  or task argument
 00000530: 730a 2020 2020 da04 6e61 6d65 da0a 6578  s.    ..name..ex
-00000540: 6563 7574 6162 6c65 5a0a 696e 7075 745f  ecutableZ.input_
+00000540: 6563 7574 6162 6c65 da0a 696e 7075 745f  ecutable..input_
 00000550: 7479 7065 da0b 6f75 7470 7574 5f74 7970  type..output_typ
 00000560: 6529 01da 0f64 6566 6175 6c74 5f66 6163  e)...default_fac
 00000570: 746f 7279 da04 6d65 7461 da0b 6172 6773  tory..meta..args
 00000580: 5f73 6368 656d 614e 290b da08 5f5f 6e61  _schemaN)...__na
 00000590: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 000005a0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
 000005b0: 5f5f 646f 635f 5fda 0373 7472 da0f 5f5f  __doc__..str..__
 000005c0: 616e 6e6f 7461 7469 6f6e 735f 5f72 0600  annotations__r..
-000005d0: 0000 da04 6469 6374 7210 0000 0072 0300  ....dictr....r..
-000005e0: 0000 7202 0000 00a9 0072 1900 0000 7219  ..r......r....r.
+000005d0: 0000 da04 6469 6374 7211 0000 0072 0300  ....dictr....r..
+000005e0: 0000 7202 0000 00a9 0072 1a00 0000 721a  ..r......r....r.
 000005f0: 0000 00fa 4e2f 686f 6d65 2f74 6f6d 6d61  ....N/home/tomma
 00000600: 736f 2f46 7261 6374 616c 2f66 7261 6374  so/Fractal/fract
 00000610: 616c 2d73 6572 7665 722f 6672 6163 7461  al-server/fracta
 00000620: 6c5f 7365 7276 6572 2f63 6f6d 6d6f 6e2f  l_server/common/
 00000630: 7363 6865 6d61 732f 6d61 6e69 6665 7374  schemas/manifest
 00000640: 2e70 7972 0b00 0000 0e00 0000 7310 0000  .pyr........s...
 00000650: 000a 0004 0108 1b08 0108 0108 011e 0118  ................
@@ -174,83 +174,83 @@
 00000ad0: 656c 206f 6620 686f 7720 6061 7267 735f  el of how `args_
 00000ae0: 7363 6865 6d61 6073 2077 6572 6520 6765  schema`s were ge
 00000af0: 6e65 7261 7465 6420 2865 2e67 2e20 6070  nerated (e.g. `p
 00000b00: 7964 616e 7469 635f 7631 6029 2e0a 2020  ydantic_v1`)..  
 00000b10: 2020 da10 6d61 6e69 6665 7374 5f76 6572    ..manifest_ver
 00000b20: 7369 6f6e da09 7461 736b 5f6c 6973 7446  sion..task_listF
 00000b30: da10 6861 735f 6172 6773 5f73 6368 656d  ..has_args_schem
-00000b40: 6173 5a13 6172 6773 5f73 6368 656d 615f  asZ.args_schema_
+00000b40: 6173 da13 6172 6773 5f73 6368 656d 615f  as..args_schema_
 00000b50: 7665 7273 696f 6e63 0200 0000 0000 0000  versionc........
 00000b60: 0000 0000 0500 0000 0900 0000 4300 0000  ............C...
 00000b70: 734c 0000 007c 0164 0119 007d 027c 0164  sL...|.d...}.|.d
 00000b80: 0219 007d 037c 0272 247c 0344 005d 177d  ...}.|.r$|.D.].}
 00000b90: 047c 046a 0064 0075 0072 2374 0164 037c  .|.j.d.u.r#t.d.|
 00000ba0: 029b 0064 047c 046a 029b 0064 057c 046a  ...d.|.j...d.|.j
 00000bb0: 009b 0064 069d 0783 0182 0171 0c7c 0153  ...d.......q.|.S
-00000bc0: 0029 074e 7220 0000 0072 1f00 0000 7a11  .).Nr ...r....z.
+00000bc0: 0029 074e 7221 0000 0072 2000 0000 7a11  .).Nr!...r ...z.
 00000bd0: 6861 735f 6172 6773 5f73 6368 656d 6173  has_args_schemas
 00000be0: 3d7a 0b20 6275 7420 7461 736b 2022 7a12  =z. but task "z.
 00000bf0: 2220 6861 7320 6172 6773 5f73 6368 656d  " has args_schem
-00000c00: 613d da01 2e29 0372 1100 0000 da0a 5661  a=...).r......Va
+00000c00: 613d da01 2e29 0372 1200 0000 da0a 5661  a=...).r......Va
 00000c10: 6c75 6545 7272 6f72 720c 0000 0029 05da  lueErrorr....)..
-00000c20: 0363 6c73 da06 7661 6c75 6573 7220 0000  .cls..valuesr ..
-00000c30: 0072 1f00 0000 da04 7461 736b 7219 0000  .r......taskr...
-00000c40: 0072 1900 0000 721a 0000 00da 1f5f 6368  .r....r......_ch
+00000c20: 0363 6c73 da06 7661 6c75 6573 7221 0000  .cls..valuesr!..
+00000c30: 0072 2000 0000 da04 7461 736b 721a 0000  .r .....taskr...
+00000c40: 0072 1a00 0000 721b 0000 00da 1f5f 6368  .r....r......_ch
 00000c50: 6563 6b5f 6172 6773 5f73 6368 656d 6173  eck_args_schemas
 00000c60: 5f61 7265 5f70 7265 7365 6e74 5400 0000  _are_presentT...
 00000c70: 731c 0000 0008 0208 0104 0108 010a 0102  s...............
 00000c80: 0108 0104 0104 ff04 0106 ff04 ff02 ff04  ................
 00000c90: 057a 2d5f 4d61 6e69 6665 7374 4261 7365  .z-_ManifestBase
 00000ca0: 2e5f 6368 6563 6b5f 6172 6773 5f73 6368  ._check_args_sch
 00000cb0: 656d 6173 5f61 7265 5f70 7265 7365 6e74  emas_are_present
-00000cc0: 4e29 0d72 1200 0000 7213 0000 0072 1400  N).r....r....r..
-00000cd0: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000ce0: 00da 046c 6973 7472 1b00 0000 7220 0000  ...listr....r ..
+00000cc0: 4e29 0d72 1300 0000 7214 0000 0072 1500  N).r....r....r..
+00000cd0: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00000ce0: 00da 046c 6973 7472 1c00 0000 7221 0000  ...listr....r!..
 00000cf0: 00da 0462 6f6f 6c72 0300 0000 7207 0000  ...boolr....r...
-00000d00: 0072 2600 0000 7219 0000 0072 1900 0000  .r&...r....r....
-00000d10: 7219 0000 0072 1a00 0000 721d 0000 0035  r....r....r....5
+00000d00: 0072 2800 0000 721a 0000 0072 1a00 0000  .r(...r....r....
+00000d10: 721a 0000 0072 1b00 0000 721e 0000 0035  r....r....r....5
 00000d20: 0000 0073 1000 0000 0a00 0401 0819 0c01  ...s............
-00000d30: 0c01 0c01 0402 0e01 721d 0000 0063 0000  ........r....c..
+00000d30: 0c01 0c01 0402 0e01 721e 0000 0063 0000  ........r....c..
 00000d40: 0000 0000 0000 0000 0000 0000 0000 0100  ................
 00000d50: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
 00000d60: 005a 0264 0153 0029 0272 0900 0000 4e29  .Z.d.S.).r....N)
-00000d70: 0372 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000d80: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00000d90: 1a00 0000 7209 0000 0062 0000 0073 0400  ....r....b...s..
+00000d70: 0372 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000d80: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00000d90: 1b00 0000 7209 0000 0062 0000 0073 0400  ....r....b...s..
 00000da0: 0000 0800 0401 7209 0000 0063 0000 0000  ......r....c....
 00000db0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
 00000dc0: 4000 0000 732e 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
 00000dd0: 0255 0064 015a 0365 0465 0519 0065 0664  .U.d.Z.e.e...e.d
 00000de0: 023c 0065 0764 0383 0164 0464 0584 0083  .<.e.d...d.d....
 00000df0: 015a 0864 0653 0029 0772 0a00 0000 7a23  .Z.d.S.).r....z#
 00000e00: 0a20 2020 204d 616e 6966 6573 7420 7363  .    Manifest sc
 00000e10: 6865 6d61 2076 6572 7369 6f6e 2031 0a20  hema version 1. 
-00000e20: 2020 2072 1f00 0000 721e 0000 0063 0200     r....r....c..
+00000e20: 2020 2072 2000 0000 721f 0000 0063 0200     r ...r....c..
 00000e30: 0000 0000 0000 0000 0000 0200 0000 0400  ................
 00000e40: 0000 4300 0000 731c 0000 007c 0164 016b  ..C...s....|.d.k
 00000e50: 0372 0c74 0064 027c 019b 0064 039d 0383  .r.t.d.|...d....
 00000e60: 0182 0164 0053 0029 044e da01 317a 1e57  ...d.S.).N..1z.W
 00000e70: 726f 6e67 206d 616e 6966 6573 7420 7665  rong manifest ve
 00000e80: 7273 696f 6e20 2867 6976 656e 20fa 0129  rsion (given ..)
-00000e90: 2901 7222 0000 0029 0272 2300 0000 da05  ).r"...).r#.....
-00000ea0: 7661 6c75 6572 1900 0000 7219 0000 0072  valuer....r....r
-00000eb0: 1a00 0000 da12 6d61 6e69 6665 7374 5f76  ......manifest_v
+00000e90: 2901 7224 0000 0029 0272 2500 0000 da05  ).r$...).r%.....
+00000ea0: 7661 6c75 6572 1a00 0000 721a 0000 0072  valuer....r....r
+00000eb0: 1b00 0000 da12 6d61 6e69 6665 7374 5f76  ......manifest_v
 00000ec0: 6572 7369 6f6e 5f31 6d00 0000 7306 0000  ersion_1m...s...
 00000ed0: 0008 0210 0104 ff7a 1d4d 616e 6966 6573  .......z.Manifes
 00000ee0: 7456 312e 6d61 6e69 6665 7374 5f76 6572  tV1.manifest_ver
-00000ef0: 7369 6f6e 5f31 4e29 0972 1200 0000 7213  sion_1N).r....r.
-00000f00: 0000 0072 1400 0000 7215 0000 0072 2700  ...r....r....r'.
-00000f10: 0000 7209 0000 0072 1700 0000 7208 0000  ..r....r....r...
-00000f20: 0072 2c00 0000 7219 0000 0072 1900 0000  .r,...r....r....
-00000f30: 7219 0000 0072 1a00 0000 720a 0000 0066  r....r....r....f
+00000ef0: 7369 6f6e 5f31 4e29 0972 1300 0000 7214  sion_1N).r....r.
+00000f00: 0000 0072 1500 0000 7216 0000 0072 2900  ...r....r....r).
+00000f10: 0000 7209 0000 0072 1800 0000 7208 0000  ..r....r....r...
+00000f20: 0072 2e00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00000f30: 721a 0000 0072 1b00 0000 720a 0000 0066  r....r....r....f
 00000f40: 0000 0073 0a00 0000 0a00 0401 0c04 0602  ...s............
 00000f50: 0e01 720a 0000 004e 290f da06 7479 7069  ..r....N)...typi
 00000f60: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
 00000f70: 00da 0870 7964 616e 7469 6372 0500 0000  ...pydanticr....
 00000f80: 7206 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
-00000f90: 075f 5f61 6c6c 5f5f 720b 0000 0072 1b00  .__all__r....r..
-00000fa0: 0000 721d 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00000fb0: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
-00000fc0: 721a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000f90: 075f 5f61 6c6c 5f5f 720b 0000 0072 1c00  .__all__r....r..
+00000fa0: 0000 721e 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00000fb0: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00000fc0: 721b 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
 00000fd0: 0000 0073 1a00 0000 0c00 0c01 0c01 0c02  ...s............
 00000fe0: 0c01 0c01 0c01 0403 1003 0c24 1003 102d  ...........$...-
 00000ff0: 1404                                     ..
```

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 20:08:58 2023 UTC, .py size: 2483 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5a07 9264 b309 0000  o.......Z..d....
+00000000: 6f0d 0d0a 0000 0000 5237 9964 b309 0000  o.......R7.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c03 6d06 5a06 0100 6406 6407 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6406 6408 6c07 6d09 5a09  m.Z...d.d.l.m.Z.
@@ -68,15 +68,15 @@
 00000430: 721e 0000 004e 7220 0000 0072 1b00 0000  r....Nr ...r....
 00000440: 721b 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
 00000450: 1200 0000 2900 0000 7222 0000 0072 1200  ....)...r"...r..
 00000460: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
 00000470: 0000 0003 0000 0040 0000 0073 1e00 0000  .......@...s....
 00000480: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
 00000490: 3c00 6503 6504 6402 3c00 6403 5300 2904  <.e.e.d.<.d.S.).
-000004a0: 7211 0000 00da 0269 645a 0a64 6174 6173  r......idZ.datas
+000004a0: 7211 0000 00da 0269 64da 0a64 6174 6173  r......id..datas
 000004b0: 6574 5f69 644e 2905 7215 0000 0072 1600  et_idN).r....r..
 000004c0: 0000 7217 0000 00da 0369 6e74 721a 0000  ..r......intr...
 000004d0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
 000004e0: 721c 0000 0072 1100 0000 2e00 0000 7306  r....r........s.
 000004f0: 0000 000a 0008 010c 0172 1100 0000 6300  .........r....c.
 00000500: 0000 0000 0000 0000 0000 0000 0000 0003  ................
 00000510: 0000 0040 0000 0073 4c00 0000 6500 5a01  ...@...sL...e.Z.
@@ -94,129 +94,129 @@
 000005d0: 2020 206d 6574 613a 2054 4244 0a20 2020     meta: TBD.   
 000005e0: 2020 2020 2072 6561 645f 6f6e 6c79 3a20       read_only: 
 000005f0: 5442 440a 2020 2020 da04 6e61 6d65 da04  TBD.    ..name..
 00000600: 7479 7065 2901 da07 6465 6661 756c 74da  type)...default.
 00000610: 046d 6574 6146 da09 7265 6164 5f6f 6e6c  .metaF..read_onl
 00000620: 794e 290d 7215 0000 0072 1600 0000 7217  yN).r....r....r.
 00000630: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
-00000640: 0000 7203 0000 0072 0500 0000 7229 0000  ..r....r....r)..
-00000650: 00da 0464 6963 7472 0200 0000 722a 0000  ...dictr....r*..
+00000640: 0000 7203 0000 0072 0500 0000 722a 0000  ..r....r....r*..
+00000650: 00da 0464 6963 7472 0200 0000 722b 0000  ...dictr....r+..
 00000660: 00da 0462 6f6f 6c72 1b00 0000 721b 0000  ...boolr....r...
-00000670: 0072 1b00 0000 721c 0000 0072 2500 0000  .r....r....r%...
+00000670: 0072 1b00 0000 721c 0000 0072 2600 0000  .r....r....r&...
 00000680: 3600 0000 730c 0000 000a 0004 0108 0a0c  6...s...........
-00000690: 011a 0110 0172 2500 0000 6300 0000 0000  .....r%...c.....
+00000690: 011a 0110 0172 2600 0000 6300 0000 0000  .....r&...c.....
 000006a0: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
 000006b0: 0000 0073 6600 0000 6500 5a01 6400 5a02  ...sf...e.Z.d.Z.
 000006c0: 5500 6503 6504 1900 6505 6401 3c00 6402  U.e.e...e.d.<.d.
 000006d0: 5a06 6503 6507 6504 6508 6602 1900 1900  Z.e.e.e.e.f.....
 000006e0: 6505 6403 3c00 6503 6509 1900 6505 6404  e.d.<.e.e...e.d.
 000006f0: 3c00 650a 6401 6405 6406 8d02 650b 6401  <.e.d.d.d...e.d.
 00000700: 8301 8301 5a0c 650a 6407 6405 6406 8d02  ....Z.e.d.d.d...
 00000710: 650b 6407 8301 8301 5a0d 6402 5300 2908  e.d.....Z.d.S.).
-00000720: 720d 0000 0072 2600 0000 4e72 2900 0000  r....r&...Nr)...
-00000730: 722a 0000 0054 721e 0000 0072 2700 0000  r*...Tr....r'...
+00000720: 720d 0000 0072 2700 0000 4e72 2a00 0000  r....r'...Nr*...
+00000730: 722b 0000 0054 721e 0000 0072 2800 0000  r+...Tr....r(...
 00000740: 290e 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
 00000750: 0072 0300 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000760: 7229 0000 0072 2b00 0000 7202 0000 0072  r)...r+...r....r
-00000770: 2c00 0000 7206 0000 0072 0900 0000 da05  ,...r....r......
+00000760: 722a 0000 0072 2c00 0000 7202 0000 0072  r*...r,...r....r
+00000770: 2d00 0000 7206 0000 0072 0900 0000 da05  -...r....r......
 00000780: 5f6e 616d 65da 055f 7479 7065 721b 0000  _name.._typer...
 00000790: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
 000007a0: 720d 0000 0047 0000 0073 0c00 0000 0a00  r....G...s......
 000007b0: 0c01 1801 0c01 1403 1801 720d 0000 0063  ..........r....c
 000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007d0: 0400 0000 4000 0000 7334 0000 0065 005a  ....@...s4...e.Z
 000007e0: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
 000007f0: 0464 0183 0183 015a 0565 0364 0464 0264  .d.....Z.e.d.d.d
 00000800: 038d 0265 0464 0483 0183 015a 0664 0553  ...e.d.....Z.d.S
-00000810: 0029 0672 0e00 0000 7226 0000 0054 721e  .).r....r&...Tr.
-00000820: 0000 0072 2700 0000 4e29 0772 1500 0000  ...r'...N).r....
+00000810: 0029 0672 0e00 0000 7227 0000 0054 721e  .).r....r'...Tr.
+00000820: 0000 0072 2800 0000 4e29 0772 1500 0000  ...r(...N).r....
 00000830: 7216 0000 0072 1700 0000 7206 0000 0072  r....r....r....r
-00000840: 0900 0000 722d 0000 0072 2e00 0000 721b  ....r-...r....r.
+00000840: 0900 0000 722e 0000 0072 2f00 0000 721b  ....r....r/...r.
 00000850: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
 00000860: 0000 720e 0000 0051 0000 0073 0600 0000  ..r....Q...s....
 00000870: 0800 1402 1801 720e 0000 0063 0000 0000  ......r....c....
 00000880: 0000 0000 0000 0000 0000 0000 0300 0000  ................
 00000890: 4000 0000 7332 0000 0065 005a 0164 005a  @...s2...e.Z.d.Z
 000008a0: 0255 0065 0365 0464 013c 0065 0565 0619  .U.e.e.d.<.e.e..
 000008b0: 0065 0464 023c 0065 0365 0464 033c 0065  .e.d.<.e.e.d.<.e
 000008c0: 0765 0464 043c 0064 0553 0029 0672 0f00  .e.d.<.d.S.).r..
-000008d0: 0000 7223 0000 005a 0d72 6573 6f75 7263  ..r#...Z.resourc
+000008d0: 0000 7223 0000 00da 0d72 6573 6f75 7263  ..r#.....resourc
 000008e0: 655f 6c69 7374 da0a 7072 6f6a 6563 745f  e_list..project_
-000008f0: 6964 722a 0000 004e 2908 7215 0000 0072  idr*...N).r....r
-00000900: 1600 0000 7217 0000 0072 2400 0000 721a  ....r....r$...r.
-00000910: 0000 00da 046c 6973 7472 1100 0000 722c  .....listr....r,
+000008f0: 6964 722b 0000 004e 2908 7215 0000 0072  idr+...N).r....r
+00000900: 1600 0000 7217 0000 0072 2500 0000 721a  ....r....r%...r.
+00000910: 0000 00da 046c 6973 7472 1100 0000 722d  .....listr....r-
 00000920: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
 00000930: 0000 721c 0000 0072 0f00 0000 5700 0000  ..r....r....W...
 00000940: 730a 0000 000a 0008 010c 0108 010c 0172  s..............r
 00000950: 0f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
 00000960: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
 00000970: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
 00000980: 6504 6505 6402 3c00 6403 5a06 6507 6505  e.e.d.<.d.Z.e.e.
 00000990: 6404 3c00 6405 5300 2906 da0c 5f50 726f  d.<.d.S.)..._Pro
 000009a0: 6a65 6374 4261 7365 7a5a 0a20 2020 2042  jectBasezZ.    B
 000009b0: 6173 6520 636c 6173 7320 666f 7220 5072  ase class for Pr
 000009c0: 6f6a 6563 740a 0a20 2020 2041 7474 7269  oject..    Attri
 000009d0: 6275 7465 733a 0a20 2020 2020 2020 206e  butes:.        n
 000009e0: 616d 653a 2054 4244 0a20 2020 2020 2020  ame: TBD.       
 000009f0: 2072 6561 645f 6f6e 6c79 3a20 5442 440a   read_only: TBD.
-00000a00: 2020 2020 7226 0000 0046 722a 0000 004e      r&...Fr*...N
+00000a00: 2020 2020 7227 0000 0046 722b 0000 004e      r'...Fr+...N
 00000a10: 2908 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
 00000a20: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000a30: 722a 0000 0072 2c00 0000 721b 0000 0072  r*...r,...r....r
-00000a40: 1b00 0000 721b 0000 0072 1c00 0000 7231  ....r....r....r1
+00000a30: 722b 0000 0072 2d00 0000 721b 0000 0072  r+...r-...r....r
+00000a40: 1b00 0000 721b 0000 0072 1c00 0000 7233  ....r....r....r3
 00000a50: 0000 0061 0000 0073 0800 0000 0a00 0401  ...a...s........
-00000a60: 0808 1001 7231 0000 0063 0000 0000 0000  ....r1...c......
+00000a60: 0808 1001 7233 0000 0063 0000 0000 0000  ....r3...c......
 00000a70: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
 00000a80: 0000 7346 0000 0065 005a 0164 005a 0255  ..sF...e.Z.d.Z.U
 00000a90: 0064 015a 0365 0465 0519 0065 0664 023c  .d.Z.e.e...e.d.<
 00000aa0: 0065 0764 0364 0464 058d 0265 0864 0383  .e.d.d.d...e.d..
 00000ab0: 0183 015a 0965 0764 0264 0464 058d 0265  ...Z.e.d.d.d...e
 00000ac0: 0864 0283 0183 015a 0a64 0653 0029 0772  .d.....Z.d.S.).r
-00000ad0: 0a00 0000 7228 0000 00da 1464 6566 6175  ....r(.....defau
+00000ad0: 0a00 0000 7229 0000 00da 1464 6566 6175  ....r).....defau
 00000ae0: 6c74 5f64 6174 6173 6574 5f6e 616d 6572  lt_dataset_namer
-00000af0: 2600 0000 5472 1e00 0000 4e29 0b72 1500  &...Tr....N).r..
-00000b00: 0000 7216 0000 0072 1700 0000 7232 0000  ..r....r....r2..
+00000af0: 2700 0000 5472 1e00 0000 4e29 0b72 1500  '...Tr....N).r..
+00000b00: 0000 7216 0000 0072 1700 0000 7234 0000  ..r....r....r4..
 00000b10: 0072 0300 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000b20: 7206 0000 0072 0900 0000 722d 0000 005a  r....r....r-...Z
+00000b20: 7206 0000 0072 0900 0000 722e 0000 00da  r....r....r.....
 00000b30: 155f 6465 6661 756c 745f 6461 7461 7365  ._default_datase
 00000b40: 745f 6e61 6d65 721b 0000 0072 1b00 0000  t_namer....r....
 00000b50: 721b 0000 0072 1c00 0000 720a 0000 006e  r....r....r....n
 00000b60: 0000 0073 1000 0000 0a00 1001 1403 0201  ...s............
 00000b70: 0401 04ff 0602 08fe 720a 0000 0063 0000  ........r....c..
 00000b80: 0000 0000 0000 0000 0000 0000 0000 0300  ................
 00000b90: 0000 4000 0000 7326 0000 0065 005a 0164  ..@...s&...e.Z.d
 00000ba0: 005a 0255 0065 0365 0464 013c 0067 005a  .Z.U.e.e.d.<.g.Z
 00000bb0: 0565 0665 0719 0065 0464 023c 0064 0353  .e.e...e.d.<.d.S
 00000bc0: 0029 0472 0b00 0000 7223 0000 00da 0c64  .).r....r#.....d
 00000bd0: 6174 6173 6574 5f6c 6973 744e 2908 7215  ataset_listN).r.
-00000be0: 0000 0072 1600 0000 7217 0000 0072 2400  ...r....r....r$.
-00000bf0: 0000 721a 0000 0072 3300 0000 7230 0000  ..r....r3...r0..
+00000be0: 0000 0072 1600 0000 7217 0000 0072 2500  ...r....r....r%.
+00000bf0: 0000 721a 0000 0072 3600 0000 7232 0000  ..r....r6...r2..
 00000c00: 0072 0f00 0000 721b 0000 0072 1b00 0000  .r....r....r....
 00000c10: 721b 0000 0072 1c00 0000 720b 0000 0078  r....r....r....x
 00000c20: 0000 0073 0600 0000 0a00 0801 1401 720b  ...s..........r.
 00000c30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 00000c40: 0000 0000 0400 0000 4000 0000 733a 0000  ........@...s:..
 00000c50: 0065 005a 0164 005a 0255 0065 0365 0419  .e.Z.d.Z.U.e.e..
 00000c60: 0065 0564 013c 0065 0365 0619 0065 0564  .e.d.<.e.e...e.d
 00000c70: 023c 0065 0764 0164 0364 048d 0265 0864  .<.e.d.d.d...e.d
 00000c80: 0183 0183 015a 0964 0553 0029 0672 0c00  .....Z.d.S.).r..
-00000c90: 0000 7226 0000 0072 2a00 0000 5472 1e00  ..r&...r*...Tr..
+00000c90: 0000 7227 0000 0072 2b00 0000 5472 1e00  ..r'...r+...Tr..
 00000ca0: 0000 4e29 0a72 1500 0000 7216 0000 0072  ..N).r....r....r
 00000cb0: 1700 0000 7203 0000 0072 1900 0000 721a  ....r....r....r.
-00000cc0: 0000 0072 2c00 0000 7206 0000 0072 0900  ...r,...r....r..
-00000cd0: 0000 722d 0000 0072 1b00 0000 721b 0000  ..r-...r....r...
+00000cc0: 0000 0072 2d00 0000 7206 0000 0072 0900  ...r-...r....r..
+00000cd0: 0000 722e 0000 0072 1b00 0000 721b 0000  ..r....r....r...
 00000ce0: 0072 1b00 0000 721c 0000 0072 0c00 0000  .r....r....r....
 00000cf0: 7d00 0000 7308 0000 000a 000c 010c 0118  }...s...........
 00000d00: 0372 0c00 0000 4e29 17da 0674 7970 696e  .r....N)...typin
 00000d10: 6772 0200 0000 7203 0000 00da 0870 7964  gr....r......pyd
 00000d20: 616e 7469 6372 0400 0000 7205 0000 0072  anticr....r....r
 00000d30: 0600 0000 da0b 5f76 616c 6964 6174 6f72  ......_validator
 00000d40: 7372 0800 0000 7209 0000 00da 075f 5f61  sr....r......__a
 00000d50: 6c6c 5f5f 7213 0000 0072 1000 0000 7212  ll__r....r....r.
-00000d60: 0000 0072 1100 0000 7225 0000 0072 0d00  ...r....r%...r..
-00000d70: 0000 720e 0000 0072 0f00 0000 7231 0000  ..r....r....r1..
+00000d60: 0000 0072 1100 0000 7226 0000 0072 0d00  ...r....r&...r..
+00000d70: 0000 720e 0000 0072 0f00 0000 7233 0000  ..r....r....r3..
 00000d80: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
 00000d90: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
 00000da0: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
 00000db0: 0000 7328 0000 000c 000c 010c 020c 010c  ..s(............
 00000dc0: 010c 020c 0104 0310 1010 0810 0510 0510  ................
 00000dd0: 0810 1110 0a10 0610 0a10 0d10 0a14 05    ...............
```

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 20:08:58 2023 UTC, .py size: 673 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5a07 9264 a102 0000  o.......Z..d....
+00000000: 6f0d 0d0a 0000 0000 5237 9964 a102 0000  o.......R7.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c01 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
 00000060: 5a06 4700 6406 6407 8400 6407 6505 8303  Z.G.d.d...d.e...
 00000070: 5a07 4700 6408 6409 8400 6409 6507 8303  Z.G.d.d...d.e...
```

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 20:08:58 2023 UTC, .py size: 2578 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5a07 9264 120a 0000  o.......Z..d....
+00000000: 6f0d 0d0a 0000 0000 5237 9964 120a 0000  o.......R7.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c03 6d06 5a06 0100 6406 6407 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6408 5a09 4700 6409 640a  m.Z...d.Z.G.d.d.
@@ -147,15 +147,15 @@
 00000920: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
 00000930: 0000 5472 1000 0000 4e29 1272 1200 0000  ..Tr....N).r....
 00000940: 7213 0000 0072 1400 0000 7216 0000 0072  r....r....r....r
 00000950: 1700 0000 7205 0000 0072 1f00 0000 7203  ....r....r....r.
 00000960: 0000 0072 2300 0000 7202 0000 0072 0600  ...r#...r....r..
 00000970: 0000 7208 0000 0072 2400 0000 7225 0000  ..r....r$...r%..
 00000980: 0072 2600 0000 7227 0000 0072 2800 0000  .r&...r'...r(...
-00000990: 5a14 5f61 7267 735f 7363 6865 6d61 5f76  Z._args_schema_v
+00000990: da14 5f61 7267 735f 7363 6865 6d61 5f76  .._args_schema_v
 000009a0: 6572 7369 6f6e 7219 0000 0072 1900 0000  ersionr....r....
 000009b0: 7219 0000 0072 1a00 0000 7209 0000 004e  r....r....r....N
 000009c0: 0000 0073 2a00 0000 0a00 0801 0801 0801  ...s*...........
 000009d0: 0801 1e01 0c01 1401 0c01 1403 0a01 0601  ................
 000009e0: 04ff 0a03 0601 04ff 1403 1401 0a01 0601  ................
 000009f0: 08ff 7209 0000 004e 2910 da06 7479 7069  ..r....N)...typi
 00000a00: 6e67 7202 0000 0072 0300 0000 da08 7079  ngr....r......py
```

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc` & `fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 20:08:58 2023 UTC, .py size: 2935 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5a07 9264 770b 0000  o.......Z..dw...
+00000000: 6f0d 0d0a 0000 0000 5237 9964 770b 0000  o.......R7.dw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c05 6d07 5a07 0100 6400 6406 6c05  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6407 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -131,17 +131,17 @@
 00000820: 6f6c 6c65 6374 5069 702e 7061 636b 6167  ollectPip.packag
 00000830: 655f 7661 6c69 6461 746f 7229 1272 0e00  e_validator).r..
 00000840: 0000 720f 0000 0072 1000 0000 da07 5f5f  ..r....r......__
 00000850: 646f 635f 5fda 0373 7472 da0f 5f5f 616e  doc__..str..__an
 00000860: 6e6f 7461 7469 6f6e 735f 5f72 1400 0000  notations__r....
 00000870: 7204 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
 00000880: 1700 0000 da04 6469 6374 7207 0000 0072  ......dictr....r
-00000890: 0900 0000 5a10 5f70 6163 6b61 6765 5f76  ....Z._package_v
-000008a0: 6572 7369 6f6e 5a0f 5f70 6163 6b61 6765  ersionZ._package
-000008b0: 5f65 7874 7261 735a 0f5f 7079 7468 6f6e  _extrasZ._python
+00000890: 0900 0000 da10 5f70 6163 6b61 6765 5f76  ......_package_v
+000008a0: 6572 7369 6f6e da0f 5f70 6163 6b61 6765  ersion.._package
+000008b0: 5f65 7874 7261 73da 0f5f 7079 7468 6f6e  _extras.._python
 000008c0: 5f76 6572 7369 6f6e 721f 0000 0072 1100  _versionr....r..
 000008d0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
 000008e0: 0072 0b00 0000 1600 0000 7324 0000 000a  .r........s$....
 000008f0: 0004 0108 1a10 0110 0110 0118 010a 0206  ................
 00000900: 0104 ff0a 0306 0104 ff0a 0306 0104 ff06  ................
 00000910: 040e 0172 0b00 0000 6300 0000 0000 0000  ...r....c.......
 00000920: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
@@ -159,41 +159,41 @@
 000009e0: 7475 733a 2054 4244 0a20 2020 2020 2020  tus: TBD.       
 000009f0: 2070 6163 6b61 6765 3a20 5442 440a 2020   package: TBD.  
 00000a00: 2020 2020 2020 7665 6e76 5f70 6174 683a        venv_path:
 00000a10: 2054 4244 0a20 2020 2020 2020 2074 6173   TBD.        tas
 00000a20: 6b5f 6c69 7374 3a20 5442 440a 2020 2020  k_list: TBD.    
 00000a30: 2020 2020 6c6f 673a 2054 4244 0a20 2020      log: TBD.   
 00000a40: 2020 2020 2069 6e66 6f3a 2054 4244 0a20       info: TBD. 
-00000a50: 2020 2029 05da 0770 656e 6469 6e67 5a0a     )...pendingZ.
-00000a60: 696e 7374 616c 6c69 6e67 5a0a 636f 6c6c  installingZ.coll
+00000a50: 2020 2029 05da 0770 656e 6469 6e67 da0a     )...pending..
+00000a60: 696e 7374 616c 6c69 6e67 da0a 636f 6c6c  installing..coll
 00000a70: 6563 7469 6e67 da04 6661 696c da02 4f4b  ecting..fail..OK
 00000a80: da06 7374 6174 7573 7213 0000 00da 0976  ..statusr......v
 00000a90: 656e 765f 7061 7468 2901 da07 6465 6661  env_path)...defa
 00000aa0: 756c 74da 0974 6173 6b5f 6c69 7374 da03  ult..task_list..
 00000ab0: 6c6f 67da 0469 6e66 6f63 0100 0000 0000  log..infoc......
 00000ac0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
 00000ad0: 0000 731a 0000 007c 00a0 00a1 007d 0174  ..s....|.....}.t
 00000ae0: 017c 006a 0283 017c 0164 013c 007c 0153  .|.j...|.d.<.|.S
 00000af0: 0029 027a 510a 2020 2020 2020 2020 5265  .).zQ.        Re
 00000b00: 7475 726e 2060 7365 6c66 2e64 6963 7428  turn `self.dict(
 00000b10: 2960 2061 6674 6572 2063 6173 7469 6e67  )` after casting
 00000b20: 2060 7365 6c66 2e76 656e 765f 7061 7468   `self.venv_path
 00000b30: 6020 746f 2061 2073 7472 696e 670a 2020  ` to a string.  
-00000b40: 2020 2020 2020 7228 0000 0029 0372 2300        r(...).r#.
-00000b50: 0000 7221 0000 0072 2800 0000 2902 da04  ..r!...r(...)...
+00000b40: 2020 2020 2020 722d 0000 0029 0372 2300        r-...).r#.
+00000b50: 0000 7221 0000 0072 2d00 0000 2902 da04  ..r!...r-...)...
 00000b60: 7365 6c66 da01 6472 1100 0000 7211 0000  self..dr....r...
 00000b70: 0072 1200 0000 da0e 7361 6e69 7469 7365  .r......sanitise
 00000b80: 645f 6469 6374 6400 0000 7306 0000 0008  d_dictd...s.....
 00000b90: 040e 0104 017a 2054 6173 6b43 6f6c 6c65  .....z TaskColle
 00000ba0: 6374 5374 6174 7573 2e73 616e 6974 6973  ctStatus.sanitis
 00000bb0: 6564 5f64 6963 744e 290e 720e 0000 0072  ed_dictN).r....r
 00000bc0: 0f00 0000 7210 0000 0072 2000 0000 7203  ....r....r ...r.
 00000bd0: 0000 0072 2200 0000 7221 0000 0072 0200  ...r"...r!...r..
-00000be0: 0000 7206 0000 0072 2a00 0000 7204 0000  ..r....r*...r...
-00000bf0: 00da 046c 6973 7472 0a00 0000 722f 0000  ...listr....r/..
+00000be0: 0000 7206 0000 0072 2f00 0000 7204 0000  ..r....r/...r...
+00000bf0: 00da 046c 6973 7472 0a00 0000 7234 0000  ...listr....r4..
 00000c00: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
 00000c10: 7212 0000 0072 0c00 0000 5000 0000 7312  r....r....P...s.
 00000c20: 0000 000a 0004 010c 0c08 0108 011a 010c  ................
 00000c30: 010c 010c 0272 0c00 0000 4e29 11da 0770  .....r....N)...p
 00000c40: 6174 686c 6962 7202 0000 00da 0674 7970  athlibr......typ
 00000c50: 696e 6772 0300 0000 7204 0000 00da 0870  ingr....r......p
 00000c60: 7964 616e 7469 6372 0500 0000 7206 0000  ydanticr....r...
```

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 20:08:58 2023 UTC, .py size: 1216 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5a07 9264 c004 0000  o.......Z..d....
+00000000: 6f0d 0d0a 0000 0000 5237 9964 c004 0000  o.......R7.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6404 6405 6c06 6d07 5a07 0100 6404  ..d.d.l.m.Z...d.
 00000060: 6406 6c06 6d08 5a08 0100 6407 5a09 4700  d.l.m.Z...d.Z.G.
 00000070: 6408 6409 8400 6409 6503 6a0a 650b 1900  d.d...d.e.j.e...
@@ -44,33 +44,33 @@
 000002b0: 6404 6405 8d02 6507 6403 8301 8301 5a09  d.d...e.d.....Z.
 000002c0: 6506 6402 6404 6405 8d02 650a 6402 8301  e.d.d.d...e.d...
 000002d0: 8301 5a0b 6406 5300 2907 7209 0000 0072  ..Z.d.S.).r....r
 000002e0: 0b00 0000 720c 0000 0072 0d00 0000 54a9  ....r....r....T.
 000002f0: 01da 0b61 6c6c 6f77 5f72 6575 7365 4ea9  ...allow_reuseN.
 00000300: 0c72 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
 00000310: 7202 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00000320: 0400 0000 7207 0000 005a 0b5f 736c 7572  ....r....Z._slur
-00000330: 6d5f 7573 6572 5a09 5f75 7365 726e 616d  m_userZ._usernam
-00000340: 6572 0600 0000 5a0a 5f63 6163 6865 5f64  er....Z._cache_d
+00000320: 0400 0000 7207 0000 00da 0b5f 736c 7572  ....r......_slur
+00000330: 6d5f 7573 6572 da09 5f75 7365 726e 616d  m_user.._usernam
+00000340: 6572 0600 0000 da0a 5f63 6163 6865 5f64  er......_cache_d
 00000350: 6972 7213 0000 0072 1300 0000 7213 0000  irr....r....r...
 00000360: 0072 1400 0000 7209 0000 0017 0000 00f3  .r....r.........
 00000370: 1600 0000 0a00 0c01 0c01 0c01 0a03 0601  ................
 00000380: 04ff 1403 0a01 0601 08ff 7209 0000 0063  ..........r....c
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0400 0000 4000 0000 7215 0000 0029 0772  ....@...r....).r
 000003b0: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
 000003c0: 0000 0054 7216 0000 004e 7218 0000 0072  ...Tr....Nr....r
 000003d0: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-000003e0: 0000 0072 0a00 0000 2600 0000 7219 0000  ...r....&...r...
+000003e0: 0000 0072 0a00 0000 2600 0000 721c 0000  ...r....&...r...
 000003f0: 0072 0a00 0000 4e29 11da 0674 7970 696e  .r....N)...typin
-00000400: 6772 0200 0000 5a0d 6661 7374 6170 695f  gr....Z.fastapi_
+00000400: 6772 0200 0000 da0d 6661 7374 6170 695f  gr......fastapi_
 00000410: 7573 6572 7372 0300 0000 da08 7079 6461  usersr......pyda
 00000420: 6e74 6963 7204 0000 00da 0b5f 7661 6c69  nticr......_vali
 00000430: 6461 746f 7273 7206 0000 0072 0700 0000  datorsr....r....
-00000440: da07 5f5f 616c 6c5f 5f5a 0842 6173 6555  ..__all__Z.BaseU
-00000450: 7365 72da 0369 6e74 7208 0000 005a 0e42  ser..intr....Z.B
+00000440: da07 5f5f 616c 6c5f 5fda 0842 6173 6555  ..__all__..BaseU
+00000450: 7365 72da 0369 6e74 7208 0000 00da 0e42  ser..intr......B
 00000460: 6173 6555 7365 7255 7064 6174 6572 0900  aseUserUpdater..
-00000470: 0000 5a0e 4261 7365 5573 6572 4372 6561  ..Z.BaseUserCrea
+00000470: 0000 da0e 4261 7365 5573 6572 4372 6561  ....BaseUserCrea
 00000480: 7465 720a 0000 0072 1300 0000 7213 0000  ter....r....r...
 00000490: 0072 1300 0000 7214 0000 00da 083c 6d6f  .r....r......<mo
 000004a0: 6475 6c65 3e01 0000 0073 1200 0000 0c00  dule>....s......
 000004b0: 0c02 0c01 0c02 0c01 0403 1607 1206 160f  ................
```

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.3.1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun 20 20:08:58 2023 UTC, .py size: 2457 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5a07 9264 9909 0000  o.......Z..d....
+00000000: 6f0d 0d0a 0000 0000 5237 9964 9909 0000  o.......R7.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3401 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c06 6d07 5a07 0100 6405 6407 6c06  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6405 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -105,15 +105,15 @@
 00000680: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
 00000690: 0000 0300 0000 4000 0000 731c 0000 0065  ......@...s....e
 000006a0: 005a 0164 005a 0265 0364 0183 0164 0264  .Z.d.Z.e.d...d.d
 000006b0: 0384 0083 015a 0464 0453 0029 0572 1500  .....Z.d.S.).r..
 000006c0: 0000 7217 0000 0063 0200 0000 0000 0000  ..r....c........
 000006d0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
 000006e0: 7314 0000 0064 017c 0176 0072 0874 0064  s....d.|.v.r.t.d
-000006f0: 0283 0182 017c 0153 0029 034e 5a15 7061  .....|.S.).NZ.pa
+000006f0: 0283 0182 017c 0153 0029 034e da15 7061  .....|.S.).N..pa
 00000700: 7261 6c6c 656c 697a 6174 696f 6e5f 6c65  rallelization_le
 00000710: 7665 6c7a 3b4f 7665 7272 6964 696e 6720  velz;Overriding 
 00000720: 7461 736b 2070 6172 616c 6c65 6c69 7a61  task paralleliza
 00000730: 7469 6f6e 206c 6576 656c 2063 7572 7265  tion level curre
 00000740: 6e74 6c79 206e 6f74 2061 6c6c 6f77 6564  ntly not allowed
 00000750: 2901 da0a 5661 6c75 6545 7272 6f72 2902  )...ValueError).
 00000760: da03 636c 73da 016d 721f 0000 0072 1f00  ..cls..mr....r..
@@ -121,25 +121,25 @@
 00000780: 6f5f 7061 7261 6c6c 656c 6973 6174 696f  o_parallelisatio
 00000790: 6e5f 6c65 7665 6c3a 0000 0073 0a00 0000  n_level:...s....
 000007a0: 0802 0201 0201 04ff 0403 7a31 576f 726b  ..........z1Work
 000007b0: 666c 6f77 5461 736b 5570 6461 7465 2e63  flowTaskUpdate.c
 000007c0: 6865 636b 5f6e 6f5f 7061 7261 6c6c 656c  heck_no_parallel
 000007d0: 6973 6174 696f 6e5f 6c65 7665 6c4e 2905  isation_levelN).
 000007e0: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-000007f0: 0500 0000 7230 0000 0072 1f00 0000 721f  ....r0...r....r.
+000007f0: 0500 0000 7231 0000 0072 1f00 0000 721f  ....r1...r....r.
 00000800: 0000 0072 1f00 0000 7220 0000 0072 1500  ...r....r ...r..
 00000810: 0000 3800 0000 7306 0000 0008 0006 020e  ..8...s.........
 00000820: 0172 1500 0000 6300 0000 0000 0000 0000  .r....c.........
 00000830: 0000 0000 0000 0003 0000 0040 0000 0072  ...........@...r
 00000840: 2b00 0000 2903 da0d 5f57 6f72 6b66 6c6f  +...)..._Workflo
 00000850: 7742 6173 65da 046e 616d 654e 2905 7219  wBase..nameN).r.
 00000860: 0000 0072 1a00 0000 721b 0000 0072 1d00  ...r....r....r..
 00000870: 0000 721e 0000 0072 1f00 0000 721f 0000  ..r....r....r...
-00000880: 0072 1f00 0000 7220 0000 0072 3100 0000  .r....r ...r1...
-00000890: 4300 0000 722c 0000 0072 3100 0000 6300  C...r,...r1...c.
+00000880: 0072 1f00 0000 7220 0000 0072 3200 0000  .r....r ...r2...
+00000890: 4300 0000 722c 0000 0072 3200 0000 6300  C...r,...r2...c.
 000008a0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
 000008b0: 0000 0040 0000 0073 2a00 0000 6500 5a01  ...@...s*...e.Z.
 000008c0: 6400 5a02 5500 6503 6504 6401 3c00 6503  d.Z.U.e.e.d.<.e.
 000008d0: 6504 6402 3c00 6505 6506 1900 6504 6403  e.d.<.e.e...e.d.
 000008e0: 3c00 6404 5300 2905 720d 0000 0072 2700  <.d.S.).r....r'.
 000008f0: 0000 da0a 7072 6f6a 6563 745f 6964 da09  ....project_id..
 00000900: 7461 736b 5f6c 6973 744e 2907 7219 0000  task_listN).r...
@@ -148,28 +148,28 @@
 00000930: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
 00000940: 2000 0000 720d 0000 0047 0000 0073 0800   ...r....G...s..
 00000950: 0000 0a00 0801 0801 1001 720d 0000 0063  ..........r....c
 00000960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000970: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
 00000980: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
 00000990: 0464 0183 0183 015a 0564 0453 0029 0572  .d.....Z.d.S.).r
-000009a0: 0c00 0000 7232 0000 0054 7222 0000 004e  ....r2...Tr"...N
+000009a0: 0c00 0000 7233 0000 0054 7222 0000 004e  ....r3...Tr"...N
 000009b0: 2906 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
 000009c0: 0072 0500 0000 7208 0000 00da 055f 6e61  .r....r......_na
 000009d0: 6d65 721f 0000 0072 1f00 0000 721f 0000  mer....r....r...
 000009e0: 0072 2000 0000 720c 0000 004d 0000 0073  .r ...r....M...s
 000009f0: 0400 0000 0800 1802 720c 0000 0063 0000  ........r....c..
 00000a00: 0000 0000 0000 0000 0000 0000 0000 0400  ................
 00000a10: 0000 4000 0000 734e 0000 0065 005a 0164  ..@...sN...e.Z.d
 00000a20: 005a 0255 0065 0365 0419 0065 0564 013c  .Z.U.e.e...e.d.<
 00000a30: 0065 0365 0665 0719 0019 0065 0564 023c  .e.e.e.....e.d.<
 00000a40: 0065 0864 0164 0364 048d 0265 0964 0183  .e.d.d.d...e.d..
 00000a50: 0183 015a 0a65 0864 0283 0164 0564 0684  ...Z.e.d...d.d..
 00000a60: 0083 015a 0b64 0753 0029 0872 0e00 0000  ...Z.d.S.).r....
-00000a70: 7232 0000 005a 1a72 656f 7264 6572 6564  r2...Z.reordered
+00000a70: 7233 0000 00da 1a72 656f 7264 6572 6564  r3.....reordered
 00000a80: 5f77 6f72 6b66 6c6f 7774 6173 6b5f 6964  _workflowtask_id
 00000a90: 7354 7222 0000 0063 0200 0000 0000 0000  sTr"...c........
 00000aa0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
 00000ab0: 733a 0000 0074 0064 0164 0284 007c 0144  s:...t.d.d...|.D
 00000ac0: 0083 0183 0172 0d74 0164 0383 0182 0174  .....r.t.d.....t
 00000ad0: 027c 0183 0174 0274 037c 0183 0183 016b  .|...t.t.|.....k
 00000ae0: 0372 1b74 0164 0483 0182 017c 0153 0029  .r.t.d.....|.S.)
@@ -186,59 +186,59 @@
 00000b90: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
 00000ba0: 723e 7a2d 4e65 6761 7469 7665 2060 6964  r>z-Negative `id
 00000bb0: 6020 696e 2060 7265 6f72 6465 7265 645f  ` in `reordered_
 00000bc0: 776f 726b 666c 6f77 7461 736b 5f69 6473  workflowtask_ids
 00000bd0: 607a 2c60 7265 6f72 6465 7265 645f 776f  `z,`reordered_wo
 00000be0: 726b 666c 6f77 7461 736b 5f69 6473 6020  rkflowtask_ids` 
 00000bf0: 6861 7320 7265 7065 7469 7469 6f6e 7329  has repetitions)
-00000c00: 04da 0361 6e79 722d 0000 00da 036c 656e  ...anyr-.....len
-00000c10: da03 7365 7429 0272 2e00 0000 da05 7661  ..set).r......va
+00000c00: 04da 0361 6e79 722e 0000 00da 036c 656e  ...anyr......len
+00000c10: da03 7365 7429 0272 2f00 0000 da05 7661  ..set).r/.....va
 00000c20: 6c75 6572 1f00 0000 721f 0000 0072 2000  luer....r....r .
 00000c30: 0000 da19 6368 6563 6b5f 706f 7369 7469  ....check_positi
 00000c40: 7665 5f61 6e64 5f75 6e69 7175 6559 0000  ve_and_uniqueY..
 00000c50: 0073 0a00 0000 1202 0801 1401 0801 0401  .s..............
 00000c60: 7a28 576f 726b 666c 6f77 5570 6461 7465  z(WorkflowUpdate
 00000c70: 2e63 6865 636b 5f70 6f73 6974 6976 655f  .check_positive_
 00000c80: 616e 645f 756e 6971 7565 4e29 0c72 1900  and_uniqueN).r..
 00000c90: 0000 721a 0000 0072 1b00 0000 7203 0000  ..r....r....r...
-00000ca0: 0072 1d00 0000 721e 0000 0072 3500 0000  .r....r....r5...
+00000ca0: 0072 1d00 0000 721e 0000 0072 3600 0000  .r....r....r6...
 00000cb0: 7225 0000 0072 0500 0000 7208 0000 0072  r%...r....r....r
-00000cc0: 3600 0000 723e 0000 0072 1f00 0000 721f  6...r>...r....r.
+00000cc0: 3700 0000 7240 0000 0072 1f00 0000 721f  7...r@...r....r.
 00000cd0: 0000 0072 1f00 0000 7220 0000 0072 0e00  ...r....r ...r..
 00000ce0: 0000 5200 0000 730c 0000 000a 000c 0110  ..R...s.........
 00000cf0: 0114 0306 020e 0172 0e00 0000 6300 0000  .......r....c...
 00000d00: 0000 0000 0000 0000 0000 0000 0004 0000  ................
 00000d10: 0040 0000 0073 2e00 0000 6500 5a01 6400  .@...s....e.Z.d.
 00000d20: 5a02 5500 6503 6504 1900 6505 6401 3c00  Z.U.e.e...e.d.<.
 00000d30: 6506 6402 6403 6404 8d02 6507 6402 8301  e.d.d.d...e.d...
 00000d40: 8301 5a08 6405 5300 2906 720f 0000 0072  ..Z.d.S.).r....r
-00000d50: 3400 0000 7232 0000 0054 7222 0000 004e  4...r2...Tr"...N
+00000d50: 3500 0000 7233 0000 0054 7222 0000 004e  5...r3...Tr"...N
 00000d60: 2909 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
-00000d70: 0072 3500 0000 7212 0000 0072 1e00 0000  .r5...r....r....
-00000d80: 7205 0000 0072 0800 0000 7236 0000 0072  r....r....r6...r
+00000d70: 0072 3600 0000 7212 0000 0072 1e00 0000  .r6...r....r....
+00000d80: 7205 0000 0072 0800 0000 7237 0000 0072  r....r....r7...r
 00000d90: 1f00 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
 00000da0: 0000 0072 0f00 0000 6200 0000 7306 0000  ...r....b...s...
 00000db0: 000a 000c 0118 0372 0f00 0000 6300 0000  .......r....c...
 00000dc0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
 00000dd0: 0040 0000 0073 1a00 0000 6500 5a01 6400  .@...s....e.Z.d.
 00000de0: 5a02 5500 6503 6504 1900 6505 6401 3c00  Z.U.e.e...e.d.<.
-00000df0: 6402 5300 2903 7210 0000 0072 3400 0000  d.S.).r....r4...
+00000df0: 6402 5300 2903 7210 0000 0072 3500 0000  d.S.).r....r5...
 00000e00: 4e29 0672 1900 0000 721a 0000 0072 1b00  N).r....r....r..
-00000e10: 0000 7235 0000 0072 1300 0000 721e 0000  ..r5...r....r...
+00000e10: 0000 7236 0000 0072 1300 0000 721e 0000  ..r6...r....r...
 00000e20: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
 00000e30: 7220 0000 0072 1000 0000 6900 0000 7304  r ...r....i...s.
 00000e40: 0000 000a 0010 0172 1000 0000 4e29 1ada  .......r....N)..
 00000e50: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
 00000e60: 00da 0870 7964 616e 7469 6372 0400 0000  ...pydanticr....
 00000e70: 7205 0000 00da 0b5f 7661 6c69 6461 746f  r......_validato
 00000e80: 7273 7207 0000 0072 0800 0000 722a 0000  rsr....r....r*..
 00000e90: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
 00000ea0: da07 5f5f 616c 6c5f 5f72 1600 0000 7211  ..__all__r....r.
 00000eb0: 0000 0072 1400 0000 7212 0000 0072 1300  ...r....r....r..
-00000ec0: 0000 7215 0000 0072 3100 0000 720d 0000  ..r....r1...r...
+00000ec0: 0000 7215 0000 0072 3200 0000 720d 0000  ..r....r2...r...
 00000ed0: 0072 0c00 0000 720e 0000 0072 0f00 0000  .r....r....r....
 00000ee0: 7210 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
 00000ef0: 1f00 0000 7220 0000 00da 083c 6d6f 6475  ....r .....<modu
 00000f00: 6c65 3e01 0000 0073 2c00 0000 0c00 0c01  le>....s,.......
 00000f10: 0c02 0c01 0c02 0c01 0c01 0c01 0c01 0403  ................
 00000f20: 100e 1006 1006 1008 1004 1004 100b 1004  ................
 00000f30: 1006 1005 1010 1407                      ........
```

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/_validators.py` & `fractal_server-1.3.1/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.3.1/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/manifest.py` & `fractal_server-1.3.1/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/project.py` & `fractal_server-1.3.1/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/state.py` & `fractal_server-1.3.1/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/task.py` & `fractal_server-1.3.1/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/task_collection.py` & `fractal_server-1.3.1/fractal_server/common/schemas/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/user.py` & `fractal_server-1.3.1/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/schemas/workflow.py` & `fractal_server-1.3.1/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.3.1/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.3.1/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/tests/test_project.py` & `fractal_server-1.3.1/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/tests/test_state.py` & `fractal_server-1.3.1/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/tests/test_task.py` & `fractal_server-1.3.1/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/tests/test_task_collection.py` & `fractal_server-1.3.1/fractal_server/common/tests/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/tests/test_user.py` & `fractal_server-1.3.1/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.3.1/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/config.py` & `fractal_server-1.3.1/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/logger.py` & `fractal_server-1.3.1/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/main.py` & `fractal_server-1.3.1/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/migrations/env.py` & `fractal_server-1.3.1/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/migrations/script.py.mako` & `fractal_server-1.3.1/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-1.3.1/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-1.3.1/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-1.3.1/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/syringe.py` & `fractal_server-1.3.1/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/tasks/collection.py` & `fractal_server-1.3.1/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/fractal_server/utils.py` & `fractal_server-1.3.1/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a9/pyproject.toml` & `fractal_server-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.3.0a9"
+version = "1.3.1"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -73,15 +73,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.3.0a9"
+current_version = "1.3.1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.3.0a9/PKG-INFO` & `fractal_server-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.3.0a9
+Version: 1.3.1
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

