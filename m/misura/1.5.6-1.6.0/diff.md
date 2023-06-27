# Comparing `tmp/misura-1.5.6.tar.gz` & `tmp/misura-1.6.0.tar.gz`

## Comparing `misura-1.5.6.tar` & `misura-1.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.5.6/.gitattributes
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 misura-1.5.6/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.5.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.5.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.5.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.5.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    11257 2020-02-02 00:00:00.000000 misura-1.5.6/docs/docs.md
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 misura-1.5.6/src/test.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 misura-1.5.6/src/misura/__init__.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.5.6/src/misura/__main__.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 misura-1.5.6/src/misura/exceptions.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 misura-1.5.6/src/misura/globals.py
--rw-r--r--   0        0        0    24487 2020-02-02 00:00:00.000000 misura-1.5.6/src/misura/quantities.py
--rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 misura-1.5.6/src/misura/tables.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 misura-1.5.6/src/misura/utilities.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.5.6/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.5.6/LICENSE
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 misura-1.5.6/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 misura-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.6.0/.gitattributes
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 misura-1.6.0/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 misura-1.6.0/src/test.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 misura-1.6.0/src/misura/__init__.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 misura-1.6.0/src/misura/__main__.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 misura-1.6.0/src/misura/currencies.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 misura-1.6.0/src/misura/exceptions.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 misura-1.6.0/src/misura/globals.py
+-rw-r--r--   0        0        0    25362 2020-02-02 00:00:00.000000 misura-1.6.0/src/misura/quantities.py
+-rw-r--r--   0        0        0    21415 2020-02-02 00:00:00.000000 misura-1.6.0/src/misura/tables.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 misura-1.6.0/src/misura/utilities.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.6.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.6.0/LICENSE
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 misura-1.6.0/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 misura-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 misura-1.6.0/PKG-INFO
```

### Comparing `misura-1.5.6/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.6.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.5.6/.github/workflows/python-publish.yml` & `misura-1.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.5.6/src/test.py` & `misura-1.6.0/src/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Test suite for misura.
 
 from colorama import Style
 from misura.quantities import quantity, convert, unpack, pack
 from misura.tables import addUnit
+from misura.currencies import currency
 
 addUnit("bananas", {"bnn": 1, "dabnn": 10, "hbnn": 100, "kbnn": 1000})
 
 num0 = quantity(5, "m2")
 num1 = quantity(67, "km")
 num2 = quantity(12, "A s")
 num3 = quantity(1, "C mW")
@@ -69,7 +70,16 @@
 print("\nCUSTOM UNITS OF MEASURE.\n")
 print("{} to 'bnn': {}".format(num11, convert(num11, "bnn")))
 
 # Uncertainty.
 print("\nUNCERTAINTY.\n")
 print("({}) ** 2: {}".format(num12, num12**2))
 print("({}) / ({}): {}".format(num12, num13, num12 / num13))
