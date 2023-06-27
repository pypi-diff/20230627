# Comparing `tmp/jupyter_scheduler-1.3.2.tar.gz` & `tmp/jupyter_scheduler-1.3.3.tar.gz`

## Comparing `jupyter_scheduler-1.3.2.tar` & `jupyter_scheduler-1.3.3.tar`

### file list

```diff
@@ -1,168 +1,168 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.eslintrc.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.prettierrc
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.stylelintrc
--rw-r--r--   0        0        0    31582 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/CHANGELOG.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/MANIFEST.in
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/babel.config.js
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/conftest.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/install.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jest.config.js
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/setup.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/tsconfig.json
--rw-r--r--   0        0        0   473708 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/yarn.lock
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/binder/environment.yml
--rwxr-xr-x   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/binder/postBuild
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/dev/seed.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/dev/templates/1.ipynb
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/dev/templates/2.ipynb
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/dev/templates/3.ipynb
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/Makefile
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/conf.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/make.bat
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/requirements.txt
--rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/_static/jupyter_logo.png
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/contributors/index.md
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/developers/index.md
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/operators/index.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/index.md
--rw-r--r--   0        0        0    91253 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/actions_definition_details.png
--rw-r--r--   0        0        0    72256 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/actions_job_details.png
--rw-r--r--   0        0        0    23784 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/actions_list.png
--rw-r--r--   0        0        0   102590 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/create_job_form.png
--rw-r--r--   0        0        0   130914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/create_job_from_filebrowser.png
--rw-r--r--   0        0        0    28924 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/create_job_from_notebook.png
--rw-r--r--   0        0        0    74875 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/custom_schedule.png
--rw-r--r--   0        0        0    39322 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/download_button.png
--rw-r--r--   0        0        0    45498 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/downloaded_files.png
--rw-r--r--   0        0        0    67024 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/headers.png
--rw-r--r--   0        0        0    58085 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/item_name.png
--rw-r--r--   0        0        0    92104 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/launcher.png
--rw-r--r--   0        0        0    56679 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/run_on_schedule.png
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter-config/nb-config/jupyter_scheduler.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter-config/server-config/jupyter_scheduler.json
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/_version.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/environments.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/exceptions.py
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/executors.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/extension.py
--rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/handlers.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/job_files_manager.py
--rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/models.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/orm.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/parameterize.py
--rw-r--r--   0        0        0    30914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/scheduler.py
--rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/task_runner.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/utils.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/package.json
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/122.b4ab1a65371e7c0f8bdd.js
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js
--rw-r--r--   0        0        0   347357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/177.57d0a2a23069220f5e7d.js
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js
--rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js
--rw-r--r--   0        0        0    19234 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js
--rw-r--r--   0        0        0   121687 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js.LICENSE.txt
--rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js.LICENSE.txt
--rw-r--r--   0        0        0   210890 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js
--rw-r--r--   0        0        0    21625 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js.LICENSE.txt
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js
--rw-r--r--   0        0        0    80399 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/810.a39d1a3a560985b29e1f.js
--rw-r--r--   0        0        0    25917 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js
--rw-r--r--   0        0        0    10078 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/remoteEntry.a26c2ca760e8eddba3c9.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/style.js
--rw-r--r--   0        0        0    40850 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/mocks.py
--rw-r--r--   0        0        0    27273 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_handlers.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_job_files_manager.py
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_scheduler.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/utils.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.html
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/schema/plugin.json
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/advanced-options.tsx
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/context.ts
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/handler.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/hooks.ts
--rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/index.tsx
--rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/model.ts
--rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/notebook-jobs-panel.tsx
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/size.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/svg.d.ts
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/theme-provider.ts
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/tokens.ts
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/__tests__/jupyter_scheduler.spec.ts
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/box.tsx
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/button-bar.tsx
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/button.tsx
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/cluster.tsx
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/collapsible-panel.tsx
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/compute-type-picker.tsx
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/confirm-buttons.tsx
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/confirm-dialog-buttons.tsx
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/create-schedule-options.tsx
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/environment-picker.tsx
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/error-boundary.tsx
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/heading.tsx
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/icon-buttons.tsx
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/icons.ts
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/input-file-snapshot.tsx
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/job-definition-row.tsx
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/job-file-link.tsx
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/job-row.tsx
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/labeled-value.tsx
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/output-format-picker.tsx
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/parameters-picker.tsx
--rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/schedule-inputs.tsx
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/stack.tsx
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/advanced-table/advanced-table-header.tsx
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/advanced-table/advanced-table.tsx
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/advanced-table/index.tsx
--rw-r--r--   0        0        0     8298 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/create-job-from-definition.tsx
--rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/create-job.tsx
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/edit-job-definition.tsx
--rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/list-jobs.tsx
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/detail-view/detail-view.tsx
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/detail-view/index.tsx
--rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/detail-view/job-definition.tsx
--rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/detail-view/job-detail.tsx
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/util/errors.tsx
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/util/job-name-validation.tsx
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/base.css
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/box.css
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/button.css
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/cluster.css
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/collapsible-panel.css
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/edit-job-definitions.css
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/heading.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/index.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/labeled-value.css
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/stack.css
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/variables.css
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/icons/calendar-add-on.svg
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/icons/calendar-month.svg
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/icons/event-note.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/ui-tests/tests/jupyter_scheduler.spec.ts
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/LICENSE
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/README.md
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.eslintrc.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.prettierrc
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.stylelintrc
+-rw-r--r--   0        0        0    32953 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/MANIFEST.in
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/babel.config.js
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/conftest.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/install.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jest.config.js
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/setup.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/tsconfig.json
+-rw-r--r--   0        0        0   473708 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/yarn.lock
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/binder/environment.yml
+-rwxr-xr-x   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/binder/postBuild
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/dev/seed.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/dev/templates/1.ipynb
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/dev/templates/2.ipynb
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/dev/templates/3.ipynb
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/Makefile
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/conf.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/make.bat
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/requirements.txt
+-rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/_static/jupyter_logo.png
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/contributors/index.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/developers/index.md
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/operators/index.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/index.md
+-rw-r--r--   0        0        0    91253 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/actions_definition_details.png
+-rw-r--r--   0        0        0    72256 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/actions_job_details.png
+-rw-r--r--   0        0        0    23784 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/actions_list.png
+-rw-r--r--   0        0        0   102590 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/create_job_form.png
+-rw-r--r--   0        0        0   130914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/create_job_from_filebrowser.png
+-rw-r--r--   0        0        0    28924 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/create_job_from_notebook.png
+-rw-r--r--   0        0        0    74875 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/custom_schedule.png
+-rw-r--r--   0        0        0    39322 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/download_button.png
+-rw-r--r--   0        0        0    45498 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/downloaded_files.png
+-rw-r--r--   0        0        0    67024 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/headers.png
+-rw-r--r--   0        0        0    58085 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/item_name.png
+-rw-r--r--   0        0        0    92104 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/launcher.png
+-rw-r--r--   0        0        0    56679 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/docs/users/images/run_on_schedule.png
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter-config/nb-config/jupyter_scheduler.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter-config/server-config/jupyter_scheduler.json
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/_version.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/environments.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/exceptions.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/executors.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/extension.py
+-rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/handlers.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/job_files_manager.py
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/models.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/orm.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/parameterize.py
+-rw-r--r--   0        0        0    30914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/scheduler.py
+-rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/task_runner.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/utils.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/package.json
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/122.b4ab1a65371e7c0f8bdd.js
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js
+-rw-r--r--   0        0        0   347357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/177.57d0a2a23069220f5e7d.js
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js
+-rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js
+-rw-r--r--   0        0        0    19234 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js
+-rw-r--r--   0        0        0   121687 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js.LICENSE.txt
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js.LICENSE.txt
+-rw-r--r--   0        0        0   210890 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js
+-rw-r--r--   0        0        0    21625 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js.LICENSE.txt
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js
+-rw-r--r--   0        0        0    80414 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/810.e798ed21e01eb5bbedc6.js
+-rw-r--r--   0        0        0    25917 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js
+-rw-r--r--   0        0        0    10072 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/remoteEntry.4716e9b91831e140cc89.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/style.js
+-rw-r--r--   0        0        0    40850 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/mocks.py
+-rw-r--r--   0        0        0    27273 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_handlers.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_job_files_manager.py
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_scheduler.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/utils.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.html
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/schema/plugin.json
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/advanced-options.tsx
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/context.ts
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/handler.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/hooks.ts
+-rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/index.tsx
+-rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/model.ts
+-rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/notebook-jobs-panel.tsx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/size.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/svg.d.ts
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/theme-provider.ts
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/tokens.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/__tests__/jupyter_scheduler.spec.ts
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/box.tsx
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/button-bar.tsx
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/button.tsx
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/cluster.tsx
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/collapsible-panel.tsx
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/compute-type-picker.tsx
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/confirm-buttons.tsx
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/confirm-dialog-buttons.tsx
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/create-schedule-options.tsx
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/environment-picker.tsx
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/error-boundary.tsx
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/heading.tsx
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/icon-buttons.tsx
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/icons.ts
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/input-file-snapshot.tsx
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/job-definition-row.tsx
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/job-file-link.tsx
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/job-row.tsx
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/labeled-value.tsx
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/output-format-picker.tsx
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/parameters-picker.tsx
+-rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/schedule-inputs.tsx
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/stack.tsx
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/advanced-table/advanced-table-header.tsx
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/advanced-table/advanced-table.tsx
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/components/advanced-table/index.tsx
+-rw-r--r--   0        0        0     8298 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/create-job-from-definition.tsx
+-rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/create-job.tsx
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/edit-job-definition.tsx
+-rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/list-jobs.tsx
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/detail-view/detail-view.tsx
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/detail-view/index.tsx
+-rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/detail-view/job-definition.tsx
+-rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/mainviews/detail-view/job-detail.tsx
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/util/errors.tsx
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/src/util/job-name-validation.tsx
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/base.css
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/box.css
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/button.css
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/cluster.css
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/collapsible-panel.css
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/edit-job-definitions.css
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/heading.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/index.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/labeled-value.css
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/stack.css
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/variables.css
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/icons/calendar-add-on.svg
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/icons/calendar-month.svg
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/style/icons/event-note.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/ui-tests/tests/jupyter_scheduler.spec.ts
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/LICENSE
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/README.md
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.3/PKG-INFO
```

