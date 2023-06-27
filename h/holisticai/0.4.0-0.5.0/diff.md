# Comparing `tmp/holisticai-0.4.0.tar.gz` & `tmp/holisticai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holisticai-0.4.0.tar", max compression
+gzip compressed data, was "holisticai-0.5.0.tar", max compression
```

## Comparing `holisticai-0.4.0.tar` & `holisticai-0.5.0.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0    11357 2023-05-18 12:20:34.013740 holisticai-0.4.0/LICENSE
--rw-r--r--   0        0        0      796 2023-05-18 12:20:34.013740 holisticai-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-18 12:20:34.077741 holisticai-0.4.0/holisticai/__init__.py
--rw-r--r--   0        0        0      159 2023-05-18 12:20:34.077741 holisticai-0.4.0/holisticai/bias/__init__.py
--rw-r--r--   0        0        0     3378 2023-05-18 12:20:34.077741 holisticai-0.4.0/holisticai/bias/metrics/__init__.py
--rw-r--r--   0        0        0    28027 2023-05-18 12:20:34.077741 holisticai-0.4.0/holisticai/bias/metrics/_classification.py
--rw-r--r--   0        0        0    20317 2023-05-18 12:20:34.077741 holisticai-0.4.0/holisticai/bias/metrics/_clustering.py
--rw-r--r--   0        0        0    27996 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/metrics/_multiclass.py
--rw-r--r--   0        0        0    41982 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/metrics/_recommender.py
--rw-r--r--   0        0        0    30079 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/metrics/_regression.py
--rw-r--r--   0        0        0     2212 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/__init__.py
--rw-r--r--   0        0        0     5662 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py
--rw-r--r--   0        0        0    10434 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py
--rw-r--r--   0        0        0     2149 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py
--rw-r--r--   0        0        0     1365 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py
--rw-r--r--   0        0        0     7801 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py
--rw-r--r--   0        0        0     2166 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py
--rw-r--r--   0        0        0     1977 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py
--rw-r--r--   0        0        0    14757 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py
--rw-r--r--   0        0        0       63 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_base.py
--rw-r--r--   0        0        0     8244 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py
--rw-r--r--   0        0        0     2832 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py
--rw-r--r--   0        0        0      140 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/__init__.py
--rw-r--r--   0        0        0       63 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_base.py
--rw-r--r--   0        0        0     8117 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py
--rw-r--r--   0        0        0     3093 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py
--rw-r--r--   0        0        0     1487 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/__init__.py
--rw-r--r--   0        0        0      740 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py
--rw-r--r--   0        0        0     2088 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py
--rw-r--r--   0        0        0     6067 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py
--rw-r--r--   0        0        0     7278 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py
--rw-r--r--   0        0        0       66 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/__init__.py
--rw-r--r--   0        0        0      475 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/_conventions.py
--rw-r--r--   0        0        0     2381 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py
--rw-r--r--   0        0        0     2225 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py
--rw-r--r--   0        0        0    10220 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py
--rw-r--r--   0        0        0      906 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py
--rw-r--r--   0        0        0     4382 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py
--rw-r--r--   0        0        0     1435 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py
--rw-r--r--   0        0        0     7834 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py
--rw-r--r--   0        0        0     9599 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py
--rw-r--r--   0        0        0     6923 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py
--rw-r--r--   0        0        0    13843 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py
--rw-r--r--   0        0        0     4152 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py
--rw-r--r--   0        0        0     5017 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py
--rw-r--r--   0        0        0     2821 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py
--rw-r--r--   0        0        0    11078 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py
--rw-r--r--   0        0        0     3473 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py
--rw-r--r--   0        0        0     5213 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py
--rw-r--r--   0        0        0     1680 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py
--rw-r--r--   0        0        0     4772 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py
--rw-r--r--   0        0        0     3341 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py
--rw-r--r--   0        0        0     5623 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py
--rw-r--r--   0        0        0     6894 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py
--rw-r--r--   0        0        0     3231 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py
--rw-r--r--   0        0        0      559 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py
--rw-r--r--   0        0        0     1853 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py
--rw-r--r--   0        0        0     3541 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py
--rw-r--r--   0        0        0     9446 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py
--rw-r--r--   0        0        0     4496 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py
--rw-r--r--   0        0        0     2950 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py
--rw-r--r--   0        0        0     5282 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py
--rw-r--r--   0        0        0      614 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py
--rw-r--r--   0        0        0     3432 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py
--rw-r--r--   0        0        0     3952 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py
--rw-r--r--   0        0        0     3456 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py
--rw-r--r--   0        0        0     3437 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py
--rw-r--r--   0        0        0     3884 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py
--rw-r--r--   0        0        0     4097 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py
--rw-r--r--   0        0        0     6557 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py
--rw-r--r--   0        0        0     2217 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py
--rw-r--r--   0        0        0     2254 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py
--rw-r--r--   0        0        0     2231 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py
--rw-r--r--   0        0        0     2097 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py
--rw-r--r--   0        0        0     5463 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py
--rw-r--r--   0        0        0      828 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py
--rw-r--r--   0        0        0     4915 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py
--rw-r--r--   0        0        0     3457 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py
--rw-r--r--   0        0        0     3104 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py
--rw-r--r--   0        0        0     4954 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py
--rw-r--r--   0        0        0     1223 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/__init__.py
--rw-r--r--   0        0        0     8950 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py
--rw-r--r--   0        0        0     9796 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py
--rw-r--r--   0        0        0     7433 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py
--rw-r--r--   0        0        0     6954 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py
--rw-r--r--   0        0        0     4006 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py
--rw-r--r--   0        0        0     9322 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py
--rw-r--r--   0        0        0     6784 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py
--rw-r--r--   0        0        0     1963 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py
--rw-r--r--   0        0        0     2220 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py
--rw-r--r--   0        0        0     7114 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py
--rw-r--r--   0        0        0     3690 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py
--rw-r--r--   0        0        0     2278 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py
--rw-r--r--   0        0        0     2481 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py
--rw-r--r--   0        0        0     6238 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py
--rw-r--r--   0        0        0     3712 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py
--rw-r--r--   0        0        0      868 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py
--rw-r--r--   0        0        0     6369 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py
--rw-r--r--   0        0        0     5421 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py
--rw-r--r--   0        0        0     4286 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py
--rw-r--r--   0        0        0     3570 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py
--rw-r--r--   0        0        0     4032 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py
--rw-r--r--   0        0        0     1668 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py
--rw-r--r--   0        0        0     5413 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py
--rw-r--r--   0        0        0     2791 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py
--rw-r--r--   0        0        0     4968 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py
--rw-r--r--   0        0        0      640 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py
--rw-r--r--   0        0        0     5751 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py
--rw-r--r--   0        0        0     1314 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py
--rw-r--r--   0        0        0     1294 2023-05-18 12:20:34.081741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py
--rw-r--r--   0        0        0     3688 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py
--rw-r--r--   0        0        0    10585 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py
--rw-r--r--   0        0        0     2177 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py
--rw-r--r--   0        0        0     3599 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py
--rw-r--r--   0        0        0      578 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/__init__.py
--rw-r--r--   0        0        0     3873 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py
--rw-r--r--   0        0        0     2674 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py
--rw-r--r--   0        0        0     3914 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py
--rw-r--r--   0        0        0     7337 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py
--rw-r--r--   0        0        0     3813 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/reweighing.py
--rw-r--r--   0        0        0     1266 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/__init__.py
--rw-r--r--   0        0        0     2157 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/_bias_classification_plots.py
--rw-r--r--   0        0        0     6909 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/_bias_exploratory_plots.py
--rw-r--r--   0        0        0    11349 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/_bias_multiclass_plots.py
--rw-r--r--   0        0        0     8066 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/_bias_recommender_plots.py
--rw-r--r--   0        0        0    14148 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/bias/plots/_bias_regression_plots.py
--rw-r--r--   0        0        0      333 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/datasets/__init__.py
--rw-r--r--   0        0        0    13961 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/datasets/_dataloaders.py
--rw-r--r--   0        0        0      951 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/datasets/synthetic/recruitment.py
--rw-r--r--   0        0        0      966 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/datasets/synthetic/user_feedback.py
--rw-r--r--   0        0        0    11570 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/efficacy/metrics.py
--rw-r--r--   0        0        0       54 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/__init__.py
--rw-r--r--   0        0        0     5952 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/_pipeline.py
--rw-r--r--   0        0        0     6559 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/_pipeline_helper.py
--rw-r--r--   0        0        0     3134 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/handlers/_estimator.py
--rw-r--r--   0        0        0     1821 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/handlers/_pipeline_params.py
--rw-r--r--   0        0        0     4816 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/pipeline/handlers/_utransformers.py
--rw-r--r--   0        0        0      435 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/__init__.py
--rw-r--r--   0        0        0     5103 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/_formatting.py
--rw-r--r--   0        0        0     1353 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/_plotting.py
--rw-r--r--   0        0        0     5755 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/_recommender_tools.py
--rw-r--r--   0        0        0    13794 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/_validation.py
--rw-r--r--   0        0        0      100 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/cluster/__init__.py
--rw-r--r--   0        0        0     1908 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/cluster/_kcenters.py
--rw-r--r--   0        0        0    14757 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/cluster/_kmedoids.py
--rw-r--r--   0        0        0      549 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/cluster/_utils.py
--rw-r--r--   0        0        0      813 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/recommender/_rsbase.py
--rw-r--r--   0        0        0     3157 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/recommender/item_selection/selectors.py
--rw-r--r--   0        0        0     1321 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py
--rw-r--r--   0        0        0       68 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/optimizers/__init__.py
--rw-r--r--   0        0        0    15852 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/optimizers/_genetic_algorithm.py
--rw-r--r--   0        0        0     4484 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/_transformer_base.py
--rw-r--r--   0        0        0      499 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/bias/__init__.py
--rw-r--r--   0        0        0     1049 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/bias/_group_utils.py
--rw-r--r--   0        0        0     1243 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/bias/_inprocessing.py
--rw-r--r--   0        0        0     2137 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/bias/_postprocessing.py
--rw-r--r--   0        0        0     1346 2023-05-18 12:20:34.085741 holisticai-0.4.0/holisticai/utils/transformers/bias/_preprocessing.py
--rw-r--r--   0        0        0      698 2023-05-18 12:20:34.085741 holisticai-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 holisticai-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-27 20:41:50.394914 holisticai-0.5.0/LICENSE
+-rw-r--r--   0        0        0      808 2023-06-27 20:41:50.394914 holisticai-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/__init__.py
+-rw-r--r--   0        0        0     3378 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/__init__.py
+-rw-r--r--   0        0        0    28027 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/_classification.py
+-rw-r--r--   0        0        0    20317 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/_clustering.py
+-rw-r--r--   0        0        0    27996 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/_multiclass.py
+-rw-r--r--   0        0        0    41982 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/_recommender.py
+-rw-r--r--   0        0        0    30239 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/metrics/_regression.py
+-rw-r--r--   0        0        0     2212 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/__init__.py
+-rw-r--r--   0        0        0     5662 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py
+-rw-r--r--   0        0        0    10434 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py
+-rw-r--r--   0        0        0     2149 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py
+-rw-r--r--   0        0        0     1365 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py
+-rw-r--r--   0        0        0     7801 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py
+-rw-r--r--   0        0        0     2166 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py
+-rw-r--r--   0        0        0     1977 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py
+-rw-r--r--   0        0        0    14757 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py
+-rw-r--r--   0        0        0       63 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_base.py
+-rw-r--r--   0        0        0     8244 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py
+-rw-r--r--   0        0        0     2832 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py
+-rw-r--r--   0        0        0      140 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_base.py
+-rw-r--r--   0        0        0     8117 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py
+-rw-r--r--   0        0        0     3093 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py
+-rw-r--r--   0        0        0     1487 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/__init__.py
+-rw-r--r--   0        0        0      740 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py
+-rw-r--r--   0        0        0     2088 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py
+-rw-r--r--   0        0        0     6067 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py
+-rw-r--r--   0        0        0     7278 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py
+-rw-r--r--   0        0        0       66 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/__init__.py
+-rw-r--r--   0        0        0      475 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/_conventions.py
+-rw-r--r--   0        0        0     2381 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py
+-rw-r--r--   0        0        0     2225 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py
+-rw-r--r--   0        0        0    10288 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py
+-rw-r--r--   0        0        0      906 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py
+-rw-r--r--   0        0        0     4433 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py
+-rw-r--r--   0        0        0     1435 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py
+-rw-r--r--   0        0        0     7834 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py
+-rw-r--r--   0        0        0     9599 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py
+-rw-r--r--   0        0        0     6923 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py
+-rw-r--r--   0        0        0    13843 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py
+-rw-r--r--   0        0        0     4152 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py
+-rw-r--r--   0        0        0     5017 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py
+-rw-r--r--   0        0        0     2821 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py
+-rw-r--r--   0        0        0    11078 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py
+-rw-r--r--   0        0        0     3473 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py
+-rw-r--r--   0        0        0     5213 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py
+-rw-r--r--   0        0        0     1680 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py
+-rw-r--r--   0        0        0     4772 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py
+-rw-r--r--   0        0        0     3341 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py
+-rw-r--r--   0        0        0     5644 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py
+-rw-r--r--   0        0        0     6894 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py
+-rw-r--r--   0        0        0     3231 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py
+-rw-r--r--   0        0        0      559 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py
+-rw-r--r--   0        0        0     1853 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py
+-rw-r--r--   0        0        0     3541 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py
+-rw-r--r--   0        0        0     9437 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py
+-rw-r--r--   0        0        0     4493 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py
+-rw-r--r--   0        0        0     2950 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py
+-rw-r--r--   0        0        0     5287 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py
+-rw-r--r--   0        0        0      614 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py
+-rw-r--r--   0        0        0     3432 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py
+-rw-r--r--   0        0        0     3952 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py
+-rw-r--r--   0        0        0     3456 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py
+-rw-r--r--   0        0        0     3437 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py
+-rw-r--r--   0        0        0     3884 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py
+-rw-r--r--   0        0        0     4088 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py
+-rw-r--r--   0        0        0     6557 2023-06-27 20:41:50.506913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py
+-rw-r--r--   0        0        0     2217 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py
+-rw-r--r--   0        0        0     2254 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py
+-rw-r--r--   0        0        0     2231 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py
+-rw-r--r--   0        0        0     2097 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py
+-rw-r--r--   0        0        0     5463 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py
+-rw-r--r--   0        0        0      828 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py
+-rw-r--r--   0        0        0     4912 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py
+-rw-r--r--   0        0        0     3457 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py
+-rw-r--r--   0        0        0     3101 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py
+-rw-r--r--   0        0        0     4954 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py
+-rw-r--r--   0        0        0     1223 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/__init__.py
+-rw-r--r--   0        0        0     8950 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py
+-rw-r--r--   0        0        0     9796 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py
+-rw-r--r--   0        0        0     7433 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py
+-rw-r--r--   0        0        0     6954 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py
+-rw-r--r--   0        0        0     4006 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py
+-rw-r--r--   0        0        0     9322 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py
+-rw-r--r--   0        0        0     6784 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py
+-rw-r--r--   0        0        0     1963 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py
+-rw-r--r--   0        0        0     2220 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py
+-rw-r--r--   0        0        0     7114 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py
+-rw-r--r--   0        0        0     3690 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py
+-rw-r--r--   0        0        0     2278 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py
+-rw-r--r--   0        0        0     2481 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py
+-rw-r--r--   0        0        0     6238 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py
+-rw-r--r--   0        0        0     3712 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py
+-rw-r--r--   0        0        0      868 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py
+-rw-r--r--   0        0        0     6369 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py
+-rw-r--r--   0        0        0     5421 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py
+-rw-r--r--   0        0        0     4286 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py
+-rw-r--r--   0        0        0     3570 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py
+-rw-r--r--   0        0        0     4032 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py
+-rw-r--r--   0        0        0     1668 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py
+-rw-r--r--   0        0        0     5413 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py
+-rw-r--r--   0        0        0     2791 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py
+-rw-r--r--   0        0        0     4968 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py
+-rw-r--r--   0        0        0      640 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py
+-rw-r--r--   0        0        0     5751 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py
+-rw-r--r--   0        0        0     1314 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py
+-rw-r--r--   0        0        0     1294 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py
+-rw-r--r--   0        0        0     3844 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py
+-rw-r--r--   0        0        0    10585 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py
+-rw-r--r--   0        0        0     2177 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py
+-rw-r--r--   0        0        0     3599 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py
+-rw-r--r--   0        0        0      578 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3873 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py
+-rw-r--r--   0        0        0     2674 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py
+-rw-r--r--   0        0        0     3914 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py
+-rw-r--r--   0        0        0     7337 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py
+-rw-r--r--   0        0        0     3813 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/reweighing.py
+-rw-r--r--   0        0        0     1343 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/__init__.py
+-rw-r--r--   0        0        0     2157 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/_bias_classification_plots.py
+-rw-r--r--   0        0        0     8449 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/_bias_exploratory_plots.py
+-rw-r--r--   0        0        0    11349 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/_bias_multiclass_plots.py
+-rw-r--r--   0        0        0     8066 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/_bias_recommender_plots.py
+-rw-r--r--   0        0        0    14148 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/bias/plots/_bias_regression_plots.py
+-rw-r--r--   0        0        0      333 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/datasets/__init__.py
+-rw-r--r--   0        0        0    13961 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/datasets/_dataloaders.py
+-rw-r--r--   0        0        0      951 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/datasets/synthetic/recruitment.py
+-rw-r--r--   0        0        0      966 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/datasets/synthetic/user_feedback.py
+-rw-r--r--   0        0        0    11570 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/efficacy/metrics.py
+-rw-r--r--   0        0        0       54 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/__init__.py
+-rw-r--r--   0        0        0     5952 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/_pipeline.py
+-rw-r--r--   0        0        0     6559 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/_pipeline_helper.py
+-rw-r--r--   0        0        0     3134 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/handlers/_estimator.py
+-rw-r--r--   0        0        0     1821 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/handlers/_pipeline_params.py
+-rw-r--r--   0        0        0     4816 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/pipeline/handlers/_utransformers.py
+-rw-r--r--   0        0        0      435 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/__init__.py
+-rw-r--r--   0        0        0     5103 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/_formatting.py
+-rw-r--r--   0        0        0     1353 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/_plotting.py
+-rw-r--r--   0        0        0     5755 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/_recommender_tools.py
+-rw-r--r--   0        0        0    13794 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/_validation.py
+-rw-r--r--   0        0        0      100 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/cluster/__init__.py
+-rw-r--r--   0        0        0     1908 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/cluster/_kcenters.py
+-rw-r--r--   0        0        0    14757 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/cluster/_kmedoids.py
+-rw-r--r--   0        0        0      549 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/cluster/_utils.py
+-rw-r--r--   0        0        0      813 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/recommender/_rsbase.py
+-rw-r--r--   0        0        0     3157 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/recommender/item_selection/selectors.py
+-rw-r--r--   0        0        0     1321 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py
+-rw-r--r--   0        0        0       68 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/optimizers/__init__.py
+-rw-r--r--   0        0        0    15852 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/optimizers/_genetic_algorithm.py
+-rw-r--r--   0        0        0     4484 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/_transformer_base.py
+-rw-r--r--   0        0        0      499 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/bias/__init__.py
+-rw-r--r--   0        0        0     1049 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/bias/_group_utils.py
+-rw-r--r--   0        0        0     1243 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/bias/_inprocessing.py
+-rw-r--r--   0        0        0     2137 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/bias/_postprocessing.py
+-rw-r--r--   0        0        0     1346 2023-06-27 20:41:50.510913 holisticai-0.5.0/holisticai/utils/transformers/bias/_preprocessing.py
+-rw-r--r--   0        0        0      699 2023-06-27 20:41:50.514913 holisticai-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 holisticai-0.5.0/PKG-INFO
```

### Comparing `holisticai-0.4.0/LICENSE` & `holisticai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/README.md` & `holisticai-0.5.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 <br>Holistic AI
 </h1>
 
 The Holistic AI library is an open-source tool to assess and improve the trustworthiness of AI systems.  
 
 Currently, the library offers a set of techniques to easily measure and mitigate Bias across numerous tasks. In the future, it will be extended to include tools for Efficacy, Robustness, Privacy and Explainability as well. This will allow a holistic assessment of AI systems.  
 
