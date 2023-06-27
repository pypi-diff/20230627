# Comparing `tmp/saw-client-0.9.0.tar.gz` & `tmp/saw_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saw-client-0.9.0.tar", max compression
+gzip compressed data, was "saw_client-1.0.0.tar", max compression
```

## Comparing `saw-client-0.9.0.tar` & `saw_client-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     7375 2021-11-19 17:12:25.932117 saw-client-0.9.0/README.md
--rw-r--r--   0        0        0      352 2021-11-19 17:12:25.932321 saw-client-0.9.0/mypy.ini
--rw-r--r--   0        0        0      560 2021-11-19 23:27:38.591047 saw-client-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    24120 2021-11-19 17:12:25.933390 saw-client-0.9.0/saw_client/__init__.py
--rw-r--r--   0        0        0     6493 2021-11-19 17:12:25.933651 saw-client-0.9.0/saw_client/commands.py
--rw-r--r--   0        0        0    10247 2021-11-19 17:12:25.933892 saw-client-0.9.0/saw_client/connection.py
--rw-r--r--   0        0        0    24204 2021-11-19 17:12:25.934251 saw-client-0.9.0/saw_client/crucible.py
--rw-r--r--   0        0        0    10102 2021-11-19 17:12:25.934545 saw-client-0.9.0/saw_client/dashboard.py
--rw-r--r--   0        0        0     3076 2021-11-19 17:12:25.934759 saw-client-0.9.0/saw_client/exceptions.py
--rw-r--r--   0        0        0      112 2021-11-19 17:12:25.934933 saw-client-0.9.0/saw_client/jvm.py
--rw-r--r--   0        0        0     1955 2021-11-19 17:12:25.935118 saw-client-0.9.0/saw_client/jvm_type.py
--rw-r--r--   0        0        0     1387 2021-11-19 17:12:25.935293 saw-client-0.9.0/saw_client/llvm.py
--rw-r--r--   0        0        0     1736 2021-11-19 17:12:25.935606 saw-client-0.9.0/saw_client/llvm_type.py
--rw-r--r--   0        0        0     3303 2021-11-19 17:12:25.935806 saw-client-0.9.0/saw_client/proofscript.py
--rw-r--r--   0        0        0        0 2021-11-19 17:12:25.935903 saw-client-0.9.0/saw_client/py.typed
--rw-r--r--   0        0        0      855 2021-11-19 17:12:25.936123 saw-client-0.9.0/saw_client/utils.py
--rw-r--r--   0        0        0     8287 2021-11-19 23:58:54.057618 saw-client-0.9.0/setup.py
--rw-r--r--   0        0        0     7976 2021-11-19 23:58:54.058270 saw-client-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     7375 2022-03-17 13:59:21.541995 saw_client-1.0.0/README.md
+-rw-r--r--   0        0        0      353 2023-03-10 19:55:21.873409 saw_client-1.0.0/mypy.ini
+-rw-r--r--   0        0        0      584 2023-06-27 14:10:08.700038 saw_client-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    25016 2022-05-17 16:50:26.153303 saw_client-1.0.0/saw_client/__init__.py
+-rw-r--r--   0        0        0    10225 2023-03-10 19:55:17.485354 saw_client-1.0.0/saw_client/commands.py
+-rw-r--r--   0        0        0    12668 2023-03-10 19:55:17.485354 saw_client-1.0.0/saw_client/connection.py
+-rw-r--r--   0        0        0    28795 2022-03-17 13:59:21.541995 saw_client-1.0.0/saw_client/crucible.py
+-rw-r--r--   0        0        0    10102 2022-03-17 13:59:21.541995 saw_client-1.0.0/saw_client/dashboard.py
+-rw-r--r--   0        0        0     3152 2023-03-10 19:55:17.485354 saw_client-1.0.0/saw_client/exceptions.py
+-rw-r--r--   0        0        0      112 2022-03-17 13:59:21.541995 saw_client-1.0.0/saw_client/jvm.py
+-rw-r--r--   0        0        0     1955 2022-03-17 13:59:21.541995 saw_client-1.0.0/saw_client/jvm_type.py
+-rw-r--r--   0        0        0     1387 2022-03-17 13:59:21.541995 saw_client-1.0.0/saw_client/llvm.py
+-rw-r--r--   0        0        0     1736 2022-03-17 13:59:21.545995 saw_client-1.0.0/saw_client/llvm_type.py
+-rw-r--r--   0        0        0      976 2022-03-17 13:59:21.545995 saw_client-1.0.0/saw_client/option.py
+-rw-r--r--   0        0        0     3619 2023-04-03 14:01:02.767699 saw_client-1.0.0/saw_client/proofscript.py
+-rw-r--r--   0        0        0        0 2022-03-17 13:59:21.545995 saw_client-1.0.0/saw_client/py.typed
+-rw-r--r--   0        0        0      855 2022-03-17 13:59:21.545995 saw_client-1.0.0/saw_client/utils.py
+-rw-r--r--   0        0        0     8071 1970-01-01 00:00:00.000000 saw_client-1.0.0/PKG-INFO
```

### Comparing `saw-client-0.9.0/README.md` & `saw_client-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `saw-client-0.9.0/pyproject.toml` & `saw_client-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "saw-client"
-version = "0.9.0"
+version = "1.0.0"
 readme = "README.md"
 description = "SAW client for the SAW 0.9 RPC server"
 authors = ["Galois, Inc. <saw@galois.com>"]
 license = "BSD License"
 include = [
     "LICENSE",
     "mypy.ini",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.25.1"
 BitVector = "^3.4.9"
-cryptol = "2.12.0" # { path = "../../deps/cryptol/cryptol-remote-api/python/", develop = true }
-argo-client = "~0.0.6"
+cryptol = "3.0.0" # { path = "../../deps/cryptol/cryptol-remote-api/python/", develop = true }
+argo-client = "0.0.11"
 
 [tool.poetry.dev-dependencies]
-mypy = "^0.812"
+mypy = "^0.991"
 
 [build-system]
-requires = ["poetry>=1.1.4", "setuptools>=40.8.0"]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `saw-client-0.9.0/saw_client/__init__.py` & `saw_client-1.0.0/saw_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import cryptol
 
 from cryptol import cryptoltypes
 from . import connection
 from argo_client.connection import ServerConnection
 from . import llvm
 from . import exceptions
+from . import option
 from . import proofscript
 
 __designated_connection = None  # type: Optional[connection.SAWConnection]
 __designated_views = []         # type: List[View]
 __global_success = True         # type: bool
 
 # Script-execution-global set of all results verified so far
@@ -353,15 +354,15 @@
             print(f'✅  The goal was verified!', file=self.file)
         else:
             print(f'✅  All {successes!r} goals verified!', file=self.file)
 
     def on_abort(self) -> None:
         print("🛑  Aborting proof script.", file=self.file)
 
-        
+
 def view(v: View) -> None:
     """Add a view to the global list of views. Future verification results will
        be handed to this view, and its on_finish() handler will be called at
        the end of the script."""
     global __designated_views
     __designated_views.append(v)
 
@@ -628,28 +629,53 @@
           proof_script: proofscript.ProofScript) -> ProofResult:
     """Atempts to prove that the expression given as the first argument, `goal`, is
     true for all possible values of free symbolic variables. Uses the proof
     script (potentially specifying an automated prover) provided by the second
     argument.
     """
     conn = __get_designated_connection()
