# Comparing `tmp/sdc_scissor-2.2.0rc4.tar.gz` & `tmp/sdc_scissor-2.2.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdc_scissor-2.2.0rc4.tar", max compression
+gzip compressed data, was "sdc_scissor-2.2.0rc5.tar", max compression
```

## Comparing `sdc_scissor-2.2.0rc4.tar` & `sdc_scissor-2.2.0rc5.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0    34916 2023-06-27 06:51:34.530924 sdc_scissor-2.2.0rc4/LICENSE.md
--rw-r--r--   0        0        0    10981 2023-06-27 06:51:34.530924 sdc_scissor-2.2.0rc4/README.md
--rw-r--r--   0        0        0     1494 2023-06-27 06:51:34.634924 sdc_scissor-2.2.0rc4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/can_api/__init__.py
--rw-r--r--   0        0        0     4671 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/can_api/can_bus_handler.py
--rw-r--r--   0        0        0     1730 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/can_api/can_msg_generator.py
--rw-r--r--   0        0        0     3907 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/can_api/can_output.py
--rw-r--r--   0        0        0    18875 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/cli.py
--rw-r--r--   0        0        0     1448 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/config.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/__init__.py
--rw-r--r--   0        0        0     4763 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/angle_based_strategy.py
--rw-r--r--   0        0        0     3980 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/equi_distance_strategy.py
--rw-r--r--   0        0        0    10519 2023-06-27 06:51:34.694923 sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/feature_extraction.py
--rw-r--r--   0        0        0     2587 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py
--rw-r--r--   0        0        0     3203 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/road_geometry_calculator.py
--rw-r--r--   0        0        0      401 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/segmentation_strategy.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/machine_learning_api/__init__.py
--rw-r--r--   0        0        0     9597 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py
--rw-r--r--   0        0        0      255 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/machine_learning_api/csv_loader.py
--rw-r--r--   0        0        0     7726 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/machine_learning_api/model_evaluator.py
--rw-r--r--   0        0        0     2382 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/machine_learning_api/predictor.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/__init__.py
--rw-r--r--   0        0        0      643 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/beamng_bump.py
--rw-r--r--   0        0        0      569 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/beamng_delineator.py
--rw-r--r--   0        0        0      764 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/beamng_obstacle_factory.py
--rw-r--r--   0        0        0      675 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/beamng_tree.py
--rw-r--r--   0        0        0      828 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/bump.py
--rw-r--r--   0        0        0      160 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/carla_bump.py
--rw-r--r--   0        0        0      190 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/carla_delineator.py
--rw-r--r--   0        0        0      753 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/carla_obstacle_factory.py
--rw-r--r--   0        0        0      160 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/carla_tree.py
--rw-r--r--   0        0        0      664 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/delineator.py
--rw-r--r--   0        0        0      522 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/obstacle_factory.py
--rw-r--r--   0        0        0      709 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/tree.py
--rw-r--r--   0        0        0      966 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization
--rw-r--r--   0        0        0       95 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/README.md
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/__init__.py
--rw-r--r--   0        0        0      510 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/faultDetection.m
--rw-r--r--   0        0        0     6298 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m
--rw-r--r--   0        0        0      463 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/featureSelection.m
--rw-r--r--   0        0        0      391 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/fitness.m
--rw-r--r--   0        0        0     1075 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/initialPopulation.m
--rw-r--r--   0        0        0      574 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/main.m
--rw-r--r--   0        0        0      609 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/mainGreedy.m
--rw-r--r--   0        0        0      220 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/objectives.m
--rw-r--r--   0        0        0      750 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m
--rw-r--r--   0        0        0     1501 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/permutationMutation.m
--rw-r--r--   0        0        0      302 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/plotResults.m
--rw-r--r--   0        0        0     1367 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py
--rw-r--r--   0        0        0    10251 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R
--rw-r--r--   0        0        0     5034 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf
--rw-r--r--   0        0        0     2128 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv
--rw-r--r--   0        0        0      125 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/medians_APFDc.csv
--rw-r--r--   0        0        0     1869 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/plot.R
--rw-r--r--   0        0        0     1694 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/table.R
--rw-r--r--   0        0        0      395 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/utils.R
--rw-r--r--   0        0        0      584 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv
--rw-r--r--   0        0        0      958 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv
--rw-r--r--   0        0        0     1051 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/runGreedy.m
--rw-r--r--   0        0        0     4258 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/runMOSearch.m
--rw-r--r--   0        0        0     3480 2023-06-27 06:51:34.698923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/runSearch.m
--rw-r--r--   0        0        0   239182 2023-06-27 06:51:34.702924 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv
--rw-r--r--   0        0        0  1146691 2023-06-27 06:51:34.710924 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv
--rw-r--r--   0        0        0   440097 2023-06-27 06:51:34.714923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv
--rw-r--r--   0        0        0     1070 2023-06-27 06:51:34.714923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py
--rw-r--r--   0        0        0   353423 2023-06-27 06:51:34.714923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv
--rw-r--r--   0        0        0      660 2023-06-27 06:51:34.714923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md
--rw-r--r--   0        0        0  1142098 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv
--rw-r--r--   0        0        0     4431 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md
--rwxr-xr-x   0        0        0      650 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh
--rwxr-xr-x   0        0        0      729 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh
--rw-r--r--   0        0        0       65 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/requirements.txt
--rw-r--r--   0        0        0      324 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/setup.cfg
--rw-r--r--   0        0        0       38 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/setup.py
--rw-r--r--   0        0        0     2413 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/README.md
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/__init__.py
--rw-r--r--   0        0        0      780 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py
--rw-r--r--   0        0        0     1306 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py
--rw-r--r--   0        0        0      843 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py
--rw-r--r--   0        0        0     7798 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/run.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/simulator_api/__init__.py
--rw-r--r--   0        0        0     1661 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/simulator_api/abstract_simulator.py
--rw-r--r--   0        0        0     6672 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/simulator_api/beamng_simulator.py
--rw-r--r--   0        0        0      807 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/simulator_api/simulator_factory.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/__init__.py
--rw-r--r--   0        0        0      424 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/road_model.py
--rw-r--r--   0        0        0     2323 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test.py
--rw-r--r--   0        0        0     5482 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generator.py
--rw-r--r--   0        0        0    13513 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py
--rw-r--r--   0        0        0      304 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/duplicate_elimination.py
--rw-r--r--   0        0        0      862 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py
--rw-r--r--   0        0        0    13276 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py
--rw-r--r--   0        0        0     2443 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py
--rw-r--r--   0        0        0     2580 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py
--rw-r--r--   0        0        0     3786 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py
--rw-r--r--   0        0        0      587 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py
--rw-r--r--   0        0        0     8854 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/__init__.py
--rw-r--r--   0        0        0     2829 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py
--rw-r--r--   0        0        0      575 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/config.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/__init__.py
--rw-r--r--   0        0        0     1067 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.718923 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/__init__.py
--rw-r--r--   0        0        0   372723 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/generators/__init__.py
--rw-r--r--   0        0        0     2658 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py
--rw-r--r--   0        0        0     4908 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py
--rw-r--r--   0        0        0    14117 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/utils/__init__.py
--rw-r--r--   0        0        0      731 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/__init__.py
--rw-r--r--   0        0        0     1067 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/__init__.py
--rw-r--r--   0        0        0   372723 2023-06-27 06:51:34.722924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/__init__.py
--rw-r--r--   0        0        0     5693 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py
--rw-r--r--   0        0        0     5135 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py
--rw-r--r--   0        0        0    14499 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py
--rw-r--r--   0        0        0        0 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/__init__.py
--rw-r--r--   0        0        0      694 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py
--rw-r--r--   0        0        0     2762 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_loader.py
--rw-r--r--   0        0        0     6630 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_monitor.py
--rw-r--r--   0        0        0     1843 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_plotter.py
--rw-r--r--   0        0        0     6954 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_runner.py
--rw-r--r--   0        0        0     3150 2023-06-27 06:51:34.726924 sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_validator.py
--rw-r--r--   0        0        0    12115 1970-01-01 00:00:00.000000 sdc_scissor-2.2.0rc4/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-06-27 09:06:17.116606 sdc_scissor-2.2.0rc5/LICENSE.md
+-rw-r--r--   0        0        0    10981 2023-06-27 09:06:17.116606 sdc_scissor-2.2.0rc5/README.md
+-rw-r--r--   0        0        0     1494 2023-06-27 09:06:17.236615 sdc_scissor-2.2.0rc5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/can_api/__init__.py
+-rw-r--r--   0        0        0     4671 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/can_api/can_bus_handler.py
+-rw-r--r--   0        0        0     1730 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/can_api/can_msg_generator.py
+-rw-r--r--   0        0        0     3907 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/can_api/can_output.py
+-rw-r--r--   0        0        0    18875 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/cli.py
+-rw-r--r--   0        0        0     1448 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/config.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/__init__.py
+-rw-r--r--   0        0        0     4763 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/angle_based_strategy.py
+-rw-r--r--   0        0        0     3980 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/equi_distance_strategy.py
+-rw-r--r--   0        0        0    10519 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/feature_extraction.py
+-rw-r--r--   0        0        0     2587 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py
+-rw-r--r--   0        0        0     3203 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/road_geometry_calculator.py
+-rw-r--r--   0        0        0      401 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/segmentation_strategy.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/machine_learning_api/__init__.py
+-rw-r--r--   0        0        0     9597 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py
+-rw-r--r--   0        0        0      255 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/machine_learning_api/csv_loader.py
+-rw-r--r--   0        0        0     7726 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/machine_learning_api/model_evaluator.py
+-rw-r--r--   0        0        0     2382 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/machine_learning_api/predictor.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/beamng_bump.py
+-rw-r--r--   0        0        0      569 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/beamng_delineator.py
+-rw-r--r--   0        0        0      764 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/beamng_obstacle_factory.py
+-rw-r--r--   0        0        0      675 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/beamng_tree.py
+-rw-r--r--   0        0        0      828 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/bump.py
+-rw-r--r--   0        0        0      160 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/carla_bump.py
+-rw-r--r--   0        0        0      190 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/carla_delineator.py
+-rw-r--r--   0        0        0      753 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/carla_obstacle_factory.py
+-rw-r--r--   0        0        0      160 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/carla_tree.py
+-rw-r--r--   0        0        0      664 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/delineator.py
+-rw-r--r--   0        0        0      522 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/obstacle_factory.py
+-rw-r--r--   0        0        0      709 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/tree.py
+-rw-r--r--   0        0        0      966 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization
+-rw-r--r--   0        0        0       95 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/__init__.py
+-rw-r--r--   0        0        0      510 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/faultDetection.m
+-rw-r--r--   0        0        0     6298 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m
+-rw-r--r--   0        0        0      463 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/featureSelection.m
+-rw-r--r--   0        0        0      391 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/fitness.m
+-rw-r--r--   0        0        0     1075 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/initialPopulation.m
+-rw-r--r--   0        0        0      574 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/main.m
+-rw-r--r--   0        0        0      609 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/mainGreedy.m
+-rw-r--r--   0        0        0      220 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/objectives.m
+-rw-r--r--   0        0        0      750 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m
+-rw-r--r--   0        0        0     1501 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/permutationMutation.m
+-rw-r--r--   0        0        0      302 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/plotResults.m
+-rw-r--r--   0        0        0     1367 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py
+-rw-r--r--   0        0        0    10251 2023-06-27 09:06:17.304619 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R
+-rw-r--r--   0        0        0     5034 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf
+-rw-r--r--   0        0        0     2128 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv
+-rw-r--r--   0        0        0      125 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/medians_APFDc.csv
+-rw-r--r--   0        0        0     1869 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/plot.R
+-rw-r--r--   0        0        0     1694 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/table.R
+-rw-r--r--   0        0        0      395 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/utils.R
+-rw-r--r--   0        0        0      584 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv
+-rw-r--r--   0        0        0      958 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv
+-rw-r--r--   0        0        0     1051 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/runGreedy.m
+-rw-r--r--   0        0        0     4258 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/runMOSearch.m
+-rw-r--r--   0        0        0     3480 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/runSearch.m
+-rw-r--r--   0        0        0   239182 2023-06-27 09:06:17.308620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv
+-rw-r--r--   0        0        0  1146691 2023-06-27 09:06:17.320620 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv
+-rw-r--r--   0        0        0   440097 2023-06-27 09:06:17.324621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv
+-rw-r--r--   0        0        0     1070 2023-06-27 09:06:17.324621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py
+-rw-r--r--   0        0        0   353423 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv
+-rw-r--r--   0        0        0      660 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md
+-rw-r--r--   0        0        0  1142098 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv
+-rw-r--r--   0        0        0     4431 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md
+-rwxr-xr-x   0        0        0      650 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh
+-rwxr-xr-x   0        0        0      729 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh
+-rw-r--r--   0        0        0       65 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/requirements.txt
+-rw-r--r--   0        0        0      324 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/setup.cfg
+-rw-r--r--   0        0        0       38 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/setup.py
+-rw-r--r--   0        0        0     2413 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/__init__.py
+-rw-r--r--   0        0        0      780 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py
+-rw-r--r--   0        0        0     1306 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py
+-rw-r--r--   0        0        0      843 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py
+-rw-r--r--   0        0        0     7798 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/run.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/simulator_api/__init__.py
+-rw-r--r--   0        0        0     1661 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/simulator_api/abstract_simulator.py
+-rw-r--r--   0        0        0     6672 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/simulator_api/beamng_simulator.py
+-rw-r--r--   0        0        0      807 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/simulator_api/simulator_factory.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/__init__.py
+-rw-r--r--   0        0        0      424 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/road_model.py
+-rw-r--r--   0        0        0     2323 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test.py
+-rw-r--r--   0        0        0     5482 2023-06-27 09:06:17.328621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generator.py
+-rw-r--r--   0        0        0    13513 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py
+-rw-r--r--   0        0        0      304 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/duplicate_elimination.py
+-rw-r--r--   0        0        0      862 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py
+-rw-r--r--   0        0        0    13276 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py
+-rw-r--r--   0        0        0     2443 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py
+-rw-r--r--   0        0        0     2580 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py
+-rw-r--r--   0        0        0     3786 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py
+-rw-r--r--   0        0        0      587 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py
+-rw-r--r--   0        0        0     8854 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/__init__.py
+-rw-r--r--   0        0        0     2829 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py
+-rw-r--r--   0        0        0      575 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/config.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/__init__.py
+-rw-r--r--   0        0        0     1067 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/__init__.py
+-rw-r--r--   0        0        0   372723 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/generators/__init__.py
+-rw-r--r--   0        0        0     2658 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py
+-rw-r--r--   0        0        0     4908 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py
+-rw-r--r--   0        0        0    14117 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/utils/__init__.py
+-rw-r--r--   0        0        0      731 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/__init__.py
+-rw-r--r--   0        0        0     1067 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.332621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/__init__.py
+-rw-r--r--   0        0        0   372723 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/__init__.py
+-rw-r--r--   0        0        0     5693 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py
+-rw-r--r--   0        0        0     5135 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py
+-rw-r--r--   0        0        0    14499 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py
+-rw-r--r--   0        0        0        0 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/__init__.py
+-rw-r--r--   0        0        0      694 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py
+-rw-r--r--   0        0        0     2762 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_loader.py
+-rw-r--r--   0        0        0     6630 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_monitor.py
+-rw-r--r--   0        0        0     1843 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_plotter.py
+-rw-r--r--   0        0        0     6954 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_runner.py
+-rw-r--r--   0        0        0     3150 2023-06-27 09:06:17.336621 sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_validator.py
+-rw-r--r--   0        0        0    12115 1970-01-01 00:00:00.000000 sdc_scissor-2.2.0rc5/PKG-INFO
```

### Comparing `sdc_scissor-2.2.0rc4/LICENSE.md` & `sdc_scissor-2.2.0rc5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/README.md` & `sdc_scissor-2.2.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/pyproject.toml` & `sdc_scissor-2.2.0rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SDC-Scissor"
-version = "2.2.0-rc.4"
+version = "2.2.0-rc.5"
 description = "A cost-effective test selection for self-driving cars in virtual environments"
 authors = ["Christian Birchler <birchler.chr@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/ChristianBirchler/sdc-scissor"
 documentation = "https://sdc-scissor.readthedocs.io/"
 packages = [
```

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/can_api/can_bus_handler.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/can_api/can_bus_handler.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/can_api/can_msg_generator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/can_api/can_msg_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/can_api/can_output.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/can_api/can_output.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/cli.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/cli.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/config.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/config.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/angle_based_strategy.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/angle_based_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/equi_distance_strategy.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/equi_distance_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/feature_extraction.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/feature_extraction_api/road_geometry_calculator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/feature_extraction_api/road_geometry_calculator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/machine_learning_api/model_evaluator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/machine_learning_api/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/machine_learning_api/predictor.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/machine_learning_api/predictor.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/beamng_bump.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/beamng_bump.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/beamng_delineator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/beamng_delineator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/beamng_obstacle_factory.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/beamng_obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/beamng_tree.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/beamng_tree.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/bump.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/bump.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/carla_obstacle_factory.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/carla_obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/delineator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/delineator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/obstacle_factory.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/obstacle_api/tree.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/obstacle_api/tree.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/initialPopulation.m` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/initialPopulation.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/main.m` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/main.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/mainGreedy.m` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/mainGreedy.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/permutationMutation.m` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/permutationMutation.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/plot.R` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/plot.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/table.R` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/table.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/runGreedy.m` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/runGreedy.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/runMOSearch.m` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/runMOSearch.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/code/runSearch.m` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/code/runSearch.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/README.md` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/sdc_prioritizer/testPrioritization/run.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/sdc_prioritizer/testPrioritization/run.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/simulator_api/abstract_simulator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/simulator_api/abstract_simulator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/simulator_api/beamng_simulator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/simulator_api/beamng_simulator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/simulator_api/simulator_factory.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/simulator_api/simulator_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/ambiegen/config.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/ambiegen/config.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_loader.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_loader.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_monitor.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_plotter.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_plotter.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_runner.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_runner.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/sdc_scissor/testing_api/test_validator.py` & `sdc_scissor-2.2.0rc5/sdc_scissor/testing_api/test_validator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc4/PKG-INFO` & `sdc_scissor-2.2.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdc-scissor
-Version: 2.2.0rc4
+Version: 2.2.0rc5
 Summary: A cost-effective test selection for self-driving cars in virtual environments
 Home-page: https://github.com/ChristianBirchler/sdc-scissor
 License: GPL-3.0-or-later
 Author: Christian Birchler
 Author-email: birchler.chr@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