### Comparing `jupyter_scheduler-1.3.2/.eslintrc.js` & `jupyter_scheduler-1.3.3/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/.pre-commit-config.yaml` & `jupyter_scheduler-1.3.3/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     rev: 5.12.0
     hooks:
       - id: isort
         args: ["--profile", "black"]
         files: \.py$
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.4.0
+    rev: v3.7.0
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
 
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
@@ -42,15 +42,15 @@
             "flake8-bugbear==20.1.4",
             "flake8-logging-format==0.6.0",
             "flake8-implicit-str-concat==0.2.0",
           ]
         stages: [manual]
 
   - repo: https://github.com/sirosen/check-jsonschema
-    rev: 0.23.0
+    rev: 0.23.2
     hooks:
       - id: check-jsonschema
         name: "Check GitHub Workflows"
         files: ^\.github/workflows/
         types: [yaml]
         args: ["--schemafile", "https://json.schemastore.org/github-workflow"]
         stages: [manual]
```

### Comparing `jupyter_scheduler-1.3.2/.stylelintrc` & `jupyter_scheduler-1.3.3/.stylelintrc`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/CHANGELOG.md` & `jupyter_scheduler-1.3.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.3.3
+
+([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v1.3.2...5cd14b538a656e8fd2318dbbb687f2bf4da8fd37))
+
+### Bugs fixed
+
+- Fix 'icon' prop typing for ConfirmButton component [#386](https://github.com/jupyter-server/jupyter-scheduler/pull/386) ([@andrii-i](https://github.com/andrii-i))
+- Add click handler to mouseDown on confirm button for Safari compatibilty [#385](https://github.com/jupyter-server/jupyter-scheduler/pull/385) ([@JasonWeill](https://github.com/JasonWeill))
+
+### Maintenance and upkeep improvements
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-scheduler/graphs/contributors?from=2023-05-11&to=2023-06-27&type=c))
+
+[@andrii-i](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Aandrii-i+updated%3A2023-05-11..2023-06-27&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Agithub-actions+updated%3A2023-05-11..2023-06-27&type=Issues) | [@JasonWeill](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3AJasonWeill+updated%3A2023-05-11..2023-06-27&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Apre-commit-ci+updated%3A2023-05-11..2023-06-27&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.3.2
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v1.3.1...6e4081a273b6da508942d3fe0b4a8ee75f2eade3))
 
 ### Bugs fixed
 
 - Fixed encoding while reading notebook in some platforms [#354](https://github.com/jupyter-server/jupyter-scheduler/pull/354) ([@3coins](https://github.com/3coins))
@@ -20,16 +39,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-scheduler/graphs/contributors?from=2023-02-27&to=2023-05-11&type=c))
 
 [@3coins](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3A3coins+updated%3A2023-02-27..2023-05-11&type=Issues) | [@dependabot](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Adependabot+updated%3A2023-02-27..2023-05-11&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Agithub-actions+updated%3A2023-02-27..2023-05-11&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Apre-commit-ci+updated%3A2023-02-27..2023-05-11&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.3.1
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v1.3.0...e36032d3331200b4f21261bdc50e8d733e66b2bc))
 
 ### Bugs fixed
 
 - Fixed issue with extension always deactivating [#347](https://github.com/jupyter-server/jupyter-scheduler/pull/347) ([@3coins](https://github.com/3coins))
```

