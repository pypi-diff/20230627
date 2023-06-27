# Comparing `tmp/acore_server-0.1.1.tar.gz` & `tmp/acore_server-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server-0.1.1.tar", last modified: Tue Jun 27 05:32:45 2023, max compression
+gzip compressed data, was "acore_server-0.1.2.tar", last modified: Tue Jun 27 16:01:02 2023, max compression
```

## Comparing `acore_server-0.1.1.tar` & `acore_server-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 05:32:45.525287 acore_server-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-27 04:12:52.000000 acore_server-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2023-06-27 04:12:52.000000 acore_server-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      320 2023-06-27 04:12:52.000000 acore_server-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4817 2023-06-27 05:32:45.525088 acore_server-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3694 2023-06-27 05:07:58.000000 acore_server-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 05:32:45.522899 acore_server-0.1.1/acore_server/
--rw-r--r--   0 sanhehu    (501) staff       (20)      393 2023-06-27 04:56:34.000000 acore_server-0.1.1/acore_server/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-27 04:12:52.000000 acore_server-0.1.1/acore_server/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-06-27 04:49:35.000000 acore_server-0.1.1/acore_server/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      107 2023-06-27 04:26:27.000000 acore_server-0.1.1/acore_server/constants.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 05:32:45.523811 acore_server-0.1.1/acore_server/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-27 04:12:52.000000 acore_server-0.1.1/acore_server/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    13329 2023-06-27 05:28:51.000000 acore_server-0.1.1/acore_server/fleet.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      936 2023-06-27 04:26:42.000000 acore_server-0.1.1/acore_server/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 05:32:45.524373 acore_server-0.1.1/acore_server/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-27 04:12:52.000000 acore_server-0.1.1/acore_server/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-27 04:12:52.000000 acore_server-0.1.1/acore_server/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 05:32:45.524724 acore_server-0.1.1/acore_server/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-27 04:12:52.000000 acore_server-0.1.1/acore_server/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-27 04:12:52.000000 acore_server-0.1.1/acore_server/vendor/pytest_cov_helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3272 2023-06-26 05:55:10.000000 acore_server-0.1.1/acore_server/wserver_infra_exports.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 05:32:45.523640 acore_server-0.1.1/acore_server.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4817 2023-06-27 05:32:45.000000 acore_server-0.1.1/acore_server.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      722 2023-06-27 05:32:45.000000 acore_server-0.1.1/acore_server.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-27 05:32:45.000000 acore_server-0.1.1/acore_server.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      421 2023-06-27 05:32:45.000000 acore_server-0.1.1/acore_server.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       13 2023-06-27 05:32:45.000000 acore_server-0.1.1/acore_server.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      604 2023-06-27 04:57:14.000000 acore_server-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-27 04:12:52.000000 acore_server-0.1.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-27 04:12:52.000000 acore_server-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-27 04:12:52.000000 acore_server-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-27 04:12:52.000000 acore_server-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      282 2023-06-27 04:38:45.000000 acore_server-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-27 05:32:45.525343 acore_server-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7561 2023-06-27 04:12:52.000000 acore_server-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 05:32:45.524895 acore_server-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1001 2023-06-27 05:26:10.000000 acore_server-0.1.1/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 16:01:02.996520 acore_server-0.1.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-27 04:12:52.000000 acore_server-0.1.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2023-06-27 04:12:52.000000 acore_server-0.1.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      320 2023-06-27 04:12:52.000000 acore_server-0.1.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4817 2023-06-27 16:01:02.996395 acore_server-0.1.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3694 2023-06-27 05:07:58.000000 acore_server-0.1.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 16:01:02.994451 acore_server-0.1.2/acore_server/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      393 2023-06-27 04:56:34.000000 acore_server-0.1.2/acore_server/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-27 16:00:31.000000 acore_server-0.1.2/acore_server/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-06-27 04:49:35.000000 acore_server-0.1.2/acore_server/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      107 2023-06-27 04:26:27.000000 acore_server-0.1.2/acore_server/constants.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 16:01:02.995212 acore_server-0.1.2/acore_server/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-27 04:12:52.000000 acore_server-0.1.2/acore_server/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    16460 2023-06-27 15:25:03.000000 acore_server-0.1.2/acore_server/fleet.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      936 2023-06-27 04:26:42.000000 acore_server-0.1.2/acore_server/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 16:01:02.995662 acore_server-0.1.2/acore_server/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-27 04:12:52.000000 acore_server-0.1.2/acore_server/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-27 04:12:52.000000 acore_server-0.1.2/acore_server/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 16:01:02.995974 acore_server-0.1.2/acore_server/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-27 04:12:52.000000 acore_server-0.1.2/acore_server/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-27 04:12:52.000000 acore_server-0.1.2/acore_server/vendor/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3272 2023-06-26 05:55:10.000000 acore_server-0.1.2/acore_server/wserver_infra_exports.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 16:01:02.995093 acore_server-0.1.2/acore_server.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4817 2023-06-27 16:01:02.000000 acore_server-0.1.2/acore_server.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      722 2023-06-27 16:01:02.000000 acore_server-0.1.2/acore_server.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-27 16:01:02.000000 acore_server-0.1.2/acore_server.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      421 2023-06-27 16:01:02.000000 acore_server-0.1.2/acore_server.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       13 2023-06-27 16:01:02.000000 acore_server-0.1.2/acore_server.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1064 2023-06-27 16:00:23.000000 acore_server-0.1.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-27 04:12:52.000000 acore_server-0.1.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-27 04:12:52.000000 acore_server-0.1.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-27 04:12:52.000000 acore_server-0.1.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-27 04:12:52.000000 acore_server-0.1.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      282 2023-06-27 14:29:27.000000 acore_server-0.1.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-27 16:01:02.996560 acore_server-0.1.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7561 2023-06-27 04:12:52.000000 acore_server-0.1.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-27 16:01:02.996114 acore_server-0.1.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1016 2023-06-27 14:01:20.000000 acore_server-0.1.2/tests/test_api.py
```

### Comparing `acore_server-0.1.1/AUTHORS.rst` & `acore_server-0.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server-0.1.1/LICENSE.txt` & `acore_server-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server-0.1.1/PKG-INFO` & `acore_server-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server
-Version: 0.1.1
+Version: 0.1.2
 Summary: AzerothCore World of Warcraft Logic Server Data Model.
 Home-page: https://github.com/MacHu-GWU/acore_server-project
