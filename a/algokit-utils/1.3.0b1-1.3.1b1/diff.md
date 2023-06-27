# Comparing `tmp/algokit_utils-1.3.0b1-py3-none-any.whl.zip` & `tmp/algokit_utils-1.3.1b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 36703 bytes, number of entries: 16
--rw-r--r--  2.0 unx     4159 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
+Zip file size: 37027 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     4133 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     2841 b- defN 80-Jan-01 00:00 algokit_utils/_simulate_315_compat.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
--rw-r--r--  2.0 unx    56488 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
+-rw-r--r--  2.0 unx    56581 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    34650 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
--rw-r--r--  2.0 unx     6319 b- defN 80-Jan-01 00:00 algokit_utils/models.py
+-rw-r--r--  2.0 unx     8246 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     5267 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2072 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1357 b- defN 16-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/RECORD
-16 files, 139676 bytes uncompressed, 34461 bytes compressed:  75.3%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.3.1b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2116 b- defN 80-Jan-01 00:00 algokit_utils-1.3.1b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.3.1b1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1357 b- defN 16-Jan-01 00:00 algokit_utils-1.3.1b1.dist-info/RECORD
+16 files, 141714 bytes uncompressed, 34785 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.3.0b1.dist-info/LICENSE
+Filename: algokit_utils-1.3.1b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.3.0b1.dist-info/METADATA
+Filename: algokit_utils-1.3.1b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.3.0b1.dist-info/WHEEL
+Filename: algokit_utils-1.3.1b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.3.0b1.dist-info/RECORD
+Filename: algokit_utils-1.3.1b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/__init__.py

```diff
@@ -59,22 +59,22 @@
 )
 from algokit_utils.logic_error import LogicError
 from algokit_utils.models import (
     ABIArgsDict,
     ABIMethod,
     ABITransactionResponse,
     Account,
-    CommonCallParameters,
-    CommonCallParametersDict,
+    CommonCallParameters,  # noqa: ignore[F401]
+    CommonCallParametersDict,  # noqa: ignore[F401]
     CreateCallParameters,
     CreateCallParametersDict,
     CreateTransactionParameters,
     OnCompleteCallParameters,
     OnCompleteCallParametersDict,
-    RawTransactionParameters,
+    RawTransactionParameters,  # noqa: ignore[F401]
     TransactionParameters,
     TransactionResponse,
 )
 from algokit_utils.network_clients import (
     AlgoClientConfig,
     get_algod_client,
     get_algonode_config,
@@ -107,26 +107,23 @@
     "replace_template_variables",
     "ABIArgsDict",
     "ABICallArgs",
     "ABICallArgsDict",
     "ABICreateCallArgs",
     "ABICreateCallArgsDict",
     "ABIMethod",
-    "CommonCallParameters",
-    "CommonCallParametersDict",
     "CreateCallParameters",
     "CreateCallParametersDict",
     "CreateTransactionParameters",
     "DeployCallArgs",
     "DeployCreateCallArgs",
     "DeployCallArgsDict",
     "DeployCreateCallArgsDict",
     "OnCompleteCallParameters",
     "OnCompleteCallParametersDict",
-    "RawTransactionParameters",
     "TransactionParameters",
     "ApplicationClient",
     "DeployResponse",
     "OnUpdate",
     "OnSchemaBreak",
     "OperationPerformed",
     "TemplateValueDict",
```

## algokit_utils/application_client.py