+
+# Currencies.
+cur0 = currency(2, "EUR")
+cur1 = currency(3, "USD")
+
+print("\nCURRENCIES.\n")
+print("({}) * 2: {}".format(cur0, cur0 * 2))
+print("({}) // 3: {}".format(cur1, cur1 // 3))
+print("({}) + ({}): {:.2f}".format(cur1, cur0, cur1 + cur0))
```

### Comparing `misura-1.5.6/src/misura/exceptions.py` & `misura-1.6.0/src/misura/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # Exceptions.
+from typing import Any
 
 
 class UnitError(Exception):
     """
     Raised on invalid units.
     """
 
     def __init__(self, unit: str) -> None:
         super().__init__("invalid unit '{}'".format(unit))
 
 
 class InitError(Exception):
     """
-    Raised on invalid parameters passed to quantity.__init__().
+    Raised on invalid parameters passed to quantity/currency.__init__().
     """
 
-    def __init__(self, value: any, unit: str = "", uncertainty: any = 0) -> None:
+    def __init__(self, value: Any, unit: str = "", uncertainty: Any = 0) -> None:
         from .utilities import uAny
 
         super().__init__(
-            "wrong parameters on quantity definition\nraised by: quantity({}{}{})".format(
+            "wrong parameters on quantity definition\nraised by passing: ({}{}{})".format(
                 value,
                 ", {}".format(unit) if unit else "",
                 ", {}".format(uncertainty) if uAny(uncertainty) else "",
             )
         )
 
 
@@ -112,7 +113,41 @@
     """
     Raised on errors during unit definition.
     """
 
     # Custom error defined in tables.py.
     def __init__(self, error: str = "") -> None:
         super().__init__(error)
+
+
+# CURRENCIES.
+
+
+class OperationError(Exception):
+    """
+    Raised on illegal operations with currencies.
+    """
+
+    def __init__(self, first, second, operator: str) -> None:
+        super().__init__(
+            "unsupported operand type(s) for {0}\nraised by: '{1}' {0} '{2}'".format(
+                operator, first, second
+            )
+        )
+
+
+class CurrencyPackingError(Exception):
+    """
+    Raised on (un)packing currencies.
+    """
+
+    def __init__(self, crn) -> None:
+        super().__init__("cannot (un)pack a currency\nraised by '{}'".format(crn))
+
+
+class MixingError(Exception):
+    """
+    Raised on mixing quantities and currencies.
+    """
+
+    def __init__(self) -> None:
+        super().__init__("quantities and currencies should not be mixed")
```

### Comparing `misura-1.5.6/src/misura/quantities.py` & `misura-1.6.0/src/misura/quantities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,54 @@
 # Quantities.
 from __future__ import annotations
 
+from math import log, sqrt
+from typing import Any
+
 from colorama import Style
-from math import sqrt, log
 
 from .exceptions import (
-    InitError,
-    QuantityError,
     ConversionError,
-    UnpackError,
+    CurrencyPackingError,
+    InitError,
+    MixingError,
     PackError,
+    QuantityError,
     UncertaintyComparisonError,
+    UnpackError,
 )
-from .tables import getBase, getDerived, getDerivedUnpacking, getFamily, getRep
-from .utilities import checkIter, uAll, uAny
-from .utilities import unitFromDict as ufd
+from .globals import logic, style
+from .tables import (
+    fetchCurrencies,
+    getBase,
+    getCurrencies,
+    getDerived,
+    getDerivedUnpacking,
+)
+from .tables import getFamily as gf
+from .tables import getRep
+from .utilities import checkIter
 from .utilities import dictFromUnit as dfu
-from .globals import style, logic
+from .utilities import uAll, uAny
+from .utilities import unitFromDict as ufd
+
+"""
+'for' convention.
+
+u : short for unit.
+us: short for units.
+"""
 
 
 class quantity:
     """
     misura's quantity class.
     """
 
-    def __init__(self, value: any, unit: str = "", uncertainty: any = 0) -> None:
+    def __init__(self, value: Any, unit: str = "", uncertainty: Any = 0) -> None:
         """
         Quantity initialization.
 
         - value: Can be anything that can be somewhat treated as a number.
         - unit: A properly formatted string including all the units with their exponents. e.g. "m s-1".
         - uncertainty: Value's uncertainty.
         """
@@ -41,125 +61,132 @@
                 if uAny(uncertainty)
                 else True
             )
 
         except AssertionError:
             raise InitError(value, unit, uncertainty)
 
-        self.value: any = value
-        self.uncertainty = uncertainty
+        # Value.
+        self.value: Any = value
+
+        # Uncertainty.
+        if not uAny(uncertainty):
+            # For when value is iterable.
+            self.uncertainty = 0 * self.value
 
+        else:
+            self.uncertainty = uncertainty
+
+        # Units of measure's table.
         table: dict = getBase()
         table.update(getDerived())
 
         # From unit: str to self.units: dict.
         self.units: dict = dfu(unit)
+        us = self.units.copy()
 
-        # Checks whether the unit can be converted with the available units.
+        # Checks whether the quantity can be converted with the defined units.
         self.convertible: bool = all(
-            [any([unit in table[family] for family in table]) for unit in self.units]
+            [any([u in table[family] for family in table]) for u in us]
         )
 
-        # Define quantity's dimentsionality based on self.units.
+        # Define quantity's dimentsions based on self.units.
         self.dimensions: dict = (
-            {getFamily(unit): self.units[unit] for unit in self.units}
-            if self.convertible
-            else dict()
+            {gf(u): self.units[u] for u in us} if self.convertible else dict()
         )
 
+        # Checks currencies.
+        if type(self) == quantity:
+            table: dict = getCurrencies()
+            if uAny(
+                [uAny([u in table[family] for u in self.units]) for family in table]
+            ):
+                raise MixingError()
+
+    # PRINTERS.
+
+    # this is unique as per 'sorted'.
+    # {"m": 1, "s": -1} and {"s": -1, "m": 1} return the same unit.
     def unit(self, print: bool = False) -> str:
         """
         Returns a readable version of the quantity's unit.
 
         'print = True' makes the output fancier.
         """
 
         if not len(self.units):
             return ""
 
-        uts: dict = self.units.copy()
-        # ut: short for unit.
+        us: dict = self.units.copy()
 
         if not print:
             # Plain version.
             # {"m": 1, "s": -1} -> "m s-1".
+            # The plain version is the same as the definition one.
             return ufd(self.units)
 
         # Fancy version.
         # {"m": 1, "s": -1} -> "[m / s]".
 
         # Numerator with exponent
-        numeratorWE = [
-            "{}({})".format(ut, uts[ut]) for ut in uts if uts[ut] > 0 and uts[ut] != 1
-        ]
+        numWE = ["{}({})".format(u, us[u]) for u in us if us[u] > 0 and us[u] != 1]
 
         # Denominator with exponent
-        denominatorWE = [
-            "{}({})".format(ut, -uts[ut]) for ut in uts if uts[ut] < 0 and uts[ut] != 1
-        ]
+        denWE = ["{}({})".format(u, -us[u]) for u in us if us[u] < 0 and us[u] != 1]
 
         # Numerator without exponent
-        numeratorWOE = [ut for ut in uts if uts[ut] > 0 and uts[ut] == 1]
+        numWOE = [u for u in us if us[u] > 0 and us[u] == 1]
 
         # Denominator without exponent
-        denominatorWOE = [ut for ut in uts if uts[ut] < 0 and uts[ut] == 1]
+        denWOE = [u for u in us if us[u] < 0 and us[u] == 1]
 
-        numerator = " ".join(sorted(numeratorWE + numeratorWOE))
-        denominator = " ".join(sorted(denominatorWE + denominatorWOE))
+        num = " ".join(sorted(numWE + numWOE))
+        den = " ".join(sorted(denWE + denWOE))
 
-        if not numerator and denominator:
-            numerator = "1"
+        if not num and den:
+            num = "1"
 
-        fraction = numerator + " / " + denominator if denominator else numerator
+        fraction = num + " / " + den if den else num
 
         if style.quantityHighlighting:
-            return Style.BRIGHT + fraction + Style.RESET_ALL if numerator else ""
+            return Style.BRIGHT + fraction + Style.RESET_ALL if num else ""
 
-        return "[" + fraction + "]" if numerator else ""
+        return "[" + fraction + "]" if num else ""
 
     def dimension(self) -> str:
         """
         Returns a readable version of the quantity's dimension.
         """
 
         if not len(self.dimensions):
             return ""
 
-        uts: dict = self.units.copy()
-        # ut: short for unit.
+        us: dict = self.units.copy()
 
         # Numerator with exponent
-        numeratorWE = [
-            "{}({})".format(getFamily(ut), uts[ut])
-            for ut in uts
-            if uts[ut] > 0 and uts[ut] != 1
-        ]
+        numWE = ["{}({})".format(gf(u), us[u]) for u in us if us[u] > 0 and us[u] != 1]
 
         # Denominator with exponent
-        denominatorWE = [
-            "{}({})".format(getFamily(ut), -uts[ut])
-            for ut in uts
-            if uts[ut] < 0 and uts[ut] != 1
-        ]
+        denWE = ["{}({})".format(gf(u), -us[u]) for u in us if us[u] < 0 and us[u] != 1]
 
         # Numerator without exponent
-        numeratorWOE = [getFamily(ut) for ut in uts if uts[ut] > 0 and uts[ut] == 1]
+        numWOE = [gf(u) for u in us if us[u] > 0 and us[u] == 1]
 
         # Denominator without exponent
-        denominatorWOE = [getFamily(ut) for ut in uts if uts[ut] < 0 and uts[ut] == 1]
+        denWOE = [gf(u) for u in us if us[u] < 0 and us[u] == 1]
 
-        numerator = " * ".join(sorted(numeratorWE + numeratorWOE))
-        denominator = " * ".join(sorted(denominatorWE + denominatorWOE))
+        num = " * ".join(sorted(numWE + numWOE))
+        den = " * ".join(sorted(denWE + denWOE))
 
-        if not numerator and denominator:
-            numerator = "1"
+        if not num and den:
+            num = "1"
 
-        fraction = numerator + " / " + denominator if denominator else numerator
+        fraction = num + " / " + den if den else num
 
-        return "[" + fraction + "]" if numerator else ""
+        return "[" + fraction + "]" if num else ""
 
     # STRINGS.
 
     def __str__(self) -> str:
         pm = style.quantityPlusMinus
         unit = self.unit(print=True)
         uncert = self.uncertainty
@@ -215,18 +242,14 @@
     def __pos__(self) -> quantity:
         return quantity(+self.value, self.unit(), self.uncertainty)
 
     # Negative.
     def __neg__(self) -> quantity:
         return quantity(-self.value, self.unit(), self.uncertainty)
 
-    # Invert.
-    # def __invert__(self) -> quantity:
-    #     return quantity(~self.value, self.unit())
-
     # Round.
     def __round__(self, number: int) -> quantity:
         return quantity(
             round(self.value, number), self.unit(), round(self.uncertainty, number + 1)
         )
 
     # Floor.
@@ -244,23 +267,23 @@
     # Trunc.
     def __trunc__(self) -> quantity:
         from math import trunc
 
         return quantity(trunc(self.value), self.unit(), trunc(self.uncertainty))
 
     # Addition.
-    def __add__(self, other: any) -> quantity:
+    def __add__(self, other: Any) -> quantity:
         if not isinstance(other, quantity):
             # Addition between pure numbers.
             if self.unit():
                 raise QuantityError(self, quantity(other, ""), "+")
 
             return quantity(self.value + other, "", self.uncertainty)
 
-        if self.unit() != other.unit():
+        if not compare(self, other):
             if self.convertible and other.convertible:
                 # Chooses the one to convert based on unit length.
                 first = convert(self, other.unit())
                 second = convert(other, self.unit())
 
                 self, other = (
                     (first, other)
@@ -277,23 +300,23 @@
             sqrt(self.uncertainty**2 + other.uncertainty**2),
         )
 
     def __radd__(self, other: quantity) -> quantity:
         return self.__add__(other)
 
     # Subtraction.
-    def __sub__(self, other: any) -> quantity:
+    def __sub__(self, other: Any) -> quantity:
         if not isinstance(other, quantity):
             # Subtraction between pure numbers.
             if self.unit():
                 raise QuantityError(self, quantity(other, ""), "-")
 
             return quantity(self.value - other, "", self.uncertainty)
 
-        if self.unit() != other.unit():
+        if not compare(self, other):
             if self.convertible and other.convertible:
                 # Chooses the one to convert based on unit length.
                 first = convert(self, other.unit())
                 second = convert(other, self.unit())
 
                 self, other = (
                     (first, other)
@@ -310,15 +333,15 @@
             sqrt(self.uncertainty**2 + other.uncertainty**2),
         )
 
     def __rsub__(self, other: quantity) -> quantity:
         return self.__sub__(other) * (-1)
 
     # Multiplication.
-    def __mul__(self, other: any) -> any:
+    def __mul__(self, other: Any) -> any:
         if not isinstance(other, quantity):
             return quantity(
                 self.value * other, self.unit(), abs(self.uncertainty * other)
             )
 
         newUnits = self.units.copy()
 
@@ -338,19 +361,19 @@
             ufd(newUnits),
             sqrt(
                 (other.value * self.uncertainty) ** 2
                 + (self.value * other.uncertainty) ** 2
             ),
         )
 
-    def __rmul__(self, other: any) -> any:
+    def __rmul__(self, other: Any) -> any:
         return self.__mul__(other)
 
     # Division.
-    def __truediv__(self, other: any) -> any:
+    def __truediv__(self, other: Any) -> any:
         if not isinstance(other, quantity):
             return quantity(
                 self.value / other, self.unit(), abs(self.uncertainty / other)
             )
 
         newUnits = self.units.copy()
 
@@ -370,24 +393,24 @@
             ufd(newUnits),
             sqrt(
                 (self.uncertainty / other.value) ** 2
                 + (self.value * other.uncertainty / (other.value**2)) ** 2
             ),
         )
 