-Download-URL: https://pypi.python.org/pypi/acore_server/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server-0.1.1/README.rst` & `acore_server-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server-0.1.1/acore_server/fleet.py` & `acore_server-0.1.2/acore_server/fleet.py`

 * *Files 13% similar despite different names*

```diff
@@ -118,31 +118,55 @@
     @property
     def server_name(self) -> str:
         """
         Server name, e.g. ``blue``, ``green``.
         """
         return self.id.split("-", 1)[1]
 
-    @property
-    def bootstrap_command(self) -> str:
-        return (
-            "sudo -H -u ubuntu /home/ubuntu/.pyenv/shims/python3.8 -c "
-            '"$(curl -fsSL https://raw.githubusercontent.com/MacHu-GWU/acore_server_bootstrap-project/main/install.py)" '
-            f"--acore_soap_app_version {self.config.acore_soap_app_version} "
-            f"--acore_server_bootstrap_version {self.config.acore_server_bootstrap_version}"
+    def build_bootstrap_command(
+        self,
+        python_version: str = "3.8",
+        acore_soap_app_version: T.Optional[str] = None,
+        acore_server_bootstrap_version: T.Optional[str] = None,
+    ) -> str:
+        cmd = (
+            f"sudo /home/ubuntu/.pyenv/shims/python{python_version} -c "
+            '"$(curl -fsSL https://raw.githubusercontent.com/MacHu-GWU/acore_server_bootstrap-project/main/install.py)"'
         )
+        if acore_soap_app_version:
+            cmd = (
+                cmd + f" --acore_soap_app_version {self.config.acore_soap_app_version}"
+            )
+        if acore_server_bootstrap_version:
+            cmd = (
+                cmd
+                + f" --acore_server_bootstrap_version {self.config.acore_server_bootstrap_version}"
+            )
+        return cmd
 
     def run_ec2(
         self,
         bsm: "BotoSesManager",
         stack_exports: "StackExports",
+        python_version: str = "3.8",
+        acore_soap_app_version: T.Optional[str] = None,
+        acore_server_bootstrap_version: T.Optional[str] = None,
     ):
+        """
+        为服务器创建一台新的 EC2. 注意, 一般先创建 RDS, 等 RDS 已经在运行了, 再创建 EC2.
+        因为 EC2 有一个 bootstrap 的过程, 这个过程中需要跟数据库通信.
+        """
+        bootstrap_command = self.build_bootstrap_command(
+            python_version=python_version,
+            acore_soap_app_version=acore_soap_app_version,
+            acore_server_bootstrap_version=acore_server_bootstrap_version,
+        )
         user_data_lines = [
             "#!/bin/bash",
-            self.bootstrap_command,
+            bootstrap_command,
         ]
         return self.metadata.run_ec2(
             ec2_client=bsm.ec2_client,
             ami_id=self.config.ec2_ami_id,
             instance_type=self.config.ec2_instance_type,
             key_name=self.config.ec2_key_name,
             subnet_id=self.config.ec2_subnet_id,
@@ -157,14 +181,17 @@
         )
 
     def run_rds(
         self,
         bsm: "BotoSesManager",
         stack_exports: "StackExports",
     ):
+        """
+        为服务器创建一台新的数据库.
+        """
         return self.metadata.run_rds(
             rds_client=bsm.rds_client,
             db_snapshot_identifier=self.config.db_snapshot_id,
             db_instance_class=self.config.db_instance_class,
             db_subnet_group_name=stack_exports.get_db_subnet_group_name(),
             security_group_ids=[
                 stack_exports.get_default_sg_id(server_id=self.id),
@@ -173,114 +200,186 @@
             check_exists=False,
         )
 
     def start_ec2(
         self,
         bsm: "BotoSesManager",
     ):
+        """
+        启动关闭着的 EC2.
+        """
         return self.metadata.start_ec2(ec2_client=bsm.ec2_client)
 
     def start_rds(
         self,
         bsm: "BotoSesManager",
     ):
+        """
+        启动关闭着的 RDS.
+        """
         return self.metadata.start_rds(rds_client=bsm.rds_client)
 
     def associate_eip_address(
         self,
         bsm: "BotoSesManager",
     ) -> T.Optional[dict]:
+        """
+        给 EC2 关联 EIP.
+        """
         if self.config.ec2_eip_allocation_id is not None:
             return self.metadata.associate_eip_address(
                 ec2_client=bsm.ec2_client,
                 allocation_id=self.config.ec2_eip_allocation_id,
                 check_exists=True,
             )
         return None
 
     def update_db_master_password(
         self,
         bsm: "BotoSesManager",
     ) -> T.Optional[dict]:
+        """
+        更新数据库的 master password.
+        """
         return self.metadata.update_db_master_password(
             rds_client=bsm.rds_client,
             master_password=self.config.db_admin_password,
             check_exists=False,
         )
 
     def stop_ec2(
         self,
         bsm: "BotoSesManager",
     ):
+        """
+        关闭 EC2.
+        """
         return self.metadata.stop_ec2(bsm.ec2_client)
 
     def stop_rds(
         self,
         bsm: "BotoSesManager",
     ):
+        """
+        关闭 RDS.
+        """
         return self.metadata.stop_rds(bsm.rds_client)
 
     def delete_ec2(
         self,
         bsm: "BotoSesManager",
     ):
+        """
+        删除 EC2.
+        """
         return self.metadata.delete_ec2(bsm.ec2_client)
 
     def delete_rds(
         self,
         bsm: "BotoSesManager",
     ):
+        """
+        删除 RDS.
+        """
         create_final_snapshot = self.env_name == EnvEnum.prd.value
         return self.metadata.delete_rds(
             bsm.rds_client,
             create_final_snapshot=create_final_snapshot,
         )
 
     def bootstrap(
         self,
         bsm: "BotoSesManager",
+        python_version: str = "3.8",
+        acore_soap_app_version: T.Optional[str] = None,
+        acore_server_bootstrap_version: T.Optional[str] = None,
     ):
         """
+        远程执行 EC2 引导程序.
+
         这个命令不会失败. 它只是一个 async API call.
         """
+        bootstrap_command = self.build_bootstrap_command(
+            python_version=python_version,
+            acore_soap_app_version=acore_soap_app_version,
+            acore_server_bootstrap_version=acore_server_bootstrap_version,
+        )
         return ssm_better_boto.send_command(
             ssm_client=bsm.ssm_client,
             instance_id=self.metadata.ec2_inst.id,
             commands=[
-                self.bootstrap_command,
+                bootstrap_command,
+            ],
+        )
+
+    def run_check_server_status_cron_job(
+        self,
+        bsm: "BotoSesManager",
+    ):
+        """
+        启动检测游戏服务器状态的定时任务.
+
+        这个命令不会失败. 它只是一个 async API call.
+        """
+        return ssm_better_boto.send_command(
+            ssm_client=bsm.ssm_client,
+            instance_id=self.metadata.ec2_inst.id,
+            commands=[
+                f"sudo -H -u ubuntu {path_acore_server_bootstrap_cli} run_check_server_status_cron_job",
+            ],
+        )
+
+    def stop_check_server_status_cron_job(
+        self,
+        bsm: "BotoSesManager",
+    ):
+        """
+        停止检测游戏服务器状态的定时任务.
+
+        这个命令不会失败. 它只是一个 async API call.
+        """
+        return ssm_better_boto.send_command(
+            ssm_client=bsm.ssm_client,
+            instance_id=self.metadata.ec2_inst.id,
+            commands=[
+                f"sudo -H -u ubuntu {path_acore_server_bootstrap_cli} stop_check_server_status_cron_job",
             ],
         )
 
     def run_server(
         self,
         bsm: "BotoSesManager",
     ):
         """
+        启动魔兽世界游戏服务器.
+
         这个命令不会失败. 它只是一个 async API call.
         """
         return ssm_better_boto.send_command(
             ssm_client=bsm.ssm_client,
             instance_id=self.metadata.ec2_inst.id,
             commands=[
-                f"{path_acore_server_bootstrap_cli} run_server",
+                f"sudo -H -u ubuntu {path_acore_server_bootstrap_cli} run_server",
             ],
         )
 
     def stop_server(
         self,
         bsm: "BotoSesManager",
     ):
         """
+        停止魔兽世界游戏服务器.
+
         这个命令不会失败. 它只是一个 async API call.
         """
         return ssm_better_boto.send_command(
             ssm_client=bsm.ssm_client,
             instance_id=self.metadata.ec2_inst.id,
             commands=[
-                f"{path_acore_server_bootstrap_cli} stop_server",
+                f"sudo -H -u ubuntu {path_acore_server_bootstrap_cli} stop_server",
             ],
         )
 
     @property
     def wow_status(self) -> str:
         """
         从 EC2 的 Tag 中获取魔兽世界服务器的状态.
@@ -313,15 +412,17 @@
         self,
         path_pem_file=default_path_pem_file,
     ):
         """
         创建一个本地的 SSH Tunnel, 用于本地数据库开发.
         """
         if self.metadata.is_running() is False:
-            raise ConnectionError("cannot create ssh tunnel, EC2 or RDS is not running.")
+            raise ConnectionError(
+                "cannot create ssh tunnel, EC2 or RDS is not running."
+            )
         acore_db_ssh_tunnel.create_ssh_tunnel(
             path_pem_file=path_pem_file,
             db_host=self.metadata.rds_inst.endpoint,
             db_port=DB_PORT,
             jump_host_username=EC2_USERNAME,
             jump_host_public_ip=self.metadata.ec2_inst.public_ip,
         )
```

