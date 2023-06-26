# Comparing `tmp/databento_dbn-0.7.0-cp39-none-win_amd64.whl.zip` & `tmp/databento_dbn-0.7.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 559738 bytes, number of entries: 8
--rw-r--r--  4.6 unx     3052 b- defN 23-Jun-20 17:37 databento_dbn-0.7.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jun-20 17:37 databento_dbn-0.7.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     9868 b- defN 23-Jun-20 17:37 databento_dbn-0.7.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      135 b- defN 23-Jun-20 17:37 databento_dbn/__init__.py
--rw-r--r--  4.6 unx    37101 b- defN 23-Jun-20 17:37 databento_dbn/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-20 17:37 databento_dbn/py.typed
--rwxr-xr-x  4.6 unx  1616384 b- defN 23-Jun-20 17:37 databento_dbn/databento_dbn.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      679 b- defN 23-Jun-20 17:37 databento_dbn-0.7.0.dist-info/RECORD
-8 files, 1667313 bytes uncompressed, 558550 bytes compressed:  66.5%
+Zip file size: 585697 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     3052 b- defN 23-Jun-26 23:39 databento_dbn-0.7.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jun-26 23:39 databento_dbn-0.7.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     9868 b- defN 23-Jun-26 23:39 databento_dbn-0.7.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      135 b- defN 23-Jun-26 23:39 databento_dbn/__init__.py
+-rw-r--r--  4.6 unx    40122 b- defN 23-Jun-26 23:39 databento_dbn/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-26 23:39 databento_dbn/py.typed
+-rwxr-xr-x  4.6 unx  1675264 b- defN 23-Jun-26 23:39 databento_dbn/databento_dbn.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      679 b- defN 23-Jun-26 23:39 databento_dbn-0.7.1.dist-info/RECORD
+8 files, 1729214 bytes uncompressed, 584509 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: databento_dbn-0.7.0.dist-info/METADATA
+Filename: databento_dbn-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: databento_dbn-0.7.0.dist-info/WHEEL
+Filename: databento_dbn-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: databento_dbn-0.7.0.dist-info/license_files/LICENSE
+Filename: databento_dbn-0.7.1.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: databento_dbn/__init__.py
 Comment: 
 
 Filename: databento_dbn/__init__.pyi
 Comment: 
 
 Filename: databento_dbn/py.typed
 Comment: 
 
 Filename: databento_dbn/databento_dbn.cp39-win_amd64.pyd
 Comment: 
 
-Filename: databento_dbn-0.7.0.dist-info/RECORD
+Filename: databento_dbn-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databento_dbn/__init__.pyi

