# Comparing `tmp/dbnomics_fetcher_ops-0.6.0.tar.gz` & `tmp/dbnomics_fetcher_ops-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnomics_fetcher_ops-0.6.0.tar", max compression
+gzip compressed data, was "dbnomics_fetcher_ops-0.6.1.tar", max compression
```

## Comparing `dbnomics_fetcher_ops-0.6.0.tar` & `dbnomics_fetcher_ops-0.6.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0    34475 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/LICENSE
--rw-r--r--   0        0        0     1228 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-06-06 14:46:00.231417 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/__init__.py
--rw-r--r--   0        0        0      883 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/app_args.py
--rw-r--r--   0        0        0     2443 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/cli.py
--rw-r--r--   0        0        0      845 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/cli_utils.py
--rw-r--r--   0        0        0      251 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/__init__.py
--rw-r--r--   0        0        0     4687 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/apply.py
--rw-r--r--   0        0        0     2162 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/clean_workspace.py
--rw-r--r--   0        0        0     2752 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/clean_workspaces.py
--rw-r--r--   0        0        0    23542 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/configure.py
--rw-r--r--   0        0        0     1227 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/list.py
--rw-r--r--   0        0        0     1813 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/prune.py
--rw-r--r--   0        0        0     1429 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/run.py
--rw-r--r--   0        0        0     6351 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/undeploy.py
--rw-r--r--   0        0        0      798 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/file_utils.py
--rw-r--r--   0        0        0      499 2023-06-06 14:43:54.022811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/format_utils.py
--rw-r--r--   0        0        0      379 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/gitlab_utils.py
--rw-r--r--   0        0        0     1309 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/loaders.py
--rw-r--r--   0        0        0      441 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/errors.py
--rw-r--r--   0        0        0     1667 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/fetcher_metadata/base.py
--rw-r--r--   0        0        0     1619 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/fetcher_metadata/gitlab.py
--rw-r--r--   0        0        0     2487 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipeline_repo/gitlab.py
--rw-r--r--   0        0        0     1332 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipeline_repo/in_memory.py
--rw-r--r--   0        0        0      356 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipeline_repo/protocol.py
--rw-r--r--   0        0        0      685 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipelines_config.py
--rw-r--r--   0        0        0      453 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/validators.py
--rw-r--r--   0        0        0        0 2023-06-06 14:46:00.231417 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/py.typed
--rw-r--r--   0        0        0        0 2023-06-06 14:46:00.231417 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/__init__.py
--rw-r--r--   0        0        0     3567 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/clean_pipeline_workspaces.py
--rw-r--r--   0        0        0     2380 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/prune_fetcher.py
--rw-r--r--   0        0        0     2893 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/run_fetcher_pipeline.py
--rw-r--r--   0        0        0      845 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/ssh.py
--rw-r--r--   0        0        0      483 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/utils.py
--rw-r--r--   0        0        0     1437 2023-06-06 14:43:54.026811 dbnomics_fetcher_ops-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 dbnomics_fetcher_ops-0.6.0/setup.py
--rw-r--r--   0        0        0     2210 1970-01-01 00:00:00.000000 dbnomics_fetcher_ops-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34475 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1228 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 16:50:55.430025 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/__init__.py
+-rw-r--r--   0        0        0      883 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/app_args.py
+-rw-r--r--   0        0        0     2485 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/cli.py
+-rw-r--r--   0        0        0      845 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/cli_utils.py
+-rw-r--r--   0        0        0      276 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/__init__.py
+-rw-r--r--   0        0        0     4687 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/apply.py
+-rw-r--r--   0        0        0     2162 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/clean_workspace.py
+-rw-r--r--   0        0        0     2752 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/clean_workspaces.py
+-rw-r--r--   0        0        0    23542 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/configure.py
+-rw-r--r--   0        0        0     1227 2023-06-27 16:48:57.273458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/list.py
+-rw-r--r--   0        0        0     1813 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/prune.py
+-rw-r--r--   0        0        0     1602 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/retry.py
+-rw-r--r--   0        0        0     1429 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/run.py
+-rw-r--r--   0        0        0     6351 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/undeploy.py
+-rw-r--r--   0        0        0      798 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/file_utils.py
+-rw-r--r--   0        0        0      499 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/format_utils.py
+-rw-r--r--   0        0        0      379 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/gitlab_utils.py
+-rw-r--r--   0        0        0     1309 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/loaders.py
+-rw-r--r--   0        0        0      441 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/errors.py
+-rw-r--r--   0        0        0     1667 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/fetcher_metadata/base.py
+-rw-r--r--   0        0        0     1619 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/fetcher_metadata/gitlab.py
+-rw-r--r--   0        0        0     2690 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/pipeline_repo/gitlab.py
+-rw-r--r--   0        0        0     1334 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/pipeline_repo/in_memory.py
+-rw-r--r--   0        0        0      358 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/pipeline_repo/protocol.py
+-rw-r--r--   0        0        0      685 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/pipelines_config.py
+-rw-r--r--   0        0        0      453 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/validators.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:50:55.434025 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/py.typed
+-rw-r--r--   0        0        0        0 2023-06-27 16:50:55.434025 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/services/__init__.py
+-rw-r--r--   0        0        0     3569 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/services/clean_pipeline_workspaces.py
+-rw-r--r--   0        0        0     2544 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/services/prune_fetcher.py
+-rw-r--r--   0        0        0     3467 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/services/retry_fetcher_pipeline_job.py
+-rw-r--r--   0        0        0     2893 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/services/run_fetcher_pipeline.py
+-rw-r--r--   0        0        0      845 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/ssh.py
+-rw-r--r--   0        0        0      483 2023-06-27 16:48:57.277458 dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/utils.py
+-rw-r--r--   0        0        0     1437 2023-06-27 16:48:57.281458 dbnomics_fetcher_ops-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 dbnomics_fetcher_ops-0.6.1/setup.py
+-rw-r--r--   0        0        0     2210 1970-01-01 00:00:00.000000 dbnomics_fetcher_ops-0.6.1/PKG-INFO
```

### Comparing `dbnomics_fetcher_ops-0.6.0/LICENSE` & `dbnomics_fetcher_ops-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/README.md` & `dbnomics_fetcher_ops-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/app_args.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/app_args.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/cli.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 app = typer.Typer()
 app.command(name="apply")(commands.apply)
 app.command(name="clean-workspace")(commands.clean_workspace)
 app.command(name="clean-workspaces")(commands.clean_workspaces)
 app.command(name="configure")(commands.configure)
 app.command(name="list")(commands.list_)
 app.command(name="prune")(commands.prune)