### Comparing `acore_server-0.1.1/acore_server/paths.py` & `acore_server-0.1.2/acore_server/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server-0.1.1/acore_server/vendor/pytest_cov_helper.py` & `acore_server-0.1.2/acore_server/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server-0.1.1/acore_server/wserver_infra_exports.py` & `acore_server-0.1.2/acore_server/wserver_infra_exports.py`

 * *Files identical despite different names*

### Comparing `acore_server-0.1.1/acore_server.egg-info/PKG-INFO` & `acore_server-0.1.2/acore_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server
-Version: 0.1.1
+Version: 0.1.2
 Summary: AzerothCore World of Warcraft Logic Server Data Model.
 Home-page: https://github.com/MacHu-GWU/acore_server-project
-Download-URL: https://pypi.python.org/pypi/acore_server/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server-0.1.1/acore_server.egg-info/SOURCES.txt` & `acore_server-0.1.2/acore_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server-0.1.1/requirements-doc.txt` & `acore_server-0.1.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server-0.1.1/setup.py` & `acore_server-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server-0.1.1/tests/test_api.py` & `acore_server-0.1.2/tests/test_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,26 +9,26 @@
     _ = api.Fleet
     _ = api.InfraStackExports
 
     _ = api.Server
     _ = api.Server.id
     _ = api.Server.env_name
     _ = api.Server.server_name
-    _ = api.Server.bootstrap_command
     _ = api.Server.run_ec2
     _ = api.Server.run_rds
     _ = api.Server.start_ec2
     _ = api.Server.start_rds
     _ = api.Server.associate_eip_address
     _ = api.Server.update_db_master_password
     _ = api.Server.stop_ec2
     _ = api.Server.stop_rds
     _ = api.Server.delete_ec2
     _ = api.Server.delete_rds
     _ = api.Server.bootstrap
+    _ = api.Server.run_check_server_status_cron_job
     _ = api.Server.run_server
     _ = api.Server.stop_server
     _ = api.Server.wow_status
     _ = api.Server.create_ssh_tunnel
     _ = api.Server.list_ssh_tunnel
     _ = api.Server.test_ssh_tunnel
     _ = api.Server.kill_ssh_tunnel
```

