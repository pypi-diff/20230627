# Comparing `tmp/orchestrator_core-1.1.1rc2.tar.gz` & `tmp/orchestrator_core-1.1.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator_core-1.1.1rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orchestrator_core-1.1.1rc3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator_core-1.1.1rc2.tar` & `orchestrator_core-1.1.1rc3.tar`

### file list

```diff
@@ -1,386 +1,386 @@
--rw-r--r--   0        0        0      341 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.coveragerc
--rw-r--r--   0        0        0     2620 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      371 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      550 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1163 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2113 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1809 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.gitignore
--rw-r--r--   0        0        0     2099 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/.stignore
--rw-r--r--   0        0        0    29970 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/CHANGELOG.md
--rw-r--r--   0        0        0      333 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/Dockerfile
--rw-r--r--   0        0        0    11409 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/LICENSE
--rw-r--r--   0        0        0      150 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/NOTICE
--rw-r--r--   0        0        0     4965 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/README.md
--rw-r--r--   0        0        0       76 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/codecov.yml
--rw-r--r--   0        0        0       45 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/api.md
--rw-r--r--   0        0        0    16572 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0    13931 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    48867 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     1565 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/python.md
--rw-r--r--   0        0        0     5585 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2371 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11465 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0     2080 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/contributing/guidelines.md
--rw-r--r--   0        0        0    10000 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/getting-started/development.md
--rw-r--r--   0        0        0     2367 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/index.md
--rw-r--r--   0        0        0     3897 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2023-06-21 12:35:30.019624 orchestrator_core-1.1.1rc2/docs/js/termynal.js
--rw-r--r--   0        0        0     8925 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/circuit-workflow.md
--rw-r--r--   0        0        0      254 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/database-migration.md
--rw-r--r--   0        0        0     3776 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/docker-installation.md
--rw-r--r--   0        0        0     2563 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/domain-models.md
--rw-r--r--   0        0        0     4126 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/node-workflow.md
--rw-r--r--   0        0        0     3079 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/overview.md
--rw-r--r--   0        0        0     1750 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/scenario.md
--rw-r--r--   0        0        0     4369 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/advanced/workflow-introduction.md
--rw-r--r--   0        0        0     5605 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4438 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7471 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3700 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3063 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6106 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1952 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3996 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3595 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2143 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2885 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      786 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3637 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2023-06-21 12:35:30.023624 orchestrator_core-1.1.1rc2/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0   983304 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/docs/workshops/images/netbox_devices_active.png
--rw-r--r--   0        0        0      771 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/examples/basic/basic_orchestrator.py
--rw-r--r--   0        0        0     4214 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/mkdocs.yml
--rw-r--r--   0        0        0     1267 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/mutmut_config.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/orchestrator/.stignore
--rw-r--r--   0        0        0     1098 2023-06-21 12:35:30.027623 orchestrator_core-1.1.1rc2/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     2871 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     2841 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1236 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    12955 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     2703 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     3331 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     2552 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     5803 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     2866 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    11864 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      996 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1833 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     1961 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1543 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    11705 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5636 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/api/models.py
--rw-r--r--   0        0        0     7395 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/app.py
--rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13831 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6853 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     1953 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10653 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9423 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    24095 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1439 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0     2371 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generate.md
--rw-r--r--   0        0        0     5168 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generate.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/__init__.py
--rw-r--r--   0        0        0     1758 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/fixed_input.py
--rw-r--r--   0        0        0     2626 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/helpers.py
--rw-r--r--   0        0        0     2607 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/migration.py
--rw-r--r--   0        0        0     2152 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/product.py
--rw-r--r--   0        0        0     5811 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/product_block.py
--rw-r--r--   0        0        0     1400 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/settings.py
--rw-r--r--   0        0        0     1794 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/translations.py
--rw-r--r--   0        0        0     4234 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/unittest.py
--rw-r--r--   0        0        0     1957 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/validations.py
--rw-r--r--   0        0        0     6559 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/workflow.py
--rw-r--r--   0        0        0      779 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/circuit.yaml
--rw-r--r--   0        0        0      557 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/node.yaml
--rw-r--r--   0        0        0      553 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/user.yaml
--rw-r--r--   0        0        0      380 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/user_group.yaml
--rw-r--r--   0        0        0      289 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/constrained_int_definitions.j2
--rw-r--r--   0        0        0     4196 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/create_product.j2
--rw-r--r--   0        0        0      337 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/list_definitions.j2
--rw-r--r--   0        0        0      520 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/macros.j2
--rw-r--r--   0        0        0     4405 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/modify_product.j2
--rw-r--r--   0        0        0     2639 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/new_product_migration.j2
--rw-r--r--   0        0        0     1675 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/product.j2
--rw-r--r--   0        0        0     2275 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/product_block.j2
--rw-r--r--   0        0        0      514 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/shared_forms.j2
--rw-r--r--   0        0        0     2808 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/terminate_product.j2
--rw-r--r--   0        0        0     1764 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_create_workflow.j2
--rw-r--r--   0        0        0     1689 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2
--rw-r--r--   0        0        0     1860 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_product_type.j2
--rw-r--r--   0        0        0     1518 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2
--rw-r--r--   0        0        0      984 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2
--rw-r--r--   0        0        0     2391 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/validate_product.j2
--rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1165 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      830 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      983 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20183 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8943 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4113 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2984 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10288 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/database.py
--rw-r--r--   0        0        0      303 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     3618 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0      774 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/__init__.py
--rw-r--r--   0        0        0      992 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/bool_filter.py
--rw-r--r--   0        0        0      952 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/is_like_filter.py
--rw-r--r--   0        0        0     2542 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/range_filter.py
--rw-r--r--   0        0        0      993 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/values_in_column_filter.py
--rw-r--r--   0        0        0     3592 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0     1251 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/product.py
--rw-r--r--   0        0        0     3203 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/filters/subscription.py
--rw-r--r--   0        0        0    23630 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/models.py
--rw-r--r--   0        0        0      104 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     1439 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      419 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0      603 2023-06-21 12:35:30.031623 orchestrator_core-1.1.1rc2/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0      418 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/db/sorting/product.py
--rw-r--r--   0        0        0     4427 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0      606 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/db/sorting/subscription.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    16866 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0     2508 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2533 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3062 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3329 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      924 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    62844 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2694 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     2977 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0     5434 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     2145 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/forms/network_type_validators.py
--rw-r--r--   0        0        0    11483 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/forms/validators.py
--rw-r--r--   0        0        0     5373 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4325 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     1777 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/extensions/error_collector_extension.py
--rw-r--r--   0        0        0     2334 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0      420 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/__init__.py
--rw-r--r--   0        0        0     3674 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2154 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/product.py
--rw-r--r--   0        0        0     3727 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/settings.py
--rw-r--r--   0        0        0     2907 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/subscription.py
--rw-r--r--   0        0        0      203 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/errors.py
--rw-r--r--   0        0        0      513 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/fixed_input.py
--rw-r--r--   0        0        0     3674 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0     1776 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/product.py
--rw-r--r--   0        0        0      530 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/product_block.py
--rw-r--r--   0        0        0      305 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/resource_type.py
--rw-r--r--   0        0        0      980 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/settings.py
--rw-r--r--   0        0        0     7736 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/subscription.py
--rw-r--r--   0        0        0      172 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/workflow.py
--rw-r--r--   0        0        0     1789 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      114 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/utils/__init__.py
--rw-r--r--   0        0        0     1071 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/utils/create_resolver_error_handler.py
--rw-r--r--   0        0        0      992 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0       39 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3365 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40397 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2641 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1266 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    38591 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      951 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1213 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1556 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5105 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7723 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0      989 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/py.typed
--rw-r--r--   0        0        0     1090 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1535 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1053 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2131 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2631 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      886 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1293 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1346 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      842 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     3390 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1670 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1735 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      951 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3180 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1013 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1803 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1797 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/security.py
--rw-r--r--   0        0        0      571 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3586 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/services/celery.py
--rw-r--r--   0        0        0    22605 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1530 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/services/products.py
--rw-r--r--   0        0        0     3879 2023-06-21 12:35:30.035622 orchestrator_core-1.1.1rc2/orchestrator/services/settings.py
--rw-r--r--   0        0        0    24525 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5708 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1719 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/services/translations.py
--rw-r--r--   0        0        0     3708 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/settings.py
--rw-r--r--   0        0        0      766 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/targets.py
--rw-r--r--   0        0        0     9449 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/types.py
--rw-r--r--   0        0        0      571 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5593 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0     6207 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     3839 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     8079 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     2785 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8512 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/json.py
--rw-r--r--   0        0        0     3376 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/redis.py
--rw-r--r--   0        0        0     2972 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/show_process.py
--rw-r--r--   0        0        0     2395 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/speed.py
--rw-r--r--   0        0        0    13148 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     7231 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/utils/vlans.py
--rw-r--r--   0        0        0     1323 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/version.py
--rw-r--r--   0        0        0     4476 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     3535 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3312 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2900 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    33615 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflow.py
--rw-r--r--   0        0        0     4085 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2135 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9204 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1510 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2120 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8335 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0    12830 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     4618 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/pyproject.toml
--rw-r--r--   0        0        0     2413 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/setup.cfg
--rw-r--r--   0        0        0      665 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/setup.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1855 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1608 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2828 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5159 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1578 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1192 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3049 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    19964 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    16019 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3742 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     7942 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2486 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     1772 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     2985 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    37706 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     2367 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0    25724 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27170 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      511 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/config.py
--rw-r--r--   0        0        0    22649 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    50537 2023-06-21 12:35:30.039622 orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8092 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4493 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     2824 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7530 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1683 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2569 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1609 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2642 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2590 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1232 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1055 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2262 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4191 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3240 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2977 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2298 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2282 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1671 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1898 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      527 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     1462 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/forms/shared.py
--rw-r--r--   0        0        0    25426 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0     7644 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_network_validators.py
--rw-r--r--   0        0        0     6626 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_post_process.py
--rw-r--r--   0        0        0    11107 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0     7301 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_product.py
--rw-r--r--   0        0        0     5174 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_settings.py
--rw-r--r--   0        0        0    23655 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_subscriptions.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    26695 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1083 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     5830 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     7353 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      385 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    12048 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1871 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3517 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3052 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     1144 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_speed.py
--rw-r--r--   0        0        0    11501 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0     8339 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_vlans.py
--rw-r--r--   0        0        0    12492 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2091 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2039 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2584 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     3390 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1877 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2023-06-21 12:35:30.043622 orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     5364 1970-01-01 00:00:00.000000 orchestrator_core-1.1.1rc2/PKG-INFO
+-rw-r--r--   0        0        0      341 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.coveragerc
+-rw-r--r--   0        0        0     2620 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      371 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      550 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1163 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2113 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1809 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.gitignore
+-rw-r--r--   0        0        0     2099 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/.stignore
+-rw-r--r--   0        0        0    29970 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/Dockerfile
+-rw-r--r--   0        0        0    11409 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/LICENSE
+-rw-r--r--   0        0        0      150 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/NOTICE
+-rw-r--r--   0        0        0     4965 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/README.md
+-rw-r--r--   0        0        0       76 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/codecov.yml
+-rw-r--r--   0        0        0       45 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/application/api.md
+-rw-r--r--   0        0        0    16572 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0    13931 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    48867 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     1565 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/application/python.md
+-rw-r--r--   0        0        0     5585 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2371 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11465 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0     2080 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0    10000 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/getting-started/development.md
+-rw-r--r--   0        0        0     2367 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/index.md
+-rw-r--r--   0        0        0     3897 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/js/termynal.js
+-rw-r--r--   0        0        0     8925 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/advanced/circuit-workflow.md
+-rw-r--r--   0        0        0      254 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/advanced/database-migration.md
+-rw-r--r--   0        0        0     3776 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/advanced/docker-installation.md
+-rw-r--r--   0        0        0     2563 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/advanced/domain-models.md
+-rw-r--r--   0        0        0     4126 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/advanced/node-workflow.md
+-rw-r--r--   0        0        0     3079 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/advanced/overview.md
+-rw-r--r--   0        0        0     1750 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/advanced/scenario.md
+-rw-r--r--   0        0        0     4369 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/advanced/workflow-introduction.md
+-rw-r--r--   0        0        0     5605 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4438 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7471 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3700 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3063 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6106 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1952 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3996 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3595 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2143 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2885 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      786 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3637 2023-06-27 07:30:52.436263 orchestrator_core-1.1.1rc3/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2023-06-27 07:30:52.440263 orchestrator_core-1.1.1rc3/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0   983304 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/docs/workshops/images/netbox_devices_active.png
+-rw-r--r--   0        0        0      771 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/examples/basic/basic_orchestrator.py
+-rw-r--r--   0        0        0     4214 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/mkdocs.yml
+-rw-r--r--   0        0        0     1267 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/mutmut_config.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/.stignore
+-rw-r--r--   0        0        0     1098 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     2819 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     2841 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1236 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    13583 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     2703 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     3331 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     2552 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     5803 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     2866 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    11864 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0     1033 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1833 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     1961 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1543 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    11705 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5636 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/api/models.py
+-rw-r--r--   0        0        0     7482 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13831 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6853 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     1953 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10653 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9423 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    24095 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1439 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0     2371 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generate.md
+-rw-r--r--   0        0        0     5168 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generate.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/__init__.py
+-rw-r--r--   0        0        0     1758 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/fixed_input.py
+-rw-r--r--   0        0        0     2626 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/helpers.py
+-rw-r--r--   0        0        0     2607 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/migration.py
+-rw-r--r--   0        0        0     2152 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/product.py
+-rw-r--r--   0        0        0     5811 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/product_block.py
+-rw-r--r--   0        0        0     1400 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/settings.py
+-rw-r--r--   0        0        0     1794 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/translations.py
+-rw-r--r--   0        0        0     4234 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/unittest.py
+-rw-r--r--   0        0        0     1957 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/validations.py
+-rw-r--r--   0        0        0     6543 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/workflow.py
+-rw-r--r--   0        0        0      779 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/products/workshop/circuit.yaml
+-rw-r--r--   0        0        0      557 2023-06-27 07:30:52.444263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/products/workshop/node.yaml
+-rw-r--r--   0        0        0      553 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/products/workshop/user.yaml
+-rw-r--r--   0        0        0      380 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/products/workshop/user_group.yaml
+-rw-r--r--   0        0        0      289 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/constrained_int_definitions.j2
+-rw-r--r--   0        0        0     4196 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/create_product.j2
+-rw-r--r--   0        0        0      337 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/list_definitions.j2
+-rw-r--r--   0        0        0      520 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/macros.j2
+-rw-r--r--   0        0        0     4405 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/modify_product.j2
+-rw-r--r--   0        0        0     2639 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/new_product_migration.j2
+-rw-r--r--   0        0        0     1675 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/product.j2
+-rw-r--r--   0        0        0     2275 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/product_block.j2
+-rw-r--r--   0        0        0      514 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/shared_forms.j2
+-rw-r--r--   0        0        0     2808 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/terminate_product.j2
+-rw-r--r--   0        0        0     1764 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/test_create_workflow.j2
+-rw-r--r--   0        0        0     1689 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/test_modify_workflow.j2
+-rw-r--r--   0        0        0     1860 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/test_product_type.j2
+-rw-r--r--   0        0        0     1518 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/test_terminate_workflow.j2
+-rw-r--r--   0        0        0      984 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/test_validate_workflow.j2
+-rw-r--r--   0        0        0     2391 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/validate_product.j2
+-rw-r--r--   0        0        0      571 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1165 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      830 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      983 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20183 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8943 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4113 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2984 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10288 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/database.py
+-rw-r--r--   0        0        0      303 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     3618 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0      774 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/filters/generic_filters/__init__.py
+-rw-r--r--   0        0        0      992 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/filters/generic_filters/bool_filter.py
+-rw-r--r--   0        0        0      952 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/filters/generic_filters/is_like_filter.py
+-rw-r--r--   0        0        0     2542 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/filters/generic_filters/range_filter.py
+-rw-r--r--   0        0        0      993 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/filters/generic_filters/values_in_column_filter.py
+-rw-r--r--   0        0        0     3592 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0     1251 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0     3203 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/filters/subscription.py
+-rw-r--r--   0        0        0    23630 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/models.py
+-rw-r--r--   0        0        0      104 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     1439 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      419 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0      603 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      418 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0     4427 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0      606 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/db/sorting/subscription.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    16866 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0     2508 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2533 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3062 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3329 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      924 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    62796 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2694 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     2977 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0     5434 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     2145 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/forms/network_type_validators.py
+-rw-r--r--   0        0        0    11483 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/forms/validators.py
+-rw-r--r--   0        0        0     5373 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4325 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     1777 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/extensions/error_collector_extension.py
+-rw-r--r--   0        0        0     2334 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      420 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0     3674 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2154 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     3727 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0     2907 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/resolvers/subscription.py
+-rw-r--r--   0        0        0      203 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     3674 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0     1776 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0      530 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      305 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      980 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0     7736 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/subscription.py
+-rw-r--r--   0        0        0      172 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     1789 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      114 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0     1071 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/utils/create_resolver_error_handler.py
+-rw-r--r--   0        0        0      992 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0       39 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3365 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40397 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2023-06-27 07:30:52.448263 orchestrator_core-1.1.1rc3/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2641 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1266 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    38591 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      951 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1213 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1556 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5105 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7723 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0      989 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/py.typed
+-rw-r--r--   0        0        0     1090 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1535 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1053 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2131 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2631 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      886 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1293 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1346 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      842 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     3390 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1670 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1735 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      951 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3180 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1013 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1803 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1797 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3586 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/services/celery.py
+-rw-r--r--   0        0        0    22589 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1530 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/services/products.py
+-rw-r--r--   0        0        0     3879 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    24525 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5708 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1719 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     3708 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/targets.py
+-rw-r--r--   0        0        0     9449 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5593 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0     6207 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     3839 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     8079 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     2785 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8512 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     3376 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0     2972 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/show_process.py
+-rw-r--r--   0        0        0     2395 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/speed.py
+-rw-r--r--   0        0        0    13148 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     7231 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/utils/vlans.py
+-rw-r--r--   0        0        0     1323 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/version.py
+-rw-r--r--   0        0        0     4476 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     3535 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3312 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2900 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    33615 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4085 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2135 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9188 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2120 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8335 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0    12830 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     4617 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/pyproject.toml
+-rw-r--r--   0        0        0     2413 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/setup.cfg
+-rw-r--r--   0        0        0      665 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/setup.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.452263 orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1855 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1608 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2828 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5159 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1578 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1192 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3049 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    19964 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    16019 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3742 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     7942 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2486 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     1772 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     2985 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    37706 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     2367 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0    25724 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27170 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/config.py
+-rw-r--r--   0        0        0    22649 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    50537 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8092 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4493 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     2824 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7530 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1683 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2569 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1609 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2642 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2590 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1232 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1055 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2262 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4191 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3240 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2977 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2298 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2282 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1671 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1898 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      527 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     1462 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/forms/shared.py
+-rw-r--r--   0        0        0    25426 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0     7644 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/forms/test_network_validators.py
+-rw-r--r--   0        0        0     6626 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/forms/test_post_process.py
+-rw-r--r--   0        0        0    11107 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     7301 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0     5174 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0    23655 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/graphql/test_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    26695 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1083 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     5830 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     7353 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      385 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    12048 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-27 07:30:52.456263 orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1871 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3517 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3052 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     1144 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_speed.py
+-rw-r--r--   0        0        0    11501 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0     8339 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_vlans.py
+-rw-r--r--   0        0        0    12492 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2091 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2039 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2584 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     3390 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1877 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2023-06-27 07:30:52.460263 orchestrator_core-1.1.1rc3/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     5363 1970-01-01 00:00:00.000000 orchestrator_core-1.1.1rc3/PKG-INFO
```