```diff
@@ -36,20 +36,20 @@
 from algokit_utils.logic_error import LogicError, parse_logic_error
 from algokit_utils.models import (
     ABIArgsDict,
     ABIArgType,
     ABIMethod,
     ABITransactionResponse,
     Account,
-    CommonCallParameters,
-    CommonCallParametersDict,
     CreateCallParameters,
     CreateCallParametersDict,
     OnCompleteCallParameters,
     OnCompleteCallParametersDict,
+    TransactionParameters,
+    TransactionParametersDict,
     TransactionResponse,
 )
 
 if typing.TYPE_CHECKING:
     from algosdk.v2client.algod import AlgodClient
     from algosdk.v2client.indexer import IndexerClient
 
@@ -368,15 +368,15 @@
         /,
         call_abi_method: ABIMethod | bool | None = None,
         transaction_parameters: CreateCallParameters | CreateCallParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> None:
         """Adds a signed transaction with application id == 0 and the schema and source of client's app_spec to atc"""
         approval_program, clear_program = self._check_is_compiled()
-        transaction_parameters = _convert_call_parameters(transaction_parameters)
+        transaction_parameters = _convert_transaction_parameters(transaction_parameters)
 
         extra_pages = transaction_parameters.extra_pages or num_extra_program_pages(
             approval_program.raw_binary, clear_program.raw_binary
         )
 
         self.add_method_call(
             atc,
@@ -440,15 +440,15 @@
         return create_result
 
     def compose_update(
         self,
         atc: AtomicTransactionComposer,
         /,
         call_abi_method: ABIMethod | bool | None = None,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> None:
         """Adds a signed transaction with on_complete=UpdateApplication to atc"""
         approval_program, clear_program = self._check_is_compiled()
 
         self.add_method_call(
             atc=atc,
@@ -460,40 +460,40 @@
             clear_program=clear_program.raw_binary,
         )
 
     @overload
     def update(
         self,
         call_abi_method: ABIMethod | Literal[True],
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = ...,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = ...,
         **abi_kwargs: ABIArgType,
     ) -> ABITransactionResponse:
         ...
 
     @overload
     def update(
         self,
         call_abi_method: Literal[False],
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = ...,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = ...,
     ) -> TransactionResponse:
         ...
 
     @overload
     def update(
         self,
         call_abi_method: ABIMethod | bool | None = ...,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = ...,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = ...,
         **abi_kwargs: ABIArgType,
     ) -> TransactionResponse | ABITransactionResponse:
         ...
 
     def update(
         self,
         call_abi_method: ABIMethod | bool | None = None,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> TransactionResponse | ABITransactionResponse:
         """Submits a signed transaction with on_complete=UpdateApplication"""
 
         atc = AtomicTransactionComposer()
         self.compose_update(
             atc,
@@ -504,15 +504,15 @@
         return self._execute_atc_tr(atc)
 
     def compose_delete(
         self,
         atc: AtomicTransactionComposer,
         /,
         call_abi_method: ABIMethod | bool | None = None,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> None:
         """Adds a signed transaction with on_complete=DeleteApplication to atc"""
 
         self.add_method_call(
             atc,
             call_abi_method,
@@ -521,40 +521,40 @@
             on_complete=transaction.OnComplete.DeleteApplicationOC,
         )
 
     @overload
     def delete(
         self,
         call_abi_method: ABIMethod | Literal[True],
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = ...,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = ...,
         **abi_kwargs: ABIArgType,
     ) -> ABITransactionResponse:
         ...
 
     @overload
     def delete(
         self,
         call_abi_method: Literal[False],
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = ...,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = ...,
     ) -> TransactionResponse:
         ...
 
     @overload
     def delete(
         self,
         call_abi_method: ABIMethod | bool | None = ...,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = ...,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = ...,
         **abi_kwargs: ABIArgType,
     ) -> TransactionResponse | ABITransactionResponse:
         ...
 
     def delete(
         self,
         call_abi_method: ABIMethod | bool | None = None,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> TransactionResponse | ABITransactionResponse:
         """Submits a signed transaction with on_complete=DeleteApplication"""
 
         atc = AtomicTransactionComposer()
         self.compose_delete(
             atc,
@@ -569,15 +569,15 @@
         atc: AtomicTransactionComposer,
         /,
         call_abi_method: ABIMethod | bool | None = None,
         transaction_parameters: OnCompleteCallParameters | OnCompleteCallParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> None:
         """Adds a signed transaction with specified parameters to atc"""
-        _parameters = _convert_call_parameters(transaction_parameters)
+        _parameters = _convert_transaction_parameters(transaction_parameters)
         self.add_method_call(
             atc,
             abi_method=call_abi_method,
             abi_args=abi_kwargs,
             parameters=_parameters,
             on_complete=_parameters.on_complete or transaction.OnComplete.NoOpOC,
         )
@@ -612,15 +612,15 @@
         self,
         call_abi_method: ABIMethod | bool | None = None,
         transaction_parameters: OnCompleteCallParameters | OnCompleteCallParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> TransactionResponse | ABITransactionResponse:
         """Submits a signed transaction with specified parameters"""
         atc = AtomicTransactionComposer()
-        _parameters = _convert_call_parameters(transaction_parameters)
+        _parameters = _convert_transaction_parameters(transaction_parameters)
         self.compose_call(
             atc,
             call_abi_method=call_abi_method,
             transaction_parameters=_parameters,
             **abi_kwargs,
         )
 
@@ -635,15 +635,15 @@
         return self._execute_atc_tr(atc)
 
     def compose_opt_in(
         self,
         atc: AtomicTransactionComposer,
         /,
         call_abi_method: ABIMethod | bool | None = None,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> None:
         """Adds a signed transaction with on_complete=OptIn to atc"""
         self.add_method_call(
             atc,
             abi_method=call_abi_method,
             abi_args=abi_kwargs,
@@ -651,40 +651,40 @@
             on_complete=transaction.OnComplete.OptInOC,
         )
 
     @overload
     def opt_in(
         self,
         call_abi_method: ABIMethod | Literal[True] = ...,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> ABITransactionResponse:
         ...
 
     @overload
     def opt_in(
         self,
         call_abi_method: Literal[False] = ...,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
     ) -> TransactionResponse:
         ...
 
     @overload
     def opt_in(
         self,
         call_abi_method: ABIMethod | bool | None = ...,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = ...,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = ...,
         **abi_kwargs: ABIArgType,
     ) -> TransactionResponse | ABITransactionResponse:
         ...
 
     def opt_in(
         self,
         call_abi_method: ABIMethod | bool | None = None,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> TransactionResponse | ABITransactionResponse:
         """Submits a signed transaction with on_complete=OptIn"""
         atc = AtomicTransactionComposer()
         self.compose_opt_in(
             atc,
             call_abi_method=call_abi_method,
@@ -694,15 +694,15 @@
         return self._execute_atc_tr(atc)
 
     def compose_close_out(
         self,
         atc: AtomicTransactionComposer,
         /,
         call_abi_method: ABIMethod | bool | None = None,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> None:
         """Adds a signed transaction with on_complete=CloseOut to ac"""
         self.add_method_call(
             atc,
             abi_method=call_abi_method,
             abi_args=abi_kwargs,
@@ -710,40 +710,40 @@
             on_complete=transaction.OnComplete.CloseOutOC,
         )
 
     @overload
     def close_out(
         self,
         call_abi_method: ABIMethod | Literal[True],
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = ...,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = ...,
         **abi_kwargs: ABIArgType,
     ) -> ABITransactionResponse:
         ...
 
     @overload
     def close_out(
         self,
         call_abi_method: Literal[False],
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = ...,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = ...,
     ) -> TransactionResponse:
         ...
 
     @overload
     def close_out(
         self,
         call_abi_method: ABIMethod | bool | None = ...,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = ...,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = ...,
         **abi_kwargs: ABIArgType,
     ) -> TransactionResponse | ABITransactionResponse:
         ...
 
     def close_out(
         self,
         call_abi_method: ABIMethod | bool | None = None,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         **abi_kwargs: ABIArgType,
     ) -> TransactionResponse | ABITransactionResponse:
         """Submits a signed transaction with on_complete=CloseOut"""
         atc = AtomicTransactionComposer()
         self.compose_close_out(
             atc,
             call_abi_method=call_abi_method,
@@ -752,28 +752,28 @@
         )
         return self._execute_atc_tr(atc)
 
     def compose_clear_state(
         self,
         atc: AtomicTransactionComposer,
         /,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         app_args: list[bytes] | None = None,
     ) -> None:
         """Adds a signed transaction with on_complete=ClearState to atc"""
         return self.add_method_call(
             atc,
             parameters=transaction_parameters,
             on_complete=transaction.OnComplete.ClearStateOC,
             app_args=app_args,
         )
 
     def clear_state(
         self,
-        transaction_parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        transaction_parameters: TransactionParameters | TransactionParametersDict | None = None,
         app_args: list[bytes] | None = None,
     ) -> TransactionResponse:
         """Submits a signed transaction with on_complete=ClearState"""
         atc = AtomicTransactionComposer()
         self.compose_clear_state(
             atc,
             transaction_parameters=transaction_parameters,
@@ -995,29 +995,29 @@
     def add_method_call(
         self,
         atc: AtomicTransactionComposer,
         abi_method: ABIMethod | bool | None = None,
         *,
         abi_args: ABIArgsDict | None = None,
         app_id: int | None = None,
-        parameters: CommonCallParameters | CommonCallParametersDict | None = None,
+        parameters: TransactionParameters | TransactionParametersDict | None = None,
         on_complete: transaction.OnComplete = transaction.OnComplete.NoOpOC,
         local_schema: transaction.StateSchema | None = None,
         global_schema: transaction.StateSchema | None = None,
         approval_program: bytes | None = None,
         clear_program: bytes | None = None,
         extra_pages: int | None = None,
         app_args: list[bytes] | None = None,
         call_config: au_spec.CallConfig = au_spec.CallConfig.CALL,
     ) -> None:
         """Adds a transaction to the AtomicTransactionComposer passed"""
         if app_id is None:
             self._load_reference_and_check_app_id()
             app_id = self.app_id
-        parameters = _convert_call_parameters(parameters)
+        parameters = _convert_transaction_parameters(parameters)
         method = self._resolve_method(abi_method, abi_args, on_complete, call_config)
         sp = parameters.suggested_params or self.suggested_params or self.algod_client.suggested_params()
         signer, sender = self.resolve_signer_sender(parameters.signer, parameters.sender)
         if parameters.boxes is not None:
             # TODO: algosdk actually does this, but it's type hints say otherwise...
             encoded_boxes = [(id_, algosdk.encoding.encode_as_bytes(name)) for id_, name in parameters.boxes]
         else:
@@ -1279,16 +1279,18 @@
     except Exception as ex:
         logic_error = _try_convert_to_logic_error(ex, approval_program, approval_source_map)
         if logic_error:
             raise logic_error from ex
         raise ex
 
 
-def _convert_call_parameters(args: CommonCallParameters | CommonCallParametersDict | None) -> CreateCallParameters:
-    _args = args.__dict__ if isinstance(args, CommonCallParameters) else (args or {})
+def _convert_transaction_parameters(
+    args: TransactionParameters | TransactionParametersDict | None,
+) -> CreateCallParameters:
+    _args = args.__dict__ if isinstance(args, TransactionParameters) else (args or {})
     return CreateCallParameters(**_args)
 
 
 def get_sender_from_signer(signer: TransactionSigner | None) -> str | None:
     """Returns the associated address of a signer, return None if no address found"""
 
     if isinstance(signer, AccountTransactionSigner):
```

