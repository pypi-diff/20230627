# Comparing `tmp/credmark-1.3.0.tar.gz` & `tmp/credmark-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credmark-1.3.0.tar", max compression
+gzip compressed data, was "credmark-1.4.0.tar", max compression
```

## Comparing `credmark-1.3.0.tar` & `credmark-1.4.0.tar`

### file list

```diff
@@ -1,142 +1,171 @@
--rw-r--r--   0        0        0     4502 2023-04-18 12:36:26.442770 credmark-1.3.0/README.md
--rw-r--r--   0        0        0      110 2023-05-05 12:58:23.125826 credmark-1.3.0/credmark/__init__.py
--rw-r--r--   0        0        0       47 2023-05-05 12:58:20.691648 credmark-1.3.0/credmark/api/__init__.py
--rw-r--r--   0        0        0     9643 2023-05-05 12:58:23.217765 credmark-1.3.0/credmark/api/defi_api/__init__.py
--rw-r--r--   0        0        0     8159 2023-05-05 12:58:23.251810 credmark-1.3.0/credmark/api/defi_api/get_cached_model_results.py
--rw-r--r--   0        0        0     3679 2023-05-05 12:58:23.191652 credmark-1.3.0/credmark/api/defi_api/get_model_by_slug.py
--rw-r--r--   0        0        0     4016 2023-05-05 12:58:23.197737 credmark-1.3.0/credmark/api/defi_api/get_model_deployments_by_slug.py
--rw-r--r--   0        0        0     3513 2023-05-05 12:58:23.195403 credmark-1.3.0/credmark/api/defi_api/get_model_runtime_stats.py
--rw-r--r--   0        0        0     3725 2023-05-05 12:58:23.205315 credmark-1.3.0/credmark/api/defi_api/list_models.py
--rw-r--r--   0        0        0     3912 2023-05-05 12:58:23.208691 credmark-1.3.0/credmark/api/defi_api/run_model.py
--rw-r--r--   0        0        0    79472 2023-05-05 13:02:14.091929 credmark-1.3.0/credmark/api/token_api/__init__.py
--rw-r--r--   0        0        0     7328 2023-05-05 12:58:23.254320 credmark-1.3.0/credmark/api/token_api/get_token_abi.py
--rw-r--r--   0        0        0    11298 2023-05-05 12:58:23.291430 credmark-1.3.0/credmark/api/token_api/get_token_balance.py
--rw-r--r--   0        0        0    15309 2023-05-05 12:58:23.345687 credmark-1.3.0/credmark/api/token_api/get_token_balance_historical.py
--rw-r--r--   0        0        0     8410 2023-05-05 12:58:23.279601 credmark-1.3.0/credmark/api/token_api/get_token_creation_block.py
--rw-r--r--   0        0        0     8274 2023-05-05 12:58:23.302161 credmark-1.3.0/credmark/api/token_api/get_token_decimals.py
--rw-r--r--   0        0        0    11822 2023-05-05 12:58:23.343893 credmark-1.3.0/credmark/api/token_api/get_token_holders.py
--rw-r--r--   0        0        0     7940 2023-05-05 12:58:23.305865 credmark-1.3.0/credmark/api/token_api/get_token_holders_count.py
--rw-r--r--   0        0        0    12559 2023-05-05 12:58:23.358950 credmark-1.3.0/credmark/api/token_api/get_token_holders_count_historical.py
--rw-r--r--   0        0        0     8170 2023-05-05 12:58:23.313369 credmark-1.3.0/credmark/api/token_api/get_token_logo.py
--rw-r--r--   0        0        0     8255 2023-05-05 12:58:23.329081 credmark-1.3.0/credmark/api/token_api/get_token_metadata.py
--rw-r--r--   0        0        0     8170 2023-05-05 12:58:23.364176 credmark-1.3.0/credmark/api/token_api/get_token_name.py
--rw-r--r--   0        0        0    11243 2023-05-05 12:58:23.394357 credmark-1.3.0/credmark/api/token_api/get_token_price.py
--rw-r--r--   0        0        0    16235 2023-05-05 12:58:23.469327 credmark-1.3.0/credmark/api/token_api/get_token_price_historical.py
--rw-r--r--   0        0        0     8222 2023-05-05 12:58:23.407436 credmark-1.3.0/credmark/api/token_api/get_token_symbol.py
--rw-r--r--   0        0        0     9238 2023-05-05 12:58:23.445394 credmark-1.3.0/credmark/api/token_api/get_token_total_supply.py
--rw-r--r--   0        0        0    13225 2023-05-05 12:58:23.517891 credmark-1.3.0/credmark/api/token_api/get_token_total_supply_historical.py
--rw-r--r--   0        0        0    11276 2023-05-05 12:58:23.485870 credmark-1.3.0/credmark/api/token_api/get_token_volume.py
--rw-r--r--   0        0        0    13437 2023-05-05 12:58:23.527021 credmark-1.3.0/credmark/api/token_api/get_token_volume_historical.py
--rw-r--r--   0        0        0     5822 2023-05-05 12:58:23.407441 credmark-1.3.0/credmark/api/utilities/__init__.py
--rw-r--r--   0        0        0     3575 2023-05-05 12:58:23.410726 credmark-1.3.0/credmark/api/utilities/check_health.py
--rw-r--r--   0        0        0     6512 2023-05-05 12:58:23.520382 credmark-1.3.0/credmark/api/utilities/get_daily_model_usage.py
--rw-r--r--   0        0        0     3373 2023-05-05 12:58:23.458974 credmark-1.3.0/credmark/api/utilities/get_top_models.py
--rw-r--r--   0        0        0     3351 2023-05-05 12:58:23.503111 credmark-1.3.0/credmark/api/utilities/get_total_model_usage.py
--rw-r--r--   0        0        0     2645 2023-05-05 12:58:23.492532 credmark-1.3.0/credmark/client.py
--rw-r--r--   0        0        0      320 2023-05-05 12:58:20.677683 credmark-1.3.0/credmark/docs/CheckHealthResponse200.md
--rw-r--r--   0        0        0       79 2023-05-05 12:58:20.676539 credmark-1.3.0/credmark/docs/CheckHealthResponse200Details.md
--rw-r--r--   0        0        0      172 2023-05-05 12:58:20.675934 credmark-1.3.0/credmark/docs/CheckHealthResponse200DetailsAdditionalProperty.md
--rw-r--r--   0        0        0       33 2023-05-05 12:58:20.675270 credmark-1.3.0/credmark/docs/CheckHealthResponse200Error.md
--rw-r--r--   0        0        0      170 2023-05-05 12:58:20.674662 credmark-1.3.0/credmark/docs/CheckHealthResponse200ErrorAdditionalProperty.md
--rw-r--r--   0        0        0       76 2023-05-05 12:58:20.674010 credmark-1.3.0/credmark/docs/CheckHealthResponse200Info.md
--rw-r--r--   0        0        0      169 2023-05-05 12:58:20.673413 credmark-1.3.0/credmark/docs/CheckHealthResponse200InfoAdditionalProperty.md
--rw-r--r--   0        0        0      320 2023-05-05 12:58:20.683024 credmark-1.3.0/credmark/docs/CheckHealthResponse503.md
--rw-r--r--   0        0        0      140 2023-05-05 12:58:20.681933 credmark-1.3.0/credmark/docs/CheckHealthResponse503Details.md
--rw-r--r--   0        0        0      172 2023-05-05 12:58:20.681317 credmark-1.3.0/credmark/docs/CheckHealthResponse503DetailsAdditionalProperty.md
--rw-r--r--   0        0        0      108 2023-05-05 12:58:20.680669 credmark-1.3.0/credmark/docs/CheckHealthResponse503Error.md
--rw-r--r--   0        0        0      170 2023-05-05 12:58:20.679966 credmark-1.3.0/credmark/docs/CheckHealthResponse503ErrorAdditionalProperty.md
--rw-r--r--   0        0        0       76 2023-05-05 12:58:20.679223 credmark-1.3.0/credmark/docs/CheckHealthResponse503Info.md
--rw-r--r--   0        0        0      169 2023-05-05 12:58:20.678419 credmark-1.3.0/credmark/docs/CheckHealthResponse503InfoAdditionalProperty.md
--rw-r--r--   0        0        0     2629 2023-05-05 12:58:20.751191 credmark-1.3.0/credmark/docs/DefiApi.md
--rw-r--r--   0        0        0      390 2023-05-05 12:58:20.638588 credmark-1.3.0/credmark/docs/ModelCallStackEntry.md
--rw-r--r--   0        0        0      259 2023-05-05 12:58:20.592875 credmark-1.3.0/credmark/docs/ModelDeployment.md
--rw-r--r--   0        0        0      519 2023-05-05 12:58:20.591849 credmark-1.3.0/credmark/docs/ModelMetadata.md
--rw-r--r--   0        0        0      795 2023-05-05 12:58:20.642466 credmark-1.3.0/credmark/docs/ModelRunResponse.md
--rw-r--r--   0        0        0      637 2023-05-05 12:58:20.640825 credmark-1.3.0/credmark/docs/ModelRunResponseError.md
--rw-r--r--   0        0        0      418 2023-05-05 12:58:20.595290 credmark-1.3.0/credmark/docs/ModelRuntimeStatistics.md
--rw-r--r--   0        0        0      165 2023-05-05 12:58:20.618305 credmark-1.3.0/credmark/docs/ModelRuntimeStatsResponse.md
--rw-r--r--   0        0        0      471 2023-05-05 12:58:20.637545 credmark-1.3.0/credmark/docs/RunModelDto.md
--rw-r--r--   0        0        0      597 2023-05-05 12:58:20.655516 credmark-1.3.0/credmark/docs/TokenAbiResponse.md
--rw-r--r--   0        0        0    20809 2023-05-05 12:58:20.808162 credmark-1.3.0/credmark/docs/TokenApi.md
--rw-r--r--   0        0        0      318 2023-05-05 12:58:20.661673 credmark-1.3.0/credmark/docs/TokenBalanceHistoricalItem.md
--rw-r--r--   0        0        0      646 2023-05-05 12:58:20.663241 credmark-1.3.0/credmark/docs/TokenBalanceHistoricalResponse.md
--rw-r--r--   0        0        0      530 2023-05-05 12:58:20.660767 credmark-1.3.0/credmark/docs/TokenBalanceResponse.md
--rw-r--r--   0        0        0      371 2023-05-05 12:58:20.653813 credmark-1.3.0/credmark/docs/TokenCreationBlockResponse.md
--rw-r--r--   0        0        0      347 2023-05-05 12:58:20.648254 credmark-1.3.0/credmark/docs/TokenDecimalsResponse.md
--rw-r--r--   0        0        0      491 2023-05-05 12:58:20.645100 credmark-1.3.0/credmark/docs/TokenErrorResponse.md
--rw-r--r--   0        0        0      518 2023-05-05 12:58:20.672722 credmark-1.3.0/credmark/docs/TokenHistoricalHoldersCountResponse.md
--rw-r--r--   0        0        0      214 2023-05-05 12:58:20.667973 credmark-1.3.0/credmark/docs/TokenHolder.md
--rw-r--r--   0        0        0      283 2023-05-05 12:58:20.671377 credmark-1.3.0/credmark/docs/TokenHoldersCountHistoricalItem.md
--rw-r--r--   0        0        0      357 2023-05-05 12:58:20.670576 credmark-1.3.0/credmark/docs/TokenHoldersCountResponse.md
--rw-r--r--   0        0        0      613 2023-05-05 12:58:20.669537 credmark-1.3.0/credmark/docs/TokenHoldersResponse.md
--rw-r--r--   0        0        0      341 2023-05-05 12:58:20.652797 credmark-1.3.0/credmark/docs/TokenLogoResponse.md
--rw-r--r--   0        0        0      399 2023-05-05 12:58:20.643671 credmark-1.3.0/credmark/docs/TokenMetadataResponse.md
--rw-r--r--   0        0        0      333 2023-05-05 12:58:20.646118 credmark-1.3.0/credmark/docs/TokenNameResponse.md
--rw-r--r--   0        0        0      379 2023-05-05 12:58:20.657848 credmark-1.3.0/credmark/docs/TokenPriceHistoricalItem.md
--rw-r--r--   0        0        0      582 2023-05-05 12:58:20.659450 credmark-1.3.0/credmark/docs/TokenPriceHistoricalResponse.md
--rw-r--r--   0        0        0      531 2023-05-05 12:58:20.656841 credmark-1.3.0/credmark/docs/TokenPriceResponse.md
--rw-r--r--   0        0        0      339 2023-05-05 12:58:20.647119 credmark-1.3.0/credmark/docs/TokenSymbolResponse.md
--rw-r--r--   0        0        0      284 2023-05-05 12:58:20.650206 credmark-1.3.0/credmark/docs/TokenTotalSupplyHistoricalItem.md
--rw-r--r--   0        0        0      581 2023-05-05 12:58:20.651782 credmark-1.3.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md
--rw-r--r--   0        0        0      423 2023-05-05 12:58:20.649377 credmark-1.3.0/credmark/docs/TokenTotalSupplyResponse.md
--rw-r--r--   0        0        0      404 2023-05-05 12:58:20.665741 credmark-1.3.0/credmark/docs/TokenVolumeHistoricalItem.md
--rw-r--r--   0        0        0      565 2023-05-05 12:58:20.667197 credmark-1.3.0/credmark/docs/TokenVolumeHistoricalResponse.md
--rw-r--r--   0        0        0      537 2023-05-05 12:58:20.664647 credmark-1.3.0/credmark/docs/TokenVolumeResponse.md
--rw-r--r--   0        0        0     1421 2023-05-05 12:58:20.742237 credmark-1.3.0/credmark/docs/Utilities.md
--rw-r--r--   0        0        0      592 2023-05-05 12:58:23.422483 credmark-1.3.0/credmark/errors.py
--rw-r--r--   0        0        0     5318 2023-05-05 12:58:20.687784 credmark-1.3.0/credmark/models/__init__.py
--rw-r--r--   0        0        0     4203 2023-05-05 12:58:23.559507 credmark-1.3.0/credmark/models/check_health_response_200.py
--rw-r--r--   0        0        0     2144 2023-05-05 12:58:23.505245 credmark-1.3.0/credmark/models/check_health_response_200_details.py
--rw-r--r--   0        0        0     1658 2023-05-05 12:58:23.499383 credmark-1.3.0/credmark/models/check_health_response_200_details_additional_property.py
--rw-r--r--   0        0        0     2061 2023-05-05 12:58:23.517069 credmark-1.3.0/credmark/models/check_health_response_200_error.py
--rw-r--r--   0        0        0     1648 2023-05-05 12:58:23.544210 credmark-1.3.0/credmark/models/check_health_response_200_error_additional_property.py
--rw-r--r--   0        0        0     2074 2023-05-05 12:58:23.537806 credmark-1.3.0/credmark/models/check_health_response_200_info.py
--rw-r--r--   0        0        0     1643 2023-05-05 12:58:23.542897 credmark-1.3.0/credmark/models/check_health_response_200_info_additional_property.py
--rw-r--r--   0        0        0     4364 2023-05-05 12:58:23.609660 credmark-1.3.0/credmark/models/check_health_response_503.py
--rw-r--r--   0        0        0     2205 2023-05-05 12:58:23.556933 credmark-1.3.0/credmark/models/check_health_response_503_details.py
--rw-r--r--   0        0        0     1658 2023-05-05 12:58:23.551649 credmark-1.3.0/credmark/models/check_health_response_503_details_additional_property.py
--rw-r--r--   0        0        0     2149 2023-05-05 12:58:23.567359 credmark-1.3.0/credmark/models/check_health_response_503_error.py
--rw-r--r--   0        0        0     1648 2023-05-05 12:58:23.561995 credmark-1.3.0/credmark/models/check_health_response_503_error_additional_property.py
--rw-r--r--   0        0        0     2074 2023-05-05 12:58:23.566967 credmark-1.3.0/credmark/models/check_health_response_503_info.py
--rw-r--r--   0        0        0     1643 2023-05-05 12:58:23.569688 credmark-1.3.0/credmark/models/check_health_response_503_info_additional_property.py
--rw-r--r--   0        0        0      165 2023-05-05 12:58:21.830432 credmark-1.3.0/credmark/models/get_cached_model_results_order.py
--rw-r--r--   0        0        0      163 2023-05-05 12:58:21.768992 credmark-1.3.0/credmark/models/get_token_price_historical_src.py
--rw-r--r--   0        0        0      153 2023-05-05 12:58:21.833451 credmark-1.3.0/credmark/models/get_token_price_src.py
--rw-r--r--   0        0        0     2470 2023-05-05 12:58:23.617959 credmark-1.3.0/credmark/models/model_call_stack_entry.py
--rw-r--r--   0        0        0     1894 2023-05-05 12:58:23.591293 credmark-1.3.0/credmark/models/model_deployment.py
--rw-r--r--   0        0        0     3325 2023-05-05 12:58:23.636706 credmark-1.3.0/credmark/models/model_metadata.py
--rw-r--r--   0        0        0     4460 2023-05-05 12:58:23.657788 credmark-1.3.0/credmark/models/model_run_response.py
--rw-r--r--   0        0        0     3362 2023-05-05 12:58:23.637117 credmark-1.3.0/credmark/models/model_run_response_error.py
--rw-r--r--   0        0        0     2412 2023-05-05 12:58:23.636927 credmark-1.3.0/credmark/models/model_runtime_statistics.py
--rw-r--r--   0        0        0     2042 2023-05-05 12:58:23.620457 credmark-1.3.0/credmark/models/model_runtime_stats_response.py
--rw-r--r--   0        0        0     3280 2023-05-05 12:58:23.655632 credmark-1.3.0/credmark/models/run_model_dto.py
--rw-r--r--   0        0        0      180 2023-05-05 12:58:21.788363 credmark-1.3.0/credmark/models/run_model_dto_block_number_type_1.py
--rw-r--r--   0        0        0     5771 2023-05-05 12:58:23.653858 credmark-1.3.0/credmark/models/token_abi_response.py
--rw-r--r--   0        0        0     2319 2023-05-05 12:58:23.634433 credmark-1.3.0/credmark/models/token_balance_historical_item.py
--rw-r--r--   0        0        0     4365 2023-05-05 12:58:23.684860 credmark-1.3.0/credmark/models/token_balance_historical_response.py
--rw-r--r--   0        0        0     3378 2023-05-05 12:58:23.681623 credmark-1.3.0/credmark/models/token_balance_response.py
--rw-r--r--   0        0        0     2692 2023-05-05 12:58:23.673028 credmark-1.3.0/credmark/models/token_creation_block_response.py
--rw-r--r--   0        0        0     2587 2023-05-05 12:58:23.680658 credmark-1.3.0/credmark/models/token_decimals_response.py
--rw-r--r--   0        0        0     2779 2023-05-05 12:58:23.695458 credmark-1.3.0/credmark/models/token_error_response.py
--rw-r--r--   0        0        0     3856 2023-05-05 12:58:23.705892 credmark-1.3.0/credmark/models/token_historical_holders_count_response.py
--rw-r--r--   0        0        0     1836 2023-05-05 12:58:23.681752 credmark-1.3.0/credmark/models/token_holder.py
--rw-r--r--   0        0        0     2104 2023-05-05 12:58:23.681485 credmark-1.3.0/credmark/models/token_holders_count_historical_item.py
--rw-r--r--   0        0        0     2589 2023-05-05 12:58:23.711832 credmark-1.3.0/credmark/models/token_holders_count_response.py
--rw-r--r--   0        0        0     4074 2023-05-05 12:58:23.736104 credmark-1.3.0/credmark/models/token_holders_response.py
--rw-r--r--   0        0        0     2711 2023-05-05 12:58:23.711254 credmark-1.3.0/credmark/models/token_logo_response.py
--rw-r--r--   0        0        0     2951 2023-05-05 12:58:23.737078 credmark-1.3.0/credmark/models/token_metadata_response.py
--rw-r--r--   0        0        0     2527 2023-05-05 12:58:23.733880 credmark-1.3.0/credmark/models/token_name_response.py
--rw-r--r--   0        0        0     2551 2023-05-05 12:58:23.738444 credmark-1.3.0/credmark/models/token_price_historical_item.py
--rw-r--r--   0        0        0     4118 2023-05-05 12:58:23.756842 credmark-1.3.0/credmark/models/token_price_historical_response.py
--rw-r--r--   0        0        0     3387 2023-05-05 12:58:23.746549 credmark-1.3.0/credmark/models/token_price_response.py
--rw-r--r--   0        0        0     2553 2023-05-05 12:58:23.742689 credmark-1.3.0/credmark/models/token_symbol_response.py
--rw-r--r--   0        0        0     2168 2023-05-05 12:58:23.743722 credmark-1.3.0/credmark/models/token_total_supply_historical_item.py
--rw-r--r--   0        0        0     4072 2023-05-05 12:58:23.769114 credmark-1.3.0/credmark/models/token_total_supply_historical_response.py
--rw-r--r--   0        0        0     2881 2023-05-05 12:58:23.759899 credmark-1.3.0/credmark/models/token_total_supply_response.py
--rw-r--r--   0        0        0     2758 2023-05-05 12:58:23.759863 credmark-1.3.0/credmark/models/token_volume_historical_item.py
--rw-r--r--   0        0        0     4001 2023-05-05 12:58:23.783603 credmark-1.3.0/credmark/models/token_volume_historical_response.py
--rw-r--r--   0        0        0     3465 2023-05-05 12:58:23.778417 credmark-1.3.0/credmark/models/token_volume_response.py
--rw-r--r--   0        0        0       25 2023-05-05 12:58:20.546306 credmark-1.3.0/credmark/py.typed
--rw-r--r--   0        0        0      964 2023-05-05 12:58:23.757166 credmark-1.3.0/credmark/types.py
--rw-r--r--   0        0        0      853 2023-05-05 13:03:00.626630 credmark-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5384 1970-01-01 00:00:00.000000 credmark-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5667 2023-06-27 02:31:33.985643 credmark-1.4.0/README.md
+-rw-r--r--   0        0        0      110 2023-06-27 02:20:04.339659 credmark-1.4.0/credmark/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-27 02:20:02.500389 credmark-1.4.0/credmark/api/__init__.py
+-rw-r--r--   0        0        0     9643 2023-06-27 02:20:04.450405 credmark-1.4.0/credmark/api/defi_api/__init__.py
+-rw-r--r--   0        0        0     8159 2023-06-27 02:20:04.506067 credmark-1.4.0/credmark/api/defi_api/get_cached_model_results.py
+-rw-r--r--   0        0        0     3679 2023-06-27 02:20:04.423334 credmark-1.4.0/credmark/api/defi_api/get_model_by_slug.py
+-rw-r--r--   0        0        0     4016 2023-06-27 02:20:04.437059 credmark-1.4.0/credmark/api/defi_api/get_model_deployments_by_slug.py
+-rw-r--r--   0        0        0     3513 2023-06-27 02:20:04.424356 credmark-1.4.0/credmark/api/defi_api/get_model_runtime_stats.py
+-rw-r--r--   0        0        0     3725 2023-06-27 02:20:04.445982 credmark-1.4.0/credmark/api/defi_api/list_models.py
+-rw-r--r--   0        0        0     3912 2023-06-27 02:20:04.446360 credmark-1.4.0/credmark/api/defi_api/run_model.py
+-rw-r--r--   0        0        0    24046 2023-06-27 02:20:04.649987 credmark-1.4.0/credmark/api/portfolio_api/__init__.py
+-rw-r--r--   0        0        0     8817 2023-06-27 02:20:04.526955 credmark-1.4.0/credmark/api/portfolio_api/get_positions.py
+-rw-r--r--   0        0        0    13500 2023-06-27 02:20:04.618156 credmark-1.4.0/credmark/api/portfolio_api/get_positions_historical.py
+-rw-r--r--   0        0        0     8815 2023-06-27 02:20:04.538096 credmark-1.4.0/credmark/api/portfolio_api/get_returns.py
+-rw-r--r--   0        0        0    11130 2023-06-27 02:20:04.600846 credmark-1.4.0/credmark/api/portfolio_api/get_value.py
+-rw-r--r--   0        0        0    15801 2023-06-27 02:20:04.692637 credmark-1.4.0/credmark/api/portfolio_api/get_value_historical.py
+-rw-r--r--   0        0        0    79472 2023-06-27 02:20:05.221430 credmark-1.4.0/credmark/api/token_api/__init__.py
+-rw-r--r--   0        0        0     7328 2023-06-27 02:20:04.586508 credmark-1.4.0/credmark/api/token_api/get_token_abi.py
+-rw-r--r--   0        0        0    11298 2023-06-27 02:20:04.645089 credmark-1.4.0/credmark/api/token_api/get_token_balance.py
+-rw-r--r--   0        0        0    15309 2023-06-27 02:20:04.698932 credmark-1.4.0/credmark/api/token_api/get_token_balance_historical.py
+-rw-r--r--   0        0        0     8410 2023-06-27 02:20:04.598554 credmark-1.4.0/credmark/api/token_api/get_token_creation_block.py
+-rw-r--r--   0        0        0     8274 2023-06-27 02:20:04.684562 credmark-1.4.0/credmark/api/token_api/get_token_decimals.py
+-rw-r--r--   0        0        0    11822 2023-06-27 02:20:04.747749 credmark-1.4.0/credmark/api/token_api/get_token_holders.py
+-rw-r--r--   0        0        0     7940 2023-06-27 02:20:04.706940 credmark-1.4.0/credmark/api/token_api/get_token_holders_count.py
+-rw-r--r--   0        0        0    12559 2023-06-27 02:20:04.822957 credmark-1.4.0/credmark/api/token_api/get_token_holders_count_historical.py
+-rw-r--r--   0        0        0     8170 2023-06-27 02:20:04.772196 credmark-1.4.0/credmark/api/token_api/get_token_logo.py
+-rw-r--r--   0        0        0     8255 2023-06-27 02:20:04.740574 credmark-1.4.0/credmark/api/token_api/get_token_metadata.py
+-rw-r--r--   0        0        0     8170 2023-06-27 02:20:04.765249 credmark-1.4.0/credmark/api/token_api/get_token_name.py
+-rw-r--r--   0        0        0    11243 2023-06-27 02:20:04.859749 credmark-1.4.0/credmark/api/token_api/get_token_price.py
+-rw-r--r--   0        0        0    16235 2023-06-27 02:20:04.946692 credmark-1.4.0/credmark/api/token_api/get_token_price_historical.py
+-rw-r--r--   0        0        0     8222 2023-06-27 02:20:04.851252 credmark-1.4.0/credmark/api/token_api/get_token_symbol.py
+-rw-r--r--   0        0        0     9238 2023-06-27 02:20:04.894617 credmark-1.4.0/credmark/api/token_api/get_token_total_supply.py
+-rw-r--r--   0        0        0    13225 2023-06-27 02:20:04.965237 credmark-1.4.0/credmark/api/token_api/get_token_total_supply_historical.py
+-rw-r--r--   0        0        0    11276 2023-06-27 02:20:04.947612 credmark-1.4.0/credmark/api/token_api/get_token_volume.py
+-rw-r--r--   0        0        0    13437 2023-06-27 02:20:05.004814 credmark-1.4.0/credmark/api/token_api/get_token_volume_historical.py
+-rw-r--r--   0        0        0     5822 2023-06-27 02:20:04.878383 credmark-1.4.0/credmark/api/utilities/__init__.py
+-rw-r--r--   0        0        0     3575 2023-06-27 02:20:04.900296 credmark-1.4.0/credmark/api/utilities/check_health.py
+-rw-r--r--   0        0        0     6512 2023-06-27 02:20:04.936784 credmark-1.4.0/credmark/api/utilities/get_daily_model_usage.py
+-rw-r--r--   0        0        0     3373 2023-06-27 02:20:04.931488 credmark-1.4.0/credmark/api/utilities/get_top_models.py
+-rw-r--r--   0        0        0     3351 2023-06-27 02:20:04.951836 credmark-1.4.0/credmark/api/utilities/get_total_model_usage.py
+-rw-r--r--   0        0        0     2744 2023-06-27 02:20:04.938688 credmark-1.4.0/credmark/client.py
+-rw-r--r--   0        0        0      320 2023-06-27 02:20:02.485834 credmark-1.4.0/credmark/docs/CheckHealthResponse200.md
+-rw-r--r--   0        0        0       79 2023-06-27 02:20:02.484789 credmark-1.4.0/credmark/docs/CheckHealthResponse200Details.md
+-rw-r--r--   0        0        0      172 2023-06-27 02:20:02.484187 credmark-1.4.0/credmark/docs/CheckHealthResponse200DetailsAdditionalProperty.md
+-rw-r--r--   0        0        0       33 2023-06-27 02:20:02.483492 credmark-1.4.0/credmark/docs/CheckHealthResponse200Error.md
+-rw-r--r--   0        0        0      170 2023-06-27 02:20:02.482908 credmark-1.4.0/credmark/docs/CheckHealthResponse200ErrorAdditionalProperty.md
+-rw-r--r--   0        0        0       76 2023-06-27 02:20:02.482108 credmark-1.4.0/credmark/docs/CheckHealthResponse200Info.md
+-rw-r--r--   0        0        0      169 2023-06-27 02:20:02.481435 credmark-1.4.0/credmark/docs/CheckHealthResponse200InfoAdditionalProperty.md
+-rw-r--r--   0        0        0      320 2023-06-27 02:20:02.490781 credmark-1.4.0/credmark/docs/CheckHealthResponse503.md
+-rw-r--r--   0        0        0      140 2023-06-27 02:20:02.489717 credmark-1.4.0/credmark/docs/CheckHealthResponse503Details.md
+-rw-r--r--   0        0        0      172 2023-06-27 02:20:02.489069 credmark-1.4.0/credmark/docs/CheckHealthResponse503DetailsAdditionalProperty.md
+-rw-r--r--   0        0        0      108 2023-06-27 02:20:02.488376 credmark-1.4.0/credmark/docs/CheckHealthResponse503Error.md
+-rw-r--r--   0        0        0      170 2023-06-27 02:20:02.487753 credmark-1.4.0/credmark/docs/CheckHealthResponse503ErrorAdditionalProperty.md
+-rw-r--r--   0        0        0       76 2023-06-27 02:20:02.487098 credmark-1.4.0/credmark/docs/CheckHealthResponse503Info.md
+-rw-r--r--   0        0        0      169 2023-06-27 02:20:02.486493 credmark-1.4.0/credmark/docs/CheckHealthResponse503InfoAdditionalProperty.md
+-rw-r--r--   0        0        0     2629 2023-06-27 02:20:02.561635 credmark-1.4.0/credmark/docs/DefiApi.md
+-rw-r--r--   0        0        0      390 2023-06-27 02:20:02.431544 credmark-1.4.0/credmark/docs/ModelCallStackEntry.md
+-rw-r--r--   0        0        0      259 2023-06-27 02:20:02.397600 credmark-1.4.0/credmark/docs/ModelDeployment.md
+-rw-r--r--   0        0        0      991 2023-06-27 02:20:02.396800 credmark-1.4.0/credmark/docs/ModelMetadata.md
+-rw-r--r--   0        0        0      795 2023-06-27 02:20:02.435648 credmark-1.4.0/credmark/docs/ModelRunResponse.md
+-rw-r--r--   0        0        0      637 2023-06-27 02:20:02.434000 credmark-1.4.0/credmark/docs/ModelRunResponseError.md
+-rw-r--r--   0        0        0      418 2023-06-27 02:20:02.399511 credmark-1.4.0/credmark/docs/ModelRuntimeStatistics.md
+-rw-r--r--   0        0        0      165 2023-06-27 02:20:02.410430 credmark-1.4.0/credmark/docs/ModelRuntimeStatsResponse.md
+-rw-r--r--   0        0        0     6354 2023-06-27 02:20:02.640905 credmark-1.4.0/credmark/docs/PortfolioApi.md
+-rw-r--r--   0        0        0      495 2023-06-27 02:20:02.470160 credmark-1.4.0/credmark/docs/PortfolioErrorResponse.md
+-rw-r--r--   0        0        0      192 2023-06-27 02:20:02.467357 credmark-1.4.0/credmark/docs/Position.md
+-rw-r--r--   0        0        0      270 2023-06-27 02:20:02.471093 credmark-1.4.0/credmark/docs/PositionHistoricalItem.md
+-rw-r--r--   0        0        0      491 2023-06-27 02:20:02.472670 credmark-1.4.0/credmark/docs/PositionsHistoricalResponse.md
+-rw-r--r--   0        0        0      335 2023-06-27 02:20:02.468694 credmark-1.4.0/credmark/docs/PositionsResponse.md
+-rw-r--r--   0        0        0      465 2023-06-27 02:20:02.480694 credmark-1.4.0/credmark/docs/ReturnsResponse.md
+-rw-r--r--   0        0        0      467 2023-06-27 02:20:02.430459 credmark-1.4.0/credmark/docs/RunModelDto.md
+-rw-r--r--   0        0        0      597 2023-06-27 02:20:02.448628 credmark-1.4.0/credmark/docs/TokenAbiResponse.md
+-rw-r--r--   0        0        0    20809 2023-06-27 02:20:02.621803 credmark-1.4.0/credmark/docs/TokenApi.md
+-rw-r--r--   0        0        0      318 2023-06-27 02:20:02.454900 credmark-1.4.0/credmark/docs/TokenBalanceHistoricalItem.md
+-rw-r--r--   0        0        0      646 2023-06-27 02:20:02.456488 credmark-1.4.0/credmark/docs/TokenBalanceHistoricalResponse.md
+-rw-r--r--   0        0        0      530 2023-06-27 02:20:02.454014 credmark-1.4.0/credmark/docs/TokenBalanceResponse.md
+-rw-r--r--   0        0        0      371 2023-06-27 02:20:02.446836 credmark-1.4.0/credmark/docs/TokenCreationBlockResponse.md
+-rw-r--r--   0        0        0      347 2023-06-27 02:20:02.441324 credmark-1.4.0/credmark/docs/TokenDecimalsResponse.md
+-rw-r--r--   0        0        0      491 2023-06-27 02:20:02.438203 credmark-1.4.0/credmark/docs/TokenErrorResponse.md
+-rw-r--r--   0        0        0      518 2023-06-27 02:20:02.466660 credmark-1.4.0/credmark/docs/TokenHistoricalHoldersCountResponse.md
+-rw-r--r--   0        0        0      214 2023-06-27 02:20:02.461631 credmark-1.4.0/credmark/docs/TokenHolder.md
+-rw-r--r--   0        0        0      283 2023-06-27 02:20:02.465131 credmark-1.4.0/credmark/docs/TokenHoldersCountHistoricalItem.md
+-rw-r--r--   0        0        0      357 2023-06-27 02:20:02.464281 credmark-1.4.0/credmark/docs/TokenHoldersCountResponse.md
+-rw-r--r--   0        0        0      613 2023-06-27 02:20:02.463275 credmark-1.4.0/credmark/docs/TokenHoldersResponse.md
+-rw-r--r--   0        0        0      341 2023-06-27 02:20:02.445826 credmark-1.4.0/credmark/docs/TokenLogoResponse.md
+-rw-r--r--   0        0        0      399 2023-06-27 02:20:02.436842 credmark-1.4.0/credmark/docs/TokenMetadataResponse.md
+-rw-r--r--   0        0        0      333 2023-06-27 02:20:02.439194 credmark-1.4.0/credmark/docs/TokenNameResponse.md
+-rw-r--r--   0        0        0      379 2023-06-27 02:20:02.451130 credmark-1.4.0/credmark/docs/TokenPriceHistoricalItem.md
+-rw-r--r--   0        0        0      582 2023-06-27 02:20:02.452694 credmark-1.4.0/credmark/docs/TokenPriceHistoricalResponse.md
+-rw-r--r--   0        0        0      531 2023-06-27 02:20:02.450131 credmark-1.4.0/credmark/docs/TokenPriceResponse.md
+-rw-r--r--   0        0        0      319 2023-06-27 02:20:02.479046 credmark-1.4.0/credmark/docs/TokenReturn.md
+-rw-r--r--   0        0        0      339 2023-06-27 02:20:02.440298 credmark-1.4.0/credmark/docs/TokenSymbolResponse.md
+-rw-r--r--   0        0        0      284 2023-06-27 02:20:02.443294 credmark-1.4.0/credmark/docs/TokenTotalSupplyHistoricalItem.md
+-rw-r--r--   0        0        0      581 2023-06-27 02:20:02.444819 credmark-1.4.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md
+-rw-r--r--   0        0        0      423 2023-06-27 02:20:02.442437 credmark-1.4.0/credmark/docs/TokenTotalSupplyResponse.md
+-rw-r--r--   0        0        0      296 2023-06-27 02:20:02.473610 credmark-1.4.0/credmark/docs/TokenValue.md
+-rw-r--r--   0        0        0      404 2023-06-27 02:20:02.459184 credmark-1.4.0/credmark/docs/TokenVolumeHistoricalItem.md
+-rw-r--r--   0        0        0      565 2023-06-27 02:20:02.460815 credmark-1.4.0/credmark/docs/TokenVolumeHistoricalResponse.md
+-rw-r--r--   0        0        0      537 2023-06-27 02:20:02.457776 credmark-1.4.0/credmark/docs/TokenVolumeResponse.md
+-rw-r--r--   0        0        0     1421 2023-06-27 02:20:02.551577 credmark-1.4.0/credmark/docs/Utilities.md
+-rw-r--r--   0        0        0      321 2023-06-27 02:20:02.476224 credmark-1.4.0/credmark/docs/ValueHistoricalItem.md
+-rw-r--r--   0        0        0      562 2023-06-27 02:20:02.478065 credmark-1.4.0/credmark/docs/ValueHistoricalResponse.md
+-rw-r--r--   0        0        0      463 2023-06-27 02:20:02.475098 credmark-1.4.0/credmark/docs/ValueResponse.md
+-rw-r--r--   0        0        0      592 2023-06-27 02:20:04.898970 credmark-1.4.0/credmark/errors.py
+-rw-r--r--   0        0        0     6147 2023-06-27 02:20:02.496667 credmark-1.4.0/credmark/models/__init__.py
+-rw-r--r--   0        0        0     3507 2023-06-27 02:20:04.999705 credmark-1.4.0/credmark/models/check_health_response_200.py
+-rw-r--r--   0        0        0     2144 2023-06-27 02:20:04.961118 credmark-1.4.0/credmark/models/check_health_response_200_details.py
+-rw-r--r--   0        0        0     1658 2023-06-27 02:20:04.974984 credmark-1.4.0/credmark/models/check_health_response_200_details_additional_property.py
+-rw-r--r--   0        0        0     2061 2023-06-27 02:20:04.987038 credmark-1.4.0/credmark/models/check_health_response_200_error.py
+-rw-r--r--   0        0        0     1648 2023-06-27 02:20:04.988762 credmark-1.4.0/credmark/models/check_health_response_200_error_additional_property.py
+-rw-r--r--   0        0        0     2074 2023-06-27 02:20:04.990141 credmark-1.4.0/credmark/models/check_health_response_200_info.py
+-rw-r--r--   0        0        0     1643 2023-06-27 02:20:04.994077 credmark-1.4.0/credmark/models/check_health_response_200_info_additional_property.py
+-rw-r--r--   0        0        0     3668 2023-06-27 02:20:05.040458 credmark-1.4.0/credmark/models/check_health_response_503.py
+-rw-r--r--   0        0        0     2205 2023-06-27 02:20:05.003562 credmark-1.4.0/credmark/models/check_health_response_503_details.py
+-rw-r--r--   0        0        0     1658 2023-06-27 02:20:05.008657 credmark-1.4.0/credmark/models/check_health_response_503_details_additional_property.py
+-rw-r--r--   0        0        0     2149 2023-06-27 02:20:05.018002 credmark-1.4.0/credmark/models/check_health_response_503_error.py
+-rw-r--r--   0        0        0     1648 2023-06-27 02:20:05.030653 credmark-1.4.0/credmark/models/check_health_response_503_error_additional_property.py
+-rw-r--r--   0        0        0     2074 2023-06-27 02:20:05.045240 credmark-1.4.0/credmark/models/check_health_response_503_info.py
+-rw-r--r--   0        0        0     1643 2023-06-27 02:20:05.044907 credmark-1.4.0/credmark/models/check_health_response_503_info_additional_property.py
+-rw-r--r--   0        0        0      165 2023-06-27 02:20:03.632689 credmark-1.4.0/credmark/models/get_cached_model_results_order.py
+-rw-r--r--   0        0        0      163 2023-06-27 02:20:03.554528 credmark-1.4.0/credmark/models/get_token_price_historical_src.py
+-rw-r--r--   0        0        0      153 2023-06-27 02:20:03.635634 credmark-1.4.0/credmark/models/get_token_price_src.py
+-rw-r--r--   0        0        0     1777 2023-06-27 02:20:05.047009 credmark-1.4.0/credmark/models/model_call_stack_entry.py
+-rw-r--r--   0        0        0     1207 2023-06-27 02:20:05.033756 credmark-1.4.0/credmark/models/model_deployment.py
+-rw-r--r--   0        0        0     4961 2023-06-27 02:20:05.117396 credmark-1.4.0/credmark/models/model_metadata.py
+-rw-r--r--   0        0        0     3771 2023-06-27 02:20:05.087099 credmark-1.4.0/credmark/models/model_run_response.py
+-rw-r--r--   0        0        0     2673 2023-06-27 02:20:05.064191 credmark-1.4.0/credmark/models/model_run_response_error.py
+-rw-r--r--   0        0        0     1717 2023-06-27 02:20:05.059152 credmark-1.4.0/credmark/models/model_runtime_statistics.py
+-rw-r--r--   0        0        0     1349 2023-06-27 02:20:05.051106 credmark-1.4.0/credmark/models/model_runtime_stats_response.py
+-rw-r--r--   0        0        0     2112 2023-06-27 02:20:05.076224 credmark-1.4.0/credmark/models/portfolio_error_response.py
+-rw-r--r--   0        0        0     1056 2023-06-27 02:20:05.059880 credmark-1.4.0/credmark/models/position.py
+-rw-r--r--   0        0        0     1845 2023-06-27 02:20:05.081699 credmark-1.4.0/credmark/models/position_historical_item.py
+-rw-r--r--   0        0        0     3030 2023-06-27 02:20:05.102377 credmark-1.4.0/credmark/models/positions_historical_response.py
+-rw-r--r--   0        0        0     2322 2023-06-27 02:20:05.093405 credmark-1.4.0/credmark/models/positions_response.py
+-rw-r--r--   0        0        0     2898 2023-06-27 02:20:05.106941 credmark-1.4.0/credmark/models/returns_response.py
+-rw-r--r--   0        0        0     2592 2023-06-27 02:20:05.108887 credmark-1.4.0/credmark/models/run_model_dto.py
+-rw-r--r--   0        0        0      180 2023-06-27 02:20:03.581984 credmark-1.4.0/credmark/models/run_model_dto_block_number_type_1.py
+-rw-r--r--   0        0        0     5088 2023-06-27 02:20:05.110667 credmark-1.4.0/credmark/models/token_abi_response.py
+-rw-r--r--   0        0        0     1619 2023-06-27 02:20:05.093996 credmark-1.4.0/credmark/models/token_balance_historical_item.py
+-rw-r--r--   0        0        0     3667 2023-06-27 02:20:05.129382 credmark-1.4.0/credmark/models/token_balance_historical_response.py
+-rw-r--r--   0        0        0     2685 2023-06-27 02:20:05.123293 credmark-1.4.0/credmark/models/token_balance_response.py
+-rw-r--r--   0        0        0     1992 2023-06-27 02:20:05.121544 credmark-1.4.0/credmark/models/token_creation_block_response.py
+-rw-r--r--   0        0        0     1893 2023-06-27 02:20:05.123297 credmark-1.4.0/credmark/models/token_decimals_response.py
+-rw-r--r--   0        0        0     2094 2023-06-27 02:20:05.138893 credmark-1.4.0/credmark/models/token_error_response.py
+-rw-r--r--   0        0        0     3152 2023-06-27 02:20:05.149991 credmark-1.4.0/credmark/models/token_historical_holders_count_response.py
+-rw-r--r--   0        0        0     1153 2023-06-27 02:20:05.134057 credmark-1.4.0/credmark/models/token_holder.py
+-rw-r--r--   0        0        0     1398 2023-06-27 02:20:05.135781 credmark-1.4.0/credmark/models/token_holders_count_historical_item.py
+-rw-r--r--   0        0        0     1890 2023-06-27 02:20:05.143441 credmark-1.4.0/credmark/models/token_holders_count_response.py
+-rw-r--r--   0        0        0     3387 2023-06-27 02:20:05.179625 credmark-1.4.0/credmark/models/token_holders_response.py
+-rw-r--r--   0        0        0     2021 2023-06-27 02:20:05.154151 credmark-1.4.0/credmark/models/token_logo_response.py
+-rw-r--r--   0        0        0     2257 2023-06-27 02:20:05.168842 credmark-1.4.0/credmark/models/token_metadata_response.py
+-rw-r--r--   0        0        0     1837 2023-06-27 02:20:05.162742 credmark-1.4.0/credmark/models/token_name_response.py
+-rw-r--r--   0        0        0     1853 2023-06-27 02:20:05.163005 credmark-1.4.0/credmark/models/token_price_historical_item.py
+-rw-r--r--   0        0        0     3422 2023-06-27 02:20:05.191360 credmark-1.4.0/credmark/models/token_price_historical_response.py
+-rw-r--r--   0        0        0     2696 2023-06-27 02:20:05.184668 credmark-1.4.0/credmark/models/token_price_response.py
+-rw-r--r--   0        0        0     1537 2023-06-27 02:20:05.170697 credmark-1.4.0/credmark/models/token_return.py
+-rw-r--r--   0        0        0     1861 2023-06-27 02:20:05.177817 credmark-1.4.0/credmark/models/token_symbol_response.py
+-rw-r--r--   0        0        0     1463 2023-06-27 02:20:05.178289 credmark-1.4.0/credmark/models/token_total_supply_historical_item.py
+-rw-r--r--   0        0        0     3369 2023-06-27 02:20:05.217718 credmark-1.4.0/credmark/models/token_total_supply_historical_response.py
+-rw-r--r--   0        0        0     2183 2023-06-27 02:20:05.198446 credmark-1.4.0/credmark/models/token_total_supply_response.py
+-rw-r--r--   0        0        0     1558 2023-06-27 02:20:05.204644 credmark-1.4.0/credmark/models/token_value.py
+-rw-r--r--   0        0        0     2059 2023-06-27 02:20:05.203952 credmark-1.4.0/credmark/models/token_volume_historical_item.py
+-rw-r--r--   0        0        0     3304 2023-06-27 02:20:05.227369 credmark-1.4.0/credmark/models/token_volume_historical_response.py
+-rw-r--r--   0        0        0     2773 2023-06-27 02:20:05.221134 credmark-1.4.0/credmark/models/token_volume_response.py
+-rw-r--r--   0        0        0     2070 2023-06-27 02:20:05.220435 credmark-1.4.0/credmark/models/value_historical_item.py
+-rw-r--r--   0        0        0     3344 2023-06-27 02:20:05.232636 credmark-1.4.0/credmark/models/value_historical_response.py
+-rw-r--r--   0        0        0     2894 2023-06-27 02:20:05.229673 credmark-1.4.0/credmark/models/value_response.py
+-rw-r--r--   0        0        0       25 2023-06-27 02:20:02.356524 credmark-1.4.0/credmark/py.typed
+-rw-r--r--   0        0        0      964 2023-06-27 02:20:05.211284 credmark-1.4.0/credmark/types.py
+-rw-r--r--   0        0        0      853 2023-06-26 12:42:42.671649 credmark-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6549 1970-01-01 00:00:00.000000 credmark-1.4.0/PKG-INFO
```

### Comparing `credmark-1.3.0/README.md` & `credmark-1.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -34,54 +34,83 @@
 
 Now call your endpoint by tag and use your models:
 
 ```python
 metadata = client.token_api.get_token_metadata(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9")
 
 print(metadata)
-# TokenMetadataResponse(chain_id=1, block_number=17044112, block_timestamp=1681459199, token_address='0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9', name='Aave Token', symbol='AAVE', decimals=18, additional_properties={})
+# TokenMetadataResponse(chain_id=1, block_number=17044112, block_timestamp=1681459199, token_address='0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9', name='Aave Token', symbol='AAVE', decimals=18)
 ```
 
 Or do the same thing with an async version:
 
 ```python
 import asyncio
 
 async def get_metadata():
     metadata = await client.token_api.get_token_metadata_async(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9")
     print(metadata)
-    # TokenMetadataResponse(chain_id=1, block_number=17044112, block_timestamp=1681459199, token_address='0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9', name='Aave Token', symbol='AAVE', decimals=18, additional_properties={})
+    # TokenMetadataResponse(chain_id=1, block_number=17044112, block_timestamp=1681459199, token_address='0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9', name='Aave Token', symbol='AAVE', decimals=18)
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(get_metadata())
 loop.close()
 ```
 