### Comparing `orchestrator_core-1.1.1rc2/.github/workflows/README.md` & `orchestrator_core-1.1.1rc3/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/.github/workflows/build-push-container.yml` & `orchestrator_core-1.1.1rc3/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/.github/workflows/codeql-analysis.yml` & `orchestrator_core-1.1.1rc3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/.github/workflows/publish-package.yml` & `orchestrator_core-1.1.1rc3/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/.github/workflows/run-linting-tests.yml` & `orchestrator_core-1.1.1rc3/.github/workflows/run-linting-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/.github/workflows/run-unit-tests.yml` & `orchestrator_core-1.1.1rc3/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/.github/workflows/scheduled-build.yml` & `orchestrator_core-1.1.1rc3/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/.gitignore` & `orchestrator_core-1.1.1rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/.pre-commit-config.yaml` & `orchestrator_core-1.1.1rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/.stignore` & `orchestrator_core-1.1.1rc3/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/CHANGELOG.md` & `orchestrator_core-1.1.1rc3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/LICENSE` & `orchestrator_core-1.1.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/README.md` & `orchestrator_core-1.1.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/architecture/application/cli.md` & `orchestrator_core-1.1.1rc3/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/architecture/application/domainmodels.md` & `orchestrator_core-1.1.1rc3/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/architecture/application/forms.md` & `orchestrator_core-1.1.1rc3/docs/architecture/application/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/architecture/application/openapi.json` & `orchestrator_core-1.1.1rc3/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/architecture/application/python.md` & `orchestrator_core-1.1.1rc3/docs/architecture/application/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/architecture/application/scaling.md` & `orchestrator_core-1.1.1rc3/docs/architecture/application/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/architecture/application/tasks.md` & `orchestrator_core-1.1.1rc3/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/architecture/application/websockets.md` & `orchestrator_core-1.1.1rc3/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/architecture/application/workflow.md` & `orchestrator_core-1.1.1rc3/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/architecture/tldr.md` & `orchestrator_core-1.1.1rc3/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/contributing/guidelines.md` & `orchestrator_core-1.1.1rc3/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/contributing/testing.md` & `orchestrator_core-1.1.1rc3/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/css/termynal.css` & `orchestrator_core-1.1.1rc3/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/getting-started/base.md` & `orchestrator_core-1.1.1rc3/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/getting-started/development.md` & `orchestrator_core-1.1.1rc3/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/index.md` & `orchestrator_core-1.1.1rc3/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/js/custom.js` & `orchestrator_core-1.1.1rc3/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/js/termynal.js` & `orchestrator_core-1.1.1rc3/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/advanced/circuit-workflow.md` & `orchestrator_core-1.1.1rc3/docs/workshops/advanced/circuit-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/advanced/docker-installation.md` & `orchestrator_core-1.1.1rc3/docs/workshops/advanced/docker-installation.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/advanced/domain-models.md` & `orchestrator_core-1.1.1rc3/docs/workshops/advanced/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/advanced/node-workflow.md` & `orchestrator_core-1.1.1rc3/docs/workshops/advanced/node-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/advanced/overview.md` & `orchestrator_core-1.1.1rc3/docs/workshops/advanced/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/advanced/scenario.md` & `orchestrator_core-1.1.1rc3/docs/workshops/advanced/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/advanced/workflow-introduction.md` & `orchestrator_core-1.1.1rc3/docs/workshops/advanced/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/create-user.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/database-migration.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/debian.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/docker.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/domain-models.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/explore.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/input-forms.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/macos.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/modify-user.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/overview.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/scenario.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/start-applications.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-1.1.1rc3/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/images/metadata_products.png` & `orchestrator_core-1.1.1rc3/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/docs/workshops/images/netbox_devices_active.png` & `orchestrator_core-1.1.1rc3/docs/workshops/images/netbox_devices_active.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/examples/basic/basic_orchestrator.py` & `orchestrator_core-1.1.1rc3/examples/basic/basic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/mkdocs.yml` & `orchestrator_core-1.1.1rc3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/mutmut_config.py` & `orchestrator_core-1.1.1rc3/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "1.1.1rc2"
+__version__ = "1.1.1rc3"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/api.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,15 @@
 api_router = APIRouter()
 api_router.include_router(
     fixed_input.router,
     prefix="/fixed_inputs",
     tags=["Core", "Fixed Inputs"],
     dependencies=[Depends(opa_security_default)],
 )