+app.command(name="retry")(commands.retry)
 app.command(name="run")(commands.run)
 app.command(name="undeploy")(commands.undeploy)
 
 
 @app.callback(context_settings={"help_option_names": ["-h", "--help"]})
 def main_callback(
     debug: bool = typer.Option(False, "-d", "--debug", envvar="DEBUG", help="Display DEBUG log messages"),
```

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/cli_utils.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/apply.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/apply.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/clean_workspace.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/clean_workspace.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/clean_workspaces.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/clean_workspaces.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/configure.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/configure.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/list.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/list.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/prune.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/prune.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/run.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/run.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/commands/undeploy.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/commands/undeploy.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/file_utils.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/file_utils.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/loaders.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/loaders.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/fetcher_metadata/base.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/fetcher_metadata/base.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/fetcher_metadata/gitlab.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/fetcher_metadata/gitlab.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipeline_repo/gitlab.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/pipeline_repo/gitlab.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,39 +19,42 @@
     def from_app_args(cls, app_args: AppArgs):
         gitlab_base_url = app_args.fetcher_metadata.gitlab.base_url
         gl = init_gitlab_client(
             gitlab_base_url, enable_debug=app_args.debug_gitlab, private_token=app_args.gitlab_private_token
         )
         return cls(fetcher_metadata=app_args.fetcher_metadata, gl=gl)
 
-    def get_pipelines_to_keep(
+    def fetch_latest_pipeline(self, project: Project, *, status: str | None = None) -> ProjectPipeline | None:
+        return next(self.fetch_latest_pipelines(project, status=status), None)
+
+    def fetch_latest_pipelines(self, project: Project, *, status: str | None = None) -> Iterator[ProjectPipeline]:
+        return cast(
+            Iterator[ProjectPipeline],
+            project.pipelines.list(status=status, order_by="updated_at", sorted="desc", iterator=True),
+        )
+
+    def fetch_pipelines_to_keep(
         self, provider_slug: str, *, keep_failed_count: int, keep_success_count: int
     ) -> PipelinesByStatus:
         project = self._fetch_project(provider_slug)
         return self._fetch_pipelines_to_keep(
             project, keep_failed_count=keep_failed_count, keep_success_count=keep_success_count
         )
 
-    def _fetch_latest_pipelines(self, project: Project, *, status: str) -> Iterator[ProjectPipeline]:
-        return cast(
-            Iterator[ProjectPipeline],
-            project.pipelines.list(status=status, order_by="updated_at", sorted="desc", iterator=True),
-        )
-
     def _fetch_pipelines_to_keep(
         self, project: Project, *, keep_failed_count: int, keep_success_count: int
     ) -> PipelinesByStatus:
         return PipelinesByStatus(
             failed=[
                 pipeline.id
-                for pipeline in islice(self._fetch_latest_pipelines(project, status="failed"), keep_failed_count)
+                for pipeline in islice(self.fetch_latest_pipelines(project, status="failed"), keep_failed_count)
             ],
-            running=[pipeline.id for pipeline in self._fetch_latest_pipelines(project, status="running")],
+            running=[pipeline.id for pipeline in self.fetch_latest_pipelines(project, status="running")],
             success=[
                 pipeline.id
-                for pipeline in islice(self._fetch_latest_pipelines(project, status="success"), keep_success_count)
+                for pipeline in islice(self.fetch_latest_pipelines(project, status="success"), keep_success_count)
             ],
         )
 
     def _fetch_project(self, provider_slug: str) -> Project:
         project_path_with_namespace = self._fetcher_metadata.gitlab.fetcher.get_path_with_namespace(provider_slug)
         return self._gl.projects.get(project_path_with_namespace)
```

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipeline_repo/in_memory.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/pipeline_repo/in_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dbnomics_fetcher_ops.model.pipeline_repo.protocol import PipelinesByStatus
 
 
 class InMemoryPipelineRepo:
     def __init__(self, pipelines_by_provider_slug: dict[str, PipelinesByStatus]):
         self._pipelines_by_provider_slug = pipelines_by_provider_slug
 
-    def get_pipelines_to_keep(
+    def fetch_pipelines_to_keep(
         self, provider_slug: str, *, keep_failed_count: int, keep_success_count: int
     ) -> PipelinesByStatus:
         provider_pipelines = self._pipelines_by_provider_slug[provider_slug]
         return PipelinesByStatus(
             failed=list(islice(provider_pipelines.failed, keep_failed_count)),
             running=provider_pipelines.running,
             success=list(islice(provider_pipelines.success, keep_success_count)),
```

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/model/pipelines_config.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/model/pipelines_config.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/clean_pipeline_workspaces.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/services/clean_pipeline_workspaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     pipeline_repo: PipelineRepo,
 ) -> Optional[int]:
     provider_slug = workspace_dir.name
 
     fetcher_def = fetcher_metadata.find_fetcher_def_by_provider_slug(provider_slug)
     provider_code = fetcher_def.provider_code
 
-    pipelines_to_keep = pipeline_repo.get_pipelines_to_keep(
+    pipelines_to_keep = pipeline_repo.fetch_pipelines_to_keep(
         provider_slug, keep_failed_count=keep_failed_count, keep_success_count=keep_success_count
     )
     logger.debug("Keeping pipeline directories of fetcher %r: %r", provider_code, pipelines_to_keep)
 
     reclaimed_bytes = 0
     for pipeline_dir in sorted(iter_child_directories(workspace_dir / "pipelines", warn_other=True)):
         pipeline_dir_size = clean_fetcher_workspace_pipeline_directory(
```

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/prune_fetcher.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/services/prune_fetcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,9 +48,13 @@
 
     def _delete_deploy_key(self, title: str, *, project: Project) -> None:
         logger.debug("Deleting the deploy key %r from %r...", title, project.path_with_namespace)
         key = next((key for key in project.keys.list() if key.title == title), None)
         if key is None:
             logger.debug("No deploy key with title %r found for %r", title, project.path_with_namespace)
             return
-        key.delete()
-        logger.info("%r deleted from %r", key, project.path_with_namespace)
+
+        if self.dry_run:
+            logger.info("[SKIPPED (dry-run)] %r would have been deleted from %r", key, project.path_with_namespace)
+        else:
+            key.delete()
+            logger.info("%r deleted from %r", key, project.path_with_namespace)
```

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/services/run_fetcher_pipeline.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/services/run_fetcher_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/dbnomics_fetcher_ops/ssh.py` & `dbnomics_fetcher_ops-0.6.1/dbnomics_fetcher_ops/ssh.py`

 * *Files identical despite different names*

### Comparing `dbnomics_fetcher_ops-0.6.0/pyproject.toml` & `dbnomics_fetcher_ops-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbnomics-fetcher-ops"
-version = "0.6.0"
+version = "0.6.1"
 description = "Manage DBnomics fetchers"
 authors = ["Christophe Benz <christophe.benz@nomics.world>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [{ include = "dbnomics_fetcher_ops" }]
 
 [tool.poetry.dependencies]
```

### Comparing `dbnomics_fetcher_ops-0.6.0/setup.py` & `dbnomics_fetcher_ops-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'xdg>=5.1.1,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['dbnomics-fetchers = dbnomics_fetcher_ops.cli:app']}
 
 setup_kwargs = {
     'name': 'dbnomics-fetcher-ops',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': 'Manage DBnomics fetchers',
     'long_description': '# DBnomics fetcher ops\n\nManage DBnomics fetchers: list, configure and run pipelines.\n\n## Install\n\n```bash\npip install dbnomics-fetcher-ops[cli]\n```\n\n## Usage\n\n### Configure a fetcher\n\nThe configure command needs write privileges. Create a GitLab [personal access token](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) having the `api` scope, and pass it using the `--gitlab-private-token` option or the `GITLAB_PRIVATE_TOKEN` environment variable in `~/.config/dbnomics/dbnomics-fetchers.env`.\n\n```bash\ndbnomics-fetchers -v configure scsmich --dry-run\n# If everything seems OK, remove the --dry-run flag:\ndbnomics-fetchers -v configure scsmich\n```\n\n### List fetchers\n\n```bash\ndbnomics-fetchers -v list\n```\n\n### Run fetcher pipelines\n\n```bash\n# Replace PROVIDER_SLUG by the real value:\ndbnomics-fetchers -v run --provider-slug PROVIDER_SLUG\n\n# To run a pipeline for each fetcher:\ndbnomics-fetchers -v list --slug | xargs -I {} dbnomics-fetchers -v run --provider-slug {}\n```\n\n## Development\n\nInstall [Poetry](https://python-poetry.org/).\n\n```bash\n# git clone repo or fork\ncd dbnomics-fetcher-ops\npoetry install\ncp .env.example .env\n```\n\nRun commands with:\n\n```bash\npoetry shell\ndbnomics-fetchers COMMAND\n```\n',
     'author': 'Christophe Benz',
     'author_email': 'christophe.benz@nomics.world',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dbnomics_fetcher_ops-0.6.0/PKG-INFO` & `dbnomics_fetcher_ops-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnomics-fetcher-ops
-Version: 0.6.0
+Version: 0.6.1
 Summary: Manage DBnomics fetchers
 License: AGPL-3.0-or-later
 Author: Christophe Benz
 Author-email: christophe.benz@nomics.world
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