-- Documentation:https://holisticai.readthedocs.io/en/latest/ 
+- Documentation: https://holistic-ai.readthedocs.io/en/latest/
 - Tutorials: https://github.com/holistic-ai/holisticai/tree/main/tutorials
 - Source code: https://github.com/holistic-ai/holisticai/tree/main
 - Holistic Ai website: https://holisticai.com
 
 ## Installation
 
 Install the library with:
-
+```bash
     pip install holisticai
+```
```

### Comparing `holisticai-0.4.0/holisticai/bias/metrics/__init__.py` & `holisticai-0.5.0/holisticai/bias/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/metrics/_classification.py` & `holisticai-0.5.0/holisticai/bias/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/metrics/_clustering.py` & `holisticai-0.5.0/holisticai/bias/metrics/_clustering.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/metrics/_multiclass.py` & `holisticai-0.5.0/holisticai/bias/metrics/_multiclass.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/metrics/_recommender.py` & `holisticai-0.5.0/holisticai/bias/metrics/_recommender.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/metrics/_regression.py` & `holisticai-0.5.0/holisticai/bias/metrics/_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -948,21 +948,30 @@
         "RMSE Ratio": {},
         "RMSE Ratio Q80": {"q": 0.8},
         "MAE Ratio": {},
         "MAE Ratio Q80": {"q": 0.8},
         "Correlation Difference": {},
     }
 