-    def __floordiv__(self, other: any) -> quantity:
+    def __floordiv__(self, other: Any) -> quantity:
         return quantity(
             self.value // other, self.unit(), abs(self.uncertainty // other)
         )
 
-    def __rtruediv__(self, other: any) -> any:
+    def __rtruediv__(self, other: Any) -> any:
         return self**-1 * other
 
     # Power.
-    def __pow__(self, other: any) -> quantity:
+    def __pow__(self, other: Any) -> quantity:
         if isinstance(other, quantity):
             raise QuantityError(self, other, "**")
 
         if other == 0:
             return quantity(1 * bool(self.value), "", 1 * self.uncertainty != 0)
 
         if other == 1:
@@ -400,15 +423,15 @@
 
         return quantity(
             self.value**other,
             ufd(newUnits),
             abs(other) * (self.value ** (other - 1)) * self.uncertainty,
         )
 
-    def __rpow__(self, other: any) -> quantity:
+    def __rpow__(self, other: Any) -> quantity:
         if isinstance(other, quantity):
             raise QuantityError(other, self, "**")
 
         if uAny(other <= 0):
             raise ValueError(
                 "math domain error\nraised on '{}' ** '{}'".format(other, self)
             )
@@ -416,118 +439,118 @@
         return quantity(
             other**self.value,
             "",
             abs(log(other) * (other**self.value) * self.uncertainty),
         ) * (other != 1) + quantity(1) * (other == 1)
 
     # Modulo.