-## Run a model
+## Examples
 
-You can run a model using DeFi API:
+### 1. DeFi API - Run models
+
+Get all Uniswap V3 pools for USDC on Ethereum Mainnet:
 
 ```python
 from credmark.models import RunModelDto
 
 result = client.defi_api.run_model(
     json_body=RunModelDto(
         chain_id=1, 
         block_number="latest", 
-        slug="price.quote", 
-        input={"base": {"symbol": "AAVE"}, "prefer": "dex"}
+        slug="uniswap-v3.get-pools", 
+        input={"symbol": "USDC"}
     ),
 )
 
 print(result.chain_id, result.block_number)
-# 1 17044112
+# 1 17563869
 print(result.slug, result.version)
-# price.quote 1.11
+# uniswap-v3.get-pools 0.1
 print(result.output)
-# {'src': 'dex|uniswap-v2,sushiswap,uniswap-v3|Non-zero:9|Zero:2|4.0', 'price': 82.19716419870656, 'quoteAddress': '0x0000000000000000000000000000000000000348'}
+# {'contracts': [{'address': '0x5777d92f208679db4b9778590fa3cab3ac9e2168'}, {'address': '0x6c6bc977e13df9b0de53b251522280bb72383700'}, {'address': '0xa63b490aa077f541c9d64bfc1cc0db2a752157b5'}, {'address': '0x6958686b6348c3d6d5f2dca3106a5c09c156873a'}, {'address': '0x3416cf6c708da44db2624d63ea0aaef7113527c6'}, {'address': '0x7858e59e0c01ea06df3af3d20ac7b0003275d4bf'}, {'address': '0xee4cf3b78a74affa38c6a926282bcd8b5952818d'}, {'address': '0xbb256c2f1b677e27118b0345fd2b3894d2e6d487'}]}
+```
+
+### 2. Portfolio API
+
+Get all positions, i.e. tokens and balances for a wallet
+
+```python
+result = client.portfolio_api.get_positions(1, ["0x5291fBB0ee9F51225f0928Ff6a83108c86327636"])
+
+print(result.chain_id, result.block_number)
+# 1 17567721
+print(result.positions)
+# [Position(token_address='0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48', balance=2.169356), Position(token_address='0xdac17f958d2ee523a2206206994597c13d831ec7', balance=479.354369)]
+```
+
+### 3. Token API
+
+Get price of AAVE token (0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9)
+
+```python
+result = client.token_api.get_token_price(1, "0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9")
+
+print(result.chain_id, result.block_number)
+# 1 17567740
+print(result.price, result.src, result.quote_address)
+# 64.599481 cex 0x0000000000000000000000000000000000000348
+# 0x0000000000000000000000000000000000000348 => USD address
 ```
 
 ## Handling Errors
 
 Each method can raise:
 
 - errors.CredmarkError: If the server returns a non 2xx status code.
