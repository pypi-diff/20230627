# Comparing `tmp/byquant-1.6.15.tar.gz` & `tmp/byquant-1.6.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byquant-1.6.15.tar", last modified: Thu Jun 15 06:01:34 2023, max compression
+gzip compressed data, was "byquant-1.6.27.tar", last modified: Tue Jun 27 01:32:07 2023, max compression
```

## Comparing `byquant-1.6.15.tar` & `byquant-1.6.27.tar`

### file list

```diff
@@ -1,130 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 06:01:34.588982 byquant-1.6.15/
--rw-rw-rw-   0        0        0     1266 2023-06-15 06:01:34.588982 byquant-1.6.15/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.6.15/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 06:01:34.141578 byquant-1.6.15/byquant/
--rw-rw-rw-   0        0        0    21857 2023-05-17 05:50:41.000000 byquant-1.6.15/byquant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:01:34.588982 byquant-1.6.15/byquant/exchange/
--rw-rw-rw-   0        0        0        0 2023-05-16 08:03:11.000000 byquant-1.6.15/byquant/exchange/__init__.py
--rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.6.15/byquant/exchange/ace.py
--rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/alpaca.py
--rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/ascendex.py
--rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bequant.py
--rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bigone.py
--rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/binance.py
--rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/binancecoinm.py
--rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/binanceus.py
--rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/binanceusdm.py
--rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bit2c.py
--rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitbank.py
--rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitbay.py
--rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitbns.py
--rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitcoincom.py
--rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitfinex.py
--rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitfinex2.py
--rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitflyer.py
--rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitforex.py
--rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitget.py
--rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bithumb.py
--rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitmart.py
--rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitmex.py
--rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitopro.py
--rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitpanda.py
--rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitrue.py
--rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitso.py
--rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitstamp.py
--rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitstamp1.py
--rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bittrex.py
--rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bitvavo.py
--rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bkex.py
--rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bl3p.py
--rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/blockchaincom.py
--rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btcalpha.py
--rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btcbox.py
--rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btcex.py
--rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btcmarkets.py
--rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btctradeua.py
--rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/btcturk.py
--rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/buda.py
--rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/bybit.py
--rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/cex.py
--rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinbase.py
--rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinbaseprime.py
--rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinbasepro.py
--rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coincheck.py
--rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinex.py
--rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinfalcon.py
--rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinmate.py
--rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinone.py
--rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinsph.py
--rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/coinspot.py
--rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/cryptocom.py
--rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/currencycom.py
--rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/delta.py
--rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/deribit.py
--rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/digifinex.py
--rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/exmo.py
--rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/flowbtc.py
--rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/fmfwio.py
--rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/gate.py
--rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/gateio.py
--rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/gemini.py
--rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/hitbtc.py
--rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/hitbtc3.py
--rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/hollaex.py
--rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/huobi.py
--rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/huobijp.py
--rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/huobipro.py
--rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/idex.py
--rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/independentreserve.py
--rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/indodax.py
--rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/itbit.py
--rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/kraken.py
--rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/krakenfutures.py
--rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/kucoin.py
--rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/kucoinfutures.py
--rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/kuna.py
--rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/latoken.py
--rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/lbank.py
--rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/lbank2.py
--rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/luno.py
--rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/lykke.py
--rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/mercado.py
--rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/mexc.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/mexc3.py
--rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/ndax.py
--rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/novadax.py
--rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/oceanex.py
--rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/okcoin.py
--rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/okex.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/okex5.py
--rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.6.15/byquant/exchange/okx.py
--rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/paymium.py
--rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/phemex.py
--rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/poloniex.py
--rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/poloniexfutures.py
--rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/probit.py
--rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/ripio.py
--rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/stex.py
--rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/tidex.py
--rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/timex.py
--rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/tokocrypto.py
--rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/upbit.py
--rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/wavesexchange.py
--rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/wazirx.py
--rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/whitebit.py
--rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/woo.py
--rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/xt.py
--rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/yobit.py
--rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/zaif.py
--rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/zb.py
--rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.6.15/byquant/exchange/zonda.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:01:34.162793 byquant-1.6.15/byquant.egg-info/
--rw-rw-rw-   0        0        0     1266 2023-06-15 06:01:34.000000 byquant-1.6.15/byquant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3413 2023-06-15 06:01:34.000000 byquant-1.6.15/byquant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 06:01:34.000000 byquant-1.6.15/byquant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-15 06:01:34.000000 byquant-1.6.15/byquant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 06:01:34.000000 byquant-1.6.15/byquant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.6.15/byquant.egg-info/zip-safe
--rw-rw-rw-   0        0        0       97 2023-06-15 05:53:38.000000 byquant-1.6.15/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 06:01:34.588982 byquant-1.6.15/setup.cfg
--rw-rw-rw-   0        0        0     2682 2023-06-15 05:51:16.000000 byquant-1.6.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.539946 byquant-1.6.27/
+-rw-rw-rw-   0        0        0     1328 2023-06-27 01:32:07.539946 byquant-1.6.27/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.6.27/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.038142 byquant-1.6.27/byquant/
+-rw-rw-rw-   0        0        0    21860 2023-06-25 06:21:22.000000 byquant-1.6.27/byquant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.069376 byquant-1.6.27/byquant/crypto/
+-rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.6.27/byquant/crypto/__init__.py
+-rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.6.27/byquant/crypto/broker.py
+-rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.6.27/byquant/crypto/feed.py
+-rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.6.27/byquant/crypto/store.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.538914 byquant-1.6.27/byquant/exchange/
+-rw-rw-rw-   0        0        0        0 2023-05-16 08:03:11.000000 byquant-1.6.27/byquant/exchange/__init__.py
+-rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.6.27/byquant/exchange/ace.py
+-rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/alpaca.py
+-rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/ascendex.py
+-rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bequant.py
+-rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bigone.py
+-rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/binance.py
+-rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/binancecoinm.py
+-rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/binanceus.py
+-rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/binanceusdm.py
+-rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bit2c.py
+-rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitbank.py
+-rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitbay.py
+-rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitbns.py
+-rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitcoincom.py
+-rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitfinex.py
+-rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitfinex2.py
+-rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitflyer.py
+-rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitforex.py
+-rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitget.py
+-rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bithumb.py
+-rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitmart.py
+-rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitmex.py
+-rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitopro.py
+-rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitpanda.py
+-rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitrue.py
+-rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitso.py
+-rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitstamp.py
+-rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitstamp1.py
+-rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bittrex.py
+-rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bitvavo.py
+-rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bkex.py
+-rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bl3p.py
+-rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/blockchaincom.py
+-rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btcalpha.py
+-rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btcbox.py
+-rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btcex.py
+-rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btcmarkets.py
+-rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btctradeua.py
+-rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/btcturk.py
+-rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/buda.py
+-rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/bybit.py
+-rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/cex.py
+-rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinbase.py
+-rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinbaseprime.py
+-rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinbasepro.py
+-rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coincheck.py
+-rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinex.py
+-rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinfalcon.py
+-rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinmate.py
+-rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinone.py
+-rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinsph.py
+-rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/coinspot.py
+-rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/cryptocom.py
+-rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/currencycom.py
+-rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/delta.py
+-rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/deribit.py
+-rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/digifinex.py
+-rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/exmo.py
+-rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/flowbtc.py
+-rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/fmfwio.py
+-rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/gate.py
+-rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/gateio.py
+-rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/gemini.py
+-rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/hitbtc.py
+-rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/hitbtc3.py
+-rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/hollaex.py
+-rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/huobi.py
+-rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/huobijp.py
+-rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/huobipro.py
+-rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/idex.py
+-rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/independentreserve.py
+-rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/indodax.py
+-rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/itbit.py
+-rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/kraken.py
+-rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/krakenfutures.py
+-rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/kucoin.py
+-rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/kucoinfutures.py
+-rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/kuna.py
+-rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/latoken.py
+-rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/lbank.py
+-rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/lbank2.py
+-rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/luno.py
+-rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/lykke.py
+-rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/mercado.py
+-rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/mexc.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/mexc3.py
+-rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/ndax.py
+-rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/novadax.py
+-rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/oceanex.py
+-rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/okcoin.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/okex.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/okex5.py
+-rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.6.27/byquant/exchange/okx.py
+-rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/paymium.py
+-rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/phemex.py
+-rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/poloniex.py
+-rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/poloniexfutures.py
+-rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/probit.py
+-rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/ripio.py
+-rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/stex.py
+-rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/tidex.py
+-rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/timex.py
+-rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/tokocrypto.py
+-rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/upbit.py
+-rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/wavesexchange.py
+-rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/wazirx.py
+-rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/whitebit.py
+-rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/woo.py
+-rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/xt.py
+-rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/yobit.py
+-rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/zaif.py
+-rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/zb.py
+-rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.6.27/byquant/exchange/zonda.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.539946 byquant-1.6.27/byquant/tool/
+-rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.6.27/byquant/tool/__init__.py
+-rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.6.27/byquant/tool/tawPlus.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:32:07.069376 byquant-1.6.27/byquant.egg-info/
+-rw-rw-rw-   0        0        0     1328 2023-06-27 01:32:06.000000 byquant-1.6.27/byquant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3561 2023-06-27 01:32:07.000000 byquant-1.6.27/byquant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 01:32:06.000000 byquant-1.6.27/byquant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-27 01:32:06.000000 byquant-1.6.27/byquant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-27 01:32:06.000000 byquant-1.6.27/byquant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.6.27/byquant.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      125 2023-06-27 01:29:04.000000 byquant-1.6.27/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 01:32:07.539946 byquant-1.6.27/setup.cfg
+-rw-rw-rw-   0        0        0     2760 2023-06-27 01:28:02.000000 byquant-1.6.27/setup.py
```

### Comparing `byquant-1.6.15/PKG-INFO` & `byquant-1.6.27/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.6.15
-Summary: A Python trading library with support for 130+ exchanges
+Version: 1.6.27
+Summary: ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: MIT
 Project-URL: Homepage, https://byquant.com
