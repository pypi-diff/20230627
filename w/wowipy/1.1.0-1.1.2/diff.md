# Comparing `tmp/wowipy-1.1.0.tar.gz` & `tmp/wowipy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wowipy-1.1.0.tar", last modified: Fri Jun  9 09:33:10 2023, max compression
+gzip compressed data, was "wowipy-1.1.2.tar", last modified: Tue Jun 27 13:20:39 2023, max compression
```

## Comparing `wowipy-1.1.0.tar` & `wowipy-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 09:33:10.019625 wowipy-1.1.0/
--rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.0/COPYING
--rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-06-09 09:33:10.019625 wowipy-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-09 09:33:10.019625 wowipy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1277 2023-06-09 09:33:03.000000 wowipy-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:33:10.008653 wowipy-1.1.0/wowipy/
--rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.0/wowipy/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.0/wowipy/exceptions.py
--rw-rw-rw-   0        0        0    34007 2023-06-09 08:48:32.000000 wowipy-1.1.0/wowipy/models.py
--rw-rw-rw-   0        0        0     4515 2023-06-06 12:53:23.000000 wowipy-1.1.0/wowipy/rest_adapter.py
--rw-rw-rw-   0        0        0    33020 2023-06-09 09:08:56.000000 wowipy-1.1.0/wowipy/wowipy.py
-drwxrwxrwx   0        0        0        0 2023-06-09 09:33:10.018651 wowipy-1.1.0/wowipy.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-06-09 09:33:09.000000 wowipy-1.1.0/wowipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-09 09:33:09.000000 wowipy-1.1.0/wowipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 09:33:09.000000 wowipy-1.1.0/wowipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-09 09:33:09.000000 wowipy-1.1.0/wowipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 09:33:09.000000 wowipy-1.1.0/wowipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 13:20:39.389423 wowipy-1.1.2/
+-rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.2/COPYING
+-rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-06-27 13:20:39.388411 wowipy-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-27 13:20:39.389423 wowipy-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1277 2023-06-27 13:19:57.000000 wowipy-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:20:39.372455 wowipy-1.1.2/wowipy/
+-rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.2/wowipy/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.2/wowipy/exceptions.py
+-rw-rw-rw-   0        0        0    38772 2023-06-27 12:49:00.000000 wowipy-1.1.2/wowipy/models.py
+-rw-rw-rw-   0        0        0     4550 2023-06-27 13:11:28.000000 wowipy-1.1.2/wowipy/rest_adapter.py
+-rw-rw-rw-   0        0        0    40022 2023-06-27 13:11:28.000000 wowipy-1.1.2/wowipy/wowipy.py
+drwxrwxrwx   0        0        0        0 2023-06-27 13:20:39.387414 wowipy-1.1.2/wowipy.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-06-27 13:20:39.000000 wowipy-1.1.2/wowipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-27 13:20:39.000000 wowipy-1.1.2/wowipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 13:20:39.000000 wowipy-1.1.2/wowipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-27 13:20:39.000000 wowipy-1.1.2/wowipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 13:20:39.000000 wowipy-1.1.2/wowipy.egg-info/top_level.txt
```

### Comparing `wowipy-1.1.0/COPYING` & `wowipy-1.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.0/LICENSE` & `wowipy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.0/PKG-INFO` & `wowipy-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.0
+Version: 1.1.2
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `wowipy-1.1.0/setup.py` & `wowipy-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wowipy',
-    version='1.1.0',
+    version='1.1.2',
     description='OPENWOWI Wowiport API wrapper for python',
     url='https://github.com/seb-bau/WowiPy',
     author='Sebastian Bauhaus',
     author_email='sebastian@bytewish.de',
     license='GPL-3.0',
     packages=['wowipy'],
     install_requires=['requests>=2.0',
```

### Comparing `wowipy-1.1.0/wowipy/models.py` & `wowipy-1.1.2/wowipy/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -109,14 +109,74 @@
     pass
 
 
 class ContractorType(IdNameCombination):
     pass
 
 