+    y_pred = np.squeeze(y_pred)
+
+    if y_true is not None:
+        y_true = np.squeeze(y_true)
+
     out_metrics = [
         [pf, fn(group_a, group_b, y_pred, **hypers[pf]), ref_vals[pf]]
         for pf, fn in equal_outcome_metrics.items()
     ]
     if y_true is not None:
         opp_metrics = [
-            [pf, fn(group_a, group_b, y_pred, y_true, **hypers[pf]), ref_vals[pf]]
+            [
+                pf,
+                fn(group_a, group_b, y_pred, y_true, **hypers[pf]),
+                ref_vals[pf],
+            ]
             for pf, fn in equal_opportunity_metrics.items()
         ]
 
     if metric_type == "both":
         metrics = out_metrics + opp_metrics
         return pd.DataFrame(
             metrics, columns=["Metric", "Value", "Reference"]
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/__init__.py` & `holisticai-0.5.0/holisticai/bias/mitigation/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_feature.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_categorical_repairer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_numerical_repairer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_sparse_list.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/disparate_impact_remover/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kcenters.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/clustering/_kmedoids.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_scalable.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decomposition/_vanilla.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_scalable.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py` & `holisticai-0.5.0/holisticai/bias/mitigation/commons/fairlet_clustering/decompositions/_vanilla.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/__init__.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/dataset.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/models.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/adversarial_debiasing/torch/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/_logger.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/_moments_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/classification/_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,17 @@
 
         Parameters
         ----------
         lambda_vec : :class:`pandas:pandas.Series`
             The vector of Lagrange multipliers indexed by `index`
         """
 
-        lambda_event = (lambda_vec["+"] - self.ratio * lambda_vec["-"]).sum(
+        lambda_event = (lambda_vec["+"] - self.ratio * lambda_vec["-"]).groupby(
             level=_EVENT
-        ) / self.event_prob
+        ).sum() / self.event_prob
 
         lambda_group_event = (
             self.ratio * lambda_vec["+"] - lambda_vec["-"]
         ) / self.group_event_prob
 
         adjust = lambda_event - lambda_group_event
 
@@ -142,16 +142,17 @@
         predictions = np.squeeze(predictor(self.X))
         pred = utility_diff.T * predictions + self.utilities[:, 0]
 
         return self._gamma_signed(pred)
 
     def _gamma_signed(self, pred):
         self.tags[_PRED] = pred
-        expect_event = self.tags.groupby(_EVENT).mean()
-        expect_group_event = self.tags.groupby([_EVENT, _GROUP_ID]).mean()
+        tags = self.tags.set_index([_GROUP_ID, _EVENT])
+        expect_event = tags.groupby(level=_EVENT).mean()
+        expect_group_event = tags.groupby(level=[_EVENT, _GROUP_ID]).mean()
         expect_group_event[_UPPER_BOUND_DIFF] = (
             self.ratio * expect_group_event[_PRED] - expect_event[_PRED]
         )
         expect_group_event[_LOWER_BOUND_DIFF] = (
             -expect_group_event[_PRED] + self.ratio * expect_event[_PRED]
         )
         gamma_signed = pd.concat(
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/classification/_objectives.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/regression/_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,16 @@
 
     def gamma(self, predictor):
         """Calculate the degree to which constraints are currently violated by the predictor."""
         self.tags[_PREDICTION] = predictor(self.X)
         self.tags[_LOSS] = self.reduction_loss.eval(
             self.tags[_LABEL], self.tags[_PREDICTION]
         )
-        expect_attr = self.tags.groupby(_GROUP_ID).mean()
+        tags = self.tags.set_index([_GROUP_ID, _EVENT])
+        expect_attr = tags.groupby(_GROUP_ID).mean()
         return expect_attr[_LOSS]
 
     def bound(self):
         """Return the vector of bounds.
         Returns
         -------
         pandas.Series
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/commons/regression/_losses.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/_lagrangian.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/exponentiated_gradient/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/algorithms.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_center_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_k_mediam_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fair_scoring_classifier/utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/fairlet_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/_grid_generator.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,15 +100,16 @@
             grid_limit=self.grid_limit,
             neg_allowed=neg_allowed,
             force_L1_norm=objective_in_the_span,
         )
 
         grid = self.generator.generate_grid(self.constraint)
         self.monitor.total_steps = grid.shape[1]