## algokit_utils/models.py

```diff
@@ -8,14 +8,29 @@
 from algosdk.atomic_transaction_composer import (
     AccountTransactionSigner,
     AtomicTransactionResponse,
     SimulateAtomicTransactionResponse,
     TransactionSigner,
 )
 from algosdk.encoding import decode_address
+from deprecated import deprecated
+
+__all__ = [
+    "ABIArgsDict",
+    "ABIMethod",
+    "ABITransactionResponse",
+    "Account",
+    "CreateCallParameters",
+    "CreateCallParametersDict",
+    "CreateTransactionParameters",
+    "OnCompleteCallParameters",
+    "OnCompleteCallParametersDict",
+    "TransactionParameters",
+    "TransactionResponse",
+]
 
 ReturnType = TypeVar("ReturnType")
 
 
 @dataclasses.dataclass(kw_only=True)
 class Account:
     """Holds the private_key and address for an account"""
@@ -111,79 +126,108 @@
 
 
 ABIMethod: TypeAlias = ABIReturnSubroutine | Method | str
 
 
 @dataclasses.dataclass(kw_only=True)
 class TransactionParameters:
-    """Transaction parameters that can be used on ABI and non-ABI calls"""
+    """Additional parameters that can be included in a transaction"""
 
     signer: TransactionSigner | None = None
+    """Signer to use when signing this transaction"""
     sender: str | None = None
+    """Sender of this transaction"""
     suggested_params: transaction.SuggestedParams | None = None
+    """SuggestedParams to use for this transaction"""
     note: bytes | str | None = None
+    """Note for this transaction"""
     lease: bytes | str | None = None
+    """Lease value for this transaction"""
     boxes: Sequence[tuple[int, bytes | bytearray | str | int]] | None = None
-
-
-@dataclasses.dataclass(kw_only=True)
-class CreateTransactionParameters(TransactionParameters):
-    """Transaction parameters that can be used on ABI and non-ABI create calls"""
-
-    extra_pages: int | None = None
-
-
-@dataclasses.dataclass(kw_only=True)
-class RawTransactionParameters(TransactionParameters):
-    """Transaction parameters that can be used on non-ABI calls"""
-
+    """Box references to include in transaction. A sequence of (app id, box key) tuples"""
     accounts: list[str] | None = None
+    """Accounts to include in transaction"""
     foreign_apps: list[int] | None = None
+    """List of foreign apps (by app id) to include in transaction"""
     foreign_assets: list[int] | None = None
+    """List of foreign assets (by asset id) to include in transaction"""
+    rekey_to: str | None = None
+    """Address to rekey to"""
 
 
+# CreateTransactionParameters is used by algokit-client-generator clients
 @dataclasses.dataclass(kw_only=True)
-class CommonCallParameters(RawTransactionParameters):
-    """Transaction parameters used when making update, delete, opt_in, close_out or clear_state calls"""
+class CreateTransactionParameters(TransactionParameters):
+    """Additional parameters that can be included in a transaction when calling a create method"""
 
-    rekey_to: str | None = None
+    extra_pages: int | None = None
 
 
 @dataclasses.dataclass(kw_only=True)
-class OnCompleteCallParameters(CommonCallParameters):
-    """Transaction parameters used when making any call to an Application"""
+class OnCompleteCallParameters(TransactionParameters):
+    """Additional parameters that can be included in a transaction when using the
+    ApplicationClient.call/compose_call methods"""
 
     on_complete: transaction.OnComplete | None = None
 
 
 @dataclasses.dataclass(kw_only=True)
 class CreateCallParameters(OnCompleteCallParameters):
-    """Transaction parameters used when making a create call for Application"""
+    """Additional parameters that can be included in a transaction when using the
+    ApplicationClient.create/compose_create methods"""
 
     extra_pages: int | None = None
 
 
-class CommonCallParametersDict(TypedDict, total=False):
-    """Common transaction parameters used when making update, delete, opt_in, close_out or clear_state calls"""
+class TransactionParametersDict(TypedDict, total=False):
+    """Additional parameters that can be included in a transaction"""
 
     signer: TransactionSigner
+    """Signer to use when signing this transaction"""
     sender: str
+    """Sender of this transaction"""
     suggested_params: transaction.SuggestedParams
+    """SuggestedParams to use for this transaction"""
     note: bytes | str
+    """Note for this transaction"""
     lease: bytes | str
+    """Lease value for this transaction"""
+    boxes: Sequence[tuple[int, bytes | bytearray | str | int]]
+    """Box references to include in transaction. A sequence of (app id, box key) tuples"""
     accounts: list[str]
+    """Accounts to include in transaction"""
     foreign_apps: list[int]
+    """List of foreign apps (by app id) to include in transaction"""
     foreign_assets: list[int]
-    boxes: Sequence[tuple[int, bytes | bytearray | str | int]]
+    """List of foreign assets (by asset id) to include in transaction"""
     rekey_to: str
+    """Address to rekey to"""
 
 
-class OnCompleteCallParametersDict(TypedDict, CommonCallParametersDict, total=False):
-    """Transaction parameters used when making any call to an Application"""
+class OnCompleteCallParametersDict(TypedDict, TransactionParametersDict, total=False):
+    """Additional parameters that can be included in a transaction when using the
+    ApplicationClient.call/compose_call methods"""
 
     on_complete: transaction.OnComplete
 
 
 class CreateCallParametersDict(TypedDict, OnCompleteCallParametersDict, total=False):
-    """Transaction parameters used when making a create call for Application"""
+    """Additional parameters that can be included in a transaction when using the
+    ApplicationClient.create/compose_create methods"""
 
     extra_pages: int
+
+
+# Pre 1.3.1 backwards compatibility
+@deprecated(reason="Use TransactionParameters instead", version="1.3.1")
+class RawTransactionParameters(TransactionParameters):
+    """Deprecated, use TransactionParameters instead"""
+
+
+@deprecated(reason="Use TransactionParameters instead", version="1.3.1")
+class CommonCallParameters(TransactionParameters):
+    """Deprecated, use TransactionParameters instead"""
+
+
+@deprecated(reason="Use TransactionParametersDict instead", version="1.3.1")
+class CommonCallParametersDict(TransactionParametersDict):
+    """Deprecated, use TransactionParametersDict instead"""
```