+class ChangeReasonContracts(IdNameCombination):
+    pass
+
+
+class ValidContractPosition(IdNameCombination):
+    pass
+
+
+class ContractPositionType:
+    id_: int
+    node_id: int
+    name: str
+    short_code: str
+    deposit: bool
+    wb_relevant: bool
+    bgb_relevant: bool
+    is_part_of_net_rent: bool
+    using_cp_as_prepayment_block: bool
+    assignment_prepayment: str
+    is_gross_rent_without_heating: bool
+    is_part_of_net_rent_census: bool
+    is_basis_calculation_reminder_charge_interest: bool
+    is_prepayment_heating: bool
+    is_prepayment_running_cost: bool
+    report_as_sinking_fund: bool
+
+    def __init__(self, id_: int, node_id: int, name: str, short_code: str, deposit: bool, wb_relevant: bool,
+                 bgb_relevant: bool, is_part_of_net_rent: bool, using_cp_as_prepayment_block: bool,
+                 assignment_prepayment: str, is_gross_rent_without_heating: bool, is_part_of_net_rent_census: bool,
+                 is_basis_calculation_reminder_charge_interest: bool, is_prepayment_heating: bool,
+                 is_prepayment_running_cost: bool, report_as_sinking_fund: bool) -> None:
+        self.id_ = id_
+        self.node_id = node_id
+        self.name = name
+        self.short_code = short_code
+        self.deposit = deposit
+        self.wb_relevant = wb_relevant
+        self.bgb_relevant = bgb_relevant
+        self.is_part_of_net_rent = is_part_of_net_rent
+        self.using_cp_as_prepayment_block = using_cp_as_prepayment_block
+        self.assignment_prepayment = assignment_prepayment
+        self.is_gross_rent_without_heating = is_gross_rent_without_heating
+        self.is_part_of_net_rent_census = is_part_of_net_rent_census
+        self.is_basis_calculation_reminder_charge_interest = is_basis_calculation_reminder_charge_interest
+        self.is_prepayment_heating = is_prepayment_heating
+        self.is_prepayment_running_cost = is_prepayment_running_cost
+        self.report_as_sinking_fund = report_as_sinking_fund
+
+
+class ContractPositionTypeSlim:
+    id_: int
+    name: str
+    short_code: str
+
+    def __init__(self, id_: int, name: str, short_code: str) -> None:
+        self.id_ = id_
+        self.name = name
+        self.short_code = short_code
+
+
 class Country:
     id_: int
     name: str
     code: str
 
     def __init__(self, id_: int, name: str, code: str) -> None:
         self.id_ = id_
@@ -204,16 +264,16 @@
 class UseUnitShort:
     id_: int
     use_unit_number: str
     building_land_id: int
     economic_unit_id: int
     economic_unit: str
 
-    def __init__(self, id_: int, use_unit_number: str, building_land_id: int, economic_unit_id: int,
-                 economic_unit: str) -> None:
+    def __init__(self, id_: int, use_unit_number: str, building_land_id: int = 0, economic_unit_id: int = 0,
+                 economic_unit: str = 0) -> None:
         self.id_ = id_
         self.use_unit_number = use_unit_number
         self.building_land_id = building_land_id
         self.economic_unit_id = economic_unit_id
         self.economic_unit = economic_unit
 
 
@@ -923,14 +983,35 @@
         person["id_"] = person.pop("id")
         self.person = Person(**person)
         default_address["id_"] = default_address.pop("id")
         default_address["zip_"] = default_address.pop("zip")
         self.default_address = Address(**default_address)
 
 
+class LicenseAgreementShort:
+    id_: int
+    id_num: str
+    use_unit: UseUnitShort
+
+    def __init__(self, id_: int, id_num: str, use_unit: Dict) -> None:
+        self.id_ = id_
+        self.id_num = id_num
+        use_unit["id_"] = use_unit.pop("id")
+        self.use_unit = UseUnitShort(**use_unit)
+
+
+class VatRate:
+    id_: int
+    code: str
+
+    def __init__(self, id_: int, code: str) -> None:
+        self.id_ = id_
+        self.code = code
+
+
 class LicenseAgreement:
     id_: int
     id_num: str
     use_unit: UseUnitShort
     restriction_of_use: RestrictionOfUse
     status_contract: StatusContract
     life_of_contract: LifeOfContract
@@ -968,7 +1049,48 @@
             period_of_notice["id_"] = period_of_notice.pop("id")
             self.period_of_notice = PeriodOfNotice(**period_of_notice)
         else:
             self.period_of_notice = None
         self.debit_entry_type = DebitEntryType(**debit_entry_type)
         self.contractors = contractors
         self.__dict__.update(kwargs)
