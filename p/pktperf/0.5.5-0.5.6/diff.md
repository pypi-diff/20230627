# Comparing `tmp/pktperf-0.5.5.tar.gz` & `tmp/pktperf-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pktperf-0.5.5.tar", last modified: Fri Jun  9 15:16:41 2023, max compression
+gzip compressed data, was "pktperf-0.5.6.tar", last modified: Tue Jun 27 13:46:42 2023, max compression
```

## Comparing `pktperf-0.5.5.tar` & `pktperf-0.5.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.193414 pktperf-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.189414 pktperf-0.5.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.193414 pktperf-0.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-09 15:16:30.000000 pktperf-0.5.5/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-09 15:16:30.000000 pktperf-0.5.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-09 15:16:30.000000 pktperf-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-09 15:16:30.000000 pktperf-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 15:16:30.000000 pktperf-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-09 15:16:41.193414 pktperf-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-09 15:16:30.000000 pktperf-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-09 15:16:30.000000 pktperf-0.5.5/example.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.193414 pktperf-0.5.5/pktperf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/ethtoolsar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.193414 pktperf-0.5.5/pktperf/module/
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/module/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14580 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/module/common.mk
--rw-r--r--   0 runner    (1001) docker     (123)   144669 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/module/pktgen_5.4.c
--rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/pktgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/pktperf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/pktsar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.193414 pktperf-0.5.5/pktperf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-09 15:16:30.000000 pktperf-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:16:41.193414 pktperf-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 15:16:30.000000 pktperf-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:46:42.509535 pktperf-0.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:46:42.505535 pktperf-0.5.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:46:42.509535 pktperf-0.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-27 13:46:32.000000 pktperf-0.5.6/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-27 13:46:32.000000 pktperf-0.5.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 13:46:32.000000 pktperf-0.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-27 13:46:32.000000 pktperf-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-27 13:46:32.000000 pktperf-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-27 13:46:42.509535 pktperf-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-27 13:46:32.000000 pktperf-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-27 13:46:32.000000 pktperf-0.5.6/example.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:46:42.509535 pktperf-0.5.6/pktperf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:46:32.000000 pktperf-0.5.6/pktperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-06-27 13:46:32.000000 pktperf-0.5.6/pktperf/ethtoolsar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:46:42.509535 pktperf-0.5.6/pktperf/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-27 13:46:32.000000 pktperf-0.5.6/pktperf/module/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14580 2023-06-27 13:46:32.000000 pktperf-0.5.6/pktperf/module/common.mk
+-rw-r--r--   0 runner    (1001) docker     (123)   151530 2023-06-27 13:46:32.000000 pktperf-0.5.6/pktperf/module/pktgen_5.4.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31148 2023-06-27 13:46:32.000000 pktperf-0.5.6/pktperf/pktgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-27 13:46:32.000000 pktperf-0.5.6/pktperf/pktperf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-27 13:46:32.000000 pktperf-0.5.6/pktperf/pktsar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:46:42.509535 pktperf-0.5.6/pktperf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-27 13:46:42.000000 pktperf-0.5.6/pktperf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-27 13:46:42.000000 pktperf-0.5.6/pktperf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:46:42.000000 pktperf-0.5.6/pktperf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-27 13:46:42.000000 pktperf-0.5.6/pktperf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 13:46:42.000000 pktperf-0.5.6/pktperf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 13:46:42.000000 pktperf-0.5.6/pktperf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 13:46:32.000000 pktperf-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 13:46:42.509535 pktperf-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-27 13:46:32.000000 pktperf-0.5.6/setup.py
```

### Comparing `pktperf-0.5.5/.github/workflows/pylint.yml` & `pktperf-0.5.6/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.5/.github/workflows/python-publish.yml` & `pktperf-0.5.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.5/LICENSE` & `pktperf-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.5/PKG-INFO` & `pktperf-0.5.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pktperf
-Version: 0.5.5
+Version: 0.5.6
 Summary: pktgen scripts tool
 Author-email: junka <wan.junjie@foxmail.com>
 Project-URL: Homepage, https://github.com/junka/pktperf
 Project-URL: Bug Tracker, https://github.com/junka/pktperf/issues
 Platform: manylinux2014_x86_64
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pktperf-0.5.5/README.md` & `pktperf-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.5/pktperf/ethtoolsar.py` & `pktperf-0.5.6/pktperf/ethtoolsar.py`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.5/pktperf/module/Makefile` & `pktperf-0.5.6/pktperf/module/Makefile`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.5/pktperf/module/common.mk` & `pktperf-0.5.6/pktperf/module/common.mk`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.5/pktperf/module/pktgen_5.4.c` & `pktperf-0.5.6/pktperf/module/pktgen_5.4.c`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,17 @@
 #include <linux/bitops.h>
 #include <linux/io.h>
 #include <linux/timex.h>
 #include <linux/uaccess.h>
 #include <asm/dma.h>
 #include <asm/div64.h>        /* do_div */
 #include <linux/version.h>
+#include <linux/percpu.h>
+#include <linux/netfilter.h>
+#include <linux/netfilter_ipv4.h>
 
 #if LINUX_VERSION_CODE < KERNEL_VERSION(6, 1, 0)
 #define PRANDOM32_INCLUSIVE(a, b) (prandom_u32() % (b - a) + a)
 #define PRANDOM32_BELOW(v) (prandom_u32() % v)
 #define PRANDOM32() prandom_u32()
 #else
 #define PRANDOM32_INCLUSIVE(a, b) get_random_u32_inclusive(a, b)
@@ -271,14 +274,19 @@
 #define T_REMDEVALL   (1<<2)    /* Remove all devs */
 #define T_REMDEV      (1<<3)    /* Remove one dev */
 
 /* Xmit modes */
 #define M_START_XMIT        0    /* Default normal TX */
 #define M_NETIF_RECEIVE     1    /* Inject packets into stack */
 #define M_QUEUE_XMIT        2    /* Inject packet into qdisc */
+#define M_RX_ONLY           3    /* RX only, no tx packet */
+
+/* tcp modes */
+#define M_SYN_SENT  1
+#define M_SYN_ACK   2
 
 /* If lock -- protects updating of if_list */
 #define if_lock(t)    mutex_lock(&(t->if_lock));
 #define if_unlock(t)  mutex_unlock(&(t->if_lock));
 
 /* Used to help with determining the pkts on receive */
 #define PKTGEN_MAGIC  0xbe9be955
@@ -311,23 +319,32 @@
 #endif
     __u32 flags;
 };
 
 /* flow flag bits */
 #define F_INIT   (1<<0)        /* flow has been initialized */
 
