# Comparing `tmp/akerbp.mlops-3.2.0a5.tar.gz` & `tmp/akerbp.mlops-3.2.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-t43vayh4/akerbp.mlops-3.2.0a5.tar", last modified: Wed Jun 14 12:47:08 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-iop7e8h2/akerbp.mlops-3.2.0a6.tar", last modified: Tue Jun 27 08:09:57 2023, max compression
```

## Comparing `akerbp.mlops-3.2.0a5.tar` & `akerbp.mlops-3.2.0a6.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.082091 akerbp.mlops-3.2.0a5/
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    48989 2023-06-14 12:47:08.082091 akerbp.mlops-3.2.0a5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35467 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.070091 akerbp.mlops-3.2.0a5/bitbucket_pipeline_helpers/
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/build.sh
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/increment_package_version.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/install.sh
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/mlops_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.070091 akerbp.mlops-3.2.0a5/model_artifact/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/model_artifact/README.md
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/model_artifact/mlpet_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.070091 akerbp.mlops-3.2.0a5/model_code/
--rw-rw-rw-   0 root         (0) root         (0)     9932 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/model_code/model.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/model_code/requirements.model
--rw-rw-rw-   0 root         (0) root         (0)     5427 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/model_code/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-14 12:47:08.082091 akerbp.mlops-3.2.0a5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.066091 akerbp.mlops-3.2.0a5/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.066091 akerbp.mlops-3.2.0a5/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.074091 akerbp.mlops-3.2.0a5/src/akerbp/mlops/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-14 12:47:07.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.074091 akerbp.mlops-3.2.0a5/src/akerbp/mlops/cdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/cdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/cdf/download_function_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/cdf/handler.py
--rw-rw-rw-   0 root         (0) root         (0)    38715 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/cdf/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.074091 akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16504 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/logger_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/mappings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.078091 akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     5828 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/deploy_prediction_service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/deploy_training_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21442 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/platforms.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.078091 akerbp.mlops-3.2.0a5/src/akerbp/mlops/model_manager/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/model_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22658 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/model_manager/model_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.078091 akerbp.mlops-3.2.0a5/src/akerbp/mlops/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8607 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/services/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/services/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/src/akerbp/mlops/services/training.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.074091 akerbp.mlops-3.2.0a5/src/akerbp.mlops.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    48989 2023-06-14 12:47:07.000000 akerbp.mlops-3.2.0a5/src/akerbp.mlops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-06-14 12:47:08.000000 akerbp.mlops-3.2.0a5/src/akerbp.mlops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-14 12:47:07.000000 akerbp.mlops-3.2.0a5/src/akerbp.mlops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-14 12:47:07.000000 akerbp.mlops-3.2.0a5/src/akerbp.mlops.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-14 12:47:07.000000 akerbp.mlops-3.2.0a5/src/akerbp.mlops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-06-14 12:47:07.000000 akerbp.mlops-3.2.0a5/src/akerbp.mlops.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.078091 akerbp.mlops-3.2.0a5/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_data_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_install_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_metadata_validation.py
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-14 12:47:08.082091 akerbp.mlops-3.2.0a5/test/test_settings/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_settings/installing_reqs_in_venv.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_settings/multiple_models_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_settings/multiple_models_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_settings/single_model_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_settings/single_model_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_settings/single_model_missing_petrel_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_settings/single_model_no_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_settings/single_model_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3562 2023-06-14 12:46:35.000000 akerbp.mlops-3.2.0a5/test/test_version_increment.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.154502 akerbp.mlops-3.2.0a6/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-06-27 08:09:57.154502 akerbp.mlops-3.2.0a6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35467 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4229 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.146502 akerbp.mlops-3.2.0a6/bitbucket_pipeline_helpers/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/increment_package_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/install.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/mlops_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.146502 akerbp.mlops-3.2.0a6/model_artifact/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/model_artifact/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/model_artifact/mlpet_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.146502 akerbp.mlops-3.2.0a6/model_code/
+-rw-rw-rw-   0 root         (0) root         (0)     9932 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/model_code/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/model_code/requirements.model
+-rw-rw-rw-   0 root         (0) root         (0)     5427 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/model_code/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-27 08:09:57.154502 akerbp.mlops-3.2.0a6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.142502 akerbp.mlops-3.2.0a6/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.142502 akerbp.mlops-3.2.0a6/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.146502 akerbp.mlops-3.2.0a6/src/akerbp/mlops/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-27 08:09:57.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.146502 akerbp.mlops-3.2.0a6/src/akerbp/mlops/cdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/cdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/cdf/download_function_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/cdf/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    38715 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/cdf/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.150502 akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16504 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/logger_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/mappings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.150502 akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5828 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/deploy_prediction_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/deploy_training_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    21442 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/platforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.150502 akerbp.mlops-3.2.0a6/src/akerbp/mlops/model_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/model_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22658 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/model_manager/model_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.150502 akerbp.mlops-3.2.0a6/src/akerbp/mlops/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8607 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/services/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/services/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/src/akerbp/mlops/services/training.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.146502 akerbp.mlops-3.2.0a6/src/akerbp.mlops.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-06-27 08:09:57.000000 akerbp.mlops-3.2.0a6/src/akerbp.mlops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-06-27 08:09:57.000000 akerbp.mlops-3.2.0a6/src/akerbp.mlops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-27 08:09:57.000000 akerbp.mlops-3.2.0a6/src/akerbp.mlops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-27 08:09:57.000000 akerbp.mlops-3.2.0a6/src/akerbp.mlops.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-27 08:09:57.000000 akerbp.mlops-3.2.0a6/src/akerbp.mlops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-06-27 08:09:57.000000 akerbp.mlops-3.2.0a6/src/akerbp.mlops.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.150502 akerbp.mlops-3.2.0a6/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_data_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_install_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_metadata_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-27 08:09:57.154502 akerbp.mlops-3.2.0a6/test/test_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_settings/installing_reqs_in_venv.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_settings/multiple_models_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_settings/multiple_models_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_settings/single_model_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_settings/single_model_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_settings/single_model_missing_petrel_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_settings/single_model_no_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_settings/single_model_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3562 2023-06-27 08:09:36.000000 akerbp.mlops-3.2.0a6/test/test_version_increment.py
```

### Comparing `akerbp.mlops-3.2.0a5/.flake8` & `akerbp.mlops-3.2.0a6/.flake8`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/.pre-commit-config.yaml` & `akerbp.mlops-3.2.0a6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/LICENSE` & `akerbp.mlops-3.2.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/PKG-INFO` & `akerbp.mlops-3.2.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.2.0a5
+Version: 3.2.0a6
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.2.0a5/README.md` & `akerbp.mlops-3.2.0a6/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.0a6/bitbucket-pipelines.yml`

 * *Files 14% similar despite different names*

