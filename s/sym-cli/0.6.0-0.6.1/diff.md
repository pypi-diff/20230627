# Comparing `tmp/sym_cli-0.6.0.tar.gz` & `tmp/sym_cli-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym_cli-0.6.0.tar", max compression
+gzip compressed data, was "sym_cli-0.6.1.tar", max compression
```

## Comparing `sym_cli-0.6.0.tar` & `sym_cli-0.6.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0      147 2023-06-27 13:27:51.123022 sym_cli-0.6.0/DESCRIPTION.md
--rw-r--r--   0        0        0     2246 2023-06-27 13:27:53.303039 sym_cli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       60 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/actions/__init__.py
--rw-r--r--   0        0        0     2175 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/actions/action_registry.py
--rw-r--r--   0        0        0     1463 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/actions/ansible_action.py
--rw-r--r--   0        0        0     1614 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/actions/ansible_playbook_action.py
--rw-r--r--   0        0        0     1438 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/actions/ssh_session_action.py
--rw-r--r--   0        0        0     1299 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/actions/sym_action.py
--rw-r--r--   0        0        0     1675 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/actions/write_creds_action.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/ansible/__init__.py
--rw-r--r--   0        0        0    18609 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/ansible/connection/__init__.py
--rw-r--r--   0        0        0    13933 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/ansible/connection/sym_aws_ssm.py
--rw-r--r--   0        0        0       90 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/__init__.py
--rw-r--r--   0        0        0     1897 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/ansible.py
--rw-r--r--   0        0        0     2179 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/ansible_playbook.py
--rw-r--r--   0        0        0      664 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/check.py
--rw-r--r--   0        0        0     2073 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/config.py
--rw-r--r--   0        0        0     1016 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/defaults.py
--rw-r--r--   0        0        0     3503 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/doctor.py
--rw-r--r--   0        0        0      798 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/exec.py
--rw-r--r--   0        0        0     1098 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/host_to_instance.py
--rw-r--r--   0        0        0      683 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/login.py
--rw-r--r--   0        0        0     1040 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/resources.py
--rw-r--r--   0        0        0     7895 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/ssh.py
--rw-r--r--   0        0        0     1224 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/ssh_session.py
--rw-r--r--   0        0        0     1767 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/ssh_tunnel.py
--rw-r--r--   0        0        0      894 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/ssm.py
--rw-r--r--   0        0        0     2750 2023-06-27 13:27:51.131022 sym_cli-0.6.0/sym/cli/commands/sym.py
--rw-r--r--   0        0        0      204 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/commands/version.py
--rw-r--r--   0        0        0     1894 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/commands/write_creds.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/constants/__init__.py
--rw-r--r--   0        0        0      746 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/constants/env.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/data/__init__.py
--rw-r--r--   0        0        0      310 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/data/ansible_options.py
--rw-r--r--   0        0        0     1376 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/data/request_data.py
--rw-r--r--   0        0        0      142 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/data/target_options.py
--rw-r--r--   0        0        0     5000 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/decorators.py
--rw-r--r--   0        0        0     5573 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/errors.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/__init__.py
--rw-r--r--   0        0        0     6376 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/ansible.py
--rw-r--r--   0        0        0     5241 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/boto.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/check/__init__.py
--rw-r--r--   0        0        0     1614 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/check/core.py
--rw-r--r--   0        0        0     1827 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/check/ec2.py
--rw-r--r--   0        0        0     1088 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/check/model.py
--rw-r--r--   0        0        0     1694 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/check/runner.py
--rw-r--r--   0        0        0     2202 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/check/ssh.py
--rw-r--r--   0        0        0     3938 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/config.py
--rw-r--r--   0        0        0      626 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/constants.py
--rw-r--r--   0        0        0     8538 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/doctor.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/ec2/__init__.py
--rw-r--r--   0        0        0     2086 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/ec2/cache.py
--rw-r--r--   0        0        0     7538 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/ec2/client.py
--rw-r--r--   0        0        0      214 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/ec2/factory.py
--rw-r--r--   0        0        0     2867 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/ec2/multiregion.py
--rw-r--r--   0        0        0     3908 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/flags.py
--rw-r--r--   0        0        0      912 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/global_options.py
--rw-r--r--   0        0        0     4865 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/options.py
--rw-r--r--   0        0        0      287 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/org.py
--rw-r--r--   0        0        0    12133 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/params.py
--rw-r--r--   0        0        0      946 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/pty.py
--rw-r--r--   0        0        0    10719 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/ssh.py
--rw-r--r--   0        0        0     1543 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/sym_group.py
--rw-r--r--   0        0        0      812 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/threading.py
--rw-r--r--   0        0        0      262 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/validations.py
--rw-r--r--   0        0        0     1722 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/helpers/version.py
--rw-r--r--   0        0        0       90 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/saml_clients/__init__.py
--rw-r--r--   0        0        0     3578 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/saml_clients/aws_config.py
--rw-r--r--   0        0        0     5733 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/saml_clients/aws_okta.py
--rw-r--r--   0        0        0     2887 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/saml_clients/aws_profile.py
--rw-r--r--   0        0        0     1324 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/saml_clients/chooser.py
--rw-r--r--   0        0        0     6699 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/saml_clients/saml2aws.py
--rw-r--r--   0        0        0     8989 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/saml_clients/saml_client.py
--rw-r--r--   0        0        0     1247 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/saml_clients/saml_client_factory.py
--rw-r--r--   0        0        0      277 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/sym.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/__init__.py
--rw-r--r--   0        0        0     3834 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/commands/conftest.py
--rw-r--r--   0        0        0    10471 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/commands/test_ansible.py
--rw-r--r--   0        0        0      677 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/commands/test_host_to_instance.py
--rw-r--r--   0        0        0     6642 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/commands/test_ssh.py
--rw-r--r--   0        0        0     1685 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/commands/test_ssh_session.py
--rw-r--r--   0        0        0    11563 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/commands/test_write_creds.py
--rw-r--r--   0        0        0     5112 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/decorators/__init__.py
--rw-r--r--   0        0        0      635 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/decorators/test_intercept_error.py
--rw-r--r--   0        0        0      425 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/decorators/test_retry.py
--rw-r--r--   0        0        0     1108 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/decorators/test_setup_sentry.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/helpers/ec2/__init__.py
--rw-r--r--   0        0        0      957 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/helpers/ec2/conftest.py
--rw-r--r--   0        0        0     3642 2023-06-27 13:27:51.135022 sym_cli-0.6.0/sym/cli/tests/helpers/ec2/test_caching.py
--rw-r--r--   0        0        0     6985 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/helpers/ec2/test_client.py
--rw-r--r--   0        0        0     2084 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/helpers/ec2/test_multiregion.py
--rw-r--r--   0        0        0      846 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/helpers/sandbox.py
--rw-r--r--   0        0        0     1702 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/helpers/test_ansible.py
--rw-r--r--   0        0        0     2383 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/helpers/test_boto.py
--rw-r--r--   0        0        0     3087 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/helpers/test_config.py
--rw-r--r--   0        0        0      581 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/helpers/test_has_command.py
--rw-r--r--   0        0        0      563 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/helpers/test_params.py
--rw-r--r--   0        0        0     2786 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/helpers/test_ssh.py
--rw-r--r--   0        0        0     1497 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/integration/conftest.py
--rw-r--r--   0        0        0     2832 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/integration/test_ld.py
--rw-r--r--   0        0        0      944 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/matchers.py
--rw-r--r--   0        0        0        0 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/saml_clients/__init__.py
--rw-r--r--   0        0        0     3953 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/saml_clients/conftest.py
--rw-r--r--   0        0        0     2187 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/saml_clients/test_aws_okta.py
--rw-r--r--   0        0        0     1224 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/saml_clients/test_aws_profile.py
--rw-r--r--   0        0        0     1365 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/saml_clients/test_chooser.py
--rw-r--r--   0        0        0     3722 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/saml_clients/test_saml2aws.py
--rw-r--r--   0        0        0     1333 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/saml_clients/test_saml_client.py
--rw-r--r--   0        0        0     3730 2023-06-27 13:27:51.139022 sym_cli-0.6.0/sym/cli/tests/test_sym.py
--rw-r--r--   0        0        0       22 2023-06-27 13:27:53.359040 sym_cli-0.6.0/sym/cli/version.py
--rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 sym_cli-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      147 2023-06-27 14:14:48.692917 sym_cli-0.6.1/DESCRIPTION.md
+-rw-r--r--   0        0        0     2246 2023-06-27 14:14:50.852937 sym_cli-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/actions/__init__.py
+-rw-r--r--   0        0        0     2175 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/actions/action_registry.py
+-rw-r--r--   0        0        0     1463 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/actions/ansible_action.py
+-rw-r--r--   0        0        0     1614 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/actions/ansible_playbook_action.py
+-rw-r--r--   0        0        0     1438 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/actions/ssh_session_action.py
+-rw-r--r--   0        0        0     1299 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/actions/sym_action.py
+-rw-r--r--   0        0        0     1675 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/actions/write_creds_action.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/ansible/__init__.py
+-rw-r--r--   0        0        0    18609 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/ansible/connection/__init__.py
+-rw-r--r--   0        0        0    13933 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/ansible/connection/sym_aws_ssm.py
+-rw-r--r--   0        0        0       90 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1897 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/ansible.py
+-rw-r--r--   0        0        0     2179 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/ansible_playbook.py
+-rw-r--r--   0        0        0      664 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/check.py
+-rw-r--r--   0        0        0     2073 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/config.py
+-rw-r--r--   0        0        0     1016 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/defaults.py
+-rw-r--r--   0        0        0     3503 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/doctor.py
+-rw-r--r--   0        0        0      798 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/exec.py
+-rw-r--r--   0        0        0     1098 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/host_to_instance.py
+-rw-r--r--   0        0        0      683 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/login.py
+-rw-r--r--   0        0        0     1040 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/resources.py
+-rw-r--r--   0        0        0     7895 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/ssh.py
+-rw-r--r--   0        0        0     1224 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/ssh_session.py
+-rw-r--r--   0        0        0     1767 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/ssh_tunnel.py
+-rw-r--r--   0        0        0      894 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/ssm.py
+-rw-r--r--   0        0        0     2750 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/sym.py
+-rw-r--r--   0        0        0      204 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/version.py
+-rw-r--r--   0        0        0     1894 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/commands/write_creds.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/constants/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/constants/env.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/data/__init__.py
+-rw-r--r--   0        0        0      310 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/data/ansible_options.py
+-rw-r--r--   0        0        0     1376 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/data/request_data.py
+-rw-r--r--   0        0        0      142 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/data/target_options.py
+-rw-r--r--   0        0        0     5000 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/decorators.py
+-rw-r--r--   0        0        0     5573 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/errors.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     6376 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/ansible.py
+-rw-r--r--   0        0        0     5241 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/boto.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/check/__init__.py
+-rw-r--r--   0        0        0     1614 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/check/core.py
+-rw-r--r--   0        0        0     1827 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/check/ec2.py
+-rw-r--r--   0        0        0     1088 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/check/model.py
+-rw-r--r--   0        0        0     1694 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/check/runner.py
+-rw-r--r--   0        0        0     2202 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/check/ssh.py
+-rw-r--r--   0        0        0     3938 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/config.py
+-rw-r--r--   0        0        0      626 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/constants.py
+-rw-r--r--   0        0        0     8538 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/doctor.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/ec2/__init__.py
+-rw-r--r--   0        0        0     2086 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/ec2/cache.py
+-rw-r--r--   0        0        0     7538 2023-06-27 14:14:48.700917 sym_cli-0.6.1/sym/cli/helpers/ec2/client.py
+-rw-r--r--   0        0        0      214 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/ec2/factory.py
+-rw-r--r--   0        0        0     2867 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/ec2/multiregion.py
+-rw-r--r--   0        0        0     3908 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/flags.py
+-rw-r--r--   0        0        0      912 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/global_options.py
+-rw-r--r--   0        0        0     4865 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/options.py
+-rw-r--r--   0        0        0      287 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/org.py
+-rw-r--r--   0        0        0    12133 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/params.py
+-rw-r--r--   0        0        0      946 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/pty.py
+-rw-r--r--   0        0        0    10719 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/ssh.py
+-rw-r--r--   0        0        0     1543 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/sym_group.py
+-rw-r--r--   0        0        0      812 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/threading.py
+-rw-r--r--   0        0        0      262 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/validations.py
+-rw-r--r--   0        0        0     1722 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/helpers/version.py
+-rw-r--r--   0        0        0       90 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/saml_clients/__init__.py
+-rw-r--r--   0        0        0     3578 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/saml_clients/aws_config.py
+-rw-r--r--   0        0        0     5733 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/saml_clients/aws_okta.py
+-rw-r--r--   0        0        0     2887 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/saml_clients/aws_profile.py
+-rw-r--r--   0        0        0     1328 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/saml_clients/chooser.py
+-rw-r--r--   0        0        0     6699 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/saml_clients/saml2aws.py
+-rw-r--r--   0        0        0     8989 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/saml_clients/saml_client.py
+-rw-r--r--   0        0        0     1247 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/saml_clients/saml_client_factory.py
+-rw-r--r--   0        0        0      277 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/sym.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/__init__.py
+-rw-r--r--   0        0        0     3834 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/commands/conftest.py
+-rw-r--r--   0        0        0    10471 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/commands/test_ansible.py
+-rw-r--r--   0        0        0      677 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/commands/test_host_to_instance.py
+-rw-r--r--   0        0        0     6642 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/commands/test_ssh.py
+-rw-r--r--   0        0        0     1685 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/commands/test_ssh_session.py
+-rw-r--r--   0        0        0    11563 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/commands/test_write_creds.py
+-rw-r--r--   0        0        0     5112 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/decorators/__init__.py
+-rw-r--r--   0        0        0      635 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/decorators/test_intercept_error.py
+-rw-r--r--   0        0        0      425 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/decorators/test_retry.py
+-rw-r--r--   0        0        0     1108 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/decorators/test_setup_sentry.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/ec2/__init__.py
+-rw-r--r--   0        0        0      957 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/ec2/conftest.py
+-rw-r--r--   0        0        0     3642 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/ec2/test_caching.py
+-rw-r--r--   0        0        0     6985 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/ec2/test_client.py
+-rw-r--r--   0        0        0     2084 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/ec2/test_multiregion.py
+-rw-r--r--   0        0        0      846 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/sandbox.py
+-rw-r--r--   0        0        0     1702 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/test_ansible.py
+-rw-r--r--   0        0        0     2383 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/test_boto.py
+-rw-r--r--   0        0        0     3087 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/test_config.py
+-rw-r--r--   0        0        0      581 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/test_has_command.py
+-rw-r--r--   0        0        0      563 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/test_params.py
+-rw-r--r--   0        0        0     2786 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/helpers/test_ssh.py
+-rw-r--r--   0        0        0     1497 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2832 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/integration/test_ld.py
+-rw-r--r--   0        0        0      944 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/matchers.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/saml_clients/__init__.py
+-rw-r--r--   0        0        0     3953 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/saml_clients/conftest.py
+-rw-r--r--   0        0        0     2187 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/saml_clients/test_aws_okta.py
+-rw-r--r--   0        0        0     1224 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/saml_clients/test_aws_profile.py
+-rw-r--r--   0        0        0     1365 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/saml_clients/test_chooser.py
+-rw-r--r--   0        0        0     3722 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/saml_clients/test_saml2aws.py
+-rw-r--r--   0        0        0     1333 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/saml_clients/test_saml_client.py
+-rw-r--r--   0        0        0     3730 2023-06-27 14:14:48.704917 sym_cli-0.6.1/sym/cli/tests/test_sym.py
+-rw-r--r--   0        0        0       22 2023-06-27 14:14:50.900937 sym_cli-0.6.1/sym/cli/version.py
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 sym_cli-0.6.1/PKG-INFO
```

### Comparing `sym_cli-0.6.0/pyproject.toml` & `sym_cli-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sym-cli"
-version = "0.6.0"
+version = "0.6.1"
 description = "Sym's Official CLI for Users"
 authors = ["SymOps, Inc. <pypi@symops.io>"]
 packages = [{ include = "sym/*" }]
 readme = "DESCRIPTION.md"
 homepage = "https://symops.com/"
 documentation = "https://docs.symops.com/docs/install-sym-cli"
 classifiers = [
```

### Comparing `sym_cli-0.6.0/sym/cli/actions/action_registry.py` & `sym_cli-0.6.1/sym/cli/actions/action_registry.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/actions/ansible_action.py` & `sym_cli-0.6.1/sym/cli/actions/ansible_action.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/actions/ansible_playbook_action.py` & `sym_cli-0.6.1/sym/cli/actions/ansible_playbook_action.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/actions/ssh_session_action.py` & `sym_cli-0.6.1/sym/cli/actions/ssh_session_action.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/actions/sym_action.py` & `sym_cli-0.6.1/sym/cli/actions/sym_action.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/actions/write_creds_action.py` & `sym_cli-0.6.1/sym/cli/actions/write_creds_action.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/ansible/connection/__init__.py` & `sym_cli-0.6.1/sym/cli/ansible/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/ansible/connection/sym_aws_ssm.py` & `sym_cli-0.6.1/sym/cli/ansible/connection/sym_aws_ssm.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/ansible.py` & `sym_cli-0.6.1/sym/cli/commands/ansible.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/ansible_playbook.py` & `sym_cli-0.6.1/sym/cli/commands/ansible_playbook.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/check.py` & `sym_cli-0.6.1/sym/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/config.py` & `sym_cli-0.6.1/sym/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/defaults.py` & `sym_cli-0.6.1/sym/cli/commands/defaults.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/doctor.py` & `sym_cli-0.6.1/sym/cli/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/exec.py` & `sym_cli-0.6.1/sym/cli/commands/exec.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/host_to_instance.py` & `sym_cli-0.6.1/sym/cli/commands/host_to_instance.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/login.py` & `sym_cli-0.6.1/sym/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/resources.py` & `sym_cli-0.6.1/sym/cli/commands/resources.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/ssh.py` & `sym_cli-0.6.1/sym/cli/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/ssh_session.py` & `sym_cli-0.6.1/sym/cli/commands/ssh_session.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/ssh_tunnel.py` & `sym_cli-0.6.1/sym/cli/commands/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/ssm.py` & `sym_cli-0.6.1/sym/cli/commands/ssm.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/sym.py` & `sym_cli-0.6.1/sym/cli/commands/sym.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/commands/write_creds.py` & `sym_cli-0.6.1/sym/cli/commands/write_creds.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/constants/env.py` & `sym_cli-0.6.1/sym/cli/constants/env.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/data/request_data.py` & `sym_cli-0.6.1/sym/cli/data/request_data.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/decorators.py` & `sym_cli-0.6.1/sym/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/errors.py` & `sym_cli-0.6.1/sym/cli/errors.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/ansible.py` & `sym_cli-0.6.1/sym/cli/helpers/ansible.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/boto.py` & `sym_cli-0.6.1/sym/cli/helpers/boto.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/check/core.py` & `sym_cli-0.6.1/sym/cli/helpers/check/core.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/check/ec2.py` & `sym_cli-0.6.1/sym/cli/helpers/check/ec2.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/check/model.py` & `sym_cli-0.6.1/sym/cli/helpers/check/model.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/check/runner.py` & `sym_cli-0.6.1/sym/cli/helpers/check/runner.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/check/ssh.py` & `sym_cli-0.6.1/sym/cli/helpers/check/ssh.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/config.py` & `sym_cli-0.6.1/sym/cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/constants.py` & `sym_cli-0.6.1/sym/cli/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/doctor.py` & `sym_cli-0.6.1/sym/cli/helpers/doctor.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/ec2/cache.py` & `sym_cli-0.6.1/sym/cli/helpers/ec2/cache.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/ec2/client.py` & `sym_cli-0.6.1/sym/cli/helpers/ec2/client.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/ec2/multiregion.py` & `sym_cli-0.6.1/sym/cli/helpers/ec2/multiregion.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/flags.py` & `sym_cli-0.6.1/sym/cli/helpers/flags.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/global_options.py` & `sym_cli-0.6.1/sym/cli/helpers/global_options.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/options.py` & `sym_cli-0.6.1/sym/cli/helpers/options.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/params.py` & `sym_cli-0.6.1/sym/cli/helpers/params.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/pty.py` & `sym_cli-0.6.1/sym/cli/helpers/pty.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/ssh.py` & `sym_cli-0.6.1/sym/cli/helpers/ssh.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/sym_group.py` & `sym_cli-0.6.1/sym/cli/helpers/sym_group.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/threading.py` & `sym_cli-0.6.1/sym/cli/helpers/threading.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/helpers/version.py` & `sym_cli-0.6.1/sym/cli/helpers/version.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/saml_clients/aws_config.py` & `sym_cli-0.6.1/sym/cli/saml_clients/aws_config.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/saml_clients/aws_okta.py` & `sym_cli-0.6.1/sym/cli/saml_clients/aws_okta.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/saml_clients/aws_profile.py` & `sym_cli-0.6.1/sym/cli/saml_clients/aws_profile.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/saml_clients/chooser.py` & `sym_cli-0.6.1/sym/cli/saml_clients/chooser.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 @requires_all_imports(import_all)
 def choose_saml_client(
     saml_client_name: SAMLClientName, none_ok=False
 ) -> Optional[Type[SAMLClient]]:
     if saml_client_name == "auto":
         excludes = AUTO_EXCLUDED_SAML_CLIENT_NAMES
-        if Config.is_logged_in() and is_sso_enabled():
+        if Config.is_logged_in() and not is_sso_enabled():
             excludes.append("aws-config")
         for client in SAMLClient.sorted_subclasses():
             if client.option_value not in excludes and has_command(client.binary):
                 return client
     else:
         for client in SAMLClient.sorted_subclasses():
             if client.option_value == saml_client_name:
```

### Comparing `sym_cli-0.6.0/sym/cli/saml_clients/saml2aws.py` & `sym_cli-0.6.1/sym/cli/saml_clients/saml2aws.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/saml_clients/saml_client.py` & `sym_cli-0.6.1/sym/cli/saml_clients/saml_client.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/saml_clients/saml_client_factory.py` & `sym_cli-0.6.1/sym/cli/saml_clients/saml_client_factory.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/commands/conftest.py` & `sym_cli-0.6.1/sym/cli/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/commands/test_ansible.py` & `sym_cli-0.6.1/sym/cli/tests/commands/test_ansible.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/commands/test_host_to_instance.py` & `sym_cli-0.6.1/sym/cli/tests/commands/test_host_to_instance.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/commands/test_ssh.py` & `sym_cli-0.6.1/sym/cli/tests/commands/test_ssh.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/commands/test_ssh_session.py` & `sym_cli-0.6.1/sym/cli/tests/commands/test_ssh_session.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/commands/test_write_creds.py` & `sym_cli-0.6.1/sym/cli/tests/commands/test_write_creds.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/conftest.py` & `sym_cli-0.6.1/sym/cli/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/decorators/test_intercept_error.py` & `sym_cli-0.6.1/sym/cli/tests/decorators/test_intercept_error.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/decorators/test_setup_sentry.py` & `sym_cli-0.6.1/sym/cli/tests/decorators/test_setup_sentry.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/ec2/conftest.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/ec2/conftest.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/ec2/test_caching.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/ec2/test_caching.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/ec2/test_client.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/ec2/test_client.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/ec2/test_multiregion.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/ec2/test_multiregion.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/sandbox.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/sandbox.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/test_ansible.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/test_ansible.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/test_boto.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/test_boto.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/test_config.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/test_config.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/test_has_command.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/test_has_command.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/test_params.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/test_params.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/helpers/test_ssh.py` & `sym_cli-0.6.1/sym/cli/tests/helpers/test_ssh.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/integration/conftest.py` & `sym_cli-0.6.1/sym/cli/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/integration/test_ld.py` & `sym_cli-0.6.1/sym/cli/tests/integration/test_ld.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/matchers.py` & `sym_cli-0.6.1/sym/cli/tests/matchers.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/saml_clients/conftest.py` & `sym_cli-0.6.1/sym/cli/tests/saml_clients/conftest.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/saml_clients/test_aws_okta.py` & `sym_cli-0.6.1/sym/cli/tests/saml_clients/test_aws_okta.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/saml_clients/test_aws_profile.py` & `sym_cli-0.6.1/sym/cli/tests/saml_clients/test_aws_profile.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/saml_clients/test_chooser.py` & `sym_cli-0.6.1/sym/cli/tests/saml_clients/test_chooser.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/saml_clients/test_saml2aws.py` & `sym_cli-0.6.1/sym/cli/tests/saml_clients/test_saml2aws.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/saml_clients/test_saml_client.py` & `sym_cli-0.6.1/sym/cli/tests/saml_clients/test_saml_client.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/sym/cli/tests/test_sym.py` & `sym_cli-0.6.1/sym/cli/tests/test_sym.py`

 * *Files identical despite different names*

### Comparing `sym_cli-0.6.0/PKG-INFO` & `sym_cli-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sym-cli
-Version: 0.6.0
+Version: 0.6.1
 Summary: Sym's Official CLI for Users
 Home-page: https://symops.com/
 Author: SymOps, Inc.
 Author-email: pypi@symops.io
 Requires-Python: >=3.8,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