-api_router.include_router(
-    processes.router, prefix="/processes", tags=["Core", "Processes"], dependencies=[Depends(opa_security_default)]
-)
+api_router.include_router(processes.router, prefix="/processes", tags=["Core", "Processes"])
 
 api_router.include_router(
     product_blocks.router,
     prefix="/product_blocks",
     tags=["Core", "Product Blocks"],
     dependencies=[Depends(opa_security_default)],
 )
```

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import zlib
 from dataclasses import asdict
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
 
 import structlog
-from fastapi import Query, Request, WebSocket
+from fastapi import Request, WebSocket
 from fastapi.param_functions import Body, Depends, Header
 from fastapi.routing import APIRouter
 from fastapi_etag.dependency import CacheHit
 from more_itertools import chunked
 from oauth2_lib.fastapi import OIDCUserModel
 from sqlalchemy.orm import contains_eager, defer, joinedload
 from sqlalchemy.sql import expression
@@ -43,15 +43,15 @@
     ProcessListItemSchema,
     ProcessResumeAllSchema,
     ProcessSchema,
     ProcessSubscriptionBaseSchema,
     ProcessSubscriptionSchema,
 )
 from orchestrator.schemas.process import ProcessStatusCounts
-from orchestrator.security import oidc_user
+from orchestrator.security import oidc_user, opa_security_default
 from orchestrator.services.processes import (
     SYSTEM_USER,
     _async_resume_processes,
     _get_process,
     abort_process,
     api_broadcast_process_data,
     load_process,
@@ -65,28 +65,35 @@
 from orchestrator.workflow import ProcessStatus
 
 router = APIRouter()
 
 logger = structlog.get_logger(__name__)
 
 
-@router.delete("/{pid}", response_model=None, status_code=HTTPStatus.NO_CONTENT)
+@router.delete(
+    "/{pid}", response_model=None, status_code=HTTPStatus.NO_CONTENT, dependencies=[Depends(opa_security_default)]
+)
 def delete(pid: UUID) -> None:
     process = ProcessTable.query.filter_by(pid=pid).one_or_none()
     if not process:
         raise_status(HTTPStatus.NOT_FOUND)
 
     websocket_data = {"process": {"id": process.pid, "status": ProcessStatus.ABORTED}}
     send_process_data_to_websocket(process.pid, websocket_data)
 
     ProcessTable.query.filter_by(pid=pid).delete()
     db.session.commit()
 
 
-@router.post("/{workflow_key}", response_model=ProcessIdSchema, status_code=HTTPStatus.CREATED)
+@router.post(
+    "/{workflow_key}",
+    response_model=ProcessIdSchema,
+    status_code=HTTPStatus.CREATED,
+    dependencies=[Depends(opa_security_default)],
+)
 def new_process(
     workflow_key: str,
     request: Request,
     json_data: Optional[List[Dict[str, Any]]] = Body(...),
     user: Optional[OIDCUserModel] = Depends(oidc_user),
 ) -> Dict[str, UUID]:
     check_global_lock()
@@ -94,15 +101,20 @@
     user_name = user.user_name if user else SYSTEM_USER
     broadcast_func = api_broadcast_process_data(request)
     pid = start_process(workflow_key, user_inputs=json_data, user=user_name, broadcast_func=broadcast_func)
 
     return {"id": pid}
 
 
-@router.put("/{pid}/resume", response_model=None, status_code=HTTPStatus.NO_CONTENT)
+@router.put(
+    "/{pid}/resume",
+    response_model=None,
+    status_code=HTTPStatus.NO_CONTENT,
+    dependencies=[Depends(opa_security_default)],
+)
 def resume_process_endpoint(
     pid: UUID, request: Request, json_data: JSON = Body(...), user: Optional[OIDCUserModel] = Depends(oidc_user)
 ) -> None:
     check_global_lock()
 
     process = _get_process(pid)
 
@@ -117,15 +129,15 @@
 
     user_name = user.user_name if user else SYSTEM_USER
 
     broadcast_func = api_broadcast_process_data(request)
     resume_process(process, user=user_name, user_inputs=json_data, broadcast_func=broadcast_func)
 
 
-@router.put("/resume-all", response_model=ProcessResumeAllSchema)
+@router.put("/resume-all", response_model=ProcessResumeAllSchema, dependencies=[Depends(opa_security_default)])
 async def resume_all_processess_endpoint(
     request: Request, user: Optional[OIDCUserModel] = Depends(oidc_user)
 ) -> Dict[str, int]:
     """Retry all task processes in status Failed, Waiting, API Unavailable or Inconsistent Data.
 
     The retry is started in the background, returning status 200 and number of processes in message.
     When it is already running, refuse and return status 409 instead.
@@ -155,41 +167,49 @@
         raise_status(HTTPStatus.CONFLICT, "Another request to resume all processes is in progress")
 
     logger.info("Resuming all processes", count=len(processes_to_resume))
 
     return {"count": len(processes_to_resume)}
 
 
-@router.put("/{pid}/abort", response_model=None, status_code=HTTPStatus.NO_CONTENT)
+@router.put(
+    "/{pid}/abort", response_model=None, status_code=HTTPStatus.NO_CONTENT, dependencies=[Depends(opa_security_default)]
+)
 def abort_process_endpoint(pid: UUID, request: Request, user: Optional[OIDCUserModel] = Depends(oidc_user)) -> None:
     process = _get_process(pid)
 
     user_name = user.user_name if user else SYSTEM_USER
     broadcast_func = api_broadcast_process_data(request)
     try:
         abort_process(process, user_name, broadcast_func=broadcast_func)
         return None
     except Exception as e:
         raise_status(HTTPStatus.INTERNAL_SERVER_ERROR, str(e))
 
 
 @router.get(
-    "/process-subscriptions-by-subscription-id/{subscription_id}", response_model=List[ProcessSubscriptionSchema]
+    "/process-subscriptions-by-subscription-id/{subscription_id}",
+    response_model=List[ProcessSubscriptionSchema],
+    dependencies=[Depends(opa_security_default)],
 )
 def process_subscriptions_by_subscription_id(subscription_id: UUID) -> List[ProcessSubscriptionSchema]:
     query = (
         ProcessSubscriptionTable.query.options(contains_eager(ProcessSubscriptionTable.process))
         .join(ProcessTable)
         .filter(ProcessSubscriptionTable.subscription_id == subscription_id)
         .order_by(ProcessTable.started_at.asc())
     )
     return query.all()
 
 
-@router.get("/process-subscriptions-by-pid/{pid}", response_model=List[ProcessSubscriptionBaseSchema])
+@router.get(
+    "/process-subscriptions-by-pid/{pid}",
+    response_model=List[ProcessSubscriptionBaseSchema],
+    dependencies=[Depends(opa_security_default)],
+)
 def process_subscriptions_by_process_pid(pid: UUID) -> List[ProcessSubscriptionTable]:
     return ProcessSubscriptionTable.query.filter_by(pid=pid).all()
 
 
 def check_global_lock() -> None:
     """
     Check the global lock of the engine.
@@ -202,20 +222,20 @@
     if engine_settings.global_lock:
         logger.info("Unable to interact with processes at this time. Engine StatusEnum is locked")
         raise_status(
             HTTPStatus.SERVICE_UNAVAILABLE, detail="Engine is locked cannot accept changes on processes at this time"
         )
 
 
-@router.get("/statuses", response_model=List[ProcessStatus])
+@router.get("/statuses", response_model=List[ProcessStatus], dependencies=[Depends(opa_security_default)])
 def statuses() -> List[str]:
     return [status.value for status in ProcessStatus]
 
 
-@router.get("/status-counts", response_model=ProcessStatusCounts)
+@router.get("/status-counts", response_model=ProcessStatusCounts, dependencies=[Depends(opa_security_default)])
 def status_counts() -> ProcessStatusCounts:
     """Retrieve status counts for processes and tasks."""
     rows = (
         ProcessTable.query.with_entities(
             ProcessTable.is_task, ProcessTable.last_status, count(ProcessTable.last_status)
         )
         .group_by(ProcessTable.is_task, ProcessTable.last_status)
@@ -223,34 +243,34 @@
     )
     return ProcessStatusCounts(
         process_counts={status: num_processes for is_task, status, num_processes in rows if not is_task},
         task_counts={status: num_processes for is_task, status, num_processes in rows if is_task},
     )
 
 
-@router.get("/assignees", response_model=List[Assignee])
+@router.get("/assignees", response_model=List[Assignee], dependencies=[Depends(opa_security_default)])
 def assignees() -> List[str]:
     return [assignee.value for assignee in Assignee]
 
 
-@router.get("/{pid}", response_model=ProcessSchema)
+@router.get("/{pid}", response_model=ProcessSchema, dependencies=[Depends(opa_security_default)])
 def show(pid: UUID) -> Dict[str, Any]:
     process = _get_process(pid)
     p = load_process(process)
 
     data = show_process(process, p)
     return data
 
 
 def handle_process_error(message: str, **kwargs: Any) -> None:
     logger.debug(message, **kwargs)
     raise_status(HTTPStatus.BAD_REQUEST, message)
 
 
-@router.get("/", response_model=List[ProcessListItemSchema])
+@router.get("/", response_model=List[ProcessListItemSchema], dependencies=[Depends(opa_security_default)])
 def processes_filterable(
     response: Response,
     range: Optional[str] = None,
     sort: Optional[str] = None,
     filter: Optional[str] = None,
     if_none_match: Optional[str] = Header(None),
 ) -> List[Dict[str, Any]]:
@@ -320,15 +340,15 @@
 
     return [asdict(enrich_process(p)) for p in results]
 
 
 if app_settings.ENABLE_WEBSOCKETS:
 
     @router.websocket("/all/")
-    async def websocket_process_list(websocket: WebSocket, token: str = Query(...)) -> None:
+    async def websocket_process_list(websocket: WebSocket, token: str) -> None:
         error = await websocket_manager.authorize(websocket, token)
 
         await websocket.accept()
         if error:
             await websocket_manager.disconnect(websocket, reason=error)
             return
```

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/product_blocks.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import structlog
-from fastapi import Query
 from fastapi.routing import APIRouter