-    def __mod__(self, other: any) -> quantity:
+    def __mod__(self, other: Any) -> quantity:
         return quantity(self.value % other, self.unit(), self.uncertainty % other)
 
     # COMPARISONS.
 
     # Less than.
-    def __lt__(self, other: any) -> quantity:
+    def __lt__(self, other: Any) -> quantity:
         if not isinstance(other, quantity):
             return self.value < other
 
-        if self.unit() != other.unit():
+        if not compare(self, other):
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, "<")
 
         if (
             uAny(self.uncertainty) or uAny(self.uncertainty)
         ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, "<")
 
         return self.value < other.value
 
     # Less or equal.
-    def __le__(self, other: any) -> quantity:
+    def __le__(self, other: Any) -> quantity:
         if not isinstance(other, quantity):
             return self.value <= other
 
-        if self.unit() != other.unit():
+        if not compare(self, other):
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, "<=")
 
         if (
             uAny(self.uncertainty) or uAny(self.uncertainty)
         ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, "<=")
 
         return self.value <= other.value
 
     # Greater than.
-    def __gt__(self, other: any) -> quantity:
+    def __gt__(self, other: Any) -> quantity:
         if not isinstance(other, quantity):
             return self.value > other
 
-        if self.unit() != other.unit():
+        if not compare(self, other):
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, ">")
 
         if (
             uAny(self.uncertainty) or uAny(self.uncertainty)
         ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, ">")
 
         return self.value > other.value
 
     # Greater or equal.
-    def __ge__(self, other: any) -> quantity:
+    def __ge__(self, other: Any) -> quantity:
         if not isinstance(other, quantity):
             return self.value >= other
 
-        if self.unit() != other.unit():
+        if not compare(self, other):
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, ">=")
 
         if (
             uAny(self.uncertainty) or uAny(self.uncertainty)
         ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, ">=")
 
         return self.value >= other.value
 
     # Equal.
-    def __eq__(self, other: any) -> quantity:
+    def __eq__(self, other: Any) -> quantity:
         if not isinstance(other, quantity):
             return self.value == other
 
         if (
             uAny(self.uncertainty) or uAny(self.uncertainty)
         ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, "==")
 
-        return self.value == other.value and self.unit() == other.unit()
+        return self.value == other.value and compare(self, other)
 
     # Not equal.
-    def __ne__(self, other: any) -> quantity:
+    def __ne__(self, other: Any) -> quantity:
         if not isinstance(other, quantity):
             return self.value != other
 
         if (
             uAny(self.uncertainty) or uAny(self.uncertainty)
         ) and not logic.ignoreUncertainty:
             raise UncertaintyComparisonError(self, other, "!=")
 
-        return self.value != other.value or self.unit() != other.unit()
+        return self.value != other.value or not compare(self, other)
 
     # SHORTCUTS
 
     def cto(
         self, targets: str, partial: bool = False, un_pack: bool = True
     ) -> quantity:  # Convert to.
         return convert(self, targets, partial, un_pack)
@@ -550,29 +573,43 @@
 ) -> quantity:
     """
     Conversion function; converts the passed quantity object to the specified target units.
 
     "partial = True" converts only the specified units and "un_pack = True" enables automatic (un)packing.
     """
 
+    from .currencies import currency
+
+    if isinstance(qnt, currency):
+        partial = False
+        un_pack = False
+
+        fetchCurrencies()  # Checks conversion rates.
+        table: dict = getCurrencies()
+
+    else:
+        table: dict = getBase()
+        table.update(getDerived())
+
     # Cannot convert non-convertible units.
     if not qnt.convertible:
         raise ConversionError(qnt, targets)
 
     # Check dimension.
-    if not partial:
+    if not partial and not isinstance(qnt, currency):
+        # Currencies cannot be unpacked but are always compatible.
         if unpack(qnt).dimension() != unpack(quantity(1, targets)).dimension():
             raise ConversionError(qnt, targets)
 
     # Automatic (un)packing, version 2.
     if un_pack and not partial:
         # Tries to pack qnt.
         target = quantity(1, targets)
-        packUnits = {ut: target.units[ut] for ut in target.units if ut not in qnt.units}
-        ignoreUnits = {ut: qnt.units[ut] for ut in qnt.units if ut not in target.units}
+        packUnits = {u: target.units[u] for u in target.units if u not in qnt.units}
+        ignoreUnits = {u: qnt.units[u] for u in qnt.units if u not in target.units}
 
         for tr in range(3):
             try:
                 if tr == 0:
                     # First try: uses ignore and full packing.
                     return convert(
                         pack(qnt, ufd(packUnits), ignore=ufd(ignoreUnits), full=True),
@@ -607,19 +644,16 @@
         )
 
     factor: float = 1.0
     tUnits: dict = dfu(targets)  # Target units.
 
     pTargets: dict = dict()  # Partial targets.
 
-    table: dict = getBase()
-    table.update(getDerived())
-
     for unit in qnt.units.keys():
-        family = getFamily(unit)
+        family = gf(unit)
 
         # Number of corresponding families.
         families = len([tgt for tgt in tUnits if tgt in table[family]])
 
         # Check target presence if not partial.
         if families == 0 and not partial:
             raise ConversionError(qnt, targets)
@@ -646,14 +680,17 @@
             pTargets[target] = tUnits[target]
             continue
 
         # Partial conversion.
         elif partial:
             pTargets[unit] = qnt.units[unit]
 
+    if isinstance(qnt, currency):
+        return currency(qnt.value * factor, targets)
+
     return (
         quantity(qnt.value * factor, targets, qnt.uncertainty * factor)
         if not partial
         else quantity(qnt.value * factor, ufd(pTargets), qnt.uncertainty * factor)
     )
 
 