@@ -93,15 +122,15 @@
 
 try:
     metadata = client.token_api.get_token_metadata(1, "WRONG TOKEN ADDRESS")
 except CredmarkError as e:
     print(e.status_code)
     # 400
     print(e.parsed)
-    # TokenErrorResponse(status_code=400, error='Bad Request', message=['Invalid token address'], additional_properties={})
+    # TokenErrorResponse(status_code=400, error='Bad Request', message=['Invalid token address'])
     print(str(e.content, "UTF-8"))
     # {"statusCode":400,"message":["Invalid token address"],"error":"Bad Request"}
 except TimeoutException:
     print('timeout occurred')
 ```
 
 ## Available APIs
```

### Comparing `credmark-1.3.0/credmark/api/defi_api/__init__.py` & `credmark-1.4.0/credmark/api/defi_api/__init__.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/defi_api/get_cached_model_results.py` & `credmark-1.4.0/credmark/api/defi_api/get_cached_model_results.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/defi_api/get_model_by_slug.py` & `credmark-1.4.0/credmark/api/defi_api/get_model_by_slug.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/defi_api/get_model_deployments_by_slug.py` & `credmark-1.4.0/credmark/api/defi_api/get_model_deployments_by_slug.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/defi_api/get_model_runtime_stats.py` & `credmark-1.4.0/credmark/api/defi_api/get_model_runtime_stats.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/defi_api/list_models.py` & `credmark-1.4.0/credmark/api/defi_api/list_models.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/defi_api/run_model.py` & `credmark-1.4.0/credmark/api/defi_api/run_model.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/__init__.py` & `credmark-1.4.0/credmark/api/token_api/__init__.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_abi.py` & `credmark-1.4.0/credmark/api/token_api/get_token_abi.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_balance.py` & `credmark-1.4.0/credmark/api/token_api/get_token_balance.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_balance_historical.py` & `credmark-1.4.0/credmark/api/token_api/get_token_balance_historical.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_creation_block.py` & `credmark-1.4.0/credmark/api/token_api/get_token_creation_block.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_decimals.py` & `credmark-1.4.0/credmark/api/token_api/get_token_decimals.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_holders.py` & `credmark-1.4.0/credmark/api/token_api/get_token_holders.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_holders_count.py` & `credmark-1.4.0/credmark/api/token_api/get_token_holders_count.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_holders_count_historical.py` & `credmark-1.4.0/credmark/api/token_api/get_token_holders_count_historical.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_logo.py` & `credmark-1.4.0/credmark/api/token_api/get_token_logo.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_metadata.py` & `credmark-1.4.0/credmark/api/token_api/get_token_metadata.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_name.py` & `credmark-1.4.0/credmark/api/token_api/get_token_name.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_price.py` & `credmark-1.4.0/credmark/api/token_api/get_token_price.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_price_historical.py` & `credmark-1.4.0/credmark/api/token_api/get_token_price_historical.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_symbol.py` & `credmark-1.4.0/credmark/api/token_api/get_token_symbol.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_total_supply.py` & `credmark-1.4.0/credmark/api/token_api/get_token_total_supply.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_total_supply_historical.py` & `credmark-1.4.0/credmark/api/token_api/get_token_total_supply_historical.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_volume.py` & `credmark-1.4.0/credmark/api/token_api/get_token_volume.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/token_api/get_token_volume_historical.py` & `credmark-1.4.0/credmark/api/token_api/get_token_volume_historical.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/utilities/__init__.py` & `credmark-1.4.0/credmark/api/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/utilities/check_health.py` & `credmark-1.4.0/credmark/api/utilities/check_health.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/utilities/get_daily_model_usage.py` & `credmark-1.4.0/credmark/api/utilities/get_daily_model_usage.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/utilities/get_top_models.py` & `credmark-1.4.0/credmark/api/utilities/get_top_models.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/api/utilities/get_total_model_usage.py` & `credmark-1.4.0/credmark/api/utilities/get_total_model_usage.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/client.py` & `credmark-1.4.0/credmark/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import ssl
 from typing import Dict, Union
 
 from .api.defi_api import DefiApi