-        for (_, lambda_vec) in grid.iteritems():
+        for col_name in grid:
+            lambda_vec = grid[col_name]
 
             weights = self.constraint.signed_weights(lambda_vec)
             if not objective_in_the_span:
                 weights += self.objective.signed_weights()
 
             if self.constraint.PROBLEM_TYPE == "classification":
                 y_reduction = 1 * (weights > 0)
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/grid_search/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/blind_spot_aware.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/propensity_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/common_utils/utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/algorithm_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         allItemParams = np.concatenate((item_vectors, item_biases[:, None]), axis=1)
 
         allParams = np.concatenate((allUserParams, allItemParams), axis=0)
         paramVector = np.reshape(
             allParams, (self.numUsers + self.numItems) * (self.num_dimensions + 1)
         )
         paramVector = np.concatenate((paramVector, [global_bias]))
-        return paramVector.astype(np.float)
+        return paramVector.astype(float)
 
     def deserialize(self, paramVector):
         globalBias = paramVector[-1]
         remainingParams = paramVector[:-1]
         allParams = np.reshape(
             remainingParams, (self.numUsers + self.numItems, self.num_dimensions + 1)
         )
@@ -253,16 +253,16 @@
     if start_vec is None:
         userVectorsInit = np.random.standard_normal(
             (config["numUsers"], config["num_dimensions"])
         )
         itemVectorsInit = np.random.standard_normal(
             (config["numItems"], config["num_dimensions"])
         )