```diff
@@ -83,38 +83,23 @@
           - pip install pydantic
           - pip install types-PyYAML types-requests
           - mypy
     - step: &security-scan-secrets
         name: Security Scan for Secrets
         script:
           - pipe: atlassian/git-secrets-scan:0.5.1
-    - step: &snyk-scan
-        name: Snyk Scan for Vulnerabilities
-        caches:
-          - pip
-        script:
-          - pip install .[dev,cdf,gc]
-          - pip uninstall akerbp.mlops -y
-          - pip freeze > requirements.txt
-          - curl https://static.snyk.io/cli/latest/snyk-linux -o snyk
-          - chmod +x ./snyk
-          - mv ./snyk /usr/local/bin
-          - snyk auth $SNYK_TOKEN
-          - snyk test --fail-on=all --print-deps
 
 pipelines:
   pull-requests:
     "**": # Run for PRs on all branches
       - parallel:
           - step: *unit-testing
           - step: *flake8-linting
           - step: *mypy-type-checking
           - step: *security-scan-secrets
-          - step: *snyk-scan
-      # TODO: if not restricted by cognite, figure out how to install wheels from private repo and run integration tests before deploying pre-release to PyPI
       - step: *deploy-test-package
       - step: *run-tests-without-deploying
       - step: *deploy-dev-prediction-service
       - step:
           name: Promote Artifacts to Test and Prod
           script:
             - *set-environment-dev
```