+from .api.portfolio_api import PortfolioApi
 from .api.token_api import TokenApi
 from .api.utilities import Utilities
 
 
 class Credmark:
     """A class for keeping track of data related to the API
 
@@ -47,14 +48,15 @@
         self.api_key = api_key
         self.prefix = prefix
         self.auth_header_name = auth_header_name
 
         self.utilities = Utilities(client=self)
         self.defi_api = DefiApi(client=self)
         self.token_api = TokenApi(client=self)
+        self.portfolio_api = PortfolioApi(client=self)
 
     def get_headers(self) -> Dict[str, str]:
         """Get headers to be used in all endpoints"""
         if not self.api_key:
             return {**self.headers}
         auth_header_value = f"{self.prefix} {self.api_key}" if self.prefix else self.api_key
         return {self.auth_header_name: auth_header_value, **self.headers}
```

### Comparing `credmark-1.3.0/credmark/docs/DefiApi.md` & `credmark-1.4.0/credmark/docs/DefiApi.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/ModelRunResponse.md` & `credmark-1.4.0/credmark/docs/ModelRunResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/ModelRunResponseError.md` & `credmark-1.4.0/credmark/docs/ModelRunResponseError.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenAbiResponse.md` & `credmark-1.4.0/credmark/docs/TokenAbiResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenApi.md` & `credmark-1.4.0/credmark/docs/TokenApi.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenBalanceHistoricalResponse.md` & `credmark-1.4.0/credmark/docs/TokenBalanceHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenBalanceResponse.md` & `credmark-1.4.0/credmark/docs/TokenBalanceResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenHistoricalHoldersCountResponse.md` & `credmark-1.4.0/credmark/docs/TokenHistoricalHoldersCountResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenHoldersResponse.md` & `credmark-1.4.0/credmark/docs/TokenHoldersResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenPriceHistoricalResponse.md` & `credmark-1.4.0/credmark/docs/TokenPriceHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenPriceResponse.md` & `credmark-1.4.0/credmark/docs/TokenPriceResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md` & `credmark-1.4.0/credmark/docs/TokenTotalSupplyHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenVolumeHistoricalResponse.md` & `credmark-1.4.0/credmark/docs/TokenVolumeHistoricalResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/TokenVolumeResponse.md` & `credmark-1.4.0/credmark/docs/TokenVolumeResponse.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/docs/Utilities.md` & `credmark-1.4.0/credmark/docs/Utilities.md`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/errors.py` & `credmark-1.4.0/credmark/errors.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/__init__.py` & `credmark-1.4.0/credmark/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 from .model_call_stack_entry import ModelCallStackEntry
 from .model_deployment import ModelDeployment
 from .model_metadata import ModelMetadata
 from .model_run_response import ModelRunResponse
 from .model_run_response_error import ModelRunResponseError
 from .model_runtime_statistics import ModelRuntimeStatistics
 from .model_runtime_stats_response import ModelRuntimeStatsResponse
+from .portfolio_error_response import PortfolioErrorResponse
+from .position import Position
+from .position_historical_item import PositionHistoricalItem
+from .positions_historical_response import PositionsHistoricalResponse
+from .positions_response import PositionsResponse
+from .returns_response import ReturnsResponse
 from .run_model_dto import RunModelDto
 from .run_model_dto_block_number_type_1 import RunModelDtoBlockNumberType1
 from .token_abi_response import TokenAbiResponse
 from .token_balance_historical_item import TokenBalanceHistoricalItem
 from .token_balance_historical_response import TokenBalanceHistoricalResponse
 from .token_balance_response import TokenBalanceResponse
 from .token_creation_block_response import TokenCreationBlockResponse
@@ -40,21 +46,26 @@
 from .token_holders_response import TokenHoldersResponse
 from .token_logo_response import TokenLogoResponse
 from .token_metadata_response import TokenMetadataResponse
 from .token_name_response import TokenNameResponse
 from .token_price_historical_item import TokenPriceHistoricalItem
 from .token_price_historical_response import TokenPriceHistoricalResponse
 from .token_price_response import TokenPriceResponse
+from .token_return import TokenReturn
 from .token_symbol_response import TokenSymbolResponse
 from .token_total_supply_historical_item import TokenTotalSupplyHistoricalItem
 from .token_total_supply_historical_response import TokenTotalSupplyHistoricalResponse
 from .token_total_supply_response import TokenTotalSupplyResponse
+from .token_value import TokenValue
 from .token_volume_historical_item import TokenVolumeHistoricalItem
 from .token_volume_historical_response import TokenVolumeHistoricalResponse
 from .token_volume_response import TokenVolumeResponse
+from .value_historical_item import ValueHistoricalItem
+from .value_historical_response import ValueHistoricalResponse
+from .value_response import ValueResponse
 
 __all__ = (
     "CheckHealthResponse200",
     "CheckHealthResponse200Details",
     "CheckHealthResponse200DetailsAdditionalProperty",
     "CheckHealthResponse200Error",
     "CheckHealthResponse200ErrorAdditionalProperty",
@@ -73,14 +84,20 @@
     "ModelCallStackEntry",
     "ModelDeployment",
     "ModelMetadata",
     "ModelRunResponse",
     "ModelRunResponseError",
     "ModelRuntimeStatistics",
     "ModelRuntimeStatsResponse",
+    "PortfolioErrorResponse",
+    "Position",
+    "PositionHistoricalItem",
+    "PositionsHistoricalResponse",
+    "PositionsResponse",
+    "ReturnsResponse",
     "RunModelDto",
     "RunModelDtoBlockNumberType1",
     "TokenAbiResponse",
     "TokenBalanceHistoricalItem",
     "TokenBalanceHistoricalResponse",
     "TokenBalanceResponse",
     "TokenCreationBlockResponse",
@@ -93,15 +110,20 @@
     "TokenHoldersResponse",
     "TokenLogoResponse",
     "TokenMetadataResponse",
     "TokenNameResponse",
     "TokenPriceHistoricalItem",
     "TokenPriceHistoricalResponse",
     "TokenPriceResponse",
+    "TokenReturn",
     "TokenSymbolResponse",
     "TokenTotalSupplyHistoricalItem",
     "TokenTotalSupplyHistoricalResponse",
     "TokenTotalSupplyResponse",
+    "TokenValue",
     "TokenVolumeHistoricalItem",
     "TokenVolumeHistoricalResponse",
     "TokenVolumeResponse",
+    "ValueHistoricalItem",
+    "ValueHistoricalResponse",
+    "ValueResponse",
 )
```

### Comparing `credmark-1.3.0/credmark/models/check_health_response_200.py` & `credmark-1.4.0/credmark/models/check_health_response_200.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.check_health_response_200_details import CheckHealthResponse200Details
@@ -23,15 +23,14 @@
         details (Union[Unset, CheckHealthResponse200Details]):  Example: {'database': {'status': 'up'}}.
     """
 
     status: Union[Unset, str] = UNSET
     info: Union[Unset, None, "CheckHealthResponse200Info"] = UNSET
     error: Union[Unset, None, "CheckHealthResponse200Error"] = UNSET
     details: Union[Unset, "CheckHealthResponse200Details"] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         status = self.status
         info: Union[Unset, None, Dict[str, Any]] = UNSET
         if not isinstance(self.info, Unset):
             info = self.info.to_dict() if self.info else None
 
