# Comparing `tmp/banditcoot-0.1.5.tar.gz` & `tmp/banditcoot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banditcoot-0.1.5.tar", max compression
+gzip compressed data, was "banditcoot-0.1.6.tar", max compression
```

## Comparing `banditcoot-0.1.5.tar` & `banditcoot-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      703 2023-02-24 03:42:56.784428 banditcoot-0.1.5/README.md
--rw-r--r--   0        0        0      438 2023-04-21 03:27:00.377376 banditcoot-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-24 03:42:56.785625 banditcoot-0.1.5/src/banditcoot/__init__.py
--rw-r--r--   0        0        0      211 2023-02-24 03:42:56.785792 banditcoot-0.1.5/src/banditcoot/algorithms/__init__.py
--rw-r--r--   0        0        0     3489 2023-04-21 03:26:49.930802 banditcoot-0.1.5/src/banditcoot/algorithms/_epsilon_greedy.py
--rw-r--r--   0        0        0     1834 2023-02-24 03:42:56.786032 banditcoot-0.1.5/src/banditcoot/algorithms/_softmax.py
--rw-r--r--   0        0        0       68 2023-02-24 03:42:56.786183 banditcoot-0.1.5/src/banditcoot/arms/__init__.py
--rw-r--r--   0        0        0      174 2023-02-24 03:42:56.786284 banditcoot-0.1.5/src/banditcoot/arms/_bernoulli.py
--rw-r--r--   0        0        0       82 2023-02-24 03:42:56.786425 banditcoot-0.1.5/src/banditcoot/utility/__init__.py
--rw-r--r--   0        0        0     1513 2023-02-24 03:42:56.786532 banditcoot-0.1.5/src/banditcoot/utility/_batch_monte_carlo_test.py
--rw-r--r--   0        0        0     1508 2023-02-24 03:42:56.786644 banditcoot-0.1.5/src/banditcoot/utility/_monte_carlo_test.py
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 banditcoot-0.1.5/setup.py
--rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 banditcoot-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      703 2023-02-24 03:42:56.784428 banditcoot-0.1.6/README.md
+-rw-r--r--   0        0        0      496 2023-06-26 23:01:09.614337 banditcoot-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-24 03:42:56.785625 banditcoot-0.1.6/src/banditcoot/__init__.py
+-rw-r--r--   0        0        0      210 2023-06-24 15:47:48.974646 banditcoot-0.1.6/src/banditcoot/algorithms/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-26 01:18:44.766730 banditcoot-0.1.6/src/banditcoot/algorithms/_epsilon_greedy.py
+-rw-r--r--   0        0        0     1834 2023-02-24 03:42:56.786032 banditcoot-0.1.6/src/banditcoot/algorithms/_softmax.py
+-rw-r--r--   0        0        0       68 2023-02-24 03:42:56.786183 banditcoot-0.1.6/src/banditcoot/arms/__init__.py
+-rw-r--r--   0        0        0      299 2023-06-21 17:11:07.648470 banditcoot-0.1.6/src/banditcoot/arms/_bernoulli.py
+-rw-r--r--   0        0        0       82 2023-02-24 03:42:56.786425 banditcoot-0.1.6/src/banditcoot/utility/__init__.py
+-rw-r--r--   0        0        0     1513 2023-06-21 17:11:07.648577 banditcoot-0.1.6/src/banditcoot/utility/_batch_monte_carlo_sim.py
+-rw-r--r--   0        0        0     1514 2023-06-21 17:11:07.648711 banditcoot-0.1.6/src/banditcoot/utility/_monte_carlo_sim.py
+-rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 banditcoot-0.1.6/setup.py
+-rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 banditcoot-0.1.6/PKG-INFO
```

### Comparing `banditcoot-0.1.5/README.md` & `banditcoot-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.5/src/banditcoot/algorithms/_epsilon_greedy.py` & `banditcoot-0.1.6/src/banditcoot/algorithms/_epsilon_greedy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import random
 
-def hello_world(x):
-    result = "hello "+x
-    return result
-
 def ind_max(x):
     """
     returns the index that corresponds to the maximum value in array x
     """
     m = max(x)
     return x.index(m)
 
+def hello_world():
+    """
+    test function to see if package is installed in editable mode
+    """
+    print("hello universe")
+
 class EpsilonGreedy():
     """
 
     Parameters
     ----------
     epsilon: float
         Percentage of time the bandit explores
@@ -33,15 +35,15 @@
         average number of successes observed for each arm (i.e. conversion rate)
     """
     def __init__(self, epsilon, n_arms, rewards, conv_rates=None, counts=None):
         self.epsilon    = epsilon
         self.rewards    = rewards
         self.conv_rates = [0 for i in range(n_arms)] if conv_rates is None else conv_rates
         self.counts     = [0 for i in range(n_arms)] if counts is None else counts
-        self.values     = [i*j for i,j in zip(conv_rates,rewards)]
+        self.values     = [i*j for i,j in zip(self.conv_rates,self.rewards)]
         # raise error if n_arms does not equal number of entries in counts or values
         if ((n_arms != len(self.counts)) or (n_arms != len(self.values)) or (n_arms != len(self.conv_rates))):
             raise ValueError("n_arms does not match the length of counts/values/conv_rates")
         return
 
     def select_arm(self):
         if random.random() > self.epsilon:
@@ -58,30 +60,29 @@
         prev_value = self.values[chosen_arm]
         new_value = ((n - 1) / float(n)) * prev_value + (1 / float(n)) * success_flag * self.rewards[chosen_arm]
         self.values[chosen_arm] = new_value
         return
     
     def batch_update(self, chosen_arm, num_times_chosen, num_successes, observed_reward=None):
         
-        observed_reward = self.rewards[chosen_arm] if observed_reward is None else observed_reward
+        # save previous algo parameter values
+        prev_counts     = self.counts.copy()
+        prev_conv_rates = self.conv_rates.copy()
+        prev_rewards    = self.rewards.copy()
+        prev_values     = self.values.copy()
 
         # increments counts for chosen arm
-        prev_count              = self.counts[chosen_arm]
-        new_count               = prev_count + num_times_chosen
-        self.counts[chosen_arm] = new_count
+        self.counts[chosen_arm] = prev_counts[chosen_arm] + num_times_chosen
 
         # update conversion rates
-        prev_conv_rate              = self.conv_rates[chosen_arm]
-        prev_successes              = prev_count * prev_conv_rate
-        new_conv_rate               = (prev_successes / (prev_successes + num_successes)) * prev_conv_rate + (num_successes / (prev_successes + num_successes)) * (num_successes/num_times_chosen)
-        self.conv_rates[chosen_arm] = new_conv_rate
+        self.conv_rates[chosen_arm] = ((prev_conv_rates[chosen_arm] * prev_counts[chosen_arm]) + num_successes) / self.counts[chosen_arm]
 
         # calculate new average reward for chosen arm
-        total_successes = [i*j for i,j in zip(self.counts, self.conv_rates)]
-        prev_reward = self.rewards[chosen_arm]
-        new_reward = (prev_successes / (prev_successes + num_successes)) * prev_reward + (num_successes / (prev_successes + num_successes)) * observed_reward
-        self.rewards[chosen_arm] = new_reward
+        observed_reward = self.rewards[chosen_arm] if observed_reward is None else observed_reward
+        prev_total_rewards = (prev_rewards[chosen_arm] * prev_conv_rates[chosen_arm] * prev_counts[chosen_arm])
+        new_total_rewards  = num_successes * observed_reward
+        self.rewards[chosen_arm] = (prev_total_rewards + new_total_rewards) / self.counts[chosen_arm]
         
         # calculate new average value for chosen arm
-        self.values[chosen_arm] = self.conv_rates[chosen_arm] * self.rewards[chosen_arm]
+        self.values[chosen_arm] = (self.conv_rates[chosen_arm] * self.counts[chosen_arm] * self.rewards[chosen_arm])/self.counts[chosen_arm]
         return
```

### Comparing `banditcoot-0.1.5/src/banditcoot/algorithms/_softmax.py` & `banditcoot-0.1.6/src/banditcoot/algorithms/_softmax.py`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.5/src/banditcoot/utility/_batch_monte_carlo_test.py` & `banditcoot-0.1.6/src/banditcoot/utility/_batch_monte_carlo_sim.py`

 * *Files identical despite different names*

### Comparing `banditcoot-0.1.5/src/banditcoot/utility/_monte_carlo_test.py` & `banditcoot-0.1.6/src/banditcoot/utility/_monte_carlo_sim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def MonteCarloTest(algo, arms, reward_amounts, n_iter, horizon):
+def MonteCarloSimulation(algo, arms, reward_amounts, n_iter, horizon):
     """
     Monte Carlo simulation used to test bandit algorithms with synthetic data
 
     algo: bandit algorithm of choice
     arms: array of arms to draw from
     n_iter: number of iterations
     horizon: horizon of time to simulate for each iteration
```

### Comparing `banditcoot-0.1.5/setup.py` & `banditcoot-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.5.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'banditcoot',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Python module for developing and testing multi-armed bandits',
     'long_description': 'Banditcoot\n====================\n\n<img align="left" width="75" src="https://github.com/dan-kwon/banditcoot/blob/master/resources/Banditcoot.png"/> \n\n**banditcoot** is a Python module is intended for my own personal use when developing and testing multi-armed bandit algorithms. Forked from the accompanying [code repository](https://github.com/johnmyleswhite/BanditsBook) for [Bandit Algorithms for Website Optimization](https://www.oreilly.com/library/view/bandit-algorithms-for/9781449341565/).\n\n*Any use of this code is at your own risk.*\n</br>\n\n## Installation\n--------------------\nRecommended method of installation is to use pip \n```\npip install banditcoot\n```\n\n\n## Quickstart\n--------------------\n',
     'author': 'dan-kwon',
     'author_email': 'danielkwon02@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `banditcoot-0.1.5/PKG-INFO` & `banditcoot-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banditcoot
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python module for developing and testing multi-armed bandits
 License: MIT
 Author: dan-kwon
 Author-email: danielkwon02@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