+struct pktgen_rx {
+    u64 rx_packets; /*packets arrived*/
+    u64 rx_bytes;   /*bytes arrived*/
+};
+
+DEFINE_PER_CPU(struct pktgen_rx, pg_rx_stats);
+DEFINE_PER_CPU(struct pktgen_dev *, pg_devs);
+
 struct pktgen_dev {
     /*
      * Try to keep frequent/infrequent used vars. separated.
      */
     struct proc_dir_entry *entry;    /* proc file */
     struct pktgen_thread *pg_thread;/* the owner */
     struct list_head list;        /* chaining in the thread's run-queue */
     struct rcu_head     rcu;        /* freed by RCU */
 
+
     int running;        /* if false, the test will stop */
 
     /* If min != max, then we will either do a linear iteration, or
      * we will do a random selection from within the range.
      */
     __u32 flags;
     int xmit_mode;
@@ -342,14 +359,17 @@
     u64 delay;        /* nano-seconds */
 
     __u64 count;        /* Default No packets to send */
     __u64 sofar;        /* How many pkts we've sent so far */
     __u64 tx_bytes;        /* How many bytes we've transmitted */
     __u64 errors;        /* Errors when trying to transmit, */
 
+    __u64 rx_bytes;
+    __u64 rx_packets;
+
     /* runtime counters relating to clone_skb */
 
     __u32 clone_count;
     int last_ok;        /* Was last skb sent?
                  * Or a failed transmit of some sort?
                  * This will keep sequence numbers in order
                  */
@@ -422,19 +442,21 @@
     __be32 daddr_max;    /* exclusive, dest IP address */
 
     __u16 udp_src_min;    /* inclusive, source UDP port */
     __u16 udp_src_max;    /* exclusive, source UDP port */
     __u16 udp_dst_min;    /* inclusive, dest UDP port */
     __u16 udp_dst_max;    /* exclusive, dest UDP port */
 
-    /* DSCP + ECN */
-    __u8 tos;            /* six MSB of (former) IPv4 TOS
-                are for dscp codepoint */
-    __u8 traffic_class;  /* ditto for the (former) Traffic Class in IPv6
-                (see RFC 3260, sec. 4) */
+    union {
+        /* DSCP + ECN */
+        __u8 tos;            /* six MSB of (former) IPv4 TOS
+                    are for dscp codepoint */
+        __u8 traffic_class;  /* ditto for the (former) Traffic Class in IPv6
+                    (see RFC 3260, sec. 4) */
+    };
 
     /* IMIX */
     unsigned int n_imix_entries;
     struct imix_pkt imix_entries[MAX_IMIX_ENTRIES];
     /* Maps 0-IMIX_PRECISION range to imix_entry based on probability*/
     __u8 imix_distribution[IMIX_PRECISION];
 
@@ -488,14 +510,17 @@
 
     __u8 inner_hh[14];
     __u16 pad1; /* pad out the hh struct to an even 16 bytes */
 
     struct sk_buff *skb;    /* skb we are to transmit next, used for when we
                  * are transmitting the same one multiple times
                  */
+    struct net_device *idev; /* The in-coming device, usually same with
+                              * odev
+                              */
     struct net_device *odev; /* The out-going device.
                   * Note that the device should have it's
                   * pg_info pointer pointing back to this
                   * device.
                   * Set when the user specifies the out-going
                   * device name (not when the inject is
                   * started as it used to do.)
@@ -509,14 +534,15 @@
 
     u16 queue_map_min;
     u16 queue_map_max;
     __u32 skb_priority;    /* skb priority field */
     unsigned int burst;    /* number of duplicated packets to burst */
     int node;               /* Memory node */
 
+    int tcp_mode;
 #ifdef CONFIG_XFRM
     __u8    ipsmode;        /* IPSEC mode (config) */
     __u8    ipsproto;        /* IPSEC type (config) */
     __u32    spi;
     struct xfrm_dst xdst;
     struct dst_ops dstops;
 #endif
@@ -666,219 +692,223 @@
 
 static int pktgen_if_show(struct seq_file *seq, void *v)
 {
     const struct pktgen_dev *pkt_dev = seq->private;
     ktime_t stopped;
     unsigned int i;
     u64 idle;
+    if (pkt_dev->xmit_mode != M_RX_ONLY) {
+        seq_printf(seq,
+            "Params: count %llu  min_pkt_size: %u  max_pkt_size: %u\n",
+            (unsigned long long)pkt_dev->count, pkt_dev->min_pkt_size,
+            pkt_dev->max_pkt_size);
 
-    seq_printf(seq,
-           "Params: count %llu  min_pkt_size: %u  max_pkt_size: %u\n",
-           (unsigned long long)pkt_dev->count, pkt_dev->min_pkt_size,
-           pkt_dev->max_pkt_size);
-
-    if (pkt_dev->n_imix_entries > 0) {
-        seq_puts(seq, "     imix_weights: ");
-        for (i = 0; i < pkt_dev->n_imix_entries; i++) {
-            seq_printf(seq, "%llu,%llu ",
-                   pkt_dev->imix_entries[i].size,
-                   pkt_dev->imix_entries[i].weight);
+        if (pkt_dev->n_imix_entries > 0) {
+            seq_puts(seq, "     imix_weights: ");
+            for (i = 0; i < pkt_dev->n_imix_entries; i++) {
+                seq_printf(seq, "%llu,%llu ",
+                    pkt_dev->imix_entries[i].size,
+                    pkt_dev->imix_entries[i].weight);
+            }
+            seq_puts(seq, "\n");
         }
-        seq_puts(seq, "\n");
-    }
 
-    seq_printf(seq,
-           "     frags: %d  delay: %llu  clone_skb: %d  ifname: %s\n",
-           pkt_dev->nfrags, (unsigned long long) pkt_dev->delay,
-           pkt_dev->clone_skb, pkt_dev->odevname);
-
-    seq_printf(seq, "     flows: %u flowlen: %u\n", pkt_dev->cflows,
-           pkt_dev->lflow);
-
-    if (pkt_dev->pause_time > 0) {
-        seq_printf(seq, "     pause_time: %u poll_time: %u\n", pkt_dev->pause_time,
-                   pkt_dev->poll_time);
-    }
-
-    seq_printf(seq,
-           "     queue_map_min: %u  queue_map_max: %u\n",
-           pkt_dev->queue_map_min,
-           pkt_dev->queue_map_max);
-
-    if (pkt_dev->skb_priority)
-        seq_printf(seq, "     skb_priority: %u\n",
-               pkt_dev->skb_priority);
-
-    if (pkt_dev->tun_vni_min || pkt_dev->tun_udp_dst) {
-        seq_printf(seq, "     tun_udp_dst: 0x%x\n", pkt_dev->tun_udp_dst);
-        seq_printf(seq, "     tun_vni_min: 0x%x tun_vni_max: 0x%x\n",
-                pkt_dev->tun_vni_min, pkt_dev->tun_vni_max);
-        seq_printf(seq, "     tun_dst_min: %s tun_dst_max: %s\n",
-                pkt_dev->tun_dst_min, pkt_dev->tun_dst_max);
-        seq_printf(seq, "     tun_src_min: %s tun_src_max: %s\n",
-                pkt_dev->tun_src_min, pkt_dev->tun_src_max);
-        seq_printf(seq, "     inner_src_mac: %pM inner_dst_mac: %pM\n",
-                pkt_dev->inner_src_mac, pkt_dev->inner_dst_mac);
         seq_printf(seq,
-            "     inner_src_mac_count: %d  inner_dst_mac_count: %d\n",
-            pkt_dev->inner_src_mac_count, pkt_dev->inner_dst_mac_count);
-    }
+            "     frags: %d  delay: %llu  clone_skb: %d  ifname: %s\n",
+            pkt_dev->nfrags, (unsigned long long) pkt_dev->delay,
+            pkt_dev->clone_skb, pkt_dev->odevname);
+
+        seq_printf(seq, "     flows: %u flowlen: %u\n", pkt_dev->cflows,
+            pkt_dev->lflow);
+
+        if (pkt_dev->pause_time > 0) {
+            seq_printf(seq, "     pause_time: %u poll_time: %u\n", pkt_dev->pause_time,
+                    pkt_dev->poll_time);
+        }
 
-    if (pkt_dev->flags & F_IPV6) {
-        seq_printf(seq,
-               "     saddr: %pI6c  min_saddr: %pI6c  max_saddr: %pI6c\n"
-               "     daddr: %pI6c  min_daddr: %pI6c  max_daddr: %pI6c\n",
-               &pkt_dev->in6_saddr,
-               &pkt_dev->min_in6_saddr, &pkt_dev->max_in6_saddr,
-               &pkt_dev->in6_daddr,
-               &pkt_dev->min_in6_daddr, &pkt_dev->max_in6_daddr);
-    } else {
-        seq_printf(seq,
-               "     dst_min: %s  dst_max: %s\n",
-               pkt_dev->dst_min, pkt_dev->dst_max);
         seq_printf(seq,
-               "     src_min: %s  src_max: %s\n",
-               pkt_dev->src_min, pkt_dev->src_max);
-    }
-
-    seq_puts(seq, "     src_mac: ");
-
-    seq_printf(seq, "%pM ",
-           is_zero_ether_addr(pkt_dev->src_mac) ?
-                 pkt_dev->odev->dev_addr : pkt_dev->src_mac);
+            "     queue_map_min: %u  queue_map_max: %u\n",
+            pkt_dev->queue_map_min,
+            pkt_dev->queue_map_max);
+
+        if (pkt_dev->skb_priority)
+            seq_printf(seq, "     skb_priority: %u\n",
+                pkt_dev->skb_priority);
 
-    seq_puts(seq, "dst_mac: ");
-    seq_printf(seq, "%pM\n", pkt_dev->dst_mac);
-
-    seq_printf(seq,
-           "     udp_src_min: %d  udp_src_max: %d"
-           "  udp_dst_min: %d  udp_dst_max: %d\n",
-           pkt_dev->udp_src_min, pkt_dev->udp_src_max,
-           pkt_dev->udp_dst_min, pkt_dev->udp_dst_max);
+        if (pkt_dev->tun_vni_min || pkt_dev->tun_udp_dst) {
+            seq_printf(seq, "     tun_udp_dst: 0x%x\n", pkt_dev->tun_udp_dst);
+            seq_printf(seq, "     tun_vni_min: 0x%x tun_vni_max: 0x%x\n",
+                    pkt_dev->tun_vni_min, pkt_dev->tun_vni_max);
+            seq_printf(seq, "     tun_dst_min: %s tun_dst_max: %s\n",
+                    pkt_dev->tun_dst_min, pkt_dev->tun_dst_max);
+            seq_printf(seq, "     tun_src_min: %s tun_src_max: %s\n",
+                    pkt_dev->tun_src_min, pkt_dev->tun_src_max);
+            seq_printf(seq, "     inner_src_mac: %pM inner_dst_mac: %pM\n",
+                    pkt_dev->inner_src_mac, pkt_dev->inner_dst_mac);
+            seq_printf(seq,
+                "     inner_src_mac_count: %d  inner_dst_mac_count: %d\n",
+                pkt_dev->inner_src_mac_count, pkt_dev->inner_dst_mac_count);
+        }
+
+        if (pkt_dev->flags & F_IPV6) {
+            seq_printf(seq,
+                "     saddr: %pI6c  min_saddr: %pI6c  max_saddr: %pI6c\n"
+                "     daddr: %pI6c  min_daddr: %pI6c  max_daddr: %pI6c\n",
+                &pkt_dev->in6_saddr,
+                &pkt_dev->min_in6_saddr, &pkt_dev->max_in6_saddr,
+                &pkt_dev->in6_daddr,
+                &pkt_dev->min_in6_daddr, &pkt_dev->max_in6_daddr);
+        } else {
+            seq_printf(seq,
+                "     dst_min: %s  dst_max: %s\n",
+                pkt_dev->dst_min, pkt_dev->dst_max);
+            seq_printf(seq,
+                "     src_min: %s  src_max: %s\n",
+                pkt_dev->src_min, pkt_dev->src_max);
+        }
+
+        seq_puts(seq, "     src_mac: ");
+
+        seq_printf(seq, "%pM ",
+            is_zero_ether_addr(pkt_dev->src_mac) ?
+                    pkt_dev->odev->dev_addr : pkt_dev->src_mac);
 
-    seq_printf(seq,
-           "     src_mac_count: %d  dst_mac_count: %d\n",
-           pkt_dev->src_mac_count, pkt_dev->dst_mac_count);
+        seq_puts(seq, "dst_mac: ");
+        seq_printf(seq, "%pM\n", pkt_dev->dst_mac);
 
-    if (pkt_dev->nr_labels) {
-        seq_puts(seq, "     mpls: ");
-        for (i = 0; i < pkt_dev->nr_labels; i++)
-            seq_printf(seq, "%08x%s", ntohl(pkt_dev->labels[i]),
-                   i == pkt_dev->nr_labels-1 ? "\n" : ", ");
-    }
+        seq_printf(seq,
+            "     udp_src_min: %d  udp_src_max: %d"
+            "  udp_dst_min: %d  udp_dst_max: %d\n",
+            pkt_dev->udp_src_min, pkt_dev->udp_src_max,
+            pkt_dev->udp_dst_min, pkt_dev->udp_dst_max);
 
-    if (pkt_dev->vlan_id != 0xffff)
-        seq_printf(seq, "     vlan_id: %u  vlan_p: %u  vlan_cfi: %u\n",
-               pkt_dev->vlan_id, pkt_dev->vlan_p,
-               pkt_dev->vlan_cfi);
+        seq_printf(seq,
+            "     src_mac_count: %d  dst_mac_count: %d\n",
+            pkt_dev->src_mac_count, pkt_dev->dst_mac_count);
 
-    if (pkt_dev->svlan_id != 0xffff)
-        seq_printf(seq, "     svlan_id: %u  vlan_p: %u  vlan_cfi: %u\n",
-               pkt_dev->svlan_id, pkt_dev->svlan_p,
-               pkt_dev->svlan_cfi);
+        if (pkt_dev->nr_labels) {
+            seq_puts(seq, "     mpls: ");
+            for (i = 0; i < pkt_dev->nr_labels; i++)
+                seq_printf(seq, "%08x%s", ntohl(pkt_dev->labels[i]),
+                    i == pkt_dev->nr_labels-1 ? "\n" : ", ");
+        }
+
+        if (pkt_dev->vlan_id != 0xffff)
+            seq_printf(seq, "     vlan_id: %u  vlan_p: %u  vlan_cfi: %u\n",
+                pkt_dev->vlan_id, pkt_dev->vlan_p,
+                pkt_dev->vlan_cfi);
+
+        if (pkt_dev->svlan_id != 0xffff)
+            seq_printf(seq, "     svlan_id: %u  vlan_p: %u  vlan_cfi: %u\n",
+                pkt_dev->svlan_id, pkt_dev->svlan_p,
+                pkt_dev->svlan_cfi);
 
-    if (pkt_dev->tos)
-        seq_printf(seq, "     tos: 0x%02x\n", pkt_dev->tos);
+        if (pkt_dev->tos)
+            seq_printf(seq, "     tos: 0x%02x\n", pkt_dev->tos);
 
-    if (pkt_dev->traffic_class)
-        seq_printf(seq, "     traffic_class: 0x%02x\n", pkt_dev->traffic_class);
+        if (pkt_dev->traffic_class)
+            seq_printf(seq, "     traffic_class: 0x%02x\n", pkt_dev->traffic_class);
 
-    if (pkt_dev->burst > 1)
-        seq_printf(seq, "     burst: %d\n", pkt_dev->burst);
+        if (pkt_dev->burst > 1)
+            seq_printf(seq, "     burst: %d\n", pkt_dev->burst);
 
-    if (pkt_dev->node >= 0)
-        seq_printf(seq, "     node: %d\n", pkt_dev->node);
+        if (pkt_dev->node >= 0)
+            seq_printf(seq, "     node: %d\n", pkt_dev->node);
 
-    if (pkt_dev->xmit_mode == M_NETIF_RECEIVE)
-        seq_puts(seq, "     xmit_mode: netif_receive\n");
-    else if (pkt_dev->xmit_mode == M_QUEUE_XMIT)
-        seq_puts(seq, "     xmit_mode: xmit_queue\n");
+        if (pkt_dev->xmit_mode == M_NETIF_RECEIVE)
+            seq_puts(seq, "     xmit_mode: netif_receive\n");
+        else if (pkt_dev->xmit_mode == M_QUEUE_XMIT)
+            seq_puts(seq, "     xmit_mode: xmit_queue\n");
 
-    seq_puts(seq, "     Flags: ");
+        seq_puts(seq, "     Flags: ");
 
-    for (i = 0; i < NR_PKT_FLAGS; i++) {
-        if (i == F_FLOW_SEQ)
-            if (!pkt_dev->cflows)
-                continue;
+        for (i = 0; i < NR_PKT_FLAGS; i++) {
+            if (i == F_FLOW_SEQ)
+                if (!pkt_dev->cflows)
+                    continue;
 
-        if (pkt_dev->flags & (1 << i))
-            seq_printf(seq, "%s  ", pkt_flag_names[i]);
-        else if (i == F_FLOW_SEQ)
-            seq_puts(seq, "FLOW_RND  ");
+            if (pkt_dev->flags & (1 << i))
+                seq_printf(seq, "%s  ", pkt_flag_names[i]);
+            else if (i == F_FLOW_SEQ)
+                seq_puts(seq, "FLOW_RND  ");
 
 #ifdef CONFIG_XFRM
-        if (i == F_IPSEC && pkt_dev->spi)
-            seq_printf(seq, "spi:%u", pkt_dev->spi);
+            if (i == F_IPSEC && pkt_dev->spi)
+                seq_printf(seq, "spi:%u", pkt_dev->spi);
 #endif
-    }
-
-    seq_puts(seq, "\n");
+        }
 
+        seq_puts(seq, "\n");
+    }
     /* not really stopped, more like last-running-at */
     stopped = pkt_dev->running ? ktime_get() : pkt_dev->stopped_at;
     idle = pkt_dev->idle_acc;
     do_div(idle, NSEC_PER_USEC);
 
-    seq_printf(seq,
-           "Current:\n     pkts-sofar: %llu  errors: %llu\n",
-           (unsigned long long)pkt_dev->sofar,
-           (unsigned long long)pkt_dev->errors);
+    seq_printf(seq, "Current:\n");
+    if (pkt_dev->xmit_mode != M_RX_ONLY) {
+        seq_printf(seq, "     pkts-sofar: %llu  errors: %llu\n",
+                (unsigned long long)pkt_dev->sofar,
+                (unsigned long long)pkt_dev->errors);
+    } else {
+        seq_printf(seq, "     pkts-rx: %llu  bytes: %llu\n",
+                (unsigned long long)pkt_dev->rx_packets,
+                (unsigned long long)pkt_dev->rx_bytes);
+    }
+
+    seq_printf(seq, "     started: %lluus  stopped: %lluus idle: %lluus\n",
+               (unsigned long long)ktime_to_us(pkt_dev->started_at),
+               (unsigned long long)ktime_to_us(stopped),
+               (unsigned long long)idle);
 
-    if (pkt_dev->n_imix_entries > 0) {
-        int i;
+    if (pkt_dev->xmit_mode != M_RX_ONLY) {
+        if (pkt_dev->n_imix_entries > 0) {
+            int i;
 
-        seq_puts(seq, "     imix_size_counts: ");
-        for (i = 0; i < pkt_dev->n_imix_entries; i++) {
-            seq_printf(seq, "%llu,%llu ",
-                   pkt_dev->imix_entries[i].size,
-                   pkt_dev->imix_entries[i].count_so_far);
+            seq_puts(seq, "     imix_size_counts: ");
+            for (i = 0; i < pkt_dev->n_imix_entries; i++) {
+                seq_printf(seq, "%llu,%llu ",
+                    pkt_dev->imix_entries[i].size,
+                    pkt_dev->imix_entries[i].count_so_far);
+            }
+            seq_puts(seq, "\n");
         }
-        seq_puts(seq, "\n");
-    }
 
-    seq_printf(seq,
-           "     started: %lluus  stopped: %lluus idle: %lluus\n",
-           (unsigned long long) ktime_to_us(pkt_dev->started_at),
-           (unsigned long long) ktime_to_us(stopped),
-           (unsigned long long) idle);
-
-    seq_printf(seq,
-           "     seq_num: %d  cur_dst_mac_offset: %d  cur_src_mac_offset: %d\n",
-           pkt_dev->seq_num, pkt_dev->cur_dst_mac_offset,
-           pkt_dev->cur_src_mac_offset);
-
-    if (pkt_dev->cur_tun_vni) {
-        seq_printf(seq, "     cur_tun_vni: %d  tun_udp_dst: %d\n",
-                pkt_dev->cur_tun_vni,
-                pkt_dev->tun_udp_dst);
-        seq_printf(seq, "     cur_tun_saddr: %pI4  cur_tun_daddr: %pI4\n",
-                &pkt_dev->cur_tun_saddr,
-                &pkt_dev->cur_tun_daddr);
-    }
 
-    if (pkt_dev->flags & F_IPV6) {
-        seq_printf(seq, "     cur_saddr: %pI6c  cur_daddr: %pI6c\n",
-                &pkt_dev->cur_in6_saddr,
-                &pkt_dev->cur_in6_daddr);
-    } else
-        seq_printf(seq, "     cur_saddr: %pI4  cur_daddr: %pI4\n",
-               &pkt_dev->cur_saddr, &pkt_dev->cur_daddr);
-
-    seq_printf(seq, "     cur_udp_dst: %d  cur_udp_src: %d\n",
-           pkt_dev->cur_udp_dst, pkt_dev->cur_udp_src);
+        seq_printf(seq,
+            "     seq_num: %d  cur_dst_mac_offset: %d  cur_src_mac_offset: %d\n",
+            pkt_dev->seq_num, pkt_dev->cur_dst_mac_offset,
+            pkt_dev->cur_src_mac_offset);
+
+        if (pkt_dev->cur_tun_vni) {
+            seq_printf(seq, "     cur_tun_vni: %d  tun_udp_dst: %d\n",
+                    pkt_dev->cur_tun_vni, pkt_dev->tun_udp_dst);
+            seq_printf(seq, "     cur_tun_saddr: %pI4  cur_tun_daddr: %pI4\n",
+                    &pkt_dev->cur_tun_saddr, &pkt_dev->cur_tun_daddr);
+        }
 
-    seq_printf(seq, "     cur_queue_map: %u\n", pkt_dev->cur_queue_map);
+        if (pkt_dev->flags & F_IPV6) {
+            seq_printf(seq, "     cur_saddr: %pI6c  cur_daddr: %pI6c\n",
+                    &pkt_dev->cur_in6_saddr, &pkt_dev->cur_in6_daddr);
+        } else
+            seq_printf(seq, "     cur_saddr: %pI4  cur_daddr: %pI4\n",
+                &pkt_dev->cur_saddr, &pkt_dev->cur_daddr);
 
-    seq_printf(seq, "     flows: %u\n", pkt_dev->nflows);
+        seq_printf(seq, "     cur_udp_dst: %d  cur_udp_src: %d\n",
+            pkt_dev->cur_udp_dst, pkt_dev->cur_udp_src);
 
-    if (pkt_dev->result[0])
-        seq_printf(seq, "Result: %s\n", pkt_dev->result);
-    else
-        seq_puts(seq, "Result: Idle\n");
+        seq_printf(seq, "     cur_queue_map: %u\n", pkt_dev->cur_queue_map);
+
+        seq_printf(seq, "     flows: %u\n", pkt_dev->nflows);
 
+        if (pkt_dev->result[0])
+            seq_printf(seq, "Result: %s\n", pkt_dev->result);
+        else
+            seq_puts(seq, "Result: Idle\n");
+    }
     return 0;
 }
 
 
 static int hex32_arg(const char __user *user_buffer, unsigned long maxlen,
              __u32 *num)
 {
@@ -1227,14 +1257,38 @@
         i += len;
         pkt_dev->pause_time = value;
         sprintf(pg_result, "OK: micro_burst=%u,%u", pkt_dev->poll_time,
                 pkt_dev->pause_time);
         return count;
     }
 
+    if (!strcmp(name, "syn_flood") || !strcmp(name, "tcp_syn")) {
+        char f[32];
+
+        memset(f, 0, 32);
+        len = strn_len(&user_buffer[i], sizeof(f) - 1);
+        if (len < 0)
+            return len;
+
+        if (copy_from_user(f, &user_buffer[i], len))
+            return -EFAULT;
+        i += len;
+        if (!strcmp(f, "syn")) {
+            pkt_dev->tcp_mode = M_SYN_SENT;
+        } else if (!strcmp(f, "syn_ack")) {
+            pkt_dev->tcp_mode = M_SYN_ACK;
+        } else {
+            sprintf(pg_result, "tcp syn mode -:%s:- unknown\nAvailable modes: %s",
+                    f, "syn, syn_ack\n");
+            return count;
+        }
+        sprintf(pg_result, "OK: syn_flood=%s", f);
+        return count;
+    }
+
     if (!strcmp(name, "debug")) {
         len = num_arg(&user_buffer[i], 10, &value);
         if (len < 0)
             return len;
 
         i += len;
         debug = value;
@@ -1471,14 +1525,18 @@
             /* override clone_skb if user passed default value
              * at module loading time
              */
             pkt_dev->clone_skb = 0;
         } else if (strcmp(f, "queue_xmit") == 0) {
             pkt_dev->xmit_mode = M_QUEUE_XMIT;
             pkt_dev->last_ok = 1;
+        } else if (strcmp(f, "rx_only") == 0) {
+            pkt_dev->xmit_mode = M_RX_ONLY;
+            pkt_dev->last_ok = 1;
+            pkt_dev->clone_skb = 0;
         } else {
             sprintf(pg_result,
                 "xmit_mode -:%s:- unknown\nAvailable modes: %s",
                 f, "start_xmit, netif_receive\n");
             return count;
         }
         sprintf(pg_result, "OK: xmit_mode=%s", f);
@@ -2159,14 +2217,28 @@
         if (value != pkt_dev->tun_udp_dst) {
             pkt_dev->tun_udp_dst = value;
         }
         sprintf(pg_result, "OK: tun_udp_dst=%u", pkt_dev->tun_udp_dst);
         return count;
     }
 