+
+
+class ContractPosition:
+    id_: int
+    net_amount: int
+    amount: int
+    active_from: datetime
+    active_to: datetime
+    license_agreement: LicenseAgreementShort
+    vat_rate: VatRate
+    valid_contract_position: ValidContractPosition
+    change_reason_contracts: ChangeReasonContracts
+    contract_position_type: ContractPositionType
+    contract_position_type_slim: Optional[ContractPositionTypeSlim]
+
+    def __init__(self, id_: int, net_amount: int, amount: int, active_from: datetime,
+                 active_to: datetime, license_agreement: Dict,
+                 vat_rate: Dict, valid_contract_position: Dict,
+                 change_reason_contracts: Dict,
+                 contract_position_type: Dict,
+                 contract_position_type_slim: Dict) -> None:
+        self.id_ = id_
+        self.net_amount = net_amount
+        self.amount = amount
+        self.active_from = active_from
+        self.active_to = active_to
+        license_agreement["id_"] = license_agreement.pop("id")
+        self.license_agreement = LicenseAgreementShort(**license_agreement)
+        vat_rate["id_"] = vat_rate.pop("id")
+        self.vat_rate = VatRate(**vat_rate)
+        valid_contract_position["id_"] = valid_contract_position.pop("id")
+        self.valid_contract_position = ValidContractPosition(**valid_contract_position)
+        change_reason_contracts["id_"] = change_reason_contracts.pop("id")
+        self.change_reason_contracts = ChangeReasonContracts(**change_reason_contracts)
+        contract_position_type["id_"] = contract_position_type.pop("id")
+        self.contract_position_type = ContractPositionType(**contract_position_type)
+        if contract_position_type_slim is not None:
+            contract_position_type_slim["id_"] = contract_position_type_slim.pop("id")
+            self.contract_position_type_slim = ContractPositionTypeSlim(**contract_position_type_slim)
+        else:
+            self.contract_position_type_slim = None
```

### Comparing `wowipy-1.1.0/wowipy/rest_adapter.py` & `wowipy-1.1.2/wowipy/rest_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         """
         self._logger = logger or logging.getLogger(__name__)
         self.host_base = hostname
         self.url = f"https://{hostname}/openwowi/{version}/"
         self.user = user
         self.password = password
         self.api_key = api_key
-        self.token = self._create_token()
+        if len(hostname) > 0:
+            self.token = self._create_token()
 
     def _create_token(self):
         full_url = f"https://{self.host_base}/oauth2/token"
         payload = f"grant_type=password&" \
                   f"username={self.user}&" \
                   f"password={self.password}"
         headers = {
```

### Comparing `wowipy-1.1.0/wowipy/wowipy.py` & `wowipy-1.1.2/wowipy/wowipy.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,112 @@
     def cache_from_disk(self, cache_type: str, file_name: str):
         if cache_type not in self._cache.keys():
             raise WowiPyException("Unknown Cache Type")
 
         with open(file_name, 'rb') as fp:
             self._cache[cache_type] = pickle.load(fp)
 
+    def search_string(self, haystack: str, needle: str, search_mode: str = SEARCH_POS_CONTAINS) -> bool:
+        haystack = haystack.lower()
+        needle = needle.lower()
+        if (search_mode == self.SEARCH_POS_CONTAINS and needle in haystack) or \
+                (search_mode == self.SEARCH_POS_LEFT and haystack.startswith(needle)):
+            return True
+        else:
+            return False
+
+    def search_contractor(self, search_name: str = None, search_address: str = None, search_phone: str = None,
+                          search_email: str = None, max_results: int = 10,
+                          search_mode: str = SEARCH_POS_CONTAINS) -> List:
+        person_ids = []
+        res = []
+        entry: Contractor
+        for entry in self._cache.get(self.CACHE_CONTRACTORS):
+            if len(res) >= max_results:
+                break
+
+            if entry.person.id_ in person_ids:
+                continue
+
+            if search_name is not None:
+                first_name = entry.person.natural_person.first_name.lower()
+                last_name = entry.person.natural_person.last_name.lower()
+                if self.search_string(first_name, search_name, search_mode) or \
+                        self.search_string(last_name, search_name, search_mode):
+                    res.append(entry)
+                    person_ids.append(entry.person.id_)
+                    continue
+
+            if search_address is not None:
+                address: Address
+                address_found = False
+                for address in entry.person.addresses:
+                    street = address.street_complete
+                    if self.search_string(street, search_address, search_mode):
+                        address_found = True
+                        break
+                if address_found:
+                    res.append(entry)
+                    person_ids.append(entry.person.id_)
+                    continue
+
+            if search_phone is not None:
+                communication: Communication
+                phone_found = False
+                if entry.person.communications is None:
+                    continue
+                for comm in entry.person.communications:
+                    if comm.communication_type.name == "Festnetz" or comm.communication_type.name == "Handynummer":
+                        content = comm.content.strip()
+                        search_phone = search_phone.strip()
+                        # Problem: Es gibt diverse gängige Formate für Rufnummern. Es gibt keine Formatvorgabe in
+                        # Wowiport, also können wir auch nicht vorhersehen, welches gewählt wurde.
+                        # Wenn ein + gefunden wurde, werden die ersten drei Zeichen von needle und haystack entfernt.
+                        # Ansonsten werden alle führenden Nullen entfernt
+                        if content.startswith('+'):
+                            content = content[3:]
+                        if search_phone.startswith('+'):
+                            search_phone = search_phone[3:]
+                        if search_phone.startswith('0049'):
+                            search_phone = search_phone[4:]
+                        if content.startswith('0049'):
+                            content = content[4:]
+
+                        content = content.lstrip('0')
+                        search_phone = search_phone.lstrip('0')
+
+                        content = content.replace(' ', '')
+                        search_phone = search_phone.replace(' ', '')
+
+                        if self.search_string(content, search_phone, search_mode):
+                            phone_found = True
+                            break
+                if phone_found:
+                    res.append(entry)
+                    person_ids.append(entry.person.id_)
+                    continue
+
+            if search_email is not None:
+                communication: Communication
+                email_found = False
+                if entry.person.communications is None:
+                    continue
+                for comm in entry.person.communications:
+                    if comm.communication_type.name == "E-Mail":
+                        content = comm.content.strip()
+                        if self.search_string(content, search_email, search_mode):
+                            email_found = True
+                            break
+                if email_found:
+                    res.append(entry)
+                    person_ids.append(entry.person.id_)
+                    continue
+
+        return res
+
     def search_cache(self, search_str: str, cache_types: Dict = None, max_results: int = 10,
                      find_pos: str = SEARCH_POS_CONTAINS) -> Dict:
         if cache_types is None:
             scope = self._cache
         else:
             scope = {}
             for ttype in self._cache.keys():
@@ -554,17 +652,20 @@
                       use_unit_idnum: str = None,
                       building_land_idnum: str = None,
                       economic_unit_idnum: str = None,
                       management_idnum: str = None,
                       owner_number: str = None,
                       limit: int = None,
                       offset: int = 0,
-                      add_args: Dict = None) -> List[UseUnit]:
+                      add_args: Dict = None,
+                      use_cache: bool = False) -> List[UseUnit]:
         """
         Gibt eine Liste von Nutzungseinheiten zurück