@@ -40,15 +39,14 @@
             error = self.error.to_dict() if self.error else None
 
         details: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.details, Unset):
             details = self.details.to_dict()
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update({})
         if status is not UNSET:
             field_dict["status"] = status
         if info is not UNSET:
             field_dict["info"] = info
         if error is not UNSET:
             field_dict["error"] = error
@@ -94,25 +92,8 @@
         check_health_response_200 = cls(
             status=status,
             info=info,
             error=error,
             details=details,
         )
 
-        check_health_response_200.additional_properties = d
         return check_health_response_200
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
```

### Comparing `credmark-1.3.0/credmark/models/check_health_response_200_details.py` & `credmark-1.4.0/credmark/models/check_health_response_200_details.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_200_details_additional_property.py` & `credmark-1.4.0/credmark/models/check_health_response_200_details_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_200_error.py` & `credmark-1.4.0/credmark/models/check_health_response_200_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_200_error_additional_property.py` & `credmark-1.4.0/credmark/models/check_health_response_200_error_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_200_info.py` & `credmark-1.4.0/credmark/models/check_health_response_200_info.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_200_info_additional_property.py` & `credmark-1.4.0/credmark/models/check_health_response_200_info_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_503_details.py` & `credmark-1.4.0/credmark/models/check_health_response_503_details.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_503_details_additional_property.py` & `credmark-1.4.0/credmark/models/check_health_response_503_details_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_503_error.py` & `credmark-1.4.0/credmark/models/check_health_response_503_error.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_503_error_additional_property.py` & `credmark-1.4.0/credmark/models/check_health_response_503_error_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_503_info.py` & `credmark-1.4.0/credmark/models/check_health_response_503_info.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/check_health_response_503_info_additional_property.py` & `credmark-1.4.0/credmark/models/check_health_response_503_info_additional_property.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/credmark/models/model_run_response.py` & `credmark-1.4.0/credmark/models/model_run_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.model_run_response_error import ModelRunResponseError
@@ -36,15 +36,14 @@
     block_number: float
     block_timestamp: float
     dependencies: Dict[str, Any]
     cached: bool
     runtime: float
     output: Union[Unset, Dict[str, Any]] = UNSET
     error: Union[Unset, "ModelRunResponseError"] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         slug = self.slug
         version = self.version
         chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
@@ -53,15 +52,14 @@
         runtime = self.runtime
         output = self.output
         error: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.error, Unset):
             error = self.error.to_dict()
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "slug": slug,
                 "version": version,
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
@@ -116,25 +114,8 @@
             dependencies=dependencies,
             cached=cached,
             runtime=runtime,
             output=output,
             error=error,
         )
 
-        model_run_response.additional_properties = d
         return model_run_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
```

### Comparing `credmark-1.3.0/credmark/models/model_run_response_error.py` & `credmark-1.4.0/credmark/models/model_run_response_error.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
     type: str
     message: str
     code: str
     permanent: bool
     stack: List["ModelCallStackEntry"]
     detail: Optional[Dict[str, Any]]
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type
         message = self.message
         code = self.code
         permanent = self.permanent
         stack = []
@@ -42,15 +41,14 @@
             stack_item = stack_item_data.to_dict()
 
             stack.append(stack_item)
 
         detail = self.detail
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "type": type,
                 "message": message,
                 "code": code,
                 "permanent": permanent,
                 "stack": stack,
@@ -87,25 +85,8 @@
             message=message,
             code=code,
             permanent=permanent,
             stack=stack,
             detail=detail,
         )
 
-        model_run_response_error.additional_properties = d
         return model_run_response_error
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
```

### Comparing `credmark-1.3.0/credmark/models/run_model_dto.py` & `credmark-1.4.0/credmark/models/run_model_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, Type, TypeVar, Union, cast
 
 import attr
 
 from ..models.run_model_dto_block_number_type_1 import RunModelDtoBlockNumberType1
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="RunModelDto")
@@ -10,26 +10,25 @@
 
 @attr.s(auto_attribs=True)
 class RunModelDto:
     """
     Attributes:
         slug (str): slug of the model to run
         chain_id (int): chainId number, for example 1 for mainnet Default: 1.
-        block_number (Union[RunModelDtoBlockNumberType1, int]): blockNumber is a number or a string with a number,
-            'latest', 'earliest'
+        block_number (Union[RunModelDtoBlockNumberType1, int]): BlockNumber is a number, a number as string, 'latest' or
+            'earliest'
         input (Dict[str, Any]): Model input data
         version (Union[Unset, str]): Typically not required but you may specify version of the model to run
     """
 
     slug: str
     block_number: Union[RunModelDtoBlockNumberType1, int]
     input: Dict[str, Any]
     chain_id: int = 1
     version: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         slug = self.slug
         chain_id = self.chain_id
         block_number: Union[int, str]
 
         if isinstance(self.block_number, RunModelDtoBlockNumberType1):