+    if (!strcmp(name, "rx_cmd")) {
+        char f[32];
+        memset(f, 0, 32);
+        len = strn_len(&user_buffer[i], sizeof(f) - 1);
+        if (len < 0) {
+            return len;
+        }
+        if (copy_from_user(f, &user_buffer[i], len))
+            return -EFAULT;
+        i += len;
+        sprintf(pg_result, "OK: rx_cmd=%s", f);
+        return count;
+    }
+
     sprintf(pkt_dev->result, "No such parameter \"%s\"", name);
     return -EINVAL;
 }
 
 static int pktgen_if_open(struct inode *inode, struct file *file)
 {
     return single_open(file, pktgen_if_show, PDE_DATA(inode));
@@ -2426,15 +2498,14 @@
         break;
     }
 
     return NOTIFY_DONE;
 }
 
 static struct net_device *pktgen_dev_get_by_name(const struct pktgen_net *pn,
-                         struct pktgen_dev *pkt_dev,
                          const char *ifname)
 {
     char b[IFNAMSIZ+5];
     int i;
 
     for (i = 0; ifname[i] != '@'; i++) {
         if (i == IFNAMSIZ)
@@ -2445,46 +2516,44 @@
     b[i] = 0;
 
     return dev_get_by_name(pn->net, b);
 }
 
 
 /* Associate pktgen_dev with a device. */
-
 static int pktgen_setup_dev(const struct pktgen_net *pn,
-                struct pktgen_dev *pkt_dev, const char *ifname)
+                             struct net_device **dev, const char *ifname)
 {
-    struct net_device *odev;
+    struct net_device *idev;
     int err;
 
     /* Clean old setups */
-    if (pkt_dev->odev) {
-
-        dev_put(pkt_dev->odev);
-        pkt_dev->odev = NULL;
+    if (*dev) {
+        dev_put(*dev);
+        *dev = NULL;
     }
 
-    odev = pktgen_dev_get_by_name(pn, pkt_dev, ifname);
-    if (!odev) {
+    idev = pktgen_dev_get_by_name(pn, ifname);
+    if (!idev) {
         pr_err("no such netdevice: \"%s\"\n", ifname);
         return -ENODEV;
     }
 
-    if (odev->type != ARPHRD_ETHER) {
+    if (idev->type != ARPHRD_ETHER) {
         pr_err("not an ethernet device: \"%s\"\n", ifname);
         err = -EINVAL;
-    } else if (!netif_running(odev)) {
+    } else if (!netif_running(idev)) {
         pr_err("device is down: \"%s\"\n", ifname);
         err = -ENETDOWN;
     } else {
-        pkt_dev->odev = odev;
+        *dev = idev;
         return 0;
     }
 
-    dev_put(odev);
+    dev_put(idev);
     return err;
 }
 
 /* Read pkt_dev from the interface and set up internal pktgen_dev
  * structure to have the right information to create/send packets
  */
 static void pktgen_setup_inject(struct pktgen_dev *pkt_dev)
@@ -3400,33 +3469,36 @@
         *vlan_encapsulated_proto = htons(ETH_P_IPV6);
     }
 }
 
 static void fill_ipv4_layer(struct iphdr *iph, struct pktgen_dev *pkt_dev,
                      int datalen, bool tun)
 {
-    int iplen;
+    int iplen = 20 + 8 + datalen;
     iph->ihl = 5;
     iph->version = 4;
     iph->ttl = 32;
     iph->tos = pkt_dev->tos;
-    iph->protocol = IPPROTO_UDP;    /* UDP */
+    iph->protocol = IPPROTO_UDP; /* UDP */
     if (tun) {
         iph->saddr = pkt_dev->cur_tun_saddr;
         iph->daddr = pkt_dev->cur_tun_daddr;
         iph->id = htons(pkt_dev->tun_ip_id);
         pkt_dev->tun_ip_id ++;
     } else {
         iph->saddr = pkt_dev->cur_saddr;
         iph->daddr = pkt_dev->cur_daddr;
         iph->id = htons(pkt_dev->ip_id);
         pkt_dev->ip_id ++;
+        if (pkt_dev->tcp_mode) {
+            iph->protocol = IPPROTO_TCP;
+            iplen = 20 + datalen + sizeof(struct tcphdr);
+        }
     }
     iph->frag_off = 0;
-    iplen = 20 + 8 + datalen;
     iph->tot_len = htons(iplen);
     ip_send_check(iph);
 }
 
 static inline __be16 udp_tun_flow_src_port(struct sk_buff *skb, int min, int max)
 {
     u32 hash = jhash(skb->data + 50 + ETH_HLEN + 12, 12, skb->protocol);
@@ -3450,21 +3522,31 @@
 }
 
 static void fill_tcp_syn(struct sk_buff *skb, struct tcphdr *tcph,
                          struct pktgen_dev *pkt_dev, int datalen)
 {
     tcph->source = htons(pkt_dev->cur_udp_src);
     tcph->dest = htons(pkt_dev->cur_udp_dst);
-    // tcph->len = htons(datalen + 8); /* DATA + udphdr */
     tcph->check = 0;
     tcph->seq = 0;
     tcph->ack_seq = 0;
-    tcph->window = htons(0x100);
+    tcph->window = htons(0x4000);
     tcph->urg_ptr = 0;
     tcph->syn = 1;
+    if (pkt_dev->tcp_mode == M_SYN_ACK) {\
+        tcph->ack = 1;
+    } else {
+        tcph->ack = 0;
+    }
+    tcph->urg = 0;
+    tcph->ece = 0;
+    tcph->fin = 0;
+    tcph->psh = 0;
+    tcph->cwr = 0;
+    tcph->rst = 0;
     tcph->doff = 5;
     tcph->res1 = 0;
 }
 
 static void fill_ipv6_layer(struct ipv6hdr *iph, struct pktgen_dev *pkt_dev,
                      int datalen, bool tun)
 {
@@ -3482,19 +3564,21 @@
     iph->nexthdr = IPPROTO_UDP;
     if (tun) {
         iph->daddr = pkt_dev->cur_tun6_daddr;
         iph->saddr = pkt_dev->cur_tun6_saddr;
     } else {
         iph->daddr = pkt_dev->cur_in6_daddr;
         iph->saddr = pkt_dev->cur_in6_saddr;
+        if (pkt_dev->tcp_mode) {
+            iph->nexthdr = IPPROTO_TCP;
+        }
     }
 
 }
 
-
 static void fill_ipv4_csum(struct net_device *odev, struct pktgen_dev *pkt_dev,
                     struct sk_buff *skb, int datalen,
                     struct iphdr *iph, struct udphdr *udph)
 {
     if (!(pkt_dev->flags & F_UDPCSUM)) {
         skb->ip_summed = CHECKSUM_NONE;
     } else if (odev->features & (NETIF_F_HW_CSUM | NETIF_F_IP_CSUM)) {
@@ -3509,14 +3593,37 @@
                         datalen + 8, IPPROTO_UDP, csum);
 
         if (udph->check == 0)
             udph->check = CSUM_MANGLED_0;
     }
 }
 
