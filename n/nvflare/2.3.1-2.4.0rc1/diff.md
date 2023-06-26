# Comparing `tmp/nvflare-2.3.1-py3-none-any.whl.zip` & `tmp/nvflare-2.4.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,64 +1,68 @@
-Zip file size: 859355 bytes, number of entries: 507
+Zip file size: 951159 bytes, number of entries: 559
 -rw-rw-r--  2.0 unx      764 b- defN 23-May-30 23:31 nvflare/__init__.py
--rw-rw-r--  2.0 unx      497 b- defN 23-Jun-26 22:46 nvflare/_version.py
+-rw-rw-r--  2.0 unx      500 b- defN 23-Jun-26 22:54 nvflare/_version.py
 -rw-rw-r--  2.0 unx     4979 b- defN 23-May-30 23:31 nvflare/cli.py
 -rw-rw-r--  2.0 unx      652 b- defN 23-May-30 23:31 nvflare/cli_exception.py
--rw-rw-r--  2.0 unx     8219 b- defN 23-Jun-26 22:46 nvflare/poc.zip
+-rw-rw-r--  2.0 unx     8219 b- defN 23-Jun-26 22:54 nvflare/poc.zip
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/apis/__init__.py
--rw-rw-r--  2.0 unx     7512 b- defN 23-Jun-26 22:45 nvflare/apis/analytix.py
+-rw-rw-r--  2.0 unx     7730 b- defN 23-Jun-26 22:53 nvflare/apis/analytix.py
+-rw-rw-r--  2.0 unx      923 b- defN 23-Jun-26 22:53 nvflare/apis/app_deployer_spec.py
 -rw-rw-r--  2.0 unx     1323 b- defN 23-May-30 23:31 nvflare/apis/app_validation.py
 -rw-rw-r--  2.0 unx     1660 b- defN 23-May-30 23:31 nvflare/apis/aux_spec.py
 -rw-rw-r--  2.0 unx     1311 b- defN 23-May-30 23:31 nvflare/apis/client.py
 -rw-rw-r--  2.0 unx     1047 b- defN 23-May-30 23:31 nvflare/apis/client_engine_spec.py
--rw-rw-r--  2.0 unx    19130 b- defN 23-Jun-26 22:45 nvflare/apis/controller_spec.py
--rw-rw-r--  2.0 unx     5500 b- defN 23-Jun-26 22:45 nvflare/apis/dxo.py
+-rw-rw-r--  2.0 unx    20102 b- defN 23-Jun-26 22:53 nvflare/apis/controller_spec.py
+-rw-rw-r--  2.0 unx     7023 b- defN 23-Jun-26 22:53 nvflare/apis/dxo.py
 -rw-rw-r--  2.0 unx     5451 b- defN 23-May-30 23:31 nvflare/apis/dxo_filter.py
 -rw-rw-r--  2.0 unx     1028 b- defN 23-May-30 23:31 nvflare/apis/engine_spec.py
 -rw-rw-r--  2.0 unx     2571 b- defN 23-May-30 23:31 nvflare/apis/event_type.py
 -rw-rw-r--  2.0 unx     1791 b- defN 23-Jun-26 22:45 nvflare/apis/executor.py
--rw-rw-r--  2.0 unx     1773 b- defN 23-Jun-26 22:45 nvflare/apis/filter.py
+-rw-rw-r--  2.0 unx     1777 b- defN 23-Jun-26 22:53 nvflare/apis/filter.py
 -rw-rw-r--  2.0 unx     9586 b- defN 23-May-30 23:31 nvflare/apis/fl_component.py
--rw-rw-r--  2.0 unx    10610 b- defN 23-Jun-26 22:45 nvflare/apis/fl_constant.py
+-rw-rw-r--  2.0 unx    11020 b- defN 23-Jun-26 22:53 nvflare/apis/fl_constant.py
 -rw-rw-r--  2.0 unx    12075 b- defN 23-Jun-26 22:45 nvflare/apis/fl_context.py
 -rw-rw-r--  2.0 unx     1216 b- defN 23-Jun-26 22:45 nvflare/apis/fl_exception.py
 -rw-rw-r--  2.0 unx     2720 b- defN 23-May-30 23:31 nvflare/apis/fl_snapshot.py
--rw-rw-r--  2.0 unx     6149 b- defN 23-Jun-26 22:45 nvflare/apis/job_def.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-26 22:53 nvflare/apis/job_def.py
 -rw-rw-r--  2.0 unx     6626 b- defN 23-May-30 23:31 nvflare/apis/job_def_manager_spec.py
+-rw-rw-r--  2.0 unx     1039 b- defN 23-Jun-26 22:53 nvflare/apis/job_meta_validator_spec.py
 -rw-rw-r--  2.0 unx     2138 b- defN 23-May-30 23:31 nvflare/apis/job_scheduler_spec.py
+-rw-rw-r--  2.0 unx     1364 b- defN 23-Jun-26 22:53 nvflare/apis/operator_spec.py
 -rw-rw-r--  2.0 unx     2083 b- defN 23-May-30 23:31 nvflare/apis/overseer_spec.py
 -rw-rw-r--  2.0 unx     1151 b- defN 23-May-30 23:31 nvflare/apis/persistable.py
 -rw-rw-r--  2.0 unx     2894 b- defN 23-May-30 23:31 nvflare/apis/resource_manager_spec.py
 -rw-rw-r--  2.0 unx     3297 b- defN 23-May-30 23:31 nvflare/apis/responder.py
 -rw-rw-r--  2.0 unx     6094 b- defN 23-May-30 23:31 nvflare/apis/server_engine_spec.py
--rw-rw-r--  2.0 unx     4877 b- defN 23-Jun-26 22:45 nvflare/apis/shareable.py
+-rw-rw-r--  2.0 unx     4917 b- defN 23-Jun-26 22:53 nvflare/apis/shareable.py
 -rw-rw-r--  2.0 unx     1322 b- defN 23-May-30 23:31 nvflare/apis/signal.py
 -rw-rw-r--  2.0 unx     1708 b- defN 23-May-30 23:31 nvflare/apis/state_persistor.py
 -rw-rw-r--  2.0 unx     4119 b- defN 23-May-30 23:31 nvflare/apis/storage.py
--rw-rw-r--  2.0 unx     6467 b- defN 23-Jun-26 22:45 nvflare/apis/workspace.py
+-rw-rw-r--  2.0 unx     7331 b- defN 23-Jun-26 22:53 nvflare/apis/workspace.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/apis/impl/__init__.py
 -rw-rw-r--  2.0 unx     6797 b- defN 23-May-30 23:31 nvflare/apis/impl/any_relay_manager.py
 -rw-rw-r--  2.0 unx     5194 b- defN 23-May-30 23:31 nvflare/apis/impl/bcast_manager.py
--rw-rw-r--  2.0 unx    45931 b- defN 23-Jun-26 22:45 nvflare/apis/impl/controller.py
--rw-rw-r--  2.0 unx    11058 b- defN 23-Jun-26 22:45 nvflare/apis/impl/job_def_manager.py
+-rw-rw-r--  2.0 unx    46175 b- defN 23-Jun-26 22:53 nvflare/apis/impl/controller.py
+-rw-rw-r--  2.0 unx    11259 b- defN 23-Jun-26 22:53 nvflare/apis/impl/job_def_manager.py
 -rw-rw-r--  2.0 unx     4727 b- defN 23-May-30 23:31 nvflare/apis/impl/send_manager.py
 -rw-rw-r--  2.0 unx     9653 b- defN 23-May-30 23:31 nvflare/apis/impl/seq_relay_manager.py
 -rw-rw-r--  2.0 unx     3787 b- defN 23-May-30 23:31 nvflare/apis/impl/task_manager.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/apis/utils/__init__.py
--rw-rw-r--  2.0 unx     3579 b- defN 23-Jun-26 22:45 nvflare/apis/utils/fl_context_utils.py
+-rw-rw-r--  2.0 unx     3583 b- defN 23-Jun-26 22:53 nvflare/apis/utils/fl_context_utils.py
 -rw-rw-r--  2.0 unx     2613 b- defN 23-May-30 23:31 nvflare/apis/utils/format_check.py
--rw-rw-r--  2.0 unx     3233 b- defN 23-Jun-26 22:45 nvflare/apis/utils/job_utils.py
+-rw-rw-r--  2.0 unx     3654 b- defN 23-Jun-26 22:53 nvflare/apis/utils/job_utils.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/apis/utils/decomposers/__init__.py
 -rw-rw-r--  2.0 unx     2370 b- defN 23-May-30 23:31 nvflare/apis/utils/decomposers/flare_decomposers.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/__init__.py
 -rw-rw-r--  2.0 unx     6349 b- defN 23-May-30 23:31 nvflare/app_common/app_constant.py
 -rw-rw-r--  2.0 unx     2844 b- defN 23-May-30 23:31 nvflare/app_common/app_event_type.py
 -rw-rw-r--  2.0 unx     1115 b- defN 23-May-30 23:31 nvflare/app_common/model_desc.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/abstract/__init__.py
--rw-rw-r--  2.0 unx     1463 b- defN 23-Jun-26 22:45 nvflare/app_common/abstract/aggregator.py
+-rw-rw-r--  2.0 unx     1648 b- defN 23-Jun-26 22:53 nvflare/app_common/abstract/aggregator.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-26 22:53 nvflare/app_common/abstract/fl_model.py
 -rw-rw-r--  2.0 unx     1043 b- defN 23-May-30 23:31 nvflare/app_common/abstract/formatter.py
 -rw-rw-r--  2.0 unx     1166 b- defN 23-May-30 23:31 nvflare/app_common/abstract/init_final_component.py
 -rw-rw-r--  2.0 unx     1238 b- defN 23-May-30 23:31 nvflare/app_common/abstract/learnable.py
 -rw-rw-r--  2.0 unx     1335 b- defN 23-May-30 23:31 nvflare/app_common/abstract/learnable_persistor.py
 -rw-rw-r--  2.0 unx     3239 b- defN 23-May-30 23:31 nvflare/app_common/abstract/learner_spec.py
 -rw-rw-r--  2.0 unx     2288 b- defN 23-May-30 23:31 nvflare/app_common/abstract/model.py
 -rw-rw-r--  2.0 unx     1361 b- defN 23-May-30 23:31 nvflare/app_common/abstract/model_locator.py
@@ -67,53 +71,58 @@
 -rw-rw-r--  2.0 unx     2239 b- defN 23-May-30 23:31 nvflare/app_common/abstract/persistor_filter.py
 -rw-rw-r--  2.0 unx     2500 b- defN 23-May-30 23:31 nvflare/app_common/abstract/response_processor.py
 -rw-rw-r--  2.0 unx     1533 b- defN 23-May-30 23:31 nvflare/app_common/abstract/shareable_generator.py
 -rw-rw-r--  2.0 unx    11465 b- defN 23-May-30 23:31 nvflare/app_common/abstract/statistics_spec.py
 -rw-rw-r--  2.0 unx     1192 b- defN 23-May-30 23:31 nvflare/app_common/abstract/statistics_writer.py
 -rw-rw-r--  2.0 unx     2652 b- defN 23-May-30 23:31 nvflare/app_common/abstract/task_handler.py
 -rw-rw-r--  2.0 unx      846 b- defN 23-May-30 23:31 nvflare/app_common/aggregators/__init__.py
--rw-rw-r--  2.0 unx     1002 b- defN 23-Jun-26 22:45 nvflare/app_common/aggregators/accumulate_model_aggregator.py
--rw-rw-r--  2.0 unx     2465 b- defN 23-Jun-26 22:45 nvflare/app_common/aggregators/assembler.py
--rw-rw-r--  2.0 unx     4927 b- defN 23-Jun-26 22:45 nvflare/app_common/aggregators/collect_and_assemble_aggregator.py
--rw-rw-r--  2.0 unx     8443 b- defN 23-Jun-26 22:45 nvflare/app_common/aggregators/dxo_aggregator.py
--rw-rw-r--  2.0 unx    11460 b- defN 23-Jun-26 22:45 nvflare/app_common/aggregators/intime_accumulate_model_aggregator.py
+-rw-rw-r--  2.0 unx      894 b- defN 23-Jun-26 22:53 nvflare/app_common/aggregators/accumulate_model_aggregator.py
+-rw-rw-r--  2.0 unx     2513 b- defN 23-Jun-26 22:53 nvflare/app_common/aggregators/assembler.py
+-rw-rw-r--  2.0 unx     4822 b- defN 23-Jun-26 22:53 nvflare/app_common/aggregators/collect_and_assemble_aggregator.py
+-rw-rw-r--  2.0 unx     8500 b- defN 23-Jun-26 22:53 nvflare/app_common/aggregators/dxo_aggregator.py
+-rw-rw-r--  2.0 unx     1699 b- defN 23-Jun-26 22:53 nvflare/app_common/aggregators/dxo_collector.py
+-rw-rw-r--  2.0 unx    11464 b- defN 23-Jun-26 22:53 nvflare/app_common/aggregators/intime_accumulate_model_aggregator.py
 -rw-rw-r--  2.0 unx     3436 b- defN 23-May-30 23:31 nvflare/app_common/aggregators/weighted_aggregation_helper.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/decomposers/__init__.py
--rw-rw-r--  2.0 unx     3011 b- defN 23-Jun-26 22:45 nvflare/app_common/decomposers/common_decomposers.py
+-rw-rw-r--  2.0 unx     3828 b- defN 23-Jun-26 22:53 nvflare/app_common/decomposers/common_decomposers.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/executors/__init__.py
--rw-rw-r--  2.0 unx     4204 b- defN 23-Jun-26 22:45 nvflare/app_common/executors/error_handling_executor.py
+-rw-rw-r--  2.0 unx     4208 b- defN 23-Jun-26 22:53 nvflare/app_common/executors/error_handling_executor.py
 -rw-rw-r--  2.0 unx     6755 b- defN 23-Jun-26 22:45 nvflare/app_common/executors/learner_executor.py
--rw-rw-r--  2.0 unx    13807 b- defN 23-Jun-26 22:45 nvflare/app_common/executors/multi_process_executor.py
+-rw-rw-r--  2.0 unx    13819 b- defN 23-Jun-26 22:53 nvflare/app_common/executors/multi_process_executor.py
 -rw-rw-r--  2.0 unx     4433 b- defN 23-May-30 23:31 nvflare/app_common/executors/splitnn_learner_executor.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/executors/statistics/__init__.py
 -rw-rw-r--  2.0 unx     1792 b- defN 23-May-30 23:31 nvflare/app_common/executors/statistics/statistics_executor.py
--rw-rw-r--  2.0 unx      666 b- defN 23-Jun-26 22:45 nvflare/app_common/executors/statistics/statistics_executor_exception.py
--rw-rw-r--  2.0 unx    13518 b- defN 23-Jun-26 22:45 nvflare/app_common/executors/statistics/statistics_task_handler.py
+-rw-rw-r--  2.0 unx      670 b- defN 23-Jun-26 22:53 nvflare/app_common/executors/statistics/statistics_executor_exception.py
+-rw-rw-r--  2.0 unx    13522 b- defN 23-Jun-26 22:53 nvflare/app_common/executors/statistics/statistics_task_handler.py
 -rw-rw-r--  2.0 unx      797 b- defN 23-May-30 23:31 nvflare/app_common/filters/__init__.py
 -rw-rw-r--  2.0 unx     4441 b- defN 23-May-30 23:31 nvflare/app_common/filters/convert_weights.py
 -rw-rw-r--  2.0 unx     2567 b- defN 23-May-30 23:31 nvflare/app_common/filters/dxo_blocker.py
 -rw-rw-r--  2.0 unx     4804 b- defN 23-May-30 23:31 nvflare/app_common/filters/exclude_vars.py
 -rw-rw-r--  2.0 unx     3902 b- defN 23-May-30 23:31 nvflare/app_common/filters/percentile_privacy.py
 -rw-rw-r--  2.0 unx     3309 b- defN 23-May-30 23:31 nvflare/app_common/filters/statistics_privacy_filter.py
 -rw-rw-r--  2.0 unx     5584 b- defN 23-May-30 23:31 nvflare/app_common/filters/svt_privacy.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/homomorphic_encryption/__init__.py
 -rw-rw-r--  2.0 unx      928 b- defN 23-May-30 23:31 nvflare/app_common/homomorphic_encryption/he_intime_accumulate_model_aggregator.py
 -rw-rw-r--  2.0 unx      870 b- defN 23-May-30 23:31 nvflare/app_common/homomorphic_encryption/he_model_decryptor.py
 -rw-rw-r--  2.0 unx      870 b- defN 23-May-30 23:31 nvflare/app_common/homomorphic_encryption/he_model_encryptor.py
 -rw-rw-r--  2.0 unx      899 b- defN 23-May-30 23:31 nvflare/app_common/homomorphic_encryption/he_model_shareable_generator.py
 -rw-rw-r--  2.0 unx      889 b- defN 23-May-30 23:31 nvflare/app_common/homomorphic_encryption/he_pt_model_reader_writer.py
 -rw-rw-r--  2.0 unx      921 b- defN 23-May-30 23:31 nvflare/app_common/homomorphic_encryption/homomorphic_encrypt.py
+-rw-rw-r--  2.0 unx      610 b- defN 23-Jun-26 22:53 nvflare/app_common/hub/__init__.py
+-rw-rw-r--  2.0 unx     8229 b- defN 23-Jun-26 22:53 nvflare/app_common/hub/hub_app_deployer.py
+-rw-rw-r--  2.0 unx    20787 b- defN 23-Jun-26 22:53 nvflare/app_common/hub/hub_controller.py
+-rw-rw-r--  2.0 unx     6504 b- defN 23-Jun-26 22:53 nvflare/app_common/hub/hub_executor.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/job_schedulers/__init__.py
 -rw-rw-r--  2.0 unx    15917 b- defN 23-May-30 23:31 nvflare/app_common/job_schedulers/job_scheduler.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/np/__init__.py
 -rw-rw-r--  2.0 unx      659 b- defN 23-May-30 23:31 nvflare/app_common/np/constants.py
 -rw-rw-r--  2.0 unx     2584 b- defN 23-May-30 23:31 nvflare/app_common/np/np_formatter.py
 -rw-rw-r--  2.0 unx     3262 b- defN 23-May-30 23:31 nvflare/app_common/np/np_model_locator.py
 -rw-rw-r--  2.0 unx     3058 b- defN 23-May-30 23:31 nvflare/app_common/np/np_model_persistor.py
--rw-rw-r--  2.0 unx     8593 b- defN 23-Jun-26 22:45 nvflare/app_common/np/np_trainer.py
+-rw-rw-r--  2.0 unx     8597 b- defN 23-Jun-26 22:53 nvflare/app_common/np/np_trainer.py
 -rw-rw-r--  2.0 unx     5499 b- defN 23-May-30 23:31 nvflare/app_common/np/np_validator.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/psi/__init__.py
 -rw-rw-r--  2.0 unx     2452 b- defN 23-May-30 23:31 nvflare/app_common/psi/file_psi_writer.py
 -rw-rw-r--  2.0 unx     2847 b- defN 23-May-30 23:31 nvflare/app_common/psi/psi_controller.py
 -rw-rw-r--  2.0 unx     1906 b- defN 23-May-30 23:31 nvflare/app_common/psi/psi_executor.py
 -rw-rw-r--  2.0 unx     2883 b- defN 23-May-30 23:31 nvflare/app_common/psi/psi_spec.py
 -rw-rw-r--  2.0 unx     1223 b- defN 23-May-30 23:31 nvflare/app_common/psi/psi_workflow_spec.py
@@ -127,24 +136,24 @@
 -rw-rw-r--  2.0 unx      858 b- defN 23-May-30 23:31 nvflare/app_common/pt/pt_fedopt.py
 -rw-rw-r--  2.0 unx      859 b- defN 23-May-30 23:31 nvflare/app_common/pt/pt_fedproxloss.py
 -rw-rw-r--  2.0 unx      878 b- defN 23-May-30 23:31 nvflare/app_common/pt/pt_file_model_locator.py
 -rw-rw-r--  2.0 unx      884 b- defN 23-May-30 23:31 nvflare/app_common/pt/pt_file_model_persistor.py
 -rw-rw-r--  2.0 unx      881 b- defN 23-May-30 23:31 nvflare/app_common/pt/pt_model_reader_writer.py
 -rw-rw-r--  2.0 unx      890 b- defN 23-May-30 23:31 nvflare/app_common/pt/pt_multi_process_executor.py
 -rw-rw-r--  2.0 unx      871 b- defN 23-May-30 23:31 nvflare/app_common/pt/pt_scaffold.py
--rw-rw-r--  2.0 unx      878 b- defN 23-Jun-26 22:45 nvflare/app_common/pt/tb_receiver.py
+-rw-rw-r--  2.0 unx      881 b- defN 23-Jun-26 22:53 nvflare/app_common/pt/tb_receiver.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/resource_consumers/__init__.py
 -rw-rw-r--  2.0 unx     1431 b- defN 23-May-30 23:31 nvflare/app_common/resource_consumers/gpu_resource_consumer.py
 -rw-rw-r--  2.0 unx     1734 b- defN 23-May-30 23:31 nvflare/app_common/resource_consumers/list_resource_consumer.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/resource_managers/__init__.py
 -rw-rw-r--  2.0 unx     7594 b- defN 23-May-30 23:31 nvflare/app_common/resource_managers/auto_clean_resource_manager.py
 -rw-rw-r--  2.0 unx     5519 b- defN 23-May-30 23:31 nvflare/app_common/resource_managers/gpu_resource_manager.py
 -rw-rw-r--  2.0 unx     3285 b- defN 23-May-30 23:31 nvflare/app_common/resource_managers/list_resource_manager.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/response_processors/__init__.py
--rw-rw-r--  2.0 unx     5494 b- defN 23-Jun-26 22:45 nvflare/app_common/response_processors/global_weights_initializer.py
+-rw-rw-r--  2.0 unx     5498 b- defN 23-Jun-26 22:53 nvflare/app_common/response_processors/global_weights_initializer.py
 -rw-rw-r--  2.0 unx      726 b- defN 23-May-30 23:31 nvflare/app_common/shareablegenerators/__init__.py
 -rw-rw-r--  2.0 unx     3328 b- defN 23-May-30 23:31 nvflare/app_common/shareablegenerators/full_model_shareable_generator.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/state_persistors/__init__.py
 -rw-rw-r--  2.0 unx     2987 b- defN 23-May-30 23:31 nvflare/app_common/state_persistors/storage_state_persistor.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/statistics/__init__.py
 -rw-rw-r--  2.0 unx     3841 b- defN 23-May-30 23:31 nvflare/app_common/statistics/histogram_bins_cleanser.py
 -rw-rw-r--  2.0 unx     2945 b- defN 23-May-30 23:31 nvflare/app_common/statistics/json_stats_file_persistor.py
@@ -154,356 +163,399 @@
 -rw-rw-r--  2.0 unx     3041 b- defN 23-May-30 23:31 nvflare/app_common/statistics/numpy_utils.py
 -rw-rw-r--  2.0 unx     3274 b- defN 23-May-30 23:31 nvflare/app_common/statistics/statisitcs_objects_decomposer.py
 -rw-rw-r--  2.0 unx     1201 b- defN 23-May-30 23:31 nvflare/app_common/statistics/statistics_config_utils.py
 -rw-rw-r--  2.0 unx     1906 b- defN 23-May-30 23:31 nvflare/app_common/statistics/statistics_privacy_cleanser.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/storages/__init__.py
 -rw-rw-r--  2.0 unx     9072 b- defN 23-May-30 23:31 nvflare/app_common/storages/filesystem_storage.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/tracking/__init__.py
+-rw-rw-r--  2.0 unx     1565 b- defN 23-Jun-26 22:53 nvflare/app_common/tracking/log_writer.py
 -rw-rw-r--  2.0 unx      988 b- defN 23-May-30 23:31 nvflare/app_common/tracking/track_exception.py
--rw-rw-r--  2.0 unx     2275 b- defN 23-Jun-26 22:45 nvflare/app_common/tracking/tracker_types.py
+-rw-rw-r--  2.0 unx     1419 b- defN 23-Jun-26 22:53 nvflare/app_common/tracking/tracker_types.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/utils/__init__.py
 -rw-rw-r--  2.0 unx      774 b- defN 23-May-30 23:31 nvflare/app_common/utils/component_utils.py
 -rw-rw-r--  2.0 unx     1135 b- defN 23-May-30 23:31 nvflare/app_common/utils/file_utils.py
+-rw-rw-r--  2.0 unx     5764 b- defN 23-Jun-26 22:53 nvflare/app_common/utils/fl_model_utils.py
 -rw-rw-r--  2.0 unx     1730 b- defN 23-May-30 23:31 nvflare/app_common/utils/json_utils.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/widgets/__init__.py
 -rw-rw-r--  2.0 unx     2119 b- defN 23-May-30 23:31 nvflare/app_common/widgets/convert_to_fed_event.py
 -rw-rw-r--  2.0 unx    15452 b- defN 23-May-30 23:31 nvflare/app_common/widgets/event_recorder.py
 -rw-rw-r--  2.0 unx     5926 b- defN 23-May-30 23:31 nvflare/app_common/widgets/intime_model_selector.py
--rw-rw-r--  2.0 unx     9297 b- defN 23-Jun-26 22:45 nvflare/app_common/widgets/streaming.py
--rw-rw-r--  2.0 unx     3808 b- defN 23-Jun-26 22:45 nvflare/app_common/widgets/validation_json_generator.py
+-rw-rw-r--  2.0 unx    10386 b- defN 23-Jun-26 22:53 nvflare/app_common/widgets/streaming.py
+-rw-rw-r--  2.0 unx     4673 b- defN 23-Jun-26 22:53 nvflare/app_common/widgets/validation_json_generator.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_common/workflows/__init__.py
 -rw-rw-r--  2.0 unx     5293 b- defN 23-May-30 23:31 nvflare/app_common/workflows/broadcast_and_process.py
 -rw-rw-r--  2.0 unx     4083 b- defN 23-May-30 23:31 nvflare/app_common/workflows/broadcast_operator.py
--rw-rw-r--  2.0 unx    25598 b- defN 23-Jun-26 22:45 nvflare/app_common/workflows/cross_site_model_eval.py
--rw-rw-r--  2.0 unx    11412 b- defN 23-Jun-26 22:45 nvflare/app_common/workflows/cyclic_ctl.py
+-rw-rw-r--  2.0 unx    26530 b- defN 23-Jun-26 22:53 nvflare/app_common/workflows/cross_site_model_eval.py
+-rw-rw-r--  2.0 unx    11589 b- defN 23-Jun-26 22:53 nvflare/app_common/workflows/cyclic_ctl.py
 -rw-rw-r--  2.0 unx     1880 b- defN 23-May-30 23:31 nvflare/app_common/workflows/error_handling_controller.py
 -rw-rw-r--  2.0 unx     2945 b- defN 23-May-30 23:31 nvflare/app_common/workflows/global_model_eval.py
 -rw-rw-r--  2.0 unx     3023 b- defN 23-May-30 23:31 nvflare/app_common/workflows/initialize_global_weights.py
--rw-rw-r--  2.0 unx    19381 b- defN 23-Jun-26 22:45 nvflare/app_common/workflows/scatter_and_gather.py
--rw-rw-r--  2.0 unx    11586 b- defN 23-Jun-26 22:45 nvflare/app_common/workflows/scatter_and_gather_scaffold.py
--rw-rw-r--  2.0 unx    13125 b- defN 23-Jun-26 22:45 nvflare/app_common/workflows/splitnn_workflow.py
+-rw-rw-r--  2.0 unx    20050 b- defN 23-Jun-26 22:53 nvflare/app_common/workflows/scatter_and_gather.py
+-rw-rw-r--  2.0 unx    11826 b- defN 23-Jun-26 22:53 nvflare/app_common/workflows/scatter_and_gather_scaffold.py
+-rw-rw-r--  2.0 unx    13129 b- defN 23-Jun-26 22:53 nvflare/app_common/workflows/splitnn_workflow.py
 -rw-rw-r--  2.0 unx    24627 b- defN 23-May-30 23:31 nvflare/app_common/workflows/statistics_controller.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/__init__.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/he/__init__.py
 -rw-rw-r--  2.0 unx      638 b- defN 23-May-30 23:31 nvflare/app_opt/he/constant.py
 -rw-rw-r--  2.0 unx     5823 b- defN 23-May-30 23:31 nvflare/app_opt/he/cross_site_model_eval.py
 -rw-rw-r--  2.0 unx     1309 b- defN 23-May-30 23:31 nvflare/app_opt/he/decomposers.py
 -rw-rw-r--  2.0 unx     2498 b- defN 23-May-30 23:31 nvflare/app_opt/he/homomorphic_encrypt.py
 -rw-rw-r--  2.0 unx     3184 b- defN 23-May-30 23:31 nvflare/app_opt/he/intime_accumulate_model_aggregator.py
 -rw-rw-r--  2.0 unx     5552 b- defN 23-May-30 23:31 nvflare/app_opt/he/model_decryptor.py
 -rw-rw-r--  2.0 unx     9884 b- defN 23-May-30 23:31 nvflare/app_opt/he/model_encryptor.py
 -rw-rw-r--  2.0 unx     3367 b- defN 23-May-30 23:31 nvflare/app_opt/he/model_serialize_filter.py
--rw-rw-r--  2.0 unx     6331 b- defN 23-Jun-26 22:45 nvflare/app_opt/he/model_shareable_generator.py
+-rw-rw-r--  2.0 unx     6339 b- defN 23-Jun-26 22:53 nvflare/app_opt/he/model_shareable_generator.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/psi/__init__.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/psi/dh_psi/__init__.py
 -rw-rw-r--  2.0 unx     2414 b- defN 23-May-30 23:31 nvflare/app_opt/psi/dh_psi/dh_psi_client.py
 -rw-rw-r--  2.0 unx     2485 b- defN 23-May-30 23:31 nvflare/app_opt/psi/dh_psi/dh_psi_server.py
 -rw-rw-r--  2.0 unx     6861 b- defN 23-May-30 23:31 nvflare/app_opt/psi/dh_psi/dh_psi_task_handler.py
 -rw-rw-r--  2.0 unx     1370 b- defN 23-May-30 23:31 nvflare/app_opt/pt/__init__.py
 -rw-rw-r--  2.0 unx     1286 b- defN 23-May-30 23:31 nvflare/app_opt/pt/decomposers.py
 -rw-rw-r--  2.0 unx     4894 b- defN 23-May-30 23:31 nvflare/app_opt/pt/ditto.py
--rw-rw-r--  2.0 unx     9328 b- defN 23-Jun-26 22:45 nvflare/app_opt/pt/fedopt.py
+-rw-rw-r--  2.0 unx     9336 b- defN 23-Jun-26 22:53 nvflare/app_opt/pt/fedopt.py
 -rw-rw-r--  2.0 unx     1634 b- defN 23-May-30 23:31 nvflare/app_opt/pt/fedproxloss.py
 -rw-rw-r--  2.0 unx     2996 b- defN 23-May-30 23:31 nvflare/app_opt/pt/file_model_locator.py
--rw-rw-r--  2.0 unx    12584 b- defN 23-Jun-26 22:45 nvflare/app_opt/pt/file_model_persistor.py
--rw-rw-r--  2.0 unx     3070 b- defN 23-Jun-26 22:45 nvflare/app_opt/pt/he_model_reader_writer.py
+-rw-rw-r--  2.0 unx    12627 b- defN 23-Jun-26 22:53 nvflare/app_opt/pt/file_model_persistor.py
+-rw-rw-r--  2.0 unx     3074 b- defN 23-Jun-26 22:53 nvflare/app_opt/pt/he_model_reader_writer.py
 -rw-rw-r--  2.0 unx     4901 b- defN 23-May-30 23:31 nvflare/app_opt/pt/model_persistence_format_manager.py
 -rw-rw-r--  2.0 unx     2889 b- defN 23-May-30 23:31 nvflare/app_opt/pt/model_reader_writer.py
 -rw-rw-r--  2.0 unx     1153 b- defN 23-May-30 23:31 nvflare/app_opt/pt/multi_process_executor.py
 -rw-rw-r--  2.0 unx     5047 b- defN 23-May-30 23:31 nvflare/app_opt/pt/scaffold.py
 -rw-rw-r--  2.0 unx     1943 b- defN 23-May-30 23:31 nvflare/app_opt/pt/utils.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/sklearn/__init__.py
 -rw-rw-r--  2.0 unx     2133 b- defN 23-May-30 23:31 nvflare/app_opt/sklearn/data_loader.py
 -rw-rw-r--  2.0 unx     3226 b- defN 23-May-30 23:31 nvflare/app_opt/sklearn/joblib_model_param_persistor.py
--rw-rw-r--  2.0 unx     6176 b- defN 23-Jun-26 22:45 nvflare/app_opt/sklearn/sklearn_executor.py
+-rw-rw-r--  2.0 unx     7289 b- defN 23-Jun-26 22:53 nvflare/app_opt/sklearn/sklearn_executor.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/statistics/__init__.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/statistics/visualization/__init__.py
 -rw-rw-r--  2.0 unx     4470 b- defN 23-May-30 23:31 nvflare/app_opt/statistics/visualization/statistics_visualization.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/tracking/__init__.py
--rw-rw-r--  2.0 unx     3870 b- defN 23-Jun-26 22:45 nvflare/app_opt/tracking/tb_receiver.py
+-rw-rw-r--  2.0 unx      610 b- defN 23-Jun-26 22:53 nvflare/app_opt/tracking/mlflow/__init__.py
+-rw-rw-r--  2.0 unx    14967 b- defN 23-Jun-26 22:53 nvflare/app_opt/tracking/mlflow/mlflow_receiver.py
+-rw-rw-r--  2.0 unx     5569 b- defN 23-Jun-26 22:53 nvflare/app_opt/tracking/mlflow/mlflow_writer.py
+-rw-rw-r--  2.0 unx      610 b- defN 23-Jun-26 22:53 nvflare/app_opt/tracking/tb/__init__.py
+-rw-rw-r--  2.0 unx     3769 b- defN 23-Jun-26 22:53 nvflare/app_opt/tracking/tb/tb_receiver.py
+-rw-rw-r--  2.0 unx     2416 b- defN 23-Jun-26 22:53 nvflare/app_opt/tracking/tb/tb_writer.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/xgboost/__init__.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/xgboost/histogram_based/__init__.py
 -rw-rw-r--  2.0 unx      807 b- defN 23-May-30 23:31 nvflare/app_opt/xgboost/histogram_based/constants.py
--rw-rw-r--  2.0 unx     6964 b- defN 23-Jun-26 22:45 nvflare/app_opt/xgboost/histogram_based/controller.py
--rw-rw-r--  2.0 unx     9712 b- defN 23-Jun-26 22:45 nvflare/app_opt/xgboost/histogram_based/executor.py
+-rw-rw-r--  2.0 unx     6968 b- defN 23-Jun-26 22:53 nvflare/app_opt/xgboost/histogram_based/controller.py
+-rw-rw-r--  2.0 unx     9716 b- defN 23-Jun-26 22:53 nvflare/app_opt/xgboost/histogram_based/executor.py
 -rw-rw-r--  2.0 unx     2143 b- defN 23-May-30 23:31 nvflare/app_opt/xgboost/histogram_based/executor_spec.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/app_opt/xgboost/tree_based/__init__.py
--rw-rw-r--  2.0 unx     5078 b- defN 23-Jun-26 22:45 nvflare/app_opt/xgboost/tree_based/bagging_aggregator.py
+-rw-rw-r--  2.0 unx     5082 b- defN 23-Jun-26 22:53 nvflare/app_opt/xgboost/tree_based/bagging_aggregator.py
 -rw-rw-r--  2.0 unx    11777 b- defN 23-May-30 23:31 nvflare/app_opt/xgboost/tree_based/executor.py
 -rw-rw-r--  2.0 unx     3666 b- defN 23-May-30 23:31 nvflare/app_opt/xgboost/tree_based/model_persistor.py
 -rw-rw-r--  2.0 unx     6830 b- defN 23-May-30 23:31 nvflare/app_opt/xgboost/tree_based/shareable_generator.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/dashboard/__init__.py
--rw-rw-r--  2.0 unx     6767 b- defN 23-Jun-26 22:45 nvflare/dashboard/cli.py
+-rw-rw-r--  2.0 unx     7388 b- defN 23-Jun-26 22:53 nvflare/dashboard/cli.py
 -rw-rw-r--  2.0 unx     1268 b- defN 23-May-30 23:31 nvflare/dashboard/config.py
 -rw-rw-r--  2.0 unx     1229 b- defN 23-May-30 23:31 nvflare/dashboard/wsgi.py
 -rw-rw-r--  2.0 unx     1697 b- defN 23-May-30 23:31 nvflare/dashboard/application/__init__.py
--rw-rw-r--  2.0 unx    14394 b- defN 23-Jun-26 22:45 nvflare/dashboard/application/blob.py
+-rw-rw-r--  2.0 unx    15738 b- defN 23-Jun-26 22:53 nvflare/dashboard/application/blob.py
 -rw-rw-r--  2.0 unx     4940 b- defN 23-May-30 23:31 nvflare/dashboard/application/cert.py
 -rw-rw-r--  2.0 unx     3001 b- defN 23-May-30 23:31 nvflare/dashboard/application/clients.py
--rw-rw-r--  2.0 unx     4487 b- defN 23-Jun-26 22:45 nvflare/dashboard/application/models.py
+-rw-rw-r--  2.0 unx     4543 b- defN 23-Jun-26 22:53 nvflare/dashboard/application/models.py
 -rw-rw-r--  2.0 unx     4401 b- defN 23-May-30 23:31 nvflare/dashboard/application/project.py
--rw-rw-r--  2.0 unx    12846 b- defN 23-Jun-26 22:45 nvflare/dashboard/application/store.py
+-rw-rw-r--  2.0 unx    12862 b- defN 23-Jun-26 22:53 nvflare/dashboard/application/store.py
 -rw-rw-r--  2.0 unx     2918 b- defN 23-May-30 23:31 nvflare/dashboard/application/users.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/__init__.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/common/__init__.py
 -rw-rw-r--  2.0 unx     2062 b- defN 23-May-30 23:31 nvflare/fuel/common/ctx.py
 -rw-rw-r--  2.0 unx      711 b- defN 23-May-30 23:31 nvflare/fuel/common/excepts.py
 -rw-rw-r--  2.0 unx     1571 b- defN 23-May-30 23:31 nvflare/fuel/common/multi_process_executor_constants.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/f3/__init__.py
 -rw-rw-r--  2.0 unx     3259 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/comm_config.py
 -rw-rw-r--  2.0 unx     1116 b- defN 23-May-30 23:31 nvflare/fuel/f3/comm_error.py
--rw-rw-r--  2.0 unx     8760 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/communicator.py
+-rw-rw-r--  2.0 unx     8760 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/communicator.py
 -rw-rw-r--  2.0 unx     3733 b- defN 23-May-30 23:31 nvflare/fuel/f3/connection.py
 -rw-rw-r--  2.0 unx     2198 b- defN 23-May-30 23:31 nvflare/fuel/f3/endpoint.py
--rw-rw-r--  2.0 unx     2136 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/message.py
+-rw-rw-r--  2.0 unx     2033 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/message.py
 -rw-rw-r--  2.0 unx     6247 b- defN 23-May-30 23:31 nvflare/fuel/f3/mpm.py
--rw-rw-r--  2.0 unx     3837 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/stats_pool.py
+-rw-rw-r--  2.0 unx    19445 b- defN 23-Jun-26 22:53 nvflare/fuel/f3/stats_pool.py
+-rw-rw-r--  2.0 unx     9813 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/stream_cell.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/f3/cellnet/__init__.py
 -rw-rw-r--  2.0 unx     1388 b- defN 23-May-30 23:31 nvflare/fuel/f3/cellnet/cbs.py
--rw-rw-r--  2.0 unx    82944 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/cellnet/cell.py
+-rw-rw-r--  2.0 unx    81908 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/cellnet/cell.py
 -rw-rw-r--  2.0 unx     9249 b- defN 23-May-30 23:31 nvflare/fuel/f3/cellnet/connector_manager.py
 -rw-rw-r--  2.0 unx     3367 b- defN 23-May-30 23:31 nvflare/fuel/f3/cellnet/defs.py
 -rw-rw-r--  2.0 unx     2498 b- defN 23-May-30 23:31 nvflare/fuel/f3/cellnet/fqcn.py
--rw-rw-r--  2.0 unx    34394 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/cellnet/net_agent.py
--rw-rw-r--  2.0 unx    17335 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/cellnet/net_manager.py
--rw-rw-r--  2.0 unx     2676 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/cellnet/utils.py
+-rw-rw-r--  2.0 unx    34221 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/cellnet/net_agent.py
+-rw-rw-r--  2.0 unx    17331 b- defN 23-Jun-26 22:53 nvflare/fuel/f3/cellnet/net_manager.py
+-rw-rw-r--  2.0 unx     1743 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/cellnet/registry.py
+-rw-rw-r--  2.0 unx     2452 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/cellnet/utils.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/__init__.py
 -rw-rw-r--  2.0 unx     4963 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/aio_conn.py
 -rw-rw-r--  2.0 unx     4354 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/aio_context.py
 -rw-rw-r--  2.0 unx    16267 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/aio_grpc_driver.py
 -rw-rw-r--  2.0 unx     6470 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/aio_http_driver.py
 -rw-rw-r--  2.0 unx     3895 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/aio_tcp_driver.py
 -rw-rw-r--  2.0 unx     2376 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/base_driver.py
--rw-rw-r--  2.0 unx     1154 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/drivers/connector_info.py
+-rw-rw-r--  2.0 unx     1122 b- defN 23-Jun-26 22:53 nvflare/fuel/f3/drivers/connector_info.py
 -rw-rw-r--  2.0 unx     3583 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/driver.py
 -rw-rw-r--  2.0 unx     4108 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/drivers/driver_manager.py
 -rw-rw-r--  2.0 unx     1380 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/driver_params.py
 -rw-rw-r--  2.0 unx     7632 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/net_utils.py
 -rw-rw-r--  2.0 unx     5550 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/socket_conn.py
 -rw-rw-r--  2.0 unx     3622 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/tcp_driver.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/grpc/__init__.py
 -rw-rw-r--  2.0 unx     1840 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/grpc/streamer_pb2.py
 -rw-rw-r--  2.0 unx     2817 b- defN 23-May-30 23:31 nvflare/fuel/f3/drivers/grpc/streamer_pb2_grpc.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/f3/sfm/__init__.py
--rw-rw-r--  2.0 unx    17618 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/sfm/conn_manager.py
+-rw-rw-r--  2.0 unx    17630 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/sfm/conn_manager.py
 -rw-rw-r--  2.0 unx     1082 b- defN 23-May-30 23:31 nvflare/fuel/f3/sfm/constants.py
 -rw-rw-r--  2.0 unx     2417 b- defN 23-May-30 23:31 nvflare/fuel/f3/sfm/prefix.py
--rw-rw-r--  2.0 unx     4928 b- defN 23-Jun-26 22:45 nvflare/fuel/f3/sfm/sfm_conn.py
+-rw-rw-r--  2.0 unx     4888 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/sfm/sfm_conn.py
 -rw-rw-r--  2.0 unx     3088 b- defN 23-May-30 23:31 nvflare/fuel/f3/sfm/sfm_endpoint.py
+-rw-rw-r--  2.0 unx      610 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/__init__.py
+-rw-rw-r--  2.0 unx     3906 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/blob_streamer.py
+-rw-rw-r--  2.0 unx     8229 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/byte_receiver.py
+-rw-rw-r--  2.0 unx     7577 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/byte_streamer.py
+-rw-rw-r--  2.0 unx     3675 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/file_streamer.py
+-rw-rw-r--  2.0 unx     5078 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/object_streamer.py
+-rw-rw-r--  2.0 unx     1565 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/stream_const.py
+-rw-rw-r--  2.0 unx     7840 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/stream_types.py
+-rw-rw-r--  2.0 unx     1268 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/stream_utils.py
+-rw-rw-r--  2.0 unx      610 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/tools/__init__.py
+-rw-rw-r--  2.0 unx     2779 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/tools/file_receiver.py
+-rw-rw-r--  2.0 unx     2549 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/tools/file_sender.py
+-rw-rw-r--  2.0 unx     2169 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/tools/receiver.py
+-rw-rw-r--  2.0 unx     1640 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/tools/sender.py
+-rw-rw-r--  2.0 unx     1544 b- defN 23-Jun-26 22:54 nvflare/fuel/f3/streaming/tools/utils.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/flare_api/__init__.py
--rw-rw-r--  2.0 unx     6518 b- defN 23-Jun-26 22:45 nvflare/fuel/flare_api/api_spec.py
+-rw-rw-r--  2.0 unx    15841 b- defN 23-Jun-26 22:53 nvflare/fuel/flare_api/api_spec.py
 -rw-rw-r--  2.0 unx     3107 b- defN 23-May-30 23:31 nvflare/fuel/flare_api/config.py
--rw-rw-r--  2.0 unx    18877 b- defN 23-Jun-26 22:45 nvflare/fuel/flare_api/flare_api.py
+-rw-rw-r--  2.0 unx    35086 b- defN 23-Jun-26 22:53 nvflare/fuel/flare_api/flare_api.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/hci/__init__.py
 -rw-rw-r--  2.0 unx     2541 b- defN 23-May-30 23:31 nvflare/fuel/hci/base64_utils.py
--rw-rw-r--  2.0 unx     2036 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/cmd_arg_utils.py
--rw-rw-r--  2.0 unx     5674 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/conn.py
+-rw-rw-r--  2.0 unx     4691 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/cmd_arg_utils.py
+-rw-rw-r--  2.0 unx     5752 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/conn.py
 -rw-rw-r--  2.0 unx     1254 b- defN 23-May-30 23:31 nvflare/fuel/hci/file_transfer_defs.py
--rw-rw-r--  2.0 unx     6196 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/proto.py
+-rw-rw-r--  2.0 unx     6636 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/proto.py
 -rw-rw-r--  2.0 unx     8408 b- defN 23-May-30 23:31 nvflare/fuel/hci/reg.py
 -rw-rw-r--  2.0 unx     3773 b- defN 23-May-30 23:31 nvflare/fuel/hci/security.py
 -rw-rw-r--  2.0 unx     4136 b- defN 23-May-30 23:31 nvflare/fuel/hci/shell_cmd_val.py
 -rw-rw-r--  2.0 unx     3352 b- defN 23-May-30 23:31 nvflare/fuel/hci/table.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/hci/client/__init__.py
--rw-rw-r--  2.0 unx    32607 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/client/api.py
--rw-rw-r--  2.0 unx     4974 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/client/api_spec.py
+-rw-rw-r--  2.0 unx    34099 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/client/api.py
+-rw-rw-r--  2.0 unx     5011 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/client/api_spec.py
 -rw-rw-r--  2.0 unx     1607 b- defN 23-May-30 23:31 nvflare/fuel/hci/client/api_status.py
--rw-rw-r--  2.0 unx    18067 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/client/cli.py
+-rw-rw-r--  2.0 unx    18850 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/client/cli.py
 -rw-rw-r--  2.0 unx    13935 b- defN 23-May-30 23:31 nvflare/fuel/hci/client/file_transfer.py
--rw-rw-r--  2.0 unx    48215 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/client/fl_admin_api.py
+-rw-rw-r--  2.0 unx    48451 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/client/fl_admin_api.py
 -rw-rw-r--  2.0 unx     1071 b- defN 23-May-30 23:31 nvflare/fuel/hci/client/fl_admin_api_constants.py
 -rw-rw-r--  2.0 unx     6734 b- defN 23-May-30 23:31 nvflare/fuel/hci/client/fl_admin_api_runner.py
 -rw-rw-r--  2.0 unx    15874 b- defN 23-May-30 23:31 nvflare/fuel/hci/client/fl_admin_api_spec.py
--rw-rw-r--  2.0 unx     2476 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/client/overseer_service_finder.py
+-rw-rw-r--  2.0 unx     2475 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/client/overseer_service_finder.py
 -rw-rw-r--  2.0 unx     2047 b- defN 23-May-30 23:31 nvflare/fuel/hci/client/rr_service_finder.py
--rw-rw-r--  2.0 unx      932 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/client/static_service_finder.py
+-rw-rw-r--  2.0 unx      966 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/client/static_service_finder.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/hci/server/__init__.py
 -rw-rw-r--  2.0 unx     1640 b- defN 23-May-30 23:31 nvflare/fuel/hci/server/audit.py
 -rw-rw-r--  2.0 unx     3231 b- defN 23-May-30 23:31 nvflare/fuel/hci/server/authz.py
 -rw-rw-r--  2.0 unx     3377 b- defN 23-May-30 23:31 nvflare/fuel/hci/server/builtin.py
--rw-rw-r--  2.0 unx     1208 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/server/constants.py
--rw-rw-r--  2.0 unx     7964 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/server/file_transfer.py
--rw-rw-r--  2.0 unx     6437 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/server/hci.py
--rw-rw-r--  2.0 unx     7646 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/server/login.py
--rw-rw-r--  2.0 unx     3874 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/server/reg.py
+-rw-rw-r--  2.0 unx     1240 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/server/constants.py
+-rw-rw-r--  2.0 unx     7968 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/server/file_transfer.py
+-rw-rw-r--  2.0 unx     7176 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/server/hci.py
+-rw-rw-r--  2.0 unx     7654 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/server/login.py
+-rw-rw-r--  2.0 unx     3878 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/server/reg.py
 -rw-rw-r--  2.0 unx     6464 b- defN 23-May-30 23:31 nvflare/fuel/hci/server/sess.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/hci/tools/__init__.py
--rw-rw-r--  2.0 unx     4147 b- defN 23-Jun-26 22:45 nvflare/fuel/hci/tools/admin.py
+-rw-rw-r--  2.0 unx     4179 b- defN 23-Jun-26 22:53 nvflare/fuel/hci/tools/admin.py
 -rw-rw-r--  2.0 unx     5149 b- defN 23-May-30 23:31 nvflare/fuel/hci/tools/authz_preview.py
 -rw-rw-r--  2.0 unx     1198 b- defN 23-May-30 23:31 nvflare/fuel/hci/tools/make_pwd.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/sec/__init__.py
 -rw-rw-r--  2.0 unx     3907 b- defN 23-May-30 23:31 nvflare/fuel/sec/audit.py
 -rw-rw-r--  2.0 unx    15241 b- defN 23-May-30 23:31 nvflare/fuel/sec/authz.py
 -rw-rw-r--  2.0 unx     5241 b- defN 23-May-30 23:31 nvflare/fuel/sec/security_content_service.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/utils/__init__.py
 -rw-rw-r--  2.0 unx     2773 b- defN 23-May-30 23:31 nvflare/fuel/utils/argument_utils.py
 -rw-rw-r--  2.0 unx     5832 b- defN 23-May-30 23:31 nvflare/fuel/utils/class_utils.py
--rw-rw-r--  2.0 unx     4373 b- defN 23-Jun-26 22:45 nvflare/fuel/utils/component_builder.py
+-rw-rw-r--  2.0 unx     4377 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/component_builder.py
+-rw-rw-r--  2.0 unx     4645 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/config.py
+-rw-rw-r--  2.0 unx     4503 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/config_factory.py
 -rw-rw-r--  2.0 unx     9389 b- defN 23-Jun-26 22:45 nvflare/fuel/utils/config_service.py
--rw-rw-r--  2.0 unx     4066 b- defN 23-Jun-26 22:45 nvflare/fuel/utils/dict_utils.py
--rw-rw-r--  2.0 unx     3137 b- defN 23-Jun-26 22:45 nvflare/fuel/utils/fsm.py
+-rw-rw-r--  2.0 unx      704 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/constants.py
+-rw-rw-r--  2.0 unx     1858 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/deprecated.py
+-rw-rw-r--  2.0 unx     6024 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/dict_utils.py
+-rw-rw-r--  2.0 unx     3314 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/fsm.py
 -rw-rw-r--  2.0 unx     2113 b- defN 23-May-30 23:31 nvflare/fuel/utils/gpu_utils.py
 -rw-rw-r--  2.0 unx     7347 b- defN 23-May-30 23:31 nvflare/fuel/utils/import_utils.py
--rw-rw-r--  2.0 unx     4941 b- defN 23-Jun-26 22:45 nvflare/fuel/utils/json_scanner.py
+-rw-rw-r--  2.0 unx     2327 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/json_config_loader.py
+-rw-rw-r--  2.0 unx     4949 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/json_scanner.py
 -rw-rw-r--  2.0 unx     1259 b- defN 23-May-30 23:31 nvflare/fuel/utils/network_utils.py
 -rw-rw-r--  2.0 unx     1349 b- defN 23-May-30 23:31 nvflare/fuel/utils/obj_utils.py
--rw-rw-r--  2.0 unx    10876 b- defN 23-Jun-26 22:45 nvflare/fuel/utils/stats_utils.py
 -rw-rw-r--  2.0 unx      924 b- defN 23-May-30 23:31 nvflare/fuel/utils/time_utils.py
+-rw-rw-r--  2.0 unx     1938 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/validation_utils.py
 -rw-rw-r--  2.0 unx    10957 b- defN 23-May-30 23:31 nvflare/fuel/utils/wfconf.py
 -rw-rw-r--  2.0 unx     5278 b- defN 23-May-30 23:31 nvflare/fuel/utils/zip_utils.py
 -rw-rw-r--  2.0 unx     1072 b- defN 23-May-30 23:31 nvflare/fuel/utils/fobs/__init__.py
 -rw-rw-r--  2.0 unx     3788 b- defN 23-May-30 23:31 nvflare/fuel/utils/fobs/decomposer.py
 -rw-rw-r--  2.0 unx     7652 b- defN 23-May-30 23:31 nvflare/fuel/utils/fobs/fobs.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/fuel/utils/fobs/decomposers/__init__.py
 -rw-rw-r--  2.0 unx     1815 b- defN 23-May-30 23:31 nvflare/fuel/utils/fobs/decomposers/core_decomposers.py
+-rw-rw-r--  2.0 unx      610 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/pipe/__init__.py
+-rw-rw-r--  2.0 unx     1163 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/pipe/file_accessor.py
+-rw-rw-r--  2.0 unx     2280 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/pipe/file_name_utils.py
+-rw-rw-r--  2.0 unx     8613 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/pipe/file_pipe.py
+-rw-rw-r--  2.0 unx     1429 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/pipe/fobs_file_accessor.py
+-rw-rw-r--  2.0 unx     3531 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/pipe/pipe.py
+-rw-rw-r--  2.0 unx     8554 b- defN 23-Jun-26 22:53 nvflare/fuel/utils/pipe/pipe_handler.py
+-rw-rw-r--  2.0 unx      610 b- defN 23-Jun-26 22:53 nvflare/fuel_opt/__init__.py
+-rw-rw-r--  2.0 unx      610 b- defN 23-Jun-26 22:53 nvflare/fuel_opt/utils/__init__.py
+-rw-rw-r--  2.0 unx     1982 b- defN 23-Jun-26 22:53 nvflare/fuel_opt/utils/omegaconf_loader.py
+-rw-rw-r--  2.0 unx     2843 b- defN 23-Jun-26 22:53 nvflare/fuel_opt/utils/pyhocon_loader.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/ha/__init__.py
 -rw-rw-r--  2.0 unx     3875 b- defN 23-May-30 23:31 nvflare/ha/dummy_overseer_agent.py
--rw-rw-r--  2.0 unx     5583 b- defN 23-Jun-26 22:45 nvflare/ha/ha_admin_cmds.py
+-rw-rw-r--  2.0 unx     6098 b- defN 23-Jun-26 22:53 nvflare/ha/ha_admin_cmds.py
 -rw-rw-r--  2.0 unx     6452 b- defN 23-May-30 23:31 nvflare/ha/overseer_agent.py
 -rw-rw-r--  2.0 unx     3477 b- defN 23-May-30 23:31 nvflare/ha/overseer_agent_app.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/ha/overseer/__init__.py
 -rw-rw-r--  2.0 unx      701 b- defN 23-May-30 23:31 nvflare/ha/overseer/app.py
 -rw-rw-r--  2.0 unx     1716 b- defN 23-May-30 23:31 nvflare/ha/overseer/mem_store.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-26 22:45 nvflare/ha/overseer/overseer.py
+-rw-rw-r--  2.0 unx     3544 b- defN 23-Jun-26 22:53 nvflare/ha/overseer/overseer.py
 -rw-rw-r--  2.0 unx     3144 b- defN 23-May-30 23:31 nvflare/ha/overseer/utils.py
 -rw-rw-r--  2.0 unx     1197 b- defN 23-May-30 23:31 nvflare/ha/overseer/worker.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/lighter/__init__.py
--rw-rw-r--  2.0 unx     2045 b- defN 23-Jun-26 22:45 nvflare/lighter/dummy_project.yml
--rw-rw-r--  2.0 unx     2636 b- defN 23-Jun-26 22:45 nvflare/lighter/ha_project.yml
--rw-rw-r--  2.0 unx     3915 b- defN 23-Jun-26 22:45 nvflare/lighter/poc.py
--rw-rw-r--  2.0 unx    13438 b- defN 23-Jun-26 22:45 nvflare/lighter/poc_commands.py
--rw-rw-r--  2.0 unx     6198 b- defN 23-Jun-26 22:45 nvflare/lighter/provision.py
--rw-rw-r--  2.0 unx      887 b- defN 23-Jun-26 22:45 nvflare/lighter/service_constants.py
--rw-rw-r--  2.0 unx     7022 b- defN 23-Jun-26 22:45 nvflare/lighter/spec.py
--rw-rw-r--  2.0 unx     7880 b- defN 23-Jun-26 22:45 nvflare/lighter/utils.py
+-rw-rw-r--  2.0 unx     2155 b- defN 23-Jun-26 22:53 nvflare/lighter/dummy_project.yml
+-rw-rw-r--  2.0 unx     2752 b- defN 23-Jun-26 22:53 nvflare/lighter/ha_project.yml
+-rw-rw-r--  2.0 unx     3923 b- defN 23-Jun-26 22:53 nvflare/lighter/poc.py
+-rw-rw-r--  2.0 unx    30470 b- defN 23-Jun-26 22:53 nvflare/lighter/poc_commands.py
+-rw-rw-r--  2.0 unx     7312 b- defN 23-Jun-26 22:53 nvflare/lighter/provision.py
+-rw-rw-r--  2.0 unx      939 b- defN 23-Jun-26 22:53 nvflare/lighter/service_constants.py
+-rw-rw-r--  2.0 unx     7026 b- defN 23-Jun-26 22:53 nvflare/lighter/spec.py
+-rw-rw-r--  2.0 unx      791 b- defN 23-Jun-26 22:53 nvflare/lighter/tplt_utils.py
+-rw-rw-r--  2.0 unx     8392 b- defN 23-Jun-26 22:53 nvflare/lighter/utils.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/lighter/impl/__init__.py
--rw-rw-r--  2.0 unx     8317 b- defN 23-Jun-26 22:45 nvflare/lighter/impl/cert.py
--rw-rw-r--  2.0 unx     4784 b- defN 23-Jun-26 22:45 nvflare/lighter/impl/docker.py
+-rw-rw-r--  2.0 unx     8413 b- defN 23-Jun-26 22:53 nvflare/lighter/impl/cert.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-26 22:53 nvflare/lighter/impl/docker.py
 -rw-rw-r--  2.0 unx     3177 b- defN 23-May-30 23:31 nvflare/lighter/impl/he.py
 -rw-rw-r--  2.0 unx     6123 b- defN 23-May-30 23:31 nvflare/lighter/impl/helm_chart.py
--rw-rw-r--  2.0 unx    62178 b- defN 23-Jun-26 22:45 nvflare/lighter/impl/master_template.yml
+-rw-rw-r--  2.0 unx      861 b- defN 23-Jun-26 22:53 nvflare/lighter/impl/local_cert.py
+-rw-rw-r--  2.0 unx     2836 b- defN 23-Jun-26 22:53 nvflare/lighter/impl/local_static_file.py
+-rw-rw-r--  2.0 unx    65602 b- defN 23-Jun-26 22:53 nvflare/lighter/impl/master_template.yml
 -rw-rw-r--  2.0 unx     1903 b- defN 23-May-30 23:31 nvflare/lighter/impl/signature.py
--rw-rw-r--  2.0 unx    14480 b- defN 23-Jun-26 22:45 nvflare/lighter/impl/static_file.py
+-rw-rw-r--  2.0 unx    15041 b- defN 23-Jun-26 22:53 nvflare/lighter/impl/static_file.py
 -rw-rw-r--  2.0 unx     1299 b- defN 23-May-30 23:31 nvflare/lighter/impl/template.py
--rw-rw-r--  2.0 unx     4157 b- defN 23-Jun-26 22:45 nvflare/lighter/impl/workspace.py
+-rw-rw-r--  2.0 unx     4127 b- defN 23-Jun-26 22:53 nvflare/lighter/impl/workspace.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/private/__init__.py
 -rw-rw-r--  2.0 unx     2581 b- defN 23-May-30 23:31 nvflare/private/admin_defs.py
--rw-rw-r--  2.0 unx    11175 b- defN 23-Jun-26 22:45 nvflare/private/aux_runner.py
--rw-rw-r--  2.0 unx     4551 b- defN 23-Jun-26 22:45 nvflare/private/defs.py
+-rw-rw-r--  2.0 unx    11126 b- defN 23-Jun-26 22:54 nvflare/private/aux_runner.py
+-rw-rw-r--  2.0 unx     4535 b- defN 23-Jun-26 22:54 nvflare/private/defs.py
 -rw-rw-r--  2.0 unx     2923 b- defN 23-May-30 23:31 nvflare/private/event.py
 -rw-rw-r--  2.0 unx     7536 b- defN 23-May-30 23:31 nvflare/private/fed_json_config.py
--rw-rw-r--  2.0 unx     5366 b- defN 23-Jun-26 22:45 nvflare/private/json_configer.py
+-rw-rw-r--  2.0 unx     5370 b- defN 23-Jun-26 22:53 nvflare/private/json_configer.py
 -rw-rw-r--  2.0 unx     4226 b- defN 23-May-30 23:31 nvflare/private/privacy_manager.py
 -rw-rw-r--  2.0 unx      737 b- defN 23-May-30 23:31 nvflare/private/scheduler_constants.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/private/fed/__init__.py
--rw-rw-r--  2.0 unx    10032 b- defN 23-Jun-26 22:45 nvflare/private/fed/cmi.py
+-rw-rw-r--  2.0 unx     9975 b- defN 23-Jun-26 22:54 nvflare/private/fed/cmi.py
 -rw-rw-r--  2.0 unx      919 b- defN 23-May-30 23:31 nvflare/private/fed/runner.py
 -rw-rw-r--  2.0 unx      641 b- defN 23-May-30 23:31 nvflare/private/fed/app/__init__.py
 -rw-rw-r--  2.0 unx     2092 b- defN 23-May-30 23:31 nvflare/private/fed/app/default_app_validator.py
 -rw-rw-r--  2.0 unx     1783 b- defN 23-May-30 23:31 nvflare/private/fed/app/fl_app_validator.py
--rw-rw-r--  2.0 unx    17853 b- defN 23-Jun-26 22:45 nvflare/private/fed/app/fl_conf.py
+-rw-rw-r--  2.0 unx    17861 b- defN 23-Jun-26 22:53 nvflare/private/fed/app/fl_conf.py
 -rw-rw-r--  2.0 unx     3209 b- defN 23-May-30 23:31 nvflare/private/fed/app/utils.py
 -rw-rw-r--  2.0 unx      648 b- defN 23-May-30 23:31 nvflare/private/fed/app/client/__init__.py
--rw-rw-r--  2.0 unx     6322 b- defN 23-Jun-26 22:45 nvflare/private/fed/app/client/client_train.py
--rw-rw-r--  2.0 unx    13818 b- defN 23-Jun-26 22:45 nvflare/private/fed/app/client/sub_worker_process.py
--rw-rw-r--  2.0 unx     7016 b- defN 23-Jun-26 22:45 nvflare/private/fed/app/client/worker_process.py
+-rw-rw-r--  2.0 unx     6326 b- defN 23-Jun-26 22:53 nvflare/private/fed/app/client/client_train.py
+-rw-rw-r--  2.0 unx    14191 b- defN 23-Jun-26 22:53 nvflare/private/fed/app/client/sub_worker_process.py
+-rw-rw-r--  2.0 unx     7284 b- defN 23-Jun-26 22:53 nvflare/private/fed/app/client/worker_process.py
 -rw-rw-r--  2.0 unx      649 b- defN 23-May-30 23:31 nvflare/private/fed/app/deployer/__init__.py
 -rw-rw-r--  2.0 unx     3603 b- defN 23-May-30 23:31 nvflare/private/fed/app/deployer/base_client_deployer.py
 -rw-rw-r--  2.0 unx     4862 b- defN 23-May-30 23:31 nvflare/private/fed/app/deployer/server_deployer.py
--rw-rw-r--  2.0 unx     6152 b- defN 23-Jun-26 22:45 nvflare/private/fed/app/deployer/simulator_deployer.py
+-rw-rw-r--  2.0 unx     6156 b- defN 23-Jun-26 22:53 nvflare/private/fed/app/deployer/simulator_deployer.py
 -rw-rw-r--  2.0 unx      649 b- defN 23-May-30 23:31 nvflare/private/fed/app/server/__init__.py
--rw-rw-r--  2.0 unx     6356 b- defN 23-Jun-26 22:45 nvflare/private/fed/app/server/runner_process.py
--rw-rw-r--  2.0 unx     5786 b- defN 23-Jun-26 22:45 nvflare/private/fed/app/server/server_train.py
+-rw-rw-r--  2.0 unx     6630 b- defN 23-Jun-26 22:53 nvflare/private/fed/app/server/runner_process.py
+-rw-rw-r--  2.0 unx     5790 b- defN 23-Jun-26 22:53 nvflare/private/fed/app/server/server_train.py
 -rw-rw-r--  2.0 unx      636 b- defN 23-May-30 23:31 nvflare/private/fed/app/simulator/__init__.py
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-30 23:31 nvflare/private/fed/app/simulator/log.config
 -rw-rw-r--  2.0 unx     2574 b- defN 23-May-30 23:31 nvflare/private/fed/app/simulator/simulator.py
--rw-rw-r--  2.0 unx    24803 b- defN 23-Jun-26 22:45 nvflare/private/fed/app/simulator/simulator_runner.py
--rw-rw-r--  2.0 unx    11272 b- defN 23-Jun-26 22:45 nvflare/private/fed/app/simulator/simulator_worker.py
+-rw-rw-r--  2.0 unx    25568 b- defN 23-Jun-26 22:53 nvflare/private/fed/app/simulator/simulator_runner.py
+-rw-rw-r--  2.0 unx    11276 b- defN 23-Jun-26 22:53 nvflare/private/fed/app/simulator/simulator_worker.py
 -rw-rw-r--  2.0 unx      653 b- defN 23-May-30 23:31 nvflare/private/fed/client/__init__.py
--rw-rw-r--  2.0 unx     6169 b- defN 23-Jun-26 22:45 nvflare/private/fed/client/admin.py
+-rw-rw-r--  2.0 unx     6173 b- defN 23-Jun-26 22:53 nvflare/private/fed/client/admin.py
 -rw-rw-r--  2.0 unx     7851 b- defN 23-May-30 23:31 nvflare/private/fed/client/admin_commands.py
 -rw-rw-r--  2.0 unx     5521 b- defN 23-Jun-22 21:32 nvflare/private/fed/client/client_app_runner.py
--rw-rw-r--  2.0 unx     9741 b- defN 23-Jun-26 22:45 nvflare/private/fed/client/client_engine.py
+-rw-rw-r--  2.0 unx    10272 b- defN 23-Jun-26 22:53 nvflare/private/fed/client/client_engine.py
 -rw-rw-r--  2.0 unx     4618 b- defN 23-May-30 23:31 nvflare/private/fed/client/client_engine_executor_spec.py
 -rw-rw-r--  2.0 unx     3194 b- defN 23-May-30 23:31 nvflare/private/fed/client/client_engine_internal_spec.py
 -rw-rw-r--  2.0 unx    15638 b- defN 23-May-30 23:31 nvflare/private/fed/client/client_executor.py
 -rw-rw-r--  2.0 unx     5410 b- defN 23-May-30 23:31 nvflare/private/fed/client/client_json_config.py
 -rw-rw-r--  2.0 unx     2195 b- defN 23-May-30 23:31 nvflare/private/fed/client/client_req_processors.py
 -rw-rw-r--  2.0 unx     9812 b- defN 23-May-30 23:31 nvflare/private/fed/client/client_run_manager.py
--rw-rw-r--  2.0 unx    26410 b- defN 23-Jun-26 22:45 nvflare/private/fed/client/client_runner.py
+-rw-rw-r--  2.0 unx    26526 b- defN 23-Jun-26 22:53 nvflare/private/fed/client/client_runner.py
 -rw-rw-r--  2.0 unx      998 b- defN 23-May-30 23:31 nvflare/private/fed/client/client_status.py
 -rw-rw-r--  2.0 unx     3982 b- defN 23-May-30 23:31 nvflare/private/fed/client/command_agent.py
--rw-rw-r--  2.0 unx    14499 b- defN 23-Jun-26 22:45 nvflare/private/fed/client/communicator.py
+-rw-rw-r--  2.0 unx    14529 b- defN 23-Jun-26 22:53 nvflare/private/fed/client/communicator.py
 -rw-rw-r--  2.0 unx     2138 b- defN 23-May-30 23:31 nvflare/private/fed/client/comp_caller_cmd.py
 -rw-rw-r--  2.0 unx     3997 b- defN 23-Jun-26 22:45 nvflare/private/fed/client/fed_client.py
 -rw-rw-r--  2.0 unx    16151 b- defN 23-Jun-26 22:45 nvflare/private/fed/client/fed_client_base.py
 -rw-rw-r--  2.0 unx     2040 b- defN 23-May-30 23:31 nvflare/private/fed/client/info_coll_cmd.py
--rw-rw-r--  2.0 unx     7031 b- defN 23-Jun-26 22:45 nvflare/private/fed/client/scheduler_cmds.py
+-rw-rw-r--  2.0 unx     7035 b- defN 23-Jun-26 22:53 nvflare/private/fed/client/scheduler_cmds.py
 -rw-rw-r--  2.0 unx     1139 b- defN 23-May-30 23:31 nvflare/private/fed/client/shell_cmd.py
 -rw-rw-r--  2.0 unx     1974 b- defN 23-May-30 23:31 nvflare/private/fed/client/sys_cmd.py
--rw-rw-r--  2.0 unx     7186 b- defN 23-Jun-26 22:46 nvflare/private/fed/client/training_cmds.py
+-rw-rw-r--  2.0 unx     7322 b- defN 23-Jun-26 22:53 nvflare/private/fed/client/training_cmds.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/private/fed/server/__init__.py
 -rw-rw-r--  2.0 unx    10174 b- defN 23-May-30 23:31 nvflare/private/fed/server/admin.py
 -rw-rw-r--  2.0 unx     9880 b- defN 23-May-30 23:31 nvflare/private/fed/server/client_manager.py
--rw-rw-r--  2.0 unx     8087 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/cmd_utils.py
--rw-rw-r--  2.0 unx    31837 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/fed_server.py
--rw-rw-r--  2.0 unx     7383 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/info_coll_cmd.py
--rw-rw-r--  2.0 unx    30237 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/job_cmds.py
--rw-rw-r--  2.0 unx     8025 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/job_meta_validator.py
--rw-rw-r--  2.0 unx    25377 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/job_runner.py
--rw-rw-r--  2.0 unx     3512 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/message_send.py
+-rw-rw-r--  2.0 unx     8479 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/cmd_utils.py
+-rw-rw-r--  2.0 unx    32128 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/fed_server.py
+-rw-rw-r--  2.0 unx     6671 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/info_coll_cmd.py
+-rw-rw-r--  2.0 unx    30474 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/job_cmds.py
+-rw-rw-r--  2.0 unx     8117 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/job_meta_validator.py
+-rw-rw-r--  2.0 unx    26711 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/job_runner.py
+-rw-rw-r--  2.0 unx     3705 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/message_send.py
 -rw-rw-r--  2.0 unx      929 b- defN 23-May-30 23:31 nvflare/private/fed/server/run_info.py
 -rw-rw-r--  2.0 unx     3870 b- defN 23-May-30 23:31 nvflare/private/fed/server/run_manager.py
--rw-rw-r--  2.0 unx     3456 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/server_app_runner.py
+-rw-rw-r--  2.0 unx     3460 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/server_app_runner.py
 -rw-rw-r--  2.0 unx     1364 b- defN 23-May-30 23:31 nvflare/private/fed/server/server_cmd_modules.py
 -rw-rw-r--  2.0 unx     5546 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/server_command_agent.py
 -rw-rw-r--  2.0 unx    13913 b- defN 23-May-30 23:31 nvflare/private/fed/server/server_commands.py
--rw-rw-r--  2.0 unx    32016 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/server_engine.py
+-rw-rw-r--  2.0 unx    32006 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/server_engine.py
 -rw-rw-r--  2.0 unx     7240 b- defN 23-May-30 23:31 nvflare/private/fed/server/server_engine_internal_spec.py
 -rw-rw-r--  2.0 unx     6163 b- defN 23-May-30 23:31 nvflare/private/fed/server/server_json_config.py
--rw-rw-r--  2.0 unx    22528 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/server_runner.py
+-rw-rw-r--  2.0 unx    22561 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/server_runner.py
 -rw-rw-r--  2.0 unx     6711 b- defN 23-May-30 23:31 nvflare/private/fed/server/server_state.py
 -rw-rw-r--  2.0 unx     1049 b- defN 23-May-30 23:31 nvflare/private/fed/server/server_status.py
--rw-rw-r--  2.0 unx    10418 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/shell_cmd.py
--rw-rw-r--  2.0 unx     6119 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/sys_cmd.py
--rw-rw-r--  2.0 unx    16962 b- defN 23-Jun-26 22:45 nvflare/private/fed/server/training_cmds.py
+-rw-rw-r--  2.0 unx    10824 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/shell_cmd.py
+-rw-rw-r--  2.0 unx     5999 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/sys_cmd.py
+-rw-rw-r--  2.0 unx    17529 b- defN 23-Jun-26 22:53 nvflare/private/fed/server/training_cmds.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/private/fed/simulator/__init__.py
 -rw-rw-r--  2.0 unx     1884 b- defN 23-May-30 23:31 nvflare/private/fed/simulator/simulator_app_runner.py
 -rw-rw-r--  2.0 unx     1030 b- defN 23-May-30 23:31 nvflare/private/fed/simulator/simulator_audit.py
 -rw-rw-r--  2.0 unx     1724 b- defN 23-May-30 23:31 nvflare/private/fed/simulator/simulator_client_engine.py
 -rw-rw-r--  2.0 unx      787 b- defN 23-May-30 23:31 nvflare/private/fed/simulator/simulator_const.py
--rw-rw-r--  2.0 unx     5275 b- defN 23-Jun-26 22:45 nvflare/private/fed/simulator/simulator_server.py
+-rw-rw-r--  2.0 unx     5279 b- defN 23-Jun-26 22:53 nvflare/private/fed/simulator/simulator_server.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/private/fed/utils/__init__.py
 -rw-rw-r--  2.0 unx     2019 b- defN 23-May-30 23:31 nvflare/private/fed/utils/app_authz.py
--rw-rw-r--  2.0 unx     3038 b- defN 23-Jun-26 22:45 nvflare/private/fed/utils/app_deployer.py
--rw-rw-r--  2.0 unx     8154 b- defN 23-Jun-26 22:45 nvflare/private/fed/utils/fed_utils.py
+-rw-rw-r--  2.0 unx     2938 b- defN 23-Jun-26 22:53 nvflare/private/fed/utils/app_deployer.py
+-rw-rw-r--  2.0 unx    10386 b- defN 23-Jun-26 22:53 nvflare/private/fed/utils/fed_utils.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/private/fed/utils/decomposers/__init__.py
 -rw-rw-r--  2.0 unx     1293 b- defN 23-May-30 23:31 nvflare/private/fed/utils/decomposers/private_decomposers.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/security/__init__.py
--rw-rw-r--  2.0 unx     4133 b- defN 23-Jun-26 22:45 nvflare/security/logging.py
+-rw-rw-r--  2.0 unx     4112 b- defN 23-Jun-26 22:53 nvflare/security/logging.py
 -rw-rw-r--  2.0 unx     2875 b- defN 23-May-30 23:31 nvflare/security/security.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/tool/__init__.py
--rw-rw-r--  2.0 unx     4429 b- defN 23-Jun-26 22:45 nvflare/tool/api_utils.py
+-rw-rw-r--  2.0 unx     4432 b- defN 23-Jun-26 22:53 nvflare/tool/api_utils.py
 -rw-rw-r--  2.0 unx     2001 b- defN 23-May-30 23:31 nvflare/tool/preflight_check.py
 -rw-rw-r--  2.0 unx      904 b- defN 23-May-30 23:31 nvflare/tool/package_checker/__init__.py
 -rw-rw-r--  2.0 unx     9553 b- defN 23-May-30 23:31 nvflare/tool/package_checker/check_rule.py
 -rw-rw-r--  2.0 unx     2510 b- defN 23-May-30 23:31 nvflare/tool/package_checker/client_package_checker.py
 -rw-rw-r--  2.0 unx     1075 b- defN 23-May-30 23:31 nvflare/tool/package_checker/nvflare_console_package_checker.py
 -rw-rw-r--  2.0 unx     1990 b- defN 23-May-30 23:31 nvflare/tool/package_checker/overseer_package_checker.py
 -rw-rw-r--  2.0 unx     7550 b- defN 23-May-30 23:31 nvflare/tool/package_checker/package_checker.py
 -rw-rw-r--  2.0 unx     4477 b- defN 23-May-30 23:31 nvflare/tool/package_checker/server_package_checker.py
 -rw-rw-r--  2.0 unx     8198 b- defN 23-May-30 23:31 nvflare/tool/package_checker/utils.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/utils/__init__.py
 -rw-rw-r--  2.0 unx     1452 b- defN 23-May-30 23:31 nvflare/utils/decorators.py
 -rw-rw-r--  2.0 unx      610 b- defN 23-May-30 23:31 nvflare/widgets/__init__.py
 -rw-rw-r--  2.0 unx     3921 b- defN 23-May-30 23:31 nvflare/widgets/comp_caller.py
--rw-rw-r--  2.0 unx     9057 b- defN 23-Jun-26 22:45 nvflare/widgets/fed_event.py
--rw-rw-r--  2.0 unx     8939 b- defN 23-Jun-26 22:45 nvflare/widgets/info_collector.py
+-rw-rw-r--  2.0 unx     9061 b- defN 23-Jun-26 22:53 nvflare/widgets/fed_event.py
+-rw-rw-r--  2.0 unx     8996 b- defN 23-Jun-26 22:53 nvflare/widgets/info_collector.py
 -rw-rw-r--  2.0 unx     1365 b- defN 23-May-30 23:31 nvflare/widgets/widget.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-26 22:46 nvflare-2.3.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6277 b- defN 23-Jun-26 22:46 nvflare-2.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 22:46 nvflare-2.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       45 b- defN 23-Jun-26 22:46 nvflare-2.3.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jun-26 22:46 nvflare-2.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 21-Nov-25 00:35 nvflare-2.3.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx    48790 b- defN 23-Jun-26 22:46 nvflare-2.3.1.dist-info/RECORD
-507 files, 2613667 bytes uncompressed, 780785 bytes compressed:  70.1%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-26 22:54 nvflare-2.4.0rc1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6761 b- defN 23-Jun-26 22:54 nvflare-2.4.0rc1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 22:54 nvflare-2.4.0rc1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       45 b- defN 23-Jun-26 22:54 nvflare-2.4.0rc1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jun-26 22:54 nvflare-2.4.0rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 21-Nov-25 00:35 nvflare-2.4.0rc1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    53800 b- defN 23-Jun-26 22:54 nvflare-2.4.0rc1.dist-info/RECORD
+559 files, 2892085 bytes uncompressed, 864529 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -15,14 +15,17 @@
 
 Filename: nvflare/apis/__init__.py
 Comment: 
 
 Filename: nvflare/apis/analytix.py
 Comment: 
 
+Filename: nvflare/apis/app_deployer_spec.py
+Comment: 
+
 Filename: nvflare/apis/app_validation.py
 Comment: 
 
 Filename: nvflare/apis/aux_spec.py
 Comment: 
 
 Filename: nvflare/apis/client.py
@@ -69,17 +72,23 @@
 
 Filename: nvflare/apis/job_def.py
 Comment: 
 
 Filename: nvflare/apis/job_def_manager_spec.py
 Comment: 
 
+Filename: nvflare/apis/job_meta_validator_spec.py
+Comment: 
+
 Filename: nvflare/apis/job_scheduler_spec.py
 Comment: 
 
+Filename: nvflare/apis/operator_spec.py
+Comment: 
+
 Filename: nvflare/apis/overseer_spec.py
 Comment: 
 
 Filename: nvflare/apis/persistable.py
 Comment: 
 
 Filename: nvflare/apis/resource_manager_spec.py
@@ -162,14 +171,17 @@
 
 Filename: nvflare/app_common/abstract/__init__.py
 Comment: 
 
 Filename: nvflare/app_common/abstract/aggregator.py
 Comment: 
 
+Filename: nvflare/app_common/abstract/fl_model.py
+Comment: 
+
 Filename: nvflare/app_common/abstract/formatter.py
 Comment: 
 
 Filename: nvflare/app_common/abstract/init_final_component.py
 Comment: 
 
 Filename: nvflare/app_common/abstract/learnable.py
@@ -222,14 +234,17 @@
 
 Filename: nvflare/app_common/aggregators/collect_and_assemble_aggregator.py
 Comment: 
 
 Filename: nvflare/app_common/aggregators/dxo_aggregator.py
 Comment: 
 
+Filename: nvflare/app_common/aggregators/dxo_collector.py
+Comment: 
+
 Filename: nvflare/app_common/aggregators/intime_accumulate_model_aggregator.py
 Comment: 
 
 Filename: nvflare/app_common/aggregators/weighted_aggregation_helper.py
 Comment: 
 
 Filename: nvflare/app_common/decomposers/__init__.py
@@ -303,14 +318,26 @@
 
 Filename: nvflare/app_common/homomorphic_encryption/he_pt_model_reader_writer.py
 Comment: 
 
 Filename: nvflare/app_common/homomorphic_encryption/homomorphic_encrypt.py
 Comment: 
 
+Filename: nvflare/app_common/hub/__init__.py
+Comment: 
+
+Filename: nvflare/app_common/hub/hub_app_deployer.py
+Comment: 
+
+Filename: nvflare/app_common/hub/hub_controller.py
+Comment: 
+
+Filename: nvflare/app_common/hub/hub_executor.py
+Comment: 
+
 Filename: nvflare/app_common/job_schedulers/__init__.py
 Comment: 
 
 Filename: nvflare/app_common/job_schedulers/job_scheduler.py
 Comment: 
 
 Filename: nvflare/app_common/np/__init__.py
@@ -471,14 +498,17 @@
 
 Filename: nvflare/app_common/storages/filesystem_storage.py
 Comment: 
 
 Filename: nvflare/app_common/tracking/__init__.py
 Comment: 
 
+Filename: nvflare/app_common/tracking/log_writer.py
+Comment: 
+
 Filename: nvflare/app_common/tracking/track_exception.py
 Comment: 
 
 Filename: nvflare/app_common/tracking/tracker_types.py
 Comment: 
 
 Filename: nvflare/app_common/utils/__init__.py
@@ -486,14 +516,17 @@
 
 Filename: nvflare/app_common/utils/component_utils.py
 Comment: 
 
 Filename: nvflare/app_common/utils/file_utils.py
 Comment: 
 
+Filename: nvflare/app_common/utils/fl_model_utils.py
+Comment: 
+
 Filename: nvflare/app_common/utils/json_utils.py
 Comment: 
 
 Filename: nvflare/app_common/widgets/__init__.py
 Comment: 
 
 Filename: nvflare/app_common/widgets/convert_to_fed_event.py
@@ -654,15 +687,30 @@
 
 Filename: nvflare/app_opt/statistics/visualization/statistics_visualization.py
 Comment: 
 
 Filename: nvflare/app_opt/tracking/__init__.py
 Comment: 
 
-Filename: nvflare/app_opt/tracking/tb_receiver.py
+Filename: nvflare/app_opt/tracking/mlflow/__init__.py
+Comment: 
+
+Filename: nvflare/app_opt/tracking/mlflow/mlflow_receiver.py
+Comment: 
+
+Filename: nvflare/app_opt/tracking/mlflow/mlflow_writer.py
+Comment: 
+
+Filename: nvflare/app_opt/tracking/tb/__init__.py
+Comment: 
+
+Filename: nvflare/app_opt/tracking/tb/tb_receiver.py
+Comment: 
+
+Filename: nvflare/app_opt/tracking/tb/tb_writer.py
 Comment: 
 
 Filename: nvflare/app_opt/xgboost/__init__.py
 Comment: 
 
 Filename: nvflare/app_opt/xgboost/histogram_based/__init__.py
 Comment: 
@@ -768,14 +816,17 @@
 
 Filename: nvflare/fuel/f3/mpm.py
 Comment: 
 
 Filename: nvflare/fuel/f3/stats_pool.py
 Comment: 
 
+Filename: nvflare/fuel/f3/stream_cell.py
+Comment: 
+
 Filename: nvflare/fuel/f3/cellnet/__init__.py
 Comment: 
 
 Filename: nvflare/fuel/f3/cellnet/cbs.py
 Comment: 
 
 Filename: nvflare/fuel/f3/cellnet/cell.py
@@ -792,14 +843,17 @@
 
 Filename: nvflare/fuel/f3/cellnet/net_agent.py
 Comment: 
 
 Filename: nvflare/fuel/f3/cellnet/net_manager.py
 Comment: 
 
+Filename: nvflare/fuel/f3/cellnet/registry.py
+Comment: 
+
 Filename: nvflare/fuel/f3/cellnet/utils.py
 Comment: 
 
 Filename: nvflare/fuel/f3/drivers/__init__.py
 Comment: 
 
 Filename: nvflare/fuel/f3/drivers/aio_conn.py
@@ -864,14 +918,59 @@
 
 Filename: nvflare/fuel/f3/sfm/sfm_conn.py
 Comment: 
 
 Filename: nvflare/fuel/f3/sfm/sfm_endpoint.py
 Comment: 
 
+Filename: nvflare/fuel/f3/streaming/__init__.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/blob_streamer.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/byte_receiver.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/byte_streamer.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/file_streamer.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/object_streamer.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/stream_const.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/stream_types.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/stream_utils.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/tools/__init__.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/tools/file_receiver.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/tools/file_sender.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/tools/receiver.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/tools/sender.py
+Comment: 
+
+Filename: nvflare/fuel/f3/streaming/tools/utils.py
+Comment: 
+
 Filename: nvflare/fuel/flare_api/__init__.py
 Comment: 
 
 Filename: nvflare/fuel/flare_api/api_spec.py
 Comment: 
 
 Filename: nvflare/fuel/flare_api/config.py
@@ -1011,42 +1110,57 @@
 
 Filename: nvflare/fuel/utils/class_utils.py
 Comment: 
 
 Filename: nvflare/fuel/utils/component_builder.py
 Comment: 
 
+Filename: nvflare/fuel/utils/config.py
+Comment: 
+
+Filename: nvflare/fuel/utils/config_factory.py
+Comment: 
+
 Filename: nvflare/fuel/utils/config_service.py
 Comment: 
 
+Filename: nvflare/fuel/utils/constants.py
+Comment: 
+
+Filename: nvflare/fuel/utils/deprecated.py
+Comment: 
+
 Filename: nvflare/fuel/utils/dict_utils.py
 Comment: 
 
 Filename: nvflare/fuel/utils/fsm.py
 Comment: 
 
 Filename: nvflare/fuel/utils/gpu_utils.py
 Comment: 
 
 Filename: nvflare/fuel/utils/import_utils.py
 Comment: 
 
+Filename: nvflare/fuel/utils/json_config_loader.py
+Comment: 
+
 Filename: nvflare/fuel/utils/json_scanner.py
 Comment: 
 
 Filename: nvflare/fuel/utils/network_utils.py
 Comment: 
 
 Filename: nvflare/fuel/utils/obj_utils.py
 Comment: 
 
-Filename: nvflare/fuel/utils/stats_utils.py
+Filename: nvflare/fuel/utils/time_utils.py
 Comment: 
 
-Filename: nvflare/fuel/utils/time_utils.py
+Filename: nvflare/fuel/utils/validation_utils.py
 Comment: 
 
 Filename: nvflare/fuel/utils/wfconf.py
 Comment: 
 
 Filename: nvflare/fuel/utils/zip_utils.py
 Comment: 
@@ -1062,14 +1176,47 @@
 
 Filename: nvflare/fuel/utils/fobs/decomposers/__init__.py
 Comment: 
 
 Filename: nvflare/fuel/utils/fobs/decomposers/core_decomposers.py
 Comment: 
 
+Filename: nvflare/fuel/utils/pipe/__init__.py
+Comment: 
+
+Filename: nvflare/fuel/utils/pipe/file_accessor.py
+Comment: 
+
+Filename: nvflare/fuel/utils/pipe/file_name_utils.py
+Comment: 
+
+Filename: nvflare/fuel/utils/pipe/file_pipe.py
+Comment: 
+
+Filename: nvflare/fuel/utils/pipe/fobs_file_accessor.py
+Comment: 
+
+Filename: nvflare/fuel/utils/pipe/pipe.py
+Comment: 
+
+Filename: nvflare/fuel/utils/pipe/pipe_handler.py
+Comment: 
+
+Filename: nvflare/fuel_opt/__init__.py
+Comment: 
+
+Filename: nvflare/fuel_opt/utils/__init__.py
+Comment: 
+
+Filename: nvflare/fuel_opt/utils/omegaconf_loader.py
+Comment: 
+
+Filename: nvflare/fuel_opt/utils/pyhocon_loader.py
+Comment: 
+
 Filename: nvflare/ha/__init__.py
 Comment: 
 
 Filename: nvflare/ha/dummy_overseer_agent.py
 Comment: 
 
 Filename: nvflare/ha/ha_admin_cmds.py
@@ -1119,14 +1266,17 @@
 
 Filename: nvflare/lighter/service_constants.py
 Comment: 
 
 Filename: nvflare/lighter/spec.py
 Comment: 
 
+Filename: nvflare/lighter/tplt_utils.py
+Comment: 
+
 Filename: nvflare/lighter/utils.py
 Comment: 
 
 Filename: nvflare/lighter/impl/__init__.py
 Comment: 
 
 Filename: nvflare/lighter/impl/cert.py
@@ -1137,14 +1287,20 @@
 
 Filename: nvflare/lighter/impl/he.py
 Comment: 
 
 Filename: nvflare/lighter/impl/helm_chart.py
 Comment: 
 
+Filename: nvflare/lighter/impl/local_cert.py
+Comment: 
+
+Filename: nvflare/lighter/impl/local_static_file.py
+Comment: 
+
 Filename: nvflare/lighter/impl/master_template.yml
 Comment: 
 
 Filename: nvflare/lighter/impl/signature.py
 Comment: 
 
 Filename: nvflare/lighter/impl/static_file.py
@@ -1494,29 +1650,29 @@
 
 Filename: nvflare/widgets/info_collector.py
 Comment: 
 
 Filename: nvflare/widgets/widget.py
 Comment: 
 
-Filename: nvflare-2.3.1.dist-info/LICENSE
+Filename: nvflare-2.4.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: nvflare-2.3.1.dist-info/METADATA
+Filename: nvflare-2.4.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: nvflare-2.3.1.dist-info/WHEEL
+Filename: nvflare-2.4.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: nvflare-2.3.1.dist-info/entry_points.txt
+Filename: nvflare-2.4.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: nvflare-2.3.1.dist-info/top_level.txt
+Filename: nvflare-2.4.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: nvflare-2.3.1.dist-info/zip-safe
+Filename: nvflare-2.4.0rc1.dist-info/zip-safe
 Comment: 
 
-Filename: nvflare-2.3.1.dist-info/RECORD
+Filename: nvflare-2.4.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvflare/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-06-26T15:18:53-0400",
+ "date": "2023-06-26T16:38:47-0400",
  "dirty": false,
  "error": null,
- "full-revisionid": "2994afc55927f38461ea52fac8c487f126cb18e5",
- "version": "2.3.1"
+ "full-revisionid": "430521af4375505ce66ed90929e385f46693132b",
+ "version": "2.4.0rc1"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## nvflare/apis/analytix.py

```diff
@@ -9,18 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from enum import Enum
-from typing import Dict, Optional
 
 from nvflare.apis.dxo import DXO, DataKind
-from nvflare.app_common.tracking.tracker_types import TrackConst, Tracker
+from nvflare.app_common.tracking.tracker_types import LogWriterName, TrackConst
 
 _DATA_TYPE_KEY = "analytics_data_type"
 _KWARGS_KEY = "analytics_kwargs"
 
 
 class AnalyticsDataType(Enum):
     SCALARS = "SCALARS"
@@ -43,65 +42,62 @@
 
 class AnalyticsData:
     def __init__(
         self,
         key: str,
         value,
         data_type: AnalyticsDataType,
-        sender: Tracker = Tracker.TORCH_TB,
-        kwargs: Optional[dict] = None,
-        step: Optional[int] = None,
-        path: Optional[str] = None,
+        sender: LogWriterName = LogWriterName.TORCH_TB,
+        **kwargs,
     ):
         """This class defines AnalyticsData format.
 
         It is a wrapper to provide to/from DXO conversion.
 
         Args:
             key (str): tag name
             value: value
             data_type (AnalyticDataType): type of the analytic data.
-            sender (Tracker): Syntax of Tracker such as Tensorboard or MLFLow
+            sender (LogWriterName): Type of sender for syntax such as Tensorboard or MLflow
             kwargs (optional, dict): additional arguments to be passed.
         """
-        self._validate_data_types(data_type, kwargs, key, value, step, path)
+        self._validate_data_types(data_type, key, value, **kwargs)
         self.tag = key
         self.value = value
         self.data_type = data_type
         self.kwargs = kwargs
-        self.step = step
-        self.path = path
         self.sender = sender
+        self.step = kwargs.get(TrackConst.GLOBAL_STEP_KEY, None)
+        self.path = kwargs.get(TrackConst.PATH_KEY, None)
 
     def to_dxo(self):
         """Converts the AnalyticsData to DXO object.
 
         Returns:
             DXO object
         """
 
         data = {TrackConst.TRACK_KEY: self.tag, TrackConst.TRACK_VALUE: self.value}
-        if self.step:
+        if self.step is not None:
             data[TrackConst.GLOBAL_STEP_KEY] = self.step
         if self.path:
             data[TrackConst.PATH_KEY] = self.path
         if self.kwargs:
             data[TrackConst.KWARGS_KEY] = self.kwargs
         dxo = DXO(data_kind=DataKind.ANALYTIC, data=data)
         dxo.set_meta_prop(TrackConst.DATA_TYPE_KEY, self.data_type)
         dxo.set_meta_prop(TrackConst.TRACKER_KEY, self.sender)
         return dxo
 
     @classmethod
-    def from_dxo(cls, dxo: DXO, receiver: Tracker = Tracker.TORCH_TB):
+    def from_dxo(cls, dxo: DXO, receiver: LogWriterName = LogWriterName.TORCH_TB):
         """Generates the AnalyticsData from DXO object.
 
         Args:
-            receiver: type experiment tacker, default to Tensorboard. TrackerType.TORCH_TB
-            sender: type experiment tacker, default to Tensorboard. TrackerType.TORCH_TB
+            receiver: type of the experiment tacker, defaults to Tensorboard with LogWriterName.TORCH_TB.
             dxo (DXO): The DXO object to convert.
 
         Returns:
             AnalyticsData object
         """
         if not isinstance(dxo, DXO):
             raise TypeError("expect dxo to be an instance of DXO, but got {}.".format(type(dxo)))
@@ -109,45 +105,53 @@
         if len(dxo.data) == 0:
             raise ValueError(
                 "dxo does not have the correct format for AnalyticsData; expected dxo.data to be length > 0, but got 0"
             )
         data = dxo.data
         key = data[TrackConst.TRACK_KEY]
         value = data[TrackConst.TRACK_VALUE]
-        step = data[TrackConst.GLOBAL_STEP_KEY] if TrackConst.GLOBAL_STEP_KEY in data else None
-        path = data[TrackConst.PATH_KEY] if TrackConst.PATH_KEY in data else None
-        kwargs = data[TrackConst.KWARGS_KEY] if TrackConst.KWARGS_KEY in data else None
+        kwargs = data.get(TrackConst.KWARGS_KEY, {})
+        step = data.get(TrackConst.GLOBAL_STEP_KEY, None)
+        if step is not None:
+            kwargs[TrackConst.GLOBAL_STEP_KEY] = step
         data_type = dxo.get_meta_prop(TrackConst.DATA_TYPE_KEY)
-        sender = dxo.get_meta_prop(TrackConst.TRACKER_KEY)
-        if sender is not None and sender != receiver:
-            data_type = cls.convert_data_type(data_type, sender, receiver)
-        return cls(key, value, data_type, sender, kwargs, step, path)
+        writer = dxo.get_meta_prop(TrackConst.TRACKER_KEY)
+        if writer is not None and writer != receiver:
+            data_type = cls.convert_data_type(data_type, writer, receiver)
+
+        if not data_type:
+            return None
+
+        if not kwargs:
+            return cls(key, value, data_type, writer)
+        else:
+            return cls(key, value, data_type, writer, **kwargs)
 
     def _validate_data_types(
         self,
         data_type: AnalyticsDataType,
-        kwargs: Optional[Dict],
         key: str,
         value: any,
-        step: Optional[int] = None,
-        path: Optional[str] = None,
+        **kwargs,
     ):
         if not isinstance(key, str):
             raise TypeError("expect tag to be an instance of str, but got {}.".format(type(key)))
         if not isinstance(data_type, AnalyticsDataType):
             raise TypeError(
                 "expect data_type to be an instance of AnalyticsDataType, but got {}.".format(type(data_type))
             )
         if kwargs and not isinstance(kwargs, dict):
             raise TypeError("expect kwargs to be an instance of dict, but got {}.".format(type(kwargs)))
+        step = kwargs.get(TrackConst.GLOBAL_STEP_KEY, None)
         if step:
             if not isinstance(step, int):
                 raise TypeError("expect step to be an instance of int, but got {}.".format(type(step)))
             if step < 0:
                 raise ValueError("expect step to be non-negative int, but got {}.".format(step))
+        path = kwargs.get(TrackConst.PATH_KEY, None)
         if path and not isinstance(path, str):
             raise TypeError("expect path to be an instance of str, but got {}.".format(type(step)))
         if data_type in [AnalyticsDataType.SCALAR, AnalyticsDataType.METRIC] and not isinstance(value, float):
             raise TypeError(f"expect '{key}' value to be an instance of float, but got '{type(value)}'.")
         elif data_type in [
             AnalyticsDataType.METRICS,
             AnalyticsDataType.PARAMETERS,
@@ -159,29 +163,32 @@
         elif data_type == AnalyticsDataType.TAGS and not isinstance(value, dict):
             raise TypeError(
                 f"expect '{key}' data type expects value to be an instance of dict, but got '{type(value)}'"
             )
 
     @classmethod
     def convert_data_type(
-        cls, sender_data_type: AnalyticsDataType, sender: Tracker, receiver: Tracker
+        cls, sender_data_type: AnalyticsDataType, sender: LogWriterName, receiver: LogWriterName
     ) -> AnalyticsDataType:
 
-        if sender == Tracker.TORCH_TB and receiver == Tracker.MLFLOW:
+        if sender == LogWriterName.TORCH_TB and receiver == LogWriterName.MLFLOW:
             if AnalyticsDataType.SCALAR == sender_data_type:
                 return AnalyticsDataType.METRIC
             elif AnalyticsDataType.SCALARS == sender_data_type:
                 return AnalyticsDataType.METRICS
             else:
                 return sender_data_type
 
-        if sender == Tracker.MLFLOW and receiver == Tracker.TORCH_TB:
+        if sender == LogWriterName.MLFLOW and receiver == LogWriterName.TORCH_TB:
             if AnalyticsDataType.PARAMETER == sender_data_type:
                 return AnalyticsDataType.SCALAR
             elif AnalyticsDataType.PARAMETERS == sender_data_type:
                 return AnalyticsDataType.SCALARS
             elif AnalyticsDataType.METRIC == sender_data_type:
                 return AnalyticsDataType.SCALAR
             elif AnalyticsDataType.METRICS == sender_data_type:
                 return AnalyticsDataType.SCALARS
             else:
                 return sender_data_type
+
+    def __str__(self) -> str:
+        return f"AnalyticsData(tag: {self.tag}, value: {self.value}, data_type: {self.data_type}, kwargs: {self.kwargs}, step: {self.step})"
```

## nvflare/apis/controller_spec.py

```diff
@@ -33,25 +33,54 @@
     ERROR = "error"
     CANCELLED = "cancelled"
     ABORTED = "aborted"
     IGNORED = "ignored"
     CLIENT_DEAD = "client_dead"
 
 
+class TaskOperatorKey:
+
+    OP_ID = "op_id"
+    METHOD = "method"  # bcast, relay, etc.
+    NUM_ROUNDS = "num_rounds"
+    TARGETS = "targets"  # list of leaf nodes
+    DATA_FILTERS = "data_filters"
+    RESULT_FILTERS = "result_filters"
+    AGGREGATOR = "aggregator"  # only for bcast
+    SHAREABLE_GENERATOR = "shareable_gen"  # only for relay
+    PERSISTOR = "persistor"  # only for relay
+    TIMEOUT = "timeout"
+    TASK_ASSIGNMENT_TIMEOUT = "task_assign_timeout"  # for relay
+    MIN_TARGETS = "min_targets"
+    WAIT_TIME_AFTER_MIN_RESPS = "wait_time_after_min_received"
+
+
+class OperatorMethod:
+
+    BROADCAST = "bcast"
+    RELAY = "relay"
+
+
+class OperatorConfigKey:
+
+    OPERATORS = "operators"
+
+
 class Task(object):
     def __init__(
         self,
         name: str,
         data: Shareable,
         props: Optional[Dict] = None,
         timeout: int = 0,
         before_task_sent_cb=None,
         after_task_sent_cb=None,
         result_received_cb=None,
         task_done_cb=None,
+        operator=None,
     ):
         """Init the Task.
 
         A task is a piece of work that is assigned by the Controller to client workers.
         Depending on how the task is assigned (broadcast, send, or relay), the task will be performed by one or more clients.
 
         Args:
@@ -63,24 +92,29 @@
                 It needs to follow the before_task_sent_cb_signature.
             after_task_sent_cb: If provided, this callback would be called after controller sends the tasks to clients.
                 It needs to follow the after_task_sent_cb_signature.
             result_received_cb: If provided, this callback would be called when controller receives results from clients.
                 It needs to follow the result_received_cb_signature.
             task_done_cb: If provided, this callback would be called when task is done.
                 It needs to follow the task_done_cb_signature.
+            operator: task operator that describes the operation of the task
 
         """
         if not isinstance(name, str):
             raise TypeError("name must be str, but got {}.".format(type(name)))
 
         if not isinstance(data, Shareable):
             raise TypeError("data must be an instance of Shareable, but got {}.".format(type(data)))
 
+        if operator and not isinstance(operator, dict):
+            raise TypeError(f"operator must be a dict but got {type(operator)}")
+
         self.name = name  # name of the task
         self.data = data  # task data to be sent to client(s)
+        self.operator = operator
         self.cb_lock = threading.Lock()
 
         if props is None:
             self.props = {}
         else:
             if not isinstance(props, dict):
                 raise TypeError("props must be None or dict, but got {}.".format(type(props)))
```

## nvflare/apis/dxo.py

```diff
@@ -16,14 +16,15 @@
 from typing import List, Union
 
 from nvflare.apis.shareable import ReservedHeaderKey, Shareable
 from nvflare.fuel.utils import fobs
 
 
 class DataKind(object):
+    FL_MODEL = "FL_MODEL"
     WEIGHTS = "WEIGHTS"
     WEIGHT_DIFF = "WEIGHT_DIFF"
     XGB_MODEL = "XGB_MODEL"
     METRICS = "METRICS"
     ANALYTIC = "ANALYTIC"
     COLLECTION = "COLLECTION"  # Dict or List of DXO objects
     STATISTICS = "STATISTICS"
@@ -33,14 +34,20 @@
 class MetaKey(object):
     NUM_STEPS_CURRENT_ROUND = "NUM_STEPS_CURRENT_ROUND"
     PROCESSED_ALGORITHM = "PROCESSED_ALGORITHM"
     PROCESSED_KEYS = "PROCESSED_KEYS"
     INITIAL_METRICS = "initial_metrics"
     FILTER_HISTORY = "filter_history"
 
+    CONFIGS = "configs"
+    VALIDATE_TYPE = "validate_type"
+    CLIENT_WEIGHTS = "client_weights"
+    CURRENT_ROUND = "current_round"
+    TOTAL_ROUNDS = "total_rounds"
+
 
 _KEY_KIND = "kind"
 _KEY_DATA = "data"
 _KEY_META = "meta"
 _KEY_DXO = "DXO"
 
 
@@ -185,7 +192,47 @@
 
     """
     x = fobs.loads(data)
     if isinstance(x, DXO):
         return x
     else:
         raise ValueError("Data bytes are from type {} and do not represent a valid DXO instance.".format(type(x)))
+
+
+def get_leaf_dxos(dxo: DXO, root_name: str = "") -> (dict, list):
+    """Traverse the specified dxo tree and return all leaf DXOs.
+    The input dxo is a simple DXO or a collection DXO as a dict of DXOs.
+
+    Args:
+        dxo: the DXO object to be traversed
+        root_name: the root name of the DXO
+
+    Returns: a dict of dxo_path => DXO object. The dxo path is the full path from the root to the leaf node,
+    concatenation of all node names, separated by dots.
+    A list of errors encountered during traversing.
+
+    """
+    result = {}
+    errors = []
+    _traverse(dxo, root_name, result, errors, {})
+    return result, errors
+
+
+def _traverse(dxo: DXO, name: str, result, errors, visited: dict):
+    obj_id = id(dxo)
+    if visited.get(obj_id):
+        print(f"dxo {name} already visited - ignore it")
+        return
+    visited[obj_id] = True
+
+    if not isinstance(dxo, DXO):
+        errors.append(f"dxo '{name}' must be DXO but got {type(dxo)}")
+        return
+
+    if dxo.data_kind == DataKind.COLLECTION:
+        if not isinstance(dxo.data, dict):
+            errors.append(f"dxo '{name}' is a collection but data is {type(dxo.data)} - must be dict")
+            return
+        for k, v in dxo.data.items():
+            _traverse(v, f"{name}.{k}", result, errors, visited)
+    else:
+        result[name] = dxo
```

## nvflare/apis/filter.py

```diff
@@ -15,15 +15,15 @@
 from abc import ABC, abstractmethod
 
 from nvflare.apis.fl_component import FLComponent
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.shareable import Shareable
 
 
-class ContentBlockedException(Exception):
+class ContentBlockedException(BaseException):
     """
     A filter should raise this exception when the content is to be blocked
     """
 
     pass
```

## nvflare/apis/fl_constant.py

```diff
@@ -35,16 +35,16 @@
     TASK_UNKNOWN = "TASK_UNKNOWN"
     TASK_UNSUPPORTED = "TASK_UNSUPPORTED"
     TOPIC_UNKNOWN = "TOPIC_UNKNOWN"
     MODEL_UNRECOGNIZED = "MODEL_UNRECOGNIZED"
     VALIDATE_TYPE_UNKNOWN = "VALIDATE_TYPE_UNKNOWN"
     EMPTY_RESULT = "EMPTY_RESULT"
     UNSAFE_JOB = "UNSAFE_JOB"
-
     SERVER_NOT_READY = "SERVER_NOT_READY"
+    SERVICE_UNAVAILABLE = "SERVICE_UNAVAILABLE"
 
 
 class MachineStatus(Enum):
     """Constants for machine status.
 
     Status Lifecycle
         STOPPED <-> STARTING -> STARTED -> STOPPING -> STOPPED
@@ -297,55 +297,64 @@
     JOB_RUNNER = "job_runner"
     SERVER_RUNNER = "server_runner"
     CLIENT_RUNNER = "client_runner"
     CHECK_RESOURCE_PROCESSOR = "check_resource_processor"
     CANCEL_RESOURCE_PROCESSOR = "cancel_resource_processor"
     RESOURCE_MANAGER = "resource_manager"
     RESOURCE_CONSUMER = "resource_consumer"
+    APP_DEPLOYER = "app_deployer"
+    DEFAULT_APP_DEPLOYER = "default_app_deployer"
+    JOB_META_VALIDATOR = "job_meta_validator"
+
+
+class JobConstants:
+    SERVER_JOB_CONFIG = "config_fed_server.json"
+    CLIENT_JOB_CONFIG = "config_fed_client.json"
+    META_FILE = "meta.json"
 
 
 class WorkspaceConstants:
     """hard coded file names inside the workspace folder."""
 
     STARTUP_FOLDER_NAME = "startup"
     SITE_FOLDER_NAME = "local"
     CUSTOM_FOLDER_NAME = "custom"
 
     LOGGING_CONFIG = "log.config"
     DEFAULT_LOGGING_CONFIG = LOGGING_CONFIG + ".default"
     AUDIT_LOG = "audit.log"
     LOG_FILE_NAME = "log.txt"
+    STATS_POOL_SUMMARY_FILE_NAME = "stats_pool_summary.json"
+    STATS_POOL_RECORDS_FILE_NAME = "stats_pool_records.csv"
 
     # these two files is used by shell scripts to determine restart / shutdown
     RESTART_FILE = "restart.fl"
     SHUTDOWN_FILE = "shutdown.fl"
 
     WORKSPACE_PREFIX = ""
     APP_PREFIX = "app_"
 
     SERVER_STARTUP_CONFIG = "fed_server.json"
     CLIENT_STARTUP_CONFIG = "fed_client.json"
+
+    SERVER_APP_CONFIG = JobConstants.SERVER_JOB_CONFIG
+    CLIENT_APP_CONFIG = JobConstants.CLIENT_JOB_CONFIG
+
     JOB_META_FILE = "meta.json"
 
     AUTHORIZATION_CONFIG = "authorization.json"
     DEFAULT_AUTHORIZATION_CONFIG = AUTHORIZATION_CONFIG + ".default"
     RESOURCES_CONFIG = "resources.json"
     DEFAULT_RESOURCES_CONFIG = RESOURCES_CONFIG + ".default"
     PRIVACY_CONFIG = "privacy.json"
     SAMPLE_PRIVACY_CONFIG = PRIVACY_CONFIG + ".sample"
 
     ADMIN_STARTUP_CONFIG = "fed_admin.json"
 
 
-class JobConstants:
-    SERVER_JOB_CONFIG = "config_fed_server.json"
-    CLIENT_JOB_CONFIG = "config_fed_client.json"
-    META_FILE = "meta.json"
-
-
 class SiteType:
     SERVER = "server"
     CLIENT = "client"
     ALL = "@ALL"
 
 
 class SystemConfigs:
```

## nvflare/apis/job_def.py

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+import uuid
 from enum import Enum
 from typing import Dict, List, Optional
 
 from nvflare.apis.fl_constant import SystemComponents
 from nvflare.apis.fl_context import FLContext
 
 # this is treated as all online sites in job deploy_map
@@ -66,14 +66,16 @@
     DURATION = "duration"
     JOB_DEPLOY_DETAIL = "job_deploy_detail"
     SCHEDULE_COUNT = "schedule_count"
     SCOPE = "scope"
     CLONED_FROM = "cloned_from"
     LAST_SCHEDULE_TIME = "last_schedule_time"
     SCHEDULE_HISTORY = "schedule_history"
+    STATS_POOL_CONFIG = "stats_pool_config"
+    FROM_HUB_SITE = "from_hub_site"
 
     def __repr__(self):
         return self.value
 
 
 class TopDir(object):
     JOB = "job"
@@ -184,7 +186,25 @@
         resource_spec=meta.get(JobMetaKey.RESOURCE_SPEC, {}),
         deploy_map=meta.get(JobMetaKey.DEPLOY_MAP, {}),
         meta=meta,
         min_sites=meta.get(JobMetaKey.MIN_CLIENTS, 1),
         required_sites=meta.get(JobMetaKey.MANDATORY_CLIENTS, []),
     )
     return job
+
+
+def new_job_id() -> str:
+    return str(uuid.uuid4())
+
+
+def is_valid_job_id(jid: str) -> bool:
+    if not isinstance(jid, str):
+        return False
+
+    try:
+        val = uuid.UUID(jid, version=4)
+    except ValueError:
+        return False
+
+    # If the jid string is a valid hex code, but an invalid uuid4,the UUID.__init__ will convert it to a
+    # valid uuid4. This is bad for validation purposes.
+    return val.hex == jid.replace("-", "")
```

## nvflare/apis/shareable.py

```diff
@@ -26,14 +26,15 @@
     PEER_PROPS = "__peer_props__"
     REPLY_IS_LATE = "__reply_is_late__"
     TASK_NAME = ReservedKey.TASK_NAME
     TASK_ID = ReservedKey.TASK_ID
     WORKFLOW = ReservedKey.WORKFLOW
     AUDIT_EVENT_ID = ReservedKey.AUDIT_EVENT_ID
     CONTENT_TYPE = "__content_type__"
+    TASK_OPERATOR = "__task_operator__"
 
 
 class Shareable(dict):
     """The information communicated between server and client.
 
     Shareable is just a dict that can have any keys and values, defined by developers and users.
     It is recommended that keys are strings. Values must be serializable.
```

## nvflare/apis/workspace.py

```diff
@@ -104,14 +104,20 @@
     def get_file_path_in_root(self, file_basename: str):
         return os.path.join(self.root_dir, file_basename)
 
     def get_server_startup_file_path(self):
         # this is to get the full path to "fed_server.json"
         return self.get_file_path_in_startup(WorkspaceConstants.SERVER_STARTUP_CONFIG)
 
+    def get_server_app_config_file_path(self, job_id):
+        return os.path.join(self.get_app_config_dir(job_id), WorkspaceConstants.SERVER_APP_CONFIG)
+
+    def get_client_app_config_file_path(self, job_id):
+        return os.path.join(self.get_app_config_dir(job_id), WorkspaceConstants.CLIENT_APP_CONFIG)
+
     def get_client_startup_file_path(self):
         # this is to get the full path to "fed_client.json"
         return self.get_file_path_in_startup(WorkspaceConstants.CLIENT_STARTUP_CONFIG)
 
     def get_admin_startup_file_path(self):
         # this is to get the full path to "fed_admin.json"
         return self.get_file_path_in_startup(WorkspaceConstants.ADMIN_STARTUP_CONFIG)
@@ -153,7 +159,19 @@
         return os.path.join(self.get_run_dir(job_id), WorkspaceConstants.JOB_META_FILE)
 
     def get_site_privacy_file_path(self):
         return self.get_file_path_in_site_config(WorkspaceConstants.PRIVACY_CONFIG)
 
     def get_client_custom_dir(self) -> str:
         return os.path.join(self.get_site_config_dir(), WorkspaceConstants.CUSTOM_FOLDER_NAME)
+
+    def get_stats_pool_summary_path(self, job_id: str, prefix=None) -> str:
+        file_name = WorkspaceConstants.STATS_POOL_SUMMARY_FILE_NAME
+        if prefix:
+            file_name = f"{prefix}.{file_name}"
+        return os.path.join(self.get_run_dir(job_id), file_name)
+
+    def get_stats_pool_records_path(self, job_id: str, prefix=None) -> str:
+        file_name = WorkspaceConstants.STATS_POOL_RECORDS_FILE_NAME
+        if prefix:
+            file_name = f"{prefix}.{file_name}"
+        return os.path.join(self.get_run_dir(job_id), file_name)
```

## nvflare/apis/impl/controller.py

```diff
@@ -18,15 +18,15 @@
 from typing import List, Optional, Tuple, Union
 
 from nvflare.apis.client import Client
 from nvflare.apis.controller_spec import ClientTask, ControllerSpec, SendOrder, Task, TaskCompletionStatus
 from nvflare.apis.fl_constant import FLContextKey, ReservedTopic
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.responder import Responder
-from nvflare.apis.shareable import Shareable, make_copy
+from nvflare.apis.shareable import ReservedHeaderKey, Shareable, make_copy
 from nvflare.apis.signal import Signal
 from nvflare.fuel.utils.config_service import ConfigService
 from nvflare.security.logging import secure_format_exception
 from nvflare.widgets.info_collector import GroupInfoCollector, InfoCollector
 
 from .any_relay_manager import AnyRelayTaskManager
 from .bcast_manager import BcastForeverTaskManager, BcastTaskManager
@@ -241,15 +241,15 @@
         with task.cb_lock:
             # Note: must guarantee the after_task_sent_cb is always called
             # regardless whether the task is sent successfully.
             # This is so that the app could clear up things in after_task_sent_cb.
             if task.before_task_sent_cb is not None:
                 try:
                     task.before_task_sent_cb(client_task=client_task_to_send, fl_ctx=fl_ctx)
-                except Exception as e:
+                except BaseException as e:
                     self.log_exception(
                         fl_ctx,
                         "processing error in before_task_sent_cb on task {} ({}): {}".format(
                             client_task_to_send.task.name, client_task_to_send.id, secure_format_exception(e)
                         ),
                     )
                     # this task cannot proceed anymore
@@ -262,19 +262,20 @@
             if task.completion_status is not None:
                 can_send_task = False
 
             # remember the task name and data to be sent to the client
             # since task.data could be reset by the after_task_sent_cb
             task_name = task.name
             task_data = task.data
+            operator = task.operator
 
             if task.after_task_sent_cb is not None:
                 try:
                     task.after_task_sent_cb(client_task=client_task_to_send, fl_ctx=fl_ctx)
-                except Exception as e:
+                except BaseException as e:
                     self.log_exception(
                         fl_ctx,
                         "processing error in after_task_sent_cb on task {} ({}): {}".format(
                             client_task_to_send.task.name, client_task_to_send.id, secure_format_exception(e)
                         ),
                     )
                     task.completion_status = TaskCompletionStatus.ERROR
@@ -291,18 +292,23 @@
 
         with self._task_lock:
             # sent the ClientTask and remember it
             now = time.time()
             client_task_to_send.task_sent_time = now
             client_task_to_send.task_send_count += 1
 
+            # add task operator to task_data shareable
+            if operator:
+                task_data.set_header(key=ReservedHeaderKey.TASK_OPERATOR, value=operator)
+
             if not resend_task:
                 task.last_client_task_map[client.name] = client_task_to_send
                 task.client_tasks.append(client_task_to_send)
                 self._client_task_map[client_task_to_send.id] = client_task_to_send
+
             return task_name, client_task_to_send.id, make_copy(task_data)
 
     def handle_exception(self, task_id: str, fl_ctx: FLContext) -> None:
         """Called to cancel one task as its client_task is causing exception at upper level.
 
         Args:
             task_id (str): an id to the failing client_task
@@ -404,15 +410,15 @@
             manager = task.props[_TASK_KEY_MANAGER]
             manager.check_task_result(result, client_task, fl_ctx)
 
             if task.result_received_cb is not None:
                 try:
                     self.log_debug(fl_ctx, "invoking result_received_cb ...")
                     task.result_received_cb(client_task=client_task, fl_ctx=fl_ctx)
-                except Exception as e:
+                except BaseException as e:
                     # this task cannot proceed anymore
                     self.log_exception(
                         fl_ctx,
                         "processing error in result_received_cb on task {}({}): {}".format(
                             task_name, task_id, secure_format_exception(e)
                         ),
                     )
@@ -901,15 +907,15 @@
                     self.log_info(
                         fl_ctx, "task {} exit with status {}".format(exit_task.name, exit_task.completion_status)
                     )
 
                     if exit_task.task_done_cb is not None:
                         try:
                             exit_task.task_done_cb(task=exit_task, fl_ctx=fl_ctx)
-                        except Exception as e:
+                        except BaseException as e:
                             self.log_exception(
                                 fl_ctx,
                                 "processing error in task_done_cb error on task {}: {}".format(
                                     exit_task.name, secure_format_exception(e)
                                 ),
                             )
                             exit_task.completion_status = TaskCompletionStatus.ERROR
```

## nvflare/apis/impl/job_def_manager.py

```diff
@@ -14,20 +14,20 @@
 
 import datetime
 import os
 import pathlib
 import shutil
 import tempfile
 import time
-import uuid
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional
 
+from nvflare.apis.client_engine_spec import ClientEngineSpec
 from nvflare.apis.fl_context import FLContext
-from nvflare.apis.job_def import Job, JobDataKey, JobMetaKey, job_from_meta
+from nvflare.apis.job_def import Job, JobDataKey, JobMetaKey, job_from_meta, new_job_id
 from nvflare.apis.job_def_manager_spec import JobDefManagerSpec, RunStatus
 from nvflare.apis.server_engine_spec import ServerEngineSpec
 from nvflare.apis.storage import StorageException, StorageSpec
 from nvflare.fuel.utils import fobs
 from nvflare.fuel.utils.zip_utils import unzip_all_from_bytes, zip_directory_to_bytes
 
 
@@ -78,30 +78,33 @@
         super().__init__()
         self.uri_root = uri_root
         os.makedirs(uri_root, exist_ok=True)
         self.job_store_id = job_store_id
 
     def _get_job_store(self, fl_ctx):
         engine = fl_ctx.get_engine()
-        if not isinstance(engine, ServerEngineSpec):
-            raise TypeError(f"engine should be of type ServerEngineSpec, but got {type(engine)}")
+
+        if not (isinstance(engine, ServerEngineSpec) or isinstance(engine, ClientEngineSpec)):
+            raise TypeError(f"engine should be of type ServerEngineSpec or ClientEngineSpec, but got {type(engine)}")
         store = engine.get_component(self.job_store_id)
         if not isinstance(store, StorageSpec):
             raise TypeError(f"engine should have a job store component of type StorageSpec, but got {type(store)}")
         return store
 
     def job_uri(self, jid: str):
         return os.path.join(self.uri_root, jid)
 
     def create(self, meta: dict, uploaded_content: bytes, fl_ctx: FLContext) -> Dict[str, Any]:
         # validate meta to make sure it has:
+        jid = meta.get(JobMetaKey.JOB_ID.value, None)
+        if not jid:
+            jid = new_job_id()
+            meta[JobMetaKey.JOB_ID.value] = jid
 
-        jid = str(uuid.uuid4())
         now = time.time()
-        meta[JobMetaKey.JOB_ID.value] = jid
         meta[JobMetaKey.SUBMIT_TIME.value] = now
         meta[JobMetaKey.SUBMIT_TIME_ISO.value] = datetime.datetime.fromtimestamp(now).astimezone().isoformat()
         meta[JobMetaKey.START_TIME.value] = ""
         meta[JobMetaKey.DURATION.value] = "N/A"
         meta[JobMetaKey.STATUS.value] = RunStatus.SUBMITTED.value
 
         # write it to the store
```

## nvflare/apis/utils/fl_context_utils.py

```diff
@@ -27,15 +27,15 @@
 def get_serializable_data(fl_ctx: FLContext):
     new_fl_ctx = FLContext()
     for k, v in fl_ctx.props.items():
         if k not in NonSerializableKeys.KEYS:
             try:
                 fobs.dumps(v)
                 new_fl_ctx.props[k] = v
-            except Exception as e:
+            except BaseException as e:
                 msg = f"Object in FLContext with key {k} and type {type(v)} is not serializable (discarded): {secure_format_exception(e)}"
                 logger.warning(generate_log_message(fl_ctx, msg))
 
     return new_fl_ctx
 
 
 def generate_log_message(fl_ctx: FLContext, msg: str):
```

## nvflare/apis/utils/job_utils.py

```diff
@@ -16,15 +16,15 @@
 import json
 import os
 from typing import Optional
 from zipfile import ZipFile
 
 from nvflare.apis.fl_constant import JobConstants
 from nvflare.apis.job_def import ALL_SITES, JobMetaKey
-from nvflare.fuel.utils.zip_utils import normpath_for_zip
+from nvflare.fuel.utils.zip_utils import normpath_for_zip, zip_directory_to_bytes
 
 
 def _get_default_meta(job_folder_name: str) -> str:
     # A format string for the dummy meta.json
     meta = f"""{{
                  "{JobMetaKey.JOB_NAME.value}": "{job_folder_name}",
                  "{JobMetaKey.JOB_FOLDER_NAME.value}": "{job_folder_name}",
@@ -77,7 +77,22 @@
                     name = info.filename
                     content = in_zip.read(name)
                     path = folder_name + "/" + name
                     info.filename = path
                     out_zip.writestr(info, content)
 
         return writer.getvalue()
+
+
+def load_job_def_bytes(from_path: str, def_name: str) -> bytes:
+    """Load a job definition from specified path and return zipped bytes
+
+    Args:
+        from_path: path where the job definition is located
+        def_name: name of the job
+
+    Returns:
+
+    """
+    # zip the job folder
+    data = zip_directory_to_bytes(from_path, def_name)
+    return convert_legacy_zipped_app_to_job(data)
```

## nvflare/app_common/abstract/aggregator.py

```diff
@@ -16,14 +16,25 @@
 
 from nvflare.apis.fl_component import FLComponent
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.shareable import Shareable
 
 
 class Aggregator(FLComponent, ABC):
+    def reset(self, fl_ctx: FLContext):
+        """Reset the internal state of the aggregator.
+
+        Args:
+            fl_ctx: FLContext
+
+        Returns:
+
+        """
+        pass
+
     @abstractmethod
     def accept(self, shareable: Shareable, fl_ctx: FLContext) -> bool:
         """Accept the shareable submitted by the client.
 
         Args:
             shareable: submitted Shareable object
             fl_ctx: FLContext
```

## nvflare/app_common/aggregators/accumulate_model_aggregator.py

```diff
@@ -8,16 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from nvflare.fuel.utils.deprecated import deprecated
+
 from .intime_accumulate_model_aggregator import InTimeAccumulateWeightedAggregator
 
 
+@deprecated("Please use 'InTimeAccumulateWeightedAggregator'")
 class AccumulateWeightedAggregator(InTimeAccumulateWeightedAggregator):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.logger.warning(
-            "'AccumulateWeightedAggregator' was deprecated, please use " "'InTimeAccumulateWeightedAggregator'"
-        )
+    pass
```

## nvflare/app_common/aggregators/assembler.py

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABC, abstractmethod
 from typing import Dict
 
+from nvflare.apis.dxo import DXO
 from nvflare.apis.fl_component import FLComponent
 from nvflare.apis.fl_context import FLContext
 
 
 class Assembler(FLComponent, ABC):
     """Assembler class for aggregation functionality
     This defines the functionality of assembling the collected submissions
@@ -38,31 +39,31 @@
     def collection(self):
         return self._collection
 
     def get_expected_data_kind(self):
         return self.expected_data_kind
 
     @abstractmethod
-    def get_model_params(self, data: dict) -> dict:
+    def get_model_params(self, dxo: DXO) -> dict:
         """Connects the assembler's _collection with CollectAndAssembleAggregator
         Get the collected parameters from the main aggregator
         Return:
             A dict of parameters needed for further assembling
         """
         raise NotImplementedError
 
     @abstractmethod
-    def assemble(self, data: Dict[str, dict], fl_ctx: FLContext) -> dict:
+    def assemble(self, data: Dict[str, dict], fl_ctx: FLContext) -> DXO:
         """Assemble the collected submissions.
         This will be specified according to the specific algorithm
         E.g. global svm round on the collected local supporting vectors;
         global k-means step on the local centroids and counts
 
         Return:
-            A dict of parameters to be returned to clients
+            A DXO containing all information ready to be returned to clients
         """
         raise NotImplementedError
 
     def reset(self) -> None:
         # Reset parameters for next round,
         # This will be performed at the end of each aggregation round,
         # it can include, but not limited to, clearing the _collection
```

## nvflare/app_common/aggregators/collect_and_assemble_aggregator.py

```diff
@@ -41,36 +41,36 @@
         if not self.assembler:
             self.assembler = fl_ctx.get_engine().get_component(self.assembler_id)
         contributor_name = shareable.get_peer_prop(key=ReservedKey.IDENTITY_NAME, default="?")
         dxo = self._get_contribution(shareable, fl_ctx)
         if dxo is None or dxo.data is None:
             self.log_error(fl_ctx, "no data to aggregate")
             return False
-        data = dxo.data
+
         current_round = fl_ctx.get_prop(AppConstants.CURRENT_ROUND)
-        return self._accept_contribution(contributor_name, current_round, data, fl_ctx)
+        return self._accept_contribution(contributor_name, current_round, dxo, fl_ctx)
 
-    def _accept_contribution(self, contributor: str, current_round: int, data: dict, fl_ctx: FLContext) -> bool:
+    def _accept_contribution(self, contributor: str, current_round: int, dxo: DXO, fl_ctx: FLContext) -> bool:
         collection = self.assembler.collection
         if contributor not in collection:
-            collection[contributor] = self.assembler.get_model_params(data)
+            collection[contributor] = self.assembler.get_model_params(dxo)
             accepted = True
         else:
             self.log_info(
                 fl_ctx,
                 f"Discarded: Current round: {current_round} " + f"contributions already include client: {contributor}",
             )
             accepted = False
         return accepted
 
     def _get_contribution(self, shareable: Shareable, fl_ctx: FLContext) -> Optional[DXO]:
         contributor_name = shareable.get_peer_prop(key=ReservedKey.IDENTITY_NAME, default="?")
         try:
             dxo = from_shareable(shareable)
-        except Exception:
+        except BaseException:
             self.log_exception(fl_ctx, "shareable data is not a valid DXO")
             return None
 
         rc = shareable.get_return_code()
         if rc and rc != ReturnCode.OK:
             self.log_warning(
                 fl_ctx,
@@ -100,13 +100,13 @@
     def aggregate(self, fl_ctx: FLContext) -> Shareable:
         self.log_debug(fl_ctx, "Start aggregation")
         current_round = fl_ctx.get_prop(AppConstants.CURRENT_ROUND)
         collection = self.assembler.collection
         site_num = len(collection)
         self.log_info(fl_ctx, f"aggregating {site_num} update(s) at round {current_round}")
 
-        model = self.assembler.assemble(data=collection, fl_ctx=fl_ctx)
+        dxo = self.assembler.assemble(data=collection, fl_ctx=fl_ctx)
         # Reset assembler for next round
         self.assembler.reset()
         self.log_debug(fl_ctx, "End aggregation")
-        dxo = DXO(data_kind=self.assembler.get_expected_data_kind(), data=model)
+
         return dxo.to_shareable()
```

## nvflare/app_common/aggregators/dxo_aggregator.py

```diff
@@ -173,11 +173,12 @@
         current_round = fl_ctx.get_prop(AppConstants.CURRENT_ROUND)
         self.log_info(fl_ctx, f"aggregating {self.aggregation_helper.get_len()} update(s) at round {current_round}")
         self.log_debug(fl_ctx, f"complete history {self.aggregation_helper.get_len()}")
         aggregated_dict = self.aggregation_helper.get_result()
         self.log_debug(fl_ctx, "End aggregation")
 
         dxo = DXO(data_kind=self.expected_data_kind, data=aggregated_dict)
-        dxo.set_meta_prop(MetaKey.PROCESSED_ALGORITHM, self.processed_algorithm)
-        self.processed_algorithm = None
+        if self.processed_algorithm is not None:
+            dxo.set_meta_prop(MetaKey.PROCESSED_ALGORITHM, self.processed_algorithm)
+            self.processed_algorithm = None
 
         return dxo
```

## nvflare/app_common/aggregators/intime_accumulate_model_aggregator.py

```diff
@@ -171,15 +171,15 @@
 
         Returns:
             The first boolean indicates if this shareable is accepted.
             The second boolean indicates if aggregate can be called.
         """
         try:
             dxo = from_shareable(shareable)
-        except Exception:
+        except BaseException:
             self.log_exception(fl_ctx, "shareable data is not a valid DXO")
             return False
 
         if dxo.data_kind not in (DataKind.WEIGHT_DIFF, DataKind.WEIGHTS, DataKind.METRICS, DataKind.COLLECTION):
             self.log_error(
                 fl_ctx,
                 f"cannot handle data kind {dxo.data_kind}, "
```

## nvflare/app_common/decomposers/common_decomposers.py

```diff
@@ -7,30 +7,61 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 """Decomposers for types from app_common and Machine Learning libraries."""
 import os
 from abc import ABC
 from io import BytesIO
 from typing import Any
 
 import numpy as np
 
+from nvflare.app_common.abstract.fl_model import FLModel
 from nvflare.app_common.abstract.learnable import Learnable
 from nvflare.app_common.abstract.model import ModelLearnable
 from nvflare.app_common.widgets.event_recorder import _CtxPropReq, _EventReq, _EventStats
 from nvflare.fuel.utils import fobs
 from nvflare.fuel.utils.fobs import Decomposer
 from nvflare.fuel.utils.fobs.decomposer import DictDecomposer
 
 
+class FLModelDecomposer(fobs.Decomposer):
+    def supported_type(self):
+        return FLModel
+
+    def decompose(self, b: FLModel) -> Any:
+        return [
+            b.params_type,
+            b.params,
+            b.optimizer_params,
+            b.metrics,
+            b.client_weights,
+            b.current_round,
+            b.total_rounds,
+            b.meta,
+        ]
+
+    def recompose(self, data: list) -> FLModel:
+        return FLModel(
+            params_type=data[0],
+            params=data[1],
+            optimizer_params=data[2],
+            metrics=data[3],
+            client_weights=data[4],
+            current_round=data[5],
+            total_rounds=data[6],
+            meta=data[7],
+        )
+
+
 class ModelLearnableDecomposer(fobs.Decomposer):
     def supported_type(self):
         return ModelLearnable
 
     def decompose(self, target: ModelLearnable) -> Any:
         return target.copy()
 
@@ -87,14 +118,15 @@
 
 def register():
     if register.registered:
         return
 
     fobs.register(DictDecomposer(Learnable))
     fobs.register(DictDecomposer(ModelLearnable))
+    fobs.register(FLModelDecomposer)
 
     fobs.register_data_classes(
         _CtxPropReq,
         _EventReq,
         _EventStats,
     )
```

## nvflare/app_common/executors/error_handling_executor.py

```diff
@@ -81,15 +81,15 @@
 
             self.log_error(
                 fl_ctx,
                 f"task:{task_name} failed on client:{fl_ctx.get_identity_name()} due to result is '{result}'\n",
             )
             return make_reply(ReturnCode.EXECUTION_RESULT_ERROR)
 
-        except Exception:
+        except BaseException:
             self.log_exception(fl_ctx, f"{self.__class__.__name__} executes task {task_name} failed.")
             return make_reply(ReturnCode.EXECUTION_RESULT_ERROR)
 
     def _check_init_status(self, fl_ctx: FLContext):
 
         if not self.init_status_ok:
             for fail_key in self.init_failure:
```

## nvflare/app_common/executors/multi_process_executor.py

```diff
@@ -137,15 +137,15 @@
                         request = new_cell_message({}, data)
                         self.engine.client.cell.fire_and_forget(
                             targets=self.targets,
                             channel=CellChannel.CLIENT_SUB_WORKER_COMMAND,
                             topic=MultiProcessCommandNames.FIRE_EVENT,
                             message=request,
                         )
-                    except Exception:
+                    except BaseException:
                         # Warning: Have to set fire_event=False, otherwise it will cause dead loop on the event handling!!!
                         self.log_warning(
                             fl_ctx,
                             f"Failed to relay the event to child processes. Event: {event_type}",
                             fire_event=False,
                         )
 
@@ -227,15 +227,15 @@
                 topic=MultiProcessCommandNames.INITIALIZE,
                 request=request,
             )
             for name, reply in replies.items():
                 if reply.get_header(MessageHeaderKey.RETURN_CODE) != F3ReturnCode.OK:
                     self.log_exception(fl_ctx, "error initializing multi_process executor")
                     raise ValueError(reply.get_header(MessageHeaderKey.ERROR))
-        except Exception as e:
+        except BaseException as e:
             self.log_exception(fl_ctx, f"error initializing multi_process executor: {secure_format_exception(e)}")
 
     def receive_execute_result(self, request: CellMessage) -> CellMessage:
         return_data = request.payload
         with self.engine.new_context() as fl_ctx:
             fl_ctx.props.update(return_data[CommunicationMetaData.FL_CTX].props)
             self.execute_result = return_data[CommunicationMetaData.SHAREABLE]
@@ -295,15 +295,15 @@
             request = new_cell_message({}, data)
             self.engine.client.cell.fire_and_forget(
                 targets=self.targets,
                 channel=CellChannel.CLIENT_SUB_WORKER_COMMAND,
                 topic=MultiProcessCommandNames.TASK_EXECUTION,
                 message=request,
             )
-        except Exception:
+        except BaseException:
             self.log_error(fl_ctx, "Multi-Process Execution error.")
             return make_reply(ReturnCode.EXECUTION_RESULT_ERROR)
 
     def finalize(self, fl_ctx: FLContext):
         """This is called when exiting/aborting the executor."""
         if self.finalized:
             return
```

## nvflare/app_common/executors/statistics/statistics_executor_exception.py

```diff
@@ -9,9 +9,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-class StatisticExecutorException(Exception):
+class StatisticExecutorException(BaseException):
     pass
```

## nvflare/app_common/executors/statistics/statistics_task_handler.py

```diff
@@ -103,15 +103,15 @@
             statistics_result[tm.name][ds_name] = {}
             features: List[Feature] = ds_features[ds_name]
             for feature in features:
                 try:
                     statistics_result[tm.name][ds_name][feature.feature_name] = fn(
                         ds_name, feature.feature_name, tm, shareable, fl_ctx
                     )
-                except Exception as e:
+                except BaseException as e:
                     self.log_exception(
                         fl_ctx,
                         f"Failed to populate result  statistics of dataset {ds_name}"
                         f" and feature {feature.feature_name} with exception: {secure_format_exception(e)}",
                     )
 
     def get_numeric_features(self) -> Dict[str, List[Feature]]:
```

## nvflare/app_common/np/np_trainer.py

```diff
@@ -62,15 +62,15 @@
         #     # Clean up resources (closing files, joining threads, removing dirs etc.)
         pass
 
     def _train(self, shareable: Shareable, fl_ctx: FLContext, abort_signal: Signal):
         # First we extract DXO from the shareable.
         try:
             incoming_dxo = from_shareable(shareable)
-        except Exception as e:
+        except BaseException as e:
             self.system_panic(
                 f"Unable to convert shareable to model definition. Exception {secure_format_exception(e)}", fl_ctx
             )
             return make_reply(ReturnCode.BAD_TASK_DATA)
 
         # Information about workflow is retrieved from the shareable header.
         current_round = shareable.get_header(AppConstants.CURRENT_ROUND, None)
```

## nvflare/app_common/pt/tb_receiver.py

```diff
@@ -17,8 +17,8 @@
 warnings.warn(
     f"This module: {__file__} is deprecated. Please use nvflare.app_opt.tracking.tb_receiver.",
     category=FutureWarning,
     stacklevel=2,
 )
 
 # flake8: noqa: F401
-from nvflare.app_opt.tracking.tb_receiver import TBAnalyticsReceiver
+from nvflare.app_opt.tracking.tb.tb_receiver import TBAnalyticsReceiver
```

## nvflare/app_common/response_processors/global_weights_initializer.py

```diff
@@ -92,15 +92,15 @@
                 fl_ctx,
                 f"bad response from client {client.name}: " f"response must be Shareable but got {type(response)}",
             )
             return False
 
         try:
             dxo = from_shareable(response)
-        except Exception:
+        except BaseException:
             self.log_exception(fl_ctx, f"bad response from client {client.name}: " f"it does not contain DXO")
             return False
 
         if dxo.data_kind != DataKind.WEIGHTS:
             self.log_error(
                 fl_ctx,
                 f"bad response from client {client.name}: "
```

## nvflare/app_common/tracking/tracker_types.py

```diff
@@ -8,46 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-    W&B vs MLFLOW vs. Tensorboad
-    DATA --> PARAMETER --> Scalar
-    DATA --> PARAMETERS --> Scalars
-    DATA --> METRIC --> Scalar
-    DATA --> METRICS --> Scalars
-    DATA --> TEXT --> TEXT
-    DATA --> IMAGE --> IMAGE
-    ARTIFACT:type=model --> MODEL
-
-    NOT SUPPORTED
-    PLOT --> FIGURE
-    ARTIFACT --> TEXT
-    DATA --> ? --> Histogram
-    ARTIFACT --> DICT
-    ARTIFACT:type=dataset --> ARTIFACT
-
-    wandb.log(data) ==> mlflow.log_params(data) ==> writer.add_scalas(data)
-    wandb.log(data) ==> mlflow.log_metrics(data) ==> writer.add_scalas(data)
-    wandb.log({"examples": images} ==>  mlflow.log_image(image, output_path) ==> writer.add_image('images', image, 0)
-
-    art = wandb.Artifact("my-object-detector", type="model")
-    art.add_file("saved_model_weights.pt")
-    wandb.log_artifact(art) ==> mlflow.register_model(model_uri, "my-object-detector")  ==> ?
-
-  """
 from enum import Enum
 
 ANALYTIC_EVENT_TYPE = "analytix_log_stats"
 
 
-class Tracker(Enum):
+class LogWriterName(Enum):
     TORCH_TB = "TORCH_TENSORBOARD"
     MLFLOW = "MLFLOW"
     WANDB = "WEIGHTS_AND_BIASES"
 
 
 class TrackConst(object):
     TRACKER_KEY = "tracker_key"
@@ -65,13 +39,14 @@
     DATA_TYPE_KEY = "analytics_data_type"
     KWARGS_KEY = "analytics_kwargs"
 
     PROJECT_NAME = "project_name"
     PROJECT_TAGS = "project_name"
 
     EXPERIMENT_NAME = "experiment_name"
-    EXPERIMENT_TAG = "experiment_tag"
+    RUN_NAME = "run_name"
+    EXPERIMENT_TAGS = "experiment_tags"
     INIT_CONFIG = "init_config"
     RUN_TAGS = "run_tags"
 
     SITE_KEY = "site"
     JOB_ID_KEY = "job_id"
```

## nvflare/app_common/widgets/streaming.py

```diff
@@ -19,23 +19,27 @@
 from nvflare.apis.analytix import AnalyticsData, AnalyticsDataType
 from nvflare.apis.dxo import DXO
 from nvflare.apis.event_type import EventType
 from nvflare.apis.fl_component import FLComponent
 from nvflare.apis.fl_constant import EventScope, FLContextKey, ReservedKey
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.shareable import Shareable
-from nvflare.app_common.tracking.tracker_types import Tracker
+from nvflare.app_common.tracking.tracker_types import LogWriterName, TrackConst
+from nvflare.fuel.utils.deprecated import deprecated
 from nvflare.widgets.widget import Widget
 
 ANALYTIC_EVENT_TYPE = "analytix_log_stats"
 
 
 def send_analytic_dxo(comp: FLComponent, dxo: DXO, fl_ctx: FLContext, event_type: str = ANALYTIC_EVENT_TYPE):
     """Sends analytic dxo.
 
+    Sends analytic dxo by firing an event (of type "analytix_log_stats" by default unless otherwise specified)
+    with the dxo in the fl_ctx.
+
     Args:
         comp (FLComponent): An FLComponent.
         dxo (DXO): analytic data in dxo.
         fl_ctx (FLContext): fl context info.
         event_type (str): Event type.
     """
     if not isinstance(comp, FLComponent):
@@ -46,125 +50,126 @@
         raise TypeError(f"expect fl_ctx to be an instance of FLContext, but got {type(fl_ctx)}")
 
     fl_ctx.set_prop(key=FLContextKey.EVENT_DATA, value=dxo.to_shareable(), private=True, sticky=False)
     comp.fire_event(event_type=event_type, fl_ctx=fl_ctx)
 
 
 def create_analytic_dxo(
-    tag: str, value, data_type: AnalyticsDataType, step: int = None, sender: Tracker = Tracker.TORCH_TB, **kwargs
+    tag: str,
+    value,
+    data_type: AnalyticsDataType,
+    writer: LogWriterName = LogWriterName.TORCH_TB,
+    **kwargs,
 ) -> DXO:
     """Creates the analytic DXO.
 
     Args:
         tag (str): the tag associated with this value.
         value: the analytic data.
         data_type: (AnalyticsDataType): analytic data type.
-        step (int) : global step
-        sender: (Tracker), syntax of the sender: such TensorBoard or MLFLow
+        writer (LogWriterName): syntax of the sender: such TensorBoard or MLflow
         kwargs: additional arguments to be passed into the receiver side's function.
 
     Returns:
         A DXO object that contains the analytic data.
     """
-    step = step if step else kwargs.get("global_step", None)
-    data = AnalyticsData(key=tag, value=value, data_type=data_type, step=step, sender=sender, kwargs=kwargs)
+    data = AnalyticsData(key=tag, value=value, data_type=data_type, sender=writer, **kwargs)
     dxo = data.to_dxo()
     return dxo
 
 
 class AnalyticsSender(Widget):
-    def __init__(self, event_type=ANALYTIC_EVENT_TYPE):
-        """Sends analytics data.
+    def __init__(self, event_type=ANALYTIC_EVENT_TYPE, writer_name=LogWriterName.TORCH_TB):
+        """Sender for analytics data.
 
-        Note::
-            This class implements some common methods follows signatures from PyTorch SummaryWriter.
-            It provides a convenient way for Learner to use.
+        This class has some legacy methods that implement some common methods following signatures from
+        PyTorch SummaryWriter. New code should use :py:class:`TBWriter <nvflare.app_opt.tracking.tb.tb_writer.TBWriter>` instead,
+        which contains an AnalyticsSender.
 
         Args:
-            event_type (str): event type to fire.
+            event_type (str): event type to fire (defaults to "analytix_log_stats").
+            writer_name: the log writer for syntax information (defaults to LogWriterName.TORCH_TB)
         """
         super().__init__()
-        self.fl_ctx = None
         self.engine = None
         self.event_type = event_type
+        self.writer = writer_name
 
-    def get_tracker_name(self) -> Tracker:
-        return Tracker.TORCH_TB
+    def get_writer_name(self) -> LogWriterName:
+        return self.writer
 
     def handle_event(self, event_type: str, fl_ctx: FLContext):
-        if event_type == EventType.START_RUN:
+        if event_type == EventType.ABOUT_TO_START_RUN:
             self.engine = fl_ctx.get_engine()
 
-    def _add(
-        self,
-        tag: str,
-        value,
-        data_type: AnalyticsDataType,
-        global_step: Optional[int] = None,
-        kwargs: Optional[dict] = None,
-    ):
+    def add(self, tag: str, value, data_type: AnalyticsDataType, global_step: Optional[int] = None, **kwargs):
+        """Create and send a DXO by firing an event.
+
+        Args:
+            tag (str): Tag name
+            value (_type_): Value to send
+            data_type (AnalyticsDataType): Data type of the value being sent
+            global_step (optional, int): Global step value.
+
+        Raises:
+            TypeError: global_step must be an int
+        """
         kwargs = kwargs if kwargs else {}
-        if global_step:
+        if global_step is not None:
             if not isinstance(global_step, int):
                 raise TypeError(f"Expect global step to be an instance of int, but got {type(global_step)}")
-            kwargs["global_step"] = global_step
-        dxo = create_analytic_dxo(
-            tag=tag, value=value, data_type=data_type, step=global_step, sender=self.get_tracker_name(), **kwargs
-        )
+            kwargs[TrackConst.GLOBAL_STEP_KEY] = global_step
+        dxo = create_analytic_dxo(tag=tag, value=value, data_type=data_type, writer=self.get_writer_name(), **kwargs)
         with self.engine.new_context() as fl_ctx:
             send_analytic_dxo(self, dxo=dxo, fl_ctx=fl_ctx, event_type=self.event_type)
 
+    @deprecated(
+        "This method is deprecated, please use :py:class:`TBWriter <nvflare.app_opt.tracking.tb.tb_writer.TBWriter>` instead."
+    )
     def add_scalar(self, tag: str, scalar: float, global_step: Optional[int] = None, **kwargs):
-        """Sends a scalar.
+        """Legacy method to send a scalar.
+
+        This follows the signature from PyTorch SummaryWriter and is here in case it is used in previous code. If
+        you are writing new code, use :py:class:`TBWriter <nvflare.app_opt.tracking.tb.tb_writer.TBWriter>` instead.
 
         Args:
             tag (str): Data identifier.
             scalar (float): Value to send.
             global_step (optional, int): Global step value.
             **kwargs: Additional arguments to pass to the receiver side.
         """
-        self._add(tag=tag, value=scalar, data_type=AnalyticsDataType.SCALAR, global_step=global_step, kwargs=kwargs)
+        self.add(tag=tag, value=scalar, data_type=AnalyticsDataType.SCALAR, global_step=global_step, **kwargs)
 
+    @deprecated(
+        "This method is deprecated, please use :py:class:`TBWriter <nvflare.app_opt.tracking.tb.tb_writer.TBWriter>` instead."
+    )
     def add_scalars(self, tag: str, scalars: dict, global_step: Optional[int] = None, **kwargs):
-        """Sends scalars.
+        """Legacy method to send scalars.
+
+        This follows the signature from PyTorch SummaryWriter and is here in case it is used in previous code. If
+        you are writing new code, use :py:class:`TBWriter <nvflare.app_opt.tracking.tb.tb_writer.TBWriter>` instead.
 
         Args:
             tag (str): The parent name for the tags.
             scalars (dict): Key-value pair storing the tag and corresponding values.
             global_step (optional, int): Global step value.
             **kwargs: Additional arguments to pass to the receiver side.
         """
-        self._add(tag=tag, value=scalars, data_type=AnalyticsDataType.SCALARS, global_step=global_step, kwargs=kwargs)
-
-    def add_text(self, tag: str, text: str, global_step: Optional[int] = None, **kwargs):
-        """Sends a text.
-
-        Args:
-            tag (str): Data identifier.
-            text (str): String to send.
-            global_step (optional, int): Global step value.
-            **kwargs: Additional arguments to pass to the receiver side.
-        """
-        self._add(tag=tag, value=text, data_type=AnalyticsDataType.TEXT, global_step=global_step, kwargs=kwargs)
-
-    def add_image(self, tag: str, image, global_step: Optional[int] = None, **kwargs):
-        """Sends an image.
-
-        Args:
-            tag (str): Data identifier.
-            image: Image to send.
-            global_step (optional, int): Global step value.
-            **kwargs: Additional arguments to pass to the receiver side.
-        """
-        self._add(tag=tag, value=image, data_type=AnalyticsDataType.IMAGE, global_step=global_step, kwargs=kwargs)
+        self.add(tag=tag, value=scalars, data_type=AnalyticsDataType.SCALARS, global_step=global_step, **kwargs)
 
+    @deprecated(
+        "This method is deprecated, please use :py:class:`TBWriter <nvflare.app_opt.tracking.tb.tb_writer.TBWriter>` instead."
+    )
     def flush(self):
-        """Flushes out the message.
+        """Legacy method to flush out the message.
+
+        This follows the signature from PyTorch SummaryWriter and is here in case it is used in previous code. If
+        you are writing new code, use :py:class:`TBWriter <nvflare.app_opt.tracking.tb.tb_writer.TBWriter>` instead.
 
-        This is doing nothing, it is defined for mimic the PyTorch SummaryWriter behavior.
+        This does nothing, it is defined to mimic the PyTorch SummaryWriter.
         """
         pass
 
     def close(self):
         """Close resources."""
         if self.engine:
             self.engine = None
@@ -184,34 +189,40 @@
         self._save_lock = Lock()
         self._end = False
 
     @abstractmethod
     def initialize(self, fl_ctx: FLContext):
         """Initializes the receiver.
 
+        Called after EventType.START_RUN.
+
         Args:
             fl_ctx (FLContext): fl context.
         """
         pass
 
     @abstractmethod
     def save(self, fl_ctx: FLContext, shareable: Shareable, record_origin: str):
         """Saves the received data.
 
+        Specific implementations of AnalyticsReceiver will implement save in their own way.
+
         Args:
             fl_ctx (FLContext): fl context.
             shareable (Shareable): the received message.
             record_origin (str): the sender of this message / record.
         """
         pass
 
     @abstractmethod
     def finalize(self, fl_ctx: FLContext):
         """Finalizes the receiver.
 
+        Called after EventType.END_RUN.
+
         Args:
             fl_ctx (FLContext): fl context.
         """
         pass
 
     def handle_event(self, event_type: str, fl_ctx: FLContext):
         if event_type == EventType.START_RUN:
```

## nvflare/app_common/widgets/validation_json_generator.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, NVIDIA CORPORATION.  All rights reserved.
+# Copyright (c) 2021, NVIDIA CORPORATION.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os.path
 
-from nvflare.apis.dxo import DataKind, from_shareable
+from nvflare.apis.dxo import DataKind, from_shareable, get_leaf_dxos
 from nvflare.apis.event_type import EventType
 from nvflare.apis.fl_context import FLContext
 from nvflare.app_common.app_constant import AppConstants
 from nvflare.app_common.app_event_type import AppEventType
 from nvflare.widgets.widget import Widget
 
 
@@ -60,19 +60,32 @@
                     dxo = from_shareable(val_results)
                     dxo.validate()
 
                     if dxo.data_kind == DataKind.METRICS:
                         if data_client not in self._val_results:
                             self._val_results[data_client] = {}
                         self._val_results[data_client][model_owner] = dxo.data
+                    elif dxo.data_kind == DataKind.COLLECTION:
+                        # The DXO could contain multiple sub-DXOs (e.g. received from a T2 system)
+                        leaf_dxos, errors = get_leaf_dxos(dxo, data_client)
+                        if errors:
+                            for err in errors:
+                                self.log_error(fl_ctx, f"Bad result from {data_client}: {err}")
+                        for _sub_data_client, _dxo in leaf_dxos.items():
+                            _dxo.validate()
+                            if _sub_data_client not in self._val_results:
+                                self._val_results[_sub_data_client] = {}
+                            self._val_results[_sub_data_client][model_owner] = _dxo.data
                     else:
                         self.log_error(
-                            fl_ctx, f"Expected dxo of kind METRICS but got {dxo.data_kind} instead.", fire_event=False
+                            fl_ctx,
+                            f"Expected dxo of kind METRICS or COLLECTION but got {dxo.data_kind} instead.",
+                            fire_event=False,
                         )
-                except:
+                except Exception:
                     self.log_exception(fl_ctx, "Exception in handling validation result.", fire_event=False)
             else:
                 self.log_error(fl_ctx, "Validation result not found.", fire_event=False)
         elif event_type == EventType.END_RUN:
             run_dir = fl_ctx.get_engine().get_workspace().get_run_dir(fl_ctx.get_job_id())
             cross_val_res_dir = os.path.join(run_dir, self._results_dir)
             if not os.path.exists(cross_val_res_dir):
```

## nvflare/app_common/workflows/cross_site_model_eval.py

```diff
@@ -15,15 +15,15 @@
 import os
 import shutil
 import time
 from typing import Union
 
 from nvflare.apis.client import Client
 from nvflare.apis.controller_spec import ClientTask, Task
-from nvflare.apis.dxo import DXO, from_bytes, from_shareable
+from nvflare.apis.dxo import DXO, from_bytes, from_shareable, get_leaf_dxos
 from nvflare.apis.fl_constant import ReturnCode
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.impl.controller import Controller
 from nvflare.apis.shareable import Shareable
 from nvflare.apis.signal import Signal
 from nvflare.apis.workspace import Workspace
 from nvflare.app_common.abstract.formatter import Formatter
@@ -51,21 +51,21 @@
     ):
         """Cross Site Model Validation workflow.
 
         Args:
             task_check_period (float, optional): How often to check for new tasks or tasks being finished.
                 Defaults to 0.5.
             cross_val_dir (str, optional): Path to cross site validation directory relative to run directory.
-                Defaults to `AppConstants.CROSS_VAL_DIR`.
+                Defaults to "cross_site_val".
             submit_model_timeout (int, optional): Timeout of submit_model_task. Defaults to 600 secs.
             validation_timeout (int, optional): Timeout for validate_model task. Defaults to 6000 secs.
             model_locator_id (str, optional): ID for model_locator component. Defaults to "".
             formatter_id (str, optional): ID for formatter component. Defaults to "".
-            submit_model_task_name (str, optional): Name of submit_model task. Defaults to `AppConstants.TASK_SUBMIT_MODEL`.
-            validation_task_name (str, optional): Name of validate_model task. Defaults to `AppConstants.TASK_VALIDATION`.
+            submit_model_task_name (str, optional): Name of submit_model task. Defaults to "".
+            validation_task_name (str, optional): Name of validate_model task. Defaults to "validate".
             cleanup_models (bool, optional): Whether or not models should be deleted after run. Defaults to False.
             participating_clients (list, optional): List of participating client names. If not provided, defaults
                 to all clients connected at start of controller.
             wait_for_clients_timeout (int, optional): Timeout for clients to appear. Defaults to 300 secs
         """
         super().__init__(task_check_period=task_check_period)
 
@@ -233,14 +233,16 @@
                 time.sleep(self._task_check_period)
         except Exception as e:
             error_msg = f"Exception in cross site validator control_flow: {secure_format_exception(e)}"
             self.log_exception(fl_ctx, error_msg)
             self.system_panic(error_msg, fl_ctx)
 
     def stop_controller(self, fl_ctx: FLContext):
+        self.cancel_all_tasks(fl_ctx=fl_ctx)
+
         if self._cleanup_models:
             self.log_info(fl_ctx, "Removing local models kept for validation.")
             for model_name, model_path in self._server_models.items():
                 if model_path and os.path.isfile(model_path):
                     os.remove(model_path)
                     self.log_debug(fl_ctx, f"Removing server model {model_name} at {model_path}.")
             for model_name, model_path in self._client_models.items():
@@ -313,15 +315,15 @@
                 self.system_panic(f"ModelLocator produced invalid data: expect DXO but got {type(dxo)}.", fl_ctx)
                 return False
 
             # Save to workspace
             unique_name = "SRV_" + name
             unique_names.append(unique_name)
             try:
-                save_path = self._save_validation_content(unique_name, self._cross_val_models_dir, dxo, fl_ctx)
+                save_path = self._save_dxo_content(unique_name, self._cross_val_models_dir, dxo, fl_ctx)
             except:
                 self.log_exception(fl_ctx, f"Unable to save shareable contents of server model {unique_name}")
                 self.system_panic(f"Unable to save shareable contents of server model {unique_name}", fl_ctx)
                 return False
 
             self._server_models[unique_name] = save_path
             self._val_results[unique_name] = {}
@@ -329,17 +331,17 @@
         if unique_names:
             self.log_info(fl_ctx, f"Server models loaded: {unique_names}.")
         else:
             self.log_info(fl_ctx, "no server models to validate!")
         return True
 
     def _accept_local_model(self, client_name: str, result: Shareable, fl_ctx: FLContext):
-        fl_ctx.set_prop(AppConstants.RECEIVED_MODEL, result, private=False, sticky=False)
-        fl_ctx.set_prop(AppConstants.RECEIVED_MODEL_OWNER, client_name, private=False, sticky=False)
-        fl_ctx.set_prop(AppConstants.CROSS_VAL_DIR, self._cross_val_dir, private=False, sticky=False)
+        fl_ctx.set_prop(AppConstants.RECEIVED_MODEL, result, private=True, sticky=False)
+        fl_ctx.set_prop(AppConstants.RECEIVED_MODEL_OWNER, client_name, private=True, sticky=False)
+        fl_ctx.set_prop(AppConstants.CROSS_VAL_DIR, self._cross_val_dir, private=True, sticky=False)
         self.fire_event(AppEventType.RECEIVE_BEST_MODEL, fl_ctx)
 
         # get return code
         rc = result.get_return_code()
         if rc and rc != ReturnCode.OK:
             # Raise errors if bad peer context or execution exception.
             if rc in [ReturnCode.MISSING_PEER_CONTEXT, ReturnCode.BAD_PEER_CONTEXT]:
@@ -359,31 +361,38 @@
             else:
                 self.log_error(fl_ctx, "Return code set. Model submission from client will be ignored.")
         else:
             # Save shareable in models directory.
             try:
                 self.log_debug(fl_ctx, "Extracting DXO from shareable.")
                 dxo = from_shareable(result)
-                save_path = self._save_validation_content(client_name, self._cross_val_models_dir, dxo, fl_ctx)
             except ValueError as e:
                 self.log_error(
                     fl_ctx,
-                    f"Unable to save shareable contents of {client_name}'s model. Exception: {secure_format_exception(e)}",
+                    f"Ignored bad result from {client_name}: {secure_format_exception(e)}",
                 )
-                self.log_warning(fl_ctx, f"Ignoring client {client_name}'s model.")
                 return
 
-            self.log_info(fl_ctx, f"Received local model from client {client_name}.")
-
-            self._client_models[client_name] = save_path
+            # The DXO could contain multiple sub-DXOs (e.g. received from a T2 system)
+            leaf_dxos, errors = get_leaf_dxos(dxo, client_name)
+            if errors:
+                for err in errors:
+                    self.log_error(fl_ctx, f"Bad result from {client_name}: {err}")
+            for k, v in leaf_dxos.items():
+                self._save_client_model(k, v, fl_ctx)
+
+    def _save_client_model(self, model_name: str, dxo: DXO, fl_ctx: FLContext):
+        save_path = self._save_dxo_content(model_name, self._cross_val_models_dir, dxo, fl_ctx)
+        self.log_info(fl_ctx, f"Saved client model {model_name} to {save_path}")
+        self._client_models[model_name] = save_path
 
-            self._send_validation_task(client_name, fl_ctx)
+        # Send a model to this client to validate
+        self._send_validation_task(model_name, fl_ctx)
 
     def _send_validation_task(self, model_name: str, fl_ctx: FLContext):
-        """Sends the model to all participating clients for validation."""
         self.log_info(fl_ctx, f"Sending {model_name} model to all participating clients for validation.")
 
         # Create validation task and broadcast to all participating clients.
         task = Task(
             name=self._validation_task_name,
             data=Shareable(),
             before_task_sent_cb=self._before_send_validate_task_cb,
@@ -426,32 +435,49 @@
             else:
                 self.log_error(
                     fl_ctx,
                     f"Client {client_name} sent results for validating {model_owner} model with return code set."
                     " Logging empty results.",
                 )
 
+            if client_name not in self._val_results:
+                self._val_results[client_name] = {}
             self._val_results[client_name][model_owner] = {}
         else:
-            save_file_name = client_name + "_" + model_owner
-
             try:
                 dxo = from_shareable(result)
-                self._save_validation_content(save_file_name, self._cross_val_results_dir, dxo, fl_ctx)
-                self._val_results[client_name][model_owner] = os.path.join(self._cross_val_results_dir, save_file_name)
-
-                self.log_info(fl_ctx, f"Client {client_name} sent results for validating {model_owner} model.")
             except ValueError as e:
                 reason = (
-                    f"Unable to save validation result from {client_name} of {model_owner}'s model. "
+                    f"Bad validation result from {client_name} on model {model_owner}. "
                     f"Exception: {secure_format_exception(e)}"
                 )
                 self.log_exception(fl_ctx, reason)
+                return
+
+            # The DXO could contain multiple sub-DXOs (e.g. received from a T2 system)
+            leaf_dxos, errors = get_leaf_dxos(dxo, client_name)
+            if errors:
+                for err in errors:
+                    self.log_error(fl_ctx, f"Bad result from {client_name}: {err}")
+            for k, v in leaf_dxos.items():
+                self._save_validation_result(k, model_owner, v, fl_ctx)
+
+    def _save_validation_result(self, client_name: str, model_name: str, dxo, fl_ctx):
+        file_name = client_name + "_" + model_name
+        file_path = self._save_dxo_content(file_name, self._cross_val_results_dir, dxo, fl_ctx)
+        client_results = self._val_results.get(client_name, None)
+        if not client_results:
+            client_results = {}
+            self._val_results[client_name] = client_results
+        client_results[model_name] = file_path
+        self.log_info(
+            fl_ctx, f"Saved validation result from client '{client_name}' on model '{model_name}' in {file_path}"
+        )
 
-    def _save_validation_content(self, name: str, save_dir: str, dxo: DXO, fl_ctx: FLContext) -> str:
+    def _save_dxo_content(self, name: str, save_dir: str, dxo: DXO, fl_ctx: FLContext) -> str:
         """Saves shareable to given directory within the app_dir.
 
         Args:
             name (str): Name of shareable
             save_dir (str): Relative path to directory in which to save
             dxo (DXO): DXO object
             fl_ctx (FLContext): FLContext object
@@ -468,17 +494,15 @@
             raise ValueError(f"Unable to extract shareable contents. Exception: {(secure_format_exception(e))}")
 
         # Save contents to path
         try:
             with open(data_filename, "wb") as f:
                 f.write(bytes_to_save)
         except Exception as e:
-            raise ValueError(f"Unable to save shareable contents: {secure_format_exception(e)}")
-
-        self.log_debug(fl_ctx, f"Saved cross validation model with name: {name}.")
+            raise ValueError(f"Unable to save DXO content: {secure_format_exception(e)}")
 
         return data_filename
 
     def _load_validation_content(self, name: str, load_dir: str, fl_ctx: FLContext) -> Union[DXO, None]:
         # Load shareable from disk
         shareable_filename = os.path.join(load_dir, name)
```

## nvflare/app_common/workflows/cyclic_ctl.py

```diff
@@ -150,14 +150,15 @@
         # update the global learnable with the received result (shareable)
         # e.g. the received result could be weight_diffs, the learnable could be full weights.
         self._last_learnable = self.shareable_generator.shareable_to_learnable(client_task.result, fl_ctx)
 
         # prepare task shareable data for next client
         task.data = self.shareable_generator.learnable_to_shareable(self._last_learnable, fl_ctx)
         task.data.set_header(AppConstants.CURRENT_ROUND, self._current_round)
+        task.data.add_cookie(AppConstants.CONTRIBUTION_ROUND, self._current_round)
 
     def control_flow(self, abort_signal: Signal, fl_ctx: FLContext):
         try:
             self.log_debug(fl_ctx, "Cyclic starting.")
 
             for self._current_round in range(self._start_round, self._end_round):
                 if abort_signal.triggered:
@@ -169,14 +170,15 @@
                 # Task for one cyclic
                 targets = self._get_relay_orders()
                 targets_names = [t.name for t in targets]
                 self.log_debug(fl_ctx, f"Relay on {targets_names}")
 
                 shareable = self.shareable_generator.learnable_to_shareable(self._last_learnable, fl_ctx)
                 shareable.set_header(AppConstants.CURRENT_ROUND, self._current_round)
+                shareable.add_cookie(AppConstants.CONTRIBUTION_ROUND, self._current_round)
 
                 task = Task(
                     name=self.task_name,
                     data=shareable,
                     result_received_cb=self._process_result,
                 )
 
@@ -199,18 +201,18 @@
                 if (
                     self._snapshot_every_n_rounds != 0
                     and (self._current_round + 1) % self._snapshot_every_n_rounds == 0
                 ):
                     # Call the self._engine to persist the snapshot of all the FLComponents
                     self._engine.persist_components(fl_ctx, completed=False)
 
-                self.log_debug(fl_ctx, "Ending current round={}.".format(self._current_round))
+                self.log_info(fl_ctx, "Ending current round={}.".format(self._current_round))
 
             self.log_debug(fl_ctx, "Cyclic ended.")
-        except Exception as e:
+        except BaseException as e:
             error_msg = f"Cyclic control_flow exception: {secure_format_exception(e)}"
             self.log_error(fl_ctx, error_msg)
             self.system_panic(error_msg, fl_ctx)
 
     def stop_controller(self, fl_ctx: FLContext):
         self.persistor.save(learnable=self._last_learnable, fl_ctx=fl_ctx)
         self.log_debug(fl_ctx, "controller stopped")
```

## nvflare/app_common/workflows/scatter_and_gather.py

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any
 
 from nvflare.apis.client import Client
+from nvflare.apis.controller_spec import OperatorMethod, TaskOperatorKey
 from nvflare.apis.fl_constant import ReturnCode
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.impl.controller import ClientTask, Controller, Task
 from nvflare.apis.shareable import Shareable
 from nvflare.apis.signal import Signal
 from nvflare.app_common.abstract.aggregator import Aggregator
 from nvflare.app_common.abstract.learnable_persistor import LearnablePersistor
@@ -37,15 +38,15 @@
     if data < 0:
         raise ValueError(f"{name} must be greater than or equal to 0.")
 
 
 class ScatterAndGather(Controller):
     def __init__(
         self,
-        min_clients: int = 1,
+        min_clients: int = 1000,
         num_rounds: int = 5,
         start_round: int = 0,
         wait_time_after_min_received: int = 10,
         aggregator_id=AppConstants.DEFAULT_AGGREGATOR_ID,
         persistor_id=AppConstants.DEFAULT_PERSISTOR_ID,
         shareable_generator_id=AppConstants.DEFAULT_SHAREABLE_GENERATOR_ID,
         train_task_name=AppConstants.TASK_TRAIN,
@@ -61,19 +62,21 @@
         The ScatterAndGather workflow defines FederatedAveraging on all clients.
         The model persistor (persistor_id) is used to load the initial global model which is sent to all clients.
         Each client sends it's updated weights after local training which is aggregated (aggregator_id). The
         shareable generator is used to convert the aggregated weights to shareable and shareable back to weight.
         The model_persistor also saves the model after training.
 
         Args:
-            min_clients (int, optional): Min number of clients in training. Defaults to 1.
+            min_clients (int, optional): The minimum number of clients responses before
+                SAG starts to wait for `wait_time_after_min_received`. Note that SAG will move forward when all
+                available clients have responded regardless of this value. Defaults to 1000.
             num_rounds (int, optional): The total number of training rounds. Defaults to 5.
             start_round (int, optional): Start round for training. Defaults to 0.
             wait_time_after_min_received (int, optional): Time to wait before beginning aggregation after
-                contributions received. Defaults to 10.
+                minimum number of clients responses has been received. Defaults to 10.
             aggregator_id (str, optional): ID of the aggregator component. Defaults to "aggregator".
             persistor_id (str, optional): ID of the persistor component. Defaults to "persistor".
             shareable_generator_id (str, optional): ID of the shareable generator. Defaults to "shareable_generator".
             train_task_name (str, optional): Name of the train task. Defaults to "train".
             train_timeout (int, optional): Time to wait for clients to do local training.
             ignore_result_error (bool, optional): whether this controller can proceed if client result has errors.
                 Defaults to False.
@@ -223,17 +226,25 @@
 
                 # Create train_task
                 data_shareable: Shareable = self.shareable_gen.learnable_to_shareable(self._global_weights, fl_ctx)
                 data_shareable.set_header(AppConstants.CURRENT_ROUND, self._current_round)
                 data_shareable.set_header(AppConstants.NUM_ROUNDS, self._num_rounds)
                 data_shareable.add_cookie(AppConstants.CONTRIBUTION_ROUND, self._current_round)
 
+                operator = {
+                    TaskOperatorKey.OP_ID: self.train_task_name,
+                    TaskOperatorKey.METHOD: OperatorMethod.BROADCAST,
+                    TaskOperatorKey.TIMEOUT: self._train_timeout,
+                    TaskOperatorKey.AGGREGATOR: self.aggregator_id,
+                }
+
                 train_task = Task(
                     name=self.train_task_name,
                     data=data_shareable,
+                    operator=operator,
                     props={},
                     timeout=self._train_timeout,
                     before_task_sent_cb=self._prepare_train_task_data,
                     result_received_cb=self._process_train_result,
                 )
 
                 self.broadcast_and_wait(
@@ -282,15 +293,15 @@
                 # need to persist snapshot after round increased because the global weights should be set to
                 # the last finished round's result
                 if self._snapshot_every_n_rounds != 0 and self._current_round % self._snapshot_every_n_rounds == 0:
                     self._engine.persist_components(fl_ctx, completed=False)
 
             self._phase = AppConstants.PHASE_FINISHED
             self.log_info(fl_ctx, "Finished ScatterAndGather Training.")
-        except Exception as e:
+        except BaseException as e:
             error_msg = f"Exception in ScatterAndGather control_flow: {secure_format_exception(e)}"
             self.log_exception(fl_ctx, error_msg)
             self.system_panic(error_msg, fl_ctx)
 
     def stop_controller(self, fl_ctx: FLContext):
         self._phase = AppConstants.PHASE_FINISHED
```

## nvflare/app_common/workflows/scatter_and_gather_scaffold.py

```diff
@@ -26,15 +26,15 @@
 from nvflare.app_common.workflows.scatter_and_gather import ScatterAndGather
 from nvflare.security.logging import secure_format_exception
 
 
 class ScatterAndGatherScaffold(ScatterAndGather):
     def __init__(
         self,
-        min_clients: int = 1,
+        min_clients: int = 1000,
         num_rounds: int = 5,
         start_round: int = 0,
         wait_time_after_min_received: int = 10,
         aggregator_id=AppConstants.DEFAULT_AGGREGATOR_ID,
         persistor_id=AppConstants.DEFAULT_PERSISTOR_ID,
         shareable_generator_id=AppConstants.DEFAULT_SHAREABLE_GENERATOR_ID,
         train_task_name=AppConstants.TASK_TRAIN,
@@ -48,19 +48,21 @@
 
         The model persistor (persistor_id) is used to load the initial global model which is sent to all clients.
         Each client sends it's updated weights after local training which is aggregated (aggregator_id). The
         shareable generator is used to convert the aggregated weights to shareable and shareable back to weight.
         The model_persistor also saves the model after training.
 
         Args:
-            min_clients (int, optional): Min number of clients in training. Defaults to 1.
+            min_clients (int, optional): The minimum number of clients responses before
+                SAG starts to wait for `wait_time_after_min_received`. Note that SAG will move forward when all
+                available clients have responded regardless of this value. Defaults to 1000.
             num_rounds (int, optional): The total number of training rounds. Defaults to 5.
             start_round (int, optional): Start round for training. Defaults to 0.
             wait_time_after_min_received (int, optional): Time to wait before beginning aggregation after
-                contributions received. Defaults to 10.
+                minimum number of clients responses has been received. Defaults to 10.
             aggregator_id (str, optional): ID of the aggregator component. Defaults to "aggregator".
             persistor_id (str, optional): ID of the persistor component. Defaults to "persistor".
             shareable_generator_id (str, optional): ID of the shareable generator. Defaults to "shareable_generator".
             train_task_name (str, optional): Name of the train task. Defaults to "train".
             train_timeout (int, optional): Time to wait for clients to do local training.
             ignore_result_error (bool, optional): whether this controller can proceed if client result has errors.
                 Defaults to False.
@@ -218,11 +220,11 @@
                 # need to persist snapshot after round increased because the global weights should be set to
                 # the last finished round's result
                 if self._snapshot_every_n_rounds != 0 and self._current_round % self._snapshot_every_n_rounds == 0:
                     self._engine.persist_components(fl_ctx, completed=False)
 
             self._phase = AppConstants.PHASE_FINISHED
             self.log_info(fl_ctx, "Finished ScatterAndGatherScaffold Training.")
-        except Exception as e:
+        except BaseException as e:
             error_msg = f"Exception in ScatterAndGatherScaffold control_flow: {secure_format_exception(e)}"
             self.log_exception(fl_ctx, error_msg)
             self.system_panic(error_msg, fl_ctx)
```

## nvflare/app_common/workflows/splitnn_workflow.py

```diff
@@ -250,15 +250,15 @@
 
             # 2. Start split learning
             self._phase = AppConstants.PHASE_TRAIN
             self._train(abort_signal=abort_signal, fl_ctx=fl_ctx)
 
             self._phase = AppConstants.PHASE_FINISHED
             self.log_debug(fl_ctx, "SplitNN training ended.")
-        except Exception as e:
+        except BaseException as e:
             error_msg = f"SplitNN control_flow exception {secure_format_exception(e)}"
             self.log_error(fl_ctx, error_msg)
             self.system_panic(error_msg, fl_ctx)
 
     def stop_controller(self, fl_ctx: FLContext):
         self._phase = AppConstants.PHASE_FINISHED
         self.log_debug(fl_ctx, "controller stopped")
```

## nvflare/app_opt/he/model_shareable_generator.py

```diff
@@ -48,15 +48,15 @@
             n_vars_total = global_var.size()
         else:
             raise ValueError(f"global_var has type {type(global_var)} which is not supported.")
 
         # update the global model
         updated_vars = new_val + global_var
 
-    except Exception as e:
+    except BaseException as e:
         raise ValueError(f"add_to_global_weights Exception: {secure_format_exception(e)}") from e
 
     return updated_vars, n_vars_total
 
 
 class HEModelShareableGenerator(ShareableGenerator):
     def __init__(self, tenseal_context_file="server_context.tenseal"):
@@ -134,15 +134,15 @@
 
         Returns:
             Learnable object
         """
         self.log_info(fl_ctx, "shareable_to_learnable...")
         try:
             return self._shareable_to_learnable(shareable, fl_ctx)
-        except Exception as e:
+        except BaseException as e:
             self.log_exception(fl_ctx, "error converting shareable to model")
             raise ValueError(f"{self._name} Exception {secure_format_exception(e)}") from e
 
     def learnable_to_shareable(self, model_learnable: ModelLearnable, fl_ctx: FLContext) -> Shareable:
         """Convert ModelLearnable to Shareable.
 
         Args:
```

## nvflare/app_opt/pt/fedopt.py

```diff
@@ -122,15 +122,15 @@
                 # use provided or default optimizer arguments and add the model parameters
                 if "args" not in self.optimizer_args:
                     self.optimizer_args["args"] = {}
                 self.optimizer_args["args"]["params"] = self.model.parameters()
                 self.optimizer = engine.build_component(self.optimizer_args)
                 # get optimizer name for log
                 self.optimizer_name = self._get_component_name(self.optimizer_args)
-            except Exception as e:
+            except BaseException as e:
                 self.system_panic(
                     f"Exception while parsing `optimizer_args`({self.optimizer_args}): {secure_format_exception(e)}",
                     fl_ctx,
                 )
                 return
 
             # set up lr scheduler
@@ -138,15 +138,15 @@
                 try:
                     self.lr_scheduler_name = self._get_component_name(self.lr_scheduler_args)
                     # use provided or default lr scheduler argument and add the optimizer
                     if "args" not in self.lr_scheduler_args:
                         self.lr_scheduler_args["args"] = {}
                     self.lr_scheduler_args["args"]["optimizer"] = self.optimizer
                     self.lr_scheduler = engine.build_component(self.lr_scheduler_args)
-                except Exception as e:
+                except BaseException as e:
                     self.system_panic(
                         f"Exception while parsing `lr_scheduler_args`({self.lr_scheduler_args}): {secure_format_exception(e)}",
                         fl_ctx,
                     )
                     return
 
     def server_update(self, model_diff):
```

## nvflare/app_opt/pt/file_model_persistor.py

```diff
@@ -107,27 +107,27 @@
         self.global_model_file_name = global_model_file_name
         self.best_global_model_file_name = best_global_model_file_name
         self.source_ckpt_file_full_name = source_ckpt_file_full_name
 
         self.default_train_conf = None
 
         if source_ckpt_file_full_name and not os.path.exists(source_ckpt_file_full_name):
-            raise ValueError("specified source checkpoint model file {} does not exist")
+            raise ValueError(f"specified source checkpoint model file {source_ckpt_file_full_name} does not exist")
 
     def _initialize(self, fl_ctx: FLContext):
         app_root = fl_ctx.get_prop(FLContextKey.APP_ROOT)
         env = None
         run_args = fl_ctx.get_prop(FLContextKey.ARGS)
         if run_args:
             env_config_file_name = os.path.join(app_root, run_args.env)
             if os.path.exists(env_config_file_name):
                 try:
                     with open(env_config_file_name) as file:
                         env = json.load(file)
-                except Exception:
+                except BaseException:
                     self.system_panic(
                         reason="error opening env config file {}".format(env_config_file_name), fl_ctx=fl_ctx
                     )
                     return
 
         if env is not None:
             if env.get(self.ckpt_dir_env_key, None):
@@ -193,24 +193,24 @@
             src_file_name = self.ckpt_preload_path
 
         if src_file_name:
             try:
                 device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
                 data = torch.load(src_file_name, map_location=device)
                 # "checkpoint may contain 'model', 'optimizer', 'lr_scheduler', etc. or only contain model dict directly."
-            except Exception:
+            except BaseException:
                 self.log_exception(fl_ctx, "error loading checkpoint from {}".format(src_file_name))
                 self.system_panic(reason="cannot load model checkpoint", fl_ctx=fl_ctx)
                 return None
         else:
             # if no pretrained model provided, use the generated network weights from APP config
             # note that, if set "determinism" in the config, the init model weights will always be the same
             try:
                 data = self.model.state_dict() if self.model is not None else OrderedDict()
-            except Exception:
+            except BaseException:
                 self.log_exception(fl_ctx, "error getting state_dict from model object")
                 self.system_panic(reason="cannot create state_dict from model object", fl_ctx=fl_ctx)
                 return None
 
         if self.model:
             self.default_train_conf = {"train": {"model": type(self.model).__name__}}
 
@@ -237,15 +237,15 @@
             # device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
             # Use the "cpu" to load the global model weights, avoid GPU out of memory
             device = "cpu"
             location = os.path.join(self.log_dir, model_file)
             data = torch.load(location, map_location=device)
             persistence_manager = PTModelPersistenceFormatManager(data, default_train_conf=self.default_train_conf)
             return persistence_manager.to_model_learnable(self.exclude_vars)
-        except Exception:
+        except BaseException:
             self.log_exception(fl_ctx, "error loading checkpoint from {}".format(model_file))
             return {}
 
     def get_model_inventory(self, fl_ctx: FLContext) -> Dict[str, ModelDescriptor]:
         model_inventory = {}
         location = os.path.join(self.log_dir, self.global_model_file_name)
         if os.path.exists(location):
```

## nvflare/app_opt/pt/he_model_reader_writer.py

```diff
@@ -60,9 +60,9 @@
                         raise RuntimeError(f"{self._name} reshaping Exception: {secure_format_exception(e)}")
 
             assign_ops, updated_local_model = feed_vars(net, model_params)
             self.logger.debug(f"assign_ops: {len(assign_ops)}")
             self.logger.debug(f"updated_local_model: {len(updated_local_model)}")
             net.load_state_dict(updated_local_model)
             return assign_ops
-        except Exception as e:
+        except BaseException as e:
             raise RuntimeError(f"{self._name} apply_model Exception: {secure_format_exception(e)}")
```

## nvflare/app_opt/sklearn/sklearn_executor.py

```diff
@@ -19,125 +19,147 @@
 from nvflare.apis.dxo import DXO, DataKind, MetaKey, from_shareable
 from nvflare.apis.event_type import EventType
 from nvflare.apis.executor import Executor
 from nvflare.apis.fl_constant import FLContextKey, ReturnCode
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.shareable import Shareable, make_reply
 from nvflare.apis.signal import Signal
+from nvflare.app_common.abstract.learner_spec import Learner
 from nvflare.app_common.app_constant import AppConstants
 from nvflare.security.logging import secure_format_exception
 
 
+def _get_global_params(shareable: Shareable, fl_ctx: FLContext):
+    # retrieve current global params download from server's shareable
+    dxo = from_shareable(shareable)
+    current_round = shareable.get_header(AppConstants.CURRENT_ROUND)
+    fl_ctx.set_prop(AppConstants.CURRENT_ROUND, current_round)
+    return current_round, dxo.data
+
+
 class SKLearnExecutor(Executor):
-    def __init__(self, learner_id: str):
+    def __init__(self, learner_id: str, train_task=AppConstants.TASK_TRAIN):
+        """An Executor interface for scikit-learn Learner.
+
+        Args:
+            learner_id (str): id pointing to the learner object
+            train_task (str, optional): label to dispatch train task. Defaults to AppConstants.TASK_TRAIN.
+        """
         super().__init__()
-        self.client_id = None
-        self.writer = None
         self.learner_id = learner_id
+        self.learner = None
+        self.train_task = train_task
         self.local_model_path = None
         self.global_model_path = None
-        self.learner = None
+        self.client_id = None
+        self.writer = None
         self.fl_ctx = None
 
+    def handle_event(self, event_type: str, fl_ctx: FLContext):
+        if event_type == EventType.START_RUN:
+            self.initialize(fl_ctx)
+        elif event_type == EventType.ABORT_TASK:
+            try:
+                if self.learner:
+                    self.learner.abort(fl_ctx)
+            except Exception as e:
+                self.log_exception(fl_ctx, f"learner abort exception: {secure_format_exception(e)}")
+        elif event_type == EventType.END_RUN:
+            self.finalize(fl_ctx)
+
     def initialize(self, fl_ctx: FLContext):
         self.fl_ctx = fl_ctx
         self._print_configs(fl_ctx)
         self.load_log_tracker()
 
-        engine = fl_ctx.get_engine()
-        self.learner = engine.get_component(self.learner_id)
-        self.learner.initialize(fl_ctx)
+        try:
+            engine = fl_ctx.get_engine()
+            self.learner = engine.get_component(self.learner_id)
+            if not isinstance(self.learner, Learner):
+                raise TypeError(f"learner must be Learner type. Got: {type(self.learner)}")
+            self.learner.initialize(engine.get_all_components(), fl_ctx)
+        except Exception as e:
+            self.log_exception(fl_ctx, f"learner initialize exception: {secure_format_exception(e)}")
 
         # set the paths according to fl_ctx
         app_dir = fl_ctx.get_prop(FLContextKey.APP_ROOT)
         self.local_model_path = os.path.join(app_dir, "model_local.joblib")
         self.global_model_path = os.path.join(app_dir, "model_global.joblib")
 
-    def get_global_params(self, shareable: Shareable, fl_ctx: FLContext):
-        # retrieve current global center download from server's shareable
-        dxo = from_shareable(shareable)
-        current_round = shareable.get_header(AppConstants.CURRENT_ROUND)
-        fl_ctx.set_prop(AppConstants.CURRENT_ROUND, current_round)
-        return current_round, dxo.data
+    def execute(
+        self,
+        task_name: str,
+        shareable: Shareable,
+        fl_ctx: FLContext,
+        abort_signal: Signal,
+    ) -> Shareable:
+        self.log_info(fl_ctx, f"Client trainer got task: {task_name}")
+        if abort_signal.triggered:
+            self.finalize(fl_ctx)
+            return make_reply(ReturnCode.TASK_ABORTED)
+
+        try:
+            if task_name == self.train_task:
+                (current_round, global_params) = _get_global_params(shareable, fl_ctx)
+                if current_round > 0:
+                    # first round for parameter initialization
+                    # no model evaluation
+                    self.validate(current_round, global_params, fl_ctx)
+                return self.train(current_round, global_params, fl_ctx)
+            else:
+                self.log_error(fl_ctx, f"Could not handle task: {task_name}")
+                return make_reply(ReturnCode.TASK_UNKNOWN)
+        except Exception as e:
+            # Task execution error, return EXECUTION_EXCEPTION Shareable
+            self.log_exception(fl_ctx, f"learner execute exception: {secure_format_exception(e)}")
+            return make_reply(ReturnCode.EXECUTION_EXCEPTION)
 
     def train(self, current_round, global_param, fl_ctx: FLContext) -> Shareable:
-        self._msg_log(f"Client {self.client_id} perform local train")
+        self.log_info(fl_ctx, f"Client {self.client_id} perform local train")
         # sklearn algorithms usually needs two different processing schemes
         # one for first round (generate initial centers for clustering, regular training for svm)
         # the other for following rounds (regular training for clustering, no further training for svm)
         # hence the current round is fed to learner to distinguish the two
         params, model = self.learner.train(current_round, global_param, fl_ctx)
         # save model and return dxo containing the params
         self.save_model_local(model)
         dxo = DXO(data_kind=DataKind.WEIGHTS, data=params)
         dxo.set_meta_prop(MetaKey.NUM_STEPS_CURRENT_ROUND, self.learner.n_samples)
-        self._msg_log("Local epochs finished. Returning shareable")
+        self.log_info(fl_ctx, "Local epochs finished. Returning shareable")
 
         return dxo.to_shareable()
 
     def validate(self, current_round, global_param, fl_ctx: FLContext) -> Shareable:
         # retrieve current global center download from server's shareable
-        self._msg_log(f"Client {self.client_id} perform local evaluation")
+        self.log_info(fl_ctx, f"Client {self.client_id} perform local evaluation")
         metrics, model = self.learner.validate(current_round, global_param, fl_ctx)
         self.save_model_global(model)
         for key, value in metrics.items():
             self.log_value(key, value, current_round)
 
     def finalize(self, fl_ctx: FLContext):
-        self.learner.finalize(fl_ctx)
-
-    def execute(
-        self,
-        task_name: str,
-        shareable: Shareable,
-        fl_ctx: FLContext,
-        abort_signal: Signal,
-    ) -> Shareable:
-        self._msg_log(f"Client trainer got task: {task_name}")
-        if abort_signal.triggered:
-            self.finalize(fl_ctx)
-            return make_reply(ReturnCode.TASK_ABORTED)
         try:
-            if task_name == AppConstants.TASK_TRAIN:
-                (current_round, global_params) = self.get_global_params(shareable, fl_ctx)
-                if current_round > 0:
-                    # first round for parameter initialization
-                    # no model evaluation
-                    self.validate(current_round, global_params, fl_ctx)
-                return self.train(current_round, global_params, fl_ctx)
-            else:
-                self.log_error(fl_ctx, f"Could not handle task: {task_name}")
-                return make_reply(ReturnCode.TASK_UNKNOWN)
+            if self.learner:
+                self.learner.finalize(fl_ctx)
         except Exception as e:
-            # Task execution error, return EXECUTION_EXCEPTION Shareable
-            self.log_exception(fl_ctx, f"execute exception: {secure_format_exception(e)}")
-            return make_reply(ReturnCode.EXECUTION_EXCEPTION)
-
-    def handle_event(self, event_type: str, fl_ctx: FLContext):
-        if event_type == EventType.START_RUN:
-            self.initialize(fl_ctx)
-        elif event_type == EventType.END_RUN:
-            self.finalize(fl_ctx)
+            self.log_exception(fl_ctx, f"learner finalize exception: {secure_format_exception(e)}")
 
     def _print_configs(self, fl_ctx: FLContext):
         # get and print the args
         fl_args = fl_ctx.get_prop(FLContextKey.ARGS)
         self.client_id = fl_ctx.get_identity_name()
         self.log_info(
             fl_ctx,
             f"Client {self.client_id} initialized with configs: \n {fl_args}",
         )
 
     def load_log_tracker(self):
         app_dir = self.fl_ctx.get_prop(FLContextKey.APP_ROOT)
         self.writer = tensorboard.summary.Writer(app_dir)
 
-    def _msg_log(self, msg: str):
-        self.log_info(self.fl_ctx, msg)
-
     def log_value(self, key, value, step):
         if self.writer:
             self.writer.add_scalar(key, value, step)
             self.writer.flush()
 
     def save_model_local(self, model: any) -> None:
         joblib.dump(model, self.local_model_path)
```

## nvflare/app_opt/xgboost/histogram_based/controller.py

```diff
@@ -155,12 +155,12 @@
                 min_responses=len(self._participate_clients),
                 fl_ctx=fl_ctx,
                 abort_signal=abort_signal,
             )
 
             self.log_info(fl_ctx, "Finish training phase.")
 
-        except Exception as e:
+        except BaseException as e:
             err = secure_format_traceback()
             error_msg = f"Exception in control_flow: {secure_format_exception(e)}: {err}"
             self.log_exception(fl_ctx, error_msg)
             self.system_panic(secure_format_exception(e), fl_ctx)
```

## nvflare/app_opt/xgboost/histogram_based/executor.py

```diff
@@ -208,13 +208,13 @@
 
                 # Save the model.
                 workspace = fl_ctx.get_prop(FLContextKey.WORKSPACE_OBJECT)
                 run_number = fl_ctx.get_prop(FLContextKey.CURRENT_RUN)
                 run_dir = workspace.get_run_dir(run_number)
                 bst.save_model(os.path.join(run_dir, "test.model.json"))
                 xgb.collective.communicator_print("Finished training\n")
-        except Exception as e:
+        except BaseException as e:
             secure_log_traceback()
             self.log_error(fl_ctx, f"Exception happens when running xgb train: {secure_format_exception(e)}")
             return make_reply(ReturnCode.EXECUTION_EXCEPTION)
 
         return make_reply(ReturnCode.OK)
```

## nvflare/app_opt/xgboost/tree_based/bagging_aggregator.py

```diff
@@ -47,15 +47,15 @@
 
         Returns:
             The first boolean indicates if this shareable is accepted.
             The second boolean indicates if aggregate can be called.
         """
         try:
             dxo = from_shareable(shareable)
-        except Exception:
+        except BaseException:
             self.log_exception(fl_ctx, "shareable data is not a valid DXO")
             return False
 
         contributor_name = shareable.get_peer_prop(key=ReservedKey.IDENTITY_NAME, default="?")
         contribution_round = shareable.get_cookie(AppConstants.CONTRIBUTION_ROUND)
 
         rc = shareable.get_return_code()
```

## nvflare/dashboard/cli.py

```diff
@@ -15,14 +15,15 @@
 import argparse
 import os
 import signal
 import subprocess
 import sys
 
 import docker
+import nvflare
 from nvflare.apis.utils.format_check import name_check
 from nvflare.dashboard.application.blob import _write
 from nvflare.lighter import utils
 
 supported_csp = ("azure", "aws")
 
 
@@ -59,15 +60,22 @@
         print(f"Project admin credential is {answer} and the password is {pwd}")
         environment.update({"NVFL_CREDENTIAL": f"{answer}:{pwd}"})
     try:
         client = docker.from_env()
     except docker.errors.DockerException:
         print("Unable to communicate to docker daemon/socket.  Please make sure your docker is up and running.")
         exit(0)
-    dashboard_image = "nvflare/nvflare"
+    version = nvflare.__version__
+    dashboard_image = f"nvflare/nvflare:{version}"
+    if args.image:
+        if dashboard_image != args.image:
+            print(
+                f"Current dashboard container image is nvflare/nvflare:{version}, but requesting to use {args.image}.  Use it at your own risk."
+            )
+            dashboard_image = args.image
     try:
         print(f"Pulling {dashboard_image}, may take some time to finish.")
         _ = client.images.pull(dashboard_image)
     except docker.errors.APIError:
         print(f"unable to pull {dashboard_image}")
         exit(1)
     print(f"Launching {dashboard_image}")
@@ -118,22 +126,25 @@
 
 def cloud(args):
     lighter_folder = os.path.dirname(utils.__file__)
     template = utils.load_yaml(os.path.join(lighter_folder, "impl", "master_template.yml"))
     cwd = os.getcwd()
     csp = args.cloud
     dest = os.path.join(cwd, f"{csp}_start_dsb.sh")
+    dsb_start = template[f"{csp}_start_dsb_sh"]
+    version = nvflare.__version__
+    replacement_dict = {"NVFLARE": f"nvflare=={version}", "START_OPT": f"-i {args.image}" if args.image else ""}
     _write(
         dest,
-        template[f"{csp}_start_dsb_sh"],
+        utils.sh_replace(dsb_start, replacement_dict),
         "t",
         exe=True,
     )
     print(f"Dashboard launch script for cloud is written at {dest}.  Now running the script.")
-    process = subprocess.run(dest)
+    _ = subprocess.run(dest)
     os.remove(dest)
 
 
 def has_no_arguments() -> bool:
     last_item = sys.argv[-1]
     return (
         last_item.endswith("dashboard.cli") or last_item.endswith("dashboard/cli.py") or last_item.endswith("dashboard")
@@ -161,14 +172,15 @@
         "-f", "--folder", type=str, help="folder containing necessary info (default: current working directory)"
     )
     parser.add_argument(
         "--passphrase", help="Passphrase to encrypt/decrypt root CA private key.  !!! Do not share it with others. !!!"
     )
     parser.add_argument("-e", "--env", action="append", help="additonal environment variables: var1=value1")
     parser.add_argument("--cred", help="set credential directly in the form of USER_EMAIL:PASSWORD")
+    parser.add_argument("-i", "--image", help="set the container image name")
 
 
 def handle_dashboard(args):
     support_csp_string = ", ".join(supported_csp)
     if args.stop:
         stop()
     elif args.start:
```

## nvflare/dashboard/application/blob.py

```diff
@@ -14,15 +14,15 @@
 
 import io
 import json
 import os
 import subprocess
 import tempfile
 
-from nvflare.lighter import utils
+from nvflare.lighter import tplt_utils, utils
 
 from .cert import CertPair, Entity, deserialize_ca_key, make_cert
 from .models import Client, Project, User
 
 lighter_folder = os.path.dirname(utils.__file__)
 template = utils.load_yaml(os.path.join(lighter_folder, "impl", "master_template.yml"))
 
@@ -92,14 +92,15 @@
     signing_cert_pair = CertPair(issuer, project.root_key, project.root_cert)
     cert_pair = make_cert(entity, signing_cert_pair)
 
     config = json.loads(template["fed_server"])
     server_0 = config["servers"][0]
     server_0["name"] = project.short_name
     server_0["service"]["target"] = f"{entity.name}:{fl_port}"
+    server_0["service"]["scheme"] = project.scheme if hasattr(project, "scheme") else "grpc"
     server_0["admin_host"] = entity.name
     server_0["admin_port"] = admin_port
     if project.ha_mode:
         overseer_agent = {"path": "nvflare.ha.overseer_agent.HttpOverseerAgent"}
         overseer_agent["args"] = {
             "role": "server",
             "overseer_end_point": f"https://{project.overseer}:8443/api/v1",
@@ -114,23 +115,31 @@
 
     config["overseer_agent"] = overseer_agent
     replacement_dict = {
         "admin_port": admin_port,
         "fed_learn_port": fl_port,
         "config_folder": "config",
         "ha_mode": "true" if project.ha_mode else "false",
+        "docker_image": project.app_location.split(" ")[-1] if project.app_location else "nvflare/nvflare",
         "org_name": "",
     }
+    tplt = tplt_utils.Template(template)
     with tempfile.TemporaryDirectory() as tmp_dir:
         server_dir = os.path.join(tmp_dir, entity.name)
         dest_dir = os.path.join(server_dir, "startup")
         os.mkdir(server_dir)
         os.mkdir(dest_dir)
         _write(os.path.join(dest_dir, "fed_server.json"), json.dumps(config, indent=2), "t")
         _write(
+            os.path.join(dest_dir, "docker.sh"),
+            utils.sh_replace(template["docker_svr_sh"], replacement_dict),
+            "t",
+            exe=True,
+        )
+        _write(
             os.path.join(dest_dir, "start.sh"),
             utils.sh_replace(template["start_svr_sh"], replacement_dict),
             "t",
             exe=True,
         )
         _write(
             os.path.join(dest_dir, "sub_start.sh"),
@@ -146,21 +155,27 @@
         )
         _write(os.path.join(dest_dir, "server.crt"), cert_pair.ser_cert, "b", exe=False)
         _write(os.path.join(dest_dir, "server.key"), cert_pair.ser_pri_key, "b", exe=False)
         _write(os.path.join(dest_dir, "rootCA.pem"), project.root_cert, "b", exe=False)
         if not project.ha_mode:
             _write(
                 os.path.join(dest_dir, get_csp_start_script_name("azure")),
-                utils.sh_replace(get_csp_template("azure", "svr", template), {"server_name": entity.name}),
+                utils.sh_replace(
+                    tplt.get_cloud_script_header() + get_csp_template("azure", "svr", template),
+                    {"server_name": entity.name, "ORG": ""},
+                ),
                 "t",
                 exe=True,
             )
             _write(
                 os.path.join(dest_dir, get_csp_start_script_name("aws")),
-                utils.sh_replace(get_csp_template("aws", "svr", template), {"server_name": entity.name}),
+                utils.sh_replace(
+                    tplt.get_cloud_script_header() + get_csp_template("aws", "svr", template),
+                    {"server_name": entity.name, "ORG": ""},
+                ),
                 "t",
                 exe=True,
             )
         signatures = utils.sign_all(dest_dir, deserialize_ca_key(project.root_key))
         json.dump(signatures, open(os.path.join(dest_dir, "signature.json"), "wt"))
 
         # local folder creation
@@ -208,18 +223,19 @@
     entity = Entity(client.name, client.organization.name)
     issuer = Entity(project.short_name)
     signing_cert_pair = CertPair(issuer, project.root_key, project.root_cert)
     cert_pair = make_cert(entity, signing_cert_pair)
 
     config = json.loads(template["fed_client"])
     config["servers"][0]["name"] = project.short_name
+    config["servers"][0]["service"]["scheme"] = project.scheme if hasattr(project, "scheme") else "grpc"
     replacement_dict = {
         "client_name": entity.name,
         "config_folder": "config",
-        "docker_image": "",
+        "docker_image": project.app_location.split(" ")[-1] if project.app_location else "nvflare/nvflare",
         "org_name": entity.org,
     }
     if project.ha_mode:
         overseer_agent = {"path": "nvflare.ha.overseer_agent.HttpOverseerAgent"}
         overseer_agent["args"] = {
             "role": "client",
             "overseer_end_point": f"https://{project.overseer}:8443/api/v1",
@@ -227,22 +243,29 @@
             "name": entity.name,
         }
     else:
         overseer_agent = {"path": "nvflare.ha.dummy_overseer_agent.DummyOverseerAgent"}
         overseer_agent["args"] = {"sp_end_point": f"{project.server1}:8002:8003"}
     config["overseer_agent"] = overseer_agent
 
+    tplt = tplt_utils.Template(template)
     with tempfile.TemporaryDirectory() as tmp_dir:
         client_dir = os.path.join(tmp_dir, entity.name)
         dest_dir = os.path.join(client_dir, "startup")
         os.mkdir(client_dir)
         os.mkdir(dest_dir)
 
         _write(os.path.join(dest_dir, "fed_client.json"), json.dumps(config, indent=2), "t")
         _write(
+            os.path.join(dest_dir, "docker.sh"),
+            utils.sh_replace(template["docker_cln_sh"], replacement_dict),
+            "t",
+            exe=True,
+        )
+        _write(
             os.path.join(dest_dir, "start.sh"),
             template["start_cln_sh"],
             "t",
             exe=True,
         )
         _write(
             os.path.join(dest_dir, "sub_start.sh"),
@@ -257,21 +280,27 @@
             exe=True,
         )
         _write(os.path.join(dest_dir, "client.crt"), cert_pair.ser_cert, "b", exe=False)
         _write(os.path.join(dest_dir, "client.key"), cert_pair.ser_pri_key, "b", exe=False)
         _write(os.path.join(dest_dir, "rootCA.pem"), project.root_cert, "b", exe=False)
         _write(
             os.path.join(dest_dir, get_csp_start_script_name("azure")),
-            get_csp_template("azure", "cln", template),
+            utils.sh_replace(
+                tplt.get_cloud_script_header() + get_csp_template("azure", "cln", template),
+                {"SITE": entity.name, "ORG": entity.org},
+            ),
             "t",
             exe=True,
         )
         _write(
             os.path.join(dest_dir, get_csp_start_script_name("aws")),
-            get_csp_template("aws", "cln", template),
+            utils.sh_replace(
+                tplt.get_cloud_script_header() + get_csp_template("aws", "cln", template),
+                {"SITE": entity.name, "ORG": entity.org},
+            ),
             "t",
             exe=True,
         )
         signatures = utils.sign_all(dest_dir, deserialize_ca_key(project.root_key))
         json.dump(signatures, open(os.path.join(dest_dir, "signature.json"), "wt"))
 
         # local folder creation
```

## nvflare/dashboard/application/models.py

```diff
@@ -51,14 +51,15 @@
 class Project(db.Model):
     id = db.Column(db.Integer, primary_key=True)
     frozen = db.Column(db.Boolean, default=False)
     public = db.Column(db.Boolean, default=False)
     short_name = db.Column(db.String(128), default="")
     title = db.Column(db.String(512), default="")
     description = db.Column(db.String(2048), default="")
+    # scheme = db.Column(db.String(16), default="grpc")
     app_location = db.Column(db.String(2048), default="")
     ha_mode = db.Column(db.Boolean, default=False)
     starting_date = db.Column(db.String(128), default="")
     end_date = db.Column(db.String(128), default="")
     overseer = db.Column(db.String(128), default="")
     server1 = db.Column(db.String(128), default="")
     server2 = db.Column(db.String(128), default="")
```

## nvflare/dashboard/application/store.py

```diff
@@ -172,15 +172,15 @@
             cap = get_or_create(db.session, Capacity, capacity=json.dumps(capacity))
         client = Client(name=name, description=description, creator_id=creator_id)
         client.organization_id = org.id
         client.capacity_id = cap.id
         try:
             db.session.add(client)
             db.session.commit()
-        except Exception as e:
+        except BaseException as e:
             log.error(f"Error while creating client: {e}")
             return None
         return add_ok({"client": _dict_or_empty(client)})
 
     @classmethod
     def get_clients(cls, org=None):
         if org is None:
@@ -217,15 +217,15 @@
             cap = get_or_create(db.session, Capacity, capacity=capacity)
             client.capacity_id = cap.id
         for k, v in req.items():
             setattr(client, k, v)
         try:
             db.session.add(client)
             db.session.commit()
-        except Exception as e:
+        except BaseException as e:
             log.error(f"Error while patching client: {e}")
             return None
         return add_ok({"client": _dict_or_empty(client)})
 
     @classmethod
     def patch_client_by_creator(cls, id, req):
         client = Client.query.get(id)
@@ -240,15 +240,15 @@
             cap = get_or_create(db.session, Capacity, capacity=capacity)
             client.capacity_id = cap.id
         for k, v in req.items():
             setattr(client, k, v)
         try:
             db.session.add(client)
             db.session.commit()
-        except Exception as e:
+        except BaseException as e:
             log.error(f"Error while patching client: {e}")
             return None
         return add_ok({"client": _dict_or_empty(client)})
 
     @classmethod
     def delete_client(cls, id):
         client = Client.query.get(id)
@@ -282,15 +282,15 @@
                 description=description,
                 approval_state=approval_state,
             )
             user.organization_id = org.id
             user.role_id = role.id
             db.session.add(user)
             db.session.commit()
-        except Exception as e:
+        except BaseException as e:
             log.error(f"Error while creating user: {e}")
             return None
         return add_ok({"user": _dict_or_empty(user)})
 
     @classmethod
     def verify_user(cls, email, password):
         user = User.query.filter_by(email=email).first()
```

## nvflare/fuel/f3/message.py

```diff
@@ -8,40 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import Any, Optional
 
 from nvflare.fuel.f3.connection import Connection
 from nvflare.fuel.f3.endpoint import Endpoint
 
 
 class AppIds:
     """Reserved application IDs"""
 
     ALL = 0
     DEFAULT = 1
     CELL_NET = 2
     PUB_SUB = 3
 
 
-class Headers(dict):
-
-    # Reserved Keys
-    MSG_ID = "_MSG_ID_"
-    TOPIC = "_TOPIC_"
-    DEST = "_DEST_"
-    JOB_ID = "_JOB_ID_"
-
-
 class Message:
-    def __init__(self, headers: Headers, payload: Any):
+    def __init__(self, headers: Optional[dict] = None, payload: Any = None):
         """Construct an FCI message"""
 
         self.headers = headers
         self.payload = payload
 
     def set_header(self, key: str, value):
         if self.headers is None:
```

## nvflare/fuel/f3/stats_pool.py

```diff
@@ -8,46 +8,440 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import csv
+import json
+import sys
 import threading
+import time
+from typing import List, Tuple, Union
 
-from nvflare.fuel.utils.stats_utils import CounterPool, HistPool, new_message_size_pool, new_time_pool
+_KEY_MAX = "max"
+_KEY_MIN = "min"
+_KEY_NAME = "name"
+_KEY_DESC = "description"
+_KEY_TOTAL = "total"
+_KEY_COUNT = "count"
+_KEY_UNIT = "unit"
+_KEY_MARKS = "marks"
+_KEY_COUNTER_NAMES = "counter_names"
+_KEY_CAT_DATA = "cat_data"
+
+
+class StatsMode:
+
+    COUNT = "count"
+    PERCENT = "percent"
+    AVERAGE = "avg"
+    MIN = "min"
+    MAX = "max"
+
+
+VALID_HIST_MODES = [StatsMode.COUNT, StatsMode.PERCENT, StatsMode.AVERAGE, StatsMode.MAX, StatsMode.MIN]
+
+
+def format_value(v: float, n=3):
+    if v is None:
+        return "n/a"
+    fmt = "{:." + str(n) + "e}"
+    return fmt.format(v)
+
+
+class _Bin:
+    def __init__(self, count=0, total_value=0.0, min_value=None, max_value=None):
+        self.count = count
+        self.total = total_value
+        self.min = min_value
+        self.max = max_value
+
+    def record_value(self, value: float):
+        self.count += 1
+        self.total += value
+        if self.min is None or self.min > value:
+            self.min = value
+        if self.max is None or self.max < value:
+            self.max = value
+
+    def get_content(self, mode=StatsMode.COUNT, total_count=0):
+        if self.count == 0:
+            return ""
+        if mode == StatsMode.COUNT:
+            return str(self.count)
+        if mode == StatsMode.PERCENT:
+            return str(round(self.count / total_count, 2))
+        if mode == StatsMode.AVERAGE:
+            avg = self.total / self.count
+            return format_value(avg)
+        if mode == StatsMode.MIN:
+            return format_value(self.min)
+        if mode == StatsMode.MAX:
+            return format_value(self.max)
+        return "n/a"
+
+    def to_dict(self) -> dict:
+        return {
+            _KEY_COUNT: self.count,
+            _KEY_TOTAL: self.total,
+            _KEY_MIN: self.min if self.min is not None else "",
+            _KEY_MAX: self.max if self.max is not None else "",
+        }
+
+    @staticmethod
+    def from_dict(d: dict):
+        if not isinstance(d, dict):
+            raise ValueError(f"d must be dict but got {type(d)}")
+        b = _Bin()
+        b.count = d.get(_KEY_COUNT, 0)
+        b.total = d.get(_KEY_TOTAL, 0)
+        m = d.get(_KEY_MIN)
+        if isinstance(m, str):
+            b.min = None
+        else:
+            b.min = m
+        x = d.get(_KEY_MAX)
+        if isinstance(x, str):
+            b.max = None
+        else:
+            b.max = x
+        return b
+
+
+class StatsPool:
+    def __init__(self, name: str, description: str):
+        self.name = name
+        self.description = description
+
+    def to_dict(self) -> dict:
+        pass
+
+    def get_table(self, mode):
+        pass
+
+    @staticmethod
+    def from_dict(d: dict):
+        pass
+
+
+class RecordWriter:
+    def write(self, pool_name: str, category: str, value: float, report_time: float):
+        pass
+
+    def close(self):
+        pass
+
+
+class HistPool(StatsPool):
+    def __init__(self, name: str, description: str, marks: Union[List[float], Tuple], unit: str, record_writer=None):
+        if record_writer:
+            if not isinstance(record_writer, RecordWriter):
+                raise TypeError(f"record_writer must be RecordWriter but got {type(record_writer)}")
+
+        StatsPool.__init__(self, name, description)
+        self.update_lock = threading.Lock()
+        self.unit = unit
+        self.marks = marks
+        self.record_writer = record_writer  # used for writing raw records
+        self.cat_bins = {}  # category name => list of bins
+
+        if not marks:
+            raise ValueError("marks not specified")
+        if len(marks) < 2:
+            raise ValueError(f"marks must have at least two numbers but got {len(marks)}")
+
+        for i in range(1, len(marks)):
+            if marks[i] <= marks[i - 1]:
+                raise ValueError(f"marks must contain increasing values, but got {marks}")
+
+        # A range is defined: left <= N < right  [...)
+        # [..., M1) [M1, M2) [M2, M3) [M3, ...)
+        m = sys.float_info.max
+        self.ranges = [(-m, marks[0])]
+        self.range_names = [f"<{marks[0]}"]
+        for i in range(len(marks) - 1):
+            self.ranges.append((marks[i], marks[i + 1]))
+            self.range_names.append(f"{marks[i]}-{marks[i+1]}")
+        self.ranges.append((marks[-1], m))
+        self.range_names.append(f">={marks[-1]}")
+
+    def record_value(self, category: str, value: float):
+        with self.update_lock:
+            bins = self.cat_bins.get(category)
+            if bins is None:
+                bins = [None for _ in range(len(self.ranges))]
+                self.cat_bins[category] = bins
+
+            for i in range(len(self.ranges)):
+                r = self.ranges[i]
+                if r[0] <= value < r[1]:
+                    b = bins[i]
+                    if not b:
+                        b = _Bin()
+                        bins[i] = b
+                    b.record_value(value)
+
+            if self.record_writer:
+                self.record_writer.write(pool_name=self.name, category=category, value=value, report_time=time.time())
+
+    def get_table(self, mode=StatsMode.COUNT):
+        with self.update_lock:
+            headers = ["category"]
+            has_values = [False for _ in range(len(self.ranges))]
+
+            # determine bins that have values in any category
+            for _, bins in self.cat_bins.items():
+                for i in range(len(self.ranges)):
+                    if bins[i]:
+                        has_values[i] = True
+
+            for i in range(len(self.ranges)):
+                if has_values[i]:
+                    headers.append(self.range_names[i])
+
+            headers.append("overall")
+
+            rows = []
+            for cat_name in sorted(self.cat_bins.keys()):
+                bins = self.cat_bins[cat_name]
+                total_count = 0
+                total_value = 0.0
+                overall_min = None
+                overall_max = None
+
+                for b in bins:
+                    if b:
+                        total_count += b.count
+                        total_value += b.total
+                        if b.max is not None:
+                            if overall_max is None or overall_max < b.max:
+                                overall_max = b.max
+
+                        if b.min is not None:
+                            if overall_min is None or overall_min > b.min:
+                                overall_min = b.min
+
+                r = [cat_name]
+                for i in range(len(bins)):
+                    if not has_values[i]:
+                        continue
+
+                    b = bins[i]
+                    if not b:
+                        r.append("")
+                    else:
+                        r.append(b.get_content(mode, total_count))
+
+                # compute overall values
+                overall_bin = _Bin(
+                    count=total_count, total_value=total_value, max_value=overall_max, min_value=overall_min
+                )
+                r.append(overall_bin.get_content(mode, total_count))
+
+                rows.append(r)
+            return headers, rows
+
+    def to_dict(self):
+        with self.update_lock:
+            cat_bins = {}
+            for cat, bins in self.cat_bins.items():
+                exp_bins = []
+                for b in bins:
+                    if not b:
+                        exp_bins.append("")
+                    else:
+                        exp_bins.append(b.to_dict())
+                cat_bins[cat] = exp_bins
+            return {
+                _KEY_NAME: self.name,
+                _KEY_DESC: self.description,
+                _KEY_MARKS: list(self.marks),
+                _KEY_UNIT: self.unit,
+                _KEY_CAT_DATA: cat_bins,
+            }
+
+    @staticmethod
+    def from_dict(d: dict):
+        p = HistPool(
+            name=d.get(_KEY_NAME, ""),
+            description=d.get(_KEY_DESC, ""),
+            unit=d.get(_KEY_UNIT, ""),
+            marks=d.get(_KEY_MARKS),
+        )
+        cat_bins = d.get(_KEY_CAT_DATA)
+        if not cat_bins:
+            return p
+
+        for cat, bins in cat_bins.items():
+            in_bins = []
+            for b in bins:
+                if not b:
+                    in_bins.append(None)
+                else:
+                    assert isinstance(b, dict)
+                    in_bins.append(_Bin.from_dict(b))
+            p.cat_bins[cat] = in_bins
+        return p
+
+
+class CounterPool(StatsPool):
+    def __init__(self, name: str, description: str, counter_names: List[str], dynamic_counter_name=True):
+        if not counter_names and not dynamic_counter_name:
+            raise ValueError("counter_names cannot be empty")
+        StatsPool.__init__(self, name, description)
+        self.counter_names = counter_names
+        self.cat_counters = {}  # dict of cat_name => counter dict (counter_name => int)
+        self.dynamic_counter_name = dynamic_counter_name
+        self.update_lock = threading.Lock()
+
+    def increment(self, category: str, counter_name: str, amount=1):
+        with self.update_lock:
+            if counter_name not in self.counter_names:
+                if self.dynamic_counter_name:
+                    self.counter_names.append(counter_name)
+                else:
+                    raise ValueError(f"'{counter_name}' is not defined in pool '{self.name}'")
+
+            counters = self.cat_counters.get(category)
+            if not counters:
+                counters = {}
+                self.cat_counters[category] = counters
+            c = counters.get(counter_name, 0)
+            c += amount
+            counters[counter_name] = c
+
+    def get_table(self, mode=""):
+        with self.update_lock:
+            headers = ["category"]
+            eff_counter_names = []
+            for cn in self.counter_names:
+                for _, counters in self.cat_counters.items():
+                    v = counters.get(cn, 0)
+                    if v > 0:
+                        eff_counter_names.append(cn)
+                        break
+
+            headers.extend(eff_counter_names)
+            rows = []
+            for cat_name in sorted(self.cat_counters.keys()):
+                counters = self.cat_counters[cat_name]
+                r = [cat_name]
+                for cn in eff_counter_names:
+                    value = counters.get(cn, 0)
+                    r.append(str(value))
+                rows.append(r)
+            return headers, rows
+
+    def to_dict(self):
+        with self.update_lock:
+            return {
+                _KEY_NAME: self.name,
+                _KEY_DESC: self.description,
+                _KEY_COUNTER_NAMES: list(self.counter_names),
+                _KEY_CAT_DATA: self.cat_counters,
+            }
+
+    @staticmethod
+    def from_dict(d: dict):
+        p = CounterPool(
+            name=d.get(_KEY_NAME, ""), description=d.get(_KEY_DESC, ""), counter_names=d.get(_KEY_COUNTER_NAMES)
+        )
+        p.cat_counters = d.get(_KEY_CAT_DATA)
+        return p
+
+
+def new_time_pool(name: str, description="", marks=None, record_writer=None) -> HistPool:
+    if not marks:
+        marks = (0.0001, 0.0005, 0.001, 0.002, 0.004, 0.008, 0.01, 0.02, 0.04, 0.08, 0.1, 0.2, 0.4, 0.8, 1.0, 2.0)
+    return HistPool(name=name, description=description, marks=marks, unit="second", record_writer=record_writer)
+
+
+def new_message_size_pool(name: str, description="", marks=None, record_writer=None) -> HistPool:
+    if not marks:
+        marks = (0.01, 0.1, 1, 10, 50, 100, 200, 500, 800, 1000)
+    return HistPool(name=name, description=description, marks=marks, unit="MB", record_writer=record_writer)
+
+
+def parse_hist_mode(mode: str) -> str:
+    if not mode:
+        return StatsMode.COUNT
+
+    if mode.startswith("p"):
+        return StatsMode.PERCENT
+    elif mode.startswith("c"):
+        return StatsMode.COUNT
+    elif mode.startswith("a"):
+        return StatsMode.AVERAGE
+
+    if mode not in VALID_HIST_MODES:
+        return ""
+    else:
+        return mode
 
 
 class StatsPoolManager:
 
+    _CONFIG_KEY_SAVE_POOLS = "save_pools"
+
     lock = threading.Lock()
     pools = {}  # name => pool
+    pool_config = {}
+    record_writer = None
 
     @classmethod
     def _check_name(cls, name, scope):
         name = name.lower()
         if name not in cls.pools:
             return name
         if scope:
             name = f"{name}@{scope}"
             if name not in cls.pools:
                 return name
         raise ValueError(f"pool '{name}' is already defined")
 
     @classmethod
+    def set_pool_config(cls, config: dict):
+        if not isinstance(config, dict):
+            raise ValueError(f"config data must be dict but got {type(config)}")
+        for k, v in config.items():
+            cls.pool_config[k.lower()] = v
+
+    @classmethod
+    def set_record_writer(cls, record_writer: RecordWriter):
+        if not isinstance(record_writer, RecordWriter):
+            raise TypeError(f"record_writer must be RecordWriter but got {type(record_writer)}")
+        cls.record_writer = record_writer
+
+    @classmethod
+    def _keep_hist_records(cls, name):
+        name = name.lower()
+        save_pools_list = cls.pool_config.get(cls._CONFIG_KEY_SAVE_POOLS, None)
+        if not save_pools_list:
+            return False
+
+        return ("*" in save_pools_list) or (name in save_pools_list)
+
+    @classmethod
     def add_time_hist_pool(cls, name: str, description: str, marks=None, scope=None):
+        # check pool config
+        keep_records = cls._keep_hist_records(name)
         name = cls._check_name(name, scope)
-        p = new_time_pool(name, description, marks)
+        record_writer = cls.record_writer if keep_records else None
+        p = new_time_pool(name, description, marks, record_writer=record_writer)
         cls.pools[name] = p
         return p
 
     @classmethod
     def add_msg_size_pool(cls, name: str, description: str, marks=None, scope=None):
+        keep_records = cls._keep_hist_records(name)
         name = cls._check_name(name, scope)
-        p = new_message_size_pool(name, description, marks)
+        record_writer = cls.record_writer if keep_records else None
+        p = new_message_size_pool(name, description, marks, record_writer=record_writer)
         cls.pools[name] = p
         return p
 
     @classmethod
     def add_counter_pool(cls, name: str, description: str, counter_names: list, scope=None):
         name = cls._check_name(name, scope)
         p = CounterPool(name, description, counter_names)
@@ -113,7 +507,88 @@
             if t == "hist":
                 p = HistPool.from_dict(pd)
             elif t == "counter":
                 p = CounterPool.from_dict(pd)
             else:
                 raise ValueError(f"invalid pool type {t}")
             cls.pools[k] = p
+
+    @classmethod
+    def dump_summary(cls, file_name: str):
+        stats_dict = cls.to_dict()
+        json_string = json.dumps(stats_dict, indent=4)
+        with open(file_name, "w") as f:
+            f.write(json_string)
+
+    @classmethod
+    def close(cls):
+        if cls.record_writer:
+            cls.record_writer.close()
+
+
+class CsvRecordHandler(RecordWriter):
+    def __init__(self, file_name):
+        self.file = open(file_name, "w")
+        self.writer = csv.writer(self.file)
+        self.lock = threading.Lock()
+
+    def write(self, pool_name: str, category: str, value: float, report_time: float):
+        if not pool_name.isascii():
+            raise ValueError(f"pool_name {pool_name} contains non-ascii chars")
+        if not category.isascii():
+            raise ValueError(f"category {category} contains non-ascii chars")
+
+        row = [pool_name, category, report_time, value]
+        with self.lock:
+            self.writer.writerow(row)
+
+    def close(self):
+        self.file.close()
+
+    @staticmethod
+    def read_records(csv_file_name: str):
+        pools = {}
+        reader = CsvRecordReader(csv_file_name)
+        for rec in reader:
+            pool_name = rec.pool_name
+            cat_name = rec.category
+            report_time = rec.report_time
+            value = rec.value
+
+            cats = pools.get(pool_name)
+            if not cats:
+                cats = {}
+                pools[pool_name] = cats
+            recs = cats.get(cat_name)
+            if not recs:
+                recs = []
+                cats[cat_name] = recs
+            recs.append((report_time, value))
+        return pools
+
+
+class StatsRecord:
+    def __init__(self, pool_name, category, report_time, value):
+        self.pool_name = pool_name
+        self.category = category
+        self.report_time = report_time
+        self.value = value
+
+
+class CsvRecordReader:
+    def __init__(self, csv_file_name: str):
+        self.csv_file_name = csv_file_name
+        self.file = open(csv_file_name)
+        self.reader = csv.reader(self.file)
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        row = next(self.reader)
+        if len(row) != 4:
+            raise ValueError(f"'{self.csv_file_name}' is not a valid stats pool record file: bad row length {len(row)}")
+        pool_name = row[0]
+        cat_name = row[1]
+        report_time = float(row[2])
+        value = float(row[3])
+        return StatsRecord(pool_name, cat_name, report_time, value)
```

## nvflare/fuel/f3/cellnet/cell.py

```diff
@@ -33,15 +33,16 @@
     MessagePropKey,
     MessageType,
     ReturnCode,
     ReturnReason,
     ServiceUnavailable,
 )
 from nvflare.fuel.f3.cellnet.fqcn import FQCN, FqcnInfo, same_family
-from nvflare.fuel.f3.cellnet.utils import decode_payload, encode_payload, format_log_message, make_reply, new_message
+from nvflare.fuel.f3.cellnet.registry import Callback, Registry
+from nvflare.fuel.f3.cellnet.utils import decode_payload, encode_payload, format_log_message, make_reply
 from nvflare.fuel.f3.comm_config import CommConfigurator
 from nvflare.fuel.f3.communicator import Communicator, MessageReceiver
 from nvflare.fuel.f3.connection import Connection
 from nvflare.fuel.f3.drivers.driver_params import DriverParams
 from nvflare.fuel.f3.endpoint import Endpoint, EndpointMonitor, EndpointState
 from nvflare.fuel.f3.message import Message
 from nvflare.fuel.f3.mpm import MainProcessMonitor
@@ -82,15 +83,15 @@
             "topic": self.topic,
             "message": {"headers": dict(self.message.headers), "payload": self.message.payload},
         }
 
     @staticmethod
     def from_dict(d: dict):
         msg_dict = d.get("message")
-        msg = new_message(headers=msg_dict.get("headers"), payload=msg_dict.get("payload"))
+        msg = Message(headers=msg_dict.get("headers"), payload=msg_dict.get("payload"))
         return TargetMessage(target=d.get("target"), channel=d.get("channel"), topic=d.get("topic"), message=msg)
 
 
 class CellAgent:
     """A CellAgent represents a cell in another cell."""
 
     def __init__(self, fqcn: str, endpoint: Endpoint):
@@ -106,54 +107,14 @@
         self.info = FqcnInfo(FQCN.normalize(fqcn))
         self.endpoint = endpoint
 
     def get_fqcn(self):
         return self.info.fqcn
 
 
-class _CB:
-    def __init__(self, cb, args, kwargs):
-        self.cb = cb
-        self.args = args
-        self.kwargs = kwargs
-
-
-class _Registry:
-    def __init__(self):
-        self.reg = {}  # channel/topic => _CB
-
-    @staticmethod
-    def _item_key(channel: str, topic: str) -> str:
-        return f"{channel}:{topic}"
-
-    def set(self, channel: str, topic: str, items):
-        key = self._item_key(channel, topic)
-        self.reg[key] = items
-
-    def append(self, channel: str, topic: str, items):
-        key = self._item_key(channel, topic)
-        item_list = self.reg.get(key)
-        if not item_list:
-            item_list = []
-            self.reg[key] = item_list
-        item_list.append(items)
-
-    def find(self, channel: str, topic: str):
-        items = self.reg.get(self._item_key(channel, topic))
-        if not items:
-            # try topic * in channel
-            items = self.reg.get(self._item_key(channel, "*"))
-
-        if not items:
-            # try topic * in channel *
-            items = self.reg.get(self._item_key("*", "*"))
-
-        return items
-
-
 class _Waiter(threading.Event):
     def __init__(self, targets: List[str]):
         super().__init__()
         self.targets = [x for x in targets]
         self.reply_time = {}  # target_id => reply recv timestamp
         self.send_time = time.time()
         self.id = str(uuid.uuid4())
@@ -211,15 +172,15 @@
                 messages_to_send = self.messages[: self.max_queue_size]
                 self.messages = self.messages[self.max_queue_size :]
 
         self.logger.debug(
             f"{self.cell.get_fqcn()}: bulk sender {self.target} sending bulk size {len(messages_to_send)}"
         )
         tms = [m.to_dict() for m in messages_to_send]
-        bulk_msg = new_message(payload=tms)
+        bulk_msg = Message(None, tms)
         send_errs = self.cell.fire_and_forget(
             channel=_CHANNEL, topic=_TOPIC_BULK, targets=[self.target], message=bulk_msg
         )
         if send_errs[self.target]:
             log_messaging_error(
                 logger=self.logger,
                 msg=bulk_msg,
@@ -376,20 +337,20 @@
         self.endpoint = ep
         self.connector_manager = ConnectorManager(
             communicator=self.communicator, secure=secure, comm_configurator=comm_configurator
         )
 
         self.communicator.register_message_receiver(app_id=self.APP_ID, receiver=self)
         self.communicator.register_monitor(monitor=self)
-        self.req_reg = _Registry()
-        self.in_req_filter_reg = _Registry()  # for request received
-        self.out_reply_filter_reg = _Registry()  # for reply going out
-        self.out_req_filter_reg = _Registry()  # for request sent
-        self.in_reply_filter_reg = _Registry()  # for reply received
-        self.error_handler_reg = _Registry()
+        self.req_reg = Registry()
+        self.in_req_filter_reg = Registry()  # for request received
+        self.out_reply_filter_reg = Registry()  # for reply going out
+        self.out_req_filter_reg = Registry()  # for request sent
+        self.in_reply_filter_reg = Registry()  # for reply received
+        self.error_handler_reg = Registry()
         self.cell_connected_cb = None
         self.cell_connected_cb_args = None
         self.cell_connected_cb_kwargs = None
         self.cell_disconnected_cb = None
         self.cell_disconnected_cb_args = None
         self.cell_disconnected_cb_kwargs = None
         self.message_interceptor = None
@@ -862,15 +823,15 @@
             if self.agents:
                 targets = [peer_name for peer_name in self.agents.keys()]
                 self.logger.debug(f"broadcasting goodbye to {targets}")
                 self.broadcast_request(
                     channel=_CHANNEL,
                     topic=_TOPIC_BYE,
                     targets=targets,
-                    request=new_message(),
+                    request=Message(),
                     timeout=0.5,
                     optional=True,
                 )
 
         self.running = False
         self.asked_to_stop = True
         if self.bulk_checker is not None and self.bulk_checker.is_alive():
@@ -901,47 +862,47 @@
             **kwargs:
 
         Returns:
 
         """
         if not callable(cb):
             raise ValueError(f"specified request_cb {type(cb)} is not callable")
-        self.req_reg.set(channel, topic, _CB(cb, args, kwargs))
+        self.req_reg.set(channel, topic, Callback(cb, args, kwargs))
 
     def add_incoming_request_filter(self, channel: str, topic: str, cb, *args, **kwargs):
         if not callable(cb):
             raise ValueError(f"specified incoming_request_filter {type(cb)} is not callable")
-        self.in_req_filter_reg.append(channel, topic, _CB(cb, args, kwargs))
+        self.in_req_filter_reg.append(channel, topic, Callback(cb, args, kwargs))
 
     def add_outgoing_reply_filter(self, channel: str, topic: str, cb, *args, **kwargs):
         if not callable(cb):
             raise ValueError(f"specified outgoing_reply_filter {type(cb)} is not callable")
-        self.out_reply_filter_reg.append(channel, topic, _CB(cb, args, kwargs))
+        self.out_reply_filter_reg.append(channel, topic, Callback(cb, args, kwargs))
 
     def add_outgoing_request_filter(self, channel: str, topic: str, cb, *args, **kwargs):
         if not callable(cb):
             raise ValueError(f"specified outgoing_request_filter {type(cb)} is not callable")
-        self.out_req_filter_reg.append(channel, topic, _CB(cb, args, kwargs))
+        self.out_req_filter_reg.append(channel, topic, Callback(cb, args, kwargs))
 
     def add_incoming_reply_filter(self, channel: str, topic: str, cb, *args, **kwargs):
         if not callable(cb):
             raise ValueError(f"specified incoming_reply_filter {type(cb)} is not callable")
-        self.in_reply_filter_reg.append(channel, topic, _CB(cb, args, kwargs))
+        self.in_reply_filter_reg.append(channel, topic, Callback(cb, args, kwargs))
 
     def add_error_handler(self, channel: str, topic: str, cb, *args, **kwargs):
         if not callable(cb):
             raise ValueError(f"specified error_handler {type(cb)} is not callable")
-        self.error_handler_reg.set(channel, topic, _CB(cb, args, kwargs))
+        self.error_handler_reg.set(channel, topic, Callback(cb, args, kwargs))
 
     def _filter_outgoing_request(self, channel: str, topic: str, request: Message) -> Union[None, Message]:
         cbs = self.out_req_filter_reg.find(channel, topic)
         if not cbs:
             return None
         for _cb in cbs:
-            assert isinstance(_cb, _CB)
+            assert isinstance(_cb, Callback)
             reply = self._try_cb(request, _cb.cb, *_cb.args, **_cb.kwargs)
             if reply:
                 return reply
 
     def _try_path(self, fqcn_path: List[str]) -> Union[None, Endpoint]:
         self.logger.debug(f"{self.my_info.fqcn}: trying path {fqcn_path} ...")
         target = FQCN.join(fqcn_path)
@@ -1108,15 +1069,15 @@
 
             # invoke outgoing req filters
             req_filters = self.out_req_filter_reg.find(tm.channel, tm.topic)
             if req_filters:
                 self.logger.debug(f"{self.my_info.fqcn}: invoking outgoing request filters")
                 assert isinstance(req_filters, list)
                 for f in req_filters:
-                    assert isinstance(f, _CB)
+                    assert isinstance(f, Callback)
                     r = self._try_cb(req, f.cb, *f.args, **f.kwargs)
                     if r:
                         send_errs[t] = ReturnCode.FILTER_ERROR
                         break
                 if send_errs.get(t):
                     # process next target
                     continue
@@ -1339,15 +1300,15 @@
             ep = self.agents.pop(peer_ep.name, None)
             if ep:
                 self.logger.debug(f"{self.my_info.fqcn}: removed agent for {peer_ep.name}")
             else:
                 self.logger.debug(f"{self.my_info.fqcn}: agent for {peer_ep.name} is already gone")
 
         # ack back
-        return new_message()
+        return Message()
 
     def _receive_bulk_message(self, request: Message):
         target_msgs = request.payload
         assert isinstance(target_msgs, list)
         with self.bulk_msg_lock:
             if self.bulk_processor is None:
                 self.logger.debug(f"{self.my_info.fqcn}: starting bulk message processor")
@@ -1473,28 +1434,27 @@
 
         # invoke incoming request filters
         req_filters = self.in_req_filter_reg.find(channel, topic)
         if req_filters:
             self.logger.debug(f"{self.my_info.fqcn}: invoking incoming request filters")
             assert isinstance(req_filters, list)
             for f in req_filters:
-                assert isinstance(f, _CB)
+                assert isinstance(f, Callback)
                 reply = self._try_cb(message, f.cb, *f.args, **f.kwargs)
                 if reply:
                     return reply
 
-        assert isinstance(_cb, _CB)
+        assert isinstance(_cb, Callback)
         self.logger.debug(f"{self.my_info.fqcn}: calling registered request CB")
         cb_start = time.perf_counter()
         reply = self._try_cb(message, _cb.cb, *_cb.args, **_cb.kwargs)
         cb_end = time.perf_counter()
         self.req_cb_stats_pool.record_value(category=self._stats_category(message), value=cb_end - cb_start)
         if not reply:
             # the CB doesn't have anything to reply
-            self.logger.debug("no reply is returned from the CB")
             return None
 
         if not isinstance(reply, Message):
             self.log_error(
                 f"bad result from request CB for topic {topic} on channel {channel}: "
                 f"expect Message but got {type(reply)}",
                 msg=message,
@@ -1626,15 +1586,15 @@
         else:
             # invoking incoming reply filter
             reply_filters = self.in_reply_filter_reg.find(channel, topic)
             if reply_filters:
                 self.logger.debug(f"{self.my_info.fqcn}: invoking incoming reply filters")
                 assert isinstance(reply_filters, list)
                 for f in reply_filters:
-                    assert isinstance(f, _CB)
+                    assert isinstance(f, Callback)
                     self._try_cb(message, f.cb, *f.args, **f.kwargs)
 
         for rid in req_ids:
             waiter = self.waiters.get(rid, None)
             if waiter:
                 assert isinstance(waiter, _Waiter)
                 if req_destination not in waiter.targets:
@@ -1787,28 +1747,31 @@
                     # the origin already has a listener
                     # create an ad-hoc connector to connect to the origin cell
                     self.logger.debug(f"{self.my_info.fqcn}: creating adhoc connector to {origin} at {conn_url}")
                     self._add_adhoc_connector(origin, conn_url)
                 elif msg_type == MessageType.REQ:
                     # see whether we can offer a listener
                     allow_adhoc = self.connector_manager.is_adhoc_allowed(oi, self.my_info)
-                    if allow_adhoc and not oi.is_on_server and self.my_info.fqcn > origin:
+                    if (
+                        allow_adhoc
+                        and (not oi.is_on_server)
+                        and (self.my_info.fqcn > origin or self.my_info.is_on_server)
+                    ):
                         self.logger.debug(f"{self.my_info.fqcn}: trying to offer ad-hoc listener to {origin}")
                         listener = self._create_external_listener("")
                         if listener:
                             my_conn_url = listener.get_connection_url()
 
         if msg_type == MessageType.REQ:
             # this is a request for me - dispatch to the right CB
             channel = message.get_header(MessageHeaderKey.CHANNEL, "")
             topic = message.get_header(MessageHeaderKey.TOPIC, "")
             reply = self._process_request(origin, message)
 
             if not reply:
-                self.logger.debug(f"{self.my_info.fqcn}: don't send response - nothing to send")
                 self.received_msg_counter_pool.increment(
                     category=self._stats_category(message), counter_name=_CounterName.REPLY_NONE
                 )
                 return
 
             is_optional = message.get_header(MessageHeaderKey.OPTIONAL, False)
             reply.set_header(MessageHeaderKey.OPTIONAL, is_optional)
@@ -1855,15 +1818,15 @@
 
             # invoke outgoing reply filters
             reply_filters = self.out_reply_filter_reg.find(channel, topic)
             if reply_filters:
                 self.logger.debug(f"{self.my_info.fqcn}: invoking outgoing reply filters")
                 assert isinstance(reply_filters, list)
                 for f in reply_filters:
-                    assert isinstance(f, _CB)
+                    assert isinstance(f, Callback)
                     r = self._try_cb(reply, f.cb, *f.args, **f.kwargs)
                     if r:
                         reply = r
                         break
             self._send_reply(reply, endpoint)
         else:
             # the message is either a reply or a return for a previous request: handle replies
```

## nvflare/fuel/f3/cellnet/net_agent.py

```diff
@@ -23,15 +23,15 @@
 from abc import ABC
 from typing import List, Union
 
 from nvflare.fuel.f3.cellnet.cell import Cell, Message
 from nvflare.fuel.f3.cellnet.connector_manager import ConnectorData
 from nvflare.fuel.f3.cellnet.defs import MessageHeaderKey, ReturnCode
 from nvflare.fuel.f3.cellnet.fqcn import FQCN
-from nvflare.fuel.f3.cellnet.utils import make_reply, new_message
+from nvflare.fuel.f3.cellnet.utils import make_reply
 from nvflare.fuel.f3.stats_pool import StatsPoolManager
 from nvflare.fuel.utils.config_service import ConfigService
 
 _CHANNEL = "_net_manager"
 _TOPIC_PEERS = "peers"
 _TOPIC_CELLS = "cells"
 _TOPIC_ROUTE = "route"
@@ -273,15 +273,15 @@
     def stop_subnet(self, monitor: SubnetMonitor):
         cells_to_stop = []
         for member_fqcn, member in monitor.members.items():
             if member.state == member.STATE_ONLINE:
                 cells_to_stop.append(member_fqcn)
         if cells_to_stop:
             return self.cell.broadcast_request(
-                channel=_CHANNEL, topic=_TOPIC_STOP_CELL, request=new_message(), targets=cells_to_stop, timeout=1.0
+                channel=_CHANNEL, topic=_TOPIC_STOP_CELL, request=Message(), targets=cells_to_stop, timeout=1.0
             )
         else:
             return None
 
     def delete_subnet_monitor(self, subnet_id: str):
         with self.monitor_lock:
             self.monitors.pop(subnet_id, None)
@@ -306,15 +306,15 @@
         while True:
             with self.hb_lock:
                 for subnet_id, target in self.subnets.items():
                     self.cell.fire_and_forget(
                         channel=_CHANNEL,
                         topic=_TOPIC_HEARTBEAT,
                         targets=target,
-                        message=new_message(payload={"subnet_id": subnet_id}),
+                        message=Message(payload={"subnet_id": subnet_id}),
                     )
 
             # wait for interval time, but watch for "asked_to_stop" every 0.1 secs
             start = time.time()
             while True:
                 time.sleep(0.1)
                 if self.asked_to_close:
@@ -359,34 +359,34 @@
 
     def _do_stop(self, request: Message) -> Union[None, Message]:
         self.stop()
         return None
 
     def _do_stop_cell(self, request: Message) -> Union[None, Message]:
         self.stop()
-        return new_message()
+        return Message()
 
     def _do_route(self, request: Message) -> Union[None, Message]:
-        return new_message(payload=dict(request.headers))
+        return Message(payload=dict(request.headers))
 
     def _do_start_route(self, request: Message) -> Union[None, Message]:
         target_fqcn = request.payload
         err = FQCN.validate(target_fqcn)
         if err:
             return make_reply(ReturnCode.PROCESS_EXCEPTION, f"bad target fqcn {err}")
         assert isinstance(target_fqcn, str)
         reply_headers, req_headers = self.get_route_info(target_fqcn)
-        return new_message(payload={"request": dict(req_headers), "reply": dict(reply_headers)})
+        return Message(payload={"request": dict(req_headers), "reply": dict(reply_headers)})
 
     def _do_peers(self, request: Message) -> Union[None, Message]:
-        return new_message(payload=list(self.cell.agents.keys()))
+        return Message(payload=list(self.cell.agents.keys()))
 
     def get_peers(self, target_fqcn: str) -> (Union[None, dict], List[str]):
         reply = self.cell.send_request(
-            channel=_CHANNEL, topic=_TOPIC_PEERS, target=target_fqcn, timeout=1.0, request=new_message()
+            channel=_CHANNEL, topic=_TOPIC_PEERS, target=target_fqcn, timeout=1.0, request=Message()
         )
 
         err = ""
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE)
         if rc == ReturnCode.OK:
             result = reply.payload
             if not isinstance(result, list):
@@ -421,19 +421,19 @@
             conns = {}
             for k, v in cell.adhoc_connectors.items():
                 conns[k] = self._connector_info(v)
             result["adhoc_connectors"] = conns
         return result
 
     def _do_connectors(self, request: Message) -> Union[None, Message]:
-        return new_message(payload=self._get_connectors())
+        return Message(payload=self._get_connectors())
 
     def get_connectors(self, target_fqcn: str) -> (dict, dict):
         reply = self.cell.send_request(
-            channel=_CHANNEL, topic=_TOPIC_CONNS, target=target_fqcn, timeout=1.0, request=new_message()
+            channel=_CHANNEL, topic=_TOPIC_CONNS, target=target_fqcn, timeout=1.0, request=Message()
         )
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE)
         if rc == ReturnCode.OK:
             result = reply.payload
             if not isinstance(result, dict):
                 return {
                     "error": f"reply payload should be dict but got {type(reply.payload)}",
@@ -477,34 +477,34 @@
             for _, h in cell.adhoc_connectors.items():
                 if h.connect_url == url:
                     return "adhoc_connect"
         return "none"
 
     def get_url_use(self, url) -> dict:
         result = {self.cell.get_fqcn(): self._get_url_use_of_cell(url)}
-        replies = self._broadcast_to_subs(topic=_TOPIC_URL_USE, message=new_message(payload=url))
+        replies = self._broadcast_to_subs(topic=_TOPIC_URL_USE, message=Message(payload=url))
         for t, r in replies.items():
             assert isinstance(r, Message)
             rc = r.get_header(MessageHeaderKey.RETURN_CODE)
             if rc == ReturnCode.OK:
                 if not isinstance(r.payload, dict):
                     result[t] = f"bad reply type {type(r.payload)}"
                 else:
                     result.update(r.payload)
             else:
                 result[t] = f"error {rc}"
         return result
 
     def _do_url_use(self, request: Message) -> Union[None, Message]:
         results = self.get_url_use(request.payload)
-        return new_message(payload=results)
+        return Message(payload=results)
 
     def get_route_info(self, target_fqcn: str) -> (dict, dict):
         reply = self.cell.send_request(
-            channel=_CHANNEL, topic=_TOPIC_ROUTE, target=target_fqcn, timeout=1.0, request=new_message()
+            channel=_CHANNEL, topic=_TOPIC_ROUTE, target=target_fqcn, timeout=1.0, request=Message()
         )
         reply_headers = reply.headers
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE, ReturnCode.OK)
         if rc == ReturnCode.OK:
             if not isinstance(reply.payload, dict):
                 return reply_headers, {"error": f"reply payload got {type(reply.payload)}"}
             return reply_headers, reply.payload
@@ -516,15 +516,15 @@
         reply_headers = {}
         req_headers = {}
         reply = self.cell.send_request(
             channel=_CHANNEL,
             topic=_TOPIC_START_ROUTE,
             target=from_fqcn,
             timeout=1.0,
-            request=new_message(payload=target_fqcn),
+            request=Message(payload=target_fqcn),
         )
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE)
         if rc == ReturnCode.OK:
             result = reply.payload
             if not isinstance(result, dict):
                 err = f"reply payload should be dict but got {type(reply.payload)}"
             else:
@@ -533,27 +533,27 @@
         else:
             err = f"error in reply {rc}"
             reply_headers = reply.headers
         return err, reply_headers, req_headers
 
     def _do_report_cells(self, request: Message) -> Union[None, Message]:
         _, results = self.request_cells_info()
-        return new_message(payload=results)
+        return Message(payload=results)
 
     def stop(self):
         # ask all children to stop
         self._broadcast_to_subs(topic=_TOPIC_STOP, timeout=0.0)
         self.close()
 
     def stop_cell(self, target: str) -> str:
         # if self.cell.get_fqcn() == target:
         #     self.stop()
         #     return ReturnCode.OK
         reply = self.cell.send_request(
-            channel=_CHANNEL, topic=_TOPIC_STOP_CELL, request=new_message(), target=target, timeout=1.0
+            channel=_CHANNEL, topic=_TOPIC_STOP_CELL, request=Message(), target=target, timeout=1.0
         )
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE)
         return rc
 
     def _request_speed_test(self, target_fqcn: str, num, size) -> Message:
         start = time.perf_counter()
         payload = bytes(_ONE_K * size)
@@ -569,15 +569,15 @@
         size_errs = 0
         start = time.perf_counter()
         for i in range(num):
             r = self.cell.send_request(
                 channel=_CHANNEL,
                 topic=_TOPIC_ECHO,
                 target=target_fqcn,
-                request=new_message(payload=payload),
+                request=Message(payload=payload),
                 timeout=10.0,
             )
             rc = r.get_header(MessageHeaderKey.RETURN_CODE, ReturnCode.OK)
             if rc == ReturnCode.OK:
                 if len(r.payload) != payload_size:
                     self.cell.logger.error(
                         f"{self.cell.get_fqcn()}: expect {payload_size} bytes but received {len(r.payload)}"
@@ -596,15 +596,15 @@
             elif rc == ReturnCode.MSG_TOO_BIG:
                 size_errs += 1
             else:
                 errs += 1
         end = time.perf_counter()
         total = end - start
         avg = total / num
-        return new_message(
+        return Message(
             payload={
                 "test": f"{size:,}KB {num} rounds between {self.cell.get_fqcn()} and {target_fqcn}",
                 "prep": payload_prep_time,
                 "timeouts": timeouts,
                 "comm_errors": comm_errs,
                 "size_errors": size_errs,
                 "proc_errors": proc_errs,
@@ -629,15 +629,15 @@
         if size <= 0:
             size = 1000
         if num <= 0:
             num = 100
         return self._request_speed_test(to_fqcn, num, size)
 
     def _do_echo(self, request: Message) -> Union[None, Message]:
-        return new_message(payload=request.payload)
+        return Message(payload=request.payload)
 
     def _do_stress_test(self, params):
         if not isinstance(params, dict):
             return {"error": f"bad params - expect dict but got {type(params)}"}
         targets = params.get("targets")
         if not targets:
             return {"error": "no targets specified"}
@@ -656,15 +656,15 @@
 
         start = time.perf_counter()
         for i in range(num_rounds):
             payload = os.urandom(1024)
             h = hashlib.md5(payload)
             d1 = h.digest()
             target = targets[random.randrange(len(targets))]
-            req = new_message(payload=payload)
+            req = Message(payload=payload)
             reply = self.cell.send_request(channel=_CHANNEL, topic=_TOPIC_ECHO, target=target, request=req, timeout=1.0)
             if target not in counts:
                 counts[target] = 0
             counts[target] += 1
             rc = reply.get_header(MessageHeaderKey.RETURN_CODE, ReturnCode.OK)
             if rc != ReturnCode.OK:
                 self.cell.logger.error(f"{self.cell.get_fqcn()}: return code from {target}: {rc}")
@@ -681,15 +681,15 @@
                     errors[target] += 1
         end = time.perf_counter()
         return {"counts": counts, "errors": errors, "time": end - start}
 
     def _do_stress(self, request: Message) -> Union[None, Message]:
         params = request.payload
         result = self._do_stress_test(params)
-        return new_message(payload=result)
+        return Message(payload=result)
 
     def start_stress_test(self, targets: list, num_rounds=10, timeout=5.0):
         self.cell.logger.info(f"{self.cell.get_fqcn()}: starting stress test on {targets}")
         result = {}
         payload = {"targets": targets, "num": num_rounds}
         msg_targets = [x for x in targets]
         my_fqcn = self.cell.get_fqcn()
@@ -698,15 +698,15 @@
         if not msg_targets:
             return {"error": "no targets for stress test"}
 
         replies = self.cell.broadcast_request(
             channel=_CHANNEL,
             topic=_TOPIC_STRESS,
             targets=msg_targets,
-            request=new_message(payload=payload),
+            request=Message(payload=payload),
             timeout=timeout,
         )
         for t, r in replies.items():
             rc = r.get_header(MessageHeaderKey.RETURN_CODE, ReturnCode.OK)
             if rc != ReturnCode.OK:
                 result[t] = f"RC={rc}"
             else:
@@ -724,15 +724,15 @@
 
         result = {}
 
         start = time.perf_counter()
         reply = self.cell.send_request(
             channel=_CHANNEL,
             topic=_TOPIC_SPEED,
-            request=new_message(payload={"to": to_fqcn, "num": num_tries, "size": payload_size}),
+            request=Message(payload={"to": to_fqcn, "num": num_tries, "size": payload_size}),
             target=from_fqcn,
             timeout=100.0,
         )
         end = time.perf_counter()
         result["test_time"] = end - start
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE, ReturnCode.OK)
         if rc != ReturnCode.OK:
@@ -740,15 +740,15 @@
         elif not isinstance(reply.payload, dict):
             result.update({"error": f"bad reply: expect dict but got {type(reply.payload)}"})
         else:
             result.update(reply.payload)
         return result
 
     def change_root(self, new_root_url: str):
-        self._broadcast_to_subs(topic=_TOPIC_CHANGE_ROOT, message=new_message(payload=new_root_url), timeout=0.0)
+        self._broadcast_to_subs(topic=_TOPIC_CHANGE_ROOT, message=Message(payload=new_root_url), timeout=0.0)
 
     def _do_change_root(self, request: Message) -> Union[None, Message]:
         new_root_url = request.payload
         assert isinstance(new_root_url, str)
         self.change_root(new_root_url)
         if self.change_root_cb is not None:
             self.change_root_cb(new_root_url)
@@ -764,15 +764,15 @@
             return {"error": "no targets for bulk test"}
 
         result = {}
         replies = self.cell.broadcast_request(
             channel=_CHANNEL,
             topic=_TOPIC_BULK_TEST,
             targets=msg_targets,
-            request=new_message(payload=size),
+            request=Message(payload=size),
             timeout=1.0,
         )
         for t, r in replies.items():
             rc = r.get_header(MessageHeaderKey.RETURN_CODE, ReturnCode.OK)
             if rc != ReturnCode.OK:
                 result[t] = f"RC={rc}"
             else:
@@ -782,70 +782,70 @@
     def _do_bulk_test(self, request: Message) -> Union[None, Message]:
         size = request.payload
         assert isinstance(size, int)
         nums = []
         for _ in range(size):
             num = random.randint(0, 100)
             nums.append(num)
-            msg = new_message(payload=num)
+            msg = Message(payload=num)
             self.cell.queue_message(
                 channel=_CHANNEL,
                 topic=_TOPIC_BULK_ITEM,
                 targets=FQCN.ROOT_SERVER,
                 message=msg,
             )
-        return new_message(payload=f"queued: {nums}")
+        return Message(payload=f"queued: {nums}")
 
     def _do_bulk_item(self, request: Message) -> Union[None, Message]:
         num = request.payload
         origin = request.get_header(MessageHeaderKey.ORIGIN)
         self.cell.logger.info(f"{self.cell.get_fqcn()}: got {num} from {origin}")
         return None
 
     def get_msg_stats_table(self, target: str, mode: str):
         reply = self.cell.send_request(
             channel=_CHANNEL,
             topic=_TOPIC_MSG_STATS,
-            request=new_message(payload={"mode": mode}),
+            request=Message(payload={"mode": mode}),
             timeout=1.0,
             target=target,
         )
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE)
         if rc != ReturnCode.OK:
             return f"error: {rc}"
         return reply.payload
 
     def _do_msg_stats(self, request: Message) -> Union[None, Message]:
         p = request.payload
         assert isinstance(p, dict)
         mode = p.get("mode")
         headers, rows = self.cell.msg_stats_pool.get_table(mode)
         reply = {"headers": headers, "rows": rows}
-        return new_message(payload=reply)
+        return Message(payload=reply)
 
     def get_pool_list(self, target: str):
         reply = self.cell.send_request(
-            channel=_CHANNEL, topic=_TOPIC_LIST_POOLS, request=new_message(), timeout=1.0, target=target
+            channel=_CHANNEL, topic=_TOPIC_LIST_POOLS, request=Message(), timeout=1.0, target=target
         )
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE)
         err = reply.get_header(MessageHeaderKey.ERROR, "")
         if rc != ReturnCode.OK:
             return f"{rc}: {err}"
         return reply.payload
 
     def _do_list_pools(self, request: Message) -> Union[None, Message]:
         headers, rows = StatsPoolManager.get_table()
         reply = {"headers": headers, "rows": rows}
-        return new_message(payload=reply)
+        return Message(payload=reply)
 
     def show_pool(self, target: str, pool_name: str, mode: str):
         reply = self.cell.send_request(
             channel=_CHANNEL,
             topic=_TOPIC_SHOW_POOL,
-            request=new_message(payload={"mode": mode, "pool": pool_name}),
+            request=Message(payload={"mode": mode, "pool": pool_name}),
             timeout=1.0,
             target=target,
         )
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE)
         if rc != ReturnCode.OK:
             err = reply.get_header(MessageHeaderKey.ERROR, "")
             return f"{rc}: {err}"
@@ -854,79 +854,79 @@
     def _do_show_pool(self, request: Message) -> Union[None, Message]:
         p = request.payload
         assert isinstance(p, dict)
         pool_name = p.get("pool", "")
         mode = p.get("mode", "")
         pool = StatsPoolManager.get_pool(pool_name)
         if not pool:
-            return new_message(
+            return Message(
                 headers={
                     MessageHeaderKey.RETURN_CODE: ReturnCode.INVALID_REQUEST,
                     MessageHeaderKey.ERROR: f"unknown pool '{pool_name}'",
                 }
             )
         headers, rows = pool.get_table(mode)
         reply = {"headers": headers, "rows": rows}
-        return new_message(payload=reply)
+        return Message(payload=reply)
 
     def get_comm_config(self, target: str):
         reply = self.cell.send_request(
-            channel=_CHANNEL, topic=_TOPIC_COMM_CONFIG, request=new_message(), timeout=1.0, target=target
+            channel=_CHANNEL, topic=_TOPIC_COMM_CONFIG, request=Message(), timeout=1.0, target=target
         )
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE)
         if rc != ReturnCode.OK:
             err = reply.get_header(MessageHeaderKey.ERROR, "")
             return f"{rc}: {err}"
         return reply.payload
 
     def get_config_vars(self, target: str):
         reply = self.cell.send_request(
-            channel=_CHANNEL, topic=_TOPIC_CONFIG_VARS, request=new_message(), timeout=1.0, target=target
+            channel=_CHANNEL, topic=_TOPIC_CONFIG_VARS, request=Message(), timeout=1.0, target=target
         )
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE)
         if rc != ReturnCode.OK:
             err = reply.get_header(MessageHeaderKey.ERROR, "")
             return f"{rc}: {err}"
         return reply.payload
 
     def get_process_info(self, target: str):
         reply = self.cell.send_request(
-            channel=_CHANNEL, topic=_TOPIC_PROCESS_INFO, request=new_message(), timeout=1.0, target=target
+            channel=_CHANNEL, topic=_TOPIC_PROCESS_INFO, request=Message(), timeout=1.0, target=target
         )
         rc = reply.get_header(MessageHeaderKey.RETURN_CODE)
         if rc != ReturnCode.OK:
             err = reply.get_header(MessageHeaderKey.ERROR, "")
             return f"{rc}: {err}"
         return reply.payload
 
     def _do_comm_config(self, request: Message) -> Union[None, Message]:
         info = self.cell.connector_manager.get_config_info()
-        return new_message(payload=info)
+        return Message(payload=info)
 
     def _do_config_vars(self, request: Message) -> Union[None, Message]:
         info = ConfigService.get_var_values()
-        return new_message(payload=info)
+        return Message(payload=info)
 
     def _do_process_info(self, request: Message) -> Union[None, Message]:
 
         usage = resource.getrusage(resource.RUSAGE_SELF).ru_maxrss
         rows = [
             ["Process ID", str(os.getpid())],
             ["Memory Usage", str(usage)],
             ["Thread Count", str(threading.active_count())],
         ]
 
         for thread in threading.enumerate():
             rows.append([f"Thread:{thread.ident}", thread.name])
 
-        return new_message(payload={"headers": ["Resource", "Value"], "rows": rows})
+        return Message(payload={"headers": ["Resource", "Value"], "rows": rows})
 
     def _broadcast_to_subs(self, topic: str, message=None, timeout=1.0):
         if not message:
-            message = new_message()
+            message = Message()
 
         children, clients = self.cell.get_sub_cell_names()
         targets = []
         targets.extend(children)
         targets.extend(clients)
 
         if targets:
```

## nvflare/fuel/f3/cellnet/net_manager.py

```diff
@@ -9,18 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from nvflare.fuel.f3.cellnet.fqcn import FQCN
 from nvflare.fuel.f3.cellnet.net_agent import NetAgent
+from nvflare.fuel.f3.stats_pool import VALID_HIST_MODES, parse_hist_mode
 from nvflare.fuel.hci.conn import Connection
 from nvflare.fuel.hci.reg import CommandModule, CommandModuleSpec, CommandSpec
 from nvflare.fuel.hci.server.constants import ConnProps
-from nvflare.fuel.utils.stats_utils import VALID_HIST_MODES, parse_hist_mode
 from nvflare.security.logging import secure_format_exception
 
 
 def _to_int(s: str):
     try:
         return int(s)
     except Exception as ex:
```

## nvflare/fuel/f3/cellnet/utils.py

```diff
@@ -9,32 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import nvflare.fuel.utils.fobs as fobs
 from nvflare.fuel.f3.cellnet.defs import Encoding, MessageHeaderKey
-from nvflare.fuel.f3.message import Headers, Message
+from nvflare.fuel.f3.message import Message
 
 
 def make_reply(rc: str, error: str = "", body=None) -> Message:
-    headers = Headers()
-    headers[MessageHeaderKey.RETURN_CODE] = rc
+    headers = {MessageHeaderKey.RETURN_CODE: rc}
     if error:
         headers[MessageHeaderKey.ERROR] = error
     return Message(headers, payload=body)
 
 
-def new_message(headers: dict = None, payload=None):
-    msg_headers = Headers()
-    if headers:
-        msg_headers.update(headers)
-    return Message(msg_headers, payload)
-
-
 def format_log_message(fqcn: str, message: Message, log: str) -> str:
     parts = [
         "[ME=" + fqcn,
         "O=" + message.get_header(MessageHeaderKey.ORIGIN, "?"),
         "D=" + message.get_header(MessageHeaderKey.DESTINATION, "?"),
         "F=" + message.get_header(MessageHeaderKey.FROM_CELL, "?"),
         "T=" + message.get_header(MessageHeaderKey.TO_CELL, "?"),
@@ -46,15 +38,15 @@
 
 
 def encode_payload(message: Message):
     encoding = message.get_header(MessageHeaderKey.PAYLOAD_ENCODING)
     if not encoding:
         if message.payload is None:
             encoding = Encoding.NONE
-        elif isinstance(message.payload, bytes) or isinstance(message.payload, bytearray):
+        elif isinstance(message.payload, (bytes, bytearray, memoryview)):
             encoding = Encoding.BYTES
         else:
             encoding = Encoding.FOBS
             message.payload = fobs.dumps(message.payload)
         message.set_header(MessageHeaderKey.PAYLOAD_ENCODING, encoding)
```

## nvflare/fuel/f3/drivers/connector_info.py

```diff
@@ -7,23 +7,19 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 from dataclasses import dataclass
-from enum import IntEnum
 
 from nvflare.fuel.f3.drivers.net_utils import short_url
-
-
-class Mode(IntEnum):
-    ACTIVE = 0
-    PASSIVE = 1
+from nvflare.fuel.utils.constants import Mode
 
 
 @dataclass
 class ConnectorInfo:
     """Connector information"""
 
     handle: str
```

## nvflare/fuel/f3/sfm/conn_manager.py

```diff
@@ -22,15 +22,15 @@
 from nvflare.fuel.f3.comm_error import CommError
 from nvflare.fuel.f3.connection import BytesAlike, Connection, ConnState, FrameReceiver
 from nvflare.fuel.f3.drivers.connector_info import ConnectorInfo, Mode
 from nvflare.fuel.f3.drivers.driver import ConnMonitor, Driver
 from nvflare.fuel.f3.drivers.driver_params import DriverCap, DriverParams
 from nvflare.fuel.f3.drivers.net_utils import ssl_required
 from nvflare.fuel.f3.endpoint import Endpoint, EndpointMonitor, EndpointState
-from nvflare.fuel.f3.message import Headers, Message, MessageReceiver
+from nvflare.fuel.f3.message import Message, MessageReceiver
 from nvflare.fuel.f3.sfm.constants import HandshakeKeys, Types
 from nvflare.fuel.f3.sfm.prefix import PREFIX_LEN, Prefix
 from nvflare.fuel.f3.sfm.sfm_conn import SfmConnection
 from nvflare.fuel.f3.sfm.sfm_endpoint import SfmEndpoint
 from nvflare.fuel.f3.stats_pool import StatsPoolManager
 from nvflare.security.logging import secure_format_exception, secure_format_traceback
 
@@ -173,15 +173,15 @@
         sfm_endpoint = self.sfm_endpoints.get(name)
         if not sfm_endpoint:
             log.debug("Endpoint {name} doesn't exist")
             return None
 
         return sfm_endpoint.connections
 
-    def send_message(self, endpoint: Endpoint, app_id: int, headers: Headers, payload: BytesAlike):
+    def send_message(self, endpoint: Endpoint, app_id: int, headers: Optional[dict], payload: BytesAlike):
         """Send a message to endpoint for app
 
         The message is asynchronous, no response is expected.
 
         Args:
             endpoint: An endpoint to send the message to
             app_id: Application ID
@@ -425,21 +425,21 @@
             sfm_endpoint.remove_connection(sfm_conn)
 
             state = EndpointState.READY if sfm_endpoint.connections else EndpointState.DISCONNECTED
             sfm_endpoint.endpoint.state = state
             if old_state != state:
                 self.notify_monitors(sfm_endpoint.endpoint)
 
-    def send_loopback_message(self, endpoint: Endpoint, app_id: int, headers: Headers, payload: BytesAlike):
+    def send_loopback_message(self, endpoint: Endpoint, app_id: int, headers: Optional[dict], payload: BytesAlike):
         """Send message to itself"""
 
         # Call receiver in a different thread to avoid deadlock
         self.frame_mgr_executor.submit(self.loopback_message_task, endpoint, app_id, headers, payload)
 
-    def loopback_message_task(self, endpoint: Endpoint, app_id: int, headers: Headers, payload: BytesAlike):
+    def loopback_message_task(self, endpoint: Endpoint, app_id: int, headers: Optional[dict], payload: BytesAlike):
 
         receiver = self.receivers.get(app_id)
         if not receiver:
             log.debug(f"No receiver registered for App ID {app_id}, loopback message ignored")
             return
 
         try:
```

## nvflare/fuel/f3/sfm/sfm_conn.py

```diff
@@ -17,15 +17,14 @@
 import time
 from typing import Optional
 
 import msgpack
 
 from nvflare.fuel.f3.connection import BytesAlike, Connection
 from nvflare.fuel.f3.endpoint import Endpoint
-from nvflare.fuel.f3.message import Headers
 from nvflare.fuel.f3.sfm.constants import HandshakeKeys, Types
 from nvflare.fuel.f3.sfm.prefix import PREFIX_LEN, Prefix
 
 log = logging.getLogger(__name__)
 
 
 class SfmConnection:
@@ -84,29 +83,29 @@
         data = {HandshakeKeys.ENDPOINT_NAME: self.local_endpoint.name, HandshakeKeys.TIMESTAMP: time.time()}
 
         if self.local_endpoint.properties:
             data.update(self.local_endpoint.properties)
 
         self.send_dict(frame_type, 1, data)
 
-    def send_data(self, app_id: int, stream_id: int, headers: Headers, payload: BytesAlike):
+    def send_data(self, app_id: int, stream_id: int, headers: Optional[dict], payload: BytesAlike):
         """Send user data"""
 
         prefix = Prefix(0, 0, Types.DATA, 0, 0, app_id, stream_id, 0)
         self.send_frame(prefix, headers, payload)
 
     def send_dict(self, frame_type: int, stream_id: int, data: dict):
         """Send a dict as payload"""
 
         prefix = Prefix(0, 0, frame_type, 0, 0, 0, stream_id, 0)
 
         payload = msgpack.packb(data)
         self.send_frame(prefix, None, payload)
 
-    def send_frame(self, prefix: Prefix, headers: Optional[Headers], payload: Optional[BytesAlike]):
+    def send_frame(self, prefix: Prefix, headers: Optional[dict], payload: Optional[BytesAlike]):
 
         headers_bytes = self.headers_to_bytes(headers)
         header_len = len(headers_bytes) if headers_bytes else 0
 
         length = PREFIX_LEN + header_len
 
         if payload:
```

## nvflare/fuel/flare_api/api_spec.py

```diff
@@ -11,60 +11,82 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import enum
 import time
 from abc import ABC, abstractmethod
-from typing import List
+from typing import List, Optional
 
 
 class MonitorReturnCode(int, enum.Enum):
 
     JOB_FINISHED = 0
     TIMEOUT = 1
     ENDED_BY_CB = 2
 
 
-class NoConnection(Exception):
+class NoConnection(BaseException):
     pass
 
 
-class SessionClosed(Exception):
+class SessionClosed(BaseException):
     pass
 
 
-class InvalidArgumentError(Exception):
+class InvalidArgumentError(BaseException):
     pass
 
 
-class InvalidJobDefinition(Exception):
+class InvalidJobDefinition(BaseException):
     pass
 
 
-class JobNotFound(Exception):
+class JobNotFound(BaseException):
     pass
 
 
-class JobNotDone(Exception):
+class JobNotRunning(BaseException):
     pass
 
 
-class InternalError(Exception):
+class JobNotDone(BaseException):
     pass
 
 
-class AuthenticationError(Exception):
+class InternalError(BaseException):
     pass
 
 
-class AuthorizationError(Exception):
+class AuthenticationError(BaseException):
     pass
 
 
+class AuthorizationError(BaseException):
+    pass
+
+
+class NoClientsAvailable(BaseException):
+    pass
+
+
+class ClientsStillRunning(BaseException):
+    pass
+
+
+class InvalidTarget(BaseException):
+    pass
+
+
+class TargetType:
+    ALL = "all"
+    SERVER = "server"
+    CLIENT = "client"
+
+
 class ServerInfo:
     def __init__(self, status, start_time):
         self.status = status
         self.start_time = start_time
 
     def __str__(self) -> str:
         return f"status: {self.status}, start_time: {time.asctime(time.localtime(self.start_time))}"
@@ -132,28 +154,28 @@
     @abstractmethod
     def get_job_meta(self, job_id: str) -> dict:
         """Get the meta info of the specified job
 
         Args:
             job_id: ID of the job
 
-        Returns: a dict of job meta data
+        Returns: a dict of job metadata
 
         """
         pass
 
     @abstractmethod
     def list_jobs(self, detailed: bool = False, all: bool = False) -> List[dict]:
         """Get the job info from the server
 
         Args:
             detailed: True to get the detailed information for each job, False by default
             all: True to get jobs submitted by all users (default is to only list jobs submitted by the same user)
 
-        Returns: a list of of job meta data
+        Returns: a list of job metadata
 
         """
         pass
 
     @abstractmethod
     def download_job_result(self, job_id: str) -> str:
         """
@@ -201,14 +223,295 @@
         the FL server and clients.
 
         """
         pass
 
     @abstractmethod
     def get_system_info(self) -> SystemInfo:
+        """Get general info of the FLARE system"""
+        pass
+
+    @abstractmethod
+    def get_client_job_status(self, client_names: List[str] = None) -> List[dict]:
+        """Get job status info of specified FL clients
+
+        Args:
+            client_names: names of the clients to get status info
+
+        Returns: A list of jobs running on the clients. Each job is described by a dict of: id, app name and status.
+        If there are multiple jobs running on one client, the list contains one entry for each job for that client.
+        If no FL clients are connected or the server failed to communicate to them, this method returns None.
+
+        """
+        pass
+
+    @abstractmethod
+    def restart(self, target_type: str, client_names: Optional[List[str]] = None) -> dict:
+        """
+        Restart specified system target(s)
+
+        Args:
+            target_type: what system target (server, client, or all) to restart
+            client_names: clients to be restarted if target_type is client. If not specified, all clients.
+
+        Returns: a dict that contains detailed info about the restart request:
+        status - the overall status of the result.
+        server_status - whether the server is restarted successfully - only if target_type is "all" or "server".
+        client_status - a dict (keyed on client name) that specifies status of each client - only if target_type
+        is "all" or "client".
+
+        """
+        pass
+
+    @abstractmethod
+    def shutdown(self, target_type: TargetType, client_names: Optional[List[str]] = None):
+        """Shut down specified system target(s)
+
+        Args:
+            target_type: what system target (server, client, or all) to shut down
+            client_names: clients to be shut down if target_type is client. If not specified, all clients.
+
+        Returns: None
+        """
+        pass
+
+    @abstractmethod
+    def set_timeout(self, value: float):
+        """
+        Set a session-specific command timeout. This is the amount of time the server will wait for responses
+        after sending commands to FL clients.
+
+        Note that this value is only effective for the current API session.
+
+        Args:
+            value: a positive float number
+
+        Returns: None
+
+        """
+        pass
+
+    @abstractmethod
+    def unset_timeout(self):
+        """
+        Unset the session-specific command timeout. Once unset, the FL Admin Server's default will be used.
+
+        Returns: None
+
+        """
+        pass
+
+    @abstractmethod
+    def list_sp(self) -> dict:
+        """List available service providers
+
+        Returns: a dict that contains information about the primary SP and others
+
+        """
+        pass
+
+    @abstractmethod
+    def get_active_sp(self) -> dict:
+        """Get the current active service provider (SP).
+
+        Returns: a dict that describes the current active SP. If no SP is available currently, the 'name' attribute of
+        the result is empty.
+        """
+        pass
+
+    @abstractmethod
+    def promote_sp(self, sp_end_point: str):
+        """Promote the specified endpoint to become the active SP.
+
+        Args:
+            sp_end_point: the endpoint of the SP. It's string in this format: <url>:<server_port>:<admin_port>
+
+        Returns: None
+
+        """
+        pass
+
+    @abstractmethod
+    def get_available_apps_to_upload(self):
+        """Get defined FLARE app folders from the upload folder on the machine the FLARE API is running
+
+        Returns: a list of app folders
+
+        """
+        pass
+
+    @abstractmethod
+    def shutdown_system(self):
+        """Shut down the whole NVFLARE system including the overseer, FL server(s), and all FL clients.
+
+        Returns: None
+
+        Note: the user must be a Project Admin to use this method; otherwise the NOT_AUTHORIZED exception will raise.
+
+        """
+        pass
+
+    @abstractmethod
+    def ls_target(self, target: str, options: str = None, path: str = None) -> str:
+        """Run the "ls" command on the specified target and return result
+
+        Args:
+            target: the target (server or a client name) the command will run
+            options: options of the "ls" command
+            path: the optional file path
+
+        Returns: result of "ls" command
+
+        """
+        pass
+
+    @abstractmethod
+    def cat_target(self, target: str, options: str = None, file: str = None) -> str:
+        """Run the "cat" command on the specified target and return result
+
+        Args:
+            target: the target (server or a client name) the command will run
+            options: options of the "cat" command
+            file: the file that the "cat" command will run against
+
+        Returns: result of "cat" command
+
+        """
+        pass
+
+    @abstractmethod
+    def tail_target(self, target: str, options: str = None, file: str = None) -> str:
+        """Run the "tail" command on the specified target and return result
+
+        Args:
+            target: the target (server or a client name) the command will run
+            options: options of the "tail" command
+            file: the file that the "tail" command will run against
+
+        Returns: result of "tail" command
+
+        """
+        pass
+
+    @abstractmethod
+    def tail_target_log(self, target: str, options: str = None) -> str:
+        """Run the "tail log.txt" command on the specified target and return result
+
+        Args:
+            target: the target (server or a client name) the command will run
+            options: options of the "tail" command
+
+        Returns: result of "tail" command
+
+        """
+        pass
+
+    @abstractmethod
+    def head_target(self, target: str, options: str = None, file: str = None) -> str:
+        """Run the "head" command on the specified target and return result
+
+        Args:
+            target: the target (server or a client name) the command will run
+            options: options of the "head" command
+            file: the file that the "head" command will run against
+
+        Returns: result of "head" command
+
+        """
+        pass
+
+    @abstractmethod
+    def head_target_log(self, target: str, options: str = None) -> str:
+        """Run the "head log.txt" command on the specified target and return result
+
+        Args:
+            target: the target (server or a client name) the command will run
+            options: options of the "head" command
+
+        Returns: result of "head" command
+
+        """
+        pass
+
+    @abstractmethod
+    def grep_target(self, target: str, options: str = None, pattern: str = None, file: str = None) -> str:
+        """Run the "grep" command on the specified target and return result
+
+        Args:
+            target: the target (server or a client name) the command will run
+            options: options of the "grep" command
+            pattern: the grep pattern
+            file: the file that the "grep" command will run against
+
+        Returns: result of "grep" command
+
+        """
+        pass
+
+    @abstractmethod
+    def get_working_directory(self, target: str) -> str:
+        """Get the working directory of the specified target
+
+        Args:
+            target: the target (server of a client name)
+
+        Returns: current working directory of the specified target
+
+        """
+        pass
+
+    @abstractmethod
+    def show_stats(self, job_id: str, target_type: str, targets: Optional[List[str]] = None) -> dict:
+        """Show processing stats of specified job on specified targets
+
+        Args:
+            job_id: ID of the job
+            target_type: type of target (server or client)
+            targets: list of client names if target type is "client". All clients if not specified.
+
+        Returns: a dict that contains job stats on specified targets. The key of the dict is target name. The value is
+        a dict of stats reported by different system components (ServerRunner or ClientRunner).
+
+        """
+        pass
+
+    @abstractmethod
+    def show_errors(self, job_id: str, target_type: str, targets: Optional[List[str]] = None) -> dict:
+        """Show processing errors of specified job on specified targets
+
+        Args:
+            job_id: ID of the job
+            target_type: type of target (server or client)
+            targets: list of client names if target type is "client". All clients if not specified.
+
+        Returns: a dict that contains job errors (if any) on specified targets. The key of the dict is target name.
+        The value is a dict of errors reported by different system components (ServerRunner or ClientRunner).
+
+        """
+        pass
+
+    @abstractmethod
+    def reset_errors(self, job_id: str):
+        """Clear errors for all system targets for the specified job
+
+        Args:
+            job_id: ID of the job
+
+        Returns: None
+
+        """
+        pass
+
+    @abstractmethod
+    def get_connected_client_list(self) -> List[ClientInfo]:
+        """Get the list of connected clients
+
+        Returns: a list of ClientInfo objects
+
+        """
         pass
 
     @abstractmethod
     def monitor_job(
         self, job_id: str, timeout: int = 0, poll_interval: float = 2.0, cb=None, *cb_args, **cb_kwargs
     ) -> MonitorReturnCode:
         """Monitor the job progress until one of the conditions occurs:
```

## nvflare/fuel/flare_api/flare_api.py

```diff
@@ -8,54 +8,70 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
 import os
 import time
 from typing import List, Optional
 
 from nvflare.apis.fl_constant import AdminCommandNames
 from nvflare.apis.job_def import JobMetaKey
 from nvflare.apis.workspace import Workspace
 from nvflare.fuel.common.excepts import ConfigError
 from nvflare.fuel.hci.client.api import AdminAPI, APIStatus, ResultKey
 from nvflare.fuel.hci.client.overseer_service_finder import ServiceFinderByOverseer
-from nvflare.fuel.hci.proto import MetaKey, MetaStatusValue
+from nvflare.fuel.hci.cmd_arg_utils import (
+    process_targets_into_str,
+    validate_file_string,
+    validate_options_string,
+    validate_path_string,
+    validate_required_target_string,
+    validate_sp_string,
+)
+from nvflare.fuel.hci.proto import MetaKey, MetaStatusValue, ProtoKey
 
 from .api_spec import (
     AuthenticationError,
     AuthorizationError,
     ClientInfo,
+    ClientsStillRunning,
     InternalError,
     InvalidArgumentError,
     InvalidJobDefinition,
+    InvalidTarget,
     JobInfo,
     JobNotDone,
     JobNotFound,
+    JobNotRunning,
     MonitorReturnCode,
+    NoClientsAvailable,
     NoConnection,
     ServerInfo,
     SessionClosed,
     SessionSpec,
     SystemInfo,
+    TargetType,
 )
 from .config import FLAdminClientStarterConfigurator
 
+_VALID_TARGET_TYPES = [TargetType.ALL, TargetType.SERVER, TargetType.CLIENT]
+
 
 class Session(SessionSpec):
     def __init__(self, username: str = None, startup_path: str = None, secure_mode: bool = True, debug: bool = False):
-        """Initializes a session with the NVFLARE system
+        """Initializes a session with the NVFLARE system.
 
         Args:
-            username: string of username to log in with
-            startup_path: path to the provisioned startup kit, which contains endpoint of the system
-            secure_mode: whether to run in secure mode or not
+            username (str): string of username to log in with
+            startup_path (str): path to the provisioned startup kit, which contains endpoint of the system
+            secure_mode (bool): whether to run in secure mode or not
         """
         assert isinstance(username, str), "username must be str"
         self.username = username
         assert isinstance(startup_path, str), "startup_path must be str"
         self.secure_mode = secure_mode
 
         assert os.path.isdir(startup_path), f"startup kit does not exist at {startup_path}"
@@ -97,84 +113,89 @@
 
             if not os.path.isfile(client_cert):
                 raise ConfigError(f"client.crt does not exist at {client_cert}")
 
             if not os.path.isfile(client_key):
                 raise ConfigError(f"client.key does not exist at {client_key}")
 
-        # Connect with admin client
-        if conf.overseer_agent:
-            service_finder = ServiceFinderByOverseer(conf.overseer_agent)
-        else:
-            service_finder = None
+        service_finder = ServiceFinderByOverseer(conf.overseer_agent)
 
         self.api = AdminAPI(
             ca_cert=ca_cert,
             client_cert=client_cert,
             client_key=client_key,
             upload_dir=upload_dir,
             download_dir=download_dir,
             service_finder=service_finder,
             user_name=username,
             poc=(not self.secure_mode),
             debug=debug,
         )
         self.upload_dir = upload_dir
         self.download_dir = download_dir
+        self.overseer_agent = conf.overseer_agent
 
     def close(self):
-        """Close the session
-
-        Returns:
-
-        """
+        """Close the session."""
         self.api.close()
 
     def try_connect(self, timeout):
         if self.api.closed:
             raise SessionClosed("session closed")
 
         start_time = time.time()
         while not self.api.is_ready():
             if time.time() - start_time > timeout:
                 self.api.close()
                 raise NoConnection(f"cannot connect to FLARE in {timeout} seconds")
             time.sleep(0.5)
 
-    def _do_command(self, command: str):
+    def _do_command(self, command: str, enforce_meta=True):
         if self.api.closed:
             raise SessionClosed("session closed")
 
         result = self.api.do_command(command)
-
         if not isinstance(result, dict):
             raise InternalError(f"result from server must be dict but got {type(result)}")
 
         # check meta status first
         meta = result.get(ResultKey.META, None)
-        if not meta:
+        if enforce_meta and not meta:
             raise InternalError("missing meta from result")
 
-        if not isinstance(meta, dict):
-            raise InternalError(f"meta must be dict but got {type(meta)}")
-
-        cmd_status = meta.get(MetaKey.STATUS)
-        info = meta.get(MetaKey.INFO, "")
-        if cmd_status == MetaStatusValue.INVALID_JOB_DEFINITION:
-            raise InvalidJobDefinition(f"invalid job definition: {info}")
-        elif cmd_status == MetaStatusValue.NOT_AUTHORIZED:
-            raise AuthorizationError(f"user not authorized for the action '{command}: {info}'")
-        elif cmd_status == MetaStatusValue.SYNTAX_ERROR:
-            raise InternalError(f"protocol error: {info}")
-        elif cmd_status == MetaStatusValue.INVALID_JOB_ID:
-            raise JobNotFound(f"no such job: {info}")
-        elif cmd_status == MetaStatusValue.JOB_RUNNING:
-            raise JobNotDone(f"job {info} is still running")
-        elif cmd_status != MetaStatusValue.OK:
-            raise InternalError(f"server internal error ({cmd_status}): {info}")
+        if meta:
+            if not isinstance(meta, dict):
+                raise InternalError(f"meta must be dict but got {type(meta)}")
+
+            cmd_status = meta.get(MetaKey.STATUS, MetaStatusValue.OK)
+            info = meta.get(MetaKey.INFO, "")
+            if cmd_status == MetaStatusValue.INVALID_JOB_DEFINITION:
+                raise InvalidJobDefinition(f"invalid job definition: {info}")
+            elif cmd_status == MetaStatusValue.NOT_AUTHORIZED:
+                raise AuthorizationError(f"user not authorized for the action '{command}: {info}'")
+            elif cmd_status == MetaStatusValue.NOT_AUTHENTICATED:
+                raise AuthenticationError(f"user not authenticated: {info}")
+            elif cmd_status == MetaStatusValue.SYNTAX_ERROR:
+                raise InternalError(f"syntax error: {info}")
+            elif cmd_status == MetaStatusValue.INVALID_JOB_ID:
+                raise JobNotFound(f"no such job: {info}")
+            elif cmd_status == MetaStatusValue.JOB_RUNNING:
+                raise JobNotDone(f"job {info} is still running")
+            elif cmd_status == MetaStatusValue.JOB_NOT_RUNNING:
+                raise JobNotRunning(f"job {info} is not running")
+            elif cmd_status == MetaStatusValue.CLIENTS_RUNNING:
+                raise ClientsStillRunning("one or more clients are still running")
+            elif cmd_status == MetaStatusValue.NO_CLIENTS:
+                raise NoClientsAvailable("no clients available")
+            elif cmd_status == MetaStatusValue.INTERNAL_ERROR:
+                raise InternalError(f"server internal error: {info}")
+            elif cmd_status == MetaStatusValue.INVALID_TARGET:
+                raise InvalidTarget(info)
+            elif cmd_status != MetaStatusValue.OK:
+                raise InternalError(f"{cmd_status}: {info}")
 
         status = result.get(ResultKey.STATUS, None)
         if not status:
             raise InternalError("missing status in result")
 
         if status in [APIStatus.ERROR_CERT, APIStatus.ERROR_AUTHENTICATION]:
             raise AuthenticationError(f"user not authenticated: {status}")
@@ -188,23 +209,24 @@
             raise ConnectionError(f"cannot connect to server: {status}")
         elif status != APIStatus.SUCCESS:
             details = result.get(ResultKey.DETAILS, "")
             raise RuntimeError(f"runtime error encountered: {status}: {details}")
 
         return result
 
-    def _validate_job_id(self, job_id: str):
+    @staticmethod
+    def _validate_job_id(job_id: str):
         if not job_id:
             raise JobNotFound("job_id is required but not specified.")
 
         if not isinstance(job_id, str):
             raise JobNotFound(f"invalid job_id {job_id}")
 
     def clone_job(self, job_id: str) -> str:
-        """Create a new job by cloning a specified job
+        """Create a new job by cloning a specified job.
 
         Args:
             job_id: job to be cloned
 
         Returns: ID of the new job
 
         """
@@ -214,22 +236,22 @@
         job_id = meta.get(MetaKey.JOB_ID, None)
         info = meta.get(MetaKey.INFO, "")
         if not job_id:
             raise InternalError(f"server failed to return job id: {info}")
         return job_id
 
     def submit_job(self, job_definition_path: str) -> str:
-        """Submit a predefined job to the NVFLARE system
+        """Submit a predefined job to the NVFLARE system.
 
         Args:
             job_definition_path: path to the folder that defines a NVFLARE job
 
         Returns: the job id if accepted by the system
 
-        If the submission fails, exception will be raised:
+        If the submission fails, an exception will be raised.
 
         """
         if not job_definition_path:
             raise InvalidJobDefinition("job_definition_path is required but not specified.")
 
         if not isinstance(job_definition_path, str):
             raise InvalidJobDefinition(f"job_definition_path must be str but got {type(job_definition_path)}.")
@@ -244,15 +266,15 @@
         meta = result[ResultKey.META]
         job_id = meta.get(MetaKey.JOB_ID, None)
         if not job_id:
             raise InternalError("server failed to return job id")
         return job_id
 
     def get_job_meta(self, job_id: str) -> dict:
-        """Get the meta info of the specified job
+        """Get the meta info of the specified job.
 
         Args:
             job_id: ID of the job
 
         Returns: a dict of job metadata
 
         """
@@ -268,23 +290,24 @@
         self,
         detailed: bool = False,
         limit: Optional[int] = None,
         id_prefix: str = None,
         name_prefix: str = None,
         reverse: bool = False,
     ) -> List[dict]:
-        """Get the job info from the server
+        """Get the job info from the server.
 
         Args:
-            detailed: True to get the detailed information for each job, False by default
-            limit: maximum number of jobs to show, with 0 or None to show all (defaults to None to show all)
-            id_prefix: if included, only return jobs with the beginning of the job ID matching the id_prefix
-            name_prefix: if included, only return jobs with the beginning of the job name matching the name_prefix
-            reverse: if specified, list jobs in the reverse order of submission times
-        Returns: a dict of job metadata
+            detailed (bool): True to get the detailed information for each job, False by default
+            limit (int, optional): maximum number of jobs to show, with 0 or None to show all (defaults to None to show all)
+            id_prefix (str): if included, only return jobs with the beginning of the job ID matching the id_prefix
+            name_prefix (str): if included, only return jobs with the beginning of the job name matching the name_prefix
+            reverse (bool): if specified, list jobs in the reverse order of submission times
+
+        Returns: a list of job metadata
 
         """
         if not isinstance(detailed, bool):
             raise ValueError(f"detailed must be bool but got {type(detailed)}")
         if not isinstance(reverse, bool):
             raise ValueError(f"reverse must be bool but got {type(reverse)}")
         if limit is not None and not isinstance(limit, int):
@@ -315,19 +338,18 @@
                 command = command + " " + id_prefix
         result = self._do_command(command)
         meta = result[ResultKey.META]
         jobs_list = meta.get(MetaKey.JOBS, [])
         return jobs_list
 
     def download_job_result(self, job_id: str) -> str:
-        """
-        Download result of the job
+        """Download result of the job.
 
         Args:
-            job_id: ID of the job
+            job_id (str): ID of the job
 
         Returns: folder path to the location of the job result
 
         If the job size is smaller than the maximum size set on the server, the job will download to the download_dir
         set in Session through the admin config, and the path to the downloaded result will be returned. If the size
         of the job is larger than the maximum size, the location to download the job will be returned.
 
@@ -339,47 +361,55 @@
         job_download_url = meta.get(MetaKey.JOB_DOWNLOAD_URL, None)
         if not job_download_url:
             return os.path.join(self.download_dir, download_job_id)
         else:
             return job_download_url
 
     def abort_job(self, job_id: str):
-        """Abort the specified job
+        """Abort the specified job.
 
         Args:
-            job_id: job to be aborted
+            job_id (str): job to be aborted
 
         Returns: dict of (status, info)
 
         If the job is already done, no effect;
-        If job is not started yet, it will be cancelled and won't be scheduled
-        If the job is being executed, it will be aborted
+        If job is not started yet, it will be cancelled and won't be scheduled.
+        If the job is being executed, it will be aborted.
 
         """
         self._validate_job_id(job_id)
         # result = self._do_command(AdminCommandNames.ABORT_JOB + " " + job_id)
         # return result.get(ResultKey.META, None)
         self._do_command(AdminCommandNames.ABORT_JOB + " " + job_id)
 
     def delete_job(self, job_id: str):
-        """Delete the specified job completely from the system
+        """Delete the specified job completely from the system.
 
         Args:
-            job_id: job to be deleted
+            job_id (str): job to be deleted
 
         Returns: None
 
-        The job will be deleted from the job store if the job is not currently running
+        The job will be deleted from the job store if the job is not currently running.
 
         """
         self._validate_job_id(job_id)
         self._do_command(AdminCommandNames.DELETE_JOB + " " + job_id)
 
     def get_system_info(self):
-        result = self._do_command(AdminCommandNames.CHECK_STATUS + " server")
+        """Get general system information.
+
+        Returns: a SystemInfo object
+
+        """
+        return self._do_get_system_info(AdminCommandNames.CHECK_STATUS)
+
+    def _do_get_system_info(self, cmd: str):
+        result = self._do_command(f"{cmd} {TargetType.SERVER}")
         meta = result[ResultKey.META]
         server_info = ServerInfo(status=meta.get(MetaKey.SERVER_STATUS), start_time=meta.get(MetaKey.SERVER_START_TIME))
 
         clients = []
         client_meta_list = meta.get(MetaKey.CLIENTS, None)
         if client_meta_list:
             for c in client_meta_list:
@@ -393,26 +423,406 @@
         if job_meta_list:
             for j in job_meta_list:
                 job_info = JobInfo(app_name=j.get(MetaKey.APP_NAME), job_id=j.get(MetaKey.JOB_ID))
                 jobs.append(job_info)
 
         return SystemInfo(server_info=server_info, client_info=clients, job_info=jobs)
 
+    def get_client_job_status(self, client_names: List[str] = None) -> List[dict]:
+        """Get job status info of specified FL clients.
+
+        Args:
+            client_names (List[str]): names of the clients to get status info
+
+        Returns: A list of jobs running on the clients. Each job is described by a dict of: id, app name and status.
+        If there are multiple jobs running on one client, the list contains one entry for each job for that client.
+        If no FL clients are connected or the server failed to communicate to them, this method returns None.
+
+        """
+        parts = [AdminCommandNames.CHECK_STATUS, TargetType.CLIENT]
+        if client_names:
+            processed_targets_str = process_targets_into_str(client_names)
+            parts.append(processed_targets_str)
+
+        command = " ".join(parts)
+        result = self._do_command(command)
+        meta = result[ResultKey.META]
+        return meta.get(MetaKey.CLIENT_STATUS, None)
+
+    def restart(self, target_type: str, client_names: Optional[List[str]] = None) -> dict:
+        """Restart specified system target(s).
+
+        Args:
+            target_type (str): what system target (server, client, or all) to restart
+            client_names (List[str]): clients to be restarted if target_type is client. If not specified, all clients.
+
+        Returns: a dict that contains detailed info about the restart request:
+            status - the overall status of the result.
+            server_status - whether the server is restarted successfully - only if target_type is "all" or "server".
+            client_status - a dict (keyed on client name) that specifies status of each client - only if target_type
+            is "all" or "client".
+
+        """
+        if target_type not in _VALID_TARGET_TYPES:
+            raise ValueError(f"invalid target_type {target_type} - must be in {_VALID_TARGET_TYPES}")
+
+        parts = [AdminCommandNames.RESTART, target_type]
+        if target_type == TargetType.CLIENT and client_names:
+            processed_targets_str = process_targets_into_str(client_names)
+            parts.append(processed_targets_str)
+
+        command = " ".join(parts)
+        result = self._do_command(command)
+        return result[ResultKey.META]
+
+    def shutdown(self, target_type: TargetType, client_names: Optional[List[str]] = None):
+        """Shut down specified system target(s).
+
+        Args:
+            target_type: what system target (server, client, or all) to shut down
+            client_names: clients to be shut down if target_type is client. If not specified, all clients.
+
+        Returns: None
+        """
+        if target_type not in _VALID_TARGET_TYPES:
+            raise ValueError(f"invalid target_type {target_type} - must be in {_VALID_TARGET_TYPES}")
+
+        parts = [AdminCommandNames.SHUTDOWN, target_type]
+        if target_type == TargetType.CLIENT and client_names:
+            processed_targets_str = process_targets_into_str(client_names)
+            parts.append(processed_targets_str)
+
+        command = " ".join(parts)
+        self._do_command(command)
+
+    def set_timeout(self, value: float):
+        """Set a session-specific command timeout.
+
+        This is the amount of time the server will wait for responses after sending commands to FL clients.
+
+        Note that this value is only effective for the current API session.
+
+        Args:
+            value (float): a positive float number for the timeout in seconds
+
+        Returns: None
+
+        """
+        self.api.set_command_timeout(value)
+
+    def unset_timeout(self):
+        """Unset the session-specific command timeout.
+
+        Once unset, the FL Admin Server's default timeout will be used.
+
+        Returns: None
+
+        """
+        self.api.unset_command_timeout()
+
+    def list_sp(self) -> dict:
+        """List available service providers.
+
+        Returns: a dict that contains information about the primary SP and others
+
+        """
+        reply = self._do_command("list_sp", enforce_meta=False)
+        return reply.get(ResultKey.DETAILS)
+
+    def get_active_sp(self) -> dict:
+        """Get the current active service provider (SP).
+
+        Returns: a dict that describes the current active SP. If no SP is available currently, the 'name' attribute of
+        the result is empty.
+        """
+        reply = self._do_command("get_active_sp", enforce_meta=False)
+        return reply.get(ResultKey.META)
+
+    def promote_sp(self, sp_end_point: str):
+        """Promote the specified endpoint to become the active SP.
+
+        Args:
+            sp_end_point: the endpoint of the SP. It's string in this format: <url>:<server_port>:<admin_port>
+
+        Returns: None
+
+        """
+        sp_end_point = validate_sp_string(sp_end_point)
+        self._do_command("promote_sp " + sp_end_point)
+
+    def get_available_apps_to_upload(self):
+        """Get defined FLARE app folders from the upload folder on the machine the FLARE API is running.
+
+        Returns: a list of app folders
+
+        """
+        dir_list = []
+        for item in os.listdir(self.upload_dir):
+            if os.path.isdir(os.path.join(self.upload_dir, item)):
+                dir_list.append(item)
+        return dir_list
+
+    def shutdown_system(self):
+        """Shutdown the whole NVFLARE system including the overseer, FL server(s), and all FL clients.
+
+        Returns: None
+
+        Note: the user must be a Project Admin to use this method; otherwise the NOT_AUTHORIZED exception will be raised.
+
+        """
+        sys_info = self._do_get_system_info(AdminCommandNames.ADMIN_CHECK_STATUS)
+        if sys_info.server_info.status != "stopped":
+            raise JobNotDone("there are still running jobs")
+
+        resp = self.overseer_agent.set_state("shutdown")
+        err = json.loads(resp.text).get("Error")
+        if err:
+            raise RuntimeError(err)
+
+    def ls_target(self, target: str, options: str = None, path: str = None) -> str:
+        """Run the "ls" command on the specified target and return the result.
+
+        Args:
+            target: the target (server or a client name) the command will be run on
+            options: options of the "ls" command
+            path: the optional file path
+
+        Returns: result of "ls" command
+
+        """
+        return self._shell_command_on_target("ls", target, options, path)
+
+    def cat_target(self, target: str, options: str = None, file: str = None) -> str:
+        """Run the "cat" command on the specified target and return the result.
+
+        Args:
+            target: the target (server or a client name) the command will be run on
+            options: options of the "cat" command
+            file: the file that the "cat" command will run against
+
+        Returns: result of "cat" command
+
+        """
+        return self._shell_command_on_target("cat", target, options, file, fp_required=True, fp_type="file")
+
+    def tail_target(self, target: str, options: str = None, file: str = None) -> str:
+        """Run the "tail" command on the specified target and return the result.
+
+        Args:
+            target: the target (server or a client name) the command will be run on
+            options: options of the "tail" command
+            file: the file that the "tail" command will run against
+
+        Returns: result of "tail" command
+
+        """
+        return self._shell_command_on_target("tail", target, options, file, fp_required=True, fp_type="file")
+
+    def tail_target_log(self, target: str, options: str = None) -> str:
+        """Run the "tail log.txt" command on the specified target and return the result.
+
+        Args:
+            target: the target (server or a client name) the command will be run on
+            options: options of the "tail" command
+
+        Returns: result of "tail" command
+
+        """
+        return self.tail_target(target, options, file="log.txt")
+
+    def head_target(self, target: str, options: str = None, file: str = None) -> str:
+        """Run the "head" command on the specified target and return the result.
+
+        Args:
+            target: the target (server or a client name) the command will be run on
+            options: options of the "head" command
+            file: the file that the "head" command will run against
+
+        Returns: result of "head" command
+
+        """
+        return self._shell_command_on_target("head", target, options, file, fp_required=True, fp_type="file")
+
+    def head_target_log(self, target: str, options: str = None) -> str:
+        """Run the "head log.txt" command on the specified target and return the result.
+
+        Args:
+            target: the target (server or a client name) the command will be run on
+            options: options of the "head" command
+
+        Returns: result of "head" command
+
+        """
+        return self.head_target(target, options, file="log.txt")
+
+    def grep_target(self, target: str, options: str = None, pattern: str = None, file: str = None) -> str:
+        """Run the "grep" command on the specified target and return the result.
+
+        Args:
+            target: the target (server or a client name) the command will be run on
+            options: options of the "grep" command
+            pattern: the grep pattern
+            file: the file that the "grep" command will run against
+
+        Returns: result of "grep" command
+
+        """
+        return self._shell_command_on_target(
+            "grep", target, options, file, pattern=pattern, pattern_required=True, fp_required=True, fp_type="file"
+        )
+
+    def get_working_directory(self, target: str) -> str:
+        """Get the working directory of the specified target.
+
+        Args:
+            target (str): the target (server of a client name)
+
+        Returns: current working directory of the specified target
+
+        """
+        return self._shell_command_on_target("pwd", target, options=None, fp=None)
+
+    def _shell_command_on_target(
+        self,
+        cmd: str,
+        target: str,
+        options,
+        fp,
+        pattern=None,
+        pattern_required=False,
+        fp_required=False,
+        fp_type="path",
+    ) -> str:
+        target = validate_required_target_string(target)
+        parts = [cmd, target]
+        if options:
+            options = validate_options_string(options)
+            parts.append(options)
+
+        if pattern_required:
+            if not pattern:
+                raise SyntaxError("pattern is required but not specified.")
+            if not isinstance(pattern, str):
+                raise ValueError("pattern is not str.")
+            parts.append('"' + pattern + '"')
+
+        if fp_required and not fp:
+            raise SyntaxError(f"{fp_type} is required but not specified.")
+
+        if fp:
+            if fp_type == "path":
+                validate_path_string(fp)
+            else:
+                validate_file_string(fp)
+            parts.append(fp)
+        command = " ".join(parts)
+        reply = self._do_command(command, enforce_meta=False)
+        return self._get_string_data(reply)
+
+    @staticmethod
+    def _get_string_data(reply: dict) -> str:
+        result = ""
+        data_items = reply.get(ProtoKey.DATA, [])
+        for it in data_items:
+            if isinstance(it, dict):
+                if it.get(ProtoKey.TYPE) == ProtoKey.STRING:
+                    result += it.get(ProtoKey.DATA, "")
+        return result
+
+    @staticmethod
+    def _get_dict_data(reply: dict) -> dict:
+        result = {}
+        data_items = reply.get(ProtoKey.DATA, [])
+        for it in data_items:
+            if isinstance(it, dict):
+                if it.get(ProtoKey.TYPE) == ProtoKey.DICT:
+                    return it.get(ProtoKey.DATA, {})
+        return result
+
+    def show_stats(self, job_id: str, target_type: str, targets: Optional[List[str]] = None) -> dict:
+        """Show processing stats of specified job on specified targets.
+
+        Args:
+            job_id (str): ID of the job
+            target_type (str): type of target (server or client)
+            targets: list of client names if target type is "client". All clients if not specified.
+
+        Returns: a dict that contains job stats on specified targets. The key of the dict is target name. The value is
+        a dict of stats reported by different system components (ServerRunner or ClientRunner).
+
+        """
+        return self._collect_info(AdminCommandNames.SHOW_STATS, job_id, target_type, targets)
+
+    def show_errors(self, job_id: str, target_type: str, targets: Optional[List[str]] = None) -> dict:
+        """Show processing errors of specified job on specified targets.
+
+        Args:
+            job_id (str): ID of the job
+            target_type (str): type of target (server or client)
+            targets: list of client names if target type is "client". All clients if not specified.
+
+        Returns: a dict that contains job errors (if any) on specified targets. The key of the dict is target name.
+        The value is a dict of errors reported by different system components (ServerRunner or ClientRunner).
+
+        """
+        return self._collect_info(AdminCommandNames.SHOW_ERRORS, job_id, target_type, targets)
+
+    def reset_errors(self, job_id: str):
+        """Clear errors for all system targets for the specified job.
+
+        Args:
+            job_id (str): ID of the job
+
+        Returns: None
+
+        """
+        self._collect_info(AdminCommandNames.RESET_ERRORS, job_id, TargetType.ALL)
+
+    def _collect_info(self, cmd: str, job_id: str, target_type: str, targets=None) -> dict:
+        if not job_id:
+            raise ValueError("job_id is required but not specified.")
+
+        if not isinstance(job_id, str):
+            raise TypeError("job_id must be str but got {}.".format(type(job_id)))
+
+        if target_type not in _VALID_TARGET_TYPES:
+            raise ValueError(f"invalid target_type {target_type}: must be one of {_VALID_TARGET_TYPES}")
+
+        parts = [cmd, job_id, target_type]
+        if target_type == TargetType.CLIENT and targets:
+            processed_targets_str = process_targets_into_str(targets)
+            parts.append(processed_targets_str)
+
+        command = " ".join(parts)
+        reply = self._do_command(command, enforce_meta=False)
+        return self._get_dict_data(reply)
+
+    def get_connected_client_list(self) -> List[ClientInfo]:
+        """Get the list of connected clients.
+
+        Returns: a list of ClientInfo objects
+
+        """
+        sys_info = self.get_system_info()
+        return sys_info.client_info
+
     def monitor_job(
         self, job_id: str, timeout: float = 0.0, poll_interval: float = 2.0, cb=None, *cb_args, **cb_kwargs
     ) -> MonitorReturnCode:
-        """Monitor the job progress until one of the conditions occurs:
-         - job is done
-         - timeout
-         - the status_cb returns False
+        """Monitor the job progress.
+
+        Monitors until one of the conditions occurs:
+            - job is done
+            - timeout
+            - the status_cb returns False
 
         Args:
-            job_id: the job to be monitored
-            timeout: how long to monitor. If 0, never time out.
-            poll_interval: how often to poll job status
+            job_id (str): the job to be monitored
+            timeout (float): how long to monitor. If 0, never time out.
+            poll_interval (float): how often to poll job status
             cb: if provided, callback to be called after each status poll
 
         Returns: a MonitorReturnCode
 
         Every time the cb is called, it must return a bool indicating whether the monitor
         should continue. If False, this method ends.
 
@@ -436,16 +846,17 @@
             if job_status.startswith("FINISHED"):
                 return MonitorReturnCode.JOB_FINISHED
 
             time.sleep(poll_interval)
 
 
 def basic_cb_with_print(session: Session, job_id: str, job_meta, *cb_args, **cb_kwargs) -> bool:
-    """This is a sample callback to use with monitor_job that demonstrates how a custom callback can
-    be used
+    """This is a sample callback to use with monitor_job.
+
+    This demonstrates how a custom callback can be used.
 
     """
     if job_meta["status"] == "RUNNING":
         if cb_kwargs["cb_run_counter"]["count"] < 3:
             print(job_meta)
         else:
             print(".", end="")
@@ -453,41 +864,41 @@
         print("\n" + str(job_meta))
 
     cb_kwargs["cb_run_counter"]["count"] += 1
     return True
 
 
 def new_secure_session(username: str, startup_kit_location: str, debug: bool = False, timeout: float = 10.0) -> Session:
-    """Create a new secure session with NVFLARE system
+    """Create a new secure FLARE API session with the NVFLARE system.
 
     Args:
-        username: username assigned to the user
-        startup_kit_location: path to the provisioned startup folder, the root admin dir containing the startup folder
-        debug: enable debug mode
-        timeout: how long to try to establish the session
+        username (str): username assigned to the user
+        startup_kit_location (str): path to the provisioned startup folder, the root admin dir containing the startup folder
+        debug (bool): enable debug mode
+        timeout (float): how long to try to establish the session, in seconds
 
     Returns: a Session object
 
     """
     session = Session(username=username, startup_path=startup_kit_location, secure_mode=True, debug=debug)
 
     session.try_connect(timeout)
     return session
 
 
 def new_insecure_session(startup_kit_location: str, debug: bool = False, timeout: float = 10.0) -> Session:
-    """Create a new secure session with NVFLARE system
+    """Create a new insecure FLARE API session with the NVFLARE system.
 
     Args:
-        startup_kit_location: path to the provisioned startup folder
-        debug: enable debug mode
-        timeout: how long to try to establish the session
+        startup_kit_location (str): path to the provisioned startup folder
+        debug (bool): enable debug mode
+        timeout (float): how long to try to establish the session, in seconds
 
     Returns: a Session object
 
-    The username for insecure session is always "admin"
+    The username for insecure session is always "admin".
 
     """
     session = Session(username="admin", startup_path=startup_kit_location, secure_mode=False, debug=debug)
 
     session.try_connect(timeout)
     return session
```

## nvflare/fuel/hci/cmd_arg_utils.py

```diff
@@ -10,18 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
 import io
+import os
 import re
 import shlex
 from typing import List
 
+from nvflare.apis.utils.format_check import type_pattern_mapping
+
 
 def split_to_args(line: str) -> List[str]:
     if '"' in line:
         return shlex.split(line)
     else:
         line = re.sub(" +", " ", line)
         return line.split(" ")
@@ -55,16 +58,86 @@
     def error(self, message):
         self.err = message
 
     def validate(self, args):
         try:
             result = self.parse_args(args)
             return self.err, result
-        except Exception:
+        except BaseException:
             return 'argument error; try "? cmdName to show supported usage for a command"', None
 
     def get_usage(self) -> str:
         buffer = io.StringIO()
         self.print_help(buffer)
         usage_output = buffer.getvalue().split("\n", 1)[1]
         buffer.close()
         return usage_output
+
+
+def process_targets_into_str(targets: List[str]) -> str:
+    if not isinstance(targets, list):
+        raise SyntaxError("targets is not a list.")
+    if not all(isinstance(t, str) for t in targets):
+        raise SyntaxError("all targets in the list of targets must be strings.")
+    for t in targets:
+        try:
+            validate_required_target_string(t)
+        except SyntaxError:
+            raise SyntaxError(f"invalid target {t}")
+    return " ".join(targets)
+
+
+def validate_required_target_string(target: str) -> str:
+    """Returns the target string if it exists and is valid."""
+    if not target:
+        raise SyntaxError("target is required but not specified.")
+    if not isinstance(target, str):
+        raise SyntaxError("target is not str.")
+    if not re.match("^[A-Za-z0-9._-]*$", target):
+        raise SyntaxError("target must be a string of only valid characters and no spaces.")
+    return target
+
+
+def validate_options_string(options: str) -> str:
+    """Returns the options string if it is valid."""
+    if not isinstance(options, str):
+        raise SyntaxError("options is not str.")
+    if not re.match("^[A-Za-z0-9- ]*$", options):
+        raise SyntaxError("options must be a string of only valid characters.")
+    return options
+
+
+def validate_path_string(path: str) -> str:
+    """Returns the path string if it is valid."""
+    if not isinstance(path, str):
+        raise SyntaxError("path is not str.")
+    if not re.match("^[A-Za-z0-9-._/]*$", path):
+        raise SyntaxError("unsupported characters in path {}".format(path))
+    if os.path.isabs(path):
+        raise SyntaxError("absolute path is not allowed")
+    paths = path.split(os.path.sep)
+    for p in paths:
+        if p == "..":
+            raise SyntaxError(".. in path name is not allowed")
+    return path
+
+
+def validate_file_string(file: str) -> str:
+    """Returns the file string if it is valid."""
+    validate_path_string(file)
+    basename, file_extension = os.path.splitext(file)
+    if file_extension not in [".txt", ".log", ".json", ".csv", ".sh", ".config", ".py"]:
+        raise SyntaxError(
+            "this command cannot be applied to file {}. Only files with the following extensions are "
+            "permitted: .txt, .log, .json, .csv, .sh, .config, .py".format(file)
+        )
+    return file
+
+
+def validate_sp_string(sp_string) -> str:
+    if re.match(
+        type_pattern_mapping.get("sp_end_point"),
+        sp_string,
+    ):
+        return sp_string
+    else:
+        raise SyntaxError("sp_string must be of the format example.com:8002:8003")
```

## nvflare/fuel/hci/conn.py

```diff
@@ -174,14 +174,17 @@
         if isinstance(data, str):
             self.append_string(data, flush, meta=meta)
         elif isinstance(data, dict):
             self.append_dict(data, flush, meta)
         else:
             self.append_error("unsupported data type {}".format(type(data)))
 
+    def update_meta(self, meta: dict):
+        self.buffer.update_meta(meta)
+
     def flush(self):
         line = self.buffer.encode()
         if line is None or len(line) <= 0:
             return
 
         self.buffer.reset()
         self._send_line(line, all_end=False)
```

## nvflare/fuel/hci/proto.py

```diff
@@ -31,14 +31,16 @@
     ROWS = "rows"
     DICT = "dict"
     SUCCESS = "success"
     ERROR = "error"
     SHUTDOWN = "shutdown"
     COMMAND = "command"
     TOKEN = "token"
+    DETAILS = "details"
+    STATUS = "status"
 
 
 class MetaKey(object):
 
     STATUS = "status"
     INFO = "info"
     JOB_ID = "job_id"
@@ -46,36 +48,46 @@
     JOB_DOWNLOAD_URL = "job_download_url"
     APP_NAME = "app_name"
     SERVER_STATUS = "server_status"
     SERVER_START_TIME = "server_start_time"
     CLIENT_NAME = "client_name"
     CLIENT_LAST_CONNECT_TIME = "client_last_conn_time"
     CLIENTS = "clients"
+    CLIENT_STATUS = "client_status"
     JOBS = "jobs"
     JOB_NAME = "job_name"
     SUBMIT_TIME = "submit_time"
     DURATION = "duration"
+    CMD_TIMEOUT = "cmd_timeout"
 
 
 class MetaStatusValue(object):
 
     OK = "ok"
     SYNTAX_ERROR = "syntax_error"
     NOT_AUTHORIZED = "not_authorized"
+    NOT_AUTHENTICATED = "not_authenticated"
     ERROR = "error"
     INTERNAL_ERROR = "internal_error"
+    INVALID_TARGET = "invalid_target"
     INVALID_JOB_DEFINITION = "invalid_job_def"
     INVALID_JOB_ID = "invalid_job_id"
     JOB_RUNNING = "job_running"
+    JOB_NOT_RUNNING = "job_not_running"
+    CLIENTS_RUNNING = "clients_running"
+    NO_JOBS = "no_jobs"
+    NO_REPLY = "no_reply"
+    NO_CLIENTS = "no_clients"
 
 
 class CredentialType(str, Enum):
 
     PASSWORD = "password"
     CERT = "cert"
+    LOCAL_CERT = "local_cert"
 
 
 class InternalCommands(object):
 
     PWD_LOGIN = "_login"
     CERT_LOGIN = "_cert_login"
     LOGOUT = "_logout"
@@ -103,35 +115,37 @@
         meta_rows = []
         if name:
             self.meta.update({name: meta_rows})
         t = Table(headers, meta_rows)
         self.data.append({ProtoKey.TYPE: ProtoKey.TABLE, ProtoKey.ROWS: t.rows})
         return t
 
-    def append_string(self, data: str, meta: dict = None):
-        self.data.append({ProtoKey.TYPE: ProtoKey.STRING, ProtoKey.DATA: data})
+    def update_meta(self, meta: dict):
         if meta:
             self.meta.update(meta)
 
+    def append_string(self, data: str, meta: dict = None):
+        self.data.append({ProtoKey.TYPE: ProtoKey.STRING, ProtoKey.DATA: data})
+        self.update_meta(meta)
+
     def append_dict(self, data: dict, meta: dict = None):
         self.data.append({ProtoKey.TYPE: ProtoKey.DICT, ProtoKey.DATA: data})
-        if meta:
-            self.meta.update(meta)
+        self.update_meta(meta)
 
     def append_success(self, data: str, meta: dict = None):
         self.data.append({ProtoKey.TYPE: ProtoKey.SUCCESS, ProtoKey.DATA: data})
         if not meta:
             meta = make_meta(MetaStatusValue.OK, data)
-        self.meta.update(meta)
+        self.update_meta(meta)
 
     def append_error(self, data: str, meta: dict = None):
         self.data.append({ProtoKey.TYPE: ProtoKey.ERROR, ProtoKey.DATA: data})
         if not meta:
             meta = make_meta(MetaStatusValue.ERROR, data)
-        self.meta.update(meta)
+        self.update_meta(meta)
 
     def append_command(self, cmd: str):
         self.data.append({ProtoKey.TYPE: ProtoKey.COMMAND, ProtoKey.DATA: cmd})
 
     def append_token(self, token: str):
         self.data.append({ProtoKey.TYPE: ProtoKey.TOKEN, ProtoKey.DATA: token})
 
@@ -203,15 +217,15 @@
                 assert ProtoKey.ROWS in item
                 rows = item[ProtoKey.ROWS]
                 assert isinstance(rows, list)
                 for row in rows:
                     assert isinstance(row, list)
 
         return json_data
-    except Exception:
+    except BaseException:
         return None
 
 
 def make_meta(status: str, info: str = "", extra: dict = None) -> dict:
     meta = {MetaKey.STATUS: status, MetaKey.INFO: info}
     if extra:
         meta.update(extra)
```

## nvflare/fuel/hci/client/api.py

```diff
@@ -19,15 +19,15 @@
 import threading
 import time
 from datetime import datetime
 from typing import List, Optional
 
 from nvflare.fuel.hci.cmd_arg_utils import split_to_args
 from nvflare.fuel.hci.conn import Connection, receive_and_process
-from nvflare.fuel.hci.proto import ConfirmMethod, InternalCommands, ProtoKey, make_error
+from nvflare.fuel.hci.proto import ConfirmMethod, InternalCommands, MetaKey, ProtoKey, make_error
 from nvflare.fuel.hci.reg import CommandEntry, CommandModule, CommandRegister
 from nvflare.fuel.hci.table import Table
 from nvflare.fuel.utils.fsm import FSM, State
 from nvflare.security.logging import secure_format_exception, secure_log_traceback
 
 from .api_spec import (
     AdminAPISpec,
@@ -40,20 +40,23 @@
 )
 from .api_status import APIStatus
 
 _CMD_TYPE_UNKNOWN = 0
 _CMD_TYPE_CLIENT = 1
 _CMD_TYPE_SERVER = 2
 
+MAX_AUTO_LOGIN_TRIES = 300
+AUTO_LOGIN_INTERVAL = 1.0
+
 
 class ResultKey(object):
 
-    STATUS = "status"
-    DETAILS = "details"
-    META = "meta"
+    STATUS = ProtoKey.STATUS
+    DETAILS = ProtoKey.DETAILS
+    META = ProtoKey.META
 
 
 def session_event_cb_signature(event_type: str, info: str):
     """
     This defines the signature of session_event callback.
     When creating the AdminAPI object, you can provide a session event callback function.
     This function is called when a session event happens.
@@ -66,14 +69,16 @@
 
     """
     pass
 
 
 class _ServerReplyJsonProcessor(object):
     def __init__(self, ctx: CommandContext):
+        if not isinstance(ctx, CommandContext):
+            raise TypeError(f"ctx is not an instance of CommandContext. but get {type(ctx)}")
         api = ctx.get_api()
         self.debug = api.debug
         self.ctx = ctx
 
     def process_server_reply(self, resp):
         """Process the server reply and store the status/details into API's `command_result`
         NOTE: this func is used for receive_and_process(), which is defined by conn!
@@ -82,15 +87,14 @@
         Args:
             resp: The raw response that returns by the server.
         """
         if self.debug:
             print("DEBUG: Server Reply: {}".format(resp))
 
         ctx = self.ctx
-        assert isinstance(ctx, CommandContext)
 
         # this resp is what is usually directly used to return, straight from server
         ctx.set_command_result(resp)
         reply_processor = ctx.get_reply_processor()
         if reply_processor is None:
             reply_processor = _DefaultReplyProcessor()
 
@@ -197,15 +201,15 @@
 class SessionEventType(object):
 
     WAIT_FOR_SERVER_ADDR = "wait_for_server_addr"
     SERVER_ADDR_OBTAINED = "server_addr_obtained"
     SESSION_CLOSED = "session_closed"  # close the current session
     LOGIN_SUCCESS = "login_success"  # logged in to server
     LOGIN_FAILURE = "login_failure"  # cannot login to server
-    TRYING_LOGIN = "trying_login"  # still try to login
+    TRYING_LOGIN = "trying_login"  # still try to log in
     SP_ADDR_CHANGED = "sp_addr_changed"  # service provider address changed
     SESSION_TIMEOUT = "session_timeout"  # server timed out current session
 
 
 _STATE_NAME_WAIT_FOR_SERVER_ADDR = "wait_for_server_addr"
 _STATE_NAME_LOGIN = "login"
 _STATE_NAME_OPERATE = "operate"
@@ -291,15 +295,15 @@
 
         with api.addr_lock:
             cur_host = api.host
             cur_port = api.port
             cur_ssid = api.ssid
 
         if new_host != cur_host or new_port != cur_port or cur_ssid != new_ssid:
-            # need to relogin
+            # need to re-login
             api.fire_session_event(SessionEventType.SP_ADDR_CHANGED, f"Server address changed to {new_host}:{new_port}")
             return _STATE_NAME_LOGIN
 
         # check server session status
         if not self.sess_check_interval:
             return ""
 
@@ -330,31 +334,33 @@
         download_dir: str = "",
         cmd_modules: Optional[List] = None,
         poc: bool = False,
         debug: bool = False,
         session_event_cb=None,
         session_timeout_interval=None,
         session_status_check_interval=None,
+        auto_login_max_tries: int = 5,
     ):
-        """Underlying API to keep certs, keys and connection information and to execute admin commands through do_command.
+        """API to keep certs, keys and connection information and to execute admin commands through do_command.
 
         Args:
             ca_cert: path to CA Cert file, by default provisioned rootCA.pem
             client_cert: path to admin client Cert file, by default provisioned as client.crt
             client_key: path to admin client Key file, by default provisioned as client.key
             upload_dir: File transfer upload directory. Folders uploaded to the server to be deployed must be here. Folder must already exist and be accessible.
             download_dir: File transfer download directory. Can be same as upload_dir. Folder must already exist and be accessible.
             cmd_modules: command modules to load and register. Note that FileTransferModule is initialized here with upload_dir and download_dir if cmd_modules is None.
             service_finder: used to obtain the primary service provider to set the host and port of the active server
             user_name: Username to authenticate with FL server
             poc: Whether to enable poc mode for using the proof of concept example without secure communication.
             debug: Whether to print debug messages, which can help with diagnosing problems. False by default.
             session_event_cb: the session event callback
-            session_timeout_interval: if specified, automatically close the session after inactive for this long
-            session_status_check_interval: how often to check session status with server
+            session_timeout_interval: if specified, automatically close the session after inactive for this long, unit is second
+            session_status_check_interval: how often to check session status with server, unit is second
+            auto_login_max_tries: maximum number of tries to auto-login.
         """
         super().__init__()
         if cmd_modules is None:
             from .file_transfer import FileTransferModule
 
             cmd_modules = [FileTransferModule(upload_dir=upload_dir, download_dir=download_dir)]
         elif not isinstance(cmd_modules, list):
@@ -398,14 +404,15 @@
                 raise Exception("missing Client Key file name")
             self.client_key = client_key
 
             self.service_finder.set_secure_context(
                 ca_cert_path=self.ca_cert, cert_path=self.client_cert, private_key_path=self.client_key
             )
         self.debug = debug
+        self.cmd_timeout = None
 
         # for login
         self.token = None
         self.login_result = None
         if not user_name:
             raise Exception("user_name is required.")
         self.user_name = user_name
@@ -423,33 +430,48 @@
 
         self.server_sess_active = False
         self.shutdown_asked = False
 
         self.sess_monitor_thread = None
         self.sess_monitor_active = False
 
-        if session_event_cb is not None:
-            assert callable(session_event_cb), "session_event_cb must be callable"
+        if session_event_cb is not None and not callable(session_event_cb):
+            raise RuntimeError("session_event_cb must be callable")
         self.session_event_cb = session_event_cb
 
         # create the FSM for session monitoring
+        if auto_login_max_tries < 0 or auto_login_max_tries > MAX_AUTO_LOGIN_TRIES:
+            raise ValueError(f"auto_login_max_tries is out of range: [0, {MAX_AUTO_LOGIN_TRIES}]")
+        self.auto_login_max_tries = auto_login_max_tries
         fsm = FSM("session monitor")
         fsm.add_state(_WaitForServerAddress(self))
         fsm.add_state(_TryLogin(self))
         fsm.add_state(_Operate(self, session_status_check_interval))
         self.fsm = fsm
 
         self.session_timeout_interval = session_timeout_interval
         self.last_sess_activity_time = time.time()
 
         self.closed = False
         self.in_logout = False
         self.service_finder.start(self._handle_sp_address_change)
         self._start_session_monitor()
 
+    def set_command_timeout(self, timeout: float):
+        if not isinstance(timeout, (int, float)):
+            raise TypeError(f"timeout must be a number but got {type(timeout)}")
+        timeout = float(timeout)
+        if timeout <= 0.0:
+            raise ValueError(f"invalid timeout value {timeout} - must be > 0.0")
+
+        self.cmd_timeout = timeout
+
+    def unset_command_timeout(self):
+        self.cmd_timeout = None
+
     def fire_session_event(self, event_type: str, msg: str):
         if self.session_event_cb is not None:
             self.session_event_cb(event_type, msg)
 
     def _handle_sp_address_change(self, host: str, port: int, ssid: str):
         with self.addr_lock:
             if host == self.host and port == self.port and ssid == self.ssid:
@@ -458,36 +480,41 @@
 
         with self.new_addr_lock:
             self.new_host = host
             self.new_port = port
             self.new_ssid = ssid
 
     def _try_auto_login(self):
-        resp = {}
-        for i in range(5):
+        resp = None
+        for i in range(self.auto_login_max_tries):
             self.fire_session_event(SessionEventType.TRYING_LOGIN, "Trying to login, please wait ...")
 
             if self.poc:
                 resp = self.login_with_poc(username=self.user_name, poc_key=self.poc_key)
             else:
                 resp = self.login(username=self.user_name)
             if resp[ResultKey.STATUS] in [APIStatus.SUCCESS, APIStatus.ERROR_AUTHENTICATION, APIStatus.ERROR_CERT]:
                 return resp
-            time.sleep(1.0)
+            time.sleep(AUTO_LOGIN_INTERVAL)
+        if resp is None:
+            resp = {
+                ResultKey.STATUS: APIStatus.ERROR_RUNTIME,
+                ResultKey.DETAILS: f"Auto login failed after {self.auto_login_max_tries} tries",
+            }
         return resp
 
     def auto_login(self):
         try:
             result = self._try_auto_login()
             if self.debug:
                 print(f"DEBUG: login result is {result}")
-        except:
+        except Exception as e:
             result = {
                 ResultKey.STATUS: APIStatus.ERROR_RUNTIME,
-                ResultKey.DETAILS: "Exception occurred when trying to login - please try later",
+                ResultKey.DETAILS: f"Exception occurred ({secure_format_exception(e)}) when trying to login - please try later",
             }
         return result
 
     def _load_client_cmds_from_modules(self, cmd_modules):
         if cmd_modules:
             for m in cmd_modules:
                 self.client_cmd_reg.register_module(m, include_invisible=False)
@@ -535,30 +562,30 @@
                 self.last_sess_activity_time
                 and self.session_timeout_interval
                 and time.time() - self.last_sess_activity_time > self.session_timeout_interval
             ):
                 return "Your session is ended due to inactivity"
 
             next_state = self.fsm.execute()
-            if not next_state:
+            if next_state is None:
                 if self.fsm.error:
                     return self.fsm.error
                 else:
                     return ""
 
     def _monitor_session(self, interval):
         try:
             msg = self._do_monitor_session(interval)
-        except:
-            msg = "exception occurred"
+        except Exception as e:
+            msg = f"exception occurred: {secure_format_exception(e)}"
 
         self.server_sess_active = False
         self.fire_session_event(SessionEventType.SESSION_CLOSED, msg)
 
-        # this is in the session_monitor thread - do not close the monitor or we'll run into
+        # this is in the session_monitor thread - do not close the monitor, or we'll run into
         # "cannot join current thread" error!
         self.close(close_session_monitor=False)
 
     def logout(self):
         """Send logout command to server."""
         self.in_logout = True
         resp = self.server_execute(InternalCommands.LOGOUT)
@@ -665,14 +692,17 @@
         process_json_func = json_processor.process_server_reply
 
         conn = Connection(sock, self)
         conn.append_command(command)
         if self.token:
             conn.append_token(self.token)
 
+        if self.cmd_timeout:
+            conn.update_meta({MetaKey.CMD_TIMEOUT: self.cmd_timeout})
+
         conn.close()
         ok = receive_and_process(sock, process_json_func)
         if not ok:
             process_json_func(
                 make_error("Failed to communicate with Admin Server {} on {}".format(self.host, self.port))
             )
```

## nvflare/fuel/hci/client/api_spec.py

```diff
@@ -173,18 +173,20 @@
         pass
 
 
 def service_address_changed_cb_signature(host: str, port: int, ssid: str):
     pass
 
 
-class ServiceFinder(object):
+class ServiceFinder(ABC):
+    @abstractmethod
     def start(self, service_address_changed_cb):
         pass
 
+    @abstractmethod
     def stop(self):
         pass
 
     def set_secure_context(self, ca_cert_path: str, cert_path: str, private_key_path: str):
         pass
 
     def get_command_module(self) -> CommandModule:
```

## nvflare/fuel/hci/client/cli.py

```diff
@@ -18,15 +18,15 @@
 import os
 import signal
 import time
 from datetime import datetime
 from typing import List, Optional
 
 from nvflare.fuel.hci.cmd_arg_utils import join_args, split_to_args
-from nvflare.fuel.hci.proto import CredentialType
+from nvflare.fuel.hci.proto import CredentialType, ProtoKey
 from nvflare.fuel.hci.reg import CommandModule, CommandModuleSpec, CommandRegister, CommandSpec
 from nvflare.fuel.hci.security import hash_password, verify_password
 from nvflare.fuel.hci.table import Table
 from nvflare.security.logging import secure_format_exception, secure_log_traceback
 
 from .api import AdminAPI, CommandInfo, SessionEventType
 from .api_spec import ServiceFinder
@@ -39,31 +39,32 @@
             name="",
             cmd_specs=[
                 CommandSpec(name="bye", description="exit from the client", usage="bye", handler_func=None),
                 CommandSpec(name="help", description="get command help information", usage="help", handler_func=None),
                 CommandSpec(
                     name="lpwd", description="print local work dir of the admin client", usage="lpwd", handler_func=None
                 ),
+                CommandSpec(
+                    name="timeout", description="set/show command timeout", usage="timeout [value]", handler_func=None
+                ),
             ],
         )
 
 
 class AdminClient(cmd.Cmd):
     """Admin command prompt for submitting admin commands to the server through the CLI.
 
     Args:
-        host: cn provisioned for the server, with this fully qualified domain name resolving to the IP of the FL server. This may be set by the OverseerAgent.
-        port: port provisioned as admin_port for FL admin communication, by default provisioned as 8003, must be int if provided. This may be set by the OverseerAgent.
         prompt: prompt to use for the command prompt
         ca_cert: path to CA Cert file, by default provisioned rootCA.pem
         client_cert: path to admin client Cert file, by default provisioned as client.crt
         client_key: path to admin client Key file, by default provisioned as client.key
         credential_type: what type of credential to use
         cmd_modules: command modules to load and register
-        idp_agent: IdpAgent to obtain the primary service provider to set the host and port of the active server
+        service_finder: used to obtain the primary service provider to set the host and port of the active server
         debug: whether to print debug messages. False by default.
     """
 
     def __init__(
         self,
         prompt: str = "> ",
         credential_type: CredentialType = CredentialType.PASSWORD,
@@ -72,27 +73,29 @@
         client_key=None,
         upload_dir="",
         download_dir="",
         cmd_modules: Optional[List] = None,
         service_finder: ServiceFinder = None,
         session_timeout_interval=900,  # close the client after 15 minutes of inactivity
         debug: bool = False,
+        username: str = "",
     ):
-        cmd.Cmd.__init__(self)
+        super().__init__()
         self.intro = "Type help or ? to list commands.\n"
         self.prompt = prompt
         self.user_name = "admin"
         self.pwd = None
         self.credential_type = credential_type
 
         self.service_finder = service_finder
         self.debug = debug
         self.out_file = None
         self.no_stdout = False
         self.stopped = False  # use this flag to prevent unnecessary signal exception
+        self.username = username
 
         if not isinstance(service_finder, ServiceFinder):
             raise TypeError("service_finder must be ServiceProvider but got {}.".format(type(service_finder)))
 
         if not isinstance(credential_type, CredentialType):
             raise TypeError("invalid credential_type {}".format(credential_type))
 
@@ -172,14 +175,33 @@
         self.api.logout()
         return True
 
     def do_lpwd(self, arg):
         """print local current work dir"""
         self.write_string(os.getcwd())
 
+    def do_timeout(self, arg):
+        if not arg:
+            # display current setting
+            t = self.api.cmd_timeout
+            if t:
+                self.write_string(str(t))
+            else:
+                self.write_string("not set")
+            return
+        try:
+            t = float(arg)
+            self.api.set_command_timeout(t)
+            if t == 0:
+                self.write_string("command timeout is unset")
+            else:
+                self.write_string(f"command timeout is set to {t}")
+        except:
+            self.write_string("invalid timeout value - must be float number >= 0.0")
+
     def emptyline(self):
         return
 
     def _show_one_command(self, cmd_name, reg, show_invisible=False):
         entries = reg.get_command_entries(cmd_name)
         if len(entries) <= 0:
             self.write_string("Undefined command {}\n".format(cmd_name))
@@ -245,15 +267,15 @@
 
     def default(self, line):
         self._close_output_file()
         try:
             return self._do_default(line)
         except KeyboardInterrupt:
             self.write_stdout("\n")
-        except Exception as e:
+        except BaseException as e:
             if self.debug:
                 secure_log_traceback()
             self.write_stdout(f"exception occurred: {secure_format_exception(e)}")
         self._close_output_file()
 
     def _do_default(self, line):
         args = split_to_args(line)
@@ -284,15 +306,15 @@
             if len(out_file_name) <= 0:
                 self.write_error("output file name must not be empty")
                 return
             args.pop(out_arg_idx)
             line = join_args(args)
             try:
                 out_file = open(out_file_name, "w")
-            except Exception as e:
+            except BaseException as e:
                 self.write_error(f"cannot open file {out_file_name}: {secure_format_exception(e)}")
                 return
 
             self._set_output_file(out_file, no_stdout)
 
         # check client command first
         info = self.api.check_command(line)
@@ -412,46 +434,50 @@
             self.stopped = True
             self.api.close()
 
     def _get_login_creds(self):
         if self.credential_type == CredentialType.PASSWORD:
             self.user_name = "admin"
             self.pwd = hash_password("admin")
+        elif self.credential_type == CredentialType.LOCAL_CERT:
+            self.user_name = self.username
         else:
             self.user_name = input("User Name: ")
 
     def print_resp(self, resp: dict):
         """Prints the server response
 
         Args:
             resp (dict): The server response.
         """
-        if "details" in resp:
-            if isinstance(resp["details"], str):
-                self.write_string(resp["details"])
-            if isinstance(resp["details"], Table):
-                self.write_table(resp["details"])
+        if ProtoKey.DETAILS in resp:
+            details = resp[ProtoKey.DETAILS]
+            if isinstance(details, str):
+                self.write_string(details)
+            elif isinstance(details, Table):
+                self.write_table(details)
 
-        if "data" in resp:
-            for item in resp["data"]:
+        if ProtoKey.DATA in resp:
+            for item in resp[ProtoKey.DATA]:
                 if not isinstance(item, dict):
                     continue
-                item_type = item.get("type")
-                if item_type == "string":
-                    self.write_string(item["data"])
-                elif item_type == "table":
+                item_type = item.get(ProtoKey.TYPE)
+                item_data = item.get(ProtoKey.DATA)
+                if item_type == ProtoKey.STRING:
+                    self.write_string(item_data)
+                elif item_type == ProtoKey.TABLE:
                     table = Table(None)
-                    table.set_rows(item["rows"])
+                    table.set_rows(item[ProtoKey.ROWS])
                     self.write_table(table)
-                elif item_type == "error":
-                    self.write_error(item["data"])
-                elif item_type == "dict":
-                    self.write_dict(item["data"])
+                elif item_type == ProtoKey.ERROR:
+                    self.write_error(item_data)
+                elif item_type == ProtoKey.DICT:
+                    self.write_dict(item_data)
 
-        if "details" not in resp and "data" not in resp:
+        if ProtoKey.DETAILS not in resp and ProtoKey.DATA not in resp:
             self.write_string("Response is not correct.")
 
     def write_stdout(self, data: str):
         self.stdout.write(data + "\n")
 
     def _write(self, content: str):
         if not self.no_stdout:
```

## nvflare/fuel/hci/client/fl_admin_api.py

```diff
@@ -93,24 +93,28 @@
     else:
         return False
 
 
 class FLAdminAPI(AdminAPI, FLAdminAPISpec):
     def __init__(
         self,
+        overseer_agent: OverseerAgent,
         ca_cert: str = "",
         client_cert: str = "",
         client_key: str = "",
         upload_dir: str = "",
         download_dir: str = "",
         cmd_modules: Optional[List] = None,
-        overseer_agent: OverseerAgent = None,
         user_name: str = None,
         poc=False,
         debug=False,
+        session_event_cb=None,
+        session_timeout_interval=None,
+        session_status_check_interval=None,
+        auto_login_max_tries: int = 5,
     ):
         """FLAdminAPI serves as foundation for communications to FL server through the AdminAPI.
 
         Upon initialization, FLAdminAPI will start the overseer agent to get the active server and then try to log in.
         This happens in a thread, so code that executes after should check that the FLAdminAPI is successfully logged in.
 
         Args:
@@ -120,32 +124,37 @@
             upload_dir: File transfer upload directory. Folders uploaded to the server to be deployed must be here. Folder must already exist and be accessible.
             download_dir: File transfer download directory. Can be same as upload_dir. Folder must already exist and be accessible.
             cmd_modules: command modules to load and register. Note that FileTransferModule is initialized here with upload_dir and download_dir if cmd_modules is None.
             overseer_agent: initialized OverseerAgent to obtain the primary service provider to set the host and port of the active server
             user_name: Username to authenticate with FL server
             poc: Whether to enable poc mode for using the proof of concept example without secure communication.
             debug: Whether to print debug messages. False by default.
+            session_event_cb: the session event callback
+            session_timeout_interval: if specified, automatically close the session after inactive for this long
+            session_status_check_interval: how often to check session status with server
+            auto_login_max_tries: maximum number of tries to auto-login.
         """
-        if overseer_agent:
-            service_finder = ServiceFinderByOverseer(overseer_agent)
-        else:
-            service_finder = None
+        service_finder = ServiceFinderByOverseer(overseer_agent)
 
         AdminAPI.__init__(
             self,
             ca_cert=ca_cert,
             client_cert=client_cert,
             client_key=client_key,
             upload_dir=upload_dir,
             download_dir=download_dir,
             cmd_modules=cmd_modules,
             service_finder=service_finder,
             user_name=user_name,
             poc=poc,
             debug=debug,
+            session_event_cb=session_event_cb,
+            session_timeout_interval=session_timeout_interval,
+            session_status_check_interval=session_status_check_interval,
+            auto_login_max_tries=auto_login_max_tries,
         )
         self.upload_dir = upload_dir
         self.download_dir = download_dir
         self._error_buffer = None
 
     def _process_targets_into_str(self, targets: List[str]) -> str:
         if not isinstance(targets, list):
@@ -878,15 +887,15 @@
                     met = callback(reply, **kwargs)
                     if met:
                         return FLAdminAPIResponse(APIStatus.SUCCESS, {}, None)
                     fail_attempts = 0
                 else:
                     print("Could not get reply from check status client, trying again later")
                     failed_attempts += 1
-            except Exception as e:
+            except BaseException as e:
                 print(f"Could not get clients stats, trying again later. Exception: {secure_format_exception(e)}")
                 failed_attempts += 1
 
             now = time.time()
             if timeout is not None:
                 if now - start >= timeout:
                     return FLAdminAPIResponse(APIStatus.SUCCESS, {"message": "Waited until timeout."}, None)
@@ -940,15 +949,15 @@
                     else:
                         print("Could not get reply from show stats server, trying again later")
                         failed_attempts += 1
                 except AttributeError:
                     # if attribute cannot be found, check if app is no longer running to return APIStatus.SUCCESS
                     if reply.get("details").get("message") == "App is not running":
                         return FLAdminAPIResponse(APIStatus.SUCCESS, {"message": "Waited until app not running."}, None)
-            except Exception as e:
+            except BaseException as e:
                 print(f"Could not get server stats, trying again later. Exception: {secure_format_exception(e)}")
                 failed_attempts += 1
 
             now = time.time()
             if timeout is not None:
                 if now - start >= timeout:
                     return FLAdminAPIResponse(APIStatus.SUCCESS, {"message": "Waited until timeout."}, None)
@@ -958,15 +967,7 @@
                     {
                         "message": "FL server stats was not obtainable for more than the specified number of "
                         "fail_attempts. "
                     },
                     None,
                 )
             time.sleep(interval)
-
-    def login(self, username: str):
-        result = AdminAPI.login(self, username=username)
-        return FLAdminAPIResponse(status=result["status"], details=result["details"])
-
-    def login_with_poc(self, username: str, poc_key: str):
-        result = AdminAPI.login_with_poc(self, username=username, poc_key=poc_key)
-        return FLAdminAPIResponse(status=result["status"], details=result["details"])
```

## nvflare/fuel/hci/client/overseer_service_finder.py

```diff
@@ -17,17 +17,16 @@
 from nvflare.ha.ha_admin_cmds import HACommandModule
 
 from .api_spec import ServiceFinder
 
 
 class ServiceFinderByOverseer(ServiceFinder):
     def __init__(self, overseer_agent: OverseerAgent):
-        assert isinstance(overseer_agent, OverseerAgent), "overseer_agent must be OverseerAgent but got {}".format(
-            type(overseer_agent)
-        )
+        if not isinstance(overseer_agent, OverseerAgent):
+            raise TypeError(f"overseer_agent must be OverseerAgent but got {type(overseer_agent)}")
 
         self.overseer_agent = overseer_agent
         self.sp_address_changed_cb = None
         self.host = ""
         self.port = 0
         self.ssid = ""
```

## nvflare/fuel/hci/client/static_service_finder.py

```diff
@@ -19,7 +19,10 @@
     def __init__(self, host: str, port: int):
         self.host = host
         self.port = port
         self.ssid = "1234"
 
     def start(self, service_address_changed_cb):
         service_address_changed_cb(self.host, self.port, self.ssid)
+
+    def stop(self):
+        pass
```

## nvflare/fuel/hci/server/constants.py

```diff
@@ -30,7 +30,8 @@
     UPLOAD_DIR = "_uploadDir"
     DOWNLOAD_DIR = "_downloadDir"
     DOWNLOAD_JOB_URL = "_downloadJobUrl"
 
     CMD_ENTRY = "_cmdEntry"
     JOB_DATA = "_jobData"
     JOB_META = "_jobMeta"
+    CMD_TIMEOUT = "_cmdTimeout"
```

## nvflare/fuel/hci/server/file_transfer.py

```diff
@@ -173,15 +173,15 @@
             unzip_all_from_bytes(data_bytes, tmp_dir)
             tmp_folder_path = os.path.join(tmp_dir, folder_name)
 
             if not os.path.isdir(tmp_folder_path):
                 conn.append_error("logic error: unzip failed to create folder {}".format(tmp_folder_path))
                 return False, None
             return True, None
-        except Exception as e:
+        except BaseException as e:
             secure_log_traceback()
             conn.append_error(f"exception occurred: {secure_format_exception(e)}")
             return False, None
         finally:
             shutil.rmtree(tmp_dir)
 
     def upload_folder(self, conn: Connection, args: List[str]):
```

## nvflare/fuel/hci/server/hci.py

```diff
@@ -14,15 +14,15 @@
 
 import logging
 import socketserver
 import ssl
 import threading
 
 from nvflare.fuel.hci.conn import Connection, receive_til_end
-from nvflare.fuel.hci.proto import validate_proto
+from nvflare.fuel.hci.proto import MetaKey, MetaStatusValue, ProtoKey, make_meta, validate_proto
 from nvflare.fuel.hci.security import IdentityKey, get_identity_info
 from nvflare.security.logging import secure_log_traceback
 
 from .constants import ConnProps
 from .reg import ServerCommandRegister
 
 logger = logging.getLogger(__name__)
@@ -50,39 +50,51 @@
                 identity = get_identity_info(self.request.getpeercert())
                 conn.set_prop(ConnProps.CLIENT_IDENTITY, identity)
                 valid = self.server.validate_client_cn(identity[IdentityKey.NAME])
             else:
                 valid = True
 
             if not valid:
-                conn.append_error("authentication error")
+                conn.append_error(
+                    "authentication error", meta=make_meta(MetaStatusValue.NOT_AUTHENTICATED, info="invalid credential")
+                )
             else:
                 req = receive_til_end(self.request).strip()
                 command = None
                 req_json = validate_proto(req)
                 conn.request = req_json
                 if req_json is not None:
-                    data = req_json["data"]
+                    meta = req_json.get(ProtoKey.META, None)
+                    if meta and isinstance(meta, dict):
+                        cmd_timeout = meta.get(MetaKey.CMD_TIMEOUT)
+                        if cmd_timeout:
+                            conn.set_prop(ConnProps.CMD_TIMEOUT, cmd_timeout)
+
+                    data = req_json[ProtoKey.DATA]
                     for item in data:
-                        it = item["type"]
-                        if it == "command":
-                            command = item["data"]
+                        it = item[ProtoKey.TYPE]
+                        if it == ProtoKey.COMMAND:
+                            command = item[ProtoKey.DATA]
                             break
 
                     if command is None:
-                        conn.append_error("protocol violation")
+                        conn.append_error(
+                            "protocol violation", meta=make_meta(MetaStatusValue.INTERNAL_ERROR, "protocol violation")
+                        )
                     else:
                         self.server.cmd_reg.process_command(conn, command)
                 else:
                     # not json encoded
-                    conn.append_error("protocol violation")
+                    conn.append_error(
+                        "protocol violation", meta=make_meta(MetaStatusValue.INTERNAL_ERROR, "protocol violation")
+                    )
 
             if not conn.ended:
                 conn.close()
-        except Exception:
+        except BaseException:
             secure_log_traceback()
 
 
 def initialize_hci():
     socketserver.TCPServer.allow_reuse_address = True
```

## nvflare/fuel/hci/server/login.py

```diff
@@ -133,15 +133,15 @@
         pwd = args[2]
 
         ok = self.authenticator.authenticate(user_name, pwd, CredentialType.PASSWORD)
         if not ok:
             conn.append_string("REJECT")
             return
 
-        session = self.session_mgr.create_session(user_name=user_name, user_org="global", user_role="super")
+        session = self.session_mgr.create_session(user_name=user_name, user_org="global", user_role="project_admin")
         conn.append_string("OK")
         conn.append_token(session.token)
 
     def handle_cert_login(self, conn: Connection, args: List[str]):
         if not self.authenticator:
             conn.append_string("OK")
             return
```

## nvflare/fuel/hci/server/reg.py

```diff
@@ -99,15 +99,15 @@
         if len(self.filters) > 0:
             for f in self.filters:
                 f.post_command(conn, args)
 
     def process_command(self, conn: Connection, command: str):
         try:
             self._do_command(conn, command)
-        except Exception as e:
+        except BaseException as e:
             secure_log_traceback()
             conn.append_error(f"Exception Occurred: {secure_format_exception(e)}")
 
     def close(self):
         if self.closed:
             return
```

## nvflare/fuel/hci/tools/admin.py

```diff
@@ -98,17 +98,18 @@
         prompt=admin_config.get("prompt", "> "),
         cmd_modules=modules,
         ca_cert=ca_cert,
         client_cert=client_cert,
         client_key=client_key,
         upload_dir=admin_config.get("upload_dir"),
         download_dir=admin_config.get("download_dir"),
-        credential_type=CredentialType.PASSWORD if admin_config.get("cred_type") == "password" else CredentialType.CERT,
+        credential_type=CredentialType(admin_config.get("cred_type", CredentialType.PASSWORD.value)),
         debug=args.with_debug,
         service_finder=service_finder,
+        username=admin_config.get("username", ""),
         # cli_history_size=args.cli_history_size,
     )
 
     client.run()
 
 
 if __name__ == "__main__":
```

## nvflare/fuel/utils/component_builder.py

```diff
@@ -69,15 +69,15 @@
         class_args = config_dict.get("args", dict())
         for k, v in class_args.items():
             if isinstance(v, dict) and self.is_class_config(v):
                 # try to replace the arg with a component
                 try:
                     t = self.build_component(v)
                     class_args[k] = t
-                except Exception as e:
+                except BaseException as e:
                     raise ValueError(f"failed to instantiate class: {secure_format_exception(e)} ")
 
         class_path = self.get_class_path(config_dict)
 
         # Handle the special case, if config pass in the class_attributes, use the user defined class attributes
         # parameters directly.
         if "class_attributes" in class_args:
```

## nvflare/fuel/utils/dict_utils.py

```diff
@@ -10,14 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import collections
 
+from .validation_utils import check_object_type
+
 
 def update(d, u):
     for k, v in u.items():
         if isinstance(v, collections.Mapping):
             d[k] = update(d.get(k, {}), v)
         else:
             d[k] = v
@@ -67,19 +69,16 @@
         An error message if any; empty str if success.
 
     .. note::
 
        The content of the to_dict is updated
 
     """
-    if not isinstance(to_dict, dict):
-        return f"to_dict must be dict but got {type(to_dict)}"
-
-    if not isinstance(from_dict, dict):
-        return f"from_dict must be dict but got {type(from_dict)}"
+    check_object_type("to_dict", to_dict, dict)
+    check_object_type("from_dict", from_dict, dict)
 
     for k, fv in from_dict.items():
         if k not in to_dict:
             to_dict[k] = fv
             continue
 
         tv = to_dict[k]
@@ -116,7 +115,70 @@
         if type(fv) != type(tv):
             return f"type conflict in element '{k}': {type(fv)} in from_dict but {type(tv)} in to_dict"
 
         if from_override_to:
             to_dict[k] = fv
 
     return ""
+
+
+def _update_component_dict(comp_list: list, target: dict) -> str:
+    for c in comp_list:
+        check_object_type("element in comp_list", c, dict)
+        cid = c.get("id", None)
+        if not cid:
+            return "missing 'id' from a component"
+        target[cid] = c
+    return ""
+
+
+def update_components(target_dict: dict, from_dict: dict) -> str:
+    """update components in target_dict with components from the from_dict.
+    If a component with the same ID exists in both target_dict and from_dict, the component in from_dict
+    will replace the one in target_dict.
+    If a component only exists in from_dict, it will be added to the component list of target_dict.
+    Args:
+        target_dict: the dict to be updated
+        from_dict: the dict that will be used to update the target_dict
+    Returns:
+    """
+    key_components = "components"
+
+    from_comp_list = from_dict.get(key_components, None)
+    if not from_comp_list:
+        # no components to update
+        return ""
+
+    check_object_type("from_comp_list", from_comp_list, list)
+
+    target_comp_list = target_dict.get(key_components, None)
+    if not target_comp_list:
+        target_dict[key_components] = from_comp_list
+        return ""
+
+    check_object_type("target_comp_list", target_comp_list, list)
+
+    from_comp_dict = {}
+    err = _update_component_dict(from_comp_list, from_comp_dict)
+    if err:
+        return f"error in from_dict: {err}"
+
+    target_comp_dict = {}
+    err = _update_component_dict(target_comp_list, target_comp_dict)
+    if err:
+        return f"error in target_dict: {err}"
+
+    # determine components in both
+    dups = []
+    for cid in target_comp_dict.keys():
+        if cid in from_comp_dict:
+            dups.append(cid)
+
+    for cid in dups:
+        # remove from target_comp_dict
+        target_comp_dict.pop(cid)
+
+    new_target_comp_list = list(target_comp_dict.values())
+    new_target_comp_list.extend(from_comp_list)
+
+    target_dict[key_components] = new_target_comp_list
+    return ""
```

## nvflare/fuel/utils/fsm.py

```diff
@@ -13,17 +13,19 @@
 # limitations under the License.
 
 from nvflare.security.logging import secure_format_exception
 
 
 class State(object):
     def __init__(self, name: str):
-        assert isinstance(name, str), "name must be str but got {}".format(type(name))
+        if not isinstance(name, str):
+            raise TypeError(f"name must be str but got {type(name)}")
         name = name.strip()
-        assert len(name) > 0, "name must not be empty"
+        if len(name) <= 0:
+            raise ValueError("name must not be empty")
         self.name = name
         self.fsm = None
 
     def execute(self, **kwargs):
         pass
 
     def leave(self):
@@ -47,47 +49,51 @@
     def set_prop(self, name, value):
         self.props[name] = value
 
     def get_prop(self, name, default=None):
         return self.props.get(name, default=default)
 
     def add_state(self, state: State):
-        assert isinstance(state, State), "state must be State but got {}".format(type(state))
-        s = self.states.get(state.name, None)
-        assert s is None, 'duplicate state "{}"'.format(state.name)
+        if not isinstance(state, State):
+            raise TypeError(f"state must be State but got {type(state)}")
+        if state.name in self.states:
+            raise RuntimeError(f"can't add duplicate state '{state.name}'")
         state.fsm = self
         self.states[state.name] = state
 
     def set_current_state(self, name: str):
         s = self.states.get(name)
-        assert s, 'unknown state "{}"'.format(name)
+        if s is None:
+            raise RuntimeError(f'FSM has no such state "{name}"')
         self.current_state = s
 
     def get_current_state(self):
         return self.current_state
 
     def execute(self, **kwargs) -> State:
         try:
             self.current_state = self._try_execute(**kwargs)
-        except Exception as e:
+        except BaseException as e:
             self.error = f"exception occurred in state execution: {secure_format_exception(e)}"
             self.current_state = None
         return self.current_state
 
     def _try_execute(self, **kwargs) -> State:
-        assert self.current_state, "FSM has no current state"
+        if self.current_state is None:
+            raise RuntimeError("FSM has no current state")
         next_state_name = self.current_state.execute(**kwargs)
         if next_state_name:
             if next_state_name == FSM.STATE_NAME_EXIT:
                 # go to the end
                 return None
 
             # enter next state
             next_state = self.states.get(next_state_name, None)
-            assert next_state, 'FSM has no such state "{}"'.format(next_state_name)
+            if next_state is None:
+                raise RuntimeError(f'FSM has no such state "{next_state_name}"')
 
             # leave current state
             self.current_state.leave()
 
             # enter the next state
             next_state.enter()
```

## nvflare/fuel/utils/json_scanner.py

```diff
@@ -92,15 +92,15 @@
         self.location = location
         self.data = json_data
         self.logger = logging.getLogger("JsonScanner")
 
     def _do_scan(self, node: Node):
         try:
             node.processor.process_element(node)
-        except Exception as e:
+        except BaseException as e:
             secure_log_traceback(self.logger)
 
             if self.location:
                 raise ConfigError(
                     "Error processing {} in JSON element {}: path: {}, exception: {}".format(
                         self.location, node.element, node.path(), secure_format_exception(e)
                     )
@@ -122,15 +122,15 @@
         elif isinstance(element, list):
             for i in range(len(element)):
                 self._do_scan(_child_node(node, node.key, i + 1, element[i]))
 
         if node.exit_cb is not None:
             try:
                 node.exit_cb(node)
-            except Exception as e:
+            except BaseException as e:
                 if self.location:
                     raise ConfigError(
                         "Error post-processing {} in JSON element: {}, exception: {}".format(
                             self.location, node.path(), secure_format_exception(e)
                         )
                     )
                 else:
```

## nvflare/ha/ha_admin_cmds.py

```diff
@@ -15,15 +15,15 @@
 import json
 import logging
 
 from nvflare.apis.fl_constant import AdminCommandNames
 from nvflare.apis.overseer_spec import OverseerAgent
 from nvflare.fuel.hci.client.api_spec import CommandContext
 from nvflare.fuel.hci.client.api_status import APIStatus
-from nvflare.fuel.hci.proto import MetaStatusValue
+from nvflare.fuel.hci.proto import MetaStatusValue, ProtoKey, make_meta
 from nvflare.fuel.hci.reg import CommandModule, CommandModuleSpec, CommandSpec
 from nvflare.security.logging import secure_format_exception
 
 
 class HACommandModule(CommandModule):
     """Command module with commands for management in relation to the high availability framework."""
 
@@ -66,64 +66,73 @@
         """Lists service provider information based on the last heartbeat from the overseer.
 
         Details are used for displaying the response in the CLI, and data is the data in a dict that is provided in FLAdminAPI.
 
         """
         overseer_agent = self.overseer_agent
         return {
-            "status": APIStatus.SUCCESS,
-            "details": str(overseer_agent.overseer_info),
-            "data": overseer_agent.overseer_info,
+            ProtoKey.STATUS: APIStatus.SUCCESS,
+            ProtoKey.DETAILS: str(overseer_agent.overseer_info),
+            ProtoKey.DATA: overseer_agent.overseer_info,
         }
 
     def get_active_sp(self, args, ctx: CommandContext):
         overseer_agent = self.overseer_agent
-        return {"status": APIStatus.SUCCESS, "details": str(overseer_agent.get_primary_sp())}
+        sp = overseer_agent.get_primary_sp()
+        return {ProtoKey.STATUS: APIStatus.SUCCESS, ProtoKey.DETAILS: str(sp), ProtoKey.META: sp.__dict__}
 
     def promote_sp(self, args, ctx: CommandContext):
         overseer_agent = self.overseer_agent
         if len(args) != 2:
-            return {"status": APIStatus.ERROR_SYNTAX, "details": "usage: promote_sp example1.com:8002:8003"}
+            return {
+                ProtoKey.STATUS: APIStatus.ERROR_SYNTAX,
+                ProtoKey.DETAILS: "usage: promote_sp example1.com:8002:8003",
+                ProtoKey.META: make_meta(MetaStatusValue.SYNTAX_ERROR),
+            }
 
         sp_end_point = args[1]
         resp = overseer_agent.promote_sp(sp_end_point)
-        if json.loads(resp.text).get("Error"):
+        err = json.loads(resp.text).get("Error")
+        if err:
             return {
-                "status": APIStatus.ERROR_RUNTIME,
-                "details": "Error: {}".format(json.loads(resp.text).get("Error")),
+                ProtoKey.STATUS: APIStatus.ERROR_RUNTIME,
+                ProtoKey.DETAILS: f"Error: {err}",
+                ProtoKey.META: make_meta(MetaStatusValue.INTERNAL_ERROR, err),
             }
         else:
+            info = f"Promoted endpoint: {sp_end_point}. Synchronizing with overseer..."
             return {
-                "status": APIStatus.SUCCESS,
-                "details": "Promoted endpoint: {}. Synchronizing with overseer...".format(sp_end_point),
+                ProtoKey.STATUS: APIStatus.SUCCESS,
+                ProtoKey.DETAILS: info,
+                ProtoKey.META: make_meta(MetaStatusValue.OK, info),
             }
 
     def shutdown_system(self, args, ctx: CommandContext):
         api = ctx.get_api()
         overseer_agent = self.overseer_agent
         try:
-            admin_status_result = api.do_command(AdminCommandNames.ADMIN_CHECK_STATUS)
-            if admin_status_result.get("meta").get("status") == MetaStatusValue.NOT_AUTHORIZED:
+            admin_status_result = api.do_command(AdminCommandNames.ADMIN_CHECK_STATUS + " server")
+            if admin_status_result.get(ProtoKey.META).get(ProtoKey.STATUS) == MetaStatusValue.NOT_AUTHORIZED:
                 return {
-                    "status": APIStatus.ERROR_AUTHORIZATION,
-                    "details": "Error: Not authorized for this command.",
+                    ProtoKey.STATUS: APIStatus.ERROR_AUTHORIZATION,
+                    ProtoKey.DETAILS: "Error: Not authorized for this command.",
                 }
-            status = admin_status_result.get("data")
-            if status[0].get("data") != "Engine status: stopped":
+            status = admin_status_result.get(ProtoKey.DATA)
+            if status[0].get(ProtoKey.DATA) != "Engine status: stopped":
                 return {
-                    "status": APIStatus.ERROR_RUNTIME,
-                    "details": "Error: There are still jobs running. Please let them finish or abort_job before attempting shutdown.",
+                    ProtoKey.STATUS: APIStatus.ERROR_RUNTIME,
+                    ProtoKey.DETAILS: "Error: There are still jobs running. Please let them finish or abort_job before attempting shutdown.",
                 }
         except Exception as e:
             return {
-                "status": APIStatus.ERROR_RUNTIME,
-                "details": f"Error getting server status to make sure all jobs are stopped before shutting down system: {secure_format_exception(e)}",
+                ProtoKey.STATUS: APIStatus.ERROR_RUNTIME,
+                ProtoKey.DETAILS: f"Error getting server status to make sure all jobs are stopped before shutting down system: {secure_format_exception(e)}",
             }
-        print("Shutting down the system...")
+        # print("Shutting down the system...")
         resp = overseer_agent.set_state("shutdown")
         if json.loads(resp.text).get("Error"):
             return {
-                "status": APIStatus.ERROR_RUNTIME,
-                "details": "Error: {}".format(json.loads(resp.text).get("Error")),
+                ProtoKey.STATUS: APIStatus.ERROR_RUNTIME,
+                ProtoKey.DETAILS: "Error: {}".format(json.loads(resp.text).get("Error")),
             }
         else:
-            return {"status": APIStatus.SUCCESS, "details": "Set state to shutdown in overseer."}
+            return {ProtoKey.STATUS: APIStatus.SUCCESS, ProtoKey.DETAILS: "Set state to shutdown in overseer."}
```

## nvflare/ha/overseer/overseer.py

```diff
@@ -27,15 +27,15 @@
     simple_PSP_policy,
     update_sp_state,
 )
 
 heartbeat_timeout = os.environ.get("NVFL_OVERSEER_HEARTBEAT_TIMEOUT", "10")
 try:
     heartbeat_timeout = int(heartbeat_timeout)
-except Exception:
+except BaseException:
     heartbeat_timeout = 10
 
 
 @app.route("/api/v1/heartbeat", methods=["GET", "POST"])
 def heartbeat():
     if request.method == "POST":
         req = request.json
```

## nvflare/lighter/dummy_project.yml

```diff
@@ -27,14 +27,17 @@
       template_file: master_template.yml
   - path: nvflare.lighter.impl.template.TemplateBuilder
   - path: nvflare.lighter.impl.static_file.StaticFileBuilder
     args:
       # config_folder can be set to inform NVIDIA FLARE where to get configuration
       config_folder: config
 
+      # scheme for communication driver (currently supporting the default, grpc, only).
+      # scheme: grpc
+
       # app_validator is used to verify if uploaded app has proper structures
       # if not set, no app_validator is included in fed_server.json
       # app_validator: PATH_TO_YOUR_OWN_APP_VALIDATOR
 
       # when docker_image is set to a docker image name, docker.sh will be generated on server/client/admin
       # docker_image:
```

## nvflare/lighter/ha_project.yml

```diff
@@ -46,14 +46,17 @@
     args:
       docker_image: localhost:32000/nvfl-min:0.0.1
   - path: nvflare.lighter.impl.static_file.StaticFileBuilder
     args:
       # config_folder can be set to inform NVIDIA FLARE where to get configuration
       config_folder: config
 
+      # scheme for communication driver (currently supporting the default, grpc, only).
+      # scheme: grpc
+      
       # app_validator is used to verify if uploaded app has proper structures
       # if not set, no app_validator is included in fed_server.json
       # app_validator: PATH_TO_YOUR_OWN_APP_VALIDATOR
 
       # when docker_image is set to a docker image name, docker.sh will be generated on server/client/admin
       # docker_image:
```

## nvflare/lighter/poc.py

```diff
@@ -45,15 +45,15 @@
     except shutil.ReadError:
         return False
 
 
 def copy_from_src(src_poc_folder, dest_poc_folder):
     try:
         shutil.copytree(src_poc_folder, dest_poc_folder)
-    except Exception as e:
+    except BaseException as e:
         print(f"Unable to copy poc folder from {src_poc_folder}, Exit. {e} ")
         exit(1)
 
 
 def clone_poc_folder(src_poc_folder, dest_poc_folder):
     shutil.rmtree(dest_poc_folder, ignore_errors=True)
     success = unpack_poc(dest_poc_folder)
@@ -61,15 +61,15 @@
         copy_from_src(src_poc_folder, dest_poc_folder)
 
     for root, dirs, files in os.walk(dest_poc_folder):
         for dir in dirs:
             if dir == "admin":
                 try:
                     os.mkdir(os.path.join(root, dir, "local"))
-                except Exception:
+                except BaseException:
                     pass
                 break
         for file in files:
             if file.endswith(".sh"):
                 os.chmod(os.path.join(root, file), 0o755)
```

## nvflare/lighter/poc_commands.py

```diff
@@ -7,31 +7,37 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 import json
 import os
 import random
+import shutil
+import socket
 import subprocess
 import sys
 import time
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, OrderedDict, Tuple
+
+import yaml
 
 from nvflare.cli_exception import CLIException
+from nvflare.fuel.utils.class_utils import instantiate_class
 from nvflare.fuel.utils.gpu_utils import get_host_gpu_ids
-from nvflare.lighter.poc import generate_poc
+from nvflare.lighter.provision import gen_default_project_config, prepare_project
 from nvflare.lighter.service_constants import FlareServiceConstants as SC
-from nvflare.lighter.utils import update_storage_locations
+from nvflare.lighter.spec import Provisioner
+from nvflare.lighter.utils import load_yaml, update_project_server_name_config, update_storage_locations
 from nvflare.tool.api_utils import shutdown_system
 
 DEFAULT_WORKSPACE = "/tmp/nvflare/poc"
+DEFAULT_PROJECT_NAME = "example_project"
 
 
 def client_gpu_assignments(clients: List[str], gpu_ids: List[int]) -> Dict[str, List[int]]:
     n_gpus = len(gpu_ids)
     n_clients = len(clients)
     gpu_assignments = {}
     if n_gpus == 0:
@@ -52,116 +58,432 @@
             client = client_name_map[client_id]
             if client not in gpu_assignments:
                 gpu_assignments[client] = []
             gpu_assignments[client].append(gpu_ids[gpu_index])
     return gpu_assignments
 
 
-def get_package_command(cmd_type: str, poc_workspace: str, package_dir) -> str:
+def get_service_command(cmd_type: str, prod_dir: str, service_dir, service_config: Dict) -> str:
+    cmd = ""
+    admin_dir_name = service_config.get(SC.FLARE_PROJ_ADMIN, SC.FLARE_PROJ_ADMIN)
     if cmd_type == SC.CMD_START:
-        if package_dir == SC.FLARE_CONSOLE:
-            cmd = get_cmd_path(poc_workspace, package_dir, "fl_admin.sh")
-        elif package_dir == SC.FLARE_SERVER:
-            cmd = get_cmd_path(poc_workspace, package_dir, "start.sh")
+        if not service_config.get(SC.IS_DOCKER_RUN):
+            if service_dir == admin_dir_name:
+                cmd = get_cmd_path(prod_dir, service_dir, "fl_admin.sh")
+            else:
+                cmd = get_cmd_path(prod_dir, service_dir, "start.sh")
         else:
-            cmd = get_cmd_path(poc_workspace, package_dir, "start.sh")
+            if service_dir == admin_dir_name:
+                cmd = get_cmd_path(prod_dir, service_dir, "fl_admin.sh")
+            else:
+                cmd = get_cmd_path(prod_dir, service_dir, "docker.sh -d")
 
     elif cmd_type == SC.CMD_STOP:
-        cmd = get_stop_cmd(poc_workspace, package_dir)
+        if not service_config.get(SC.IS_DOCKER_RUN):
+            cmd = get_stop_cmd(prod_dir, service_dir)
+        else:
+            if service_dir == admin_dir_name:
+                cmd = get_stop_cmd(prod_dir, service_dir)
+            else:
+                cmd = f"docker stop {service_dir}"
+
     else:
-        raise ValueError("unknown cmd_type :", cmd_type)
+        raise CLIException("unknown cmd_type :", cmd_type)
     return cmd
 
 
 def get_stop_cmd(poc_workspace: str, service_dir_name: str):
     service_dir = os.path.join(poc_workspace, service_dir_name)
     stop_file = os.path.join(service_dir, "shutdown.fl")
     return f"touch {stop_file}"
 
 
-def get_nvflare_home() -> str:
-    nvflare_home = os.getenv("NVFLARE_HOME")
-    if nvflare_home:
-        if nvflare_home.endswith("/"):
-            nvflare_home = nvflare_home[:-1]
+def get_nvflare_home() -> Optional[str]:
+    nvflare_home = None
+    if "NVFLARE_HOME" in os.environ:
+        nvflare_home = os.getenv("NVFLARE_HOME")
+        if nvflare_home:
+            if nvflare_home.endswith("/"):
+                nvflare_home = nvflare_home[:-1]
     return nvflare_home
 
 
-def get_upload_dir(poc_workspace: str) -> str:
-    console_config_path = os.path.join(poc_workspace, f"{SC.FLARE_CONSOLE}/{SC.STARTUP}/fed_admin.json")
+def get_upload_dir(startup_dir) -> str:
+    console_config_path = os.path.join(startup_dir, "fed_admin.json")
     try:
         with open(console_config_path, "r") as f:
             console_config = json.load(f)
-            upload_dir = console_config[SC.FLARE_CONSOLE]["upload_dir"]
+            upload_dir = console_config["admin"]["upload_dir"]
     except IOError as e:
         raise CLIException(f"failed to load {console_config_path} {e}")
     except json.decoder.JSONDecodeError as e:
         raise CLIException(f"failed to load {console_config_path}, please double check the configuration {e}")
-
     return upload_dir
 
 
-def prepare_examples(poc_workspace: str):
-    nvflare_home = get_nvflare_home()
-    if nvflare_home:
-        src = os.path.join(nvflare_home, SC.EXAMPLES)
-        dst = os.path.join(poc_workspace, f"{SC.FLARE_CONSOLE}/{get_upload_dir(poc_workspace)}")
+def is_dir_empty(path: str):
+    targe_dir = os.listdir(path)
+    return len(targe_dir) == 0
+
+
+def prepare_examples(example_dir: str, workspace: str, config_packages: Optional[Tuple] = None):
+    _, service_config = config_packages if config_packages else setup_service_config(workspace)
+    if example_dir is None or example_dir == "":
+        raise CLIException("example_dir is required")
+    src = os.path.abspath(example_dir)
+    if not os.path.isdir(src):
+        raise CLIException(f"example_dir '{example_dir}' is not valid directory")
+
+    prod_dir = get_prod_dir(workspace)
+    if not os.path.exists(prod_dir):
+        raise CLIException("please use nvflare poc --prepare to create workspace first")
+
+    console_dir = os.path.join(prod_dir, f"{service_config[SC.FLARE_PROJ_ADMIN]}")
+    startup_dir = os.path.join(console_dir, SC.STARTUP)
+    transfer = get_upload_dir(startup_dir)
+    dst = os.path.join(console_dir, transfer)
+    if not is_dir_empty(dst):
+        print(" ")
+        answer = input(f"Examples at {dst} is already exists, replace with new one ? (y/N) ")
+        if answer.strip().upper() == "Y":
+            if os.path.islink(dst):
+                os.unlink(dst)
+            if os.path.isdir(dst):
+                shutil.rmtree(dst, ignore_errors=True)
+
+            print(f"link examples from {src} to {dst}")
+            os.symlink(src, dst)
+    else:
+        if os.path.isdir(dst):
+            shutil.rmtree(dst, ignore_errors=True)
         print(f"link examples from {src} to {dst}")
         os.symlink(src, dst)
 
 
-def prepare_poc(number_of_clients: int, poc_workspace: str):
-    print(f"prepare_poc at {poc_workspace} for {number_of_clients} clients")
-    ret_code = generate_poc(number_of_clients, poc_workspace)
-    if poc_workspace != DEFAULT_WORKSPACE:
+def get_prod_dir(workspace, project_name: str = DEFAULT_PROJECT_NAME):
+    prod_dir = os.path.join(workspace, project_name, "prod_00")
+    return prod_dir
+
+
+def gen_project_config_file(workspace: str) -> str:
+    project_file = os.path.join(workspace, "project.yml")
+    if not os.path.isfile(project_file):
+        gen_default_project_config("dummy_project.yml", project_file)
+    return project_file
+
+
+def verify_host(host_name: str) -> bool:
+    try:
+        host_name = socket.gethostbyname(host_name)
+        return True
+    except:
+        return False
+
+
+def verify_hosts(project_config: OrderedDict):
+    hosts: List[str] = get_project_hosts(project_config)
+    for h in hosts:
+        if not verify_host(h):
+            print(f"host name: '{h}' is not defined, considering modify /etc/hosts to add localhost alias")
+            exit(0)
+
+
+def get_project_hosts(project_config) -> List[str]:
+    participants: List[dict] = project_config["participants"]
+    return [p["name"] for p in participants if p["type"] == "client" or p["type"] == "server"]
+
+
+def get_fl_server_name(project_config: OrderedDict) -> str:
+    participants: List[dict] = project_config["participants"]
+    servers = [p["name"] for p in participants if p["type"] == "server"]
+    if len(servers) == 1:
+        return servers[0]
+    else:
+        raise CLIException(f"project should only have one server, but {len(servers)} are provided: {servers}")
+
+
+def get_proj_admin(project_config: OrderedDict):
+    participants: List[dict] = project_config["participants"]
+    admins = [p["name"] for p in participants if p["type"] == "admin"]
+
+    if len(admins) == 1:
+        return admins[0]
+    else:
+        raise CLIException(f"project should only have only one project admin, but {len(admins)} are provided: {admins}")
+
+
+def get_fl_client_names(project_config: OrderedDict) -> List[str]:
+    participants: List[dict] = project_config["participants"]
+    client_names = [p["name"] for p in participants if p["type"] == "client"]
+    return client_names
+
+
+def prepare_builders(project_dict: OrderedDict) -> List:
+    builders = list()
+    admin_name = [p["name"] for p in project_dict["participants"] if p["type"] == "admin"][0]
+    for b in project_dict.get("builders"):
+        path = b.get("path")
+        args = b.get("args")
+
+        if b.get("path") == "nvflare.lighter.impl.static_file.StaticFileBuilder":
+            path = "nvflare.lighter.impl.local_static_file.LocalStaticFileBuilder"
+            args["overseer_agent"]["args"]["sp_end_point"] = "localhost:8002:8003"
+            args["username"] = admin_name
+
+        elif b.get("path") == "nvflare.lighter.impl.cert.CertBuilder":
+            path = "nvflare.lighter.impl.local_cert.LocalCertBuilder"
+
+        builders.append(instantiate_class(path, args))
+    return builders
+
+
+def local_provision(
+    clients: List[str],
+    number_of_clients: int,
+    workspace: str,
+    docker_image: str,
+    use_he: bool = False,
+    project_conf_path: str = "",
+) -> Tuple:
+    user_provided_project_config = False
+    if project_conf_path:
+        src_project_file = project_conf_path
+        dst_project_file = os.path.join(workspace, "project.yml")
+        user_provided_project_config = True
+    else:
+        src_project_file = gen_project_config_file(workspace)
+        dst_project_file = src_project_file
+
+    print(f"provision at {workspace} for {number_of_clients} clients with {src_project_file}")
+    project_config: OrderedDict = load_yaml(src_project_file)
+    if not project_config:
+        raise CLIException(f"empty or invalid project config from project yaml file: {src_project_file}")
+
+    if not user_provided_project_config:
+        project_config = update_server_name(project_config)
+        project_config = update_clients(clients, number_of_clients, project_config)
+        project_config = add_he_builder(use_he, project_config)
+        if docker_image:
+            project_config = update_static_file_builder(docker_image, project_config)
+    save_project_config(project_config, dst_project_file)
+    service_config = get_service_config(project_config)
+    project = prepare_project(project_config)
+    builders = prepare_builders(project_config)
+    provisioner = Provisioner(workspace, builders)
+    provisioner.provision(project)
+
+    return project_config, service_config
+
+
+def get_service_config(project_config):
+    service_config = {
+        SC.FLARE_SERVER: get_fl_server_name(project_config),
+        SC.FLARE_PROJ_ADMIN: get_proj_admin(project_config),
+        SC.FLARE_CLIENTS: get_fl_client_names(project_config),
+        SC.IS_DOCKER_RUN: is_docker_run(project_config),
+    }
+    return service_config
+
+
+def save_project_config(project_config, project_file):
+    with open(project_file, "w") as file:
+        yaml.dump(project_config, file)
+
+
+def update_server_name(project_config):
+    old_server_name = get_fl_server_name(project_config)
+    server_name = "server"
+    if old_server_name != server_name:
+        update_project_server_name_config(project_config, old_server_name, server_name)
+    return project_config
+
+
+def is_docker_run(project_config: OrderedDict):
+    if "builders" not in project_config:
+        return False
+    static_builder = [
+        b
+        for b in project_config.get("builders")
+        if b.get("path") == "nvflare.lighter.impl.static_file.StaticFileBuilder"
+    ][0]
+    return "docker_image" in static_builder["args"]
+
+
+def update_static_file_builder(docker_image: str, project_config: OrderedDict):
+    # need to keep the order of the builders
+    for b in project_config.get("builders"):
+        if b.get("path") == "nvflare.lighter.impl.static_file.StaticFileBuilder":
+            b["args"]["docker_image"] = docker_image
+
+    return project_config
+
+
+def add_docker_builder(use_docker: bool, project_config: OrderedDict):
+    if use_docker:
+        docker_builder = {
+            "path": "nvflare.lighter.impl.docker.DockerBuilder",
+            "args": {"base_image": "python:3.8", "requirements_file": "requirements.txt"},
+        }
+        project_config["builders"].append(docker_builder)
+
+    return project_config
+
+
+def add_he_builder(use_he: bool, project_config: OrderedDict):
+    if use_he:
+        he_builder = {
+            "path": "nvflare.lighter.impl.he.HEBuilder",
+            "args": {},
+        }
+        project_config["builders"].append(he_builder)
+
+    return project_config
+
+
+def update_clients(clients: List[str], n_clients: int, project_config: OrderedDict) -> OrderedDict:
+    requested_clients = prepare_clients(clients, n_clients)
+
+    participants: List[dict] = project_config["participants"]
+    new_participants = [p for p in participants if p["type"] != "client"]
+
+    for client in requested_clients:
+        client_dict = {"name": client, "type": "client", "org": "nvidia"}
+        new_participants.append(client_dict)
+
+    project_config["participants"] = new_participants
+
+    return project_config
+
+
+def prepare_clients(clients, number_of_clients):
+    if not clients:
+        clients = []
+        for i in range(number_of_clients):
+            clients.append(f"site-{(i + 1)}")
+
+    return clients
+
+
+def prepare_poc(
+    clients: List[str],
+    number_of_clients: int,
+    workspace: str,
+    docker_image: str,
+    use_he: bool,
+    project_conf_path: str = "",
+    examples_dir: Optional[str] = None,
+) -> bool:
+    if clients:
+        number_of_clients = len(clients)
+    if not project_conf_path:
+        print(f"prepare poc at {workspace} for {number_of_clients} clients")
+    else:
+        print(f"prepare poc at {workspace} with {project_conf_path}")
+
+    if os.path.exists(workspace):
+        answer = input(
+            f"This will delete poc folder in {workspace} directory and create a new one. Is it OK to proceed? (y/N) "
+        )
+        if answer.strip().upper() == "Y":
+            from pathlib import Path
+
+            workspace_path = Path(workspace)
+            project_file = Path(project_conf_path)
+            if workspace_path in project_file.parents:
+                raise CLIException(
+                    f"\nProject file: '{project_conf_path}' is under workspace directory:"
+                    f"'{workspace}', which is to be deleted. "
+                    f"Please copy {project_conf_path} to different location before running this command."
+                )
+
+            shutil.rmtree(workspace, ignore_errors=True)
+            prepare_poc_provision(
+                clients, number_of_clients, workspace, docker_image, use_he, project_conf_path, examples_dir
+            )
+            return True
+        else:
+            return False
+    else:
+        prepare_poc_provision(
+            clients, number_of_clients, workspace, docker_image, use_he, project_conf_path, examples_dir
+        )
+        return True
+
+
+def prepare_poc_provision(
+    clients: List[str],
+    number_of_clients: int,
+    workspace: str,
+    docker_image: str,
+    use_he: bool = False,
+    project_conf_path: str = "",
+    examples_dir: Optional[str] = None,
+):
+    os.makedirs(workspace, exist_ok=True)
+    os.makedirs(os.path.join(workspace, "data"), exist_ok=True)
+    _, service_config = local_provision(clients, number_of_clients, workspace, docker_image, use_he, project_conf_path)
+    server_name = service_config[SC.FLARE_SERVER]
+    # update storage
+    if workspace != DEFAULT_WORKSPACE:
         update_storage_locations(
-            local_dir=f"{poc_workspace}/server/local", default_resource_name="resources.json", workspace=poc_workspace
+            local_dir=f"{workspace}/{server_name}/local", default_resource_name="resources.json", workspace=workspace
         )
-    if ret_code:
-        prepare_examples(poc_workspace)
+    examples_dir = get_examples_dir(examples_dir)
+    if examples_dir is not None:
+        prepare_examples(examples_dir, workspace, None)
 
 
-def sort_package_cmds(cmd_type, package_cmds: list) -> list:
+def get_examples_dir(examples_dir):
+    if examples_dir:
+        return examples_dir
+
+    nvflare_home = get_nvflare_home()
+    default_examples_dir = os.path.join(nvflare_home, "examples") if nvflare_home else None
+    return default_examples_dir
+
+
+def sort_service_cmds(cmd_type, service_cmds: list, service_config) -> list:
     def sort_first(val):
         return val[0]
 
-    order_packages = []
-    for package_name, cmd_path in package_cmds:
-        if package_name == SC.FLARE_SERVER:
-            order_packages.append((0, package_name, cmd_path))
-        elif package_name == SC.FLARE_CONSOLE:
-            order_packages.append((sys.maxsize, package_name, cmd_path))
+    order_services = []
+    for service_name, cmd_path in service_cmds:
+        if service_name == service_config[SC.FLARE_SERVER]:
+            order_services.append((0, service_name, cmd_path))
+        elif service_name == service_config[SC.FLARE_PROJ_ADMIN]:
+            order_services.append((sys.maxsize, service_name, cmd_path))
         else:
-            if len(package_cmds) == 1:
-                order_packages.append((0, package_name, cmd_path))
+            if len(service_cmds) == 1:
+                order_services.append((0, service_name, cmd_path))
             else:
-                order_packages.append((random.randint(2, len(package_cmds)), package_name, cmd_path))
+                order_services.append((random.randint(2, len(service_cmds)), service_name, cmd_path))
 
-    order_packages.sort(key=sort_first)
+    order_services.sort(key=sort_first)
     if cmd_type == SC.CMD_STOP:
-        order_packages.reverse()
-    return [(package_name, cmd_path) for n, package_name, cmd_path in order_packages]
+        order_services.reverse()
+    return [(service_name, cmd_path) for n, service_name, cmd_path in order_services]
 
 
 def get_cmd_path(poc_workspace, service_name, cmd):
     service_dir = os.path.join(poc_workspace, service_name)
     bin_dir = os.path.join(service_dir, SC.STARTUP)
     cmd_path = os.path.join(bin_dir, cmd)
     return cmd_path
 
 
-def is_poc_ready(poc_workspace: str):
+def is_poc_ready(poc_workspace: str, service_config):
     # check server and admin directories exist
-    console_dir = os.path.join(poc_workspace, SC.FLARE_CONSOLE)
-    server_dir = os.path.join(poc_workspace, SC.FLARE_SERVER)
+    prod_dir = get_prod_dir(poc_workspace)
+    console_dir = os.path.join(prod_dir, service_config[SC.FLARE_PROJ_ADMIN])
+    server_dir = os.path.join(prod_dir, service_config[SC.FLARE_SERVER])
     return os.path.isdir(server_dir) and os.path.isdir(console_dir)
 
 
-def validate_poc_workspace(poc_workspace: str):
-    if not is_poc_ready(poc_workspace):
+def validate_poc_workspace(poc_workspace: str, service_config):
+    if not is_poc_ready(poc_workspace, service_config):
         raise CLIException(f"workspace {poc_workspace} is not ready, please use poc --prepare to prepare poc workspace")
 
 
 def validate_gpu_ids(gpu_ids: list, host_gpu_ids: list):
     for gpu_id in gpu_ids:
         if gpu_id not in host_gpu_ids:
             raise CLIException(
@@ -175,208 +497,343 @@
     else:
         gpu_ids = user_input_gpu_ids
         validate_gpu_ids(gpu_ids, host_gpu_ids)
     return gpu_ids
 
 
 def start_poc(poc_workspace: str, gpu_ids: List[int], excluded=None, white_list=None):
+    project_config, service_config = setup_service_config(poc_workspace)
     if white_list is None:
         white_list = []
     if excluded is None:
         excluded = []
     print(f"start_poc at {poc_workspace}, gpu_ids={gpu_ids}, excluded = {excluded}, white_list={white_list}")
-    validate_poc_workspace(poc_workspace)
-    _run_poc(SC.CMD_START, poc_workspace, gpu_ids, excluded=excluded, white_list=white_list)
+    validate_services(project_config, white_list, excluded)
+    validate_poc_workspace(poc_workspace, service_config)
+    _run_poc(SC.CMD_START, poc_workspace, gpu_ids, service_config, excluded=excluded, white_list=white_list)
+
+
+def validate_services(project_config, white_list: List, excluded: List):
+    participant_names = [p["name"] for p in project_config["participants"]]
+    validate_participants(participant_names, white_list)
+    validate_participants(participant_names, excluded)
+
+
+def validate_participants(participant_names, list_participants):
+    for p in list_participants:
+        if p not in participant_names:
+            print(f"participant '{p}' is not defined, expecting one of followings: {participant_names}")
+            exit(1)
+
+
+def setup_service_config(poc_workspace) -> Tuple:
+    project_file = os.path.join(poc_workspace, "project.yml")
+    if os.path.isfile(project_file):
+        project_config = load_yaml(project_file)
+        service_config = get_service_config(project_config) if project_config else None
+        return project_config, service_config
+    else:
+        raise CLIException(f"{project_file} is missing, make sure you have first run 'nvflare poc --prepare'")
 
 
 def stop_poc(poc_workspace: str, excluded=None, white_list=None):
+    project_config, service_config = setup_service_config(poc_workspace)
+
     if white_list is None:
         white_list = []
     if excluded is None:
-        excluded = [SC.FLARE_CONSOLE]
+        excluded = [service_config[SC.FLARE_PROJ_ADMIN]]
     else:
-        excluded.append(SC.FLARE_CONSOLE)
+        excluded.append(service_config[SC.FLARE_PROJ_ADMIN])
 
-    print("start shutdown NVFLARE")
-    validate_poc_workspace(poc_workspace)
+    validate_services(project_config, white_list, excluded)
+
+    validate_poc_workspace(poc_workspace, service_config)
     gpu_ids: List[int] = []
-    shutdown_system(poc_workspace)
-    _run_poc(SC.CMD_STOP, poc_workspace, gpu_ids, excluded=excluded, white_list=white_list)
+    prod_dir = get_prod_dir(poc_workspace)
+
+    p_size = len(white_list)
+    if p_size == 0 or service_config[SC.FLARE_SERVER] in white_list:
+        print("start shutdown NVFLARE")
+        shutdown_system(prod_dir, username=service_config[SC.FLARE_PROJ_ADMIN])
+    else:
+        print(f"start shutdown {white_list}")
 
+    _run_poc(SC.CMD_STOP, poc_workspace, gpu_ids, service_config, excluded=excluded, white_list=white_list)
 
-def _get_clients(package_commands: list) -> List[str]:
+
+def _get_clients(service_commands: list, service_config) -> List[str]:
     clients = [
-        package_dir_name
-        for package_dir_name, _ in package_commands
-        if package_dir_name != SC.FLARE_CONSOLE and package_dir_name != SC.FLARE_SERVER
+        service_dir_name
+        for service_dir_name, _ in service_commands
+        if service_dir_name != service_config[SC.FLARE_PROJ_ADMIN]
+        and service_dir_name != service_config[SC.FLARE_SERVER]
     ]
     return clients
 
 
-def _build_commands(cmd_type: str, poc_workspace: str, excluded: list, white_list=None) -> list:
+def _build_commands(cmd_type: str, poc_workspace: str, service_config, excluded: list, white_list=None) -> list:
     """
     :param cmd_type: start/stop
     :param poc_workspace:  poc workspace directory path
-    :param excluded: excluded package namae
-    :param white_list: whitelist, package name. If empty, include every package
+    :param service_config:  service_config
+    :param excluded: excluded service/participants name
+    :param white_list: whitelist, service name. If empty, include every service/participants
     :return:
     """
 
-    def is_fl_package_dir(p_dir_name: str) -> bool:
-        return p_dir_name == "admin" or p_dir_name == "server" or p_dir_name.startswith("site-")
+    def is_fl_service_dir(p_dir_name: str) -> bool:
+        fl_service = (
+            p_dir_name == service_config[SC.FLARE_PROJ_ADMIN]
+            or p_dir_name == service_config[SC.FLARE_SERVER]
+            or p_dir_name in service_config[SC.FLARE_CLIENTS]
+        )
+        return fl_service
+
+    prod_dir = get_prod_dir(poc_workspace)
 
     if white_list is None:
         white_list = []
-    package_commands = []
-    for root, dirs, files in os.walk(poc_workspace):
-        if root == poc_workspace:
-            fl_dirs = [d for d in dirs if is_fl_package_dir(d)]
-            for package_dir_name in fl_dirs:
-                if package_dir_name not in excluded:
-                    if len(white_list) == 0 or package_dir_name in white_list:
-                        cmd = get_package_command(cmd_type, poc_workspace, package_dir_name)
+    service_commands = []
+    for root, dirs, files in os.walk(prod_dir):
+        if root == prod_dir:
+            fl_dirs = [d for d in dirs if is_fl_service_dir(d)]
+            for service_dir_name in fl_dirs:
+                if service_dir_name not in excluded:
+                    if len(white_list) == 0 or service_dir_name in white_list:
+                        cmd = get_service_command(cmd_type, prod_dir, service_dir_name, service_config)
                         if cmd:
-                            package_commands.append((package_dir_name, cmd))
-    return sort_package_cmds(cmd_type, package_commands)
+                            service_commands.append((service_dir_name, cmd))
+    return sort_service_cmds(cmd_type, service_commands, service_config)
 
 
-def prepare_env(gpu_ids: Optional[List[int]] = None):
+def prepare_env(service_name, gpu_ids: Optional[List[int]], service_config: Dict):
     import os
 
+    my_env = None
     if gpu_ids:
         my_env = os.environ.copy()
-        if gpu_ids and len(gpu_ids) > 0:
+        if len(gpu_ids) > 0:
             my_env["CUDA_VISIBLE_DEVICES"] = ",".join([str(gid) for gid in gpu_ids])
-            return my_env
 
-    return None
+    if service_config.get(SC.IS_DOCKER_RUN):
+        my_env = os.environ.copy() if my_env is None else my_env
+        if gpu_ids and len(gpu_ids) > 0:
+            my_env["GPU2USE"] = f"--gpus={my_env['CUDA_VISIBLE_DEVICES']}"
+
+        my_env["MY_DATA_DIR"] = os.path.join(get_poc_workspace(), "data")
+        my_env["SVR_NAME"] = service_name
 
+    return my_env
 
-def async_process(cmd_path, gpu_ids: Optional[List[int]] = None):
-    my_env = prepare_env(gpu_ids)
+
+def async_process(service_name, cmd_path, gpu_ids: Optional[List[int]], service_config: Dict):
+    my_env = prepare_env(service_name, gpu_ids, service_config)
     if my_env:
         subprocess.Popen(cmd_path.split(" "), env=my_env)
     else:
         subprocess.Popen(cmd_path.split(" "))
 
-    time.sleep(3)
-
 
-def sync_process(cmd_path):
-    subprocess.run(cmd_path.split(" "))
+def sync_process(service_name, cmd_path):
+    my_env = os.environ.copy()
+    subprocess.run(cmd_path.split(" "), env=my_env)
 
 
-def _run_poc(cmd_type: str, poc_workspace: str, gpu_ids: List[int], excluded: list, white_list=None):
+def _run_poc(
+    cmd_type: str, poc_workspace: str, gpu_ids: List[int], service_config: Dict, excluded: list, white_list=None
+):
     if white_list is None:
         white_list = []
-    package_commands = _build_commands(cmd_type, poc_workspace, excluded, white_list)
-
-    clients = _get_clients(package_commands)
+    service_commands = _build_commands(cmd_type, poc_workspace, service_config, excluded, white_list)
+    clients = _get_clients(service_commands, service_config)
     gpu_assignments: Dict[str, List[int]] = client_gpu_assignments(clients, gpu_ids)
-
-    for package_name, cmd_path in package_commands:
-        print(f"{cmd_type}: package: {package_name}, executing {cmd_path}")
-        if package_name == SC.FLARE_CONSOLE:
-            sync_process(cmd_path)
-        elif package_name == SC.FLARE_SERVER:
-            async_process(cmd_path, None)
+    for service_name, cmd_path in service_commands:
+        if service_name == service_config[SC.FLARE_PROJ_ADMIN]:
+            # give other commands a chance to start first
+            if len(service_commands) > 1:
+                time.sleep(2)
+            sync_process(service_name, cmd_path)
+        elif service_name == service_config[SC.FLARE_SERVER]:
+            async_process(service_name, cmd_path, None, service_config)
         else:
-            async_process(cmd_path, gpu_assignments[package_name])
+            async_process(service_name, cmd_path, gpu_assignments[service_name], service_config)
 
 
 def clean_poc(poc_workspace: str):
     import shutil
 
-    if is_poc_ready(poc_workspace):
-        shutil.rmtree(poc_workspace, ignore_errors=True)
-        print(f"{poc_workspace} is removed")
+    if os.path.isdir(poc_workspace):
+        project_config, service_config = setup_service_config(poc_workspace)
+        if project_config is not None:
+            if is_poc_ready(poc_workspace, service_config):
+                shutil.rmtree(poc_workspace, ignore_errors=True)
+                print(f"{poc_workspace} is removed")
+            else:
+                raise CLIException(f"{poc_workspace} is not valid poc directory")
     else:
         raise CLIException(f"{poc_workspace} is not valid poc directory")
 
 
 def def_poc_parser(sub_cmd):
     cmd = "poc"
     poc_parser = sub_cmd.add_parser(cmd)
     poc_parser.add_argument(
         "-n", "--number_of_clients", type=int, nargs="?", default=2, help="number of sites or clients, default to 2"
     )
     poc_parser.add_argument(
+        "-c",
+        "--clients",
+        nargs="*",  # 0 or more values expected => creates a list
+        type=str,
+        default=[],  # default if nothing is provided
+        help="Space separated client names. If specified, number_of_clients argument will be ignored.",
+    )
+    poc_parser.add_argument(
         "-p",
-        "--package",
+        "--service",
         type=str,
         nargs="?",
         default="all",
-        help="package directory, default to all = all packages, only used for start/stop-poc commands when specified",
+        help="participant, Default to all participants, only used for start/stop poc commands when specified",
+    )
+    poc_parser.add_argument(
+        "-e",
+        "--examples",
+        type=str,
+        nargs="?",
+        default=None,
+        help="examples directory, only used in '--prepare' or '--prepare-example' command",
     )
     poc_parser.add_argument(
         "-ex",
         "--exclude",
         type=str,
         nargs="?",
         default="",
-        help="exclude package directory during --start or --stop, default to " ", i.e. nothing to exclude",
+        help="exclude service directory during --start or --stop, default to " ", i.e. nothing to exclude",
     )
     poc_parser.add_argument(
         "-gpu",
         "--gpu",
         type=int,
         nargs="*",
-        default="-1",
+        default=None,
         help="gpu device ids will be used as CUDA_VISIBLE_DEVICES. used for poc start command",
     )
     poc_parser.add_argument(
+        "-he",
+        "--he",
+        action="store_true",
+        help="enable homomorphic encryption. Use with '--prepare' command ",
+    )
+
+    poc_parser.add_argument(
+        "-i",
+        "--project_input",
+        type=str,
+        nargs="?",
+        default="",
+        help="project.yaml file path, it should be used with '--prepare' command. If specified, "
+        + "'number_of_clients','clients' and 'docker' specific options will be ignored.",
+    )
+    poc_parser.add_argument(
+        "-d",
+        "--docker_image",
+        nargs="?",
+        default=None,
+        const="nvflare/nvflare",
+        help="generate docker.sh based on the docker_image, used in '--prepare' command. and generate docker.sh "
+        + " '--start/stop' commands will start with docker.sh ",
+    )
+    poc_parser.add_argument(
         "--prepare",
         dest="prepare_poc",
         action="store_const",
         const=prepare_poc,
-        help="prepare poc workspace. "
-        + "export NVFLARE_HOME=<NVFLARE github cloned directory> to setup examples with prepare command",
+        help="prepare poc workspace and provision",
+    )
+
+    poc_parser.add_argument(
+        "--prepare-examples",
+        dest="prepare_examples",
+        action="store_const",
+        const=prepare_examples,
+        help="create an symbolic link to the examples directory, requires nvflare_example directory with '-e'",
     )
-    poc_parser.add_argument("--start", dest="start_poc", action="store_const", const=start_poc, help="start poc")
-    poc_parser.add_argument("--stop", dest="stop_poc", action="store_const", const=stop_poc, help="stop poc")
+
+    poc_parser.add_argument("--start", dest="start_poc", action="store_const", const=start_poc, help="start local")
+    poc_parser.add_argument("--stop", dest="stop_poc", action="store_const", const=stop_poc, help="stop local")
     poc_parser.add_argument(
-        "--clean", dest="clean_poc", action="store_const", const=clean_poc, help="cleanup poc workspace"
+        "--clean", dest="clean_poc", action="store_const", const=clean_poc, help="cleanup local workspace"
     )
     return {cmd: poc_parser}
 
 
 def is_poc(cmd_args) -> bool:
     return (
         hasattr(cmd_args, "start_poc")
         or hasattr(cmd_args, "prepare_poc")
         or hasattr(cmd_args, "stop_poc")
         or hasattr(cmd_args, "clean_poc")
+        or hasattr(cmd_args, "prepare_examples")
     )
 
 
 def get_local_host_gpu_ids():
     try:
         return get_host_gpu_ids()
     except Exception as e:
         raise CLIException(f"Failed to get host gpu ids:{e}")
 
 
 def handle_poc_cmd(cmd_args):
-    if cmd_args.package != "all":
-        white_list = [cmd_args.package]
+    if cmd_args.service != "all":
+        white_list = [cmd_args.service]
     else:
         white_list = []
 
     excluded = None
     if cmd_args.exclude != "":
         excluded = [cmd_args.exclude]
 
-    poc_workspace = os.getenv("NVFLARE_POC_WORKSPACE")
-    if poc_workspace is None or len(poc_workspace.strip()) == 0:
-        poc_workspace = DEFAULT_WORKSPACE
+    if cmd_args.gpu is not None and cmd_args.prepare_poc:
+        raise CLIException(
+            "-gpu should not be used for 'nvflare poc --prepare' command,"
+            " it is intended to use in 'nvflare poc --start' command "
+        )
 
+    poc_workspace = get_poc_workspace()
     if cmd_args.start_poc:
-        gpu_ids = get_gpu_ids(cmd_args.gpu, get_local_host_gpu_ids())
+        if cmd_args.gpu is not None and isinstance(cmd_args.gpu, list) and len(cmd_args.gpu) > 0:
+            gpu_ids = get_gpu_ids(cmd_args.gpu, get_local_host_gpu_ids())
+        else:
+            gpu_ids = []
         start_poc(poc_workspace, gpu_ids, excluded, white_list)
     elif cmd_args.prepare_poc:
-        prepare_poc(cmd_args.number_of_clients, poc_workspace)
+        project_conf_path = ""
+        if cmd_args.project_input:
+            project_conf_path = cmd_args.project_input
+        prepare_poc(
+            cmd_args.clients,
+            cmd_args.number_of_clients,
+            poc_workspace,
+            cmd_args.docker_image,
+            cmd_args.he,
+            project_conf_path,
+            cmd_args.examples,
+        )
+    elif cmd_args.prepare_examples:
+        prepare_examples(cmd_args.examples, poc_workspace)
     elif cmd_args.stop_poc:
         stop_poc(poc_workspace, excluded, white_list)
     elif cmd_args.clean_poc:
         clean_poc(poc_workspace)
     else:
         raise Exception(f"unable to handle poc command:{cmd_args}")
+
+
+def get_poc_workspace():
+    poc_workspace = os.getenv("NVFLARE_POC_WORKSPACE")
+    if poc_workspace is None or len(poc_workspace.strip()) == 0:
+        poc_workspace = DEFAULT_WORKSPACE
+    return poc_workspace
```

## nvflare/lighter/provision.py

```diff
@@ -15,14 +15,15 @@
 from __future__ import absolute_import
 
 import argparse
 import os
 import pathlib
 import shutil
 import sys
+from typing import Optional
 
 from nvflare.fuel.utils.class_utils import instantiate_class
 from nvflare.lighter.spec import Participant, Project, Provisioner
 from nvflare.lighter.utils import load_yaml
 
 adding_client_error_msg = """
 name: $SITE-NAME
@@ -90,63 +91,91 @@
 
     workspace = args.workspace
     workspace_full_path = os.path.join(current_path, workspace)
 
     project_full_path = os.path.join(current_path, project_file)
     print(f"Project yaml file: {project_full_path}.")
 
+    add_user_full_path = os.path.join(current_path, args.add_user) if args.add_user else None
+    add_client_full_path = os.path.join(current_path, args.add_client) if args.add_client else None
+
+    provision(project_full_path, workspace_full_path, add_user_full_path, add_client_full_path)
+
+
+def gen_default_project_config(src_project_name, dest_project_file):
+    file_path = pathlib.Path(__file__).parent.absolute()
+    shutil.copyfile(os.path.join(file_path, src_project_name), dest_project_file)
+
+
+def provision(
+    project_full_path: str,
+    workspace_full_path: str,
+    add_user_full_path: Optional[str] = None,
+    add_client_full_path: Optional[str] = None,
+):
     project_dict = load_yaml(project_full_path)
+    project = prepare_project(project_dict, add_user_full_path, add_client_full_path)
+    builders = prepare_builders(project_dict)
+    provisioner = Provisioner(workspace_full_path, builders)
+    provisioner.provision(project)
+
+
+def prepare_builders(project_dict):
+    builders = list()
+    for b in project_dict.get("builders"):
+        path = b.get("path")
+        args = b.get("args")
+        builders.append(instantiate_class(path, args))
+    return builders
+
+
+def prepare_project(project_dict, add_user_file_path=None, add_client_file_path=None):
     api_version = project_dict.get("api_version")
     if api_version not in [3]:
         raise ValueError(f"API version expected 3 but found {api_version}")
-
     project_name = project_dict.get("name")
     project_description = project_dict.get("description", "")
     participants = list()
     for p in project_dict.get("participants"):
         participants.append(Participant(**p))
-    if args.add_user:
-        try:
-            extra = load_yaml(os.path.join(current_path, args.add_user))
-            extra.update({"type": "admin"})
-            participants.append(Participant(**extra))
-        except Exception:
-            print("** Error during adding user **")
-            print("The yaml file format is")
-            print(adding_user_error_msg)
-            exit(0)
-    if args.add_client:
-        try:
-            extra = load_yaml(os.path.join(current_path, args.add_client))
-            extra.update({"type": "client"})
-            participants.append(Participant(**extra))
-        except Exception as e:
-            print("** Error during adding client **")
-            print("The yaml file format is")
-            print(adding_client_error_msg)
-            exit(0)
-
+    if add_user_file_path:
+        add_extra_users(add_user_file_path, participants)
+    if add_client_file_path:
+        add_extra_clients(add_client_file_path, participants)
     project = Project(name=project_name, description=project_description, participants=participants)
-
     n_servers = len(project.get_participants_by_type("server", first_only=False))
     if n_servers > 2:
-        print(
-            f"Configuration error: Expect 2 or 1 server to be provisioned.  {project_full_path} contains {n_servers} servers."
+        raise ValueError(
+            f"Configuration error: Expect 2 or 1 server to be provisioned. project contains {n_servers} servers."
         )
-        return
+    return project
 
-    builders = list()
-    for b in project_dict.get("builders"):
-        path = b.get("path")
-        args = b.get("args")
-        builders.append(instantiate_class(path, args))
 
-    provisioner = Provisioner(workspace_full_path, builders)
+def add_extra_clients(add_client_file_path, participants):
+    try:
+        extra = load_yaml(add_client_file_path)
+        extra.update({"type": "client"})
+        participants.append(Participant(**extra))
+    except BaseException as e:
+        print("** Error during adding client **")
+        print("The yaml file format is")
+        print(adding_client_error_msg)
+        exit(0)
 
-    provisioner.provision(project)
+
+def add_extra_users(add_user_file_path, participants):
+    try:
+        extra = load_yaml(add_user_file_path)
+        extra.update({"type": "admin"})
+        participants.append(Participant(**extra))
+    except BaseException:
+        print("** Error during adding user **")
+        print("The yaml file format is")
+        print(adding_user_error_msg)
+        exit(0)
 
 
 def main():
     print("*****************************************************************************")
     print("** provision command is deprecated, please use 'nvflare provision' instead **")
     print("*****************************************************************************")
```

## nvflare/lighter/service_constants.py

```diff
@@ -10,16 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 class FlareServiceConstants(object):
-    FLARE_CONSOLE = "admin"
+    FLARE_PROJ_ADMIN = "admin@nvidia.com"
     FLARE_SERVER = "server"
-    FLARE_CLIENT = "client"
+    FLARE_CLIENTS = "clients"
     FLARE_OVERSEER = "overseer"
     STARTUP = "startup"
     CMD_START = "start"
     CMD_STOP = "stop"
     EXAMPLES = "examples"
     TRANSFER = "transfer"
+    IS_DOCKER_RUN = "is_docker_run"
```

## nvflare/lighter/spec.py

```diff
@@ -172,15 +172,15 @@
             # call builders!
             for b in self.builders:
                 b.build(project, ctx)
 
             for b in self.builders[::-1]:
                 b.finalize(ctx)
 
-        except Exception as ex:
+        except BaseException as ex:
             prod_dir = ctx.get("current_prod_dir")
             if prod_dir:
                 shutil.rmtree(prod_dir)
             print("Exception raised during provision.  Incomplete prod_n folder removed.")
             traceback.print_exc()
         finally:
             wip_dir = ctx.get("wip_dir")
```

## nvflare/lighter/utils.py

```diff
@@ -46,19 +46,21 @@
 
 def load_private_key_file(file_path):
     with open(file_path, "rt") as f:
         pri_key = serialization.load_pem_private_key(f.read().encode("ascii"), password=None, backend=default_backend())
     return pri_key
 
 
-def sign_folders(folder, signing_pri_key, crt_path):
+def sign_folders(folder, signing_pri_key, crt_path, max_depth=9999):
+    depth = 0
     for root, folders, files in os.walk(folder):
+        depth = depth + 1
         signatures = dict()
         for file in files:
-            if file == ".__nvfl_sig.json":
+            if file == ".__nvfl_sig.json" or file == ".__nvfl_submitter.crt":
                 continue
             signature = signing_pri_key.sign(
                 data=open(os.path.join(root, file), "rb").read(),
                 padding=padding.PSS(
                     mgf=padding.MGF1(hashes.SHA256()),
                     salt_length=padding.PSS.MAX_LENGTH,
                 ),
@@ -71,29 +73,32 @@
                 padding=padding.PSS(
                     mgf=padding.MGF1(hashes.SHA256()),
                     salt_length=padding.PSS.MAX_LENGTH,
                 ),
                 algorithm=hashes.SHA256(),
             )
             signatures[folder] = b64encode(signature).decode("utf-8")
+
         json.dump(signatures, open(os.path.join(root, ".__nvfl_sig.json"), "wt"))
         shutil.copyfile(crt_path, os.path.join(root, ".__nvfl_submitter.crt"))
+        if depth >= max_depth:
+            break
 
 
-def verify_folder_signature(folder, root_ca_path):
+def verify_folder_signature(src_folder, root_ca_path):
     try:
         root_ca_cert = load_crt(root_ca_path)
         root_ca_public_key = root_ca_cert.public_key()
-        for root, folders, files in os.walk(folder):
+        for root, folders, files in os.walk(src_folder):
             try:
                 signatures = json.load(open(os.path.join(root, ".__nvfl_sig.json"), "rt"))
                 cert = load_crt(os.path.join(root, ".__nvfl_submitter.crt"))
                 public_key = cert.public_key()
             except:
-                continue
+                continue  # TODO: shall return False
             root_ca_public_key.verify(
                 cert.signature, cert.tbs_certificate_bytes, padding.PKCS1v15(), cert.signature_hash_algorithm
             )
             for k in signatures:
                 signatures[k] = b64decode(signatures[k].encode("utf-8"))
             for file in files:
                 if file == ".__nvfl_sig.json" or file == ".__nvfl_submitter.crt":
@@ -112,15 +117,15 @@
                     public_key.verify(
                         signature=signature,
                         data=folder.encode("utf-8"),
                         padding=padding.PSS(mgf=padding.MGF1(hashes.SHA256()), salt_length=padding.PSS.MAX_LENGTH),
                         algorithm=hashes.SHA256(),
                     )
         return True
-    except Exception as e:
+    except BaseException as e:
         return False
 
 
 def sign_all(content_folder, signing_pri_key):
     signatures = dict()
     for f in os.listdir(content_folder):
         path = os.path.join(content_folder, f)
@@ -149,40 +154,47 @@
 def sh_replace(src, mapping_dict):
     result = src
     for k, v in mapping_dict.items():
         result = result.replace("{~~" + k + "~~}", str(v))
     return result
 
 
-def update_project_config(project_config: dict, old_server_name, server_name) -> dict:
-    if project_config:
-        # update participants
-        participants = project_config["participants"]
-        for p in participants:
-            if p["name"] == old_server_name:
-                p["name"] = server_name
-
-        # update overseer_agent builder
-        builders = project_config["builders"]
-        for b in builders:
-            if "args" in b:
-                if "overseer_agent" in b["args"]:
-                    end_point = b["args"]["overseer_agent"]["args"]["sp_end_point"]
-                    new_end_point = end_point.replace(old_server_name, server_name)
-                    b["args"]["overseer_agent"]["args"]["sp_end_point"] = new_end_point
-    else:
-        RuntimeError("project_config is empty")
+def update_project_server_name_config(project_config: dict, old_server_name, server_name) -> dict:
+    update_participant_server_name(project_config, old_server_name, server_name)
+    update_overseer_server_name(project_config, old_server_name, server_name)
     return project_config
 
 
+def update_overseer_server_name(project_config, old_server_name, server_name):
+    # update overseer_agent builder
+    builders = project_config.get("builders", [])
+    for b in builders:
+        if "args" in b:
+            if "overseer_agent" in b["args"]:
+                end_point = b["args"]["overseer_agent"]["args"]["sp_end_point"]
+                new_end_point = end_point.replace(old_server_name, server_name)
+                b["args"]["overseer_agent"]["args"]["sp_end_point"] = new_end_point
+
+
+def update_participant_server_name(project_config, old_server_name, new_server_name):
+    participants = project_config["participants"]
+    for p in participants:
+        if p["type"] == "server" and p["name"] == old_server_name:
+            p["name"] = new_server_name
+            return
+
+
 def update_project_server_name(project_file: str, old_server_name, server_name):
     with open(project_file, "r") as file:
         project_config = yaml.safe_load(file)
 
-    update_project_config(project_config, old_server_name, server_name)
+    if not project_config:
+        raise RuntimeError("project_config is empty")
+
+    update_project_server_name_config(project_config, old_server_name, server_name)
 
     with open(project_file, "w") as file:
         yaml.dump(project_config, file)
 
 
 def update_storage_locations(
     local_dir: str,
```

## nvflare/lighter/impl/cert.py

```diff
@@ -75,15 +75,15 @@
             self.pri_key = pri_key
             self.pub_key = pub_key
             self.serialized_cert = serialize_cert(self.root_cert)
             self.persistent_state["root_cert"] = self.serialized_cert.decode("ascii")
             self.persistent_state["root_pri_key"] = serialize_pri_key(self.pri_key).decode("ascii")
 
     def _build_write_cert_pair(self, participant, base_name, ctx):
-        subject = participant.subject
+        subject = self.get_subject(participant)
         if self.persistent_state and subject in self.persistent_state:
             cert = x509.load_pem_x509_certificate(
                 self.persistent_state[subject]["cert"].encode("ascii"), default_backend()
             )
             pri_key = serialization.load_pem_private_key(
                 self.persistent_state[subject]["pri_key"].encode("ascii"), password=None, backend=default_backend()
             )
@@ -121,23 +121,26 @@
             self._build_write_cert_pair(client, "client", ctx)
 
         for admin in project.get_participants_by_type("admin", first_only=False):
             self._build_write_cert_pair(admin, "client", ctx)
 
     def get_pri_key_cert(self, participant):
         pri_key, pub_key = self._generate_keys()
-        subject = participant.subject
+        subject = self.get_subject(participant)
         subject_org = participant.org
         if participant.type == "admin":
             role = participant.props.get("role")
         else:
             role = None
         cert = self._generate_cert(subject, subject_org, self.issuer, self.pri_key, pub_key, role=role)
         return pri_key, cert
 
+    def get_subject(self, participant):
+        return participant.subject
+
     def _generate_keys(self):
         pri_key = rsa.generate_private_key(public_exponent=65537, key_size=2048, backend=default_backend())
         pub_key = pri_key.public_key()
         return pri_key, pub_key
 
     def _generate_cert(
         self, subject, subject_org, issuer, signing_pri_key, subject_pub_key, valid_days=360, ca=False, role=None
```

## nvflare/lighter/impl/docker.py

```diff
@@ -93,10 +93,10 @@
         compose_build_dir = os.path.join(self.get_wip_dir(ctx), "nvflare_compose")
         os.mkdir(compose_build_dir)
         with open(os.path.join(compose_build_dir, "Dockerfile"), "wt") as f:
             f.write(f"FROM {self.base_image}\n")
             f.write(self.template.get("dockerfile"))
         try:
             shutil.copyfile(self.requirements_file, os.path.join(compose_build_dir, "requirements.txt"))
-        except Exception:
+        except BaseException:
             f = open(os.path.join(compose_build_dir, "requirements.txt"), "wt")
             f.close()
```

## nvflare/lighter/impl/master_template.yml

```diff
@@ -99,18 +99,14 @@
 fed_client: |
   {
     "format_version": 2,
     "servers": [
       {
         "name": "spleen_segmentation",
         "service": {
-          "options": [
-            ["grpc.max_send_message_length",    2147483647],
-            ["grpc.max_receive_message_length", 2147483647]
-          ]
         }
       }
     ],
     "client": {
       "ssl_private_key": "client.key",
       "ssl_cert": "client.crt",
       "ssl_root_cert": "rootCA.pem"
@@ -227,19 +223,15 @@
 fed_server: |
   {
     "format_version": 2,
     "servers": [
         {
             "name": "spleen_segmentation",
             "service": {
-                "target": "localhost:8002",
-                "options": [
-                    ["grpc.max_send_message_length",    2147483647],
-                    ["grpc.max_receive_message_length", 2147483647]
-                ]
+                "target": "localhost:8002"
             },
             "admin_host": "localhost",
             "admin_port": 5005,
             "ssl_private_key": "server.key",
             "ssl_cert": "server.crt",
             "ssl_root_cert": "rootCA.pem"
         }
@@ -646,40 +638,66 @@
   rm -f $DIR/../pid.fl $DIR/../shutdown.fl $DIR/../restart.fl $DIR/../daemon_pid.fl
 
 docker_cln_sh: |
   #!/usr/bin/env bash
   DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" >/dev/null 2>&1 && pwd )"
   # docker run script for FL client
   # local data directory
-  MY_DATA_DIR=/home/flclient/data
+  : ${MY_DATA_DIR:="/home/flclient/data"}
+  # The syntax above is to set MY_DATA_DIR to /home/flcient/data if this
+  # environment variable is not set previously.
+  # Therefore, users can set their own MY_DATA_DIR with
+  # export MY_DATA_DIR=$SOME_DIRECTORY
+  # before running docker.sh
+
   # for all gpus use line below 
-  GPU2USE=all 
+  #GPU2USE='--gpus=all'
   # for 2 gpus use line below
-  #GPU2USE=2 
+  #GPU2USE='--gpus=2' 
   # for specific gpus as gpu#0 and gpu#2 use line below
-  #GPU2USE='"device=0,2"'
+  #GPU2USE='--gpus="device=0,2"'
   # to use host network, use line below
   NETARG="--net=host"
   # FL clients do not need to open ports, so the following line is not needed.
   #NETARG="-p 443:443 -p 8003:8003"
   DOCKER_IMAGE={~~docker_image~~}
   echo "Starting docker with $DOCKER_IMAGE"
-  docker run --rm -it --name={~~client_name~~} --gpus=$GPU2USE -u $(id -u):$(id -g) -v /etc/passwd:/etc/passwd -v /etc/group:/etc/group -v $DIR/..:/workspace/ -v $MY_DATA_DIR:/data/:ro -w /workspace/ --ipc=host $NETARG $DOCKER_IMAGE /bin/bash
+  mode="${1:--r}"
+  if [ $mode = "-d" ]
+  then
+    docker run -d --rm --name={~~client_name~~} $GPU2USE -u $(id -u):$(id -g) \
+    -v /etc/passwd:/etc/passwd -v /etc/group:/etc/group -v $DIR/..:/workspace/ \
+    -v $MY_DATA_DIR:/data/:ro -w /workspace/ --ipc=host $NETARG $DOCKER_IMAGE \
+    /bin/bash -c "python -u -m nvflare.private.fed.app.client.client_train -m /workspace -s fed_client.json --set uid={~~client_name~~} secure_train=true config_folder=config org={~~org_name~~}"
+  else
+    docker run --rm -it --name={~~client_name~~} $GPU2USE -u $(id -u):$(id -g) \
+    -v /etc/passwd:/etc/passwd -v /etc/group:/etc/group -v $DIR/..:/workspace/ \
+    -v $MY_DATA_DIR:/data/:ro -w /workspace/ --ipc=host $NETARG $DOCKER_IMAGE /bin/bash
+  fi
 
 docker_svr_sh: |
   #!/usr/bin/env bash
   DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" >/dev/null 2>&1 && pwd )"
   # docker run script for FL server
   # to use host network, use line below
   NETARG="--net=host"
   # or to expose specific ports, use line below
   #NETARG="-p {~~admin_port~~}:{~~admin_port~~} -p {~~fed_learn_port~~}:{~~fed_learn_port~~}"
   DOCKER_IMAGE={~~docker_image~~}
   echo "Starting docker with $DOCKER_IMAGE"
-  docker run --rm -it --name=flserver -v $DIR/..:/workspace/ -w /workspace/ --ipc=host $NETARG $DOCKER_IMAGE /bin/bash
+  svr_name="${SVR_NAME:-flserver}"
+  mode="${1:-r}"
+  if [ $mode = "-d" ]
+  then
+    docker run -d --rm --name=$svr_name -v $DIR/..:/workspace/ -w /workspace \
+    --ipc=host $NETARG $DOCKER_IMAGE /bin/bash -c \
+    "python -u -m nvflare.private.fed.app.server.server_train -m /workspace -s fed_server.json --set secure_train=true config_folder=config org={~~org_name~~}"
+  else
+    docker run --rm -it --name=$svr_name -v $DIR/..:/workspace/ -w /workspace/ --ipc=host $NETARG $DOCKER_IMAGE /bin/bash
+  fi
 
 docker_adm_sh: |
   #!/usr/bin/env bash
   DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" >/dev/null 2>&1 && pwd )"
   # docker run script for FL admin
   # to use host network, use line below
   #NETARG="--net=host"
@@ -882,15 +900,15 @@
               - containerPort: 8003
                 protocol: TCP
 helm_chart_values: |
   workspace: /home/nvflare
   persist: /home/nvflare
 
 
-azure_start_svr_sh: |
+cloud_script_header: |
   #!/usr/bin/env bash
   
   DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" >/dev/null 2>&1 && pwd )"
   function report_status() {
     status="$1"
     if [ "${status}" -ne 0 ]
     then
@@ -924,65 +942,86 @@
   do
     key="$1"
     case $key in
       --config)
         config_file=$2
         shift
       ;;
+      --image)
+        image_name=$2
+        shift
+      ;;
     esac
     shift
   done
-  
+
+azure_start_svr_sh: |
   RESOURCE_GROUP=nvflare_rg
   VM_NAME=nvflare_server
   VM_IMAGE=Canonical:0001-com-ubuntu-server-focal:20_04-lts-gen2:latest
   VM_SIZE=Standard_B2ms
   NSG_NAME=nvflare_nsgs
   ADMIN_USERNAME=nvflare
   PASSWORD="NVFl@r3_P@88"$RANDOM"w0rd"
   DEST_FOLDER=/var/tmp/cloud
   NIC_NAME=${VM_NAME}VMNic
   SERVER_NAME={~~server_name~~}
   FL_PORT=8002
   ADMIN_PORT=8003
 
+  echo "This script requires az (Azure CLI), sshpass and jq.  Now checking if they are installed."
+
+  check_binary az "Please see https://learn.microsoft.com/en-us/cli/azure/install-azure-cli on how to install it on your system."
+  check_binary sshpass "Please install it first."
+  check_binary jq "Please install it first."
+
   self_dns=true
   if [[ "$SERVER_NAME" = *".cloudapp.azure.com"* ]]
   then
     DNS_TAG=$(echo $SERVER_NAME | cut -d "." -f 1)
     DERIVED_LOCATION=$(echo $SERVER_NAME | cut -d "." -f 2)
     LOCATION=$DERIVED_LOCATION
     self_dns=false
   else
     echo "Warning: ${SERVER_NAME} does not end with .cloudapp.azure.com."
     echo "The cloud launch process will not create the domain name for you."
     echo "Please use your own DNS to set the information."
     LOCATION=westus2
   fi
 
+  if [ -z ${image_name+x} ]
+  then
+      container=false
+  else
+      container=true
+  fi
+
+  if [ $container = true ]
+  then
+    VM_IMAGE=Canonical:0001-com-ubuntu-server-focal:20_04-lts-gen2:latest
+    VM_SIZE=Standard_D8s_v3
+  else
+    VM_IMAGE=Canonical:0001-com-ubuntu-server-focal:20_04-lts-gen2:latest
+    VM_SIZE=Standard_B2ms
+  fi
+
   if [ -z ${config_file+x} ]
   then
     useDefault=true
   else
     useDefault=false
     . $config_file
     report_status "$?" "Loading config file"
     if [ $self_dns = false ] && [ $DERIVED_LOCATION != $LOCATION ]
     then
       echo "Server name implies LOCATION=${DERIVED_LOCATION} but the config file specifies LOCATION=${LOCATION}.  Unable to continue provisioning."
       exit 1
     fi
   fi
 
-  echo "This script requires az (Azure CLI), sshpass and jq.  Now checking if they are installed."
-
-  check_binary az "Please see https://learn.microsoft.com/en-us/cli/azure/install-azure-cli on how to install it on your system."
-  check_binary sshpass "Please install it first."
-  check_binary jq "Please install it first."
-
   if [ $useDefault = true ]
   then
     while true
     do
       prompt VM_IMAGE "Cloud VM image, press ENTER to accept default ${VM_IMAGE}: "
       prompt VM_SIZE "Cloud VM size, press ENTER to accept default ${VM_SIZE}: "
       if [ $self_dns = true ]
@@ -992,16 +1031,19 @@
       else
         prompt ans "VM image = ${VM_IMAGE}, VM size = ${VM_SIZE}, OK? (Y/n) "
       fi
       if [[ $ans = "" ]] || [[ $ans =~ ^(y|Y)$ ]]; then break; fi
     done
   fi
 
-  echo "If the client requires additional dependencies, please copy the requirements.txt to ${DIR}."
-  prompt ans "Press ENTER when it's done or no additional dependencies. "
+  if [ $container = false ]
+  then
+    echo "If the client requires additional dependencies, please copy the requirements.txt to ${DIR}."
+    prompt ans "Press ENTER when it's done or no additional dependencies. "
+  fi
 
   az login --use-device-code -o none
   report_status "$?" "login"
 
   # Start provisioning
 
   if [ $(az group exists -n $RESOURCE_GROUP) == 'false' ]
@@ -1098,122 +1140,127 @@
 
   echo "Copying files to $VM_NAME"
   DEST=$ADMIN_USERNAME@${IP_ADDRESS}:$DEST_FOLDER
   echo "Destination folder is ${DEST}"
   cd $DIR/.. && sshpass -p $PASSWORD scp -r -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null $PWD $DEST
   report_status "$?" "copying startup kits to VM"
 
-  echo "Installing packages in $VM_NAME, may take a few minutes."
-  az vm run-command invoke \
-    --output json \
-    --resource-group $RESOURCE_GROUP \
-    --command-id RunShellScript \
-    --name $VM_NAME \
-    --scripts \
-    "echo ${DEST_FOLDER} && \
-    wget -q https://bootstrap.pypa.io/get-pip.py && \
-    python3 get-pip.py && \
-    python3 -m pip install --ignore-installed nvflare && \
-    touch ${DEST_FOLDER}/startup/requirements.txt && \
-    python3 -m pip install -r ${DEST_FOLDER}/startup/requirements.txt && \
-    ${DEST_FOLDER}/startup/start.sh && \
-    sleep 20 && \
-    cat ${DEST_FOLDER}/log.txt" > /tmp/vm_create.json
-  report_status "$?" "installing packages"
-
+  if [ $container = true ]
+  then
+    echo "Installing and lauching container in $VM_NAME, may take a few minutes."
+    az vm run-command invoke \
+      --output json \
+      --resource-group $RESOURCE_GROUP \
+      --command-id RunShellScript \
+      --name $VM_NAME \
+      --scripts \
+      "sudo apt-get update && \
+      sudo DEBIAN_FRONTEND=noninteractive apt-get install -y ca-certificates curl gnupg lsb-release && \
+      sudo mkdir -p /etc/apt/keyrings && \
+      curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg && \
+      echo \
+      \"deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
+      $(lsb_release -cs) stable\" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null && \
+      sudo apt-get update && \
+      sudo DEBIAN_FRONTEND=noninteractive apt-get install -y docker-ce docker-ce-cli containerd.io && \
+      sudo usermod -aG docker $ADMIN_USERNAME" > /tmp/docker_engine.json
+    report_status "$?" "installing docker engine"
+    az vm run-command invoke \
+      --output json \
+      --resource-group $RESOURCE_GROUP \
+      --command-id RunShellScript \
+      --name $VM_NAME \
+      --scripts \
+      "docker run -d -v ${DEST_FOLDER}:${DEST_FOLDER} --network host ${DOCKER_OPTION} ${image_name} \
+      /bin/bash -c \"python -u -m nvflare.private.fed.app.server.server_train -m ${DEST_FOLDER} \
+      -s fed_server.json --set secure_train=true config_folder=config org={~~ORG~~} \" " > /tmp/vm_create.json 2>&1 
+      report_status "$?" "launching container"
+  else
+    echo "Installing packages in $VM_NAME, may take a few minutes."
+    az vm run-command invoke \
+      --output json \
+      --resource-group $RESOURCE_GROUP \
+      --command-id RunShellScript \
+      --name $VM_NAME \
+      --scripts \
+      "echo ${DEST_FOLDER} && \
+      wget -q https://bootstrap.pypa.io/get-pip.py && \
+      python3 get-pip.py && \
+      python3 -m pip install --ignore-installed nvflare && \
+      touch ${DEST_FOLDER}/startup/requirements.txt && \
+      python3 -m pip install -r ${DEST_FOLDER}/startup/requirements.txt && \
+      ${DEST_FOLDER}/startup/start.sh && \
+      sleep 20 && \
+      cat ${DEST_FOLDER}/log.txt" > /tmp/vm_create.json
+    report_status "$?" "installing packages"
+  fi
   echo "System was provisioned"
   echo "To delete the resource group (also delete the VM), run the following command"
   echo "az group delete -n ${RESOURCE_GROUP}"
   echo "To login to the VM with SSH, use ${ADMIN_USERNAME} : ${PASSWORD}" > vm_credential.txt
 
 azure_start_cln_sh: |
-  #!/usr/bin/env bash
-  DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" >/dev/null 2>&1 && pwd )"
-  function report_status() {
-    status="$1"
-    if [ "${status}" -ne 0 ]
-    then
-      echo "$2 failed"
-      exit "${status}"
-    fi
-  }
-
-  function check_binary() {
-    echo -n "Checking if $1 exists. => "
-    if ! command -v $1 &> /dev/null
-    then
-      echo "not found. $2"
-      exit 1
-    else
-      echo "found"
-    fi
-  }
-
-  function prompt() {
-    local __default="$1"
-    read -p "$2" ans
-    if [[ ! -z "$ans" ]]
-    then
-      eval $__default="'$ans'"
-    fi
-  }
-
-  # parse arguments
-  while [[ $# -gt 0 ]]
-  do
-      key="$1"
-      case $key in
-          --config)
-              config_file=$2
-              shift
-          ;;
-      esac
-      shift
-  done
-
   RESOURCE_GROUP=nvflare_client_rg_${RANDOM}_${RANDOM}
   VM_NAME=nvflare_client
   VM_IMAGE=Canonical:0001-com-ubuntu-server-focal:20_04-lts-gen2:latest
   VM_SIZE=Standard_B2ms
   NSG_NAME=nvflare_nsgc
   ADMIN_USERNAME=nvflare
   PASSWORD="NVFl@r3_P@88"$RANDOM"w0rd"
   DEST_FOLDER=/var/tmp/cloud
   LOCATION=westus2
   NIC_NAME=${VM_NAME}VMNic
+  echo "This script requires az (Azure CLI), sshpass and jq.  Now checking if they are installed."
 
+  check_binary az "Please see https://learn.microsoft.com/en-us/cli/azure/install-azure-cli on how to install it on your system."
+  check_binary sshpass "Please install it first."
+  check_binary jq "Please install it first."
+
+
+  if [ -z ${image_name+x} ]
+  then
+      container=false
+  else
+      container=true
+  fi
+
+  if [ $container = true ]
+  then
+    VM_IMAGE=Canonical:0001-com-ubuntu-server-focal:20_04-lts-gen2:latest
+    VM_SIZE=Standard_D8s_v3
+  else
+    VM_IMAGE=Canonical:0001-com-ubuntu-server-focal:20_04-lts-gen2:latest
+    VM_SIZE=Standard_B2ms
+  fi
   if [ -z ${config_file+x} ]
   then
       useDefault=true
   else
       useDefault=false
       . $config_file
       report_status "$?" "Loading config file"
   fi
 
-  echo "This script requires az (Azure CLI), sshpass and jq.  Now checking if they are installed."
-
-  check_binary az "Please see https://learn.microsoft.com/en-us/cli/azure/install-azure-cli on how to install it on your system."
-  check_binary sshpass "Please install it first."
-  check_binary jq "Please install it first."
-
   if [ $useDefault = true ]
   then
     while true
     do
       prompt LOCATION "Cloud location, press ENTER to accept default ${LOCATION}: "
       prompt VM_IMAGE "Cloud VM image, press ENTER to accept default ${VM_IMAGE}: "
       prompt VM_SIZE "Cloud VM size, press ENTER to accept default ${VM_SIZE}: "
       prompt ans "location = ${LOCATION}, VM image = ${VM_IMAGE}, VM size = ${VM_SIZE}, OK? (Y/n) "
       if [[ $ans = "" ]] || [[ $ans =~ ^(y|Y)$ ]]; then break; fi
     done
   fi
 
-  echo "If the client requires additional dependencies, please copy the requirements.txt to ${DIR}."
-  prompt ans "Press ENTER when it's done or no additional dependencies. "
+  if [ $container = false ]
+  then
+    echo "If the client requires additional dependencies, please copy the requirements.txt to ${DIR}."
+    prompt ans "Press ENTER when it's done or no additional dependencies. "
+  fi
 
   az login --use-device-code -o none
   report_status "$?" "login"
 
   # Start provisioning
 
   if [ $(az group exists -n $RESOURCE_GROUP) == 'false' ]
@@ -1269,69 +1316,69 @@
 
   echo "Copying files to $VM_NAME"
   DEST=$ADMIN_USERNAME@$IP_ADDRESS:$DEST_FOLDER
   echo "Destination folder is ${DEST}"
   cd $DIR/.. && sshpass -p $PASSWORD scp -r -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null $PWD $DEST
   report_status "$?" "copying startup kits to VM"
 
-  echo "Installing packages in $VM_NAME, may take a few minutes."
-  az vm run-command invoke \
-    --output json \
-    --resource-group $RESOURCE_GROUP \
-    --command-id RunShellScript \
-    --name $VM_NAME \
-    --scripts \
-    "echo ${DEST_FOLDER} && \
-    wget -q https://bootstrap.pypa.io/get-pip.py && \
-    python3 get-pip.py && \
-    python3 -m pip install --ignore-installed nvflare && \
-    touch ${DEST_FOLDER}/startup/requirements.txt && \
-    python3 -m pip install -r ${DEST_FOLDER}/startup/requirements.txt && \
-    ${DEST_FOLDER}/startup/start.sh && \
-    sleep 20 && \
-    cat ${DEST_FOLDER}/log.txt" > /tmp/vm_create.json
-  report_status "$?" "installing packages"
-
+  if [ $container = true ]
+  then
+    echo "Installing and lauching container in $VM_NAME, may take a few minutes."
+    az vm run-command invoke \
+      --output json \
+      --resource-group $RESOURCE_GROUP \
+      --command-id RunShellScript \
+      --name $VM_NAME \
+      --scripts \
+      "sudo apt-get update && \
+      sudo DEBIAN_FRONTEND=noninteractive apt-get install -y ca-certificates curl gnupg lsb-release && \
+      sudo mkdir -p /etc/apt/keyrings && \
+      curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg && \
+      echo \
+      \"deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
+      $(lsb_release -cs) stable\" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null && \
+      sudo apt-get update && \
+      sudo DEBIAN_FRONTEND=noninteractive apt-get install -y docker-ce docker-ce-cli containerd.io && \
+      sudo usermod -aG docker $ADMIN_USERNAME" > /tmp/docker_engine.json
+    report_status "$?" "installing docker engine"
+    az vm run-command invoke \
+      --output json \
+      --resource-group $RESOURCE_GROUP \
+      --command-id RunShellScript \
+      --name $VM_NAME \
+      --scripts \
+      "docker run -d -v ${DEST_FOLDER}:${DEST_FOLDER} ${image_name} \
+      /bin/bash -c \"python -u -m nvflare.private.fed.app.client.client_train -m ${DEST_FOLDER} \
+      -s fed_client.json --set uid={~~SITE~~} secure_train=true config_folder=config org={~~ORG~~} \" " > /tmp/vm_create.json 2>&1 
+      report_status "$?" "launching container"
+  else
+    echo "Installing packages in $VM_NAME, may take a few minutes."
+    az vm run-command invoke \
+      --output json \
+      --resource-group $RESOURCE_GROUP \
+      --command-id RunShellScript \
+      --name $VM_NAME \
+      --scripts \
+      "echo ${DEST_FOLDER} && \
+      wget -q https://bootstrap.pypa.io/get-pip.py && \
+      python3 get-pip.py && \
+      python3 -m pip install --ignore-installed nvflare && \
+      touch ${DEST_FOLDER}/startup/requirements.txt && \
+      python3 -m pip install -r ${DEST_FOLDER}/startup/requirements.txt && \
+      ${DEST_FOLDER}/startup/start.sh && \
+      sleep 20 && \
+      cat ${DEST_FOLDER}/log.txt" > /tmp/vm_create.json
+    report_status "$?" "installing packages"
+  fi
   echo "System was provisioned"
   echo "To delete the resource group (also delete the VM), run the following command"
   echo "az group delete -n ${RESOURCE_GROUP}"
   echo "To login to the VM with SSH, use ${ADMIN_USERNAME} : ${PASSWORD}" > vm_credential.txt
 
 azure_start_dsb_sh: |
-  #!/usr/bin/env bash
-
-  function report_status() {
-    status="$1"
-    if [ "${status}" -ne 0 ]
-    then
-      echo "$2 failed"
-      exit "${status}"
-    fi
-  }
-
-  function check_binary() {
-    echo -n "Checking if $1 exists. => "
-    if ! command -v $1 &> /dev/null
-    then
-      echo "not found $2"
-      exit 1
-    else
-      echo "found"
-    fi
-  }
-  
-  function prompt() {
-  local __default="$1"
-  read -p "$2" ans
-  if [[ ! -z "$ans" ]]
-  then
-    eval $__default="'$ans'"
-  fi
-  }
-
   RESOURCE_GROUP=nvflare_dashboard_rg_${RANDOM}_${RANDOM}
   VM_NAME=nvflare_dashboard
   VM_IMAGE=Canonical:0001-com-ubuntu-server-focal:20_04-lts-gen2:latest
   VM_SIZE=Standard_B2ms
   NSG_NAME=nvflare_nsgc
   ADMIN_USERNAME=nvflare
   PASSWORD="NVFl@r3_P@88"$RANDOM"w0rd"
@@ -1441,15 +1488,15 @@
     --resource-group $RESOURCE_GROUP \
     --command-id RunShellScript \
     --name $VM_NAME \
     --scripts \
     "echo ${DEST_FOLDER} && \
     wget -q https://bootstrap.pypa.io/get-pip.py && \
     python3 get-pip.py && \
-    python3 -m pip install --ignore-installed nvflare && \
+    python3 -m pip install --ignore-installed {~~NVFLARE~~} && \
     mkdir -p ${DEST_FOLDER}/cert && \
     chown -R ${ADMIN_USERNAME} ${DEST_FOLDER}" > /tmp/nvflare.json && \
   report_status "$?" "installing nvflare"
 
   echo "Checking if certificate (web.crt) and private key (web.key) are available"
   if [[ -f "web.crt" && -f "web.key" ]]; then
     DEST=$ADMIN_USERNAME@$IP_ADDRESS:${DEST_FOLDER}/cert
@@ -1466,15 +1513,15 @@
   az vm run-command invoke \
     --output json \
     --resource-group $RESOURCE_GROUP \
     --command-id RunShellScript \
     --name $VM_NAME \
     --scripts \
     "cd ${DEST_FOLDER} && \
-     python3 -m nvflare.dashboard.cli --start -f ${DEST_FOLDER} --cred ${credential}" > /tmp/dashboard.json
+     python3 -m nvflare.dashboard.cli --start -f ${DEST_FOLDER} --cred ${credential} {~~START_OPT~~}" > /tmp/dashboard.json
 
   # credential=$(jq -r .value[0].message /tmp/dashboard.json | grep "Project admin")
   # echo "The VM was created with user: ${ADMIN_USERNAME} and password: ${PASSWORD}"
   if [ "$secure" = true ]
   then
     echo "URL is https://${IP_ADDRESS}"
   else
@@ -1600,77 +1647,45 @@
     }
   },
   "nbformat": 4,
   "nbformat_minor": 5
   }
 
 aws_start_svr_sh: |
-  #!/usr/bin/env bash
-
-  set +e
-  DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" >/dev/null 2>&1 && pwd )"
-
-  function report_status() {
-    status="$1"
-    if [ "${status}" -ne 0 ]
-    then
-      echo "$2 failed"
-      exit "${status}"
-    fi
-  }
-
-  function check_binary() {
-    echo -n "Checking if $1 exists. => "
-    if ! command -v $1 &> /dev/null
-    then
-      echo "not found. $2"
-      exit 1
-    else
-      echo "found"
-    fi
-  }
-
-  function prompt() {
-    local __default="$1"
-    read -p "$2" ans
-    if [[ ! -z "$ans" ]]
-    then
-      eval $__default="'$ans'"
-    fi
-  }
-
-  # parse arguments
-  while [[ $# -gt 0 ]]
-  do
-    key="$1"
-    case $key in
-      --config)
-        config_file=$2
-        shift
-      ;;
-    esac
-    shift
-  done
-
   VM_NAME=nvflare_server
-  AMI_IMAGE=ami-04bad3c587fe60d89
-  EC2_TYPE=t2.small
   SECURITY_GROUP=nvflare_server_sg
   DEST_FOLDER=/var/tmp/cloud
-  REGION=us-west-2
   KEY_PAIR=NVFlareServerKeyPair
   KEY_FILE=${KEY_PAIR}.pem
 
   echo "This script requires aws (AWS CLI), sshpass, dig and jq.  Now checking if they are installed."
 
   check_binary aws "Please see https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html on how to install it on your system."
   check_binary sshpass "Please install it first."
   check_binary dig "Please install it first."
   check_binary jq "Please install it first."
 
+  if [ -z ${image_name+x} ]
+  then
+      container=false
+  else
+      container=true
+  fi
+
+  if [ $container = true ]
+  then
+    AMI_IMAGE=ami-06b8d5099f3a8d79d
+    EC2_TYPE=t2.xlarge
+    REGION=us-west-2
+  else
+    AMI_IMAGE=ami-04bad3c587fe60d89
+    EC2_TYPE=t2.small
+    REGION=us-west-2
+  fi
+
   if [ -z ${config_file+x} ]
   then
       useDefault=true
   else
       useDefault=false
       . $config_file
       report_status "$?" "Loading config file"
@@ -1688,16 +1703,19 @@
       if [[ $ans = "" ]] || [[ $ans =~ ^(y|Y)$ ]]
       then
         break
       fi
     done
   fi
 
-  echo "If the server requires additional dependencies, please copy the requirements.txt to ${DIR}."
-  prompt ans "Press ENTER when it's done or no additional dependencies. "
+  if [ $container = false ]
+  then
+    echo "If the server requires additional dependencies, please copy the requirements.txt to ${DIR}."
+    prompt ans "Press ENTER when it's done or no additional dependencies. "
+  fi
 
   cd $DIR/..
   # Generate key pair
 
   echo "Generating key pair for VM"
 
   aws ec2 delete-key-pair --key-name $KEY_PAIR > /dev/null 2>&1
@@ -1735,96 +1753,72 @@
   echo "Copying files to $VM_NAME"
   DEST_SITE=ubuntu@${IP_ADDRESS}
   DEST=${DEST_SITE}:${DEST_FOLDER}
   echo "Destination folder is ${DEST}"
   scp -q -i $KEY_FILE -r -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null $PWD $DEST
   report_status "$?" "copying startup kits to VM"
 
-  echo "Installing packages in $VM_NAME, may take a few minutes."
-
-  ssh -f -i $KEY_FILE -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null ${DEST_SITE} \
-  "pwd && wget -q https://bootstrap.pypa.io/get-pip.py && \
-  python3 get-pip.py && python3 -m pip install nvflare && \
-  touch ${DEST_FOLDER}/startup/requirements.txt && \
-  python3 -m pip install -r ${DEST_FOLDER}/startup/requirements.txt && \
-  nohup ${DEST_FOLDER}/startup/start.sh && sleep 20 && \
-  exit" > /tmp/nvflare.log 2>&1 
-  report_status "$?" "installing packages"
+  if [ $container = true ]
+  then
+    echo "Launching container with docker option ${DOCKER_OPTION}."
+    ssh -f -i $KEY_FILE -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null ${DEST_SITE} \
+    "docker run -d -v ${DEST_FOLDER}:${DEST_FOLDER} --network host ${DOCKER_OPTION} ${image_name} \
+    /bin/bash -c \"python -u -m nvflare.private.fed.app.server.server_train -m ${DEST_FOLDER} \
+    -s fed_server.json --set secure_train=true config_folder=config org={~~ORG~~} \" " > /tmp/nvflare.log 2>&1 
+    report_status "$?" "launching container"
+  else
+    ssh -f -i $KEY_FILE -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null ${DEST_SITE} \
+    "pwd && wget -q https://bootstrap.pypa.io/get-pip.py && \
+    python3 get-pip.py && python3 -m pip install nvflare && \
+    touch ${DEST_FOLDER}/startup/requirements.txt && \
+    python3 -m pip install -r ${DEST_FOLDER}/startup/requirements.txt && \
+    nohup ${DEST_FOLDER}/startup/start.sh && sleep 20 && \
+    exit" > /tmp/nvflare.log 2>&1 
+    report_status "$?" "installing packages"
+  fi
 
   echo "System was provisioned"
   echo "To terminate the EC2 instance, run the following command."
   echo "aws ec2 terminate-instances --instance-ids ${instance_id}"
   echo "Other resources provisioned"
   echo "security group: ${SECURITY_GROUP}"
   echo "key pair: ${KEY_PAIR}"
 
 aws_start_cln_sh: |
-  #!/usr/bin/env bash
-
-  set +e
-  DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" >/dev/null 2>&1 && pwd )"
-
-  function report_status() {
-    status="$1"
-    if [ "${status}" -ne 0 ]
-    then
-      echo "$2 failed"
-      exit "${status}"
-    fi
-  }
-
-  function check_binary() {
-    echo -n "Checking if $1 exists. => "
-    if ! command -v $1 &> /dev/null
-    then
-      echo "not found. $2"
-      exit 1
-    else
-      echo "found"
-    fi
-  }
-
-  function prompt() {
-    local __default="$1"
-    read -p "$2" ans
-    if [[ ! -z "$ans" ]]
-    then
-      eval $__default="'$ans'"
-    fi
-  }
-
-  # parse arguments
-  while [[ $# -gt 0 ]]
-  do
-    key="$1"
-    case $key in
-      --config)
-        config_file=$2
-        shift
-      ;;
-    esac
-    shift
-  done
-
   VM_NAME=nvflare_client
-  AMI_IMAGE=ami-04bad3c587fe60d89
-  EC2_TYPE=t2.small
   SECURITY_GROUP=nvflare_client_sg_$RANDOM
   DEST_FOLDER=/var/tmp/cloud
-  REGION=us-west-2
   KEY_PAIR=NVFlareClientKeyPair
   KEY_FILE=${KEY_PAIR}.pem
 
   echo "This script requires aws (AWS CLI), sshpass, dig and jq.  Now checking if they are installed."
 
   check_binary aws "Please see https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html on how to install it on your system."
   check_binary sshpass "Please install it first."
   check_binary dig "Please install it first."
   check_binary jq "Please install it first."
 
+  if [ -z ${image_name+x} ]
+  then
+      container=false
+  else
+      container=true
+  fi
+
+  if [ $container = true ]
+  then
+    AMI_IMAGE=ami-06b8d5099f3a8d79d
+    EC2_TYPE=t2.xlarge
+    REGION=us-west-2
+  else
+    AMI_IMAGE=ami-04bad3c587fe60d89
+    EC2_TYPE=t2.small
+    REGION=us-west-2
+  fi
+
   if [ -z ${config_file+x} ]
   then
       useDefault=true
   else
       useDefault=false
       . $config_file
       report_status "$?" "Loading config file"
@@ -1841,16 +1835,19 @@
       if [[ $ans = "" ]] || [[ $ans =~ ^(y|Y)$ ]]
       then
         break
       fi
     done
   fi
 
-  echo "If the client requires additional dependencies, please copy the requirements.txt to ${DIR}."
-  prompt ans "Press ENTER when it's done or no additional dependencies. "
+  if [ $container = false ]
+  then
+    echo "If the client requires additional dependencies, please copy the requirements.txt to ${DIR}."
+    prompt ans "Press ENTER when it's done or no additional dependencies. "
+  fi
 
   cd $DIR/..
   # Generate key pair
 
   echo "Generating key pair for VM"
 
   aws ec2 delete-key-pair --key-name $KEY_PAIR > /dev/null 2>&1
@@ -1886,66 +1883,44 @@
   echo "Copying files to $VM_NAME"
   DEST_SITE=ubuntu@${IP_ADDRESS}
   DEST=${DEST_SITE}:${DEST_FOLDER}
   echo "Destination folder is ${DEST}"
   scp -q -i $KEY_FILE -r -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null $PWD $DEST
   report_status "$?" "copying startup kits to VM"
 
-  echo "Installing packages in $VM_NAME, may take a few minutes."
-
-  ssh -f -i $KEY_FILE -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null ${DEST_SITE} \
-  "pwd && wget -q https://bootstrap.pypa.io/get-pip.py && \
-  python3 get-pip.py && python3 -m pip install nvflare && \
-  touch ${DEST_FOLDER}/startup/requirements.txt && \
-  python3 -m pip install -r ${DEST_FOLDER}/startup/requirements.txt && \
-  nohup ${DEST_FOLDER}/startup/start.sh && sleep 20 && \
-  exit" > /tmp/nvflare.log 2>&1 
+  if [ $container = true ]
+  then
+    echo "Launching container with docker option ${DOCKER_OPTION}."
+    ssh -f -i $KEY_FILE -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null ${DEST_SITE} \
+    "docker run -d -v ${DEST_FOLDER}:${DEST_FOLDER} --network host ${DOCKER_OPTION} ${image_name} \
+    /bin/bash -c \"python -u -m nvflare.private.fed.app.client.client_train -m ${DEST_FOLDER} \
+    -s fed_client.json --set uid={~~SITE~~} secure_train=true config_folder=config org={~~ORG~~} \" " > /tmp/nvflare.log 2>&1 
+    report_status "$?" "launching container"
+  else
+    echo "Installing packages in $VM_NAME, may take a few minutes."
+    ssh -f -i $KEY_FILE -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null ${DEST_SITE} \
+    "pwd && wget -q https://bootstrap.pypa.io/get-pip.py && \
+    python3 get-pip.py && python3 -m pip install nvflare && \
+    touch ${DEST_FOLDER}/startup/requirements.txt && \
+    python3 -m pip install -r ${DEST_FOLDER}/startup/requirements.txt && \
+    nohup ${DEST_FOLDER}/startup/start.sh && sleep 20 && \
+    exit" > /tmp/nvflare.log 2>&1 
 
-  report_status "$?" "installing packages"
+    report_status "$?" "installing packages"
+  fi
 
   echo "System was provisioned"
   echo "To terminate the EC2 instance, run the following command."
   echo "aws ec2 terminate-instances --instance-ids ${instance_id}"
   echo "Other resources provisioned"
   echo "security group: ${SECURITY_GROUP}"
   echo "key pair: ${KEY_PAIR}"
 
 
 aws_start_dsb_sh: |
-  #!/usr/bin/env bash
-
-  function report_status() {
-    status="$1"
-    if [ "${status}" -ne 0 ]
-    then
-      echo "$2 failed"
-      exit "${status}"
-    fi
-  }
-
-  function check_binary() {
-    echo -n "Checking if $1 exists. => "
-    if ! command -v $1 &> /dev/null
-    then
-      echo "not found $2"
-      exit 1
-    else
-      echo "found"
-    fi
-  }
-  
-  function prompt() {
-  local __default="$1"
-  read -p "$2" ans
-  if [[ ! -z "$ans" ]]
-  then
-    eval $__default="'$ans'"
-  fi
-  }
-
   VM_NAME=nvflare_dashboard
   AMI_IMAGE=ami-04bad3c587fe60d89
   EC2_TYPE=t2.small
   SECURITY_GROUP=nvflare_dashboard_sg_$RANDOM
   REGION=us-west-2
   ADMIN_USERNAME=ubuntu
   DEST_FOLDER=/home/${ADMIN_USERNAME}
@@ -2013,15 +1988,15 @@
     sudo usermod -aG docker $ADMIN_USERNAME && exit" > /tmp/docker_engine.log
   report_status "$?" "installing docker engine"
 
   echo "Installing nvflare in $VM_NAME, may take a few minutes."
   ssh -i $KEY_FILE -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null ${DEST_SITE} \
     "export PATH=/home/ubuntu/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin && \
     wget -q https://bootstrap.pypa.io/get-pip.py && python3 get-pip.py && \
-    python3 -m pip install nvflare && \
+    python3 -m pip install {~~NVFLARE~~} && \
     mkdir -p ./cert && \
     exit" > /tmp/nvflare.json
   report_status "$?" "installing nvflare"
 
   echo "Checking if certificate (web.crt) and private key (web.key) are available"
   if [[ -f "web.crt" && -f "web.key" ]]; then
     CERT_FOLDER=${DEST_SITE}:${DEST_FOLDER}/cert
@@ -2033,15 +2008,15 @@
     echo "No web.crt and web.key found"
     secure=false
   fi
 
   echo "Starting dashboard"
   ssh -i $KEY_FILE -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null ${DEST_SITE} \
     "export PATH=/home/ubuntu/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin && \
-    python3 -m nvflare.dashboard.cli --start -f ${DEST_FOLDER} --cred ${credential}" > /tmp/dashboard.json
+    python3 -m nvflare.dashboard.cli --start -f ${DEST_FOLDER} --cred ${credential} {~~START_OPT~~}" > /tmp/dashboard.json
 
   echo "Dashboard url is running at IP address ${IP_ADDRESS}, listening to port 443."
   if [ "$secure" = true ]
   then
     echo "URL is https://${IP_ADDRESS}"
   else
     echo "URL is http://${IP_ADDRESS}:443"
```

## nvflare/lighter/impl/static_file.py

```diff
@@ -23,14 +23,15 @@
 
 
 class StaticFileBuilder(Builder):
     def __init__(
         self,
         enable_byoc=False,
         config_folder="",
+        scheme="grpc",
         app_validator="",
         download_job_url="",
         docker_image="",
         snapshot_persistor="",
         overseer_agent="",
         components="",
     ):
@@ -48,41 +49,48 @@
             enable_byoc: for each participant, true to enable loading of code in the custom folder of applications
             config_folder: usually "config"
             app_validator: optional path to an app validator to verify that uploaded app has the expected structure
             docker_image: when docker_image is set to a docker image name, docker.sh will be generated on server/client/admin
         """
         self.enable_byoc = enable_byoc
         self.config_folder = config_folder
+        self.scheme = scheme
         self.docker_image = docker_image
         self.download_job_url = download_job_url
         self.app_validator = app_validator
         self.overseer_agent = overseer_agent
         self.snapshot_persistor = snapshot_persistor
         self.components = components
 
     def _write(self, file_full_path, content, mode, exe=False):
         mode = mode + "w"
         with open(file_full_path, mode) as f:
             f.write(content)
         if exe:
             os.chmod(file_full_path, 0o755)
 
+    def get_server_name(self, server):
+        return server.name
+
+    def get_overseer_name(self, overseer):
+        return overseer.name
+
     def _build_overseer(self, overseer, ctx):
         dest_dir = self.get_kit_dir(overseer, ctx)
         self._write(
             os.path.join(dest_dir, "start.sh"),
             self.template["start_svr_sh"],
             "t",
             exe=True,
         )
         protocol = overseer.props.get("protocol", "http")
         api_root = overseer.props.get("api_root", "/api/v1/")
         default_port = "443" if protocol == "https" else "80"
         port = overseer.props.get("port", default_port)
-        replacement_dict = {"port": port, "hostname": overseer.name}
+        replacement_dict = {"port": port, "hostname": self.get_overseer_name(overseer)}
         admins = self.project.get_participants_by_type("admin", first_only=False)
         privilege_dict = dict()
         for admin in admins:
             role = admin.props.get("role")
             if role in privilege_dict:
                 privilege_dict[role].append(admin.subject)
             else:
@@ -110,44 +118,45 @@
         self._write(
             os.path.join(dest_dir, "start.sh"),
             self.template["start_ovsr_sh"],
             "t",
             exe=True,
         )
         if port:
-            ctx["overseer_end_point"] = f"{protocol}://{overseer.name}:{port}{api_root}"
+            ctx["overseer_end_point"] = f"{protocol}://{self.get_overseer_name(overseer)}:{port}{api_root}"
         else:
-            ctx["overseer_end_point"] = f"{protocol}://{overseer.name}{api_root}"
+            ctx["overseer_end_point"] = f"{protocol}://{self.get_overseer_name(overseer)}{api_root}"
 
     def _build_server(self, server, ctx):
         config = json.loads(self.template["fed_server"])
         dest_dir = self.get_kit_dir(server, ctx)
         server_0 = config["servers"][0]
         server_0["name"] = self.project_name
         admin_port = server.props.get("admin_port", 8003)
         ctx["admin_port"] = admin_port
         fed_learn_port = server.props.get("fed_learn_port", 8002)
         ctx["fed_learn_port"] = fed_learn_port
-        ctx["server_name"] = server.name
-        server_0["service"]["target"] = f"{server.name}:{fed_learn_port}"
-        server_0["admin_host"] = server.name
+        ctx["server_name"] = self.get_server_name(server)
+        server_0["service"]["target"] = f"{self.get_server_name(server)}:{fed_learn_port}"
+        server_0["service"]["scheme"] = self.scheme
+        server_0["admin_host"] = self.get_server_name(server)
         server_0["admin_port"] = admin_port
         # if self.download_job_url:
         #     server_0["download_job_url"] = self.download_job_url
         # config["enable_byoc"] = server.enable_byoc
         # if self.app_validator:
         #     config["app_validator"] = {"path": self.app_validator}
         if self.overseer_agent:
             overseer_agent = copy.deepcopy(self.overseer_agent)
             if overseer_agent.get("overseer_exists", True):
                 overseer_agent["args"] = {
                     "role": "server",
                     "overseer_end_point": ctx.get("overseer_end_point", ""),
                     "project": self.project_name,
-                    "name": server.name,
+                    "name": self.get_server_name(server),
                     "fl_port": str(fed_learn_port),
                     "admin_port": str(admin_port),
                 }
             overseer_agent.pop("overseer_exists", None)
             config["overseer_agent"] = overseer_agent
         # if self.snapshot_persistor:
         #     config["snapshot_persistor"] = self.snapshot_persistor
@@ -226,14 +235,15 @@
 
     def _build_client(self, client, ctx):
         config = json.loads(self.template["fed_client"])
         dest_dir = self.get_kit_dir(client, ctx)
         fed_learn_port = ctx.get("fed_learn_port")
         server_name = ctx.get("server_name")
         # config["servers"][0]["service"]["target"] = f"{server_name}:{fed_learn_port}"
+        config["servers"][0]["service"]["scheme"] = self.scheme
         config["servers"][0]["name"] = self.project_name
         # config["enable_byoc"] = client.enable_byoc
         replacement_dict = {
             "client_name": f"{client.subject}",
             "config_folder": self.config_folder,
             "docker_image": self.docker_image,
             "org_name": client.org,
@@ -309,37 +319,26 @@
         self._write(
             os.path.join(self.get_ws_dir(client, ctx), "readme.txt"),
             self.template["readme_fc"],
             "t",
         )
 
     def _build_admin(self, admin, ctx):
-        config = json.loads(self.template["fed_admin"])
         dest_dir = self.get_kit_dir(admin, ctx)
         admin_port = ctx.get("admin_port")
         server_name = ctx.get("server_name")
 
         replacement_dict = {
             "cn": f"{server_name}",
             "admin_port": f"{admin_port}",
             "docker_image": self.docker_image,
         }
-        agent_config = dict()
-        if self.overseer_agent:
-            overseer_agent = copy.deepcopy(self.overseer_agent)
-            if overseer_agent.get("overseer_exists", True):
-                overseer_agent["args"] = {
-                    "role": "admin",
-                    "overseer_end_point": ctx.get("overseer_end_point", ""),
-                    "project": self.project_name,
-                    "name": admin.subject,
-                }
-            overseer_agent.pop("overseer_exists", None)
-            agent_config["overseer_agent"] = overseer_agent
-        config["admin"].update(agent_config)
+
+        config = self.prepare_admin_config(admin, ctx)
+
         self._write(os.path.join(dest_dir, "fed_admin.json"), json.dumps(config, indent=2), "t")
         if self.docker_image:
             self._write(
                 os.path.join(dest_dir, "docker.sh"),
                 sh_replace(self.template["docker_adm_sh"], replacement_dict),
                 "t",
                 exe=True,
@@ -352,14 +351,31 @@
         )
         self._write(
             os.path.join(dest_dir, "readme.txt"),
             self.template["readme_am"],
             "t",
         )
 
+    def prepare_admin_config(self, admin, ctx):
+        config = json.loads(self.template["fed_admin"])
+        agent_config = dict()
+        if self.overseer_agent:
+            overseer_agent = copy.deepcopy(self.overseer_agent)
+            if overseer_agent.get("overseer_exists", True):
+                overseer_agent["args"] = {
+                    "role": "admin",
+                    "overseer_end_point": ctx.get("overseer_end_point", ""),
+                    "project": self.project_name,
+                    "name": admin.subject,
+                }
+            overseer_agent.pop("overseer_exists", None)
+            agent_config["overseer_agent"] = overseer_agent
+        config["admin"].update(agent_config)
+        return config
+
     def build(self, project, ctx):
         self.template = ctx.get("template")
         self.project_name = project.name
         self.project = project
         overseer = project.get_participants_by_type("overseer")
         if overseer:
             self._build_overseer(overseer, ctx)
```

## nvflare/lighter/impl/workspace.py

```diff
@@ -79,9 +79,9 @@
             print(f"Please clean up {ctx['workspace']} by removing prod_N folders")
             print("After clean-up, rerun the provision command.")
         else:
             current_prod_stage = str(ctx["last_prod_stage"] + 1).zfill(2)
             current_prod_dir = os.path.join(ctx["workspace"], f"prod_{current_prod_stage}")
             shutil.move(self.get_wip_dir(ctx), current_prod_dir)
             ctx.pop("wip_dir", None)
-            print(f"Generated results can be found under {current_prod_dir}.  Builder's wip folder removed.")
+            print(f"Generated results can be found under {current_prod_dir}. ")
             ctx["current_prod_dir"] = current_prod_dir
```

## nvflare/private/aux_runner.py

```diff
@@ -19,15 +19,14 @@
 from nvflare.apis.client import Client
 from nvflare.apis.fl_component import FLComponent
 from nvflare.apis.fl_constant import ReturnCode
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.shareable import ReservedHeaderKey, Shareable, make_reply
 from nvflare.fuel.f3.cellnet.cell import Message, MessageHeaderKey
 from nvflare.fuel.f3.cellnet.cell import ReturnCode as CellReturnCode
-from nvflare.fuel.f3.cellnet.cell import new_message
 from nvflare.fuel.f3.cellnet.fqcn import FQCN
 from nvflare.private.defs import CellChannel
 from nvflare.security.logging import secure_format_traceback
 
 
 class AuxRunner(FLComponent):
     def __init__(self, engine):
@@ -104,15 +103,15 @@
             self.log_error(
                 fl_ctx,
                 f"bad peer_props from client: expects dict but got {type(peer_props)}",
             )
             return make_reply(ReturnCode.BAD_PEER_CONTEXT)
         try:
             reply = handler_f(topic=topic, request=request, fl_ctx=fl_ctx)
-        except Exception:
+        except BaseException:
             self.log_exception(fl_ctx, "processing error in message handling")
             return make_reply(ReturnCode.HANDLER_EXCEPTION)
 
         return reply
 
     def dispatch(self, topic: str, request: Shareable, fl_ctx: FLContext) -> Shareable:
         """This method is to be called by the Engine when an aux message is received from peer.
@@ -183,15 +182,15 @@
                 topic=topic,
                 request=request,
                 timeout=timeout,
                 fl_ctx=fl_ctx,
                 bulk_send=bulk_send,
                 optional=optional,
             )
-        except Exception:
+        except BaseException:
             if optional:
                 self.logger.debug(f"Failed to send aux message {topic} to targets: {targets}")
                 self.logger.debug(secure_format_traceback())
             else:
                 self.logger.error(f"Failed to send aux message {topic} to targets: {targets}")
                 self.logger.error(secure_format_traceback())
             return {}
@@ -247,15 +246,15 @@
             if t not in target_names:
                 target_names.append(t)
 
         target_fqcns = []
         for name in target_names:
             target_fqcns.append(FQCN.join([name, job_id]))
 
-        cell_msg = new_message(payload=request)
+        cell_msg = Message(payload=request)
         if timeout > 0:
             cell_replies = cell.broadcast_request(
                 channel=channel, topic=topic, request=cell_msg, targets=target_fqcns, timeout=timeout, optional=optional
             )
 
             replies = {}
             if cell_replies:
```

## nvflare/private/defs.py

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from nvflare.fuel.f3.message import Headers, Message
+from nvflare.fuel.f3.message import Message
 from nvflare.fuel.hci.server.constants import ConnProps
 
 
 class SpecialTaskName(object):
 
     TRY_AGAIN = "__try_again__"
     END_RUN = "__end_run__"
@@ -173,11 +173,11 @@
     JOB_ID = "job_id"
     JOB_IDS = "job_ids"
     MESSAGE = "message"
     ABORT_JOBS = "abort_jobs"
 
 
 def new_cell_message(headers: dict, payload=None):
-    msg_headers = Headers()
+    msg_headers = {}
     if headers:
         msg_headers.update(headers)
     return Message(msg_headers, payload)
```

## nvflare/private/json_configer.py

```diff
@@ -77,15 +77,15 @@
 
         config_data = {}
         for f in config_files:
             with open(f) as file:
                 try:
                     data = json.load(file)
                     augment(to_dict=config_data, from_dict=data, from_override_to=False)
-                except Exception as e:
+                except BaseException as e:
                     print("Error processing config file {}: {}".format(file, secure_format_exception(e)))
                     raise e
 
         self.config_data = config_data
         self.json_scanner = JsonScanner(config_data, config_files)
 
     def get_module_scanner(self):
```

## nvflare/private/fed/cmi.py

```diff
@@ -16,15 +16,14 @@
 
 from nvflare.apis.fl_component import FLComponent
 from nvflare.apis.fl_constant import FLContextKey, ReturnCode
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.shareable import ReservedHeaderKey, Shareable, make_reply
 from nvflare.fuel.f3.cellnet.cell import FQCN, Cell, Message, MessageHeaderKey
 from nvflare.fuel.f3.cellnet.cell import ReturnCode as CellReturnCode
-from nvflare.fuel.f3.cellnet.cell import new_message
 from nvflare.private.defs import CellMessageHeaderKeys
 
 
 class CellMessageInterface(FLComponent, ABC):
 
     HEADER_KEY_PEER_PROPS = "cmi.peer_props"
     HEADER_JOB_ID = "cmi.job_id"
@@ -62,15 +61,15 @@
         self.cell.add_outgoing_reply_filter(channel="*", topic="*", cb=self._filter_outgoing_message)
 
         self.cell.add_outgoing_request_filter(channel="*", topic="*", cb=self._filter_outgoing_message)
 
         self.cell.add_incoming_reply_filter(channel="*", topic="*", cb=self._filter_incoming_message)
 
     def new_cmi_message(self, fl_ctx: FLContext, headers=None, payload=None):
-        msg = new_message(headers, payload)
+        msg = Message(headers, payload)
         msg.set_prop(self.PROP_KEY_FL_CTX, fl_ctx)
         return msg
 
     def _filter_incoming_message(self, message: Message):
         public_props = message.get_header(self.HEADER_KEY_PEER_PROPS)
         if public_props:
             peer_ctx = self._make_peer_ctx(public_props)
```

## nvflare/private/fed/app/fl_conf.py

```diff
@@ -101,15 +101,15 @@
                     )
                 if server.get(SSLConstants.CERT):
                     server[SSLConstants.CERT] = self.workspace.get_file_path_in_startup(server[SSLConstants.CERT])
                 if server.get(SSLConstants.ROOT_CERT):
                     server[SSLConstants.ROOT_CERT] = self.workspace.get_file_path_in_startup(
                         server[SSLConstants.ROOT_CERT]
                     )
-        except Exception:
+        except BaseException:
             raise ValueError(f"Server config error: '{self.server_config_file_names}'")
 
     def build_component(self, config_dict):
         t = super().build_component(config_dict)
         if isinstance(t, FLComponent):
             if type(t).__name__ not in [type(h).__name__ for h in self.handlers]:
                 self.handlers.append(t)
@@ -295,15 +295,15 @@
                 client[SSLConstants.PRIVATE_KEY] = self.workspace.get_file_path_in_startup(
                     client[SSLConstants.PRIVATE_KEY]
                 )
             if client.get(SSLConstants.CERT):
                 client[SSLConstants.CERT] = self.workspace.get_file_path_in_startup(client[SSLConstants.CERT])
             if client.get(SSLConstants.ROOT_CERT):
                 client[SSLConstants.ROOT_CERT] = self.workspace.get_file_path_in_startup(client[SSLConstants.ROOT_CERT])
-        except Exception:
+        except BaseException:
             raise ValueError(f"Client config error: '{self.client_config_file_names}'")
 
     def finalize_config(self, config_ctx: ConfigContext):
         """Finalize the config process.
 
         Args:
             config_ctx: config context
```

## nvflare/private/fed/app/client/client_train.py

```diff
@@ -62,15 +62,15 @@
     workspace = Workspace(root_dir=args.workspace)
 
     for name in [WorkspaceConstants.RESTART_FILE, WorkspaceConstants.SHUTDOWN_FILE]:
         try:
             f = workspace.get_file_path_in_root(name)
             if os.path.exists(f):
                 os.remove(f)
-        except Exception:
+        except BaseException:
             print("Could not remove the {} file.  Please check your system before starting FL.".format(name))
             sys.exit(-1)
 
     rank = args.local_rank
 
     try:
         os.chdir(args.workspace)
```

## nvflare/private/fed/app/client/sub_worker_process.py

```diff
@@ -47,26 +47,33 @@
 from nvflare.fuel.sec.security_content_service import SecurityContentService
 from nvflare.private.defs import CellChannel, CellChannelTopic, new_cell_message
 from nvflare.private.fed.app.fl_conf import create_privacy_manager
 from nvflare.private.fed.app.utils import monitor_parent_process
 from nvflare.private.fed.client.client_run_manager import ClientRunManager
 from nvflare.private.fed.runner import Runner
 from nvflare.private.fed.simulator.simulator_app_runner import SimulatorClientRunManager
-from nvflare.private.fed.utils.fed_utils import add_logfile_handler, configure_logging, fobs_initialize
+from nvflare.private.fed.utils.fed_utils import (
+    add_logfile_handler,
+    configure_logging,
+    create_stats_pool_files_for_job,
+    fobs_initialize,
+    set_stats_pool_config_for_job,
+)
 from nvflare.private.privacy_manager import PrivacyService
 
 
 class EventRelayer(FLComponent):
     """To relay the event from the worker_process."""
 
     def __init__(self, cell, parent_fqcn, local_rank):
         """To init the EventRelayer.
 
         Args:
-            conn: worker_process connection.
+            cell: the local cell.
+            parent_fqcn: FQCN of the parent cell
             local_rank: process local rank
         """
         super().__init__()
         self.cell = cell
         self.parent_fqcn = parent_fqcn
         self.local_rank = local_rank
 
@@ -121,15 +128,15 @@
                         target=self.parent_fqcn,
                         channel=CellChannel.MULTI_PROCESS_EXECUTOR,
                         topic=CellChannelTopic.FIRE_EVENT,
                         request=request,
                     )
                     # update the fl_ctx from the child process return data.
                     fl_ctx.props.update(return_data.payload[CommunicationMetaData.FL_CTX].props)
-                except Exception:
+                except BaseException:
                     self.log_warning(
                         fl_ctx, f"Failed to relay the event to parent process. Event: {event_type}", fire_event=False
                     )
 
 
 class SubWorkerExecutor(Runner):
     def __init__(self, args, workspace, num_of_processes, local_rank) -> None:
@@ -330,31 +337,38 @@
 
     # configure privacy control!
     privacy_manager = create_privacy_manager(workspace, names_only=True)
 
     # initialize Privacy Service
     PrivacyService.initialize(privacy_manager)
 
-    # local_rank = args.local_rank
     local_rank = int(os.environ["LOCAL_RANK"])
+    prefix = f"rank{local_rank}"
+    set_stats_pool_config_for_job(workspace, args.job_id, prefix=prefix)
+
     num_of_processes = int(args.num_processes)
     sub_executor = SubWorkerExecutor(args, workspace, num_of_processes, local_rank)
 
     # start parent process checking thread
     parent_pid = args.parent_pid
     stop_event = threading.Event()
     thread = threading.Thread(target=monitor_parent_process, args=(sub_executor, parent_pid, stop_event))
     thread.start()
 
     job_id = args.job_id
     log_file = workspace.get_app_log_file_path(job_id)
     add_logfile_handler(log_file)
+    logger = logging.getLogger("sub_worker_process")
 
     sub_executor.run()
+
     AuditService.close()
+    err = create_stats_pool_files_for_job(workspace, job_id, prefix=prefix)
+    if err:
+        logger.warning(err)
 
 
 if __name__ == "__main__":
     """
     This is the program for running rank processes in multi-process mode.
     """
     # main()
```

## nvflare/private/fed/app/client/worker_process.py

```diff
@@ -28,15 +28,20 @@
 from nvflare.fuel.sec.security_content_service import SecurityContentService
 from nvflare.fuel.utils.argument_utils import parse_vars
 from nvflare.private.defs import EngineConstant
 from nvflare.private.fed.app.fl_conf import FLClientStarterConfiger
 from nvflare.private.fed.app.utils import monitor_parent_process
 from nvflare.private.fed.client.client_app_runner import ClientAppRunner
 from nvflare.private.fed.client.client_status import ClientStatus
-from nvflare.private.fed.utils.fed_utils import add_logfile_handler, fobs_initialize
+from nvflare.private.fed.utils.fed_utils import (
+    add_logfile_handler,
+    create_stats_pool_files_for_job,
+    fobs_initialize,
+    set_stats_pool_config_for_job,
+)
 from nvflare.security.logging import secure_format_exception
 
 
 def main():
     """Worker process start program."""
     parser = argparse.ArgumentParser()
     parser.add_argument("--workspace", "-m", type=str, help="WORKSPACE folder", required=True)
@@ -69,32 +74,32 @@
     if config_folder == "":
         args.client_config = JobConstants.CLIENT_JOB_CONFIG
     else:
         args.client_config = os.path.join(config_folder, JobConstants.CLIENT_JOB_CONFIG)
     args.config_folder = config_folder
     args.env = os.path.join("config", "environment.json")
     workspace = Workspace(args.workspace, args.client_name, config_folder)
+    set_stats_pool_config_for_job(workspace, args.job_id)
 
     try:
         remove_restart_file(workspace)
-    except Exception:
+    except BaseException:
         print("Could not remove the restart.fl / shutdown.fl file.  Please check your system before starting FL.")
         sys.exit(-1)
 
     restart_file = workspace.get_file_path_in_root("restart.fl")
     if os.path.exists(restart_file):
         os.remove(restart_file)
 
     fobs_initialize()
     # Initialize audit service since the job execution will need it!
     audit_file_name = workspace.get_audit_file_path()
     AuditService.initialize(audit_file_name)
 
     # print("starting the client .....")
-
     SecurityContentService.initialize(content_folder=workspace.get_startup_kit_dir())
 
     thread = None
     stop_event = threading.Event()
     deployer = None
     client_app_runner = None
     federated_client = None
@@ -131,29 +136,32 @@
         # start parent process checking thread
         thread = threading.Thread(target=monitor_parent_process, args=(client_app_runner, parent_pid, stop_event))
         thread.start()
 
         sp = _create_sp(args)
         client_app_runner.start_run(app_root, args, config_folder, federated_client, secure_train, sp)
 
-    except Exception as e:
+    except BaseException as e:
         if logger:
             logger.error(f"FL client execution exception: {secure_format_exception(e)}")
         raise e
     finally:
         if client_app_runner:
             client_app_runner.close()
         if deployer:
             deployer.close()
         if federated_client:
             federated_client.terminate()
         stop_event.set()
         if thread and thread.is_alive():
             thread.join()
         AuditService.close()
+        err = create_stats_pool_files_for_job(workspace, args.job_id)
+        if err:
+            logger.warning(err)
 
 
 def _create_sp(args):
     sp = SP()
     target = args.sp_target.split(":")
     sp.name = target[0]
     sp.fl_port = target[1]
```

## nvflare/private/fed/app/deployer/simulator_deployer.py

```diff
@@ -139,15 +139,15 @@
 
         resources = os.path.join(args.workspace, "local/resources.json")
         if os.path.exists(resources):
             with open(resources) as file:
                 try:
                     data = json.load(file)
                     augment(to_dict=client_config, from_dict=data, from_override_to=False)
-                except Exception as e:
+                except BaseException as e:
                     raise RuntimeError(f"Error processing config file {resources}: {secure_format_exception(e)}")
 
         build_ctx = {
             "client_name": client_name,
             "server_config": client_config.get("servers", []),
             "client_config": client_config["client"],
             "server_host": None,
```

## nvflare/private/fed/app/server/runner_process.py

```diff
@@ -28,15 +28,20 @@
 from nvflare.fuel.sec.security_content_service import SecurityContentService
 from nvflare.fuel.utils.argument_utils import parse_vars
 from nvflare.private.defs import AppFolderConstants
 from nvflare.private.fed.app.fl_conf import FLServerStarterConfiger
 from nvflare.private.fed.app.utils import monitor_parent_process
 from nvflare.private.fed.server.server_app_runner import ServerAppRunner
 from nvflare.private.fed.server.server_state import HotState
-from nvflare.private.fed.utils.fed_utils import add_logfile_handler, fobs_initialize
+from nvflare.private.fed.utils.fed_utils import (
+    add_logfile_handler,
+    create_stats_pool_files_for_job,
+    fobs_initialize,
+    set_stats_pool_config_for_job,
+)
 from nvflare.security.logging import secure_format_exception, secure_log_traceback
 
 
 def main():
     """FL Server program starting point."""
     parser = argparse.ArgumentParser()
     parser.add_argument("--workspace", "-m", type=str, help="WORKSPACE folder", required=True)
@@ -69,14 +74,16 @@
     args.log_config = None
     args.snapshot = kv_list.get("restore_snapshot")
 
     # get parent process id
     parent_pid = os.getppid()
     stop_event = threading.Event()
     workspace = Workspace(root_dir=args.workspace, site_name="server")
+    set_stats_pool_config_for_job(workspace, args.job_id)
+
     app_custom_folder = workspace.get_client_custom_dir()
     if os.path.isdir(app_custom_folder):
         sys.path.append(app_custom_folder)
 
     try:
         os.chdir(args.workspace)
         fobs_initialize()
@@ -133,14 +140,17 @@
 
             server_app_runner.start_server_app(workspace, args, args.app_root, args.job_id, snapshot, logger, args.set)
         finally:
             if deployer:
                 deployer.close()
             stop_event.set()
             AuditService.close()
+            err = create_stats_pool_files_for_job(workspace, args.job_id)
+            if err:
+                logger.warning(err)
 
     except ConfigError as e:
         logger = logging.getLogger("runner_process")
         logger.exception(f"ConfigError: {secure_format_exception(e)}")
         secure_log_traceback(logger)
         raise e
```

## nvflare/private/fed/app/server/server_train.py

```diff
@@ -62,15 +62,15 @@
 
     workspace = Workspace(root_dir=args.workspace, site_name="server")
     for name in [WorkspaceConstants.RESTART_FILE, WorkspaceConstants.SHUTDOWN_FILE]:
         try:
             f = workspace.get_file_path_in_root(name)
             if os.path.exists(f):
                 os.remove(f)
-        except Exception:
+        except BaseException:
             print(f"Could not remove file '{name}'.  Please check your system before starting FL.")
             sys.exit(-1)
 
     try:
         os.chdir(args.workspace)
 
         fobs_initialize()
```

## nvflare/private/fed/app/simulator/simulator_runner.py

```diff
@@ -34,26 +34,26 @@
 from nvflare.apis.workspace import Workspace
 from nvflare.fuel.common.multi_process_executor_constants import CommunicationMetaData
 from nvflare.fuel.f3.mpm import MainProcessMonitor as mpm
 from nvflare.fuel.f3.stats_pool import StatsPoolManager
 from nvflare.fuel.hci.server.authz import AuthorizationService
 from nvflare.fuel.sec.audit import AuditService
 from nvflare.fuel.utils.argument_utils import parse_vars
+from nvflare.fuel.utils.gpu_utils import get_host_gpu_ids
 from nvflare.fuel.utils.network_utils import get_open_ports
 from nvflare.fuel.utils.zip_utils import split_path, unzip_all_from_bytes, zip_directory_to_bytes
-from nvflare.lighter.poc_commands import get_host_gpu_ids
 from nvflare.private.defs import AppFolderConstants
 from nvflare.private.fed.app.deployer.simulator_deployer import SimulatorDeployer
 from nvflare.private.fed.app.utils import kill_child_processes
 from nvflare.private.fed.client.client_status import ClientStatus
 from nvflare.private.fed.server.job_meta_validator import JobMetaValidator
 from nvflare.private.fed.simulator.simulator_app_runner import SimulatorServerAppRunner
 from nvflare.private.fed.simulator.simulator_audit import SimulatorAuditor
 from nvflare.private.fed.simulator.simulator_const import SimulatorConstants
-from nvflare.private.fed.utils.fed_utils import add_logfile_handler, fobs_initialize
+from nvflare.private.fed.utils.fed_utils import add_logfile_handler, fobs_initialize, split_gpus
 from nvflare.security.logging import secure_format_exception
 from nvflare.security.security import EmptyAuthorizer
 
 CLIENT_CREATE_POOL_SIZE = 200
 POOL_STATS_DIR = "pool_stats"
 SIMULATOR_POOL_STATS = "simulator_cell_stats.json"
 
@@ -171,35 +171,41 @@
                 self.logger.error(
                     f"The number of clients ({len(self.client_names)}) can not be more than the "
                     f"max_number of clients ({self.max_clients})"
                 )
                 return False
 
             if self.args.gpu:
-                gpus = self.args.gpu.split(",")
+                try:
+                    gpu_groups = split_gpus(self.args.gpu)
+                except ValueError as e:
+                    self.logger.error(f"GPUs group list option in wrong format. Error: {e}")
+                    return False
+
                 host_gpus = [str(x) for x in (get_host_gpu_ids())]
-                if host_gpus and not set(gpus).issubset(host_gpus):
-                    wrong_gpus = [x for x in gpus if x not in host_gpus]
+                gpu_ids = [x.split(",") for x in gpu_groups]
+                if host_gpus and not set().union(*gpu_ids).issubset(host_gpus):
+                    wrong_gpus = [x for x in gpu_groups if x not in host_gpus]
                     self.logger.error(f"These GPUs are not available: {wrong_gpus}")
                     return False
 
-                if len(gpus) > len(self.client_names):
+                if len(gpu_groups) > len(self.client_names):
                     self.logger.error(
                         f"The number of clients ({len(self.client_names)}) must be larger than or equal to "
-                        f"the number of GPUS: ({len(gpus)})"
+                        f"the number of GPU groups: ({len(gpu_groups)})"
                     )
                     return False
-                if len(gpus) > 1:
+                if len(gpu_groups) > 1:
                     if self.args.threads and self.args.threads > 1:
                         self.logger.info(
-                            "When running with multi GPU, each GPU will run with only 1 thread. "
+                            "When running with multi GPU, each GPU group will run with only 1 thread. "
                             "Set the Threads to 1."
                         )
                     self.args.threads = 1
-                elif len(gpus) == 1:
+                elif len(gpu_groups) == 1:
                     if self.args.threads is None:
                         self.args.threads = 1
                         self.logger.warn("The number of threads is not provided. Set it to default: 1")
 
             if self.args.threads and self.args.threads > len(self.client_names):
                 self.logger.error("The number of threads to run can not be larger than the number of clients.")
                 return False
@@ -215,15 +221,15 @@
             # self.services.deploy(self.args, grpc_args=simulator_server)
 
             self.logger.info("Deploy the Apps.")
             self._deploy_apps(job_name, data_bytes, meta)
 
             return True
 
-        except Exception as e:
+        except BaseException as e:
             self.logger.error(f"Simulator setup error: {secure_format_exception(e)}")
             return False
 
     def validate_job_data(self):
         # Validate the simulate job
         job_name = split_path(self.args.job_folder)[1]
         data = zip_directory_to_bytes("", self.args.job_folder)
@@ -232,25 +238,25 @@
         valid, error, meta = job_validator.validate(job_name, data_bytes)
         if not valid:
             raise RuntimeError(error)
         return data_bytes, job_name, meta
 
     def _extract_client_names_from_meta(self, meta):
         client_names = []
-        for _, participants in meta.get(JobMetaKey.DEPLOY_MAP).items():
+        for _, participants in meta.get(JobMetaKey.DEPLOY_MAP, {}).items():
             for p in participants:
                 if p.upper() != ALL_SITES and p != "server":
                     client_names.append(p)
         return client_names
 
     def _validate_client_names(self, meta, client_names):
         no_app_clients = []
         for name in client_names:
             name_matched = False
-            for app_name, participants in meta.get(JobMetaKey.DEPLOY_MAP).items():
+            for _, participants in meta.get(JobMetaKey.DEPLOY_MAP, {}).items():
                 if len(participants) == 1 and participants[0].upper() == ALL_SITES:
                     name_matched = True
                     break
                 if name in participants:
                     name_matched = True
                     break
             if not name_matched:
@@ -277,14 +283,18 @@
                         app = os.path.join(temp_job_folder, app_name)
                         shutil.copytree(app, app_server_root)
                     elif p in self.client_names:
                         app_client_root = os.path.join(self.simulator_root, "app_" + p)
                         app = os.path.join(temp_job_folder, app_name)
                         shutil.copytree(app, app_client_root)
 
+            job_meta_file = os.path.join(self.simulator_root, WorkspaceConstants.JOB_META_FILE)
+            with open(job_meta_file, "w") as f:
+                json.dump(meta, f, indent=4)
+
     def split_clients(self, clients: [], gpus: []):
         split_clients = []
         for _ in gpus:
             split_clients.append([])
         index = 0
         for client in clients:
             split_clients[index % len(gpus)].append(client)
@@ -365,15 +375,15 @@
                         raise RuntimeError("Could not start the Server App.")
 
                 # # Start the client heartbeat calls.
                 # for client in self.federated_clients:
                 #     client.start_heartbeat(interval=2)
 
                 if self.args.gpu:
-                    gpus = self.args.gpu.split(",")
+                    gpus = split_gpus(self.args.gpu)
                     split_clients = self.split_clients(self.federated_clients, gpus)
                 else:
                     gpus = [None]
                     split_clients = [self.federated_clients]
 
                 executor = ThreadPoolExecutor(max_workers=len(gpus))
                 for index in range(len(gpus)):
@@ -381,15 +391,15 @@
                     executor.submit(lambda p: self.client_run(*p), [clients, gpus[index]])
 
                 executor.shutdown()
                 # Abort the server after all clients finished run
                 self.server.abort_run()
                 server_thread.join()
                 run_status = 0
-            except Exception as e:
+            except BaseException as e:
                 self.logger.error(f"Simulator run error: {secure_format_exception(e)}")
                 run_status = 2
             finally:
                 # self.services.close()
                 self.deployer.close()
         else:
             run_status = 1
@@ -466,15 +476,15 @@
             lock = threading.Lock()
             timeout = self.kv_list.get("simulator_worker_timeout", 60.0)
             for i in range(self.args.threads):
                 executor.submit(lambda p: self.run_client_thread(*p), [self.args.threads, gpu, lock, timeout])
 
             # wait for the server and client running thread to finish.
             executor.shutdown()
-        except Exception as e:
+        except BaseException as e:
             self.logger.error(f"SimulatorClientRunner run error: {secure_format_exception(e)}")
         finally:
             for client in self.federated_clients:
                 threading.Thread(target=self._shutdown_client, args=[client]).start()
 
     def _shutdown_client(self, client):
         try:
@@ -494,23 +504,23 @@
         client_to_run = None  # indicates the next client to run
 
         try:
             while not stop_run:
                 time.sleep(interval)
                 with lock:
                     if not client_to_run:
-                        client = self.get_next_run_client()
+                        client = self.get_next_run_client(gpu)
                     else:
                         client = client_to_run
 
                 client.simulate_running = True
                 stop_run, client_to_run = self.do_one_task(client, num_of_threads, gpu, lock, timeout=timeout)
 
                 client.simulate_running = False
-        except Exception as e:
+        except BaseException as e:
             self.logger.error(f"run_client_thread error: {secure_format_exception(e)}")
 
     def do_one_task(self, client, num_of_threads, gpu, lock, timeout=60.0):
         open_port = get_open_ports(1)[0]
         command = (
             sys.executable
             + " -m nvflare.private.fed.app.simulator.simulator_worker -o "
@@ -528,15 +538,20 @@
             + " --root_url "
             + str(client.cell.get_root_url_for_child())
             + " --parent_url "
             + str(client.cell.get_internal_listener_url())
         )
         if gpu:
             command += " --gpu " + str(gpu)
-        _ = subprocess.Popen(shlex.split(command, True), preexec_fn=os.setsid, env=os.environ.copy())
+        new_env = os.environ.copy()
+        if not sys.path[0]:
+            new_env["PYTHONPATH"] = os.pathsep.join(sys.path[1:])
+        else:
+            new_env["PYTHONPATH"] = os.pathsep.join(sys.path)
+        _ = subprocess.Popen(shlex.split(command, True), preexec_fn=os.setsid, env=new_env)
 
         conn = self._create_connection(open_port, timeout=timeout)
 
         self.build_ctx["client_name"] = client.client_name
         data = {
             # SimulatorConstants.CLIENT: client,
             SimulatorConstants.CLIENT_CONFIG: self.client_config,
@@ -546,15 +561,15 @@
         conn.send(data)
 
         while True:
             stop_run = conn.recv()
 
             with lock:
                 if num_of_threads != len(self.federated_clients):
-                    next_client = self.get_next_run_client()
+                    next_client = self.get_next_run_client(gpu)
                 else:
                     next_client = client
             if not stop_run and next_client.client_name == client.client_name:
                 conn.send(True)
             else:
                 conn.send(False)
                 break
@@ -564,26 +579,26 @@
     def _create_connection(self, open_port, timeout=60.0):
         conn = None
         start = time.time()
         while not conn:
             try:
                 address = ("localhost", open_port)
                 conn = Client(address, authkey=CommunicationMetaData.CHILD_PASSWORD.encode())
-            except Exception:
+            except BaseException:
                 if time.time() - start > timeout:
                     raise RuntimeError(
                         f"Failed to create connection to the child process in {self.__class__.__name__},"
                         f" timeout: {timeout}"
                     )
                 time.sleep(1.0)
                 pass
         return conn
 
-    def get_next_run_client(self):
+    def get_next_run_client(self, gpu):
         # Find the next client which is not currently running
         while True:
             self.run_client_index = (self.run_client_index + 1) % len(self.federated_clients)
             client = self.federated_clients[self.run_client_index]
             if not client.simulate_running:
                 break
-        self.logger.info(f"Simulate Run client: {client.client_name}")
+        self.logger.info(f"Simulate Run client: {client.client_name} on GPU group: {gpu}")
         return client
```

## nvflare/private/fed/app/simulator/simulator_worker.py

```diff
@@ -148,15 +148,15 @@
 
                 continue_run = conn.recv()
                 if not continue_run:
                     self.release_resources(client)
                     break
                 time.sleep(interval)
 
-        except Exception as e:
+        except BaseException as e:
             self.logger.error(f"ClientTaskWorker run error: {secure_format_exception(e)}")
         finally:
             if client:
                 client.cell.stop()
             if admin_agent:
                 admin_agent.shutdown()
```

## nvflare/private/fed/client/admin.py

```diff
@@ -146,13 +146,13 @@
                     reply = processor.process(req, self.app_ctx)
                     if reply is None:
                         # simply ack
                         reply = ok_reply()
                     else:
                         if not isinstance(reply, Message):
                             raise RuntimeError(f"processor for topic {topic} failed to produce valid reply")
-            except Exception as e:
+            except BaseException as e:
                 secure_log_traceback()
                 reply = error_reply(f"exception_occurred: {secure_format_exception(e)}")
         else:
             reply = error_reply("invalid_request")
         return new_cell_message({}, reply)
```

## nvflare/private/fed/client/client_engine.py

```diff
@@ -17,20 +17,21 @@
 import re
 import shutil
 import sys
 import threading
 
 from nvflare.apis.event_type import EventType
 from nvflare.apis.fl_component import FLComponent
-from nvflare.apis.fl_constant import MachineStatus, WorkspaceConstants
+from nvflare.apis.fl_constant import MachineStatus, SystemComponents, WorkspaceConstants
 from nvflare.apis.fl_context import FLContext, FLContextManager
 from nvflare.apis.workspace import Workspace
 from nvflare.fuel.utils.network_utils import get_open_ports
 from nvflare.private.defs import ERROR_MSG_PREFIX, ClientStatusKey, EngineConstant
 from nvflare.private.event import fire_event
+from nvflare.private.fed.server.job_meta_validator import JobMetaValidator
 from nvflare.private.fed.utils.app_deployer import AppDeployer
 from nvflare.private.fed.utils.fed_utils import security_close
 from nvflare.security.logging import secure_format_exception, secure_log_traceback
 
 from .client_engine_internal_spec import ClientEngineInternalSpec
 from .client_executor import ProcessExecutor
 from .client_run_manager import ClientRunInfo
@@ -62,15 +63,22 @@
         self.client_name = client_name
         self.args = args
         self.rank = rank
         self.client_executor = ProcessExecutor(client, os.path.join(args.workspace, "startup"))
         self.admin_agent = None
 
         self.fl_ctx_mgr = FLContextManager(
-            engine=self, identity_name=client_name, job_id="", public_stickers={}, private_stickers={}
+            engine=self,
+            identity_name=client_name,
+            job_id="",
+            public_stickers={},
+            private_stickers={
+                SystemComponents.DEFAULT_APP_DEPLOYER: AppDeployer(),
+                SystemComponents.JOB_META_VALIDATOR: JobMetaValidator(),
+            },
         )
 
         self.status = MachineStatus.STOPPED
 
         if workers < 1:
             raise ValueError("workers must >= 1")
         self.logger = logging.getLogger(self.__class__.__name__)
@@ -218,20 +226,28 @@
         self.fire_event(EventType.SYSTEM_END, self.new_context())
         thread = threading.Thread(target=shutdown_client, args=(self.client, touch_file))
         thread.start()
 
         return "Restart the client..."
 
     def deploy_app(self, app_name: str, job_id: str, job_meta: dict, client_name: str, app_data) -> str:
-
         workspace = Workspace(root_dir=self.args.workspace, site_name=client_name)
-        app_deployer = AppDeployer(
-            workspace=workspace, job_id=job_id, job_meta=job_meta, app_name=app_name, app_data=app_data
+        app_deployer = self.get_component(SystemComponents.APP_DEPLOYER)
+        if not app_deployer:
+            # use default deployer
+            app_deployer = AppDeployer()
+
+        err = app_deployer.deploy(
+            workspace=workspace,
+            job_id=job_id,
+            job_meta=job_meta,
+            app_name=app_name,
+            app_data=app_data,
+            fl_ctx=self.new_context(),
         )
-        err = app_deployer.deploy()
         if err:
             return f"{ERROR_MSG_PREFIX}: {err}"
 
         return ""
 
     def delete_run(self, job_id: str) -> str:
         job_id_folder = os.path.join(self.args.workspace, WorkspaceConstants.WORKSPACE_PREFIX + str(job_id))
@@ -261,10 +277,10 @@
         federated_client.communicator.heartbeat_done = True
         # time.sleep(3)
         federated_client.close()
 
         federated_client.status = ClientStatus.STOPPED
         # federated_client.cell.stop()
         security_close()
-    except Exception as e:
+    except BaseException as e:
         secure_log_traceback()
         print(f"Failed to shutdown client: {secure_format_exception(e)}")
```

## nvflare/private/fed/client/client_runner.py

```diff
@@ -165,14 +165,18 @@
                 ref=server_audit_event_id,
                 fl_ctx=fl_ctx,
                 msg=f"submit result: {ReturnCode.RUN_MISMATCH}",
             )
 
         executor = self.task_table.get(task.name)
         if not executor:
+            # try default
+            executor = self.task_table.get("*")
+
+        if not executor:
             self.log_error(fl_ctx, f"bad task assignment: no executor available for task {task.name}")
             return self._reply_and_audit(
                 reply=make_reply(ReturnCode.TASK_UNKNOWN),
                 ref=server_audit_event_id,
                 fl_ctx=fl_ctx,
                 msg=f"submit result: {ReturnCode.TASK_UNKNOWN}",
             )
@@ -206,15 +210,15 @@
                     fl_ctx.set_job_is_unsafe()
                     return self._reply_and_audit(
                         reply=make_reply(ReturnCode.UNSAFE_JOB),
                         ref=server_audit_event_id,
                         fl_ctx=fl_ctx,
                         msg=f"submit result: {ReturnCode.UNSAFE_JOB}",
                     )
-                except Exception as e:
+                except BaseException as e:
                     self.log_exception(
                         fl_ctx, f"Processing error from Task Data Filter {filter_name}: {secure_format_exception(e)}"
                     )
                     return self._reply_and_audit(
                         reply=make_reply(ReturnCode.TASK_DATA_FILTER_ERROR),
                         ref=server_audit_event_id,
                         fl_ctx=fl_ctx,
@@ -298,15 +302,15 @@
             fl_ctx.set_job_is_unsafe()
             return self._reply_and_audit(
                 reply=make_reply(ReturnCode.UNSAFE_JOB),
                 ref=server_audit_event_id,
                 fl_ctx=fl_ctx,
                 msg=f"submit result: {ReturnCode.UNSAFE_JOB}",
             )
-        except Exception as e:
+        except BaseException as e:
             self.log_exception(fl_ctx, f"Processing error from executor {executor_name}: {secure_format_exception(e)}")
             return self._reply_and_audit(
                 reply=make_reply(ReturnCode.EXECUTION_EXCEPTION),
                 ref=server_audit_event_id,
                 fl_ctx=fl_ctx,
                 msg=f"submit result: {ReturnCode.EXECUTION_EXCEPTION}",
             )
@@ -338,15 +342,15 @@
                     fl_ctx.set_job_is_unsafe()
                     return self._reply_and_audit(
                         reply=make_reply(ReturnCode.UNSAFE_JOB),
                         ref=server_audit_event_id,
                         fl_ctx=fl_ctx,
                         msg=f"submit result: {ReturnCode.UNSAFE_JOB}",
                     )
-                except Exception as e:
+                except BaseException as e:
                     self.log_exception(
                         fl_ctx, f"Processing error in Task Result Filter {filter_name}: {secure_format_exception(e)}"
                     )
                     return self._reply_and_audit(
                         reply=make_reply(ReturnCode.TASK_RESULT_FILTER_ERROR),
                         ref=server_audit_event_id,
                         fl_ctx=fl_ctx,
@@ -465,15 +469,15 @@
         return task_fetch_interval, True
 
     def run(self, app_root, args):
         self.init_run(app_root, args)
 
         try:
             self._try_run()
-        except Exception as e:
+        except BaseException as e:
             with self.engine.new_context() as fl_ctx:
                 self.log_exception(fl_ctx, f"processing error in RUN execution: {secure_format_exception(e)}")
         finally:
             # in case any task is still running, abort it
             self._abort_current_task()
             self.end_run_events_sequence("run method")
```

## nvflare/private/fed/client/communicator.py

```diff
@@ -139,15 +139,15 @@
                 token = result.get_header(CellMessageHeaderKeys.TOKEN)
                 ssid = result.get_header(CellMessageHeaderKeys.SSID)
                 if not token and not self.should_stop:
                     time.sleep(self.client_register_interval)
                 else:
                     break
 
-            except Exception as ex:
+            except BaseException as ex:
                 raise FLCommunicationError("error:client_registration", ex)
 
         return token, ssid
 
     def pull_task(self, servers, project_name, token, ssid, fl_ctx: FLContext):
         """Get a task from server.
 
@@ -191,15 +191,15 @@
         end_time = time.time()
         return_code = task.get_header(MessageHeaderKey.RETURN_CODE)
 
         if return_code == ReturnCode.OK:
             size = len(task.payload)
             task.payload = fobs.loads(task.payload)
             task_name = task.payload.get_header(ServerCommandKey.TASK_NAME)
-            fl_ctx.set_prop(FLContextKey.SSID, ssid)
+            fl_ctx.set_prop(FLContextKey.SSID, ssid, sticky=False)
             if task_name not in [SpecialTaskName.END_RUN, SpecialTaskName.TRY_AGAIN]:
                 self.logger.info(
                     f"Received from {project_name} server "
                     f" ({size} Bytes). getTask: {task_name} time: {end_time - start_time} seconds"
                 )
         elif return_code == ReturnCode.AUTHENTICATION_ERROR:
             self.logger.warning("get_task request authentication failed.")
@@ -303,15 +303,15 @@
             )
             return_code = result.get_header(MessageHeaderKey.RETURN_CODE)
             if return_code == ReturnCode.UNAUTHENTICATED:
                 self.logger.info(f"Client token: {token} has been removed from the server.")
 
             server_message = result.get_header(CellMessageHeaderKeys.MESSAGE)
 
-        except Exception as ex:
+        except BaseException as ex:
             raise FLCommunicationError("error:client_quit", ex)
 
         return server_message
 
     def send_heartbeat(self, servers, task_name, token, ssid, client_name, engine: ClientEngineInternalSpec, interval):
         fl_ctx = engine.new_context()
         simulate_mode = fl_ctx.get_prop(FLContextKey.SIMULATE_MODE, False)
@@ -346,22 +346,22 @@
                         # server_message = result.get_header(CellMessageHeaderKeys.MESSAGE)
                         abort_jobs = result.get_header(CellMessageHeaderKeys.ABORT_JOBS, [])
                         self._clean_up_runs(engine, abort_jobs)
                     else:
                         if return_code != ReturnCode.OK:
                             break
 
-                except Exception as ex:
+                except BaseException as ex:
                     raise FLCommunicationError("error:client_quit", ex)
 
                 for i in range(wait_times):
                     time.sleep(2)
                     if self.heartbeat_done:
                         break
-            except Exception as e:
+            except BaseException as e:
                 self.logger.info(f"Failed to send heartbeat. Will try again. Exception: {secure_format_exception(e)}")
                 time.sleep(5)
 
     def _clean_up_runs(self, engine, abort_runs):
         # abort_runs = list(set(response.abort_jobs))
         display_runs = ",".join(abort_runs)
         try:
```

## nvflare/private/fed/client/scheduler_cmds.py

```diff
@@ -75,15 +75,15 @@
                 if block_reason:
                     is_resource_enough = False
                     token = block_reason
                 else:
                     is_resource_enough, token = resource_manager.check_resources(
                         resource_requirement=resource_spec, fl_ctx=fl_ctx
                     )
-            except Exception:
+            except BaseException:
                 result.set_return_code(ReturnCode.EXECUTION_EXCEPTION)
 
         result.set_header(ShareableHeader.IS_RESOURCE_ENOUGH, is_resource_enough)
         result.set_header(ShareableHeader.RESOURCE_RESERVE_TOKEN, token)
 
         return Message(topic="reply_" + req.topic, body=fobs.dumps(result))
```

## nvflare/private/fed/client/training_cmds.py

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
 from typing import List
 
+from nvflare.apis.job_def import JobMetaKey
 from nvflare.apis.workspace import Workspace
 from nvflare.fuel.hci.proto import MetaStatusValue, make_meta
 from nvflare.fuel.utils.argument_utils import parse_vars
 from nvflare.lighter.utils import verify_folder_signature
 from nvflare.private.admin_defs import Message, error_reply, ok_reply
 from nvflare.private.defs import RequestHeader, ScopeInfoKey, TrainingTopic
 from nvflare.private.fed.client.admin import RequestProcessor
@@ -114,28 +115,30 @@
         job_meta = json.loads(req.get_header(RequestHeader.JOB_META))
         app_name = req.get_header(RequestHeader.APP_NAME)
         client_name = engine.get_client_name()
 
         if not job_meta:
             return error_reply("missing job meta")
 
-        err = engine.deploy_app(
-            app_name=app_name, job_id=job_id, job_meta=job_meta, client_name=client_name, app_data=req.body
-        )
-        if err:
-            return error_reply(err)
-
         kv_list = parse_vars(engine.args.set)
         secure_train = kv_list.get("secure_train", True)
-        if secure_train:
+        from_hub_site = job_meta.get(JobMetaKey.FROM_HUB_SITE.value)
+        if secure_train and not from_hub_site:
             workspace = Workspace(root_dir=engine.args.workspace, site_name=client_name)
             app_path = workspace.get_app_dir(job_id)
             root_ca_path = os.path.join(workspace.get_startup_kit_dir(), "rootCA.pem")
             if not verify_folder_signature(app_path, root_ca_path):
                 return error_reply(f"app {app_name} does not pass signature verification")
+
+        err = engine.deploy_app(
+            app_name=app_name, job_id=job_id, job_meta=job_meta, client_name=client_name, app_data=req.body
+        )
+        if err:
+            return error_reply(err)
+
         return ok_reply(body=f"deployed {app_name} to {client_name}")
 
 
 class DeleteRunNumberProcessor(RequestProcessor):
     def get_topics(self) -> List[str]:
         return [TrainingTopic.DELETE_RUN]
```

## nvflare/private/fed/server/cmd_utils.py

```diff
@@ -10,19 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
 
-from nvflare.apis.fl_constant import AdminCommandNames
-from nvflare.apis.job_def import JobMetaKey
+from nvflare.apis.job_def import JobMetaKey, is_valid_job_id
 from nvflare.apis.server_engine_spec import ServerEngineSpec
 from nvflare.fuel.hci.conn import Connection
-from nvflare.fuel.hci.proto import MetaStatusValue, make_meta
+from nvflare.fuel.hci.proto import MetaKey, MetaStatusValue, make_meta
 from nvflare.fuel.hci.server.authz import PreAuthzReturnCode
 from nvflare.fuel.hci.server.constants import ConnProps
 from nvflare.private.fed.server.admin import FedAdminServer
 
 
 class CommandUtil(object):
 
@@ -50,21 +49,28 @@
             conn.append_error(err)
             return PreAuthzReturnCode.ERROR
 
         return PreAuthzReturnCode.REQUIRE_AUTHZ
 
     def authorize_abort_client_task(self, conn: Connection, args: List[str]) -> PreAuthzReturnCode:
         if len(args) < 2:
-            conn.append_error("missing job_id (syntax is: abort_task job_id <client-name>)")
+            conn.append_error(
+                "missing job_id (syntax is: abort_task job_id <client-name>)",
+                meta=make_meta(MetaStatusValue.SYNTAX_ERROR, "missing job_id"),
+            )
             return PreAuthzReturnCode.ERROR
 
         auth_args = [args[0], self.TARGET_TYPE_CLIENT]
         auth_args.extend(args[2:])
 
         job_id = args[1].lower()
+        if not is_valid_job_id(job_id):
+            conn.append_error(f"invalid job_id {job_id}", meta=make_meta(MetaStatusValue.INVALID_JOB_ID, job_id))
+            return PreAuthzReturnCode.ERROR
+
         conn.set_prop(self.JOB_ID, job_id)
 
         err = self.validate_command_targets(conn, auth_args[1:])
         if err:
             conn.append_error(err)
             return PreAuthzReturnCode.ERROR
 
@@ -130,19 +136,17 @@
         # else:
         #     client_names = []
         conn.set_prop(self.TARGET_CLIENT_NAMES, client_names)
         conn.set_prop(self.TARGET_CLIENTS, all_clients)
         return ""
 
     def must_be_project_admin(self, conn: Connection, args: List[str]):
-        if args[0] == AdminCommandNames.ADMIN_CHECK_STATUS and len(args) == 1:
-            args.extend(["server"])
         role = conn.get_prop(ConnProps.USER_ROLE, "")
-        if role != "project_admin":
-            conn.append_error("Not authorized as project_admin.", meta=make_meta(MetaStatusValue.NOT_AUTHORIZED))
+        if role not in ["project_admin"]:
+            conn.append_error(f"Not authorized for {role}", meta=make_meta(MetaStatusValue.NOT_AUTHORIZED))
             return PreAuthzReturnCode.ERROR
         else:
             return PreAuthzReturnCode.OK
 
     def authorize_server_operation(self, conn: Connection, args: List[str]):
         err = self.validate_command_targets(conn, args[1:])
         if err:
@@ -162,15 +166,18 @@
             return None
 
         requests = {}
         for token in client_tokens:
             requests.update({token: message})
 
         admin_server: FedAdminServer = conn.server
-        replies = admin_server.send_requests(requests, timeout_secs=admin_server.timeout)
+        cmd_timeout = conn.get_prop(ConnProps.CMD_TIMEOUT)
+        if not cmd_timeout:
+            cmd_timeout = admin_server.timeout
+        replies = admin_server.send_requests(requests, timeout_secs=cmd_timeout)
 
         return replies
 
     @staticmethod
     def get_job_name(meta: dict) -> str:
         """Gets job name from job meta."""
 
@@ -186,22 +193,21 @@
         Args:
             conn: A Connection object.
             replies: replies from clients
         """
         if not replies:
             conn.append_string("no responses from clients")
 
-        engine = conn.app_ctx
         table = conn.append_table(["Client", "Response"])
         for r in replies:
             if r.reply:
                 resp = r.reply.body
             else:
                 resp = ""
-            client_name = engine.get_client_name_from_token(r.client_token)
+            client_name = r.client_name
             if not client_name:
                 clients = conn.get_prop(self.TARGET_CLIENTS)
                 client_name = clients.get(r.client_token, "")
 
             table.add_row([client_name, resp])
 
     def _process_replies_to_string(self, conn: Connection, replies) -> str:
@@ -210,19 +216,23 @@
         Args:
             conn: A Connection object.
             replies: replies from clients
 
         Returns:
             A string response.
         """
-        engine = conn.app_ctx
         response = "no responses from clients"
+        client_replies = {}
         if replies:
             response = ""
             for r in replies:
-                client_name = engine.get_client_name_from_token(r.client_token)
+                client_name = r.client_name
                 response += "client:" + client_name
                 if r.reply:
                     response += " : " + r.reply.body + "\n"
+                    client_replies[client_name] = r.reply.body
                 else:
                     response += " : No replies\n"
+                    client_replies[client_name] = MetaStatusValue.NO_REPLY
+
+        conn.update_meta({MetaKey.CLIENT_STATUS: client_replies})
         return response
```

## nvflare/private/fed/server/fed_server.py

```diff
@@ -561,15 +561,15 @@
                 self.cell.fire_and_forget(
                     targets=fqcn,
                     channel=CellChannel.SERVER_COMMAND,
                     topic=ServerCommandNames.HANDLE_DEAD_JOB,
                     message=request,
                     optional=True,
                 )
-        except Exception:
+        except BaseException:
             self.logger.info("Could not connect to server runner process")
 
     def notify_dead_client(self, client):
         """Called to do further processing of the dead client
 
         Args:
             client: the dead client
@@ -660,15 +660,15 @@
             if self.server_runner:
                 self.server_runner.abort(fl_ctx)
 
     def run_engine(self):
         self.engine.engine_info.status = MachineStatus.STARTED
         try:
             self.server_runner.run()
-        except Exception as e:
+        except BaseException as e:
             self.logger.error(f"FL server execution exception: {secure_format_exception(e)}")
         finally:
             # self.engine.update_job_run_status()
             self.stop_run_engine_cell()
 
         self.engine.engine_info.status = MachineStatus.STOPPED
 
@@ -725,17 +725,15 @@
             with self.engine.new_context() as fl_ctx:
                 self.server_state = self.server_state.handle_sd_callback(sp, fl_ctx)
 
         if isinstance(self.server_state, Cold2HotState):
             self._turn_to_hot()
 
         elif isinstance(self.server_state, Hot2ColdState):
-            self._turn_to_cold()
-
-        self._notify_state_change(old_state_name)
+            self._turn_to_cold(old_state_name)
 
     def _notify_state_change(self, old_state_name):
         new_state_name = self.server_state.__class__.__name__
         if new_state_name != old_state_name:
             self.logger.info(f"state changed from: {old_state_name} to: {new_state_name}")
             keys = list(self.engine.run_processes.keys())
             if keys:
@@ -756,22 +754,23 @@
         if self.checking_server_state:
             self.logger.debug("busy checking server state")
             return
 
         self.checking_server_state = True
         try:
             self._check_server_state(overseer_agent)
-        except Exception as ex:
+        except BaseException as ex:
             self.logger.error(f"exception in checking server state: {secure_format_exception(ex)}")
         finally:
             self.checking_server_state = False
 
     def _turn_to_hot(self):
         # Restore Snapshot
         if self.ha_mode:
+            restored_job_ids = []
             with self.snapshot_lock:
                 fl_snapshot = self.snapshot_persistor.retrieve()
                 if fl_snapshot:
                     for run_number, snapshot in fl_snapshot.run_snapshots.items():
                         if snapshot and not snapshot.completed:
                             # Restore the workspace
                             workspace_data = snapshot.get_component_snapshot(SnapshotKey.WORKSPACE).get("content")
@@ -791,27 +790,31 @@
                                 self.engine.job_runner.restore_running_job(
                                     run_number=run_number,
                                     job_id=job_id,
                                     job_clients=job_clients,
                                     snapshot=snapshot,
                                     fl_ctx=fl_ctx,
                                 )
+                            restored_job_ids.append(job_id)
+            with self.engine.new_context() as fl_ctx:
+                self.engine.job_runner.update_abnormal_finished_jobs(restored_job_ids, fl_ctx=fl_ctx)
         else:
             with self.engine.new_context() as fl_ctx:
                 self.snapshot_persistor.delete()
                 self.engine.job_runner.update_unfinished_jobs(fl_ctx=fl_ctx)
 
         with self.lock:
             self.server_state = HotState(
                 host=self.server_state.host, port=self.server_state.service_port, ssid=self.server_state.ssid
             )
 
-    def _turn_to_cold(self):
+    def _turn_to_cold(self, old_state_name):
         with self.lock:
             self.server_state = ColdState(host=self.server_state.host, port=self.server_state.service_port)
+        self._notify_state_change(old_state_name)
         self.engine.pause_server_jobs()
 
     def stop_training(self):
         self.status = ServerStatus.STOPPED
         self.logger.info("Server app stopped.\n\n")
 
     def fl_shutdown(self):
```

## nvflare/private/fed/server/info_coll_cmd.py

```diff
@@ -13,16 +13,18 @@
 # limitations under the License.
 
 import json
 from typing import List
 
 from nvflare.apis.fl_constant import AdminCommandNames
 from nvflare.fuel.hci.conn import Connection
+from nvflare.fuel.hci.proto import MetaStatusValue, make_meta
 from nvflare.fuel.hci.reg import CommandModuleSpec, CommandSpec
 from nvflare.fuel.hci.server.authz import PreAuthzReturnCode
+from nvflare.fuel.hci.server.constants import ConnProps
 from nvflare.private.defs import InfoCollectorTopic, RequestHeader
 from nvflare.private.fed.server.admin import new_message
 from nvflare.private.fed.server.server_engine_internal_spec import ServerEngineInternalSpec
 from nvflare.widgets.info_collector import InfoCollector
 from nvflare.widgets.widget import WidgetID
 
 from .cmd_utils import CommandUtil
@@ -41,133 +43,114 @@
     def get_spec(self):
         return CommandModuleSpec(
             name="info",
             cmd_specs=[
                 CommandSpec(
                     name=AdminCommandNames.SHOW_STATS,
                     description="show current system stats for an actively running job",
-                    usage="show_stats job_id server|client",
+                    usage="show_stats job_id server|client [clients]",
                     handler_func=self.show_stats,
                     authz_func=self.authorize_info_collection,
                     visible=True,
                 ),
                 CommandSpec(
                     name=AdminCommandNames.SHOW_ERRORS,
                     description="show latest errors in an actively running job",
-                    usage="show_errors job_id server|client",
+                    usage="show_errors job_id server|client [clients]",
                     handler_func=self.show_errors,
                     authz_func=self.authorize_info_collection,
                     visible=True,
                 ),
                 CommandSpec(
                     name=AdminCommandNames.RESET_ERRORS,
                     description="reset error stats for an actively running job",
-                    usage="reset_errors",
+                    usage="reset_errors job_id server|client [clients]",
                     handler_func=self.reset_errors,
                     authz_func=self.authorize_info_collection,
                     visible=True,
                 ),
             ],
         )
 
     def authorize_info_collection(self, conn: Connection, args: List[str]):
-        if len(args) != 3:
-            conn.append_error("syntax error: missing job_id and target")
+        if len(args) < 3:
+            cmd_entry = conn.get_prop(ConnProps.CMD_ENTRY)
+            conn.append_error(f"Usage: {cmd_entry.usage}", meta=make_meta(MetaStatusValue.SYNTAX_ERROR))
             return PreAuthzReturnCode.ERROR
 
         rt = self.authorize_job(conn, args)
         if rt == PreAuthzReturnCode.ERROR:
             return rt
 
         engine = conn.app_ctx
         if not isinstance(engine, ServerEngineInternalSpec):
             raise TypeError("engine must be ServerEngineInternalSpec but got {}".format(type(engine)))
 
         collector = engine.get_widget(WidgetID.INFO_COLLECTOR)
         if not collector:
-            conn.append_error("info collector not available")
+            msg = "info collector not available"
+            conn.append_error(msg, meta=make_meta(MetaStatusValue.INTERNAL_ERROR, msg))
             return PreAuthzReturnCode.ERROR
 
         if not isinstance(collector, InfoCollector):
-            conn.append_error("system error: info collector not right object")
+            msg = "info collector not right object"
+            conn.append_error(msg, meta=make_meta(MetaStatusValue.INTERNAL_ERROR, msg))
             return PreAuthzReturnCode.ERROR
 
         conn.set_prop(self.CONN_KEY_COLLECTOR, collector)
 
         job_id = conn.get_prop(self.JOB_ID)
         if job_id not in engine.run_processes:
-            conn.append_error(f"Job_id: {job_id} is not running.")
+            conn.append_error(
+                f"Job_id: {job_id} is not running.", meta=make_meta(MetaStatusValue.JOB_NOT_RUNNING, job_id)
+            )
             return PreAuthzReturnCode.ERROR
 
         run_info = engine.get_app_run_info(job_id)
         if not run_info:
             conn.append_string(
-                "Cannot find job: {}. Please make sure the first arg following the command is a valid job_id.".format(
-                    job_id
-                )
+                f"Cannot find job: {job_id}. Please make sure the first arg following the command is a valid job_id.",
+                meta=make_meta(MetaStatusValue.INVALID_JOB_ID, job_id),
             )
             return PreAuthzReturnCode.ERROR
         return rt
 
     def show_stats(self, conn: Connection, args: List[str]):
         engine = conn.app_ctx
-        if not isinstance(engine, ServerEngineInternalSpec):
-            raise TypeError("engine must be ServerEngineInternalSpec but got {}".format(type(engine)))
+        self._collect_stats(conn, args, stats_func=engine.show_stats, msg_topic=InfoCollectorTopic.SHOW_STATS)
 
+    def _collect_stats(self, conn: Connection, args: List[str], stats_func, msg_topic):
         job_id = conn.get_prop(self.JOB_ID)
         target_type = args[2]
-        if target_type == self.TARGET_TYPE_SERVER:
-            result = engine.show_stats(job_id)
-            conn.append_any(result)
-        elif target_type == self.TARGET_TYPE_CLIENT:
-            message = new_message(conn, topic=InfoCollectorTopic.SHOW_STATS, body="", require_authz=True)
+        result = {}
+        if target_type in [self.TARGET_TYPE_SERVER, self.TARGET_TYPE_ALL]:
+            server_stats = stats_func(job_id)
+            result["server"] = server_stats
+
+        if target_type in [self.TARGET_TYPE_CLIENT, self.TARGET_TYPE_ALL]:
+            message = new_message(conn, topic=msg_topic, body="", require_authz=True)
             message.set_header(RequestHeader.JOB_ID, job_id)
             replies = self.send_request_to_clients(conn, message)
-            self._process_stats_replies(conn, replies)
+            self._process_stats_replies(conn, replies, result)
+        conn.append_any(result)
 
     def show_errors(self, conn: Connection, args: List[str]):
         engine = conn.app_ctx
-        if not isinstance(engine, ServerEngineInternalSpec):
-            raise TypeError("engine must be ServerEngineInternalSpec but got {}".format(type(engine)))
-
-        job_id = conn.get_prop(self.JOB_ID)
-        target_type = args[2]
-        if target_type == self.TARGET_TYPE_SERVER:
-            result = engine.get_errors(job_id)
-            conn.append_any(result)
-        elif target_type == self.TARGET_TYPE_CLIENT:
-            message = new_message(conn, topic=InfoCollectorTopic.SHOW_ERRORS, body="", require_authz=True)
-            message.set_header(RequestHeader.JOB_ID, job_id)
-            replies = self.send_request_to_clients(conn, message)
-            self._process_stats_replies(conn, replies)
+        self._collect_stats(conn, args, stats_func=engine.get_errors, msg_topic=InfoCollectorTopic.SHOW_ERRORS)
 
     def reset_errors(self, conn: Connection, args: List[str]):
         engine = conn.app_ctx
-        if not isinstance(engine, ServerEngineInternalSpec):
-            raise TypeError("engine must be ServerEngineInternalSpec but got {}".format(type(engine)))
-
-        job_id = conn.get_prop(self.JOB_ID)
-        target_type = args[2]
-        if target_type == self.TARGET_TYPE_SERVER:
-            result = engine.reset_errors(job_id)
-            conn.append_any(result)
-        elif target_type == self.TARGET_TYPE_CLIENT:
-            message = new_message(conn, topic=InfoCollectorTopic.RESET_ERRORS, body="", require_authz=True)
-            message.set_header(RequestHeader.JOB_ID, job_id)
-            replies = self.send_request_to_clients(conn, message)
-            self._process_stats_replies(conn, replies)
+        self._collect_stats(conn, args, stats_func=engine.reset_errors, msg_topic=InfoCollectorTopic.RESET_ERRORS)
 
-    def _process_stats_replies(self, conn, replies):
+    @staticmethod
+    def _process_stats_replies(conn, replies, result: dict):
         if not replies:
-            conn.append_error("no responses from clients")
             return
 
-        engine = conn.app_ctx
         for r in replies:
-            client_name = engine.get_client_name_from_token(r.client_token)
-
-            conn.append_string(f"--- Client ---: {client_name}")
+            client_name = r.client_name
             try:
                 body = json.loads(r.reply.body)
-                conn.append_any(body)
-            except Exception:
-                conn.append_string("Bad responses from clients")
+                result[client_name] = body
+            except BaseException:
+                result[client_name] = "invalid_reply"
+                return
```

## nvflare/private/fed/server/job_cmds.py

```diff
@@ -18,15 +18,15 @@
 import os
 import shutil
 from typing import Dict, List
 
 import nvflare.fuel.hci.file_transfer_defs as ftd
 from nvflare.apis.client import Client
 from nvflare.apis.fl_constant import AdminCommandNames, RunProcessKey
-from nvflare.apis.job_def import Job, JobDataKey, JobMetaKey, TopDir
+from nvflare.apis.job_def import Job, JobDataKey, JobMetaKey, TopDir, is_valid_job_id
 from nvflare.apis.job_def_manager_spec import JobDefManagerSpec, RunStatus
 from nvflare.apis.utils.job_utils import convert_legacy_zipped_app_to_job
 from nvflare.fuel.hci.base64_utils import b64str_to_bytes, bytes_to_b64str
 from nvflare.fuel.hci.conn import Connection
 from nvflare.fuel.hci.proto import ConfirmMethod, MetaKey, MetaStatusValue, make_meta
 from nvflare.fuel.hci.reg import CommandModule, CommandModuleSpec, CommandSpec
 from nvflare.fuel.hci.server.authz import PreAuthzReturnCode
@@ -166,14 +166,18 @@
         if len(args) < 2:
             conn.append_error(
                 "syntax error: missing job_id", meta=make_meta(MetaStatusValue.SYNTAX_ERROR, "missing job_id")
             )
             return PreAuthzReturnCode.ERROR
 
         job_id = args[1].lower()
+        if not is_valid_job_id(job_id):
+            conn.append_error(f"invalid job_id {job_id}", meta=make_meta(MetaStatusValue.INVALID_JOB_ID, job_id))
+            return PreAuthzReturnCode.ERROR
+
         conn.set_prop(self.JOB_ID, job_id)
         engine = conn.app_ctx
         job_def_manager = engine.job_def_manager
 
         with engine.new_context() as fl_ctx:
             job = job_def_manager.get_job(job_id, fl_ctx)
 
@@ -188,15 +192,15 @@
         conn.set_prop(ConnProps.SUBMITTER_NAME, job.meta.get(JobMetaKey.SUBMITTER_NAME, ""))
         conn.set_prop(ConnProps.SUBMITTER_ORG, job.meta.get(JobMetaKey.SUBMITTER_ORG, ""))
         conn.set_prop(ConnProps.SUBMITTER_ROLE, job.meta.get(JobMetaKey.SUBMITTER_ROLE, ""))
 
         if len(args) > 2:
             err = self.validate_command_targets(conn, args[2:])
             if err:
-                conn.append_error(err, meta=make_meta(MetaStatusValue.SYNTAX_ERROR, err))
+                conn.append_error(err, meta=make_meta(MetaStatusValue.INVALID_TARGET, err))
                 return PreAuthzReturnCode.ERROR
 
         return PreAuthzReturnCode.REQUIRE_AUTHZ
 
     def abort_task(self, conn, args: List[str]) -> str:
         engine = conn.app_ctx
         if not isinstance(engine, ServerEngineInternalSpec):
@@ -209,15 +213,15 @@
         return self.process_replies_to_table(conn, replies)
 
     def _start_app_on_clients(self, conn: Connection, job_id: str) -> bool:
         engine = conn.app_ctx
         client_names = conn.get_prop(self.TARGET_CLIENT_NAMES, None)
         run_process = engine.run_processes.get(job_id, {})
         if not run_process:
-            conn.append_error(f"Job: {job_id} is not running.")
+            conn.append_error(f"Job {job_id} is not running.")
             return False
 
         participants: Dict[str, Client] = run_process.get(RunProcessKey.PARTICIPANTS, {})
         wrong_clients = []
         for client in client_names:
             client_valid = False
             for _, p in participants.items():
@@ -371,15 +375,15 @@
         try:
             engine = conn.app_ctx
             job_def_manager = engine.job_def_manager
 
             with engine.new_context() as fl_ctx:
                 job_def_manager.delete(job_id, fl_ctx)
                 conn.append_string(f"Job {job_id} deleted.")
-        except Exception as e:
+        except BaseException as e:
             conn.append_error(
                 f"exception occurred: {secure_format_exception(e)}",
                 meta=make_meta(MetaStatusValue.INTERNAL_ERROR, f"exception {type(e)}"),
             )
             return
         conn.append_success("", meta=make_meta(MetaStatusValue.OK))
 
@@ -424,15 +428,15 @@
                     message = job_runner.stop_run(job_id, fl_ctx)
                     if message:
                         conn.append_error(message, meta=make_meta(MetaStatusValue.INTERNAL_ERROR, message))
                     else:
                         message = "Abort signal has been sent to the server app."
                         conn.append_string(message)
                         conn.append_success("", meta=make_meta(MetaStatusValue.OK, message))
-        except Exception as e:
+        except BaseException as e:
             conn.append_error(
                 f"Exception occurred trying to abort job: {secure_format_exception(e)}",
                 meta=make_meta(MetaStatusValue.INTERNAL_ERROR, f"exception {type(e)}"),
             )
             return
 
     def clone_job(self, conn: Connection, args: List[str]):
@@ -457,15 +461,15 @@
                 job_meta[JobMetaKey.SUBMITTER_ORG.value] = conn.get_prop(ConnProps.USER_ORG)
                 job_meta[JobMetaKey.SUBMITTER_ROLE.value] = conn.get_prop(ConnProps.USER_ROLE)
                 job_meta[JobMetaKey.CLONED_FROM.value] = job_id
 
                 meta = job_def_manager.create(job_meta, data_bytes, fl_ctx)
                 new_job_id = meta.get(JobMetaKey.JOB_ID)
                 conn.append_string("Cloned job {} as: {}".format(job_id, new_job_id))
-        except Exception as e:
+        except BaseException as e:
             conn.append_error(
                 f"Exception occurred trying to clone job: {secure_format_exception(e)}",
                 meta=make_meta(MetaStatusValue.INTERNAL_ERROR, f"exception {type(e)}"),
             )
             return
         conn.append_success("", meta=make_meta(status=MetaStatusValue.OK, extra={MetaKey.JOB_ID: new_job_id}))
 
@@ -596,15 +600,15 @@
                 meta[JobMetaKey.SUBMITTER_ORG.value] = conn.get_prop(ConnProps.USER_ORG, "")
                 meta[JobMetaKey.SUBMITTER_ROLE.value] = conn.get_prop(ConnProps.USER_ROLE, "")
 
                 meta = job_def_manager.create(meta, data_bytes, fl_ctx)
                 job_id = meta.get(JobMetaKey.JOB_ID)
                 conn.append_string(f"Submitted job: {job_id}")
                 conn.append_success("", meta=make_meta(MetaStatusValue.OK, extra={MetaKey.JOB_ID: job_id}))
-        except Exception as e:
+        except BaseException as e:
             conn.append_error(
                 f"Exception occurred trying to submit job: {secure_format_exception(e)}",
                 meta=make_meta(MetaStatusValue.INTERNAL_ERROR, f"exception {type(e)} occurred"),
             )
             return
 
     def _unzip_data(self, download_dir, job_data, job_id):
@@ -655,10 +659,10 @@
             return
         try:
             data = zip_directory_to_bytes(download_dir, job_id)
             b64str = bytes_to_b64str(data)
             conn.append_string(b64str, meta=make_meta(MetaStatusValue.OK, extra={MetaKey.JOB_ID: job_id}))
         except FileNotFoundError:
             conn.append_error("No record found for job '{}'".format(job_id))
-        except Exception:
+        except BaseException:
             secure_log_traceback()
             conn.append_error("Exception occurred during attempt to zip data to send for job: {}".format(job_id))
```

## nvflare/private/fed/server/job_meta_validator.py

```diff
@@ -17,22 +17,23 @@
 import logging
 from io import BytesIO
 from typing import Optional, Set, Tuple
 from zipfile import ZipFile
 
 from nvflare.apis.fl_constant import JobConstants
 from nvflare.apis.job_def import ALL_SITES, SERVER_SITE_NAME, JobMetaKey
+from nvflare.apis.job_meta_validator_spec import JobMetaValidatorSpec
 from nvflare.security.logging import secure_format_exception
 
 MAX_CLIENTS = 1000000
 
 logger = logging.getLogger(__name__)
 
 
-class JobMetaValidator:
+class JobMetaValidator(JobMetaValidatorSpec):
     """Job validator"""
 
     def validate(self, job_name: str, job_data: bytes) -> Tuple[bool, str, dict]:
         """Validate job
 
         Args:
             job_name (str): Job name
```

## nvflare/private/fed/server/job_runner.py

```diff
@@ -87,15 +87,16 @@
             engine = fl_ctx.get_engine()
             self.scheduler = engine.get_component(SystemComponents.JOB_SCHEDULER)
         elif event_type in [EventType.JOB_COMPLETED, EventType.END_RUN]:
             self._save_workspace(fl_ctx)
         elif event_type == EventType.SYSTEM_END:
             self.stop()
 
-    def _make_deploy_message(self, job: Job, app_data, app_name):
+    @staticmethod
+    def _make_deploy_message(job: Job, app_data, app_name):
         message = Message(topic=TrainingTopic.DEPLOY, body=app_data)
         message.set_header(RequestHeader.REQUIRE_AUTHZ, "true")
 
         message.set_header(RequestHeader.ADMIN_COMMAND, AdminCommandNames.SUBMIT_JOB)
         message.set_header(RequestHeader.JOB_ID, job.job_id)
         message.set_header(RequestHeader.APP_NAME, app_name)
 
@@ -140,26 +141,31 @@
             if len(participants) == 1 and participants[0].upper() == ALL_SITES:
                 participants = ["server"]
                 participants.extend([client.name for client in engine.get_clients()])
 
             client_sites = []
             for p in participants:
                 if p == "server":
-                    app_deployer = AppDeployer(
-                        app_name=app_name, workspace=workspace, job_id=job.job_id, job_meta=job.meta, app_data=app_data
+                    app_deployer = AppDeployer()
+                    err = app_deployer.deploy(
+                        app_name=app_name,
+                        workspace=workspace,
+                        job_id=job.job_id,
+                        job_meta=job.meta,
+                        app_data=app_data,
+                        fl_ctx=fl_ctx,
                     )
-
-                    err = app_deployer.deploy()
                     if err:
                         deploy_detail.append(f"server: {err}")
                         raise RuntimeError(f"Failed to deploy app '{app_name}': {err}")
 
                     kv_list = parse_vars(engine.args.set)
                     secure_train = kv_list.get("secure_train", True)
-                    if secure_train:
+                    from_hub_site = job.meta.get(JobMetaKey.FROM_HUB_SITE.value)
+                    if secure_train and not from_hub_site:
                         app_path = workspace.get_app_dir(job.job_id)
                         root_ca_path = os.path.join(workspace.get_startup_kit_dir(), "rootCA.pem")
                         if not verify_folder_signature(app_path, root_ca_path):
                             err = "job signature verification failed"
                             deploy_detail.append(f"server: {err}")
                             raise RuntimeError(f"Failed to verify app '{app_name}': {err}")
 
@@ -441,15 +447,15 @@
                                 job=ready_job,
                                 client_sites=deployable_clients,
                                 fl_ctx=fl_ctx,
                             )
                             with self.lock:
                                 self.running_jobs[job_id] = ready_job
                             job_manager.set_status(ready_job.job_id, RunStatus.RUNNING, fl_ctx)
-                        except Exception as e:
+                        except BaseException as e:
                             if job_id:
                                 if job_id in self.running_jobs:
                                     with self.lock:
                                         del self.running_jobs[job_id]
                                 self._stop_run(job_id, fl_ctx)
                             job_manager.set_status(ready_job.job_id, RunStatus.FAILED_TO_RUN, fl_ctx)
 
@@ -466,15 +472,16 @@
 
                 time.sleep(1.0)
 
             thread.join()
         else:
             self.log_error(fl_ctx, "There's no Job Manager defined. Won't be able to run the jobs.")
 
-    def _check_job_status(self, job_manager, job_id, job_run_status, fl_ctx: FLContext):
+    @staticmethod
+    def _check_job_status(job_manager, job_id, job_run_status, fl_ctx: FLContext):
         reload_job = job_manager.get_job(job_id, fl_ctx)
         return reload_job.meta.get(JobMetaKey.STATUS) != job_run_status
 
     def stop(self):
         self.ask_to_stop = True
 
     def restore_running_job(self, run_number: str, job_id: str, job_clients, snapshot, fl_ctx: FLContext):
@@ -490,32 +497,55 @@
                 self.running_jobs[job_id] = job
             self.scheduler.restore_scheduled_job(job_id)
         except Exception as e:
             self.log_error(
                 fl_ctx, f"Failed to restore the job: {job_id} to the running job table: {secure_format_exception(e)}."
             )
 
+    def update_abnormal_finished_jobs(self, running_job_ids, fl_ctx: FLContext):
+        engine = fl_ctx.get_engine()
+        job_manager = engine.get_component(SystemComponents.JOB_MANAGER)
+        all_jobs = self._get_all_running_jobs(job_manager, fl_ctx)
+
+        for job in all_jobs:
+            if job.job_id not in running_job_ids:
+                try:
+                    job_manager.set_status(job.job_id, RunStatus.FINISHED_ABNORMAL, fl_ctx)
+                    self.logger.info(f"Update the previous running job: {job.job_id} to {RunStatus.FINISHED_ABNORMAL}.")
+                except Exception as e:
+                    self.log_error(
+                        fl_ctx,
+                        f"Failed to update the job: {job.job_id} to {RunStatus.FINISHED_ABNORMAL}: "
+                        f"{secure_format_exception(e)}.",
+                    )
+
     def update_unfinished_jobs(self, fl_ctx: FLContext):
         engine = fl_ctx.get_engine()
         job_manager = engine.get_component(SystemComponents.JOB_MANAGER)
-        all_jobs = []
-        dispatched_jobs = job_manager.get_jobs_by_status(RunStatus.DISPATCHED, fl_ctx)
-        all_jobs.extend(dispatched_jobs)
-        running_jobs = job_manager.get_jobs_by_status(RunStatus.RUNNING, fl_ctx)
-        all_jobs.extend(running_jobs)
+        all_jobs = self._get_all_running_jobs(job_manager, fl_ctx)
 
         for job in all_jobs:
             try:
                 job_manager.set_status(job.job_id, RunStatus.ABANDONED, fl_ctx)
-                self.logger.info(f"Update the previous running job: {job.job_id} to ABANDONED.")
+                self.logger.info(f"Update the previous running job: {job.job_id} to {RunStatus.ABANDONED}.")
             except Exception as e:
                 self.log_error(
-                    fl_ctx, f"Failed to update the job: {job.job_id} to ABANDONED: {secure_format_exception(e)}."
+                    fl_ctx,
+                    f"Failed to update the job: {job.job_id} to {RunStatus.ABANDONED}: {secure_format_exception(e)}.",
                 )
 
+    @staticmethod
+    def _get_all_running_jobs(job_manager, fl_ctx):
+        all_jobs = []
+        dispatched_jobs = job_manager.get_jobs_by_status(RunStatus.DISPATCHED, fl_ctx)
+        all_jobs.extend(dispatched_jobs)
+        running_jobs = job_manager.get_jobs_by_status(RunStatus.RUNNING, fl_ctx)
+        all_jobs.extend(running_jobs)
+        return all_jobs
+
     def stop_run(self, job_id: str, fl_ctx: FLContext):
         engine = fl_ctx.get_engine()
         job_manager = engine.get_component(SystemComponents.JOB_MANAGER)
         self._stop_run(job_id, fl_ctx)
 
         job = self.running_jobs.get(job_id)
         if job:
```

## nvflare/private/fed/server/message_send.py

```diff
@@ -16,23 +16,25 @@
 from nvflare.fuel.f3.cellnet.cell import Message as CellMessage
 from nvflare.fuel.f3.cellnet.cell import TargetMessage
 from nvflare.private.admin_defs import Message
 from nvflare.private.defs import CellChannel, new_cell_message
 
 
 class ClientReply(object):
-    def __init__(self, client_token: str, req: Message, reply: Message):
+    def __init__(self, client_token: str, client_name: str, req: Message, reply: Message):
         """Client reply.
 
         Args:
             client_token (str): client token
+            client_name (str): name of the client
             req (Message): request
             reply (Message): reply
         """
         self.client_token = client_token
+        self.client_name = client_name
         self.request = req
         self.reply = reply
 
 
 def send_requests(
     cell, command: str, requests: dict, clients, job_id=None, timeout_secs=2.0, optional=False
 ) -> [ClientReply]:
@@ -93,9 +95,13 @@
         cell.fire_multi_requests_and_forget(target_msgs, optional=optional)
         return []
     else:
         result = []
         replies = cell.broadcast_multi_requests(target_msgs, timeout_secs, optional=optional)
         for name, reply in replies.items():
             assert isinstance(reply, CellMessage)
-            result.append(ClientReply(client_token=name_to_token[name], req=name_to_req[name], reply=reply.payload))
+            result.append(
+                ClientReply(
+                    client_token=name_to_token[name], client_name=name, req=name_to_req[name], reply=reply.payload
+                )
+            )
         return result
```

## nvflare/private/fed/server/server_app_runner.py

```diff
@@ -59,15 +59,15 @@
             _set_up_run_config(workspace, self.server, conf)
 
             if not isinstance(self.server.engine, ServerEngine):
                 raise TypeError(f"server.engine must be ServerEngine. Got type:{type(self.server.engine).__name__}")
             self.sync_up_parents_process(args)
 
             self.server.start_run(job_id, app_root, conf, args, snapshot)
-        except Exception as e:
+        except BaseException as e:
             with self.server.engine.new_context() as fl_ctx:
                 fl_ctx.set_prop(key=FLContextKey.FATAL_SYSTEM_ERROR, value=True, private=True, sticky=True)
             logger.exception(f"FL server execution exception: {secure_format_exception(e)}")
             raise e
         finally:
             self.update_job_run_status()
             self.server.status = ServerStatus.STOPPED
```

## nvflare/private/fed/server/server_engine.py

```diff
@@ -341,15 +341,15 @@
                 job_id=job_id,
                 command_name=AdminCommandNames.ABORT,
                 command_data=command_data,
                 timeout=1.0,
                 optional=True,
             )
             self.logger.info(f"Abort server status: {status_message}")
-        except Exception:
+        except BaseException:
             with self.lock:
                 child_process = self.run_processes.get(job_id, {}).get(RunProcessKey.CHILD_PROCESS, None)
                 if child_process:
                     child_process.terminate()
         finally:
             threading.Thread(target=self._remove_run_processes, args=[job_id]).start()
 
@@ -425,15 +425,15 @@
         run_info = None
         try:
             run_info = self.send_command_to_child_runner_process(
                 job_id=job_id,
                 command_name=ServerCommandNames.GET_RUN_INFO,
                 command_data={},
             )
-        except Exception:
+        except BaseException:
             self.logger.error(f"Failed to get_app_run_info for run: {job_id}")
         return run_info
 
     def set_run_manager(self, run_manager: RunManager):
         self.run_manager = run_manager
         for _, widget in self.widgets.items():
             self.run_manager.add_handler(widget)
@@ -656,15 +656,15 @@
             snapshot.completed = completed
 
             self.server.snapshot_location = self.snapshot_persistor.save(snapshot=snapshot)
             if not completed:
                 self.logger.info(f"persist the snapshot to: {self.server.snapshot_location}")
             else:
                 self.logger.info(f"The snapshot: {self.server.snapshot_location} has been removed.")
-        except Exception as e:
+        except BaseException as e:
             self.logger.error(f"Failed to persist the components. {secure_format_exception(e)}")
 
     def restore_components(self, snapshot: RunSnapshot, fl_ctx: FLContext):
         for component_id, component in self.run_manager.components.items():
             if isinstance(component, FLComponent):
                 component.restore(snapshot.get_component_snapshot(component_id=component_id), fl_ctx)
 
@@ -677,45 +677,45 @@
         stats = None
         try:
             stats = self.send_command_to_child_runner_process(
                 job_id=job_id,
                 command_name=ServerCommandNames.SHOW_STATS,
                 command_data={},
             )
-        except Exception:
+        except BaseException:
             self.logger.error(f"Failed to show_stats for JOB: {job_id}")
 
         if stats is None:
             stats = {}
         return stats
 
     def get_errors(self, job_id) -> dict:
         errors = None
         try:
             errors = self.send_command_to_child_runner_process(
                 job_id=job_id,
                 command_name=ServerCommandNames.GET_ERRORS,
                 command_data={},
             )
-        except Exception:
+        except BaseException:
             self.logger.error(f"Failed to get_errors for JOB: {job_id}")
 
         if errors is None:
             errors = {}
         return errors
 
     def reset_errors(self, job_id) -> str:
         errors = None
         try:
             self.send_command_to_child_runner_process(
                 job_id=job_id,
                 command_name=ServerCommandNames.RESET_ERRORS,
                 command_data={},
             )
-        except Exception:
+        except BaseException:
             self.logger.error(f"Failed to reset_errors for JOB: {job_id}")
 
         return f"reset the server error stats for job: {job_id}"
 
     def _send_admin_requests(self, requests, timeout_secs=10) -> List[ClientReply]:
         return self.server.admin_server.send_requests(requests, timeout_secs=timeout_secs)
 
@@ -731,15 +731,15 @@
             if client:
                 requests.update({client.token: request})
         replies = []
         if requests:
             replies = self._send_admin_requests(requests, 15)
         result = {}
         for r in replies:
-            site_name = self.get_client_name_from_token(r.client_token)
+            site_name = r.client_name
             if r.reply:
                 error_code = r.reply.get_header(MsgHeader.RETURN_CODE, ReturnCode.OK)
                 if error_code != ReturnCode.OK:
                     self.logger.error(f"Client reply error: {r.reply.body}")
                     result[site_name] = (False, "")
                 else:
                     resp = fobs.loads(r.reply.body)
```

## nvflare/private/fed/server/server_runner.py

```diff
@@ -109,15 +109,15 @@
                     # use the wf_lock to ensure state integrity between workflow change and message processing
                     with self.wf_lock:
                         # we only set self.current_wf to open for business after successful initialize_run!
                         self.current_wf = wf
 
                 with self.engine.new_context() as fl_ctx:
                     wf.responder.control_flow(self.abort_signal, fl_ctx)
-            except Exception as e:
+            except BaseException as e:
                 with self.engine.new_context() as fl_ctx:
                     self.log_exception(fl_ctx, "Exception in workflow {}: {}".format(wf.id, secure_format_exception(e)))
                 self.system_panic("Exception in workflow {}: {}".format(wf.id, secure_format_exception(e)), fl_ctx)
             finally:
                 with self.engine.new_context() as fl_ctx:
                     # do not execute finalize_run() until the wf_lock is acquired
                     with self.wf_lock:
@@ -127,15 +127,15 @@
                         # Note: WF finalization may take time since it needs to wait for
                         # the job monitor to join.
                         self.current_wf = None
 
                     self.log_info(fl_ctx, f"Workflow: {wf.id} finalizing ...")
                     try:
                         wf.responder.finalize_run(fl_ctx)
-                    except Exception as e:
+                    except BaseException as e:
                         self.log_exception(
                             fl_ctx, "Error finalizing workflow {}: {}".format(wf.id, secure_format_exception(e))
                         )
 
                     self.log_debug(fl_ctx, "firing event EventType.END_WORKFLOW")
                     self.fire_event(EventType.END_WORKFLOW, fl_ctx)
 
@@ -151,15 +151,15 @@
             fl_ctx.set_prop(ReservedKey.RUN_ABORT_SIGNAL, self.abort_signal, private=True, sticky=True)
             self.fire_event(EventType.START_RUN, fl_ctx)
             self.engine.persist_components(fl_ctx, completed=False)
 
         self.status = "started"
         try:
             self._execute_run()
-        except Exception as e:
+        except BaseException as e:
             with self.engine.new_context() as fl_ctx:
                 self.log_exception(fl_ctx, f"Error executing RUN: {secure_format_exception(e)}")
         finally:
             # use wf_lock to ensure state of current_wf!
             self.status = "done"
             with self.wf_lock:
                 with self.engine.new_context() as fl_ctx:
@@ -273,15 +273,15 @@
             if task_filter_list:
                 filter_list.extend(task_filter_list)
 
             if filter_list:
                 for f in filter_list:
                     try:
                         task_data = f.process(task_data, fl_ctx)
-                    except Exception as e:
+                    except BaseException as e:
                         self.log_exception(
                             fl_ctx,
                             "processing error in task data filter {}: {}; "
                             "asked client to try again later".format(type(f), secure_format_exception(e)),
                         )
 
                         with self.wf_lock:
@@ -293,27 +293,27 @@
             self.fire_event(EventType.AFTER_TASK_DATA_FILTER, fl_ctx)
             self.log_info(fl_ctx, f"sent task assignment to client. client_name:{client.name} task_id:{task_id}")
 
             audit_event_id = add_job_audit_event(fl_ctx=fl_ctx, msg=f'sent task to client "{client.name}"')
             task_data.set_header(ReservedHeaderKey.AUDIT_EVENT_ID, audit_event_id)
             task_data.set_header(TaskConstant.WAIT_TIME, self.config.task_request_interval)
             return task_name, task_id, task_data
-        except Exception as e:
+        except BaseException as e:
             self.log_exception(
                 fl_ctx,
                 f"Error processing client task request: {secure_format_exception(e)}; asked client to try again later",
             )
             return self._task_try_again()
 
     def _try_to_get_task(self, client, fl_ctx, timeout=None, retry_interval=0.005):
         start = time.time()
         while True:
             with self.wf_lock:
                 if self.current_wf is None:
-                    self.log_info(fl_ctx, "no current workflow - asked client to try again later")
+                    self.log_debug(fl_ctx, "no current workflow - asked client to try again later")
                     return "", "", None
 
                 task_name, task_id, task_data = self.current_wf.responder.process_task_request(client, fl_ctx)
 
                 if task_name and task_name != SpecialTaskName.TRY_AGAIN:
                     if task_data:
                         if not isinstance(task_data, Shareable):
@@ -350,15 +350,15 @@
     def handle_dead_job(self, client_name: str, fl_ctx: FLContext):
         with self.wf_lock:
             try:
                 if self.current_wf is None:
                     return
 
                 self.current_wf.responder.handle_dead_job(client_name=client_name, fl_ctx=fl_ctx)
-            except Exception as e:
+            except BaseException as e:
                 self.log_exception(
                     fl_ctx, f"Error processing dead job by workflow {self.current_wf.id}: {secure_format_exception(e)}"
                 )
 
     def process_submission(self, client: Client, task_name: str, task_id: str, result: Shareable, fl_ctx: FLContext):
         """Process task result submitted from a client.
 
@@ -439,15 +439,15 @@
                 if task_filter_list:
                     filter_list.extend(task_filter_list)
 
                 if filter_list:
                     for f in filter_list:
                         try:
                             result = f.process(result, fl_ctx)
-                        except Exception as e:
+                        except BaseException as e:
                             self.log_exception(
                                 fl_ctx,
                                 "Error processing in task result filter {}: {}".format(
                                     type(f), secure_format_exception(e)
                                 ),
                             )
 
@@ -463,15 +463,15 @@
                 self.current_wf.responder.process_submission(
                     client=client, task_name=task_name, task_id=task_id, result=result, fl_ctx=fl_ctx
                 )
                 self.log_info(fl_ctx, "finished processing client result by {}".format(self.current_wf.id))
 
                 self.log_debug(fl_ctx, "firing event EventType.AFTER_PROCESS_SUBMISSION")
                 self.fire_event(EventType.AFTER_PROCESS_SUBMISSION, fl_ctx)
-            except Exception as e:
+            except BaseException as e:
                 self.log_exception(
                     fl_ctx,
                     "Error processing client result by {}: {}".format(self.current_wf.id, secure_format_exception(e)),
                 )
 
     def abort(self, fl_ctx: FLContext, turn_to_cold: bool = False):
         self.status = "done"
```

## nvflare/private/fed/server/shell_cmd.py

```diff
@@ -15,14 +15,15 @@
 import os
 import re
 import subprocess
 from typing import List
 
 from nvflare.fuel.hci.cmd_arg_utils import join_args
 from nvflare.fuel.hci.conn import Connection
+from nvflare.fuel.hci.proto import MetaStatusValue, make_meta
 from nvflare.fuel.hci.reg import CommandModule, CommandModuleSpec, CommandSpec
 from nvflare.fuel.hci.server.authz import PreAuthzReturnCode
 from nvflare.fuel.hci.shell_cmd_val import (
     CatValidator,
     GrepValidator,
     HeadValidator,
     LsValidator,
@@ -88,36 +89,42 @@
             return
 
         engine = conn.app_ctx
         if not isinstance(engine, ServerEngineInternalSpec):
             raise TypeError("engine must be ServerEngineInternalSpec but got {}".format(type(engine)))
         clients, invalid_inputs = engine.validate_targets([target])
         if len(invalid_inputs) > 0:
-            conn.append_error("invalid client: {}".format(target))
+            msg = f"invalid target: {target}"
+            conn.append_error(msg, meta=make_meta(MetaStatusValue.INVALID_TARGET, info=msg))
             return
 
         if len(clients) > 1:
-            conn.append_error("this command can only be applied to one client at a time")
+            msg = "this command can only be applied to one client at a time"
+            conn.append_error(msg, meta=make_meta(MetaStatusValue.INVALID_TARGET, info=msg))
             return
 
         valid_tokens = []
         for c in clients:
             valid_tokens.append(c.token)
 
         req = new_message(conn=conn, topic=SysCommandTopic.SHELL, body=shell_cmd, require_authz=True)
         server = conn.server
         reply = server.send_request_to_client(req, valid_tokens[0], timeout_secs=server.timeout)
         if reply is None:
-            conn.append_error("no reply from client - timed out")
+            conn.append_error(
+                "no reply from client - timed out", meta=make_meta(MetaStatusValue.INTERNAL_ERROR, "client timeout")
+            )
             return
 
         if not isinstance(reply, ClientReply):
             raise TypeError("reply must be ClientReply but got {}".format(type(reply)))
         if reply.reply is None:
-            conn.append_error("no reply from client - timed out")
+            conn.append_error(
+                "no reply from client - timed out", meta=make_meta(MetaStatusValue.INTERNAL_ERROR, "client timeout")
+            )
             return
         if not isinstance(reply.reply, Message):
             raise TypeError("reply in ClientReply must be Message but got {}".format(type(reply.reply)))
         conn.append_string(reply.reply.body)
 
     def get_usage(self):
         if self.validator:
```

## nvflare/private/fed/server/sys_cmd.py

```diff
@@ -25,25 +25,24 @@
 from nvflare.private.fed.server.cmd_utils import CommandUtil
 from nvflare.security.logging import secure_format_exception
 
 
 def _parse_replies(conn, replies):
     """parses resources from replies."""
     site_resources = {}
-    engine = conn.app_ctx
     for r in replies:
-        client_name = engine.get_client_name_from_token(r.client_token)
+        client_name = r.client_name
 
         if r.reply:
             if r.reply.get_header(MsgHeader.RETURN_CODE) == ReturnCode.ERROR:
                 resources = r.reply.body
             else:
                 try:
                     resources = json.loads(r.reply.body)
-                except Exception as e:
+                except BaseException as e:
                     resources = f"Bad replies: {secure_format_exception(e)}"
         else:
             resources = "No replies"
         site_resources[client_name] = resources
     return site_resources
 
 
@@ -101,17 +100,16 @@
         conn.append_string("invalid target type {}. Usage: sys_info server|client <client-name>".format(target_type))
 
     def _process_replies(self, conn, replies):
         if not replies:
             conn.append_error("no responses from clients")
             return
 
-        engine = conn.app_ctx
         for r in replies:
-            client_name = engine.get_client_name_from_token(r.client_token)
+            client_name = r.client_name
             conn.append_string("Client: " + client_name)
 
             table = conn.append_table(["Metrics", "Value"])
             if r.reply:
                 if r.reply.get_header(MsgHeader.RETURN_CODE) == ReturnCode.ERROR:
                     table.add_row([r.reply.body, ""])
                 else:
@@ -122,15 +120,15 @@
                             table.add_row([str(k), str(v)])
                         table.add_row(
                             [
                                 "available_percent",
                                 "%.1f" % (psutil.virtual_memory().available * 100 / psutil.virtual_memory().total),
                             ]
                         )
-                    except Exception:
+                    except BaseException:
                         conn.append_string(": Bad replies")
             else:
                 conn.append_string(": No replies")
 
     def report_resources(self, conn: Connection, args: List[str]):
         if len(args) < 2:
             conn.append_error("syntax error: missing site names")
```

## nvflare/private/fed/server/training_cmds.py

```diff
@@ -58,16 +58,16 @@
                     handler_func=self.remove_client,
                     authz_func=self.authorize_client_operation,
                     visible=True,
                     confirm=ConfirmMethod.AUTH,
                 ),
                 CommandSpec(
                     name=AdminCommandNames.ADMIN_CHECK_STATUS,
-                    description="check status for shutdown system command",
-                    usage="admin_check_status",
+                    description="check status for project admin",
+                    usage="admin_check_status server|client",
                     handler_func=self.check_status,
                     authz_func=self.must_be_project_admin,
                     visible=False,
                 ),
                 CommandSpec(
                     name=AdminCommandNames.SHUTDOWN,
                     description="shutdown the FL server/client",
@@ -75,54 +75,45 @@
                     handler_func=self.shutdown,
                     authz_func=self.authorize_server_operation,
                     visible=True,
                     confirm=ConfirmMethod.AUTH,
                 ),
                 CommandSpec(
                     name=AdminCommandNames.RESTART,
-                    description="restart the FL server/client",
-                    usage="restart server|client|all",
+                    description="restart FL server and/or clients",
+                    usage="restart server|client|all [clients]",
                     handler_func=self.restart,
                     authz_func=self.authorize_server_operation,
                     visible=True,
                     confirm=ConfirmMethod.AUTH,
                 ),
                 CommandSpec(
-                    name=AdminCommandNames.SET_TIMEOUT,
-                    description="set the admin commands timeout",
-                    usage="set_timeout seconds ",
-                    handler_func=self.set_timeout,
-                    authz_func=self.command_authz_required,
-                    visible=True,
-                ),
-                CommandSpec(
                     name=AdminCommandNames.SHOW_SCOPES,
                     description="show configured scope names on server/client",
                     usage="show_scopes server|client|all ...",
                     handler_func=self.show_scopes,
                     authz_func=self.authorize_server_operation,
                     visible=True,
                 ),
             ],
         )
 
     # Shutdown
-    def _shutdown_app_on_server(self, conn: Connection) -> bool:
+    def _shutdown_app_on_server(self, conn: Connection) -> str:
         engine = conn.app_ctx
         err = engine.shutdown_server()
         if err:
             conn.append_error(err)
-            return False
+            return err
         else:
             conn.append_string("FL app has been shutdown.")
             conn.append_shutdown("Bye bye")
-            return True
+            return ""
 
     def _shutdown_app_on_clients(self, conn: Connection) -> bool:
-        engine = conn.app_ctx
         message = new_message(conn, topic=TrainingTopic.SHUTDOWN, body="", require_authz=True)
         clients = conn.get_prop(self.TARGET_CLIENT_TOKENS, None)
         if not clients:
             conn.append_error("no clients to shutdown")
             return False
 
         replies = self.send_request_to_clients(conn, message)
@@ -144,37 +135,41 @@
         target_type = args[1]
         engine = conn.app_ctx
         if not isinstance(engine, ServerEngine):
             raise TypeError("engine must be ServerEngine but got {}".format(type(engine)))
 
         for _, job in engine.job_runner.running_jobs.items():
             if not job.run_aborted:
-                conn.append_error("There are still jobs running. Please let them finish or abort_job before shutdown.")
+                conn.append_error(
+                    "There are still jobs running. Please let them finish or abort_job before shutdown.",
+                    meta=make_meta(MetaStatusValue.JOB_RUNNING, info=job.job_id),
+                )
                 return
 
         if target_type == self.TARGET_TYPE_SERVER:
             if engine.get_clients():
-                conn.append_error("There are still active clients. Shutdown all clients first.")
+                conn.append_error(
+                    "There are still active clients. Shutdown all clients first.",
+                    meta=make_meta(MetaStatusValue.CLIENTS_RUNNING),
+                )
                 return
-            if not self._shutdown_app_on_server(conn):
+
+        if target_type in [self.TARGET_TYPE_CLIENT, self.TARGET_TYPE_ALL]:
+            # must shut down clients first
+            success = self._shutdown_app_on_clients(conn)
+            if not success:
+                conn.update_meta(make_meta(MetaStatusValue.ERROR, "failed to shut down all clients"))
                 return
-        elif target_type == self.TARGET_TYPE_CLIENT:
-            if not self._shutdown_app_on_clients(conn):
+
+        if target_type in [self.TARGET_TYPE_SERVER, self.TARGET_TYPE_ALL]:
+            # shut down the server
+            err = self._shutdown_app_on_server(conn)
+            if err:
+                conn.update_meta(make_meta(MetaStatusValue.ERROR, info=err))
                 return
-        else:
-            # all
-            if engine.get_clients():
-                conn.append_string("Trying to shutdown clients before server...")
-                success = self._shutdown_app_on_clients(conn)
-                if success:
-                    if not self._shutdown_app_on_server(conn):
-                        return
-            else:
-                if not self._shutdown_app_on_server(conn):
-                    return
         conn.append_success("")
 
     # Remove Clients
     def remove_client(self, conn: Connection, args: List[str]):
         engine = conn.app_ctx
         if not isinstance(engine, ServerEngineInternalSpec):
             raise TypeError("engine must be ServerEngineInternalSpec but got {}".format(type(engine)))
@@ -182,70 +177,62 @@
         err = engine.remove_clients(clients)
         if err:
             conn.append_error(err)
             return
         conn.append_success("")
 
     # Restart
-    def _restart_clients(self, conn, clients) -> str:
+    def _restart_clients(self, conn) -> str:
         engine = conn.app_ctx
         if not isinstance(engine, ServerEngineInternalSpec):
             raise TypeError("engine must be ServerEngineInternalSpec but got {}".format(type(engine)))
         message = new_message(conn, topic=TrainingTopic.RESTART, body="", require_authz=True)
         replies = self.send_request_to_clients(conn, message)
         # engine.remove_clients(clients)
         return self._process_replies_to_string(conn, replies)
 
     def restart(self, conn: Connection, args: List[str]):
         engine = conn.app_ctx
         if not isinstance(engine, ServerEngine):
             raise TypeError("engine must be ServerEngine but got {}".format(type(engine)))
 
         if engine.job_runner.running_jobs:
-            conn.append_error("There are still jobs running. Please let them finish or abort_job before restart.")
+            msg = "There are still jobs running. Please let them finish or abort_job before restart."
+            conn.append_error(msg, meta=make_meta(MetaStatusValue.JOB_RUNNING, msg))
             return
 
         target_type = args[1]
-        if target_type == self.TARGET_TYPE_SERVER or target_type == self.TARGET_TYPE_ALL:
-
+        if target_type in [self.TARGET_TYPE_SERVER, self.TARGET_TYPE_ALL]:
             clients = engine.get_clients()
             if clients:
                 conn.append_string("Trying to restart all clients before restarting server...")
                 tokens = [c.token for c in clients]
                 conn.set_prop(
                     self.TARGET_CLIENT_TOKENS, tokens
                 )  # need this because not set in validate_command_targets when target_type == self.TARGET_TYPE_SERVER
-                response = self._restart_clients(conn, tokens)
+                response = self._restart_clients(conn)
                 conn.append_string(response)
                 # check with Isaac - no need to wait!
                 # time.sleep(5)
 
             err = engine.restart_server()
             if err:
-                conn.append_error(err)
+                conn.append_error(err, meta={MetaKey.SERVER_STATUS: MetaStatusValue.ERROR, MetaKey.INFO: err})
             else:
-                conn.append_string("Server scheduled for restart")
+                conn.append_string("Server scheduled for restart", meta={MetaKey.SERVER_STATUS: MetaStatusValue.OK})
         elif target_type == self.TARGET_TYPE_CLIENT:
             clients = conn.get_prop(self.TARGET_CLIENT_TOKENS)
             if not clients:
-                conn.append_error("no clients available")
+                conn.append_error("no clients available", meta=make_meta(MetaStatusValue.NO_CLIENTS, "no clients"))
                 return
             else:
-                response = self._restart_clients(conn, clients)
+                response = self._restart_clients(conn)
                 conn.append_string(response)
         conn.append_success("")
 
-    # Set Timeout
-    def set_timeout(self, conn: Connection, args: List[str]):
-        timeout = float(args[1])
-        server = conn.server
-        server.timeout = timeout
-        conn.append_string("admin command timeout has been set to: {}".format(timeout))
-        conn.append_success("")
-
     # Check status
     def check_status(self, conn: Connection, args: List[str]):
         # TODO:: Need more discussion on what status to be shown
         engine = conn.app_ctx
         if not isinstance(engine, ServerEngineInternalSpec):
             raise TypeError("engine must be ServerEngineInternalSpec but got {}".format(type(engine)))
         dst = args[1]
@@ -291,57 +278,72 @@
             )
 
     def _process_client_status_replies(self, conn, replies):
         if not replies:
             conn.append_error("no responses from clients")
             return
 
-        engine = conn.app_ctx
-        table = conn.append_table(["client", "app_name", "job_id", "status"])
+        table = conn.append_table(["client", "app_name", "job_id", "status"], name=MetaKey.CLIENT_STATUS)
         for r in replies:
             job_id = "?"
             app_name = "?"
-            client_name = engine.get_client_name_from_token(r.client_token)
+            client_name = r.client_name
 
             if r.reply:
                 if r.reply.get_header(MsgHeader.RETURN_CODE) == ReturnCode.ERROR:
-                    table.add_row([client_name, app_name, job_id, r.reply.body])
+                    table.add_row(
+                        [client_name, app_name, job_id, r.reply.body],
+                        meta={MetaKey.CLIENT_NAME: client_name, MetaKey.STATUS: MetaStatusValue.ERROR},
+                    )
                 else:
                     try:
                         body = json.loads(r.reply.body)
                         if isinstance(body, dict):
                             running_jobs = body.get(ClientStatusKey.RUNNING_JOBS)
                             if running_jobs:
                                 for job in running_jobs:
                                     app_name = job.get(ClientStatusKey.APP_NAME, "?")
                                     job_id = job.get(ClientStatusKey.JOB_ID, "?")
                                     status = job.get(ClientStatusKey.STATUS, "?")
-                                    table.add_row([client_name, app_name, job_id, status])
+                                    table.add_row(
+                                        [client_name, app_name, job_id, status],
+                                        meta={
+                                            MetaKey.CLIENT_NAME: client_name,
+                                            MetaKey.APP_NAME: app_name,
+                                            MetaKey.JOB_ID: job_id,
+                                            MetaKey.STATUS: status,
+                                        },
+                                    )
                             else:
-                                table.add_row([client_name, app_name, job_id, "No Jobs"])
-                    except Exception as e:
+                                table.add_row(
+                                    [client_name, app_name, job_id, "No Jobs"],
+                                    meta={MetaKey.CLIENT_NAME: client_name, MetaKey.STATUS: MetaStatusValue.NO_JOBS},
+                                )
+                    except BaseException as e:
                         self.logger.error(f"Bad reply from client: {secure_format_exception(e)}")
             else:
-                table.add_row([client_name, app_name, job_id, "No Reply"])
+                table.add_row(
+                    [client_name, app_name, job_id, "No Reply"],
+                    meta={MetaKey.CLIENT_NAME: client_name, MetaKey.STATUS: MetaStatusValue.NO_REPLY},
+                )
 
     def _add_scope_info(self, table, site_name, scope_names: List[str], default_scope: str):
         if not scope_names:
             names = ""
         else:
             names = ", ".join(scope_names)
         table.add_row([site_name, names, default_scope])
 
     def _process_scope_replies(self, table, conn, replies):
         if not replies:
             conn.append_error("no responses from clients")
             return
 
-        engine = conn.app_ctx
         for r in replies:
-            client_name = engine.get_client_name_from_token(r.client_token)
+            client_name = r.client_name
 
             if r.reply:
                 if r.reply.get_header(MsgHeader.RETURN_CODE) == ReturnCode.ERROR:
                     self._add_scope_info(table, client_name, r.reply.body, "")
                 else:
                     try:
                         body = json.loads(r.reply.body)
@@ -349,15 +351,15 @@
                             scope_names = body.get(ScopeInfoKey.SCOPE_NAMES)
                             default_scope = body.get(ScopeInfoKey.DEFAULT_SCOPE)
                             self._add_scope_info(table, client_name, scope_names, default_scope)
                         else:
                             conn.append_error(
                                 f"bad response from client {client_name}: expect dict but got {type(body)}"
                             )
-                    except Exception as e:
+                    except BaseException as e:
                         self.logger.error(f"Bad reply from client: {secure_format_exception(e)}")
                         conn.append_error(f"bad response from client {client_name}: {secure_format_exception(e)}")
             else:
                 self._add_scope_info(table, client_name, [], "no reply")
 
     def show_scopes(self, conn: Connection, args: List[str]):
         engine = conn.app_ctx
```

## nvflare/private/fed/simulator/simulator_server.py

```diff
@@ -101,15 +101,15 @@
             server_runner = fl_ctx.get_prop(FLContextKey.RUNNER)
             server_runner.process_submission(client, contribution_task_name, task_id, shareable, fl_ctx)
 
     def _aux_communicate(self, fl_ctx, shareable, shared_fl_context, topic):
         try:
             with self.engine.lock:
                 reply = self.engine.dispatch(topic=topic, request=shareable, fl_ctx=fl_ctx)
-        except Exception:
+        except BaseException:
             self.logger.info("Could not connect to server runner process - asked client to end the run")
             reply = make_reply(ReturnCode.COMMUNICATION_ERROR)
 
         return reply
 
     def _create_server_engine(self, args, snapshot_persistor):
         return SimulatorServerEngine(
```

## nvflare/private/fed/utils/app_deployer.py

```diff
@@ -12,74 +12,71 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
 import shutil
 
+from nvflare.apis.app_deployer_spec import AppDeployerSpec
+from nvflare.apis.fl_context import FLContext
 from nvflare.apis.job_def import JobMetaKey
 from nvflare.apis.workspace import Workspace
 from nvflare.fuel.utils.zip_utils import unzip_all_from_bytes
 from nvflare.private.privacy_manager import PrivacyService
 from nvflare.security.logging import secure_format_exception
 
 from .app_authz import AppAuthzService
 
 
-class AppDeployer(object):
-    def __init__(self, workspace: Workspace, job_id: str, job_meta: dict, app_name: str, app_data):
-        self.app_name = app_name
-        self.workspace = workspace
-        self.app_data = app_data
-        self.job_id = job_id
-        self.job_meta = job_meta
-
-    def deploy(self) -> str:
+class AppDeployer(AppDeployerSpec):
+    def deploy(
+        self, workspace: Workspace, job_id: str, job_meta: dict, app_name: str, app_data: bytes, fl_ctx: FLContext
+    ) -> str:
         """Deploys the app.
 
         Returns:
             error message if any
         """
-        privacy_scope = self.job_meta.get(JobMetaKey.SCOPE, "")
+        privacy_scope = job_meta.get(JobMetaKey.SCOPE, "")
 
         # check whether this scope is allowed
         if not PrivacyService.is_scope_allowed(privacy_scope):
             return f"privacy scope '{privacy_scope}' is not allowed"
 
         try:
-            run_dir = self.workspace.get_run_dir(self.job_id)
-            app_path = self.workspace.get_app_dir(self.job_id)
+            run_dir = workspace.get_run_dir(job_id)
+            app_path = workspace.get_app_dir(job_id)
             app_file = os.path.join(run_dir, "fl_app.txt")
-            job_meta_file = self.workspace.get_job_meta_path(self.job_id)
+            job_meta_file = workspace.get_job_meta_path(job_id)
 
             if os.path.exists(run_dir):
                 shutil.rmtree(run_dir)
 
             if not os.path.exists(app_path):
                 os.makedirs(app_path)
 
-            unzip_all_from_bytes(self.app_data, app_path)
+            unzip_all_from_bytes(app_data, app_path)
 
             with open(app_file, "wt") as f:
-                f.write(f"{self.app_name}")
+                f.write(f"{app_name}")
 
             with open(job_meta_file, "w") as f:
-                json.dump(self.job_meta, f, indent=4)
+                json.dump(job_meta, f, indent=4)
 
-            submitter_name = self.job_meta.get(JobMetaKey.SUBMITTER_NAME, "")
-            submitter_org = self.job_meta.get(JobMetaKey.SUBMITTER_ORG, "")
-            submitter_role = self.job_meta.get(JobMetaKey.SUBMITTER_ROLE, "")
+            submitter_name = job_meta.get(JobMetaKey.SUBMITTER_NAME, "")
+            submitter_org = job_meta.get(JobMetaKey.SUBMITTER_ORG, "")
+            submitter_role = job_meta.get(JobMetaKey.SUBMITTER_ROLE, "")
 
             authorized, err = AppAuthzService.authorize(
                 app_path=app_path,
                 submitter_name=submitter_name,
                 submitter_org=submitter_org,
                 submitter_role=submitter_role,
             )
             if err:
                 return err
 
             if not authorized:
                 return "not authorized"
 
-        except Exception as e:
-            raise Exception(f"exception {secure_format_exception(e)} when deploying app {self.app_name}")
+        except BaseException as e:
+            raise Exception(f"exception {secure_format_exception(e)} when deploying app {app_name}")
```

## nvflare/private/fed/utils/fed_utils.py

```diff
@@ -23,14 +23,15 @@
 
 from nvflare.apis.app_validation import AppValidator
 from nvflare.apis.fl_constant import FLContextKey, SiteType, WorkspaceConstants
 from nvflare.apis.job_def import JobMetaKey
 from nvflare.apis.utils.decomposers import flare_decomposers
 from nvflare.apis.workspace import Workspace
 from nvflare.app_common.decomposers import common_decomposers
+from nvflare.fuel.f3.stats_pool import CsvRecordHandler, StatsPoolManager
 from nvflare.fuel.sec.audit import AuditService
 from nvflare.fuel.sec.authz import AuthorizationService
 from nvflare.fuel.sec.security_content_service import LoadResult, SecurityContentService
 from nvflare.private.defs import SSLConstants
 from nvflare.private.fed.utils.decomposers import private_decomposers
 from nvflare.private.privacy_manager import PrivacyManager, PrivacyService
 from nvflare.security.logging import secure_format_exception, secure_log_traceback
@@ -184,14 +185,18 @@
         FLContextKey.JOB_SCOPE_NAME: scope_name,
         FLContextKey.EFFECTIVE_JOB_SCOPE_NAME: effective_scope_name,
         FLContextKey.SCOPE_PROPERTIES: scope_props,
         FLContextKey.SCOPE_OBJECT: scope_object,
     }
 
 
+def find_char_positions(s, ch):
+    return [i for i, c in enumerate(s) if c == ch]
+
+
 def configure_logging(workspace: Workspace):
     log_config_file_path = workspace.get_log_config_file_path()
     assert os.path.isfile(log_config_file_path), f"missing log config file {log_config_file_path}"
     logging.config.fileConfig(fname=log_config_file_path, disable_existing_loggers=False)
 
 
 def get_scope_info():
@@ -210,7 +215,59 @@
         return [], "processing_error"
 
 
 def fobs_initialize():
     flare_decomposers.register()
     common_decomposers.register()
     private_decomposers.register()
+
+
+def set_stats_pool_config_for_job(workspace: Workspace, job_id: str, prefix=None):
+    job_meta = get_job_meta_from_workspace(workspace, job_id)
+    config = job_meta.get(JobMetaKey.STATS_POOL_CONFIG)
+    if config:
+        StatsPoolManager.set_pool_config(config)
+        record_file = workspace.get_stats_pool_records_path(job_id, prefix)
+        record_writer = CsvRecordHandler(record_file)
+        StatsPoolManager.set_record_writer(record_writer)
+
+
+def create_stats_pool_files_for_job(workspace: Workspace, job_id: str, prefix=None):
+    err = ""
+    summary_file = workspace.get_stats_pool_summary_path(job_id, prefix)
+    try:
+        StatsPoolManager.dump_summary(summary_file)
+    except BaseException as e:
+        err = f"Failed to create stats pool summary file {summary_file}: {secure_format_exception(e)}"
+    StatsPoolManager.close()
+    return err
+
+
+def split_gpus(gpus) -> [str]:
+    gpus = gpus.replace(" ", "")
+    lefts = find_char_positions(gpus, "[")
+    rights = find_char_positions(gpus, "]")
+    if len(lefts) != len(rights):
+        raise ValueError("brackets not paired")
+    for i in range(len(lefts)):
+        if i > 0 and lefts[i] < rights[i - 1]:
+            raise ValueError("brackets cannot be nested")
+
+    offset = 0
+    for i in range(len(lefts)):
+        l: int = lefts[i] - offset
+        r: int = rights[i] - offset
+        if l > r:
+            raise ValueError("brackets not properly paired")
+
+        if l > 0 and gpus[l - 1] != ",":
+            raise ValueError(f"invalid start of a group: {gpus[l - 1]}")
+        if r < len(gpus) - 1 and gpus[r + 1] != ",":
+            raise ValueError(f"invalid end of a group: {gpus[r + 1]}")
+        g = gpus[l : r + 1]  # include both left and right brackets
+        p = g[1:-1].replace(",", "^")
+        gpus = gpus.replace(g, p, 1)  # only replace the first occurrence!
+        offset += 2  # everything after the replacement is shifted to left by 2 (since the pair of brackets removed)
+
+    result = gpus.split(",")
+    result = [g.replace("^", ",") for g in result]
+    return result
```

## nvflare/security/logging.py

```diff
@@ -111,23 +111,23 @@
 
     if not logger:
         logger = logging.getLogger()
 
     logger.error(exc_detail)
 
 
-def secure_format_exception(e: Exception) -> str:
+def secure_format_exception(e: BaseException) -> str:
     """Formats the specified exception and return a string without sensitive info.
 
     If secure mode is set, only return the type of the exception;
     If secure mode is not set, return the result of str(e).
 
     Args:
        e: the exception to be formatted
 
     Returns:
         A formatted exception string.
     """
     if is_secure():
         return str(type(e))
     else:
-        return f"{type(e).__name__}: {str(e)}"
+        return str(e)
```

## nvflare/tool/api_utils.py

```diff
@@ -15,15 +15,15 @@
 import time
 from typing import List
 
 from nvflare.fuel.flare_api.api_spec import JobNotFound, NoConnection
 from nvflare.fuel.flare_api.flare_api import Session
 
 
-def shutdown_system(prod_dir: str, username: str = "admin", secure_mode: bool = False, timeout_in_sec: int = 30):
+def shutdown_system(prod_dir: str, username: str = "admin", secure_mode: bool = True, timeout_in_sec: int = 30):
     admin_user_dir = os.path.join(prod_dir, username)
     print("connect to nvflare server")
     sess = None
     conn_timeout = 10
     try:
         sess = Session(username=username, startup_path=admin_user_dir, secure_mode=secure_mode)
         sess.try_connect(conn_timeout)
@@ -78,15 +78,15 @@
             status = sys_info.server_info.status
             curr = time.time()
             duration = curr - start
             if cnt % 25 == 0:
                 print("waiting system to shutdown")
             cnt += 1
             time.sleep(0.1)
-        except Exception:
+        except BaseException:
             # Server is already shutdown
             return
 
 
 def wait_for_system_start(
     num_clients: int,
     prod_dir: str,
```

## nvflare/widgets/fed_event.py

```diff
@@ -157,15 +157,15 @@
                     self.log_warning(fl_ctx, f"{n} items remained in in_events.  Will stop when it reaches 0.")
                 fl_ctx.set_prop(key=FLContextKey.EVENT_DATA, value=event_to_post, private=True, sticky=False)
                 fl_ctx.set_prop(key=FLContextKey.EVENT_SCOPE, value=EventScope.FEDERATION, private=True, sticky=False)
 
                 event_type = event_to_post.get_header(FedEventHeader.EVENT_TYPE)
                 try:
                     self.engine.fire_event(event_type=event_type, fl_ctx=fl_ctx)
-                except Exception as e:
+                except BaseException as e:
                     if self.asked_to_stop:
                         self.log_warning(fl_ctx, f"event {event_to_post} fired unsuccessfully during END_RUN")
                     else:
                         raise e
 
 
 class ServerFedEventRunner(FedEventRunner):
```

## nvflare/widgets/info_collector.py

```diff
@@ -98,14 +98,16 @@
             except:
                 self.log_exception(
                     fl_ctx=fl_ctx, msg="invalid event data type for event {}".format(event_type), fire_event=False
                 )
                 return
 
             analytic_data = AnalyticsData.from_dxo(dxo)
+            if not analytic_data:
+                return
 
             if event_type == EventType.CRITICAL_LOG_AVAILABLE:
                 key = "critical"
             elif event_type == EventType.ERROR_LOG_AVAILABLE:
                 key = "error"
             elif event_type == EventType.WARNING_LOG_AVAILABLE:
                 key = "warning"
```

## Comparing `nvflare-2.3.1.dist-info/LICENSE` & `nvflare-2.4.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nvflare-2.3.1.dist-info/METADATA` & `nvflare-2.4.0rc1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvflare
-Version: 2.3.1
+Version: 2.4.0rc1
 Summary: Federated Learning Application Runtime Environment
 Home-page: https://github.com/NVIDIA/NVFlare
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -23,45 +23,55 @@
 Requires-Dist: psutil (>=5.9.1)
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: requests (>=2.28.0)
 Requires-Dist: six (>=1.15.0)
 Requires-Dist: msgpack (>=1.0.3)
 Requires-Dist: docker (>=6.0)
 Requires-Dist: websockets (>=10.4)
+Provides-Extra: config
+Requires-Dist: pyhocon ; extra == 'config'
+Requires-Dist: omegaconf ; extra == 'config'
 Provides-Extra: he
 Requires-Dist: tenseal (==0.3.12) ; extra == 'he'
 Provides-Extra: psi
 Requires-Dist: openmined.psi (==1.1.1) ; extra == 'psi'
 Provides-Extra: pt
 Requires-Dist: torch ; extra == 'pt'
 Requires-Dist: torchvision ; extra == 'pt'
 Provides-Extra: sklearn
 Requires-Dist: scikit-learn ; extra == 'sklearn'
 Provides-Extra: tracking
 Requires-Dist: tensorboard ; extra == 'tracking'
 Provides-Extra: all
+Requires-Dist: pyhocon ; extra == 'all'
+Requires-Dist: omegaconf ; extra == 'all'
 Requires-Dist: tenseal (==0.3.12) ; extra == 'all'
 Requires-Dist: openmined.psi (==1.1.1) ; extra == 'all'
 Requires-Dist: torch ; extra == 'all'
 Requires-Dist: torchvision ; extra == 'all'
 Requires-Dist: scikit-learn ; extra == 'all'
 Requires-Dist: tensorboard ; extra == 'all'
 Provides-Extra: app_opt
 Requires-Dist: tenseal (==0.3.12) ; extra == 'app_opt'
 Requires-Dist: openmined.psi (==1.1.1) ; extra == 'app_opt'
 Requires-Dist: torch ; extra == 'app_opt'
 Requires-Dist: torchvision ; extra == 'app_opt'
 Requires-Dist: scikit-learn ; extra == 'app_opt'
 Requires-Dist: tensorboard ; extra == 'app_opt'
+Provides-Extra: core_opt
+Requires-Dist: pyhocon ; extra == 'core_opt'
+Requires-Dist: omegaconf ; extra == 'core_opt'
 Provides-Extra: dev
 Requires-Dist: sphinx (>=4.1.1) ; extra == 'dev'
 Requires-Dist: sphinx-rtd-theme ; extra == 'dev'
 Requires-Dist: recommonmark ; extra == 'dev'
 Requires-Dist: sphinx-copybutton ; extra == 'dev'
 Requires-Dist: sphinxcontrib-jquery ; extra == 'dev'
+Requires-Dist: pyhocon ; extra == 'dev'
+Requires-Dist: omegaconf ; extra == 'dev'
 Requires-Dist: tenseal (==0.3.12) ; extra == 'dev'
 Requires-Dist: openmined.psi (==1.1.1) ; extra == 'dev'
 Requires-Dist: torch ; extra == 'dev'
 Requires-Dist: torchvision ; extra == 'dev'
 Requires-Dist: scikit-learn ; extra == 'dev'
 Requires-Dist: tensorboard ; extra == 'dev'
 Requires-Dist: isort (==5.10.1) ; extra == 'dev'
@@ -74,14 +84,16 @@
 Provides-Extra: doc
 Requires-Dist: sphinx (>=4.1.1) ; extra == 'doc'
 Requires-Dist: sphinx-rtd-theme ; extra == 'doc'
 Requires-Dist: recommonmark ; extra == 'doc'
 Requires-Dist: sphinx-copybutton ; extra == 'doc'
 Requires-Dist: sphinxcontrib-jquery ; extra == 'doc'
 Provides-Extra: test
+Requires-Dist: pyhocon ; extra == 'test'
+Requires-Dist: omegaconf ; extra == 'test'
 Requires-Dist: tenseal (==0.3.12) ; extra == 'test'
 Requires-Dist: openmined.psi (==1.1.1) ; extra == 'test'
 Requires-Dist: torch ; extra == 'test'
 Requires-Dist: torchvision ; extra == 'test'
 Requires-Dist: scikit-learn ; extra == 'test'
 Requires-Dist: tensorboard ; extra == 'test'
 Requires-Dist: isort (==5.10.1) ; extra == 'test'
@@ -90,15 +102,15 @@
 Requires-Dist: click (==8.1.3) ; extra == 'test'
 Requires-Dist: pytest-xdist (==3.0.2) ; extra == 'test'
 Requires-Dist: pytest-cov (==4.0.0) ; extra == 'test'
 Requires-Dist: pandas (>=1.5.1) ; extra == 'test'
 
 **NV**IDIA **F**ederated **L**earning **A**pplication **R**untime **E**nvironment
 
-[NVIDIA FLARE](https://nvflare.readthedocs.io/en/2.3/index.html) is a domain-agnostic, open-source, extensible SDK that 
+[NVIDIA FLARE](https://nvflare.readthedocs.io/en/main/index.html) is a domain-agnostic, open-source, extensible SDK that 
 allows researchers and data scientists to adapt existing ML/DL workflows(PyTorch, TensorFlow, Scikit-learn, XGBoost etc.) 
 to a federated paradigm. It enables platform developers to build a secure, privacy-preserving offering 
 for a distributed multi-party collaboration. 
 
 **NVIDIA FLARE** is built on a componentized architecture that allows you to take federated learning workloads 
 from research and simulation to real-world production deployment. Key components include:
 
@@ -118,20 +130,20 @@
 ## Installation
 To install the [current release](https://pypi.org/project/nvflare/), you can simply run:
 ```
 $ python3 -m pip install nvflare
 ```
 ## Getting started
 
-You can quickly get started using the [FL simulator](https://nvflare.readthedocs.io/en/2.3/getting_started.html#the-fl-simulator).
+You can quickly get started using the [FL simulator](https://nvflare.readthedocs.io/en/main/getting_started.html#the-fl-simulator).
 
-A detailed [getting started](https://nvflare.readthedocs.io/en/2.3/getting_started.html) guide is available in the [documentation](https://nvflare.readthedocs.io/en/2.3/index.html).
+A detailed [getting started](https://nvflare.readthedocs.io/en/main/getting_started.html) guide is available in the [documentation](https://nvflare.readthedocs.io/en/main/index.html).
  
 Examples and notebook tutorials are located [here](./examples).
 
 ## Related talks and publications
 
-For a list of talks, blogs, and publications related to NVIDIA FLARE, see [here](https://nvflare.readthedocs.io/en/2.3/publications_and_talks.html).
+For a list of talks, blogs, and publications related to NVIDIA FLARE, see [here](https://nvflare.readthedocs.io/en/main/publications_and_talks.html).
 
 ## License
 
 NVIDIA FLARE has Apache 2.0 license, as found in [LICENSE](https://github.com/NVIDIA/NVFlare/blob/dev/LICENSE) file.
```

## Comparing `nvflare-2.3.1.dist-info/RECORD` & `nvflare-2.4.0rc1.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 nvflare/__init__.py,sha256=6Zj-5avHpObiG_j785ciqfk5JAH5sS-CyeE6G10YxvY,764
-nvflare/_version.py,sha256=1bt6Oub0rrdAx4d1cnuaDnULrLBrGyTMJqfSUrYl6Hs,497
+nvflare/_version.py,sha256=6eFejH9RuLVlIkCQOIxr9h_fM4Y4BHgUxcdclXi5-mg,500
 nvflare/cli.py,sha256=NKtVOYXHDzK8m06w1mykkRs0rPvRVBjKs7fmdTDCoUE,4979
 nvflare/cli_exception.py,sha256=oeTuq4kYgKko7RcgZvG4PLff7mzSMYINEOW1kxmsCiI,652
 nvflare/poc.zip,sha256=DB3EFSKVsh9a6FFqOohzKAt0-alRZyc8TCH1y7AUYeo,8219
 nvflare/apis/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
-nvflare/apis/analytix.py,sha256=EAFRdYqjtyVkap2iWpWjTLp1Pqz8qLyQyGzXYtI4LaY,7512
+nvflare/apis/analytix.py,sha256=lKWwVBkGFYLeH0vw_n2-XqGXb_j6qqEsSm53HrBgaLM,7730
+nvflare/apis/app_deployer_spec.py,sha256=wiBW81sbov029rIhbaKhNERtpDSRuFyofjiO8BlmeB0,923
 nvflare/apis/app_validation.py,sha256=CbILInWX6pfKUTniNjGbvJkiC4AEaQWFk3v1klAEix4,1323
 nvflare/apis/aux_spec.py,sha256=57DXy5HXuAcxTvzJMx1yD0Bj0WNL8yGyspZLpXZXgWw,1660
 nvflare/apis/client.py,sha256=TNmEIOloGl95v_dUXparZ7l90uneM144oqx-9aehQg4,1311
 nvflare/apis/client_engine_spec.py,sha256=TSpNngujfplvnLUDeqYkUUQK7zSUDeLxuVzBAE8S5Tg,1047
-nvflare/apis/controller_spec.py,sha256=EVOsDHepRChBKxqnzRSHoIP8UpWI5D65v6AwF3XX0fU,19130
-nvflare/apis/dxo.py,sha256=priv-spHFXEvBCOJz0UsyY0sRAhzbmUAnKAeI0_NFag,5500
+nvflare/apis/controller_spec.py,sha256=-29iN0BkJ7l2eh9vB61G6SX3Kv6MISGD8cncfjCajro,20102
+nvflare/apis/dxo.py,sha256=y0s_WTCMP_ElAxT-te9EKOx8cuhbuk00jdh0ZVps8Wo,7023
 nvflare/apis/dxo_filter.py,sha256=e1wiMjasun4htiL7yDneAbmELGElU3nETboULH-kNQI,5451
 nvflare/apis/engine_spec.py,sha256=3Y112ntvbbe7Rw882GoPbwhJa1oZcRvheHiAbvmvzlA,1028
 nvflare/apis/event_type.py,sha256=oCgRuE3gEaF2UWix1nfkUpyID8hgKaWw_hzVUgNrqGw,2571
 nvflare/apis/executor.py,sha256=TXXgWsRLc1n9H2I0T0qhTNUEX5yWsiTS8sLuflRSRBM,1791
-nvflare/apis/filter.py,sha256=04mNrBnZU8Ec7frRpHsRSVAv9iBjBLeGqzg1A-o-_KI,1773
+nvflare/apis/filter.py,sha256=OEYeQ7YY3ilg2jSb3-bsAPGDh7sgAL62VHmKZyo7QWQ,1777
 nvflare/apis/fl_component.py,sha256=YWSGsBhNaZpn9y0zJqX_GVwW5IqWSLuxsW5EcVIkwS8,9586
-nvflare/apis/fl_constant.py,sha256=35x3zZkZO-IzJQibrxFn2Pn3hvJCGeKAC8boFIPcFX8,10610
+nvflare/apis/fl_constant.py,sha256=0nwcS_iJlz4_hqlGA7LKCTgva23JGCt8-ZofQq4m53o,11020
 nvflare/apis/fl_context.py,sha256=RRlE9sV_O88WU5FFY9X6b0ZhYIGsIh2MZWSKMLTVOfM,12075
 nvflare/apis/fl_exception.py,sha256=_F126n0izHjRanTCSHkIdFlB0xjS1Cwu8U3o-MzW98A,1216
 nvflare/apis/fl_snapshot.py,sha256=qJFuMR0zbK7PWbtRbZvB6jPLEqMHEW2TSM_D49xt8MA,2720
-nvflare/apis/job_def.py,sha256=mme0SHC2Hzsa9rAunSL_3TIOZQFB4vzOZ3vzRgdT2nU,6149
+nvflare/apis/job_def.py,sha256=2PbUJeto356XcBkeiVNR7WcaKVjNP-dluByXwUe6PcE,6690
 nvflare/apis/job_def_manager_spec.py,sha256=A1R9c_oAHnrlCD8pB--63g2Mglfpn9-gVd32I9jLWIo,6626
+nvflare/apis/job_meta_validator_spec.py,sha256=b6LFEk-aDW-MYAXa2-CnAFOfb-cSf49zC0ZgCa4skYU,1039
 nvflare/apis/job_scheduler_spec.py,sha256=b4nJyndWiyUVCZtbLZ1iXuHxcG1EpeKBT7GfaW-njgc,2138
+nvflare/apis/operator_spec.py,sha256=gUEyaUzBt18LUjnWOr2SSD1o_VsPzdclwRwpdcn6nFM,1364
 nvflare/apis/overseer_spec.py,sha256=PaZ4G4iLgwMK3r_HhteKgnaV3tTM_MXViDb9pcojDBo,2083
 nvflare/apis/persistable.py,sha256=BoyQ2jGscp5NmJdbG935eGxMyZMdbkYylOiC2sdN4DA,1151
 nvflare/apis/resource_manager_spec.py,sha256=bsTFTidgZPBFYPIZ1bj8HT7Dzh5mI3n_HbblbnSkNAA,2894
 nvflare/apis/responder.py,sha256=pbRbIHoQ4N9cMLrqosmc43IvkJNfWN1YK-5zzKUQHTY,3297
 nvflare/apis/server_engine_spec.py,sha256=139FaMJEnWZtyM5XDJ8_TTU_yLflAJXi5q8-HNfZSCE,6094
-nvflare/apis/shareable.py,sha256=Im_2KCe6WU5LiT7SSlBy5fMmei5E2QUFKB09DXxKPUY,4877
+nvflare/apis/shareable.py,sha256=4DmqoQVxx8lfadCT_1AyXMcTX4PuuAssvGAbXDm_1mE,4917
 nvflare/apis/signal.py,sha256=NVrkubm9Kd3J2kzrZ_yoHJzR5Nq2TY5hpAoDCop-xKE,1322
 nvflare/apis/state_persistor.py,sha256=qG6hRH_jTl8k3QLu41Y6vBLbLpHPvGVwY4qmgjYbRKw,1708
 nvflare/apis/storage.py,sha256=LwB0_9kMw9M7ZBTNPmMpBDjCeqGYLtv19oh7MYfWZH8,4119
-nvflare/apis/workspace.py,sha256=UqqYmnqL_hE5_UaMghSbWoTJObcbt6LdwUZP0cIvuho,6467
+nvflare/apis/workspace.py,sha256=AiDFGnchr9M4vG4fEKpfT44d1hbUH54kXDx-1ffn_0Y,7331
 nvflare/apis/impl/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/apis/impl/any_relay_manager.py,sha256=yyyaZNM_48L31Z6ntAPr0UUyij7usmSam5AqOZ7cB6c,6797
 nvflare/apis/impl/bcast_manager.py,sha256=apnSGHa_VW3uImcBg1k6uohy5I9s6u2jjzo78vCPAZ0,5194
-nvflare/apis/impl/controller.py,sha256=aIDCOgqokwXLzp9aM1bCIPHcUAlzYJ0SGY_5C7XEe2Y,45931
-nvflare/apis/impl/job_def_manager.py,sha256=FOBvZYs67k9_oIHbPIbGy5jkJgIFvrkDxlK3MR303NU,11058
+nvflare/apis/impl/controller.py,sha256=A_C055IQFeN5poiUlfwsIMfDOUT6pARTi0YSuLhTPbk,46175
+nvflare/apis/impl/job_def_manager.py,sha256=oqAhNlGB9kxL1kU94ZwrmSV0xSBEpZusySdnmE5wWQE,11259
 nvflare/apis/impl/send_manager.py,sha256=G_hqwzu9wX98fgGNXq4wZDQ9MFG6xvpHQHVvqgSzgig,4727
 nvflare/apis/impl/seq_relay_manager.py,sha256=wfZvnRd3_InBHJFFWVMGUarBOH_u9v56QHMV3wPR1A0,9653
 nvflare/apis/impl/task_manager.py,sha256=XvxdvOJvbxSIE9DAqbAcs9sVCjDLnFdOOVf-qaquHPc,3787
 nvflare/apis/utils/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
-nvflare/apis/utils/fl_context_utils.py,sha256=NKlm4rqHtx0_6kur6-s1a_YqynZ2nbgha4AOLJxFzrc,3579
+nvflare/apis/utils/fl_context_utils.py,sha256=QqnwnPCruhpDegGgtlN186AZbMSpzL6S4h-unik5tig,3583
 nvflare/apis/utils/format_check.py,sha256=T7D2ISkh1D9J8pRoJKc6ovLwOUV-Lg-5GUqXn0b4m1M,2613
-nvflare/apis/utils/job_utils.py,sha256=W9_YcjQShIR6qFhDPvMK2Ps8mv-JUjImJeBE3CDXesQ,3233
+nvflare/apis/utils/job_utils.py,sha256=ZVBVLeypamSfa0-fL67xYCqcVBx-McLeWbKEOnKNJO8,3654
 nvflare/apis/utils/decomposers/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/apis/utils/decomposers/flare_decomposers.py,sha256=hUPKJCbqIm4BhL8NjUgyZ1PniK6l3WGw-a3EB7nsMNY,2370
 nvflare/app_common/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/app_common/app_constant.py,sha256=GtpEoWx9_VCkvyK1VBEuqR0KrmpqTUlXLsir2xr6w7o,6349
 nvflare/app_common/app_event_type.py,sha256=4dB8fpK8db6oB7jLcNiGyy4iGnvpm_4BBoaqP2bygVo,2844
 nvflare/app_common/model_desc.py,sha256=Z0iTICpCZKki75ZAstIdUmJuZYMjRKgBAyElghC1UwE,1115
 nvflare/app_common/abstract/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
-nvflare/app_common/abstract/aggregator.py,sha256=F1fXd_gzxiyeYeJORK603SZIWXfdxJAdRXQTHz6Vokc,1463
+nvflare/app_common/abstract/aggregator.py,sha256=LV56w6EwfISCJc_kFUC0RcftknuybwOXXj5lI1LO3Ks,1648
+nvflare/app_common/abstract/fl_model.py,sha256=xa8I3fNIaOp0PkhnuK4c7OPrAL0UnTjdNO8-VfWWeIA,4164
 nvflare/app_common/abstract/formatter.py,sha256=p25X5cTHnEha-QV0J-3bhkqyiWjAOHmWc76ZDKps-H4,1043
 nvflare/app_common/abstract/init_final_component.py,sha256=-ZC6DlKW6Hhhkz3Sc3zGO3msAmIaKMam4BMmRUPoHtI,1166
 nvflare/app_common/abstract/learnable.py,sha256=-OtSTbSnD-02I1DJQ3DV5vtTpvI9ZkZNVQxxESLzMQ0,1238
 nvflare/app_common/abstract/learnable_persistor.py,sha256=-LWsVgcAhSf1qzbDkNy7abTJLYdXQJjO2P8NlcFKF78,1335
 nvflare/app_common/abstract/learner_spec.py,sha256=0S-pUpKmPYff2_nM10-QftS2wAp7M4XX-VoNPctWuBQ,3239
 nvflare/app_common/abstract/model.py,sha256=2OGXoYrZvKhA_mEUgj6Io1YNxCg5xCbcJ6hLDG056H4,2288
 nvflare/app_common/abstract/model_locator.py,sha256=GTfzPTTihBSwhWKzwgIl6d-SaFSb4rS-BO-1VRt4Bjw,1361
@@ -66,53 +70,58 @@
 nvflare/app_common/abstract/persistor_filter.py,sha256=vDLZkRRlb5mLzYGSqetYCU9DfcJTRxJy8wyW8E0qBUg,2239
 nvflare/app_common/abstract/response_processor.py,sha256=5KnKSf861kQOUOscCy7-VmopHZYoeGb2sTjBDFxWzDM,2500
 nvflare/app_common/abstract/shareable_generator.py,sha256=5NwzEoJnJSuGrNy0w3cKvpK7VSCTDNivklnR9gemufI,1533
 nvflare/app_common/abstract/statistics_spec.py,sha256=HS9oCTe4YNK7mZFzu492L4oV8Xeakq6OB8aUrj-s6Yk,11465
 nvflare/app_common/abstract/statistics_writer.py,sha256=F2s4BEcscnvtmGeYgXfvIqsK_wIOVeQp6SL3YI45CXk,1192
 nvflare/app_common/abstract/task_handler.py,sha256=vqihb161OiwqvaAG4A3g2t_sGU-2d2gV0Jepscl09y8,2652
 nvflare/app_common/aggregators/__init__.py,sha256=rXvzHqG8yRfMZvQ9nIcYZMNcphaVcSKMJ84VTekXpEg,846
-nvflare/app_common/aggregators/accumulate_model_aggregator.py,sha256=-zpf_E8iDoeWQv5ll_3hRoLwTb7RZJ0pksA1QFibt1A,1002
-nvflare/app_common/aggregators/assembler.py,sha256=D1_UfEXRr5GBeicqjpnkz6oquaE81pPqL75toUA4WQ0,2465
-nvflare/app_common/aggregators/collect_and_assemble_aggregator.py,sha256=ql6875EuHs0bNOZMO-iuzqxSaKYGh-POyArxwke1gPA,4927
-nvflare/app_common/aggregators/dxo_aggregator.py,sha256=71-l8eIsNwTmjuaUDfnF-gD1AFb-AxZZMOO6iRBfPsQ,8443
-nvflare/app_common/aggregators/intime_accumulate_model_aggregator.py,sha256=nI6zxn7wWkofPBVHJOTu6eLKVfV_xatl6MSBmCqn-3c,11460
+nvflare/app_common/aggregators/accumulate_model_aggregator.py,sha256=I-xv49uryDYP3HwQhAabcObSxCZ8AruAqwLMGD5HPfg,894
+nvflare/app_common/aggregators/assembler.py,sha256=CvsAevmMwGghQ7FXOZ7V59wNkfWy7IzkeloHEW2rhwA,2513
+nvflare/app_common/aggregators/collect_and_assemble_aggregator.py,sha256=XJLCbvcHF-2XkpARwu9Mtk72OBXorZ75TbhMmGclTNA,4822
+nvflare/app_common/aggregators/dxo_aggregator.py,sha256=xOX8EZmzVXe0J6lMg7g46nJxuKmgRbQOmq0jPPWySA8,8500
+nvflare/app_common/aggregators/dxo_collector.py,sha256=0mougYjEgaP8_TV4dCfuEP39X7VyIuNINnzj1ymF__Y,1699
+nvflare/app_common/aggregators/intime_accumulate_model_aggregator.py,sha256=sOud2iS2V2dLvkHWv4KYXD_fpXtnWT_q92pbGfUEJ_8,11464
 nvflare/app_common/aggregators/weighted_aggregation_helper.py,sha256=Jmu3uDrBr-m6k5kUZ-aOyW6igp2FYyBtUc-mTtRBYvg,3436
 nvflare/app_common/decomposers/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
-nvflare/app_common/decomposers/common_decomposers.py,sha256=pdFV6Kjh3JsONCWCc975OaMyydjYbJQ_6nkAOJILdeI,3011
+nvflare/app_common/decomposers/common_decomposers.py,sha256=Q4aYcMhj2nyLKI3BrkNKdVezedaL6m66xJBHlcbsF44,3828
 nvflare/app_common/executors/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
-nvflare/app_common/executors/error_handling_executor.py,sha256=jAJqjt96xT9_Tt4MNmVl3pWxCBHxozRgwaxHWBxtGTI,4204
+nvflare/app_common/executors/error_handling_executor.py,sha256=vI7y8xHgzPvRTb5sQGeqvQICzIHE2KEehBhd4jMAkpM,4208
 nvflare/app_common/executors/learner_executor.py,sha256=qDdXgAKBT2SC7LPkMDWCy1IZR8zfixHy4PeKoQzwtQI,6755
-nvflare/app_common/executors/multi_process_executor.py,sha256=EmP7wEJjPh0ZQyVvqfUcOqYTcFMpJNlkxVdxuQFSWbM,13807
+nvflare/app_common/executors/multi_process_executor.py,sha256=3a7bI8cicJ6EZsFx8LiCUGqlcf32fhKLhtles3Zausg,13819
 nvflare/app_common/executors/splitnn_learner_executor.py,sha256=pjKjEbYkxmk-LFu3JhmQ04L_1wtDQG4wSDtGkiISn3M,4433
 nvflare/app_common/executors/statistics/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_common/executors/statistics/statistics_executor.py,sha256=1-uGU31OkJgLnv_oBNxly3xzK9ATWB1aFumAOtp7fUs,1792
-nvflare/app_common/executors/statistics/statistics_executor_exception.py,sha256=uwgcYTanhNKi79nKKidDU9Za-P5YzhZowUhS5Rc59Os,666
-nvflare/app_common/executors/statistics/statistics_task_handler.py,sha256=wcmF_F9gSMpSjltfw249wVu8Hoc2iTlj1KqOkWH5nf8,13518
+nvflare/app_common/executors/statistics/statistics_executor_exception.py,sha256=CIvAWZwcLRdR2N6peFND6MFfFDejkqjrkOwNdd3zST8,670
+nvflare/app_common/executors/statistics/statistics_task_handler.py,sha256=SFjyfW3zxEIC-G8GdeGKTMyLctQjUOG14z4H71o7yiA,13522
 nvflare/app_common/filters/__init__.py,sha256=H6vu0ECsW5iyHNmOgnG9tCfBlkRLjYoBtt984rlEPy4,797
 nvflare/app_common/filters/convert_weights.py,sha256=ZUdl9XoK1Ddjic2V-sSiv5X2ny8ptE-aYFJG2GJUqUU,4441
 nvflare/app_common/filters/dxo_blocker.py,sha256=enyiUGPUOjw5gYFwwMu8R3ZLmENb2MviM4EpstmW1Wo,2567
 nvflare/app_common/filters/exclude_vars.py,sha256=_vYN6haH4_6JmPEedyOGlnYF3gQ-e0gFFti8d5ZVwQ8,4804
 nvflare/app_common/filters/percentile_privacy.py,sha256=Kbz0V-LCD_jl_pJBFnOxKLDIWpTv2aBROhAglb27WMA,3902
 nvflare/app_common/filters/statistics_privacy_filter.py,sha256=y3tqJXO556qUqBmj9YTKw2c3ASsW2oYIy2oIGESBVbw,3309
 nvflare/app_common/filters/svt_privacy.py,sha256=ArHAco3n237hDexAZd7Q1akagGK6Q3Kx3lghdaaWSU4,5584
 nvflare/app_common/homomorphic_encryption/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/app_common/homomorphic_encryption/he_intime_accumulate_model_aggregator.py,sha256=TYhKhp4FfLuD8RUIb2kQfIcv-3Y6ImnvUhjjUVdiQ14,928
 nvflare/app_common/homomorphic_encryption/he_model_decryptor.py,sha256=jsFsnqtrhqfIgvLEsC4RilQaAPvqu7Tj5Fi-hSR5Kzs,870
 nvflare/app_common/homomorphic_encryption/he_model_encryptor.py,sha256=s0exgrhXBcbenv_kwUgIZo2mULU4smgGgO_thKlKOjQ,870
 nvflare/app_common/homomorphic_encryption/he_model_shareable_generator.py,sha256=l9C6P-p6Nv_tCXSDt8kVkYMyWAKogml9iyUut3dmv8Y,899
 nvflare/app_common/homomorphic_encryption/he_pt_model_reader_writer.py,sha256=yemmQpFM0BnNtcjiPi4LQsjjUTbgfwfRLVLXLVRazdo,889
 nvflare/app_common/homomorphic_encryption/homomorphic_encrypt.py,sha256=lUYKrThbHHgPt5DUkcCtSxu0tezvpMTLrugxRIORgxk,921
+nvflare/app_common/hub/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
+nvflare/app_common/hub/hub_app_deployer.py,sha256=2Toho3BRB43wE7iq76zzZIMDpZAosxf-D1vixlQOg4c,8229
+nvflare/app_common/hub/hub_controller.py,sha256=4UyISNxFpWMS4IqQ_0zbJSbur1DLcW8kRjK2nSentFM,20787
+nvflare/app_common/hub/hub_executor.py,sha256=3TxUmaJbN0tYcYw6UXgVVrhZdn0h2opC05o-QRjO17g,6504
 nvflare/app_common/job_schedulers/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_common/job_schedulers/job_scheduler.py,sha256=wqZp_iQyDB58k_5qO7I-qmcvAUtYHGjJpZJ1Ne0Sc8U,15917
 nvflare/app_common/np/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_common/np/constants.py,sha256=F8XXOqXk_IdZuzSgx6AVIqkjwHbBJ1NGTEURSfDBcJI,659
 nvflare/app_common/np/np_formatter.py,sha256=BkfoXNT5BkQ62u0tzrjcnIBV63goYx78RUhL4VWkyuE,2584
 nvflare/app_common/np/np_model_locator.py,sha256=erw4CIuSpMtZ1XIAuIDfGtg_jheFlw_jzwCOeqX4Ukc,3262
 nvflare/app_common/np/np_model_persistor.py,sha256=kiyUTV7leQv94QjfE4HvF5ibudfMTuWo7eRYzTyqF-w,3058
-nvflare/app_common/np/np_trainer.py,sha256=j84d2wVLSBtQ7bDzUm4pxpwjjRQZhhu7L9abkvUKgMk,8593
+nvflare/app_common/np/np_trainer.py,sha256=fW6yeD_n7fRkl647ecZq0FprObLDXAOyJQ6ayPWJkl8,8597
 nvflare/app_common/np/np_validator.py,sha256=6fiF_Wlm2r4abxhQwJnkXwiKMa8_TMp0O7lMK74TqsQ,5499
 nvflare/app_common/psi/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
 nvflare/app_common/psi/file_psi_writer.py,sha256=TLy9pb9mJ_lpVj8P6Jk2y3kcVx-khQWLH3fm__0m30c,2452
 nvflare/app_common/psi/psi_controller.py,sha256=LDtoW075sAMN-PN-Rp1ybBA9o4PNB0SDXJIKpFfnySI,2847
 nvflare/app_common/psi/psi_executor.py,sha256=Pry__io-tjqmrrllfuqIJL65_MD2of49IocQOucr7Xw,1906
 nvflare/app_common/psi/psi_spec.py,sha256=oir6nZjeXOYoGPHXUK7V3HKju9-h2J2j9kOA0DSYmTc,2883
 nvflare/app_common/psi/psi_workflow_spec.py,sha256=STveHewL_rKNWWsJckB7e71ovkjPVptuAAE1rTwr-eg,1223
@@ -126,24 +135,24 @@
 nvflare/app_common/pt/pt_fedopt.py,sha256=ZcNLlAO4KMjSE2TFhxYy0GwsKuTz8CY2GiVp2BR2kps,858
 nvflare/app_common/pt/pt_fedproxloss.py,sha256=Fi8vPDGlvlqteombFE_7KZ_pH8csvtmS3V2OjozscwI,859
 nvflare/app_common/pt/pt_file_model_locator.py,sha256=HWE10MURgTzvT0gCkX9383IucjsBLbe8cUx9UuzzcJE,878
 nvflare/app_common/pt/pt_file_model_persistor.py,sha256=db3Qi3zdfthILG0xA07BhkOWfIADwmFHaXSFrUgWeDA,884
 nvflare/app_common/pt/pt_model_reader_writer.py,sha256=rWkHFFgEKHWI4b6rSG1byNaEDXbYwZTVHIx6woGaIVc,881
 nvflare/app_common/pt/pt_multi_process_executor.py,sha256=QuPmEw7BfoCihl9FBZjgmDXKKixVbkj5nLqe2n4FbTE,890
 nvflare/app_common/pt/pt_scaffold.py,sha256=B-qqEhZ9HgygOu0m0A7RBb4fXEimG6U5DucOHewgvfM,871
-nvflare/app_common/pt/tb_receiver.py,sha256=tG7AeI9Z1bm9oxUW0Hq-6xAFxirzr8AcrpZl_lNRWT4,878
+nvflare/app_common/pt/tb_receiver.py,sha256=Jqpwd7Ti2OLXz-0vzBLowDRXAH1zxkxL-zaIkJXkm1E,881
 nvflare/app_common/resource_consumers/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_common/resource_consumers/gpu_resource_consumer.py,sha256=JhC40r4o24d1CPqn90sUfLtKhTwmvoEoQfPGVeY81Ik,1431
 nvflare/app_common/resource_consumers/list_resource_consumer.py,sha256=shkMkad9AhQUjUnC83DpJRY4tO1OH1I-AVOAfvQved0,1734
 nvflare/app_common/resource_managers/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_common/resource_managers/auto_clean_resource_manager.py,sha256=XBYfJPVfD4DaHJZOFnyD1NJN8YmvIlVQFz8FZ5z3640,7594
 nvflare/app_common/resource_managers/gpu_resource_manager.py,sha256=KOPYy6DMriHXjY_gypDICtaeEJVngW0H2MeCvtZJz1o,5519
 nvflare/app_common/resource_managers/list_resource_manager.py,sha256=NPsvPuQ0VNC_65J1xtZMjhVkuqquEKNSAYAoJfIzkPU,3285
 nvflare/app_common/response_processors/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
-nvflare/app_common/response_processors/global_weights_initializer.py,sha256=-0rxeAg7o78UiK2oCE9o7qVT9vQki2zeMDQ-StkayNE,5494
+nvflare/app_common/response_processors/global_weights_initializer.py,sha256=XDkOgYm1tCPDRLTuLACWX_96hh3Pg-62psXeyPrDKjA,5498
 nvflare/app_common/shareablegenerators/__init__.py,sha256=JK-9gZzjXrmFe3VdERtU0Duig2zAhPnD46Y75OezhMg,726
 nvflare/app_common/shareablegenerators/full_model_shareable_generator.py,sha256=-REuq4WAyT93MDmnUQ8wjWnqvdWs1_XjYoj-IKAbCSs,3328
 nvflare/app_common/state_persistors/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_common/state_persistors/storage_state_persistor.py,sha256=PG-n1C7HmFYXQSS-0cuLcsRid-UkmCKTVBFvPbCcR-0,2987
 nvflare/app_common/statistics/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_common/statistics/histogram_bins_cleanser.py,sha256=4BvAY0cppN3vKbYH3eFKCn19k1AY2rmzZaTFskOK06o,3841
 nvflare/app_common/statistics/json_stats_file_persistor.py,sha256=lqBCNAsjMcO87eSijWSmxnKQHHkGRWmJDJHnhKzEDnA,2945
@@ -153,355 +162,398 @@
 nvflare/app_common/statistics/numpy_utils.py,sha256=39R8Do-LCQeikUYMkt89cunvFy3yJNXyVheLZ8NMn9A,3041
 nvflare/app_common/statistics/statisitcs_objects_decomposer.py,sha256=t8cPTPs9HYi4NMjbPg7RSrpyMWZDEvYEBtfw60jENGw,3274
 nvflare/app_common/statistics/statistics_config_utils.py,sha256=1e4yNV1fiBa_yCPA072FeWl0lqbo090g6Vu4acR3IV4,1201
 nvflare/app_common/statistics/statistics_privacy_cleanser.py,sha256=XTdL1ZC6Lm7l87qQkuGA0FBEvb63MJXkgd4QtoIDx1o,1906
 nvflare/app_common/storages/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_common/storages/filesystem_storage.py,sha256=ZSWM0yQtTuWLfIeFBmxAOj8ytRpcPYQVzsNBq5iY27g,9072
 nvflare/app_common/tracking/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
+nvflare/app_common/tracking/log_writer.py,sha256=OP9Dg4Rwp0qOhwbHzCU87fkvf1qfo32XtRStDvcAxBI,1565
 nvflare/app_common/tracking/track_exception.py,sha256=yRjx9BhWGvoE32uF9eJRmXVAE22cY6V69K_rmd0lZyw,988
-nvflare/app_common/tracking/tracker_types.py,sha256=P1q2ty4-j1j1QI51GwOKzZ-_e6bMarDYg3kfe5YdpK0,2275
+nvflare/app_common/tracking/tracker_types.py,sha256=vV6mJDh92nViwv0TLmXhQXwfBcplTCdNclQr9j4VGpM,1419
 nvflare/app_common/utils/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_common/utils/component_utils.py,sha256=Ytb4YeobcIXc0UqHLI9XQpkMDks_F2bUMibL4xSfZVA,774
 nvflare/app_common/utils/file_utils.py,sha256=hrYIHagaatAULg-1_qB3AOyeZjh_EttpOtKNE-N0sgE,1135
+nvflare/app_common/utils/fl_model_utils.py,sha256=eLqsTr5lP4M0n8F5sCPUOcNMCTdKRegrnYdVgeB3qpM,5764
 nvflare/app_common/utils/json_utils.py,sha256=tvY2EYPflViY0PUG9cwD7SLfwcu2sYow1ACCDXXwxnU,1730
 nvflare/app_common/widgets/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/app_common/widgets/convert_to_fed_event.py,sha256=sVbWF8vsy5TsxKBNsSgMVlrpcMM2pIH8wHmasHY6UTs,2119
 nvflare/app_common/widgets/event_recorder.py,sha256=xxYoe8pO_CTgXvD75HQhHOqZqoIF4lbCIdUH4EPEiJw,15452
 nvflare/app_common/widgets/intime_model_selector.py,sha256=HQf6H0bBcyd9qvb0OU9DmPS6jkR4c2fH2aOv-PonPn4,5926
-nvflare/app_common/widgets/streaming.py,sha256=0-ZG9OgLg9f13Cg3Vw3SR4OACBpWK82UB1G8rqM0qUo,9297
-nvflare/app_common/widgets/validation_json_generator.py,sha256=vwd47HK0KOStM8hG4Aee-HiIp019VeuWd-NIQOQg-Q4,3808
+nvflare/app_common/widgets/streaming.py,sha256=Ae47K81EowIsCMISRPbEAwNSKusm0F5EAEpEuY7-efk,10386
+nvflare/app_common/widgets/validation_json_generator.py,sha256=u8agxE9veNWJzYJxnhMWqkW2do1IIA3EChnGoaAzZ3E,4673
 nvflare/app_common/workflows/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/app_common/workflows/broadcast_and_process.py,sha256=C4bUS_syaf9bh5FlKfR6PBDsZSM0wartVVk-1pc6hMk,5293
 nvflare/app_common/workflows/broadcast_operator.py,sha256=4j6rzxgg-6NVRtz9Cc-lXhpVqm6JquICgwFDFt6v87Y,4083
-nvflare/app_common/workflows/cross_site_model_eval.py,sha256=87O8CQx0D85Tpw9lvCPUAFmLt60IOtmDh39xMRTePfA,25598
-nvflare/app_common/workflows/cyclic_ctl.py,sha256=YGUUfOzj3ngwSIcUOOxZlmOKNhbDigS1N5p0tGqkyKs,11412
+nvflare/app_common/workflows/cross_site_model_eval.py,sha256=qe7xz4CPRWCJ_7IDixkdtAn5WV-yKFMqKHMFofv8Tlo,26530
+nvflare/app_common/workflows/cyclic_ctl.py,sha256=8C7dITPjXGu2iidT9u-2PeGm1Ppt2RG6yB07ZEoQgUI,11589
 nvflare/app_common/workflows/error_handling_controller.py,sha256=fcY-LXayt9m6BXZ8mb6byjvatpYrBI8C55C5QrKK9xo,1880
 nvflare/app_common/workflows/global_model_eval.py,sha256=Dapms3384x-NvwGyRoBm-E0qSiYlaJUazYyiw1gXnhs,2945
 nvflare/app_common/workflows/initialize_global_weights.py,sha256=ldpkVZ0EVGOHgCS6wbbS4K66L-LVbiHRwZA-7WtjyOw,3023
-nvflare/app_common/workflows/scatter_and_gather.py,sha256=8Lj6FWG8viZIBsFy2aPwUEDMYVgoLF9W7_73c-S0ZKs,19381
-nvflare/app_common/workflows/scatter_and_gather_scaffold.py,sha256=9vx6ZOuy8TlBmKrc9go4HFHwAipPDT6S9dexHEZrNCQ,11586
-nvflare/app_common/workflows/splitnn_workflow.py,sha256=iczTiJcODQi3aMMq1cPPQ3xAPlYRPkB56mIvI6M9LTg,13125
+nvflare/app_common/workflows/scatter_and_gather.py,sha256=pKD5t0MLnQw_Z8hc4SWDaHJng5Tc9ar3pgxPHd_14TI,20050
+nvflare/app_common/workflows/scatter_and_gather_scaffold.py,sha256=gawJY2N4r6cjnBRU9-6lyCIINgmUIU6q5Q65rqdXSL8,11826
+nvflare/app_common/workflows/splitnn_workflow.py,sha256=qEi6oOoren_DXSs0ZNeQ5CJXmirWY947SFGnCqrY-bQ,13129
 nvflare/app_common/workflows/statistics_controller.py,sha256=TRzTEaLFQyaQ4p5kn3pdcnBwTAk0dybMFVlb25hVs6Y,24627
 nvflare/app_opt/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_opt/he/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
 nvflare/app_opt/he/constant.py,sha256=FcfrwQUkuI3sWr5T34KwBK1JpJLCIO9CRz7G5CWGVZo,638
 nvflare/app_opt/he/cross_site_model_eval.py,sha256=IvK4saS4HHRMe7OMQEUAwfNjeCxcveSWIElGlagTl40,5823
 nvflare/app_opt/he/decomposers.py,sha256=6YqitytZ-mGKGb3qyREqQQHbcxuAxOZzAYDJoBad2xY,1309
 nvflare/app_opt/he/homomorphic_encrypt.py,sha256=Wo1O6UgR6gUYWNGtrePwLO4ZivUP-ovKcJ83mrWk0TI,2498
 nvflare/app_opt/he/intime_accumulate_model_aggregator.py,sha256=FGUMEpW85WZMiq-rB7e_h41cVC3rqFlk5EA2JEhi_Uc,3184
 nvflare/app_opt/he/model_decryptor.py,sha256=SK7Y7BjU30t5qr6IxJrSy5JJcLV5UydJI3c9tnDmhmA,5552
 nvflare/app_opt/he/model_encryptor.py,sha256=nn8oX6RSXAB_6h_-zZTt47yBDTJnsdzCSykijL8T4rY,9884
 nvflare/app_opt/he/model_serialize_filter.py,sha256=_swlKv--7ifvARwCdRlj9-o4JY78exPunv1ILT77-40,3367
-nvflare/app_opt/he/model_shareable_generator.py,sha256=K0nEr3hDFNepXgHT2WO6MuapGBeLrs1FAJU0XzRm950,6331
+nvflare/app_opt/he/model_shareable_generator.py,sha256=b3-qLkFRZkvUtN9ueg-DYZ3ON0_Z6AjQFWAOv4sR0Co,6339
 nvflare/app_opt/psi/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
 nvflare/app_opt/psi/dh_psi/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
 nvflare/app_opt/psi/dh_psi/dh_psi_client.py,sha256=yuV-dwLWFEaPmF99f3f3f2P8iiCDclsbr5ygg3y1Ysc,2414
 nvflare/app_opt/psi/dh_psi/dh_psi_server.py,sha256=ezyPTP7zhTYeRjS1GmNYxz4T6ufxmkYCyzbKlrpdHiA,2485
 nvflare/app_opt/psi/dh_psi/dh_psi_task_handler.py,sha256=Q4pTkiC6sWywO3way5dy8TA7M2yp4bbDvQjuRvct3kg,6861
 nvflare/app_opt/pt/__init__.py,sha256=353BYzId92C-H2qalfHdnPgRTDBsRt7qAzBmbiVkJ2k,1370
 nvflare/app_opt/pt/decomposers.py,sha256=OpTmf6ZiIDQCaPg1aKGOmyilldo0JFrHknJWKH2JL2Q,1286
 nvflare/app_opt/pt/ditto.py,sha256=eyXOpD5pBThn93ImUYUW5noneURSeBouUCjd0b2fApo,4894
-nvflare/app_opt/pt/fedopt.py,sha256=UficJUPUVHm5Vu88kYUAhd6jEeI_y9NEVqHlkwE5tI8,9328
+nvflare/app_opt/pt/fedopt.py,sha256=UbuJOETP2hVUVttvFzc4iipjEBWkAE6yr5LiXETbpok,9336
 nvflare/app_opt/pt/fedproxloss.py,sha256=WrxaEVfsygvn68l_BXkp1Xz9PS92cRZpM-bYOuJRChE,1634
 nvflare/app_opt/pt/file_model_locator.py,sha256=IlroBuMbIc2DVbBWPV0YHbqCcwlWfr-F_JcjxxhCp-g,2996
-nvflare/app_opt/pt/file_model_persistor.py,sha256=EovGnaTVD3_KseJkBxIUqSur4Eh0swV8PI1RrTQKWGo,12584
-nvflare/app_opt/pt/he_model_reader_writer.py,sha256=QNhAxU8-bITr-lkYP_S5Y_kz8W8I7fFCrCh8WQAwpPA,3070
+nvflare/app_opt/pt/file_model_persistor.py,sha256=GX8B1CM2cOl0y8MrWe9BrFMd38S9Fy72DKhG1LGVsIc,12627
+nvflare/app_opt/pt/he_model_reader_writer.py,sha256=sRvvbWMypdKFrz2dv8hiimyAkpybBIIP_xkR0Bu7V58,3074
 nvflare/app_opt/pt/model_persistence_format_manager.py,sha256=Lyx1Eeun_bWCG0g6MlQVjNY7NAQUnCT_I_x_DBTnQDs,4901
 nvflare/app_opt/pt/model_reader_writer.py,sha256=_QpRcVlou-Xu42ujdVMx7yGo3PsCtxUrii2-wEit2W4,2889
 nvflare/app_opt/pt/multi_process_executor.py,sha256=DwLBmMSMXc4QKVWsdttJHHI2RubK7JyMJzcDFPLaA7E,1153
 nvflare/app_opt/pt/scaffold.py,sha256=Gv8wxoP4CbQu1KSi2Eh3oswEl1KW9233p6ipckgou0I,5047
 nvflare/app_opt/pt/utils.py,sha256=ZcI5ZHd-N5PuZCMCh-rXsJ9-wUMk0qTkCQWcEHNMSX4,1943
 nvflare/app_opt/sklearn/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
 nvflare/app_opt/sklearn/data_loader.py,sha256=2HUkoLfzmNUZzkOWdccVcF8HN6_wSPHtkDeanXUwHGg,2133
 nvflare/app_opt/sklearn/joblib_model_param_persistor.py,sha256=inTiJt-S_JXbuu82Zy2OPm9Hq5klzY4_yjMVTOAUL5E,3226
-nvflare/app_opt/sklearn/sklearn_executor.py,sha256=saReqm8IV_AO3DQmS5FuEYLjX1GQBi_9icEEhZrh3S4,6176
+nvflare/app_opt/sklearn/sklearn_executor.py,sha256=IoRL_QTNKhWE40k-qVqCcipT9oqWpEJszso_NGDULCE,7289
 nvflare/app_opt/statistics/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_opt/statistics/visualization/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_opt/statistics/visualization/statistics_visualization.py,sha256=4vArYCKNYsZbiHkjXDiGXfH2ZqvcvHJs8DqylKfL2jo,4470
 nvflare/app_opt/tracking/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
-nvflare/app_opt/tracking/tb_receiver.py,sha256=km3F3dnqDE1zEiu6q_oxeCNx9MHRvX5M7f72fA8UEkk,3870
+nvflare/app_opt/tracking/mlflow/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
+nvflare/app_opt/tracking/mlflow/mlflow_receiver.py,sha256=F_x5DfZUzKkUI-FrhvXu02ER1DkRJepdSVgrdSeTo9w,14967
+nvflare/app_opt/tracking/mlflow/mlflow_writer.py,sha256=I7PGTRnSfQKEsbsqhwZz_ajoVtecf6XL2V1Od9nf0AY,5569
+nvflare/app_opt/tracking/tb/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
+nvflare/app_opt/tracking/tb/tb_receiver.py,sha256=wdLTcqOR0nOePb5xSdgD52DFDqUyU7PoB8sIfUpswMY,3769
+nvflare/app_opt/tracking/tb/tb_writer.py,sha256=8pWUfr2IGEEAwJGsjOVwHfxrGtxPNyo7SblP6EUx0qc,2416
 nvflare/app_opt/xgboost/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_opt/xgboost/histogram_based/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/app_opt/xgboost/histogram_based/constants.py,sha256=EcKRdQeRHzXIvOF4vyja6AnFDhgwI0y0QeV_SbED6no,807
-nvflare/app_opt/xgboost/histogram_based/controller.py,sha256=NCdh6lR3B6UezPiaOcy328V-eV7HZJkwAykdjckHKxM,6964
-nvflare/app_opt/xgboost/histogram_based/executor.py,sha256=JF3dQ7nqiAf5SF1kSBDnd3Yxssk48bK95InYDHhqOjU,9712
+nvflare/app_opt/xgboost/histogram_based/controller.py,sha256=EIJ7q6-FdwJmvP-R2g32Vft6iiwiYiZVArBTyGt1P_0,6968
+nvflare/app_opt/xgboost/histogram_based/executor.py,sha256=9W_d7lFCsxJMEMPl28h3MiQ4UjMf0Srhpq_Wi84tIVs,9716
 nvflare/app_opt/xgboost/histogram_based/executor_spec.py,sha256=VHDCK93excP6cmhNwja15vqY0rFXNRmKr9M-_j8AI20,2143
 nvflare/app_opt/xgboost/tree_based/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
-nvflare/app_opt/xgboost/tree_based/bagging_aggregator.py,sha256=Iuhtt1FOvf9cqIkYVpPSdx7ZwqZb4iUH3u530RK-wtA,5078
+nvflare/app_opt/xgboost/tree_based/bagging_aggregator.py,sha256=jUwiL_j670T6zcep2sVnZjc_TfANiXVYrEHt7wJt7bo,5082
 nvflare/app_opt/xgboost/tree_based/executor.py,sha256=j3VEwKapcoutIiWFzudRL4Wu_85y8W0W9J4x8_MLmko,11777
 nvflare/app_opt/xgboost/tree_based/model_persistor.py,sha256=haw8VHzOaIDsJ_vtusGGJlZIH0vjsLKUUEu_ikhLJjE,3666
 nvflare/app_opt/xgboost/tree_based/shareable_generator.py,sha256=UESYoSY50YDVozP1elm12HrEHy4GpWtbdOeLUVT3psk,6830
 nvflare/dashboard/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
-nvflare/dashboard/cli.py,sha256=LzsVi8P-n91z5Reu5h8PzMkmItyJDbASXuwz5LpMyF4,6767
+nvflare/dashboard/cli.py,sha256=lIOrvE4caW340KMdqaTr6zAoAYBXg6mhQvdPdMROLSo,7388
 nvflare/dashboard/config.py,sha256=FUPxQBkLQhFQba9w6Fx9r5xn1HGThMl0hvLJ-2BdtRo,1268
 nvflare/dashboard/wsgi.py,sha256=ktC6BislzwHL6gaOHFjwcyQlFgKoiIb05om8vSud87s,1229
 nvflare/dashboard/application/__init__.py,sha256=gagYc7ecYmXexaeSC0LxkjdDPBtX9tD64DQYNuop6AI,1697
-nvflare/dashboard/application/blob.py,sha256=6BJYNeWk7qiWKfWp7wzs9gmJs5DJ8Q_hEBN52sSxjUM,14394
+nvflare/dashboard/application/blob.py,sha256=mKZMaR-_fSJAa5EoOJOZwXpmLQLOn3DhFjQOF9fV5lM,15738
 nvflare/dashboard/application/cert.py,sha256=iYI0cM1Rj91lQv68R4z71BHcpDhySqwddW9l3s-RbRo,4940
 nvflare/dashboard/application/clients.py,sha256=6RJR7RYCiXHqjMQ8wdJKTd0ij-Gx5IxP6eZV9rhN1R8,3001
-nvflare/dashboard/application/models.py,sha256=zfriib3Hco9yFJRVszy_pB8dKsLO9FoU-YUMYj947iE,4487
+nvflare/dashboard/application/models.py,sha256=Y7mdDcKO8OIf7WSRApmZzZO0jvxtTcZh2s83XXXTXvE,4543
 nvflare/dashboard/application/project.py,sha256=U5is44aJUNZCEEmpp55zMX_e5tsEhuSm8KN-zdutQLE,4401
-nvflare/dashboard/application/store.py,sha256=ceBlksTwyWf_JJ4uDleDOLQtaOEEF0rTALlpA4DeUls,12846
+nvflare/dashboard/application/store.py,sha256=Owa8YvKsBE7MFzw8WK3VJcFauod1FlGsDue8ImzzIYc,12862
 nvflare/dashboard/application/users.py,sha256=q0_yL0nVZliL6TRKGIbqXjjj7hHGXMM_cljLHk2TsX4,2918
 nvflare/fuel/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/fuel/common/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/fuel/common/ctx.py,sha256=cC3eR877oq2M50JCLPV36mh89knqYzU1UMnuqkYqoCA,2062
 nvflare/fuel/common/excepts.py,sha256=74Cd7KgEtFEjFXZyPTtHaVzGxbolI1nfy3VCgBErd9U,711
 nvflare/fuel/common/multi_process_executor_constants.py,sha256=ymQsr8fT0str81ji2LNZCUIZpIgFhXpdo_iugwQJWpE,1571
 nvflare/fuel/f3/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
 nvflare/fuel/f3/comm_config.py,sha256=pw7mKhnFzQMkCwRlSi694yzCnSdO1UKGi4Btls_j42U,3259
 nvflare/fuel/f3/comm_error.py,sha256=Rrs6SgLZCC0PE7nosen_vQ5lSXs4TOo5fvxEYH0K040,1116
 nvflare/fuel/f3/communicator.py,sha256=joYn1hPYSH97XIk8_7Ji_oGVo1ZR_cZP7Tmu6UQT9kE,8760
 nvflare/fuel/f3/connection.py,sha256=8mEDp6QmfmHC-Aax3lAKHNu4iUDdiblsAfAHTmEH4hY,3733
 nvflare/fuel/f3/endpoint.py,sha256=s7sy1lYchAtEjf58DE2rT3d3FnGckQldaJ3roCjiIbw,2198
-nvflare/fuel/f3/message.py,sha256=mNFhD7BUr6AYwXDeE0wnnPVbYBYYBw54zO_A5sXuh-w,2136
+nvflare/fuel/f3/message.py,sha256=79Hep7MXPRGusDEugZCg5hGyOAfxOe84g0C6bpnYlFM,2033
 nvflare/fuel/f3/mpm.py,sha256=IzvyNaDwaNP-GKBOQpub6ISK84RY3CDfkIP8R7Dyiow,6247
-nvflare/fuel/f3/stats_pool.py,sha256=tmwdHNW1_YO0xeOjJU-0t8JoTIxBYlzzb2ulCo8oQXs,3837
+nvflare/fuel/f3/stats_pool.py,sha256=vyAs0rCu-L8j9treFEjC-my_tfb1jfwWFc4z--mKv28,19445
+nvflare/fuel/f3/stream_cell.py,sha256=62dRjVsxxWYOJrsdCi8YMEhWcsivHVmwfGlpgekS84M,9813
 nvflare/fuel/f3/cellnet/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
 nvflare/fuel/f3/cellnet/cbs.py,sha256=xHBkQyYg8veZN45yeseYemBn5SYZeHZelY--PwQ53mU,1388
-nvflare/fuel/f3/cellnet/cell.py,sha256=n4wLBaKU_n10Q5rLXLDnsuca0MR_uvHEmpcsbhAeFdk,82944
+nvflare/fuel/f3/cellnet/cell.py,sha256=TH_IXPspb_uMd2Q3gExGr_5sS-je5jiSDEk1QVuNu8s,81908
 nvflare/fuel/f3/cellnet/connector_manager.py,sha256=7dRxLE0j9bDn_ttRpZpfmncqYtRq5Hw8cIoj_t8XJjA,9249
 nvflare/fuel/f3/cellnet/defs.py,sha256=GYWueYlD1A2byQfluCfCjG9QKRccgMoZqUyqh4nxApY,3367
 nvflare/fuel/f3/cellnet/fqcn.py,sha256=kr7rWyx1LeAoAtgPiwQHJ9qC3-fIOKkKwmUk8-WFhrs,2498
-nvflare/fuel/f3/cellnet/net_agent.py,sha256=WW3YZp86UOKvuneAi0thi4jvJsinhBIf4qTkDiXGKMk,34394
-nvflare/fuel/f3/cellnet/net_manager.py,sha256=wP3XG_SmOz3ikoDq4vYNIfUHzbfxZKCbblvao1jJe9A,17335
-nvflare/fuel/f3/cellnet/utils.py,sha256=p4d8YtBb8Jnmbw0VDN1WmB63LtnTodbh_gdWwf6WoNM,2676
+nvflare/fuel/f3/cellnet/net_agent.py,sha256=WIEuGf3GYKmeyPH6svOZOGOR2ZxeRCYJZIMlaOFxwBc,34221
+nvflare/fuel/f3/cellnet/net_manager.py,sha256=JiW8wvK7zzap6Tr-Nk_xsD8V9FB3p2rrUq3hfknO700,17331
+nvflare/fuel/f3/cellnet/registry.py,sha256=uAdcnKXbqrKhnZkYso2b4R1Uemv7OsX7gcyjKk9NLW0,1743
+nvflare/fuel/f3/cellnet/utils.py,sha256=fvxzYBkaBZo8a58EJqx2rAMpdWno1TXRh8ig82JYHMI,2452
 nvflare/fuel/f3/drivers/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
 nvflare/fuel/f3/drivers/aio_conn.py,sha256=_CrGyKZxHAlmFmKy_CQ5l95nACDZdy7yYxujZcRSE1Y,4963
 nvflare/fuel/f3/drivers/aio_context.py,sha256=QzoP5CobCnwcU63l1ElcnAJrV03VrSaBIGU016hGRoA,4354
 nvflare/fuel/f3/drivers/aio_grpc_driver.py,sha256=TDsXm0XrQ_n1sIcGwPrWU83-IOcjDl05x7AKH7R6_D8,16267
 nvflare/fuel/f3/drivers/aio_http_driver.py,sha256=iV59nfj3SgcjU9F0HwszjmORhprhKtUaQnIKHKKRQWI,6470
 nvflare/fuel/f3/drivers/aio_tcp_driver.py,sha256=oLmRq2SqllgA79LlZwvsaHjPAj6_2HRCccu76CvS7go,3895
 nvflare/fuel/f3/drivers/base_driver.py,sha256=0QdKz9kUZjD9zLp6B-jjbtYJCiXvUQECcojDX-Dw6M4,2376
-nvflare/fuel/f3/drivers/connector_info.py,sha256=0N1R8UYLeriFzcKBs5znsX8ehTJPzYt_VF8y0RupLd4,1154
+nvflare/fuel/f3/drivers/connector_info.py,sha256=CDYAJC7AaU7RIhiUgdCKRnijPge2oXyd6tGeXSzQIGM,1122
 nvflare/fuel/f3/drivers/driver.py,sha256=UWoSJ76AF1IW0-Gf6CnmO-bA-UtJ8LOo6YgxCelRUg8,3583
 nvflare/fuel/f3/drivers/driver_manager.py,sha256=oq0_BawyoUO47cIa3qLRkszFoR5M-3G2dULsWR4NXAs,4108
 nvflare/fuel/f3/drivers/driver_params.py,sha256=DjuNSGJYwXlC7Vjfs0Q40xpyPwAfW5CM0YVek0VKyNE,1380
 nvflare/fuel/f3/drivers/net_utils.py,sha256=-dhRA7tvc7xa-WN12LZeQkhrB5O0QK8Fvm_OkMS4OQY,7632
 nvflare/fuel/f3/drivers/socket_conn.py,sha256=DDsZ1IQexuxlZXytB1_gWXwVfyJYhuGoiSfmVeSByJM,5550
 nvflare/fuel/f3/drivers/tcp_driver.py,sha256=3Yeo3XRmk3Jmkzmynz4D6egPAqKFkw2KP5qFy3pj5-A,3622
 nvflare/fuel/f3/drivers/grpc/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
 nvflare/fuel/f3/drivers/grpc/streamer_pb2.py,sha256=6853f-OiJkHBbG1oi4WlxacQZJZXDomr8NUtXOBL_tY,1840
 nvflare/fuel/f3/drivers/grpc/streamer_pb2_grpc.py,sha256=oXtnDUvTJMkkxrUAly8WXZk7fItUWv8Aw3uv6m1UdcI,2817
 nvflare/fuel/f3/sfm/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
-nvflare/fuel/f3/sfm/conn_manager.py,sha256=vAq0pTCzcqzQZY01ByMa2QKCbFlWq3CKMJik6ROQRHw,17618
+nvflare/fuel/f3/sfm/conn_manager.py,sha256=ZbwZEZ53KHTN8q4vQdi1g1w9FL5lbyzdhJWqO8DZO2A,17630
 nvflare/fuel/f3/sfm/constants.py,sha256=15RiirEXcRyS_I8M6tQpx3UhrC2v-18OLFJX4UIIan4,1082
 nvflare/fuel/f3/sfm/prefix.py,sha256=GFjRBwCGq_ufSIIeSpty0FyVcPu_BTCPPyHHHT3YRNw,2417
-nvflare/fuel/f3/sfm/sfm_conn.py,sha256=KAFWx7ALmmw8a0VsRDKt05u_j_M5O-v637jzCH9f5Vc,4928
+nvflare/fuel/f3/sfm/sfm_conn.py,sha256=MSUr953jxO1GC0mjWr33j42bDLDplQPyQIw5PyH3UTE,4888
 nvflare/fuel/f3/sfm/sfm_endpoint.py,sha256=AzbkSg_yAQ2d6xOybH_EFpTVumgyiNCRb_v0V5WijfA,3088
+nvflare/fuel/f3/streaming/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
+nvflare/fuel/f3/streaming/blob_streamer.py,sha256=yn4llJOX5OvbnxrmQNmZPdI6aP6zjseMV2TvYa4psMQ,3906
+nvflare/fuel/f3/streaming/byte_receiver.py,sha256=q8FI9NbTtIwT1SyHaVGQXi1MQae-wZqbHbizq2rSM-0,8229
+nvflare/fuel/f3/streaming/byte_streamer.py,sha256=fZ0-SuNBkCc8Qvul2aB56Wyo036eMrT0zEWW8xWJaLA,7577
+nvflare/fuel/f3/streaming/file_streamer.py,sha256=16aX-3NK0DYQi9t3BtXw2vbdrunJAuvW_fn87KSc7cI,3675
+nvflare/fuel/f3/streaming/object_streamer.py,sha256=DgLVrRi7vPjc3RBGT-5fCOViZM9Xjq9g-KcJmUZ04S4,5078
+nvflare/fuel/f3/streaming/stream_const.py,sha256=wpS2BYvnJoH-Kig837xXVoU10uO78F_q6wascs_5dek,1565
+nvflare/fuel/f3/streaming/stream_types.py,sha256=MpA8unOEemd_u2QEDNL-0EXNCdsGHNVCnntYB2f5glY,7840
+nvflare/fuel/f3/streaming/stream_utils.py,sha256=kKMIW0L9nikg_E7Qnh-_-8VXLOnKUkiwmDd6pX4YHM8,1268
+nvflare/fuel/f3/streaming/tools/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
+nvflare/fuel/f3/streaming/tools/file_receiver.py,sha256=xCY-yrUtOhUj7d97P1T7CkCxIuLn9fVSTnoJEeE61Ds,2779
+nvflare/fuel/f3/streaming/tools/file_sender.py,sha256=wqmNmK6aS6Uiit-t3JiUWA4gJBr3Lon_Uxa_z51SUyw,2549
+nvflare/fuel/f3/streaming/tools/receiver.py,sha256=OxDw7iPqzDfmeidI0Mf0_yjjY_0lCtvnJ-ra73Busi0,2169
+nvflare/fuel/f3/streaming/tools/sender.py,sha256=GKLvRWMeY85ZbmWZRAqsKLviN3-3Ginv_oyfl37VlYM,1640
+nvflare/fuel/f3/streaming/tools/utils.py,sha256=fPIXgos2L8BuPqeBLBXrjOA7aP4FLnuHbvunWfpRXQo,1544
 nvflare/fuel/flare_api/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
-nvflare/fuel/flare_api/api_spec.py,sha256=eNatpEtKru18cyF0ReWBAASr4zISy_cPueGDVbx4fPU,6518
+nvflare/fuel/flare_api/api_spec.py,sha256=MOMLXAlpOvkrsnNSfbijkve6-7Fq-ii3geAkM3LWPsI,15841
 nvflare/fuel/flare_api/config.py,sha256=JUpr3It3nxS0Vll8I6tQdY3laBtOvwhn6rz_FtfVwaw,3107
-nvflare/fuel/flare_api/flare_api.py,sha256=FRr2IWgyI2uzMn9_wHTy1dpo6E8wlyrSvVkSmf5_HVA,18877
+nvflare/fuel/flare_api/flare_api.py,sha256=lcrO0ZTr0MhOr-78259opZ01sTWI2CbM8c5w0bfrFRQ,35086
 nvflare/fuel/hci/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/fuel/hci/base64_utils.py,sha256=pH0vRyHSKVr37vckIOlA99urszFbwWx9dCjG8htCM9U,2541
-nvflare/fuel/hci/cmd_arg_utils.py,sha256=z7Vt91wLTT16t2lS5RBcFOTJnU6TauUJ_pitMd0pFr4,2036
-nvflare/fuel/hci/conn.py,sha256=MzlQLUFbbqleQLn8GeeeWRNAU8JNdBf6kdderpbcM7Y,5674
+nvflare/fuel/hci/cmd_arg_utils.py,sha256=bXCRvsk6ddhem7aG1xAmhtGtgxMnLiemH1sKKAyL7_s,4691
+nvflare/fuel/hci/conn.py,sha256=YAyZWEJrR1UFFt3IgXFJzN2EjovgpDEbarUnUcUdYGc,5752
 nvflare/fuel/hci/file_transfer_defs.py,sha256=5eZDqojl9KaXW5_Wylnw3J9nBkMmN57yzSej66TiJJY,1254
-nvflare/fuel/hci/proto.py,sha256=hpK-X1k8_nH-pmYxYUpfrOCc-kAyqMkqDy3NytWFnOE,6196
+nvflare/fuel/hci/proto.py,sha256=BtcLtxTe7amU8p9eAQj_WeQFv8rgFcB6_mZnFJvjHx8,6636
 nvflare/fuel/hci/reg.py,sha256=unLSHlSpqts88_M7Owc-7JUdwU1knDUT7HXPr9w6oFY,8408
 nvflare/fuel/hci/security.py,sha256=q8_9sMXUBXXYjhV6qhqS-LHZ-gHeamNZHoJon8BgJUA,3773
 nvflare/fuel/hci/shell_cmd_val.py,sha256=WvvFpF8zQ4u_dujmUptVErJ8W1XngpGuS4tcrWLPExw,4136
 nvflare/fuel/hci/table.py,sha256=i8puxvjf2FOSNM29OFBTDphVxNjIu6gFIyu9fwRiFTY,3352
 nvflare/fuel/hci/client/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
-nvflare/fuel/hci/client/api.py,sha256=PLssoVigi8cMiABNkLfus6nDrWrrHi1vWtmCSjfJ92c,32607
-nvflare/fuel/hci/client/api_spec.py,sha256=g2WPki02LWVq-T8OXynGpV28KkaXokq7G_9EZauMeZw,4974
+nvflare/fuel/hci/client/api.py,sha256=8n_sPIPPGg8lo1A2AB6b0hYMgTf1wPeNN3AbSdvQwsg,34099
+nvflare/fuel/hci/client/api_spec.py,sha256=hh1LUQv-yT9gOWfOK3FhckIRN08PZSPXk9SkW1g_OKc,5011
 nvflare/fuel/hci/client/api_status.py,sha256=MS_GfBSwibkCzCa6YQfQUAo8SZr0bvfkht0DtGb5tCE,1607
-nvflare/fuel/hci/client/cli.py,sha256=LQJr5K1JK3oY_ZnKq5KW5MTshUmi1P8Kd-Owa1_1FSs,18067
+nvflare/fuel/hci/client/cli.py,sha256=Fu-ZIyKAgWEBTkZLKz_hTz9g9d040UmuMVFIUG2YWK8,18850
 nvflare/fuel/hci/client/file_transfer.py,sha256=m7Jvjg-PM7qr8lIXjjwvvlCnb3-M36bjghYRwpXLr2c,13935
-nvflare/fuel/hci/client/fl_admin_api.py,sha256=X_jpEFE7ifz9clbbCkgbtN75aEzDzDDNj7BwBPaB768,48215
+nvflare/fuel/hci/client/fl_admin_api.py,sha256=IfBqbtTG-Km0iZctr7tkwxjYeGPVsuqN-GzOC6OJiIU,48451
 nvflare/fuel/hci/client/fl_admin_api_constants.py,sha256=oWDFDyHn_uMsieD0uf9awcVyJbrs05qtZlOfHar1u6g,1071
 nvflare/fuel/hci/client/fl_admin_api_runner.py,sha256=86EXEIz1CDJ_dVXQ6DMMdT0g8N42S9tymcK6up1cj0U,6734
 nvflare/fuel/hci/client/fl_admin_api_spec.py,sha256=_CvEbOHpX6Vbx3Qn40VSISLCZyOEvotsn2OUBsMdFQ4,15874
-nvflare/fuel/hci/client/overseer_service_finder.py,sha256=vQuBKbJKAKg3y_UmYY-hxsTN2TANYof_fDqp1khEzyM,2476
+nvflare/fuel/hci/client/overseer_service_finder.py,sha256=wsWPOcfEheMGTpohoLvUy_GEuXay6zzKzG4C-4-Ar0Q,2475
 nvflare/fuel/hci/client/rr_service_finder.py,sha256=F6NUCJ-TPW6cfnKJlGRN8B7rhDbhUdKRBv2KLZs3Ako,2047
-nvflare/fuel/hci/client/static_service_finder.py,sha256=4VPQVXJt-VlTqqujYeo_7tDr4kJAD_0L_99e5zUu-T4,932
+nvflare/fuel/hci/client/static_service_finder.py,sha256=Wl2sF9aZlxZ3qBmZ_AVcMEYS29XO0JxKY3gOulyLj60,966
 nvflare/fuel/hci/server/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/fuel/hci/server/audit.py,sha256=t2AIloKX9SOXiUfFXAWzjIac6a2aQtyMqRUy3mievn8,1640
 nvflare/fuel/hci/server/authz.py,sha256=VitVAvjlXpBxQTdXS5_Xe8vw7oyZ3IdvF7fdlEGZZIM,3231
 nvflare/fuel/hci/server/builtin.py,sha256=sZIoN7HAsgaLqTGGtYAtmJMnHbelzM_hUnZ-SjEV_NM,3377
-nvflare/fuel/hci/server/constants.py,sha256=N05iaTFiTLT9Z62r8WTc5f5X2QZrYqZaXOc11-6V360,1208
-nvflare/fuel/hci/server/file_transfer.py,sha256=tojkeFTlD-PsmyB2IlH_bNg8OX9kjPIqU-YVEucloWQ,7964
-nvflare/fuel/hci/server/hci.py,sha256=lPIhVxDl6FOTPIDtYEwyYhghpLzA0u8uv8OuWgFYphU,6437
-nvflare/fuel/hci/server/login.py,sha256=qr3Bsl4TRuV91lDPj7VmDaDTi1EOEo-s1OX1thd27Bo,7646
-nvflare/fuel/hci/server/reg.py,sha256=6ZBzyLJHhJgjKs86W_DRZlTA9rLIFEuiQbU7lEgW-Co,3874
+nvflare/fuel/hci/server/constants.py,sha256=mX3I_Susajc9DpKoT1EVQhWdqKbf4rsiIV91qoub2mU,1240
+nvflare/fuel/hci/server/file_transfer.py,sha256=Ap9UM9rxeyll6buvojwWdeIHg2mJxkd1VFMl8MnIAOo,7968
+nvflare/fuel/hci/server/hci.py,sha256=XCzFNoJ-LowuQvhb6QmCGgBJWV7QcKn_Gqew_Oq_yUI,7176
+nvflare/fuel/hci/server/login.py,sha256=oeq1IBgZHEeGBaVmceyxIN1ZFds3q7IKYZmTNREDZeI,7654
+nvflare/fuel/hci/server/reg.py,sha256=PvE_1qnOvak1SfTilxyRvBDmKauZlcqhrYjTra8Zm-4,3878
 nvflare/fuel/hci/server/sess.py,sha256=6aE5ZQRwGzuf3PYh7KiTCrkPBTtGwKq7SUZ_IE8dK80,6464
 nvflare/fuel/hci/tools/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
-nvflare/fuel/hci/tools/admin.py,sha256=M9N8W5PgYXzhL7Ih4dtDlG7Bgfn9yukKDb0jS_JD8NY,4147
+nvflare/fuel/hci/tools/admin.py,sha256=bttJmBq7D-e7rPQ_n7Yoid67Y9l08UH67FFICO-Tmxc,4179
 nvflare/fuel/hci/tools/authz_preview.py,sha256=JlsfqKQr8V08RAc0cSstXqe3TnwEzxtVnh98Efo5g_g,5149
 nvflare/fuel/hci/tools/make_pwd.py,sha256=M8OVTD5ZRJN6L-LApGIyJ5kLsVEAAtq3ehFYz1y7zWc,1198
 nvflare/fuel/sec/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/fuel/sec/audit.py,sha256=2Ca32iMAMzZqkZXBBFqBgW5O0o3qJjVF2ukzxfJm1pM,3907
 nvflare/fuel/sec/authz.py,sha256=pVDn34sHVk5sJFONBIgdcgcK-G84f8IJ_Lg-W3bFdwE,15241
 nvflare/fuel/sec/security_content_service.py,sha256=27ncBKLEbxFHpuMsgyMoW8EollnTB3TrzgSPM7_W7DI,5241
 nvflare/fuel/utils/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/fuel/utils/argument_utils.py,sha256=RAUYht7PtYHa560XQYEzQ65rTQgI4hsJ6H_Z5r9M86A,2773
 nvflare/fuel/utils/class_utils.py,sha256=OAJDY_JBI0haF1SlkCvFUTiMlRhoaLqRiMbYTiu8bGI,5832
-nvflare/fuel/utils/component_builder.py,sha256=PXNREYMk-K9m9dan9vrXjMR0wzCRNDoKyrhe0heGXwE,4373
+nvflare/fuel/utils/component_builder.py,sha256=gFOnN5gb-DFfD9lrply5ZsJm8YuxhRytC_GbUETzIkM,4377
+nvflare/fuel/utils/config.py,sha256=1_5xnReCUaLEKIwaNS8GUBluoqxJ6xpsQgRi3J3e4CU,4645
+nvflare/fuel/utils/config_factory.py,sha256=Op5vVri_VgjF0HsYyCqguT1ILxxtPFP4mHlgmUyVjbE,4503
 nvflare/fuel/utils/config_service.py,sha256=olF73rvadSLkTUUiI9wdfgrlSGj4Mh8cfA7FftADjNU,9389
-nvflare/fuel/utils/dict_utils.py,sha256=55MVQjlrsCKoZTAepQN_j2XCeGI0pBSrcnkHsVLKHSg,4066
-nvflare/fuel/utils/fsm.py,sha256=3FEqQfjc8mp3-4btFMcb7S_O1OJ-mQ6crCxP4Pi8Yxo,3137
+nvflare/fuel/utils/constants.py,sha256=mdL9BO83bFcOufRcKq_ZZpsXdS4eRw6bOwzYhuIlEEA,704
+nvflare/fuel/utils/deprecated.py,sha256=0fQYPQ3JtvCGquhYE2t11rq68FLblYfHWJpCPf_4baQ,1858
+nvflare/fuel/utils/dict_utils.py,sha256=flbroNoSV2ZlxKnh9vuYxfxiGlLi4d1gGVYLoxkIS2A,6024
+nvflare/fuel/utils/fsm.py,sha256=-xTfB6sfIR3w3uLke41JPHrgLWPHWP5nBXWxxdyY-yE,3314
 nvflare/fuel/utils/gpu_utils.py,sha256=rPnI3Pz994_DlksUO4vwKTicUCytGoXLcyu-1R59Fu0,2113
 nvflare/fuel/utils/import_utils.py,sha256=NBzm2sbS3gMUIE5CHKgb06gkYzhWOAL5lv43AjCjv5U,7347
-nvflare/fuel/utils/json_scanner.py,sha256=jqZRa5PFpD_5sTn3n9GGM1nNbtRJakuCLFxxmIhDXW4,4941
+nvflare/fuel/utils/json_config_loader.py,sha256=DNmXE2MAr1BwxZm43FyczvmjiBr00x6fB0Ealiki7ZE,2327
+nvflare/fuel/utils/json_scanner.py,sha256=R7kJidjn7wPC50YtIdcAEHaDVANxd4qOCO4xbnwlnM0,4949
 nvflare/fuel/utils/network_utils.py,sha256=o4r6lIvAPYNvpazuzZbANIa_RI7UfyPpnNdx55hWg8s,1259
 nvflare/fuel/utils/obj_utils.py,sha256=ZZvNitCxbu7egZLtkCCXoffnQGO5nYj2EyuDjwNWad0,1349
-nvflare/fuel/utils/stats_utils.py,sha256=FFSwaaY_2KkyxaBeL86yKt1EUjhBy5HzGdQ3_T35aI8,10876
 nvflare/fuel/utils/time_utils.py,sha256=GZ0pdMNCpGepk5Y4GUI7L4CpmJk8d846_cdZldSyYhY,924
+nvflare/fuel/utils/validation_utils.py,sha256=zbNZYnvOBIQif4Y65lpyKknSmdKOges_J4J5wBaK9EY,1938
 nvflare/fuel/utils/wfconf.py,sha256=NlGduFJzPfkf9sT-r4aRF5op7lv3MQcvroXzKAyEyS4,10957
 nvflare/fuel/utils/zip_utils.py,sha256=WnqkLwllC9Phms1smZd1dvmY87QhYawZMaEcy0rIugg,5278
 nvflare/fuel/utils/fobs/__init__.py,sha256=bXk9fSgs_9VSFNIvrSIzIYS5WVRc8dMq1fnv4OC-z4A,1072
 nvflare/fuel/utils/fobs/decomposer.py,sha256=PxMmVf99Cpk5HFfdblA1ErzDJQOWfIxc_rOE1dv1JBc,3788
 nvflare/fuel/utils/fobs/fobs.py,sha256=2bW3rDiR8_0JtasqEoI5Sb3Adt4vdUb_wMT2dXBVq5s,7652
 nvflare/fuel/utils/fobs/decomposers/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/fuel/utils/fobs/decomposers/core_decomposers.py,sha256=mU0XP_XShOXWEaIeSWrp1C8WtX0_sY3pvFPAluCHaQY,1815
+nvflare/fuel/utils/pipe/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
+nvflare/fuel/utils/pipe/file_accessor.py,sha256=2xma8oS9cUIvErfWCyysjw1ktCFphurlUhar-cdyPG4,1163
+nvflare/fuel/utils/pipe/file_name_utils.py,sha256=NUUsJ3ScjQczK3aCtHVlyQetXM0qfXE5gTxNoOgftd8,2280
+nvflare/fuel/utils/pipe/file_pipe.py,sha256=7EbbHEOO26LQLuBo0awVK5iMAC5UYNtwJdJ7PFMA8aI,8613
+nvflare/fuel/utils/pipe/fobs_file_accessor.py,sha256=2hXIZlNrZZqnJhGEkE0rm3_kTXLz3WHgDLHwg24cVmg,1429
+nvflare/fuel/utils/pipe/pipe.py,sha256=RV9xAeUIdEqW8jeNmhsAThpZ_1GXCr_ZM550hIrvVKA,3531
+nvflare/fuel/utils/pipe/pipe_handler.py,sha256=fwOon5R2zJzKCSsp71zMDNwiSkCE9XK4FOrSh77EZAA,8554
+nvflare/fuel_opt/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
+nvflare/fuel_opt/utils/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
+nvflare/fuel_opt/utils/omegaconf_loader.py,sha256=_L9EtiqlqR8AFtBwlwlQcWVWUannrzjrIDcupw5wfuo,1982
+nvflare/fuel_opt/utils/pyhocon_loader.py,sha256=WreoKRnMBOGPu5rFFFRr4kPitvtQ7CshMlMznKRVLAk,2843
 nvflare/ha/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/ha/dummy_overseer_agent.py,sha256=3t8YdBOhML1EygQ0r5kgXyGJP-LEwkVPECzW5k5juDA,3875
-nvflare/ha/ha_admin_cmds.py,sha256=ZE40cMZN8YZV6juXP8yKxUlfDK05IazulR4wtE0ZnjE,5583
+nvflare/ha/ha_admin_cmds.py,sha256=tcHW4sxznJiSv4a7P-Z2tD8VejFxQKv0slXAmpMEPao,6098
 nvflare/ha/overseer_agent.py,sha256=qddPDlwLi5GauUVLR_ZsBrE5YZ5_dlXbFBJjnhUFSwc,6452
 nvflare/ha/overseer_agent_app.py,sha256=vbxpmmr22wC1enKyKRgWTDZ1jOEhNkrdR4WWY3Ri67Q,3477
 nvflare/ha/overseer/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/ha/overseer/app.py,sha256=1U3WrcNxS6HEHmrP3DbZM9SK2rWAOEXa6IsAgodcsOo,701
 nvflare/ha/overseer/mem_store.py,sha256=NAYlftvw6z7q__tnnxgF2GLD2u4pF9xPSVKQUItvH-c,1716
-nvflare/ha/overseer/overseer.py,sha256=AQOndEaKLeuRFaT2BTxd6P9PQ5-TSa8xu4c9WR1Xs9E,3540
+nvflare/ha/overseer/overseer.py,sha256=uTERKcrVGDILiXe8QsYLNpTrMof7uSC4zz9OCvRrZbY,3544
 nvflare/ha/overseer/utils.py,sha256=hdhN5Igw_8vOCNI-PQ8ITTWnNdar3Ccxz1vNU1E5nqA,3144
 nvflare/ha/overseer/worker.py,sha256=ZUPszkrXLJS2VyFglQXpql_XQp8wsY90e3W98pbNlto,1197
 nvflare/lighter/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
-nvflare/lighter/dummy_project.yml,sha256=wI7CqAuRU7067XyudStFeKy15fnpC-LsSH9vi5ES3nE,2045
-nvflare/lighter/ha_project.yml,sha256=hOwBT0KuFpCtrw403Sm8awIoe9uqy2uan5C5Fp_F9PE,2636
-nvflare/lighter/poc.py,sha256=reagALAorIo8Ohi3TC6FbJHDpgeTXbPSGROOHr1Vbmc,3915
-nvflare/lighter/poc_commands.py,sha256=9jnPEvJZAXXM-q8crbnO3f1_7Sr5-umRt8UsDCaY1Y8,13438
-nvflare/lighter/provision.py,sha256=Hlp4gSevJJ8Ih5ylKJACxBPmX7QVZNUlyopT5jfRHxo,6198
-nvflare/lighter/service_constants.py,sha256=5q1vEozHNgJKu16uGSHorlWnhR2SWueWAbkyV5GKCGQ,887
-nvflare/lighter/spec.py,sha256=4mdwwEvUtGENu4mDbZoKj8-fxtxP4XutlaaahmMVRQM,7022
-nvflare/lighter/utils.py,sha256=1YC6wc1DClCoecNAD1UaGTFbAwe271JpuSqZ4JSkzmk,7880
+nvflare/lighter/dummy_project.yml,sha256=y-IWorqIgrHVOR63bX694eBZD7B_uWkRiiHERzEjU24,2155
+nvflare/lighter/ha_project.yml,sha256=RWTVYCkI2lX7wDXJ21IfGZB5HZY1bzPX-ah5Px6RMN0,2752
+nvflare/lighter/poc.py,sha256=vmXglOzcBUvwo9fA4mkLh4CuWHzRt7qUvcppx80XU9Q,3923
+nvflare/lighter/poc_commands.py,sha256=qIiG2uuaMzgnc4ZqhVUnD-vL_d7FqVzhv99vrGbYXog,30470
+nvflare/lighter/provision.py,sha256=QIRSZGYAOQEX77U1Fc6M5GSbyB2YIo440re4Vq62yH0,7312
+nvflare/lighter/service_constants.py,sha256=Ww6iEtgyLO9aFtplmE7vBDiMT8K5Y-QzHGNmkz7VBAs,939
+nvflare/lighter/spec.py,sha256=bDui0RqOI07GPdJU4YNjLRrk4cL4UqOKLn48kyfhcWA,7026
+nvflare/lighter/tplt_utils.py,sha256=Xw9_-POlB_gbmNM6UbdmgwFdLaLp9YFgBiMFOJq-3ck,791
+nvflare/lighter/utils.py,sha256=4ZmtbQKWUxa-nTd3PYEpuV-ct1hQmphw-l5imgJ56gU,8392
 nvflare/lighter/impl/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
-nvflare/lighter/impl/cert.py,sha256=gpFFKpLXPXDOeAXsxyMOPXD6WsvVkofPylycirw1afI,8317
-nvflare/lighter/impl/docker.py,sha256=AaV7_vRcCLNm1cJZ6Yjjdl33ja3lRqT9e73RhWjrcsE,4784
+nvflare/lighter/impl/cert.py,sha256=aXn2K9Q4zgcPLn5p4saS8eyjmrFww5RA3nvcLJF6mlc,8413
+nvflare/lighter/impl/docker.py,sha256=wWJqNHqki3apcIZxCJAaXA_YPP0NcXzqQ1CaIwrBjKw,4788
 nvflare/lighter/impl/he.py,sha256=q14wP8vQRo90kcvrWMc9dTHyDfEASkleboCo_Yl_xxg,3177
 nvflare/lighter/impl/helm_chart.py,sha256=kPGBkINvhweze7wJMfW_IhhafOYjUj-2lfjdaPt7oM4,6123
-nvflare/lighter/impl/master_template.yml,sha256=9uIwtFeLpyGVw_PeG21gnZVf3E5XZ9LH2ktwMWneTqo,62178
+nvflare/lighter/impl/local_cert.py,sha256=81cd61xEWkJc4rOvB2F6U3y_dqiUO8zLYXmQu9F2tBg,861
+nvflare/lighter/impl/local_static_file.py,sha256=oSS31WwleQ1akbMWPA7N1xU6akdnyM7VMGYI-TTBly4,2836
+nvflare/lighter/impl/master_template.yml,sha256=QsaTAW0XCxeAXefkWT805k-xTl0waadnyXyq9ajX5fM,65602
 nvflare/lighter/impl/signature.py,sha256=tfaYByr5vmn3jF3Gs0Z3L4eT6F4iJCvsw0l3A7YkKtI,1903
-nvflare/lighter/impl/static_file.py,sha256=0-cqT_MutRxe7R0syOpP0EsfWIqMspW-baA9Dcli_G0,14480
+nvflare/lighter/impl/static_file.py,sha256=MJHx8OAfRWtYsls9QPd-65HDLCiGX0zZEGBwxR6Yz2U,15041
 nvflare/lighter/impl/template.py,sha256=NsUrZU4mokXRvwgTSHRcal5_CojobS6lSNTrbwNvzcE,1299
-nvflare/lighter/impl/workspace.py,sha256=2-ohjC6sMUrAS-43ZKZxZvT-4kbJe7itUNWATEzLOMM,4157
+nvflare/lighter/impl/workspace.py,sha256=USmXAGWll8iD4Y7KzrSbXb7v9EnmWtKHlUdPbrWBZkE,4127
 nvflare/private/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/private/admin_defs.py,sha256=whpXHTw2P-dh1a_qVPdWgiVVHpJ-YUQBSHKFPvmzF2I,2581
-nvflare/private/aux_runner.py,sha256=2B8saxIV_M7tiwsXbABpZnIO9PJFyTkYEvhSvRAEJCM,11175
-nvflare/private/defs.py,sha256=PUdY1k7AH7e83ozRSvRjUFiQkk1Owv_sA4YG-RjkHkw,4551
+nvflare/private/aux_runner.py,sha256=eKrrtDcVbAr2HSOmov51a5iFE9ANoUCBM3PRnidQs4g,11126
+nvflare/private/defs.py,sha256=8v79AXmLrxXfnB14_tqZ-BuOpCZ7irNkSA3uSPElfi0,4535
 nvflare/private/event.py,sha256=-dNxODoSxY575cKNgDGzHWJ_e2heHblN2jpJRSMmz-U,2923
 nvflare/private/fed_json_config.py,sha256=enPUfD2RtYpqO_EobH1KpzrgaSzl1EEr2sMEWc5lx0U,7536
-nvflare/private/json_configer.py,sha256=5AMqMXDBzAu6MHBzh3CdoU3r_RDM9LnD3NYnBo73B5Y,5366
+nvflare/private/json_configer.py,sha256=Jljl8TK6rG4JxhjdLYZ9dLXg7-Sii1bEqOxZHG8yiPI,5370
 nvflare/private/privacy_manager.py,sha256=7syCb5f_uCtLM_Hho3HrNHoRD3F2sMuPO3mRoblxbxs,4226
 nvflare/private/scheduler_constants.py,sha256=rXidh-7CVl69x5ZnEWOhuljasehNCuH3hFvZdXAZ5so,737
 nvflare/private/fed/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
-nvflare/private/fed/cmi.py,sha256=Coaj_xDGGTmTjzippQrzOoVf-KlOl-5wox4S--fCyo0,10032
+nvflare/private/fed/cmi.py,sha256=LVsK0Yu99-6MMGXpcN3C45vKjnBrEO5l5MIBO1A0wGY,9975
 nvflare/private/fed/runner.py,sha256=mLraPV4wx7jVsuo09S_rGHf83COg9uMv7s9LHZf9vtU,919
 nvflare/private/fed/app/__init__.py,sha256=_lPUcH87g8jmxCyILRWdt0-ki2d5FYFu4CaGEYiPQKA,641
 nvflare/private/fed/app/default_app_validator.py,sha256=ZIHYOqXtrPUiRauT8Lv3OB3DjNFIzMnUsyo54irA8cU,2092
 nvflare/private/fed/app/fl_app_validator.py,sha256=c-W4W9nN_AjAiSo1tOzT9Mn57RXcxBfqjpV7gz3s7qQ,1783
-nvflare/private/fed/app/fl_conf.py,sha256=ah60UhxEOOKXUwI5_m9AhJSFUq41uIpFTw7x-ZTDEUc,17853
+nvflare/private/fed/app/fl_conf.py,sha256=f9WgwxPxthmOwfwoRbOYXzjib-8w9kmlOoUOPqCAMnY,17861
 nvflare/private/fed/app/utils.py,sha256=Wpb0t0bdu-GWNDxzDqkdPle367QV2yQuMrcysqNuOmQ,3209
 nvflare/private/fed/app/client/__init__.py,sha256=jdFyCaXD-_JN_-OM4gdd7SyVdTdSUbvyxN4k1ufA9zc,648
-nvflare/private/fed/app/client/client_train.py,sha256=vDxHOmpd-ZykN8ns-UgXgjtanjrKCIMjuzWvhNxKa0w,6322
-nvflare/private/fed/app/client/sub_worker_process.py,sha256=YlN0vlcErDqgZACmQYLmOHz8tm2Q7LsVgA0bTWb05oE,13818
-nvflare/private/fed/app/client/worker_process.py,sha256=HsL6emSVQNwSvY5ALTCIN2O2GWKyiYlcv_5_vJ7TZ_0,7016
+nvflare/private/fed/app/client/client_train.py,sha256=0hZKFaAlIUI8IAFhOUhpJL3FXAXIAuBD06r-yq1YdCg,6326
+nvflare/private/fed/app/client/sub_worker_process.py,sha256=vDEmVmj1zFArbN80DIl0UnBwBbxR9wzywU0Ks_Cwvs8,14191
+nvflare/private/fed/app/client/worker_process.py,sha256=2qZBuelhmKTAcMTiB_jwwPJZeii5sTNXFIZxYDHUFu4,7284
 nvflare/private/fed/app/deployer/__init__.py,sha256=MziKYifmgDeKVpyjkPudiADRA53q8LO0G3OYdz650kA,649
 nvflare/private/fed/app/deployer/base_client_deployer.py,sha256=aGm4O7eirkrOU7lk8IaFwbPEi3BLQxdKmGkz7b2Uwz0,3603
 nvflare/private/fed/app/deployer/server_deployer.py,sha256=1xEIZ3N3brwH1Hz2wX-Opf-A81VhwXTAU4aHF5WOsc8,4862
-nvflare/private/fed/app/deployer/simulator_deployer.py,sha256=B0BEx1efnVam7KdZIZhgpccvbI2yR-RpLHcCShn1OLI,6152
+nvflare/private/fed/app/deployer/simulator_deployer.py,sha256=E9Cokku2-JJd4RKQK0Gxa6LeZbZD2YyBZATLPviEmxg,6156
 nvflare/private/fed/app/server/__init__.py,sha256=e4lrIjiSpbNU8IgAUlGkiS2e26Hey_XHahN7IegtJ0g,649
-nvflare/private/fed/app/server/runner_process.py,sha256=91xqxgzuISqiSjJbPpPlbPbvtmACxLuZCzaBcmpctEY,6356
-nvflare/private/fed/app/server/server_train.py,sha256=XVqafkTIBz0mm9TpHbulrgpNYt9sTgB_clbCP0DnVCY,5786
+nvflare/private/fed/app/server/runner_process.py,sha256=ytaPibinGFnQhqOwF402mJD2kLZ5SMHVIHPBP2tUDHk,6630
+nvflare/private/fed/app/server/server_train.py,sha256=lAxx2o6cdS0cylWRNhalgbLxWnpRJOcLwmDWTi_GGW4,5790
 nvflare/private/fed/app/simulator/__init__.py,sha256=E6fKUounlwKXqjcFk1mGr2EtHyDSL0PEWLA1OE7XzS4,636
 nvflare/private/fed/app/simulator/log.config,sha256=zo67fEx3ml-_DktQ9_7W7FUhIXL3a3uskECSZ65ZYlo,323
 nvflare/private/fed/app/simulator/simulator.py,sha256=6uD-82VylsYUoAbk7bGiWpU_hQxi1kBq4-FcMmGZcuk,2574
-nvflare/private/fed/app/simulator/simulator_runner.py,sha256=sG49dLlPZuTrodGwuMIZzDAoD1nvnDGQ2VJscqLdDJM,24803
-nvflare/private/fed/app/simulator/simulator_worker.py,sha256=I9MfZN1aYXqSecW9qtU5Gb9bLDf2MDluenc27Jfxs4s,11272
+nvflare/private/fed/app/simulator/simulator_runner.py,sha256=ekiTsgo_mlaL4r8MLmt4EsBAuNLJcGVvFFSXur1mjus,25568
+nvflare/private/fed/app/simulator/simulator_worker.py,sha256=9Eqt8ouFLusoUrkdcrEIxnhMyNSVu71sqIHqLWEAxFU,11276
 nvflare/private/fed/client/__init__.py,sha256=aOvY5ivRRWvC9ooCZ3os_-mcmOcL2fBzr6sBD8AqtC0,653
-nvflare/private/fed/client/admin.py,sha256=RQB1U5pJP0YKWVdFHQulNy13Zs6wm8AsCS6v2FxqLlc,6169
+nvflare/private/fed/client/admin.py,sha256=D5dHmBOfJBUOP8vDVOkqApd_RwL1q5Y2yvVI1qhcptk,6173
 nvflare/private/fed/client/admin_commands.py,sha256=gFVFkZgwFYCW0tLpEMexsTtkgUR7ruaVchpxsjqD8Zk,7851
 nvflare/private/fed/client/client_app_runner.py,sha256=EqyCdRwcncl6ogVT1dCN34CR2La5A05xNTirNlVCiRE,5521
-nvflare/private/fed/client/client_engine.py,sha256=cZn9djmdX53AmKnwEpAQFrcYXg1ob_bg7PP7HTf800s,9741
+nvflare/private/fed/client/client_engine.py,sha256=txpuTG2lOr9JP0yIOv6Bz5ndJs82knZ-zV57lyHEwtQ,10272
 nvflare/private/fed/client/client_engine_executor_spec.py,sha256=0UH5PY0von6mnx2hF08CxfMpgjPdKzByiT2eauwhkss,4618
 nvflare/private/fed/client/client_engine_internal_spec.py,sha256=Ergz6ikbIDYYZqR44xxj5WhHlmB3q6iMa36qd6t1MW4,3194
 nvflare/private/fed/client/client_executor.py,sha256=_vMRWKk_6EuPTr4G8xsMPPYVHjcKJJqRVBCOLCrYFF0,15638
 nvflare/private/fed/client/client_json_config.py,sha256=UEawC0rT2JYFjaT9lXrLDvaskNV9gBNIQ_48hjaAQ-M,5410
 nvflare/private/fed/client/client_req_processors.py,sha256=MWPzO8-2BZ2-fkAQ193qBbXD4rGPKRyxYGZgAZULSWs,2195
 nvflare/private/fed/client/client_run_manager.py,sha256=2VCUwfGDneSUWbzjEWXxcbhQrOUb3MM2JN0zo5PTA10,9812
-nvflare/private/fed/client/client_runner.py,sha256=EYca9_yx1KI4RNT6U3BAFSbxwjDbq87pU3PAdZx7tJQ,26410
+nvflare/private/fed/client/client_runner.py,sha256=dgXVjXtygmW0t-o_nOwb48pNfq7QWpnYNCSJx3Y_KB8,26526
 nvflare/private/fed/client/client_status.py,sha256=SeaEH2WzT5Bcw-WWSHGCn6Rh0Ag9G7w5pvRyhZzaB8M,998
 nvflare/private/fed/client/command_agent.py,sha256=seLKkjw8KyYlRt3Y30lVldMi5-JkO6XsYmHona0jjUU,3982
-nvflare/private/fed/client/communicator.py,sha256=9DNyDky34_kD3cGQBkVFsGuMxkjEXVAmv1KJRq_QQzg,14499
+nvflare/private/fed/client/communicator.py,sha256=WUWUOMC4AtqwOt4pATcOPbH2jBHkTU_gE3NDYYkHBV0,14529
 nvflare/private/fed/client/comp_caller_cmd.py,sha256=oSavsxgn55tS5-FkJsTm344JeNVJzD8BD8QCmi3BiYU,2138
 nvflare/private/fed/client/fed_client.py,sha256=H2ZshTccZiGwVNSqkTyP4uNAzKtejHCDA-ACXQSjzbQ,3997
 nvflare/private/fed/client/fed_client_base.py,sha256=iVor4q9YVJg8ZKqdnGKNRVwpsx7TQaozJb9NMZ7Zsdk,16151
 nvflare/private/fed/client/info_coll_cmd.py,sha256=AyC2wUBUliHC4OYYYKMoP55b1gXUY5IRo266-tIicH8,2040
-nvflare/private/fed/client/scheduler_cmds.py,sha256=gKsR3gp6OQuvqUVXxqFQoUz0vT_fxsGhOcEXQIz442s,7031
+nvflare/private/fed/client/scheduler_cmds.py,sha256=tAwpehWMWo23tkkTBCpCVZHM1jEUshILbJd4ODh5HEk,7035
 nvflare/private/fed/client/shell_cmd.py,sha256=RtomOF6T_5s5YwtpcK_eD9slhW0Gd3z5TryTSBER9io,1139
 nvflare/private/fed/client/sys_cmd.py,sha256=MXpWQBdvm7QVQrqaOdML59ql5U3Uq4iIgrAox20dOfg,1974
-nvflare/private/fed/client/training_cmds.py,sha256=96ufWSb4VAW5y32RLnuuUHh_RdUdwrvbiHqy2pQYeCo,7186
+nvflare/private/fed/client/training_cmds.py,sha256=8XuHU2VroyQ_o02l8DhojaIkqqzNZ-puoTomDMPnbZs,7322
 nvflare/private/fed/server/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/private/fed/server/admin.py,sha256=cyB6K2GG3UdisvWgC59RB6R3ahevwTPxf55lZPbk6WA,10174
 nvflare/private/fed/server/client_manager.py,sha256=gVxAEKINafZ60EMqDCdlT3Ky1GprFmMVl5inf3vNKfM,9880
-nvflare/private/fed/server/cmd_utils.py,sha256=1fDaYoSac28Q-z01ljpUksUAQZAlLvHZBpWqh0fPOwc,8087
-nvflare/private/fed/server/fed_server.py,sha256=GFVPmRM1vXgU9Vise3X0qY2sVfUClbc9DATh2jDxf24,31837
-nvflare/private/fed/server/info_coll_cmd.py,sha256=BmTmpfb5SvqRNRZgaKrX7Sm7zv0wLYfHXhS6NDN8r8s,7383
-nvflare/private/fed/server/job_cmds.py,sha256=ITplmXZwCkNHDoKoLBHBhl7TbQ1Rhqak85Wd5s8GLqM,30237
-nvflare/private/fed/server/job_meta_validator.py,sha256=6ZNryVhqo3SOG3djpPuUyjB20q2nRVnLKompKSxC2oU,8025
-nvflare/private/fed/server/job_runner.py,sha256=iM5I8W7IbuaCj78fBmHcBHrqsJMiuKfIloOnxJIzl5A,25377
-nvflare/private/fed/server/message_send.py,sha256=nghk2u0Puno0jUV4OBfLnOF-Vztea2JBi4t8jNX6xU8,3512
+nvflare/private/fed/server/cmd_utils.py,sha256=xWt9c_jDgz4zmFityo2rKwapcnWuKP_D_SzGnaoHa6Y,8479
+nvflare/private/fed/server/fed_server.py,sha256=FX4T3WN7nSXWRTqnTrnBnydu47-lkHPeGkrWCVAsyso,32128
+nvflare/private/fed/server/info_coll_cmd.py,sha256=zbT-KAgOI7naNo6DIZgEcRnHbM8bH-VZG-EyCNhr1Es,6671
+nvflare/private/fed/server/job_cmds.py,sha256=i7ZxaCaJVwGiB6K_3O7xb8KwlICR8hu0UwxFd6L7hcg,30474
+nvflare/private/fed/server/job_meta_validator.py,sha256=peKb70C1kx7kLTtUtK3pt6jD4tZuP6KlYOjgULrEYkc,8117
+nvflare/private/fed/server/job_runner.py,sha256=SgVdsLQK4ph4nMMkWRU2PSrEQAPK4QJ4V_SbmLfFoQ4,26711
+nvflare/private/fed/server/message_send.py,sha256=S70nn-lyUo81JUg50ArivRnNQA9vgFtu7qlyUTmyzSE,3705
 nvflare/private/fed/server/run_info.py,sha256=l2d8ehm6RVXsgelWsBE60tX-LB1JUKHhrR_RF6yV6fM,929
 nvflare/private/fed/server/run_manager.py,sha256=4Kwx66QQAqqcNQknPhP8Z7w4vqI51viWFiIIFQv-mzI,3870
-nvflare/private/fed/server/server_app_runner.py,sha256=k3aOAKokiRqI_Tx5ovAGKcBsswxFl_j3rwJ802L2d7s,3456
+nvflare/private/fed/server/server_app_runner.py,sha256=6ooctJke3f6RXm2dQobqpN9TauOtzZfGGX2sRk5_St0,3460
 nvflare/private/fed/server/server_cmd_modules.py,sha256=p9jWZyEwFYlzqtUlAwnwyUmDQ3kmUMss45aeki5Iuvo,1364
 nvflare/private/fed/server/server_command_agent.py,sha256=QVpVK2tg908dIVbpNqqWtSK5g9FlhP_-DMAg874BwjA,5546
 nvflare/private/fed/server/server_commands.py,sha256=gH3fy_1IPf8EnxK8IPEX0PUxLLi8J06wfsiR3f_-zIw,13913
-nvflare/private/fed/server/server_engine.py,sha256=gDlud7LGsh_q_od-gURPChk_neIH_Mpt0Kd16PWiLHk,32016
+nvflare/private/fed/server/server_engine.py,sha256=a1vfUL4od4P6fAwDxKbD-eqoknFzArIJGov2f4a_nEw,32006
 nvflare/private/fed/server/server_engine_internal_spec.py,sha256=aViv5MoTXrhDu8YOCiXwO1PgvjQYDfbwWsDEQT-Z4uk,7240
 nvflare/private/fed/server/server_json_config.py,sha256=BdpOyNhYjmskxeLrO9FBRGR5_ZXsLpR7VU-9H2ZV0dw,6163
-nvflare/private/fed/server/server_runner.py,sha256=MhbWL-Jn5-djg2pdXmtqJdtCt84emO01F-9mfLZnJns,22528
+nvflare/private/fed/server/server_runner.py,sha256=VK5Gq-UKZ67wBDrObhllYcHwwsAJgFD2yZv122Y_i_o,22561
 nvflare/private/fed/server/server_state.py,sha256=JBbpjWuxpkfDJlMOwL3K9tLcICXMwxLpgrp_SG2ecTY,6711
 nvflare/private/fed/server/server_status.py,sha256=Lym5BmU0-V9rmu9CZgRy9yizsJwj11qH2qkmaLQnwyA,1049
-nvflare/private/fed/server/shell_cmd.py,sha256=0LHPQVb29WjF8z6ZCqaPoO9OMdwVr41Rx-e8xIddnbA,10418
-nvflare/private/fed/server/sys_cmd.py,sha256=xGLs8aG9lVlhcfffXk6Nw7qALNd3xMmMiRL2JfKNH0w,6119
-nvflare/private/fed/server/training_cmds.py,sha256=SOhYKLf72nzVY_AHRLKCWhWrfk069jbm88m0HJon6fM,16962
+nvflare/private/fed/server/shell_cmd.py,sha256=IQCy5D4bgNV4NduISthWugHcXCqJk8bxLM7k-A-zxpc,10824
+nvflare/private/fed/server/sys_cmd.py,sha256=HvkafjokzOfCiml3JXkOqup5aANd0wNlOsApXUQmVHg,5999
+nvflare/private/fed/server/training_cmds.py,sha256=sMvtPWIhLkEorrdxMTXRTSA_pFxDviwa4ZLcLIyXj50,17529
 nvflare/private/fed/simulator/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/private/fed/simulator/simulator_app_runner.py,sha256=HYbwcMLWBXxi1w_nojGWBMDxEZQ4CobdpBsNgT9R2QU,1884
 nvflare/private/fed/simulator/simulator_audit.py,sha256=lOGcwmugbgESzZ2utyxQV2aMs4DBECDiuHj4KOBef2k,1030
 nvflare/private/fed/simulator/simulator_client_engine.py,sha256=v66S0PwOUMMMOa7uLxuaxd3DrjgiS0Nz_xm6Fqt1kpA,1724
 nvflare/private/fed/simulator/simulator_const.py,sha256=WXBcFNli5_dKTfwwulJ2h-O9ZH3GNYoIzcS17_lOzBs,787
-nvflare/private/fed/simulator/simulator_server.py,sha256=74USIWNq_eNS5uVVsm_9JpBBLxkUvxz3PDydZSz3-BA,5275
+nvflare/private/fed/simulator/simulator_server.py,sha256=eAs7XJyw6PH_-6YzfB9sqFIfp51c0BufxRBKKd6-3b8,5279
 nvflare/private/fed/utils/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/private/fed/utils/app_authz.py,sha256=ZzATh0WdAVRNuU0RBE74rU3Lld5p4foLRoEmFwapB-Y,2019
-nvflare/private/fed/utils/app_deployer.py,sha256=DtIo-GCBiL-7y93tBNl1i-wW99aaPv5-tWxYXCA_AZM,3038
-nvflare/private/fed/utils/fed_utils.py,sha256=wg8WfLykKOhOxEmmdaBjlBUXqsChl3IjrBsRTTUu51g,8154
+nvflare/private/fed/utils/app_deployer.py,sha256=Idp5Zu6iIb6s1qK0Tq-CYak0eftlsEUdi3MdTjTDQNw,2938
+nvflare/private/fed/utils/fed_utils.py,sha256=r0JUlsEQy6vr6hMNdvduauAhjbCsa6Vx1jyAvgJmH7o,10386
 nvflare/private/fed/utils/decomposers/__init__.py,sha256=fAL6CiF1_taAoRVsurzSXhlfywLzVsXZOkEEtyBOfBQ,610
 nvflare/private/fed/utils/decomposers/private_decomposers.py,sha256=wDzTYTHXTxzw3ERfjNpoKdnLenRXSGhdN_HEBuh6Wns,1293
 nvflare/security/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
-nvflare/security/logging.py,sha256=KV5V9P14-TE-ShmjxKVDE8hlIOIOogz2mG8uiaR5Zxo,4133
+nvflare/security/logging.py,sha256=RyCbqv3n-WD62fQa8vf6WagJVU9LBU7w4WVxxL1wDBM,4112
 nvflare/security/security.py,sha256=KY6NqicqBPCCc-fEywGVCVTx89UYXXouhzTQHjkOeLM,2875
 nvflare/tool/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
-nvflare/tool/api_utils.py,sha256=6G_l6293k1tb7Ual9fOU9k6vu5kLDOz6IQVmqHATw-0,4429
+nvflare/tool/api_utils.py,sha256=BK_m8DykSJbVWk8IFo-WKpoOPCc7f6ErTlTkLY3DByc,4432
 nvflare/tool/preflight_check.py,sha256=8c3EQPnbyYFmYIX8a-PPGmSzt27HwSHprVFWGZzsp_k,2001
 nvflare/tool/package_checker/__init__.py,sha256=WlHC9C8kNF8M_cWObPeoGZue0nQbu7ZI0Q4CJlex0M0,904
 nvflare/tool/package_checker/check_rule.py,sha256=XNYskatnqmFzEsAbNOUCL_vVEPj94e8l7EMtfLvxwqA,9553
 nvflare/tool/package_checker/client_package_checker.py,sha256=haqw8Kb4EylUol1X_Ux4Ek_bKS4sRZ7m4zMSeAhFaEA,2510
 nvflare/tool/package_checker/nvflare_console_package_checker.py,sha256=8psm0FgBb5FXN7qVDvsLiwi0BWgRUwrWVvVptTEXl40,1075
 nvflare/tool/package_checker/overseer_package_checker.py,sha256=f1feRWwqRuCF8WlglKxaqMNF-zQkfvE7VXvQuo4yW6Y,1990
 nvflare/tool/package_checker/package_checker.py,sha256=KJR7IYG382figoNWX6lGteLimUoFScmPapncPAZmHCw,7550
 nvflare/tool/package_checker/server_package_checker.py,sha256=TuXlxmJKrtQvG5jROCtAOQFJY3JnzU2_vW5wPNuZyBM,4477
 nvflare/tool/package_checker/utils.py,sha256=VZL0qhD5cilFGtemEFPCZmBjakC4Iv73USIhXb_FDZs,8198
 nvflare/utils/__init__.py,sha256=Vgd9K3Anjug55M43V_v8tfW_cPxXYnaOYBJ66gyaQiQ,610
 nvflare/utils/decorators.py,sha256=6LTJLWN0yHEuDuQIlYjTsIpOHTKYDmOAt0Dl9YsnyAY,1452
 nvflare/widgets/__init__.py,sha256=TS5NMVLZXlTIgbt7grYmlxBfRKrWELPnT9DedX9kYBk,610
 nvflare/widgets/comp_caller.py,sha256=z1ZY74Vu-KnQKk3DPwf3axYGYXxGkGxjZWDtE7vataU,3921
-nvflare/widgets/fed_event.py,sha256=ksJ1FP8zhFEVVEmhXlR0AfnRcS14Uff9R7VN9Xm6W_A,9057
-nvflare/widgets/info_collector.py,sha256=LEre3Fok-PuODXCGmCTwZ2yyN0tWDrvddv7LELl_Sy8,8939
+nvflare/widgets/fed_event.py,sha256=3FcozUvtSOu7ZnYVF2i5H4LXPO0UnYIgJSYqD366LPk,9061
+nvflare/widgets/info_collector.py,sha256=D0wsymMyV8JcB7PEHpu15kzT2pGZazrzzAVZgep2-mk,8996
 nvflare/widgets/widget.py,sha256=MoLU9_vq1Ul26imdhKxPZYSCgt4Ed-D4xYV2BC5FfDQ,1365
-nvflare-2.3.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-nvflare-2.3.1.dist-info/METADATA,sha256=ry37jtw4gstnVlz3r1UV7RNWtk4YNxaCXILOeyF0Prk,6277
-nvflare-2.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-nvflare-2.3.1.dist-info/entry_points.txt,sha256=oep5Z6gAxvgAnJeSTjWNWQVJ95D0Ac4Sqq_CzIYSWVc,45
-nvflare-2.3.1.dist-info/top_level.txt,sha256=4NFDcbLXVTr75MZ1JIoaNjXzlnmQwXkquDEZq53zcRg,8
-nvflare-2.3.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nvflare-2.3.1.dist-info/RECORD,,
+nvflare-2.4.0rc1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+nvflare-2.4.0rc1.dist-info/METADATA,sha256=BqYMKaqXuONRzvw3MBNlZI4ZhqpS58YkClGCVHIk-5Y,6761
+nvflare-2.4.0rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+nvflare-2.4.0rc1.dist-info/entry_points.txt,sha256=oep5Z6gAxvgAnJeSTjWNWQVJ95D0Ac4Sqq_CzIYSWVc,45
+nvflare-2.4.0rc1.dist-info/top_level.txt,sha256=4NFDcbLXVTr75MZ1JIoaNjXzlnmQwXkquDEZq53zcRg,8
+nvflare-2.4.0rc1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nvflare-2.4.0rc1.dist-info/RECORD,,
```