### Comparing `jupyter_scheduler-1.3.2/MANIFEST.in` & `jupyter_scheduler-1.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/conftest.py` & `jupyter_scheduler-1.3.3/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jest.config.js` & `jupyter_scheduler-1.3.3/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/package.json` & `jupyter_scheduler-1.3.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'1.3.3'"}*

```diff
@@ -136,9 +136,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.3.2"
+    "version": "1.3.3"
 }
```

### Comparing `jupyter_scheduler-1.3.2/tsconfig.json` & `jupyter_scheduler-1.3.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/yarn.lock` & `jupyter_scheduler-1.3.3/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/binder/postBuild` & `jupyter_scheduler-1.3.3/binder/postBuild`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/dev/seed.py` & `jupyter_scheduler-1.3.3/dev/seed.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/dev/templates/1.ipynb` & `jupyter_scheduler-1.3.3/dev/templates/1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/dev/templates/2.ipynb` & `jupyter_scheduler-1.3.3/dev/templates/2.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/dev/templates/3.ipynb` & `jupyter_scheduler-1.3.3/dev/templates/3.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/Makefile` & `jupyter_scheduler-1.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/conf.py` & `jupyter_scheduler-1.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/make.bat` & `jupyter_scheduler-1.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/_static/jupyter_logo.png` & `jupyter_scheduler-1.3.3/docs/_static/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/contributors/index.md` & `jupyter_scheduler-1.3.3/docs/contributors/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/developers/index.md` & `jupyter_scheduler-1.3.3/docs/developers/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/operators/index.md` & `jupyter_scheduler-1.3.3/docs/operators/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/index.md` & `jupyter_scheduler-1.3.3/docs/users/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/actions_definition_details.png` & `jupyter_scheduler-1.3.3/docs/users/images/actions_definition_details.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/actions_job_details.png` & `jupyter_scheduler-1.3.3/docs/users/images/actions_job_details.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/actions_list.png` & `jupyter_scheduler-1.3.3/docs/users/images/actions_list.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/create_job_form.png` & `jupyter_scheduler-1.3.3/docs/users/images/create_job_form.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/create_job_from_filebrowser.png` & `jupyter_scheduler-1.3.3/docs/users/images/create_job_from_filebrowser.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/create_job_from_notebook.png` & `jupyter_scheduler-1.3.3/docs/users/images/create_job_from_notebook.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/custom_schedule.png` & `jupyter_scheduler-1.3.3/docs/users/images/custom_schedule.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/download_button.png` & `jupyter_scheduler-1.3.3/docs/users/images/download_button.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/downloaded_files.png` & `jupyter_scheduler-1.3.3/docs/users/images/downloaded_files.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/headers.png` & `jupyter_scheduler-1.3.3/docs/users/images/headers.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/item_name.png` & `jupyter_scheduler-1.3.3/docs/users/images/item_name.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/launcher.png` & `jupyter_scheduler-1.3.3/docs/users/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/docs/users/images/run_on_schedule.png` & `jupyter_scheduler-1.3.3/docs/users/images/run_on_schedule.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/environments.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/environments.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/exceptions.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/executors.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/executors.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/extension.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/handlers.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/job_files_manager.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/job_files_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/models.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/models.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/orm.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/orm.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/parameterize.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/parameterize.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/scheduler.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/task_runner.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/task_runner.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/utils.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/package.json` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.4716e9b91831e140cc89.js'}}",*

 * * "'version'": "'1.3.3'"}*