+from pydantic import constr
 
 from orchestrator.services.translations import generate_translations
 
 logger = structlog.get_logger(__name__)
 
 
 router = APIRouter()
 
+language_str = constr(regex="^[a-z]+-[A-Z]+$")
+
 
 @router.get("/{language}", response_model=dict)
-def get_translations(language: str = Query(..., regex="^[a-z]+-[A-Z]+$")) -> dict:
+def get_translations(language: language_str) -> dict:  # type: ignore
     translations = generate_translations(language)
 
     return translations
```

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/error_handling.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/api/models.py` & `orchestrator_core-1.1.1rc3/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/app.py` & `orchestrator_core-1.1.1rc3/orchestrator/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,16 @@
         sentry_sdk.init(
             dsn=sentry_dsn,
             traces_sample_rate=trace_sample_rate,
             server_name=server_name,
             environment=environment,
             release=f"orchestrator@{release}",
             integrations=[SqlalchemyIntegration(), RedisIntegration(), FastApiIntegration(transaction_style="url")],
+            propagate_traces=True,
+            profiles_sample_rate=trace_sample_rate,
         )
 
     @staticmethod
     def register_subscription_models(product_to_subscription_model_mapping: Dict[str, Type[SubscriptionModel]]) -> None:
         """
         Register your subscription models.
```

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/database.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generate.md` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generate.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generate.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/fixed_input.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/migration.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/product.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/product_block.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/settings.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/translations.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/unittest.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/unittest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/validations.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/validations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/generator/workflow.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/generator/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
     @wraps(f)
     def wrapper(environment: Environment, config: dict, writer: Callable) -> Any:
         def workflow_enabled() -> bool:
             return all(wf.get("enabled", True) for wf in config.get("workflows", []) if wf["name"] == workflow)
 
         if workflow_enabled():
-            return f(environment, config, writer)  # type: ignore
+            return f(environment, config, writer)
 
     return wrapper
 
 
 @generate_workflow(workflow="create")
 def generate_create_workflow(environment: Environment, config: dict, writer: Callable) -> None:
     product_block = root_product_block(config)
```

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/circuit.yaml` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/products/workshop/circuit.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/node.yaml` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/products/workshop/node.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/products/workshop/user.yaml` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/products/workshop/user.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/create_product.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/create_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/macros.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/modify_product.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/modify_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/new_product_migration.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/new_product_migration.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/product.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/product_block.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/product_block.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/shared_forms.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/shared_forms.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/terminate_product.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/terminate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_create_workflow.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/test_create_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/test_modify_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_product_type.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/test_product_type.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/test_terminate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/test_validate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/generator/templates/validate_product.j2` & `orchestrator_core-1.1.1rc3/orchestrator/cli/generator/templates/validate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/main.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/migration_helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/cli/scheduler.py` & `orchestrator_core-1.1.1rc3/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/config/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/config/assignee.py` & `orchestrator_core-1.1.1rc3/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/database.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/filters/filters.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/filters/filters.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/filters/generic_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/bool_filter.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/filters/generic_filters/bool_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/is_like_filter.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/filters/generic_filters/is_like_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/range_filter.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/filters/generic_filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/filters/generic_filters/values_in_column_filter.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/filters/generic_filters/values_in_column_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/filters/process.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/filters/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/filters/product.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/filters/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/filters/subscription.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/filters/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/models.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/range/range.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/range/range.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/sorting/process.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/sorting/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/sorting/sorting.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/sorting/sorting.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/db/sorting/subscription.py` & `orchestrator_core-1.1.1rc3/orchestrator/db/sorting/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/devtools/populator.py` & `orchestrator_core-1.1.1rc3/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/distlock/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-1.1.1rc3/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-1.1.1rc3/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-1.1.1rc3/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/domain/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/domain/base.py` & `orchestrator_core-1.1.1rc3/orchestrator/domain/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1167,15 +1167,15 @@
             description=description,
             status=status,
             insync=insync,
             start_date=start_date,
             end_date=end_date,
             note=note,
             **fixed_inputs,
-            **instances,  # type: ignore
+            **instances,
         )
         model._db_model = subscription
         return model
 
     @classmethod
     def from_other_lifecycle(
         cls: Type[S],
@@ -1271,15 +1271,15 @@
                 description=subscription.description,
                 status=status,
                 insync=subscription.insync,
                 start_date=subscription.start_date,
                 end_date=subscription.end_date,
                 note=subscription.note,
                 **fixed_inputs,
-                **instances,  # type: ignore
+                **instances,
             )
             model._db_model = subscription
             return model
         except ValidationError:
             logger.exception(
                 "Subscription is not correct in database", loaded_fixed_inputs=fixed_inputs, loaded_instances=instances
             )
@@ -1321,15 +1321,15 @@
                 description=subscription.description,
                 status=status,
                 insync=subscription.insync,
                 start_date=subscription.start_date,
                 end_date=subscription.end_date,
                 note=subscription.note,
                 **fixed_inputs,
-                **instances,  # type: ignore
+                **instances,
             )
             model._db_model = subscription
             return model
         except ValidationError:
             logger.exception(
                 "Subscription is not correct in database", loaded_fixed_inputs=fixed_inputs, loaded_instances=instances
             )
```

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/domain/lifecycle.py` & `orchestrator_core-1.1.1rc3/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/exception_handlers.py` & `orchestrator_core-1.1.1rc3/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/forms/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/forms/network_type_validators.py` & `orchestrator_core-1.1.1rc3/orchestrator/forms/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/forms/validators.py` & `orchestrator_core-1.1.1rc3/orchestrator/forms/validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/extensions/error_collector_extension.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/extensions/error_collector_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/pagination.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/resolvers/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/product.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/resolvers/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/settings.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/resolvers/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/resolvers/subscription.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/resolvers/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/fixed_input.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/process.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/product.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/product_block.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/settings.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/schemas/subscription.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/types.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/utils/create_resolver_error_handler.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/utils/create_resolver_error_handler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-1.1.1rc3/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/alembic.ini` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/env.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py` & `orchestrator_core-1.1.1rc3/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schedules/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-1.1.1rc3/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schedules/scheduling.py` & `orchestrator_core-1.1.1rc3/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-1.1.1rc3/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schedules/validate_products.py` & `orchestrator_core-1.1.1rc3/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-1.1.1rc3/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/base.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/engine_settings.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/fixed_input.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/problem_detail.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/process.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/product.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/product_block.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/resource_type.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/subscription.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/schemas/workflow.py` & `orchestrator_core-1.1.1rc3/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/security.py` & `orchestrator_core-1.1.1rc3/orchestrator/security.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/services/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/services/celery.py` & `orchestrator_core-1.1.1rc3/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/services/processes.py` & `orchestrator_core-1.1.1rc3/orchestrator/services/processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
                         logger.info("Cannot resume a resumed process", pid=_proc.pid)
                         continue
                     resume_process(process, user=user_name, broadcast_func=broadcast_func)
                 except Exception:
                     logger.exception("Failed to resume process", pid=_proc.pid)
             logger.info("Completed resuming processes")
         finally:
-            distlock_manager.release_sync(lock)  # type: ignore
+            distlock_manager.release_sync(lock)
 
     # Start all jobs in the background. BackgroundTasks might be more suited.
     workflow_executor = get_thread_pool()
     process_handle = workflow_executor.submit(run)
     if app_settings.TESTING:
         process_handle.result()
     return True
```

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/services/products.py` & `orchestrator_core-1.1.1rc3/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/services/settings.py` & `orchestrator_core-1.1.1rc3/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/services/subscriptions.py` & `orchestrator_core-1.1.1rc3/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/services/tasks.py` & `orchestrator_core-1.1.1rc3/orchestrator/services/tasks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/services/translations.py` & `orchestrator_core-1.1.1rc3/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/settings.py` & `orchestrator_core-1.1.1rc3/orchestrator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/targets.py` & `orchestrator_core-1.1.1rc3/orchestrator/targets.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/types.py` & `orchestrator_core-1.1.1rc3/orchestrator/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/crypt.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/datetime.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/docs.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/errors.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/functional.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/helpers.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/json.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/redis.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/redis.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/show_process.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/show_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/speed.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/state.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/strings.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/utils/vlans.py` & `orchestrator_core-1.1.1rc3/orchestrator/utils/vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/version.py` & `orchestrator_core-1.1.1rc3/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/websocket/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-1.1.1rc3/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-1.1.1rc3/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-1.1.1rc3/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflow.py` & `orchestrator_core-1.1.1rc3/orchestrator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflows/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflows/modify_note.py` & `orchestrator_core-1.1.1rc3/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflows/removed_workflow.py` & `orchestrator_core-1.1.1rc3/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflows/steps.py` & `orchestrator_core-1.1.1rc3/orchestrator/workflows/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                 for item in subscription_instance:
                     if isinstance(item, ProductBlockModel):
                         _cache_other_subscriptions(item)
 
             # If subscription_instance is a ProductBlockModel check the owner_subscription_id to decide the cache
             elif isinstance(subscription_instance, ProductBlockModel):
                 _cache_other_subscriptions(subscription_instance)