@@ -661,98 +698,107 @@
 def unpack(qnt: quantity, targets: str = "") -> quantity:
     """
     Unpacking function; unpacks the passed targets units form the quantity object.
 
     'targets = ""' completely unpacks the quantity.
     """
 
+    from .currencies import currency
+
+    if isinstance(qnt, currency):
+        raise CurrencyPackingError(qnt)
+
     unpackTable: dict = getDerivedUnpacking()
     derivedTable: dict = getDerived()
 
     if not targets:  # Unpacks all derived units.
-        targets = " ".join(
-            [unit for unit in qnt.units if getFamily(unit) in derivedTable]
-        )
+        us: dict = qnt.units.copy()
+
+        targets = " ".join([u for u in us if gf(u) in derivedTable])
 
     for target in dfu(targets):
+        us: dict = qnt.units.copy()
+
         # Checks target.
-        if getFamily(target) not in [getFamily(unit) for unit in qnt.units]:
+        if gf(target) not in [gf(u) for u in us]:
             raise UnpackError(qnt, target)
 
-        cTarget = getRep(getFamily(target))  # Conversion target.
+        cTarget = getRep(gf(target))  # Conversion target.
         cTargetPower = [  # Conversion target's power.
-            qnt.units[unit]
-            for unit in qnt.units
-            if getFamily(unit) == getFamily(target)
+            us[u] for u in us if gf(u) == gf(target)
         ].pop()
 
         # Raises an error if the program does not know how to unpack a unit.
         if cTarget not in unpackTable:
             raise UnpackError(qnt, target)
 
         # Converts the quantity to an unpackable one.
         qnt = convert(
             qnt,
             cTarget + str(cTargetPower),
             partial=True,
             un_pack=False,
         )
 
+        us: dict = qnt.units.copy()
+
         # Units that werent't involved in the previous conversion.
-        newUnits = {key: qnt.units[key] for key in qnt.units if key != cTarget}
+        newUnits = {u: us[u] for u in us if u != cTarget}
 
         # Uncertainty should not vary on packing.
         uncertainty = qnt.uncertainty
         qnt = (quantity(qnt.value, ufd(newUnits)) if len(newUnits) else qnt.value) * (
-            quantity(1, unpackTable[cTarget]) ** qnt.units[cTarget]
+            quantity(1, unpackTable[cTarget]) ** us[cTarget]
         )
         qnt.uncertainty = uncertainty
 
     return qnt
 
 
 # Packing function.
 def pack(qnt: quantity, targets: str, ignore: str = "", full: bool = False) -> quantity:
     """
     Packing function; packs the passed quantity object's unit according to the targets and the ones to ignore.
 
     'full = True' fully pack a unit.
     """
 
+    from .currencies import currency
+
+    if isinstance(qnt, currency):
+        raise CurrencyPackingError(qnt)
+
     packTable: dict = getDerivedUnpacking()
 
     unitsTable: dict = getBase()
     unitsTable.update(getDerived())
 
     if targets == "":
         raise PackError(qnt, "")
 
     # Simplify qnt -> base unit.
     for unit in qnt.units:
         cTarget = [
-            unit
-            for unit in unitsTable[getFamily(unit)]
-            if unitsTable[getFamily(unit)][unit] == 1
+            unit for unit in unitsTable[gf(unit)] if unitsTable[gf(unit)][unit] == 1
         ].pop()
         qnt = convert(qnt, cTarget + str(qnt.units[unit]), partial=True, un_pack=False)
 
     # Unpack only relevant units.
     if ignore:
         for ignored in dfu(ignore):
-            if getFamily(ignored) not in [getFamily(unit) for unit in qnt.units]:
+            if gf(ignored) not in [gf(unit) for unit in qnt.units]:
                 raise PackError(qnt, targets, ignore)
 
         val = qnt.value
-        uts: dict = qnt.units.copy()
-        # ut: short for unit.
+        us: dict = qnt.units.copy()
 
         # Does not completely unpack the quantity qnt but unpacks the non-ignored units
         # and then merges them with the ignored ones.
-        ignored = quantity(val, ufd({ut: uts[ut] for ut in uts if ut in dfu(ignore)}))
-        packed = quantity(1, ufd({ut: uts[ut] for ut in uts if ut not in dfu(ignore)}))
+        ignored = quantity(val, ufd({u: us[u] for u in us if u in dfu(ignore)}))
+        packed = quantity(1, ufd({u: us[u] for u in us if u not in dfu(ignore)}))
 
         qnt = ignored * unpack(packed)
 
     else:
         qnt = unpack(qnt)
 
     for target in dfu(targets):
@@ -788,7 +834,15 @@
 
         # Uncertainty should not vary on packing.
         uncertainty = qnt.uncertainty
         qnt *= (quantity(1, target) / quantity(1, ufd(targetUnits))) ** max(powers)
         qnt.uncertainty = uncertainty
 
     return qnt
+
+
+# QUANTITIES UTILITIES.
+
+
+# Compares units of measure between two quantities.
+def compare(first: quantity, second: quantity) -> bool:
+    return first.unit() == second.unit()
```

### Comparing `misura-1.5.6/src/misura/tables.py` & `misura-1.6.0/src/misura/tables.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 # Tables.
+import json
+from time import time
+
+import requests
+
 from .exceptions import DefinitionError
-from .utilities import dictFromUnit
 from .globals import defined
+from .utilities import dictFromUnit
 
 # Tables utilities
 
 
 def getRep(family: str) -> str:
     """
     Returns a reference unit given its family.
     """
 
     table = getBase()
     table.update(getDerived())
 
     if family in table:
         # This shouldn't raise an IndexError as long as there's a reference unit for every family.
-        return [unit for unit in table[family] if table[family][unit] == 1].pop()
+        return [u for u in table[family] if table[family][u] == 1].pop()
 
 
 def getFamily(unit: str) -> str:
     """
     Returns the family of a convertible unit.
     """
 
     table = getBase()
     table.update(getDerived())
+    table.update(getCurrencies())
 
     for family in table:
         if unit in table[family]:
             return family
 
     return ""
 