```diff
@@ -72,15 +72,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a26c2ca760e8eddba3c9.js",
+            "load": "static/remoteEntry.4716e9b91831e140cc89.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_scheduler"
                 },
@@ -141,9 +141,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.3.2"
+    "version": "1.3.3"
 }
```

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'1.3.3'"}*

```diff
@@ -136,9 +136,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.3.2"
+    "version": "1.3.3"
 }
```

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/177.57d0a2a23069220f5e7d.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/177.57d0a2a23069220f5e7d.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/810.a39d1a3a560985b29e1f.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/810.e798ed21e01eb5bbedc6.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5,32 +5,32 @@
             n.r(t), n.d(t, {
                 CommandIDs: () => mt,
                 JobsView: () => E,
                 NotebookJobsPanelId: () => ut,
                 Scheduler: () => st,
                 default: () => bt
             });
-            var o = n(5687),
-                a = n(3033),
-                l = n(7280),
-                r = n(1467),
-                i = n(1123),
-                s = n(8820),
-                c = n(3169),
+            var o = n(7638),
+                a = n(6303),
+                l = n(122),
+                r = n(9071),
+                i = n(127),
+                s = n(5139),
+                c = n(8720),
                 d = n(6271),
                 m = n.n(d),
                 u = n(296);
 
             function h(e) {
                 let t = "jp-jobs-Cluster";
                 return t += ` justify-content-${e.justifyContent||"flex-start"}`, t += ` align-items-${e.alignItems||"center"}`, t += ` gap-${e.gap||1}`, m().createElement("div", {
                     className: t
                 }, e.children)
             }