-    res = conn.prove(cryptoltypes.to_cryptol(goal),
-                     proof_script.to_json()).result()
+    res = conn.prove(goal, proof_script.to_json()).result()
     pr = ProofResult()
     if res['status'] == 'valid':
         pr.valid = True
     elif res['status'] == 'invalid':
         pr.valid = False
     else:
         raise ValueError("Unknown proof result " + str(res))
     if 'counterexample' in res:
         pr.counterexample = [ (arg['name'], cryptol.from_cryptol_arg(arg['value']))
                               for arg in res['counterexample'] ]
     else:
         pr.counterexample = None
     return pr
 
+def eval_int(expr: cryptoltypes.CryptolJSON) -> int:
+    """Atempts to evaluate the given expression as a concrete integer.
+    """
+    conn = __get_designated_connection()
+    res = conn.eval_int(expr).result()
+    v = res['value']
+    if not isinstance(v, int):
+        raise ValueError(str(v) + " is not an integer")
+    return v
+
+def eval_bool(expr: cryptoltypes.CryptolJSON) -> bool:
+    """Atempts to evaluate the given expression as a concrete boolean.
+    """
+    conn = __get_designated_connection()
+    res = conn.eval_bool(expr).result()
+    v = res['value']
+    if not isinstance(v, bool):
+        raise ValueError(str(v) + " is not a boolean")
+    return v
+
+def set_option(option : option.SAWOption, value : bool) -> None:
+    """Set a boolean-valued SAW option."""
+    global __designated_connection
+    if __designated_connection is not None:
+        __designated_connection.set_option(option=option,value=value)
+
 @atexit.register
 def script_exit() -> None:
     global __designated_views
     for view in __designated_views:
         view.on_finish()
```

### Comparing `saw-client-0.9.0/saw_client/commands.py` & `saw_client-1.0.0/saw_client/commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,102 @@
 import argo_client.interaction as argo
 from typing import Any, Dict, List, Optional, Set, Union, overload
 
 from cryptol import cryptoltypes
 from . import exceptions
 from .proofscript import *
+from .option import *
 
 from typing import Any, List
 
 class SAWCommand(argo.Command):
     def process_error(self, ae : argo.ArgoException) -> Exception:
         return exceptions.make_saw_exception(ae)
 