## Comparing `algokit_utils-1.3.0b1.dist-info/LICENSE` & `algokit_utils-1.3.1b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.3.0b1.dist-info/METADATA` & `algokit_utils-1.3.1b1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.3.0b1
+Version: 1.3.1b1
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: py-algorand-sdk (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # AlgoKit Python Utilities
 
 A set of core Algorand utilities written in Python and released via PyPi that make it easier to build solutions on Algorand. 
 This project is part of [AlgoKit](https://github.com/algorandfoundation/algokit-cli).
```

## Comparing `algokit_utils-1.3.0b1.dist-info/RECORD` & `algokit_utils-1.3.1b1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-algokit_utils/__init__.py,sha256=Ko-gEPeER-Ho8lRU_a6k5SsV3mTfZa6CP1I9dmZjQvk,4159
+algokit_utils/__init__.py,sha256=8_zT0ryHuEi7Vn51LRjNPCnq6wXL6er5x_tvGPg8ZLo,4133
 algokit_utils/_ensure_funded.py,sha256=DjwGnCC_6USLQV5wIMJZRVQFlQ1uLrGDMxRF471atsQ,4410
 algokit_utils/_simulate_315_compat.py,sha256=9qCsNnKa1FXYfCccMFiE0mGEcZJiBuPmUy7ZRvvUSqU,2841
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
-algokit_utils/application_client.py,sha256=k3eTyhY3zyfpajHffo1uJ2u1C0vlYPmdALl5jmgH1WM,56488
+algokit_utils/application_client.py,sha256=4_NM-RJYMCRCS4_4xFeG68yYvgTJRC1_y9mSCgYHSR4,56581
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=sY6u0T39DuF6oLpal0eJAc76EmjPWdoCPk2OSKGccnM,34650
 algokit_utils/logic_error.py,sha256=8O_4rJ1t57JEG81ucRNih2ojc1-EOm2fVxW6m-1ZXI8,2550
-algokit_utils/models.py,sha256=75tWWa3W-37Om3YgkcuKiuHAGzMkFIJ9U-eHO29RPi4,6319
+algokit_utils/models.py,sha256=KynZnM2YbOyTgr2NCT8CA-cYrO0eiyK6u48eeAzj82I,8246
 algokit_utils/network_clients.py,sha256=KmuSHG2kSdJfo9W4pIB_4RjnBL2yMQNGlF54lxXTnsQ,5267
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.3.0b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.3.0b1.dist-info/METADATA,sha256=75vQhThgjoQUr2xDl-t--FnVEl9bHz7kAs7LS4jVwns,2072
-algokit_utils-1.3.0b1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-algokit_utils-1.3.0b1.dist-info/RECORD,,
+algokit_utils-1.3.1b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.3.1b1.dist-info/METADATA,sha256=qJ1Che639w5ftvOOakseRd2P8UxuKfCSGkLdpva6RlE,2116
+algokit_utils-1.3.1b1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+algokit_utils-1.3.1b1.dist-info/RECORD,,
```

