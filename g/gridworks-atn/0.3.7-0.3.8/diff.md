# Comparing `tmp/gridworks_atn-0.3.7.tar.gz` & `tmp/gridworks_atn-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_atn-0.3.7.tar", max compression
+gzip compressed data, was "gridworks_atn-0.3.8.tar", max compression
```

## Comparing `gridworks_atn-0.3.7.tar` & `gridworks_atn-0.3.8.tar`

### file list

```diff
@@ -1,228 +1,243 @@
--rw-r--r--   0        0        0     1065 2023-06-05 22:56:56.785578 gridworks_atn-0.3.7/LICENSE
--rw-r--r--   0        0        0     3002 2023-06-05 22:56:56.785578 gridworks_atn-0.3.7/README.md
--rw-r--r--   0        0        0     2193 2023-06-05 22:57:11.781770 gridworks_atn-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      681 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/__init__.py
--rw-r--r--   0        0        0      226 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/__main__.py
--rw-r--r--   0        0        0    13411 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/api_types.py
--rw-r--r--   0        0        0    24496 2023-06-05 22:57:11.781770 gridworks_atn-0.3.7/src/gwatn/atn_actor_base.py
--rw-r--r--   0        0        0     3114 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/atn_utils.py
--rw-r--r--   0        0        0    19983 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/atn.py
--rw-r--r--   0        0        0       98 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/dev_atn_params_data.csv
--rw-r--r--   0        0        0     7337 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/dev_io.py
--rw-r--r--   0        0        0      867 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/edge.py
--rw-r--r--   0        0        0     7536 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/flo.py
--rw-r--r--   0        0        0    18355 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/flo_output.py
--rw-r--r--   0        0        0     1508 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/make_dev_input_data.py
--rw-r--r--   0        0        0      841 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/node.py
--rw-r--r--   0        0        0     6963 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/simple_scada_sim.py
--rw-r--r--   0        0        0     2671 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/strategy_utils.py
--rw-r--r--   0        0        0     4575 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/config.py
--rw-r--r--   0        0        0       43 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/conversion_factors.py
--rw-r--r--   0        0        0     6148 2023-06-05 22:56:56.793578 gridworks_atn-0.3.7/src/gwatn/data_classes/.DS_Store
--rw-r--r--   0        0        0      935 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/__init__.py
--rw-r--r--   0        0        0      577 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/d_edge.py
--rw-r--r--   0        0        0     7812 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/d_graph.py
--rw-r--r--   0        0        0     1508 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/d_node.py
--rw-r--r--   0        0        0     8684 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/hack_price_method.py
--rw-r--r--   0        0        0     4082 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/hack_weather_location.py
--rw-r--r--   0        0        0     2104 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/data_classes/hack_weather_source.py
--rw-r--r--   0        0        0    14466 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/demo_methods.py
--rw-r--r--   0        0        0      276 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dev_utils/__init__.py
--rw-r--r--   0        0        0     1792 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_discoverer.py
--rw-r--r--   0        0        0    11883 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_ta_owner.py
--rw-r--r--   0        0        0    10994 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_validator.py
--rw-r--r--   0        0        0     1171 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dev_utils/make_plants.py
--rw-r--r--   0        0        0    11409 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dispatch_contract.py
--rw-r--r--   0        0        0    12463 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/application.json
--rw-r--r--   0        0        0     5229 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/approval.teal
--rw-r--r--   0        0        0       40 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/clear.teal
--rw-r--r--   0        0        0     3937 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/contract.json
--rw-r--r--   0        0        0     2402 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/__init__.py
--rw-r--r--   0        0        0      700 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/distribution_tariff.py
--rw-r--r--   0        0        0      614 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/energy_supply_type.py
--rw-r--r--   0        0        0     1308 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/hack_price_method.py
--rw-r--r--   0        0        0      415 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/hack_recognized_p_node_alias.py
--rw-r--r--   0        0        0      590 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/hack_weather_method.py
--rw-r--r--   0        0        0      132 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/hack_weather_source.py
--rw-r--r--   0        0        0      947 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/recognized_irradiance_type.py
--rw-r--r--   0        0        0      570 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/enums/recognized_temperature_unit.py
--rw-r--r--   0        0        0      122 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/errors.py
--rw-r--r--   0        0        0        0 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/py.typed
--rw-r--r--   0        0        0     7945 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/python_ta_daemon.json
--rw-r--r--   0        0        0    12518 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/python_ta_daemon.py
--rw-r--r--   0        0        0      834 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/scada_codec.py
--rw-r--r--   0        0        0     3523 2023-06-05 22:57:11.781770 gridworks_atn-0.3.7/src/gwatn/simple_atn_actor.py
--rw-r--r--   0        0        0    26139 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/simple_scada_sim_actor_base.py
--rw-r--r--   0        0        0     3169 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/ta_daemon_rest_api.py
--rw-r--r--   0        0        0      460 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/ta_validator_rest_api.py
--rw-r--r--   0        0        0    47761 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/two_channel_actor_base.py
--rw-r--r--   0        0        0    13145 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/__init__.py
--rw-r--r--   0        0        0     7868 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/accepted_bid.py
--rw-r--r--   0        0        0    20222 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/atn_bid.py
--rw-r--r--   0        0        0     4288 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/atn_params.py
--rw-r--r--   0        0        0    22335 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/atn_params_brickstorageheater.py
--rw-r--r--   0        0        0     8144 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/atn_params_report.py
--rw-r--r--   0        0        0     8321 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/basegnode_scada_create.py
--rw-r--r--   0        0        0     1067 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/data_channel.py
--rw-r--r--   0        0        0     9885 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/discoverycert_algo_create.py
--rw-r--r--   0        0        0     8092 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/dispatch_contract_confirmed.py
--rw-r--r--   0        0        0     3235 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0.py
--rw-r--r--   0        0        0      555 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3959 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3338 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py
--rw-r--r--   0        0        0      555 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3959 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3658 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0     1690 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     4905 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7648 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/flo_params.py
--rw-r--r--   0        0        0    22826 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/flo_params_brickstorageheater.py
--rw-r--r--   0        0        0     8827 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/flo_params_report.py
--rw-r--r--   0        0        0     3885 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py
--rw-r--r--   0        0        0      600 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4184 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5457 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py
--rw-r--r--   0        0        0      620 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0     7905 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5419 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0      625 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7913 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5176 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py
--rw-r--r--   0        0        0      649 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py
--rw-r--r--   0        0        0     8053 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3885 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py
--rw-r--r--   0        0        0      593 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4203 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5392 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py
--rw-r--r--   0        0        0      613 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0     7891 2023-06-05 22:56:56.797578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3909 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py
--rw-r--r--   0        0        0      609 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4212 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7507 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py
--rw-r--r--   0        0        0     1453 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py
--rw-r--r--   0        0        0    12856 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7530 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py
--rw-r--r--   0        0        0     1453 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0    11873 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3980 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py
--rw-r--r--   0        0        0      611 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4060 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4083 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py
--rw-r--r--   0        0        0      627 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4430 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3879 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py
--rw-r--r--   0        0        0      595 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4196 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5398 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py
--rw-r--r--   0        0        0      615 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0     7901 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     8206 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0    14769 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/hack_property_format.py
--rw-r--r--   0        0        0      194 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/hack_test_dummy.py
--rw-r--r--   0        0        0      781 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/hack_type_base.py
--rw-r--r--   0        0        0      990 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/hack_utils.py
--rw-r--r--   0        0        0     9155 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/heartbeat_b.py
--rw-r--r--   0        0        0     6154 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_create.py
--rw-r--r--   0        0        0     7610 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_optin.py
--rw-r--r--   0        0        0     8932 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_transfer.py
--rw-r--r--   0        0        0     7959 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/join_dispatch_contract.py
--rw-r--r--   0        0        0    12429 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/latest_price.py
--rw-r--r--   0        0        0     5028 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/market_slot.py
--rw-r--r--   0        0        0    17161 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/market_type_gt.py
--rw-r--r--   0        0        0     5294 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/new_tadeed_algo_optin.py
--rw-r--r--   0        0        0     5196 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/new_tadeed_send.py
--rw-r--r--   0        0        0     5024 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/old_tadeed_algo_return.py
--rw-r--r--   0        0        0     8461 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/price_quantity.py
--rw-r--r--   0        0        0     2492 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/price_quantity_unitless.py
--rw-r--r--   0        0        0    13837 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py
--rw-r--r--   0        0        0    13162 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py
--rw-r--r--   0        0        0    14105 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py
--rw-r--r--   0        0        0     5624 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py
--rw-r--r--   0        0        0      558 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py
--rw-r--r--   0        0        0     8026 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5026 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py
--rw-r--r--   0        0        0      594 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py
--rw-r--r--   0        0        0     7236 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5890 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py
--rw-r--r--   0        0        0      578 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7750 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7618 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py
--rw-r--r--   0        0        0    13827 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py
--rw-r--r--   0        0        0     7319 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py
--rw-r--r--   0        0        0    12667 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py
--rw-r--r--   0        0        0     8872 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0    10345 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py
--rw-r--r--   0        0        0    14435 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py
--rw-r--r--   0        0        0     4044 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py
--rw-r--r--   0        0        0      589 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3804 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5402 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py
--rw-r--r--   0        0        0      561 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py
--rw-r--r--   0        0        0     7263 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4044 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py
--rw-r--r--   0        0        0      589 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3804 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5661 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py
--rw-r--r--   0        0        0      597 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py
--rw-r--r--   0        0        0     7829 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3535 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py
--rw-r--r--   0        0        0      653 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py
--rw-r--r--   0        0        0     3064 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4184 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0      586 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     3863 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5892 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py
--rw-r--r--   0        0        0      581 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7746 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3707 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py
--rw-r--r--   0        0        0      581 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py
--rw-r--r--   0        0        0     3547 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py
--rw-r--r--   0        0        0    13926 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py
--rw-r--r--   0        0        0    14182 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py
--rw-r--r--   0        0        0     5617 2023-06-05 22:56:56.801578 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py
--rw-r--r--   0        0        0      544 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py
--rw-r--r--   0        0        0     8022 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5864 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py
--rw-r--r--   0        0        0      573 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7746 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5004 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/scada_cert_transfer.py
--rw-r--r--   0        0        0     3682 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_data.py
--rw-r--r--   0        0        0     4166 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_data_bsh.py
--rw-r--r--   0        0        0     6534 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_report.py
--rw-r--r--   0        0        0     6774 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/simplesim_snapshot_brickstorageheater.py
--rw-r--r--   0        0        0     3220 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/sla_enter.py
--rw-r--r--   0        0        0     4101 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/tadeed_specs_hack.py
--rw-r--r--   0        0        0     5734 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/tavalidatorcert_algo_create.py
--rw-r--r--   0        0        0     6371 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/tavalidatorcert_algo_transfer.py
--rw-r--r--   0        0        0     5242 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/terminalasset_certify_hack.py
--rw-r--r--   0        0        0    30475 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py
--rw-r--r--   0        0        0    29247 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0     8474 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py
--rw-r--r--   0        0        0     1920 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py
--rw-r--r--   0        0        0    13416 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3535 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py
--rw-r--r--   0        0        0      686 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py
--rw-r--r--   0        0        0     3076 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7834 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py
--rw-r--r--   0        0        0      829 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py
--rw-r--r--   0        0        0    12801 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py
--rw-r--r--   0        0        0     8628 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0     1153 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0    12807 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3671 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py
--rw-r--r--   0        0        0      572 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py
--rw-r--r--   0        0        0     3547 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py
--rw-r--r--   0        0        0    14909 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py
--rw-r--r--   0        0        0    11616 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py
--rw-r--r--   0        0        0     4544 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py
--rw-r--r--   0        0        0      631 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py
--rw-r--r--   0        0        0     6001 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py
--rw-r--r--   0        0        0    12321 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py
--rw-r--r--   0        0        0     6939 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py
--rw-r--r--   0        0        0      642 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py
--rw-r--r--   0        0        0    10751 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4677 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py
--rw-r--r--   0        0        0      610 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py
--rw-r--r--   0        0        0     6741 2023-06-05 22:56:56.805579 gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 gridworks_atn-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-27 19:18:29.214349 gridworks_atn-0.3.8/LICENSE
+-rw-r--r--   0        0        0     3002 2023-06-27 19:18:29.218349 gridworks_atn-0.3.8/README.md
+-rw-r--r--   0        0        0     2157 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      681 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/__init__.py
+-rw-r--r--   0        0        0      226 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/__main__.py
+-rw-r--r--   0        0        0    13844 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/api_types.py
+-rw-r--r--   0        0        0    23400 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/atn_actor_base.py
+-rw-r--r--   0        0        0     3538 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/atn_utils.py
+-rw-r--r--   0        0        0     4521 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/config.py
+-rw-r--r--   0        0        0       43 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/conversion_factors.py
+-rw-r--r--   0        0        0     6148 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/.DS_Store
+-rw-r--r--   0        0        0      935 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/d_edge.py
+-rw-r--r--   0        0        0     7812 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/d_graph.py
+-rw-r--r--   0        0        0     1508 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/d_node.py
+-rw-r--r--   0        0        0     8684 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/hack_price_method.py
+-rw-r--r--   0        0        0     4082 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/hack_weather_location.py
+-rw-r--r--   0        0        0     2104 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/hack_weather_source.py
+-rw-r--r--   0        0        0    14466 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/demo_methods.py
+-rw-r--r--   0        0        0      276 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dev_utils/__init__.py
+-rw-r--r--   0        0        0     1792 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_discoverer.py
+-rw-r--r--   0        0        0    11883 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_ta_owner.py
+-rw-r--r--   0        0        0    10994 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_validator.py
+-rw-r--r--   0        0        0     1171 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dev_utils/make_plants.py
+-rw-r--r--   0        0        0    11409 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dispatch_contract.py
+-rw-r--r--   0        0        0    12463 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/application.json
+-rw-r--r--   0        0        0     5229 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/approval.teal
+-rw-r--r--   0        0        0       40 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/clear.teal
+-rw-r--r--   0        0        0     3937 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/contract.json
+-rw-r--r--   0        0        0     2069 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/enums/__init__.py
+-rw-r--r--   0        0        0     2677 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/enums/distribution_tariff.py
+-rw-r--r--   0        0        0      614 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/enums/energy_supply_type.py
+-rw-r--r--   0        0        0     1308 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/enums/hack_price_method.py
+-rw-r--r--   0        0        0      415 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/enums/hack_recognized_p_node_alias.py
+-rw-r--r--   0        0        0      590 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/enums/hack_weather_method.py
+-rw-r--r--   0        0        0      132 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/enums/hack_weather_source.py
+-rw-r--r--   0        0        0      947 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/enums/recognized_irradiance_type.py
+-rw-r--r--   0        0        0      570 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/enums/recognized_temperature_unit.py
+-rw-r--r--   0        0        0      122 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/errors.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/py.typed
+-rw-r--r--   0        0        0     7945 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/python_ta_daemon.json
+-rw-r--r--   0        0        0    12518 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/python_ta_daemon.py
+-rw-r--r--   0        0        0      834 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/scada_codec.py
+-rw-r--r--   0        0        0     3677 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/simple_atn_actor.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/__init__.py
+-rw-r--r--   0        0        0    20114 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/atn.py
+-rw-r--r--   0        0        0       98 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/dev_atn_params_data.csv
+-rw-r--r--   0        0        0     7337 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/dev_io.py
+-rw-r--r--   0        0        0      867 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/edge.py
+-rw-r--r--   0        0        0     7536 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/flo.py
+-rw-r--r--   0        0        0    18355 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/flo_output.py
+-rw-r--r--   0        0        0     1508 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/make_dev_input_data.py
+-rw-r--r--   0        0        0      841 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/node.py
+-rw-r--r--   0        0        0     2549 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/strategy_utils.py
+-rw-r--r--   0        0        0    20114 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/atn.py
+-rw-r--r--   0        0        0     8663 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/dev_io.py
+-rw-r--r--   0        0        0      867 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/edge.py
+-rw-r--r--   0        0        0     7536 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/flo.py
+-rw-r--r--   0        0        0    18355 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/flo_output.py
+-rw-r--r--   0        0        0     9363 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/flo_utils.py
+-rw-r--r--   0        0        0     1824 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/make_dev_input_data.py
+-rw-r--r--   0        0        0      841 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/node.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/output_data/__init__.py
+-rw-r--r--   0        0        0    26363 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/simple_scada_sim.py
+-rw-r--r--   0        0        0     3717 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/strategy_utils.py
+-rw-r--r--   0        0        0    11673 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/tea.py
+-rw-r--r--   0        0        0     3152 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/tea_config.py
+-rw-r--r--   0        0        0    21042 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/tea_output.py
+-rw-r--r--   0        0        0     3169 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/ta_daemon_rest_api.py
+-rw-r--r--   0        0        0      460 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/ta_validator_rest_api.py
+-rw-r--r--   0        0        0    51741 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/two_channel_actor_base.py
+-rw-r--r--   0        0        0    13733 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/__init__.py
+-rw-r--r--   0        0        0     7868 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/accepted_bid.py
+-rw-r--r--   0        0        0    20222 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/atn_bid.py
+-rw-r--r--   0        0        0     4288 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/atn_params.py
+-rw-r--r--   0        0        0    22525 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/atn_params_brickstorageheater.py
+-rw-r--r--   0        0        0     8144 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/atn_params_report.py
+-rw-r--r--   0        0        0    19280 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/atn_params_simpleresistivehydronic.py
+-rw-r--r--   0        0        0     8321 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/basegnode_scada_create.py
+-rw-r--r--   0        0        0     1067 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/data_channel.py
+-rw-r--r--   0        0        0     9885 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/discoverycert_algo_create.py
+-rw-r--r--   0        0        0     8092 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/dispatch_contract_confirmed.py
+-rw-r--r--   0        0        0     3235 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0      555 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3959 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3338 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0      555 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3959 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3658 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     1690 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     4905 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7648 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/flo_params.py
+-rw-r--r--   0        0        0    22633 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/flo_params_brickstorageheater.py
+-rw-r--r--   0        0        0     8827 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/flo_params_report.py
+-rw-r--r--   0        0        0    16757 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/flo_params_simpleresistivehydronic.py
+-rw-r--r--   0        0        0     3885 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py
+-rw-r--r--   0        0        0      600 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4184 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5457 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      620 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7905 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5419 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0      625 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7913 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5176 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py
+-rw-r--r--   0        0        0      649 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     8053 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3885 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py
+-rw-r--r--   0        0        0      593 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4203 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5392 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      613 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7891 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3909 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py
+-rw-r--r--   0        0        0      609 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4212 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7507 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py
+-rw-r--r--   0        0        0     1453 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py
+-rw-r--r--   0        0        0    12856 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7530 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py
+-rw-r--r--   0        0        0     1453 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0    11873 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3980 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py
+-rw-r--r--   0        0        0      611 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4060 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4083 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py
+-rw-r--r--   0        0        0      627 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4430 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3879 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py
+-rw-r--r--   0        0        0      595 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4196 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5398 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      615 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7901 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     8206 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0    14769 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/hack_property_format.py
+-rw-r--r--   0        0        0      194 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/hack_test_dummy.py
+-rw-r--r--   0        0        0      781 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/hack_type_base.py
+-rw-r--r--   0        0        0      990 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/hack_utils.py
+-rw-r--r--   0        0        0     9155 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/heartbeat_b.py
+-rw-r--r--   0        0        0     6154 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_create.py
+-rw-r--r--   0        0        0     7610 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     8932 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_transfer.py
+-rw-r--r--   0        0        0     7959 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/join_dispatch_contract.py
+-rw-r--r--   0        0        0    12429 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/latest_price.py
+-rw-r--r--   0        0        0     5028 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/market_slot.py
+-rw-r--r--   0        0        0    17161 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/market_type_gt.py
+-rw-r--r--   0        0        0     5294 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/new_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     5196 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/new_tadeed_send.py
+-rw-r--r--   0        0        0     5024 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/old_tadeed_algo_return.py
+-rw-r--r--   0        0        0     8461 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/price_quantity.py
+-rw-r--r--   0        0        0     2492 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/price_quantity_unitless.py
+-rw-r--r--   0        0        0    13837 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py
+-rw-r--r--   0        0        0    13162 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py
+-rw-r--r--   0        0        0    14105 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py
+-rw-r--r--   0        0        0     5624 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py
+-rw-r--r--   0        0        0      558 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py
+-rw-r--r--   0        0        0     8026 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5026 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py
+-rw-r--r--   0        0        0      594 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py
+-rw-r--r--   0        0        0     7236 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5890 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py
+-rw-r--r--   0        0        0      578 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7750 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7618 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0    13827 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py
+-rw-r--r--   0        0        0     7319 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0    12667 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py
+-rw-r--r--   0        0        0     8872 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0    10345 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py
+-rw-r--r--   0        0        0    14435 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py
+-rw-r--r--   0        0        0     4044 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0      589 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3804 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5402 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py
+-rw-r--r--   0        0        0      561 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py
+-rw-r--r--   0        0        0     7263 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4044 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0      589 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3804 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5661 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py
+-rw-r--r--   0        0        0      597 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py
+-rw-r--r--   0        0        0     7829 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3535 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py
+-rw-r--r--   0        0        0      653 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py
+-rw-r--r--   0        0        0     3064 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4184 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0      586 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     3863 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5892 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py
+-rw-r--r--   0        0        0      581 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7746 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3707 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py
+-rw-r--r--   0        0        0      581 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py
+-rw-r--r--   0        0        0     3547 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    13926 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py
+-rw-r--r--   0        0        0    14182 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py
+-rw-r--r--   0        0        0     5617 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py
+-rw-r--r--   0        0        0      544 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py
+-rw-r--r--   0        0        0     8022 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5864 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py
+-rw-r--r--   0        0        0      573 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7746 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5004 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/scada_cert_transfer.py
+-rw-r--r--   0        0        0     3682 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_data.py
+-rw-r--r--   0        0        0     4166 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_data_bsh.py
+-rw-r--r--   0        0        0     6534 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_report.py
+-rw-r--r--   0        0        0     6774 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/simplesim_snapshot_brickstorageheater.py
+-rw-r--r--   0        0        0     3220 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/sla_enter.py
+-rw-r--r--   0        0        0     4101 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/tadeed_specs_hack.py
+-rw-r--r--   0        0        0     5734 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/tavalidatorcert_algo_create.py
+-rw-r--r--   0        0        0     6371 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/tavalidatorcert_algo_transfer.py
+-rw-r--r--   0        0        0     5242 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/terminalasset_certify_hack.py
+-rw-r--r--   0        0        0    30475 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py
+-rw-r--r--   0        0        0    29247 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     8474 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py
+-rw-r--r--   0        0        0     1920 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py
+-rw-r--r--   0        0        0    13416 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3535 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py
+-rw-r--r--   0        0        0      686 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py
+-rw-r--r--   0        0        0     3076 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7834 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py
+-rw-r--r--   0        0        0      829 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py
+-rw-r--r--   0        0        0    12801 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     8628 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     1153 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0    12807 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3671 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py
+-rw-r--r--   0        0        0      572 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py
+-rw-r--r--   0        0        0     3547 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    14909 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py
+-rw-r--r--   0        0        0    11616 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py
+-rw-r--r--   0        0        0     4544 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py
+-rw-r--r--   0        0        0      631 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py
+-rw-r--r--   0        0        0     6001 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    12321 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py
+-rw-r--r--   0        0        0     6939 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py
+-rw-r--r--   0        0        0      642 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py
+-rw-r--r--   0        0        0    10751 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4677 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py
+-rw-r--r--   0        0        0      610 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py
+-rw-r--r--   0        0        0     6741 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 gridworks_atn-0.3.8/PKG-INFO
```

### Comparing `gridworks_atn-0.3.7/LICENSE` & `gridworks_atn-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/README.md` & `gridworks_atn-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/pyproject.toml` & `gridworks_atn-0.3.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "gridworks-atn"
-version = "0.3.7"
+version = "0.3.8"
 description = "Gridworks Atn Spaceheat"
-authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
+authors = ["GridWorks <gridworks@gridworks-consulting.com>"]
 license = "None"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-atn"
 repository = "https://github.com/thegridelectric/gridworks-atn"
 documentation = "https://gridworks-atn.readthedocs.io"
 packages = [
     { include = "gwatn", from = "src" },
@@ -16,21 +16,20 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/thegridelectric/gridworks-atn/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-gridworks = "^0.2.4"
-gridworks-protocol = "^0.5.2" # Note gridworks-protocol includes gridworks; these must stay in sync
-# gridworks-proactor = "^0.1.8"
 paho-mqtt = "^1.6.1"
-
-
 numpy = "^1.23.4"
+#gridworks-proactor = "0.2.2"
+#gridworks = { path = "../gridworks"}
+gridworks-proactor = "^0.2.2"
+gridworks-ps = "^0.0.1"
 
 
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/__init__.py` & `gridworks_atn-0.3.8/src/gwatn/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/api_types.py` & `gridworks_atn-0.3.8/src/gwatn/api_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 from typing import no_type_check
 
 from gwatn.types import AcceptedBid_Maker
 from gwatn.types import AtnBid_Maker
 from gwatn.types import AtnParams_Maker
 from gwatn.types import AtnParamsBrickstorageheater_Maker
 from gwatn.types import AtnParamsReport_Maker
+from gwatn.types import AtnParamsSimpleresistivehydronic_Maker
 from gwatn.types import BaseGNodeGt_Maker
 from gwatn.types import BasegnodeScadaCreate_Maker
 from gwatn.types import ComponentAttributeClassGt_Maker
 from gwatn.types import ComponentGt_Maker
 from gwatn.types import DataChannel_Maker
 from gwatn.types import DiscoverycertAlgoCreate_Maker
 from gwatn.types import DispatchContractConfirmed_Maker
 from gwatn.types import EgaugeIo_Maker
 from gwatn.types import EgaugeRegisterConfig_Maker
 from gwatn.types import ElectricMeterCacGt_Maker
 from gwatn.types import ElectricMeterComponentGt_Maker
 from gwatn.types import FloParams_Maker
 from gwatn.types import FloParamsBrickstorageheater_Maker
 from gwatn.types import FloParamsReport_Maker
+from gwatn.types import FloParamsSimpleresistivehydronic_Maker
 from gwatn.types import GNodeGt_Maker
 from gwatn.types import GNodeInstanceGt_Maker
 from gwatn.types import GtDispatchBoolean_Maker
 from gwatn.types import GtDispatchBooleanLocal_Maker
 from gwatn.types import GtDriverBooleanactuatorCmd_Maker
 from gwatn.types import GtShBooleanactuatorCmdStatus_Maker
 from gwatn.types import GtShCliAtnCmd_Maker
@@ -87,28 +89,30 @@
 def type_makers() -> List[HeartbeatA_Maker]:
     return [
         AcceptedBid_Maker,
         AtnBid_Maker,
         AtnParams_Maker,
         AtnParamsBrickstorageheater_Maker,
         AtnParamsReport_Maker,
+        AtnParamsSimpleresistivehydronic_Maker,
         BaseGNodeGt_Maker,
         BasegnodeScadaCreate_Maker,
         ComponentAttributeClassGt_Maker,
         ComponentGt_Maker,
         DataChannel_Maker,
         DiscoverycertAlgoCreate_Maker,
         DispatchContractConfirmed_Maker,
         EgaugeIo_Maker,
         EgaugeRegisterConfig_Maker,
         ElectricMeterCacGt_Maker,
         ElectricMeterComponentGt_Maker,
         FloParams_Maker,
         FloParamsBrickstorageheater_Maker,
         FloParamsReport_Maker,
+        FloParamsSimpleresistivehydronic_Maker,
         GNodeGt_Maker,
         GNodeInstanceGt_Maker,
         GtDispatchBoolean_Maker,
         GtDispatchBooleanLocal_Maker,
         GtDriverBooleanactuatorCmd_Maker,
         GtShBooleanactuatorCmdStatus_Maker,
         GtShCliAtnCmd_Maker,
@@ -176,28 +180,30 @@
 
     v: Dict[str, str] = {
         "accepted.bid": "000",
         "atn.bid": "001",
         "atn.params": "000",
         "atn.params.brickstorageheater": "000",
         "atn.params.report": "000",
+        "atn.params.simpleresistivehydronic": "000",
         "base.g.node.gt": "002",
         "basegnode.scada.create": "000",
         "component.attribute.class.gt": "000",
         "component.gt": "000",
         "data.channel": "000",
         "discoverycert.algo.create": "000",
         "dispatch.contract.confirmed": "000",
         "egauge.io": "000",
         "egauge.register.config": "000",
         "electric.meter.cac.gt": "000",
         "electric.meter.component.gt": "000",
         "flo.params": "000",
         "flo.params.brickstorageheater": "000",
         "flo.params.report": "000",
+        "flo.params.simpleresistivehydronic": "000",
         "g.node.gt": "002",
         "g.node.instance.gt": "000",
         "gt.dispatch.boolean": "110",
         "gt.dispatch.boolean.local": "110",
         "gt.driver.booleanactuator.cmd": "100",
         "gt.sh.booleanactuator.cmd.status": "100",
         "gt.sh.cli.atn.cmd": "110",
@@ -258,33 +264,35 @@
 def status_by_versioned_type_name() -> Dict[str, str]:
     """
     Returns:
         Dict[str, str]: Keys are versioned TypeNames, values are type status
     """
 
     v: Dict[str, str] = {
-        "accepted.bid.000": "Pending",
-        "atn.bid.001": "Pending",
+        "accepted.bid.000": "Active",
+        "atn.bid.001": "Active",
         "atn.params.000": "Active",
-        "atn.params.brickstorageheater.000": "Pending",
+        "atn.params.brickstorageheater.000": "Active",
         "atn.params.report.000": "Active",
+        "atn.params.simpleresistivehydronic.000": "Pending",
         "base.g.node.gt.002": "Active",
         "basegnode.scada.create.000": "Active",
         "component.attribute.class.gt.000": "Active",
         "component.gt.000": "Active",
         "data.channel.000": "Active",
         "discoverycert.algo.create.000": "Active",
         "dispatch.contract.confirmed.000": "Active",
         "egauge.io.000": "Active",
         "egauge.register.config.000": "Active",
         "electric.meter.cac.gt.000": "Active",
         "electric.meter.component.gt.000": "Active",
         "flo.params.000": "Active",
         "flo.params.brickstorageheater.000": "Active",
-        "flo.params.report.000": "Pending",
+        "flo.params.report.000": "Active",
+        "flo.params.simpleresistivehydronic.000": "Pending",
         "g.node.gt.002": "Active",
         "g.node.instance.gt.000": "Active",
         "gt.dispatch.boolean.110": "Active",
         "gt.dispatch.boolean.local.110": "Active",
         "gt.driver.booleanactuator.cmd.100": "Active",
         "gt.sh.booleanactuator.cmd.status.100": "Active",
         "gt.sh.cli.atn.cmd.110": "Active",
@@ -296,47 +304,47 @@
         "gw.cert.id.000": "Active",
         "heartbeat.a.100": "Active",
         "heartbeat.b.001": "Active",
         "initial.tadeed.algo.create.000": "Active",
         "initial.tadeed.algo.optin.002": "Active",
         "initial.tadeed.algo.transfer.000": "Active",
         "join.dispatch.contract.000": "Active",
-        "latest.price.000": "Pending",
-        "market.slot.000": "Pending",
-        "market.type.gt.000": "Pending",
+        "latest.price.000": "Active",
+        "market.slot.000": "Active",
+        "market.type.gt.000": "Active",
         "multipurpose.sensor.cac.gt.000": "Active",
         "multipurpose.sensor.component.gt.000": "Active",
         "new.tadeed.algo.optin.000": "Active",
         "new.tadeed.send.000": "Active",
         "old.tadeed.algo.return.000": "Active",
         "pipe.flow.sensor.cac.gt.000": "Active",
         "pipe.flow.sensor.component.gt.000": "Active",
         "power.watts.000": "Active",
-        "price.quantity.000": "Pending",
-        "price.quantity.unitless.000": "Pending",
+        "price.quantity.000": "Active",
+        "price.quantity.unitless.000": "Active",
         "ready.001": "Active",
         "relay.cac.gt.000": "Active",
         "relay.component.gt.000": "Active",
         "resistive.heater.cac.gt.000": "Active",
         "resistive.heater.component.gt.000": "Active",
-        "scada.cert.transfer.000": "Pending",
+        "scada.cert.transfer.000": "Active",
         "sim.timestep.000": "Active",
         "simple.temp.sensor.cac.gt.000": "Active",
         "simple.temp.sensor.component.gt.000": "Active",
-        "simplesim.driver.data.000": "Pending",
-        "simplesim.driver.data.bsh.000": "Pending",
-        "simplesim.driver.report.000": "Pending",
-        "simplesim.snapshot.brickstorageheater.000": "Pending",
-        "sla.enter.000": "Pending",
+        "simplesim.driver.data.000": "Active",
+        "simplesim.driver.data.bsh.000": "Active",
+        "simplesim.driver.report.000": "Active",
+        "simplesim.snapshot.brickstorageheater.000": "Active",
+        "sla.enter.000": "Active",
         "snapshot.spaceheat.000": "Active",
         "spaceheat.node.gt.100": "Active",
         "super.starter.000": "Active",
         "supervisor.container.gt.000": "Active",
-        "tadeed.specs.hack.000": "Pending",
+        "tadeed.specs.hack.000": "Active",
         "tavalidatorcert.algo.create.000": "Active",
         "tavalidatorcert.algo.transfer.000": "Active",
         "telemetry.reporting.config.000": "Active",
         "telemetry.snapshot.spaceheat.000": "Active",
-        "terminalasset.certify.hack.000": "Pending",
+        "terminalasset.certify.hack.000": "Active",
     }
 
     return v
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/atn_actor_base.py` & `gridworks_atn-0.3.8/src/gwatn/atn_actor_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 from gwatn.types import HeartbeatB_Maker
 from gwatn.types import JoinDispatchContract
 from gwatn.types import JoinDispatchContract_Maker
 from gwatn.types import LatestPrice
 from gwatn.types import LatestPrice_Maker
 from gwatn.types import PowerWatts
 from gwatn.types import SimTimestep
-from gwatn.types import SimTimestep_Maker
 from gwatn.types import SnapshotSpaceheat
 
 
 LOG_FORMAT = (
     "%(levelname) -10s %(sasctime)s %(name) -30s %(funcName) "
     "-35s %(lineno) -5d: %(message)s"
 )
@@ -81,47 +80,46 @@
         Version="000",
     )
 
 
 class AtnActorBase(TwoChannelActorBase):
     def __init__(self, settings: AtnSettings, use_algo: bool = False):
         super().__init__(settings=settings)
-        self.settings: AtnSettings = settings
         self.scada_gni_id = settings.scada_gni_id
         self._time: float = self.get_initial_time_s()
-
+        self.atn_params: AtnParams = dummy_atn_params()
+        self.dc_app_id: Optional[int] = None
+        self.dc_client: Optional[ApplicationClient] = None
+        self.trading_rights_id: Optional[GwCertId] = None
+        self.hb_status = HbStatus(LastHeartbeatReceivedMs=int(time.time() * 1000))
         if use_algo is True:
             self.acct: BasicAccount = BasicAccount(settings.sk.get_secret_value())
             self.client: AlgodClient = AlgodClient(
                 settings.algo_api_secrets.algod_token.get_secret_value(),
                 settings.public.algod_address,
             )
             if algo_utils.algos(self.acct.addr) < 5:
                 raise Exception(
                     f"Insufficiently funded. Make sure atn has at least 5 algos"
                 )
             # TODO: move this into spaceheat along with join_dispatch_contract_received
-            self.atn_params: AtnParams = dummy_atn_params()
+
             self.sp = self.client.suggested_params()
             self.sp.flat_fee = True
             self.sp.fee = 2000
             # this is initialized with the AppId provided by the SCADA
-            self.dc_app_id: Optional[int] = None
-            self.dc_client: Optional[ApplicationClient] = None
             self.check_for_dispatch_contract()
             self.universe_type = as_enum(
                 self.settings.universe_type_value, UniverseType, UniverseType.default()
             )
-            self.trading_rights_id: Optional[GwCertId] = None
             self.update_trading_rights()
-            self.hb_status = HbStatus(LastHeartbeatReceivedMs=int(time.time() * 1000))
 
     def local_rabbit_startup(self) -> None:
         rjb = MessageCategorySymbol.rjb.value
-        tc_alias_lrh = self.settings.time_coordinator_alias.replace(".", "-")
+        tc_alias_lrh = self.settings.my_time_coordinator_alias.replace(".", "-")
         binding = f"{rjb}.{tc_alias_lrh}.timecoordinator.sim-timestep"
 
         cb = functools.partial(self.on_timecoordinator_bindok, binding=binding)
         self._consume_channel.queue_bind(
             self.queue_name, "timecoordinatormic_tx", routing_key=binding, callback=cb
         )
         LOGGER.info(
@@ -255,24 +253,15 @@
         """Atn has received power.watts message from its SCADA"""
         raise NotImplementedError
 
     def route_message(
         self, from_alias: str, from_role: GNodeRole, payload: HeartbeatA
     ) -> None:
         self.payload = payload
-        if payload.TypeName == HeartbeatA_Maker.type_name:
-            if from_role != GNodeRole.Supervisor:
-                LOGGER.info(
-                    f"Ignoring HeartbeatA from GNode with role {from_role}; expects Supervisor"
-                )
-            try:
-                self.heartbeat_from_super(from_alias, payload)
-            except:
-                LOGGER.exception("Error in heartbeat_received")
-        elif payload.TypeName == HeartbeatB_Maker.type_name:
+        if payload.TypeName == HeartbeatB_Maker.type_name:
             if from_role != GNodeRole.Scada:
                 LOGGER.info(
                     f"Ignoring HeartbeatB from GNode with role {from_role}; expects Scada"
                 )
             try:
                 self.heartbeat_from_scada(payload)
             except:
@@ -288,34 +277,17 @@
                 LOGGER.exception("join_dispatch_contract_from_scada")
         elif payload.TypeName == LatestPrice_Maker.type_name:
             if from_role == GNodeRole.MarketMaker:
                 try:
                     self.latest_price_from_market_maker(payload)
                 except:
                     LOGGER.exception("Error in latest_price_from_market_maker")
-        elif payload.TypeName == SimTimestep_Maker.type_name:
-            try:
-                self.timestep_from_timecoordinator(payload)
-            except:
-                LOGGER.exception("Error in timestep_from_timecoordinator")
-
-    def heartbeat_from_super(self, from_alias: str, ping: HeartbeatA) -> None:
-        pong = HeartbeatA_Maker(
-            my_hex=str(random.choice("0123456789abcdef")), your_last_hex=ping.MyHex
-        ).tuple
-
-        self.send_message(
-            payload=pong,
-            to_role=GNodeRole.Supervisor,
-            to_g_node_alias=self.settings.my_super_alias,
-        )
-
-        LOGGER.debug(
-            f"[{self.alias}] Sent HB: SuHex {pong.YourLastHex}, AtnHex {pong.MyHex}"
-        )
+        else:
+            # If the message is not recognized, kick up to base class
+            super().route_message(from_alias, from_role, payload)
 
     def heartbeat_from_scada(self, ping: HeartbeatB) -> None:
         """
         This is the Atn's half of the DispatchContract Heartbeat pattern.
         It:
           - Checks that it has opted into a DispatchContract
           - Checks the  FromGNodeInstanceId to validate Scada credentials
@@ -386,15 +358,15 @@
         Turn OFF a relay (i.e. closes the electrical circuit so that current can flow),
         using the name of the relay as represented in the hardware layout as a Spaceheat
         Node with role "BooleanActuator"
 
         [SpaceheatNode](https://gridworks-protocol.readthedocs.io/en/latest/spaceheat-node.html)
         [BooleanActuator Role](https://gridworks-protocol.readthedocs.io/en/latest/enums.html#gwproto.enums.Role)
         Args:
-            relay_node_name: the name of the relay, as string in LeftRightDot format. This must be the
+            relay_node_name (str): the name of the relay, as string in LeftRightDot format. This must be the
             name of a SpaceheatNode in the hardware layout with role "BooleanActuator"
 
         Returns:
             None
         """
         self.send_scada_message(
             payload=GtDispatchBoolean_Maker(
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/atn_utils.py` & `gridworks_atn-0.3.8/src/gwatn/atn_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,44 @@
 from pydantic import BaseModel
 
 from gwatn import property_format
 from gwatn.data_classes import MarketType
 from gwatn.enums import MarketTypeName
+from gwatn.types import AtnParams
+from gwatn.types import FloParams
 from gwatn.types import MarketSlot
 from gwatn.types import MarketTypeGt_Maker
 
 
+DUMMY_TERMINALASSET_ALIAS = "d1.isone.dummy.ta"
 DUMMY_ALGO_TXN = "gqNzaWfEQNPXbrAiWd+cNgsIaM3N0PSu3repauvmjuHmoKjh6sd3L5U4/YpovcXN7/ATH1LgcI4cgV+SU3VQ6bsm/gfAOQyjdHhuiaNhbXTNB9CjZmVlzQPoomZ2HaNnZW6qc2FuZG5ldC12MaJnaMQgaJXPYTdWaeTNSs8FMMzPNfV7SrHXqJgFsJLxRbSPjzCibHbNBAWjcmN2xCBWkH3PValty0Rb0cyZo69Alhp4IbNKFnhXtgJ++A9EzKNzbmTEIOJPEbccL6IqmeBeaLzbLav25U9jBMjloaIyF1eY9HFxpHR5cGWjcGF5"
 
 
 class DijkstraChoice(BaseModel):
     PowerImportedKw: float
     NextNodeCostDollars: float
 
 
 class CostAndQuantityBought(BaseModel):
     QuantityBought: float
     Cost: float
 
 
+def is_dummy_atn_params(atn_params: AtnParams) -> bool:
+    if atn_params.GNodeAlias == DUMMY_TERMINALASSET_ALIAS:
+        return True
+    return False
+
+
+def is_dummy_flo_params(flo_params: FloParams) -> bool:
+    if flo_params.GNodeAlias == DUMMY_TERMINALASSET_ALIAS:
+        return True
+    return False
+
+
 def name_from_market_slot(slot: MarketSlot) -> str:
     return f"{slot.Type.Name.value}.{slot.MarketMakerAlias}.{slot.StartUnixS}"
 
 
 def market_slot_from_name(market_slot_name: str) -> MarketSlot:
     """rt60gate30b.d1.isone.ver.keene.1577836800"""
     try:
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/atn.py` & `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/atn.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import functools
 import logging
 import math
 import random
 import time
 import uuid
 from typing import Optional
+from typing import cast
 from typing import no_type_check
 
 import dotenv
 import gridworks.algo_utils as algo_utils
 import pendulum
 import requests
 from algosdk import encoding
@@ -37,15 +38,16 @@
 from gwatn.brick_storage_heater.flo import Flo__BrickStorageHeater as Flo
 from gwatn.brick_storage_heater.strategy_utils import SlotStuff
 from gwatn.enums import GNodeRole
 from gwatn.enums import MessageCategory
 from gwatn.enums import MessageCategorySymbol
 from gwatn.enums import UniverseType
 from gwatn.types import AcceptedBid_Maker
-from gwatn.types import AtnParamsBrickstorageheater as AtnParams
+from gwatn.types import AtnParams
+from gwatn.types import AtnParamsBrickstorageheater
 from gwatn.types import AtnParamsReport_Maker
 from gwatn.types import HeartbeatA
 from gwatn.types import HeartbeatA_Maker
 from gwatn.types import LatestPrice
 from gwatn.types import MarketSlot
 from gwatn.types import MarketTypeGt
 from gwatn.types import MarketTypeGt_Maker
@@ -78,15 +80,17 @@
         LOGGER.info("Initializing HeatPumpWithBoostStore Atn")
         self.algo_acct: BasicAccount = BasicAccount(settings.sk.get_secret_value())
         self.algo_client: AlgodClient = AlgodClient(
             settings.algo_api_secrets.algod_token.get_secret_value(),
             settings.public.algod_address,
         )
         if self.universe_type == UniverseType.Dev:
-            self.atn_params: AtnParams = strategy_utils.dummy_atn_params()
+            self.atn_params: AtnParamsBrickstorageheater = (
+                strategy_utils.dummy_atn_params()
+            )
         else:
             self.get_initial_params()
         self.market_type: MarketTypeGt = MarketTypeGt_Maker.dc_to_tuple(Rt60Gate30B)
         self.active_run: SlotStuff = strategy_utils.dummy_slot_stuff(
             slot=self.active_slot(self.market_type)
         )
         self.next_run: SlotStuff = strategy_utils.dummy_slot_stuff(
@@ -144,15 +148,15 @@
 
     def new_timestep(self, payload: SimTimestep) -> None:
         # LOGGER.info("----------------------------------------------------")
         # LOGGER.info(f"[{self.time_str()}: {self.short_alias}] NEW TIMESTEP")
         # LOGGER.info("----------------------------------------------------")
 
         # This gets called on the first timestep
-        if strategy_utils.is_dummy_atn_params(self.atn_params):
+        if atn_utils.is_dummy_atn_params(self.atn_params):
             self.get_initial_params()
             LOGGER.info("Correcting runs on initial timestep")
             self.active_run = strategy_utils.dummy_slot_stuff(
                 slot=self.last_slot(self.market_type),
             )
             try:
                 self.next_run = dev_io.initialize_slot_stuff(
@@ -418,29 +422,29 @@
             return rr
 
     ########################
     # Initialization
     ########################
 
     def dev_get_initial_params(self) -> None:
-        if not strategy_utils.is_dummy_atn_params(self.atn_params):
+        if not atn_utils.is_dummy_atn_params(cast(AtnParams, self.atn_params)):
             LOGGER.warning("Tried to get initial params but already have them")
 
         now_ms = int(self.time()) * 1000
         self.atn_params = dev_io.atn_params_from_alias(alias=self.alias, now_ms=now_ms)
         self.atn_params.GNodeInstanceId = self.g_node_instance_id
-        if strategy_utils.is_dummy_atn_params(self.atn_params):
+        if atn_utils.is_dummy_atn_params(cast(AtnParams, self.atn_params)):
             LOGGER.warning(f"No atn_params for {self.alias} before {self.time_str()}")
             return
         payload = AtnParamsReport_Maker(
             g_node_alias=self.alias,
             g_node_instance_id=self.g_node_instance_id,
             atn_params_type_name=self.atn_params.TypeName,
             time_unix_s=int(self.time()),
-            params=self.atn_params,
+            params=cast(AtnParams, self.atn_params),
             irl_time_unix_s=int(time.time()),
         ).tuple
 
         self.send_message(
             payload=payload, message_category=MessageCategory.RabbitJsonBroadcast
         )
         # LOGGER.info(f"[{self.time_str()}: {self.short_alias}] Initial params loaded")
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/dev_io.py` & `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/dev_io.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/edge.py` & `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/edge.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/flo.py` & `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/flo.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/flo_output.py` & `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/flo_output.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/make_dev_input_data.py` & `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/make_dev_input_data.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/node.py` & `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/brick_storage_heater/strategy_utils.py` & `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/strategy_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from typing import List
 from typing import Optional
+from typing import cast
 
 from pydantic import BaseModel
 
+from gwatn.atn_utils import DUMMY_TERMINALASSET_ALIAS
+from gwatn.atn_utils import is_dummy_flo_params
 from gwatn.brick_storage_heater.flo import Flo__BrickStorageHeater as Flo
 from gwatn.types import AtnBid
 from gwatn.types import AtnParamsBrickstorageheater as AtnParams
-from gwatn.types import FloParamsBrickstorageheater as FloParams
+from gwatn.types import AtnParamsBrickstorageheater_Maker as AtnParams_Maker
+from gwatn.types import FloParams
+from gwatn.types import FloParamsBrickstorageheater
 from gwatn.types import MarketSlot
 
 
 class SlotStuff(BaseModel):
     Slot: MarketSlot
-    BidParams: Optional[FloParams] = None
+    BidParams: Optional[FloParamsBrickstorageheater] = None
     Flo: Optional[Flo] = None
     Bid: Optional[AtnBid] = None
     Price: Optional[float] = None
 
 
 def dummy_bid() -> AtnBid:
     return AtnBid(
@@ -27,44 +32,27 @@
 def dummy_slot_stuff(slot: MarketSlot) -> SlotStuff:
     return SlotStuff(
         Slot=slot, FloStartIdx=50, BidParams=dummy_flo_params(), AtnBid=dummy_bid()
     )
 
 
 def is_dummy_slot_stuff(bid_stuff: SlotStuff) -> bool:
-    if is_dummy_flo_params(bid_stuff.BidParams):
-        return True
-    return False
-
-
-def is_dummy_atn_params(atn_params: AtnParams) -> bool:
-    if atn_params.GNodeAlias == "d1.isone.dummy.ta":
+    if is_dummy_flo_params(cast(FloParams, bid_stuff.BidParams)):
         return True
     return False
 
 
 def dummy_atn_params() -> AtnParams:
-    return AtnParams(
-        SliceDurationMinutes=60,
-        FloSlices=48,
-        GNodeAlias="d1.isone.dummy.ta",
-        GNodeInstanceId="00000000-0000-0000-0000-000000000000",
-        TypeName="atn.params.heatpumpwithbooststore",
-        Version="000",
-    )
-
-
-def is_dummy_flo_params(flo_params: FloParams) -> bool:
-    if flo_params.RtElecPriceUid == "00000000-0000-0000-0000-000000000000":
-        return True
-    return False
+    return AtnParams(GNodeAlias=DUMMY_TERMINALASSET_ALIAS)
 
 
-def dummy_flo_params() -> FloParams:
-    return FloParams(
+def dummy_flo_params() -> FloParamsBrickstorageheater:
+    return FloParamsBrickstorageheater(
+        GNodeAlias=DUMMY_TERMINALASSET_ALIAS,
+        FloParamsUid="00000000-0000-0000-0000-000000000000",
         RtElecPriceUid="00000000-0000-0000-0000-000000000000",
         WeatherUid="00000000-0000-0000-0000-000000000000",
     )
 
 
 def get_max_store_kwh_th(max_brick_temp_c: int, c: float, room_temp_f: int) -> float:
     """Use max store temp, room temp, and CF to get max store energy in kWh_th"""
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/config.py` & `gridworks_atn-0.3.8/src/gwatn/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,34 +7,32 @@
 from gridworks.gw_config import GNodeSettings
 from gridworks.gw_config import Public
 from pydantic import BaseSettings
 from pydantic import SecretStr
 
 
 class AtnSettings(GNodeSettings):
+    # Changing the default values for these GNodeSettings
     g_node_alias: str = "d1.isone.ver.keene.holly"
     g_node_role_value: str = "AtomicTNode"
     my_super_alias: str = "d1.isone.ver.keene.super1"
     g_node_id: str = "6bb37cc5-740d-40f5-a535-43987a5d07b4"
-    g_node_instance_id: str = "00000000-0000-0000-0000-000000000000"
-    scada_gni_id: Optional[str] = None
     sk: SecretStr = SecretStr(
         "K6iB3AHmzSQ8wDE91QdUfaheDMEtf2WJUMYeeRptKxHiTxG3HC+iKpngXmi82y2r9uVPYwTI5aGiMhdXmPRxcQ=="
     )
-    # Public address 4JHRDNY4F6RCVGPALZULZWZNVP3OKT3DATEOLINCGILVPGHUOFY7KCHVIQ
+    # Secret key for public Algorand address 4JHRDNY4F6RCVGPALZULZWZNVP3OKT3DATEOLINCGILVPGHUOFY7KCHVIQ
 
+    # Additional settings specific to AtomicTNodes
+    scada_gni_id: Optional[str] = None
     # Next 4 settings are consistent with dev env settings in gridworks-marketmaker repo
     market_maker_alias = "d1.isone.ver.keene"
     market_maker_algo_address = (
         "CYWMWYHJ7ON4IR5XQDJBBPDU472QU4KJQ6XQVZBIIRTCHT6SHTFNHEAVC4"
     )
     mm_api_root = "http://localhost:7997"
-    initial_time_unix_s = pendulum.datetime(
-        year=2020, month=1, day=1, hour=4, minute=20
-    ).int_timestamp
 
     class Config:
         env_prefix = "ATN_"
         env_nested_delimiter = "__"
 
 
 class ValidatorSettings(BaseSettings):
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/data_classes/.DS_Store` & `gridworks_atn-0.3.8/src/gwatn/data_classes/.DS_Store`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/data_classes/__init__.py` & `gridworks_atn-0.3.8/src/gwatn/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/data_classes/d_edge.py` & `gridworks_atn-0.3.8/src/gwatn/data_classes/d_edge.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/data_classes/d_graph.py` & `gridworks_atn-0.3.8/src/gwatn/data_classes/d_graph.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/data_classes/d_node.py` & `gridworks_atn-0.3.8/src/gwatn/data_classes/d_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/data_classes/hack_price_method.py` & `gridworks_atn-0.3.8/src/gwatn/data_classes/hack_price_method.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/data_classes/hack_weather_location.py` & `gridworks_atn-0.3.8/src/gwatn/data_classes/hack_weather_location.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/data_classes/hack_weather_source.py` & `gridworks_atn-0.3.8/src/gwatn/data_classes/hack_weather_source.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/demo_methods.py` & `gridworks_atn-0.3.8/src/gwatn/demo_methods.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_discoverer.py` & `gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_discoverer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_ta_owner.py` & `gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_ta_owner.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/dev_utils/dev_validator.py` & `gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_validator.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/dev_utils/make_plants.py` & `gridworks_atn-0.3.8/src/gwatn/dev_utils/make_plants.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/dispatch_contract.py` & `gridworks_atn-0.3.8/src/gwatn/dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/application.json` & `gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/application.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/approval.teal` & `gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/approval.teal`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/dispatch_contract_artifacts/contract.json` & `gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/contract.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/enums/__init__.py` & `gridworks_atn-0.3.8/src/gwatn/enums/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,18 +23,14 @@
 from gwproto.enums.role import Role
 from gwproto.enums.telemetry_name import TelemetryName
 from gwproto.enums.unit import Unit
 
 # From gwatn
 from gwatn.enums.distribution_tariff import DistributionTariff
 from gwatn.enums.energy_supply_type import EnergySupplyType
-from gwatn.enums.hack_price_method import PriceMethod
-from gwatn.enums.hack_recognized_p_node_alias import RecognizedPNodeAlias
-from gwatn.enums.hack_weather_method import WeatherMethod
-from gwatn.enums.hack_weather_source import WeatherSource
 from gwatn.enums.recognized_irradiance_type import RecognizedIrradianceType
 from gwatn.enums.recognized_temperature_unit import RecognizedTemperatureUnit
 
 
 __all__ = [
     "ActorClass",
     "AlgoCertType",
@@ -47,21 +43,17 @@
     "LocalCommInterface",
     "MakeModel",
     "MarketPriceUnit",
     "MarketQuantityUnit",
     "MarketTypeName",
     "MessageCategory",
     "MessageCategorySymbol",
-    "PriceMethod",
     "RecognizedCurrencyUnit",
     "RecognizedIrradianceType",
-    "RecognizedPNodeAlias",
     "RecognizedTemperatureUnit",
     "Role",
     "StrategyName",
     "SupervisorContainerStatus",
     "TelemetryName",
     "Unit",
     "UniverseType",
-    "WeatherMethod",
-    "WeatherSource",
 ]
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/enums/distribution_tariff.py` & `gridworks_atn-0.3.8/src/gwatn/enums/energy_supply_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from enum import auto
 from typing import List
 
 from fastapi_utils.enums import StrEnum
 
 
-class DistributionTariff(StrEnum):
+class EnergySupplyType(StrEnum):
     """
-    Name of distribution tariff of local network company/utility
+
 
     Choices and descriptions:
 
       * Unknown:
-      * VersantStorageHeatTariff:
-      * VersantATariff:
+      * StandardOffer:
+      * RealtimeLocalLmp:
     """
 
     Unknown = auto()
-    VersantStorageHeatTariff = auto()
-    VersantATariff = auto()
+    StandardOffer = auto()
+    RealtimeLocalLmp = auto()
 
     @classmethod
-    def default(cls) -> "DistributionTariff":
+    def default(cls) -> "EnergySupplyType":
         """
         Returns default value Unknown
         """
         return cls.Unknown
 
     @classmethod
     def values(cls) -> List[str]:
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/enums/hack_price_method.py` & `gridworks_atn-0.3.8/src/gwatn/enums/hack_price_method.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/enums/hack_weather_method.py` & `gridworks_atn-0.3.8/src/gwatn/enums/hack_weather_method.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/enums/recognized_irradiance_type.py` & `gridworks_atn-0.3.8/src/gwatn/enums/recognized_irradiance_type.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/enums/recognized_temperature_unit.py` & `gridworks_atn-0.3.8/src/gwatn/enums/recognized_temperature_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/python_ta_daemon.json` & `gridworks_atn-0.3.8/src/gwatn/python_ta_daemon.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/python_ta_daemon.py` & `gridworks_atn-0.3.8/src/gwatn/python_ta_daemon.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/scada_codec.py` & `gridworks_atn-0.3.8/src/gwatn/scada_codec.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/simple_atn_actor.py` & `gridworks_atn-0.3.8/src/gwatn/simple_atn_actor.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import time
 
 import dotenv
 import rich
 from gwproto.messages import PeerActiveEvent
 from gwproto.messages import Ping as GridworksPing
 
+import gwatn.atn_utils as atn_utils
 import gwatn.config as config
 from gwatn.atn_actor_base import AtnActorBase
 from gwatn.enums import TelemetryName
+from gwatn.types import AtnParams
 from gwatn.types import GtShStatus
 from gwatn.types import LatestPrice
 from gwatn.types import PowerWatts
 from gwatn.types import SimTimestep
 from gwatn.types import SnapshotSpaceheat
 
 
@@ -29,14 +31,15 @@
     def __init__(
         self,
         settings: config.AtnSettings = config.AtnSettings(
             _env_file=dotenv.find_dotenv()
         ),
     ):
         super().__init__(settings=settings)
+        self.atn_params = AtnParams(GNodeAlias=atn_utils.DUMMY_TERMINALASSET_ALIAS)
         self._power_watts: int = 0
         LOGGER.info("Simple Atn Initialized")
 
     def latest_price_from_market_maker(self, payload: LatestPrice) -> None:
         pass
 
     def new_timestep(self, payload: SimTimestep) -> None:
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/simple_scada_sim_actor_base.py` & `gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/simple_scada_sim.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 from gwatn.types import GwCertId_Maker
 from gwatn.types import HeartbeatA
 from gwatn.types import HeartbeatA_Maker
 from gwatn.types import HeartbeatB
 from gwatn.types import HeartbeatB_Maker
 from gwatn.types import JoinDispatchContract_Maker
 from gwatn.types import ScadaCertTransfer_Maker
-from gwatn.types import SimplesimDriverReport
-from gwatn.types import SimplesimDriverReport_Maker
+from gwatn.types import SimScadaDriverReportBsh as SimScadaDriverReport
+from gwatn.types import SimScadaDriverReportBsh_Maker as SimScadaDriverReport_Maker
 from gwatn.types import SimTimestep
 from gwatn.types import SimTimestep_Maker
 from gwatn.types import SnapshotBrickstorageheater as Snapshot
 
 
 DISPATCH_CONTRACT_REPORTING_ALGOS = 5
 
@@ -64,23 +64,25 @@
 
 class AtnHbStatus(BaseModel):
     LastHeartbeatReceivedMs: int
     AtnLastHex: Optional[str] = None
     ScadaLastHex: str = "0"
 
 
-class SimpleScadaSimActorBase(ActorBase):
+class ScadaActor(ActorBase):
     def __init__(
         self,
         settings: config.ScadaSettings = config.ScadaSettings(
             _env_file=dotenv.find_dotenv()
         ),
     ):
         super().__init__(settings=settings)
-
+        self.api_type_maker_by_name = (
+            api_types.TypeMakerByName
+        )  # overwrites base class to include types used in this repo
         self.settings = settings
         self.atn_gni_id = settings.atn_gni_id
         self.acct: BasicAccount = BasicAccount(settings.sk.get_secret_value())
         self.client: AlgodClient = AlgodClient(
             settings.algo_api_secrets.algod_token.get_secret_value(),
             settings.public.algod_address,
         )
@@ -95,18 +97,21 @@
         self.dc_client: Optional[ApplicationClient] = None
         self.dc_app_id: Optional[int] = None
         self.algo_init_check()
         self.universe_type = as_enum(
             self.settings.universe_type_value, UniverseType, UniverseType.default()
         )
         self._time: float = self.get_initial_time_s()
-        self.api_type_maker_by_name = (
-            api_types.TypeMakerByName
-        )  # overwrites base class to include types used in this repo
-        self.atn_params_type_name: str = "atn.params"  # overwrite in the subclass
+
+        self.boost_power_kw: float = 0
+        self.power_watts: float = 0
+        self.cop: float = 0
+        self.store_kwh: int = 0
+        self.max_store_kwh: int = 0
+        self.atn_params: Optional[AtnParams] = None
 
     @property
     def atn_alias(self):
         """Removes `scada` from the end of the SCADA's GNodeAlias"""
         return self.alias[:-6]
 
     @property
@@ -186,19 +191,19 @@
                 LOGGER.info(
                     f"Ignoring HeartbeatB from GNode with role {from_role}; expects AtomicTNode"
                 )
             try:
                 self.heartbeat_from_atn(ping=payload)
             except:
                 LOGGER.exception("Error in heartbeat_from_atn")
-        elif payload.TypeName == SimplesimDriverReport_Maker.type_name:
+        elif payload.TypeName == SimScadaDriverReport_Maker.type_name:
             try:
-                self.simplesim_driver_report_received(payload)
+                self.sim_scada_driver_report_received(payload)
             except:
-                LOGGER.exception("Error in simplesim_driver_report_received")
+                LOGGER.exception("Error in sim_scada_driver_report_received")
         elif payload.TypeName == SimTimestep_Maker.type_name:
             if from_role != GNodeRole.TimeCoordinator:
                 LOGGER.info(
                     f"Ignoring SimTimestep from GNode with role {from_role}; expects TimeCoordinator"
                 )
             try:
                 self.timestep_from_timecoordinator(payload)
@@ -528,23 +533,24 @@
         self.dc_client.opt_in()
         LOGGER.info(f"Dispatch Contract {self.dc_app_id} is live")
 
     #########################################################
     # Make the below into abstractmethods if pulling out base class
     #########################################################
 
-    def simplesim_driver_report_received(self, payload: SimplesimDriverReport) -> None:
+    def sim_scada_driver_report_received(self, payload: SimScadaDriverReport) -> None:
         """This gets received right before the top of the hour, from our
         best simulation of the TerminalAsset (which is happening in the
-        AtomicTNode).
-
-        Should be overwritten by the derived class, according to the
-        DriverDataTypeName. Should then send snapshot."""
-        if payload.FromGNodeInstanecId != self.atn_gni_id:
+        AtomicTNode)."""
+        if payload.FromGNodeInstanceId != self.atn_gni_id:
             LOGGER.info(f"Igoring {payload} - incorrect GNodeInstanceId")
+        self.power_watts = payload.PowerWatts
+        self.store_kwh = payload.StoreKwh
+        self.max_store_kwh = payload.MaxStoreKwh
+        self.send_snapshot()
 
     def send_snapshot(self):
         """Send a snapshot of current core sensed values to AtomicTNode.
         This is done every hour, and also on sensed power change."""
         if self.atn_params is None:
             return
         report_payload = Snapshot(
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/ta_daemon_rest_api.py` & `gridworks_atn-0.3.8/src/gwatn/ta_daemon_rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/two_channel_actor_base.py` & `gridworks_atn-0.3.8/src/gwatn/two_channel_actor_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import enum
 import functools
 import logging
+import random
 import threading
 import time
 import uuid
 from abc import ABC
 from abc import abstractmethod
 from enum import auto
 from typing import Dict
 from typing import Optional
 from typing import TypeVar
 from typing import no_type_check
 
 import gridworks.property_format as property_format
 import gridworks.utils as utils
+import pendulum
 import pika  # type: ignore
 from fastapi_utils.enums import StrEnum
 from gridworks.enums import GNodeRole
 from gridworks.errors import SchemaError
 from gwproto.message import Message as ScadaMessage
 from gwproto.messages import Ack
 from pydantic import ValidationError
@@ -26,14 +28,16 @@
 from gwatn.config import AtnSettings
 from gwatn.enums import MessageCategory
 from gwatn.enums import MessageCategorySymbol
 from gwatn.enums import UniverseType
 from gwatn.scada_codec import ScadaCodec
 from gwatn.types import HeartbeatA
 from gwatn.types import HeartbeatA_Maker
+from gwatn.types import SimTimestep
+from gwatn.types import SimTimestep_Maker
 
 
 PayloadT = TypeVar("PayloadT")
 
 
 class RabbitRole(StrEnum):
     atomictnode = auto()
@@ -103,31 +107,36 @@
 class DbgMsg(BaseModel):
     RoutingKey: str
     MessageType: bytes
     MessageTuple: ScadaMessage
 
 
 class TwoChannelActorBase(ABC):
-    SHUTDOWN_INTERVAL = 0.1
+    SHUTDOWN_INTERVAL: float = 0.1
 
     def __init__(
         self,
         settings: AtnSettings,
         api_type_maker_by_name: Dict[str, HeartbeatA_Maker] = api_types.TypeMakerByName,
     ):
+        self.settings: AtnSettings = settings
         self.scada_codec = ScadaCodec()
         self.dbg_messages: List[DbgMsg] = []
         self.api_type_maker_by_name = api_type_maker_by_name
         self.latest_routing_key: Optional[str] = None
         self.shutting_down: bool = False
         self.alias: str = settings.g_node_alias
         self.g_node_instance_id: str = settings.g_node_instance_id
         self.g_node_role: GNodeRole = GNodeRole(settings.g_node_role_value)
         self.rabbit_role: RabbitRole = RabbitRolebyRole[self.g_node_role]
         self.universe_type: UniverseType = UniverseType(settings.universe_type_value)
+        # Used for tracking time in simulated worlds
+        self._time: float = time.time()
+        if self.universe_type == UniverseType.Dev:
+            self._time = settings.initial_time_unix_s
         self.actor_main_stopped: bool = False
 
         adder = "-F" + str(uuid.uuid4()).split("-")[0][0:3]
         self.queue_name: str = self.alias + adder
         self._consume_exchange: str = self.rabbit_role.value + "_tx"
         self._publish_exchange: str = self.rabbit_role.value + "mic_tx"
 
@@ -187,14 +196,17 @@
         self._stopped = True
 
     def local_stop(self) -> None:
         """This should be overwritten in derived class if there is a requirement
         to stop the additional threads started in local_start"""
         pass
 
+    def __repr__(self) -> str:
+        return f"{self.alias}"
+
     @no_type_check
     def on_message(self, _unused_channel, basic_deliver, properties, body) -> None:
         """Invoked by pika when a message is delivered from RabbitMQ. If a message
         does not get here that you expect should get here, check the routing key
         of the outbound message and the rabbitmq bindings.
 
         Parses the TypeName of the message payload and the GNodeAlias of the sender.
@@ -293,19 +305,83 @@
         )
         self.route_message(
             from_alias=from_alias,
             from_role=from_role,
             payload=payload,
         )
 
-    @abstractmethod
     def route_message(
         self, from_alias: str, from_role: GNodeRole, payload: HeartbeatA
     ) -> None:
-        raise NotImplementedError
+        if payload.TypeName == HeartbeatA_Maker.type_name:
+            if from_role != GNodeRole.Supervisor:
+                LOGGER.info(
+                    f"Ignoring HeartbeatA from GNode {from_alias} with GNodeRole {from_role}; expects"
+                    f"Supervisor as the GNodeRole"
+                )
+                return
+            elif from_alias != self.settings.my_super_alias:
+                LOGGER.info(
+                    f"Ignoring HeartbeatA from supervisor {from_alias}; "
+                    f"my supervisor is {self.settings.my_super_alias}"
+                )
+                return
+
+            try:
+                self.heartbeat_from_super(from_alias, payload)
+            except:
+                LOGGER.exception("Error in heartbeat_received")
+        elif payload.TypeName == SimTimestep_Maker.type_name:
+            try:
+                self.timestep_from_timecoordinator(payload)
+            except:
+                LOGGER.exception("Error in timestep_from_timecoordinator")
+
+    def heartbeat_from_super(self, from_alias: str, ping: HeartbeatA) -> None:
+        """
+        Subordinate GNode responds to its supervisor's heartbeat with a "pong" message.
+
+        Both the received heartbeat (ping) and the response (pong) have the type HeartbeatA
+        (see: https://gridworks.readthedocs.io/en/latest/apis/types.html#heartbeata).
+
+        The subordinate GNode generates its own unique identifier (hex) and includes it
+        in the pong message along with the heartbeat it received from the supervisor.
+
+        Please note that the subordinate GNode does not have the responsibility of verifying
+        the authenticity of the last heartbeat received from the supervisor - although typically,
+        the supervisor does send the last heartbeat from this GNode (except during the initial
+        heartbeat exchange).
+
+        Args:
+            from_alias (str): the alias of the GNode that sent the ping.
+            ping (HeartbeatA): the heartbeat sent.
+
+        Raises:
+        ValueError: If `from_alias` is not this GNode's Supervisor alias.
+
+        """
+        if from_alias != self.settings.my_super_alias:
+            raise ValueError(
+                f"from_alias {from_alias} does not match my supervisor"
+                f" {self.settings.my_super_alias}. This message should"
+                f"have been filtered out in the route_message method."
+            )
+        pong = HeartbeatA_Maker(
+            my_hex=str(random.choice("0123456789abcdef")), your_last_hex=ping.MyHex
+        ).tuple
+
+        self.send_message(
+            payload=pong,
+            to_role=GNodeRole.Supervisor,
+            to_g_node_alias=self.settings.my_super_alias,
+        )
+
+        LOGGER.debug(
+            f"[{self.alias}] Sent HB: SuHex {pong.YourLastHex}, AtnHex {pong.MyHex}"
+        )
 
     def route_scada_message(self, from_alias: str, message: ScadaMessage) -> None:
         """This router should be overwritten by derived class"""
         ...
 
     @no_type_check
     def send_scada_message(
@@ -1165,17 +1241,41 @@
             raise SchemaError(
                 f"Unknown short alias {rabbit_role} in {routing_key}"
                 f" Must belong to {RabbitRole}"
             )
 
         return RoleByRabbitRole[rabbit_role]
 
-    #################################################
-    # On receiving messages broadcast to all listners
-    #################################################
-
-    #################################################
-    # Various
-    #################################################
+    ########################
+    ## Time related (simulated time)
+    ########################
 
-    def __repr__(self) -> str:
-        return f"{self.alias}"
+    def timestep_from_timecoordinator(self, payload: SimTimestep) -> None:
+        if self._time < payload.TimeUnixS:
+            self._time = payload.TimeUnixS
+            self.new_timestep(payload)
+            LOGGER.debug(f"Time is now {self.time_str()}")
+        elif self._time == payload.TimeUnixS:
+            self.repeat_timestep(payload)
+
+    def new_timestep(self, payload: SimTimestep) -> None:
+        LOGGER.info("New timestep")
+
+    def repeat_timestep(self, payload: SimTimestep) -> None:
+        LOGGER.info("Timestep received again in atn_actor_base")
+
+    def time(self) -> float:
+        if self.universe_type == UniverseType.Dev:
+            return self._time
+        else:
+            return time.time()
+
+    def time_str(self) -> str:
+        return pendulum.from_timestamp(self.time()).strftime("%m/%d/%Y, %H:%M")
+
+    ###############################
+    # Other GNode-related methods
+    ###############################
+
+    @property
+    def short_alias(self) -> str:
+        return self.alias.split(".")[-1]
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/__init__.py` & `gridworks_atn-0.3.8/src/gwatn/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,26 +97,38 @@
 from gwatn.types.atn_bid import AtnBid_Maker
 from gwatn.types.atn_params import AtnParams
 from gwatn.types.atn_params import AtnParams_Maker
 from gwatn.types.atn_params_brickstorageheater import AtnParamsBrickstorageheater
 from gwatn.types.atn_params_brickstorageheater import AtnParamsBrickstorageheater_Maker
 from gwatn.types.atn_params_report import AtnParamsReport
 from gwatn.types.atn_params_report import AtnParamsReport_Maker
+from gwatn.types.atn_params_simpleresistivehydronic import (
+    AtnParamsSimpleresistivehydronic,
+)
+from gwatn.types.atn_params_simpleresistivehydronic import (
+    AtnParamsSimpleresistivehydronic_Maker,
+)
 from gwatn.types.basegnode_scada_create import BasegnodeScadaCreate
 from gwatn.types.basegnode_scada_create import BasegnodeScadaCreate_Maker
 from gwatn.types.discoverycert_algo_create import DiscoverycertAlgoCreate
 from gwatn.types.discoverycert_algo_create import DiscoverycertAlgoCreate_Maker
 from gwatn.types.dispatch_contract_confirmed import DispatchContractConfirmed
 from gwatn.types.dispatch_contract_confirmed import DispatchContractConfirmed_Maker
 from gwatn.types.flo_params import FloParams
 from gwatn.types.flo_params import FloParams_Maker
 from gwatn.types.flo_params_brickstorageheater import FloParamsBrickstorageheater
 from gwatn.types.flo_params_brickstorageheater import FloParamsBrickstorageheater_Maker
 from gwatn.types.flo_params_report import FloParamsReport
 from gwatn.types.flo_params_report import FloParamsReport_Maker
+from gwatn.types.flo_params_simpleresistivehydronic import (
+    FloParamsSimpleresistivehydronic,
+)
+from gwatn.types.flo_params_simpleresistivehydronic import (
+    FloParamsSimpleresistivehydronic_Maker,
+)
 from gwatn.types.initial_tadeed_algo_create import InitialTadeedAlgoCreate
 from gwatn.types.initial_tadeed_algo_create import InitialTadeedAlgoCreate_Maker
 from gwatn.types.initial_tadeed_algo_optin import InitialTadeedAlgoOptin
 from gwatn.types.initial_tadeed_algo_optin import InitialTadeedAlgoOptin_Maker
 from gwatn.types.initial_tadeed_algo_transfer import InitialTadeedAlgoTransfer
 from gwatn.types.initial_tadeed_algo_transfer import InitialTadeedAlgoTransfer_Maker
 from gwatn.types.join_dispatch_contract import JoinDispatchContract
@@ -170,14 +182,16 @@
     "AtnBid_Maker",
     "AtnParams",
     "AtnParams_Maker",
     "AtnParamsBrickstorageheater",
     "AtnParamsBrickstorageheater_Maker",
     "AtnParamsReport",
     "AtnParamsReport_Maker",
+    "AtnParamsSimpleresistivehydronic",
+    "AtnParamsSimpleresistivehydronic_Maker",
     "BaseGNodeGt",
     "BaseGNodeGt_Maker",
     "BasegnodeScadaCreate",
     "BasegnodeScadaCreate_Maker",
     "ComponentAttributeClassGt",
     "ComponentAttributeClassGt_Maker",
     "ComponentGt",
@@ -198,14 +212,16 @@
     "ElectricMeterComponentGt_Maker",
     "FloParams",
     "FloParams_Maker",
     "FloParamsBrickstorageheater",
     "FloParamsBrickstorageheater_Maker",
     "FloParamsReport",
     "FloParamsReport_Maker",
+    "FloParamsSimpleresistivehydronic",
+    "FloParamsSimpleresistivehydronic_Maker",
     "GNodeGt",
     "GNodeGt_Maker",
     "GNodeInstanceGt",
     "GNodeInstanceGt_Maker",
     "GtDispatchBoolean",
     "GtDispatchBoolean_Maker",
     "GtDispatchBooleanLocal",
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/accepted_bid.py` & `gridworks_atn-0.3.8/src/gwatn/types/accepted_bid.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/atn_bid.py` & `gridworks_atn-0.3.8/src/gwatn/types/atn_bid.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/atn_params.py` & `gridworks_atn-0.3.8/src/gwatn/types/atn_params.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/atn_params_brickstorageheater.py` & `gridworks_atn-0.3.8/src/gwatn/types/atn_params_brickstorageheater.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,29 @@
 
 class DistributionTariff000SchemaEnum:
     enum_name: str = "distribution.tariff.000"
     symbols: List[str] = [
         "00000000",
         "2127aba6",
         "ea5c675a",
+        "54aec3a7",
     ]
 
     @classmethod
     def is_symbol(cls, candidate: str) -> bool:
         if candidate in cls.symbols:
             return True
         return False
 
 
 class DistributionTariff000(StrEnum):
     Unknown = auto()
-    VersantStorageHeatTariff = auto()
+    VersantA1StorageHeatTariff = auto()
     VersantATariff = auto()
+    VersantA20HeatTariff = auto()
 
     @classmethod
     def default(cls) -> "DistributionTariff000":
         return cls.Unknown
 
     @classmethod
     def values(cls) -> List[str]:
@@ -65,22 +67,24 @@
         versioned_enum = as_enum(
             distribution_tariff, DistributionTariff000, DistributionTariff000.default()
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, DistributionTariff000] = {
         "00000000": DistributionTariff000.Unknown,
-        "2127aba6": DistributionTariff000.VersantStorageHeatTariff,
+        "2127aba6": DistributionTariff000.VersantA1StorageHeatTariff,
         "ea5c675a": DistributionTariff000.VersantATariff,
+        "54aec3a7": DistributionTariff000.VersantA20HeatTariff,
     }
 
     versioned_enum_to_type_dict: Dict[DistributionTariff000, str] = {
         DistributionTariff000.Unknown: "00000000",
-        DistributionTariff000.VersantStorageHeatTariff: "2127aba6",
+        DistributionTariff000.VersantA1StorageHeatTariff: "2127aba6",
         DistributionTariff000.VersantATariff: "ea5c675a",
+        DistributionTariff000.VersantA20HeatTariff: "54aec3a7",
     }
 
 
 class RecognizedCurrencyUnit000SchemaEnum:
     enum_name: str = "recognized.currency.unit.000"
     symbols: List[str] = [
         "00000000",
@@ -335,15 +339,15 @@
     )
     CurrencyUnit: RecognizedCurrencyUnit = Field(
         title="CurrencyUnit",
         default=RecognizedCurrencyUnit.USD,
     )
     Tariff: DistributionTariff = Field(
         title="Tariff",
-        default=DistributionTariff.VersantStorageHeatTariff,
+        default=DistributionTariff.VersantA1StorageHeatTariff,
     )
     EnergyType: EnergySupplyType = Field(
         title="EnergyType",
         default=EnergySupplyType.RealtimeLocalLmp,
     )
     StandardOfferPriceDollarsPerMwh: int = Field(
         title="StandardOfferPriceDollarsPerMwh",
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/atn_params_report.py` & `gridworks_atn-0.3.8/src/gwatn/types/atn_params_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/basegnode_scada_create.py` & `gridworks_atn-0.3.8/src/gwatn/types/basegnode_scada_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/data_channel.py` & `gridworks_atn-0.3.8/src/gwatn/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/discoverycert_algo_create.py` & `gridworks_atn-0.3.8/src/gwatn/types/discoverycert_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/dispatch_contract_confirmed.py` & `gridworks_atn-0.3.8/src/gwatn/types/dispatch_contract_confirmed.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/flo_params.py` & `gridworks_atn-0.3.8/src/gwatn/types/flo_params.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/flo_params_brickstorageheater.py` & `gridworks_atn-0.3.8/src/gwatn/types/flo_params_brickstorageheater.py`

 * *Files 4% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         title="SliceDurationMinutes",
         default=[60],
     )
     PowerRequiredByHouseFromSystemAvgKwList: List[float] = Field(
         title="PowerRequiredByHouseFromSystemAvgKwList",
         default=[3.42],
     )
-    C: Optional[float] = Field(
+    C: float = Field(
         title="C",
         default=200,
     )
     RealtimeElectricityPrice: List[float] = Field(
         title="RealtimeElectricityPrice",
         default=[10.35],
     )
@@ -289,17 +289,16 @@
     RegulationPrice: List[float] = Field(
         title="RegulationPrice",
         default=[25.3],
     )
     WeatherUid: str = Field(
         title="WeatherUid",
     )
-    DistPriceUid: Optional[str] = Field(
+    DistPriceUid: str = Field(
         title="DistPriceUid",
-        default=None,
     )
     RegPriceUid: Optional[str] = Field(
         title="RegPriceUid",
         default=None,
     )
     StartYearUtc: int = Field(
         title="StartYearUtc",
@@ -369,17 +368,15 @@
         except ValueError as e:
             raise ValueError(
                 f"WeatherUid failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
     @validator("DistPriceUid")
-    def _check_dist_price_uid(cls, v: Optional[str]) -> Optional[str]:
-        if v is None:
-            return v
+    def _check_dist_price_uid(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
                 f"DistPriceUid failed UuidCanonicalTextual format validation: {e}"
             )
         return v
@@ -426,18 +423,14 @@
         del d["TempUnit"]
         TempUnit = as_enum(
             self.TempUnit,
             RecognizedTemperatureUnit,
             RecognizedTemperatureUnit.default(),
         )
         d["TempUnitGtEnumSymbol"] = RecognizedTemperatureUnitMap.local_to_type(TempUnit)
-        if d["C"] is None:
-            del d["C"]
-        if d["DistPriceUid"] is None:
-            del d["DistPriceUid"]
         if d["RegPriceUid"] is None:
             del d["RegPriceUid"]
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
@@ -460,22 +453,22 @@
         temp_unit: RecognizedTemperatureUnit,
         timezone_string: str,
         home_city: str,
         is_regulating: bool,
         storage_steps: int,
         slice_duration_minutes: List[int],
         power_required_by_house_from_system_avg_kw_list: List[float],
-        c: Optional[float],
+        c: float,
         realtime_electricity_price: List[float],
         outside_temp_f: List[float],
         distribution_price: List[float],
         rt_elec_price_uid: str,
         regulation_price: List[float],
         weather_uid: str,
-        dist_price_uid: Optional[str],
+        dist_price_uid: str,
         reg_price_uid: Optional[str],
         start_year_utc: int,
         start_month_utc: int,
         start_day_utc: int,
         start_hour_utc: int,
         start_minute_utc: int,
         starting_store_idx: int,
@@ -583,29 +576,29 @@
         if "SliceDurationMinutes" not in d2.keys():
             raise SchemaError(f"dict {d2} missing SliceDurationMinutes")
         if "PowerRequiredByHouseFromSystemAvgKwList" not in d2.keys():
             raise SchemaError(
                 f"dict {d2} missing PowerRequiredByHouseFromSystemAvgKwList"
             )
         if "C" not in d2.keys():
-            d2["C"] = None
+            raise SchemaError(f"dict {d2} missing C")
         if "RealtimeElectricityPrice" not in d2.keys():
             raise SchemaError(f"dict {d2} missing RealtimeElectricityPrice")
         if "OutsideTempF" not in d2.keys():
             raise SchemaError(f"dict {d2} missing OutsideTempF")
         if "DistributionPrice" not in d2.keys():
             raise SchemaError(f"dict {d2} missing DistributionPrice")
         if "RtElecPriceUid" not in d2.keys():
             raise SchemaError(f"dict {d2} missing RtElecPriceUid")
         if "RegulationPrice" not in d2.keys():
             raise SchemaError(f"dict {d2} missing RegulationPrice")
         if "WeatherUid" not in d2.keys():
             raise SchemaError(f"dict {d2} missing WeatherUid")
         if "DistPriceUid" not in d2.keys():
-            d2["DistPriceUid"] = None
+            raise SchemaError(f"dict {d2} missing DistPriceUid")
         if "RegPriceUid" not in d2.keys():
             d2["RegPriceUid"] = None
         if "StartYearUtc" not in d2.keys():
             raise SchemaError(f"dict {d2} missing StartYearUtc")
         if "StartMonthUtc" not in d2.keys():
             raise SchemaError(f"dict {d2} missing StartMonthUtc")
         if "StartDayUtc" not in d2.keys():
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/flo_params_report.py` & `gridworks_atn-0.3.8/src/gwatn/types/flo_params_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/gt_dispatch_boolean.py` & `gridworks_atn-0.3.8/src/gwatn/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/hack_property_format.py` & `gridworks_atn-0.3.8/src/gwatn/types/hack_property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/hack_type_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/hack_type_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/hack_utils.py` & `gridworks_atn-0.3.8/src/gwatn/types/hack_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/heartbeat_b.py` & `gridworks_atn-0.3.8/src/gwatn/types/heartbeat_b.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_create.py` & `gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_optin.py` & `gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/initial_tadeed_algo_transfer.py` & `gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/join_dispatch_contract.py` & `gridworks_atn-0.3.8/src/gwatn/types/join_dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/latest_price.py` & `gridworks_atn-0.3.8/src/gwatn/types/latest_price.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/market_slot.py` & `gridworks_atn-0.3.8/src/gwatn/types/market_slot.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/market_type_gt.py` & `gridworks_atn-0.3.8/src/gwatn/types/market_type_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/new_tadeed_algo_optin.py` & `gridworks_atn-0.3.8/src/gwatn/types/new_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/new_tadeed_send.py` & `gridworks_atn-0.3.8/src/gwatn/types/new_tadeed_send.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/old_tadeed_algo_return.py` & `gridworks_atn-0.3.8/src/gwatn/types/old_tadeed_algo_return.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/price_quantity.py` & `gridworks_atn-0.3.8/src/gwatn/types/price_quantity.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/price_quantity_unitless.py` & `gridworks_atn-0.3.8/src/gwatn/types/price_quantity_unitless.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/scada_cert_transfer.py` & `gridworks_atn-0.3.8/src/gwatn/types/scada_cert_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_data.py` & `gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_data.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_data_bsh.py` & `gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_data_bsh.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/simplesim_driver_report.py` & `gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_report.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 
 class SimplesimDriverReport(BaseModel):
     """ """
 
     FromGNodeAlias: str = Field(
         title="FromGNodeAlias",
     )
-    FromGNodeInstanecId: str = Field(
-        title="FromGNodeInstanecId",
+    FromGNodeInstanceId: str = Field(
+        title="FromGNodeInstanceId",
     )
     DriverDataTypeName: str = Field(
         title="DriverDataTypeName",
     )
     DriverData: SimplesimDriverData = Field(
         title="DriverData",
     )
@@ -93,21 +93,21 @@
             check_is_left_right_dot(v)
         except ValueError as e:
             raise ValueError(
                 f"FromGNodeAlias failed LeftRightDot format validation: {e}"
             )
         return v
 
-    @validator("FromGNodeInstanecId")
-    def _check_from_g_node_instanec_id(cls, v: str) -> str:
+    @validator("FromGNodeInstanceId")
+    def _check_from_g_node_instance_id(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
-                f"FromGNodeInstanecId failed UuidCanonicalTextual format validation: {e}"
+                f"FromGNodeInstanceId failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
     @validator("DriverDataTypeName")
     def _check_driver_data_type_name(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
@@ -132,21 +132,21 @@
 class SimplesimDriverReport_Maker:
     type_name = "simplesim.driver.report"
     version = "000"
 
     def __init__(
         self,
         from_g_node_alias: str,
-        from_g_node_instanec_id: str,
+        from_g_node_instance_id: str,
         driver_data_type_name: str,
         driver_data: SimplesimDriverData,
     ):
         self.tuple = SimplesimDriverReport(
             FromGNodeAlias=from_g_node_alias,
-            FromGNodeInstanecId=from_g_node_instanec_id,
+            FromGNodeInstanceId=from_g_node_instance_id,
             DriverDataTypeName=driver_data_type_name,
             DriverData=driver_data,
             #
         )
 
     @classmethod
     def tuple_to_type(cls, tuple: SimplesimDriverReport) -> str:
@@ -169,16 +169,16 @@
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> SimplesimDriverReport:
         d2 = dict(d)
         if "FromGNodeAlias" not in d2.keys():
             raise SchemaError(f"dict {d2} missing FromGNodeAlias")
-        if "FromGNodeInstanecId" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing FromGNodeInstanecId")
+        if "FromGNodeInstanceId" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
         if "DriverDataTypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing DriverDataTypeName")
         if "DriverData" not in d2.keys():
             raise SchemaError(f"dict {d2} missing DriverData")
         if not isinstance(d2["DriverData"], dict):
             raise SchemaError(
                 f"d['DriverData'] {d2['DriverData']} must be a SimplesimDriverData!"
@@ -186,13 +186,13 @@
         driver_data = SimplesimDriverData_Maker.dict_to_tuple(d2["DriverData"])
         d2["DriverData"] = driver_data
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
         return SimplesimDriverReport(
             FromGNodeAlias=d2["FromGNodeAlias"],
-            FromGNodeInstanecId=d2["FromGNodeInstanecId"],
+            FromGNodeInstanceId=d2["FromGNodeInstanceId"],
             DriverDataTypeName=d2["DriverDataTypeName"],
             DriverData=d2["DriverData"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/simplesim_snapshot_brickstorageheater.py` & `gridworks_atn-0.3.8/src/gwatn/types/simplesim_snapshot_brickstorageheater.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/sla_enter.py` & `gridworks_atn-0.3.8/src/gwatn/types/sla_enter.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/tadeed_specs_hack.py` & `gridworks_atn-0.3.8/src/gwatn/types/tadeed_specs_hack.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/tavalidatorcert_algo_create.py` & `gridworks_atn-0.3.8/src/gwatn/types/tavalidatorcert_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/tavalidatorcert_algo_transfer.py` & `gridworks_atn-0.3.8/src/gwatn/types/tavalidatorcert_algo_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/terminalasset_certify_hack.py` & `gridworks_atn-0.3.8/src/gwatn/types/terminalasset_certify_hack.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py` & `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.7/PKG-INFO` & `gridworks_atn-0.3.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gridworks-atn
-Version: 0.3.7
+Version: 0.3.8
 Summary: Gridworks Atn Spaceheat
 Home-page: https://github.com/thegridelectric/gridworks-atn
 License: None
-Author: Jessica Millar
-Author-email: jmillar@gridworks-consulting.com
+Author: GridWorks
+Author-email: gridworks@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: gridworks (>=0.2.4,<0.3.0)
-Requires-Dist: gridworks-protocol (>=0.5.2,<0.6.0)
+Requires-Dist: gridworks-proactor (>=0.2.2,<0.3.0)
+Requires-Dist: gridworks-ps (>=0.0.1,<0.0.2)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Project-URL: Changelog, https://github.com/thegridelectric/gridworks-atn/releases
 Project-URL: Documentation, https://gridworks-atn.readthedocs.io
 Project-URL: Repository, https://github.com/thegridelectric/gridworks-atn
 Description-Content-Type: text/markdown
```