@@ -63,82 +69,120 @@
 
     # User defined derived units.
     table.update(defined.DERIVED_UNPACKING_TABLE)
 
     return table
 
 
+def getCurrencies() -> dict:
+    # Standard currencies.
+    table = CURRENCIES_TABLE.copy()
+
+    return table
+
+
+def fetchCurrencies() -> None:
+    from .globals import currencies
+
+    try:
+        file = open(currencies.path, "r")
+        data = json.load(file)
+
+        # Reload rates older than 6 hours.
+        if time() - data["time"] < 3600 * 6:
+            rates = data["rates"]
+
+        else:
+            raise FileNotFoundError
+
+    except (FileNotFoundError, json.JSONDecodeError):
+        rates = requests.get(
+            "https://misura.diantonioandrea.com/currencies/rates.json"
+        ).json()["data"]
+
+        file = open(currencies.path, "w")
+        data = {"time": time(), "rates": rates}
+        json.dump(data, file)
+
+    file.close()
+
+    for curr in rates:
+        CURRENCIES_TABLE["currency"][curr] = 1 / rates[curr]
+
+
 # Conversion tables.
 
 
 def addUnit(family: str, units: dict, unpacks: str = ""):
     """
     addUnit function, allows users to define new units.
     """
 
     table = getBase()
     table.update(getDerived())
 
     try:
         assert isinstance(family, str)
         assert isinstance(units, dict)
-        assert family != ""
-        assert len(units)
+        assert family
+        assert units
 
         assert isinstance(unpacks, str) if unpacks else True
 
     except AssertionError:
         raise DefinitionError("invalid options")
 
     family = family.lower()
 
     # Checks family.
     if family in table:
         raise DefinitionError("'{}' already exixts".format(family))
 
     # Checks rep.
-    if len([unit for unit in units if units[unit] == 1]) != 1:
+    if len([u for u in units if units[u] == 1]) != 1:
         raise DefinitionError("missing or invalid rep for family {}".format(family))
 
     # Checks units.
-    for unit in units:
-        if not isinstance(unit, str):
-            raise DefinitionError("invalid unit '{}'".format(unit))
+    for u in units:
+        if not isinstance(u, str):
+            raise DefinitionError("invalid unit '{}'".format(u))
 
-        if not isinstance(units[unit], (int, float)):
+        if not isinstance(units[u], (int, float)):
             raise DefinitionError(
-                "invalid unit factor for '{}: {}'".format(unit, units[unit])
+                "invalid unit factor for '{}: {}'".format(u, units[u])
             )
 
-        if any([unit in table[family] for family in table]):
+        if any([u in table[family] for family in table]):
             raise DefinitionError(
-                "unit already defined in family '{}'".format(getFamily(unit))
+                "unit already defined in family '{}'".format(getFamily(u))
             )
 
     # Derived units checks.
     if unpacks:
-        rep = [unit for unit in units if units[unit] == 1].pop()
+        rep = [u for u in units if units[u] == 1].pop()
 
         if rep in getDerivedUnpacking():
             raise DefinitionError(
                 "unit already defined in the unpacking table '{}'".format(rep)
             )
 
-        for unit in dictFromUnit(unpacks):
-            if not getFamily(unit):
-                raise DefinitionError("invalid unit '{}'".format(unit))
+        for u in dictFromUnit(unpacks):
+            if not getFamily(u):
+                raise DefinitionError("invalid unit '{}'".format(u))
 
     if not unpacks:
-        defined.BASE_TABLE[family] = {unit: units[unit] for unit in units}
+        defined.BASE_TABLE[family] = {u: units[u] for u in units}
 
     else:
-        defined.DERIVED_TABLE[family] = {unit: units[unit] for unit in units}
+        defined.DERIVED_TABLE[family] = {u: units[u] for u in units}
         defined.DERIVED_UNPACKING_TABLE[rep] = unpacks
 
 