```diff
@@ -1,11 +1,13 @@
 # ruff: noqa: PYI021 PYI053
 from __future__ import annotations
 
+from collections.abc import Iterable
 from collections.abc import Sequence
+from enum import Enum
 from typing import (
     Any,
     BinaryIO,
     SupportsBytes,
     Union,
 )
 
@@ -21,14 +23,140 @@
     ImbalanceMsg,
     ErrorMsg,
     SymbolMappingMsg,
     SystemMsg,
     StatMsg,
 ]
 
+class Compression(Enum):
+    """
+    Data compression format.
+
+    NONE
+        Uncompressed
+    ZSTD
+        Zstandard compressed.
+
+    """
+
+    NONE: str
+    ZSTD: str
+
+    @classmethod
+    def from_str(cls, str) -> Compression: ...
+
+    @classmethod
+    def variants(cls) -> Iterable[Compression]: ...
+
+class Encoding(Enum):
+    """
+    Data output encoding.
+
+    DBN
+        Databento Binary Encoding.
+    CSV
+        Comma-separated values.
+    JSON
+        JavaScript object notation.
+
+    """
+
+    DBN: str
+    CSV: str
+    JSON: str
+
+    @classmethod
+    def from_str(cls, str) -> Encoding: ...
+
+    @classmethod
+    def variants(cls) -> Iterable[Compression]: ...
+
+class Schema(Enum):
+    """
+    A DBN record schema.
+
+    MBO
+        Market by order.
+    MBP_1
+        Market by price with a book depth of 1.
+    MBP_10
+        Market by price with a book depth of 10.
+    TBBO
+        All trade events with the best bid and offer (BBO) immediately before the effect of the trade.
+    TRADES
+        All trade events.
+    OHLCV_1S
+        Open, high, low, close, and volume at a one-second interval.
+    OHLCV_1M
+        Open, high, low, close, and volume at a one-minute interval.
+    OHLCV_1H
+        Open, high, low, close, and volume at an hourly interval.
+    OHLCV_1D
+        Open, high, low, close, and volume at a daily interval.
+    DEFINITION
+        Instrument definitions.
+    STATISTICS
+        Additional data disseminated by publishers.
+    STATUS
+        Exchange status.
+    IMBALANCE
+        Auction imbalance events.
+
+    """
+
+    MBO: str
+    MBP_1: str
+    MBP_10: str
+    TBBO: str
+    TRADES: str
+    OHLCV_1S: str
+    OHLCV_1M: str
+    OHLCV_1H: str
+    OHLCV_1D: str
+    DEFINITION: str
+    STATISTICS: str
+    STATUS: str
+    IMBALANCE: str
+
+    @classmethod
+    def from_str(cls, str) -> Schema: ...
+
+    @classmethod
+    def variants(cls) -> Iterable[Schema]: ...
+
+
+class SType(Enum):
+    """
+    A DBN symbology type.
+
+    INSTRUMENT_ID
+        Symbology using a unique numeric ID.
+    RAW_SYMBOL
+        Symbology using the original symbols provided by the publisher.
+    CONTINUOUS
+        A Databento-specific symbology where one symbol may point to different
+        instruments at different points of time, e.g. to always refer to the front month
+        future.
+    PARENT
+        A Databento-specific symbology for referring to a group of symbols by one
+        "parent" symbol, e.g. ES.FUT to refer to all ES futures.
+
+    """
+
+    INSTRUMENT_ID: str
+    RAW_SYMBOL: str
+    CONTINUOUS: str
+    PARENT: str
+
+    @classmethod
+    def from_str(cls, str) -> SType: ...
+
+    @classmethod
+    def variants(cls) -> Iterable[SType]: ...
+
 class Metadata(SupportsBytes):
     """
     Information about the data contained in a DBN file or stream. DBN requires
     the Metadata to be included at the start of the encoded data.
 
     See Also
     --------
@@ -208,15 +336,17 @@
         ------
         ValueError
             When the Metadata object cannot be encoded.
 
         """
 
 class RecordHeader:
-    """DBN Record Header."""
+    """
+    DBN Record Header.
+    """
 
     @property
     def length(self) -> int:
         """
         The length of the record.
 
         Returns
@@ -263,15 +393,17 @@
         Returns
         -------
         int
 
         """
 
 class Record(SupportsBytes):
-    """Base class for DBN records."""
+    """
+    Base class for DBN records.
+    """
 
     def __bytes__(self) -> bytes: ...
     def __eq__(self, other) -> bool: ...
     def __ne__(self, other) -> bool: ...
     @property
     def hd(self) -> RecordHeader:
         """
@@ -350,25 +482,27 @@
         -------
         int
 
         """
     @property
     def ts_out(self) -> int | None:
         """
-        The live gateway send timestamp expressed as number of nanoseconds since
-        the UNIX epoch.
+        The live gateway send timestamp expressed as number of nanoseconds
+        since the UNIX epoch.
 
         Returns
         -------
         int | None
 
         """
 
 class _MBOBase:
-    """Base for market-by-order messages."""
+    """
+    Base for market-by-order messages.
+    """
 
     @property
     def order_id(self) -> int:
         """
         The order ID assigned at the venue.
 
         Returns
@@ -467,18 +601,22 @@
         Returns
         -------
         int
 
         """
 
 class MBOMsg(Record, _MBOBase):
-    """A market-by-order (MBO) tick message."""
+    """
+    A market-by-order (MBO) tick message.
+    """
 
 class BidAskPair:
-    """A book level."""
+    """
+    A book level.
+    """
 
     @property
     def bid_px(self) -> int:
         """
         The bid price.
 
         Returns
@@ -534,15 +672,17 @@
         Returns
         -------
         int
 
         """
 
 class _MBPBase:
-    """Base for market-by-price messages."""
+    """
+    Base for market-by-price messages.
+    """
 
     @property
     def price(self) -> int:
         """
         The order price expressed as a signed integer where every 1 unit
         corresponds to 1e-9, i.e. 1/1,000,000,000 or 0.000000001.
 
@@ -639,15 +779,17 @@
     Market by price implementation with a book depth of 0.
 
     Equivalent to MBP-0. The record of the `Trades` schema.
 
     """
 
 class MBP1Msg(Record, _MBPBase):
-    """Market by price implementation with a known book depth of 1."""
+    """
+    Market by price implementation with a known book depth of 1.
+    """
 
     @property
     def levels(self) -> list[BidAskPair]:
         """
         The top of the order book.
 
         Returns
@@ -657,15 +799,17 @@
         Notes
         -----
         MBP1Msg contains 1 level of BidAskPair.
 
         """
 
 class MBP10Msg(Record, _MBPBase):
-    """Market by price implementation with a known book depth of 10."""
+    """
+    Market by price implementation with a known book depth of 10.
+    """
 
     @property
     def levels(self) -> list[BidAskPair]:
         """
         The top 10 levels.
 
         Returns
@@ -675,15 +819,17 @@
         Notes
         -----
         MBP10Msg contains 10 levels of BidAskPairs.
 
         """
 
 class OHLCVMsg(Record):
-    """Open, high, low, close, and volume message."""
+    """
+    Open, high, low, close, and volume message.
+    """
 
     @property
     def open(self) -> int:
         """
         The open price for the bar.
 
         Returns
@@ -729,15 +875,17 @@
         Returns
         -------
         int
 
         """
 
 class InstrumentDefMsg(Record):
-    """Definition of an instrument."""
+    """
+    Definition of an instrument.
+    """
 
     @property
     def ts_recv(self) -> int:
         """
         The capture-server-received timestamp expressed as number of
         nanoseconds since the UNIX epoch.
 
@@ -1343,15 +1491,17 @@
         Returns
         -------
         int
 
         """
 
 class ImbalanceMsg(Record):
-    """An auction imbalance message."""
+    """
+    An auction imbalance message.
+    """
 
     @property
     def ts_recv(self) -> int:
         """
         The capture-server-received timestamp expressed as the number of
         nanoseconds since the UNIX epoch.
 
@@ -1647,16 +1797,16 @@
         -------
         int
 
         """
     @property
     def update_action(self) -> int:
         """
-        Indicates if the statistic is newly added (1) or deleted (2). (Deleted is only
-        used with some stat types)
+        Indicates if the statistic is newly added (1) or deleted (2). (Deleted
+        is only used with some stat types)
 
         Returns
         -------
         int
 
         """
     @property
@@ -1667,15 +1817,17 @@
         Returns
         -------
         int
 
         """
 
 class ErrorMsg(Record):
-    """An error message from the Databento Live Subscription Gateway (LSG)."""
+    """
+    An error message from the Databento Live Subscription Gateway (LSG).
+    """
 
     @property
     def err(self) -> str:
         """
         The error message.
 
         Returns
@@ -1759,15 +1911,17 @@
         Returns
         -------
         bool
 
         """
 
 class DBNDecoder:
-    """A class for decoding DBN data to Python objects."""
+    """
+    A class for decoding DBN data to Python objects.
+    """
 
     def buffer(self) -> bytes:
         """
         Return the internal buffer of the decoder.
 
         Returns
         -------
```