-                if not subscription_instance.owner_subscription_id == subscription.subscription_id:  # type: ignore
+                if not subscription_instance.owner_subscription_id == subscription.subscription_id:
                     cached_subscription_ids.add(subscription_instance.owner_subscription_id)
 
     for field in subscription.__fields__:
         # There always is a single Root Product Block, it cannot be a list, so no need to check.
         instance: Union[ProductBlockModel, Any] = getattr(subscription, field)
         if isinstance(instance, ProductBlockModel):
             _cache_other_subscriptions(instance)
```

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-1.1.1rc3/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-1.1.1rc3/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-1.1.1rc3/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-1.1.1rc3/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-1.1.1rc3/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/orchestrator/workflows/utils.py` & `orchestrator_core-1.1.1rc3/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/pyproject.toml` & `orchestrator_core-1.1.1rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,41 +38,41 @@
 ]
 dependencies = [
     "alembic==1.5.4",
     "anyio>=3.7.0",
     "broadcaster[redis]==0.2.0",
     "click==8.0.3",
     "deepmerge==0.1.0",
-    "fastapi~=0.91.0",
+    "fastapi~=0.98.0",
     "fastapi-etag==0.4.0",
     "more-itertools~=9.0.0",
     "itsdangerous==2.1.2",
     "Jinja2==3.1.2",
     "opentelemetry-distro",
     "opentelemetry-exporter-otlp",
     "opentelemetry-instrumentation-httpx",
     "opentelemetry-instrumentation-fastapi",
     "opentelemetry-instrumentation-psycopg2",
     "opentelemetry-instrumentation-redis",
     "opentelemetry-instrumentation-sqlalchemy",
-    "orjson==3.8.0",
+    "orjson==3.9.1",
     "psycopg2-binary==2.9.5",
-    "pydantic[email]==1.10.2",
+    "pydantic[email]==1.10.9",
     "python-dateutil==2.8.2",
     "python-rapidjson==1.9",
-    "pytz==2022.7.1",
+    "pytz==2023.3",
     "redis>=4.5.5,<4.6",
     "schedule==1.1.0",
     "sentry-sdk[fastapi]==1.25.1",
-    "SQLAlchemy==1.4.28",
+    "SQLAlchemy==1.4.48",
     "SQLAlchemy-Utils==0.40.0",
     "typer==0.7.0",
     "uvicorn[standard]~=0.20.0",
-    "nwa-stdlib~=1.4.7",
-    "oauth2-lib~=1.2.9",
+    "nwa-stdlib~=1.4.8",
+    "oauth2-lib~=1.2.10",
     "markupsafe==2.0.1",
     "bandit==1.7.2",
     "tabulate==0.9.0",
     "strawberry-graphql==0.171.1"
 ]
 description-file = "README.md"
 requires-python = ">=3.9,<3.12"
```