-        userBiasesInit = np.zeros(config["numUsers"], dtype=np.float)
-        itemBiasesInit = np.zeros(config["numItems"], dtype=np.float)
+        userBiasesInit = np.zeros(config["numUsers"], dtype=float)
+        itemBiasesInit = np.zeros(config["numItems"], dtype=float)
         globalBiasInit = 0
     else:
         userVectorsInit = start_vec[0]
         itemVectorsInit = start_vec[1]
         userBiasesInit = start_vec[2]
         itemBiasesInit = start_vec[3]
         globalBiasInit = start_vec[4]
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/debiasing_learning/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         self.pred = self.algorithm.predict(model_params, bias_mode=self.bias_mode)
         self.invP = invP
         return self
 
     def _init_parameters(self, partial_observations):
         averageObservedRating = np.ma.mean(partial_observations)
         completeRatings = np.ma.filled(
-            partial_observations.astype(np.float), averageObservedRating
+            partial_observations.astype(float), averageObservedRating
         )
         numUsers, numItems = np.shape(partial_observations)
         numUsers = completeRatings.shape[0]
         ncv = (min(numUsers, numItems) + self.K) // 2
 
         u, s, vt = scipy.sparse.linalg.svds(
             completeRatings,
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/matrix_factorization/popularity_propensity.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,25 +74,25 @@
         return best_param
 
     def forward(self, dist, params, a, b, x):
         P = self.probabilities(dist=dist, x=x)
         return self.constraint.forward(P=P, params=params, a=a, b=b)
 
     def fit(self, X, y, sensitive_features, random_state=None):
+        """Returns the model given the training data and input tau."""
+
         y_true = y.copy()
         y_true[y == 0] = -1
+        y_true = np.array(y_true)
 
         groups_num = self.sens_groups.fit_transform(
             sensitive_features, convert_numeric=True
         )
-
-        """Returns the model given the training data and input tau."""
-        train = np.concatenate(
-            [X, y_true[:, np.newaxis], groups_num[:, np.newaxis]], axis=1
-        )
+        groups_num = np.array(groups_num)
+        train = np.c_[X, y_true, groups_num]
         mean = np.mean(train, axis=0)
         cov = np.cov(train, rowvar=False)
         dist = multivariate_normal(mean, cov, allow_singular=True, seed=random_state)
         nb_features = X.shape[1]
         dist_x = multivariate_normal(
             mean[:nb_features],
             cov[:nb_features, :nb_features],
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/meta_fair_classifier/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/losses.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,35 +81,35 @@
             target class of samples
         s : array, shape=(n_samples)
             values of sensitive features
         """
 
         if self.init_type == "Zero":
             # clear by zeros
-            coef = np.zeros(nb_group_values * nb_features, dtype=np.float)
+            coef = np.zeros(nb_group_values * nb_features, dtype=float)
 
         elif self.init_type == "Random":
             # at random
             coef = np.random.randn(nb_group_values * nb_features)
 
         elif self.init_type == "StandarLR":
             # learned by standard LR
-            coef = np.empty(nb_group_values * nb_features, dtype=np.float)
+            coef = np.empty(nb_group_values * nb_features, dtype=float)
             coef = coef.reshape(nb_group_values, nb_features)
 
             clr = LogisticRegression(
                 C=self.C, penalty=self.penalty, fit_intercept=self.fit_intercept
             )
             clr.fit(X, y)
 
             coef[:, :] = clr.coef_
 
         elif self.init_type == "StandarLRbyGroup":
             # learned by standard LR
-            coef = np.empty(nb_group_values * nb_features, dtype=np.float)
+            coef = np.empty(nb_group_values * nb_features, dtype=float)
             coef = coef.reshape(nb_group_values, nb_features)
 
             for i in range(nb_group_values):
                 clr = LogisticRegression(
                     C=self.C, penalty=self.penalty, fit_intercept=self.fit_intercept
                 )
                 clr.fit(X[groups == i, :], y[groups == i])
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/prejudice_remover/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/two_sided_fairness/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_bound_update.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_fair_clustering.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_logger.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_method_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         d = A.sum(axis=1)
 
     maxclusterid = np.max(clustering)
     nassoc_e = 0
     num_cluster = 0
     for k in range(maxclusterid + 1):
-        S_k = np.array(clustering == k, dtype=np.float)
+        S_k = np.array(clustering == k, dtype=float)
         # print S_k
         if 0 == np.sum(clustering == k):
             continue  # skip empty cluster
         num_cluster = num_cluster + 1
         if isinstance(A, np.ndarray):
             nassoc_e = nassoc_e + np.dot(np.dot(np.transpose(S_k), A), S_k) / np.dot(
                 np.transpose(d), S_k
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_methods.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/algorithm_utils/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             data = np.ones(X.shape[0] * (knn - 1))
         elif scale is True:
             scale = np.median(dist[:, 1:])
             data = np.exp((-dist[:, 1:] ** 2) / (2 * scale**2)).flatten()
         else:
             data = np.exp((-dist[:, 1:] ** 2) / (2 * scale**2)).flatten()
 
-        W = sparse.csc_matrix((data, (row, col)), shape=(N, N), dtype=np.float)
+        W = sparse.csc_matrix((data, (row, col)), shape=(N, N), dtype=float)
         W = (W + W.transpose(copy=True)) / 2
         elapsed = timeit.default_timer() - start_time
         print(elapsed)
 
         if isinstance(savepath, str):
             if savepath.endswith(".npz"):
                 sparse.save_npz(savepath, W)
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/inprocessing/variational_fair_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/__init__.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/calibrated_eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/debiasing_exposure/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/disparate_impact_remover_rs.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/eq_odds_postprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/fail_prob.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/mtable_generator.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/algorithm_utils/valitation_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/fair_topk/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/binary_balancer/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/constraints.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/lp_debiaser/multiclass_balancer/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/mcmf_clustering/utils/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/randomized_threshold/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/reduce2binary/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/ml_debiaser/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/plugin_estimator_and_recalibration/transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 
     References:
         Chzhen, Evgenii, et al. "Fair regression via plug-in estimator and recalibration with statistical
         guarantees." Advances in Neural Information Processing Systems 33 (2020): 19137-19148.
     """
 
     def __init__(self, L: Optional[int] = 25, beta: Optional[float] = 0.1):
-        """Create a Calibrated Equalized Odds Post-processing instance."""
+        """Create a Plugin Estimation and Calibration Post-processing instance."""
         self.algorithm = PluginEstimationAndCalibrationAlgorithm(L=L, beta=beta)
 
     def fit(self, y_pred: np.ndarray, group_a: np.ndarray, group_b: np.ndarray):
         """
-        Compute parameters for calibrated equalized odds.
+        Compute a fair regression function by minimizing the squared error subject to a fairness constraint.
 
         Description
         ----------
-        Compute parameters for calibrated equalized odds algorithm.
+        Compute a fair predictor by estimating a regression function by standard methods and then estimate
+        the thresholds to solve the minimization problem.
 
         Parameters
         ----------
         y_pred : array-like
             Predicted vector (num_examples, ).
         group_a : array-like
             Group membership vector (binary)
```

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/reject_option_classification.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/postprocessing/wasserstein_barycenters/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/__init__.py` & `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py` & `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/correlation_remover.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py` & `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/disparate_impact_remover.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py` & `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/fairlet_clustering/transformer.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py` & `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/learning_fair_representation.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/mitigation/preprocessing/reweighing.py` & `holisticai-0.5.0/holisticai/bias/mitigation/preprocessing/reweighing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/plots/__init__.py` & `holisticai-0.5.0/holisticai/bias/plots/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """
 The :mod:`holisticai.bias.plots` module includes bias plotters.
 """
 # Classification Plots
 from ._bias_classification_plots import abroca_plot
 
 # Exploratory plots
-from ._bias_exploratory_plots import distribution_plot, group_pie_plot, histogram_plot
+from ._bias_exploratory_plots import (
+    correlation_matrix_plot,
+    distribution_plot,
+    group_pie_plot,
+    histogram_plot,
+)
 
 # Multiclass Plots
 from ._bias_multiclass_plots import (
     accuracy_bar_plot,
     disparate_impact_plot,
     frequency_matrix_plot,
     frequency_plot,
@@ -49,8 +54,9 @@
     "disparate_impact_plot",
     "frequency_matrix_plot",
     "accuracy_bar_plot",
     "long_tail_plot",
     "group_pie_plot",
     "distribution_plot",
     "histogram_plot",
+    "correlation_matrix_plot",
 ]
```

### Comparing `holisticai-0.4.0/holisticai/bias/plots/_bias_classification_plots.py` & `holisticai-0.5.0/holisticai/bias/plots/_bias_classification_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/plots/_bias_exploratory_plots.py` & `holisticai-0.5.0/holisticai/bias/plots/_bias_exploratory_plots.py`

 * *Files 14% similar despite different names*

```diff
@@ -254,7 +254,61 @@
         ax=ax,
     )
     _, labels = plt.xticks()
     plt.setp(labels, rotation=45)
 
     # return
     return ax
+
+
+def correlation_matrix_plot(
+    df, target_feature, n_features=10, cmap="YlGnBu", ax=None, size=None, title=None
+):
+    """Plot the correlation matrix of a given dataframe with respect to
+    a given target and a certain number of features.
+
+    Parameters
+    ----------
+    df : (DataFrame)
+        Pandas dataframe of the data
+    target_feature : (str)
+        Column name of the target feature
+    n_features (optional) : (int)
+        Number of features to plot with the closest correlation to the target
+    cmap (optional) : (str)
+        Color map to use
+    ax (optional) : matplotlib axes
+        Pre-existing axes for the plot
+    size (optional) : (int, int)
+        Size of the figure
+    title (optional) : (str)
+        Title of the figure
+
+    Returns
+    -------
+    matplotlib ax
+    """
+    """Prints the correlation matrix """
+
+    sns.set(font_scale=1.25)
+    if ax is None:
+        fig, ax = plt.subplots(figsize=size)
+        if title is not None:
+            fig.suptitle(title)
+        else:
+            fig.suptitle("Correlation matrix")
+    corrmat = df.corr()
+    cols = corrmat.nlargest(n_features, target_feature)[target_feature].index
+    cm = np.corrcoef(df[cols].values.T)
+    sns.heatmap(
+        cm,
+        cbar=False,
+        annot=True,
+        square=True,
+        fmt=".2f",
+        annot_kws={"size": 10},
+        yticklabels=cols.values,
+        xticklabels=cols.values,
+        cmap=cmap,
+    )
+    plt.setp(ax.get_xticklabels(), rotation=45, ha="right", rotation_mode="anchor")
+    return ax
```

### Comparing `holisticai-0.4.0/holisticai/bias/plots/_bias_multiclass_plots.py` & `holisticai-0.5.0/holisticai/bias/plots/_bias_multiclass_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/plots/_bias_recommender_plots.py` & `holisticai-0.5.0/holisticai/bias/plots/_bias_recommender_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/bias/plots/_bias_regression_plots.py` & `holisticai-0.5.0/holisticai/bias/plots/_bias_regression_plots.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/datasets/_dataloaders.py` & `holisticai-0.5.0/holisticai/datasets/_dataloaders.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/datasets/synthetic/recruitment.py` & `holisticai-0.5.0/holisticai/datasets/synthetic/recruitment.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/datasets/synthetic/user_feedback.py` & `holisticai-0.5.0/holisticai/datasets/synthetic/user_feedback.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/efficacy/metrics.py` & `holisticai-0.5.0/holisticai/efficacy/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,35 +102,35 @@
     pandas DataFrame
         Metrics | Values | Reference
     """
     from sklearn import metrics
 
     perform = {
         "Accuracy": metrics.accuracy_score,
-        "Balanced accuracy": metrics.balanced_accuracy_score,
+        "Balanced Accuracy": metrics.balanced_accuracy_score,
         "Precision": metrics.precision_score,
         "Recall": metrics.recall_score,
         "F1-Score": metrics.f1_score,
     }
 
     hyper = {
         "Accuracy": {},
-        "Balanced accuracy": {},
+        "Balanced Accuracy": {},
         "Precision": {},
         "Recall": {},
         "F1-Score": {},
     }
 
     soft_perform = {"AUC": metrics.roc_auc_score, "Log Loss": metrics.log_loss}
 
     soft_hyper = {"AUC": {"average": "micro"}, "Log Loss": {}}
 
     ref_vals = {
         "Accuracy": 1,
-        "Balanced accuracy": 1,
+        "Balanced Accuracy": 1,
         "Precision": 1,
         "Recall": 1,
         "F1-Score": 1,
         "AUC": 1,
         "Log Loss": 0,
     }
     metrics = [
@@ -248,38 +248,38 @@
     y_pred = convert_to_numeric_array(y_pred, classes)
     y_true = convert_to_numeric_array(y_true, classes)
 
     n_classes = len(classes)
 
     perform = {
         "Accuracy": metrics.accuracy_score,
-        "Balanced accuracy": metrics.balanced_accuracy_score,
+        "Balanced Accuracy": metrics.balanced_accuracy_score,
         "Precision": metrics.precision_score,
         "Recall": metrics.recall_score,
         "F1-Score": metrics.f1_score,
     }
 
     hyper = {
         "Accuracy": {},
-        "Balanced accuracy": {},
+        "Balanced Accuracy": {},
         "Precision": {"average": "micro"},
         "Recall": {"average": "micro"},
         "F1-Score": {"average": "micro"},
     }
 
     soft_perform = {"AUC": metrics.roc_auc_score, "Log Loss": metrics.log_loss}
 
     soft_hyper = {
         "AUC": {"average": "macro", "multi_class": "ovr"},
         "Log Loss": {},
     }
 
     ref_vals = {
         "Accuracy": 1,
-        "Balanced accuracy": 1,
+        "Balanced Accuracy": 1,
         "Precision": 1,
         "Recall": 1,
         "F1-Score": 1,
         "AUC": 1,
         "Log Loss": 0,
     }
```

### Comparing `holisticai-0.4.0/holisticai/pipeline/_pipeline.py` & `holisticai-0.5.0/holisticai/pipeline/_pipeline.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/pipeline/_pipeline_helper.py` & `holisticai-0.5.0/holisticai/pipeline/_pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/pipeline/handlers/_estimator.py` & `holisticai-0.5.0/holisticai/pipeline/handlers/_estimator.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/pipeline/handlers/_pipeline_params.py` & `holisticai-0.5.0/holisticai/pipeline/handlers/_pipeline_params.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/pipeline/handlers/_utransformers.py` & `holisticai-0.5.0/holisticai/pipeline/handlers/_utransformers.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/_formatting.py` & `holisticai-0.5.0/holisticai/utils/_formatting.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/_plotting.py` & `holisticai-0.5.0/holisticai/utils/_plotting.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/_recommender_tools.py` & `holisticai-0.5.0/holisticai/utils/_recommender_tools.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/_validation.py` & `holisticai-0.5.0/holisticai/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/models/cluster/_kcenters.py` & `holisticai-0.5.0/holisticai/utils/models/cluster/_kcenters.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/models/cluster/_kmedoids.py` & `holisticai-0.5.0/holisticai/utils/models/cluster/_kmedoids.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/models/cluster/_utils.py` & `holisticai-0.5.0/holisticai/utils/models/cluster/_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/models/recommender/_rsbase.py` & `holisticai-0.5.0/holisticai/utils/models/recommender/_rsbase.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/models/recommender/item_selection/selectors.py` & `holisticai-0.5.0/holisticai/utils/models/recommender/item_selection/selectors.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py` & `holisticai-0.5.0/holisticai/utils/models/recommender/matrix_factorization/non_negative.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/optimizers/_genetic_algorithm.py` & `holisticai-0.5.0/holisticai/utils/optimizers/_genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/transformers/_transformer_base.py` & `holisticai-0.5.0/holisticai/utils/transformers/_transformer_base.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/transformers/bias/_group_utils.py` & `holisticai-0.5.0/holisticai/utils/transformers/bias/_group_utils.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/transformers/bias/_inprocessing.py` & `holisticai-0.5.0/holisticai/utils/transformers/bias/_inprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/transformers/bias/_postprocessing.py` & `holisticai-0.5.0/holisticai/utils/transformers/bias/_postprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/holisticai/utils/transformers/bias/_preprocessing.py` & `holisticai-0.5.0/holisticai/utils/transformers/bias/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `holisticai-0.4.0/pyproject.toml` & `holisticai-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.commitizen]
-version = "0.4.0"
+version = "0.5.0"
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
 
 [tool.poetry]
 name = "holisticai"
-version = "0.4.0"
+version = "0.5.0"
 description = "Holistic AI Library"
 authors = ["Research Team"]
 maintainers = ["Research Team <researchteam@holisticai.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<4.0.0"
 scikit-learn = ">=1.0.2"
 seaborn = ">=0.11.2"
 tqdm = "^4.64.1"
 cvxpy = {extras = ["cbc"], version = "^1.3.0"}
 cvxopt = "^1.3.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `holisticai-0.4.0/PKG-INFO` & `holisticai-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: holisticai
-Version: 0.4.0
+Version: 0.5.0
 Summary: Holistic AI Library
 Author: Research Team
 Maintainer: Research Team
 Maintainer-email: researchteam@holisticai.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cvxopt (>=1.3.0,<2.0.0)
 Requires-Dist: cvxpy[cbc] (>=1.3.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.2)
 Requires-Dist: seaborn (>=0.11.2)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
@@ -22,18 +23,19 @@
 <br>Holistic AI
 </h1>
 
 The Holistic AI library is an open-source tool to assess and improve the trustworthiness of AI systems.  
 
 Currently, the library offers a set of techniques to easily measure and mitigate Bias across numerous tasks. In the future, it will be extended to include tools for Efficacy, Robustness, Privacy and Explainability as well. This will allow a holistic assessment of AI systems.  
 
-- Documentation:https://holisticai.readthedocs.io/en/latest/ 
+- Documentation: https://holistic-ai.readthedocs.io/en/latest/
 - Tutorials: https://github.com/holistic-ai/holisticai/tree/main/tutorials
 - Source code: https://github.com/holistic-ai/holisticai/tree/main
 - Holistic Ai website: https://holisticai.com
 
 ## Installation
 
 Install the library with:
-
+```bash
     pip install holisticai
+```
```