## Comparing `databento_dbn-0.7.0.dist-info/METADATA` & `databento_dbn-0.7.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databento-dbn
-Version: 0.7.0
+Version: 0.7.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python bindings for encoding and decoding Databento Binary Encoding (DBN)
 Author: Databento <support@databento.com>
 Author-email: Databento <support@databento.com>
```

## Comparing `databento_dbn-0.7.0.dist-info/license_files/LICENSE` & `databento_dbn-0.7.1.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `databento_dbn-0.7.0.dist-info/RECORD` & `databento_dbn-0.7.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-databento_dbn-0.7.0.dist-info/METADATA,sha256=9WuYbnme04rcP43y2FPcm17nPjZF-F3PrIUexfj0J_A,3052
-databento_dbn-0.7.0.dist-info/WHEEL,sha256=AEr5m1XkYiXdLchbOjtn7VSjoPs_2BeqH39awFrbrB0,94
-databento_dbn-0.7.0.dist-info/license_files/LICENSE,sha256=d69bve2VkRS216XupRiyvjZOBPT0qV-eh9mHDCdxPSQ,9868
+databento_dbn-0.7.1.dist-info/METADATA,sha256=1vPQ0b5zmshGRfdpnUr6ZZpnhuPgLMYms8BRKxGg4t0,3052
+databento_dbn-0.7.1.dist-info/WHEEL,sha256=AEr5m1XkYiXdLchbOjtn7VSjoPs_2BeqH39awFrbrB0,94
+databento_dbn-0.7.1.dist-info/license_files/LICENSE,sha256=d69bve2VkRS216XupRiyvjZOBPT0qV-eh9mHDCdxPSQ,9868
 databento_dbn/__init__.py,sha256=TeY-_YtACSjQLT3FBRPqxJrcYFf8yu_11WeB5LcyEKo,135
-databento_dbn/__init__.pyi,sha256=ZicjU1LjQbzjIP0hv2iVkZKJqU_-NhAiRUWwvrSYN6k,37101
+databento_dbn/__init__.pyi,sha256=R714OVypbit4u3ubGSe_Uf50vslkyVGit9O08UVUpCE,40122
 databento_dbn/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-databento_dbn/databento_dbn.cp39-win_amd64.pyd,sha256=VR3le8GJz7LKr75cfshj8z7XKbgjW0N5p3gZEKGVupY,1616384
-databento_dbn-0.7.0.dist-info/RECORD,,
+databento_dbn/databento_dbn.cp39-win_amd64.pyd,sha256=cS1hM93putu2ou1dvTf1HrBjNDeSMCBNi_8i2Zcm4Wc,1675264
+databento_dbn-0.7.1.dist-info/RECORD,,
```