### Comparing `orchestrator_core-1.1.1rc2/setup.cfg` & `orchestrator_core-1.1.1rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/setup.py` & `orchestrator_core-1.1.1rc3/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/acceptance_tests/conftest.py` & `orchestrator_core-1.1.1rc3/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-1.1.1rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/acceptance_tests/test_test_product.py` & `orchestrator_core-1.1.1rc3/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_caching.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_health.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_helpers.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_models.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_processes.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_product_blocks.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_products.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_resource_types.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_settings.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/api/test_workflows.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/conftest.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/processes.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/forms/shared.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/forms/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_network_validators.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/forms/test_network_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/forms/test_post_process.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/forms/test_post_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/graphql/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_product.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/graphql/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_settings.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/graphql/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/graphql/test_subscriptions.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/graphql/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/services/test_processes.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/services/test_products.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/services/test_translations.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/test_db.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/test_workflow.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_errors.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_functional.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_json.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_speed.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_state.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/utils/test_vlans.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/utils/test_vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/__init__.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-1.1.1rc3/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc2/PKG-INFO` & `orchestrator_core-1.1.1rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 1.1.1rc2
+Version: 1.1.1rc3
 Summary: Open source orchestration software for NREN's
 Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -28,41 +28,41 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: alembic==1.5.4
 Requires-Dist: anyio>=3.7.0
 Requires-Dist: broadcaster[redis]==0.2.0
 Requires-Dist: click==8.0.3
 Requires-Dist: deepmerge==0.1.0