+static void fill_ipv4_tcp_csum(struct net_device *odev, struct pktgen_dev *pkt_dev,
+                           struct sk_buff *skb, int datalen, struct iphdr *iph,
+                           struct tcphdr *tcph) {
+    if (!(pkt_dev->flags & F_UDPCSUM)) {
+        skb->ip_summed = CHECKSUM_NONE;
+    } else if (odev->features & (NETIF_F_HW_CSUM | NETIF_F_IP_CSUM)) {
+        skb->ip_summed = CHECKSUM_PARTIAL;
+        skb->csum = ~tcp_v4_check(skb->len, iph->saddr, iph->daddr, 0);
+        skb->csum_start = skb_transport_header(skb) - skb->head;
+        skb->csum_offset = offsetof(struct tcphdr, check);
+    } else {
+        __wsum csum = skb_checksum(skb, skb_transport_offset(skb),
+                                   datalen + sizeof(struct tcphdr), 0);
+
+        /* add protocol-dependent pseudo-header */
+        tcph->check = csum_tcpudp_magic(iph->saddr, iph->daddr, datalen + sizeof(struct tcphdr),
+                                        IPPROTO_TCP, csum);
+
+        if (tcph->check == 0)
+            tcph->check = CSUM_MANGLED_0;
+    }
+}
+
 static void fill_ipv6_csum(struct net_device *odev, struct pktgen_dev *pkt_dev,
                     struct sk_buff *skb, int datalen,
                     struct ipv6hdr *iph, struct udphdr *udph)
 {
     int udplen = datalen + sizeof(struct udphdr);
     if (!(pkt_dev->flags & F_UDPCSUM)) {
         skb->ip_summed = CHECKSUM_NONE;
@@ -3550,14 +3657,15 @@
 
 static struct sk_buff *fill_packet_ipv4(struct net_device *odev,
                     struct pktgen_dev *pkt_dev)
 {
     struct sk_buff *skb = NULL;
     __u8 *eth;
     struct udphdr *udph;
+    struct tcphdr *tcph;
     int datalen;
     struct iphdr *iph;
     __be16 protocol = htons(ETH_P_IP);
     u16 queue_map;
 
     if (pkt_dev->nr_labels)
         protocol = htons(ETH_P_MPLS_UC);
@@ -3587,37 +3695,52 @@
     fill_skb_vlan(skb, pkt_dev);
 
     skb_reset_mac_header(skb);
     skb_set_network_header(skb, skb->len);
     iph = skb_put(skb, sizeof(struct iphdr));
 
     skb_set_transport_header(skb, skb->len);
-    udph = skb_put(skb, sizeof(struct udphdr));
+    if (pkt_dev->tcp_mode) {
+        tcph = skb_put(skb, sizeof(struct tcphdr));
+    } else {
+        udph = skb_put(skb, sizeof(struct udphdr));
+    }
     skb_set_queue_mapping(skb, queue_map);
     skb->priority = pkt_dev->skb_priority;
 
     fill_ether_layer(eth, pkt_dev, protocol, false);
 
     /* Eth + IPh + UDPh + mpls */
-    datalen = pkt_dev->cur_pkt_size - 14 - 20 - 8 -
+    datalen = pkt_dev->cur_pkt_size - 14 - 20 -
           pkt_dev->pkt_overhead;
+    if (pkt_dev->tcp_mode) {
+        datalen -= sizeof(struct tcphdr);
+    } else {
+        datalen -= 8;
+    }
     if (datalen < 0 || datalen < sizeof(struct pktgen_hdr))
         datalen = sizeof(struct pktgen_hdr);
 
-    fill_udp_layer(skb, udph, pkt_dev, datalen, false);
+    if (pkt_dev->tcp_mode) {
+        fill_tcp_syn(skb, tcph, pkt_dev, datalen);
+    } else {
+        fill_udp_layer(skb, udph, pkt_dev, datalen, false);
+    }
     fill_ipv4_layer(iph, pkt_dev, datalen, false);
 
     skb->protocol = protocol;
     skb->dev = odev;
     skb->pkt_type = PACKET_HOST;
 
     pktgen_finalize_skb(pkt_dev, skb, datalen);
-
-    fill_ipv4_csum(odev, pkt_dev, skb, datalen, iph, udph);
-
+    if (pkt_dev->tcp_mode) {
+        fill_ipv4_tcp_csum(odev, pkt_dev, skb, datalen, iph, tcph);
+    } else {
+        fill_ipv4_csum(odev, pkt_dev, skb, datalen, iph, udph);
+    }
 #ifdef CONFIG_XFRM
     if (!process_ipsec(pkt_dev, skb, protocol))
         return NULL;
 #endif
 
     return skb;
 }
@@ -3630,33 +3753,44 @@
 
 static void fill_inner_packet(struct sk_buff *skb, struct pktgen_dev *pkt_dev,
                               int data_len)
 {
     __be16 protocol = htons(ETH_P_IPV6);
     __u8 *inner_eth;
     struct udphdr *inner_udph;
+    struct tcphdr *inner_tcph;
     struct iphdr *inner_iph;
     struct ipv6hdr *inner_iph6;
 
     inner_eth = skb_put(skb, 14);
     if (pkt_dev->flags & F_IPV6) {
         inner_iph6 = skb_put(skb, sizeof(struct ipv6hdr));
     } else {
         protocol = htons(ETH_P_IP);
         inner_iph = skb_put(skb, sizeof(struct iphdr));
     }
-    inner_udph = skb_put(skb, sizeof(struct udphdr));
+
+    if (pkt_dev->tcp_mode) {
+        inner_tcph = skb_put(skb, sizeof(struct tcphdr));
+    } else {
+        inner_udph = skb_put(skb, sizeof(struct udphdr));
+    }
 
     fill_ether_layer(inner_eth, pkt_dev, protocol, true);
     if (pkt_dev->flags & F_IPV6) {
         fill_ipv6_layer(inner_iph6, pkt_dev, data_len, false);
     } else {
         fill_ipv4_layer(inner_iph, pkt_dev, data_len, false);
     }
-    fill_udp_layer(skb, inner_udph, pkt_dev, data_len, false);
+
+    if (pkt_dev->tcp_mode) {
+        fill_tcp_syn(skb, inner_tcph, pkt_dev, data_len);
+    } else {
+        fill_udp_layer(skb, inner_udph, pkt_dev, data_len, false);
+    }
 }
 
 static struct sk_buff *fill_tun_packet_ipv4(struct net_device *odev,
                     struct pktgen_dev *pkt_dev)
 {
     struct sk_buff *skb = NULL;
     __u8 *eth;
@@ -3705,15 +3839,20 @@
     skb_set_transport_header(skb, skb->len);
     udph = skb_put(skb, sizeof(struct udphdr));
 
     vxh = skb_put(skb, sizeof(struct vxlanhdr));
     /* Eth + IPh + UDPh + mpls */
     datalen = pkt_dev->cur_pkt_size - 14 - 20 - 8 - pkt_dev->pkt_overhead;
     /* vxlan + ether + ip + udp */
-    inner_datalen = datalen - 8 - 14 - 20 - 8;
+    inner_datalen = datalen - 8 - 14 - 20;
+    if (pkt_dev->tcp_mode) {
+        inner_datalen -= sizeof(struct tcphdr);
+    } else {
+        inner_datalen -= 8;
+    }
     if (datalen < 0 || datalen < sizeof(struct pktgen_hdr))
         datalen = sizeof(struct pktgen_hdr) + 50;
     if (inner_datalen < 0 || inner_datalen < sizeof(struct pktgen_hdr))
         inner_datalen = sizeof(struct pktgen_hdr);
 
     fill_vxlan_layer(vxh, pkt_dev);
 
@@ -3723,15 +3862,14 @@
     fill_udp_layer(skb, udph, pkt_dev, datalen, true);
     fill_ipv4_layer(iph, pkt_dev, datalen, true);
 
     skb->pkt_type = PACKET_HOST;
 
     pktgen_finalize_skb(pkt_dev, skb, inner_datalen);
 
-    //fill_ipv4_csum(odev, pkt_dev, skb, inner_datalen, inner_iph, inner_udph);
     fill_ipv4_csum(odev, pkt_dev, skb, datalen, iph, udph);
 
 #ifdef CONFIG_XFRM
     if (!process_ipsec(pkt_dev, skb, protocol))
         return NULL;
 #endif
 
@@ -3741,14 +3879,15 @@
 
 static struct sk_buff *fill_packet_ipv6(struct net_device *odev,
                     struct pktgen_dev *pkt_dev)
 {
     struct sk_buff *skb = NULL;
     __u8 *eth;
     struct udphdr *udph;
+    struct tcphdr *tcph;
     int datalen;
     struct ipv6hdr *iph;
     __be16 protocol = htons(ETH_P_IPV6);
     u16 queue_map;
 
     if (pkt_dev->nr_labels)
         protocol = htons(ETH_P_MPLS_UC);
@@ -3778,31 +3917,43 @@
     fill_skb_vlan(skb, pkt_dev);
 
     skb_reset_mac_header(skb);
     skb_set_network_header(skb, skb->len);
     iph = skb_put(skb, sizeof(struct ipv6hdr));
 
     skb_set_transport_header(skb, skb->len);
-    udph = skb_put(skb, sizeof(struct udphdr));
+    if (pkt_dev->tcp_mode) {
+        tcph = skb_put(skb, sizeof(struct tcphdr));
+    } else {
+        udph = skb_put(skb, sizeof(struct udphdr));
+    }
     skb_set_queue_mapping(skb, queue_map);
     skb->priority = pkt_dev->skb_priority;
 
     fill_ether_layer(eth, pkt_dev, protocol, false);
 
     /* Eth + IPh + UDPh + mpls */
     datalen = pkt_dev->cur_pkt_size - 14 -
-          sizeof(struct ipv6hdr) - sizeof(struct udphdr) -
+          sizeof(struct ipv6hdr) -
           pkt_dev->pkt_overhead;
-
+    if (pkt_dev->tcp_mode) {
+        datalen -= sizeof(struct tcphdr);
+    } else {
+        datalen -= sizeof(struct udphdr);
+    }
     if (datalen < 0 || datalen < sizeof(struct pktgen_hdr)) {
         datalen = sizeof(struct pktgen_hdr);
         net_info_ratelimited("increased datalen to %d\n", datalen);
     }
 
-    fill_udp_layer(skb, udph, pkt_dev, datalen, false);
+    if (pkt_dev->tcp_mode) {
+        fill_tcp_syn(skb, tcph, pkt_dev, datalen);
+    } else {
+        fill_udp_layer(skb, udph, pkt_dev, datalen, false);
+    }
     fill_ipv6_layer(iph, pkt_dev, datalen, false);
 
     skb->protocol = protocol;
     skb->dev = odev;
     skb->pkt_type = PACKET_HOST;
 
     pktgen_finalize_skb(pkt_dev, skb, datalen);
@@ -3867,15 +4018,20 @@
     vxh = skb_put(skb, sizeof(struct vxlanhdr));
 
     /* Eth + IPh + UDPh + mpls */
     datalen = pkt_dev->cur_pkt_size - 14 -
           sizeof(struct ipv6hdr) - sizeof(struct udphdr) -
           pkt_dev->pkt_overhead;
     /* vxlan + ether + ip6 + udp */
-    inner_datalen = datalen - 8 - 14 - 40 - 8;
+    inner_datalen = datalen - 8 - 14 - 40;
+    if (pkt_dev->tcp_mode) {
+        inner_datalen -= sizeof(struct tcphdr);
+    } else {
+        inner_datalen -= sizeof(struct udphdr);
+    }
 
     if (datalen < 0 || datalen < sizeof(struct pktgen_hdr)) {
         datalen = sizeof(struct pktgen_hdr) + 70;
         net_info_ratelimited("increased datalen to %d\n", datalen);
     }
     if (inner_datalen < 0 || inner_datalen < sizeof(struct pktgen_hdr))
         inner_datalen = sizeof(struct pktgen_hdr);
@@ -3913,19 +4069,27 @@
     else
         return fill_tun_packet_ipv4(odev, pkt_dev);
 }
 
 
 static void pktgen_clear_counters(struct pktgen_dev *pkt_dev)
 {
+    int cpu = 0;
     pkt_dev->seq_num = 1;
     pkt_dev->idle_acc = 0;
     pkt_dev->sofar = 0;
     pkt_dev->tx_bytes = 0;
     pkt_dev->errors = 0;
+
+    pkt_dev->rx_bytes = 0;
+    pkt_dev->rx_packets = 0;
+    for_each_online_cpu(cpu) {
+        per_cpu(pg_rx_stats, cpu).rx_bytes = 0;
+        per_cpu(pg_rx_stats, cpu).rx_packets = 0;
+    }
 }
 
 /* Set up structure for sending pkts, clear counters */
 
 static void pktgen_run(struct pktgen_thread *t)
 {
     struct pktgen_dev *pkt_dev;
@@ -4294,15 +4458,19 @@
             ktime_compare(pkt_dev->mburst_tx, next_stop) < 0) {
             spin(pkt_dev, next_stop);
             pkt_dev->mburst_tx = ktime_add_ms(
                 pkt_dev->next_tx, pkt_dev->pause_time + pkt_dev->poll_time);
         }
     }
 
-    if (pkt_dev->xmit_mode == M_NETIF_RECEIVE) {
+    if (pkt_dev->xmit_mode == M_RX_ONLY) {
+        local_bh_disable();
+        cpu_relax();
+        goto out;
+    } else if (pkt_dev->xmit_mode == M_NETIF_RECEIVE) {
         skb = pkt_dev->skb;
         skb->protocol = eth_type_trans(skb, skb->dev);
         refcount_add(burst, &skb->users);
         local_bh_disable();
         do {
             ret = netif_receive_skb(skb);
             if (ret == NET_RX_DROP)
@@ -4516,14 +4684,15 @@
 /*
  * Adds a dev at front of if_list.
  */
 
 static int add_dev_to_thread(struct pktgen_thread *t,
                  struct pktgen_dev *pkt_dev)
 {
+    struct pktgen_dev **p;
     int rv = 0;
 
     /* This function cannot be called concurrently, as its called
      * under pktgen_thread_lock mutex, but it can run from
      * userspace on another CPU than the kthread.  The if_lock()
      * is used here to sync with concurrent instances of
      * _rem_dev_from_if_list() invoked via kthread, which is also
@@ -4534,14 +4703,16 @@
         pr_err("ERROR: already assigned to a thread\n");
         rv = -EBUSY;
         goto out;
     }
 
     pkt_dev->running = 0;
     pkt_dev->pg_thread = t;
+    p = per_cpu_ptr(&pg_devs, t->cpu);
+    *p = pkt_dev;
     list_add_rcu(&pkt_dev->list, &t->if_list);
 
 out:
     if_unlock(t);
     return rv;
 }
 
@@ -4590,17 +4761,22 @@
     pkt_dev->svlan_cfi = 0;
     pkt_dev->svlan_id = 0xffff;
     pkt_dev->burst = 1;
     pkt_dev->node = NUMA_NO_NODE;
     pkt_dev->pause_time = 0;
     pkt_dev->poll_time = 0;
 
-    err = pktgen_setup_dev(t->net, pkt_dev, ifname);
+    err = pktgen_setup_dev(t->net, &pkt_dev->odev, ifname);
+    if (err)
+        goto out1;
+
+    err = pktgen_setup_dev(t->net, &pkt_dev->idev, ifname);
     if (err)
         goto out1;
+
     if (pkt_dev->odev->priv_flags & IFF_TX_SKB_SHARING)
         pkt_dev->clone_skb = pg_clone_skb_d;
 
     pkt_dev->entry = proc_create_data(ifname, 0600, t->net->proc_dir,
                       &pktgen_if_fops, pkt_dev);
     if (!pkt_dev->entry) {
         pr_err("cannot create %s/%s procfs entry\n",
@@ -4738,14 +4914,45 @@
     vfree(pkt_dev->flows);
     if (pkt_dev->page)
         put_page(pkt_dev->page);
     kfree_rcu(pkt_dev, rcu);
     return 0;
 }
 
+static unsigned int pg_pre_routing_hook_func(void *priv, struct sk_buff *skb,
+                                   const struct nf_hook_state *state)
+{
+    struct pktgen_dev *pkt_dev;
+    struct pktgen_hdr *pgh;
+    struct pktgen_rx *data_cpu;
+    int cpu;
+
+    pgh = (struct pktgen_hdr *)(((char *)(skb_transport_header(skb))) + 8);
+    if(unlikely(pgh->pgh_magic != htonl(PKTGEN_MAGIC))) {
+        return NF_ACCEPT;
+    }
+    cpu = get_cpu();
+    data_cpu = &get_cpu_var(pg_rx_stats);
+    data_cpu->rx_packets++;
+    data_cpu->rx_bytes += skb->len + ETH_HLEN;
+    pkt_dev = get_cpu_var(pg_devs);
+    if (pkt_dev) {
+        pkt_dev->rx_packets ++;
+        pkt_dev->rx_bytes += skb->len + ETH_HLEN;
+    }
+    return NF_DROP;
+}
+
+static struct nf_hook_ops pg_pre_routing = {
+    .hook = pg_pre_routing_hook_func,
+    .hooknum = NF_INET_PRE_ROUTING,
+    .pf = PF_INET,
+    .priority = NF_IP_PRI_FIRST,
+};
+
 static int __net_init pg_net_init(struct net *net)
 {
     struct pktgen_net *pn = net_generic(net, pg_net_id);
     struct proc_dir_entry *pe;
     int cpu, ret = 0;
 
     pn->net = net;
@@ -4759,14 +4966,20 @@
     pe = proc_create(PGCTRL, 0600, pn->proc_dir, &pktgen_fops);
     if (pe == NULL) {
         pr_err("cannot create %s procfs entry\n", PGCTRL);
         ret = -EINVAL;
         goto remove;
     }
 
+    ret = nf_register_net_hook(net, &pg_pre_routing);
+    if (ret) {
+        pr_err("Initialization failed for nf_hook\n");
+        goto remove;
+    }
+
     for_each_online_cpu(cpu) {
         int err;
 
         err = pktgen_create_thread(cpu, pn);
         if (err)
             pr_warn("Cannot create thread for cpu %d (%d)\n",
                    cpu, err);
@@ -4805,14 +5018,15 @@
         t = list_entry(q, struct pktgen_thread, th_list);
         list_del(&t->th_list);
         kthread_stop(t->tsk);
         put_task_struct(t->tsk);
         kfree(t);
     }
 
+    nf_unregister_net_hook(net, &pg_pre_routing);
     remove_proc_entry(PGCTRL, pn->proc_dir);
     remove_proc_entry(PG_PROC_DIR, pn->net->proc_net);
 }
 
 static struct pernet_operations pg_net_ops = {
     .init = pg_net_init,
     .exit = pg_net_exit,
```

### Comparing `pktperf-0.5.5/pktperf/pktgen.py` & `pktperf-0.5.6/pktperf/pktgen.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,34 @@
         with open(filename, mode, encoding="utf-8") as fp_dev:
             fp_dev.write("%s\n" % flag)
     except IOError as exc:
         print("Error: Cannot open %s" % (filename))
         raise IOError("Error writing flag %s" % flag) from exc
 
 
+def cpu_count():
+    try:
+        res = open('/proc/cpuinfo').read().count('processor\t:')
+        if res > 0:
+            return res
+    except IOError:
+        pass
+    # cpuset
+    # cpuset may restrict the number of *available* processors
+    try:
+        m = re.search(r'(?m)^Cpus_allowed:\s*(.*)$',
+                      open('/proc/self/status').read())
+        if m:
+            res = bin(int(m.group(1).replace(',', ''), 16)).count('1')
+            if res > 0:
+                return res
+    except IOError:
+        raise IOError("Error getting cpu count")
+
+
 def modinfo_check() -> str:
     """check module version"""
     n = platform.uname()
     depfile = "/lib/modules/%s/modules.dep" % n.release
     try:
         with open(depfile, "r", encoding="utf-8") as fp_dep:
             fp_dep.readlines()
@@ -103,34 +123,34 @@
         self.dst_port_min, self.dst_port_max = self.__init_port_range(args.portrange)
         self.src_port_min, self.src_port_max = 9, 1009
         self.frags = None
         self.csum = args.txcsum
         self.debug = args.debug
         self.verbose = args.verbose
         self.append = args.append
+        self.clone = None
         if args.clone is not None:
             self.clone = int(args.clone)
         self.num = int(args.num)
         if args.burst is not None:
             self.burst = int(args.burst)
         if args.threads is not None:
             self.threads = int(args.threads)
-        self.stats = []
+        self.stats = {}
         if args.firstthread is not None:
             self.first_thread = int(args.firstthread)
         self.thread_list = list(
             range(self.first_thread, self.first_thread + self.threads)
         )
         if args.delay is not None:
             self.tx_delay = int(args.delay)
         if args.flows is not None:
             self.flows = int(args.flows)
         if args.flowpkts is not None:
             self.flow_len = int(args.flowpkts)
-        self.__init_irq(args.queuemap)
         if args.tos is not None:
             self.tos = int(args.tos)
         self.bps_rate = args.bps
         self.pps_rate = args.pps
         if args.frags is not None:
             self.frags = int(args.frags)
         self.vlan = args.vlan
@@ -141,19 +161,23 @@
         self.tun_src_min, self.tun_src_max = self.__init_ip_input(args.tunsrc)
         self.inner_dmac = args.innerdmac
         self.inner_smac = args.innersmac
         self.inner_dmac_count = 0
         self.inner_smac_count = 0
         self.microburst = args.microburst
         self.imixweight = args.imix
+        self.tcp = None
+        self.mode = None
+        self.rxq = []
         self.__read_config_file(args.file)
         if self.pgdev is None:
             raise Exception("No interface specified")
         if self.dst_ip_min == "":
             raise Exception("No dst ip specified")
+        self.__init_irq(args.queuemap)
 
     def __read_config_file(self, file):
         cfg = configparser.ConfigParser()
         if file is not None:
             with open(file, "r", encoding="utf-8") as f:
                 config_string = "[dummy]\n" + f.read()
                 cfg.read_string(config_string)
@@ -161,23 +185,23 @@
             return
         if cfg.has_option("dummy", "interface"):
             self.pgdev = cfg.get("dummy", "interface")
         if cfg.has_option("dummy", "pkt_size"):
             self.pkt_size = cfg.getint("dummy", "pkt_size")
         if cfg.has_option("dummy", "pkt_num"):
             self.num = cfg.getint("dummy", "pkt_num")
-        if cfg.has_option("dummy", "threads"):
+        if cfg.has_option("dummy", "cpulist"):
             self.thread_list = sum(
                 (
                     (
                         list(range(*[int(b) + c for c, b in enumerate(a.split("-"))]))
                         if "-" in a
                         else [int(a)]
                     )
-                    for a in cfg.get("dummy", "threads").split(",")
+                    for a in cfg.get("dummy", "cpulist").split(",")
                 ),
                 [],
             )
             self.first_thread = self.thread_list[0]
             self.threads = len(self.thread_list)
         if cfg.has_option("dummy", "bps_limit"):
             self.bps_rate = cfg.get("dummy", "bps_limit")
@@ -232,14 +256,32 @@
         if cfg.has_option("dummy", "inner_smac_num"):
             self.inner_smac_count = cfg.getint("dummy", "inner_smac_num")
         if cfg.has_option("dummy", "micro_burst"):
             self.microburst = cfg.get("dummy", "micro_burst")
             self.burst = 0
         if cfg.has_option("dummy", "imix_weight"):
             self.imixweight = cfg.get("dummy", "imix_weight")
+        if cfg.has_option("dummy", "tcp_syn"):
+            self.tcp = cfg.get("dummy", "tcp_syn")
+        if cfg.has_option("dummy", "mode"):
+            self.mode = cfg.get("dummy", "mode")
+            if self.mode == "netif_receive" and self.clone is not None:
+                self.clone = None
+        if cfg.has_option("dummy", "rxqlist"):
+            self.rxq = sum(
+                (
+                    (
+                        list(range(*[int(b) + c for c, b in enumerate(a.split("-"))]))
+                        if "-" in a
+                        else [int(a)]
+                    )
+                    for a in cfg.get("dummy", "rxqlist").split(",")
+                ),
+                [],
+            )
 
     def __init_ip_input(self, ipstr):
         """Init pktgen module ip dst"""
         if ipstr is None:
             return "", ""
         net = None
         try:
@@ -277,21 +319,24 @@
                 port_max = int(ports[0])
             port_min = int(ports[0])
         return port_min, port_max
 
     def __init_irq(self, queuemap) -> None:
         """init irq affinity if queue mapping enabled"""
         self.queue = queuemap
+        self.irq_list = self.__get_irqs()
         if queuemap is True:
             numa = self.__get_dev_numa()
-            self.irq_list = self.__get_irqs()
             if len(self.irq_list) == 0:
                 print("irq affinity not supported")
                 sys.exit()
             self.cpu_list = self.__node_cpu_list(numa)
+            if len(self.rxq) == 0:
+                for _ in self.irq_list:
+                    self.rxq.append(cpu_count())
 
     @staticmethod
     def pg_ctrl(cmd) -> None:
         """pg_ctrl control "pgctrl" (/proc/net/pktgen/pgctrl)"""
         pgctrl = "/proc/net/pktgen/pgctrl"
         if cmd not in ["start", "stop", "reset"]:
             print("pgctrl do not support cmd %s" % cmd)
@@ -315,17 +360,17 @@
         """pg_set control setup of individual devices"""
         if dev.find(self.pgdev) < 0:
             print("device not match")
             sys.exit(1)
         pgdev = "/proc/net/pktgen/%s" % dev
         open_write_error(pgdev, flag)
 
-    def __pg_get_devpath(self, index) -> str:
+    def __pg_get_devpath(self, index, role) -> str:
         """get dev path for thread index"""
-        if self.queue is True:
+        if self.queue is True and role == 'tx':
             dev = "%s@%d" % (self.pgdev, self.cpu_list[index])
         else:
             dev = "%s@%d" % (self.pgdev, index)
         devpath = "/proc/net/pktgen/%s" % dev
         return devpath
 
     @staticmethod
@@ -338,20 +383,22 @@
         open_write_error(pgthread, cmd, "w")
 
     @staticmethod
     def os_check() -> bool:
         """check if os is linux"""
         return os.name == "posix"
 
-    def __config_irq_affinity(self, irq, thread):
+    def __config_irq_affinity(self, irq, cpu):
         """config irq affinity"""
         irq_path = "/proc/irq/%d/smp_affinity_list" % irq
-        open_write_error(irq_path, thread)
+        if cpu == cpu_count():
+            cpu = "0-%d" % (cpu_count()-1)
+        open_write_error(irq_path, cpu)
         if self.debug is True:
-            print("irq %d is set affinity to %d" % (irq, thread))
+            print("irq %d is set affinity to %d" % (irq, cpu))
 
     def __config_tos(self, dev) -> None:
         """config tos"""
         if self.tos is not None and self.tos != 0:
             if self.ipv6 is True:
                 self.pg_set(dev, "traffic_class %0x" % self.tos)
             else:
@@ -448,25 +495,37 @@
             self.pg_set(dev, "ratep %s" % (self.pps_rate))
 
     def config_queue(self) -> None:
         """configure queues for pktgen"""
         # General cleanup everything since last run
         self.reset()
 
+        # In a dedicated case, rxq num should equal to tx thread
+        # if irq for a rxq binded to tx cpu, perfermance drop to 1/40
+        for i, irq in enumerate(self.irq_list):
+            q = self.rxq[i%len(self.rxq)]
+            self.__config_irq_affinity(irq, q)
+            if q == cpu_count():
+                continue
+            dev = "%s@%d" % (self.pgdev, q)
+            if self.append is False:
+                self.pg_thread(q, "rem_device_all")
+            self.pg_thread(q, "add_device %s" % dev)
+            self.pg_set(dev, "xmit_mode rx_only")
+            self.pg_set(dev, "count 0")
+
         # Threads are specified with parameter -t value in $THREADS
         for i in self.thread_list:
             if self.queue is True:
                 dev = "%s@%d" % (self.pgdev, self.cpu_list[i])
-                irq = self.irq_list[i]
-                self.__config_irq_affinity(irq, self.cpu_list[i])
             else:
                 # The device name is extended with @name, using thread id to
-                # make then unique, but any name will do.
+                # make them unique, but any name will do.
                 dev = "%s@%d" % (self.pgdev, i)
-
+            # print(dev)
             # Add remove all other devices and add_device $dev to thread
             if self.append is False:
                 self.pg_thread(i, "rem_device_all")
             self.pg_thread(i, "add_device %s" % dev)
 
             # select queue and bind the queue and $dev in 1:1 relationship
             if self.queue is True:
@@ -478,15 +537,16 @@
 
             # Notice config queue to map to cpu (mirrors smp_processor_id())
             # It is beneficial to map IRQ /proc/irq/*/smp_affinity 1:1 to CPU
             self.pg_set(dev, "flag QUEUE_MAP_CPU")
 
             # Base config of dev
             self.pg_set(dev, "count %d" % math.ceil(self.num / self.threads))
-            self.pg_set(dev, "clone_skb %d" % self.clone)
+            if self.clone is not None:
+                self.pg_set(dev, "clone_skb %d" % self.clone)
             self.pg_set(dev, "pkt_size %d" % self.pkt_size)
             if self.frags is not None and self.frags != 1:
                 self.pg_set(dev, "frags %d" % self.frags)
             self.pg_set(dev, "delay %d" % self.tx_delay)
 
             self.__config_tos(dev)
 
@@ -500,14 +560,21 @@
             self.__config_udp_portrange(dev)
             self.__config_vlan(dev)
 
             self.__config_ratelimit(dev)
 
             self.__config_imix(dev)
             self.__config_burst_mode(dev)
+            node = self.__get_dev_numa()
+            self.pg_set(dev, "node %d" % node)
+            if self.tcp is not None:
+                self.pg_set(dev, "tcp_syn %s" % self.tcp)
+                self.pg_set(dev, "flag UDPCSUM")
+            if self.mode is not None:
+                self.pg_set(dev, "xmit_mode %s" % self.mode)
 
     def reset(self) -> None:
         """reset pktgen"""
         if self.append is False:
             self.pg_ctrl("reset")
 
     def start(self) -> None:
@@ -518,100 +585,131 @@
     def stop(self) -> None:
         """stop pktgen"""
         self.pg_ctrl("stop")
 
     @staticmethod
     def result_last(core_id, fp_dev, print_cb):
         """print last result"""
-        tpkts = 0
-        tpps = 0
-        tbps = 0
-        tbps = 0
+        pkts = 0
+        pps = 0
+        bps = 0
+        bps = 0
         stats_content = fp_dev.read()
         result_field = re.compile(
-            r"Result: (\w+): \d+\([\w\+]+\) \w+, (\d+) \(\d+byte,\d+frags\)"
+            r"Result: (\w+): \d+\([\w\+]+\) \w+, (\d+) \((\d+)byte,\d+frags\)"
         )
         throughput_field = re.compile(
             r"  (\d+)pps \d+Mb\/sec \((\d+)bps\) errors: (\d+)"
         )
         unresult_field = re.compile(r"Result: (\w+)")
         res = result_field.search(stats_content)
         pkt = throughput_field.search(stats_content)
         if res is not None and pkt is not None:
-            tpkts = int(res.group(2))
-            tpps = int(pkt.group(1))
-            tbps = int(pkt.group(2))
-            tbps = int(pkt.group(3))
+            pkts = int(res.group(2))
+            pps = int(pkt.group(1))
+            bps = int(pkt.group(2))
+            byt = pkts * int(res.group(3))
             print_cb(
-                "Core%3d send %18d pkts: %18d pps %18d bps %6d errors"
-                % (
-                    core_id,
-                    int(res.group(2)),
-                    int(pkt.group(1)),
-                    int(pkt.group(2)),
-                    int(pkt.group(3)),
-                )
+                "Core%3d TX %18d pkts: %18d pps %18d bps %6d bytes"
+                % (core_id, pkts, pps, bps, byt)
             )
         else:
             other = unresult_field.search(stats_content)
             if other is not None:
                 print_cb("Core%3d %s" % (core_id, other.group(1)))
-        return tpkts, tpps, tbps, tbps
+        return pkts, pps, bps, bps
 
     def result_transient(self, need_init, core_id, fp_dev, print_cb):
         """print result during"""
         stats_content = fp_dev.read()
         sofar_field = re.compile(r"pkts-sofar: (\d+)  errors: (\d+)")
         time_field = re.compile(r"started: (\d+)us  stopped: (\d+)us")
         sofar = sofar_field.search(stats_content)
         tim = time_field.search(stats_content)
+        if sofar is not None:
+            direction = 'TX'
+        else:
+            direction = 'RX'
+            sofar_field = re.compile(r"pkts-rx: (\d+)  bytes: (\d+)")
+            sofar = sofar_field.search(stats_content)
         if need_init is True:
-            pkt_sar = PktSar(int(tim.group(1)), self.pkt_size)
-            self.stats.append(pkt_sar)
+            pkt_sar = PktSar(int(tim.group(1)))
+            self.stats[core_id] = pkt_sar
         else:
-            pkt_sar = self.stats[core_id - self.first_thread]
-        if sofar is not None:
-            pkt_sar.update(int(sofar.group(1)), int(tim.group(2)))
-            pps, bps = pkt_sar.get_stats()
-            print_cb(
-                "Core%3d send %18d pkts: %18f pps %18f bps %6d errors"
-                % (core_id, int(sofar.group(1)), pps, bps, int(sofar.group(2)))
-            )
-            return int(sofar.group(1)), pps, bps, int(sofar.group(2))
-        return 0, 0, 0, 0
+            pkt_sar = self.stats[core_id]
+        pps = 0
+        bps = 0
+        byt = 0
+        pkt = 0
+
+        pkt = int(sofar.group(1))
+        if direction == 'TX':
+            byt = pkt * self.pkt_size
+        else:
+            byt = int(sofar.group(2))
+        pkt_sar.update(pkt, int(tim.group(2)), byt)
+        pps, bps = pkt_sar.get_stats()
+        print_cb(
+            "Core%3d %s %18d pkts: %18f pps %18f bps %6d bytes"
+            % (core_id, direction, pkt, pps, bps, byt)
+        )
+
+        return pkt, pps, bps, byt
 
     def result(self, last, print_cb) -> int:
         """Print results"""
         if last is True:
             print("%d cores enabled" % self.threads)
         need_init = False
         total_pkts = 0
         total_pps = 0
         total_bps = 0
-        total_err = 0
+        total_bytes = 0
         if len(self.stats) == 0:
             need_init = True
         for i in self.thread_list:
-            with open(self.__pg_get_devpath(i), "r") as fp_dev:
+            with open(self.__pg_get_devpath(i, 'tx'), "r") as fp_dev:
                 if last is False:
-                    sg_pkts, sg_pps, sg_bps, sg_err = self.result_transient(
+                    sg_pkts, sg_pps, sg_bps, sg_bytes = self.result_transient(
                         need_init, i, fp_dev, print_cb
                     )
                 else:
-                    sg_pkts, sg_pps, sg_bps, sg_err = self.result_last(
+                    sg_pkts, sg_pps, sg_bps, sg_bytes  = self.result_last(
                         i, fp_dev, print_cb
                     )
                 total_pkts += sg_pkts
                 total_pps += sg_pps
                 total_bps += sg_bps
-                total_err += sg_err
+                total_bytes += sg_bytes
         print_cb(
-            "Total   send %18d pkts: %18d pps %18d bps %6d errors"
-            % (total_pkts, total_pps, total_bps, total_err)
+            "Total   TX %18d pkts: %18d pps %18d bps %6d bytes"
+            % (total_pkts, total_pps, total_bps, total_bytes)
         )
+
+        total_pkts = 0
+        total_pps = 0
+        total_bps = 0
+        total_bytes = 0
+        rx_cnt = 0
+        for i, _ in enumerate(self.irq_list):
+            q = self.rxq[i % len(self.rxq)]
+            if q == cpu_count():
+                continue
+            rx_cnt += 1
+            with open(self.__pg_get_devpath(q, 'rx'), "r") as fp_dev:
+                sg_pkts, sg_pps, sg_bps, sg_bytes = self.result_transient(
+                    need_init, q, fp_dev, print_cb
+                )
+                total_pkts += sg_pkts
+                total_pps += sg_pps
+                total_bps += sg_bps
+                total_bytes += sg_bytes
+        if rx_cnt > 0:
+            print_cb("Total   RX %18d pkts: %18d pps %18d bps %6d bytes"
+                    % (total_pkts, total_pps, total_bps, total_bytes))
         if last is False and self.num > 0 and total_pkts >= self.num:
             return 1
         return 0
 
     def __get_dev_numa(self) -> int:
         """__get_dev_numa returns the numa node of the device"""
         numa_path = "/sys/class/net/%s/device/numa_node" % self.pgdev
@@ -639,29 +737,63 @@
         ret = []
         for i in ranges:
             cpu_start, cpu_end = i.split("-")
             for j in range(int(cpu_start), int(cpu_end) + 1):
                 ret.append(j)
         return ret
 
+    def __get_driver(self):
+        driverpath = "/sys/class/net/%s/device/driver/module/drivers" % self.pgdev
+        driver_types = os.listdir(driverpath)
+        driver = ''
+        pci = ''
+        for i in driver_types:
+            if i.startswith('pci:') or i.startswith('virtio:'):
+                driver = i.split(':')[1]
+                break
+        if driver != '':
+            pcipath = "/sys/bus/pci/drivers/%s/" % driver
+            pcis = os.listdir(pcipath)
+            for i in pcis:
+                if ':' in i:
+                    if driver == 'virtio_net':
+                        for j in os.listdir("/sys/bus/pci/drivers/virtio-pci/%s/" %  i):
+                            if j.startswith("virtio"):
+                                pcidev = "/sys/bus/pci/drivers/virtio-pci/%s/%s/net" % (i, j)
+                                break
+                    else:
+                        pcidev = "/sys/bus/pci/drivers/%s/%s/net" % (driver, i)
+                    namepath = os.listdir(pcidev)
+                    if namepath[0] == self.pgdev:
+                        pci = i
+                        break
+        return driver, pci
+
     def __get_irqs(self):
         """read out irqs"""
+        # driver, pci = self.__get_driver()
+        # print(driver)
+        # print(pci)
+        # pcipath = "/sys/bus/pci/devices/%s/" % pci
+        # for i in os.listdir(pcipath):
+        """ Once IRQs are allocated by the driver, they are named mlx5_comp<x>@pci:<pci_addr>.
+          The IRQs corresponding to the channels in use are renamed to <interface>-<x>,
+          while the rest maintain their default name."""
         proc_intr = "/proc/interrupts"
         msi_irqs = "/sys/class/net/%s/device/msi_irqs" % self.pgdev
         try:
             with open(proc_intr, "r") as fp_proc:
                 intrs = fp_proc.read()
         except IOError:
             return []
         irqs = []
         devq_irq = re.compile(
             r"(\d+):[ \d]+ [\w-]+ \d+-edge[ ]+%s-.*TxRx-\d+" % (self.pgdev)
         )
         match = devq_irq.finditer(intrs)
-        print(match)
         if len(devq_irq.findall(intrs)) > 0:
             for i in match:
                 irqs.append(int(i.group(1)))
             return irqs
         dev_irq = re.compile(r"(\d+):[ \d]+ [\w-]+ \d+-edge[ ]+%s-\d+" % (self.pgdev))
         match = dev_irq.finditer(intrs)
         if len(dev_irq.findall(intrs)) > 0:
```

### Comparing `pktperf-0.5.5/pktperf/pktperf.py` & `pktperf-0.5.6/pktperf/pktperf.py`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.5/pktperf.egg-info/PKG-INFO` & `pktperf-0.5.6/pktperf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pktperf
-Version: 0.5.5
+Version: 0.5.6
 Summary: pktgen scripts tool
 Author-email: junka <wan.junjie@foxmail.com>
 Project-URL: Homepage, https://github.com/junka/pktperf
 Project-URL: Bug Tracker, https://github.com/junka/pktperf/issues
 Platform: manylinux2014_x86_64
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pktperf-0.5.5/pyproject.toml` & `pktperf-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pktperf"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
   { name="junka", email="wan.junjie@foxmail.com" },
 ]
 description = "pktgen scripts tool"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