+# QUANTITIES
+
 # Base units - SI.
 SI_TABLE = {
     "time": {
         "qs": 1e-30,
         "rs": 1e-27,
         "ys": 1e-24,
         "zs": 1e-21,
@@ -917,7 +961,11 @@
     "lm": "cd sr",
     "lx": "cd sr m-2",
     "Bq": "s-1",
     "Gy": "m2 s-2",
     "Sv": "m2 s-2",
     "kat": "mol s-1",
 }
+
+# CURRENCIES
+
+CURRENCIES_TABLE = {"currency": dict()}
```

### Comparing `misura-1.5.6/src/misura/utilities.py` & `misura-1.6.0/src/misura/utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # Utilities.
 from re import findall
+from typing import Any
 
 
-def checkIter(obj: any) -> bool:
+def checkIter(obj: Any) -> bool:
     try:
         _ = iter(obj)
         return True
 
     except TypeError:
         return False
 
 
-def uAll(obj: any) -> bool:
+def uAll(obj: Any) -> bool:
     """
     Python's 'all' for (non)iterable objects.
     """
 
     return all(obj) if checkIter(obj) else bool(obj)
 
 
-def uAny(obj: any) -> bool:
+def uAny(obj: Any) -> bool:
     """
     Python's 'any' for (non)iterable objects.
     """
 
     return any(obj) if checkIter(obj) else bool(obj)
```

### Comparing `misura-1.5.6/LICENSE` & `misura-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.5.6/README.md` & `misura-1.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,38 +4,45 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/misura)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/misura)
 
 ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/diantonioandrea/misura)
 ![GitHub last commit](https://img.shields.io/github/last-commit/diantonioandrea/misura)
 ![GitHub Release Date](https://img.shields.io/github/release-date/diantonioandrea/misura)
 
+![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/diantonioandrea/misura/latest)
+
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # misura
 
 ```python
 >>> from misura.quantities import quantity
 >>> quantity(7, "m", 1.5) / quantity(2, "s")
 3.5 ± 0.75 m / s
+
+>>> from misura.currencies import currency
+>>> currency(2, "EUR") + currency(3, "USD")
+5.17 USD
 ```
 
-Python library for easy unit handling and conversion for scientific & engineering applications.
+Python library providing effortless unit handling and currency conversion for scientific and engineering purposes.
 
-**misura** is a powerful Python library designed to streamline the *handling of units of measure for scientific and engineering applications*. It offers a unified interface for dealing with *different units and their conversions*, so you can quickly and accurately *perform calculations without the need for complex manual conversions*. Additionally, **misura** provides *uncertainty handling*, so *you can work with physical quantities and their associated uncertainties in a consistent and intuitive way*. On top of that, **misura** enables you to *define your own custom units of measure*, giving you the flexibility to work in your preferred units.
+**misura** is a powerful Python library designed to facilitate the efficient handling of units of measure for scientific and engineering applications, including currencies handling and conversion with constantly updated exchange rates. With its unified interface for dealing with different units and their conversions, you can quickly and accurately complete calculations without the need for complex manual conversions. Additionally, **misura** supports uncertainty handling allowing you to work with physical quantities and their associated uncertainties in a user-friendly and intuitive fashion. What's more, **misura** grants you the flexibility to create custom units of measure, so you can work in your preferred units.
 
-Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/.github/blob/main/CONTRIBUTING.md) and at the [examples](#examples).
+Make sure to take a look at the [documentation](https://misura.diantonioandrea.com), at the [contributing guidelines](https://github.com/diantonioandrea/.github/blob/main/CONTRIBUTING.md) and at the [examples](#examples).
 
 ### Features
 
 - Mathematical and logical operations between quantities: [Example](#mathematical-operations), [example](#comparisons)
+- Currencies handling with daily updated exchange rates. ![New feature](https://img.shields.io/badge/new-green)
 - Uncertainty handling: [Example](#mathematical-operations) ![New feature](https://img.shields.io/badge/new-green)
 - Manual conversions: [Example](#manual-and-automatic-conversion)
 - Automatic conversions on operations: [Example](#manual-and-automatic-conversion)
 - Unpack and pack derived units: [Example](#unpack-derived-units), [example](#pack-units)
-- User defined base and derived units: [Example](#user-defined-units-of-measure) ![New feature](https://img.shields.io/badge/new-green)
+- User defined base and derived units: [Example](#user-defined-units-of-measure)
 - Large compatibility with other libraries: [Example](#working-with-other-libraries)
 - Custom exceptions: [Example](#comparisons)
 
 ## Installation
 
 ### Installing misura
 
@@ -49,62 +56,26 @@
 
 By:
 
 ```
 python -m misura
 ```
 
-you'll be able to verify the installation of **misura** along getting some informations about the library and on the available units of measure[^1]:
+you'll be able to verify the installation of **misura** along getting some informations about the library[^1]:
 
-[^1]: Example referring to version 1.3.1
+[^1]: Example referring to version 1.6.0
 
 ```
-misura v1.3.1
+misura v1.6.0
 
 Python library for easy unit handling and conversion for scientific & engineering applications.
 
 Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/misura
-Documentation on https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
+Documentation on https://misura.diantonioandrea.com
 Bug tracker on https://github.com/diantonioandrea/misura/issues
-
-Here's the list of available units.
-
-BASE UNITS
-
-Time: s.
-Length: m.
-Mass: kg.
-Electric current: A.
-Thermodynamic temperature: K.
-Amount of substance: mol.
-Luminous intensity: cd.
-
-DERIVED UNITS
-
-Plane angle: rad.
-Solid angle: sr.
-Frequency: Hz [s-1].
-Force: N [kg m s-2].
-Pressure: Pa [kg m-1 s-2].
-Energy: J [kg m2 s-2].
-Power: W [kg m2 s-3].
-Electric charge: C [A s].
-Electric potential: V [kg m2 s-3 A-1].
-Capacitance: F [kg-1 m-2 s4 A2].
-Resistance: Ω [kg m2 s-3 A-2].
-Electrical conductance: S [kg-1 m-2 s3 A2].
-Magnetic flux: Wb [kg m2 s-2 A-1].
-Magnetic flux density: T [kg s-2 A-1].
-Inductance: H [kg m2 s-2 A-2].
-Luminous flux: lm [cd sr].
-Illuminance: lx [cd sr m-2].
-Radionuclide activity: Bq [s-1].
-Absorbed dose: Gy [m2 s-2].
-Equivalent dose: Sv [m2 s-2].
-Catalyc activity: kat [mol s-1].
 ```
 
 ### Importing misura
 
 **misura** can be imported by:
 
 ```
@@ -138,14 +109,33 @@
 6 m / s
 [length / time]
 8 m(2) / s(2)
 1.0 ± 0.25 m / s(2)
 4 ± 2.0 s(2)
 ```
 
+### Currencies
+
+```python
+from misura.currencies import currency
+
+cur1 = currency(2, "EUR")
+cur2 = currency(3, "USD")
+
+print(cur0 * 2)
+print(cur1 + cur0)
+```
+
+The output is:
+
+```
+4 EUR
+5.17 USD
+```
+
 ### Working with other libraries
 
 ```python
 from misura.quantities import quantity, convert
 from decimal import Decimal, getcontext
 import numpy
```

### Comparing `misura-1.5.6/pyproject.toml` & `misura-1.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.5.6"
+version = "1.6.0"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ["colorama", "setuptools"]
+dependencies = ["colorama", "setuptools", "requests"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/diantonioandrea/misura"
-"Documentation" = "https://github.com/diantonioandrea/misura/blob/main/docs/docs.md"
+"Documentation" = "https://misura.diantonioandrea.com"
 "Bug Tracker" = "https://github.com/diantonioandrea/misura/issues"
```

### Comparing `misura-1.5.6/PKG-INFO` & `misura-1.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,66 @@
 Metadata-Version: 2.1
 Name: misura
-Version: 1.5.6
+Version: 1.6.0
 Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
 Project-URL: Homepage, https://github.com/diantonioandrea/misura
-Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
+Project-URL: Documentation, https://misura.diantonioandrea.com
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: colorama
+Requires-Dist: requests
 Requires-Dist: setuptools
 Description-Content-Type: text/markdown
 
 ![GitHub](https://img.shields.io/github/license/diantonioandrea/misura)
 
 ![PyPI](https://img.shields.io/pypi/v/misura?label=misura%20on%20pypi)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/misura)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/misura)
 
 ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/diantonioandrea/misura)
 ![GitHub last commit](https://img.shields.io/github/last-commit/diantonioandrea/misura)
 ![GitHub Release Date](https://img.shields.io/github/release-date/diantonioandrea/misura)
 
+![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/diantonioandrea/misura/latest)
+
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # misura
 
 ```python
 >>> from misura.quantities import quantity
 >>> quantity(7, "m", 1.5) / quantity(2, "s")
 3.5 ± 0.75 m / s
+
+>>> from misura.currencies import currency
+>>> currency(2, "EUR") + currency(3, "USD")
+5.17 USD
 ```
 
-Python library for easy unit handling and conversion for scientific & engineering applications.
+Python library providing effortless unit handling and currency conversion for scientific and engineering purposes.
 
-**misura** is a powerful Python library designed to streamline the *handling of units of measure for scientific and engineering applications*. It offers a unified interface for dealing with *different units and their conversions*, so you can quickly and accurately *perform calculations without the need for complex manual conversions*. Additionally, **misura** provides *uncertainty handling*, so *you can work with physical quantities and their associated uncertainties in a consistent and intuitive way*. On top of that, **misura** enables you to *define your own custom units of measure*, giving you the flexibility to work in your preferred units.
+**misura** is a powerful Python library designed to facilitate the efficient handling of units of measure for scientific and engineering applications, including currencies handling and conversion with constantly updated exchange rates. With its unified interface for dealing with different units and their conversions, you can quickly and accurately complete calculations without the need for complex manual conversions. Additionally, **misura** supports uncertainty handling allowing you to work with physical quantities and their associated uncertainties in a user-friendly and intuitive fashion. What's more, **misura** grants you the flexibility to create custom units of measure, so you can work in your preferred units.
 
-Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/.github/blob/main/CONTRIBUTING.md) and at the [examples](#examples).
+Make sure to take a look at the [documentation](https://misura.diantonioandrea.com), at the [contributing guidelines](https://github.com/diantonioandrea/.github/blob/main/CONTRIBUTING.md) and at the [examples](#examples).
 
 ### Features
 
 - Mathematical and logical operations between quantities: [Example](#mathematical-operations), [example](#comparisons)
+- Currencies handling with daily updated exchange rates. ![New feature](https://img.shields.io/badge/new-green)
 - Uncertainty handling: [Example](#mathematical-operations) ![New feature](https://img.shields.io/badge/new-green)
 - Manual conversions: [Example](#manual-and-automatic-conversion)
 - Automatic conversions on operations: [Example](#manual-and-automatic-conversion)
 - Unpack and pack derived units: [Example](#unpack-derived-units), [example](#pack-units)
-- User defined base and derived units: [Example](#user-defined-units-of-measure) ![New feature](https://img.shields.io/badge/new-green)
+- User defined base and derived units: [Example](#user-defined-units-of-measure)
 - Large compatibility with other libraries: [Example](#working-with-other-libraries)
 - Custom exceptions: [Example](#comparisons)
 
 ## Installation
 
 ### Installing misura
 
@@ -66,62 +74,26 @@
 
 By:
 
 ```
 python -m misura
 ```
 
-you'll be able to verify the installation of **misura** along getting some informations about the library and on the available units of measure[^1]:
+you'll be able to verify the installation of **misura** along getting some informations about the library[^1]:
 
-[^1]: Example referring to version 1.3.1
+[^1]: Example referring to version 1.6.0
 
 ```
-misura v1.3.1
+misura v1.6.0
 
 Python library for easy unit handling and conversion for scientific & engineering applications.
 
 Developed by Andrea Di Antonio, more on https://github.com/diantonioandrea/misura
-Documentation on https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
+Documentation on https://misura.diantonioandrea.com
 Bug tracker on https://github.com/diantonioandrea/misura/issues
-
-Here's the list of available units.
-
-BASE UNITS
-
-Time: s.
-Length: m.
-Mass: kg.
-Electric current: A.
-Thermodynamic temperature: K.
-Amount of substance: mol.
-Luminous intensity: cd.
-
-DERIVED UNITS
-
-Plane angle: rad.
-Solid angle: sr.
-Frequency: Hz [s-1].
-Force: N [kg m s-2].
-Pressure: Pa [kg m-1 s-2].
-Energy: J [kg m2 s-2].
-Power: W [kg m2 s-3].
-Electric charge: C [A s].
-Electric potential: V [kg m2 s-3 A-1].
-Capacitance: F [kg-1 m-2 s4 A2].
-Resistance: Ω [kg m2 s-3 A-2].
-Electrical conductance: S [kg-1 m-2 s3 A2].
-Magnetic flux: Wb [kg m2 s-2 A-1].
-Magnetic flux density: T [kg s-2 A-1].
-Inductance: H [kg m2 s-2 A-2].
-Luminous flux: lm [cd sr].
-Illuminance: lx [cd sr m-2].
-Radionuclide activity: Bq [s-1].
-Absorbed dose: Gy [m2 s-2].
-Equivalent dose: Sv [m2 s-2].
-Catalyc activity: kat [mol s-1].
 ```
 
 ### Importing misura
 
 **misura** can be imported by:
 
 ```
@@ -155,14 +127,33 @@
 6 m / s
 [length / time]
 8 m(2) / s(2)
 1.0 ± 0.25 m / s(2)
 4 ± 2.0 s(2)
 ```
 
+### Currencies
+
+```python
+from misura.currencies import currency
+
+cur1 = currency(2, "EUR")
+cur2 = currency(3, "USD")
+
+print(cur0 * 2)
+print(cur1 + cur0)
+```
+
+The output is:
+
+```
+4 EUR
+5.17 USD
+```
+
 ### Working with other libraries
 
 ```python
 from misura.quantities import quantity, convert
 from decimal import Decimal, getcontext
 import numpy
```