-Requires-Dist: fastapi~=0.91.0
+Requires-Dist: fastapi~=0.98.0
 Requires-Dist: fastapi-etag==0.4.0
 Requires-Dist: more-itertools~=9.0.0
 Requires-Dist: itsdangerous==2.1.2
 Requires-Dist: Jinja2==3.1.2
 Requires-Dist: opentelemetry-distro
 Requires-Dist: opentelemetry-exporter-otlp
 Requires-Dist: opentelemetry-instrumentation-httpx
 Requires-Dist: opentelemetry-instrumentation-fastapi
 Requires-Dist: opentelemetry-instrumentation-psycopg2
 Requires-Dist: opentelemetry-instrumentation-redis
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy
-Requires-Dist: orjson==3.8.0
+Requires-Dist: orjson==3.9.1
 Requires-Dist: psycopg2-binary==2.9.5
-Requires-Dist: pydantic[email]==1.10.2
+Requires-Dist: pydantic[email]==1.10.9
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-rapidjson==1.9
-Requires-Dist: pytz==2022.7.1
+Requires-Dist: pytz==2023.3
 Requires-Dist: redis>=4.5.5,<4.6
 Requires-Dist: schedule==1.1.0
 Requires-Dist: sentry-sdk[fastapi]==1.25.1
-Requires-Dist: SQLAlchemy==1.4.28
+Requires-Dist: SQLAlchemy==1.4.48
 Requires-Dist: SQLAlchemy-Utils==0.40.0
 Requires-Dist: typer==0.7.0
 Requires-Dist: uvicorn[standard]~=0.20.0
-Requires-Dist: nwa-stdlib~=1.4.7
-Requires-Dist: oauth2-lib~=1.2.9
+Requires-Dist: nwa-stdlib~=1.4.8
+Requires-Dist: oauth2-lib~=1.2.10
 Requires-Dist: markupsafe==2.0.1
 Requires-Dist: bandit==1.7.2
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: strawberry-graphql==0.171.1
 Requires-Dist: celery~=5.2.7 ; extra == "celery"
 Requires-Dist: toml ; extra == "dev"
 Requires-Dist: bumpversion ; extra == "dev"
```