### Comparing `akerbp.mlops-3.2.0a5/build.sh` & `akerbp.mlops-3.2.0a6/build.sh`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/increment_package_version.py` & `akerbp.mlops-3.2.0a6/increment_package_version.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/mlops_settings.yaml` & `akerbp.mlops-3.2.0a6/mlops_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/model_code/model.py` & `akerbp.mlops-3.2.0a6/model_code/model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/model_code/test_model.py` & `akerbp.mlops-3.2.0a6/model_code/test_model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/pyproject.toml` & `akerbp.mlops-3.2.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/cdf/handler.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/cdf/handler.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/cdf/helpers.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/cdf/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/config.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/exceptions.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/helpers.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/logger.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/logger.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/logger_config.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/logger_config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/core/mappings.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/core/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/bitbucket-pipelines.yml`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,14 @@
   pull-requests:
     "**":
       - step:
           name: Deploy to Dev
           deployment: dev-prediction
           script:
             # We want to deploy to dev for every commit to a feature branch PR into develop
-            - if [["$BITBUCKET_BRANCH" == "develop" || "$BITBUCKET_BRANCH" == "master" || "$BITBUCKET_BRANCH" == "main" ]]; then exit 0; fi
             - *install-mlops
             - deploy_prediction_service
 
   branches:
     development: &dev-branch
       - step: &deploy-to-test
           name: Deploy to Test
```

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/deploy.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/helpers.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/platforms.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/platforms.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/deployment/setup.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/deployment/setup.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/model_manager/model_manager.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/model_manager/model_manager.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/services/prediction.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/services/prediction.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/services/test_service.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/services/test_service.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp/mlops/services/training.py` & `akerbp.mlops-3.2.0a6/src/akerbp/mlops/services/training.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp.mlops.egg-info/PKG-INFO` & `akerbp.mlops-3.2.0a6/src/akerbp.mlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.2.0a5
+Version: 3.2.0a6
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.2.0a5/src/akerbp.mlops.egg-info/SOURCES.txt` & `akerbp.mlops-3.2.0a6/src/akerbp.mlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_data_validation.py` & `akerbp.mlops-3.2.0a6/test/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_install_requirements.py` & `akerbp.mlops-3.2.0a6/test/test_install_requirements.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_metadata_validation.py` & `akerbp.mlops-3.2.0a6/test/test_metadata_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_settings/installing_reqs_in_venv.yaml` & `akerbp.mlops-3.2.0a6/test/test_settings/installing_reqs_in_venv.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_settings/multiple_models_all_required_fields.yaml` & `akerbp.mlops-3.2.0a6/test/test_settings/multiple_models_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_settings/multiple_models_missing_field.yaml` & `akerbp.mlops-3.2.0a6/test/test_settings/multiple_models_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_settings/single_model_all_required_fields.yaml` & `akerbp.mlops-3.2.0a6/test/test_settings/single_model_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_settings/single_model_missing_field.yaml` & `akerbp.mlops-3.2.0a6/test/test_settings/single_model_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_settings/single_model_missing_petrel_field.yaml` & `akerbp.mlops-3.2.0a6/test/test_settings/single_model_missing_petrel_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_settings/single_model_no_required_input.yaml` & `akerbp.mlops-3.2.0a6/test/test_settings/single_model_no_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_settings/single_model_required_input.yaml` & `akerbp.mlops-3.2.0a6/test/test_settings/single_model_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.0a5/test/test_version_increment.py` & `akerbp.mlops-3.2.0a6/test/test_version_increment.py`

 * *Files identical despite different names*