-            var p = n(2502);
+            var p = n(1745);
             const b = {
                 lineHeight: 0
             };
 
             function v(e) {
                 return m().createElement(u.IconButton, {
                     "aria-label": "delete",
@@ -287,15 +287,15 @@
                     name: "jupyterlab-scheduler:calendar-month",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 18" height="16px" width="16px">\n  <path fill="#0097A7" d="M10 12q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q10.312 12 10 12Zm-3.25 0q-.312 0-.531-.219Q6 11.562 6 11.25q0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q7.062 12 6.75 12Zm6.5 0q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531-.219.219-.531.219ZM10 15q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q10.312 15 10 15Zm-3.25 0q-.312 0-.531-.219Q6 14.562 6 14.25q0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q7.062 15 6.75 15Zm6.5 0q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531-.219.219-.531.219ZM4.5 18q-.625 0-1.062-.448Q3 17.104 3 16.5v-11q0-.604.438-1.052Q3.875 4 4.5 4H6V2h1.5v2h5V2H14v2h1.5q.625 0 1.062.448Q17 4.896 17 5.5v11q0 .604-.438 1.052Q16.125 18 15.5 18Zm0-1.5h11V9h-11v7.5Z"/>\n</svg>\n'
                 }),
                 x = new p.LabIcon({
                     name: "jupyterlab-scheduler:event-note",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 48 48" height="48" width="48">\n  <path fill="#0097A7" d="M14 27v-3h20v3Zm0 9v-3h13.95v3Zm-5 8q-1.2 0-2.1-.9Q6 42.2 6 41V10q0-1.2.9-2.1Q7.8 7 9 7h3.25V4h3.25v3h17V4h3.25v3H39q1.2 0 2.1.9.9.9.9 2.1v31q0 1.2-.9 2.1-.9.9-2.1.9Zm0-3h30V19.5H9V41Z"/>\n</svg>\n'
                 });
-            var I, F = n(8142);
+            var I, F = n(344);
             class O {
                 constructor(e) {
                     this.serverSettings = e.serverSettings || s.ServerConnection.makeSettings()
                 }
                 serializeToQueryString(e) {
                     return "?" + Object.keys(e).map((t => {
                         if ("sort_by" === t) {
@@ -1568,28 +1568,29 @@
                 }, s), e.model.statusMessage && m().createElement(u.Alert, {
                     severity: "error"
                 }, e.model.statusMessage), b, y, j, C)
             }
             var ge = n(594);
 
             function fe(e) {
-                const [t, n] = (0, d.useState)(!1), [o, a] = (0, d.useState)(!1);
+                const [t, n] = (0, d.useState)(!1), [o, a] = (0, d.useState)(!1), l = t => {
+                    e.onConfirm(), e.remainAfterConfirmation && a(!0)
+                };
                 return m().createElement(u.Box, {
                     sx: {
                         width: "6em"
                     }
                 }, t ? e.remainAfterConfirmation && o ? m().createElement(u.Chip, {
                     label: e.remainText
                 }) : m().createElement(u.Button, {
                     variant: "contained",
                     color: "error",
                     title: e.name,
-                    onClick: t => {
-                        e.onConfirm(), e.remainAfterConfirmation && a(!0)
-                    },
+                    onClick: l,
+                    onMouseDown: l,
                     onBlur: e => n(!1),
                     style: {
                         visibility: t ? "visible" : "hidden"
                     },
                     autoFocus: !0
                 }, e.confirmationText) : m().createElement(u.IconButton, {
                     title: e.name,
```

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/remoteEntry.a26c2ca760e8eddba3c9.js` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/remoteEntry.4716e9b91831e140cc89.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, d, l, i, u, f, c, s, b, p, h, m, v, y, g, j = {
+    var e, r, t, a, n, o, d, l, i, u, f, c, s, p, b, h, m, v, y, g, j = {
             947: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(687), t.e(470), t.e(271), t.e(222), t.e(948), t.e(810)]).then((() => () => t(1810))),
                         "./extension": () => Promise.all([t.e(687), t.e(470), t.e(271), t.e(222), t.e(948), t.e(810)]).then((() => () => t(1810))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -59,15 +59,15 @@
         458: "d59c5307102faf5c19a8",
         470: "add1a31599b9c294ee16",
         506: "91939c8c6d49c197dab0",
         613: "17512dda5aad1f2a390f",
         687: "fad750aa8d73847aa14f",
         747: "c67d17d558ca77e2d691",
         799: "1008956a5a660d3a40dc",
-        810: "a39d1a3a560985b29e1f",
+        810: "e798ed21e01eb5bbedc6",
         871: "cd06f2a4174d6795c435",
         948: "e8dc554b871d1bd3bef5"
     } [e] + ".js?v=" + {
         122: "b4ab1a65371e7c0f8bdd",
         171: "7e2184d69fabf35a20de",
         177: "57d0a2a23069220f5e7d",
         211: "965ff0ba094d7e4fdd24",
@@ -79,15 +79,15 @@
         458: "d59c5307102faf5c19a8",
         470: "add1a31599b9c294ee16",
         506: "91939c8c6d49c197dab0",
         613: "17512dda5aad1f2a390f",
         687: "fad750aa8d73847aa14f",
         747: "c67d17d558ca77e2d691",
         799: "1008956a5a660d3a40dc",
-        810: "a39d1a3a560985b29e1f",
+        810: "e798ed21e01eb5bbedc6",
         871: "cd06f2a4174d6795c435",
         948: "e8dc554b871d1bd3bef5"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -141,15 +141,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : d > l.from)) && (n[r] = {
                             get: t,
                             from: d,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (l("@emotion/react", "11.10.4", (() => Promise.all([P.e(275), P.e(506), P.e(271), P.e(171)]).then((() => () => P(5506))))), l("@emotion/styled", "11.10.4", (() => Promise.all([P.e(378), P.e(271), P.e(211), P.e(799), P.e(122)]).then((() => () => P(4378))))), l("@jupyterlab/scheduler", "1.3.2", (() => Promise.all([P.e(687), P.e(470), P.e(271), P.e(222), P.e(948), P.e(810)]).then((() => () => P(1810))))), l("@mui/material", "5.10.6", (() => Promise.all([P.e(687), P.e(177), P.e(470), P.e(271), P.e(222), P.e(948)]).then((() => () => P(4177))))), l("@mui/system", "5.10.6", (() => Promise.all([P.e(275), P.e(687), P.e(871), P.e(271), P.e(211), P.e(222)]).then((() => () => P(1871))))), l("cronstrue", "2.12.0", (() => P.e(458).then((() => () => P(2458))))), l("tzdata", "1.0.33", (() => P.e(613).then((() => () => P(8613)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@emotion/react", "11.10.4", (() => Promise.all([P.e(275), P.e(506), P.e(271), P.e(171)]).then((() => () => P(5506))))), l("@emotion/styled", "11.10.4", (() => Promise.all([P.e(378), P.e(271), P.e(211), P.e(799), P.e(122)]).then((() => () => P(4378))))), l("@jupyterlab/scheduler", "1.3.3", (() => Promise.all([P.e(687), P.e(470), P.e(271), P.e(222), P.e(948), P.e(810)]).then((() => () => P(1810))))), l("@mui/material", "5.10.6", (() => Promise.all([P.e(687), P.e(177), P.e(470), P.e(271), P.e(222), P.e(948)]).then((() => () => P(4177))))), l("@mui/system", "5.10.6", (() => Promise.all([P.e(275), P.e(687), P.e(871), P.e(271), P.e(211), P.e(222)]).then((() => () => P(1871))))), l("cronstrue", "2.12.0", (() => P.e(458).then((() => () => P(2458))))), l("tzdata", "1.0.33", (() => P.e(613).then((() => () => P(8613)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -220,20 +220,20 @@
                 } else {
                     if (l <= a || f < c != n) return !1;
                     i = !1
                 } else "s" != c && "n" != c && (i = !1, l--)
             }
         }
         var s = [],
-            b = s.pop.bind(s);
+            p = s.pop.bind(s);
         for (d = 1; d < e.length; d++) {
-            var p = e[d];
-            s.push(1 == p ? b() | b() : 2 == p ? b() & b() : p ? o(p, r) : !b())
+            var b = e[d];
+            s.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? o(b, r) : !p())
         }
-        return !!b()
+        return !!p()
     }, d = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
@@ -242,48 +242,48 @@
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
         var n = i(e, t);
         return o(a, n) || "undefined" != typeof console && console.warn && console.warn(u(e, t, n, a)), s(e[t][n])
     }, c = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, s = e => (e.loaded = 1, e.get()), p = (b = e => function(r, t, a, n) {
+    }, s = e => (e.loaded = 1, e.get()), b = (p = e => function(r, t, a, n) {
         var o = P.I(r);
         return o && o.then ? o.then(e.bind(e, r, P.S[r], t, a, n)) : e(r, P.S[r], t, a, n)
-    })(((e, r, t, a) => r && P.o(r, t) ? s(l(r, t)) : a())), h = b(((e, r, t, a) => (d(e, t), f(r, 0, t, a)))), m = b(((e, r, t, a, n) => {
+    })(((e, r, t, a) => r && P.o(r, t) ? s(l(r, t)) : a())), h = p(((e, r, t, a) => (d(e, t), f(r, 0, t, a)))), m = p(((e, r, t, a, n) => {
         var o = r && P.o(r, t) && c(r, t, a);
         return o ? s(o) : n()
     })), v = {}, y = {
         6271: () => h("default", "react", [1, 17, 0, 1]),
         2148: () => m("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([P.e(275), P.e(506), P.e(282)]).then((() => () => P(5506))))),
         8800: () => m("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([P.e(378), P.e(211), P.e(799)]).then((() => () => P(4378))))),
         4456: () => h("default", "react-dom", [1, 17, 0, 1]),
         7313: () => m("default", "@mui/system", [1, 5, 10, 6], (() => Promise.all([P.e(275), P.e(871), P.e(211)]).then((() => () => P(1871))))),
+        122: () => h("default", "@jupyterlab/filebrowser", [1, 3, 6, 5]),
+        127: () => h("default", "@jupyterlab/notebook", [1, 3, 6, 5]),
         296: () => m("default", "@mui/material", [1, 5, 10, 6], (() => P.e(177).then((() => () => P(4177))))),
+        344: () => h("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
         763: () => m("default", "tzdata", [1, 1, 0, 33], (() => P.e(613).then((() => () => P(8613))))),
-        1123: () => h("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        1467: () => h("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
         1526: () => h("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        1745: () => h("default", "@jupyterlab/ui-components", [1, 3, 6, 5]),
         1840: () => h("default", "@lumino/signaling", [1, 1, 10, 0]),
         2344: () => m("default", "cronstrue", [1, 2, 12, 0], (() => P.e(458).then((() => () => P(2458))))),
-        2502: () => h("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
-        3033: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        3169: () => h("default", "@jupyterlab/translation", [1, 3, 6, 3]),
-        5687: () => h("default", "@jupyterlab/application", [1, 3, 6, 3]),
-        7280: () => h("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
-        8142: () => h("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        8820: () => h("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        5211: () => p("default", "@emotion/react", (() => Promise.all([P.e(275), P.e(506), P.e(282)]).then((() => () => P(5506))))),
+        5139: () => h("default", "@jupyterlab/services", [1, 6, 6, 5]),
+        6303: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
+        7638: () => h("default", "@jupyterlab/application", [1, 3, 6, 5]),
+        8720: () => h("default", "@jupyterlab/translation", [1, 3, 6, 5]),
+        9071: () => h("default", "@jupyterlab/launcher", [1, 3, 6, 5]),
+        5211: () => b("default", "@emotion/react", (() => Promise.all([P.e(275), P.e(506), P.e(282)]).then((() => () => P(5506))))),
         799: () => m("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([P.e(275), P.e(506)]).then((() => () => P(5506)))))
     }, g = {
         211: [5211],
         222: [2148, 8800],
         271: [6271],
         799: [799],
-        810: [296, 763, 1123, 1467, 1526, 1840, 2344, 2502, 3033, 3169, 5687, 7280, 8142, 8820],
+        810: [122, 127, 296, 344, 763, 1526, 1745, 1840, 2344, 5139, 6303, 7638, 8720, 9071],
         948: [4456, 7313]
     }, P.f.consumes = (e, r) => {
         P.o(g, e) && g[e].forEach((e => {
             if (P.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, P.m[e] = t => {
                         delete P.c[e], t.exports = r()
```

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/third-party-licenses.json` & `jupyter_scheduler-1.3.3/jupyter_scheduler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/mocks.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_handlers.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_job_files_manager.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_job_files_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_scheduler.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/utils.py` & `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb` & `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb` & `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz` & `jupyter_scheduler-1.3.3/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/schema/plugin.json` & `jupyter_scheduler-1.3.3/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/advanced-options.tsx` & `jupyter_scheduler-1.3.3/src/advanced-options.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/handler.ts` & `jupyter_scheduler-1.3.3/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/index.tsx` & `jupyter_scheduler-1.3.3/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/model.ts` & `jupyter_scheduler-1.3.3/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/notebook-jobs-panel.tsx` & `jupyter_scheduler-1.3.3/src/notebook-jobs-panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/theme-provider.ts` & `jupyter_scheduler-1.3.3/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/tokens.ts` & `jupyter_scheduler-1.3.3/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/cluster.tsx` & `jupyter_scheduler-1.3.3/src/components/cluster.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/collapsible-panel.tsx` & `jupyter_scheduler-1.3.3/src/components/collapsible-panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/compute-type-picker.tsx` & `jupyter_scheduler-1.3.3/src/components/compute-type-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/confirm-buttons.tsx` & `jupyter_scheduler-1.3.3/src/components/confirm-buttons.tsx`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-import { Box, Button, Chip, IconButton, SvgIconTypeMap } from '@mui/material';
+import { Box, Button, Chip, IconButton } from '@mui/material';
 import React, { useState } from 'react';
 import { useTranslator } from '../hooks';
 import CloseIcon from '@mui/icons-material/Close';
-import { OverridableComponent } from '@mui/material/OverridableComponent';
 
 export function ConfirmButton(props: {
   onConfirm: () => void;
   confirmationText: string;
-  icon:
-    | JSX.Element
-    | (OverridableComponent<SvgIconTypeMap<unknown, 'svg'>> & {
-        muiName: string;
-      });
+  icon?: JSX.Element;
   name?: string | undefined;
   remainAfterConfirmation?: boolean;
   remainText?: string;
 }): JSX.Element | null {
   const [clicked, setClicked] = useState(false);
   const [confirmed, setConfirmed] = useState(false);
 
+  // For Safari compatibility, also apply this to the "mouseDown" event, since the
+  // "click" event doesn't fire when the user clicks or taps on a button made visible
+  // in this way
+  const clickHandler = (e: any) => {
+    props.onConfirm();
+    if (props.remainAfterConfirmation) {
+      setConfirmed(true);
+    }
+  };
+
   return (
     <Box sx={{ width: '6em' }}>
       {clicked ? (
         props.remainAfterConfirmation && confirmed ? (
           <Chip label={props.remainText} />
         ) : (
           <Button
             variant="contained"
             color="error"
             title={props.name}
-            onClick={_ => {
-              props.onConfirm();
-              if (props.remainAfterConfirmation) {
-                setConfirmed(true);
-              }
-            }}
+            onClick={clickHandler}
+            onMouseDown={clickHandler}
             onBlur={_ => setClicked(false)}
             style={{ visibility: clicked ? 'visible' : 'hidden' }}
             autoFocus
           >
             {props.confirmationText}
           </Button>
         )
```

### Comparing `jupyter_scheduler-1.3.2/src/components/confirm-dialog-buttons.tsx` & `jupyter_scheduler-1.3.3/src/components/confirm-dialog-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/create-schedule-options.tsx` & `jupyter_scheduler-1.3.3/src/components/create-schedule-options.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/environment-picker.tsx` & `jupyter_scheduler-1.3.3/src/components/environment-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/error-boundary.tsx` & `jupyter_scheduler-1.3.3/src/components/error-boundary.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/heading.tsx` & `jupyter_scheduler-1.3.3/src/components/heading.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/icon-buttons.tsx` & `jupyter_scheduler-1.3.3/src/components/icon-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/icons.ts` & `jupyter_scheduler-1.3.3/src/components/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/input-file-snapshot.tsx` & `jupyter_scheduler-1.3.3/src/components/input-file-snapshot.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/job-definition-row.tsx` & `jupyter_scheduler-1.3.3/src/components/job-definition-row.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/job-file-link.tsx` & `jupyter_scheduler-1.3.3/src/components/job-file-link.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/job-row.tsx` & `jupyter_scheduler-1.3.3/src/components/job-row.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/labeled-value.tsx` & `jupyter_scheduler-1.3.3/src/components/labeled-value.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/output-format-picker.tsx` & `jupyter_scheduler-1.3.3/src/components/output-format-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/parameters-picker.tsx` & `jupyter_scheduler-1.3.3/src/components/parameters-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/schedule-inputs.tsx` & `jupyter_scheduler-1.3.3/src/components/schedule-inputs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/advanced-table/advanced-table-header.tsx` & `jupyter_scheduler-1.3.3/src/components/advanced-table/advanced-table-header.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/components/advanced-table/advanced-table.tsx` & `jupyter_scheduler-1.3.3/src/components/advanced-table/advanced-table.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/mainviews/create-job-from-definition.tsx` & `jupyter_scheduler-1.3.3/src/mainviews/create-job-from-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/mainviews/create-job.tsx` & `jupyter_scheduler-1.3.3/src/mainviews/create-job.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/mainviews/edit-job-definition.tsx` & `jupyter_scheduler-1.3.3/src/mainviews/edit-job-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/mainviews/list-jobs.tsx` & `jupyter_scheduler-1.3.3/src/mainviews/list-jobs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/mainviews/detail-view/detail-view.tsx` & `jupyter_scheduler-1.3.3/src/mainviews/detail-view/detail-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/mainviews/detail-view/job-definition.tsx` & `jupyter_scheduler-1.3.3/src/mainviews/detail-view/job-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/mainviews/detail-view/job-detail.tsx` & `jupyter_scheduler-1.3.3/src/mainviews/detail-view/job-detail.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/util/errors.tsx` & `jupyter_scheduler-1.3.3/src/util/errors.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/src/util/job-name-validation.tsx` & `jupyter_scheduler-1.3.3/src/util/job-name-validation.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/style/base.css` & `jupyter_scheduler-1.3.3/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/style/button.css` & `jupyter_scheduler-1.3.3/style/button.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/style/cluster.css` & `jupyter_scheduler-1.3.3/style/cluster.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/style/stack.css` & `jupyter_scheduler-1.3.3/style/stack.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/style/icons/calendar-add-on.svg` & `jupyter_scheduler-1.3.3/style/icons/calendar-add-on.svg`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/style/icons/calendar-month.svg` & `jupyter_scheduler-1.3.3/style/icons/calendar-month.svg`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/ui-tests/README.md` & `jupyter_scheduler-1.3.3/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/ui-tests/jupyter_server_test_config.py` & `jupyter_scheduler-1.3.3/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/.gitignore` & `jupyter_scheduler-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/LICENSE` & `jupyter_scheduler-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/README.md` & `jupyter_scheduler-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.2/pyproject.toml` & `jupyter_scheduler-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.3.1", "jupyterlab~=3.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter_scheduler"
-version = "1.3.2"
+version = "1.3.3"
 description = "A JupyterLab extension for running notebook jobs"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 authors = [
     { name = "Project Jupyter" },
 ]
@@ -89,15 +89,15 @@
 [tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
 build_cmd = "install:extension"
 npm = ["jlpm"]
 source_dir = "src"
 build_dir = "jupyter_scheduler/labextension"
 
 [tool.tbump.version]
-current = "1.3.2"
+current = "1.3.3"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [[tool.tbump.file]]
 src = "pyproject.toml"
 version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\""
 
 [[tool.tbump.file]]
```

### Comparing `jupyter_scheduler-1.3.2/PKG-INFO` & `jupyter_scheduler-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_scheduler
-Version: 1.3.2
+Version: 1.3.3
 Summary: A JupyterLab extension for running notebook jobs
 Project-URL: Homepage, https://github.com/jupyter-server/jupyter-scheduler
 Author: Project Jupyter
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Project Jupyter
         All rights reserved.
```

