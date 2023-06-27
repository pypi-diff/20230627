# Comparing `tmp/sfr-pyrca-1.0.0.tar.gz` & `tmp/sfr-pyrca-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfr-pyrca-1.0.0.tar", last modified: Thu May 18 06:29:27 2023, max compression
+gzip compressed data, was "sfr-pyrca-1.0.1.tar", last modified: Tue Jun 27 02:27:34 2023, max compression
```

## Comparing `sfr-pyrca-1.0.0.tar` & `sfr-pyrca-1.0.1.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.188313 sfr-pyrca-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.188313 sfr-pyrca-1.0.0/pyrca/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/epsilon_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/ht.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/analyzers/rcd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.184312 sfr-pyrca-1.0.0/pyrca/applications/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/applications/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/applications/example/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11586 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/applications/example/rca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/graphs/causal/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/fges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/ges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/lingam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/graphs/causal/pc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/outliers/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/outliers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/outliers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/outliers/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/simulation/data_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.192313 sfr-pyrca-1.0.0/pyrca/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.184312 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/AdjacencyConfusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/ArrowConfusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    25550 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Edges.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    37979 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GeneralGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GraphClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GraphNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Node.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/NodeType.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/NodeVariableType.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/SHD.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/score/
--rw-r--r--   0 runner    (1001) docker     (123)    30361 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/score/LocalScoreFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/score/LocalScoreFunctionClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.184312 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ConstraintBased/
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ConstraintBased/PC.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ScoreBased/
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ScoreBased/GES.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/BackgroundKnowledge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/DAG2CPDAG.py
--rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/GESUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/GraphUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/BackgroundKnowledgeOrientUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28855 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/Helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/Meek.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/SkeletonDiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    18852 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/UCSepset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PDAG2DAG.py
--rw-r--r--   0 runner    (1001) docker     (123)    28846 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/ScoreUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/TXT2GeneralGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/cit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/
--rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.196313 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/
--rwxr-xr-x   0 runner    (1001) docker     (123)    40652 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/DAG.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9236 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/UndirectedGraph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9735 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/BayesianEstimator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7542 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/MLE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12198 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/extern/
--rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/extern/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30221 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/extern/tabulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15811 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/FactorSet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3131 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/continuous/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13912 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/continuous/ContinuousFactor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/continuous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22540 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/CPD.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35423 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/DiscreteFactor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15809 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/JointProbabilityDistribution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/
--rwxr-xr-x   0 runner    (1001) docker     (123)    18453 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/CustomDistribution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19793 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/GaussianDistribution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      830 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/global_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/independencies/
--rwxr-xr-x   0 runner    (1001) docker     (123)    16265 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/independencies/Independencies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/independencies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.200314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5986 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/EliminationOrder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44473 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/ExactInference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8926 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35116 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/BayesianModel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12668 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/ClusterGraph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25489 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/DynamicBayesianNetwork.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17153 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/FactorGraph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4302 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/JunctionTree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29581 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/MarkovModel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      250 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/readwrite/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22279 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/readwrite/BIF.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/readwrite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/utils/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3675 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/utils/state_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/pycausal.py
--rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/rcd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/utils/GraphClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/utils/SkeletonDiscovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.204314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/
--rwxr-xr-x   0 runner    (1001) docker     (123)    83784 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/Acumin-BdPro.otf
--rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/base.css
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/modal.css
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/rca.css
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/resizing.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/upload.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/causal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/causal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/causal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.208314 sfr-pyrca-1.0.0/pyrca/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/pyrca/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-05-18 06:29:27.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-18 06:29:27.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:29:27.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:29:26.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-18 06:29:27.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 06:29:27.000000 sfr-pyrca-1.0.0/sfr_pyrca.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.188313 sfr-pyrca-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/analyzers/test_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/analyzers/test_epsilon_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/analyzers/test_ht.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/analyzers/test_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/analyzers/test_rcd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.188313 sfr-pyrca-1.0.0/tests/applications/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/applications/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-18 06:29:13.000000 sfr-pyrca-1.0.0/tests/applications/example/run_rca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/graphs/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/graphs/test_fges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/graphs/test_ges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/graphs/test_lingam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/graphs/test_pc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/outliers/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/outliers/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/outliers/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/simulation/test_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:29:27.212315 sfr-pyrca-1.0.0/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-18 06:29:14.000000 sfr-pyrca-1.0.0/tests/tools/test_causal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.140974 sfr-pyrca-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-06-27 02:27:34.140974 sfr-pyrca-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.108974 sfr-pyrca-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.108974 sfr-pyrca-1.0.1/pyrca/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.108974 sfr-pyrca-1.0.1/pyrca/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/analyzers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/analyzers/bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/analyzers/epsilon_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/analyzers/ht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/analyzers/random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/analyzers/rcd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.100974 sfr-pyrca-1.0.1/pyrca/applications/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.108974 sfr-pyrca-1.0.1/pyrca/applications/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/applications/example/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11586 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/applications/example/rca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.108974 sfr-pyrca-1.0.1/pyrca/graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/graphs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.112974 sfr-pyrca-1.0.1/pyrca/graphs/causal/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/graphs/causal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/graphs/causal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/graphs/causal/fges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/graphs/causal/ges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/graphs/causal/lingam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/graphs/causal/pc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.112974 sfr-pyrca-1.0.1/pyrca/outliers/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/outliers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/outliers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/outliers/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.112974 sfr-pyrca-1.0.1/pyrca/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/simulation/data_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.112974 sfr-pyrca-1.0.1/pyrca/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.100974 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.116974 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/AdjacencyConfusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/ArrowConfusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25550 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37979 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/GeneralGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/GraphClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/GraphNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/NodeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/NodeVariableType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/SHD.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.116974 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/score/
+-rw-r--r--   0 runner    (1001) docker     (123)    30361 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/score/LocalScoreFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/score/LocalScoreFunctionClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.100974 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.116974 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/search/ConstraintBased/
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/search/ConstraintBased/PC.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.116974 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/search/ScoreBased/
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/search/ScoreBased/GES.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.116974 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/BackgroundKnowledge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/DAG2CPDAG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17718 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/GESUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/GraphUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.120974 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/BackgroundKnowledgeOrientUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28855 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/Helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/Meek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/SkeletonDiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18852 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/UCSepset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PDAG2DAG.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28846 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/ScoreUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/TXT2GeneralGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/cit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.120974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.120974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/base/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40652 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/base/DAG.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9236 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/base/UndirectedGraph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      118 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.120974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/estimators/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9735 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/estimators/BayesianEstimator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7542 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/estimators/MLE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/estimators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12198 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/estimators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.120974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/extern/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/extern/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30221 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/extern/tabulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.120974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15811 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/FactorSet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3131 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.120974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/continuous/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13912 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/continuous/ContinuousFactor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/continuous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.124974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/discrete/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22540 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/discrete/CPD.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35423 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/discrete/DiscreteFactor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15809 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/discrete/JointProbabilityDistribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/discrete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.124974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/distributions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18453 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/distributions/CustomDistribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19793 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/distributions/GaussianDistribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/distributions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      841 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/distributions/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      830 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/global_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.124974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/independencies/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16265 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/independencies/Independencies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/independencies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.124974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/inference/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5986 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/inference/EliminationOrder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44473 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/inference/ExactInference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8926 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/inference/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.128974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35116 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/BayesianModel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12668 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/ClusterGraph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25489 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/DynamicBayesianNetwork.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17153 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/FactorGraph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4302 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/JunctionTree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29581 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/MarkovModel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      250 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.128974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/readwrite/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22279 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/readwrite/BIF.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/readwrite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.128974 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/utils/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3675 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/utils/state_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.128974 sfr-pyrca-1.0.1/pyrca/thirdparty/pycausal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pycausal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pycausal/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pycausal/pycausal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/pycausal/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.128974 sfr-pyrca-1.0.1/pyrca/thirdparty/rcd/
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/rcd/rcd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.128974 sfr-pyrca-1.0.1/pyrca/thirdparty/rcd/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/rcd/utils/GraphClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/thirdparty/rcd/utils/SkeletonDiscovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.128974 sfr-pyrca-1.0.1/pyrca/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.128974 sfr-pyrca-1.0.1/pyrca/tools/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.132974 sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    83784 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/Acumin-BdPro.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/modal.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/rca.css
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/resizing.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.132974 sfr-pyrca-1.0.1/pyrca/tools/dashboard/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/callbacks/causal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/callbacks/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.132974 sfr-pyrca-1.0.1/pyrca/tools/dashboard/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/models/causal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/models/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.132974 sfr-pyrca-1.0.1/pyrca/tools/dashboard/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/pages/causal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/pages/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/pages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.136974 sfr-pyrca-1.0.1/pyrca/tools/dashboard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/tools/dashboard/utils/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.136974 sfr-pyrca-1.0.1/pyrca/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/utils/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/pyrca/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 02:27:34.140974 sfr-pyrca-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.136974 sfr-pyrca-1.0.1/sfr_pyrca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-06-27 02:27:34.000000 sfr-pyrca-1.0.1/sfr_pyrca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-27 02:27:34.000000 sfr-pyrca-1.0.1/sfr_pyrca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 02:27:34.000000 sfr-pyrca-1.0.1/sfr_pyrca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 02:27:33.000000 sfr-pyrca-1.0.1/sfr_pyrca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 02:27:34.000000 sfr-pyrca-1.0.1/sfr_pyrca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-27 02:27:34.000000 sfr-pyrca-1.0.1/sfr_pyrca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.104974 sfr-pyrca-1.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.140974 sfr-pyrca-1.0.1/tests/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/analyzers/test_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/analyzers/test_epsilon_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/analyzers/test_ht.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/analyzers/test_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/analyzers/test_rcd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.104974 sfr-pyrca-1.0.1/tests/applications/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.140974 sfr-pyrca-1.0.1/tests/applications/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/applications/example/run_rca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.140974 sfr-pyrca-1.0.1/tests/graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/graphs/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/graphs/test_fges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/graphs/test_ges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/graphs/test_lingam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/graphs/test_pc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.140974 sfr-pyrca-1.0.1/tests/outliers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/outliers/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/outliers/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.140974 sfr-pyrca-1.0.1/tests/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/simulation/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 02:27:34.140974 sfr-pyrca-1.0.1/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-27 02:27:20.000000 sfr-pyrca-1.0.1/tests/tools/test_causal.py
```

### Comparing `sfr-pyrca-1.0.0/LICENSE` & `sfr-pyrca-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/PKG-INFO` & `sfr-pyrca-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfr-pyrca
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyRCA: A Python library for Root Cause Analysis
 Home-page: https://github.com/salesforce/PyRCA
 Author: Salesforce Research Warden AIOps
 License: 3-Clause BSD
 Keywords: AIOps RCA root cause analysis
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
@@ -16,30 +16,30 @@
 <div align="center">
   <a href="#">
   <img src="https://img.shields.io/badge/Python-3.7, 3.8, 3.9-blue">
   </a>
   <a href="https://pypi.python.org/pypi/sfr-pyrca">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/sfr-pyrca.svg"/>
   </a>