-Keywords: algorithmic,algotrading
+Keywords: quant,strategy,algorithmic,algotrading
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `byquant-1.6.15/byquant/__init__.py` & `byquant-1.6.27/byquant/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 from byquant.exchange.okex5 import okex5                                          # noqa: F401
 from byquant.exchange.okx import okx                                              # noqa: F401  Uakeey
 from byquant.exchange.paymium import paymium                                      # noqa: F401
 from byquant.exchange.phemex import phemex                                        # noqa: F401
 from byquant.exchange.poloniex import poloniex                                    # noqa: F401
 from byquant.exchange.poloniexfutures import poloniexfutures                      # noqa: F401
 from byquant.exchange.probit import probit                                        # noqa: F401
-from byquant.exchange.stex import stex                                            # noqa: F401
+#from byquant.exchange.stex import stex                                            # noqa: F401
 from byquant.exchange.tidex import tidex                                          # noqa: F401
 from byquant.exchange.timex import timex                                          # noqa: F401
 from byquant.exchange.tokocrypto import tokocrypto                                # noqa: F401
 from byquant.exchange.upbit import upbit                                          # noqa: F401
 from byquant.exchange.wavesexchange import wavesexchange                          # noqa: F401
 from byquant.exchange.wazirx import wazirx                                        # noqa: F401
 from byquant.exchange.whitebit import whitebit                                    # noqa: F401
@@ -263,15 +263,15 @@
     'okex5',
     'okx',
     'paymium',
     'phemex',
     'poloniex',
     'poloniexfutures',
     'probit',
-    'stex',
+#    'stex',
     'tidex',
     'timex',
     'tokocrypto',
     'upbit',
     'wavesexchange',
     'wazirx',
     'whitebit',
@@ -379,15 +379,15 @@
     elif exName == 'okx': result = okx()
     elif exName == 'paymium': result = paymium()
     elif exName == 'phemex': result = phemex()
     elif exName == 'poloniex': result = poloniex()
     elif exName == 'poloniexfutures': result = poloniexfutures()
     elif exName == 'probit': result = probit()
     elif exName == 'ripio': result = ripio()
-    elif exName == 'stex': result = stex()
+#    elif exName == 'stex': result = stex()
     elif exName == 'tidex': result = tidex()
     elif exName == 'timex': result = timex()
     elif exName == 'tokocrypto': result = tokocrypto()
     elif exName == 'upbit': result = upbit()
     elif exName == 'wavesexchange': result = wavesexchange()
     elif exName == 'wazirx': result = wazirx()
     elif exName == 'whitebit': result = whitebit()
```