@@ -38,15 +37,14 @@
         else:
             block_number = self.block_number
 
         input = self.input
         version = self.version
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "slug": slug,
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "input": input,
             }
@@ -84,25 +82,8 @@
             slug=slug,
             chain_id=chain_id,
             block_number=block_number,
             input=input,
             version=version,
         )
 
-        run_model_dto.additional_properties = d
         return run_model_dto
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
```

### Comparing `credmark-1.3.0/credmark/models/token_abi_response.py` & `credmark-1.4.0/credmark/models/token_abi_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,28 +42,26 @@
     chain_id: float
     block_number: float
     block_timestamp: float
     token_address: str
     abi: List[Dict[str, Any]]
     is_transparent_proxy: bool
     proxy_implementation_address: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
         token_address = self.token_address
         abi = self.abi
 
         is_transparent_proxy = self.is_transparent_proxy
         proxy_implementation_address = self.proxy_implementation_address
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
                 "tokenAddress": token_address,
                 "abi": abi,
@@ -98,25 +96,8 @@
             block_timestamp=block_timestamp,
             token_address=token_address,
             abi=abi,
             is_transparent_proxy=is_transparent_proxy,
             proxy_implementation_address=proxy_implementation_address,
         )
 
-        token_abi_response.additional_properties = d
         return token_abi_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
```

### Comparing `credmark-1.3.0/credmark/models/token_balance_historical_item.py` & `credmark-1.4.0/credmark/models/token_holders_count_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,66 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenBalanceHistoricalItem")
+T = TypeVar("T", bound="TokenHoldersCountResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenBalanceHistoricalItem:
+class TokenHoldersCountResponse:
     """
     Attributes:
+        chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
-        balance (float): Token balance Example: 248367.58266143446.
-        value (float): Token value in quoted currency. Example: 18990392.724937014.
+        token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
+        count (float): Total number of holders Example: 42.
     """
 
+    chain_id: float
     block_number: float
     block_timestamp: float
-    balance: float
-    value: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    token_address: str
+    count: float
 
     def to_dict(self) -> Dict[str, Any]:
+        chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
-        balance = self.balance
-        value = self.value
+        token_address = self.token_address
+        count = self.count
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
+                "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
-                "balance": balance,
-                "value": value,
+                "tokenAddress": token_address,
+                "count": count,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
+        chain_id = d.pop("chainId")
+
         block_number = d.pop("blockNumber")
 
         block_timestamp = d.pop("blockTimestamp")
 
-        balance = d.pop("balance")
+        token_address = d.pop("tokenAddress")
 
-        value = d.pop("value")
+        count = d.pop("count")
 
-        token_balance_historical_item = cls(
+        token_holders_count_response = cls(
+            chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
-            balance=balance,
-            value=value,
+            token_address=token_address,
+            count=count,
         )
 
-        token_balance_historical_item.additional_properties = d
-        return token_balance_historical_item
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_holders_count_response
```

### Comparing `credmark-1.3.0/credmark/models/token_balance_historical_response.py` & `credmark-1.4.0/credmark/models/token_balance_historical_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     end_block_number: float
     start_timestamp: float
     end_timestamp: float
     token_address: str
     scaled: bool
     quote_address: str
     data: List["TokenBalanceHistoricalItem"]
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         start_block_number = self.start_block_number
         end_block_number = self.end_block_number
         start_timestamp = self.start_timestamp
         end_timestamp = self.end_timestamp
@@ -48,15 +47,14 @@
         data = []
         for data_item_data in self.data:
             data_item = data_item_data.to_dict()
 
             data.append(data_item)
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "startBlockNumber": start_block_number,
                 "endBlockNumber": end_block_number,
                 "startTimestamp": start_timestamp,
                 "endTimestamp": end_timestamp,
@@ -105,25 +103,8 @@
             end_timestamp=end_timestamp,
             token_address=token_address,
             scaled=scaled,
             quote_address=quote_address,
             data=data,
         )
 
-        token_balance_historical_response.additional_properties = d
         return token_balance_historical_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
```

### Comparing `credmark-1.3.0/credmark/models/token_balance_response.py` & `credmark-1.4.0/credmark/models/token_holders_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,107 +1,114 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-T = TypeVar("T", bound="TokenBalanceResponse")
+from ..types import UNSET, Unset
+
+if TYPE_CHECKING:
+    from ..models.token_holder import TokenHolder
+
+
+T = TypeVar("T", bound="TokenHoldersResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenBalanceResponse:
+class TokenHoldersResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        scaled (bool): If the balance is scaled by token decimals. Example: True.
+        scaled (bool): If the holders' balance is scaled by token decimals. Example: True.
         quote_address (str): Quote address is the token/currency of the price units. Example:
             0x0000000000000000000000000000000000000348.
-        balance (float): Token balance Example: 248367.58266143446.
-        value (float): Token value in quoted currency. Example: 18990392.724937014.
+        data (List['TokenHolder']): Paginated list of holders
+        total (float): Total number of holders Example: 10.
+        cursor (Union[Unset, str]): Cursor to fetch the next page
     """
 
     chain_id: float
     block_number: float
     block_timestamp: float
     token_address: str
     scaled: bool
     quote_address: str
-    balance: float
-    value: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    data: List["TokenHolder"]
+    total: float
+    cursor: Union[Unset, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
         token_address = self.token_address
         scaled = self.scaled
         quote_address = self.quote_address
-        balance = self.balance
-        value = self.value
+        data = []
+        for data_item_data in self.data:
+            data_item = data_item_data.to_dict()
+
+            data.append(data_item)
+
+        total = self.total
+        cursor = self.cursor
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
                 "tokenAddress": token_address,
                 "scaled": scaled,
                 "quoteAddress": quote_address,
-                "balance": balance,
-                "value": value,
+                "data": data,
+                "total": total,
             }
         )
+        if cursor is not UNSET:
+            field_dict["cursor"] = cursor
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.token_holder import TokenHolder
+
         d = src_dict.copy()
         chain_id = d.pop("chainId")
 
         block_number = d.pop("blockNumber")
 
         block_timestamp = d.pop("blockTimestamp")
 
         token_address = d.pop("tokenAddress")
 
         scaled = d.pop("scaled")
 
         quote_address = d.pop("quoteAddress")
 
-        balance = d.pop("balance")
+        data = []
+        _data = d.pop("data")
+        for data_item_data in _data:
+            data_item = TokenHolder.from_dict(data_item_data)
+
+            data.append(data_item)
 
-        value = d.pop("value")
+        total = d.pop("total")
 
-        token_balance_response = cls(
+        cursor = d.pop("cursor", UNSET)
+
+        token_holders_response = cls(
             chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
             token_address=token_address,
             scaled=scaled,
             quote_address=quote_address,
-            balance=balance,
-            value=value,
+            data=data,
+            total=total,
+            cursor=cursor,
         )
 
-        token_balance_response.additional_properties = d
-        return token_balance_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_holders_response
```

### Comparing `credmark-1.3.0/credmark/models/token_creation_block_response.py` & `credmark-1.4.0/credmark/models/token_creation_block_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, Type, TypeVar
 
 import attr
 
 T = TypeVar("T", bound="TokenCreationBlockResponse")
 
 
 @attr.s(auto_attribs=True)
@@ -17,25 +17,23 @@
     """
 
     chain_id: float
     block_number: float
     block_timestamp: float
     token_address: str
     creation_block: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
         token_address = self.token_address
         creation_block = self.creation_block
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
                 "tokenAddress": token_address,
                 "creationBlock": creation_block,
@@ -61,25 +59,8 @@
             chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
             token_address=token_address,
             creation_block=creation_block,
         )
 
-        token_creation_block_response.additional_properties = d
         return token_creation_block_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
```

### Comparing `credmark-1.3.0/credmark/models/token_decimals_response.py` & `credmark-1.4.0/credmark/models/token_metadata_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,53 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenDecimalsResponse")
+T = TypeVar("T", bound="TokenMetadataResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenDecimalsResponse:
+class TokenMetadataResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
+        name (str): Token name Example: Aave Token.
+        symbol (str): Token symbol Example: AAVE.
         decimals (float): Token decimals Example: 18.
     """
 
     chain_id: float
     block_number: float
     block_timestamp: float
     token_address: str
+    name: str
+    symbol: str
     decimals: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
         token_address = self.token_address
+        name = self.name
+        symbol = self.symbol
         decimals = self.decimals
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
                 "tokenAddress": token_address,
+                "name": name,
+                "symbol": symbol,
                 "decimals": decimals,
             }
         )
 
         return field_dict
 
     @classmethod
@@ -51,35 +57,24 @@
 
         block_number = d.pop("blockNumber")
 
         block_timestamp = d.pop("blockTimestamp")
 
         token_address = d.pop("tokenAddress")
 
+        name = d.pop("name")
+
+        symbol = d.pop("symbol")
+
         decimals = d.pop("decimals")
 
-        token_decimals_response = cls(
+        token_metadata_response = cls(
             chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
             token_address=token_address,
+            name=name,
+            symbol=symbol,
             decimals=decimals,
         )
 
-        token_decimals_response.additional_properties = d
-        return token_decimals_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_metadata_response
```

### Comparing `credmark-1.3.0/credmark/models/token_error_response.py` & `credmark-1.4.0/credmark/models/token_error_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,29 +15,27 @@
         message (Union[List[str], str]): If an error response (non-200 status code), the message will be set with an
             error message. It can either be a string or a list of strings. Example: ['Invalid token address'].
     """
 
     status_code: float
     error: str
     message: Union[List[str], str]
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         status_code = self.status_code
         error = self.error
         message: Union[List[str], str]
 
         if isinstance(self.message, list):
             message = self.message
 
         else:
             message = self.message
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "statusCode": status_code,
                 "error": error,
                 "message": message,
             }
         )
@@ -66,25 +64,8 @@
 
         token_error_response = cls(
             status_code=status_code,
             error=error,
             message=message,
         )
 
-        token_error_response.additional_properties = d
         return token_error_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
```

### Comparing `credmark-1.3.0/credmark/models/token_historical_holders_count_response.py` & `credmark-1.4.0/credmark/models/token_total_supply_historical_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,102 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
 if TYPE_CHECKING:
-    from ..models.token_holders_count_historical_item import TokenHoldersCountHistoricalItem
+    from ..models.token_total_supply_historical_item import TokenTotalSupplyHistoricalItem
 
 
-T = TypeVar("T", bound="TokenHistoricalHoldersCountResponse")
+T = TypeVar("T", bound="TokenTotalSupplyHistoricalResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenHistoricalHoldersCountResponse:
+class TokenTotalSupplyHistoricalResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         start_block_number (float): Start block number. Example: 15384120.
         end_block_number (float): End block number. Example: 15581908.
         start_timestamp (float): Start timestamp. Number of seconds since January 1, 1970. Example: 1661086905.
         end_timestamp (float): End timestamp. Number of seconds since January 1, 1970. Example: 1663765199.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        data (List['TokenHoldersCountHistoricalItem']):
+        scaled (bool): If the total supply is scaled by token decimals. Example: True.
+        data (List['TokenTotalSupplyHistoricalItem']):
     """
 
     chain_id: float
     start_block_number: float
     end_block_number: float
     start_timestamp: float
     end_timestamp: float
     token_address: str
-    data: List["TokenHoldersCountHistoricalItem"]
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    scaled: bool
+    data: List["TokenTotalSupplyHistoricalItem"]
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         start_block_number = self.start_block_number
         end_block_number = self.end_block_number
         start_timestamp = self.start_timestamp
         end_timestamp = self.end_timestamp
         token_address = self.token_address
+        scaled = self.scaled
         data = []
         for data_item_data in self.data:
             data_item = data_item_data.to_dict()
 
             data.append(data_item)
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "startBlockNumber": start_block_number,
                 "endBlockNumber": end_block_number,
                 "startTimestamp": start_timestamp,
                 "endTimestamp": end_timestamp,
                 "tokenAddress": token_address,
+                "scaled": scaled,
                 "data": data,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.token_holders_count_historical_item import TokenHoldersCountHistoricalItem
+        from ..models.token_total_supply_historical_item import TokenTotalSupplyHistoricalItem
 
         d = src_dict.copy()
         chain_id = d.pop("chainId")
 
         start_block_number = d.pop("startBlockNumber")
 
         end_block_number = d.pop("endBlockNumber")
 
         start_timestamp = d.pop("startTimestamp")
 
         end_timestamp = d.pop("endTimestamp")
 
         token_address = d.pop("tokenAddress")
 
+        scaled = d.pop("scaled")
+
         data = []
         _data = d.pop("data")
         for data_item_data in _data:
-            data_item = TokenHoldersCountHistoricalItem.from_dict(data_item_data)
+            data_item = TokenTotalSupplyHistoricalItem.from_dict(data_item_data)
 
             data.append(data_item)
 
-        token_historical_holders_count_response = cls(
+        token_total_supply_historical_response = cls(
             chain_id=chain_id,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
             token_address=token_address,
+            scaled=scaled,
             data=data,
         )
 
-        token_historical_holders_count_response.additional_properties = d
-        return token_historical_holders_count_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_total_supply_historical_response
```

### Comparing `credmark-1.3.0/credmark/models/token_holders_count_historical_item.py` & `credmark-1.4.0/credmark/models/token_symbol_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,66 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenHoldersCountHistoricalItem")
+T = TypeVar("T", bound="TokenSymbolResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenHoldersCountHistoricalItem:
+class TokenSymbolResponse:
     """
     Attributes:
+        chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
-        count (float): Total number of holders Example: 42.
+        token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
+        symbol (str): Token symbol Example: AAVE.
     """
 
+    chain_id: float
     block_number: float
     block_timestamp: float
-    count: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    token_address: str
+    symbol: str
 
     def to_dict(self) -> Dict[str, Any]:
+        chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
-        count = self.count
+        token_address = self.token_address
+        symbol = self.symbol
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
+                "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
-                "count": count,
+                "tokenAddress": token_address,
+                "symbol": symbol,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
+        chain_id = d.pop("chainId")
+
         block_number = d.pop("blockNumber")
 
         block_timestamp = d.pop("blockTimestamp")
 
-        count = d.pop("count")
+        token_address = d.pop("tokenAddress")
+
+        symbol = d.pop("symbol")
 
-        token_holders_count_historical_item = cls(
+        token_symbol_response = cls(
+            chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
-            count=count,
+            token_address=token_address,
+            symbol=symbol,
         )
 
-        token_holders_count_historical_item.additional_properties = d
-        return token_holders_count_historical_item
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_symbol_response
```

### Comparing `credmark-1.3.0/credmark/models/token_holders_count_response.py` & `credmark-1.4.0/credmark/models/token_volume_historical_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,102 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenHoldersCountResponse")
+if TYPE_CHECKING:
+    from ..models.token_volume_historical_item import TokenVolumeHistoricalItem
+
+
+T = TypeVar("T", bound="TokenVolumeHistoricalResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenHoldersCountResponse:
+class TokenVolumeHistoricalResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
-        block_number (float): Block number. Example: 15490034.
-        block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
+        start_block_number (float): Start block number. Example: 15384120.
+        end_block_number (float): End block number. Example: 15581908.
+        start_timestamp (float): Start timestamp. Number of seconds since January 1, 1970. Example: 1661086905.
+        end_timestamp (float): End timestamp. Number of seconds since January 1, 1970. Example: 1663765199.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        count (float): Total number of holders Example: 42.
+        scaled (bool): If the volume is scaled by token decimals. Example: True.
+        data (List['TokenVolumeHistoricalItem']):
     """
 
     chain_id: float
-    block_number: float
-    block_timestamp: float
+    start_block_number: float
+    end_block_number: float
+    start_timestamp: float
+    end_timestamp: float
     token_address: str
-    count: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    scaled: bool
+    data: List["TokenVolumeHistoricalItem"]
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
-        block_number = self.block_number
-        block_timestamp = self.block_timestamp
+        start_block_number = self.start_block_number
+        end_block_number = self.end_block_number
+        start_timestamp = self.start_timestamp
+        end_timestamp = self.end_timestamp
         token_address = self.token_address
-        count = self.count
+        scaled = self.scaled
+        data = []
+        for data_item_data in self.data:
+            data_item = data_item_data.to_dict()
+
+            data.append(data_item)
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
-                "blockNumber": block_number,
-                "blockTimestamp": block_timestamp,
+                "startBlockNumber": start_block_number,
+                "endBlockNumber": end_block_number,
+                "startTimestamp": start_timestamp,
+                "endTimestamp": end_timestamp,
                 "tokenAddress": token_address,
-                "count": count,
+                "scaled": scaled,
+                "data": data,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.token_volume_historical_item import TokenVolumeHistoricalItem
+
         d = src_dict.copy()
         chain_id = d.pop("chainId")
 
-        block_number = d.pop("blockNumber")
+        start_block_number = d.pop("startBlockNumber")
 
-        block_timestamp = d.pop("blockTimestamp")
+        end_block_number = d.pop("endBlockNumber")
 
-        token_address = d.pop("tokenAddress")
+        start_timestamp = d.pop("startTimestamp")
 
-        count = d.pop("count")
+        end_timestamp = d.pop("endTimestamp")
 
-        token_holders_count_response = cls(
-            chain_id=chain_id,
-            block_number=block_number,
-            block_timestamp=block_timestamp,
-            token_address=token_address,
-            count=count,
-        )
-
-        token_holders_count_response.additional_properties = d
-        return token_holders_count_response
+        token_address = d.pop("tokenAddress")
 
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
+        scaled = d.pop("scaled")
 
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
+        data = []
+        _data = d.pop("data")
+        for data_item_data in _data:
+            data_item = TokenVolumeHistoricalItem.from_dict(data_item_data)
 
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
+            data.append(data_item)
 
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
+        token_volume_historical_response = cls(
+            chain_id=chain_id,
+            start_block_number=start_block_number,
+            end_block_number=end_block_number,
+            start_timestamp=start_timestamp,
+            end_timestamp=end_timestamp,
+            token_address=token_address,
+            scaled=scaled,
+            data=data,
+        )
 
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_volume_historical_response
```

### Comparing `credmark-1.3.0/credmark/models/token_holders_response.py` & `credmark-1.4.0/credmark/models/token_price_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,88 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
-if TYPE_CHECKING:
-    from ..models.token_holder import TokenHolder
-
-
-T = TypeVar("T", bound="TokenHoldersResponse")
+T = TypeVar("T", bound="TokenPriceResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenHoldersResponse:
+class TokenPriceResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        scaled (bool): If the holders' balance is scaled by token decimals. Example: True.
         quote_address (str): Quote address is the token/currency of the price units. Example:
             0x0000000000000000000000000000000000000348.
-        data (List['TokenHolder']): Paginated list of holders
-        total (float): Total number of holders Example: 10.
-        cursor (Union[Unset, str]): Cursor to fetch the next page
+        price (float): Price of the token in quote units. Example: 82.82911921.
+        src (str): Source of the token price. Example: dex or cex.
+        src_internal (str): The internal source for tracing Example: db, model, cache, etc..
     """
 
     chain_id: float
     block_number: float
     block_timestamp: float
     token_address: str
-    scaled: bool
     quote_address: str
-    data: List["TokenHolder"]
-    total: float
-    cursor: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    price: float
+    src: str
+    src_internal: str
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
         token_address = self.token_address
-        scaled = self.scaled
         quote_address = self.quote_address
-        data = []
-        for data_item_data in self.data:
-            data_item = data_item_data.to_dict()
-
-            data.append(data_item)
-
-        total = self.total
-        cursor = self.cursor
+        price = self.price
+        src = self.src
+        src_internal = self.src_internal
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
                 "tokenAddress": token_address,
-                "scaled": scaled,
                 "quoteAddress": quote_address,
-                "data": data,
-                "total": total,
+                "price": price,
+                "src": src,
+                "srcInternal": src_internal,
             }
         )
-        if cursor is not UNSET:
-            field_dict["cursor"] = cursor
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.token_holder import TokenHolder
-
         d = src_dict.copy()
         chain_id = d.pop("chainId")
 
         block_number = d.pop("blockNumber")
 
         block_timestamp = d.pop("blockTimestamp")
 
         token_address = d.pop("tokenAddress")
 
-        scaled = d.pop("scaled")
-
         quote_address = d.pop("quoteAddress")
 
-        data = []
-        _data = d.pop("data")
-        for data_item_data in _data:
-            data_item = TokenHolder.from_dict(data_item_data)
+        price = d.pop("price")
 
-            data.append(data_item)
+        src = d.pop("src")
 
-        total = d.pop("total")
+        src_internal = d.pop("srcInternal")
 
-        cursor = d.pop("cursor", UNSET)
-
-        token_holders_response = cls(
+        token_price_response = cls(
             chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
             token_address=token_address,
-            scaled=scaled,
             quote_address=quote_address,
-            data=data,
-            total=total,
-            cursor=cursor,
+            price=price,
+            src=src,
+            src_internal=src_internal,
         )
 
-        token_holders_response.additional_properties = d
-        return token_holders_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_price_response
```

### Comparing `credmark-1.3.0/credmark/models/token_logo_response.py` & `credmark-1.4.0/credmark/models/token_balance_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,59 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenLogoResponse")
+T = TypeVar("T", bound="TokenBalanceResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenLogoResponse:
+class TokenBalanceResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        logo_url (str): Token logo url Example: https://raw.githubusercontent.com/trustwallet/assets/master/blockchains/
-            ethereum/assets/0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9/logo.png.
+        scaled (bool): If the balance is scaled by token decimals. Example: True.
+        quote_address (str): Quote address is the token/currency of the price units. Example:
+            0x0000000000000000000000000000000000000348.
+        balance (float): Token balance Example: 248367.58266143446.
+        value (float): Token value in quoted currency. Example: 18990392.724937014.
     """
 
     chain_id: float
     block_number: float
     block_timestamp: float
     token_address: str
-    logo_url: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    scaled: bool
+    quote_address: str
+    balance: float
+    value: float
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
         token_address = self.token_address
-        logo_url = self.logo_url
+        scaled = self.scaled
+        quote_address = self.quote_address
+        balance = self.balance
+        value = self.value
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
                 "tokenAddress": token_address,
-                "logoUrl": logo_url,
+                "scaled": scaled,
+                "quoteAddress": quote_address,
+                "balance": balance,
+                "value": value,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
@@ -52,35 +62,27 @@
 
         block_number = d.pop("blockNumber")
 
         block_timestamp = d.pop("blockTimestamp")
 
         token_address = d.pop("tokenAddress")
 
-        logo_url = d.pop("logoUrl")
+        scaled = d.pop("scaled")
 
-        token_logo_response = cls(
+        quote_address = d.pop("quoteAddress")
+
+        balance = d.pop("balance")
+
+        value = d.pop("value")
+
+        token_balance_response = cls(
             chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
             token_address=token_address,
-            logo_url=logo_url,
+            scaled=scaled,
+            quote_address=quote_address,
+            balance=balance,
+            value=value,
         )
 
-        token_logo_response.additional_properties = d
-        return token_logo_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_balance_response
```

### Comparing `credmark-1.3.0/credmark/models/token_metadata_response.py` & `credmark-1.4.0/credmark/models/token_price_historical_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,103 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenMetadataResponse")
+if TYPE_CHECKING:
+    from ..models.token_price_historical_item import TokenPriceHistoricalItem
+
+
+T = TypeVar("T", bound="TokenPriceHistoricalResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenMetadataResponse:
+class TokenPriceHistoricalResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
-        block_number (float): Block number. Example: 15490034.
-        block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
+        start_block_number (float): Start block number. Example: 15384120.
+        end_block_number (float): End block number. Example: 15581908.
+        start_timestamp (float): Start timestamp. Number of seconds since January 1, 1970. Example: 1661086905.
+        end_timestamp (float): End timestamp. Number of seconds since January 1, 1970. Example: 1663765199.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        name (str): Token name Example: Aave Token.
-        symbol (str): Token symbol Example: AAVE.
-        decimals (float): Token decimals Example: 18.
+        quote_address (str): Quote address is the token/currency of the price units. Example:
+            0x0000000000000000000000000000000000000348.
+        data (List['TokenPriceHistoricalItem']):
     """
 
     chain_id: float
-    block_number: float
-    block_timestamp: float
+    start_block_number: float
+    end_block_number: float
+    start_timestamp: float
+    end_timestamp: float
     token_address: str
-    name: str
-    symbol: str
-    decimals: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    quote_address: str
+    data: List["TokenPriceHistoricalItem"]
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
-        block_number = self.block_number
-        block_timestamp = self.block_timestamp
+        start_block_number = self.start_block_number
+        end_block_number = self.end_block_number
+        start_timestamp = self.start_timestamp
+        end_timestamp = self.end_timestamp
         token_address = self.token_address
-        name = self.name
-        symbol = self.symbol
-        decimals = self.decimals
+        quote_address = self.quote_address
+        data = []
+        for data_item_data in self.data:
+            data_item = data_item_data.to_dict()
+
+            data.append(data_item)
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
-                "blockNumber": block_number,
-                "blockTimestamp": block_timestamp,
+                "startBlockNumber": start_block_number,
+                "endBlockNumber": end_block_number,
+                "startTimestamp": start_timestamp,
+                "endTimestamp": end_timestamp,
                 "tokenAddress": token_address,
-                "name": name,
-                "symbol": symbol,
-                "decimals": decimals,
+                "quoteAddress": quote_address,
+                "data": data,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.token_price_historical_item import TokenPriceHistoricalItem
+
         d = src_dict.copy()
         chain_id = d.pop("chainId")
 
-        block_number = d.pop("blockNumber")
+        start_block_number = d.pop("startBlockNumber")
+
+        end_block_number = d.pop("endBlockNumber")
+
+        start_timestamp = d.pop("startTimestamp")
 
-        block_timestamp = d.pop("blockTimestamp")
+        end_timestamp = d.pop("endTimestamp")
 
         token_address = d.pop("tokenAddress")
 
-        name = d.pop("name")
+        quote_address = d.pop("quoteAddress")
 
-        symbol = d.pop("symbol")
+        data = []
+        _data = d.pop("data")
+        for data_item_data in _data:
+            data_item = TokenPriceHistoricalItem.from_dict(data_item_data)
 
-        decimals = d.pop("decimals")
+            data.append(data_item)
 
-        token_metadata_response = cls(
+        token_price_historical_response = cls(
             chain_id=chain_id,
-            block_number=block_number,
-            block_timestamp=block_timestamp,
+            start_block_number=start_block_number,
+            end_block_number=end_block_number,
+            start_timestamp=start_timestamp,
+            end_timestamp=end_timestamp,
             token_address=token_address,
-            name=name,
-            symbol=symbol,
-            decimals=decimals,
+            quote_address=quote_address,
+            data=data,
         )
 
-        token_metadata_response.additional_properties = d
-        return token_metadata_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_price_historical_response
```

### Comparing `credmark-1.3.0/credmark/models/token_total_supply_historical_item.py` & `credmark-1.4.0/credmark/models/token_name_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,66 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenTotalSupplyHistoricalItem")
+T = TypeVar("T", bound="TokenNameResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenTotalSupplyHistoricalItem:
+class TokenNameResponse:
     """
     Attributes:
+        chain_id (float): Chain ID. Example: 1.
         block_number (float): Block number. Example: 15490034.
         block_timestamp (float): Block timestamp. Number of seconds since January 1, 1970. Example: 1662550007.
-        total_supply (float): Token total supply Example: 16000000.
+        token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
+        name (str): Token name Example: Aave Token.
     """
 
+    chain_id: float
     block_number: float
     block_timestamp: float
-    total_supply: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    token_address: str
+    name: str
 
     def to_dict(self) -> Dict[str, Any]:
+        chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
-        total_supply = self.total_supply
+        token_address = self.token_address
+        name = self.name
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
+                "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
-                "totalSupply": total_supply,
+                "tokenAddress": token_address,
+                "name": name,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
+        chain_id = d.pop("chainId")
+
         block_number = d.pop("blockNumber")
 
         block_timestamp = d.pop("blockTimestamp")
 
-        total_supply = d.pop("totalSupply")
+        token_address = d.pop("tokenAddress")
+
+        name = d.pop("name")
 
-        token_total_supply_historical_item = cls(
+        token_name_response = cls(
+            chain_id=chain_id,
             block_number=block_number,
             block_timestamp=block_timestamp,
-            total_supply=total_supply,
+            token_address=token_address,
+            name=name,
         )
 
-        token_total_supply_historical_item.additional_properties = d
-        return token_total_supply_historical_item
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_name_response
```

### Comparing `credmark-1.3.0/credmark/models/token_total_supply_response.py` & `credmark-1.4.0/credmark/models/token_total_supply_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, Type, TypeVar
 
 import attr
 
 T = TypeVar("T", bound="TokenTotalSupplyResponse")
 
 
 @attr.s(auto_attribs=True)
@@ -19,26 +19,24 @@
 
     chain_id: float
     block_number: float
     block_timestamp: float
     token_address: str
     scaled: bool
     total_supply: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         block_number = self.block_number
         block_timestamp = self.block_timestamp
         token_address = self.token_address
         scaled = self.scaled
         total_supply = self.total_supply
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "blockNumber": block_number,
                 "blockTimestamp": block_timestamp,
                 "tokenAddress": token_address,
                 "scaled": scaled,
@@ -68,25 +66,8 @@
             block_number=block_number,
             block_timestamp=block_timestamp,
             token_address=token_address,
             scaled=scaled,
             total_supply=total_supply,
         )
 
-        token_total_supply_response.additional_properties = d
         return token_total_supply_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
```

### Comparing `credmark-1.3.0/credmark/models/token_volume_historical_item.py` & `credmark-1.4.0/credmark/models/token_volume_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,87 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenVolumeHistoricalItem")
+T = TypeVar("T", bound="TokenVolumeResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenVolumeHistoricalItem:
+class TokenVolumeResponse:
     """
     Attributes:
+        chain_id (float): Chain ID. Example: 1.
         start_block_number (float): Start block number. Example: 15384120.
         end_block_number (float): End block number. Example: 15581908.
         start_timestamp (float): Start timestamp. Number of seconds since January 1, 1970. Example: 1661086905.
         end_timestamp (float): End timestamp. Number of seconds since January 1, 1970. Example: 1663765199.
+        token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
+        scaled (bool): If the volume is scaled by token decimals. Example: True.
         volume (float): Token volume Example: 16173531.8220335.
     """
 
+    chain_id: float
     start_block_number: float
     end_block_number: float
     start_timestamp: float
     end_timestamp: float
+    token_address: str
+    scaled: bool
     volume: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        chain_id = self.chain_id
         start_block_number = self.start_block_number
         end_block_number = self.end_block_number
         start_timestamp = self.start_timestamp
         end_timestamp = self.end_timestamp
+        token_address = self.token_address
+        scaled = self.scaled
         volume = self.volume
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
+                "chainId": chain_id,
                 "startBlockNumber": start_block_number,
                 "endBlockNumber": end_block_number,
                 "startTimestamp": start_timestamp,
                 "endTimestamp": end_timestamp,
+                "tokenAddress": token_address,
+                "scaled": scaled,
                 "volume": volume,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
+        chain_id = d.pop("chainId")
+
         start_block_number = d.pop("startBlockNumber")
 
         end_block_number = d.pop("endBlockNumber")
 
         start_timestamp = d.pop("startTimestamp")
 
         end_timestamp = d.pop("endTimestamp")
 
+        token_address = d.pop("tokenAddress")
+
+        scaled = d.pop("scaled")
+
         volume = d.pop("volume")
 
-        token_volume_historical_item = cls(
+        token_volume_response = cls(
+            chain_id=chain_id,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
+            token_address=token_address,
+            scaled=scaled,
             volume=volume,
         )
 
-        token_volume_historical_item.additional_properties = d
-        return token_volume_historical_item
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_volume_response
```

### Comparing `credmark-1.3.0/credmark/models/token_volume_response.py` & `credmark-1.4.0/credmark/models/token_historical_holders_count_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,95 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="TokenVolumeResponse")
+if TYPE_CHECKING:
+    from ..models.token_holders_count_historical_item import TokenHoldersCountHistoricalItem
+
+
+T = TypeVar("T", bound="TokenHistoricalHoldersCountResponse")
 
 
 @attr.s(auto_attribs=True)
-class TokenVolumeResponse:
+class TokenHistoricalHoldersCountResponse:
     """
     Attributes:
         chain_id (float): Chain ID. Example: 1.
         start_block_number (float): Start block number. Example: 15384120.
         end_block_number (float): End block number. Example: 15581908.
         start_timestamp (float): Start timestamp. Number of seconds since January 1, 1970. Example: 1661086905.
         end_timestamp (float): End timestamp. Number of seconds since January 1, 1970. Example: 1663765199.
         token_address (str): Token address for the price. Example: 0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9.
-        scaled (bool): If the volume is scaled by token decimals. Example: True.
-        volume (float): Token volume Example: 16173531.8220335.
+        data (List['TokenHoldersCountHistoricalItem']):
     """
 
     chain_id: float
     start_block_number: float
     end_block_number: float
     start_timestamp: float
     end_timestamp: float
     token_address: str
-    scaled: bool
-    volume: float
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    data: List["TokenHoldersCountHistoricalItem"]
 
     def to_dict(self) -> Dict[str, Any]:
         chain_id = self.chain_id
         start_block_number = self.start_block_number
         end_block_number = self.end_block_number
         start_timestamp = self.start_timestamp
         end_timestamp = self.end_timestamp
         token_address = self.token_address
-        scaled = self.scaled
-        volume = self.volume
+        data = []
+        for data_item_data in self.data:
+            data_item = data_item_data.to_dict()
+
+            data.append(data_item)
 
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "chainId": chain_id,
                 "startBlockNumber": start_block_number,
                 "endBlockNumber": end_block_number,
                 "startTimestamp": start_timestamp,
                 "endTimestamp": end_timestamp,
                 "tokenAddress": token_address,
-                "scaled": scaled,
-                "volume": volume,
+                "data": data,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.token_holders_count_historical_item import TokenHoldersCountHistoricalItem
+
         d = src_dict.copy()
         chain_id = d.pop("chainId")
 
         start_block_number = d.pop("startBlockNumber")
 
         end_block_number = d.pop("endBlockNumber")
 
         start_timestamp = d.pop("startTimestamp")
 
         end_timestamp = d.pop("endTimestamp")
 
         token_address = d.pop("tokenAddress")
 
-        scaled = d.pop("scaled")
+        data = []
+        _data = d.pop("data")
+        for data_item_data in _data:
+            data_item = TokenHoldersCountHistoricalItem.from_dict(data_item_data)
 
-        volume = d.pop("volume")
+            data.append(data_item)
 
-        token_volume_response = cls(
+        token_historical_holders_count_response = cls(
             chain_id=chain_id,
             start_block_number=start_block_number,
             end_block_number=end_block_number,
             start_timestamp=start_timestamp,
             end_timestamp=end_timestamp,
             token_address=token_address,
-            scaled=scaled,
-            volume=volume,
+            data=data,
         )
 
-        token_volume_response.additional_properties = d
-        return token_volume_response
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
+        return token_historical_holders_count_response
```

### Comparing `credmark-1.3.0/credmark/types.py` & `credmark-1.4.0/credmark/types.py`

 * *Files identical despite different names*

### Comparing `credmark-1.3.0/pyproject.toml` & `credmark-1.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "credmark"
-version = "1.3.0"
+version = "1.4.0"
 description = "A client library for accessing Credmark Gateway"
 license = "MIT"
 
 authors = [
   "Credmark <info@credmark.com>",
 ]
```

### Comparing `credmark-1.3.0/PKG-INFO` & `credmark-1.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credmark
-Version: 1.3.0
+Version: 1.4.0
 Summary: A client library for accessing Credmark Gateway
 Home-page: https://credmark.com
 License: MIT
 Author: Credmark
 Author-email: info@credmark.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -57,54 +57,83 @@
 
 Now call your endpoint by tag and use your models:
 
 ```python
 metadata = client.token_api.get_token_metadata(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9")
 
 print(metadata)
-# TokenMetadataResponse(chain_id=1, block_number=17044112, block_timestamp=1681459199, token_address='0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9', name='Aave Token', symbol='AAVE', decimals=18, additional_properties={})
+# TokenMetadataResponse(chain_id=1, block_number=17044112, block_timestamp=1681459199, token_address='0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9', name='Aave Token', symbol='AAVE', decimals=18)
 ```
 
 Or do the same thing with an async version:
 
 ```python
 import asyncio
 
 async def get_metadata():
     metadata = await client.token_api.get_token_metadata_async(1, "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9")
     print(metadata)
-    # TokenMetadataResponse(chain_id=1, block_number=17044112, block_timestamp=1681459199, token_address='0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9', name='Aave Token', symbol='AAVE', decimals=18, additional_properties={})
+    # TokenMetadataResponse(chain_id=1, block_number=17044112, block_timestamp=1681459199, token_address='0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9', name='Aave Token', symbol='AAVE', decimals=18)
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(get_metadata())
 loop.close()
 ```
 
-## Run a model
+## Examples
 
-You can run a model using DeFi API:
+### 1. DeFi API - Run models
+
+Get all Uniswap V3 pools for USDC on Ethereum Mainnet:
 
 ```python
 from credmark.models import RunModelDto
 
 result = client.defi_api.run_model(
     json_body=RunModelDto(
         chain_id=1, 
         block_number="latest", 
-        slug="price.quote", 
-        input={"base": {"symbol": "AAVE"}, "prefer": "dex"}
+        slug="uniswap-v3.get-pools", 
+        input={"symbol": "USDC"}
     ),
 )
 
 print(result.chain_id, result.block_number)
-# 1 17044112
+# 1 17563869
 print(result.slug, result.version)
-# price.quote 1.11
+# uniswap-v3.get-pools 0.1
 print(result.output)
-# {'src': 'dex|uniswap-v2,sushiswap,uniswap-v3|Non-zero:9|Zero:2|4.0', 'price': 82.19716419870656, 'quoteAddress': '0x0000000000000000000000000000000000000348'}
+# {'contracts': [{'address': '0x5777d92f208679db4b9778590fa3cab3ac9e2168'}, {'address': '0x6c6bc977e13df9b0de53b251522280bb72383700'}, {'address': '0xa63b490aa077f541c9d64bfc1cc0db2a752157b5'}, {'address': '0x6958686b6348c3d6d5f2dca3106a5c09c156873a'}, {'address': '0x3416cf6c708da44db2624d63ea0aaef7113527c6'}, {'address': '0x7858e59e0c01ea06df3af3d20ac7b0003275d4bf'}, {'address': '0xee4cf3b78a74affa38c6a926282bcd8b5952818d'}, {'address': '0xbb256c2f1b677e27118b0345fd2b3894d2e6d487'}]}
+```
+
+### 2. Portfolio API
+
+Get all positions, i.e. tokens and balances for a wallet
+
+```python
+result = client.portfolio_api.get_positions(1, ["0x5291fBB0ee9F51225f0928Ff6a83108c86327636"])
+
+print(result.chain_id, result.block_number)
+# 1 17567721
+print(result.positions)
+# [Position(token_address='0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48', balance=2.169356), Position(token_address='0xdac17f958d2ee523a2206206994597c13d831ec7', balance=479.354369)]
+```
+
+### 3. Token API
+
+Get price of AAVE token (0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9)
+
+```python
+result = client.token_api.get_token_price(1, "0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9")
+
+print(result.chain_id, result.block_number)
+# 1 17567740
+print(result.price, result.src, result.quote_address)
+# 64.599481 cex 0x0000000000000000000000000000000000000348
+# 0x0000000000000000000000000000000000000348 => USD address
 ```
 
 ## Handling Errors
 
 Each method can raise:
 
 - errors.CredmarkError: If the server returns a non 2xx status code.
@@ -116,15 +145,15 @@
 
 try:
     metadata = client.token_api.get_token_metadata(1, "WRONG TOKEN ADDRESS")
 except CredmarkError as e:
     print(e.status_code)
     # 400
     print(e.parsed)
-    # TokenErrorResponse(status_code=400, error='Bad Request', message=['Invalid token address'], additional_properties={})
+    # TokenErrorResponse(status_code=400, error='Bad Request', message=['Invalid token address'])
     print(str(e.content, "UTF-8"))
     # {"statusCode":400,"message":["Invalid token address"],"error":"Bad Request"}
 except TimeoutException:
     print('timeout occurred')
 ```
 
 ## Available APIs
```