+        :param use_cache:
+        :type use_cache:
         :param use_unit_idnum: (Optional) Nur diese Nutzungseinheit zurückgeben
         :type use_unit_idnum: str
         :param building_land_idnum: (Optional) Nur Einheiten dieses Gebäudes zurückgeben
         :type building_land_idnum: str
         :param economic_unit_idnum: (Optional) Nur Einheiten dieser Wirtschaftseinheit zurückgeben
         :type economic_unit_idnum: str
         :param management_idnum: (Optional) Nur Einheiten dieses Managements zurückgeben
@@ -578,46 +679,56 @@
         :param add_args: Zusätzliche Parameter, die per GET an die URL angehängt werden
         :type add_args: Dict
         :return: Liste aus Nutzungseinheiten (auch bei nur einem Ergebnis!)
         :rtype: List[UseUnit]
         """
         filter_params = {}
         if use_unit_idnum is not None:
-            filter_params['useUnitNumber'] = owner_number
+            filter_params['useUnitNumber'] = use_unit_idnum
         if building_land_idnum is not None:
-            filter_params['buildingLandIdNum'] = owner_number
+            filter_params['buildingLandIdNum'] = building_land_idnum
         if economic_unit_idnum is not None:
-            filter_params['EconomicUnitIdNum'] = owner_number
+            filter_params['EconomicUnitIdNum'] = economic_unit_idnum
         if management_idnum is not None:
-            filter_params['managementIdNum'] = owner_number
+            filter_params['managementIdNum'] = management_idnum
         if owner_number is not None:
             filter_params['ownerNumber'] = owner_number
         if limit is not None:
             filter_params['limit'] = limit
         filter_params['offset'] = offset
 
         # Standardparameter, können via add_args überschrieben werden
         filter_params['includeUseUnitTypes'] = 'true'
         filter_params['includeBillingUnits'] = 'true'
         filter_params['includeMarketingTags'] = 'false'
 
         if add_args is not None:
             filter_params.update(add_args)
-
-        result = self._rest_adapter.get(endpoint='CommercialInventory/UseUnits', ep_params=filter_params)
         retlist = []
-        for entry in result.data:
-            data = dict(humps.decamelize(entry))
-            data['id_'] = data.pop('id')
-            if data.get('estate_address') is not None:
-                data.get('estate_address')['zip_'] = data.get('estate_address').pop('zip')
-            if data.get('floor') is not None:
-                data.get('floor')['id_'] = data.get('floor').pop('id')
-            ret_la = UseUnit(**data)
-            retlist.append(ret_la)
+
+        if use_cache:
+            cache_entry: UseUnit
+            for cache_entry in self._cache[self.CACHE_USE_UNITS]:
+                if (use_unit_idnum is not None and cache_entry.id_num == use_unit_idnum) or \
+                        (building_land_idnum is not None and
+                         cache_entry.building_land.id_num == building_land_idnum) or \
+                        (economic_unit_idnum is not None and
+                         cache_entry.economic_unit.id_num == economic_unit_idnum):
+                    retlist.append(copy.deepcopy(cache_entry))
+        else:
+            result = self._rest_adapter.get(endpoint='CommercialInventory/UseUnits', ep_params=filter_params)
+            for entry in result.data:
+                data = dict(humps.decamelize(entry))
+                data['id_'] = data.pop('id')
+                if data.get('estate_address') is not None:
+                    data.get('estate_address')['zip_'] = data.get('estate_address').pop('zip')
+                if data.get('floor') is not None:
+                    data.get('floor')['id_'] = data.get('floor').pop('id')
+                ret_la = UseUnit(**data)
+                retlist.append(ret_la)
         return retlist
 
     def get_contractors(self,
                         license_agreement_id: int = None,
                         person_id: int = None,
                         license_agreement_active_on: datetime = None,
                         contractual_use_active_on: datetime = None,
@@ -682,7 +793,43 @@
 
             for entry in result.data:
                 data = dict(humps.decamelize(entry))
                 data['id_'] = data.pop('id')
                 ret_la = Contractor(**data)
                 retlist.append(ret_la)
         return retlist
+
+    def get_contract_positions(self,
+                               license_agreement_idnum: str = None,
+                               license_agreement_id: int = None,
+                               contract_positions_active_on: datetime = None,
+                               limit: int = None,
+                               offset: int = 0,
+                               add_args: Dict = None) -> List[ContractPosition]:
+
+        filter_params = {}
+        if license_agreement_idnum is not None:
+            filter_params['licenseAgreementIdNum'] = license_agreement_idnum
+        if license_agreement_id is not None:
+            filter_params['licenseAgreementId'] = license_agreement_id
+        if contract_positions_active_on is not None:
+            filter_params['contractPositionsActiveOn'] = contract_positions_active_on.strftime("%Y-%m-%d")
+        if limit is not None:
+            filter_params['limit'] = limit
+        filter_params['offset'] = offset
+
+        filter_params['includeContractPositionTypeDetails'] = 'true'
+        filter_params['showNullValues'] = 'true'
+
+        if add_args is not None:
+            filter_params.update(add_args)
+
+        retlist = []
+        result = self._rest_adapter.get(endpoint='RentAccounting/ContractPositions', ep_params=filter_params)
+
+        for entry in result.data:
+            data = dict(humps.decamelize(entry))
+            data['id_'] = data.pop('id')
+            ret_la = ContractPosition(**data)
+            retlist.append(ret_la)
+
+        return retlist
```

### Comparing `wowipy-1.1.0/wowipy.egg-info/PKG-INFO` & `wowipy-1.1.2/wowipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.0
+Version: 1.1.2
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