### Comparing `byquant-1.6.15/byquant/exchange/ace.py` & `byquant-1.6.27/byquant/exchange/ace.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/alpaca.py` & `byquant-1.6.27/byquant/exchange/alpaca.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/ascendex.py` & `byquant-1.6.27/byquant/exchange/ascendex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bequant.py` & `byquant-1.6.27/byquant/exchange/bequant.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bigone.py` & `byquant-1.6.27/byquant/exchange/bigone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/binance.py` & `byquant-1.6.27/byquant/exchange/binance.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/binancecoinm.py` & `byquant-1.6.27/byquant/exchange/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/binanceus.py` & `byquant-1.6.27/byquant/exchange/binanceus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/binanceusdm.py` & `byquant-1.6.27/byquant/exchange/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bit2c.py` & `byquant-1.6.27/byquant/exchange/bit2c.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitbank.py` & `byquant-1.6.27/byquant/exchange/bitbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitbns.py` & `byquant-1.6.27/byquant/exchange/bitbns.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitfinex.py` & `byquant-1.6.27/byquant/exchange/bitfinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitfinex2.py` & `byquant-1.6.27/byquant/exchange/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitflyer.py` & `byquant-1.6.27/byquant/exchange/bitflyer.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitforex.py` & `byquant-1.6.27/byquant/exchange/bitforex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitget.py` & `byquant-1.6.27/byquant/exchange/bitget.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bithumb.py` & `byquant-1.6.27/byquant/exchange/bithumb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitmart.py` & `byquant-1.6.27/byquant/exchange/bitmart.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitmex.py` & `byquant-1.6.27/byquant/exchange/bitmex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitopro.py` & `byquant-1.6.27/byquant/exchange/bitopro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitpanda.py` & `byquant-1.6.27/byquant/exchange/bitpanda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitrue.py` & `byquant-1.6.27/byquant/exchange/bitrue.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitso.py` & `byquant-1.6.27/byquant/exchange/bitso.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitstamp.py` & `byquant-1.6.27/byquant/exchange/bitstamp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitstamp1.py` & `byquant-1.6.27/byquant/exchange/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bittrex.py` & `byquant-1.6.27/byquant/exchange/bittrex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bitvavo.py` & `byquant-1.6.27/byquant/exchange/bitvavo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bkex.py` & `byquant-1.6.27/byquant/exchange/bkex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bl3p.py` & `byquant-1.6.27/byquant/exchange/bl3p.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/blockchaincom.py` & `byquant-1.6.27/byquant/exchange/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/btcalpha.py` & `byquant-1.6.27/byquant/exchange/btcalpha.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/btcbox.py` & `byquant-1.6.27/byquant/exchange/btcbox.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/btcex.py` & `byquant-1.6.27/byquant/exchange/btcex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/btcmarkets.py` & `byquant-1.6.27/byquant/exchange/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/btctradeua.py` & `byquant-1.6.27/byquant/exchange/btctradeua.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/btcturk.py` & `byquant-1.6.27/byquant/exchange/btcturk.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/buda.py` & `byquant-1.6.27/byquant/exchange/buda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/bybit.py` & `byquant-1.6.27/byquant/exchange/bybit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/cex.py` & `byquant-1.6.27/byquant/exchange/cex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/coinbase.py` & `byquant-1.6.27/byquant/exchange/coinbase.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/coinbaseprime.py` & `byquant-1.6.27/byquant/exchange/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/coinbasepro.py` & `byquant-1.6.27/byquant/exchange/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/coincheck.py` & `byquant-1.6.27/byquant/exchange/coincheck.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/coinex.py` & `byquant-1.6.27/byquant/exchange/coinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/coinfalcon.py` & `byquant-1.6.27/byquant/exchange/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/coinmate.py` & `byquant-1.6.27/byquant/exchange/coinmate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/coinone.py` & `byquant-1.6.27/byquant/exchange/coinone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/coinsph.py` & `byquant-1.6.27/byquant/exchange/coinsph.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/coinspot.py` & `byquant-1.6.27/byquant/exchange/coinspot.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/cryptocom.py` & `byquant-1.6.27/byquant/exchange/cryptocom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/currencycom.py` & `byquant-1.6.27/byquant/exchange/currencycom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/delta.py` & `byquant-1.6.27/byquant/exchange/delta.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/deribit.py` & `byquant-1.6.27/byquant/exchange/deribit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/digifinex.py` & `byquant-1.6.27/byquant/exchange/digifinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/exmo.py` & `byquant-1.6.27/byquant/exchange/exmo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/flowbtc.py` & `byquant-1.6.27/byquant/exchange/flowbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/fmfwio.py` & `byquant-1.6.27/byquant/exchange/fmfwio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/gate.py` & `byquant-1.6.27/byquant/exchange/gate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/gemini.py` & `byquant-1.6.27/byquant/exchange/gemini.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/hitbtc.py` & `byquant-1.6.27/byquant/exchange/hitbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/hitbtc3.py` & `byquant-1.6.27/byquant/exchange/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/hollaex.py` & `byquant-1.6.27/byquant/exchange/hollaex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/huobi.py` & `byquant-1.6.27/byquant/exchange/huobi.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/huobijp.py` & `byquant-1.6.27/byquant/exchange/huobijp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/huobipro.py` & `byquant-1.6.27/byquant/exchange/huobipro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/idex.py` & `byquant-1.6.27/byquant/exchange/idex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/independentreserve.py` & `byquant-1.6.27/byquant/exchange/independentreserve.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/indodax.py` & `byquant-1.6.27/byquant/exchange/indodax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/itbit.py` & `byquant-1.6.27/byquant/exchange/itbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/kraken.py` & `byquant-1.6.27/byquant/exchange/kraken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/krakenfutures.py` & `byquant-1.6.27/byquant/exchange/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/kucoin.py` & `byquant-1.6.27/byquant/exchange/kucoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/kucoinfutures.py` & `byquant-1.6.27/byquant/exchange/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/kuna.py` & `byquant-1.6.27/byquant/exchange/kuna.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/latoken.py` & `byquant-1.6.27/byquant/exchange/latoken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/lbank.py` & `byquant-1.6.27/byquant/exchange/lbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/lbank2.py` & `byquant-1.6.27/byquant/exchange/lbank2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/luno.py` & `byquant-1.6.27/byquant/exchange/luno.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/lykke.py` & `byquant-1.6.27/byquant/exchange/lykke.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/mercado.py` & `byquant-1.6.27/byquant/exchange/mercado.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/mexc.py` & `byquant-1.6.27/byquant/exchange/mexc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/ndax.py` & `byquant-1.6.27/byquant/exchange/ndax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/novadax.py` & `byquant-1.6.27/byquant/exchange/novadax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/oceanex.py` & `byquant-1.6.27/byquant/exchange/oceanex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/okcoin.py` & `byquant-1.6.27/byquant/exchange/okcoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/okx.py` & `byquant-1.6.27/byquant/exchange/okx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/paymium.py` & `byquant-1.6.27/byquant/exchange/paymium.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/phemex.py` & `byquant-1.6.27/byquant/exchange/phemex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/poloniex.py` & `byquant-1.6.27/byquant/exchange/poloniex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/poloniexfutures.py` & `byquant-1.6.27/byquant/exchange/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/probit.py` & `byquant-1.6.27/byquant/exchange/probit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/ripio.py` & `byquant-1.6.27/byquant/exchange/ripio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/stex.py` & `byquant-1.6.27/byquant/exchange/stex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/tidex.py` & `byquant-1.6.27/byquant/exchange/tidex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/timex.py` & `byquant-1.6.27/byquant/exchange/timex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/tokocrypto.py` & `byquant-1.6.27/byquant/exchange/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/upbit.py` & `byquant-1.6.27/byquant/exchange/upbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/wavesexchange.py` & `byquant-1.6.27/byquant/exchange/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/wazirx.py` & `byquant-1.6.27/byquant/exchange/wazirx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/whitebit.py` & `byquant-1.6.27/byquant/exchange/whitebit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/woo.py` & `byquant-1.6.27/byquant/exchange/woo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/xt.py` & `byquant-1.6.27/byquant/exchange/xt.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/yobit.py` & `byquant-1.6.27/byquant/exchange/yobit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/zaif.py` & `byquant-1.6.27/byquant/exchange/zaif.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/zb.py` & `byquant-1.6.27/byquant/exchange/zb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant/exchange/zonda.py` & `byquant-1.6.27/byquant/exchange/zonda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.15/byquant.egg-info/PKG-INFO` & `byquant-1.6.27/byquant.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.6.15
-Summary: A Python trading library with support for 130+ exchanges
+Version: 1.6.27
+Summary: ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: MIT
 Project-URL: Homepage, https://byquant.com