-  <a href="https://fuzzy-disco-r42n6p1.pages.github.io">
+  <a href="https://opensource.salesforce.com/PyRCA/">
   <img alt="Documentation" src="https://github.com/salesforce/PyRCA/actions/workflows/docs.yml/badge.svg"/>
   </a>
   <a href="https://pepy.tech/project/sfr-pyrca">
   <img alt="Downloads" src="https://pepy.tech/badge/sfr-pyrca">
   </a>
-  <a href="https://arxiv.org/abs/xxxx.xxxxx">
-  <img alt="DOI" src="https://zenodo.org/badge/DOI/10.48550/ARXIV.xxxx.xxxxx.svg"/>
+  <a href="https://arxiv.org/abs/2306.11417">
+  <img alt="DOI" src="https://zenodo.org/badge/DOI/10.48550/ARXIV.2306.11417.svg"/>
   </a>
 </div>
 
 ## Table of Contents
 1. [Introduction](#introduction)
 2. [Installation](#installation)
 3. [Getting Started](#getting-started)
-4. [Documentation](https://fuzzy-disco-r42n6p1.pages.github.io/)
+4. [Documentation](https://opensource.salesforce.com/PyRCA/)
 5. [Tutorial](https://github.com/salesforce/PyRCA/tree/main/examples)
 6. [Example](#application-example)
 7. [Benchmarks](#benchmarks)
 8. [How to Contribute](#how-to-contribute)
 
 ## Introduction
 
@@ -136,15 +136,15 @@
 ```
 
 where ``abnormal_data`` is the time series data collected in an incident window.
 
 As mentioned above, some RCA methods such as ``BayesianNetwork`` require causal graphs as their inputs. To construct such causal
 graphs from the observed time series data, you can utilize our tool by running ``python -m pyrca.tools``.
 This command will launch a Dash app for time series data analysis and causal discovery.
-![alt text](https://github.com/salesforce/PyRCA/raw/main/docs/_static/dashboard.png)
+![alt text](https://github.com/salesforce/PyRCA/raw/main/docs/_static/dashboard_gif.gif)
 
 The dashboard enables users to experiment with different causal discovery methods, customize causal discovery 
 parameters, add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required links), and visualize 
 the generated causal graphs. This feature simplifies the process of manually revising causal graphs based on 
 domain knowledge. Users can download the graph generated by this tool if they are satisfied with it. The graph 
 can then be used by the RCA methods supported in PyRCA.
```

#### html2text {}

```diff
@@ -1,69 +1,69 @@
-Metadata-Version: 2.1 Name: sfr-pyrca Version: 1.0.0 Summary: PyRCA: A Python
+Metadata-Version: 2.1 Name: sfr-pyrca Version: 1.0.1 Summary: PyRCA: A Python
 library for Root Cause Analysis Home-page: https://github.com/salesforce/PyRCA
 Author: Salesforce Research Warden AIOps License: 3-Clause BSD Keywords: AIOps
 RCA root cause analysis Requires-Python: >=3.7,<4 Description-Content-Type:
 text/markdown Provides-Extra: plot Provides-Extra: all License-File: LICENSE #
 PyRCA: A Python library for Root Cause Analysis
 [https://img.shields.io/badge/Python-3.7,_3.8,_3.9-blue] [PyPI] [Documentation]
                                [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
-(https://fuzzy-disco-r42n6p1.pages.github.io/) 5. [Tutorial](https://
-github.com/salesforce/PyRCA/tree/main/examples) 6. [Example](#application-
-example) 7. [Benchmarks](#benchmarks) 8. [How to Contribute](#how-to-
-contribute) ## Introduction The adoption of microservices architectures is
-growing at a rapid pace, making multi-service applications the standard
-paradigm in real-world IT applications. Typically, a multi-service application
-consists of hundreds of interacting services, making it increasingly
-challenging to detect service failures and identify their root causes. Root
-cause analysis (RCA) methods typically rely on KPI metrics, traces, or logs
-monitored on these services to determine the root causes when a system failure
-is detected. Such methods can aid engineers and SREs in the troubleshooting
-process. PyRCA is a Python machine-learning library designed to facilitate root
-cause analysis by offering various state-of-the-art RCA algorithms and an end-
-to-end pipeline for building RCA solutions. At present, PyRCA primarily focuses
-on metric-based RCA, including two types of algorithms: (1) identifying
-anomalous metrics in parallel with the observed anomaly through metric data
-analysis, such as Îµ-diagnosis, and (2) identifying root causes based on a
-topology/causal graph representing the causal relationships between the
-observed metrics, such as Bayesian inference and Random Walk. PyRCA also
-provides a convenient tool for building causal graphs from the observed time
-series data and domain knowledge, enabling users to develop graph-based
-solutions quickly. Furthermore, PyRCA offers a benchmark for evaluating various
-RCA methods, which is valuable for industry and academic research. The
-following list shows the supported RCA methods in our library: 1. [Îµ-
-Diagnosis](https://dl.acm.org/doi/10.1145/3308558.3313653) 2. Bayesian
-Inference-based RCA (BI) 3. Random Walk-based RCA (RW) 4. [Root Casue Discovery
-method (RCD)](https://openreview.net/pdf?id=weoLjoYFvXY) 5. [Hypothesis
-Testing-based RCA (HT)](https://dl.acm.org/doi/10.1145/3534678.3539041) We will
-continue improving this library to make it more comprehensive in the future. In
-the future, PyRCA will support trace and log-based RCA methods as well. ##
-Installation You can install ``pyrca`` from PyPI by calling ``pip install sfr-
-pyrca``. You may install from source by cloning the PyRCA repo, navigating to
-the root directory, and calling ``pip install .``, or ``pip install -e .`` to
-install in editable mode. You may install additional dependencies: - **For
-plotting & visualization**: Calling ``pip install sfr-pyrca[plot]``, or ``pip
-install .[plot]`` from the root directory of the repo. - **Install all the
-dependencies**: Calling ``pip install sfr-pyrca[all]``, or ``pip install .
-[all]`` from the root directory of the repo. ## Getting Started PyRCA provides
-a unified interface for training RCA models and finding root causes. To apply a
-certain RCA method, you only need to specify: - **The selected RCA method**:
-e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``. - **The method
-configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. -
-**Time series data for initialization/training**: e.g., A time series data in a
-pandas dataframe. - **Abnormal time series data in an incident window**: The
-RCA methods require the anomalous KPI metrics in an incident window. Let's take
-``BayesianNetwork`` as an example. Suppose that ``graph_df`` is the pandas
-dataframe of a graph representing the causal relationships between metrics (how
-to construct such causal graph will be discussed later), and ``df`` is the
-pandas dataframe containing the historical observed time series data (e.g., the
-index is the timestamp and each column represents one monitored metric). To
-train a ``BayesianNetwork``, you can simply run the following code: ```python
-from pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
+(https://opensource.salesforce.com/PyRCA/) 5. [Tutorial](https://github.com/
+salesforce/PyRCA/tree/main/examples) 6. [Example](#application-example) 7.
+[Benchmarks](#benchmarks) 8. [How to Contribute](#how-to-contribute) ##
+Introduction The adoption of microservices architectures is growing at a rapid
+pace, making multi-service applications the standard paradigm in real-world IT
+applications. Typically, a multi-service application consists of hundreds of
+interacting services, making it increasingly challenging to detect service
+failures and identify their root causes. Root cause analysis (RCA) methods
+typically rely on KPI metrics, traces, or logs monitored on these services to
+determine the root causes when a system failure is detected. Such methods can
+aid engineers and SREs in the troubleshooting process. PyRCA is a Python
+machine-learning library designed to facilitate root cause analysis by offering
+various state-of-the-art RCA algorithms and an end-to-end pipeline for building
+RCA solutions. At present, PyRCA primarily focuses on metric-based RCA,
+including two types of algorithms: (1) identifying anomalous metrics in
+parallel with the observed anomaly through metric data analysis, such as Îµ-
+diagnosis, and (2) identifying root causes based on a topology/causal graph
+representing the causal relationships between the observed metrics, such as
+Bayesian inference and Random Walk. PyRCA also provides a convenient tool for
+building causal graphs from the observed time series data and domain knowledge,
+enabling users to develop graph-based solutions quickly. Furthermore, PyRCA
+offers a benchmark for evaluating various RCA methods, which is valuable for
+industry and academic research. The following list shows the supported RCA
+methods in our library: 1. [Îµ-Diagnosis](https://dl.acm.org/doi/10.1145/
+3308558.3313653) 2. Bayesian Inference-based RCA (BI) 3. Random Walk-based RCA
+(RW) 4. [Root Casue Discovery method (RCD)](https://openreview.net/
+pdf?id=weoLjoYFvXY) 5. [Hypothesis Testing-based RCA (HT)](https://dl.acm.org/
+doi/10.1145/3534678.3539041) We will continue improving this library to make it
+more comprehensive in the future. In the future, PyRCA will support trace and
+log-based RCA methods as well. ## Installation You can install ``pyrca`` from
+PyPI by calling ``pip install sfr-pyrca``. You may install from source by
+cloning the PyRCA repo, navigating to the root directory, and calling ``pip
+install .``, or ``pip install -e .`` to install in editable mode. You may
+install additional dependencies: - **For plotting & visualization**: Calling
+``pip install sfr-pyrca[plot]``, or ``pip install .[plot]`` from the root
+directory of the repo. - **Install all the dependencies**: Calling ``pip
+install sfr-pyrca[all]``, or ``pip install .[all]`` from the root directory of
+the repo. ## Getting Started PyRCA provides a unified interface for training
+RCA models and finding root causes. To apply a certain RCA method, you only
+need to specify: - **The selected RCA method**: e.g., ``BayesianNetwork``,
+``EpsilonDiagnosis``. - **The method configuration**: e.g.,
+``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. - **Time series data for
+initialization/training**: e.g., A time series data in a pandas dataframe. -
+**Abnormal time series data in an incident window**: The RCA methods require
+the anomalous KPI metrics in an incident window. Let's take ``BayesianNetwork``
+as an example. Suppose that ``graph_df`` is the pandas dataframe of a graph
+representing the causal relationships between metrics (how to construct such
+causal graph will be discussed later), and ``df`` is the pandas dataframe
+containing the historical observed time series data (e.g., the index is the
+timestamp and each column represents one monitored metric). To train a
+``BayesianNetwork``, you can simply run the following code: ```python from
+pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
 (config=BayesianNetwork.config_class(graph=graph_df)) model.train(df)
 model.save("model_folder") ``` After the model is trained, you can use it to
 find root causes of an incident given a list of anomalous metrics detected by a
 certain anomaly detector (you can use the stats-based detector supported in
 PyRCA or other anomaly detection methods supported by our [Merlion](https://
 github.com/salesforce/Merlion) library), e.g., ```python from
 pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork.load
@@ -78,15 +78,15 @@
 ```python results = model.find_root_causes(abnormal_data) print(results.to_dict
 ()) ``` where ``abnormal_data`` is the time series data collected in an
 incident window. As mentioned above, some RCA methods such as
 ``BayesianNetwork`` require causal graphs as their inputs. To construct such
 causal graphs from the observed time series data, you can utilize our tool by
 running ``python -m pyrca.tools``. This command will launch a Dash app for time
 series data analysis and causal discovery. ![alt text](https://github.com/
-salesforce/PyRCA/raw/main/docs/_static/dashboard.png) The dashboard enables
+salesforce/PyRCA/raw/main/docs/_static/dashboard_gif.gif) The dashboard enables
 users to experiment with different causal discovery methods, customize causal
 discovery parameters, add domain knowledge constraints (e.g., root/leaf nodes,
 forbidden/required links), and visualize the generated causal graphs. This
 feature simplifies the process of manually revising causal graphs based on
 domain knowledge. Users can download the graph generated by this tool if they
 are satisfied with it. The graph can then be used by the RCA methods supported
 in PyRCA. Alternatively, users can write code to build such graphs instead of
```

### Comparing `sfr-pyrca-1.0.0/README.md` & `sfr-pyrca-1.0.1/sfr_pyrca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,45 @@
+Metadata-Version: 2.1
+Name: sfr-pyrca
+Version: 1.0.1
+Summary: PyRCA: A Python library for Root Cause Analysis
+Home-page: https://github.com/salesforce/PyRCA
+Author: Salesforce Research Warden AIOps
+License: 3-Clause BSD
+Keywords: AIOps RCA root cause analysis
+Requires-Python: >=3.7,<4
+Description-Content-Type: text/markdown
+Provides-Extra: plot
+Provides-Extra: all
+License-File: LICENSE
+
 # PyRCA: A Python library for Root Cause Analysis
 <div align="center">
   <a href="#">
   <img src="https://img.shields.io/badge/Python-3.7, 3.8, 3.9-blue">
   </a>
   <a href="https://pypi.python.org/pypi/sfr-pyrca">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/sfr-pyrca.svg"/>
   </a>
-  <a href="https://fuzzy-disco-r42n6p1.pages.github.io">
+  <a href="https://opensource.salesforce.com/PyRCA/">
   <img alt="Documentation" src="https://github.com/salesforce/PyRCA/actions/workflows/docs.yml/badge.svg"/>
   </a>
   <a href="https://pepy.tech/project/sfr-pyrca">
   <img alt="Downloads" src="https://pepy.tech/badge/sfr-pyrca">
   </a>
-  <a href="https://arxiv.org/abs/xxxx.xxxxx">
-  <img alt="DOI" src="https://zenodo.org/badge/DOI/10.48550/ARXIV.xxxx.xxxxx.svg"/>
+  <a href="https://arxiv.org/abs/2306.11417">
+  <img alt="DOI" src="https://zenodo.org/badge/DOI/10.48550/ARXIV.2306.11417.svg"/>
   </a>
 </div>
 
 ## Table of Contents
 1. [Introduction](#introduction)
 2. [Installation](#installation)
 3. [Getting Started](#getting-started)
-4. [Documentation](https://fuzzy-disco-r42n6p1.pages.github.io/)
+4. [Documentation](https://opensource.salesforce.com/PyRCA/)
 5. [Tutorial](https://github.com/salesforce/PyRCA/tree/main/examples)
 6. [Example](#application-example)
 7. [Benchmarks](#benchmarks)
 8. [How to Contribute](#how-to-contribute)
 
 ## Introduction
 
@@ -122,15 +136,15 @@
 ```
 
 where ``abnormal_data`` is the time series data collected in an incident window.
 
 As mentioned above, some RCA methods such as ``BayesianNetwork`` require causal graphs as their inputs. To construct such causal
 graphs from the observed time series data, you can utilize our tool by running ``python -m pyrca.tools``.
 This command will launch a Dash app for time series data analysis and causal discovery.
-![alt text](https://github.com/salesforce/PyRCA/raw/main/docs/_static/dashboard.png)
+![alt text](https://github.com/salesforce/PyRCA/raw/main/docs/_static/dashboard_gif.gif)
 
 The dashboard enables users to experiment with different causal discovery methods, customize causal discovery 
 parameters, add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required links), and visualize 
 the generated causal graphs. This feature simplifies the process of manually revising causal graphs based on 
 domain knowledge. Users can download the graph generated by this tool if they are satisfied with it. The graph 
 can then be used by the RCA methods supported in PyRCA.
```

#### html2text {}

```diff
@@ -1,64 +1,69 @@
-# PyRCA: A Python library for Root Cause Analysis
+Metadata-Version: 2.1 Name: sfr-pyrca Version: 1.0.1 Summary: PyRCA: A Python
+library for Root Cause Analysis Home-page: https://github.com/salesforce/PyRCA
+Author: Salesforce Research Warden AIOps License: 3-Clause BSD Keywords: AIOps
+RCA root cause analysis Requires-Python: >=3.7,<4 Description-Content-Type:
+text/markdown Provides-Extra: plot Provides-Extra: all License-File: LICENSE #
+PyRCA: A Python library for Root Cause Analysis
 [https://img.shields.io/badge/Python-3.7,_3.8,_3.9-blue] [PyPI] [Documentation]
                                [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
-(https://fuzzy-disco-r42n6p1.pages.github.io/) 5. [Tutorial](https://
-github.com/salesforce/PyRCA/tree/main/examples) 6. [Example](#application-
-example) 7. [Benchmarks](#benchmarks) 8. [How to Contribute](#how-to-
-contribute) ## Introduction The adoption of microservices architectures is
-growing at a rapid pace, making multi-service applications the standard
-paradigm in real-world IT applications. Typically, a multi-service application
-consists of hundreds of interacting services, making it increasingly
-challenging to detect service failures and identify their root causes. Root
-cause analysis (RCA) methods typically rely on KPI metrics, traces, or logs
-monitored on these services to determine the root causes when a system failure
-is detected. Such methods can aid engineers and SREs in the troubleshooting
-process. PyRCA is a Python machine-learning library designed to facilitate root
-cause analysis by offering various state-of-the-art RCA algorithms and an end-
-to-end pipeline for building RCA solutions. At present, PyRCA primarily focuses
-on metric-based RCA, including two types of algorithms: (1) identifying
-anomalous metrics in parallel with the observed anomaly through metric data
-analysis, such as Îµ-diagnosis, and (2) identifying root causes based on a
-topology/causal graph representing the causal relationships between the
-observed metrics, such as Bayesian inference and Random Walk. PyRCA also
-provides a convenient tool for building causal graphs from the observed time
-series data and domain knowledge, enabling users to develop graph-based
-solutions quickly. Furthermore, PyRCA offers a benchmark for evaluating various
-RCA methods, which is valuable for industry and academic research. The
-following list shows the supported RCA methods in our library: 1. [Îµ-
-Diagnosis](https://dl.acm.org/doi/10.1145/3308558.3313653) 2. Bayesian
-Inference-based RCA (BI) 3. Random Walk-based RCA (RW) 4. [Root Casue Discovery
-method (RCD)](https://openreview.net/pdf?id=weoLjoYFvXY) 5. [Hypothesis
-Testing-based RCA (HT)](https://dl.acm.org/doi/10.1145/3534678.3539041) We will
-continue improving this library to make it more comprehensive in the future. In
-the future, PyRCA will support trace and log-based RCA methods as well. ##
-Installation You can install ``pyrca`` from PyPI by calling ``pip install sfr-
-pyrca``. You may install from source by cloning the PyRCA repo, navigating to
-the root directory, and calling ``pip install .``, or ``pip install -e .`` to
-install in editable mode. You may install additional dependencies: - **For
-plotting & visualization**: Calling ``pip install sfr-pyrca[plot]``, or ``pip
-install .[plot]`` from the root directory of the repo. - **Install all the
-dependencies**: Calling ``pip install sfr-pyrca[all]``, or ``pip install .
-[all]`` from the root directory of the repo. ## Getting Started PyRCA provides
-a unified interface for training RCA models and finding root causes. To apply a
-certain RCA method, you only need to specify: - **The selected RCA method**:
-e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``. - **The method
-configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. -
-**Time series data for initialization/training**: e.g., A time series data in a
-pandas dataframe. - **Abnormal time series data in an incident window**: The
-RCA methods require the anomalous KPI metrics in an incident window. Let's take
-``BayesianNetwork`` as an example. Suppose that ``graph_df`` is the pandas
-dataframe of a graph representing the causal relationships between metrics (how
-to construct such causal graph will be discussed later), and ``df`` is the
-pandas dataframe containing the historical observed time series data (e.g., the
-index is the timestamp and each column represents one monitored metric). To
-train a ``BayesianNetwork``, you can simply run the following code: ```python
-from pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
+(https://opensource.salesforce.com/PyRCA/) 5. [Tutorial](https://github.com/
+salesforce/PyRCA/tree/main/examples) 6. [Example](#application-example) 7.
+[Benchmarks](#benchmarks) 8. [How to Contribute](#how-to-contribute) ##
+Introduction The adoption of microservices architectures is growing at a rapid
+pace, making multi-service applications the standard paradigm in real-world IT
+applications. Typically, a multi-service application consists of hundreds of
+interacting services, making it increasingly challenging to detect service
+failures and identify their root causes. Root cause analysis (RCA) methods
+typically rely on KPI metrics, traces, or logs monitored on these services to
+determine the root causes when a system failure is detected. Such methods can
+aid engineers and SREs in the troubleshooting process. PyRCA is a Python
+machine-learning library designed to facilitate root cause analysis by offering
+various state-of-the-art RCA algorithms and an end-to-end pipeline for building
+RCA solutions. At present, PyRCA primarily focuses on metric-based RCA,
+including two types of algorithms: (1) identifying anomalous metrics in
+parallel with the observed anomaly through metric data analysis, such as Îµ-
+diagnosis, and (2) identifying root causes based on a topology/causal graph
+representing the causal relationships between the observed metrics, such as
+Bayesian inference and Random Walk. PyRCA also provides a convenient tool for
+building causal graphs from the observed time series data and domain knowledge,
+enabling users to develop graph-based solutions quickly. Furthermore, PyRCA
+offers a benchmark for evaluating various RCA methods, which is valuable for
+industry and academic research. The following list shows the supported RCA
+methods in our library: 1. [Îµ-Diagnosis](https://dl.acm.org/doi/10.1145/
+3308558.3313653) 2. Bayesian Inference-based RCA (BI) 3. Random Walk-based RCA
+(RW) 4. [Root Casue Discovery method (RCD)](https://openreview.net/
+pdf?id=weoLjoYFvXY) 5. [Hypothesis Testing-based RCA (HT)](https://dl.acm.org/
+doi/10.1145/3534678.3539041) We will continue improving this library to make it
+more comprehensive in the future. In the future, PyRCA will support trace and
+log-based RCA methods as well. ## Installation You can install ``pyrca`` from
+PyPI by calling ``pip install sfr-pyrca``. You may install from source by
+cloning the PyRCA repo, navigating to the root directory, and calling ``pip
+install .``, or ``pip install -e .`` to install in editable mode. You may
+install additional dependencies: - **For plotting & visualization**: Calling
+``pip install sfr-pyrca[plot]``, or ``pip install .[plot]`` from the root
+directory of the repo. - **Install all the dependencies**: Calling ``pip
+install sfr-pyrca[all]``, or ``pip install .[all]`` from the root directory of
+the repo. ## Getting Started PyRCA provides a unified interface for training
+RCA models and finding root causes. To apply a certain RCA method, you only
+need to specify: - **The selected RCA method**: e.g., ``BayesianNetwork``,
+``EpsilonDiagnosis``. - **The method configuration**: e.g.,
+``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. - **Time series data for
+initialization/training**: e.g., A time series data in a pandas dataframe. -
+**Abnormal time series data in an incident window**: The RCA methods require
+the anomalous KPI metrics in an incident window. Let's take ``BayesianNetwork``
+as an example. Suppose that ``graph_df`` is the pandas dataframe of a graph
+representing the causal relationships between metrics (how to construct such
+causal graph will be discussed later), and ``df`` is the pandas dataframe
+containing the historical observed time series data (e.g., the index is the
+timestamp and each column represents one monitored metric). To train a
+``BayesianNetwork``, you can simply run the following code: ```python from
+pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
 (config=BayesianNetwork.config_class(graph=graph_df)) model.train(df)
 model.save("model_folder") ``` After the model is trained, you can use it to
 find root causes of an incident given a list of anomalous metrics detected by a
 certain anomaly detector (you can use the stats-based detector supported in
 PyRCA or other anomaly detection methods supported by our [Merlion](https://
 github.com/salesforce/Merlion) library), e.g., ```python from
 pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork.load
@@ -73,15 +78,15 @@
 ```python results = model.find_root_causes(abnormal_data) print(results.to_dict
 ()) ``` where ``abnormal_data`` is the time series data collected in an
 incident window. As mentioned above, some RCA methods such as
 ``BayesianNetwork`` require causal graphs as their inputs. To construct such
 causal graphs from the observed time series data, you can utilize our tool by
 running ``python -m pyrca.tools``. This command will launch a Dash app for time
 series data analysis and causal discovery. ![alt text](https://github.com/
-salesforce/PyRCA/raw/main/docs/_static/dashboard.png) The dashboard enables
+salesforce/PyRCA/raw/main/docs/_static/dashboard_gif.gif) The dashboard enables
 users to experiment with different causal discovery methods, customize causal
 discovery parameters, add domain knowledge constraints (e.g., root/leaf nodes,
 forbidden/required links), and visualize the generated causal graphs. This
 feature simplifies the process of manually revising causal graphs based on
 domain knowledge. Users can download the graph generated by this tool if they
 are satisfied with it. The graph can then be used by the RCA methods supported
 in PyRCA. Alternatively, users can write code to build such graphs instead of
```

### Comparing `sfr-pyrca-1.0.0/docs/conf.py` & `sfr-pyrca-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/analyzers/base.py` & `sfr-pyrca-1.0.1/pyrca/analyzers/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/analyzers/bayesian.py` & `sfr-pyrca-1.0.1/pyrca/analyzers/bayesian.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/analyzers/epsilon_diagnosis.py` & `sfr-pyrca-1.0.1/pyrca/analyzers/epsilon_diagnosis.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/analyzers/ht.py` & `sfr-pyrca-1.0.1/pyrca/analyzers/ht.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/analyzers/random_walk.py` & `sfr-pyrca-1.0.1/pyrca/analyzers/random_walk.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/analyzers/rcd.py` & `sfr-pyrca-1.0.1/pyrca/analyzers/rcd.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/applications/example/dataset.py` & `sfr-pyrca-1.0.1/pyrca/applications/example/dataset.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/applications/example/rca.py` & `sfr-pyrca-1.0.1/pyrca/applications/example/rca.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/base.py` & `sfr-pyrca-1.0.1/pyrca/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/graphs/causal/base.py` & `sfr-pyrca-1.0.1/pyrca/graphs/causal/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/graphs/causal/fges.py` & `sfr-pyrca-1.0.1/pyrca/graphs/causal/fges.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/graphs/causal/ges.py` & `sfr-pyrca-1.0.1/pyrca/graphs/causal/ges.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/graphs/causal/lingam.py` & `sfr-pyrca-1.0.1/pyrca/graphs/causal/lingam.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/graphs/causal/pc.py` & `sfr-pyrca-1.0.1/pyrca/graphs/causal/pc.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/outliers/base.py` & `sfr-pyrca-1.0.1/pyrca/outliers/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/outliers/stats.py` & `sfr-pyrca-1.0.1/pyrca/outliers/stats.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/simulation/data_gen.py` & `sfr-pyrca-1.0.1/pyrca/simulation/data_gen.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/AdjacencyConfusion.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/AdjacencyConfusion.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/ArrowConfusion.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/ArrowConfusion.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Dag.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Dag.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Edge.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Edge.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Edges.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Edges.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Endpoint.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Endpoint.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GeneralGraph.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/GeneralGraph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Graph.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Graph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GraphClass.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/GraphClass.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/GraphNode.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/GraphNode.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/Node.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/Node.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/graph/SHD.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/graph/SHD.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/score/LocalScoreFunction.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/score/LocalScoreFunction.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/score/LocalScoreFunctionClass.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/score/LocalScoreFunctionClass.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ConstraintBased/PC.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/search/ConstraintBased/PC.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/search/ScoreBased/GES.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/search/ScoreBased/GES.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/BackgroundKnowledge.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/BackgroundKnowledge.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/DAG2CPDAG.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/DAG2CPDAG.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/GESUtils.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/GESUtils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/GraphUtils.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/GraphUtils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/BackgroundKnowledgeOrientUtils.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/BackgroundKnowledgeOrientUtils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/Helper.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/Helper.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/Meek.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/Meek.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/SkeletonDiscovery.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/SkeletonDiscovery.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PCUtils/UCSepset.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PCUtils/UCSepset.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/PDAG2DAG.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/PDAG2DAG.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/ScoreUtils.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/ScoreUtils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/TXT2GeneralGraph.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/TXT2GeneralGraph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/causallearn/utils/cit.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/causallearn/utils/cit.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/DAG.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/base/DAG.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/base/UndirectedGraph.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/base/UndirectedGraph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/BayesianEstimator.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/estimators/BayesianEstimator.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/MLE.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/estimators/MLE.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/estimators/base.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/estimators/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/extern/tabulate.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/extern/tabulate.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/FactorSet.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/FactorSet.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/base.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/continuous/ContinuousFactor.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/continuous/ContinuousFactor.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/CPD.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/discrete/CPD.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/DiscreteFactor.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/discrete/DiscreteFactor.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/discrete/JointProbabilityDistribution.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/discrete/JointProbabilityDistribution.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/CustomDistribution.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/distributions/CustomDistribution.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/GaussianDistribution.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/distributions/GaussianDistribution.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/factors/distributions/base.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/factors/distributions/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/global_vars.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/global_vars.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/independencies/Independencies.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/independencies/Independencies.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/EliminationOrder.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/inference/EliminationOrder.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/ExactInference.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/inference/ExactInference.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/inference/base.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/inference/base.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/BayesianModel.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/BayesianModel.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/ClusterGraph.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/ClusterGraph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/DynamicBayesianNetwork.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/DynamicBayesianNetwork.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/FactorGraph.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/FactorGraph.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/JunctionTree.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/JunctionTree.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/models/MarkovModel.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/models/MarkovModel.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/readwrite/BIF.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/readwrite/BIF.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pgmpy/utils/state_name.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pgmpy/utils/state_name.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/prior.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pycausal/prior.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/pycausal.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pycausal/pycausal.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/pycausal/search.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/pycausal/search.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/rcd.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/rcd/rcd.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/utils/GraphClass.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/rcd/utils/GraphClass.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/thirdparty/rcd/utils/SkeletonDiscovery.py` & `sfr-pyrca-1.0.1/pyrca/thirdparty/rcd/utils/SkeletonDiscovery.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/Acumin-BdPro.otf` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/Acumin-BdPro.otf`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/base.css` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/base.css`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/logo.png` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/logo.png`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/modal.css` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/modal.css`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/rca.css` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/rca.css`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/styles.css` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/styles.css`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/assets/upload.svg` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/assets/upload.svg`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/causal.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/callbacks/causal.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/callbacks/data.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/callbacks/data.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/dashboard.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/causal.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/models/causal.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/models/data.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/models/data.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/causal.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/pages/causal.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/data.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/pages/data.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/pages/utils.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/pages/utils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/file_manager.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/layout.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/utils/layout.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/log.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/utils/log.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/tools/dashboard/utils/plot.py` & `sfr-pyrca-1.0.1/pyrca/tools/dashboard/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/utils/domain.py` & `sfr-pyrca-1.0.1/pyrca/utils/domain.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/utils/evaluation.py` & `sfr-pyrca-1.0.1/pyrca/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/utils/misc.py` & `sfr-pyrca-1.0.1/pyrca/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/utils/plot.py` & `sfr-pyrca-1.0.1/pyrca/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/pyrca/utils/utils.py` & `sfr-pyrca-1.0.1/pyrca/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/setup.py` & `sfr-pyrca-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # Copyright (c) 2023 salesforce.com, inc.
 # All rights reserved.
 # SPDX-License-Identifier: BSD-3-Clause
 # For full license text, see the LICENSE file in the repo root or https://opensource.org/licenses/BSD-3-Clause#
 from setuptools import setup, find_namespace_packages
 
 extras_require = {
-    "plot": ["plotly>=4", "dash>=2.0", "dash_bootstrap_components>=1.0", "jupyter-dash>=0.4", "dash[diskcache]"]
+    "plot": ["plotly>=4", "dash>=2.0", "dash_bootstrap_components>=1.0", "jupyter-dash>=0.4", "dash[diskcache]", "dash_cytoscape"]
 }
 extras_require["all"] = sum(extras_require.values(), [])
 
 setup(
     name="sfr-pyrca",
-    version="1.0.0",
+    version="1.0.1",
     author="Salesforce Research Warden AIOps",
     description="PyRCA: A Python library for Root Cause Analysis",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="AIOps RCA root cause analysis",
     url="https://github.com/salesforce/PyRCA",
     license="3-Clause BSD",
```

### Comparing `sfr-pyrca-1.0.0/sfr_pyrca.egg-info/PKG-INFO` & `sfr-pyrca-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,31 @@
-Metadata-Version: 2.1
-Name: sfr-pyrca
-Version: 1.0.0
-Summary: PyRCA: A Python library for Root Cause Analysis
-Home-page: https://github.com/salesforce/PyRCA
-Author: Salesforce Research Warden AIOps
-License: 3-Clause BSD
-Keywords: AIOps RCA root cause analysis
-Requires-Python: >=3.7,<4
-Description-Content-Type: text/markdown
-Provides-Extra: plot
-Provides-Extra: all
-License-File: LICENSE
-
 # PyRCA: A Python library for Root Cause Analysis
 <div align="center">
   <a href="#">
   <img src="https://img.shields.io/badge/Python-3.7, 3.8, 3.9-blue">
   </a>
   <a href="https://pypi.python.org/pypi/sfr-pyrca">
   <img alt="PyPI" src="https://img.shields.io/pypi/v/sfr-pyrca.svg"/>
   </a>
-  <a href="https://fuzzy-disco-r42n6p1.pages.github.io">
+  <a href="https://opensource.salesforce.com/PyRCA/">
   <img alt="Documentation" src="https://github.com/salesforce/PyRCA/actions/workflows/docs.yml/badge.svg"/>
   </a>
   <a href="https://pepy.tech/project/sfr-pyrca">
   <img alt="Downloads" src="https://pepy.tech/badge/sfr-pyrca">
   </a>
-  <a href="https://arxiv.org/abs/xxxx.xxxxx">
-  <img alt="DOI" src="https://zenodo.org/badge/DOI/10.48550/ARXIV.xxxx.xxxxx.svg"/>
+  <a href="https://arxiv.org/abs/2306.11417">
+  <img alt="DOI" src="https://zenodo.org/badge/DOI/10.48550/ARXIV.2306.11417.svg"/>
   </a>
 </div>
 
 ## Table of Contents
 1. [Introduction](#introduction)
 2. [Installation](#installation)
 3. [Getting Started](#getting-started)
-4. [Documentation](https://fuzzy-disco-r42n6p1.pages.github.io/)
+4. [Documentation](https://opensource.salesforce.com/PyRCA/)
 5. [Tutorial](https://github.com/salesforce/PyRCA/tree/main/examples)
 6. [Example](#application-example)
 7. [Benchmarks](#benchmarks)
 8. [How to Contribute](#how-to-contribute)
 
 ## Introduction
 
@@ -136,15 +122,15 @@
 ```
 
 where ``abnormal_data`` is the time series data collected in an incident window.
 
 As mentioned above, some RCA methods such as ``BayesianNetwork`` require causal graphs as their inputs. To construct such causal
 graphs from the observed time series data, you can utilize our tool by running ``python -m pyrca.tools``.
 This command will launch a Dash app for time series data analysis and causal discovery.
-![alt text](https://github.com/salesforce/PyRCA/raw/main/docs/_static/dashboard.png)
+![alt text](https://github.com/salesforce/PyRCA/raw/main/docs/_static/dashboard_gif.gif)
 
 The dashboard enables users to experiment with different causal discovery methods, customize causal discovery 
 parameters, add domain knowledge constraints (e.g., root/leaf nodes, forbidden/required links), and visualize 
 the generated causal graphs. This feature simplifies the process of manually revising causal graphs based on 
 domain knowledge. Users can download the graph generated by this tool if they are satisfied with it. The graph 
 can then be used by the RCA methods supported in PyRCA.
```

#### html2text {}

```diff
@@ -1,69 +1,64 @@
-Metadata-Version: 2.1 Name: sfr-pyrca Version: 1.0.0 Summary: PyRCA: A Python
-library for Root Cause Analysis Home-page: https://github.com/salesforce/PyRCA
-Author: Salesforce Research Warden AIOps License: 3-Clause BSD Keywords: AIOps
-RCA root cause analysis Requires-Python: >=3.7,<4 Description-Content-Type:
-text/markdown Provides-Extra: plot Provides-Extra: all License-File: LICENSE #
-PyRCA: A Python library for Root Cause Analysis
+# PyRCA: A Python library for Root Cause Analysis
 [https://img.shields.io/badge/Python-3.7,_3.8,_3.9-blue] [PyPI] [Documentation]
                                [Downloads] [DOI]
 ## Table of Contents 1. [Introduction](#introduction) 2. [Installation]
 (#installation) 3. [Getting Started](#getting-started) 4. [Documentation]
-(https://fuzzy-disco-r42n6p1.pages.github.io/) 5. [Tutorial](https://
-github.com/salesforce/PyRCA/tree/main/examples) 6. [Example](#application-
-example) 7. [Benchmarks](#benchmarks) 8. [How to Contribute](#how-to-
-contribute) ## Introduction The adoption of microservices architectures is
-growing at a rapid pace, making multi-service applications the standard
-paradigm in real-world IT applications. Typically, a multi-service application
-consists of hundreds of interacting services, making it increasingly
-challenging to detect service failures and identify their root causes. Root
-cause analysis (RCA) methods typically rely on KPI metrics, traces, or logs
-monitored on these services to determine the root causes when a system failure
-is detected. Such methods can aid engineers and SREs in the troubleshooting
-process. PyRCA is a Python machine-learning library designed to facilitate root
-cause analysis by offering various state-of-the-art RCA algorithms and an end-
-to-end pipeline for building RCA solutions. At present, PyRCA primarily focuses
-on metric-based RCA, including two types of algorithms: (1) identifying
-anomalous metrics in parallel with the observed anomaly through metric data
-analysis, such as Îµ-diagnosis, and (2) identifying root causes based on a
-topology/causal graph representing the causal relationships between the
-observed metrics, such as Bayesian inference and Random Walk. PyRCA also
-provides a convenient tool for building causal graphs from the observed time
-series data and domain knowledge, enabling users to develop graph-based
-solutions quickly. Furthermore, PyRCA offers a benchmark for evaluating various
-RCA methods, which is valuable for industry and academic research. The
-following list shows the supported RCA methods in our library: 1. [Îµ-
-Diagnosis](https://dl.acm.org/doi/10.1145/3308558.3313653) 2. Bayesian
-Inference-based RCA (BI) 3. Random Walk-based RCA (RW) 4. [Root Casue Discovery
-method (RCD)](https://openreview.net/pdf?id=weoLjoYFvXY) 5. [Hypothesis
-Testing-based RCA (HT)](https://dl.acm.org/doi/10.1145/3534678.3539041) We will
-continue improving this library to make it more comprehensive in the future. In
-the future, PyRCA will support trace and log-based RCA methods as well. ##
-Installation You can install ``pyrca`` from PyPI by calling ``pip install sfr-
-pyrca``. You may install from source by cloning the PyRCA repo, navigating to
-the root directory, and calling ``pip install .``, or ``pip install -e .`` to
-install in editable mode. You may install additional dependencies: - **For
-plotting & visualization**: Calling ``pip install sfr-pyrca[plot]``, or ``pip
-install .[plot]`` from the root directory of the repo. - **Install all the
-dependencies**: Calling ``pip install sfr-pyrca[all]``, or ``pip install .
-[all]`` from the root directory of the repo. ## Getting Started PyRCA provides
-a unified interface for training RCA models and finding root causes. To apply a
-certain RCA method, you only need to specify: - **The selected RCA method**:
-e.g., ``BayesianNetwork``, ``EpsilonDiagnosis``. - **The method
-configuration**: e.g., ``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. -
-**Time series data for initialization/training**: e.g., A time series data in a
-pandas dataframe. - **Abnormal time series data in an incident window**: The
-RCA methods require the anomalous KPI metrics in an incident window. Let's take
-``BayesianNetwork`` as an example. Suppose that ``graph_df`` is the pandas
-dataframe of a graph representing the causal relationships between metrics (how
-to construct such causal graph will be discussed later), and ``df`` is the
-pandas dataframe containing the historical observed time series data (e.g., the
-index is the timestamp and each column represents one monitored metric). To
-train a ``BayesianNetwork``, you can simply run the following code: ```python
-from pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
+(https://opensource.salesforce.com/PyRCA/) 5. [Tutorial](https://github.com/
+salesforce/PyRCA/tree/main/examples) 6. [Example](#application-example) 7.
+[Benchmarks](#benchmarks) 8. [How to Contribute](#how-to-contribute) ##
+Introduction The adoption of microservices architectures is growing at a rapid
+pace, making multi-service applications the standard paradigm in real-world IT
+applications. Typically, a multi-service application consists of hundreds of
+interacting services, making it increasingly challenging to detect service
+failures and identify their root causes. Root cause analysis (RCA) methods
+typically rely on KPI metrics, traces, or logs monitored on these services to
+determine the root causes when a system failure is detected. Such methods can
+aid engineers and SREs in the troubleshooting process. PyRCA is a Python
+machine-learning library designed to facilitate root cause analysis by offering
+various state-of-the-art RCA algorithms and an end-to-end pipeline for building
+RCA solutions. At present, PyRCA primarily focuses on metric-based RCA,
+including two types of algorithms: (1) identifying anomalous metrics in
+parallel with the observed anomaly through metric data analysis, such as Îµ-
+diagnosis, and (2) identifying root causes based on a topology/causal graph
+representing the causal relationships between the observed metrics, such as
+Bayesian inference and Random Walk. PyRCA also provides a convenient tool for
+building causal graphs from the observed time series data and domain knowledge,
+enabling users to develop graph-based solutions quickly. Furthermore, PyRCA
+offers a benchmark for evaluating various RCA methods, which is valuable for
+industry and academic research. The following list shows the supported RCA
+methods in our library: 1. [Îµ-Diagnosis](https://dl.acm.org/doi/10.1145/
+3308558.3313653) 2. Bayesian Inference-based RCA (BI) 3. Random Walk-based RCA
+(RW) 4. [Root Casue Discovery method (RCD)](https://openreview.net/
+pdf?id=weoLjoYFvXY) 5. [Hypothesis Testing-based RCA (HT)](https://dl.acm.org/
+doi/10.1145/3534678.3539041) We will continue improving this library to make it
+more comprehensive in the future. In the future, PyRCA will support trace and
+log-based RCA methods as well. ## Installation You can install ``pyrca`` from
+PyPI by calling ``pip install sfr-pyrca``. You may install from source by
+cloning the PyRCA repo, navigating to the root directory, and calling ``pip
+install .``, or ``pip install -e .`` to install in editable mode. You may
+install additional dependencies: - **For plotting & visualization**: Calling
+``pip install sfr-pyrca[plot]``, or ``pip install .[plot]`` from the root
+directory of the repo. - **Install all the dependencies**: Calling ``pip
+install sfr-pyrca[all]``, or ``pip install .[all]`` from the root directory of
+the repo. ## Getting Started PyRCA provides a unified interface for training
+RCA models and finding root causes. To apply a certain RCA method, you only
+need to specify: - **The selected RCA method**: e.g., ``BayesianNetwork``,
+``EpsilonDiagnosis``. - **The method configuration**: e.g.,
+``BayesianNetworkConfig``, ``EpsilonDiagnosisConfig``. - **Time series data for
+initialization/training**: e.g., A time series data in a pandas dataframe. -
+**Abnormal time series data in an incident window**: The RCA methods require
+the anomalous KPI metrics in an incident window. Let's take ``BayesianNetwork``
+as an example. Suppose that ``graph_df`` is the pandas dataframe of a graph
+representing the causal relationships between metrics (how to construct such
+causal graph will be discussed later), and ``df`` is the pandas dataframe
+containing the historical observed time series data (e.g., the index is the
+timestamp and each column represents one monitored metric). To train a
+``BayesianNetwork``, you can simply run the following code: ```python from
+pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork
 (config=BayesianNetwork.config_class(graph=graph_df)) model.train(df)
 model.save("model_folder") ``` After the model is trained, you can use it to
 find root causes of an incident given a list of anomalous metrics detected by a
 certain anomaly detector (you can use the stats-based detector supported in
 PyRCA or other anomaly detection methods supported by our [Merlion](https://
 github.com/salesforce/Merlion) library), e.g., ```python from
 pyrca.analyzers.bayesian import BayesianNetwork model = BayesianNetwork.load
@@ -78,15 +73,15 @@
 ```python results = model.find_root_causes(abnormal_data) print(results.to_dict
 ()) ``` where ``abnormal_data`` is the time series data collected in an
 incident window. As mentioned above, some RCA methods such as
 ``BayesianNetwork`` require causal graphs as their inputs. To construct such
 causal graphs from the observed time series data, you can utilize our tool by
 running ``python -m pyrca.tools``. This command will launch a Dash app for time
 series data analysis and causal discovery. ![alt text](https://github.com/
-salesforce/PyRCA/raw/main/docs/_static/dashboard.png) The dashboard enables
+salesforce/PyRCA/raw/main/docs/_static/dashboard_gif.gif) The dashboard enables
 users to experiment with different causal discovery methods, customize causal
 discovery parameters, add domain knowledge constraints (e.g., root/leaf nodes,
 forbidden/required links), and visualize the generated causal graphs. This
 feature simplifies the process of manually revising causal graphs based on
 domain knowledge. Users can download the graph generated by this tool if they
 are satisfied with it. The graph can then be used by the RCA methods supported
 in PyRCA. Alternatively, users can write code to build such graphs instead of
```

### Comparing `sfr-pyrca-1.0.0/sfr_pyrca.egg-info/SOURCES.txt` & `sfr-pyrca-1.0.1/sfr_pyrca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/analyzers/test_bayesian.py` & `sfr-pyrca-1.0.1/tests/analyzers/test_bayesian.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/analyzers/test_epsilon_diagnosis.py` & `sfr-pyrca-1.0.1/tests/analyzers/test_epsilon_diagnosis.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/analyzers/test_ht.py` & `sfr-pyrca-1.0.1/tests/analyzers/test_ht.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/analyzers/test_random_walk.py` & `sfr-pyrca-1.0.1/tests/analyzers/test_random_walk.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/analyzers/test_rcd.py` & `sfr-pyrca-1.0.1/tests/analyzers/test_rcd.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/applications/example/run_rca.py` & `sfr-pyrca-1.0.1/tests/applications/example/run_rca.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/graphs/test_domain.py` & `sfr-pyrca-1.0.1/tests/graphs/test_domain.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/graphs/test_fges.py` & `sfr-pyrca-1.0.1/tests/graphs/test_fges.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/graphs/test_ges.py` & `sfr-pyrca-1.0.1/tests/graphs/test_ges.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/graphs/test_lingam.py` & `sfr-pyrca-1.0.1/tests/graphs/test_lingam.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/graphs/test_pc.py` & `sfr-pyrca-1.0.1/tests/graphs/test_pc.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/outliers/test_config.py` & `sfr-pyrca-1.0.1/tests/outliers/test_config.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/outliers/test_stats.py` & `sfr-pyrca-1.0.1/tests/outliers/test_stats.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/simulation/test_simulation.py` & `sfr-pyrca-1.0.1/tests/simulation/test_simulation.py`

 * *Files identical despite different names*

### Comparing `sfr-pyrca-1.0.0/tests/tools/test_causal.py` & `sfr-pyrca-1.0.1/tests/tools/test_causal.py`

 * *Files identical despite different names*