+class YosysImport(SAWCommand):
+    def __init__(self,
+                 connection : argo.HasProtocolState,
+                 name : str,
+                 path : str,
+                 timeout : Optional[float]) -> None:
+        super(YosysImport, self).__init__(
+            'SAW/Yosys/import',
+            {'name': name, 'path': path},
+            connection,
+            timeout=timeout
+        )
+
+    def process_result(self, res : Any) -> Any:
+        return res
+
+class YosysVerify(SAWCommand):
+    def __init__(
+            self,
+            connection : argo.HasProtocolState,
+            imp: str,
+            module : str,
+            preconds: List[str],
+            spec : str,
+            lemmas : List[str],
+            script : ProofScript,
+            lemma_name : str,
+            timeout : Optional[float]) -> None:
+        params = {
+            'import': imp,
+            'module': module,
+            'preconds': preconds,
+            'spec': spec,
+            'lemmas': lemmas,
+            'script': script,
+            'lemma name': lemma_name
+        }
+        super(YosysVerify, self).__init__(
+            'SAW/Yosys/verify',
+            params,
+            connection,
+            timeout=timeout
+        )
+
+    def process_result(self, res : Any) -> Any:
+        return res
+
+class YosysImportSequential(SAWCommand):
+    def __init__(self,
+                 connection : argo.HasProtocolState,
+                 name : str,
+                 path : str,
+                 module : str,
+                 timeout : Optional[float]) -> None:
+        super(YosysImportSequential, self).__init__(
+            'SAW/Yosys/import sequential',
+            {'name': name, 'path': path, 'module': module},
+            connection,
+            timeout=timeout
+        )
+
+    def process_result(self, res : Any) -> Any:
+        return res
+
+class YosysExtractSequential(SAWCommand):
+    def __init__(self,
+                 connection : argo.HasProtocolState,
+                 name : str,
+                 module : str,
+                 cycles : int,
+                 timeout : Optional[float]) -> None:
+        super(YosysExtractSequential, self).__init__(
+            'SAW/Yosys/extract sequential',
+            {'name': name, 'cycles': cycles, 'module': module},
+            connection,
+            timeout=timeout
+        )
+
+    def process_result(self, res : Any) -> Any:
+        return res
+
 class CryptolLoadFile(SAWCommand):
     def __init__(self, connection : argo.HasProtocolState,
                  filename : str,
                  timeout : Optional[float]) -> None:
         super(CryptolLoadFile, self).__init__(
             'SAW/Cryptol/load file',
             {'file': filename},
@@ -172,21 +254,45 @@
 class Prove(SAWCommand):
     def __init__(
             self,
             connection : argo.HasProtocolState,
             goal : cryptoltypes.CryptolJSON,
             script : ProofScript,
             timeout : Optional[float]) -> None:
-        params = {'goal': goal,
+        params = {'goal': cryptoltypes.to_cryptol(goal),
                   'script': script}
         super(Prove, self).__init__('SAW/prove', params, connection, timeout=timeout)
 
     def process_result(self, res : Any) -> Any:
         return res
 
+class EvalInt(SAWCommand):
+    def __init__(
+            self,
+            connection : argo.HasProtocolState,
+            expr : cryptoltypes.CryptolJSON,
+            timeout : Optional[float]) -> None:
+        params = {'expr': cryptoltypes.to_cryptol(expr)}
+        super(EvalInt, self).__init__('SAW/eval int', params, connection, timeout=timeout)
+
+    def process_result(self, res : Any) -> Any:
+        return res
+
+class EvalBool(SAWCommand):
+    def __init__(
+            self,
+            connection : argo.HasProtocolState,
+            expr : cryptoltypes.CryptolJSON,
+            timeout : Optional[float]) -> None:
+        params = {'expr': cryptoltypes.to_cryptol(expr)}
+        super(EvalBool, self).__init__('SAW/eval bool', params, connection, timeout=timeout)
+
+    def process_result(self, res : Any) -> Any:
+        return res
+
 class SAWReset(argo.Notification):
     def __init__(self, connection : argo.HasProtocolState) -> None:
         super(SAWReset, self).__init__(
             'SAW/clear state',
             {'state to clear': connection.protocol_state()},
             connection
         )
@@ -195,7 +301,19 @@
 class SAWResetServer(argo.Notification):
     def __init__(self, connection : argo.HasProtocolState) -> None:
         super(SAWResetServer, self).__init__(
             'SAW/clear all states',
             {},
             connection
         )
+
+
+class SAWSetOption(SAWCommand):
+    def __init__(self, connection : argo.HasProtocolState,
+                 option : SAWOption, value : bool,
+                 timeout : Optional[float]) -> None:
+        params = {'option': str(option),
+                  'value': value}
+        super(SAWSetOption, self).__init__('SAW/set option', params, connection, timeout=timeout)
+
+    def process_result(self, _res : Any) -> Any:
+        return None
```

### Comparing `saw-client-0.9.0/saw_client/connection.py` & `saw_client-1.0.0/saw_client/connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import signal
 import sys
 from distutils.spawn import find_executable
 from argo_client.connection import ServerConnection, DynamicSocketProcess, HttpProcess, ManagedProcess
 from argo_client.interaction import Interaction, Command
 from .commands import *
+from .option import *
 from typing import Optional, Union, Any, List, TextIO
 
 # FIXME cryptol_path isn't always used...?
 def connect(command: Union[str, ServerConnection, None] = None,
             *,
             cryptol_path: Optional[str] = None,
             persist: bool = False,
@@ -224,16 +225,67 @@
         and use of this command is associated with the top-level `llvm_assume`
         function.
         """
         self.most_recent_result = \
             LLVMAssume(self, module, function, contract, lemma_name, timeout)
         return self.most_recent_result
 
+    def yosys_import(self, name: str, path: str, timeout : Optional[float] = None) -> Command:
+        self.most_recent_result = YosysImport(self, name, path, timeout)
+        return self.most_recent_result
+
+    def yosys_verify(self,
+                     imp: str,
+                     module: str,
+                     preconds: List[str],
+                     spec: str,
+                     lemmas: List[str],
+                     script: ProofScript,
+                     lemma_name: str,
+                     timeout : Optional[float] = None) -> Command:
+        self.most_recent_result = \
+            YosysVerify(self, imp, module, preconds, spec, lemmas, script, lemma_name, timeout)
+        return self.most_recent_result
+
+    def yosys_import_sequential(self, name: str, path: str, module: str, timeout : Optional[float] = None) -> Command:
+        self.most_recent_result = YosysImportSequential(self, name, path, module, timeout)
+        return self.most_recent_result
+
+    def yosys_extract_sequential(self, name: str, module: str, cycles: int, timeout : Optional[float] = None) -> Command:
+        self.most_recent_result = YosysExtractSequential(self, name, module, cycles, timeout)
+        return self.most_recent_result
+
     def prove(self,
               goal: cryptoltypes.CryptolJSON,
               proof_script: ProofScript,
               timeout : Optional[float] = None) -> Command:
         """Create an instance of the `Prove` command. Documentation on the purpose and
         use of this command is associated with the top-level `prove` function.
         """
         self.most_recent_result = Prove(self, goal, proof_script, timeout)
         return self.most_recent_result
+
+    def eval_int(self,
+              expr: cryptoltypes.CryptolJSON,
+              timeout : Optional[float] = None) -> Command:
+        """Create an instance of the `EvalInt` command. Documentation on the purpose and
+        use of this command is associated with the top-level `eval_int` function.
+        """
+        self.most_recent_result = EvalInt(self, expr, timeout)
+        return self.most_recent_result
+
+    def eval_bool(self,
+              expr: cryptoltypes.CryptolJSON,
+              timeout : Optional[float] = None) -> Command:
+        """Create an instance of the `EvalBool` command. Documentation on the purpose and
+        use of this command is associated with the top-level `eval_bool` function.
+        """
+        self.most_recent_result = EvalBool(self, expr, timeout)
+        return self.most_recent_result
+
+    def set_option(self,
+                   option : SAWOption,
+                   value : bool,
+                   timeout : Optional[float] = None) -> Command:
+        """Set a boolean-valued SAW option."""
+        self.most_recent_result = SAWSetOption(self, option, value, timeout)
+        return self.most_recent_result
```

### Comparing `saw-client-0.9.0/saw_client/crucible.py` & `saw_client-1.0.0/saw_client/crucible.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from abc import ABCMeta, abstractmethod
 from cryptol import cryptoltypes
+from cryptol.quoting import to_cryptol_str_customf
 from .utils import deprecated
 from dataclasses import dataclass
 import dataclasses
 import re
-from typing import Any, Dict, List, Optional, Set, Union, overload
+from typing import Any, Dict, List, Tuple, Optional, Set, Union, overload
 from typing_extensions import Literal
 import inspect
 import uuid
 
 from .llvm_type import *
 from .jvm_type import *
 
+JSON = Union[None, bool, int, float, str, Dict, Tuple, List]
+
 class SetupVal(metaclass=ABCMeta):
     """Represent a ``SetupValue`` in SawScript, which "corresponds to
     values that can occur during symbolic execution, which includes both 'Term'
     values, pointers, and composite types consisting of either of these
     (both structures and arrays)."
     """
     @abstractmethod
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         """JSON representation for this ``SetupVal`` (i.e., how it is represented in expressions, etc).
 
         N.B., should be a JSON object with a ``'setup value'`` field with a unique tag which the
         server will dispatch on to then interpret the rest of the JSON object.``"""
         pass
 
     @overload
@@ -46,15 +49,15 @@
             raise ValueError(f'{key!r} is not a valid element index or field name.')
 
 
 class NamedSetupVal(SetupVal):
     """Represents those ``SetupVal``s which are a named reference to some value, e.e., a variable
     or reference to allocated memory."""
     @abstractmethod
-    def to_init_json(self) -> Any:
+    def to_init_json(self) -> JSON:
         """JSON representation with the information for those ``SetupVal``s which require additional
         information to initialize/allocate them vs that which is required later to reference them.
 
         I.e., ``.to_json()`` will be used to refer to such ``SetupVal``s in expressions, and
         ``.to_init_json() is used to initialize/allocate them.``
         """
         pass
@@ -65,150 +68,144 @@
     def __init__(self, code : Union[str, cryptoltypes.CryptolJSON]):
         if isinstance(code, str):
             self.expression = cryptoltypes.CryptolLiteral(code)
         else:
             self.expression = code
 
     def __call__(self, *args : cryptoltypes.CryptolJSON) -> 'CryptolTerm':
-        out_term = self.expression
-        for a in args:
-            out_term = cryptoltypes.CryptolApplication(out_term, a)
-
-        return CryptolTerm(out_term)
+        return CryptolTerm(cryptoltypes.CryptolApplication(self.expression, *args))
 
     def __repr__(self) -> str:
         return f"CryptolTerm({self.expression!r})"
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {'setup value': 'Cryptol', 'expression': cryptoltypes.to_cryptol(self.expression)}
 
-    def __to_cryptol__(self, ty : Any) -> Any:
-        return self.expression.__to_cryptol__(ty)
+    def __to_cryptol__(self) -> cryptoltypes.JSON:
+        return self.expression.__to_cryptol__()
+
+    def __to_cryptol_str__(self) -> str:
+        return self.expression.__to_cryptol_str__()
 
 class FreshVar(NamedSetupVal):
     __name : Optional[str]
 
     def __init__(self, spec : 'Contract', type : Union['LLVMType', 'JVMType'], suggested_name : Optional[str] = None) -> None:
         self.__name = suggested_name
         self.spec = spec
         self.type = type
 
-    def __to_cryptol__(self, ty : Any) -> Any:
-        return cryptoltypes.CryptolLiteral(self.name()).__to_cryptol__(ty)
+    def __to_cryptol__(self) -> cryptoltypes.JSON:
+        return cryptoltypes.CryptolLiteral(self.name()).__to_cryptol__()
+
+    def __to_cryptol_str__(self) -> str:
+        return cryptoltypes.CryptolLiteral(self.name()).__to_cryptol_str__()
 
-    def to_init_json(self) -> Any:
+    def to_init_json(self) -> JSON:
         #FIXME it seems we don't actually use two names ever... just the one...do we actually need both?
         name = self.name()
         return {"server name": name,
                 "name": name,
                 "type": self.type.to_json()}
 
     def name(self) -> str:
         if self.__name is None:
             self.__name = self.spec.get_fresh_name()
         return self.__name
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {'setup value': 'named', 'name': self.name()}
 
-    def __gt__(self, other : cryptoltypes.CryptolJSON) -> CryptolTerm:
-        gt = CryptolTerm("(>)")
-        return gt(self, other)
-
-    def __lt__(self, other : cryptoltypes.CryptolJSON) -> CryptolTerm:
-        lt = CryptolTerm("(<)")
-        return lt(self, other)
-
 
 class Allocated(NamedSetupVal):
     name : Optional[str]
 
     def __init__(self, spec : 'Contract', type : Union['LLVMType','JVMType'], *,
                  mutable : bool = True, alignment : Optional[int] = None) -> None:
         self.name = None
         self.spec = spec
         self.type = type
         self.mutable = mutable
         self.alignment = alignment
 
-    def to_init_json(self) -> Any:
+    def to_init_json(self) -> JSON:
         if self.name is None:
             self.name = self.spec.get_fresh_name()
         return {"server name": self.name,
                 "type": self.type.to_json(),
                 "mutable": self.mutable,
                 "alignment": self.alignment}
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         if self.name is None:
             self.name = self.spec.get_fresh_name()
         return {'setup value': 'named', 'name': self.name}
 
 class StructVal(SetupVal):
     fields : List[SetupVal]
 
     def __init__(self, fields : List[SetupVal]) -> None:
         self.fields = fields
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {'setup value': 'tuple', 'elements': [fld.to_json() for fld in self.fields]}
 
 class ElemVal(SetupVal):
     base : SetupVal
     index : int
 
     def __init__(self, base : SetupVal, index : int) -> None:
         self.base = base
         self.index = index
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {'setup value': 'element lvalue',
                 'base': self.base.to_json(), 'index': self.index}
 
 class FieldVal(SetupVal):
     base : SetupVal
     field_name : str
 
     def __init__(self, base : SetupVal, field_name : str) -> None:
         self.base = base
         self.field_name = field_name
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {'setup value': 'field',
                 'base': self.base.to_json(), 'field': self.field_name}
 
 class GlobalInitializerVal(SetupVal):
     name : str
 
     def __init__(self, name : str) -> None:
         self.name = name
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {'setup value': 'global initializer', 'name': self.name}
 
 class GlobalVarVal(SetupVal):
     name : str
 
     def __init__(self, name : str) -> None:
         self.name = name
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {'setup value': 'global lvalue', 'name': self.name}
 
 class NullVal(SetupVal):
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {'setup value': 'null'}
 
 class ArrayVal(SetupVal):
     elements : List[SetupVal]
 
     def __init__(self, elements : List[SetupVal]) -> None:
         self.elements = elements
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {'setup value': 'array',
                 'elements': [element.to_json() for element in self.elements]}
 
 name_regexp = re.compile('^(?P<prefix>.*[^0-9])?(?P<number>[0-9]+)?$')
 
 def next_name(x : str) -> str:
     match = name_regexp.match(x)
@@ -238,85 +235,103 @@
     pass
 
 
 class Condition:
     def __init__(self, condition : CryptolTerm) -> None:
         self.cryptol_term = condition
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return cryptoltypes.to_cryptol(self.cryptol_term)
 
 
 class PointsTo:
     """The workhorse for ``points_to``.
     """
     def __init__(self, pointer : SetupVal, target : SetupVal, *,
                  check_target_type : Union[PointerType, 'LLVMType', 'JVMType', None] = PointerType(),
                  condition : Optional[Condition] = None) -> None:
         self.pointer = pointer
         self.target = target
         self.check_target_type = check_target_type
         self.condition = condition
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         check_target_type_json: Optional[Dict[str, Any]]
         if self.check_target_type is None:
             check_target_type_json = None
         elif isinstance(self.check_target_type, PointerType):
             check_target_type_json = { "check against": "pointer type" }
         elif isinstance(self.check_target_type, LLVMType):
             check_target_type_json = { "check against": "casted type"
                                      , "type": self.check_target_type.to_json() }
         return {"pointer": self.pointer.to_json(),
                 "points to": self.target.to_json(),
                 "check points to type": check_target_type_json,
                 "condition": self.condition.to_json() if self.condition is not None else self.condition}
 
+
+class PointsToBitfield:
+    """The workhorse for ``points_to_bitfield``.
+    """
+    def __init__(self, pointer : SetupVal, field_name : str,
+                 target : SetupVal) -> None:
+        self.pointer = pointer
+        self.field_name = field_name
+        self.target = target
+
+    def to_json(self) -> Any:
+        return {"pointer": self.pointer.to_json(),
+                "field name": self.field_name,
+                "points to": self.target.to_json()}
+
+
 @dataclass
 class GhostVariable:
     name: str
     server_name: str
 
 class GhostValue:
     """A class containing the statement that a given ghost variable should have the
     value given by a Cryptol expression.
     """
-    def __init__(self, name: str, value: CryptolTerm) -> None:
+    def __init__(self, name: str, value: cryptoltypes.CryptolJSON) -> None:
         self.name = name
         self.value = value
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {"server name": self.name,
                 "value": cryptoltypes.to_cryptol(self.value)}
 
 @dataclass
 class State:
     contract : 'Contract'
     fresh : List[FreshVar] = dataclasses.field(default_factory=list)
     conditions : List[Condition] = dataclasses.field(default_factory=list)
     allocated : List[Allocated] = dataclasses.field(default_factory=list)
     points_to : List[PointsTo] = dataclasses.field(default_factory=list)
+    points_to_bitfield : List[PointsToBitfield] = dataclasses.field(default_factory=list)
     ghost_values : List[GhostValue] = dataclasses.field(default_factory=list)
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return {'variables': [v.to_init_json() for v in self.fresh],
                 'conditions': [c.to_json() for c in self.conditions],
                 'allocated': [a.to_init_json() for a in self.allocated],
                 'points to': [p.to_json() for p in self.points_to],
+                'points to bitfield': [p.to_json() for p in self.points_to_bitfield],
                 'ghost values': [g.to_json() for g in self.ghost_values]
                }
 
 ContractState = \
   Union[Literal['pre'],
         Literal['post'],
         Literal['done']]
 
 @dataclass
 class Void:
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         return None
 
 void = Void()
 
 @dataclass
 class VerifyResult:
     contract : 'Contract'
@@ -340,15 +355,15 @@
     __returns : Optional[Union[SetupVal, Void]]
 
     __arguments : Optional[List[SetupVal]]
 
     __definition_lineno : Optional[int]
     __definition_filename : Optional[str]
     __unique_id : uuid.UUID
-    __cached_json : Optional[Any]
+    __cached_json : JSON
 
     def __init__(self) -> None:
         self.__pre_state = State(self)
         self.__post_state = State(self)
         self.__used_names = set()
         self.__arguments = None
         self.__returns = None
@@ -443,15 +458,32 @@
         if self.__state == 'pre':
             self.__pre_state.points_to.append(pt)
         elif self.__state == 'post':
             self.__post_state.points_to.append(pt)
         else:
             raise Exception("wrong state")
 
-    def ghost_value(self, var: GhostVariable, value: CryptolTerm) -> None:
+    def points_to_bitfield(self, pointer : SetupVal, field_name : str,
+                           target : SetupVal) -> None:
+        """Declare that the memory location indicated by the ``pointer``
+        is a bitfield whose field, indicated by the ``field_name``,
+        contains the ``target``.
+
+        Currently, this function only supports LLVM verification. Attempting to
+        use this function for JVM verification will result in an error.
+        """
+        pt = PointsToBitfield(pointer, field_name, target)
+        if self.__state == 'pre':
+            self.__pre_state.points_to_bitfield.append(pt)
+        elif self.__state == 'post':
+            self.__post_state.points_to_bitfield.append(pt)
+        else:
+            raise Exception("wrong state")
+
+    def ghost_value(self, var: GhostVariable, value: cryptoltypes.CryptolJSON) -> None:
         """Declare that the given ghost variable should have a value specified by the given Cryptol expression.
 
         Usable either before or after `execute_func`.
         """
         gv = GhostValue(var.name, value)
         if self.__state == 'pre':
             self.__pre_state.ghost_values.append(gv)
@@ -485,37 +517,55 @@
         else:
             condition = Condition(proposition)
         if self.__state == 'pre':
             self.__pre_state.conditions.append(condition)
         else:
             raise Exception("preconditions must be specified before execute_func is called in the contract")
 
+    def precondition_f(self, s : str) -> None:
+        """Declares a precondition using a ``cry_f``-style format string, i.e.
+        ``precondition_f(...)`` is equivalent to ``precondition(cry_f(...))``"""
+        expression = to_cryptol_str_customf(s, frames=1, filename="<precondition_f>")
+        return self.precondition(expression)
+
     def postcondition(self, proposition : Union[str, CryptolTerm, cryptoltypes.CryptolJSON]) -> None:
         """Establishes ``proposition`` as a postcondition for the function ```Contract```
         being specified.
 
         Postconditions must be specified after ``execute_func`` is called in the contract specification."""
         if not isinstance(proposition, CryptolTerm):
             condition = Condition(CryptolTerm(proposition))
         else:
             condition = Condition(proposition)
         if self.__state == 'post':
             self.__post_state.conditions.append(condition)
         else:
             raise Exception("postconditions must be specified after execute_func is called in the contract")
 
+    def postcondition_f(self, s : str) -> None:
+        """Declares a postcondition using a ``cry_f``-style format string, i.e.
+        ``postcondition_f(...)`` is equivalent to ``postcondition(cry_f(...))``"""
+        expression = to_cryptol_str_customf(s, frames=1, filename="<postcondition_f>")
+        return self.postcondition(expression)
+
     def returns(self, val : Union[Void,SetupVal]) -> None:
         if self.__state == 'post':
             if self.__returns is None:
                 self.__returns = val
             else:
                 raise ValueError("Return value already specified")
         else:
             raise ValueError("Not in postcondition")
 
+    def returns_f(self, s : str) -> None:
+        """Declares a return value using a ``cry_f``-style format string, i.e.
+        ``returns_f(...)`` is equivalent to ``returns(cry_f(...))``"""
+        expression = to_cryptol_str_customf(s, frames=1, filename="<returns_f>")
+        return self.returns(CryptolTerm(expression))
+
     def lemma_name(self, hint  : Optional[str] = None) -> str:
         if hint is None:
             hint = self.__class__.__name__
 
         name = uniquify('lemma_' + hint, used_lemma_names)
 
         used_lemma_names.add(name)
@@ -524,15 +574,15 @@
 
     def definition_lineno(self) -> Optional[int]:
         return self.__definition_lineno
 
     def definition_filename(self) -> Optional[str]:
         return self.__definition_filename
 
-    def to_json(self) -> Any:
+    def to_json(self) -> JSON:
         if self.__cached_json is not None:
             return self.__cached_json
         else:
             if self.__state != 'pre':
                 raise Exception(f'Internal error: wrong contract state -- expected \'pre\', but got: {self.__state!r}')
 
             self.specification()
@@ -547,40 +597,79 @@
 
             self.__cached_json = \
                 {'pre vars': [v.to_init_json() for v in self.__pre_state.fresh],
                  'pre conds': [c.to_json() for c in self.__pre_state.conditions],
                  'pre allocated': [a.to_init_json() for a in self.__pre_state.allocated],
                  'pre ghost values': [g.to_json() for g in self.__pre_state.ghost_values],
                  'pre points tos': [pt.to_json() for pt in self.__pre_state.points_to],
+                 'pre points to bitfields': [pt.to_json() for pt in self.__pre_state.points_to_bitfield],
                  'argument vals': [a.to_json() for a in self.__arguments] if self.__arguments is not None else [],
                  'post vars': [v.to_init_json() for v in self.__post_state.fresh],
                  'post conds': [c.to_json() for c in self.__post_state.conditions],
                  'post allocated': [a.to_init_json() for a in self.__post_state.allocated],
                  'post ghost values': [g.to_json() for g in self.__post_state.ghost_values],
                  'post points tos': [pt.to_json() for pt in self.__post_state.points_to],
+                 'post points to bitfields': [pt.to_json() for pt in self.__post_state.points_to_bitfield],
                  'return val': self.__returns.to_json()}
 
             return self.__cached_json
 
 ##################################################
 # Helpers for value construction
 ##################################################
 
 # It's tempting to name this `global` to mirror SAWScript's `llvm_global`,
 # but that would clash with the Python keyword `global`.
 def global_var(name: str) -> SetupVal:
     """Returns a pointer to the named global ``name`` (i.e., a ``GlobalVarVal``)."""
     return GlobalVarVal(name)
 
-# FIXME Is `Any` too permissive here -- can we be a little more precise?
-def cryptol(data : Any) -> 'CryptolTerm':
-    """Constructs a Cryptol value from ``data`` (i.e., a ``CryptolTerm``, which is also a ``SetupVal``).
-
-    ``data`` should be a string literal representing Cryptol syntax or the result of a Cryptol-realted server computation."""
-    return CryptolTerm(data)
+def cry(s : str) -> CryptolTerm:
+    """Embed a string of Cryptol syntax as a ``CryptolTerm`` (which is also a
+       ``SetupVal``) - also see ``cry_f``."""
+    return CryptolTerm(s)
+
+def cry_f(s : str) -> CryptolTerm:
+    """Embed a string of Cryptol syntax as a ``CryptolTerm`` (which is also a
+       ``SetupVal``), where the given string is parsed as an f-string, and the
+       values within brackets are converted to Cryptol syntax using
+       ``to_cryptol_str`` from the Cryptol Python library.
+
+       Like f-strings, values in brackets (``{``, ``}``) are parsed as python
+       expressions in the caller's context of local and global variables, and
+       to include a literal bracket in the final string, it must be doubled
+       (i.e. ``{{`` or ``}}``). The latter is needed when using explicit type
+       application or record syntax. For example, if ``x = [0,1]`` then
+       ``cry_f('length `{{2}} {x}')`` is equal to ``cry('length `{2} [0,1]')``
+       and ``cry_f('{{ x = {x} }}')`` is equal to ``cry('{ x = [0,1] }')``.
+
+       When formatting Cryptol, it is recomended to use this function rather
+       than any of Python's built-in methods of string formatting (e.g.
+       f-strings, ``str.format``) as the latter will not always produce valid
+       Cryptol syntax. Specifically, this function differs from these methods
+       in the cases of ``BV``s, string literals, function application (this
+       function will add parentheses as needed), and dicts. For example,
+       ``cry_f('{ {"x": 5, "y": 4} }')`` equals ``cry('{x = 5, y = 4}')``
+       but ``f'{ {"x": 5, "y": 4} }'`` equals ``'{"x": 5, "y": 4}'``. Only
+       the former is valid Cryptol syntax for a record.
+       
+       Note that any conversion or format specifier will always result in the
+       argument being rendered as a Cryptol string literal with the conversion
+       and/or formating applied. For example, `cry('f {5}')` is equal to
+       ``cry('f 5')`` but ``cry_f('f {5!s}')`` is equal to ``cry(`f "5"`)``
+       and ``cry_f('f {5:+.2%}')`` is equal to ``cry('f "+500.00%"')``.
+
+       :example:
+
+       >>> x = BV(size=7, value=1)
+       >>> y = cry_f('fun1 {x}')
+       >>> cry_f('fun2 {y}')
+       'fun2 (fun1 (1 : [7]))'
+    """
+    return CryptolTerm(to_cryptol_str_customf(s, frames=1))
 
 def array(*elements: SetupVal) -> SetupVal:
     """Returns an array with the provided ``elements`` (i.e., an ``ArrayVal``).
 
     N.B., one or more ``elements`` must be provided.""" # FIXME why? document this here when we figure it out.
     if len(elements) == 0:
         raise ValueError('An array must be constructed with one or more elements')
```

### Comparing `saw-client-0.9.0/saw_client/dashboard.py` & `saw_client-1.0.0/saw_client/dashboard.py`

 * *Files identical despite different names*

### Comparing `saw-client-0.9.0/saw_client/exceptions.py` & `saw_client-1.0.0/saw_client/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 class NotAnLLVMSetupValue(ServerValueError): pass
 class NotAnLLVMMethodSpecification(ServerValueError): pass
 class NotAnLLVMMethodSpecIR(ServerValueError): pass
 class NotAJVMClass(ServerValueError): pass
 class NotAJVMMethodSpecIR(ServerValueError): pass
 class NotASimpset(ServerValueError): pass
 class NotATerm(ServerValueError): pass
+class NotAYosysTheorem(ServerValueError): pass
 
 # Setup errors:
 class SetupError(SAWException): pass
 class NotSettingUpCryptol(SetupError): pass
 class NotSettingUpCrucibleLLVM(SetupError): pass
 class NotAtTopLevel(SetupError): pass
 
@@ -81,14 +82,15 @@
     10040: NotAnLLVMSetupValue,
     10040: NotAnLLVMMethodSpecification,
     10050: NotAnLLVMMethodSpecIR,
     10060: NotASimpset,
     10070: NotATerm,
     10080: NotAJVMClass,
     10090: NotAJVMMethodSpecIR,
+    10130: NotAYosysTheorem,
     # Setup errors:
     10100: NotSettingUpCryptol,
     10110: NotSettingUpCrucibleLLVM,
     10120: NotAtTopLevel,
     # Loading errors:
     10200: CantLoadLLVMModule,
     # Verification errors:
```

### Comparing `saw-client-0.9.0/saw_client/jvm_type.py` & `saw_client-1.0.0/saw_client/jvm_type.py`

 * *Files identical despite different names*

### Comparing `saw-client-0.9.0/saw_client/llvm.py` & `saw_client-1.0.0/saw_client/llvm.py`

 * *Files identical despite different names*

### Comparing `saw-client-0.9.0/saw_client/llvm_type.py` & `saw_client-1.0.0/saw_client/llvm_type.py`

 * *Files identical despite different names*

### Comparing `saw-client-0.9.0/saw_client/proofscript.py` & `saw_client-1.0.0/saw_client/proofscript.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,26 +41,34 @@
   def to_json(self) -> Any:
     return { "name": self.name, "uninterpreted functions": self.unints }
 
 class CVC4(UnintProver):
   def __init__(self, unints : List[str]) -> None:
     super().__init__("w4-cvc4", unints)
 
+class CVC5(UnintProver):
+  def __init__(self, unints : List[str]) -> None:
+    super().__init__("w4-cvc5", unints)
+
 class Yices(UnintProver):
   def __init__(self, unints : List[str]) -> None:
     super().__init__("w4-yices", unints)
 
 class Z3(UnintProver):
   def __init__(self, unints : List[str]) -> None:
     super().__init__("w4-z3", unints)
 
 class CVC4_SBV(UnintProver):
   def __init__(self, unints : List[str]) -> None:
     super().__init__("sbv-cvc4", unints)
 
+class CVC5_SBV(UnintProver):
+  def __init__(self, unints : List[str]) -> None:
+    super().__init__("sbv-cvc5", unints)
+
 class Yices_SBV(UnintProver):
   def __init__(self, unints : List[str]) -> None:
     super().__init__("sbv-yices", unints)
 
 class Z3_SBV(UnintProver):
   def __init__(self, unints : List[str]) -> None:
     super().__init__("sbv-z3", unints)
@@ -117,12 +125,15 @@
 abc_verilog = UseProver(ABC_Verilog())
 rme = UseProver(RME())
 boolector = UseProver(Boolector())
 
 def cvc4(unints : List[str]) -> ProofTactic:
   return UseProver(CVC4(unints))
 
+def cvc5(unints : List[str]) -> ProofTactic:
+  return UseProver(CVC5(unints))
+
 def yices(unints : List[str]) -> ProofTactic:
   return UseProver(Yices(unints))
 
 def z3(unints : List[str]) -> ProofTactic:
   return UseProver(Z3(unints))
```

### Comparing `saw-client-0.9.0/saw_client/utils.py` & `saw_client-1.0.0/saw_client/utils.py`

 * *Files identical despite different names*

### Comparing `saw-client-0.9.0/setup.py` & `saw_client-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,222 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: saw-client
+Version: 1.0.0
+Summary: SAW client for the SAW 0.9 RPC server
+License: BSD License
+Author: Galois, Inc.
+Author-email: saw@galois.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: BitVector (>=3.4.9,<4.0.0)
+Requires-Dist: argo-client (==0.0.11)
+Requires-Dist: cryptol (==3.0.0)
+Requires-Dist: requests (>=2.25.1,<3.0.0)
+Description-Content-Type: text/markdown
+
+# SAW Python Client
+
+In-development Python client for SAW. Currently tested on Linux and MacOS -- at present there may be some minor issues running the Python Client in a Windows environment that needs addressed (e.g., some Python process management methods are not cross-OS-compatible).
+
+This SAW client depends on the [saw-remote-api](https://github.com/GaloisInc/saw-script/tree/master/saw-remote-api) server.
+
+# TL;DR Steps to running SAW Python scripts
+
+1. Clone the repo 
+```
+git clone https://github.com/GaloisInc/saw-script.git
+```
+2. Enter the repo
+```
+cd saw-script
+```
+3. Initialize git submodules 
+```
+git submodule update --init
+```
+4. Navigate to the python client
+```
+cd saw-remote-api/python
+```
+5. Install and setup some version of the `saw-remote-api` server and update any
+   relevant environment variables as needed (see `saw_client.connect()` documentation
+   for the various ways a server can be connected to).
+   E.g., here is how the docker image of the server might be used:
+```
+$ docker run --name=saw-remote-api -d \
+  -v $PWD/tests/saw/test-files:/home/saw/tests/saw/test-files \
+  -p 8080:8080 \
+  galoisinc/saw-remote-api:nightly
+$ export SAW_SERVER_URL="http://localhost:8080/"
+```
+6. Install the Python client (requires Python v3.8 or newer -- we recommend using [`poetry`](https://python-poetry.org/docs/#installation) to install the package):
+```
+$ poetry install 
+```
+7. Run tests or individual scripts:
+```
+$ poetry run python -m unittest discover tests/saw
+$ poetry run python tests/saw/test_salsa20.py
+```
+
+(We're aware the tests currently emit some `ResourceWarning`s regarding
+subprocesses when run via `unittest` even though they pass and successfully
+verify the goals. It's on our to-do list.)
+
+# Python Client Installation (via Poetry)
+
+First, clone the repository and submodules.
+
+```
+$ git clone https://github.com/GaloisInc/saw-script.git
+$ cd saw-script
+$ git submodule update --init
+```
+
+Then, use [`poetry`](https://python-poetry.org/docs/#installation) to install
+the python client from the `saw-remote-api/python` directory:
+
+```
+$ cd saw-remote-api/python
+$ poetry install
+```
+
+# SAW server
+
+To run the verification scripts a `saw-remote-api` server must be available,
+either as a local executable or running in docker image listening on a port.
+
+## Connecting with a server in a script
+
+Connecting to a server in a Python script is accomplished via the `saw_client.connect`
+method. Its accompanying Python doc strings describe the various ways it can be
+used. Below is a brief summary:
+
+`saw_client.connect()`, when provided no arguments, will attempt the following in order:
+
+1. If the environment variable ``SAW_SERVER`` is set and refers to an
+   executable, it is assumed to be a `saw-remote-api` executable and will be
+   used for the duration of the script.
+2. If the environment variable ``SAW_SERVER_URL`` is set, it is assumed to be
+   the URL for a running SAW server in ``http`` mode and will be connected to.
+   (N.B., this can be a local server or a server running in a docker image.)
+3. If an executable ``saw-remote-api`` is available on the ``PATH`` it is
+    assumed to be a SAW server and will be used for the duration of the script.
+
+Additional arguments and options are documented with the function.
+
+Notable, the `reset_server` keyword can be used to connect to a running server
+and reset it, ensuring states from previous scrips have been cleared. E.g.,
+`saw_client.connect(reset_server=True)`.
+
+
+## Acquiring a SAW Server
+
+There are several ways a server executable can be obtained.
+
+### Server executables
+
+An executable of the server is included in the SAW release/nightly tarballs.
+
+If using a SAW [release](https://github.com/GaloisInc/saw-script/releases), it
+is recommended to use `v0.8` or greater if possible. (`v0.7` _does_ include the
+server and may work for individual use cases, but running repeated scripts
+against the same persistent server will not work as intended.)
+
+Nightly server builds can be found as `Artifacts` of the [Nightly
+Builds](https://github.com/GaloisInc/saw-script/actions/workflows/nightly.yml)
+github action. I.e., go to the `Nightly Builds` Github Action, click on a
+successful build, scroll to the bottom and under `Artifacts` a Linux, Windows,
+and MacOS tarball will be listed. (Apologies... we need to make these easier to
+find...)
+
+### Server docker images
+
+Docker images for the SAW server are currently uploaded to
+[DockerHub](https://hub.docker.com/r/galoisinc/saw-remote-api).
+
+These images are set up to run as HTTP `saw-remote-api` servers, e.g.:
+
+```
+docker run --name=saw-remote-api -d \
+  -p 8080:8080 \
+  galoisinc/saw-remote-api:TAG
+```
+
+(where `TAG` is either `latest` or `nightly`) will launch a server listening at
+`http://localhost:8080/`. (As of March 2020, `nightly` is recommended, as the
+server in the last official release (i.e., the one accompanying SAW `v0.7`)
+contains some non-trivial bugs that greatly limit its utility.)
+
+The `-v` option to `docker run` can be used to load files into the docker
+server's working directory so they can be loaded into the server at the request
+of python scripts. E.g., `-v PATH_TO_FILES:/home/saw/files/` will upload the
+contents of the host machine's directory `PATH_TO_FILES` to the
+`/home/saw/files/` directory in the docker container, which corresponds to the
+relative path `files/` for the SAW server. (If desired, it can be useful to
+place files in a location in the Docker container such that the same relative
+paths in scripts refer to the same files in the host machine and docker
+container.)
+
+### Building from Source
+
+If this repository is checked out and the build directions are successfully run,
+`cabal v2-exec which saw-remote-api` should indicate where the server executable has
+been stored by `cabal`.
+
+Alternatively `cabal v2-install saw-remote-api` should install the server
+executable into the user's `~/.cabal/bin` directory (or similar), which (if
+configured properly) should then appear as `saw-remote-api` in a user's `PATH`.
+
+
+# Running Python SAW verification scripts
+
+Once the server is setup and any path variables are setup as desired, the
+Python (>= v3.8) client can be installed using
+[`poetry`](https://python-poetry.org/docs/#installation) as follows:
+
+```
+$ cd saw-remote-api/python
+$ poetry install
+```
+
+Then the tests or individual scripts can be run as follows:
+```
+$ poetry run python -m unittest discover tests/saw
+$ poetry run python tests/saw/test_salsa20.py
+```
+
+If leveraging environment variables is undesirable, the scripts themselves can
+specify a command to launch the server, e.g.:
+
+```
+saw_client.connect(COMMAND)
+```
+
+where `COMMAND` is a command to launch a new SAW server in socket mode.
+
+Or a server URL can be specified directly in the script, e.g.:
+
+```
+saw_client.connect(url=URL)
+```
+
+where `URL` is a URL for a running SAW server in HTTP mode.
+
+## Running Verification Scripts from a clean state
+
+To ensure any previous server state is cleared when running a SAW Python script
+against a persistent server (e.g., one running in HTTP mode in a different process),
+the `reset_server` keyword can be passed to `saw_client.connect()`. E.g.,
+
+```
+saw_client.connect(url="http://localhost:8080/", reset_server=True)
+```
 
-packages = \
-['saw_client']
+will connect to a SAW server running at `http://localhost:8080/` and will
+guarantee any previous state on the server is cleared.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['BitVector>=3.4.9,<4.0.0',
- 'argo-client>=0.0.6,<0.1.0',
- 'cryptol==2.12.0',
- 'requests>=2.25.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'saw-client',
-    'version': '0.9.0',
-    'description': 'SAW client for the SAW 0.9 RPC server',
-    'long_description': '# SAW Python Client\n\nIn-development Python client for SAW. Currently tested on Linux and MacOS -- at present there may be some minor issues running the Python Client in a Windows environment that needs addressed (e.g., some Python process management methods are not cross-OS-compatible).\n\nThis SAW client depends on the [saw-remote-api](https://github.com/GaloisInc/saw-script/tree/master/saw-remote-api) server.\n\n# TL;DR Steps to running SAW Python scripts\n\n1. Clone the repo \n```\ngit clone https://github.com/GaloisInc/saw-script.git\n```\n2. Enter the repo\n```\ncd saw-script\n```\n3. Initialize git submodules \n```\ngit submodule update --init\n```\n4. Navigate to the python client\n```\ncd saw-remote-api/python\n```\n5. Install and setup some version of the `saw-remote-api` server and update any\n   relevant environment variables as needed (see `saw_client.connect()` documentation\n   for the various ways a server can be connected to).\n   E.g., here is how the docker image of the server might be used:\n```\n$ docker run --name=saw-remote-api -d \\\n  -v $PWD/tests/saw/test-files:/home/saw/tests/saw/test-files \\\n  -p 8080:8080 \\\n  galoisinc/saw-remote-api:nightly\n$ export SAW_SERVER_URL="http://localhost:8080/"\n```\n6. Install the Python client (requires Python v3.8 or newer -- we recommend using [`poetry`](https://python-poetry.org/docs/#installation) to install the package):\n```\n$ poetry install \n```\n7. Run tests or individual scripts:\n```\n$ poetry run python -m unittest discover tests/saw\n$ poetry run python tests/saw/test_salsa20.py\n```\n\n(We\'re aware the tests currently emit some `ResourceWarning`s regarding\nsubprocesses when run via `unittest` even though they pass and successfully\nverify the goals. It\'s on our to-do list.)\n\n# Python Client Installation (via Poetry)\n\nFirst, clone the repository and submodules.\n\n```\n$ git clone https://github.com/GaloisInc/saw-script.git\n$ cd saw-script\n$ git submodule update --init\n```\n\nThen, use [`poetry`](https://python-poetry.org/docs/#installation) to install\nthe python client from the `saw-remote-api/python` directory:\n\n```\n$ cd saw-remote-api/python\n$ poetry install\n```\n\n# SAW server\n\nTo run the verification scripts a `saw-remote-api` server must be available,\neither as a local executable or running in docker image listening on a port.\n\n## Connecting with a server in a script\n\nConnecting to a server in a Python script is accomplished via the `saw_client.connect`\nmethod. Its accompanying Python doc strings describe the various ways it can be\nused. Below is a brief summary:\n\n`saw_client.connect()`, when provided no arguments, will attempt the following in order:\n\n1. If the environment variable ``SAW_SERVER`` is set and refers to an\n   executable, it is assumed to be a `saw-remote-api` executable and will be\n   used for the duration of the script.\n2. If the environment variable ``SAW_SERVER_URL`` is set, it is assumed to be\n   the URL for a running SAW server in ``http`` mode and will be connected to.\n   (N.B., this can be a local server or a server running in a docker image.)\n3. If an executable ``saw-remote-api`` is available on the ``PATH`` it is\n    assumed to be a SAW server and will be used for the duration of the script.\n\nAdditional arguments and options are documented with the function.\n\nNotable, the `reset_server` keyword can be used to connect to a running server\nand reset it, ensuring states from previous scrips have been cleared. E.g.,\n`saw_client.connect(reset_server=True)`.\n\n\n## Acquiring a SAW Server\n\nThere are several ways a server executable can be obtained.\n\n### Server executables\n\nAn executable of the server is included in the SAW release/nightly tarballs.\n\nIf using a SAW [release](https://github.com/GaloisInc/saw-script/releases), it\nis recommended to use `v0.8` or greater if possible. (`v0.7` _does_ include the\nserver and may work for individual use cases, but running repeated scripts\nagainst the same persistent server will not work as intended.)\n\nNightly server builds can be found as `Artifacts` of the [Nightly\nBuilds](https://github.com/GaloisInc/saw-script/actions/workflows/nightly.yml)\ngithub action. I.e., go to the `Nightly Builds` Github Action, click on a\nsuccessful build, scroll to the bottom and under `Artifacts` a Linux, Windows,\nand MacOS tarball will be listed. (Apologies... we need to make these easier to\nfind...)\n\n### Server docker images\n\nDocker images for the SAW server are currently uploaded to\n[DockerHub](https://hub.docker.com/r/galoisinc/saw-remote-api).\n\nThese images are set up to run as HTTP `saw-remote-api` servers, e.g.:\n\n```\ndocker run --name=saw-remote-api -d \\\n  -p 8080:8080 \\\n  galoisinc/saw-remote-api:TAG\n```\n\n(where `TAG` is either `latest` or `nightly`) will launch a server listening at\n`http://localhost:8080/`. (As of March 2020, `nightly` is recommended, as the\nserver in the last official release (i.e., the one accompanying SAW `v0.7`)\ncontains some non-trivial bugs that greatly limit its utility.)\n\nThe `-v` option to `docker run` can be used to load files into the docker\nserver\'s working directory so they can be loaded into the server at the request\nof python scripts. E.g., `-v PATH_TO_FILES:/home/saw/files/` will upload the\ncontents of the host machine\'s directory `PATH_TO_FILES` to the\n`/home/saw/files/` directory in the docker container, which corresponds to the\nrelative path `files/` for the SAW server. (If desired, it can be useful to\nplace files in a location in the Docker container such that the same relative\npaths in scripts refer to the same files in the host machine and docker\ncontainer.)\n\n### Building from Source\n\nIf this repository is checked out and the build directions are successfully run,\n`cabal v2-exec which saw-remote-api` should indicate where the server executable has\nbeen stored by `cabal`.\n\nAlternatively `cabal v2-install saw-remote-api` should install the server\nexecutable into the user\'s `~/.cabal/bin` directory (or similar), which (if\nconfigured properly) should then appear as `saw-remote-api` in a user\'s `PATH`.\n\n\n# Running Python SAW verification scripts\n\nOnce the server is setup and any path variables are setup as desired, the\nPython (>= v3.8) client can be installed using\n[`poetry`](https://python-poetry.org/docs/#installation) as follows:\n\n```\n$ cd saw-remote-api/python\n$ poetry install\n```\n\nThen the tests or individual scripts can be run as follows:\n```\n$ poetry run python -m unittest discover tests/saw\n$ poetry run python tests/saw/test_salsa20.py\n```\n\nIf leveraging environment variables is undesirable, the scripts themselves can\nspecify a command to launch the server, e.g.:\n\n```\nsaw_client.connect(COMMAND)\n```\n\nwhere `COMMAND` is a command to launch a new SAW server in socket mode.\n\nOr a server URL can be specified directly in the script, e.g.:\n\n```\nsaw_client.connect(url=URL)\n```\n\nwhere `URL` is a URL for a running SAW server in HTTP mode.\n\n## Running Verification Scripts from a clean state\n\nTo ensure any previous server state is cleared when running a SAW Python script\nagainst a persistent server (e.g., one running in HTTP mode in a different process),\nthe `reset_server` keyword can be passed to `saw_client.connect()`. E.g.,\n\n```\nsaw_client.connect(url="http://localhost:8080/", reset_server=True)\n```\n\nwill connect to a SAW server running at `http://localhost:8080/` and will\nguarantee any previous state on the server is cleared.\n',
-    'author': 'Galois, Inc.',
-    'author_email': 'saw@galois.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