-Keywords: algorithmic,algotrading
+Keywords: quant,strategy,algorithmic,algotrading
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `byquant-1.6.15/byquant.egg-info/SOURCES.txt` & `byquant-1.6.27/byquant.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 byquant/__init__.py
 byquant.egg-info/PKG-INFO
 byquant.egg-info/SOURCES.txt
 byquant.egg-info/dependency_links.txt
 byquant.egg-info/requires.txt
 byquant.egg-info/top_level.txt
 byquant.egg-info/zip-safe
+byquant/crypto/__init__.py
+byquant/crypto/broker.py
+byquant/crypto/feed.py
+byquant/crypto/store.py
 byquant/exchange/__init__.py
 byquant/exchange/ace.py
 byquant/exchange/alpaca.py
 byquant/exchange/ascendex.py
 byquant/exchange/bequant.py
 byquant/exchange/bigone.py
 byquant/exchange/binance.py
@@ -117,8 +121,10 @@
 byquant/exchange/wazirx.py
 byquant/exchange/whitebit.py
 byquant/exchange/woo.py
 byquant/exchange/xt.py
 byquant/exchange/yobit.py
 byquant/exchange/zaif.py
 byquant/exchange/zb.py
-byquant/exchange/zonda.py
+byquant/exchange/zonda.py
+byquant/tool/__init__.py
+byquant/tool/tawPlus.py
```

### Comparing `byquant-1.6.15/setup.py` & `byquant-1.6.27/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,32 @@
 
 here = path.abspath(path.dirname(__file__))
 root = path.dirname(here)
 
 readme = path.join(here, 'README.md')
 package = {
   "name": "byquant",
-  "version": "1.6.15",
-  "description": "A Python trading library with support for 130+ exchanges",
+  "version": "1.6.27",
+  "description": "ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community",
   "type": "module",
   "readme": "README.md",
   "package_json": "package.json",
   "author": {
     "name": "Uakeey",
     "email": "uakee@outlook.com",
     "url": "https://github.com/byquantcom/"
   },
   "license": "MIT",
   "bugs": {
     "url": "https://github.com/byquantcom/byquant/issues"
   },
   "homepage": "https://byquant.com",
   "keywords": [
+    "quant",
+    "strategy",
     "algorithmic",
     "algotrading"
   ]
 }
```

