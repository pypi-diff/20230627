# Comparing `tmp/jtech-1.0.1.tar.gz` & `tmp/jtech-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtech-1.0.1.tar", last modified: Mon Jun 26 16:56:51 2023, max compression
+gzip compressed data, was "jtech-1.0.2.tar", max compression
```

## Comparing `jtech-1.0.1.tar` & `jtech-1.0.2.tar`

### file list

```diff
@@ -1,56 +1,98 @@
-drwxr-xr-x   0 angelo    (1000) angelo    (1000)        0 2023-06-26 16:56:51.744652 jtech-1.0.1/
--rw-r--r--   0 angelo    (1000) angelo    (1000)      130 2023-06-26 16:52:20.000000 jtech-1.0.1/MANIFEST.in
--rw-r--r--   0 angelo    (1000) angelo    (1000)      252 2023-06-26 16:56:51.744652 jtech-1.0.1/PKG-INFO
-drwxr-xr-x   0 angelo    (1000) angelo    (1000)        0 2023-06-26 16:56:51.738652 jtech-1.0.1/jtech/
--rw-r--r--   0 angelo    (1000) angelo    (1000)        0 2023-06-19 12:53:20.000000 jtech-1.0.1/jtech/__init__.py
--rw-r--r--   0 angelo    (1000) angelo    (1000)     2255 2023-06-26 16:33:22.000000 jtech-1.0.1/jtech/__main__.py
-drwxr-xr-x   0 angelo    (1000) angelo    (1000)        0 2023-06-26 16:56:51.737652 jtech-1.0.1/jtech/resources/
-drwxr-xr-x   0 angelo    (1000) angelo    (1000)        0 2023-06-26 16:56:51.739652 jtech-1.0.1/jtech/resources/banner/
--rw-r--r--   0 angelo    (1000) angelo    (1000)      540 2023-06-23 16:17:26.000000 jtech-1.0.1/jtech/resources/banner/banner.txt
-drwxr-xr-x   0 angelo    (1000) angelo    (1000)        0 2023-06-26 16:56:51.739652 jtech-1.0.1/jtech/resources/dependencies/
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1695 2023-06-20 18:41:45.000000 jtech-1.0.1/jtech/resources/dependencies/dependencies.json
-drwxr-xr-x   0 angelo    (1000) angelo    (1000)        0 2023-06-26 16:56:51.740652 jtech-1.0.1/jtech/resources/mock/
--rw-r--r--   0 angelo    (1000) angelo    (1000)     2170 2023-06-26 14:52:11.000000 jtech-1.0.1/jtech/resources/mock/http.tar.gz
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1699 2023-06-26 14:52:21.000000 jtech-1.0.1/jtech/resources/mock/mqtt.tar.gz
-drwxr-xr-x   0 angelo    (1000) angelo    (1000)        0 2023-06-26 16:56:51.744652 jtech-1.0.1/jtech/resources/tpl/
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1096 2023-06-15 15:47:48.000000 jtech-1.0.1/jtech/resources/tpl/clean_adapter.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     2176 2023-06-20 16:45:02.000000 jtech-1.0.1/jtech/resources/tpl/clean_api_error.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)      585 2023-06-20 16:46:15.000000 jtech-1.0.1/jtech/resources/tpl/clean_api_sub_error.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1206 2023-06-20 16:47:28.000000 jtech-1.0.1/jtech/resources/tpl/clean_api_validation_error.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1042 2023-06-15 15:47:25.000000 jtech-1.0.1/jtech/resources/tpl/clean_config.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1517 2023-06-20 16:00:46.000000 jtech-1.0.1/jtech/resources/tpl/clean_controller.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1528 2023-06-23 12:50:38.000000 jtech-1.0.1/jtech/resources/tpl/clean_domain.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)      899 2023-06-23 13:22:13.000000 jtech-1.0.1/jtech/resources/tpl/clean_entity.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)      794 2023-06-20 17:40:23.000000 jtech-1.0.1/jtech/resources/tpl/clean_gen_id.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     2375 2023-06-20 16:43:30.000000 jtech-1.0.1/jtech/resources/tpl/clean_global_handler.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)      697 2023-06-15 15:48:21.000000 jtech-1.0.1/jtech/resources/tpl/clean_input_gateway.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1020 2023-06-23 12:26:52.000000 jtech-1.0.1/jtech/resources/tpl/clean_jpa_entity2.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1026 2023-06-22 17:05:47.000000 jtech-1.0.1/jtech/resources/tpl/clean_jpa_entity3.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     4654 2023-06-20 16:34:17.000000 jtech-1.0.1/jtech/resources/tpl/clean_jsons.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1171 2023-06-20 16:42:13.000000 jtech-1.0.1/jtech/resources/tpl/clean_kafka.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1107 2023-06-23 13:20:23.000000 jtech-1.0.1/jtech/resources/tpl/clean_mongo_entity.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     2490 2023-06-20 17:43:39.000000 jtech-1.0.1/jtech/resources/tpl/clean_openapi.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)      701 2023-06-15 15:48:32.000000 jtech-1.0.1/jtech/resources/tpl/clean_output_gateway.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1542 2023-06-22 16:26:15.000000 jtech-1.0.1/jtech/resources/tpl/clean_ready_listener.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     3582 2023-06-20 16:38:23.000000 jtech-1.0.1/jtech/resources/tpl/clean_redis.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)      758 2023-06-15 15:48:41.000000 jtech-1.0.1/jtech/resources/tpl/clean_repository_default.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)      856 2023-06-23 13:09:29.000000 jtech-1.0.1/jtech/resources/tpl/clean_repository_jpa.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)      860 2023-06-23 13:10:31.000000 jtech-1.0.1/jtech/resources/tpl/clean_repository_mongo.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)      974 2023-06-15 15:49:11.000000 jtech-1.0.1/jtech/resources/tpl/clean_request.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1952 2023-06-15 15:49:19.000000 jtech-1.0.1/jtech/resources/tpl/clean_response.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1276 2023-06-15 15:49:29.000000 jtech-1.0.1/jtech/resources/tpl/clean_usecase.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)      728 2023-06-15 19:19:22.000000 jtech-1.0.1/jtech/resources/tpl/cqrs_aggregate.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1003 2023-06-15 19:20:29.000000 jtech-1.0.1/jtech/resources/tpl/cqrs_aggregate_impl.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1424 2023-06-15 19:23:06.000000 jtech-1.0.1/jtech/resources/tpl/cqrs_cmd_controller.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1056 2023-06-15 18:52:17.000000 jtech-1.0.1/jtech/resources/tpl/cqrs_entity.tpl
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1348 2023-06-15 19:01:31.000000 jtech-1.0.1/jtech/resources/tpl/cqrs_qry_controller.tpl
-drwxr-xr-x   0 angelo    (1000) angelo    (1000)        0 2023-06-26 16:56:51.739652 jtech-1.0.1/jtech.egg-info/
--rw-r--r--   0 angelo    (1000) angelo    (1000)      252 2023-06-26 16:56:51.000000 jtech-1.0.1/jtech.egg-info/PKG-INFO
--rw-r--r--   0 angelo    (1000) angelo    (1000)     1673 2023-06-26 16:56:51.000000 jtech-1.0.1/jtech.egg-info/SOURCES.txt
--rw-r--r--   0 angelo    (1000) angelo    (1000)        1 2023-06-26 16:56:51.000000 jtech-1.0.1/jtech.egg-info/dependency_links.txt
--rw-r--r--   0 angelo    (1000) angelo    (1000)       46 2023-06-26 16:56:51.000000 jtech-1.0.1/jtech.egg-info/entry_points.txt
--rw-r--r--   0 angelo    (1000) angelo    (1000)      253 2023-06-26 16:56:51.000000 jtech-1.0.1/jtech.egg-info/requires.txt
--rw-r--r--   0 angelo    (1000) angelo    (1000)        6 2023-06-26 16:56:51.000000 jtech-1.0.1/jtech.egg-info/top_level.txt
--rw-r--r--   0 angelo    (1000) angelo    (1000)      253 2023-06-26 15:39:04.000000 jtech-1.0.1/requirements.txt
--rw-r--r--   0 angelo    (1000) angelo    (1000)       38 2023-06-26 16:56:51.744652 jtech-1.0.1/setup.cfg
--rw-r--r--   0 angelo    (1000) angelo    (1000)      877 2023-06-26 16:56:34.000000 jtech-1.0.1/setup.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:53:20.183574 jtech-1.0.2/jtech/__init__.py
+-rw-r--r--   0        0        0     2255 2023-06-26 16:33:22.667880 jtech-1.0.2/jtech/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:57:41.640049 jtech-1.0.2/jtech/architecture/__init__.py
+-rw-r--r--   0        0        0     5946 2023-06-26 15:01:17.570284 jtech-1.0.2/jtech/architecture/clean_architecture_generator.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:58:05.011675 jtech-1.0.2/jtech/clean_generators/__init__.py
+-rw-r--r--   0        0        0     1143 2023-06-20 16:24:08.670365 jtech-1.0.2/jtech/clean_generators/clean_adapter_generator.py
+-rw-r--r--   0        0        0      866 2023-06-20 17:33:31.654651 jtech-1.0.2/jtech/clean_generators/clean_api_error_generator.py
+-rw-r--r--   0        0        0      879 2023-06-20 17:37:47.222366 jtech-1.0.2/jtech/clean_generators/clean_api_sub_error_generator.py
+-rw-r--r--   0        0        0      907 2023-06-20 17:39:21.310839 jtech-1.0.2/jtech/clean_generators/clean_api_validation_error_generator.py
+-rw-r--r--   0        0        0     1200 2023-06-20 16:24:08.713367 jtech-1.0.2/jtech/clean_generators/clean_config_generator.py
+-rw-r--r--   0        0        0     1277 2023-06-20 16:24:08.730367 jtech-1.0.2/jtech/clean_generators/clean_controller_generator.py
+-rw-r--r--   0        0        0     1158 2023-06-20 16:24:08.675366 jtech-1.0.2/jtech/clean_generators/clean_domain_generator.py
+-rw-r--r--   0        0        0     1911 2023-06-23 18:48:38.519153 jtech-1.0.2/jtech/clean_generators/clean_entity_generator.py
+-rw-r--r--   0        0        0      835 2023-06-20 17:41:06.462602 jtech-1.0.2/jtech/clean_generators/clean_gen_id_generator.py
+-rw-r--r--   0        0        0     8065 2023-06-23 13:37:46.794747 jtech-1.0.2/jtech/clean_generators/clean_generator.py
+-rw-r--r--   0        0        0      916 2023-06-20 17:36:09.141789 jtech-1.0.2/jtech/clean_generators/clean_global_handler_generator.py
+-rw-r--r--   0        0        0     1307 2023-06-20 16:24:08.736367 jtech-1.0.2/jtech/clean_generators/clean_input_gateway_generator.py
+-rw-r--r--   0        0        0      834 2023-06-20 17:42:13.571365 jtech-1.0.2/jtech/clean_generators/clean_jsons_generator.py
+-rw-r--r--   0        0        0      874 2023-06-20 17:30:35.029010 jtech-1.0.2/jtech/clean_generators/clean_kafka_generator.py
+-rw-r--r--   0        0        0      905 2023-06-20 17:43:54.808025 jtech-1.0.2/jtech/clean_generators/clean_openapi_generator.py
+-rw-r--r--   0        0        0     1314 2023-06-20 16:24:08.692366 jtech-1.0.2/jtech/clean_generators/clean_output_gateway_generator.py
+-rw-r--r--   0        0        0      899 2023-06-20 17:46:21.255873 jtech-1.0.2/jtech/clean_generators/clean_ready_event_listener_generator.py
+-rw-r--r--   0        0        0      873 2023-06-20 17:47:43.993047 jtech-1.0.2/jtech/clean_generators/clean_redis_generator.py
+-rw-r--r--   0        0        0     1394 2023-06-20 16:25:42.838850 jtech-1.0.2/jtech/clean_generators/clean_repository_default_generator.py
+-rw-r--r--   0        0        0     1296 2023-06-20 16:24:08.719367 jtech-1.0.2/jtech/clean_generators/clean_repository_jpa_template.py
+-rw-r--r--   0        0        0     1263 2023-06-20 16:24:08.708366 jtech-1.0.2/jtech/clean_generators/clean_repository_mongo_template.py
+-rw-r--r--   0        0        0     1112 2023-06-20 16:24:08.697366 jtech-1.0.2/jtech/clean_generators/clean_request_template.py
+-rw-r--r--   0        0        0     1175 2023-06-20 16:24:08.703366 jtech-1.0.2/jtech/clean_generators/clean_response_template.py
+-rw-r--r--   0        0        0     1176 2023-06-20 16:24:08.687366 jtech-1.0.2/jtech/clean_generators/clean_usecase_template.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:58:17.065998 jtech-1.0.2/jtech/cqrs_generators/__init__.py
+-rw-r--r--   0        0        0     1213 2023-06-19 15:27:17.587214 jtech-1.0.2/jtech/cqrs_generators/cars_controller_template.py
+-rw-r--r--   0        0        0     1100 2023-06-20 16:04:27.456358 jtech-1.0.2/jtech/cqrs_generators/cqrs_aggregator_template.py
+-rw-r--r--   0        0        0     1025 2023-06-19 15:31:21.389627 jtech-1.0.2/jtech/cqrs_generators/cqrs_generator.py
+-rw-r--r--   0        0        0        0 2023-06-19 15:34:07.706004 jtech-1.0.2/jtech/creators/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-14 15:39:52.623663 jtech-1.0.2/jtech/creators/gradle_properties_creator.py
+-rw-r--r--   0        0        0      709 2023-06-14 15:43:22.480067 jtech-1.0.2/jtech/creators/readme_creator.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:00:13.758726 jtech-1.0.2/jtech/docker_compose/__init__.py
+-rw-r--r--   0        0        0     8152 2023-06-26 13:29:59.849326 jtech-1.0.2/jtech/docker_compose/generate_docker_compose.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:37:48.899891 jtech-1.0.2/jtech/manipulate/__init__.py
+-rw-r--r--   0        0        0     7631 2023-06-23 19:08:33.286070 jtech-1.0.2/jtech/manipulate/application_yml_manipulator.py
+-rw-r--r--   0        0        0     4034 2023-06-20 17:15:07.065746 jtech-1.0.2/jtech/manipulate/build_gradle_manipulator.py
+-rw-r--r--   0        0        0     2717 2023-06-20 19:28:16.842650 jtech-1.0.2/jtech/manipulate/java_class_manipulator.py
+-rw-r--r--   0        0        0      976 2023-06-23 19:08:14.046556 jtech-1.0.2/jtech/manipulate/yaml_manipulator.py
+-rw-r--r--   0        0        0        0 2023-06-26 13:36:17.584000 jtech-1.0.2/jtech/mockserver/__init__.py
+-rw-r--r--   0        0        0      586 2023-06-26 15:24:47.248281 jtech-1.0.2/jtech/mockserver/mockserver.py
+-rw-r--r--   0        0        0        0 2023-06-23 14:19:25.872787 jtech-1.0.2/jtech/project/__init__.py
+-rw-r--r--   0        0        0     6671 2023-06-26 13:29:11.648247 jtech-1.0.2/jtech/project/create_project.py
+-rw-r--r--   0        0        0      540 2023-06-23 16:17:26.834452 jtech-1.0.2/jtech/resources/banner/banner.txt
+-rw-r--r--   0        0        0     1695 2023-06-20 18:41:45.182305 jtech-1.0.2/jtech/resources/dependencies/dependencies.json
+-rw-r--r--   0        0        0     2170 2023-06-26 14:52:11.058124 jtech-1.0.2/jtech/resources/mock/http.tar.gz
+-rw-r--r--   0        0        0     1699 2023-06-26 14:52:21.954146 jtech-1.0.2/jtech/resources/mock/mqtt.tar.gz
+-rw-r--r--   0        0        0     1096 2023-06-15 15:47:48.302121 jtech-1.0.2/jtech/resources/tpl/clean_adapter.tpl
+-rw-r--r--   0        0        0     2176 2023-06-20 16:45:02.296425 jtech-1.0.2/jtech/resources/tpl/clean_api_error.tpl
+-rw-r--r--   0        0        0      585 2023-06-20 16:46:15.081344 jtech-1.0.2/jtech/resources/tpl/clean_api_sub_error.tpl
+-rw-r--r--   0        0        0     1206 2023-06-20 16:47:28.810287 jtech-1.0.2/jtech/resources/tpl/clean_api_validation_error.tpl
+-rw-r--r--   0        0        0     1042 2023-06-15 15:47:25.965530 jtech-1.0.2/jtech/resources/tpl/clean_config.tpl
+-rw-r--r--   0        0        0     1517 2023-06-20 16:00:46.105564 jtech-1.0.2/jtech/resources/tpl/clean_controller.tpl
+-rw-r--r--   0        0        0     1528 2023-06-23 12:50:38.457021 jtech-1.0.2/jtech/resources/tpl/clean_domain.tpl
+-rw-r--r--   0        0        0      899 2023-06-23 13:22:13.689725 jtech-1.0.2/jtech/resources/tpl/clean_entity.tpl
+-rw-r--r--   0        0        0      794 2023-06-20 17:40:23.718478 jtech-1.0.2/jtech/resources/tpl/clean_gen_id.tpl
+-rw-r--r--   0        0        0     2375 2023-06-20 16:43:30.448004 jtech-1.0.2/jtech/resources/tpl/clean_global_handler.tpl
+-rw-r--r--   0        0        0      697 2023-06-15 15:48:21.222993 jtech-1.0.2/jtech/resources/tpl/clean_input_gateway.tpl
+-rw-r--r--   0        0        0     1020 2023-06-23 12:26:52.913732 jtech-1.0.2/jtech/resources/tpl/clean_jpa_entity2.tpl
+-rw-r--r--   0        0        0     1026 2023-06-22 17:05:47.475660 jtech-1.0.2/jtech/resources/tpl/clean_jpa_entity3.tpl
+-rw-r--r--   0        0        0     4654 2023-06-20 16:34:17.510426 jtech-1.0.2/jtech/resources/tpl/clean_jsons.tpl
+-rw-r--r--   0        0        0     1171 2023-06-20 16:42:13.632980 jtech-1.0.2/jtech/resources/tpl/clean_kafka.tpl
+-rw-r--r--   0        0        0     1107 2023-06-23 13:20:23.008763 jtech-1.0.2/jtech/resources/tpl/clean_mongo_entity.tpl
+-rw-r--r--   0        0        0     2490 2023-06-20 17:43:39.504623 jtech-1.0.2/jtech/resources/tpl/clean_openapi.tpl
+-rw-r--r--   0        0        0      701 2023-06-15 15:48:32.462291 jtech-1.0.2/jtech/resources/tpl/clean_output_gateway.tpl
+-rw-r--r--   0        0        0     1542 2023-06-22 16:26:15.375485 jtech-1.0.2/jtech/resources/tpl/clean_ready_listener.tpl
+-rw-r--r--   0        0        0     3582 2023-06-20 16:38:23.431913 jtech-1.0.2/jtech/resources/tpl/clean_redis.tpl
+-rw-r--r--   0        0        0      758 2023-06-15 15:48:41.589532 jtech-1.0.2/jtech/resources/tpl/clean_repository_default.tpl
+-rw-r--r--   0        0        0      856 2023-06-23 13:09:29.436274 jtech-1.0.2/jtech/resources/tpl/clean_repository_jpa.tpl
+-rw-r--r--   0        0        0      860 2023-06-23 13:10:31.845943 jtech-1.0.2/jtech/resources/tpl/clean_repository_mongo.tpl
+-rw-r--r--   0        0        0      974 2023-06-15 15:49:11.150315 jtech-1.0.2/jtech/resources/tpl/clean_request.tpl
+-rw-r--r--   0        0        0     1952 2023-06-15 15:49:19.726542 jtech-1.0.2/jtech/resources/tpl/clean_response.tpl
+-rw-r--r--   0        0        0     1276 2023-06-15 15:49:29.709807 jtech-1.0.2/jtech/resources/tpl/clean_usecase.tpl
+-rw-r--r--   0        0        0      728 2023-06-15 19:19:22.686251 jtech-1.0.2/jtech/resources/tpl/cqrs_aggregate.tpl
+-rw-r--r--   0        0        0     1003 2023-06-15 19:20:29.776027 jtech-1.0.2/jtech/resources/tpl/cqrs_aggregate_impl.tpl
+-rw-r--r--   0        0        0     1424 2023-06-15 19:23:06.152169 jtech-1.0.2/jtech/resources/tpl/cqrs_cmd_controller.tpl
+-rw-r--r--   0        0        0     1056 2023-06-15 18:52:17.712070 jtech-1.0.2/jtech/resources/tpl/cqrs_entity.tpl
+-rw-r--r--   0        0        0     1348 2023-06-15 19:01:31.065875 jtech-1.0.2/jtech/resources/tpl/cqrs_qry_controller.tpl
+-rw-r--r--   0        0        0        0 2023-06-19 13:04:59.491638 jtech-1.0.2/jtech/template_processor/__init__.py
+-rw-r--r--   0        0        0      924 2023-06-23 14:11:12.824566 jtech-1.0.2/jtech/template_processor/template_processor.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:37:32.717465 jtech-1.0.2/jtech/utils/__init__.py
+-rw-r--r--   0        0        0      287 2023-06-20 19:39:52.159935 jtech-1.0.2/jtech/utils/file_remove.py
+-rw-r--r--   0        0        0      708 2023-06-26 13:29:05.616237 jtech-1.0.2/jtech/utils/param_configuration.py
+-rw-r--r--   0        0        0      521 2023-06-26 15:18:33.671487 jtech-1.0.2/jtech/utils/tar_gz_extractor.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:35:55.615903 jtech-1.0.2/jtech/webclient/__init__.py
+-rw-r--r--   0        0        0     1119 2023-06-19 17:10:17.936011 jtech-1.0.2/jtech/webclient/spring_boot_client.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:59:40.314234 jtech-1.0.2/jtech/wizards/__init__.py
+-rw-r--r--   0        0        0      575 2023-06-19 16:15:08.306931 jtech-1.0.2/jtech/wizards/architecture_choice_wizard.py
+-rw-r--r--   0        0        0     1248 2023-06-19 16:29:10.214206 jtech-1.0.2/jtech/wizards/checkbox_wizard.py
+-rw-r--r--   0        0        0     1825 2023-06-23 16:39:20.028880 jtech-1.0.2/jtech/wizards/metadata_wizard.py
+-rw-r--r--   0        0        0      741 2023-06-19 16:32:07.309879 jtech-1.0.2/jtech/wizards/project.py
+-rw-r--r--   0        0        0      570 2023-06-20 16:16:32.641378 jtech-1.0.2/jtech/wizards/samples_choice_wizard.py
+-rw-r--r--   0        0        0      503 2023-06-27 13:14:27.070636 jtech-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 jtech-1.0.2/PKG-INFO
```

### Comparing `jtech-1.0.1/jtech/__main__.py` & `jtech-1.0.2/jtech/__main__.py`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/banner/banner.txt` & `jtech-1.0.2/jtech/resources/banner/banner.txt`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/dependencies/dependencies.json` & `jtech-1.0.2/jtech/resources/dependencies/dependencies.json`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/mock/http.tar.gz` & `jtech-1.0.2/jtech/resources/mock/http.tar.gz`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/mock/mqtt.tar.gz` & `jtech-1.0.2/jtech/resources/mock/mqtt.tar.gz`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_adapter.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_adapter.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_api_error.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_api_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_api_sub_error.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_api_sub_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_api_validation_error.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_api_validation_error.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_config.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_config.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_controller.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_controller.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_domain.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_domain.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_entity.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_entity.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_gen_id.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_gen_id.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_global_handler.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_global_handler.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_input_gateway.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_input_gateway.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_jpa_entity2.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_jpa_entity2.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_jpa_entity3.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_jpa_entity3.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_jsons.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_jsons.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_kafka.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_kafka.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_mongo_entity.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_mongo_entity.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_openapi.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_openapi.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_output_gateway.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_output_gateway.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_ready_listener.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_ready_listener.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_redis.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_redis.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_repository_default.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_repository_default.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_repository_jpa.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_repository_jpa.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_repository_mongo.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_repository_mongo.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_request.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_request.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_response.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_response.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/clean_usecase.tpl` & `jtech-1.0.2/jtech/resources/tpl/clean_usecase.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/cqrs_aggregate.tpl` & `jtech-1.0.2/jtech/resources/tpl/cqrs_aggregate.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/cqrs_aggregate_impl.tpl` & `jtech-1.0.2/jtech/resources/tpl/cqrs_aggregate_impl.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/cqrs_cmd_controller.tpl` & `jtech-1.0.2/jtech/resources/tpl/cqrs_cmd_controller.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/cqrs_entity.tpl` & `jtech-1.0.2/jtech/resources/tpl/cqrs_entity.tpl`

 * *Files identical despite different names*

### Comparing `jtech-1.0.1/jtech/resources/tpl/cqrs_qry_controller.tpl` & `jtech-1.0.2/jtech/resources/tpl/cqrs_qry_controller.tpl`

 * *Files identical despite different names*

