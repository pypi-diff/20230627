# Comparing `tmp/pih-1.43.tar.gz` & `tmp/pih-1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.43.tar", last modified: Thu May  4 23:32:40 2023, max compression
+gzip compressed data, was "pih-1.45.tar", last modified: Tue Jun 27 04:00:34 2023, max compression
```

## Comparing `pih-1.43.tar` & `pih-1.45.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 23:32:40.314156 pih-1.43/
--rw-rw-rw-   0        0        0      258 2023-05-04 23:32:40.298564 pih-1.43/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-04 23:32:39.423602 pih-1.43/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.43/pih/__init__.py
--rw-rw-rw-   0        0        0    15492 2023-05-02 07:21:58.000000 pih-1.43/pih/collection.py
--rw-rw-rw-   0        0        0    49882 2023-04-26 06:39:23.000000 pih-1.43/pih/console_api.py
--rw-rw-rw-   0        0        0    92125 2023-05-04 23:30:36.000000 pih-1.43/pih/const.py
--rw-rw-rw-   0        0        0   239867 2023-05-04 23:31:39.000000 pih-1.43/pih/pih.py
--rw-rw-rw-   0        0        0    19843 2023-05-04 23:27:46.000000 pih-1.43/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.43/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.43/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      624 2023-03-29 23:40:14.000000 pih-1.43/pih/rpc_collection.py
--rw-rw-rw-   0        0        0      793 2023-04-22 17:05:00.000000 pih-1.43/pih/service_example.py
--rw-rw-rw-   0        0        0    29939 2023-05-04 01:10:38.000000 pih-1.43/pih/tools.py
--rw-rw-rw-   0        0        0     2037 2022-10-21 06:31:07.000000 pih-1.43/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-04 23:32:40.079778 pih-1.43/pih.egg-info/
--rw-rw-rw-   0        0        0      258 2023-05-04 23:32:36.000000 pih-1.43/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-04 23:32:37.000000 pih-1.43/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 23:32:36.000000 pih-1.43/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-04 23:32:36.000000 pih-1.43/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-04 23:32:36.000000 pih-1.43/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2130 2023-05-04 23:29:46.000000 pih-1.43/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-05-04 23:32:40.345417 pih-1.43/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 04:00:34.711113 pih-1.45/
+-rw-rw-rw-   0        0        0      258 2023-06-27 04:00:34.711113 pih-1.45/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 04:00:34.304880 pih-1.45/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.45/pih/__init__.py
+-rw-rw-rw-   0        0        0    17207 2023-06-27 03:44:30.000000 pih-1.45/pih/collection.py
+-rw-rw-rw-   0        0        0    53104 2023-06-26 11:43:41.000000 pih-1.45/pih/console_api.py
+-rw-rw-rw-   0        0        0   102561 2023-06-27 03:44:30.000000 pih-1.45/pih/const.py
+-rw-rw-rw-   0        0        0   282554 2023-06-27 03:46:49.000000 pih-1.45/pih/pih.py
+-rw-rw-rw-   0        0        0    24688 2023-06-27 01:47:21.000000 pih-1.45/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.45/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.45/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.45/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6222 2023-06-25 11:03:20.000000 pih-1.45/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.45/pih/service_example.py
+-rw-rw-rw-   0        0        0    35775 2023-06-27 03:14:15.000000 pih-1.45/pih/tools.py
+-rw-rw-rw-   0        0        0     2037 2022-10-21 06:31:07.000000 pih-1.45/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-27 04:00:34.664242 pih-1.45/pih.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-06-27 04:00:30.000000 pih-1.45/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-06-27 04:00:31.000000 pih-1.45/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 04:00:30.000000 pih-1.45/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-27 04:00:30.000000 pih-1.45/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-27 04:00:31.000000 pih-1.45/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2014 2023-06-27 04:00:23.000000 pih-1.45/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 04:00:34.726744 pih-1.45/setup.cfg
```

### Comparing `pih-1.43/pih/collection.py` & `pih-1.45/pih/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,44 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 from typing import Any, Generic, Tuple, TypeVar, List
+from collections import namedtuple
 
+Rect = namedtuple("Rect", ["left", "top", "width", "height"])
 
 @dataclass
 class FieldItem:
     name: str | None = None
     caption: str | None = None
     visible: bool = True
     class_type: Any | None = None
     default_value: str | None = None
     data_formatter: str = "{data}"
 
+@dataclass
+class RecipientWaitingForInput:
+    group_name: str | None = None
+    timeout: int | None = None
+    recipient: str | None = None
+    timestamp: datetime | None = None
+
+@dataclass
+class BarcodeInformation:
+    data: str | None = None
+    type: str | None = None
+    rect: Rect | None = None
+
+@dataclass
+class InaccesableEmailInformation:
+    email: str | None = None
+    person_pin: int = 0
+    person_name: str | None = None
+    workstation_name: str | None = None
+    registrator_person_name: str | None = None
 
 @dataclass
 class FullName:
     last_name: str = ""
     first_name: str = ""
     middle_name: str = ""
 
@@ -27,53 +49,14 @@
 
 
 @dataclass
 class LoginPasswordPair:
     login: str | None = None
     password: str | None = None
 
-
-@dataclass
-class ServiceRoleDescriptionBase:
-    name: str | None = None
-    description: str | None = None
-    host: str | None = None
-    login: str | None = None
-    password: str | None = None
-    port: str | None = None
-    service_path: str | None = None
-    pid: int = -1
-    pih_version: str | None = None
-    isolated: bool = False
-    visible_for_admin: bool = True
-    auto_restart: bool = True
-    weak_subscribtion: bool = False
-    auto_start: bool = True
-    start_once: bool = False
-
-
-@dataclass
-class ServiceRoleInformation(ServiceRoleDescriptionBase):
-    subscribers: list | None = None
-
-
-@dataclass
-class ServiceRoleDescription(ServiceRoleDescriptionBase):
-    #from pih.const import ServiceCommands
-    #list[ServiceCommands]
-    commands: list = field(default_factory=list)
-    modules: list[str] = field(default_factory=list)
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-    
-    def __eq__(self, another):
-         return self.name == another.name
-
-
 class FieldItemList:
 
     list: list[FieldItem]
 
     def copy_field_item(self, value: FieldItem) -> FieldItem:
         return FieldItem(
             value.name, value.caption, value.visible, value.class_type, value.default_value, value.data_formatter)
@@ -150,22 +133,22 @@
 class OGRN:
     name: str | None = None
     code: str | None = None
     data: dict | None = None
 
 
 @dataclass
-class UserContainer:
+class UserBase:
     name: str | None = None
     description: str | None = None
     distinguishedName: str | None = None
 
 
 @dataclass
-class User(UserContainer):
+class User(UserBase):
     samAccountName: str | None = None
     mail: str | None = None
     telephoneNumber: str | None = None
     userAccountControl: int | None = None
 
 
 @dataclass
@@ -200,15 +183,14 @@
     inaccessibility_counter: int = 0
 
 @dataclass
 class WSResourceStatus(ResourceStatus):
     
     pass
 
-
 @dataclass
 class SiteResourceStatus(ResourceStatus, SiteResourceDescription):
     certificate_status: str | None = None
     free_space_status: str | None = None
 
 @dataclass
 class MarkBase:
@@ -228,22 +210,25 @@
 
 @dataclass
 class PolibasePersonBase:
     pin: int | None = None
     FullName: str | None = None
     telephoneNumber: str | None = None
 
-
 @dataclass
 class PolibasePerson(PolibasePersonBase):
     Birth: datetime | None = None
     Comment: str | None = None
     ChartFolder: str | None = None
-    mail: str | None = None
-
+    email: str | None = None
+    barcode: str | None = None 
+    registrationDate: datetime | None = None
+    telephoneNumber2: str | None = None
+    telephoneNumber3: str | None = None
+    telephoneNumber4: str | None = None
 
 @dataclass
 class PolibasePersonVisitDS(PolibasePersonBase):
     id: int | None = None
     registrationDate: str | None = None
     beginDate: str | None = None
     completeDate: str | None = None
@@ -270,14 +255,21 @@
 @dataclass
 class PolibasePersonVisitNotificationDS:
     visitID: int | None = None
     messageID: int | None = None
     type: int | None = None
 
 @dataclass
+class EventDS:
+    name: str | None = None
+    parameters: dict | None = None
+    timestamp: datetime | None = None
+
+
+@dataclass
 class Message:
     message: str | None = None
     recipient: str | None = None
     sender: str | None = None
 
 @dataclass
 class DelayedMessage(Message):
@@ -399,36 +391,41 @@
 
 
 @dataclass
 class WhatsAppMessageListPayload(WhatsAppMessagePayload):
     btn_text: str
     list: dict
 
+@dataclass
+class WhatsAppMessagebButton:
+
+    body: str | None = None
+    id: str | None = None
 
 @dataclass
 class WhatsAppMessageButtonsPayload(WhatsAppMessagePayload):
-    buttons: list | None = None
-
+    buttons: list[WhatsAppMessagebButton] | None = None
 
 @dataclass
 class TimeTrackingResultByDivision:
     name: str
     list: List[TimeTrackingResultByPerson] = field(
         default_factory=list)
 
 @dataclass
 class RobocopyJobDescription:
     name: str | None = None
     start_datetime: str | None = None
     host: str | None = None
     run_from_system_account: bool = False
     run_with_elevetion: bool = False
+    live: bool = False
    
-    def clone(self, job_name: str, start_datetime: str | None = None, host: str | None = None):
-        return RobocopyJobDescription(job_name, start_datetime, host or self.host, self.run_from_system_account, self.run_with_elevetion)
+    def clone(self, job_name: str, start_datetime: str | None = None, host: str | None = None, live: bool | None = None):
+        return RobocopyJobDescription(job_name, start_datetime, host or self.host, self.run_from_system_account, self.run_with_elevetion, self.live if live is None else live)
 
 
 @dataclass
 class RobocopyJobItem(RobocopyJobDescription):
     source: str | None = None
     destination: str | None = None
 
@@ -437,44 +434,78 @@
 class RobocopyJobStatus:
     name: str | None = None
     source: str | None = None
     destination: str | None = None
     active: bool = False
     last_created: str | None = None
     last_status: int | None = None
+    live: bool = False
+    pid: int = -1
 
 
 @dataclass
 class PrinterADInformation:
     driverName: str | None = None
     adminDescription: str | None = None
     description: str | None = None
     portName: str | None = None
     serverName: str | None = None
     name: str | None = None
 
 @dataclass
-class IndicationItem:
+class IndicationsContainer:
     timestamp: datetime | None = None
 
 @dataclass
-class THIndicationValue:
-    temperature: float | None = None
+class HumidityIndicationsValue:
     humidity: float | None = None
 
+
 @dataclass
-class CTIndicationValue(THIndicationValue):
+class TemparatureIndicationsValue:
+    temperature: float | None = None
+
+@dataclass
+class TemperatureAndHumidityIndicationsValue(HumidityIndicationsValue, TemparatureIndicationsValue):
     pass
 
+
+@dataclass
+class ChillerIndicationsValue(TemparatureIndicationsValue):
+    indicators: int = 0
+
+
 @dataclass
-class CTIndicationItem(CTIndicationValue, IndicationItem):
+class ChillerIndicationsValueContainer(ChillerIndicationsValue, IndicationsContainer):
     pass
 
 
 @dataclass
+class CTIndicationsValue(TemperatureAndHumidityIndicationsValue):
+    pass
+
+@dataclass
+class CTIndicationsValueContainer(CTIndicationsValue, IndicationsContainer):
+    pass
+
+@dataclass
+class GKeepMapItem:
+
+    name: str | None = None
+    id: str | None = None
+
+@dataclass
+class Note:
+
+    title: str | None = None
+    text: str | None = None
+    id: str | None = None
+    images: list[str] | None = None
+
+@dataclass
 class InventoryReportItem:
     name: str | None = None
     inventory_number: str | None = None
     row: str | None = None
     quantity: int | None = None
     name_column: int | None = None
     inventory_number_column: int | None = None
@@ -559,37 +590,78 @@
     alphabets_lowercase_count: int
     alphabets_uppercase_count: int
     digits_count: int = 1
     shuffled: bool = False
 
 
 @dataclass
-class LogCommandDescription:
+class EventDescription:
     message: str
-    log_channel: Enum
-    log_level: int
-    params: Tuple | None = None
+    channel: Enum
+    flags: int | tuple[Enum] | Enum | list[Enum] | list[int]
+    params: tuple | None = None
 
 
 @dataclass
+class ActionDescription:
+    name: str | None = None
+    alias: str | None = None
+    description: str | None = None
+    question: str | None = None
+    confirm: bool = True
+
+
+@dataclass
+class ActionWasDone:
+    action_description: str | None = None
+    action: Enum | str | None = None
+    user_name: str | None = None
+    user_login: str | None = None
+   
+
+@dataclass
 class ParamItem:
     name: str
     caption: str
     description: str | None = None
 
 
 @dataclass
-class SettingsValue:
+class StorageValue:
     key_name: str
-    default_value: Any
+    default_value: str | None
     description: str | None = None
     auto_init: bool = True
 
 
 @dataclass
+class IntStorageValue(StorageValue):
+    default_value: int = 0
+
+
+@dataclass
+class FloatStorageValue(StorageValue):
+    default_value: float
+
+@dataclass
+class BoolStorageValue(StorageValue):
+    default_value: bool
+
+
+@dataclass
+class TimeStorageValue(StorageValue):
+    default_value: str
+
+
+@dataclass
+class DateListStorageValue(StorageValue):
+    default_value: list[str]
+
+
+@dataclass
 class PolibaseScannedDocument:
     file_path: str
     pin: int
     document_name: str
 
 @dataclass
 class ThresholdedText:
```

### Comparing `pih-1.43/pih/console_api.py` & `pih-1.45/pih/console_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 import importlib.util
 import sys
 from subprocess import CompletedProcess
 from typing import Any
 from datetime import datetime
 import os
 
-pih_is_exists = importlib.util.find_spec("pih.pih") is not None
-if not pih_is_exists:
+pih_exists = importlib.util.find_spec("pih.pih") is not None
+if not pih_exists:
     sys.path.append("//pih/facade")
-from pih.const import CONST, MarkType, PASSWORD, USER_PROPERTY, FIELD_COLLECTION, PasswordSettings, CheckableSections, HOSTS, AD, PATHS, FILE
+from pih.const import CONST, MarkType, PASSWORD, USER_PROPERTIES, FIELD_COLLECTION, PasswordSettings, CheckableSections, HOSTS, AD, PATHS, FILE
 from pih import PIH, A, NotFound, ActionValue, ActionStack, Input, Output, Session, while_not_do
-from pih.tools import EnumTool, FullNameTool, ResultTool, DataTool, StringTool, DateTimeTool, PathTool
-from pih.collection import Mark, User, FullName, MarkDivision, UserContainer, LoginPasswordPair, MarkGroup, Result, FieldItemList, WorkstationDescription, ResourceStatus, SiteResourceStatus, CTIndicationValue, Workstation, RobocopyJobStatus
+from pih.collection import Mark, User, FullName, MarkDivision, UserBase, LoginPasswordPair, MarkGroup, Result, FieldItemList, WorkstationDescription, ResourceStatus, SiteResourceStatus, CTIndicationsValue, Workstation, RobocopyJobStatus, ChillerIndicationsValueContainer
 from pih import A
 
 class ConsoleAppsApi:
 
     LINE: str = "........................................................"
 
     def __init__(self, pih: PIH = None):
@@ -29,23 +28,23 @@
         self.login: str = None
         self.password: str = None
         self.internal_email: str = None
         self.external_email: str = None
         self.email_password: str = None
         self.polibase_login: str = None
         self.polibase_password: str = None
-        self.user_container: UserContainer
+        self.user_container: UserBase
         self.description: str = None
         self.use_template_user: bool
         self.need_to_create_mark: bool = None
 
     def create_qr_code_for_mobile_helper_command(self, command: str | None = None, title: str | None = None, show_result: bool = True) -> str | None:
         command = command or self.input.input("Введите название команды")
         title = title or self.input.input("Введите заголовок")
-        result = A.A_QR.for_mobile_helper_command(command, title, os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(command, FILE.EXTENSION.PNG))), 56)
+        result = A.A_QR.for_mobile_helper_command(command, title, os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, A.PTH.replace_prohibited_symbols_from_path_with_symbol(A.PTH.add_extension(command, FILE.EXTENSION.PNG))), 56)
         qr_code_image_path: str = A.PTH_QR.mobile_helper_command(command)
         if show_result:
             if result:
                 self.output.good(
                     f"Файл qr кода {self.bold(title)} создан.\nПуть к файлу:\n{self.bold(qr_code_image_path)}\n")
             else:
                 self.output.error("qr код не был создан")
@@ -76,47 +75,66 @@
                     if resource.check_free_space_status:
                         free_space_result_list: str = resource.free_space_status.split(" ")
                         result.append(f"Cвободное место: {free_space_result_list[0]} ({free_space_result_list[1]})")
                     if resource.check_certificate_status:
                         result.append(f"Сертификат доступен до: {resource.certificate_status}")
                     result.append(ConsoleAppsApi.LINE)
                     result.append(status)
-                return "\n".join(result)
+                return A.CT.NEW_LINE.join(result)
             force_update = force_update or (ask_for_update_before and self.input.yes_no(
                 "Обновить перед получением"))
             if force_update:
                 self.output.write_line(
                     self.italic(f"{self.get_formatted_given_name()}, ожидайте получение результата..."))
             for checkable_section in [CheckableSections.RESOURCES, CheckableSections.WS]:
                 if checkable_section in checkable_section_list:
                     self.output.new_line()
-                    self.output.write_result(A.R_R.get_status_list([checkable_section], force_update, all if len(checkable_section_list) == 1 and CheckableSections.WS in checkable_section_list else False), False, label_function=label_function, separated_result_item=True, title = (self.output.bold(CONST.VISUAL.BULLET + (" Основные ресурсы" if checkable_section == CheckableSections.RESOURCES else " Наблюдаемые компьютеры")) ) if all else None )
+                    if all:
+                        self.output.write_line(self.bold(CONST.VISUAL.BULLET + (" Основные ресурсы" if checkable_section == CheckableSections.RESOURCES else " Наблюдаемые компьютеры")))
+                    with self.output.make_indent(2):
+                        self.output.write_result(A.R_R.get_status_list([checkable_section], force_update, all if len(checkable_section_list) == 1 and CheckableSections.WS in checkable_section_list else False), False, label_function=label_function, separated_result_item=True)
         if CheckableSections.INDICATIONS in checkable_section_list:
+            #self.output.separated_line()
+            #self.output.write_line(f"Показания доступны по адрессу:\n{self.bold('http://indications')}, если заходить с рабочего компьютера\nили\n{self.bold('http://192.168.100.138')}, если заходить с мобильного телефона, подключенного к корпоративной wifi сети")
             self.output.new_line()
-            self.output.write_result(A.R_I.get_last_items(), title=self.output.bold((CONST.VISUAL.BULLET + " " if all else "") + "Показания в помещение КТ"))
+            self.output.write_line(self.bold(f"{CONST.VISUAL.BULLET} Показания в помещении КТ"))
+            with self.output.make_indent(2):
+                self.output.write_result(A.R_I.last_ct_value_containers(True))
+            self.output.separated_line()
+            self.output.write_line(self.bold(f"{CONST.VISUAL.BULLET} Показания в техническом помещении МРТ"))
+            chiller_indications_value_container_result: Result[list[ChillerIndicationsValueContainer]] = A.R_I.last_chiller_value_containers(True)
+            chiller_indications_value_container: ChillerIndicationsValueContainer = A.R.get_first_element(chiller_indications_value_container_result)
+            path: str = A.PTH_I.CHILLER_DATA_IMAGE_LAST
+            modification_timstamp: float = os.path.getmtime(path)
+            modification_datetime: datetime | None = datetime.fromtimestamp(modification_timstamp if modification_timstamp > 0 else os.path.getctime(path))
+            with self.output.make_indent(2):
+                self.output.write_result(chiller_indications_value_container_result, title="Показания чиллера\n" if A.D_C.INDICATIONS.chiller_value_actual(chiller_indications_value_container) else f"{self.bold('Внимание!')}: Показания чиллера неактуальны\n", separated_result_item=False)
+                self.output.write_image(f"Изображение дисплея чиллера\nВремя снятия: {A.D_F.datetime(modification_datetime)}", A.D_CO.file_to_base64(A.PTH_I.CHILLER_DATA_IMAGE_LAST_RESULT))
         if not all:
             if CheckableSections.BACKUPS in checkable_section_list:
                 robocopy_job_status_list: Result[list[RobocopyJobStatus]] = A.R_B.robocopy_job_status_list()
+                sort_by_status: bool = self.input.yes_no("Сортировать по статусу", no_label=f"{self.bold(f'Сортировать по дате выполнения - {A.CT_V.NUMBER_SYMBOLS[0]}')}")
+                A.R.sort(robocopy_job_status_list, (lambda item: item.last_status or max(A.CT_RBK.STATUS_CODE.keys())) if sort_by_status else lambda item: datetime.fromtimestamp(0) if A.D_C.empty(item.last_created) else A.D.datetime_from_string(item.last_created), sort_by_status)
                 def job_status_item_label_function(job_status: RobocopyJobStatus, index: int) -> str:
                     name: str = job_status.name
                     source: str = job_status.source
                     destination: str = job_status.destination 
                     status: int | None = None
                     date: str | None = None
                     if job_status.active:
                         date = "выполняется"
                     else:
                         if job_status.last_created is not None:
                             date = f"{A.D_F.datetime(job_status.last_created)}"
                         status = job_status.last_status
-                    return f" {CONST.VISUAL.BULLET} {self.bold(f'{name}:{source}{CONST.VISUAL.ARROW}{destination}')}" + ("" if status is None else f" [ {self.bold(str(status))} ]") + ("" if A.D_C.empty(date) else f"\n   {date}")
+                    variants: list[str] = ["--" if status is None else self.bold(str(status)), "--" if A.D_C.empty(date) else self.bold(date)]
+                    return "".join([f" {CONST.VISUAL.BULLET} ", variants[not sort_by_status], ": ", variants[sort_by_status], "".join([ "\n   ", name, ": ", source, CONST.VISUAL.ARROW, destination])])
+                variants: list[str] = [self.bold("Статус"), self.bold("Дата выполнения")]
                 self.output.write_result(
-                    robocopy_job_status_list, False, label_function=job_status_item_label_function, separated_result_item=False, title=f" {CONST.VISUAL.BULLET} {self.bold('Название работы')}" + f" [ {self.bold('Статус')} ]" + f"\n   Дата создания\n{ConsoleAppsApi.LINE}")
-                
-
+                    robocopy_job_status_list, False, label_function=job_status_item_label_function, separated_result_item=False, title="".join([f" {CONST.VISUAL.BULLET} ", variants[not sort_by_status], ": ", variants[sort_by_status], "\n", "   Название Robocopy-задания", f"\n{ConsoleAppsApi.LINE}"]))
 
     def polibase_restart(self, forced: bool = False) -> None:
         if self.input.yes_no("Перезапустить"):
             check_word: str = CONST.POLIBASE.NAME
             test: bool = not (check_word == self.input.input(
                 f"Введите контрольное слово: {self.bold(check_word)}"))
             if not test and A.C_R.polibase_accessibility(True) and not forced:
@@ -124,61 +142,71 @@
                     "Перезапуск Polibase: перезапуск невозможен - сервер доступен")
             else:
                 notify: bool = test or self.input.yes_no("Уведомить пользователей", True)
                 title: str = f"Перезапуск Polibase{' test' if test else ''}"
                 polibase_host: str = HOSTS.POLIBASE_TEST.NAME if test else HOSTS.POLIBASE.NAME
                 self.output.write_line(A.L.it(
                     f"{title}: Начат процесс закрытия программы Polibase на компьютерах."))
-                A.A_P.program_close_for_all(notify, None, test)
+                A.A_P.client_program_close_for_all(notify, None, test)
                 self.output.new_line()
                 self.output.write_line(A.L.it(
                     f"{title}: Начат процесс перезагрузки сервера Polibase."))
                 A.A_P.restart(test)
                 while_not_do(lambda: not A.C_R.accessibility_by_ping(
                     polibase_host), sleep_time=5)
                 self.output.new_line()
                 self.output.write_line(A.L.it(
                      f"{title}: Начат процесс загрузки сервера Polibase."))
                 while_not_do(lambda: A.C_R.accessibility_by_ping(polibase_host), sleep_time=5)
                 self.output.new_line()
-                A.EV.wait_server_start(polibase_host)
+                A.E.wait_server_start(polibase_host)
                 self.output.write_line(A.L.it(f"{title}: Завершен процесс загрузки сервера Polibase."))
                 A.ME_P.notify_about_polibase_restarted(test)
 
-    def polibase_client_program_close(self, search_value: str | None = None) -> None:
-        for_all: bool = self.input.yes_no("Закрыть для всех пользователей", False, no_label=self.bold("Введите запрос для поиска компьютера"))
+    def polibase_client_program_close(self, search_value: str | None = None, for_all: bool = False) -> None:
         if for_all:
             check_word: str = CONST.POLIBASE.NAME
-            test: bool = not (check_word == self.input.input(
-            f"Введите контрольное слово: {self.bold(check_word)}"))
-            A.A_P.program_close_for_all(True, self.input.input("Введите сообщение для пользователей Polibase"), test) 
+            test: bool = not (check_word == (search_value or self.input.input(
+            f"Введите контрольное слово - {self.bold(check_word)}")))
+            A.A_P.client_program_close_for_all(True, self.input.input("Введите сообщение для пользователей Polibase"), test) 
         else:
-            search_value = self.input.answer
-            workstation_list: list[Workstation] | None = None
             try:
-                workstation_list = A.R_WS.by_any(search_value or self.input.input("Введите запрос для поиска компьютера"))
+                workstation_list: Result[list[Workstation]] = A.R_WS.by_any(search_value or self.input.input("Введите запрос для поиска компьютера"))
                 def every_action(workstation: Workstation) -> None:
                     if A.A_P.client_program_close_for_workstation(workstation):
                         self.output.good(f"Программа Polibase закрыта на компьютере {workstation.name}")
-                ResultTool.every(workstation_list, every_action)
+                A.R.every(workstation_list, every_action)
             except NotFound as error:
                 self.output.error(error.get_details())
+                search_value = None
+
+    def process_kill(self, host_name: str, process_name: str) -> None:
+        try:
+            workstation_list: Result[list[Workstation]] = A.R_WS.by_any(host_name or self.input.input("Введите запрос для поиска компьютера"))
+            def every_action(workstation: Workstation, process_name: str) -> None:
+                if A.A_WS.kill_process_via_taskkill(process_name, workstation.name):
+                    self.output.good(f"Программа {process_name} закрыта на компьютере {workstation.name}")
+            A.R.every(workstation_list, lambda workstation: every_action(workstation, process_name or self.input.input("Введите название процесса")))
+        except NotFound as error:
+            self.output.error(error.get_details())
+            host_name = None
+
        
     @property
     def output(self) -> Output:
         return self.pih.output
 
     @property
     def input(self) -> Input:
         return self.pih.input
 
     def send_whatsapp_message(self, telephone_number: str, message: str) -> bool:
         return A.ME_WH_W.send(telephone_number, message, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.IT)
 
-    def mark_find(self, value: str = None) -> None:
+    def mark_find(self, value: str | None = None) -> None:
         self.output.mark.by_any(value or self.input.mark.any())
 
     def arg(self, index: int = 0, default_value: Any = None) -> Any:
         return self.session.arg(index, default_value)
 
     def register_ct_indications(self) -> None:
         text: str = f"число, которое может содержать дробную часть разделенную {self.bold('точкой')} или {self.bold('запятой')}"
@@ -191,19 +219,19 @@
                 self.output.error(
                     f"Введите {self.bold('число')} {number_format_notification_text}")
             return None if result is None else str(result)
         temperature: float = float_check_function(self.arg(), False) or self.input.input(
             f"Введите значение {self.bold('температуры')} {number_format_notification_text}", check_function=float_check_function)
         humidity: float = float_check_function(self.arg(1), False) or self.input.input(
             f"Введите значение {self.bold('влажности')} {number_format_notification_text}", check_function=float_check_function)
-        indication: CTIndicationValue = CTIndicationValue(temperature, humidity)
-        if A.A_I_CT.register(indication):
-            with self.output.send_to_group(CONST.MESSAGE.WHATSAPP.GROUP.RD_INDICATIONS):
+        indications_value: CTIndicationsValue = CTIndicationsValue(temperature, humidity)
+        if A.A_I_CT.register(indications_value):
+            with self.output.send_to_group(CONST.MESSAGE.WHATSAPP.GROUP.CT_INDICATIONS):
                 self.output.write_result(
-                    Result(FIELD_COLLECTION.INDICATIONS.CT, indication), title=f"{self.get_formatted_given_name()}, отправил следующие показания в помещение КТ:")
+                    Result(FIELD_COLLECTION.INDICATIONS.CT_VALUE, indications_value), title=f"{self.get_formatted_given_name()}, отправил следующие показания в помещение КТ:")
             self.output.good("Спасибо, показания отправлены")
 
     def find_free_mark(self, value: str = None) -> None:
         self.output.mark.result(A.R_M.by_any(
             value or self.input.mark.any()), "Список свободных карт доступа:")
 
     def find_user(self, value: str = None) -> None:
@@ -228,45 +256,45 @@
         if self.input.yes_no("Отправить в ИТ отдел"):
             A.L.it(f"Сгенерированный пароль:")
             A.L.it(password)
         return password
 
     def make_mark_as_free(self, value: str = None) -> None:
         mark: Mark = self.input.mark.by_any(value)
-        mark_type: int = EnumTool.get(MarkType, mark.type)
+        mark_type: int = A.D.get(MarkType, mark.type)
         if mark_type == MarkType.FREE:
             self.output.error(
                 "Карта доступа с введенным номером уже свободная")
         else:
             if self.input.yes_no("Сделать карту свободной"):
                 if mark_type == MarkType.TEMPORARY:
                     temporary_tab_number: int = mark.TabNumber
                     mark = A.R_M.temporary_mark_owner(
                         mark).data
                 if A.A_M.make_as_free_by_tab_number(mark.TabNumber):
                     if mark_type == MarkType.TEMPORARY:
-                        A.L_C.it_notify_about_temporary_mark_return(
+                        A.E.it_notify_about_temporary_mark_return(
                             mark, temporary_tab_number)
                     else:
-                        A.L_C.it_notify_about_mark_return(mark)
+                        A.E.it_notify_about_mark_return(mark)
                     self.output.good(
                         f"Карта доступа с номером {mark.TabNumber} стала свободной")
                 else:
                     self.output.error("Ошибка")
             else:
                 self.output.error("Отмена")
 
     def who_lost_the_mark(self, tab_number: str = None):
         try:
             tab_number = tab_number or self.input.tab_number()
             if tab_number is not None:
                 try:
                     mark: Mark = self.pih.RESULT.MARK.by_tab_number(
                         tab_number).data
-                    mark_type: MarkType = EnumTool.get(MarkType, mark.type)
+                    mark_type: MarkType = A.D.get(MarkType, mark.type)
                     if mark_type == MarkType.FREE:
                         self.output.good("Это свободная карта доступа")
                     elif mark_type == MarkType.GUEST:
                         self.output.good("Это гостевая карта доступа")
                     else:
                         if mark_type == MarkType.TEMPORARY:
                             mark = self.pih.RESULT.MARK.temporary_mark_owner(
@@ -286,15 +314,15 @@
                             else:
                                 self.output.value(
                                     "Телефон", telephone_number)
                                 if self.input.yes_no("Отправить сообщение", True):
                                     details: str = self.input.input(
                                         f"{self.get_formatted_given_name()}, уточните, где забрать найденную карту")
                                     if self.send_whatsapp_message(
-                                            telephone_number, f"День добрый, {FullNameTool.to_given_name(mark.FullName)}, вашу карту доступа ({tab_number}) нашли, заберите ее {details}"):
+                                            telephone_number, f"День добрый, {A.D.to_given_name(mark.FullName)}, вашу карту доступа ({tab_number}) нашли, заберите ее {details}"):
                                         self.output.good(
                                             "Сообщение отправлено")
                                     else:
                                         self.output.error(
                                             "Ошибка при отправке сообщения")
                         else:
                             self.output.error("Телефон не указан")
@@ -310,15 +338,15 @@
     def italic(self, value: str) -> str:
         return self.output.italic(value)
 
     def run_command(self, command_list: list[str] = None) -> None:
         default_host: str = CONST.HOST.DC2.NAME
         host: str = None
         def get_command_list() -> list[str]:
-            command_list: tuple[list[str], list[str]] = StringTool.dequotes(
+            command_list: tuple[list[str], list[str]] = A.D.dequotes(
                 self.pih.input.input("Введите команду"))
             return list(filter(lambda item: not A.D_C.empty(item), command_list[0] + command_list[1]))
         command_list = command_list or get_command_list()
         use_psexec: bool = A.D_C.empty([value for value in list(map(
             lambda item: item.lower(), command_list)) if value in CONST.PSTOOLS.COMMAND_LIST])
         result: CompletedProcess = None
         if use_psexec:
@@ -359,22 +387,22 @@
         self.tab_number = None
         self.telephone_number = None
         self.division_id = None
 
         def get_full_name() -> ActionValue:
             self.output.header("Заполните ФИО персоны")
             self.full_name = self.input.full_name(True)
-            user_is_exsits: bool = not self.pih.CHECK.MARK.exists_by_full_name(
+            user_exists: bool = not self.pih.CHECK.MARK.exists_by_full_name(
                 self.full_name)
-            if user_is_exsits:
+            if user_exists:
                 self.output.error(
                     "Персона с данной фамилией, именем и отчеством уже есть!")
                 if not self.input.yes_no("Продолжить"):
                     self.session.exit()
-            return self.output.get_action_value("ФИО персоны", FullNameTool.to_string(self.full_name))
+            return self.output.get_action_value("ФИО персоны", A.D.fullname_to_string(self.full_name))
 
         def get_telephone_number() -> ActionValue:
             self.output.header("Заполните номер телефона")
             self.telephone_number = self.input.telephone_number()
             return self.output.get_action_value("Номер телефона", self.telephone_number, False)
 
         def get_tab_number() -> ActionValue:
@@ -398,19 +426,19 @@
                     get_tab_number,
                     input=self.input,
                     output=self.output
                     )
         if self.input.yes_no("Создать карту доступа для персоны", True):
             if self.pih.ACTION.MARK.create(self.full_name, self.division_id, self.tab_number, self.telephone_number):
                 self.output.good("Карты доступа создана!")
-                self.pih.LOG.COMMAND.it_notify_about_create_new_mark(
+                self.pih.EVENT.it_notify_about_create_new_mark(
                     self.full_name)
                 if self.input.yes_no("Уведомить персону", True):
                     self.send_whatsapp_message(
-                        self.telephone_number, f"Сообщение от ИТ отдела Pacific International Hospital: День добрый, {FullNameTool.to_given_name(self.full_name)}, Вам выдана карта доступа с номером {self.tab_number}")
+                        self.telephone_number, f"Сообщение от ИТ отдела Pacific International Hospital: День добрый, {A.D.to_given_name(self.full_name)}, Вам выдана карта доступа с номером {self.tab_number}")
             else:
                 self.output.error("Карта доступа не создана!")
 
     def send_workstation_message_to_all(self) -> None:
         message: str = self.input.message(
             f"{self.get_formatted_given_name()}, введите сообщение для всех пользователей")
         A.ME_WS.to_all_workstations(
@@ -424,42 +452,42 @@
     def user_description(self) -> str:
         return A.D_F.description(self.user.description)
 
     def send_workstation_message(self, recipient_name: str = None, message: str | None = None, ask_for_use_dialog: bool = True) -> None:
         recipient: User | WorkstationDescription = None
         while True:
             try:
-                recipient = DataTool.get_first_item(
+                recipient = A.D.get_first_item(
                     self.input.user.by_any(recipient_name, True))
                 if recipient is not None:
                     break
             except NotFound as error:
                 value: str = error.get_value()
                 if A.C_WS.name(value):
                     if A.C_WS.exists(value):
                         recipient = A.R_WS.by_name(value).data
                         break
                 if recipient is None:
                     recipient_name = None
                     self.output.error(error.get_details())
-        if isinstance(recipient, User) and ResultTool.is_empty(A.R_WS.by_login(recipient.samAccountName)):
+        if isinstance(recipient, User) and A.R.is_empty(A.R_WS.by_login(recipient.samAccountName)):
             self.output.error(
                 f"Пользователь {recipient.name} ({recipient.samAccountName}) не залогинен ни за одним компьютером.")
         else:
             try:
                 use_dialog: bool = False
                 if ask_for_use_dialog:
                     use_dialog = A.D_C.empty(message) and self.input.yes_no("Начать диалог")
                 else:
                     use_dialog = True
                 while True:
                     user_given_name: str = self.get_formatted_given_name(self.user_given_name)
                     if isinstance(recipient, User):
                         message = message or self.input.message(
-                            f"{user_given_name}, введите сообщение для пользователя {self.get_formatted_given_name(FullNameTool.to_given_name(recipient))}", f"Сообщение от {self.user_given_name} ({self.user_description}): {FullNameTool.to_given_name(recipient)}, ")
+                            f"{user_given_name}, введите сообщение для пользователя {self.get_formatted_given_name(A.D.to_given_name(recipient))}", f"Сообщение от {self.user_given_name} ({self.user_description}): {A.D.to_given_name(recipient)}, ")
                         if A.ME_WS.to_user(recipient, message):
                             self.output.good("Сообщение отправлено")
                     else:
                         message =  message or self.input.message(
                             f"{user_given_name}, введите сообщение для компьютера {recipient.name}", f"Сообщение от {self.user_given_name} ({self.user_description}): ")
                         if A.ME_WS.to_workstation(recipient, message):
                             self.output.good("Сообщение отправлено")
@@ -474,15 +502,15 @@
                 else:
                     self.output.error("Отмена...")
 
     @property
     def user_given_name(self) -> str:
         return self.session.user_given_name
     
-    def get_formatted_given_name(self, value: str = None) -> str:
+    def get_formatted_given_name(self, value: str | None = None) -> str:
         return self.output.user.get_formatted_given_name(value or self.user_given_name)
 
     def create_temporary_mark(self, owner_mark: Mark = None) -> None:
         owner_mark = owner_mark or self.input.mark.by_any()
         mark_group: MarkGroup = None
         if self.input.yes_no("Выдать временную карту доступа из той же группы доступа"):
             mark_group = owner_mark
@@ -490,18 +518,18 @@
         self.output.temporary_candidate_for_mark(temporary_mark)
         full_name: str = owner_mark.FullName
         tab_number: str = temporary_mark.TabNumber
         if self.input.yes_no(f"Создать временную карту для {full_name} с табельным номеров {tab_number}", True):
             if A.A_M.make_as_temporary(temporary_mark, owner_mark):
                 self.output.good("Временная карта создана")
                 telephone_number: str = owner_mark.telephoneNumber
-                A.L_C.it_notify_about_create_temporary_mark(
+                A.Eit_notify_about_create_temporary_mark(
                     full_name, tab_number)
                 if not A.C.telephone_number(telephone_number):
-                    user: User = ResultTool.get_first_element(A.R_U.by_any(
+                    user: User = A.R.get_first_element(A.R_U.by_any(
                         owner_mark))
                     if user is not None:
                         telephone_number = user.telephoneNumber
                 if A.C.telephone_number(telephone_number):
                     if self.input.yes_no("Уведомить персону", True):
                         self.send_whatsapp_message(
                             telephone_number, f"Сообщение от ИТ отдела: День добрый, {self.get_formatted_given_name(full_name)}, Вам выдана временная карта доступа с номером {tab_number}")
@@ -553,36 +581,36 @@
                     f"{user.name}, похоже не пользователь, у которого должен быть номер телефона")
 
     def start_user_property_setter(self, property_name: str, search_value: str = None, choose_user: bool = False) -> None:
         try:
             user_list: list[User] = None
             fields: FieldItemList = FIELD_COLLECTION.AD.USER
             active: bool | None = True if (
-                property_name == USER_PROPERTY.PASSWORD or property_name == USER_PROPERTY.TELEPHONE_NUMBER) else None
+                property_name == USER_PROPERTIES.PASSWORD or property_name == USER_PROPERTIES.TELEPHONE_NUMBER) else None
             if choose_user:
                 user_list = self.input.user.by_any(search_value, active)
             else:
                 result: Result[list[User]] = A.R_U.by_any(
                     self.input.user.title_any(), active)
                 user_list = result.data
-            if property_name == USER_PROPERTY.USER_STATUS:
+            if property_name == USER_PROPERTIES.USER_STATUS:
                 for status in [AD.ACTIVE_USERS_CONTAINER_DN, AD.INACTIVE_USERS_CONTAINER_DN]:
                     work_user_list: list[User] = self.pih.DATA.FILTER.users_by_dn(
                         user_list, AD.INACTIVE_USERS_CONTAINER_DN if status == AD.ACTIVE_USERS_CONTAINER_DN else AD.ACTIVE_USERS_CONTAINER_DN)
                     for index, user in enumerate(work_user_list):
                         try:
                             self.output.user.result(Result(fields, [user]))
                             if self.input.yes_no(f"{'Активировать' if status == AD.ACTIVE_USERS_CONTAINER_DN else 'Деактивировать' } пользователя"):
                                 if status == AD.ACTIVE_USERS_CONTAINER_DN:
                                     if self.input.yes_no("Использовать шаблон для пользователя", True):
                                         user_container = self.input.user.template()
                                     else:
                                         user_container = self.input.user.container()
                                 else:
-                                    user_container = UserContainer(
+                                    user_container = UserBase(
                                         distinguishedName=AD.INACTIVE_USERS_CONTAINER_DN)
                                 if self.pih.ACTION.USER.set_status(user, status, user_container):
                                     self.output.good("Успешно")
                                 else:
                                     self.output.error("Ошибка")
                             else:
                                 self.output.new_line()
@@ -593,26 +621,26 @@
                                 self.output.error("Отмена")
                             else:
                                 self.output.error("Отмена - следующий")
                             self.output.new_line()
             else:
                 for index, user in enumerate(user_list):
                     try:
-                        if property_name == USER_PROPERTY.TELEPHONE_NUMBER:
+                        if property_name == USER_PROPERTIES.TELEPHONE_NUMBER:
                             self.output.user.result(
                                 Result(fields, [user]), None)
                             telephone = self.input.telephone_number()
                             if self.pih.CHECK.telephone_number(telephone) and self.input.yes_no("Установить", True):
                                 if self.pih.ACTION.USER.set_telephone_number(user, telephone):
                                     self.output.good("Успешно")
                                 else:
                                     self.output.error("Ошибка")
                             else:
                                 self.output.error("Отмена")
-                        elif property_name == USER_PROPERTY.PASSWORD:
+                        elif property_name == USER_PROPERTIES.PASSWORD:
                             self.output.user.result(
                                 Result(fields, [user]), "Пользователи:")
                             password: str = None
                             while True:
                                 password = self.input.user.generate_password(True, PASSWORD.get(
                                     self.input.indexed_field_list("Выберите тип пароля", FIELD_COLLECTION.POLICY.PASSWORD_TYPE)))
                                 self.output.value("Пароль", password)
@@ -662,15 +690,15 @@
             self.user_is_exists = self.pih.CHECK.USER.exists_by_full_name(
                 self.full_name)
             if self.user_is_exists:
                 self.output.error(
                     "Пользователем с данной фамилией, именем и отчеством уже есть!")
                 if not self.input.yes_no("Продолжить"):
                     self.session.exit()
-            return self.output.get_action_value("ФИО пользователя", FullNameTool.to_string(self.full_name))
+            return self.output.get_action_value("ФИО пользователя", A.D.fullname_to_string(self.full_name))
 
         def get_login() -> ActionValue:
             self.output.header("Создание логина для аккаунта пользователя")
             self.login = self.input.user.generate_login(self.full_name)
             return self.output.get_action_value("Логин пользователя", self.login)
 
         def get_telephone_number() -> ActionValue:
@@ -699,15 +727,15 @@
             self.password = self.input.user.generate_password(
                 settings=PASSWORD.SETTINGS.PC)
             return self.output.get_action_value("Пароль", self.password, False)
 
         def get_internal_email() -> ActionValue:
             self.output.header("Создание корпоративной электронной почты")
             if self.input.yes_no("Создать", True):
-                self.internal_email = A.D.create_email(self.login)
+                self.internal_email = A.D_F.email(self.login, add_default_domain = True)
             return self.output.get_action_value("Адресс корпоративной электронной почты пользователя", self.internal_email)
 
         def get_email_password() -> ActionValue:
             if self.internal_email:
                 self.output.header(
                     "Создание пароля для корпоротивной электронной почты")
                 if self.input.yes_no("Использовать пароль от аккаунта пользователя", True):
@@ -721,15 +749,15 @@
         def get_external_email() -> ActionValue:
             self.output.header("Добавление внешней почты")
             if self.input.yes_no("Добавить"):
                 self.external_email = self.input.email()
             return self.output.get_action_value("Адресс внешней электронной почты пользователя", self.external_email if self.external_email else "Нет", False)
 
         def get_division() -> ActionValue:
-            full_name_string: str = FullNameTool.to_string(self.full_name)
+            full_name_string: str = A.D.fullname_to_string(self.full_name)
             mark: Mark = self.pih.RESULT.MARK.by_name(
                 full_name_string, True).data
             if mark is not None:
                 if self.input.yes_no(
                         f"Найдена карта доступа для персоны {full_name_string} с номером {mark.TabNumber}. Использовать", True):
                     self.need_to_create_mark = False
                     return None
@@ -775,26 +803,26 @@
                 self.pih.ACTION.USER.create_from_template(
                     self.user_container.distinguishedName, self.full_name, self.login, self.password, self.description, self.telephone_number, self.internal_email or self.external_email)
             else:
                 self.pih.ACTION.USER.create_in_container(
                     self.user_container.distinguishedName, self.full_name, self.login, self.password, self.description, self.telephone_number, self.internal_email or self.external_email)
             if self.need_to_create_mark:
                 self.tab_number = self.tab_number or self.pih.RESULT.MARK.by_name(
-                    FullNameTool.to_string(self.full_name), True).data.TabNumber
+                    A.D.fullname_to_string(self.full_name), True).data.TabNumber
                 self.pih.ACTION.MARK.create(
                     self.full_name, self.division_id, self.tab_number, self.telephone_number)
             user_account_document_path: str = self.pih.PATH.USER.get_document_name(
-                FullNameTool.to_string(self.full_name), self.login if self.user_is_exists else None)
+                A.D.fullname_to_string(self.full_name), self.login if self.user_is_exists else None)
             if self.pih.ACTION.DOCUMENTS.create_for_user(user_account_document_path, self.full_name, self.tab_number, LoginPasswordPair(self.login, self.password), LoginPasswordPair(
                     polibase_login, polibase_password), LoginPasswordPair(self.internal_email, self.email_password)):
-                self.pih.LOG.COMMAND.hr_notify_about_new_employee(self.login)
-                self.pih.LOG.COMMAND.it_notify_about_user_creation(
+                self.pih.EVENT.hr_notify_about_new_employee(self.login)
+                self.pih.EVENT.it_notify_about_user_creation(
                     self.login, self.password)
                 if self.need_to_create_mark:
-                    self.pih.LOG.COMMAND.it_notify_about_create_new_mark(
+                    self.pih.EVENT.it_notify_about_create_new_mark(
                         self.full_name)
                 if self.input.yes_no("Сообщить пользователю о создании документов", True):
                     self.send_whatsapp_message(
-                        self.telephone_number, f"Сообщение от ИТ отдела Pacific International Hospital: День добрый, {FullNameTool.to_given_name(self.full_name)}, Вас ожидает документы и карта доступа с номером {self.tab_number} в отделе")
+                        self.telephone_number, f"Сообщение от ИТ отдела Pacific International Hospital: День добрый, {A.D.to_given_name(self.full_name)}, Вас ожидает документы и карта доступа с номером {self.tab_number} в отделе")
                 if self.input.yes_no("Отправить пользователю данные об аккаунте", True):
                     self.send_whatsapp_message(
-                        self.telephone_number, f"Сообщение от ИТ отдела Pacific International Hospital: День добрый, {FullNameTool.to_given_name(self.full_name)}, данные Вашего аккаунта:\nЛогин: {self.login}\nПароль: {self.password}\nЭлектронная почта: {self.internal_email}")
+                        self.telephone_number, f"Сообщение от ИТ отдела Pacific International Hospital: День добрый, {A.D.to_given_name(self.full_name)}, данные Вашего аккаунта:\nЛогин: {self.login}\nПароль: {self.password}\nЭлектронная почта: {self.internal_email}")
```

### Comparing `pih-1.43/pih/const.py` & `pih-1.45/pih/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 ﻿from enum import *
 import os
 
-from pih.collection import FieldItem, FieldItemList, LogCommandDescription, ParamItem, PasswordSettings, ServiceRoleDescription, SettingsValue, ResourceDescription, SiteResourceDescription, PolibaseDocumentDescription, MedicalDirectionDescription
+from pih.collection import FieldItem, FieldItemList, EventDescription, ParamItem, PasswordSettings, StorageValue, ResourceDescription, SiteResourceDescription, PolibaseDocumentDescription, MedicalDirectionDescription, ActionDescription, IntStorageValue, BoolStorageValue, TimeStorageValue, DateListStorageValue, FloatStorageValue
+from pih.rpc_collection import ServiceDescription, ServiceInformationBase
+from pih.rpc_const import ServiceCommands
 
 class DATA:
 
     #deprecated
     class EXTRACTOR:
 
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
 
-    class FORMATTER:
+    class FORMATTER(Enum):
 
         MY_DATETIME: str = "my_datetime"
+        MY_DATE: str = "my_date"
+        CHILLER_INDICATIONS_VALUE_INDICATORS: str = "chiller_indications_value_indicators"
+        CHILLER_FILTER_COUNT: str = "chiller_filter_count"
+
+class INDICATIONS:
+
+    class CHILLER:
+
+        ACTUAL_VALUES_TIME_DELTA_IN_MINUTES: int = 5
+
+        INDICATOR_NAME: list[str] = [
+            "Активный сигнал тревоги",
+            "Работает нагреватель",
+            "Замораживание включено",
+            "Работает вентилятор конденсатора",
+            "Работает насос/вытяжной вентилятор",
+            "Работает компрессор"
+        ]
+
+        INDICATOR_EMPTY_DISPLAY: int = -1
 
 
-class USER_PROPERTY:
+class USER_PROPERTIES:
 
     TELEPHONE_NUMBER: str = "telephoneNumber"
     EMAIL: str = "mail"
     DN: str = "distinguishedName"
     USER_ACCOUNT_CONTROL: str = "userAccountControl"
     LOGIN: str = "samAccountName"
     DESCRIPTION: str = "description"
@@ -32,30 +54,29 @@
 class BARCODE:
 
     CODE128: str = "code128"
     I25: str = "i25"
 
 class AD:
 
-    SEARCH_ATTRIBUTES: list[str] = [
-        USER_PROPERTY.LOGIN, USER_PROPERTY.NAME]
+    SEARCH_ATTRIBUTES: list[str] = [USER_PROPERTIES.LOGIN, USER_PROPERTIES.NAME]
     SEARCH_ATTRIBUTE_DEFAULT: str = SEARCH_ATTRIBUTES[0]
     DOMAIN_NAME: str = "fmv"
     DOMAIN_ALIAS: str = "pih"
     DOMAIN_SUFFIX: str = "lan"
-    DOMAIN: str = f"{DOMAIN_NAME}.{DOMAIN_SUFFIX}"
+    DOMAIN: str = ".".join([DOMAIN_NAME, DOMAIN_SUFFIX])
     DOMAIN_MAIN: str = DOMAIN
     USER_HOME_FOLDER_DISK: str = "U:"
     OU: str = "OU="
     ROOT_CONTAINER_DN: str = f"{OU}Unit,DC={DOMAIN_NAME},DC={DOMAIN_SUFFIX}"
     WORKSTATIONS_CONTAINER_DN: str = f"{OU}Workstations,{ROOT_CONTAINER_DN}"
     USERS_CONTAINER_DN_SUFFIX: str = f"Users,{ROOT_CONTAINER_DN}"
     ACTIVE_USERS_CONTAINER_DN: str = f"{OU}{USERS_CONTAINER_DN_SUFFIX}"
     INACTIVE_USERS_CONTAINER_DN: str = f"{OU}dead{USERS_CONTAINER_DN_SUFFIX}"
-    PATH_ROOT: str = f"\\\{DOMAIN_MAIN}"
+    PATH_ROOT: str = f"\\\\{DOMAIN_MAIN}"
     SEARCH_ALL_PATTERN: str = "*"
     GROUP_CONTAINER_DN: str = f"{OU}Groups,{ROOT_CONTAINER_DN}"
     JOB_POSITION_CONTAINER_DN: str = f"{OU}Job positions,{GROUP_CONTAINER_DN}"
     LOCATION_JOINER: str = ":"
     TEMPLATED_USER_SERACH_TEMPLATE: str = "_*_"
     PROPERTY_ROOT_DN: str = f"{OU}Property,{GROUP_CONTAINER_DN}"
     PROPERTY_WS_DN: str = f"{OU}WS,{PROPERTY_ROOT_DN}"
@@ -92,17 +113,20 @@
 
     WORKSTATION_PREFIX_LIST: list[str] = [
         "ws-", "nb-", "fmvulianna"]
 
     ADMINISTRATOR: str = "Administrator"
     ADMINISTRATOR_PASSOWORD: str = "Fortun@90"
 
-    CALL_CENTRE_ADMINISTRATOR: str = "callCentreAdmin"
-
-    MARKETER: str = "marketer"
+    class USER:
+        MARKETER: str = "marketer"
+        CALL_CENTRE_ADMINISTRATOR: str = "callCentreAdmin"
+        REGISTRATION_AND_CALL: str = "reg_and_call"
+        CONTROL_SERVICE: str = "cctv"
+        INDICATIONS_ALL: str = "indications_all"
 
     class JobPisitions(Enum):
         HR: int = auto()
         IT: int = auto()
         CALL_CENTRE: int = auto()
         REGISTRATOR: int = auto()
         RD: int = auto()
@@ -147,35 +171,34 @@
 class HOSTS:
 
     class BACKUP_WORKER:
     
         NAME: str = "backup_worker"
         ALIAS: str = "backup_worker"
         IP: str = "192.168.100.11"
-    
-    class DEVELOPER:
-
-        NAME: str = "ws-735"
-        IP: str = "192.168.254.102"
 
     class WS255:
     
         NAME: str = "ws-255"
         IP: str = "192.168.100.138"
 
     class WS816:
         
         NAME: str = "ws-816"
         IP: str = "192.168.254.81"
 
     class WS735:
         
         NAME: str = "ws-735"
-        IP: str = "192.168.254.102"
         ALIAS: str = "shared_disk_owner"
+        IP: str = "192.168.254.102" 
+
+    class DEVELOPER(WS735):
+    
+        pass
 
     class DC1:
     
         NAME: str = "fmvdc1.fmv.lan"
         ALIAS: str = "dc1"
         IP: str = "192.168.100.4"
 
@@ -220,87 +243,138 @@
         ALIAS: str = "ea_archive"
         IP: str = "192.168.110.108"
 
 class URLS:
 
     PYPI: str = "https://pypi.python.org/pypi/pih/json"
 
+class EMAIL_VERIFICATION_METHODS(Enum):
+    NORMAL: int = auto()
+    ABSTRACT_API: int = auto()
+    DEFAULT: int = NORMAL
+
+class ROBOCOPY:
+
+    ERROR_CODE_START: int = 8
+
+    STATUS_CODE: dict[int, str] = {
+        0  : "No errors occurred, and no copying was done. The source and destination directory trees are completely synchronized.",
+        1  : "One or more files were copied successfully (that is, new files have arrived).",
+        2  : "Some Extra files or directories were detected. No files were copied Examine the output log for details.",
+        4  : "Some Mismatched files or directories were detected. Examine the output log. Housekeeping might be required.",
+        8  : "Some files or directories could not be copied (copy errors occurred and the retry limit was exceeded). Check these errors further.",
+        16 : "Serious error. Robocopy did not copy any files. Either a usage error or an error due to insufficient access privileges on the source or destination directories.",
+        3  : "Some files were copied. Additional files were present. No failure was encountered.",
+        5  : "Some files were copied. Some files were mismatched. No failure was encountered.",
+        6  : "Additional files and mismatched files exist. No files were copied and no failures were encountered. This means that the files already exist in the destination directory",
+        7  : "Files were copied, a file mismatch was present, and additional files were present."
+    }
+
+class WINDOWS:
+
+    class CHARSETS:
+
+        ALTERNATIVE: str = "CP866"
+
+    class SERVICES:
+
+        WIA: str = "stisvc" #Обеспечивает службы получения изображений со сканеров и цифровых камер
+
+    class PORTS:
+
+        SMB: int = 445
 
 class CONST:
 
+    #in seconds
+    HEAT_BEAT_PERIOD: int = 60
+
+    NEW_LINE: str = "\n"
+
     class TEST:
 
-        WS: str = HOSTS.DEVELOPER.NAME
+        WORKSTATION_MAME: str = HOSTS.DEVELOPER.NAME
+        USER: str = "nak"
+        PERSON_PIN: int = 100310
 
     GROUP_PREFIX: str = "group:"
 
     SITE_PROTOCOL: str = "https://"
     UNTRUST_SITE_PROTOCOL: str = "http://" 
     
     SITE_ADDRESS: str = "pacifichosp.com"
-    MAIL_ADDRESS: str = f"mail.{SITE_ADDRESS}"
+    EMAIL_ADDRESS: str = f"mail.{SITE_ADDRESS}"
+    IT_EMAIL_ADDRESS: str = "@".join(("it", EMAIL_ADDRESS))
     WIKI_ADDRESS: str = f"{UNTRUST_SITE_PROTOCOL}wiki"
+    API_SITE_ADDRESS: str = f"api.{SITE_ADDRESS}"
+    BITRIX_SITE_URL: str = "bitrix.cmrt.ru"
 
     INTERNATIONAL_TELEPHONE_NUMBER_PREFIX: str = "7"
-    TELEPHONE_NUMBER_PREFIX: str = "+" + INTERNATIONAL_TELEPHONE_NUMBER_PREFIX
+    TELEPHONE_NUMBER_PREFIX: str = f"+{INTERNATIONAL_TELEPHONE_NUMBER_PREFIX}"
     INTERNAL_TELEPHONE_NUMBER_PREFIX: str = "тел."
 
-    DATE_TIME_SPLITTER: str = "T"
-    TIME_FORMAT: str = "%H:%M:00"
+    DATETIME_SPLITTER: str = "T"
     SECONDLESS_TIME_FORMAT: str = "%H:%M"
-    DATE_TIME_FORMAT: str = f"%Y-%m-%d{DATE_TIME_SPLITTER}{TIME_FORMAT}"
-    DATE_FORMAT: str = "%d.%m.%Y"
-
-    YEARLESS_DATE_FORMAT: str = "%d.%m"
+    SECOND_ZEROS_TIME_FORMAT: str = f"{SECONDLESS_TIME_FORMAT}:00"
+    DAY_FORMAT: str = "%d"
+    ISO_DATE_FORMAT: str = f"%Y-%m-{DAY_FORMAT}"
+    ISO_DATETIME_FORMAT: str = f"{ISO_DATE_FORMAT}{DATETIME_SPLITTER}{SECOND_ZEROS_TIME_FORMAT}"
+    
+    DATE_PART_DELIMITER: str = "."
+    YEARLESS_DATE_FORMAT: str = f"%d{DATE_PART_DELIMITER}%m"
+    DATE_FORMAT: str = f"{YEARLESS_DATE_FORMAT}{DATE_PART_DELIMITER}%Y"
+    DAYLESS_DATE_FORMAT: str = f"%m{DATE_PART_DELIMITER}%Y"
 
-    MY_DATE_FORMAT: str = "%d.%m.%Y %H:%M:%S"
-
-    API_SITE_ADDRESS: str = f"api.{SITE_ADDRESS}"
-
-    BITRIX_SITE_URL: str = "bitrix.cmrt.ru"
+    DATETIME_FORMAT: str = f"{DATE_FORMAT} {SECOND_ZEROS_TIME_FORMAT}"
 
     class DATA_STORAGE:
 
         DADATA_TOKEN: str = "147c0cd53d67fb4e48e379336c5794ae146c9621"
-        DATE_TIME_SPLITTER: str = " "
+        DATETIME_SPLITTER: str = " "
         DATE_FORMAT: str = "%Y-%m-%d"
         TIME_FORMAT: str = "%H:%M:00"
-        DATE_TIME_FORMAT: str = f"{DATE_FORMAT}{DATE_TIME_SPLITTER}{TIME_FORMAT}"
+        DATE_TIME_FORMAT: str = f"{DATE_FORMAT}{DATETIME_SPLITTER}{TIME_FORMAT}"
 
     class CACHE:
         
         class TTL:
-            
+            #in seconds
             WORKSTATIONS: int = 60
+            USERS: int = 300
 
     class ERROR:
 
         class WAPPI:
 
             PROFILE_NOT_PAID: int = 402
 
     class TIME_TRACKING:
 
         REPORT_DAY_PERIOD_DEFAULT: int = 15
+        PLAIN_FORMAT_AS_DEFAULT_LOGIN_LIST: list[str] = ["bar"]
 
     class MESSAGE:
 
         class WHATSAPP:
 
             SITE_NAME: str = "https://wa.me/"
             SEND_MESSAGE_TO_TEMPLATE: str = SITE_NAME + "{}?text={}"
 
             GROUP_SUFFIX: str = "@g.us"
 
             class GROUP(Enum):
 
                 RD: str = "79146947050-1595848245@g.us"
                 CT_INDICATIONS: str = "120363084280723039@g.us"
-                DOCUMENTS_WORK_STACK: str = '120363115241877592@g.us'
-                DOCUMENTS_WORK_STACK_TEST: str = '120363128816931482@g.us'
+                DOCUMENTS_WORK_STACK: str = "120363115241877592@g.us"
+                DOCUMENTS_WORK_STACK_TEST: str = "120363128816931482@g.us"
+                MAIN: str = "79644300470-1447044803@g.us"
+                REGISTRATION_AND_CALL: str = "79242332784-1447983812@g.us"
+                CONTROL_SERVICE_INDICATIONS: str = "120363159210756301@g.us"
+                EMAIL_CONTROL: str = "120363159605715569@g.us"
 
             class WAPPI:
 
                 PROFILE_SUFFIX: str = "profile_id="
                 URL_API: str = "https://wappi.pro/api"
                 URL_API_SYNC: str = f"{URL_API}/sync"
                 URL_MESSAGE: str = f"{URL_API_SYNC}/message"
@@ -320,15 +394,16 @@
                     MARKETER: str = "c31db01c-b6d6"
                     DEFAULT: str = CALL_CENTRE
                     
                 AUTHORIZATION: str = "6b356d3f53124af3078707163fdaebca3580dc38"
             
     class PYTHON:
 
-        EXECUTOR: str = "py"
+        EXECUTOR_ALIAS: str = "py"
+        EXECUTOR: str = "python"
         PYPI: str = "pip"
 
     class SERVICE:
 
         NAME: str = "service"
 
     class FACADE:
@@ -385,14 +460,16 @@
     class BARCODE_READER:
 
         PREFIX: str = "("
         SUFFIX: str = ")"
 
     class MOBILE_HELPER:
 
+        POLIBASE_PERSON_PIN: str = "polibase_person_pin"
+
         USER_DATA_INPUT_TIMEOUT: int = 180
 
         class InteraptionTypes:
 
             INTERNAL: int = 1
             TIMEOUT: int = 2
 
@@ -409,39 +486,43 @@
         SUBSCRIBE_COMMAND: str = "__subscribe__"
 
         @staticmethod
         def PORT(add: int = 0) -> int:
             return 50051 + add
 
         TIMEOUT: int = None
-        TIMEOUT_FOR_PING: int = 2
+        TIMEOUT_FOR_PING: int = 20
+        LONG_OPERATION_DURATION: int | None = None
 
     HOST = HOSTS()
 
     class POLIBASE:
 
         NAME: str = "Polibase"
 
         PROCESS_NAME: str = "Polibase ODAC"
 
         PRERECORDING_PIN: int = 10
+        PERSON_MINIMAL_PIN: int = 100
         RESERVED_TIME_A_PIN: int = 5
         RESERVED_TIME_B_PIN: int = 6
         RESERVED_TIME_C_PIN: int = 7
+        EMPTY_VALUE: str = "xxxxx"
+        EMPTY_EMAIL_VARIANTS: list[str] = ["нет", "-"]
+        TELEPHONE_NUMBER_COUNT: int = 4
 
-        CARD_REGISTRY_FOLDER_NAME_CHECK_PATTERN: list[str] = [
-        "п", "т", "b", "p", "t", "б"]
+        CARD_REGISTRY_FOLDER_NAME_CHECK_PATTERN: list[str] = ["п", "т", "b", "p", "t", "б"]
     
         #145 - Средний Медицинский Персонал
         #300 - Реанимация
         #361 - Операционная блок
         #421 - СМП
         #221 -
         #229 -
-        CABINET_NO_EXCLUDE_FROM_VISIT_RESULT: list[int] = [145, 221, 229, 300, 361, 421]
+        CABINET_NUMBER_EXCLUDED_FROM_VISIT_RESULT: list[int] = [145, 221, 229, 300, 361, 421]
         
         #147 - УЗИ
         #201 - ЭНДОСКОПИЯ
         #202 - МРТ
         #203 - КТ
 
         class APPOINTMENT_SERVICE_GROUP_ID(Enum):
@@ -513,31 +594,34 @@
         USER: str = "POLIBASE"
         PASSWORD: str = "POLIBASE"
         
         class BARCODE:
             
             class PERSON:
                 IMAGE_FORMAT: str =  FILE.EXTENSION.JPEG
+
             class PERSON_CARD_FOLDER:
                 IMAGE_FORMAT: str = FILE.EXTENSION.PNG
             
             ACTUAL_FORMAT: str = BARCODE.CODE128
             OLD_FORMAT: str = BARCODE.I25
 
             SUPPORT_FORMATS: list[str] = [ACTUAL_FORMAT, OLD_FORMAT]
 
-            NEW_PATTERN: str = "new_"
+            NEW_PREFIX: str = "new_"
 
             @staticmethod
             def get_file_name(pin: int, with_extension: bool = False) -> str:
                 extension: str = f".{CONST.POLIBASE.BARCODE.PERSON.IMAGE_FORMAT}" if with_extension else ""
-                return f"{CONST.POLIBASE.BARCODE.NEW_PATTERN}{pin}{extension}"
+                return "".join((CONST.POLIBASE.BARCODE.NEW_PREFIX, str(pin), extension))
             
         class DOCUMENT_DESCRIPTIONS(Enum):
 
+            ABPM_JOURNAL: PolibaseDocumentDescription = PolibaseDocumentDescription(
+                "Дневник суточного мониторинга АД", 70, 70, 80)
             HOLTER_JOURNAL: PolibaseDocumentDescription = PolibaseDocumentDescription("Дневник суточного мониторинга ЭКГ", 70, 70, 80)
             PATIENT_CARD_AMBULATORY: PolibaseDocumentDescription = PolibaseDocumentDescription("Медицинская карта\nпациента, получившего медицинскую помощь\nв амбулаторных условиях", 70, 120, 120)
             PROCESSING_PRESONAL_DATA_CONSENT: PolibaseDocumentDescription = PolibaseDocumentDescription("согласие\nпациента на обработку персональных данных", 70, 70, 120, 1)
             INFORMED_VOLUNTARY_MEDICAL_INVENTION_CONSENT: PolibaseDocumentDescription = PolibaseDocumentDescription("информированное добровольное согласие\nна медицинское вмешательство", 70, 70, 120, 1)
             INFORMED_VOLUNTARY_MEDICAL_INVENTION_CONSENT_SPECIFIC: PolibaseDocumentDescription = PolibaseDocumentDescription("информированное добровольное согласие на виды медицинских\nвмешательств, включенные в перечень определенных видов\nмедицинских вмешательств, на которые граждане дают\nинформированное добровольное согласие при выборе врача и\nмедицинской организации для получения первичной медико-\nсанитарной помощи", 70, 70, 280, 2)
 
             @staticmethod
@@ -556,47 +640,60 @@
            "6️⃣",
            "7️⃣",
            "8️⃣",
            "9️⃣",
            "🔟"
         ]
 
+        TEMPERATURE_SYMBOL: str = "°C"
+
         ARROW: str = "➜"
 
         BULLET: str = "•" 
 
-class RESOURCE:
+class MATERIALIZED_RESOURCES:
+
+    NAME: str = "MATERIALIZED_RESOURCES"
+    ALIAS: str = "MR"
+
+    class TYPES(Enum):
+    
+        CHILLER_FILTER_COUNT: IntStorageValue = IntStorageValue("CHF")
+
+
+class RESOURCES:
 
     class DESCRIPTIONS:
     
         INTERNET: ResourceDescription = ResourceDescription(
             "77.88.55.242", "Интернет соединение")
         
         VPN_PACS_SPB: ResourceDescription = ResourceDescription(
             "192.168.5.3", "VPN соединение для PACS SPB", (2, 100, 5))
+        
         PACS_SPB: ResourceDescription = ResourceDescription(
             "10.76.12.124:4242", "Соединение PACS SPB", (2, 100, 5))
 
         POLIBASE: ResourceDescription = ResourceDescription("polibase", "Polibase", inaccessibility_check_values=(2, 10000, 15))
 
         SITE_LIST: list[SiteResourceDescription] = [
             SiteResourceDescription(
                         CONST.SITE_ADDRESS, f"Сайт компании: {CONST.SITE_ADDRESS}", check_certificate_status=True, check_free_space_status=False),
-            SiteResourceDescription(CONST.MAIL_ADDRESS,
-                        f"Сайт корпоративной почты: {CONST.MAIL_ADDRESS}", check_certificate_status=True, check_free_space_status=True, driver_name="/dev/mapper/centos_tenant26--02-var"),
+            SiteResourceDescription(CONST.EMAIL_ADDRESS,
+                        f"Сайт корпоративной почты: {CONST.EMAIL_ADDRESS}", check_certificate_status=True, check_free_space_status=True, driver_name="/dev/mapper/centos_tenant26--02-var"),
             SiteResourceDescription(CONST.API_SITE_ADDRESS,
                                     f"Api сайта {CONST.SITE_ADDRESS}: {CONST.API_SITE_ADDRESS}", check_certificate_status=True, check_free_space_status=False),
             SiteResourceDescription(CONST.BITRIX_SITE_URL, f"Сайт Битрикс ЦМРТ24: {CONST.BITRIX_SITE_URL}")
         ]
     
-    class INACCESSABLE_REASON(Enum):
+    class INACCESSABLE_REASONS(Enum):
 
-        SERTIFICATE_ERROR: str = "Ошибка проверки сертификата"
+        CERTIFICATE_ERROR: str = "Ошибка проверки сертификата"
 
-class MEDICAl_DOCUMENT:
+class MEDICAL_DOCUMENT:
 
     class DIRECTION_TYPES(Enum):
             
         MRI: MedicalDirectionDescription = MedicalDirectionDescription(("Магнитно-резонансная томография", ), "МРТ")
         CT: MedicalDirectionDescription = MedicalDirectionDescription(("Компьютерная томография", ), "КТ")
         ULTRASOUND: MedicalDirectionDescription = MedicalDirectionDescription(("ультразвуковая допплерография", ), "УЗИ")
 
@@ -607,14 +704,20 @@
     PRINTER: int = auto()
     INDICATIONS: int = auto()
     BACKUPS: int = auto()
 
     @staticmethod
     def all() :
         return [item for item in CheckableSections]
+    
+class DocumentTypes(Enum):
+    
+    POLIBASE: int = auto()
+    MEDICAL_DIRECTION: int = auto()
+    PERSONAL: int = auto()
 
 class PATH_SHARE:
 
     NAME: str = "shares"
     PATH: str = os.path.join(AD.PATH_ROOT, NAME)
 
 class PATH_SCAN:
@@ -623,14 +726,28 @@
     VALUE: str = os.path.join(AD.PATH_ROOT, NAME)
 
 class PATH_SCAN_TEST:
     
     NAME: str = "test"
     VALUE: str = os.path.join(PATH_SCAN.VALUE, NAME)
 
+class PATH_SCAN_SOURCE:
+    
+    NAME: str = "Исходники"
+    VALUE: str = os.path.join(PATH_SCAN.VALUE, NAME)
+
+class PATH_SCAN_RESULT:
+    
+    NAME: str = "Результат"
+    VALUE: str = os.path.join(PATH_SCAN.VALUE, NAME)
+
+    @staticmethod
+    def get_path(type: DocumentTypes) -> str:
+        if type == DocumentTypes.MEDICAL_DIRECTION:
+            return  os.path.join(PATH_SCAN_RESULT.VALUE, "Направления")
 
 class PATH_WS_816_SCAN:
     
     NAME: str = r"C$\Users\Nurse\Documents\Scanned Documents"
     VALUE: str = os.path.join(r"\\", HOSTS.WS816.NAME, NAME)
 
 class PATH_OMS:
@@ -672,25 +789,46 @@
 
     NAME: str = "data"
     FOLDER: str = os.path.join(PATH_APP.FOLDER, NAME)
 
     OCR_RESULT_NAME: str = "ocr result"
     OCR_RESULT_FOLDER: str =  os.path.join(FOLDER, OCR_RESULT_NAME)
 
+class PATH_INDICATIONS:
+
+    NAME: str = "indications"
+    FOLDER: str =  os.path.join(PATH_APP_DATA.FOLDER, NAME)
+
+    CHILLER_DATA_NAME: str = "chiller"
+    CHILLER_DATA_FOLDER: str = os.path.join(FOLDER, CHILLER_DATA_NAME)
+
+    CHILLER_DATA_IMAGE_LAST: str = os.path.join(CHILLER_DATA_FOLDER, f"last.{FILE.EXTENSION.JPG}")
+    CHILLER_DATA_IMAGE_LAST_RESULT: str = os.path.join(CHILLER_DATA_FOLDER, f"last_result.{FILE.EXTENSION.JPG}")
+
+    @staticmethod
+    def CHILLER_DATA_IMAGE_RESULT(datetime_string: str, temperature: float| None, indications: int) -> str:
+        name_list: list[str] = [str(indications)]
+        if temperature is not None:
+            name_list += [str(temperature)]
+        name_list += [datetime_string]
+        return os.path.join(PATH_INDICATIONS.CHILLER_DATA_FOLDER, f"{'_'.join(name_list)}.{FILE.EXTENSION.JPG}")
+
 class PATH_MOBILE_HELPER:
 
     NAME: str = "mobile helper"
     FOLDER: str = os.path.join(PATH_APP_DATA.FOLDER, NAME)
 
     QR_CODE_NAME: str = "qr code"
     QR_CODE_FOLDER: str =  os.path.join(FOLDER, QR_CODE_NAME)
 
     INCOME_IMAGES_NAME: str = "income images"
     INCOME_IMAGES_FOLDER: str =  os.path.join(FOLDER, INCOME_IMAGES_NAME)
 
+    TIME_TRACKING_REPORT: str = "time tracking report"
+    TIME_TRACKING_REPORT_FOLDER: str = os.path.join(FOLDER, TIME_TRACKING_REPORT)
 
 class PATH_POLIBASE_APP_DATA:
     
     NAME: str = "polibase"
     FOLDER: str = os.path.join(PATH_APP_DATA.FOLDER, NAME)
     PERSON_CARD_FOLDER: str = os.path.join(FOLDER, "person card folder")
 
@@ -747,80 +885,90 @@
     
 
 class PATHS:
 
     SHARE: PATH_SHARE = PATH_SHARE()
     SCAN: PATH_SCAN = PATH_SCAN()
     SCAN_TEST = PATH_SCAN_TEST()
+    SCAN_SOURCE = PATH_SCAN_SOURCE()
+    SCAN_RESULT = PATH_SCAN_RESULT()
     WS_816_SCAN: PATH_WS_816_SCAN = PATH_WS_816_SCAN()
     OMS: PATH_OMS = PATH_OMS()
     IT: PATH_IT = PATH_IT()
     USER: PATH_USER = PATH_USER()
     POLIBASE: PATH_POLIBASE = PATH_POLIBASE()
     POLIBASE_APP_DATA: PATH_POLIBASE_APP_DATA = PATH_POLIBASE_APP_DATA()
     WS: PATH_WS = PATH_WS()
     BACKUP: PATH_BACKUP = PATH_BACKUP()
     DOCS: PATH_DOCS = PATH_DOCS()
     FONTS: PATH_FONTS = PATH_FONTS()
     MOBILE_HELPER: PATH_MOBILE_HELPER = PATH_MOBILE_HELPER()
     APP_DATA: PATH_APP_DATA = PATH_APP_DATA()
+    INDICATIONS: PATH_INDICATIONS = PATH_INDICATIONS()
 
 class MarkType(Enum):
 
     NORMAL: int = auto()
     FREE: int = auto()
     GUEST: int = auto()
     TEMPORARY: int = auto()
 
 class FIELD_NAME_COLLECTION:
 
+    ACTION_NAME: str = "action_name"
+    ACTION_DESCRIPTION: str = "action_description"
     FULL_NAME: str = "FullName"
     TYPE: str = "type"
     GROUP_NAME: str = "GroupName"
     GROUP_ID: str = "GroupID"
     COMMENT: str = "Comment"
     CARD_FOLDER: str = "ChartFolder"
     BIRTH: str = "Birth"
     TAB_NUMBER: str = "TabNumber"
     OWNER_TAB_NUMBER: str = "OwnerTabNumber"
-    NAME: str = USER_PROPERTY.NAME
+    NAME: str = USER_PROPERTIES.NAME
     MIDNAME: str = "MidName"
     PERSON_ID: str = "pID"
     MARK_ID: str = "mID"
     ID: str = "id"
     PIN: str = "pin"
+    PID: str = "pid"
     VISIT_ID: str = "visitID"
     MESSAGE_ID: str = "messageID"
     VALUE: str = "value"
     FILE: str = "file"
     DIVISION_NAME: str = "DivisionName"
     BARCODE: str = "barcode"
     PROPERTIES: str = "properties"
+    PARAMETERS: str = "parameters"
     MESSAGE: str = "message"
     STATUS: str = "status"
     FEEDBACK_CALL_STATUS: str = "feedbackCallStatus"
     REGISTRATION_DATE: str = "registrationDate"
     TYPE: str = "type"
     CABINET_ID: str = "cabinetID"
     DOCTOR_ID: str = "doctorID"
     DOCTOR_FULL_NAME: str = "doctorFullName"
     SERVICE_GROUP_ID: str = "serviceGroupID"
     PORT_NAME: str = "portName"
     TEMPERATURE: str = "temperature"
     HUMIDITY: str = "humidity"
+    INDICATORS: str = "indicators"
+    DATA: str = "data"
 
-    SEARCH_ATTRIBUTE_LOGIN: str = USER_PROPERTY.LOGIN
-    SEARCH_ATTRIBUTE_NAME: str = USER_PROPERTY.NAME
+    SEARCH_ATTRIBUTE_LOGIN: str = USER_PROPERTIES.LOGIN
+    SEARCH_ATTRIBUTE_NAME: str = USER_PROPERTIES.NAME
 
-    TELEPHONE_NUMBER: str = USER_PROPERTY.TELEPHONE_NUMBER
-    EMAIL: str = USER_PROPERTY.EMAIL
-    DN: str = USER_PROPERTY.DN
-    LOGIN: str = USER_PROPERTY.LOGIN
-    DESCRIPTION: str = USER_PROPERTY.DESCRIPTION
-    PASSWORD: str = USER_PROPERTY.PASSWORD
+    TELEPHONE_NUMBER: str = USER_PROPERTIES.TELEPHONE_NUMBER
+    EMAIL: str = f"e{USER_PROPERTIES.EMAIL}"
+    DN: str = USER_PROPERTIES.DN
+    LOGIN: str = USER_PROPERTIES.LOGIN
+    ACTIVE_USERS_LOGIN: str = "active_" + USER_PROPERTIES.LOGIN
+    DESCRIPTION: str = USER_PROPERTIES.DESCRIPTION
+    PASSWORD: str = USER_PROPERTIES.PASSWORD
     ACCESSABLE: str = "accessable"
     STEP: str = "step"
     STEP_CONFIRMED: str = "stepConfirmed"
     GRADE: str = "grade"
     INFORMATION_WAY: str = "informationWay"
     TIME: str = "time"
 
@@ -844,23 +992,34 @@
     TEMPLATE_USER_CONTAINER: str = "templated_user"
     CONTAINER: str = "container"
 
     REMOVE: str = "remove"
     AS_FREE: str = "as_free"
     CANCEL: str = "cancel"
 
+    WORKSTATION_NAME: str = "workstation_name"
+    WORKSTATION_DESCRIPTION: str = "workstation_description"
+    PERSON_NAME: str = "person_name"
+    REGISTRATOR_PERSON_NAME: str = "registrator_person_name"
+    PERSON_PIN: str = "person_pin"
+
 
 class FIELD_ITEM_COLLECTION:
 
     TAB_NUMBER: FieldItem = FieldItem(
         FIELD_NAME_COLLECTION.TAB_NUMBER, "Табельный номер")
     OWNER_TAB_NUMBER: FieldItem = FieldItem(
         FIELD_NAME_COLLECTION.OWNER_TAB_NUMBER, "Табельный номер владельца")
     FULL_NAME: FieldItem = FieldItem(
         FIELD_NAME_COLLECTION.FULL_NAME, "Полное имя")
+    TEMPERATURE: FieldItem = FieldItem(FIELD_NAME_COLLECTION.TEMPERATURE,
+              "Температура", data_formatter="{data}°C")
+    INDICATORS: FieldItem = FieldItem(FIELD_NAME_COLLECTION.INDICATORS,
+              "Индикаторы", data_formatter=DATA.FORMATTER.CHILLER_INDICATIONS_VALUE_INDICATORS.value)
+    INDICATION_TIMESTAMP: FieldItem = FieldItem(FIELD_NAME_COLLECTION.TIMESTAMP, "Время снятия показаний", data_formatter=DATA.FORMATTER.MY_DATETIME.value)
     
 
 class FIELD_COLLECTION:
 
     INDEX: FieldItem = FieldItem("__Index__", "Индекс", True)
     POSITION: FieldItem = FieldItem("position", "Позиция", True, default_value="Нет")
 
@@ -966,17 +1125,17 @@
         WORKSTATION: FieldItemList = FieldItemList(
             FieldItem(FIELD_NAME_COLLECTION.NAME, "Имя компьютера"),
             FieldItem(FIELD_NAME_COLLECTION.DESCRIPTION, "Описание"),
             FieldItem(FIELD_NAME_COLLECTION.PROPERTIES, "Свойства", visible=False)
         )
 
         USER_ACTION: FieldItemList = FieldItemList(
-            FieldItem(USER_PROPERTY.TELEPHONE_NUMBER, "Изменить номер телефона"),
-            FieldItem(USER_PROPERTY.PASSWORD, "Изменить пароль"),
-            FieldItem(USER_PROPERTY.USER_STATUS, "Активировать или деактивировать")
+            FieldItem(USER_PROPERTIES.TELEPHONE_NUMBER, "Изменить номер телефона"),
+            FieldItem(USER_PROPERTIES.PASSWORD, "Изменить пароль"),
+            FieldItem(USER_PROPERTIES.USER_STATUS, "Активировать или деактивировать")
         )
 
 
         USER_WORKSTATION: FieldItemList = FieldItemList(
             WORKSTATION,
             FieldItem(FIELD_NAME_COLLECTION.ACCESSABLE, "Доступен"),
             FieldItem(FIELD_NAME_COLLECTION.LOGIN, "Имя залогированного пользователя")
@@ -998,15 +1157,15 @@
 
         TEMPLATED_USER: FieldItemList = FieldItemList(
             FieldItem(FIELD_NAME_COLLECTION.DESCRIPTION, "Описание"))
 
         USER: FieldItemList = FieldItemList(CONTAINER,
                                             FieldItem(FIELD_NAME_COLLECTION.LOGIN, "Логин"),
                                             FieldItem(FIELD_NAME_COLLECTION.TELEPHONE_NUMBER, "Телефон"),
-                                            FieldItem(FIELD_NAME_COLLECTION.EMAIL, "Электронная почта"),
+                                            FieldItem(USER_PROPERTIES.EMAIL, "Электронная почта"),
                                             FieldItem(FIELD_NAME_COLLECTION.DN, "Размещение"),
                                             FieldItem("userAccountControl", "Свойства аккаунта", False)).position(FIELD_NAME_COLLECTION.DESCRIPTION, 4).caption(FIELD_NAME_COLLECTION.NAME, USER_NAME.get_item_by_name(FIELD_NAME_COLLECTION.NAME).caption)
 
         CONTAINER_TYPE: FieldItemList = FieldItemList(
             FieldItem(FIELD_NAME_COLLECTION.TEMPLATE_USER_CONTAINER,
                       "Шаблонный пользователь"),
             FieldItem(FIELD_NAME_COLLECTION.CONTAINER, "Контейнер"))
@@ -1019,15 +1178,16 @@
                                               FieldItem(FIELD_NAME_COLLECTION.TELEPHONE_NUMBER, "Телефон"))
 
         PERSON_VISIT: FieldItemList = FieldItemList(PERSON_BASE,
                                               FieldItem(FIELD_NAME_COLLECTION.REGISTRATION_DATE, "Дата регистрации"),
                                               FieldItem(FIELD_NAME_COLLECTION.DOCTOR_FULL_NAME, "Имя доктора"))
 
         PERSON: FieldItemList = FieldItemList(PERSON_BASE,
-                                              FieldItem(FIELD_NAME_COLLECTION.BIRTH, "День рождения", True, "datetime"),
+                                              FieldItem(FIELD_NAME_COLLECTION.BIRTH, "День рождения", True,
+                                                        "datetime", data_formatter=f"{DATA.FORMATTER.MY_DATE.value}"),
                                               FieldItem(FIELD_NAME_COLLECTION.EMAIL, "Электронная почта"),
                                               FieldItem(FIELD_NAME_COLLECTION.CARD_FOLDER, "Папка карты пациента", default_value="Нет папки"),
                                               FieldItem(FIELD_NAME_COLLECTION.COMMENT, "Комментарий"))
 
 
     class POLICY:
 
@@ -1035,32 +1195,38 @@
             #FieldItem("EMAIL", "Для почты"),
             #FieldItem("SIMPLE", "Простой"),
             FieldItem("NORMAL", "Стандартный"),
             FieldItem("STRONG", "Сложный"))
 
     class PRINTER:
 
-        MAIN: FieldItemList = FieldItemList(
+        ITEM: FieldItemList = FieldItemList(
             FieldItem(FIELD_NAME_COLLECTION.NAME, "Name"),
             FieldItem("serverName", "Server name"),
             FieldItem(FIELD_NAME_COLLECTION.PORT_NAME, "Host name"),
             FieldItem(FIELD_NAME_COLLECTION.DESCRIPTION, "Description"),
             FieldItem("adminDescription", "Admin description", False),
             FieldItem("driverName", "Driver name")
         )
 
     class INDICATIONS:
 
-        CT: FieldItemList = FieldItemList(
-            FieldItem(FIELD_NAME_COLLECTION.TEMPERATURE, "Температура", data_formatter="{data}°C"),
+        CT_VALUE: FieldItemList = FieldItemList(
+            FIELD_ITEM_COLLECTION.TEMPERATURE,
             FieldItem(FIELD_NAME_COLLECTION.HUMIDITY, "Влажность", data_formatter="{data}%")
         )
 
-        CT_WITH_TIMESTAMP: FieldItemList = FieldItemList(CT,
-                                              FieldItem(FIELD_NAME_COLLECTION.TIMESTAMP, "Время измерения", data_formatter=f"{DATA.FORMATTER.MY_DATETIME}"))
+        CHILLER_VALUE: FieldItemList = FieldItemList(
+            FIELD_ITEM_COLLECTION.TEMPERATURE,
+            FIELD_ITEM_COLLECTION.INDICATORS
+        )
+
+        CT_VALUE_CONTAINER: FieldItemList = FieldItemList(CT_VALUE, FIELD_ITEM_COLLECTION.INDICATION_TIMESTAMP)
+        
+        CHILLER_VALUE_CONTAINER: FieldItemList = FieldItemList(CHILLER_VALUE, FIELD_ITEM_COLLECTION.INDICATION_TIMESTAMP)
 
 
 class FIELD_COLLECTION_ALIAS(Enum):
     TIME_TRACKING: FieldItem = FIELD_COLLECTION.ORION.TIME_TRACKING
     PERSON: FieldItem = FIELD_COLLECTION.ORION.PERSON
     TEMPORARY_MARK: FieldItem = FIELD_COLLECTION.ORION.TEMPORARY_MARK
     POLIBASE_PERSON: FieldItem = FIELD_COLLECTION.POLIBASE.PERSON
@@ -1126,231 +1292,100 @@
         PC: PasswordSettings = NORMAL
         EMAIL: PasswordSettings = NORMAL
 
     def get(name: str) -> SETTINGS:
         return PASSWORD.__getattribute__(PASSWORD.SETTINGS, name)
 
 
-class LogTypes(Enum):
-    MESSAGE: str = "message"
-    COMMAND: str = "command"
-    DEFAULT: str = MESSAGE
-
-
-class LogChannels(Enum):
+class LogMessageChannels(Enum):
     BACKUP: int = auto()
-    NOTIFICATION: int = auto()
-    NOTIFICATION_BOT: int = auto()
+    POLIBASE_NOTIFICATIONS: int = auto()
+    POLIBASE_NOTIFICATIONS_BOT: int = auto()
     DEBUG: int = auto()
     DEBUG_BOT: int = auto()
-    SERVICE: int = auto()
-    SERVICE_BOT: int = auto()
+    SERVICES: int = auto()
+    SERVICES_BOT: int = auto()
     HR: int = auto()
     HR_BOT: int = auto()
     IT: int = auto()
     IT_BOT: int = auto()
-    POLIBASE_PERSON_FEEDBACK_CALL: int = auto()
-    POLIBASE_PERSON_REVIEW_QUEST_RESULT: int = auto()
     RESOURCES: int = auto()
     RESOURCES_BOT: int = auto() 
     PRINTER: int = auto()
-    DEFAULT: int = NOTIFICATION
+    POLIBASE_ERROR_NOTIFICATIONS: int = auto()
+    POLIBASE_ERROR_NOTIFICATIONS_BOT: int = auto()
+    DEFAULT: int = DEBUG
 
 
-class LogLevels(Enum):
+class LogMessageFlags(Enum):
     NORMAL: int = 1
     ERROR: int = 2
-    EVENT: int = 4
+    NOTIFICATION: str = 4
     DEBUG: str = 8
-    TASK: int = 16
-    NOTIFICATION: str = 32
-    SILENCE: str = 4048
+    SAVE: int = 16
+    TASK: int = 17
+    SILENCE: str = 32
+    RESULT: int = 64
+    WHATSAPP: int = 128
+    ALERT: int = 256
     DEFAULT: str = NORMAL
 
-
-class ServiceCommands(Enum):
-    ping: int = auto()
-    subscribe: int = auto()
-    unsubscribe: int = auto()
-    unsubscribe_all: int = auto()
-    stop: int = auto()
-    #Log
-    send_log_message: int = auto()
-    send_log_command: int = auto()
-    send_message_to_user_or_workstation: int = auto()
-    add_message_to_queue: int = auto()
-    send_delayed_message: int = auto()
-    #Documents
-    create_user_document: int = auto()
-    save_time_tracking_report: int = auto()
-    create_barcodes_for_inventory: int = auto()
-    create_barcode_for_polibase_person: int = auto()
-    create_qr_code: int = auto()
-    check_inventory_report: int = auto()
-    get_inventory_report: int = auto()
-    save_inventory_report_item: int = auto()
-    close_inventory_report: int = auto()
-    #Polibase
-    get_polibase_person_by_pin: int = auto()
-    get_polibase_persons_by_pin: int = auto()
-    get_polibase_persons_by_card_registry_folder_name: int = auto() 
-    get_polibase_persons_by_full_name: int = auto()
-    get_polibase_person_pin_list_with_old_format_barcode: int = auto()
-    get_polibase_person_registrator_by_pin: int = auto()
-    get_polibase_persons_pin_by_visit_date: int = auto()
-    get_polibase_persons_by_telephone_number: int = auto()
-    #
-    get_polibase_person_visits_last_id: int = auto()
-    search_polibase_person_visits: int = auto()
-    #
-    set_polibase_person_card_folder_name: int = auto()
-    set_polibase_person_email: int = auto()
-    set_polibase_person_barcode_by_pin: int = auto()
-    check_polibase_person_card_registry_folder_name: int = auto()
-
-    #ActiveDirectory
-    check_user_exists_by_login: int = auto()
-    get_user_by_full_name: int = auto()
-    get_users_by_name: int = auto()
-    #get_active_users_by_name: int = auto()
-    get_user_by_login: int = auto()
-    get_user_by_telephone_number: int = auto()
-    get_template_users: int = auto()
-    get_containers: int = auto()
-    get_users_by_job_position: int = auto()
-    get_users_by_group: int = auto()
-    create_user_by_template: int = auto()
-    create_user_in_container: int = auto()
-    set_user_telephone: int = auto()
-    authenticate: int = auto()
-    set_user_password: int = auto()
-    set_user_status: int = auto()
-    get_printers: int = auto()
-    remove_user: int = auto()
-    get_all_workstation_description: int = auto()
-    get_all_workstations: int = auto()
-    get_workstation_by_user: int = auto()
-    get_user_by_workstation: int = auto()
-    #Printer
-    printers_report: int = auto()
-    printers_status: int = auto()
-    #Orion
-    get_free_marks: int = auto()
-    get_temporary_marks: int = auto()
-    get_person_divisions: int = auto()
-    get_time_tracking: int = auto() 
-    get_all_persons: int = auto()
-    get_owner_mark_for_temporary_mark: int = auto()
-    get_mark_by_tab_number: int = auto()
-    get_mark_by_person_name: int = auto()
-    get_free_marks_group_statistics: int = auto()
-    get_free_marks_by_group_id: int = auto()
-    set_full_name_by_tab_number: int = auto()
-    set_telephone_by_tab_number: int = auto()
-    check_mark_free: int = auto()
-    create_mark: int = auto()
-    remove_mark_by_tab_number: int = auto()
-    make_mark_as_free_by_tab_number: int = auto()
-    make_mark_as_temporary: int = auto()
-    #PolibaseDatabaseBackup
-    create_polibase_database_backup: int = auto()
-    #DataStorage::Settings
-    set_settings_value: int = auto()
-    get_settings_value: int = auto()
-    #HeatBeat
-    heat_beat: int = auto()
-    #Notifier
-    register_polibase_person_information_quest: int = auto()
-    search_polibase_person_information_quests: int = auto()
-    update_polibase_person_information_quest: int = auto()
-    #Visit Cached
-    update_polibase_person_visit_to_data_stogare: int = auto()
-    search_polibase_person_visits_in_data_storage: int = auto()
-    #Visit notification
-    register_polibase_person_visit_notification: int = auto()
-    search_polibase_person_visit_notifications: int = auto()
-    #Notification confirmation
-    search_polibase_person_notification_confirmation: int = auto()
-    update_polibase_person_notification_confirmation: int = auto()
-    #
-    check_email_accessibility: int = auto()
-    #
-    register_delayed_message: int = auto()
-    search_delayed_messages: int = auto()
-    update_delayed_message: int = auto()
-    #WORKSTATION
-    reboot: int = auto()
-    shutdown: int = auto()
-    log_out: int = auto()
-    #Robocopy::Job
-    robocopy_start_job: int = auto()
-    robocopy_get_job_status_list: int = auto()
-    #DataStorage::Storage value
-    set_storage_value: int = auto()
-    get_storage_value: int = auto()
-    #Resource Manager
-    get_resource_status_list: int = auto()
-    send_mobile_helper_message: int = auto()
-
-    register_ct_indications_value: int = auto()
-    get_last_ct_indications_value_list: int = auto()
-    #
-    test: int = auto()
-    #
-    execute_ssh_command: int = auto()
-    get_certificate_information: int = auto()
-    get_unix_free_space_information_by_drive_name: int = auto()
-    print_image: int = auto()
-    #
-    get_ogrn_value: int = auto()
-    get_fms_unit_name: int = auto()
-    #
-    start_polibase_person_information_quest: int = auto()
-
-    
+POLIBASE_BASE: ServiceDescription = ServiceDescription(
+        host=CONST.HOST.POLIBASE.NAME,
+        pyton_executor_path=r"C:\Users\adm\AppData\Local\Programs\Python\Python310\python.exe",
+        run_from_system_account=True
+        )
 
 class ServiceRoles(Enum):
 
-    LOG: ServiceRoleDescription = ServiceRoleDescription(
-                                            name="Log",
-                                            description="Log service",
+    @staticmethod
+    def description(value: Enum | str | ServiceInformationBase, get_source_description: bool = False) -> ServiceInformationBase | None:
+        def isolated_name(value: ServiceInformationBase | None) -> str | None:
+            if value is None:
+                return None
+            value.name = ":".join(("isolated", value.name)) if value.isolated and value.name.find("isolated") == -1 else value.name
+            return value
+        if isinstance(value, str):
+            for service_role in ServiceRoles:
+                if ServiceRoles.description(service_role).name == value:
+                    return isolated_name(service_role.value)
+            return None
+        if isinstance(value, ServiceInformationBase):
+            return isolated_name(ServiceRoles.description(value.name) if get_source_description else value)
+        return isolated_name(value.value)
+    
+    SERVICE_ADMIN: ServiceDescription = ServiceDescription(
+        name="ServiceAdmin",
+        description="Service admin",
+        host=CONST.HOST.WS735.NAME,
+        port=CONST.RPC.PORT(20),
+        commands=[
+            ServiceCommands.on_service_starts,
+            ServiceCommands.on_service_stops,
+            ServiceCommands.get_service_information_table,
+            ServiceCommands.heat_beat
+        ],
+        modules=["schedule"]
+    )
+
+    EVENT_AND_LOG: ServiceDescription = ServiceDescription(
+                                            name="EventAndLog",
+                                            description="Log and Event service",
                                             host=CONST.HOST.BACKUP_WORKER.NAME, 
-                                            port=CONST.RPC.PORT(),
                                             commands=[
                                                         ServiceCommands.send_log_message,
-                                                        ServiceCommands.send_log_command
+                                                        ServiceCommands.send_event
                                                      ],
                                             modules=["telegram-send"])
 
-    HEART_BEAT: ServiceRoleDescription = ServiceRoleDescription(
-        name="HeartBeat",
-        description="Heart beat service",
-        host=CONST.HOST.WS255.NAME,
-        port=CONST.RPC.PORT(),
-        commands=[
-            ServiceCommands.heat_beat
-        ],
-        modules=["schedule"])
-
-    INDICATIONS: ServiceRoleDescription = ServiceRoleDescription(
-        name="Indications",
-        description="Indications service",
-        host=CONST.HOST.WS255.NAME,
-        commands=[ServiceCommands.register_ct_indications_value,
-                  ServiceCommands.get_last_ct_indications_value_list
-                  ],
-        port=CONST.RPC.PORT(5),
-        modules=["fastapi", "uvicorn"]
-    )
-
-    DATA_STORAGE: ServiceRoleDescription = ServiceRoleDescription(
-                                            name="DataStorage",
-                                            description="DataStorage service", 
+    DATA_STORAGE_AND_SOURCE: ServiceDescription = ServiceDescription(
+                                            name="DataStorageAndSource",
+                                            description="Data storage and source service", 
                                             host=CONST.HOST.BACKUP_WORKER.NAME, 
-                                            port=CONST.RPC.PORT(1),
+                                            host_changabled=False,
                                             commands=[
                                                         ServiceCommands.register_polibase_person_information_quest,
                                                         ServiceCommands.search_polibase_person_information_quests,
                                                         ServiceCommands.update_polibase_person_information_quest,
                                                         #
                                                         ServiceCommands.update_polibase_person_visit_to_data_stogare,
                                                         ServiceCommands.search_polibase_person_visits_in_data_storage,
@@ -1368,63 +1403,59 @@
                                                         ServiceCommands.search_polibase_person_notification_confirmation,
                                                         ServiceCommands.update_polibase_person_notification_confirmation,
                                                         #
                                                         ServiceCommands.get_storage_value,
                                                         ServiceCommands.set_storage_value,
                                                         #
                                                         ServiceCommands.get_ogrn_value,
-                                                        ServiceCommands.get_fms_unit_name
+                                                        ServiceCommands.get_fms_unit_name,
+                                                        #
+                                                        ServiceCommands.register_chiller_indications_value,
+                                                        ServiceCommands.register_ct_indications_value,
+                                                        ServiceCommands.get_last_ct_indications_value_container_list,
+                                                        ServiceCommands.get_last_сhiller_indications_value_container_list,
+                                                        #
+                                                        ServiceCommands.get_gkeep_item_id,
+                                                        ServiceCommands.add_gkeep_map_item,
+                                                        #
+                                                        ServiceCommands.register_event,
+                                                        ServiceCommands.get_event,
+                                                        ServiceCommands.remove_event
                                                     ],
                                             modules=["mysql-connector-python", "pysos", "lmdbm", "dadata"])
 
-    FILE_WATCHDOG: ServiceRoleDescription = ServiceRoleDescription(
+    FILE_WATCHDOG: ServiceDescription = ServiceDescription(
         name="FileWatchdog",
         description="FileWatchdog service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
-        port=CONST.RPC.PORT(2),
         modules=["watchdog"])
 
-    MAIL: ServiceRoleDescription = ServiceRoleDescription(
+    MAIL: ServiceDescription = ServiceDescription(
         name="Mail",
         description="Mail service",
-        host=CONST.HOST.BACKUP_WORKER.NAME,
-        port=CONST.RPC.PORT(3),
+        host=CONST.HOST.WS255.NAME,
         commands=
                 [
                     ServiceCommands.check_email_accessibility
                 ],
-        modules=["py3-validate-email", "verify-email"])
-
-    WS: ServiceRoleDescription = ServiceRoleDescription(
-                                                name="WS",
-                                                description="Workstation service",
-                                                host=CONST.HOST.BACKUP_WORKER.NAME,
-                                                port=CONST.RPC.PORT(4),
-                                                commands=[
-                                                    ServiceCommands.reboot,
-                                                    ServiceCommands.shutdown,
-                                                    ServiceCommands.send_message_to_user_or_workstation
-                                                ])
-
+        modules=["py3-validate-email"])
 
-    BACKUP: ServiceRoleDescription = ServiceRoleDescription(
+    BACKUP: ServiceDescription = ServiceDescription(
                                                 name="Backup",
                                                 description="Backup service",
                                                 host=CONST.HOST.BACKUP_WORKER.NAME,
-                                                port=CONST.RPC.PORT(5),
                                                 commands=[
                                                     ServiceCommands.robocopy_start_job,
                                                     ServiceCommands.robocopy_get_job_status_list
                                                 ])
 
-    AD: ServiceRoleDescription = ServiceRoleDescription(
+    AD: ServiceDescription = ServiceDescription(
                                                 name="ActiveDirectory",
                                                 description="Active directory service",
                                                 host=CONST.HOST.DC2.NAME,
-                                                port=CONST.RPC.PORT(),
                                                 commands=
                                                         [
                                                             ServiceCommands.authenticate,
                                                             ServiceCommands.check_user_exists_by_login,
                                                             ServiceCommands.get_user_by_full_name,
                                                             ServiceCommands.get_users_by_name,
                                                             ServiceCommands.get_user_by_login,
@@ -1432,64 +1463,74 @@
                                                             ServiceCommands.get_template_users,
                                                             ServiceCommands.get_containers,
                                                             ServiceCommands.get_users_by_job_position,
                                                             ServiceCommands.get_users_by_group, 
                                                             ServiceCommands.get_printers,
                                                             ServiceCommands.get_all_workstation_description,
                                                             ServiceCommands.get_all_workstations,
-                                                            ServiceCommands.get_workstation_by_user,
+                                                            ServiceCommands.get_workstation_list_by_user_login,
                                                             ServiceCommands.get_user_by_workstation,
                                                             ServiceCommands.create_user_by_template,
                                                             ServiceCommands.create_user_in_container,
-                                                            ServiceCommands.set_user_telephone,
+                                                            ServiceCommands.set_user_telephone_number,
                                                             ServiceCommands.set_user_password,
                                                             ServiceCommands.set_user_status,
-                                                            ServiceCommands.remove_user
-                                                        ],
-                                                modules=["pyad", "pywin32", "wmi"]
-                                            )
+                                                            ServiceCommands.remove_user,
+                                                            ServiceCommands.drop_user_cache
 
-    DOCS: ServiceRoleDescription = ServiceRoleDescription(
-                                                name="Docs", 
-                                                description="Documents service",
-                                                host=CONST.HOST.DC2.NAME,
-                                                port=CONST.RPC.PORT(1),
-                                                commands=
-                                                        [
-                                                            ServiceCommands.get_inventory_report,
-                                                            ServiceCommands.create_user_document,
-                                                            ServiceCommands.save_time_tracking_report,
-                                                            ServiceCommands.create_barcodes_for_inventory,
-                                                            ServiceCommands.create_barcode_for_polibase_person,
-                                                            ServiceCommands.create_qr_code,
-                                                            ServiceCommands.check_inventory_report,
-                                                            ServiceCommands.save_inventory_report_item,
-                                                            ServiceCommands.close_inventory_report,
                                                         ],
-        modules=["xlsxwriter", "xlrd", "xlutils", "openpyxl",
-                                                    "python-barcode", "Pillow", "transliterate", "qrcode"]
+                                                modules=["pyad", "pywin32", "wmi"]
                                             )
+    WS: ServiceDescription = ServiceDescription(
+                                                name="WS",
+                                                description="Workstation service",
+                                                host=CONST.HOST.BACKUP_WORKER.NAME,
+                                                commands=[
+                                                    ServiceCommands.reboot,
+                                                    ServiceCommands.shutdown,
+                                                    ServiceCommands.send_message_to_user_or_workstation,
+                                                    ServiceCommands.kill_process
+                                                ])
 
-    PRINTER: ServiceRoleDescription = ServiceRoleDescription(
+    PRINTER: ServiceDescription = ServiceDescription(
                                                     name="Printer",
                                                     description="Printer service", 
                                                     host=CONST.HOST.DC2.NAME, 
-                                                    port=CONST.RPC.PORT(2),
                                                     commands=
                                                             [
                                                                 ServiceCommands.printers_report,
                                                                 ServiceCommands.printers_status
                                                             ]
                                                            )
+    
+    DOCS: ServiceDescription = ServiceDescription(
+                                                            name="Docs",
+                                                            description="Documents service",
+                                                            host=CONST.HOST.DC2.NAME,
+                                                            commands=[
+                                                                ServiceCommands.get_inventory_report,
+                                                                ServiceCommands.create_user_document,
+                                                                ServiceCommands.save_time_tracking_report,
+                                                                ServiceCommands.create_barcodes_for_inventory,
+                                                                ServiceCommands.create_barcode_for_polibase_person,
+                                                                ServiceCommands.create_qr_code,
+                                                                ServiceCommands.check_inventory_report,
+                                                                ServiceCommands.save_inventory_report_item,
+                                                                ServiceCommands.close_inventory_report,
+                                                                ServiceCommands.create_note,
+                                                                ServiceCommands.get_note,
+                                                            ],
+                                                            modules=["xlsxwriter", "xlrd", "xlutils", "openpyxl",
+                                                                    "python-barcode", "Pillow", "transliterate", "qrcode", "docx-mailmerge", "gkeepapi"]
+                                                        )
 
-    MARK: ServiceRoleDescription = ServiceRoleDescription(
+    MARK: ServiceDescription = ServiceDescription(
                                                 name="Orion",
                                                 description="Orion service",
                                                 host=CONST.HOST.DC2.NAME,
-                                                port=CONST.RPC.PORT(3),
                                                 commands=
                                                         [
                                                             ServiceCommands.get_free_marks,
                                                             ServiceCommands.get_temporary_marks,
                                                             ServiceCommands.get_person_divisions,
                                                             ServiceCommands.get_time_tracking,
                                                             ServiceCommands.get_all_persons,
@@ -1504,19 +1545,20 @@
                                                             ServiceCommands.create_mark,
                                                             ServiceCommands.make_mark_as_free_by_tab_number,
                                                             ServiceCommands.make_mark_as_temporary,
                                                             ServiceCommands.remove_mark_by_tab_number,
                                                         ],
                                                modules=["pymssql"])
 
-    POLIBASE: ServiceRoleDescription = ServiceRoleDescription(
+    POLIBASE: ServiceDescription = ServiceDescription(
                                                     name="Polibase",
                                                     description="Polibase service & FastApi server",
-                                                    host=CONST.HOST.POLIBASE.NAME,
-                                                    port=CONST.RPC.PORT(1),
+                                                    host=POLIBASE_BASE.host, 
+                                                    pyton_executor_path=POLIBASE_BASE.pyton_executor_path,
+                                                    run_from_system_account=POLIBASE_BASE.run_from_system_account,
                                                     commands=[
                                                                 ServiceCommands.get_polibase_person_by_pin,
                                                                 ServiceCommands.get_polibase_persons_by_pin,
                                                                 ServiceCommands.get_polibase_persons_by_telephone_number,
                                                                 ServiceCommands.get_polibase_persons_by_full_name,
                                                                 ServiceCommands.get_polibase_persons_by_card_registry_folder_name,
                                                                 ServiceCommands.get_polibase_person_registrator_by_pin,
@@ -1526,166 +1568,189 @@
                                                                 #
                                                                 ServiceCommands.search_polibase_person_visits,
                                                                 ServiceCommands.get_polibase_person_visits_last_id,
                                                                 #
                                                                 ServiceCommands.set_polibase_person_card_folder_name,
                                                                 ServiceCommands.set_polibase_person_email,
                                                                 ServiceCommands.set_polibase_person_barcode_by_pin,
-                                                                ServiceCommands.check_polibase_person_card_registry_folder_name
+                                                                ServiceCommands.check_polibase_person_card_registry_folder_name,
+                                                                ServiceCommands.set_polibase_person_telephone_number,
+                                                                ServiceCommands.get_polibase_person_operator_by_pin
                                                             ], 
                                                     modules=["cx-Oracle", "fastapi", "uvicorn", "transliterate"])
 
-    POLIBASE_DATABASE: ServiceRoleDescription = ServiceRoleDescription(
+    POLIBASE_DATABASE: ServiceDescription = ServiceDescription(
         name="PolibaseDB",
         description="Polibase database api",
-        host=CONST.HOST.POLIBASE.NAME,
-        port=CONST.RPC.PORT(2),
+        host=POLIBASE_BASE.host, 
+        pyton_executor_path=POLIBASE_BASE.pyton_executor_path,
+        run_from_system_account=POLIBASE_BASE.run_from_system_account,
         commands=[
                     ServiceCommands.create_polibase_database_backup
                 ],
         )
 
-    POLIBASE_APP: ServiceRoleDescription = ServiceRoleDescription(
+    POLIBASE_APP: ServiceDescription = ServiceDescription(
         name="PolibaseApp",
         description="Polibase Application service",
-        host=CONST.HOST.POLIBASE.NAME,
-        port=CONST.RPC.PORT(3)
+        host=POLIBASE_BASE.host, 
+        pyton_executor_path=POLIBASE_BASE.pyton_executor_path,
+        run_from_system_account=POLIBASE_BASE.run_from_system_account,
         )
 
-    MESSAGE_QUEUE: ServiceRoleDescription = ServiceRoleDescription(
+    MESSAGE_QUEUE: ServiceDescription = ServiceDescription(
         name="MessageQueue",
         description="Message queue service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
-        port=CONST.RPC.PORT(100),
         commands=[
             ServiceCommands.add_message_to_queue
         ]
         )
 
-    POLIBASE_PERSON_NOTIFICATION: ServiceRoleDescription = ServiceRoleDescription(
+    POLIBASE_PERSON_NOTIFICATION: ServiceDescription = ServiceDescription(
         name="PolibasePersonNotification",
         description="Polibase Person Notification service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
-        port=CONST.RPC.PORT(7)
         )
     
-    POLIBASE_PERSON_INFORMATION_QUEST: ServiceRoleDescription = ServiceRoleDescription(
+    POLIBASE_PERSON_INFORMATION_QUEST: ServiceDescription = ServiceDescription(
         name="PolibasePersonInformationQuest",
         description="Polibase Person Information Quest service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
-        port=CONST.RPC.PORT(10),
-         commands=[
+        commands=[
             ServiceCommands.start_polibase_person_information_quest
         ]
         )
     
-    POLIBASE_PERSON_REVIEW_NOTIFICATION: ServiceRoleDescription = ServiceRoleDescription(
+    POLIBASE_PERSON_REVIEW_NOTIFICATION: ServiceDescription = ServiceDescription(
         name="PolibasePersonReviewNotification",
         description="Polibase Person Review Notification service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
-        port=CONST.RPC.PORT(11)
         )
     
-    MESSAGE_RECEIVER: ServiceRoleDescription = ServiceRoleDescription(
+    MESSAGE_RECEIVER: ServiceDescription = ServiceDescription(
         name="MessageReceiver",
         description="Message service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
-        port=CONST.RPC.PORT(101),
-        auto_restart=False,
+        host_changabled=False,
         modules=["fastapi", "uvicorn"])
 
-    SSH: ServiceRoleDescription = ServiceRoleDescription(
+    SSH: ServiceDescription = ServiceDescription(
         name="SSH",
         description="Ssh service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
-        port=CONST.RPC.PORT(9),
         modules=["paramiko"],
         commands=[ServiceCommands.execute_ssh_command,
                   ServiceCommands.get_certificate_information,
                   ServiceCommands.get_unix_free_space_information_by_drive_name]
     )
 
-    WS_735: ServiceRoleDescription = ServiceRoleDescription(
+    WS_735: ServiceDescription = ServiceDescription(
         name="ws_735",
         description="ws-735 service",
         host=CONST.HOST.WS735.NAME,
-        port=CONST.RPC.PORT(),
         login="nak",
         password="Soad7623!",
         commands=[ServiceCommands.print_image],
         modules=["pywin32", "Pillow"]
     )
 
-    RECOGNIZE: ServiceRoleDescription = ServiceRoleDescription(
+    RECOGNIZE: ServiceDescription = ServiceDescription(
         name="Recognize",
         description="Recognize service",
         host=CONST.HOST.WS255.NAME,
-        port=CONST.RPC.PORT(-2)
+        host_changabled=False,
+        commands=[
+            ServiceCommands.get_barcode_list_information,
+            ServiceCommands.document_type_exists
+        ]
+    )
+
+    FILE_OGANIZER: ServiceDescription = ServiceDescription(
+        name="FileOrganizer",
+        description="File organizer service",
+        host=CONST.HOST.WS255.NAME
     )
 
-    RECOGNIZE_TEST: ServiceRoleDescription = ServiceRoleDescription(
+    RECOGNIZE_TEST: ServiceDescription = ServiceDescription(
         name="RecognizeTest",
         description="Recognize test service",
         host=CONST.HOST.WS255.NAME,
-        port=CONST.RPC.PORT(-3),
         auto_start=False,
         auto_restart=False,
         visible_for_admin=False
     )
 
-    CHECKER: ServiceRoleDescription = ServiceRoleDescription(
+    INDICATIONS: ServiceDescription = ServiceDescription(
+        name="Indications",
+        description="Indications service",
+        host=CONST.HOST.WS255.NAME,
+        modules=["fastapi", "uvicorn", "python-multipart"]
+    )
+
+    CHECKER: ServiceDescription = ServiceDescription(
         name="Checker",
         description="Checker service",
         host=CONST.HOST.BACKUP_WORKER.NAME,
-        commands=[ServiceCommands.get_resource_status_list],
-        port=CONST.RPC.PORT(8)
+        commands=[ServiceCommands.get_resource_status_list]
     )
 
-    AUTOMATION: ServiceRoleDescription = ServiceRoleDescription(
+    AUTOMATION: ServiceDescription = ServiceDescription(
         name="Automation",
         description="Automation service",
-        host=CONST.HOST.WS255.NAME,
-        port=CONST.RPC.PORT(-1)
+        host=HOSTS.BACKUP_WORKER.NAME
     )
 
-    MOBILE_HELPER: ServiceRoleDescription = ServiceRoleDescription(
+    MOBILE_HELPER: ServiceDescription = ServiceDescription(
         name="MobileHelper",
         description="Mobile helper service",
         host=CONST.HOST.WS255.NAME,
         commands=[ServiceCommands.send_mobile_helper_message],
-        port=CONST.RPC.PORT(4)
+        auto_restart=False,
+        modules=["requests"]
     )
 
-    DEVELOPER: ServiceRoleDescription = ServiceRoleDescription(
+    REGISTRATOR_HELPER: ServiceDescription = ServiceDescription(
+        name="RegistratorHelper",
+        description="Registrator mobile helper service",
+        host=HOSTS.BACKUP_WORKER.NAME
+    )
+
+    DEVELOPER: ServiceDescription = ServiceDescription(
         name="Developer",
         description="Developer service",
         host=CONST.HOST.DEVELOPER.NAME,
         port=CONST.RPC.PORT(1),
         visible_for_admin=False,
         auto_start=False,
         auto_restart=False,
         commands=[ServiceCommands.test]
     )
 
+    STUB: ServiceDescription = ServiceDescription(
+        name="Stub",
+        visible_for_admin=False,
+    )
+
 class SubscribtionTypes:
-    BEFORE: int = 1
-    AFTER: int = 2
+    ON_PARAMETERS: int = 1
+    ON_RESULT: int = 2
+    ON_RESULT_SEQUENTIALLY: int = 4
 
 class WorkstationMessageMethodTypes(Enum):
 
     REMOTE: int = auto()
     LOCAL_MSG: int = auto()
     LOCAL_PSTOOL_MSG: int = auto()
 
 class MessageTypes(Enum):
 
-    WHATSAPP: int = 1
-    TELEGRAM: int = 2
-    INTERNAL: int = 3
-
+    WHATSAPP: int = auto()
+    TELEGRAM: int = auto()
+    WORKSTATION: int = auto()
 
 class MessageStatuses(Enum):
 
     REGISTERED: int = 0
     COMPLETE: int = 1
     AT_WORK: int = 2
     ERROR: int = 3
@@ -1706,254 +1771,314 @@
 105 - не пришел	
 106 - предварительно
 107 - подверждено
 108 - оказано
 109 к оплате
 """
 
+class SCAN:
+    
+    SPLITTER_DATA: str = "1"
+    
+    class SOURCES(Enum):
+
+        POLICLINIC: tuple[str, str, str] = ("poly", "Поликлиника", PATH_SCAN.VALUE)
+        DIAGNOSTICS: tuple[str, str, str] = (
+            "diag", "Приёмное отделение", PATH_SCAN.VALUE)
+        TEST: tuple[str, str, str] = ("test", "Тестовый", PATH_SCAN_TEST.VALUE)
+        WS_816: tuple[str, str, str] = (
+            HOSTS.WS816, "Дневной стационар", PATH_WS_816_SCAN.VALUE)
+
+
 class SETTINGS(Enum):
 
-    VALENTA_SYNCHRONIZATION_TEST: SettingsValue = SettingsValue(None, False)
+    CHILLER_RECOGNIZE_LOG_LEVEL: IntStorageValue = IntStorageValue(
+        "CHILLER_RECOGNIZE_LOG_LEVEL", 0)
+
+    HEAT_BEAT_IS_ON: BoolStorageValue = BoolStorageValue(
+        "HEAT_BEAT_IS_ON", True)
+
+    CT_INDICATIONS_VALUE_TEMPERATURE_CORRECTION: IntStorageValue = IntStorageValue("CT_INDICATIONS_VALUE_TEMPERATURE_CORRECTION", 0.7)
+    CT_INDICATIONS_VALUE_SAVE_PERIOD_IN_MINUTES: IntStorageValue = IntStorageValue("CT_INDICATIONS_VALUE_SAVE_PERIOD_IN_MINUTES", 60)
 
-    CT_TEMPERATURE_CORRECTION: SettingsValue = SettingsValue(None, 0.7)
+    CHILLER_INDICATIONS_VALUE_SAVE_PERIOD_IN_MINUTES: IntStorageValue = IntStorageValue("CHILLER_INDICATIONS_VALUE_SAVE_PERIOD_IN_MINUTES", 60)
 
-    HOSPITAL_WORK_DAY_START_TIME: SettingsValue = SettingsValue(None, "8:00")
-    HOSPITAL_WORK_DAY_END_TIME: SettingsValue = SettingsValue(None, "20:00")
-    OFFICE_WORK_DAY_START_TIME: SettingsValue = SettingsValue(None, "8:30")
-    OFFICE_WORK_DAY_END_TIME: SettingsValue = SettingsValue(None, "17:00")
+    HOSPITAL_WORK_DAY_START_TIME: TimeStorageValue = TimeStorageValue("HOSPITAL_WORK_DAY_START_TIME", "8:30")
+    HOSPITAL_WORK_DAY_END_TIME: TimeStorageValue = TimeStorageValue("HOSPITAL_WORK_DAY_END_TIME", "20:00")
+    OFFICE_WORK_DAY_START_TIME: TimeStorageValue = TimeStorageValue("OFFICE_WORK_DAY_START_TIME", "8:30")
+    OFFICE_WORK_DAY_END_TIME: TimeStorageValue = TimeStorageValue(
+        "OFFICE_WORK_DAY_END_TIME", "17:00")
 
 
-    INDICATION_CT_NOTIFICATION_START_TIME: SettingsValue = SettingsValue(None, ["8:00", "17:00"])
+    INDICATION_CT_NOTIFICATION_START_TIME: DateListStorageValue = DateListStorageValue("INDICATION_CT_NOTIFICATION_START_TIME", ["8:00", "12:00", "15:00", "17:00"])
 
-    USER_USE_CACHE: SettingsValue = SettingsValue(None, 1)
+    USER_USE_CACHE: BoolStorageValue = BoolStorageValue(
+        "USER_USE_CACHE", True)
     
-    POLIBASE_PERSON_INFORMATION_QUEST_IS_ON: SettingsValue = SettingsValue(None, True)
+    POLIBASE_PERSON_INFORMATION_QUEST_IS_ON: BoolStorageValue = BoolStorageValue(
+        "POLIBASE_PERSON_INFORMATION_QUEST_IS_ON", False)
     #
-    POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON: SettingsValue = SettingsValue(None, True)
+    POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON: BoolStorageValue = BoolStorageValue(
+        "POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON", True)
 
-    POLIBASE_PERSON_REVIEW_NOTIFICATION_DAY_DELTA: SettingsValue = SettingsValue(None, 1)
+    POLIBASE_PERSON_REVIEW_NOTIFICATION_DAY_DELTA: StorageValue = StorageValue(
+        "POLIBASE_PERSON_REVIEW_NOTIFICATION_DAY_DELTA", 1)
 
-    POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION: SettingsValue = SettingsValue(
-        None, CONST.POLIBASE.PERSON_REVIEW_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION)
+    POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION: StorageValue = StorageValue(
+        "POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION", CONST.POLIBASE.PERSON_REVIEW_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION)
 
-    POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT: SettingsValue = SettingsValue(
-        None, CONST.POLIBASE.PERSON_REVIEW_NOTIFICATION_TEXT)
+    POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT: StorageValue = StorageValue(
+        "POLIBASE_PERSON_REVIEW_NOTIFICATION_TEXT", CONST.POLIBASE.PERSON_REVIEW_NOTIFICATION_TEXT)
 
-    POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME: SettingsValue = SettingsValue(None, "13:53")
+    POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME: TimeStorageValue = TimeStorageValue("POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME", "13:00")
     #
-    RESOURCE_MANAGER_CHECK_SITE_CERTIFICATE_START_TIME: SettingsValue = SettingsValue(None, "8:00")
+    RESOURCE_MANAGER_CHECK_SITE_CERTIFICATE_START_TIME: TimeStorageValue = TimeStorageValue("RESOURCE_MANAGER_CHECK_SITE_CERTIFICATE_START_TIME", "8:00")
     #
-    POLIBASE_CREATION_DB_DUMP_START_TIME: SettingsValue = SettingsValue(None, "20:30")
+    POLIBASE_CREATION_DB_DUMP_START_TIME: TimeStorageValue = TimeStorageValue(
+        "POLIBASE_CREATION_DB_DUMP_START_TIME", "20:30")
     #
-    RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES: SettingsValue = SettingsValue(None, 15)
+    RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES: IntStorageValue = IntStorageValue(
+        "RESOURCE_MANAGER_CHECK_SITE_FREE_SPACE_PERIOD_IN_MINUTES", 15)
     #
-    POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE_FOR_CONFIRMED_NOTIFICATION: SettingsValue = SettingsValue(
-        None, CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION + CONST.POLIBASE.SEND_TELEGRAM_BOT_TEXT)
+    POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE_FOR_CONFIRMED_NOTIFICATION: StorageValue = StorageValue(
+        "POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE_FOR_CONFIRMED_NOTIFICATION", CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION + CONST.POLIBASE.SEND_TELEGRAM_BOT_TEXT)
 
-    POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE: SettingsValue = SettingsValue(
-        None, CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_TEXT)
+    POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE: StorageValue = StorageValue(
+        "POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_DATE", CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_WITHOUT_TEXT)
 
-    POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION: SettingsValue = SettingsValue(
-        None,  CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION + CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_WITH_TIME_TEXT + CONST.POLIBASE.SEND_TELEGRAM_BOT_TEXT)
+    POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION: StorageValue = StorageValue(
+        "POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION",  CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_FOR_CONFIRMED_NOTIFICATION + CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_WITH_TIME_TEXT + CONST.POLIBASE.SEND_TELEGRAM_BOT_TEXT)
     
-    POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT: SettingsValue = SettingsValue(
-        None,  CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_BASE + CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_WITH_TIME_TEXT + CONST.POLIBASE.ASK_TO_SEND_TELEGRAM_BOT_URL_TEXT)
+    POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT: StorageValue = StorageValue(
+        "POLIBASE_PERSON_VISIT_GREETING_NOTIFICATION_TEXT",  CONST.POLIBASE.PERSON_VISIT_GREETING_NOTIFICATION_TEXT_BASE + CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_WITH_TIME_TEXT + CONST.POLIBASE.ASK_TO_SEND_TELEGRAM_BOT_URL_TEXT)
 
-    POLIBASE_PERSON_VISIT_NOTIFICATION_TEXT: SettingsValue = SettingsValue(
-        None, CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_HEADER + CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_APPOINTMENT_INFORMATION + CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_WITH_TIME_TEXT)
+    POLIBASE_PERSON_VISIT_NOTIFICATION_TEXT: StorageValue = StorageValue(
+        "POLIBASE_PERSON_VISIT_NOTIFICATION_TEXT", CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_HEADER + CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_APPOINTMENT_INFORMATION + CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_WITH_TIME_TEXT)
 
-    POLIBASE_PERSON_VISIT_REMINDER_TEXT: SettingsValue = SettingsValue(
-        None, CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_HEADER + "*{name}*, напоминаем Вам о записи сегодня {visit_time}. Вы записаны на {appointment_information}." + CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_TEXT_CANCEL_OR_REPLACE_RECEPTION)
+    POLIBASE_PERSON_VISIT_REMINDER_TEXT: StorageValue = StorageValue(
+        "POLIBASE_PERSON_VISIT_REMINDER_TEXT", CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_HEADER + "*{name}*, напоминаем Вам о записи сегодня {visit_time}. Вы записаны на {appointment_information}." + CONST.POLIBASE.PERSON_VISIT_NOTIFICATION_TEXT_CANCEL_OR_REPLACE_RECEPTION)
 
-    POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_TEXT: SettingsValue = SettingsValue(
-        None, CONST.POLIBASE.TAKE_TELEGRAM_BOT_URL_TEXT)
+    POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_TEXT: StorageValue = StorageValue(
+        "POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_TEXT", CONST.POLIBASE.TAKE_TELEGRAM_BOT_URL_TEXT)
 
-    POLIBASE_PERSON_TAKE_REVIEW_ACTION_URL_TEXT: SettingsValue = SettingsValue(
-         None, CONST.POLIBASE.TAKE_REVIEW_ACTION_URL_TEXT)
+    POLIBASE_PERSON_TAKE_REVIEW_ACTION_URL_TEXT: StorageValue = StorageValue(
+         "POLIBASE_PERSON_TAKE_REVIEW_ACTION_URL_TEXT", CONST.POLIBASE.TAKE_REVIEW_ACTION_URL_TEXT)
 
-    POLIBASE_PERSON_YES_ANSWER_VARIANTS: SettingsValue = SettingsValue(
-        None, CONST.POLIBASE.YES_ANSWER)
+    POLIBASE_PERSON_YES_ANSWER_VARIANTS: StorageValue = StorageValue(
+        "POLIBASE_PERSON_YES_ANSWER_VARIANTS", CONST.POLIBASE.YES_ANSWER)
 
-    POLIBASE_PERSON_NO_ANSWER_VARIANTS: SettingsValue = SettingsValue(
-        None, CONST.POLIBASE.NO_ANSWER)
+    POLIBASE_PERSON_NO_ANSWER_VARIANTS: StorageValue = StorageValue(
+        "POLIBASE_PERSON_NO_ANSWER_VARIANTS", CONST.POLIBASE.NO_ANSWER)
 
-    POLIBASE_PERSON_NO_ANSWER_ON_NOTIFICATION_CONFIRMATION_TEXT: SettingsValue = SettingsValue(
-        None, "Хорошего дня")
+    POLIBASE_PERSON_NO_ANSWER_ON_NOTIFICATION_CONFIRMATION_TEXT: StorageValue = StorageValue(
+        "POLIBASE_PERSON_NO_ANSWER_ON_NOTIFICATION_CONFIRMATION_TEXT", "Хорошего дня")
 
-    POLIBASE_PERSON_REVIEW_QUEST_WAIT_TIME: SettingsValue = SettingsValue(
-        None, 15)
+    POLIBASE_PERSON_REVIEW_QUEST_WAIT_TIME: IntStorageValue = IntStorageValue(
+        "POLIBASE_PERSON_REVIEW_QUEST_WAIT_TIME", 15)
     #
-    POLIBASE_PERSON_VISIT_NEED_REGISTER_GREETING_NOTIFICATION: SettingsValue = SettingsValue(
-        None, True)
+    POLIBASE_PERSON_VISIT_NEED_REGISTER_GREETING_NOTIFICATION: BoolStorageValue = BoolStorageValue(
+        "POLIBASE_PERSON_VISIT_NEED_REGISTER_GREETING_NOTIFICATION", True)
     
-    POLIBASE_PERSON_VISIT_NEED_REGISTER_REMINDER_NOTIFICATION: SettingsValue = SettingsValue(
-        None, True)
+    POLIBASE_PERSON_VISIT_NEED_REGISTER_REMINDER_NOTIFICATION: BoolStorageValue = BoolStorageValue(
+        "POLIBASE_PERSON_VISIT_NEED_REGISTER_REMINDER_NOTIFICATION", True)
     
-    POLIBASE_PERSON_VISIT_TIME_BEFORE_REMINDER_NOTIFICATION_IN_MINUTES: SettingsValue = SettingsValue(
-        None, 120)
+    POLIBASE_PERSON_VISIT_TIME_BEFORE_REMINDER_NOTIFICATION_IN_MINUTES: IntStorageValue = IntStorageValue(
+        "POLIBASE_PERSON_VISIT_TIME_BEFORE_REMINDER_NOTIFICATION_IN_MINUTES", 120)
     
-    POLIBASE_PERSON_VISIT_NEED_CONFIRMATION_STATUS_TO_SEND_NOTIFICATION: SettingsValue = SettingsValue(
-        None, True)
+    POLIBASE_PERSON_VISIT_NEED_CONFIRMATION_STATUS_TO_SEND_NOTIFICATION: BoolStorageValue = BoolStorageValue(
+        "POLIBASE_PERSON_VISIT_NEED_CONFIRMATION_STATUS_TO_SEND_NOTIFICATION", True)
     
-    POLIBASE_PERSON_VISIT_NOTIFICATION_TEST_TELEPHONE_NUMBER: SettingsValue = SettingsValue(
-        None, "+79146717744")
+    POLIBASE_PERSON_VISIT_NOTIFICATION_TEST_TELEPHONE_NUMBER: StorageValue = StorageValue(
+        "POLIBASE_PERSON_VISIT_NOTIFICATION_TEST_TELEPHONE_NUMBER", None)
 
-    POLIBASE_PERSON_REVIEW_NOTIFICATION_TEST_TELEPHONE_NUMBER: SettingsValue = SettingsValue(
-        None, None)
+    POLIBASE_PERSON_REVIEW_NOTIFICATION_TEST_TELEPHONE_NUMBER: StorageValue = StorageValue(
+        "POLIBASE_PERSON_REVIEW_NOTIFICATION_TEST_TELEPHONE_NUMBER", None)
     
-    WHATSAPP_SENDING_MESSAGES_VIA_WAPPI_IS_ON: SettingsValue = SettingsValue(
-        None, True)
+    WHATSAPP_SENDING_MESSAGES_VIA_WAPPI_IS_ON: BoolStorageValue = BoolStorageValue(
+        "WHATSAPP_SENDING_MESSAGES_VIA_WAPPI_IS_ON", True)
     
-    WHATSAPP_BUFFERED_MESSAGE_MIN_DELAY_IN_MILLISECONDS: SettingsValue = SettingsValue(
-        None, 6000)
+    WHATSAPP_BUFFERED_MESSAGE_MIN_DELAY_IN_MILLISECONDS: IntStorageValue = IntStorageValue(
+        "WHATSAPP_BUFFERED_MESSAGE_MIN_DELAY_IN_MILLISECONDS", 6000)
     
-    WHATSAPP_BUFFERED_MESSAGE_MAX_DELAY_IN_MILLISECONDS: SettingsValue = SettingsValue(
-        None, 12000)
+    WHATSAPP_BUFFERED_MESSAGE_MAX_DELAY_IN_MILLISECONDS: IntStorageValue = IntStorageValue(
+        "WHATSAPP_BUFFERED_MESSAGE_MAX_DELAY_IN_MILLISECONDS", 12000)
     
-    WHATSAPP_MESSAGE_SENDER_USER_LOGIN: SettingsValue = SettingsValue(
-        None, "Administrator")  # callCentreAdmin
+    WHATSAPP_MESSAGE_SENDER_USER_LOGIN: StorageValue = StorageValue(
+        "WHATSAPP_MESSAGE_SENDER_USER_LOGIN", "Administrator")
+    # callCentreAdmin
 
-    MOBILE_HELPER_USER_DATA_INPUT_TIMEOUT: SettingsValue = SettingsValue(
-        None, CONST.MOBILE_HELPER.USER_DATA_INPUT_TIMEOUT)
+    MOBILE_HELPER_USER_DATA_INPUT_TIMEOUT: IntStorageValue = IntStorageValue(
+        "MOBILE_HELPER_USER_DATA_INPUT_TIMEOUT", CONST.MOBILE_HELPER.USER_DATA_INPUT_TIMEOUT)
     
-    POLIBASE_WAS_EMERGENCY_CLOSED_NOTIFICATION_TEXT: SettingsValue = SettingsValue(
-        None, "к сожалениию наш Полибейс поломался и был аварийно закрыт, ожидайте сообщение о просьбе переоткрыть его!")
+    POLIBASE_WAS_EMERGENCY_CLOSED_NOTIFICATION_TEXT: StorageValue = StorageValue(
+        "POLIBASE_WAS_EMERGENCY_CLOSED_NOTIFICATION_TEXT", "к сожалениию наш Полибейс поломался и был аварийно закрыт, ожидайте сообщение о просьбе переоткрыть его!")
     
-    POLIBASE_WAS_RESTARTED_NOTIFICATION_TEXT: SettingsValue = SettingsValue(
-        None, "Полибейс перезагружен, можете переоткрыть его.")
+    POLIBASE_WAS_RESTARTED_NOTIFICATION_TEXT: StorageValue = StorageValue(
+        "POLIBASE_WAS_RESTARTED_NOTIFICATION_TEXT", "Полибейс перезагружен, можете переоткрыть его.")
     
-    WORKSTATION_SHUTDOWN_TIME: SettingsValue = SettingsValue(None, "21:00")
+    WORKSTATION_SHUTDOWN_TIME: TimeStorageValue = TimeStorageValue("WORKSTATION_SHUTDOWN_TIME", "21:00")
+
+    WORKSTATION_REBOOT_TIME: TimeStorageValue = TimeStorageValue("WORKSTATION_REBOOT_TIME", "21:00")
+
+    EMAIL_VALIDATION_IS_ON: BoolStorageValue = BoolStorageValue("EMAIL_VALIDATION_IS_ON", True)
+    EMAIL_VALIDATION_TEST: BoolStorageValue = BoolStorageValue("EMAIL_VALIDATION_TEST", False)
 
-    WORKSTATION_REBOOT_TIME: SettingsValue = SettingsValue(None, "21:00")
+    CHILLER_ALERT_TEMPEARTURE: FloatStorageValue = FloatStorageValue(
+        "CHILLER_ALERT_TEMPEARTURE", 17.0)
+    
+class PARAM_ITEMS:
 
+    NAME: ParamItem = ParamItem(FIELD_NAME_COLLECTION.NAME, "")
+    PID: ParamItem = ParamItem(FIELD_NAME_COLLECTION.PID, "")
+    STATUS: ParamItem = ParamItem(FIELD_NAME_COLLECTION.STATUS, "")
 
-class LogCommands(Enum):
+class Events(Enum):
 
-    DEBUG: LogCommandDescription = LogCommandDescription(
-        "It is a debug command", LogChannels.NOTIFICATION, LogLevels.DEBUG.value)
+    DEBUG: EventDescription = EventDescription(
+        "It is a debug event", LogMessageChannels.POLIBASE_NOTIFICATIONS, LogMessageFlags.DEBUG.value)
         
-    PRINTER_REPORT: LogCommandDescription = LogCommandDescription("Принтер {printer_name} ({location}):\n {printer_report}", LogChannels.PRINTER, LogLevels.NORMAL.value, (ParamItem(
+    PRINTER_REPORT: EventDescription = EventDescription("Принтер {printer_name} ({location}):\n {printer_report}", LogMessageChannels.PRINTER, LogMessageFlags.NORMAL, (ParamItem(
         "printer_name", "Name of printer"), ParamItem("location", "Location"), ParamItem("printer_report", "Printer report")))
     #
-    LOG_IN: LogCommandDescription = LogCommandDescription(
-        "Пользователь {full_name} ({login}) вошел с компьютера {computer_name}", LogChannels.IT, LogLevels.NORMAL.value, (ParamItem("full_name", "Name of user"), ParamItem("login", "Login of user"), ParamItem("computer_name", "Name of computer")))
-
-    SESSION_STARTED: LogCommandDescription = LogCommandDescription(
-        "Пользователь {full_name} ({login}) начал пользоваться программой {app_name}.\nВерсия: {version}.\nНазвание компьютера: {computer_name}", LogChannels.IT, LogLevels.NORMAL.value, (ParamItem("full_name", "Name of user"), ParamItem("login", "Login of user"), ParamItem("app_name", "Name of user"),  ParamItem("version", "Version"), ParamItem("computer_name", "Name of computer")))
+    LOG_IN: EventDescription = EventDescription(
+        "Пользователь {full_name} ({login}) вошел с компьютера {computer_name}", LogMessageChannels.IT, LogMessageFlags.NORMAL, (ParamItem("full_name", "Name of user"), ParamItem("login", "Login of user"), ParamItem("computer_name", "Name of computer")))
 
-    SERVICE_STARTS: LogCommandDescription = LogCommandDescription(
-        "Сервис {service_name} ({service_description}) запускается!\nИмя хоста: {host_name}\nПорт: {port}\nИдентификатор процесса: {pid}\n", LogChannels.SERVICE, LogLevels.SILENCE.value, (ParamItem("service_name", "Name of service"), ParamItem("service_description", "Description of service"), ParamItem("host_name", "Name of host"), ParamItem("port", "Port"), ParamItem("pid", "PID")))
+    SESSION_STARTED: EventDescription = EventDescription(
+        "Пользователь {full_name} ({login}) начал пользоваться программой {app_name}.\nВерсия: {version}.\nНазвание компьютера: {computer_name}", LogMessageChannels.IT, LogMessageFlags.NORMAL, (ParamItem("full_name", "Name of user"), ParamItem("login", "Login of user"), ParamItem("app_name", "Name of user"),  ParamItem("version", "Version"), ParamItem("computer_name", "Name of computer")))
     
-    SERVICE_STARTED: LogCommandDescription = LogCommandDescription(
-        "Сервис {service_name} ({service_description}) запущен!\nИмя хоста: {host_name}\nПорт: {port}\nИдентификатор процесса: {pid}\n", LogChannels.SERVICE, LogLevels.NORMAL.value, (ParamItem("service_name", "Name of service"), ParamItem("service_description", "Description of service"), ParamItem("host_name", "Name of host"), ParamItem("port", "Port"), ParamItem("pid", "PID")))
+    SERVICE_WAS_STARTED: EventDescription = EventDescription(
+        "Сервис {service_name} запущен!\nИмя хоста: {host_name}\nПорт: {port}\nИдентификатор процесса: {pid}\n", LogMessageChannels.SERVICES, LogMessageFlags.NORMAL, (ParamItem("service_name", "Name of service"), ParamItem("host_name", "Name of host"), ParamItem("port", "Port"), ParamItem("pid", "PID"), ParamItem("service_information", "Service information")))
     
-    SERVICE_NOT_STARTED: LogCommandDescription = LogCommandDescription(
-        "Сервис {service_name} ({service_description}) не запущен!\nИмя хоста: {host_name}\nПорт: {port}\nОшибка:{error}", LogChannels.SERVICE, LogLevels.ERROR.value, (ParamItem("service_name", "Name of service"), ParamItem("service_description", "Description of service"), ParamItem("host_name", "Name of host"), ParamItem("port", "Port"), ParamItem("error", "Error")))
+    SERVICE_WAS_STOPPED: EventDescription = EventDescription(
+        "Сервис {service_name} остановлен!", LogMessageChannels.SERVICES, LogMessageFlags.NORMAL, (ParamItem("service_name", "Name of service"), ParamItem("service_information", "Service information")))
+
+    SERVICE_WAS_NOT_STARTED: EventDescription = EventDescription(
+        "Сервис {service_name} не запущен!\nИмя хоста: {host_name}\nПорт: {port}\nОшибка:{error}", LogMessageChannels.SERVICES, LogMessageFlags.ERROR, (ParamItem("service_name", "Name of service"), ParamItem("host_name", "Name of host"), ParamItem("port", "Port"), ParamItem("error", "Error"), ParamItem("service_information", "Service information")))
 
-    SERVICE_IS_INACCESIBLE_AND_WAITING_TO_BE_RESTARTED: LogCommandDescription = LogCommandDescription(
-        "Сервис {service_name} ({service_description}) недоступен и будет перезапущен!\nИмя хоста: {host_name}\nПорт: {port}\nИдентификатор процесса: {pid}\n", LogChannels.SERVICE, LogLevels.ERROR.value, (ParamItem("service_name", "Name of service"), ParamItem("service_description", "Description of service"), ParamItem("host_name", "Name of host"), ParamItem("port", "Port"), ParamItem("pid", "PID")))
+    SERVICE_IS_INACCESIBLE_AND_WILL_BE_RESTARTED: EventDescription = EventDescription(
+        "Сервис {service_name} недоступен и будет перезапущен!\n", LogMessageChannels.SERVICES, LogMessageFlags.ERROR, (ParamItem("service_name", "Name of service"), ParamItem("service_information", "Service  information")))
  
-    WHATSAPP_MESSAGE_RECEIVED: LogCommandDescription = LogCommandDescription(
-        "Получено сообщение", LogChannels.NOTIFICATION, LogLevels.SILENCE.value, (ParamItem("message", "Сообщение"),))
+    WHATSAPP_MESSAGE_RECEIVED: EventDescription = EventDescription(
+        "Получено сообщение", LogMessageChannels.POLIBASE_NOTIFICATIONS, LogMessageFlags.SILENCE, (ParamItem("message", "Сообщение"),))
     
-    NEW_FILE_DETECTED: LogCommandDescription = LogCommandDescription(
-        "Новый файл", LogChannels.IT, LogLevels.SILENCE.value, (ParamItem("path", "Путь к файлу"),))
+    NEW_FILE_DETECTED: EventDescription = EventDescription(
+        "Новый файл", LogMessageChannels.IT, LogMessageFlags.SILENCE, (ParamItem("path", "Путь к файлу"),))
     
-    NEW_POLIBASE_DOCUMENT_DETECTED: LogCommandDescription = LogCommandDescription(
-        "Новый Polibase документ", LogChannels.IT, LogLevels.NORMAL.value, (ParamItem("path", "Путь к файлу"), ParamItem("person_pin", "Идентификационный номер пациента"), ParamItem("document_name", "Имя документа")))
+    NEW_POLIBASE_DOCUMENT_DETECTED: EventDescription = EventDescription(
+        "Новый Polibase документ", LogMessageChannels.IT, LogMessageFlags.NORMAL, (ParamItem("path", "Путь к файлу"), ParamItem("person_pin", "Идентификационный номер пациента"), ParamItem("document_name", "Имя документа")))
 
-    COMPUTER_WAS_STARTED: LogCommandDescription = LogCommandDescription(
-        "Компьютер {name} загрузился", LogChannels.IT, LogLevels.NORMAL.value, (ParamItem("name", "Название компьютера"),))
+    COMPUTER_WAS_STARTED: EventDescription = EventDescription(
+        "Компьютер {name} загрузился", LogMessageChannels.IT, LogMessageFlags.NORMAL, (ParamItem("name", "Название компьютера"),))
     
-    SERVER_WAS_STARTED: LogCommandDescription = LogCommandDescription(
-        "Сервер {name} загрузился", LogChannels.IT, LogLevels.NORMAL.value, (ParamItem("name", "Название сервера"),))
+    SERVER_WAS_STARTED: EventDescription = EventDescription(
+        "Сервер {name} загрузился", LogMessageChannels.IT, LogMessageFlags.NORMAL, (ParamItem("name", "Название сервера"),))
     
-    RESOURCE_INACCESSABLE: LogCommandDescription = LogCommandDescription(
-        "Ресурс {resource_name} недоступен. {reason_string}", LogChannels.RESOURCES, LogLevels.ERROR.value, (ParamItem("resource_name", "Название ресурса"), ParamItem("resource", "Ресурс"), ParamItem("at_first_time", "Признак первого раза"), ParamItem("reason_string", "Строка причины"), ParamItem("reason", "Причины")))
+    RESOURCE_INACCESSABLE: EventDescription = EventDescription(
+        "Ресурс {resource_name} недоступен. {reason_string}", LogMessageChannels.RESOURCES, LogMessageFlags.ERROR, (ParamItem("resource_name", "Название ресурса"), ParamItem("resource", "Ресурс"), ParamItem("at_first_time", "Признак первого раза"), ParamItem("reason_string", "Строка причины"), ParamItem("reason", "Причины")))
     
-    RESOURCE_ACCESSABLE: LogCommandDescription = LogCommandDescription(
-        "Ресурс {resource_name} доступен", LogChannels.RESOURCES, LogLevels.NORMAL.value, (ParamItem("resource_name", "Название ресурса"), ParamItem("resource", "Ресурс"), ParamItem("at_first_time", "Признак первого раза")))
+    RESOURCE_ACCESSABLE: EventDescription = EventDescription(
+        "Ресурс {resource_name} доступен", LogMessageChannels.RESOURCES, LogMessageFlags.NORMAL, (ParamItem("resource_name", "Название ресурса"), ParamItem("resource", "Ресурс"), ParamItem("at_first_time", "Признак первого раза")))
 
     #
-    BACKUP_NOTIFY_ABOUT_ROBOCOPY_JOB_STARTED: LogCommandDescription = LogCommandDescription(
-        "Robocopy: Начато выполнение задания: {status}", LogChannels.BACKUP, LogLevels.NOTIFICATION.value, (ParamItem("status", ""),))
+    BACKUP_ROBOCOPY_JOB_WAS_STARTED: EventDescription = EventDescription(
+        "Robocopy: Начато выполнение задания: {name}. PID процесса: {pid}", LogMessageChannels.BACKUP, (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE), (PARAM_ITEMS.NAME, PARAM_ITEMS.PID))
 
-    BACKUP_NOTIFY_ABOUT_ROBOCOPY_JOB_COMPLETED: LogCommandDescription = LogCommandDescription(
-        "Robocopy: Завершено выполнение задания: {status}", LogChannels.BACKUP, LogLevels.NOTIFICATION.value, (ParamItem("status", ""),))
+    BACKUP_ROBOCOPY_JOB_WAS_COMPLETED: EventDescription = EventDescription(
+        "Robocopy: Завершено выполнение задания: {name}. Статус: {status_string}", LogMessageChannels.BACKUP, (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE), (PARAM_ITEMS.NAME, ParamItem("status_string", ""), PARAM_ITEMS.STATUS))
     #
-    POLIBASE_CREATION_DB_DUMP_START: LogCommandDescription = LogCommandDescription(
-        "Базы данных Polibase: Начато создание дампа",  LogChannels.BACKUP, LogLevels.NORMAL.value)
+    POLIBASE_CREATION_DB_DUMP_START: EventDescription = EventDescription(
+        "Базы данных Polibase: Начато создание дампа", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL)
     
-    POLIBASE_CREATION_DB_DUMP_COMPLETE: LogCommandDescription = LogCommandDescription(
-        "Базы данных Polibase: Завершено создание дампа",  LogChannels.BACKUP, LogLevels.NORMAL.value)
+    POLIBASE_CREATION_DB_DUMP_COMPLETE: EventDescription = EventDescription(
+        "Базы данных Polibase: Завершено создание дампа", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL)
     
-    POLIBASE_CREATION_ARCHIVED_DB_DUMP_START: LogCommandDescription = LogCommandDescription(
-        "Базы данных Polibase: Начато архивирование дампа",  LogChannels.BACKUP, LogLevels.NORMAL.value)
+    POLIBASE_CREATION_ARCHIVED_DB_DUMP_START: EventDescription = EventDescription(
+        "Базы данных Polibase: Начато архивирование дампа", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL)
 
-    POLIBASE_CREATION_ARCHIVED_DB_DUMP_COMPLETE: LogCommandDescription = LogCommandDescription(
-        "Базы данных Polibase: Завершено архивирование дампа",  LogChannels.BACKUP, LogLevels.NORMAL.value)
+    POLIBASE_CREATION_ARCHIVED_DB_DUMP_COMPLETE: EventDescription = EventDescription(
+        "Базы данных Polibase: Завершено архивирование дампа", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL)
     
-    POLIBASE_COPING_ARCHIVED_DB_DUMP_START: LogCommandDescription = LogCommandDescription(
-        "Базы данных Polibase: Начато копирование архивированного дампа на {destination}",  LogChannels.BACKUP, LogLevels.NORMAL.value, (ParamItem(
+    POLIBASE_COPING_ARCHIVED_DB_DUMP_START: EventDescription = EventDescription(
+        "Базы данных Polibase: Начато копирование архивированного дампа на {destination}", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL, (ParamItem(
             "destination", ""),))
 
-    POLIBASE_COPING_ARCHIVED_DB_DUMP_COMPLETE: LogCommandDescription = LogCommandDescription(
-        "Базы данных Polibase: Завершено копирование архивированного дампа на {destination}",  LogChannels.BACKUP, LogLevels.NORMAL.value, (ParamItem(
+    POLIBASE_COPING_ARCHIVED_DB_DUMP_COMPLETE: EventDescription = EventDescription(
+        "Базы данных Polibase: Завершено копирование архивированного дампа на {destination}", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL, (ParamItem(
             "destination", ""),))
     
-    POLIBASE_COPING_DB_DUMP_START: LogCommandDescription = LogCommandDescription(
-        "Базы данных Polibase: Начато копирование дампа на {destination}",  LogChannels.BACKUP, LogLevels.NORMAL.value, (ParamItem(
+    POLIBASE_COPING_DB_DUMP_START: EventDescription = EventDescription(
+        "Базы данных Polibase: Начато копирование дампа на {destination}", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL, (ParamItem(
             "destination", ""),))
-
-    POLIBASE_COPING_DB_DUMP_COMPLETE: LogCommandDescription = LogCommandDescription(
-        "Базы данных Polibase: Завершено копирование дампа на {destination}",  LogChannels.BACKUP, LogLevels.NORMAL.value, (ParamItem(
+    
+    POLIBASE_COPING_DB_DUMP_COMPLETE: EventDescription = EventDescription(
+        "Базы данных Polibase: Завершено копирование дампа на {destination}", LogMessageChannels.BACKUP, LogMessageFlags.NORMAL, (ParamItem(
             "destination", ""),))
     #
-    HR_NOTIFY_ABOUT_NEW_EMPLOYEE: LogCommandDescription = LogCommandDescription("День добрый, {hr_given_name}.\nДокументы для нового сотрудника: {employee_full_name} готовы!\nЕго корпоративная почта: {employee_email}.", LogChannels.HR, LogLevels.NOTIFICATION.value, (ParamItem(
+    HR_NOTIFY_ABOUT_NEW_EMPLOYEE: EventDescription = EventDescription("День добрый, {hr_given_name}.\nДокументы для нового сотрудника: {employee_full_name} готовы!\nЕго корпоративная почта: {employee_email}.", LogMessageChannels.HR, LogMessageFlags.NOTIFICATION.value, (ParamItem(
         "hr_given_name", "Имя руководителя отдела HR"), ParamItem("employee_full_name", "ФИО нового сотрудника"), ParamItem("employee_email", "Корпаротивная почта нового сотрудника")))
     #
-    IT_NOTIFY_ABOUT_CREATE_USER: LogCommandDescription = LogCommandDescription("Добрый день, отдел Информационных технологий.\nДокументы для нового пользователя: {name} готовы!\nОписание: {description}\nЛогин: {login}\nПароль: {password}\nТелефон: {telephone_number}\nЭлектронная почта: {email}", LogChannels.IT, LogLevels.NOTIFICATION.value, (ParamItem(
-        "name", ""), ParamItem("description", ""), ParamItem("login", ""), ParamItem("password", ""), ParamItem("telephone_number", ""),  ParamItem("email", "")))
+    IT_NOTIFY_ABOUT_CREATE_USER: EventDescription = EventDescription("Добрый день, отдел Информационных технологий.\nДокументы для нового пользователя: {name} готовы!\nОписание: {description}\nЛогин: {login}\nПароль: {password}\nТелефон: {telephone_number}\nЭлектронная почта: {email}", LogMessageChannels.IT, LogMessageFlags.NOTIFICATION.value, (PARAM_ITEMS.NAME, ParamItem("description", ""), ParamItem("login", ""), ParamItem("password", ""), ParamItem("telephone_number", ""), ParamItem("email", "")))
 
-    IT_NOTIFY_ABOUT_CREATE_NEW_MARK: LogCommandDescription = LogCommandDescription("Добрый день, отдел Информационных технологий.\nКарта доступа для новой персоны: {name} готова!\nТелефон: {telephone_number}\nНомер карты доступа: {tab_number}\nГруппа доступа: {group_name}", LogChannels.IT, LogLevels.NOTIFICATION.value, (ParamItem(
-        "name", ""), ParamItem("telephone_number", ""), ParamItem("tab_number", ""), ParamItem("group_name", "")))
+    IT_NOTIFY_ABOUT_CREATE_NEW_MARK: EventDescription = EventDescription("Добрый день, отдел Информационных технологий.\nКарта доступа для новой персоны: {name} готова!\nТелефон: {telephone_number}\nНомер карты доступа: {tab_number}\nГруппа доступа: {group_name}", LogMessageChannels.IT, LogMessageFlags.NOTIFICATION.value, (PARAM_ITEMS.NAME, ParamItem("telephone_number", ""), ParamItem("tab_number", ""), ParamItem("group_name", "")))
 
-    IT_NOTIFY_ABOUT_CREATE_TEMPORARY_MARK: LogCommandDescription = LogCommandDescription("Добрый день, отдел Информационных технологий.\nВременная карта доступа для персоны: {name} готова!\nНомер карты: {tab_number}\nТелефон: {telephone_number}", LogChannels.IT, LogLevels.NOTIFICATION.value, (ParamItem(
-        "name", ""), ParamItem("tab_number", ""), ParamItem("telephone_number", "")))
+    IT_NOTIFY_ABOUT_CREATE_TEMPORARY_MARK: EventDescription = EventDescription("Добрый день, отдел Информационных технологий.\nВременная карта доступа для персоны: {name} готова!\nНомер карты: {tab_number}\nТелефон: {telephone_number}", LogMessageChannels.IT, LogMessageFlags.NOTIFICATION.value, (PARAM_ITEMS.NAME, ParamItem("tab_number", ""), ParamItem("telephone_number", "")))
 
-    IT_NOTIFY_ABOUT_TEMPORARY_MARK_RETURN: LogCommandDescription = LogCommandDescription("Добрый день, отдел Информационных технологий.\nВременная карта доступа для персоны: {name} возвращена!\nНомер карты: {tab_number}", LogChannels.IT, LogLevels.NOTIFICATION.value, (ParamItem(
-        "name", ""), ParamItem("tab_number", "")))
+    IT_NOTIFY_ABOUT_TEMPORARY_MARK_RETURN: EventDescription = EventDescription("Добрый день, отдел Информационных технологий.\nВременная карта доступа для персоны: {name} возвращена!\nНомер карты: {tab_number}", LogMessageChannels.IT, LogMessageFlags.NOTIFICATION.value, (PARAM_ITEMS.NAME, ParamItem("tab_number", "")))
 
-    IT_NOTIFY_ABOUT_MARK_RETURN: LogCommandDescription = LogCommandDescription("Добрый день, отдел Информационных технологий.\nКарта доступа для персоны: {name} возвращена!\nНомер карты: {tab_number}", LogChannels.IT, LogLevels.NOTIFICATION.value, (ParamItem(
-        "name", ""), ParamItem("tab_number", "")))
+    IT_NOTIFY_ABOUT_MARK_RETURN: EventDescription = EventDescription("Добрый день, отдел Информационных технологий.\nКарта доступа для персоны: {name} возвращена!\nНомер карты: {tab_number}", LogMessageChannels.IT, LogMessageFlags.NOTIFICATION.value, (PARAM_ITEMS.NAME, ParamItem("tab_number", "")))
 
-    IT_TASK_AFTER_CREATE_NEW_USER: LogCommandDescription = LogCommandDescription("Добрый день, {it_user_name}.\nНеобходимо создать почту для пользователя: {name}\nАдресс электронной почты: {mail}\nПароль: {password}", LogChannels.IT, LogLevels.TASK.value, (ParamItem(
-        "it_user_name", ""), ParamItem("name", ""), ParamItem("mail", ""), ParamItem("password", "")))
+    IT_TASK_AFTER_CREATE_NEW_USER: EventDescription = EventDescription("Добрый день, {it_user_name}.\nНеобходимо создать почту для пользователя: {name}\nАдресс электронной почты: {mail}\nПароль: {password}", LogMessageChannels.IT, LogMessageFlags.TASK.value, (ParamItem(
+        "it_user_name", ""), PARAM_ITEMS.NAME, ParamItem("mail", ""), ParamItem("password", "")))
 
-    WATCHABLE_WORKSTATION_IS_NOT_ACCESSABLE: LogCommandDescription = LogCommandDescription(
-        "Компьютер {workstation_name} вне сети", LogChannels.RESOURCES, LogLevels.ERROR.value, [ParamItem("workstation_name", "")])
+    WATCHABLE_WORKSTATION_IS_NOT_ACCESSABLE: EventDescription = EventDescription(
+        "Компьютер {workstation_name} вне сети", LogMessageChannels.RESOURCES, LogMessageFlags.ERROR, [ParamItem("workstation_name", "")])
     
-    WATCHABLE_WORKSTATION_IS_ACCESSABLE: LogCommandDescription = LogCommandDescription(
-        "Компьютер {workstation_name} в сети", LogChannels.RESOURCES, LogLevels.NORMAL.value, [ParamItem("workstation_name", "")])
+    WATCHABLE_WORKSTATION_IS_ACCESSABLE: EventDescription = EventDescription(
+        "Компьютер {workstation_name} в сети", LogMessageChannels.RESOURCES, LogMessageFlags.NORMAL, [ParamItem("workstation_name", "")])
+    
+    #MRI
+     
+    MRI_CHILLER_FILTER_WAS_CHANGED: EventDescription = EventDescription(
+        "Фильтр водяного охлаждения был заменён", LogMessageChannels.RESOURCES, (LogMessageFlags.NOTIFICATION, LogMessageFlags.SAVE))
+    
+    MRI_CHILLER_TEMPERATURE_ALERT_WAS_FIRED: EventDescription = EventDescription(
+        "Превышена температура чиллера", LogMessageChannels.RESOURCES, (LogMessageFlags.ERROR, LogMessageFlags.SAVE), (ParamItem(FIELD_NAME_COLLECTION.DATE, ""), ))
+    
+    MRI_CHILLER_WAS_TURNED_OFF: EventDescription = EventDescription(
+        "чиллера", LogMessageChannels.RESOURCES, (LogMessageFlags.ERROR, LogMessageFlags.SAVE), (ParamItem(FIELD_NAME_COLLECTION.DATE, ""), ))
 
     #POLIBASE
 
-    POLIBASE_PERSON_VISIT_WAS_REGISTERED: LogCommandDescription = LogCommandDescription("Зарегистрировано новое посещение: {name} ({type_string})", LogChannels.NOTIFICATION, LogLevels.NOTIFICATION.value, (ParamItem(
-        "name", ""), ParamItem("type_string", ""), ParamItem("visit", "")))
+    POLIBASE_PERSON_DUPLICATION_WAS_DETECTED: EventDescription("Регистратор {registrator_person_name} создал персону {person_name} ({person_pin}), которая дублирует {duplicated_person_name} ({duplicated_person_pin})", LogMessageChannels.POLIBASE_ERROR_NOTIFICATIONS, LogMessageFlags.SAVE, (ParamItem(
+        "person_name", ""), ParamItem("person_pin", ""), ParamItem("duplicated_person_name", ""), ParamItem("duplicated_person_pin", ""),  ParamItem("registrator_person_name", "")))
+
+    POLIBASE_PERSON_VISIT_WAS_REGISTERED: EventDescription = EventDescription("Зарегистрировано новое посещение: {name} ({type_string})", LogMessageChannels.POLIBASE_NOTIFICATIONS, LogMessageFlags.NOTIFICATION, (PARAM_ITEMS.NAME, ParamItem("type_string", ""), ParamItem("visit", "")))
+    
+    POLIBASE_PERSON_WAS_CREATED: EventDescription = EventDescription("Создана полибейс персона: {name} ({pin})", LogMessageChannels.POLIBASE_NOTIFICATIONS, LogMessageFlags.NOTIFICATION, (PARAM_ITEMS.NAME, ParamItem("pin", ""), ParamItem("value", "")))
+    
+    POLIBASE_PERSON_WAS_UPDATED: EventDescription = EventDescription("Обновлена полибейс персона: {name} ({pin})", LogMessageChannels.POLIBASE_NOTIFICATIONS, LogMessageFlags.SILENCE, (PARAM_ITEMS.NAME, ParamItem("pin", ""), ParamItem("value", "")))
 
-    POLIBASE_PERSON_VISIT_NOTIFICATION_WAS_REGISTERED: LogCommandDescription = LogCommandDescription("Зарегистрировано новое уведомление посещение: {name} ({type_string})", LogChannels.NOTIFICATION, LogLevels.SILENCE.value, (ParamItem(
-        "name", ""), ParamItem("type_string", ""), ParamItem("notification", "")))
+    POLIBASE_PERSON_VISIT_NOTIFICATION_WAS_REGISTERED: EventDescription = EventDescription("Зарегистрировано новое уведомление посещение: {name} ({type_string})", LogMessageChannels.POLIBASE_NOTIFICATIONS, LogMessageFlags.SILENCE, (PARAM_ITEMS.NAME, ParamItem("type_string", ""), ParamItem("notification", "")))
 
-    POLIBASE_PERSONS_WITH_OLD_FORMAT_BARCODE_WAS_DETECTED: LogCommandDescription = LogCommandDescription(
-        "Полибейс: обнаружены пациенты со старым форматом или отсутствующим штрих-кодом в количестве {persons_pin_length}", LogChannels.NOTIFICATION, LogLevels.SILENCE.value, (ParamItem("persons_pin_length", ""), ParamItem("persons_pin", "")))
+    POLIBASE_PERSONS_WITH_OLD_FORMAT_BARCODE_WAS_DETECTED: EventDescription = EventDescription(
+        "Полибейс: обнаружены пациенты со старым форматом или отсутствующим штрих-кодом", LogMessageChannels.POLIBASE_NOTIFICATIONS, LogMessageFlags.SILENCE, (ParamItem("persons_pin", ""), ))
+    
+    POLIBASE_PERSON_BARCODES_WITH_OLD_FORMAT_WERE_CREATED: EventDescription = EventDescription(
+        "Полибейс: все новые штрих-коды созданы", LogMessageChannels.POLIBASE_NOTIFICATIONS, LogMessageFlags.SILENCE, [ParamItem("persons_pin", "")])
     
-    POLIBASE_ALL_PERSON_BARCODES_WITH_OLD_FORMAT_WAS_CREATED: LogCommandDescription = LogCommandDescription(
-        "Полибейс: все новые штрих-коды созданы", LogChannels.NOTIFICATION, LogLevels.SILENCE.value, [ParamItem("persons_pin", "")])
+    POLIBASE_PERSON_WITH_INACCESSABLE_EMAIL_WAS_DETECTED: EventDescription = EventDescription(
+        "Пациент {} ({}) имеет недоступную электронную почту: {}. Регистратор: {}, компьютер: {} ({})", LogMessageChannels.POLIBASE_ERROR_NOTIFICATIONS, LogMessageFlags.SAVE, [ParamItem(FIELD_NAME_COLLECTION.PERSON_NAME, ""), ParamItem(FIELD_NAME_COLLECTION.PERSON_PIN, ""), ParamItem(FIELD_NAME_COLLECTION.EMAIL, ""), ParamItem(FIELD_NAME_COLLECTION.REGISTRATOR_PERSON_NAME, ""), ParamItem(FIELD_NAME_COLLECTION.WORKSTATION_NAME, ""), ParamItem(FIELD_NAME_COLLECTION.WORKSTATION_DESCRIPTION, "")])
 
-    POLIBASE_PERSON_WANTS_FEEDBACK_CALL_AFTER_REVIEW_QUEST_COMPLETE: LogCommandDescription = LogCommandDescription("Клиент {name} ({pin}) запросил обратный звонок.\nОценка: {grade}\nПричина: {message}\nТелефон: {telephone_number}",  LogChannels.POLIBASE_PERSON_FEEDBACK_CALL, LogLevels.NOTIFICATION.value, (ParamItem(
-        "name", ""), ParamItem("pin", ""), ParamItem("grade", ""), ParamItem("message", ""), ParamItem("telephone_number", "")))
+    POLIBASE_PERSON_EMAIL_WAS_ADDED: EventDescription = EventDescription(
+        "Электронная почта пациента {} ({}): {} была добавлена", LogMessageChannels.POLIBASE_NOTIFICATIONS, (LogMessageFlags.RESULT, LogMessageFlags.SAVE), [ParamItem(FIELD_NAME_COLLECTION.PERSON_NAME, ""), ParamItem(FIELD_NAME_COLLECTION.PERSON_PIN, ""), ParamItem(FIELD_NAME_COLLECTION.EMAIL, "")])
+    
+    ACTION_WAS_DONE: EventDescription = EventDescription(
+        "Совершено действие {} ({}).\nДействие совершил: {} ({})", LogMessageChannels.DEBUG, LogMessageFlags.SAVE, [ParamItem(FIELD_NAME_COLLECTION.ACTION_DESCRIPTION, ""), ParamItem(FIELD_NAME_COLLECTION.ACTION_NAME, ""), ParamItem(FIELD_NAME_COLLECTION.NAME, ""), ParamItem(FIELD_NAME_COLLECTION.LOGIN, "")])
+    
+    ACTION_HAVE_TO_BE_DONE: EventDescription = EventDescription(
+        "Необходимо совершить действие {}: {}", LogMessageChannels.DEBUG, LogMessageFlags.SAVE, [ParamItem(FIELD_NAME_COLLECTION.ACTION_NAME, ""), ParamItem(FIELD_NAME_COLLECTION.ACTION_DESCRIPTION, "")])
+    
 
-    POLIBASE_PERSON_REVIEW_QUEST_RESULT_FOR_HIGH_GRADE: LogCommandDescription = LogCommandDescription("Клиент {name} ({pin}) завершил опрос.\nОценка: {grade}\nОткуда узнал о нас: {information_way}\nТелефон: {telephone_number}",  LogChannels.POLIBASE_PERSON_REVIEW_QUEST_RESULT, LogLevels.NOTIFICATION.value, (ParamItem(
-        "name", ""), ParamItem("pin", ""), ParamItem("grade", ""), ParamItem("information_way", ""), ParamItem("telephone_number", "")))
+class Actions(Enum):
 
-    POLIBASE_PERSON_REVIEW_QUEST_RESULT_FOR_LOW_GRADE: LogCommandDescription = LogCommandDescription("Клиент {name} ({pin}) завершил опрос.\nОценка: {grade}\nПричина: {message}\nОткуда узнал о нас: {information_way}\nЗапросил обратный звонок: {feedback_call}\nТелефон: {telephone_number}",  LogChannels.POLIBASE_PERSON_REVIEW_QUEST_RESULT, LogLevels.NOTIFICATION.value, (ParamItem(
-        "name", ""), ParamItem("pin", ""), ParamItem("grade", ""), ParamItem("message", ""), ParamItem("information_way", ""), ParamItem("feedback_call", ""), ParamItem("telephone_number", "")))
+    CHILLER_FILTER_CHANGING: ActionDescription = ActionDescription(
+        "CHILLER_FILTER_CHANGING", "filter", "Замена фильтра очистки воды", "Заменить фильтр очистки воды")
```

### Comparing `pih-1.43/pih/pih.py` & `pih-1.45/pih/pih.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import calendar
 from collections import defaultdict
+from concurrent import futures
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta
 from getpass import getpass
 from threading import Thread
 from time import sleep
 from grpc import StatusCode
 import dataclasses
@@ -13,85 +14,81 @@
 import platform
 import json
 import pkg_resources
 import re
 import subprocess
 from subprocess import DEVNULL, STDOUT, CompletedProcess
 import sys
-from typing import Any, Callable, Tuple
+from typing import Any, Callable
 import colorama
 from colorama import Back, Style, Fore
 from prettytable import PrettyTable
 import requests
 from requests import ConnectTimeout, Response
 import traceback
 from contextlib import contextmanager
 import base64
 import uuid
-
-try:
-    from packaging.version import parse
-except ImportError:
-    from pip._vendor.packaging.version import parse
+import time
+from enum import Enum
+from string import Formatter
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
-from pih.tools import DataTool, EnumTool, PathTool, ResultTool, FullNameTool, PasswordTools, ResultUnpack, DateTimeTool, BitMask as BM, ParameterList, StringTool, ListTool, NetworkTool
-from pih.collection import ActionValue, T, FieldItem, FieldItemList, FullName, InventoryReportItem, LogCommandDescription, LoginPasswordPair, Mark, MarkDivision, MarkGroup, MarkGroupStatistics, ParamItem, PasswordSettings, PolibasePerson, PrinterADInformation, PrinterReport, PrinterStatus, Result, ServiceRoleInformation, ServiceRoleDescription, TemporaryMark, TimeTrackingEntity, TimeTrackingResultByDate, TimeTrackingResultByDivision, TimeTrackingResultByPerson, User, UserContainer, Workstation, WhatsAppMessage, WhatsAppMessageListPayload, WhatsAppMessageButtonsPayload, WorkstationDescription, SettingsValue, PolibasePersonVisitDS, PolibasePersonVisitNotification, PolibasePersonVisitNotificationDS, DelayedMessage, MessageSearchCritery, DelayedMessageDS, PolibasePersonInformationQuest, PolibasePersonVisitSearchCritery, RobocopyJobStatus, PolibasePersonNotificationConfirmation, ResourceDescription, ResourceStatus, SiteResourceStatus, CTIndicationItem, CTIndicationValue, PolibaseScannedDocument, OGRN, Message
-from pih.const import CONST, URLS, DATA, FIELD_NAME_COLLECTION, FIELD_COLLECTION, FILE, FIELD_COLLECTION_ALIAS, PASSWORD, PATHS, HOSTS, USER_PROPERTY, WorkstationMessageMethodTypes, LogChannels, LogCommands, LogLevels, MarkType, ServiceCommands, ServiceRoles, SETTINGS, MessageTypes, MessageStatuses, RESOURCE, CheckableSections, AD, MEDICAl_DOCUMENT, FONT
-from pih.rpc_collection import Subscriber
-from pih.rpc import RPC, Error, SubscribtionTypes
+
+from pih.collection import  *
+from pih.tools import *
+from pih.const import *
+from pih.rpc_collection import *
+from pih.rpc import *
+from pih.rpc_const import *
 
 class IClosable:
 
-    def close() -> None:
+    def close(self) -> None:
         raise NotImplemented()
 
 class ServiceListener:
     
     def __init__(self):
-        self.service: RPC.Service | None = None
+        self.service: IService | None = None
         self.service_command_list: list[ServiceCommands] = None
         self.host: str = A.OS.host()
         self.port: int = NetworkTool.next_free_port()
 
-    def listen_for(self, service_command_list: list[ServiceCommands], handler: Callable[[str, ParameterList, IClosable], Any]) -> None:     
+    def listen_for(self, service_command_list: list[ServiceCommands], handler: Callable[[ServiceCommands, ParameterList, IClosable], Any]) -> None:     
         self.service_command_list = service_command_list
   
-        def service_started_handler(service: RPC.Service) -> None:
+        def service_starts_handler(service: IService) -> None:
             self.service = service
             for service_command in service_command_list:
                 service.subscribe_on(service_command)
 
-        service_description: ServiceRoleDescription = ServiceRoleDescription(
-            name=f"Subscriber_{self.host}_{ self.port}",
-            description="Subscriber",
-            host=self.host,
-            port=self.port,
-            weak_subscribtion=True)
-        
-        PIH.SERVICE.ADMIN.serve(service_description, lambda command_name, parameter_list, _: handler(command_name, parameter_list, self), False, service_started_handler)
+        PIH.SERVICE.ADMIN.serve(PIH.SERVICE.ADMIN.create_event_listener_service_description(self.host, self.port), 
+                                lambda command_name, parameter_list: handler(command_name, parameter_list, self), 
+                                service_starts_handler, 
+                                show_output = True)
         
     def close(self) -> None:
         self.service.unsubscribe(self.service_command_list)
-        self.service.stop()    
-
+        PIH.SERVICE.ADMIN.stop(self.service.get_description(), False)
+       
 
 class MarkOutputAbstract:
 
     def by_any(self, value: str) -> None:
         raise NotImplemented()
 
     def result(self, result: Result[list[Mark]], caption: str, use_index: bool = False) -> None:
         raise NotImplemented()
 
 class OutputAbstract:
     
-    def indent(self, count: int = 1) -> None:
+    def set_indent(self, count: int = 1) -> None:
         raise NotImplemented()
     
     def bold(self, value: str) -> str:
         raise NotImplemented()
 
     def header(self, caption: str) -> None:
         raise NotImplemented()
@@ -227,15 +224,15 @@
 
     def bright_str(self, text: str, text_before: str = None, text_after: str = None) -> str:
         raise NotImplemented()
 
     def get_number(self, value: int) -> str:
         raise NotImplemented()
 
-    def write_result(self, result: Result[T], use_index: bool = True, item_separator: str = "\n", empty_result_text: str = "Не найдено", separated_result_item: bool = True, label_function:  Callable[[Any, int], str] = None, data_label_function: Callable[[int, FieldItem, Result[T], Any], Tuple[bool, str]] = None, title: str = None) -> None:
+    def write_result(self, result: Result[T], use_index: bool = True, item_separator: str = "\n", empty_result_text: str = "Не найдено", separated_result_item: bool = True, label_function:  Callable[[Any, int], str] = None, data_label_function: Callable[[int, FieldItem, Result[T], Any], tuple[bool, str]] = None, title: str = None) -> None:
         raise NotImplemented()
 
     @contextmanager
     def send_to_group(self, group: CONST.MESSAGE.WHATSAPP.GROUP) -> bool:
         raise NotImplemented()
 
 class MarkOutputBase(MarkOutputAbstract):
@@ -265,69 +262,69 @@
 
     def get_formatted_given_name(self, value: str | None = None) -> str:
         return value
 
 class OutputExtendedAbstract:
 
     def pih_title(self) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def rpc_service_header(self, host: str, port: int, description: str) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
-    def service_header(self, service_role_description: ServiceRoleDescription) -> None:
-        raise NotImplemented()  
+    def service_header(self, description: ServiceDescription) -> None:
+        raise NotImplemented()
 
     def free_marks(self, show_guest_marks: bool, use_index: bool = False) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def guest_marks(self, use_index: bool = False) -> None:
         raise NotImplemented()
 
     def temporary_candidate_for_mark(self, mark: Mark) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
-    def free_marks_group_statistics(self, use_index: bool = False, show_guest_marks: bool = None) -> None:
-        raise NotImplemented()  
+    def free_marks_group_statistics(self, use_index: bool = False, show_guest_marks: bool | None = None) -> None:
+        raise NotImplemented()
 
     def free_marks_by_group(self, group: dict, use_index: bool = False) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def free_marks_group_statistics_for_result(self, result: Result, use_index: bool) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def free_marks_by_group_for_result(self, group: MarkGroup, result: Result, use_index: bool) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def temporary_marks(self, use_index: bool = False,) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def containers_for_result(self, result: Result, use_index: bool = False) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def table_with_caption_first_title_is_centered(self, result: Result, caption: str, use_index: bool = False, label_function: Callable = None) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def table_with_caption_last_title_is_centered(self, result: Result, caption: str, use_index: bool = False, label_function: Callable = None) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def table_with_caption(self, result: Any, caption: str = None, use_index: bool = False, modify_table_function: Callable = None, label_function: Callable = None) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def template_users_for_result(self, data: dict, use_index: bool = False) -> None:
-        raise NotImplemented()  
+        raise NotImplemented()
 
     def clear_screen(self) -> None:
         raise NotImplemented()
     
     def write_video(self, caption: str, video_content: str) -> None:
             raise NotImplemented()
 
     def write_image(self, caption: str, image_content: str) -> None:
-        raise NotImplemented()
+        pass
 
 class UserOutputBase(UserOutputAbstract):
 
     def __init__(self):
         self.parent: OutputBase
 
 class UserOutput(UserOutputBase):
@@ -342,22 +339,22 @@
         base_location = AD.LOCATION_JOINER.join([".".join(
             root_base_location), AD.LOCATION_JOINER.join(base_location_list[2:])])
         location_field = fields.get_item_by_name(
             FIELD_NAME_COLLECTION.DN)
         pevious_caption: str = location_field.caption
         location_field.caption = f"{location_field.caption} ({base_location})"
         def modify_data(field: FieldItem, user: User) -> str:
-            if field.name == USER_PROPERTY.DN:
+            if field.name == USER_PROPERTIES.DN:
                 return AD.LOCATION_JOINER.join(filter(
                     lambda x: x not in base_location_list, PIH.DATA.FORMAT.location_list(user.distinguishedName)))
-            if field.name == USER_PROPERTY.USER_ACCOUNT_CONTROL:
+            if field.name == USER_PROPERTIES.USER_ACCOUNT_CONTROL:
                 return "\n".join(PIH.DATA.FORMAT.get_user_account_control_values(user.userAccountControl))
-            if field.name == USER_PROPERTY.DESCRIPTION:
+            if field.name == USER_PROPERTIES.DESCRIPTION:
                 return user.description
-            if field.name == USER_PROPERTY.NAME:
+            if field.name == USER_PROPERTIES.NAME:
                 return "\n".join(user.name.split(" "))
             return None
         self.parent.table_with_caption(
             result, "Пользватели:" if len(data) > 1 else "Пользватель:", False, None, modify_data)
         location_field.caption = pevious_caption
 
 
@@ -419,27 +416,27 @@
 
     def polibase_person_any(self, title: str | None = None) -> str:
         raise NotImplemented()
 
 
 class UserInputAbstract:
 
-    def container(self) -> UserContainer:
+    def container(self) -> UserBase:
         raise NotImplemented()
 
     def by_name(self) -> User:
         raise NotImplemented()
 
     def title_any(self, title: str = None) -> str:
         raise NotImplemented()
 
-    def by_any(self, value: str = None, active: bool = None, title: str = None, use_all: bool = False) -> list[User]:
+    def by_any(self, value: str = None, active: bool | None = None, title: str = None, use_all: bool = False) -> list[User]:
         raise NotImplemented()
 
-    def telephone_number(self, value: str = None, active: bool = None, title: str = None) -> User:
+    def telephone_number(self, value: str = None, active: bool | None = None, title: str = None) -> User:
         raise NotImplemented()
 
     def template(self) -> dict:
         raise NotImplemented()
 
     def search_attribute(self) -> str:
         raise NotImplemented()
@@ -491,18 +488,18 @@
         self.mark: MarkInputBase
         self.user: UserInputBase
 
 
 class OutputBase(OutputAbstract, OutputExtendedAbstract):
 
     def __init__(self, user_output: UserOutputBase = None, mark_output: MarkOutputBase = None):
-        self.TEXT_BEFORE: str = ""
-        self.TEXT_AFTER: str = ""
-        self.INDEX: str = "  "
-        self.INDEX_COUNT: int = 0
+        self.text_before: str = ""
+        self.text_after: str = ""
+        self.indent_symbol: str = " "
+        self.indent_value: int = 0
         self.user: UserOutputBase = user_output
         self.user.parent = self
         self.mark: MarkOutputBase = mark_output
         self.mark.parent = self
         self.personalize = False
 
 
@@ -598,30 +595,30 @@
     def user_given_name(self) -> str:
         return FullNameTool.to_given_name(self.get_user().name)
 
     def start(self, login: str, notify: bool = True) -> None:
         if self.login is None:
             self.login = login
             if notify:
-                PIH.LOG.COMMAND.start_session()
+                PIH.EVENT.start_session()
 
     def say_hello(self) -> None:
         user: User = self.get_user()
         if user is not None:
             self.output.good(f"Добро пожаловать, {user.name}")
             self.output.new_line()
             return
         self.output.error(f"Ты кто такой? Давай, до свидания...")
         self.exit()
 
     @property
     def argv(self) -> list[str]:
         return sys.argv[1:] if len(sys.argv) > 1 else None
     
-    def arg(self, index: int = 0, default_value: Any = None) -> str:
+    def arg(self, index: int = 0, default_value: Any | None = None) -> str:
         return DataTool.by_index(self.argv, index, default_value)
 
     def get_file_path(self) -> str:
         return sys.argv[0]
 
     @property
     def file_name(self) -> str:
@@ -637,18 +634,18 @@
             if PIH.SERVICE.check_accessibility(ServiceRoles.AD): 
                 login: str = PIH.OS.get_login()
                 self.output.head1(f"{FullNameTool.to_given_name(A.R_U.by_login(login, cached=False).data.name)}, пожалуйста, пройдите аутентификацию...")
                 self.output.new_line()
                 if not self.input.yes_no(f"Использовать логин '{login}'", True):
                     login = PIH.input.login()
                 password: str = PIH.input.password(is_new=False)
-                if DataTool.rpc_unrepresent(RPC.call(ServiceCommands.authenticate, (login, password))):
+                if DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.authenticate, (login, password))):
                     self.authenticated = True
                     self.start(login, False)
-                    PIH.LOG.COMMAND.login()
+                    PIH.EVENT.login()
                     self.output.good(self.output.text_black(
                         f"Добро пожаловать, {self.get_user().name}..."))
                     return True
                 else:
                     if exit_on_fail:
                         self.exit(
                             5, "Неверный пароль или логин. До свидания...")
@@ -676,51 +673,64 @@
         self.interrupt_type = False
         self.wait_for_data_input = False
         self.data = None
 
 
 class Output(OutputBase):
 
-    def indent(self, count: int = 1) -> None:
-        self.INDEX_COUNT = count
-        self.TEXT_BEFORE = self.INDEX*count
+    @contextmanager
+    def make_indent(self, value: int, additional: bool = False) -> bool:
+        try:
+            self.set_indent([0, self.indent][additional] + value)
+            yield True
+        finally:
+            self.set_indent([0, self.indent - value][additional])
+
+    def set_indent(self, value: int) -> None:
+        self.indent_value = value
+        self.text_before = self.indent_symbol * value
 
     def bold(self, value: str) -> str:
-        return self.text_color(Fore.RED, value)
+        return f"\033[1m{value}\033[0m"
 
     def italic(self, value: str) -> str:
         return value
 
     def reset_indent(self) -> None:
-        self.TEXT_BEFORE = ""
+        self.indent_value = 0
+        self.text_before = ""
+
+    @property
+    def indent(self) -> int:
+        return self.indent_value
 
     def restore_indent(self) -> None:
-        self.indent(self.INDEX_COUNT)
+        self.set_indent(self.indent_value)
 
     def init(self) -> None:
         colorama.init()
 
     def text_color(self, color: int, text: str) -> str:
         return f"{color}{text}{Fore.RESET}"
 
     def text_black(self, text: str) -> str:
         return self.text_color(Fore.BLACK, text)
 
     def color_str(self, color: int, text: str, text_before: str = None, text_after: str = None) -> str:
         text = f" {text} "
-        text_before = text_before if text_before is not None else self.TEXT_BEFORE
-        text_after = text_after if text_after is not None else self.TEXT_AFTER
+        text_before = text_before if text_before is not None else self.text_before
+        text_after = text_after if text_after is not None else self.text_after
         return f"{text_before}{color}{text}{Back.RESET}{text_after}"
 
     def color(self, color: int, text: str, text_before: str = None, text_after: str = None) -> None:
         self.write_line(self.color_str(
             color, text, text_before, text_after))
 
     def write_line(self, text: str) -> None:
-        print(text)
+        print("\n".join(list(map(lambda item: self.text_before + item, text.splitlines()))))
 
     @contextmanager
     def personalized(self) -> bool:
         pass
 
     def index(self, index: int, text: str, max_index: int = None) -> None:
         indent: str = ""
@@ -729,21 +739,21 @@
         if index is None:
             self.write_line(f"{indent}{text}")
         else:
             self.write_line(f"{index}. {indent}{text}")
 
     def input(self, caption: str) -> None:
         self.write_line(self.input_str(
-            caption, self.TEXT_BEFORE, text_after=":"))
+            caption, self.text_before, text_after=":"))
 
     def input_str(self, caption: str, text_before: str = None, text_after: str = None) -> str:
         return self.white_str(f"{Fore.BLACK}{caption}{Fore.RESET}", text_before, text_after)
 
     def value(self, caption: str, value: str, text_before: str = None) -> None:
-        text_before = text_before or self.TEXT_BEFORE
+        text_before = text_before or self.text_before
         self.cyan(caption, text_before, f": {value}")
 
     def get_action_value(self, caption: str, value: str, show: bool = True) -> ActionValue:
         if show:
             self.value(caption, value)
         return ActionValue(caption, value)
 
@@ -786,16 +796,16 @@
     def green(self, text: str, text_before: str = None, text_after: str = None) -> None:
         self.write_line(self.green_str(text, text_before, text_after))
 
     def yellow_str(self, text: str, text_before: str = None, text_after: str = None) -> str:
         return self.color_str(Back.YELLOW, text, text_before, text_after)
 
     def yellow(self, text: str, text_before: str = None, text_after: str = None) -> None:
-        text_before = text_before or self.TEXT_BEFORE
-        text_after = text_after or self.TEXT_AFTER
+        text_before = text_before or self.text_before
+        text_after = text_after or self.text_after
         self.write_line(self.yellow_str(text, text_before, text_after))
 
     def black_str(self, text: str, text_before: str = None, text_after: str = None) -> str:
         return self.color_str(Back.BLACK, text, text_before, text_after)
 
     def black(self, text: str, text_before: str = None, text_after: str = None) -> None:
         self.write_line(self.black_str(text, text_before, text_after))
@@ -848,38 +858,38 @@
 
     def get_number(self, value: int) -> str:
         return CONST.VISUAL.NUMBER_SYMBOLS[value - 1]
 
     def header(self, caption: str) -> None:
         self.head2(caption)
 
-    def write_result(self, result: Result[T], use_index: bool = True, item_separator: str = "\n", empty_result_text: str = "Не найдено", separated_result_item: bool = True, label_function: Callable[[Any, int], str] = None, data_label_function: Callable[[int, FieldItem, Result, Any], Tuple[bool, str]] = None, title: str = None) -> None:
+    def write_result(self, result: Result[T], use_index: bool = True, item_separator: str = "\n", empty_result_text: str = "Не найдено", separated_result_item: bool = True, label_function: Callable[[Any, int], str] = None, data_label_function: Callable[[int, FieldItem, Result, Any], tuple[bool, str]] = None, title: str = None) -> None:
         data: list = DataTool.as_list(result.data)
         result_string_list: list[str] = None
         if DataTool.is_empty(data):
             self.new_line()
             self.write_line(empty_result_text)
         else:
             if not DataTool.is_empty(title):
                 self.write_line(title)
             for index, data_item in enumerate(data):
                 result_string_list = []
                 if use_index and len(data) > 1:
-                    result_string_list.append(f"{str(index + 1)}:")
+                    result_string_list.append(f"{self.text_before}{str(index + 1)}:")
                 if label_function is None:
                     for field_item in result.fields.list:
                         field: FieldItem = field_item
                         if not field.visible:
                             continue
                         item_data_value: str = None
                         if isinstance(data_item, dict):
                             item_data_value = data_item[field.name]
                         elif dataclasses.is_dataclass(data_item):
                             item_data_value = data_item.__getattribute__(field.name)
-                        item_data_value = item_data_value if DataTool.is_empty(item_data_value) else PIH.DATA.FORMAT.by_name(field.data_formatter, item_data_value) or field.data_formatter.format(data=item_data_value) 
+                        item_data_value = item_data_value if DataTool.is_empty(item_data_value) else PIH.DATA.FORMAT.by_formatter_name(field.data_formatter, item_data_value) or field.data_formatter.format(data=item_data_value) 
                         if DataTool.is_empty(item_data_value):
                             if data_label_function is None:
                                 continue
                         default_value_label_function: Callable[[int, FieldItem, Result[T], Any], (
                             bool, str)] = lambda _1, field, _2, data_value: (True, f"{self.bold(field.caption)}: {data_value}")
                         result_data_label_function: Callable[[int, FieldItem, Result[T], Any], (bool, str)] = data_label_function or default_value_label_function 
                         label_value_result: tuple[bool, str] = result_data_label_function(index, field, data_item, item_data_value)
@@ -889,15 +899,15 @@
                             if label_value is None and field.default_value is not None:
                                 label_value = field_item.default_value
                         else:
                             label_value = default_value_label_function(index, field, data_item, item_data_value)[1]
                         if not DataTool.is_empty(label_value):
                             result_string_list.append(label_value)
                 else:
-                    result_string_list.append(label_function(data_item, index))  
+                    result_string_list.append(label_function(data_item, index))
                 if separated_result_item:
                     self.separated_line()
                 self.write_line(item_separator.join(result_string_list))
 
     def clear_screen(self):
         os.system('cls' if os.name == 'nt' else 'clear')
 
@@ -908,31 +918,29 @@
         self.cyan(self.text_color(Fore.WHITE, "█┼┼ ▄█▄ █┼█") +
                          self.text_color(Fore.BLACK, f" {PIH.VERSION.local()}"))
         self.new_line()
 
     def rpc_service_header(self, host: str, port: int, description: str) -> None:
         self.blue("PIH service")
         self.blue(f"Version: {PIH.VERSION.local()}")
-        self.blue(f"PyPi Version: {PIH.VERSION.remote()}")
+        #self.blue(f"PyPi Version: {PIH.VERSION.remote()}")
         self.green(f"Service host: {host}")
         self.green(f"Service port: {port}")
         self.green(f"Service name: {description}")
 
-    def service_header(self, service_role_description: ServiceRoleDescription) -> None:
-        if service_role_description.isolated:
+    def service_header(self, information: ServiceInformation) -> None:
+        if information.isolated:
             self.blue(f"[Isolate]")
         self.blue("Запуск сервиса")
-        self.blue(f"PIH версия: {PIH.VERSION.remote()}")
-        self.green(f"Хост: {service_role_description.host}")
-        self.green(f"Порт: {service_role_description.port}")
-        self.green(f"Имя сервиса: {service_role_description.name}")
-        self.green(
-            f"Описание сервиса: {service_role_description.description}")
+        #self.blue(f"PIH версия: {PIH.VERSION.remote()}")
+        self.green(f"Хост: {information.host}")
+        self.green(f"Порт: {information.port}")
+        self.green(f"Имя сервиса: {information.name}")
         self.green(
-            f"Идентификатор процесса: {service_role_description.pid}")
+            f"Идентификатор процесса: {information.pid}")
 
     def free_marks(self, show_guest_marks: bool, use_index: bool = False, sort_by_tab_number: bool = True) -> None:
         def sort_function(item: Mark) -> Any:
             return item.TabNumber if sort_by_tab_number else item.GroupName
         self.table_with_caption_first_title_is_centered(ResultTool.sort(PIH.RESULT.MARK.free_list(show_guest_marks), sort_function), "Свободные карты доступа:", use_index)
 
     def guest_marks(self, use_index: bool = False) -> None:
@@ -945,15 +953,15 @@
         self.table_with_caption_first_title_is_centered(
             mark_list_result, "Гостевые карты доступа:", use_index)
 
     def temporary_candidate_for_mark(self, mark: Mark) -> None:
         self.mark.result(
             Result(FIELD_COLLECTION.ORION.FREE_MARK, [mark]), "Временная карта")
 
-    def free_marks_group_statistics(self, use_index: bool = False, show_guest_marks: bool = None) -> None:
+    def free_marks_group_statistics(self, use_index: bool = False, show_guest_marks: bool | None = None) -> None:
         self.free_marks_group_statistics_for_result(
             PIH.RESULT.MARK.free_marks_group_statistics(show_guest_marks), use_index)
 
     def free_marks_by_group(self, group: dict, use_index: bool = False) -> None:
         self.free_marks_by_group_for_result(PIH.RESULT.MARK.free_marks_by_group_id(group), group, use_index)
 
     def free_marks_group_statistics_for_result(self, result: Result, use_index: bool) -> None:
@@ -1070,15 +1078,15 @@
             self.mark.parent = self
 
     def input(self, caption: str = None, new_line: bool = True, check_function: Callable[[str], str] = None) -> str:
         try:
             while True:
                 if new_line and caption is not None:
                     self.output.input(caption)
-                value: str = input(self.output.TEXT_BEFORE) if new_line else input(self.output.TEXT_BEFORE + caption)
+                value: str = input(self.output.text_before) if new_line else input(self.output.text_before + caption)
                 if check_function is not None: 
                     value_after: str = check_function(value)
                     if value_after is not None:
                         return value_after
                 else:
                     return value
         except KeyboardInterrupt:
@@ -1089,15 +1097,15 @@
             self.output.input("Номер телефона")
             use_telephone_prefix: bool = telephone_prefix is not None
             telephone_number: str = self.input(
                 telephone_prefix if use_telephone_prefix else "", False)
             if use_telephone_prefix:
                 if not telephone_number.startswith(telephone_prefix):
                     telephone_number = telephone_prefix + telephone_number
-            check: bool = None
+            check: bool | None = None
             if format:
                 telehone_number_after_fix = PIH.DATA.FORMAT.telephone_number(
                     telephone_number, telephone_prefix)
                 check = PIH.CHECK.telephone_number(telehone_number_after_fix)
                 if check and telehone_number_after_fix != telephone_number:
                     telephone_number = telehone_number_after_fix
                     self.output.value("Телефон отформатирован", telephone_number)
@@ -1111,22 +1119,22 @@
         while True:
             email = self.input(title or "Адресс электронная почта")
             if PIH.CHECK.email(email):
                 return email
             else:
                 self.output.error("Неверный формат адресса электронной почты!")
 
-    def polibase_person_card_registry_folder(self) -> str:
-        value: str = None
+    def polibase_person_card_registry_folder(self, value: str | None = None) -> str:
         while True:
-            value = self.input("Введите название папки с картами пациентов")
+            value = value or self.input("Введите название папки с картами пациентов")
             if PIH.CHECK.POLIBASE.person_card_registry_folder_name(value):
                 return PIH.DATA.FORMAT.polibase_person_card_registry_folder(value)
             else:
                 self.output.error("Неверный формат названия папки с картами пациентов!")
+                value = None
 
     def message(self, caption: str = None, prefix: str = None) -> str:
         caption = caption or "Введите сообщение"
         self.output.input(caption)
         return (prefix or "") + self.input(prefix, False)
 
     def description(self) -> str:
@@ -1215,15 +1223,15 @@
         return self.input("Введите часть имени")
 
     def full_name(self, one_line: bool = False) -> FullName:
         if one_line:
             while(True):
                 value: str = self.input("Введите полное имя")
                 if PIH.CHECK.full_name(value):
-                    return FullNameTool.from_string(PIH.DATA.FORMAT.name(value))
+                    return FullNameTool.fullname_from_string(PIH.DATA.FORMAT.name(value))
                 else:
                     pass
         else:
             def full_name_part(caption: str) -> str:
                 while(True):
                     value: str = self.input(caption)
                     value = value.strip()
@@ -1251,15 +1259,14 @@
             return head_string + message
         else:
             pass
 
     def polibase_person_any(self, title: str | None = None) -> str:
         return self.input(title or "Введите персональный номер или часть имени пациента")
 
-
 class MarkInput(MarkInputBase):
 
     def __init__(self, input: Input = None):
         self.parent = input
 
     def free(self, group: MarkGroup = None) -> Mark:
         result: Result[list[Mark]] = None
@@ -1339,40 +1346,40 @@
 
 
 class UserInput(UserInputBase):
 
     def __init__(self, input: Input = None):
         self.parent = input
 
-    def container(self) -> UserContainer:
-        result: Result[list[UserContainer]] = PIH.RESULT.USER.containers()
+    def container(self) -> UserBase:
+        result: Result[list[UserBase]] = PIH.RESULT.USER.containers()
         self.parent.output.containers_for_result(result, True)
         return self.parent.item_by_index("Выберите контейнер пользователя, введя индекс", result.data)
 
     def by_name(self) -> User:
         result: Result[list[User]] = PIH.RESULT.USER.by_name(
             self.parent.name())
         result.fields = FIELD_COLLECTION.AD.USER_NAME
         self.parent.output.table_with_caption(
             result, "Список пользователей", True)
         return self.parent.item_by_index("Выберите пользователя, введя индекс", result.data)
 
     def title_any(self, title: str = None) -> str:
         return self.parent.input(title or "Введите логин, часть имени или другой поисковый запрос")
 
-    def by_any(self, value: str = None, active: bool = None, title: str = None, use_all: bool = False) -> list[User]:
+    def by_any(self, value: str = None, active: bool | None = None, title: str = None, use_all: bool = False) -> list[User]:
         result: Result[list[User]] = PIH.RESULT.USER.by_any(value or self.title_any(title), active)
         label_function: Callable[[Any, int], str] = (lambda item, _: "Все" if item is None else item.name) if len(
             result.data) > 1 else None
         if use_all and len(result.data) > 1:
             result.data.append(None)
         result_data: User = self.parent.item_by_index("Выберите пользователя, введя индекс", result.data, label_function)
         return result.data if result_data is None else [result_data]
 
-    def telephone_number(self, value: str = None, active: bool = None, title: str = None) -> User:
+    def telephone_number(self, value: str = None, active: bool | None = None, title: str = None) -> User:
         try:
             return self.by_any(value, active, title)
         except NotFound:
             return None
 
 
     def template(self) -> dict:
@@ -1411,15 +1418,15 @@
             user: User = PIH.RESULT.USER.by_login(login_string).data
             is_active: bool = PIH.CHECK.USER.active(user)
             self.parent.output.error(
                 f"Логин '{login_string}' занят {'активным' if is_active else 'неактивным'} пользователем: {user.name}")
             self.parent.output.new_line()
             return user if not is_active else None
         login: FullName = NamePolicy.convert_to_login(full_name)
-        login_string: str = FullNameTool.to_string(login, "")
+        login_string: str = FullNameTool.fullname_to_string(login, "")
         login_list.append(login_string)
         need_enter_login: bool = False
 
         def remove_inactive_user_action():
             login_string: str = None
             need_enter_login: bool = False
             if self.parent.yes_no("Удалить неактивных пользователей, чтобы освободить логин", True):
@@ -1441,32 +1448,32 @@
                 need_enter_login = True
             return need_enter_login, login_string
         if PIH.CHECK.USER.exists_by_login(login_string):
             user: User = show_user_which_login_is_exists_and_return_user_if_it_inactive(login_string)
             if user is not None:
                 inactive_user_list.append(user)
             login_alt: FullName = NamePolicy.convert_to_alternative_login(login)
-            login_string = FullNameTool.to_string(login_alt, "")
+            login_string = FullNameTool.fullname_to_string(login_alt, "")
             login_is_exists = login_string in login_list
             if not login_is_exists:
                 login_list.append(login_string)
             if login_is_exists or PIH.CHECK.USER.exists_by_login(login_string):
                 if not login_is_exists:
                     user = show_user_which_login_is_exists_and_return_user_if_it_inactive(
                         login_string)
                     if user is not None:
                         inactive_user_list.append(user)
                 login_reversed: FullName = NamePolicy.convert_to_reverse_login(login)
                 login_is_exists = login_string in login_list
-                login_string = FullNameTool.to_string(login_reversed, "")
+                login_string = FullNameTool.fullname_to_string(login_reversed, "")
                 if not login_is_exists:
                     login_list.append(login_string)
                 if login_is_exists or PIH.CHECK.USER.exists_by_login(login_string):
                     login_last: FullName = NamePolicy.convert_to_last_login(login)
-                    login_string = FullNameTool.to_string(login_last, "")
+                    login_string = FullNameTool.fullname_to_string(login_last, "")
                     if not login_is_exists:
                         user = show_user_which_login_is_exists_and_return_user_if_it_inactive(login_string)
                         if user is not None:
                             inactive_user_list.append(user)
                     if ask_for_remove_inactive_user_if_login_is_exists and len(inactive_user_list) > 0:
                         need_enter_login, login_string = remove_inactive_user_action()
                     if need_enter_login:
@@ -1484,16 +1491,16 @@
         else:
             if ask_for_use and not self.parent.yes_no(f"Использовать логин '{login_string}' для аккаунта пользователя", True):
                 login_string = self.parent.login(True)
 
         return login_string
 
 
-def while_not_do(check_action: Callable[[None], bool], attemp_count: int = None, success_handler: Callable[[None], None] = None, start_handler: Callable[[None], None] = None, sleep_time: int = None, action: Callable[[None], None] = None) -> None:
-    while not check_action():
+def while_not_do(check_action: Callable[[None], bool] | None = None, attemp_count: int = None, success_handler: Callable[[None], None] = None, start_handler: Callable[[None], None] = None, sleep_time: int = None, action: Callable[[None], None] = None) -> None:
+    while DataTool.is_empty(check_action) or not check_action():
         if start_handler is not None:
             start_handler()
             start_handler = None
         if action is not None:
             action()
         if attemp_count is not None:
             if attemp_count == 0:
@@ -1580,92 +1587,105 @@
         else:
             self.input: Input = input
         if session is None: 
             PIH.session: Session = Session(input, output)
         else:
             self.session: Session = session
         
-    class MOBILE_HELPER:
-
+    class MIO:
+    
         ANSWER: dict[str, list[str]] = defaultdict(list)
 
         @staticmethod
-        def create_output(recipient: str) -> Output:
-            return PIH.MESSAGE.WHATSAPP.create_output(recipient)
+        def create_output(recipient: str | Enum) -> Output:
+            from MobileHelperCore.api import MobileOutput, MobileSession
+            return MobileOutput(MobileSession(recipient if isinstance(recipient, str) else EnumTool.get(recipient)))
 
         @staticmethod
         def waiting_for_input_from(recipient: str, handler: Callable[[str, Callable[[None], None]], None] | None = None) -> str | None:
             def internal_handler(message: str, close_handler: Callable[[None], None]) -> None:
-                PIH.MOBILE_HELPER.ANSWER[recipient].append(message)
+                PIH.MIO.ANSWER[recipient].append(message)
                 if DataTool.is_empty(handler):
                     close_handler()
                 else:
                     handler(message, close_handler)  
             PIH.EVENT.waiting_for_mobile_helper_message_input(
                 recipient, internal_handler)
-            return PIH.MOBILE_HELPER.ANSWER[recipient][-1] 
+            return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
         @staticmethod
         def local() -> str:
-            return "1.43"
+            return "1.45"
 
         @staticmethod
         def need_update() -> bool:
             return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
+    
+    class INPUT_WAIT:
+
+        NAME: str = "RecipientWaitingForInput"
 
         @staticmethod
-        def remote() -> str:
-            try:
-                req = requests.get(URLS.PYPI)
-                version = parse("0")
-                if req.status_code == requests.codes.ok:
-                    data = json.loads(req.text.encode(req.encoding))
-                    releases = data.get("releases", [])
-                    for release in releases:
-                        ver = parse(release)
-                        if not ver.is_prerelease:
-                            version = max(version, ver)
-                return str(version)
-            except ConnectionError:
-                return 
+        def _get_name(group_name: str, recipient:str) -> str:
+            return ":".join((group_name, recipient))
+
+        @staticmethod
+        def add(group_name: str, recipient: str, timeout: int) -> bool:
+            return PIH.ACTION.DATA_STORAGE.value(RecipientWaitingForInput(group_name, timeout, recipient, PIH.DATA.now()), PIH.INPUT_WAIT._get_name(group_name, recipient), PIH.INPUT_WAIT.NAME)
+
+        @staticmethod
+        def remove(group_name: str, recipient: str) -> bool:
+            return PIH.ACTION.DATA_STORAGE.value(None, PIH.INPUT_WAIT._get_name(group_name, recipient), PIH.INPUT_WAIT.NAME)
+        
+        @staticmethod
+        def has(group_name: str, recipient: str) -> RecipientWaitingForInput:
+            def extractor(data: Any | None) -> RecipientWaitingForInput | None:
+                if DataTool.is_none(data):
+                    return None
+                result: RecipientWaitingForInput = DataTool.fill_data_from_source(RecipientWaitingForInput(), data)
+                result.timestamp = DateTimeTool.datetime_from_string(result.timestamp)
+                return result
+            result: RecipientWaitingForInput | None = PIH.RESULT.DATA_STORAGE.value(PIH.INPUT_WAIT._get_name(group_name, recipient), extractor, PIH.INPUT_WAIT.NAME).data
+            return DataTool.is_not_none(result) and (DateTimeTool.now() - result.timestamp).seconds < result.timeout
 
     class ERROR:
 
         notify_about_error: bool = True
 
         @staticmethod
         def create_error_header(details: str) -> str:
-            return f"\nВерсия: {PIH.VERSION.local()}/{PIH.VERSION.remote()}\nПользователь: {PIH.OS.get_login()}\nКомпьютер: {PIH.OS.host()}\n{details}"
+            return f"\nВерсия: {PIH.VERSION.local()}\nПользователь: {PIH.OS.get_login()}\nКомпьютер: {PIH.OS.host()}\n{details}"
 
         @staticmethod
-        def rpc_error_handler(details: str, code: Tuple, service_role_description: ServiceRoles, command: ServiceCommands) -> None:
+        def rpc_error_handler(details: str, code: tuple, description: ServiceRoles, command: ServiceCommands) -> None:
             if isinstance(command, ServiceCommands):
                 if code == StatusCode.UNAVAILABLE:
-                    PIH.output.error(f"Error: {details}")
+                    if PIH.ERROR.notify_about_error:
+                        PIH.output.error(f"Error: {details}")
                     return
                 elif code == StatusCode.DEADLINE_EXCEEDED or details.lower().find("stream removed") != -1:
                     return
                 else:
                     if PIH.ERROR.notify_about_error:
                         PIH.LOG.debug(
-                            PIH.ERROR.create_error_header(details), LogLevels.ERROR)
+                            PIH.ERROR.create_error_header(details), LogMessageFlags.ERROR)
             raise Error(details, code) from None
 
         @staticmethod
         def global_except_hook(exctype, value, __traceback__):
             details_list: list[str] = []
             for item in value.args:
                 if isinstance(item, str):
                     details_list.append(item)
             details: str = "\n".join(traceback.format_exception(value))
             if PIH.ERROR.notify_about_error:
                 PIH.LOG.debug(
-                    PIH.ERROR.create_error_header(details), LogLevels.ERROR)
+                    PIH.ERROR.create_error_header(details), LogMessageFlags.ERROR)
             sys.__excepthook__(exctype, value, traceback)
 
         sys.excepthook = global_except_hook
 
         class POLIBASE:
 
             @staticmethod
@@ -1685,29 +1705,29 @@
                 else:
                     start = "Неактивный пользователь"
                 return NotFound(f"{start} с {title} '{value}' не найден", value)
 
     class UPDATER:
 
         @staticmethod
-        def update_for_service(service_role: ServiceRoles, pih_update: bool = True, modules_update: bool = True, show_output: bool = False) -> bool:
-            service_role_description: ServiceRoleDescription = service_role.value
+        def update_for_service(role_or_information: ServiceRoles | ServiceDescription, pih_update: bool = False, modules_update: bool = True, show_output: bool = True) -> bool:
+            description: ServiceDescription = ServiceRoles.description(role_or_information)
             returncode: int = 0
             if pih_update:
-                remote_executor_command_list: list[str] = PIH.PSTOOLS.create_remote_process_executor_for_service(service_role_description, True)
+                remote_executor_command_list: list[str] = PIH.PSTOOLS.create_remote_process_executor_for_service(description, True)
                 command_list: list[str] = remote_executor_command_list + \
                     PIH.UPDATER.get_module_updater_command_list(PIH.NAME, None)
                 process_result: CompletedProcess = PIH.PSTOOLS.execute_command_list(
                     command_list, show_output)
                 returncode = process_result.returncode
             result: bool = returncode == 0
             if modules_update and result:
                 installed_module_list: list[str] = {
                     pkg.key.lower() for pkg in pkg_resources.working_set}
-                for module_name in [item.lower() for item in service_role_description.modules]:
+                for module_name in [item.lower() for item in description.modules]:
                     if module_name not in installed_module_list:
                         result = result and PIH.UPDATER.install_module(
                             module_name, show_output=show_output)
                         if result:
                             pkg_resources.working_set.add_entry(module_name)
                         else:
                             break
@@ -1784,14 +1804,22 @@
 
         @staticmethod
         def init() -> None:
             for setting_item in SETTINGS:
                 if setting_item.value.auto_init:
                     PIH.SETTINGS.set_default(setting_item)
 
+        @staticmethod
+        def find(name: str) -> list[SETTINGS]:
+            result: list[SETTINGS] = []
+            for item in SETTINGS:
+                if StringTool.contains(item.name, name) or StringTool.contains(item.value.key_name, name):
+                    result.append(item)
+            return result
+
         class WORKSTATION:
 
             @staticmethod
             def shutdown_time() -> datetime:
                 return PIH.DATA.CONVERT.settings_to_datetime(SETTINGS.WORKSTATION_SHUTDOWN_TIME)
             
             @staticmethod
@@ -1855,282 +1883,850 @@
                 @staticmethod
                 def offer_telegram_bot_url_text(person_full_name: str) -> str:
                     return str(PIH.SETTINGS.get(SETTINGS.POLIBASE_PERSON_TAKE_TELEGRAM_BOT_URL_TEXT)).format(name=FullNameTool.to_given_name(person_full_name)) 
 
     class PSTOOLS:
 
         @staticmethod
+        def get_users_logged_on(host: str, active: bool | None = True) -> list[str]:
+            def get_login_list(complete_process: CompletedProcess) -> set[str]:
+                result: set[str] = set()
+                output: str = complete_process.stdout.decode(WINDOWS.CHARSETS.ALTERNATIVE)
+                for line in output.splitlines()[1:]:
+                    line = line.lower()
+                    if DataTool.is_none(active) or (active and (line.find("active") != -1 or line.find("активно") != -1)) or (not active and (line.find("disc") != -1 or line.find("диск") != -1)):
+                        result.add(line.split(" ")[1])
+                return result
+            result: set[str] = set()
+            result |= get_login_list(PIH.PSTOOLS.execute_command_list(
+                ["query", "user", "/server:" + host], True, True, False))
+            result |= get_login_list(PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
+                ["query", "user", "/server"], host, interactive=None, run_from_system_account=True), True, True, False))
+            return list(result)
+
+        @staticmethod
+        def stop_windows_service(name: str, workstation_name: str) -> bool:
+            output: str = A.PS.execute_command_list(A.PS.create_command_list_for_psexec_command(
+            ["sc", "stop", "stisvc"], workstation_name,  interactive=True, run_from_system_account=True), True, True).stdout
+            return output.find("3  STOP_PENDING") != -1
+
+        @staticmethod
+        def start_windows_service(name: str, workstation_name: str) -> bool:
+            output: str = A.PS.execute_command_list(A.PS.create_command_list_for_psexec_command(
+            ["sc", "start", "stisvc"], workstation_name, interactive=True, run_from_system_account=True), True, True).stdout
+            return output.find("2  START_PENDING") != -1 
+
+        @staticmethod
+        def windows_service_running(name: str, workstation_name: str) -> bool:
+            output: str = A.PS.execute_command_list(A.PS.create_command_list_for_psexec_command(
+            ["sc", "query", "stisvc"], workstation_name, interactive=True), True, True).stdout
+            return output.find("4  RUNNING") != -1
+
+        @staticmethod
         def ping(address_or_ip: str, host: str, count: int = 1, timeout: int = 100):
             command_list: list[str] = ["ping", "-4",  address_or_ip, "-n",
                                        str(count), "-w", str(timeout)]
             result: CompletedProcess = PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(command_list, host, interactive=True), True, True)
-            out: str = result.stdout
-            return result.returncode == 0 and out.count("(TTL)") < count
+            output: str = result.stdout
+            return result.returncode == 0 and output.count("(TTL)") < count
           
         @staticmethod
         def get_executor_path(executor_name: str) -> str:
             return os.path.join(
                 PATHS.WS.PATH, CONST.PSTOOLS.NAME, executor_name)
 
         @staticmethod
-        def as_host(value: str) -> str:
-            host_start: str = r"\\"
-            return ("" if value.startswith(host_start) else host_start) + value 
-
-        @staticmethod
         def create_command_list_for_command(executor_name: str, command_list: list[str], login: str = None, password: str = None) -> list[str]:
             login = "\\".join([AD.DOMAIN_NAME, AD.ADMINISTRATOR if DataTool.is_empty(login) else login])
             password = password or AD.ADMINISTRATOR_PASSOWORD
             return [PIH.PSTOOLS.get_executor_path(executor_name), CONST.PSTOOLS.NO_BANNER, CONST.PSTOOLS.ACCEPTEULA, "-u", login, "-p", password]  + command_list
         
         @staticmethod
-        def create_command_list_for_psexec_command(command_list: list[str], host: str = None, login: str = None, password: str = None, interactive: bool = False, run_from_system_account: bool = False, run_with_elevetion: bool = False) -> list[str]:
-            result_command_list: list[str] = ["-i" if interactive else "-d"]
+        def create_command_list_for_psexec_command(command_list: list[str], host: str = None, login: str = None, password: str = None, interactive: bool | None = False, run_from_system_account: bool = False, run_with_elevetion: bool = False) -> list[str]:
+            result_command_list: list[str] = DataTool.check_not_none(interactive, lambda: [["-d", "-i"][interactive]], [])
             host_start: str = r"\\"
             if not DataTool.is_empty(host):
                 result_command_list.append(("" if host.startswith(host_start) else host_start) + host)
             if run_from_system_account:
                 result_command_list.append("-s")
             if run_with_elevetion:
                 result_command_list.append("-h")
-            return PIH.PSTOOLS.create_command_list_for_command(CONST.PSTOOLS.PS_EXECUTOR, result_command_list + command_list, login, password)
+            return PIH.PSTOOLS.create_command_list_for_psexec_command_local(result_command_list + command_list, login, password)
+        
+        @staticmethod
+        def create_command_list_for_psexec_command_local(command_list: list[str], login: str = None, password: str = None) -> list[str]:
+            return PIH.PSTOOLS.create_command_list_for_command(CONST.PSTOOLS.PS_EXECUTOR, command_list, login, password)
 
         @staticmethod
-        def create_remote_process_executor_for_service(service_role_or_description: ServiceRoles | ServiceRoleDescription, interactive: bool = False) -> list[str]:
-            service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
-            return PIH.PSTOOLS.create_command_list_for_psexec_command([CONST.PYTHON.EXECUTOR], PIH.SERVICE.get_host(service_role_description), service_role_description.login, service_role_description.password, interactive)
+        def create_remote_process_executor_for_service(role_or_information: ServiceRoles | ServiceInformationBase, interactive: bool | None = False) -> list[str]:
+            description: ServiceDescription = ServiceRoles.description(role_or_information)
+            return PIH.PSTOOLS.create_command_list_for_psexec_command([role_or_information.pyton_executor_path or CONST.PYTHON.EXECUTOR_ALIAS], PIH.SERVICE.get_host(description), description.login, description.password, interactive, description.run_from_system_account)
 
         @staticmethod
-        def execute_command_list(command_list: list[str], show_output: bool, capture_output: bool = False) -> CompletedProcess:
+        def execute_command_list(command_list: list[str], show_output: bool, capture_output: bool = False, as_text: bool = True) -> CompletedProcess:
             if show_output:
                 if capture_output:
                     process_result = subprocess.run(
-                        command_list, capture_output=True, text=True)
+                        command_list, capture_output=True, text=as_text)
                 else:
                     process_result = subprocess.run(
-                        command_list, text=True)
+                        command_list, text=as_text)
             else:
                 process_result = subprocess.run(
-                    command_list, stdout=DEVNULL, stderr=STDOUT, text=True)
+                    command_list, stdout=DEVNULL, stderr=STDOUT, text=as_text)
             return process_result
-       
+
         @staticmethod
-        def kill_process(name_or_pid: str | int, host: str, show_output: bool = False) -> bool:
-           return PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_command(CONST.PSTOOLS.PS_KILL_EXECUTOR, ["-t", str(name_or_pid), PIH.PSTOOLS.as_host(host)]), show_output).returncode == 0
+        def kill_process(name_or_pid: str | int, host: str, via_taskkill: bool = True, show_output: bool = False) -> bool:
+           if via_taskkill:
+                is_string: bool = isinstance(name_or_pid, str)
+                return PIH.PSTOOLS.execute_command_list(["taskkill", "/s", host, "/t", "/f", "/im" if is_string else "/pid", PIH.PATH.add_extension(name_or_pid, FILE.EXTENSION.EXE) if is_string else str(name_or_pid)], show_output).returncode < 2
+           return PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_command(CONST.PSTOOLS.PS_KILL_EXECUTOR, [PIH.DATA.FORMAT.host(host), "-t", str(name_or_pid)]), show_output).returncode == 0
 
         @staticmethod
-        def kill_process_via_windows(name_or_pid: str | int, host: str, show_output: bool = False) -> bool:
-           is_string : bool = isinstance(name_or_pid, str)
-           return PIH.PSTOOLS.execute_command_list(["taskkill", "/S", PIH.PSTOOLS.as_host(host), "/F", "/IM" if is_string else "/PID", PIH.PATH.add_extension(name_or_pid, FILE.EXTENSION.EXE) if is_string else str(name_or_pid)], show_output).returncode == 0
+        def process_is_exists(pid: int, host: str | None = None, login: str = None, password: str = None) -> str:
+            command_list: list[str] = ["tasklist", "/fi", f"pid eq {pid}", "/fo", "list"]
+            login = "\\".join(
+                [AD.DOMAIN_NAME, AD.ADMINISTRATOR if DataTool.is_empty(login) else login])
+            password = password or AD.ADMINISTRATOR_PASSOWORD
+            if not DataTool.is_empty(host):
+                command_list += ["/s", host]
+                command_list += ["/u", login]
+                command_list += ["/p", password]
+            output: str = PIH.PSTOOLS.execute_command_list(
+                command_list, True, True, as_text=False).stdout.decode(WINDOWS.CHARSETS.ALTERNATIVE).lower()
+            return output.find("pid") != -1
 
         @staticmethod
-        def reboot(host: str, show_output: bool = False) -> bool:
-            return PIH.PSTOOLS.execute_command_list(A.PS.create_command_list_for_psexec_command(
-                ["shutdown", "/r", "/t", "0"], host), show_output).returncode == 0
+        def kill_python_process(host: str, via_taskkill: bool) -> bool:
+            return PIH.PSTOOLS.kill_process(CONST.PYTHON.EXECUTOR, host, via_taskkill)
 
         @staticmethod
-        def shutdown(host: str, show_output: bool = False) -> bool:
+        def _ws_action(value: str, host: str, show_output: bool = False) -> bool:
             return PIH.PSTOOLS.execute_command_list(A.PS.create_command_list_for_psexec_command(
-                ["shutdown", "/s", "/t", "0"], host), show_output).returncode == 0
+                ["shutdown", value, "/t", "0"], host), show_output).returncode == 0
+
+        @staticmethod
+        def ws_reboot(host: str, show_output: bool = False) -> bool:
+            return PIH.PSTOOLS._ws_action("/r", host, show_output)
+
+        @staticmethod
+        def ws_shutdown(host: str, show_output: bool = False) -> bool:
+            return PIH.PSTOOLS._ws_action("/s", host, show_output)
         
     class EVENT:
 
         @staticmethod
-        def on_log_command(handler: Callable[[ParameterList, ServiceListener], None]) -> None:
-            ServiceListener().listen_for([ServiceCommands.send_log_command], lambda _, parameter_list, service_listener: handler(parameter_list, service_listener))
+        def send(value: Events, parameters: tuple[Any] | None = None) -> None:
+            def internal_send_command(command_name: str, parameters: dict) -> None:
+                try:
+                    PIH.SERVICE.call_command(ServiceCommands.send_event,
+                             (command_name, parameters))
+                except Error as error:
+                    PIH.output.error("Log send error")
+            PIH.LOG.executor.submit(internal_send_command,
+                                    value.name, PIH.EVENT.BULDER.create_parameters_map(value, parameters))   
+
+        @staticmethod
+        def computer_was_started(name: str) -> None:
+            PIH.EVENT.send(
+                Events.COMPUTER_WAS_STARTED, (name,))
+
+        @staticmethod
+        def server_was_started(name: str) -> None:
+            PIH.EVENT.send(
+                Events.SERVER_WAS_STARTED, (name,))
+            
+        @staticmethod
+        def get_parameter(event: Events, parameters: dict[str, Any], parameter_name: str | None = None) -> Any | dict[str, Any]:
+            parameters_map: dict[str, Any] = PIH.EVENT.BULDER.create_parameters_map(event, parameters)
+            return DataTool.check_not_none(parameter_name, lambda: parameters_map[parameter_name], parameters_map)
+
+        class BULDER:
+    
+            @staticmethod
+            def create_parameters_map(event: Events, parameters: tuple[Any] | None = None, check_for_parameters_count: bool = True) -> dict:
+                event_description: EventDescription = EnumTool.get(event)
+                parameter_pattern_list: list = DataTool.as_list(
+                    event_description.params)
+                parameters = parameters or ()
+                if check_for_parameters_count and len(parameter_pattern_list) > len(parameters):
+                    raise Exception(
+                        "Income parameter list length is less that parameter list length of command")
+                result: dict[str, Any] = {}
+                for index, parameter_pattern_item in enumerate(parameter_pattern_list):
+                    if index < len(parameters):
+                        parameter_pattern: ParamItem = parameter_pattern_item
+                        result[parameter_pattern.name] = parameters[index]
+                    else:
+                        break
+                return result
+
+            @staticmethod
+            def create_event(event: Events, paramters: Any | None = None, parameters_getter: Callable[[None], Any] | None = None, default_value: tuple[Any] | Any | None = None) -> Events | tuple[Events | tuple[Any]] | tuple[Any]:
+                return DataTool.check_not_none(paramters, lambda: (event, parameters_getter()), event if DataTool.is_none(default_value) else (event, default_value))
+            
+            @staticmethod
+            def polibase_person_with_inaccessable_email_was_detected(person: PolibasePerson | None = None, registrator_person: PolibasePerson | None = None, actual: bool = False) -> tuple[Events | tuple[Any]] | Events:
+                def get_information() -> tuple[Any]:
+                    workstation_name: str = "<не определён>"
+                    workstation_description: str = "<не определён>"
+                    if actual:
+                        try:
+                            user: User = A.R_U.by_polibase_pin(
+                                registrator_person.pin).data
+                            workstation: Workstation = A.R.get_first_element(
+                                A.R_WS.by_login(user.samAccountName)) or A.R_WS.by_name(A.CT.TEST.WORKSTATION_MAME).data
+                            if A.D.is_not_none(workstation):
+                                workstation_name = workstation.name
+                                workstation_description = workstation.description
+                        except NotFound:
+                                pass
+                    return (person.FullName, person.pin, person.email, registrator_person.FullName, workstation_name, workstation_description)
+                event: Events = Events.POLIBASE_PERSON_WITH_INACCESSABLE_EMAIL_WAS_DETECTED
+                return PIH.EVENT.BULDER.create_event(event, registrator_person, get_information, DataTool.check_not_none(person, lambda: (None, person.pin)))
+
+            @staticmethod
+            def polibase_person_duplication_was_detected(person: PolibasePerson | None = None, duplicated_person: PolibasePerson | None = None, registrator_person: PolibasePerson | None = None) -> Events | tuple[Events, tuple[Any]]:
+                event: Events = Events.POLIBASE_PERSON_DUPLICATION_WAS_DETECTED
+                def get_information() -> tuple[Any]:
+                    return (person.FullName, person.pin, duplicated_person.pin, duplicated_person.pin, registrator_person.FullName)
+                return PIH.EVENT.BULDER.create_event(event, person, get_information)
+
+            @staticmethod
+            def polibase_person_email_was_added(person: PolibasePerson | None = None, person_for_search: PolibasePerson | None = None) -> Events | tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BULDER.create_event(Events.POLIBASE_PERSON_EMAIL_WAS_ADDED, person, lambda: (person.FullName, person.pin, person.email), DataTool.check_not_none(person_for_search, lambda: (None, person_for_search.pin)))
+            
+            @staticmethod
+            def service_was_started(information: ServiceInformation | None = None) -> Events | tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BULDER.create_event(Events.SERVICE_WAS_STARTED, information, lambda: (information.name,
+                                                    information.host, information.port, information.pid,  information))
+
+            @staticmethod
+            def chiller_temperature_alert_was_fired(date: str | None = None) -> Events | tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BULDER.create_event(Events.MRI_CHILLER_TEMPERATURE_ALERT_WAS_FIRED, date, lambda: (date, ))
+            
+            staticmethod
+            def chiller_was_turned_off(date: str | None = None) -> Events | tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BULDER.create_event(Events.MRI_CHILLER_TEMPERATURE_ALERT_WAS_FIRED, date, lambda: (date, ))
+
+            @staticmethod
+            def service_was_stopped(information: ServiceInformationBase | None = None) -> Events | tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BULDER.create_event(Events.SERVICE_WAS_STOPPED, information, lambda: (information.name, information) )
+            
+            @staticmethod
+            def polibase_persons_barcodes_old_format_were_detected(person_pin_list: list[int] | None = None) -> Events | tuple[Events, tuple[Any]]:
+                return  PIH.EVENT.BULDER.create_event(Events.POLIBASE_PERSONS_WITH_OLD_FORMAT_BARCODE_WAS_DETECTED, person_pin_list, lambda: (person_pin_list, ))
+            
+            @staticmethod
+            def polibase_person_barcodes_new_format_were_created(person_pin_list: list[int] | None = None) -> Events | tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BULDER.create_event(Events.POLIBASE_PERSON_BARCODES_WITH_OLD_FORMAT_WERE_CREATED, person_pin_list, lambda: (person_pin_list, ))
+
+            @staticmethod
+            def polibase_person_was_created(value: PolibasePerson | None = None) -> Events | tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BULDER.create_event(Events.POLIBASE_PERSON_WAS_CREATED, value, lambda: (value.FullName, value.pin, value))
+            
+            @staticmethod
+            def polibase_person_was_updated(value: PolibasePerson | None = None) -> tuple[Events, tuple[Any]]:
+                return PIH.EVENT.BULDER.create_event(Events.POLIBASE_PERSON_WAS_UPDATED, value, lambda: (value.FullName, value.pin, value)) 
+
+        @staticmethod
+        def polibase_person_visit_was_registered(value: PolibasePersonVisitDS) -> None:
+            PIH.EVENT.send(Events.POLIBASE_PERSON_VISIT_WAS_REGISTERED, (
+                value.FullName, "Предзапись" if value.pin == CONST.POLIBASE.PRERECORDING_PIN else value.pin, value))
+
+
+        @staticmethod
+        def resource_accessible(resource: ResourceStatus, at_first_time: bool) -> None:
+            PIH.EVENT.send(Events.RESOURCE_ACCESSABLE,
+                                (resource.name, resource, at_first_time))
+
+        @staticmethod
+        def resource_inaccessible(resource: ResourceStatus, at_first_time: bool, reason: RESOURCES.INACCESSABLE_REASONS | None = None) -> None:
+            reason_string: str = ""
+            reason_name: str | None = None
+            if not DataTool.is_empty(reason):
+                reason_string = f"Причина: {reason.value}"
+                reason_name = reason.name
+            PIH.EVENT.send(Events.RESOURCE_INACCESSABLE, (resource.name,
+                                resource, at_first_time, reason_string, reason_name))
+
+        @staticmethod
+        def polibase_person_visit_notification_was_registered(visit: PolibasePersonVisitDS, notification: PolibasePersonVisitNotificationDS) -> None:
+            PIH.EVENT.send(Events.POLIBASE_PERSON_VISIT_NOTIFICATION_WAS_REGISTERED, (
+                visit.FullName, "Предзапись" if visit.pin == CONST.POLIBASE.PRERECORDING_PIN else visit.pin, notification))
+
+        @staticmethod
+        def login() -> None:
+            login: str = PIH.session.get_login()
+            user: User = PIH.RESULT.USER.by_login(login).data
+            PIH.EVENT.send(
+                Events.LOG_IN, (user.name, login, PIH.OS.host()))
+
+        @staticmethod
+        def whatsapp_message_received(message: WhatsAppMessage) -> None:
+            PIH.EVENT.send(
+                Events.WHATSAPP_MESSAGE_RECEIVED, (message,))
+
+        @staticmethod
+        def new_file_detected(path: str) -> None:
+            PIH.EVENT.send(
+                Events.NEW_FILE_DETECTED, (path,))
+
+        @staticmethod
+        def new_polibase_scanned_document_detected(value: PolibaseScannedDocument):
+            PIH.EVENT.send(Events.NEW_POLIBASE_DOCUMENT_DETECTED,
+                                (value.file_path, value.pin, value.document_name))
+
+        @staticmethod
+        def start_session() -> None:
+            argv: list[str] = PIH.session.argv
+            argv_str: str = ""
+            if not DataTool.is_empty(argv):
+                argv_str = " ".join(argv)
+                argv_str = f"({argv_str})"
+            login: str = PIH.session.get_login()
+            user: User = PIH.RESULT.USER.by_login(login).data
+            PIH.EVENT.send(Events.SESSION_STARTED, (user.name, login,
+                                                        f"{PIH.session.file_name} {argv_str}", f"{PIH.VERSION.local()}", PIH.OS.host()))
+
+        @staticmethod
+        def backup_robocopy_job_was_started(name: str, job_status: RobocopyJobStatus) -> None:
+            PIH.EVENT.send(
+                Events.BACKUP_ROBOCOPY_JOB_WAS_STARTED, (name, job_status.pid))
+
+        @staticmethod
+        def backup_robocopy_job_was_completed(name: str, job_status: RobocopyJobStatus) -> None:
+            status: int = job_status.last_status
+            is_live: bool = job_status.pid > 0
+            status_string: str = "live job" if is_live else str(status)
+            pid_string: str = str(job_status.pid) if is_live else "not live job"
+            if status >= ROBOCOPY.ERROR_CODE_START:
+                status_string += " (есть ошибки)"
+            PIH.EVENT.send(
+                Events.BACKUP_ROBOCOPY_JOB_WAS_COMPLETED, (name, status_string, status, pid_string))
+
+        @staticmethod
+        def service_is_inaccessable_and_will_be_restarted(information: ServiceInformationBase ) -> None:
+            PIH.EVENT.send(Events.SERVICE_IS_INACCESIBLE_AND_WILL_BE_RESTARTED, (information.name, information))
+
+        @staticmethod
+        def service_was_not_started(information: ServiceInformation, error: str) -> None:
+            PIH.EVENT.send(Events.SERVICE_WAS_NOT_STARTED, (information.name,
+                                                            information.host, information.port, error, information))
+
+        @staticmethod
+        def hr_notify_about_new_employee(login: User) -> None:
+            user: User = PIH.RESULT.USER.by_login(login).data
+            hr_user: User = ResultTool.get_first_element(
+                PIH.RESULT.USER.by_job_position(AD.JobPisitions.HR))
+            PIH.EVENT.send(Events.HR_NOTIFY_ABOUT_NEW_EMPLOYEE, (FullNameTool.to_given_name(hr_user.name),
+                                                                        user.name, user.mail))
+
+        @staticmethod
+        def it_notify_about_user_creation(login: str, password: str) -> None:
+            it_user_list: list[User] = PIH.RESULT.USER.by_job_position(
+                AD.JobPisitions.IT).data
+            me_user_login: str = PIH.session.get_login()
+            it_user_list = list(
+                filter(lambda user: user.samAccountName != me_user_login, it_user_list))
+            it_user: User = it_user_list[0]
+            user: User = PIH.RESULT.USER.by_login(login).data
+            PIH.EVENT.send(Events.IT_NOTIFY_ABOUT_CREATE_USER, (
+                user.name, user.description, user.samAccountName, password, user.telephoneNumber, user.mail))
+            PIH.EVENT.send(Events.IT_TASK_AFTER_CREATE_NEW_USER, (FullNameTool.to_given_name(
+                it_user.name), user.name, user.mail, password))
+
+        @staticmethod
+        def it_notify_about_mark_creation(temporary: bool, full_name: Any, tab_number: str = None) -> None:
+            name: str = FullNameTool.fullname_to_string(full_name) if isinstance(
+                full_name, FullName) else full_name
+            mark: Mark = PIH.RESULT.MARK.by_name(name, True).data
+            telephone_number: str = PIH.DATA.FORMAT.telephone_number(
+                mark.telephoneNumber)
+            if temporary:
+                PIH.EVENT.send(Events.IT_NOTIFY_ABOUT_CREATE_TEMPORARY_MARK,
+                                    (name, tab_number, telephone_number))
+            else:
+                PIH.EVENT.send(Events.IT_NOTIFY_ABOUT_CREATE_NEW_MARK, (
+                    name, telephone_number, mark.TabNumber, mark.GroupName))
+
+        @staticmethod
+        def it_notify_about_temporary_mark_return(mark: Mark, temporary_tab_number: int) -> None:
+            PIH.EVENT.send(
+                Events.IT_NOTIFY_ABOUT_TEMPORARY_MARK_RETURN, (mark.FullName, temporary_tab_number))
+
+        @staticmethod
+        def backup_notify_about_polibase_creation_db_dumb_start() -> None:
+            PIH.EVENT.send(
+                Events.POLIBASE_CREATION_DB_DUMP_START)
+
+        @staticmethod
+        def backup_notify_about_polibase_creation_db_dumb_complete() -> None:
+            PIH.EVENT.send(
+                Events.POLIBASE_CREATION_DB_DUMP_COMPLETE)
+
+        @staticmethod
+        def backup_notify_about_polibase_creation_archived_db_dumb_start() -> None:
+            PIH.EVENT.send(
+                Events.POLIBASE_CREATION_ARCHIVED_DB_DUMP_START)
+
+        @staticmethod
+        def backup_notify_about_polibase_creation_archived_db_dumb_complete() -> None:
+            PIH.EVENT.send(
+                Events.POLIBASE_CREATION_ARCHIVED_DB_DUMP_COMPLETE)
+
+        @staticmethod
+        def backup_notify_about_polibase_coping_archived_db_dumb_start(destination: str) -> None:
+            PIH.EVENT.send(
+                Events.POLIBASE_COPING_ARCHIVED_DB_DUMP_START, (destination,))
+
+        @staticmethod
+        def backup_notify_about_polibase_coping_archived_db_dumb_complete(destination: str) -> None:
+            PIH.EVENT.send(
+                Events.POLIBASE_COPING_ARCHIVED_DB_DUMP_COMPLETE, (destination,))
+
+        @staticmethod
+        def backup_notify_about_polibase_coping_db_dumb_start(destination: str) -> None:
+            PIH.EVENT.send(
+                Events.POLIBASE_COPING_DB_DUMP_START, (destination,))
+
+        @staticmethod
+        def backup_notify_about_polibase_coping_db_dumb_complete(destination: str) -> None:
+            PIH.EVENT.send(
+                Events.POLIBASE_COPING_DB_DUMP_COMPLETE, (destination,))
+
+        @staticmethod
+        def it_notify_about_mark_return(mark: Mark) -> None:
+            PIH.EVENT.send(
+                Events.IT_NOTIFY_ABOUT_MARK_RETURN, (mark.FullName, mark.TabNumber))
+
+        @staticmethod
+        def it_notify_about_create_new_mark(full_name: Any) -> None:
+            PIH.EVENT.it_notify_about_mark_creation(
+                False, full_name)
+
+        @staticmethod
+        def it_notify_about_create_temporary_mark(full_name: Any, tab_number: str) -> None:
+            PIH.EVENT.it_notify_about_mark_creation(
+                True, full_name, tab_number)
+
+        @staticmethod
+        def printer_report(name: str, location: str, report: str) -> bool:
+            return PIH.EVENT.send(Events.PRINTER_REPORT, (name, location, report))
+
+        @staticmethod
+        def on_event(handler: Callable[[ParameterList, ServiceListener], None], block: bool = True) -> None:
+            def thread_handler() -> None:
+                ServiceListener().listen_for([ServiceCommands.send_event], lambda _, parameter_list, service_listener: handler(parameter_list, service_listener))
+            if block:
+                thread_handler()
+            else:
+                Thread(target=thread_handler).start()
 
         @staticmethod
         def wait_server_start(handler_or_server_name: Callable[[str, Callable[[None], None]], None] | str) -> None:
             def internal_handler(parameter_list: ParameterList, listener: ServiceListener) -> None:
-                log_command, parameters = PIH.DATA.EXTRACT.SERVICE_PARAMETER_LIST.log_command_parameters(parameter_list)
-                if log_command == LogCommands.SERVER_WAS_STARTED:
+                event, parameters = PIH.DATA.EXTRACT.EVENT.with_parameters(parameter_list)
+                if event == Events.SERVER_WAS_STARTED:
                     server_name: str = parameters[0]
                     if callable(handler_or_server_name):
                         handler_or_server_name(server_name, listener.close)
                     else:
                         if handler_or_server_name.startswith(server_name):
                             listener.close()
-            PIH.EVENT.on_log_command(internal_handler)
+            PIH.EVENT.on_event(internal_handler)
+
 
         @staticmethod
-        def wait_robocopy_job_complete(handler_or_robocopy_job_name: Callable[[ParameterList, ServiceListener], None] | str) -> None:
+        def on_service_starts(handler_or_service_role_or_information: Callable[[str, Callable[[None], None]], None] | ServiceRoles | ServiceInformationBase) -> None:
             def internal_handler(parameter_list: ParameterList, listener: ServiceListener) -> None:
-                log_command, parameters = PIH.DATA.EXTRACT.SERVICE_PARAMETER_LIST.log_command_parameters(parameter_list)
-                if log_command ==  A.CT_LC.BACKUP_NOTIFY_ABOUT_ROBOCOPY_JOB_COMPLETED:
-                    robocopy_job_status: str = parameters[0]
+                event, parameters = PIH.DATA.EXTRACT.EVENT.with_parameters(parameter_list)
+                if event == A.E_B.service_was_started():
+                    service_description_name: str = parameters[0]
+                    if callable(handler_or_service_role_or_information):
+                        handler_or_service_role_or_information(service_description_name, listener.close)
+                    elif handler_or_service_role_or_information == service_description_name:
+                        listener.close()
+            PIH.EVENT.on_event(internal_handler)
+        
+        @staticmethod
+        def on_robocopy_job_complete(handler_or_robocopy_job_name: Callable[[str, int, ServiceListener], None] | str) -> bool | None:
+            class DATA_HOLDER:
+                result: bool | None = None
+            def internal_handler(parameter_list: ParameterList, listener: ServiceListener) -> None:
+                event, parameters = PIH.DATA.EXTRACT.EVENT.with_parameters(parameter_list)
+                if event == A.CT_E.BACKUP_ROBOCOPY_JOB_WAS_COMPLETED:
+                    robocopy_job_status_name: str = parameters[0]
+                    robocopy_job_status: int = parameters[-1]
+                    DATA_HOLDER.result = robocopy_job_status < ROBOCOPY.ERROR_CODE_START
                     if callable(handler_or_robocopy_job_name):
                         handler_or_robocopy_job_name(
-                            robocopy_job_status, listener.close)
+                            robocopy_job_status_name, robocopy_job_status, listener)
                     else:
-                        if robocopy_job_status.startswith(handler_or_robocopy_job_name):
+                        if robocopy_job_status_name.startswith(handler_or_robocopy_job_name):
                             listener.close()
-            PIH.EVENT.on_log_command(internal_handler)
+            PIH.EVENT.on_event(internal_handler)
+            return DATA_HOLDER.result
 
         @staticmethod
         def waiting_for_mobile_helper_message_input(recipient: str, handler: Callable[[str, Callable[[None], None]], None]) -> None:
             def internal_handler(parameter_list: ParameterList, listener: ServiceListener) -> None:
-                message: WhatsAppMessage = PIH.DATA.EXTRACT.SERVICE_PARAMETER_LIST.whatsapp_message(parameter_list)
+                message: WhatsAppMessage = PIH.DATA.EXTRACT.EVENT.whatsapp_message(parameter_list)
                 if not DataTool.is_empty(message) and PIH.DATA.FORMAT.telephone_number(message.sender) == PIH.DATA.FORMAT.telephone_number(recipient):
                     handler(message.message, listener.close)
-            PIH.EVENT.on_log_command(internal_handler)
+            PIH.EVENT.on_event(internal_handler)
 
             
     class SERVICE:
 
-        command_map: dict[str, ServiceRoleDescription] = None
+        LONG_OPERATION_DURATION: int | None = None
+
+        EVENT_LISTENER_NAME_PREFIX: str = "_@@EventListener@@_"
+        SUPPORT_NAME_PREFIX: str = "_@@Support@@_"
+        command_map: dict[str, ServiceDescription] | None = None
+
+        class DATA_HOLDER:
+            long_operation_listeners: list[Callable[[None], None]] = []
+
+        @staticmethod
+        def call_listeners_on_long_operation() -> None:
+            for listener in PIH.SERVICE.DATA_HOLDER.long_operation_listeners:
+                listener()
+
+        @staticmethod
+        def start_listen_for_long_operation(listener: Callable[[None], None]) -> None:
+            PIH.SERVICE.DATA_HOLDER.long_operation_listeners.append(listener)
+
+        @staticmethod
+        def stop_listen_for_long_operation(listener: Callable[[None], None]) -> None:
+            PIH.SERVICE.DATA_HOLDER.long_operation_listeners.remove(listener)
+
+        @staticmethod
+        def call(role_or_information: ServiceRoles | ServiceInformationBase | None, service_command: ServiceCommands, parameters: Any | None = None, timeout: int | None = None, blocked: bool = True, long_operation_duration: int | None = None) -> str | None:
+            long_operation_duration = long_operation_duration or PIH.SERVICE.LONG_OPERATION_DURATION
+            class DATA_HOLDER:
+                stop_long_operation_action: bool = False
+            def long_operation_action() -> None:
+                time.sleep(long_operation_duration/1000)
+                if not DATA_HOLDER.stop_long_operation_action:
+                    PIH.SERVICE.call_listeners_on_long_operation()
+            if not DataTool.is_empty(long_operation_duration):
+                long_operation_thread: Thread = Thread(
+                    target=long_operation_action)
+                long_operation_thread.start()
+            def action() -> str | None:
+                result: str | None = RPC.call_service(role_or_information, service_command, parameters, timeout)
+                DATA_HOLDER.stop_long_operation_action = True
+                return result
+            if blocked:
+                return action()
+            else:
+                Thread(target=action).start()
+                return None
+
+        @staticmethod
+        def call_command(value: ServiceCommands, parameters: Any | None = None, timeout: int | None = None, blocked: bool = True, long_operation_duration: int | None = None) -> str | None:
+           return PIH.SERVICE.call(None, value, parameters, timeout, blocked, long_operation_duration)
+
+        @staticmethod
+        def get_support_host_list(role_or_information: ServiceRoles | ServiceInformationBase) -> list[str]:
+            return list(filter(lambda item: item.name.startswith(f"{PIH.SERVICE.SUPPORT_NAME_PREFIX}{ServiceRoles.description(role_or_information).name}"), PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP))
 
         class ADMIN:
 
+            SERVICE_INFORMATION_MAP: dict[ServiceInformationBase, ServiceInformation] = {}
+
+            @staticmethod
+            def change_host_on_local(role_or_information: ServiceRoles | ServiceInformationBase) -> None:
+                ServiceRoles.description(role_or_information).host = A.OS.host()
+
+            @staticmethod
+            def service_information_list() -> list[ServiceInformation]:
+                return DataTool.to_list(PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP)
+
             @staticmethod
-            def call(service_command: ServiceCommands, parameters: Any) -> str:
-                return RPC.call(service_command, parameters)
+            def kill_all(via_pskill: bool = False, local: bool = False) -> bool:
+                hosts: set[str] = set()
+                for server_role in A.CT_SR:
+                    host: str | None = A.CT_SR.description(server_role).host
+                    if not DataTool.is_empty(host):
+                        hosts.add(host)
+                def kill(host: str, local: bool, via_pskill: bool) -> None:
+                    if local:
+                        PIH.PSTOOLS.kill_python_process(host, via_pskill)
+                    else:
+                        PIH.ACTION.WORKSTATION.kill_python_process(host, via_pskill)
+                for host in hosts:
+                    if host != PIH.OS.host():
+                        kill(host, local, via_pskill)
+                for host in hosts:
+                    if host == PIH.OS.host():
+                        kill(host, local, via_pskill)
 
             @staticmethod
-            def subscribe_on(service_command: ServiceCommands, type: int = SubscribtionTypes.AFTER, name: str = None) -> bool:
-                return RPC.Service.service.subscribe_on(service_command, type, name)
+            def subscribe_on(service_command: ServiceCommands, type: int = SubscribtionTypes.ON_RESULT, name: str | None = None) -> bool:
+                return RPC.service.subscribe_on(service_command, type, name)
 
             @staticmethod
             def unsubscribe(service_command: ServiceCommands, type: int) -> bool:
-                return RPC.Service.service.unsubscribe(service_command, type)
+                return RPC.service.unsubscribe(service_command, type)
 
             @staticmethod
-            def create_developer_service_role_description(port: int = None) -> ServiceRoleDescription:
+            def create_developer_service_description(port: int = None) -> ServiceDescription:
                 if port is None or port == ServiceRoles.DEVELOPER.value.port:
                     return ServiceRoles.DEVELOPER.value
-                return ServiceRoleDescription(f"Developer{port}", host=CONST.HOST.DEVELOPER.NAME, port=CONST.RPC.PORT(port))
+                return ServiceDescription(f"Developer_{port}", host=CONST.HOST.DEVELOPER.NAME, port=CONST.RPC.PORT(port))
 
             @staticmethod
-            def develope(service_role: ServiceRoles, port: int = None) -> None:
-                developer_service_role_description: ServiceRoleDescription = PIH.SERVICE.ADMIN.create_developer_service_role_description(port)
-                service_role_description: ServiceRoleDescription = service_role.value
-                service_role_description.auto_restart = False
-                service_role_description.host = developer_service_role_description.host
-                service_role_description.port = developer_service_role_description.port
-
+            def create_support_service_or_master_service_description(master_service_desctiption: ServiceDescription, host: str | None = None) -> ServiceDescription:
+                if A.SRV.check_accessibility(master_service_desctiption):
+                    host = host or A.OS.host()
+                    if master_service_desctiption.host != host:
+                        port: int = PIH.SERVICE.create_port(master_service_desctiption)
+                        return ServiceDescription(
+                            name=":".join([f"{PIH.SERVICE.SUPPORT_NAME_PREFIX}{master_service_desctiption.name}", host]),
+                            description=f"Support service for {master_service_desctiption.name} on {host}",
+                            host=host,
+                            port=port,
+                            auto_restart=False)
+                return master_service_desctiption
+            
             @staticmethod
-            def isolate(service_role: ServiceRoles) -> None:
-                service_role_description: ServiceRoleDescription = service_role.value
-                service_role_description.isolated = True
+            def create_event_listener_service_description(host: str, port: int) -> ServiceDescription:
+                return ServiceDescription(
+                    name=":".join([PIH.SERVICE.EVENT_LISTENER_NAME_PREFIX, host, str(port)]),
+                    description="Subscriber",
+                    host=host,
+                    port=port,
+                    auto_start=False,
+                    auto_restart=False)
+
+            @staticmethod
+            def as_developer(service_role: ServiceRoles, port: int = None) -> ServiceDescription:
+                developer_service_description: ServiceDescription = PIH.SERVICE.ADMIN.create_developer_service_description(port)
+                description: ServiceDescription = ServiceRoles.description(service_role)
+                description.isolated = True
+                description.host = developer_service_description.host
+                description.port = developer_service_description.port
+                return description
+
+            @staticmethod
+            def isolate(role_or_information: ServiceRoles | ServiceInformationBase) -> ServiceDescription:
+                description: ServiceDescription = ServiceRoles.description(role_or_information)
+                description.isolated = True
+                #description.auto_restart = False
+                return description
 
             @staticmethod
-            def start(service_role_or_description: ServiceRoles | ServiceRoleDescription, check_if_started: bool = True, show_output: bool = False) -> bool:
-                service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
+            def start(role_or_information: ServiceRoles | ServiceInformationBase, check_if_started: bool = True, show_output: bool = True) -> bool | None:
+                description: ServiceDescription = ServiceRoles.description(role_or_information, True)
                 if check_if_started:
-                    if PIH.SERVICE.check_accessibility(service_role_description):
+                    if PIH.SERVICE.check_accessibility(description):
                         return None
-                remote_executor_command_list: list[str] = PIH.PSTOOLS.create_remote_process_executor_for_service(service_role_description)
+                remote_executor_command_list: list[str] = PIH.PSTOOLS.create_remote_process_executor_for_service(description, False)
                 service_file_path: str = None
-                if service_role_description.service_path is None:
+                if DataTool.is_empty(description.service_path):
                     service_file_path = os.path.join(
-                        CONST.FACADE.PATH, f"{service_role_description.name}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
+                        CONST.FACADE.PATH, f"{description.name}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
                 else:
                     service_file_path = os.path.join(
-                        service_role_description.service_path, PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
+                        description.service_path, PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
                 remote_executor_command_list.append(service_file_path)
-                #debug = False
-                remote_executor_command_list.append("False")
-                process_result = PIH.PSTOOLS.execute_command_list(
-                    remote_executor_command_list, show_output)
+                remote_executor_command_list.append("false")
+                process_result: CompletedProcess = PIH.PSTOOLS.execute_command_list(remote_executor_command_list, show_output)
                 returncode = process_result.returncode
                 if returncode == 2:
                     return False
-                service_role_description.pid = returncode
                 return True
 
             @staticmethod
-            def kill_via_pstools(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> bool | None:
-                service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
-                if PIH.SERVICE.check_accessibility(service_role_description):
-                    return PIH.PSTOOLS.kill_process(service_role_description.pid, PIH.PSTOOLS.as_host(PIH.SERVICE.get_host(service_role_description)))
-                return None
+            def kill(role_or_information: ServiceRoles | ServiceInformationBase, local: bool = True, via_taskkill: bool = True) -> bool | None:
+                information: ServiceInformation | None = PIH.SERVICE.get_information(role_or_information)
+                if DataTool.is_empty(information):
+                    return None
+                pid: int = information.pid
+                host: str = PIH.SERVICE.get_host(information)
+                if local:
+                    return PIH.PSTOOLS.kill_process(pid, host, via_taskkill)
+                return PIH.ACTION.WORKSTATION.kill_process(pid, host, via_taskkill)
             
             @staticmethod
-            def kill(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> bool: # | None:
-                service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
-                #if PIH.SERVICE.check_accessibility(service_role_description):
-                return PIH.PSTOOLS.kill_process_via_windows(service_role_description.pid, PIH.PSTOOLS.as_host(PIH.SERVICE.get_host(service_role_description)))
-                #return None
-            
-            @staticmethod
-            def serve(service_role_or_description: ServiceRoles | ServiceRoleDescription, call_handler: Callable[[str, ParameterList, Any], Any], isolate: bool = False, service_started_handler: Callable[[None], None] = None, depends_on_list: list[ServiceRoles | ServiceRoleDescription] = [], max_workers=None, stop_before: bool = False) -> RPC.Service:
-                if stop_before:
-                    if PIH.SERVICE.check_accessibility(service_role_or_description):
-                        PIH.SERVICE.ADMIN.stop(service_role_or_description)
-                service: RPC.Service = RPC.Service()
-                service.serve(service_role_or_description, call_handler, isolate, service_started_handler, depends_on_list, max_workers)
-
-            @staticmethod
-            def stop(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> None:
-                service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(
-                            service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
-                if PIH.SERVICE.check_accessibility(service_role_description):
-                    RPC.stop(service_role_description)  
-                    PIH.SERVICE.ADMIN.kill(service_role_description)   
-            
-            @staticmethod
-            def publish(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> bool:
-                role_descrption: ServiceRoleDescription = service_role_or_description if isinstance(
-                    service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
-                return PIH.ACTION.DATA_STORAGE.value(role_descrption)
-            
-            @staticmethod
-            def receive(name: str) -> ServiceRoleDescription:
-                return PIH.RESULT.DATA_STORAGE.value(name, ServiceRoleDescription)
-
-        @staticmethod
-        def check_accessibility(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> bool:
-            role_descrption: ServiceRoleDescription = service_role_or_description if isinstance(
-                    service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
-            return not DataTool.is_empty(PIH.SERVICE.ping(role_descrption))
-
-        @staticmethod
-        def ping(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> ServiceRoleInformation:
-            service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(
-                    service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
-            service_role_informaion: ServiceRoleInformation = RPC.ping(service_role_or_description)
-            if service_role_informaion is not None:
-                DataTool.fill_data_from_source(
-                    service_role_description, service_role_informaion)
-                service_role_informaion.subscribers = list(map(lambda item: DataTool.fill_data_from_source(
-                    Subscriber(), item), service_role_informaion.subscribers))
-            return service_role_informaion
+            def serve(role_or_information: ServiceRoles | ServiceInformationBase, 
+                      call_handler: Callable[[ServiceCommands, ParameterList], Any] | None = None, 
+                      starts_handler: Callable[[IService | None], None] | None = None, 
+                      max_workers: int | None = None, 
+                      stop_before: bool = True, 
+                      depends_on_list: list[ServiceDescription | ServiceRoles] | None = None, 
+                      isolate: bool = False,
+                      show_output: bool = True) -> None:
+                service_description: ServiceInformationBase = A.CT_SR.description(role_or_information)
+                if service_description.host_changabled and not A.D.contains(A.OS.host(), service_description.host):
+                    PIH.SERVICE.ADMIN.change_host_on_local(service_description)
+                elif isolate:
+                    PIH.SERVICE.ADMIN.isolate(service_description)
+                if stop_before and not service_description.isolated:
+                    if PIH.SERVICE.check_accessibility(service_description):
+                        PIH.SERVICE.ADMIN.stop(service_description)
+                def internal_start_handler(service: IService) -> None:
+                    if starts_handler is not None:
+                        if starts_handler.__code__.co_argcount == 1:
+                            starts_handler(service)
+                        else:
+                            starts_handler()
+                service: IService = RPC.create_service()
+                from inspect import signature
+                def internal_call_handler(command_name: str, parameter_list: ParameterList, context) -> Any | None:
+                    if not DataTool.is_empty(call_handler):
+                        sig = signature(call_handler)
+                        arg_count: int = len(sig.parameters) - ("self" in sig.parameters)
+                        if arg_count == 3:
+                            return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list, context)    
+                        return call_handler(EnumTool.get(ServiceCommands, command_name), parameter_list) 
+                    return None   
+                service.serve(service_description, internal_call_handler,
+                              internal_start_handler, max_workers, depends_on_list, show_output)
+
+            @staticmethod
+            def stop(role_or_information: ServiceRoles | ServiceInformationBase, check_on_started: bool = True, direct_call: bool = False) -> bool:
+                description: ServiceDescription = ServiceRoles.description(role_or_information)
+                if not check_on_started or PIH.SERVICE.check_accessibility(description):
+                    if PIH.SERVICE.is_service_as_listener(description) or direct_call:
+                        A.SRV.call(description, ServiceCommands.stop_service)
+                        return True
+                    service_information: ServiceInformationBase = DataTool.fill_data_from_source(
+                            ServiceInformationBase(), PIH.SERVICE.get_information(description))
+                    A.SRV.call(service_information,
+                                     ServiceCommands.stop_service)
+                    return True
+                return False
+
+            @staticmethod
+            def update_service_information(list: list[ServiceInformation], add: bool = True, overwrite: bool = False) -> None:
+                if overwrite:
+                    PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP = {}    
+                for item in list:
+                    if add:
+                        PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP[item] = item
+                    else:
+                        if item in PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP:
+                            del PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP[item]
+
+            @staticmethod
+            def validate(cached: bool = False, include_isolated: bool = False) -> tuple[list, list]:
+                if not cached:
+                    PIH.SERVICE.ADMIN.request_for_service_information_list()
+                service_information_list: list[ServiceInformation] = A.SRV_A.service_information_list()
+                if not include_isolated:
+                    service_information_list = list(filter(lambda item: not item.isolated, service_information_list)) 
+                if not DataTool.is_empty(service_information_list):
+                    length: int = len(service_information_list)
+                    with ThreadPoolExecutor(max_workers=length) as executor:
+                        future_to_bool = {executor.submit(
+                            PIH.SERVICE.check_accessibility, service_descroption): service_descroption for service_descroption in service_information_list}
+                        offline_service_list: list[ServiceInformation] = []
+                        for value in futures.as_completed(future_to_bool):
+                            if not value.result():
+                                service_information: ServiceInformation = future_to_bool[value]
+                                offline_service_list.append(service_information)
+                                service_information_list.remove(service_information)
+                                del PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP[service_information]
+                        service_description_list: list[ServiceDescription] = list(filter(lambda item: item.visible_for_admin, map(lambda item: A.CT_SR.description(item), A.CT_SR)))
+                        for service_description_item in service_description_list:
+                            if service_description_item not in service_information_list:
+                                offline_service_list.append(service_description_item)
+                        return offline_service_list, service_information_list
+                return [], []  
+
+            @staticmethod
+            def request_for_service_information_list() -> None:
+                PIH.SERVICE.ADMIN.update_service_information(list(map(PIH.DATA.EXTRACT.service_information, DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.get_service_information_table, ((RPC.service_information or A.CT_SR.STUB).name), )) or [])), True, True)
+                  
+        @staticmethod
+        def check_accessibility(role_or_information: ServiceRoles | ServiceInformationBase, cached: bool = False) -> bool:
+            return not DataTool.is_empty(PIH.SERVICE.get_information(role_or_information, cached))
         
         @staticmethod
-        def init() -> None:
-            if PIH.SERVICE.command_map is None:
-                PIH.SERVICE.command_map = {}
-                for service_role in ServiceRoles:
-                    service_role_description: ServiceRoleDescription = service_role.value
-                    for service_command in service_role_description.commands:
-                        PIH.SERVICE.command_map[service_command.name] = service_role_description
+        def is_service_as_listener(information: ServiceInformationBase) -> bool:
+            return information.name.find(PIH.SERVICE.EVENT_LISTENER_NAME_PREFIX) == 0
 
         @staticmethod
-        def get_role_description_by_command(value: ServiceCommands) -> ServiceRoleDescription:
+        def get_information(role_or_information: ServiceRoles | ServiceInformationBase, cached: bool = True) -> ServiceInformation | None:
+            service_information: ServiceInformationBase | None = ServiceRoles.description(
+                role_or_information)
+            #if PIH.SERVICE.is_service_as_listener(service_information):
+            #    return RPC.ping(service_information)
+            if DataTool.is_empty(PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP):
+                PIH.SERVICE.ADMIN.request_for_service_information_list()    
+            service_information = PIH.SERVICE.get_information_from_cache(
+                service_information)
+            if cached:
+                return service_information
+            if DataTool.is_empty(service_information):
+                return None
+            return RPC.ping(service_information)
+        
+        @staticmethod
+        def get_information_or_description(role_or_information: ServiceRoles | ServiceInformationBase) -> ServiceInformation | ServiceDescription:
+            return PIH.SERVICE.get_information(role_or_information) or ServiceRoles.description(role_or_information)
+        
+        @staticmethod
+        def get_information_from_cache(role_or_information: ServiceRoles | ServiceInformationBase) -> ServiceInformation | None:
+            description: ServiceDescription = ServiceRoles.description(role_or_information)
+            return PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP[description] if description in PIH.SERVICE.ADMIN.SERVICE_INFORMATION_MAP else None
+        
+        @staticmethod
+        def description_by_command(value: ServiceCommands) -> ServiceDescription | None:
+            if DataTool.is_empty(PIH.SERVICE.command_map):
+                PIH.SERVICE.command_map = {}
+                for service_role_item in ServiceRoles:
+                    description: ServiceDescription = ServiceRoles.description(service_role_item)
+                    for service_command_item in description.commands:
+                        service_command_item: ServiceCommands = service_command_item
+                        PIH.SERVICE.command_map[service_command_item.name] = description
             return PIH.SERVICE.command_map[value.name] if value.name in PIH.SERVICE.command_map else None
 
         @staticmethod
-        def get_host(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> str:
-            service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
-            if service_role_description.isolated:
-                service_role_description.host = PIH.OS.host()
-            return service_role_description.host
+        def get_host(role_or_information: ServiceRoles | ServiceInformationBase) -> str:
+            information: ServiceInformationBase | None = ServiceRoles.description(role_or_information)
+            if isinstance(information, ServiceDescription):
+                if not DataTool.is_empty(information.port):
+                    return information.host
+            return (PIH.SERVICE.get_information(role_or_information) or ServiceInformationBase()).host or information.host
 
         @staticmethod
-        def get_port(service_role_or_description: ServiceRoles | ServiceRoleDescription) -> str:
-            service_role_description: ServiceRoleDescription = service_role_or_description if isinstance(service_role_or_description, ServiceRoleDescription) else service_role_or_description.value
-            return service_role_description.port
+        def get_port(role_or_information: ServiceRoles | ServiceInformationBase) -> int | None:
+            information: ServiceInformationBase | None = ServiceRoles.description(role_or_information)
+            if isinstance(information, ServiceDescription):
+                if not DataTool.is_empty(information.port):
+                    return information.port
+            return (PIH.SERVICE.get_information(role_or_information) or ServiceInformationBase()).port or information.port
+        
+        @staticmethod
+        def create_port(role_or_information: ServiceRoles | ServiceInformationBase) -> int: 
+            return ServiceRoles.description(role_or_information).port or NetworkTool.next_free_port()
+        
+        @staticmethod
+        def create_host(role_or_information: ServiceRoles | ServiceInformationBase) -> int: 
+            description: ServiceDescription = ServiceRoles.description(role_or_information)
+            return PIH.OS.host() if description.isolated or DataTool.is_empty(description.host) else description.host
 
     class PATH(PATHS, PathTool):
 
         @staticmethod
+        def get_host(value: str) -> str:
+            return PIH.DATA.FORMAT.host(value, reverse=True)
+
+        @staticmethod
         def resolve(value: str) -> str:
             if value[0] == "{" and value[-1] == "}":
                 value = value[1: -1]
             return PathTool.resolve(value, PIH.OS.host())
         
+        @staticmethod
         def join(path: str, *paths) -> str:
             return os.path.join(path, *paths)
         
         class QR_CODE:
 
             @staticmethod
             def polibase_person_card_registry_folder(name: str) -> str:
@@ -2139,40 +2735,50 @@
 
             @staticmethod
             def mobile_helper_command(name: str) -> str:
                 name = PIH.DATA.FORMAT.mobile_helper_command(name)
                 return os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(name, FILE.EXTENSION.PNG)))
   
 
-    class DATA(DataTool, StringTool, ListTool, DateTimeTool, EnumTool):
+    class DATA(DataTool, StringTool, ListTool, DateTimeTool, EnumTool, FullNameTool):
+
+        class MATERIALIZED_RESOURCES:
+
+            @staticmethod
+            def find(name: str) -> list[MATERIALIZED_RESOURCES.TYPES]:
+                result: list[SETTINGS] = []
+                for item in MATERIALIZED_RESOURCES.TYPES:
+                    if StringTool.contains(item.name, name) or StringTool.contains(item.value.key_name, name):
+                        result.append(item)
+                return result
+
+            @staticmethod
+            def get_count(type: MATERIALIZED_RESOURCES.TYPES) -> int:
+                return PIH.RESULT.DATA_STORAGE.value(type.name, None, MATERIALIZED_RESOURCES.NAME).data
+
+            @staticmethod
+            def set_count(type: MATERIALIZED_RESOURCES.TYPES, value: int) -> bool:
+                return PIH.ACTION.DATA_STORAGE.value(value, type.name, MATERIALIZED_RESOURCES.NAME)
 
         @staticmethod
         def save_base64_as_image(path: str, content: str) -> bool:
             with open(path, "wb") as file:
                 file.write(base64.decodebytes(bytes(content, "utf-8")))
                 return True 
             return False
 
         @staticmethod
         def uuid() -> str:
             return str(uuid.uuid4().hex)
-        
-        @staticmethod
-        def create_email(login: str) -> str:
-            return "@".join((login, CONST.SITE_ADDRESS))
-
-        @staticmethod
-        def create_user_principal_name(login: str) -> str:
-            return "@".join((login, AD.DOMAIN_MAIN))
 
         class USER:
 
             @staticmethod
-            def by_login(value: str) -> User:
-                return PIH.RESULT.USER.by_login(value).data
+            def by_login(value: str, active: bool | None = None, cached: bool | None = None) -> User:
+                return PIH.RESULT.USER.by_login(value, active, cached).data
 
             @staticmethod
             def by_name(value: str) -> User:
                 return PIH.RESULT.USER.by_name(value).data
 
         class MARK:
 
@@ -2195,57 +2801,89 @@
             @staticmethod
             def users_by_dn(data: list[User], dn: str) -> list:
                 return list(filter(lambda x: x.distinguishedName.find(dn) != -1, data))
 
         class EXTRACT:
 
             @staticmethod
-            def date(value: str, format: str) -> datetime | None:
+            def polibase_person(value: dict) -> PolibasePerson:
+                polibase_person: PolibasePerson = DataTool.fill_data_from_source(PolibasePerson(), value)
+                polibase_person.Birth = DateTimeTool.datetime_from_string(polibase_person.Birth)
+                polibase_person.registrationDate = DateTimeTool.datetime_from_string(polibase_person.registrationDate )
+                return polibase_person
+
+            @staticmethod
+            def date(value: str | None, format: str) -> datetime | None:
+                if DataTool.is_empty(value):
+                    return None
                 result: datetime | None = None
                 try:
-                    result = DateTimeTool.from_string(value, format)
+                    result = DateTimeTool.datetime_from_string(value, format)
                 except ValueError as error:
-                    date_extract_pattern = "[0-9]{1,2}\\.[0-9]{1,2}\\.[0-9]{4}"
+                    date_extract_pattern: str = "[0-9]{1,2}\\.[0-9]{1,2}\\.[0-9]{4}"
                     date_list: list[str] = re.findall(date_extract_pattern, value)
                     if not DataTool.is_empty(date_list):
                         result = PIH.DATA.EXTRACT.date(date_list[0], format)
                 return result
             
             @staticmethod
-            def wappi_telephone_number(value: any) -> str:
+            def service_information(value: dict | ServiceInformation) -> ServiceInformation:
+                service_information: ServiceInformation = A.D.fill_data_from_source(ServiceInformation(), value) if isinstance(value, dict) else value
+                if not DataTool.is_empty(service_information.subscribtions):
+                    service_information.subscribtions = DataTool.fill_data_from_list_source(Subscribtion, service_information.subscribtions)   
+                return service_information
+
+            @staticmethod
+            def wappi_telephone_number(value: Any) -> str:
                 if isinstance(value, str):
                     return PIH.DATA.FORMAT.telephone_number(value.split(CONST.MESSAGE.WHATSAPP.WAPPI.CONTACT_SUFFIX)[0])
                 if isinstance(value, dict):
                     return PIH.DATA.FORMAT.telephone_number(value["user"])
-
-            class SERVICE_PARAMETER_LIST:
+                
+            class EVENT:
 
                 @staticmethod
-                def whatsapp_message(parameter_list: ParameterList) -> WhatsAppMessage:
-                    result: bool = parameter_list.next()
-                    message: WhatsAppMessage = None
-                    if result:
-                        message_parameters: list[Any] = parameter_list.next()
-                        message_command: LogCommands = LogCommands.WHATSAPP_MESSAGE_RECEIVED
-                        if EnumTool.get(LogCommands, message_parameters[0]) == message_command:
-                            param_item: ParamItem = message_command.value.params[0]
-                            message = DataTool.fill_data_from_source(
-                                WhatsAppMessage(), message_parameters[1][param_item.name])
+                def whatsapp_message(parameter_list: ParameterList) -> WhatsAppMessage | None:
+                    allow: bool = PIH.DATA.EXTRACT.subscribtion_result(parameter_list).result
+                    message: WhatsAppMessage | None = None
+                    if allow:
+                        event, parameters = PIH.DATA.EXTRACT.EVENT.with_parameters(parameter_list)
+                        if event == Events.WHATSAPP_MESSAGE_RECEIVED:
+                            message = DataTool.fill_data_from_source(WhatsAppMessage(), parameters[0])
                     return message
                 
                 @staticmethod
-                def log_command_parameters(parameter_list: ParameterList) -> tuple[LogCommands, list[Any]]:
-                    log_command_content: dict[str, Any] = parameter_list.list[1]
-                    log_command: LogCommands = EnumTool.get(LogCommands, log_command_content[0])
-                    log_command_parameters: dict[str, Any] = log_command_content[1]
-                    result: list[Any] = []
-                    if not A.D_C.empty(log_command.value.params):
-                        for log_command_parameters_description in log_command.value.params:
-                            result.append(log_command_parameters[log_command_parameters_description.name])
-                    return log_command, result
+                def action(parameters: dict[str, Any]) -> ActionWasDone:
+                    action: ActionWasDone = DataTool.fill_data_from_source(ActionWasDone(), PIH.EVENT.get_parameter(Events.ACTION_WAS_DONE, parameters), copy_by_index=True)
+                    action.action = EnumTool.get(Actions, action.action)
+                    return action
+                
+                @staticmethod
+                def get(parameter_list: ParameterList) -> Events:
+                    event_content: Any | list[Any] = parameter_list.list[0] if PIH.DATA.CHECK.has_subscribtion_result(parameter_list) else parameter_list.list
+                    return EnumTool.get(Events, event_content[0])
+                
+                @staticmethod
+                def with_parameters(parameter_list: ParameterList) -> tuple[Events, list[Any]]:
+                    event_content: Any | list[Any] = parameter_list.list[0] if PIH.DATA.CHECK.has_subscribtion_result(parameter_list) else parameter_list.list
+                    event: Events = EnumTool.get(Events, event_content[0])
+                    event_content_parameters: dict[str, Any] = event_content[1]
+                    parameters: list[Any] = []
+                    if not A.D_C.empty(event.value.params):
+                        for event_parameters_description in event.value.params:
+                            parameters.append(event_content_parameters[event_parameters_description.name])
+                    return event, parameters
+                
+            @staticmethod
+            def subscribtion_result(parameter_list: ParameterList) -> SubscribtionResult | None:
+                return None if DataTool.is_empty(parameter_list.list) or not PIH.DATA.CHECK.has_subscribtion_result(parameter_list) else DataTool.fill_data_from_source(SubscribtionResult(), parameter_list.list[-1])
+            
+            @staticmethod
+            def parameter_list(parameter_list: ParameterList) -> ParameterList:
+                return ParameterList(parameter_list.get()) if PIH.DATA.CHECK.has_subscribtion_result(parameter_list) else parameter_list
 
             @staticmethod
             def email(value: str) -> str:
                 emails: list[str] = re.findall(
                     r"[A-Za-z0-9_%+-.]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,5}", value)
                 if len(emails) > 0:
                     return emails[0]
@@ -2301,15 +2939,15 @@
 
             @staticmethod
             def group_id(mark_object: dict) -> str:
                 return PIH.DATA.EXTRACT.parameter(mark_object, FIELD_NAME_COLLECTION.GROUP_ID)
 
             @staticmethod
             def as_full_name(mark_object: dict) -> FullName:
-                return FullNameTool.from_string(PIH.DATA.EXTRACT.full_name(mark_object))
+                return FullNameTool.fullname_from_string(PIH.DATA.EXTRACT.full_name(mark_object))
 
             @staticmethod
             def full_name(mark_object: dict) -> str:
                 return PIH.DATA.EXTRACT.parameter(mark_object, FIELD_NAME_COLLECTION.FULL_NAME)
 
             @staticmethod
             def person_id(mark_object: dict) -> str:
@@ -2319,15 +2957,15 @@
             def mark_id(mark_object: dict) -> str:
                 return PIH.DATA.EXTRACT.parameter(mark_object, FIELD_NAME_COLLECTION.MARK_ID)
 
             @staticmethod
             def description(object: dict) -> str:
                 result = PIH.DATA.EXTRACT.parameter(
                     object, FIELD_NAME_COLLECTION.DESCRIPTION)
-                if isinstance(result, Tuple) or isinstance(result, list):
+                if isinstance(result, tuple) or isinstance(result, list):
                     return result[0]
 
             @staticmethod
             def container_dn(user_object: dict) -> str:
                 return PIH.DATA.EXTRACT.container_dn_from_dn(PIH.DATA.EXTRACT.dn(user_object))
 
             @staticmethod
@@ -2335,59 +2973,153 @@
                 return ",".join(dn.split(",")[1:])
             
         class CONVERT:
 
             @staticmethod
             def settings_to_datetime(item: SETTINGS, format: str = CONST.SECONDLESS_TIME_FORMAT) -> datetime | list[datetime]:
                 settings_value: str | list[str] = A.S.get(item)
-                return  PIH.DATA.CONVERT.settings_to_datetime_list(item, format) if isinstance(settings_value, list) else DateTimeTool.from_string(settings_value, format)
+                return  PIH.DATA.CONVERT.settings_to_datetime_list(item, format) if isinstance(settings_value, list) else DateTimeTool.datetime_from_string(settings_value, format)
             
             @staticmethod
             def settings_to_datetime_list(item: SETTINGS, format: str = CONST.SECONDLESS_TIME_FORMAT) -> list[datetime]:
-                return list(map( lambda item: DateTimeTool.from_string(item, format), A.S.get(item)))
+                return list(map( lambda item: DateTimeTool.datetime_from_string(item, format), A.S.get(item)))
 
             @staticmethod
             def file_to_base64(path: str) -> str | None:
-                with open(path, "rb") as file:
-                    return PIH.DATA.CONVERT.bytes_to_base64(file.read())
+                while True:
+                    try:
+                        with open(path, "rb") as file:
+                            return PIH.DATA.CONVERT.bytes_to_base64(file.read())
+                    except Exception:
+                        pass
                 return None
                 
             @staticmethod
             def bytes_to_base64(value: bytes) -> str:
                 return PIH.DATA.CONVERT.bytes_to_string(PIH.DATA.CONVERT.to_base64(value))
             
             @staticmethod
             def to_base64(value: Any) -> str:
                 return base64.b64encode(value)
 
             @staticmethod 
             def bytes_to_string(value: bytes) -> str:
-                return value.decode('utf-8')
-            
+                return value.decode("utf-8")
             
         class CHECK:
 
             @staticmethod
-            def by_secondless_time(value_datetime: datetime, value_str: str) -> bool:
-                return False if DataTool.is_empty(value_str) else DateTimeTool.is_equal_by_time(value_datetime, DateTimeTool.from_string(value_str, CONST.SECONDLESS_TIME_FORMAT)) 
+            def polibase_person_has_new_barcode_format(polibase_person: PolibasePerson) -> bool:
+                return not (DataTool.is_empty(polibase_person.barcode) or polibase_person.barcode.find(CONST.POLIBASE.BARCODE.NEW_PREFIX) == -1)
+
+            @staticmethod
+            def polibase_person_barcode(value: BarcodeInformation) -> bool:
+                data: int | None = None
+                try:
+                    data = int(value.data)
+                except ValueError:
+                    return False
+                return value.type == CONST.POLIBASE.BARCODE.ACTUAL_FORMAT and data > CONST.POLIBASE.PERSON_MINIMAL_PIN
+
+            @staticmethod
+            def has_subscribtion_result(parameter_list: ParameterList) -> bool:
+                return DataTool.fill_data_from_source(SubscribtionResult(), parameter_list.list[-1]).checker
+            
+            @staticmethod
+            def by_secondless_time(value_datetime: datetime, value_str: str | None) -> bool:
+                return False if DataTool.is_empty(value_str) else DateTimeTool.is_equal_by_time(value_datetime, DateTimeTool.datetime_from_string(value_str, CONST.SECONDLESS_TIME_FORMAT)) 
             
             @staticmethod
             def empty(value) -> bool:
                 return DataTool.is_empty(value)
 
             @staticmethod
             def decimal(value: int | str) -> bool:
                 return isinstance(value, int) or (isinstance(value, str) and value.isdecimal())
 
+            class INDICATIONS:
+
+                @staticmethod
+                def chiller_value_actual(value_container: ChillerIndicationsValueContainer) -> bool:
+                    return (DateTimeTool.now() - DateTimeTool.datetime_from_string(value_container.timestamp, CONST.ISO_DATETIME_FORMAT)).total_seconds() // 60 <= INDICATIONS.CHILLER.ACTUAL_VALUES_TIME_DELTA_IN_MINUTES
+
+                @staticmethod
+                def chiller_value_valid(value: ChillerIndicationsValue) -> bool:
+                    return not DataTool.is_empty(value.temperature)
+
         class FORMAT:
 
             @staticmethod
-            def by_name(value: str, data: Any) -> str | None:
+            def format(value: str) -> str:
+                fileds: list[str] = [name for _, name, _, _ in Formatter().parse(value) if name]
+                my_fields: list[str] = DataTool.to_list(DATA.FORMATTER)
+                formatter: dict[str, str] = {}
+                for field_item in fileds:
+                    if field_item in my_fields:
+                       formatter[field_item] = PIH.DATA.FORMAT.by_formatter_name(field_item, None)
+                if DataTool.is_empty(formatter):
+                    return value
+                return value.format(**formatter)
+
+            @staticmethod
+            def index(value: int) -> str:
+                return str(value + 1) if value > 0 else ""
+                      
+            @staticmethod
+            def user_principal_name(login: str) -> str:
+                return "@".join((login, AD.DOMAIN_MAIN))
+
+            @staticmethod
+            def as_string(value: Any, escaped_string: bool = False, mapper: Callable[[Any], str] | None = None) -> str:
+                result: str = None
+                if isinstance(value, Enum):
+                    result = value.name
+                else:
+                    result = str(value)
+                if escaped_string:
+                    if isinstance(value, (str, datetime, Enum)):
+                        result = f"'{result}'"
+                    if isinstance(value, dict):
+                        result = f"'{DataTool.represent(value, False)}'"
+                return DataTool.check_not_none(mapper, lambda: mapper(result), result)
+                
+            @staticmethod
+            def host(value: str, reverse: bool = False) -> str:
+                host_start: str = r"\\"
+                if reverse:
+                    if value.startswith(host_start):
+                        value = value[len(host_start):]
+                    index: int = value.find("\\")
+                    if index >= 0:
+                        return value[0: index]
+                    return value
+                return ("" if value.startswith(host_start) else host_start) + value 
+
+            @staticmethod
+            def get_chiller_indications_value_image_name(datetime: datetime | str) -> str:
+                if isinstance(datetime, str):
+                    datetime = PIH.DATA.datetime_from_string(datetime, CONST.ISO_DATETIME_FORMAT)
+                return PIH.PATH.replace_prohibited_symbols_from_path_with_symbol(PIH.DATA.datetime_to_string(datetime, A.CT.DATETIME_FORMAT))
+
+            @staticmethod
+            def by_formatter_name(value: Enum | str , data: Any | None) -> str | None:
+                if isinstance(value, str):
+                    value = A.D.get(DATA.FORMATTER, value)
                 if value == DATA.FORMATTER.MY_DATETIME:
                     return PIH.DATA.FORMAT.datetime(data)
+                if value == DATA.FORMATTER.MY_DATE:
+                    return PIH.DATA.FORMAT.date(data)
+                if value == DATA.FORMATTER.CHILLER_FILTER_COUNT:
+                    return str(PIH.DATA.MATERIALIZED_RESOURCES.get_count(MATERIALIZED_RESOURCES.TYPES.CHILLER_FILTER_COUNT))
+                if value == DATA.FORMATTER.CHILLER_INDICATIONS_VALUE_INDICATORS:
+                    result_list: list[str] = [] 
+                    for index in range(len(INDICATIONS.CHILLER.INDICATOR_NAME)):
+                        if BM.has_index(data, index):
+                            result_list.append(f"{A.CT_V.BULLET} {INDICATIONS.CHILLER.INDICATOR_NAME[index]}")
+                    return "\n\n" + "\n".join(result_list) + "\n"
                 return None
 
             @staticmethod
             def polibase_person_card_registry_folder(value: str) -> str:
                 return value.upper()
 
             @staticmethod
@@ -2399,25 +3131,25 @@
                 return PIH.DATA.FORMAT.whatsapp_send_message_to(PIH.DATA.FORMAT.telephone_number_international(PIH.DATA.TELEPHONE_NUMBER.it_administrator()), f"{PIH.NAME} {value}".replace(" ", "+"))
             
             @staticmethod
             def whatsapp_send_message_to(telephone_number: str, message: str) -> str:
                 return CONST.MESSAGE.WHATSAPP.SEND_MESSAGE_TO_TEMPLATE.format(telephone_number, message)
 
             @staticmethod
-            def string(value: str) -> str:
+            def string(value: str | None) -> str:
                 return ("" or value).lower().replace('"', '')
             
             @staticmethod
             def telephone_number(value: str, prefix: str = CONST.TELEPHONE_NUMBER_PREFIX) -> str:
-                if DataTool.is_empty(value):
+                if DataTool.is_empty(value) or value.endswith(CONST.MESSAGE.WHATSAPP.GROUP_SUFFIX):
                     return value
                 if prefix != CONST.TELEPHONE_NUMBER_PREFIX:
                     value = value[value.find(prefix):]
                 src_value: str = value
-                if value is not None and len(value) > 0:
+                if not DataTool.is_empty(value):
                     value = re.sub("[\-\(\) ]", "", value)
                     if value.startswith(prefix):
                         value = value[len(prefix):]
                     if len(value) == 0:
                         return src_value
                     value = prefix + \
                         (value[1:] if (value[0] ==
@@ -2432,15 +3164,20 @@
                     return src_value
 
             @staticmethod
             def telephone_number_international(value: str) -> str:
                 return PIH.DATA.FORMAT.telephone_number(value, CONST.INTERNATIONAL_TELEPHONE_NUMBER_PREFIX)
 
             @staticmethod
-            def email(value: str) -> str:
+            def email(value: str, add_default_domain: bool = False, remove_restricted_symbols: bool = False) -> str:
+                if add_default_domain and value.find("@") == -1:
+                    return PIH.DATA.FORMAT.email("@".join((value, CONST.SITE_ADDRESS)))
+                if remove_restricted_symbols:
+                    for char in "\"(),:;<>[\\]":
+                        value = value.replace(char, "")
                 return value.lower()
 
             @staticmethod
             def name(value: str, remove_non_alpha: bool = False, name_part_minimal_length: int | None = None) -> str:
                 name_part_list: list[str] = list(
                     filter(lambda item: len(item) > (0 if name_part_minimal_length is None else name_part_minimal_length - 1), value.split(" ")))
                 if len(name_part_list) == 1:
@@ -2468,21 +3205,35 @@
                     if (pow(2, count) & uac) != 0:
                         result.append(item)
                 return result
             
             @staticmethod
             def description(value: str) -> str:
                 return (value.split("|")[0]).rstrip()
-            
-            def datetime(iso_datetime_string: str) -> str:
-                return DateTimeTool.datetime_to_string(datetime.fromisoformat(iso_datetime_string), CONST.MY_DATE_FORMAT)
+             
+            @staticmethod
+            def to_date(value: str) -> str:
+                value = value.strip()
+                value = value.replace("/", CONST.DATE_PART_DELIMITER)
+                value = value.replace(",", CONST.DATE_PART_DELIMITER)
+                value = value.replace(" ", CONST.DATE_PART_DELIMITER)
+                return value
+
+            @staticmethod
+            def date(iso_datetime_value: str | datetime) -> str:
+                return DateTimeTool.datetime_to_string(datetime.fromisoformat(iso_datetime_value) if isinstance(iso_datetime_value, str) else iso_datetime_value, CONST.DATE_FORMAT)
+
+            @staticmethod
+            def datetime(iso_datetime_value: str | datetime) -> str:
+                return DateTimeTool.datetime_to_string(iso_datetime_value if isinstance(iso_datetime_value, datetime) else datetime.fromisoformat(iso_datetime_value), CONST.DATETIME_FORMAT)
+          
 
         class TELEPHONE_NUMBER:
 
-            wappi_profile_TO_TELEPHONE_NUMBER_MAP: dict = None
+            wappi_profile_to_telephone_number_map: dict = None
 
             @staticmethod
             def all(active: bool = True) -> list[str]:
                 def filter_function(user: User) -> str:
                     return user.telephoneNumber is not None
                 def map_function(user: User) -> str:
                     return PIH.DATA.FORMAT.telephone_number(user.telephoneNumber)
@@ -2490,37 +3241,37 @@
 
             @staticmethod
             def it_administrator() -> str:
                 return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.ADMINISTRATOR)
 
             @staticmethod
             def call_centre_administrator() -> str:
-                return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.CALL_CENTRE_ADMINISTRATOR)
+                return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.USER.CALL_CENTRE_ADMINISTRATOR)
 
             @staticmethod
             def marketer() -> str:
-                return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.MARKETER)
+                return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.USER.MARKETER)
 
             @staticmethod
-            def for_wappi(value: Any) -> str:
+            def for_wappi(value: Any) -> str | None:
                 WP = CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE
                 value = EnumTool.get_by_value_or_key(WP, value)
-                map: dict = PIH.DATA.TELEPHONE_NUMBER.wappi_profile_TO_TELEPHONE_NUMBER_MAP
-                if map is None:
+                map: dict = PIH.DATA.TELEPHONE_NUMBER.wappi_profile_to_telephone_number_map
+                if DataTool.is_none(map):
                     map = {
                         WP.CALL_CENTRE: PIH.DATA.TELEPHONE_NUMBER.call_centre_administrator(),
                         WP.IT: PIH.DATA.TELEPHONE_NUMBER.it_administrator(),
                         WP.MARKETER: PIH.DATA.TELEPHONE_NUMBER.marketer(),
                     }
-                    PIH.DATA.TELEPHONE_NUMBER.wappi_profile_TO_TELEPHONE_NUMBER_MAP = map
-                return map[value] if value in map else None
+                    PIH.DATA.TELEPHONE_NUMBER.wappi_profile_to_telephone_number_map = map
+                return DataTool.check_in(map, value)
 
             @staticmethod
-            def by_login(value: str, format: bool = True) -> str:
-                result: str = PIH.DATA.USER.by_login(value).telephoneNumber
+            def by_login(value: str, format: bool = True, active: bool = True, cached: bool = True) -> str:
+                result: str = PIH.DATA.USER.by_login(value, active, cached).telephoneNumber
                 return PIH.DATA.FORMAT.telephone_number(result) if format else result
 
             @staticmethod
             def by_workstation_name(value: str) -> str:
                 workstation: Workstation = PIH.RESULT.WORKSTATION.by_name(value).data
                 return PIH.DATA.TELEPHONE_NUMBER.by_login(workstation.samAccountName)
 
@@ -2537,38 +3288,38 @@
                 return PIH.DATA.FORMAT.telephone_number(result) if format else result
 
             @staticmethod
             def by_full_name(value: Any, format: bool = True) -> str:
                 value_string: str = None
                 if isinstance(value, str):
                     value_string = value
-                    value = FullNameTool.from_string(value)
+                    value = FullNameTool.fullname_from_string(value)
                 else:
-                    value_string = FullNameTool.to_string(value)
+                    value_string = FullNameTool.fullname_to_string(value)
                 telephone_number: str = PIH.RESULT.MARK.by_full_name(
                     value_string, True).data.telephoneNumber
                 if PIH.CHECK.telephone_number(telephone_number):
                     return PIH.DATA.FORMAT.telephone_number(telephone_number) if format else telephone_number
                 telephone_number = PIH.RESULT.USER.by_full_name(
                     value_string, True).data.telephoneNumber
                 if PIH.CHECK.telephone_number(telephone_number):
                     return PIH.DATA.FORMAT.telephone_number(telephone_number) if format else telephone_number
                 details: str = f"Телефон для {value_string} не найден"
                 raise NotFound(details)
 
         class POLIBASE:
 
             @staticmethod
-            def person_by_pin(value: int, test: bool = None) -> PolibasePerson:
+            def person_by_pin(value: int, test: bool | None = None) -> PolibasePerson:
                 return PIH.RESULT.POLIBASE.person_by_pin(value, test).data
 
             @staticmethod
-            def duplicate_persons_by_person(person: PolibasePerson, check_birth: bool = True) -> list[PolibasePerson]:
+            def duplicate_persons_by_person(person: PolibasePerson, check_for_birth: bool = True) -> list[PolibasePerson]:
                 def check_function(check_person: PolibasePerson) -> bool:
-                    return check_person.pin != person.pin and (not check_birth or check_person.Birth == person.Birth)
+                    return check_person.pin != person.pin and (not check_for_birth or check_person.Birth == person.Birth)
                 return ResultTool.get_first_element(ResultTool.filter(PIH.RESULT.POLIBASE.persons_by_full_name(person.FullName), lambda item: check_function(item)))
             
             @staticmethod
             def unique_by_telephone(value: str) -> PolibasePerson:
                 value = PIH.DATA.FORMAT.telephone_number(value)
                 def check_function(check_person: PolibasePerson) -> bool:
                     return PIH.DATA.FORMAT.telephone_number(check_person.telephoneNumber) == value
@@ -2597,74 +3348,102 @@
 
         @staticmethod
         def get_pid() -> int:
             return os.getppid()
 
     class RESULT(ResultTool):
 
+        class EVENTS:
+
+           @staticmethod
+           def get(value: Events, parameters: dict | None = None) -> Result[list[EventDS]]:
+                def extractor(data: Any) -> EventDS:
+                    result: EventDS = DataTool.fill_data_from_source(EventDS(), data)
+                    #from json string to python object
+                    result.parameters = DataTool.rpc_unrepresent(result.parameters)
+                    if isinstance(result.timestamp, str):
+                        result.timestamp = DateTimeTool.datetime_from_string(result.timestamp)
+                    return result
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_event, EventDS(value.name, PIH.EVENT.BULDER.create_parameters_map(value, parameters or {}, check_for_parameters_count = False))), extractor)
+
+        class NOTES:
+    
+            @staticmethod
+            def by_name(name: str) -> Result[Note]:
+                id: str = DataTool.rpc_unrepresent(PIH.SERVICE.call_command(
+                    ServiceCommands.get_gkeep_item_id, (name, )))
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_note, id), Note)
+
         class SSH:
 
             @staticmethod
             def execute(command: str, host: str, username: str | None = None, password: str | None = None) -> Result[list[str]]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.execute_ssh_command, (command, host, username, password)))
+                    PIH.SERVICE.call_command(ServiceCommands.execute_ssh_command, (command, host, username, password)))
 
             @staticmethod
             def get_certificate_information(host: str, username: str | None = None, password: str | None = None) -> Result[str | None]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.get_certificate_information, (host, username, password)))
+                    PIH.SERVICE.call_command(ServiceCommands.get_certificate_information, (host, username, password)))
             
             @staticmethod
             def get_unix_free_space_information_by_drive_name(drive_name: str, host: str, username: str | None = None, password: str | None = None) -> Result[str | None]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.get_unix_free_space_information_by_drive_name, (drive_name, host, username, password)))
+                    PIH.SERVICE.call_command(ServiceCommands.get_unix_free_space_information_by_drive_name, (drive_name, host, username, password)))
 
         class DATA_STORAGE:
 
             @staticmethod
-            def value(name: str, class_type: T, section: str = None) -> Result[T]:
+            def value(name: str, class_type_holder: T | Callable[[Any], T] | None, section: str = None) -> Result[T]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.get_storage_value, (name, section)), class_type)
+                    PIH.SERVICE.call_command(ServiceCommands.get_storage_value, (name, section)), class_type_holder)
             
             @staticmethod
             def ogrn(code: str) -> Result[OGRN]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.get_ogrn_value, (code, )), OGRN)
+                    PIH.SERVICE.call_command(ServiceCommands.get_ogrn_value, (code, )), OGRN)
             
             @staticmethod
             def fms_unit_name(code: str) -> Result[str]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.get_fms_unit_name, (code, )))
+                    PIH.SERVICE.call_command(ServiceCommands.get_fms_unit_name, (code, )))
 
         class MESSAGE:
 
             class DELAYED:
 
                 @staticmethod
-                def get(search_condition: MessageSearchCritery = None, take_to_work: bool = False) -> Result[list[DelayedMessageDS]]:
+                def get(search_condition: MessageSearchCritery | None = None, take_to_work: bool = False) -> Result[list[DelayedMessageDS]]:
                     return DataTool.to_result(
-                        RPC.call(ServiceCommands.search_delayed_messages, (search_condition, take_to_work)), DelayedMessageDS)
+                        PIH.SERVICE.call_command(ServiceCommands.search_delayed_messages, (search_condition, take_to_work)), DelayedMessageDS)
+
+        class RECOGNIZE:
+
+            @staticmethod
+            def barcodes_information(file_path: str, get_only_first_barcode: bool = False, log_level: int = 0) -> Result[list[list[BarcodeInformation]]]:
+                def extractor(data: list[dict[str, Any]]) -> list[BarcodeInformation]:
+                    return list(map(lambda item: DataTool.fill_data_from_source(BarcodeInformation(), item), data))
+                return DataTool.to_result(
+                        PIH.SERVICE.call_command(ServiceCommands.get_barcode_list_information, (file_path, get_only_first_barcode, log_level)), extractor)
 
         class RESOURCES:
 
             @staticmethod
-            def get_status_list(checkable_section_list: list[CheckableSections] = None, force_update: bool = False, all: bool = False) -> Result[list[ResourceStatus]]:
-                def get_type(data: dict) -> ResourceStatus:
-                    if "check_certificate_status" in data:
-                        return SiteResourceStatus()
-                    return ResourceStatus()
-                return DataTool.to_result(RPC.call(ServiceCommands.get_resource_status_list, (None if DataTool.is_empty(checkable_section_list) else list(map(lambda item: item.name, checkable_section_list)), force_update, all)), get_type)
+            def get_status_list(checkable_section_list: list[CheckableSections] | None = None, force_update: bool = False, all: bool = False) -> Result[list[ResourceStatus]]:
+                def fill_data(data: dict) -> ResourceStatus:
+                    return DataTool.fill_data_from_source(SiteResourceStatus() if "check_certificate_status" in data else ResourceStatus(), data)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_resource_status_list, (None if DataTool.is_empty(checkable_section_list) else list(map(lambda item: item.name, checkable_section_list)), force_update, all)), fill_data)
 
             @staticmethod
             def get_resource_status_list(force_update: bool = False, all: bool = False) -> Result[list[ResourceStatus]]:
                 return PIH.RESULT.RESOURCES.get_status_list([CheckableSections.RESOURCES], force_update, all)
 
             @staticmethod
             def get_status(checkable_section_list: list[CheckableSections], resource_desription_or_address: Any, force: bool = False) -> ResourceStatus:
-                address: str = None
+                address: str | None = None
                 if isinstance(resource_desription_or_address, ResourceDescription):
                     address = resource_desription_or_address.address
                 elif isinstance(resource_desription_or_address, str):
                     address = resource_desription_or_address
                 if not DataTool.is_empty(address):
                     resource_list: list[ResourceStatus] = PIH.RESULT.RESOURCES.get_status_list(checkable_section_list, force).data
                     for item in resource_list:
@@ -2675,68 +3454,66 @@
             @staticmethod
             def get_resource_status(resource_desription_or_address: Any, force: bool = False) -> ResourceStatus:
                 return PIH.RESULT.RESOURCES.get_status([CheckableSections.RESOURCES], resource_desription_or_address, force)
             
         class INDICATIONS:
 
             @staticmethod
-            def get_last_items(count: int = 1) -> Result[list[CTIndicationItem]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_last_ct_indications_value_list, (count, )), CTIndicationItem)
+            def last_ct_value_containers(cached: bool, count: int = 1) -> Result[list[CTIndicationsValueContainer]]:
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_last_ct_indications_value_container_list, (cached, count)), CTIndicationsValueContainer)
 
+            @staticmethod
+            def last_chiller_value_containers(cached: bool, count: int = 1, valid_values: bool = True) -> Result[list[ChillerIndicationsValueContainer]]:
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_last_сhiller_indications_value_container_list, (cached, count, valid_values)), ChillerIndicationsValueContainer)
 
         class BACKUP:
 
             @staticmethod
             def robocopy_job_status_list() -> Result[list[RobocopyJobStatus]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.robocopy_get_job_status_list), RobocopyJobStatus)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.robocopy_get_job_status_list), RobocopyJobStatus)
 
         class SETTINGS:
 
             @staticmethod
-            def key(key: str, default_value: Any = None) -> Result[Any]:
+            def key(key: str, default_value: Any | None = None) -> Result[Any]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.get_settings_value, (key, default_value)))
+                    PIH.SERVICE.call_command(ServiceCommands.get_settings_value, (key, default_value)))
 
             @staticmethod
             def get(settings_item: SETTINGS) -> Result[Any]:
-                settings_value: SettingsValue = settings_item.value
+                settings_value: StorageValue = settings_item.value
                 return PIH.RESULT.SETTINGS.key(settings_value.key_name or settings_item.name, settings_value.default_value)
 
-        class SERVER:
-
-            pass
-
         class WORKSTATION:
 
             @staticmethod
             def all_description() -> Result[list[WorkstationDescription]]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.get_all_workstation_description), WorkstationDescription)
+                    PIH.SERVICE.call_command(ServiceCommands.get_all_workstation_description), WorkstationDescription)
 
             @staticmethod
             def all_with_prooperty(value: AD.WSProperies) -> Result[list[Workstation]]:
                 def filter_function(workstation: Workstation) -> bool:
                     return BM.has(workstation.properties, value.value)
                 return ResultTool.filter(PIH.RESULT.WORKSTATION.all(), filter_function)
 
             @staticmethod
             def by_login(value: str) -> Result[list[Workstation]]:
                 value = PIH.DATA.FORMAT.string(value)
                 if PIH.CHECK.USER.exists_by_login(value):
                     return DataTool.to_result(
-                        RPC.call(ServiceCommands.get_workstation_by_user, value), Workstation)
+                        PIH.SERVICE.call_command(ServiceCommands.get_workstation_list_by_user_login, value), Workstation)
                 else:
-                    details: str = f"Пользователь с логином {value} не найден"
-                    raise NotFound(details)
+                    raise NotFound(f"Пользователь с логином {value} не найден")
 
             @staticmethod
             def by_internal_telephone_number(value: int) -> Result[Workstation]:
                 result: Result[list[Workstation]] = PIH.RESULT.WORKSTATION.all()
                 workstation_list: list[Workstation] = result.data
-                result_worksation: Workstation = None
+                result_worksation: Workstation | None = None
                 for workstation in workstation_list:
                     if not DataTool.is_empty(workstation.description):
                         index: int = workstation.description.find(CONST.INTERNAL_TELEPHONE_NUMBER_PREFIX)
                         if index != -1:
                             internal_telephone_number_text: str = workstation.description[index:]
                             internal_telephone_number: int = PIH.DATA.EXTRACT.decimal(internal_telephone_number_text)
                             if internal_telephone_number == value:
@@ -2745,60 +3522,60 @@
                 if result_worksation is not None:#and result_worksation.accessable and not DataTool.is_empty(result_worksation.samAccountName):
                     return Result(result.fields, workstation)
                 else:
                     raise PIH.ERROR.USER.get_not_found_error(
                         "внутренним номером телефона", True, str(value))
 
             @staticmethod
-            def by_any(value: Any) -> Result[list[Workstation]]:
+            def by_any(value: int | str) -> Result[list[Workstation]]:
                 if PIH.DATA.CHECK.decimal(value):
                     return ResultTool.as_list(PIH.RESULT.WORKSTATION.by_internal_telephone_number(int(value)))
                 if PIH.CHECK.WORKSTATION.name(value):
                     return ResultTool.as_list(PIH.RESULT.WORKSTATION.by_name(value))
                 try:
                     return PIH.RESULT.WORKSTATION.by_login(value)
                 except NotFound:
                     detail: str = f"Компьютер с параметром поиска {value} не найден"
                     raise NotFound(detail)
 
             @staticmethod
             def by_name(value: str) -> Result[Workstation]:
-                value = PIH.DATA.FORMAT.string(value)
+                value = PIH.DATA.FORMAT.string(value).lower()
                 result: Result[Workstation] = ResultTool.with_first_element(ResultTool.filter(
-                    PIH.RESULT.WORKSTATION.all(), lambda item: item.name.lower() == value.lower()))
+                    PIH.RESULT.WORKSTATION.all(), lambda item: item.name.lower() == value))
                 if ResultTool.is_empty(result):
                     raise NotFound(f"Компьютер с именем {value} не найден")
                 return result
 
             @staticmethod
             def all() -> Result[list[Workstation]]:
                 def every_action(workstation: Workstation) -> None:
                     workstation.name = workstation.name.lower()
                 return ResultTool.every(DataTool.to_result(
-                    RPC.call(ServiceCommands.get_all_workstations), Workstation), every_action)
+                    PIH.SERVICE.call_command(ServiceCommands.get_all_workstations), Workstation), every_action)
 
         class INVENTORY:
 
             @staticmethod
             def report(report_file_path: str, open_for_edit: bool = False) -> Result[list[InventoryReportItem]]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.get_inventory_report, (report_file_path, open_for_edit)), InventoryReportItem)
+                    PIH.SERVICE.call_command(ServiceCommands.get_inventory_report, (report_file_path, open_for_edit)), InventoryReportItem)
 
         class TIME_TRACKING:
 
             @staticmethod
-            def today(tab_number_list: list[str] = None) -> Result[list[TimeTrackingResultByPerson]]:
+            def today(tab_number_list: list[str] | None = None) -> Result[list[TimeTrackingResultByPerson]]:
                 return PIH.RESULT.TIME_TRACKING.create(tab_number_list=tab_number_list)
 
-            def yesterday(tab_number_list: list[str] = None) -> Result[list[TimeTrackingResultByPerson]]:
+            def yesterday(tab_number_list: list[str] | None = None) -> Result[list[TimeTrackingResultByPerson]]:
                 yesterday: datetime = DateTimeTool.yesterday()
                 return PIH.RESULT.TIME_TRACKING.create(DateTimeTool.start_date(yesterday), DateTimeTool.start_date(yesterday), tab_number_list)
 
             @staticmethod
-            def in_period(day_start: int = 1, day_end: int = None, month: int = None, tab_number: list[str] = None) -> Result[list[TimeTrackingResultByPerson]]:
+            def in_period(day_start: int = 1, day_end: int | None = None, month: int | None  = None, tab_number: list[str] | None = None) -> Result[list[TimeTrackingResultByPerson]]:
                 now: datetime = datetime.now()
                 if month is not None:
                     now = now.replace(month=month)
                 start_date: datetime = DateTimeTool.start_date(now)
                 end_date: datetime = DateTimeTool.end_date(now)
                 if day_start < 0:
                     start_date -= timedelta(days=abs(day_start))
@@ -2808,25 +3585,25 @@
                     if day_end < 0:
                         day_end -= timedelta(days=abs(day_start))
                     else:
                         day_end = start_date.replace(day=day_start)
                 return PIH.RESULT.TIME_TRACKING.create(start_date, end_date, tab_number)
 
             @staticmethod
-            def create(start_date: datetime = None, end_date: datetime = None, tab_number_list: list[str] = None) -> Result[list[TimeTrackingResultByPerson]]:
-                now: datetime = datetime.now() if start_date is None or end_date is None else None
-                start_date = start_date or DateTimeTool.start_date(now)
-                end_date = end_date or DateTimeTool.end_date(now)
+            def create(start_date: datetime | None = None, end_date: datetime | None = None, tab_number_list: list[str] | None = None) -> Result[list[TimeTrackingResultByPerson]]:
+                now: datetime | None = A.D.check(A.D_C.empty(start_date) or A.D_C.empty(end_date), datetime.now())
+                start_date = DateTimeTool.start_date(start_date or now)
+                end_date = DateTimeTool.end_date(end_date or now)
 
-                def get_date_or_time(entity: TimeTrackingEntity, date: bool) -> str:
-                    return DataTool.not_none_check(entity, lambda: entity.TimeVal.split(CONST.DATE_TIME_SPLITTER)[not date])
+                def get_date_or_time(entity: TimeTrackingEntity, date: bool) -> str :
+                    return DataTool.check_not_none(entity, lambda: entity.TimeVal.split(CONST.DATETIME_SPLITTER)[not date])
                 result_data: dict = {}
                 full_name_by_tab_number_map: dict = {}
                 result_data = defaultdict(lambda: defaultdict(lambda: defaultdict(list)))
-                data: list[TimeTrackingEntity] = DataTool.to_result(RPC.call(
+                data: list[TimeTrackingEntity] = DataTool.to_result(PIH.SERVICE.call_command(
                     ServiceCommands.get_time_tracking, (start_date, end_date, tab_number_list)), TimeTrackingEntity).data
                 for time_tracking_entity in data:
                     tab_number: str = time_tracking_entity.TabNumber
                     full_name_by_tab_number_map[tab_number] = time_tracking_entity.FullName
                     result_data[time_tracking_entity.DivisionName][tab_number][get_date_or_time(time_tracking_entity, True)].append(
                         time_tracking_entity)
                 result: list[TimeTrackingResultByDivision] = []
@@ -2872,16 +3649,16 @@
                             item: TimeTrackingResultByDate = person.list[index]
                             if item.duration == 0:
                                 # if item.enter_time is None and item.exit_time is not None:
                                 if index < length - 1:
                                     item_next: TimeTrackingResultByDate = person.list[index + 1]
                                     if item.exit_time is not None:
                                         if item_next.enter_time is not None:
-                                            duration = int(datetime.fromisoformat(item.date + CONST.DATE_TIME_SPLITTER + item.exit_time).timestamp(
-                                            ) - datetime.fromisoformat(item_next.date + CONST.DATE_TIME_SPLITTER + item_next.enter_time).timestamp())
+                                            duration = int(datetime.fromisoformat(item.date + CONST.DATETIME_SPLITTER + item.exit_time).timestamp(
+                                            ) - datetime.fromisoformat(item_next.date + CONST.DATETIME_SPLITTER + item_next.enter_time).timestamp())
                                             item.duration = duration
                                             person.duration += duration
                                             if item_next.exit_time is None:
                                                 index += 1
                             index += 1
                             if index >= length - 1:
                                 break
@@ -2891,234 +3668,244 @@
         class PRINTER:
 
             @staticmethod
             def all() -> Result[list[PrinterADInformation]]:
                 def filter_by_server_name(printer_list: list[PrinterADInformation]) -> list[PrinterADInformation]:
                     return list(filter(lambda item: item.serverName == CONST.HOST.PRINTER_SERVER.NAME, printer_list))
                 result: Result[list[PrinterADInformation]] = DataTool.to_result(
-                    RPC.call(ServiceCommands.get_printers), PrinterADInformation)
+                    PIH.SERVICE.call_command(ServiceCommands.get_printers), PrinterADInformation)
                 return Result(result.fields, filter_by_server_name(result.data))
 
             @staticmethod
             def report(redirect_to_log: bool = True) -> Result[list[PrinterReport]]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.printers_report, redirect_to_log), PrinterReport)
+                    PIH.SERVICE.call_command(ServiceCommands.printers_report, redirect_to_log), PrinterReport)
 
             @staticmethod
             def status(redirect_to_log: bool = True) -> Result[list[PrinterStatus]]:
                 return DataTool.to_result(
-                    RPC.call(ServiceCommands.printers_status, redirect_to_log), PrinterStatus)
+                    PIH.SERVICE.call_command(ServiceCommands.printers_status, redirect_to_log), PrinterStatus)
 
         class MARK:
 
             @staticmethod
             def by_tab_number(value: str) -> Result[Mark]:
                 result: Result[Mark] = DataTool.to_result(
-                    RPC.call(ServiceCommands.get_mark_by_tab_number, value), Mark)
+                    PIH.SERVICE.call_command(ServiceCommands.get_mark_by_tab_number, value), Mark)
                 if ResultTool.is_empty(result):
                     details: str = f"Карта доступа с номером '{value}' не найдена"
                     raise NotFound(details)
                 return result
 
             @staticmethod
             def person_divisions() -> Result[list[Mark]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_person_divisions), MarkDivision)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_person_divisions), MarkDivision)
 
             @staticmethod
             def by_name(value: str, first_item: bool = False) -> Result[list[Mark]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_mark_by_person_name, value), Mark, first_item)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_mark_by_person_name, value), Mark, first_item)
 
             @staticmethod
             def by_full_name(value: FullName, first_item: bool = False) -> Result[list[Mark]]:
-                return PIH.RESULT.MARK.by_name(FullNameTool.from_string(value), first_item)
+                return PIH.RESULT.MARK.by_name(FullNameTool.fullname_from_string(value), first_item)
 
             @staticmethod
             def temporary_list() -> Result[list[TemporaryMark]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_temporary_marks), TemporaryMark)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_temporary_marks), TemporaryMark)
 
             @staticmethod
             def by_any(value: str) -> Result[list[Mark]]:
                 if PIH.CHECK.MARK.tab_number(value):
                     return ResultTool.as_list(PIH.RESULT.MARK.by_tab_number(value))
                 elif PIH.CHECK.name(value, True):
                     return PIH.RESULT.MARK.by_name(value)
                 return Result()
 
             @staticmethod
             def free_list(show_with_guest_marks: bool = False) -> Result[list[Mark]]:
                 result: Result[list[Mark]] = DataTool.to_result(
-                    RPC.call(ServiceCommands.get_free_marks), Mark)
+                    PIH.SERVICE.call_command(ServiceCommands.get_free_marks), Mark)
 
                 def filter_function(item: Mark) -> bool:
                     return EnumTool.get(MarkType, item.type) != MarkType.GUEST
                 return result if show_with_guest_marks else ResultTool.filter(result, filter_function)
 
             @staticmethod
             def free_marks_by_group_id(value: int) -> Result[list[Mark]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_free_marks_by_group_id, value), Mark)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_free_marks_by_group_id, value), Mark)
 
             @staticmethod
-            def free_marks_group_statistics(show_guest_marks: bool = None) -> Result[list[MarkGroupStatistics]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_free_marks_group_statistics, show_guest_marks), MarkGroupStatistics)
+            def free_marks_group_statistics(show_guest_marks: bool | None = None) -> Result[list[MarkGroupStatistics]]:
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_free_marks_group_statistics, show_guest_marks), MarkGroupStatistics)
 
             @staticmethod
             def all() -> Result[list[Mark]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_all_persons), Mark)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_all_persons), Mark)
 
             @staticmethod
             def temporary_mark_owner(mark: Mark) -> Result[Mark]:
-                return DataTool.check(mark is not None and EnumTool.get(MarkType, mark.type) == MarkType.TEMPORARY, lambda: DataTool.to_result(RPC.call(ServiceCommands.get_owner_mark_for_temporary_mark, mark.TabNumber), Mark), None)
+                return DataTool.check(mark is not None and EnumTool.get(MarkType, mark.type) == MarkType.TEMPORARY, lambda: DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_owner_mark_for_temporary_mark, mark.TabNumber), Mark), None)
 
             @staticmethod
             def temporary_mark_owner_by_tab_number(value: str) -> Result[Mark]:
                 return PIH.RESULT.MARK.temporary_mark_owner(PIH.RESULT.MARK.by_tab_number(value).data)
 
         class POLIBASE:
 
             class NOTIFICATION:
 
                 @staticmethod
                 def by(value: PolibasePersonVisitNotification) -> Result[list[PolibasePersonVisitNotification]]:
-                    return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_visit_notifications, value), PolibasePersonVisitNotification)
+                    return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.search_polibase_person_visit_notifications, value), PolibasePersonVisitNotification)
 
                 @staticmethod
                 def by_message_id(value: int) -> Result[PolibasePersonVisitNotification]:
                     return ResultTool.with_first_element(PIH.RESULT.POLIBASE.NOTIFICATION.by(PolibasePersonVisitNotification(messageID=value)))
 
                 class CONFIRMATION:
                     
                     @staticmethod
                     def by(recipient: str, sender: str) -> Result[PolibasePersonNotificationConfirmation]:
-                        return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_notification_confirmation, PolibasePersonNotificationConfirmation(recipient, sender)), PolibasePersonNotificationConfirmation)
+                        return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.search_polibase_person_notification_confirmation, PolibasePersonNotificationConfirmation(recipient, sender)), PolibasePersonNotificationConfirmation)
 
             class INFORMATION_QUEST:
 
                 @staticmethod
                 def get(search_critery: PolibasePersonInformationQuest) -> Result[list[PolibasePersonInformationQuest]]:
                     return DataTool.to_result(
-                        RPC.call(ServiceCommands.search_polibase_person_information_quests, search_critery), PolibasePersonInformationQuest)
+                        PIH.SERVICE.call_command(ServiceCommands.search_polibase_person_information_quests, search_critery), PolibasePersonInformationQuest)
 
             class VISIT:
 
                 @staticmethod
-                def after_id(value: int, test: bool = None) -> Result[list[PolibasePersonVisitDS]]:
-                    return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_visits, (PolibasePersonVisitSearchCritery(vis_no=f">{value}"), test)), PolibasePersonVisitDS)
+                def after_id(value: int, test: bool | None = None) -> Result[list[PolibasePersonVisitDS]]:
+                    return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.search_polibase_person_visits, (PolibasePersonVisitSearchCritery(vis_no=f">{value}"), test)), PolibasePersonVisitDS)
 
                 @staticmethod
-                def by_id(value: int, test: bool = None) -> Result[PolibasePersonVisitDS]:
-                    return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_visits, (PolibasePersonVisitSearchCritery(vis_no=value), test)), PolibasePersonVisitDS, True)
+                def by_id(value: int, test: bool | None = None) -> Result[PolibasePersonVisitDS]:
+                    return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.search_polibase_person_visits, (PolibasePersonVisitSearchCritery(vis_no=value), test)), PolibasePersonVisitDS, True)
 
                 @staticmethod
-                def last_id(test: bool = None) -> Result[int]:
-                    return DataTool.to_result(RPC.call(ServiceCommands.get_polibase_person_visits_last_id, test))
+                def last_id(test: bool | None = None) -> Result[int]:
+                    return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_polibase_person_visits_last_id, test))
 
                 @staticmethod
-                def today(test: bool = None) -> Result[list[PolibasePersonVisitDS]]:
+                def today(test: bool | None = None) -> Result[list[PolibasePersonVisitDS]]:
                     return PIH.RESULT.POLIBASE.VISIT.by_registration_date(DateTimeTool.today(), test)
 
                 @staticmethod
-                def prerecording_today(test: bool = None) -> Result[list[PolibasePersonVisitDS]]:
+                def prerecording_today(test: bool | None = None) -> Result[list[PolibasePersonVisitDS]]:
                     return PIH.RESULT.POLIBASE.VISIT.prerecording_by_registration_date(DateTimeTool.today(), test)
 
                 @staticmethod
-                def by_registration_date(value: datetime, test: bool = None) -> Result[list[PolibasePersonVisitDS]]:
-                    return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_visits, (PolibasePersonVisitSearchCritery(vis_reg_date=DateTimeTool.date_to_string(value, CONST.POLIBASE.DATE_FORMAT)), test)), PolibasePersonVisitDS)
+                def by_registration_date(value: datetime, test: bool | None = None) -> Result[list[PolibasePersonVisitDS]]:
+                    return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.search_polibase_person_visits, (PolibasePersonVisitSearchCritery(vis_reg_date=DateTimeTool.date_to_string(value, CONST.POLIBASE.DATE_FORMAT)), test)), PolibasePersonVisitDS)
 
                 @staticmethod
-                def prerecording_by_registration_date(value: datetime = None, test: bool = None) -> Result[list[PolibasePersonVisitDS]]:
+                def prerecording_by_registration_date(value: datetime = None, test: bool | None = None) -> Result[list[PolibasePersonVisitDS]]:
                     def filter_function(value: PolibasePersonVisitDS) -> bool:
                         return value.pin == CONST.POLIBASE.PRERECORDING_PIN
                     return ResultTool.filter(PIH.RESULT.POLIBASE.VISIT.by_registration_date(value, test), filter_function)
 
                 class DATA_STORAGE:
 
                     @staticmethod
                     def search(value: PolibasePersonVisitDS) -> Result[PolibasePersonVisitDS]:
-                        return DataTool.to_result(RPC.call(ServiceCommands.search_polibase_person_visits_in_data_storage, (value, )), PolibasePersonVisitDS, True)
+                        return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.search_polibase_person_visits_in_data_storage, (value, )), PolibasePersonVisitDS, True)
 
                     @staticmethod
                     def last() -> Result[PolibasePersonVisitDS]:
                         return PIH.RESULT.POLIBASE.VISIT.DATA_STORAGE.search(PolibasePersonVisitDS(id=-1))
 
 
-            def person_by_telephone_number(value: str, test: bool = None) -> Result[list[PolibasePerson]]:
+            @staticmethod
+            def person_by_telephone_number(value: str, test: bool | None = None) -> Result[list[PolibasePerson]]:
                 value = PIH.DATA.FORMAT.telephone_number_international(value)
-                result: Result[PolibasePerson] = DataTool.to_result(RPC.call(
-                    ServiceCommands.get_polibase_persons_by_telephone_number, (value, test)), PolibasePerson)
+                result: Result[PolibasePerson] = DataTool.to_result(PIH.SERVICE.call_command(
+                    ServiceCommands.get_polibase_persons_by_telephone_number, (value, test)), PIH.DATA.EXTRACT.polibase_person)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error("идентификационным номером", value)
                 return result
 
             @staticmethod
-            def person_by_pin(value: int, test: bool = None) -> Result[PolibasePerson]:
-                result: Result[PolibasePerson] = DataTool.to_result(RPC.call(
-                    ServiceCommands.get_polibase_person_by_pin, (value, test)), PolibasePerson)
+            def person_by_pin(value: int, test: bool | None = None) -> Result[PolibasePerson]:
+                result: Result[PolibasePerson] = DataTool.to_result(PIH.SERVICE.call_command(
+                    ServiceCommands.get_polibase_person_by_pin, (value, test)), PIH.DATA.EXTRACT.polibase_person)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error("идентификационным номером", value)
                 return result
 
             @staticmethod
-            def persons_pin_by_visit_date(date: datetime, test: bool = None) -> Result[list[int]]:
+            def persons_pin_by_visit_date(date: datetime, test: bool | None = None) -> Result[list[int]]:
                 if test:
                     return Result(None, [100310])
-                return DataTool.to_result(RPC.call(ServiceCommands.get_polibase_persons_pin_by_visit_date, (date.strftime(CONST.DATE_FORMAT), test)))
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_polibase_persons_pin_by_visit_date, (date.strftime(CONST.DATE_FORMAT), test)))
+
+            @staticmethod
+            def person_registrator_by_pin(value: int, test: bool | None = None) -> Result[PolibasePerson]:
+                result: Result[list[PolibasePerson]] = DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_polibase_person_registrator_by_pin, (value, test)), PIH.DATA.EXTRACT.polibase_person)
+                if ResultTool.is_empty(result):
+                    raise PIH.ERROR.POLIBASE.create_not_found_error(
+                        "идентификационным номером", value)
+                return result
 
             @staticmethod
-            def person_creator_by_pin(value: int, test: bool = None) -> Result[PolibasePerson]:
-                result: Result[list[PolibasePerson]] = DataTool.to_result(RPC.call(ServiceCommands.get_polibase_person_registrator_by_pin, (value, test)), PolibasePerson)
+            def person_operator_by_pin(value: int, test: bool | None = None) -> Result[PolibasePerson]:
+                result: Result[list[PolibasePerson]] = DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_polibase_person_operator_by_pin, (value, test)), PIH.DATA.EXTRACT.polibase_person)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error(
                         "идентификационным номером", value)
                 return result
 
             @staticmethod
-            def persons_by_full_name(value: str, test: bool = None) -> Result[list[PolibasePerson]]:
-                result: Result[list[PolibasePerson]] = DataTool.to_result(RPC.call(ServiceCommands.get_polibase_persons_by_full_name, (value, test)), PolibasePerson)
+            def persons_by_full_name(value: str, test: bool | None = None) -> Result[list[PolibasePerson]]:
+                value = FullNameTool.format(value)
+                result: Result[list[PolibasePerson]] = DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_polibase_persons_by_full_name, (value, test)), PIH.DATA.EXTRACT.polibase_person)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error("именем", value)
                 return result
 
             @staticmethod
-            def persons_by_pin(value: list[int], test: bool = None) -> Result[list[PolibasePerson]]:
-                result: Result[list[PolibasePerson]] = DataTool.to_result(RPC.call(ServiceCommands.get_polibase_persons_by_pin, (value, test)), PolibasePerson)
+            def persons_by_pin(value: list[int], test: bool | None = None) -> Result[list[PolibasePerson]]:
+                result: Result[list[PolibasePerson]] = DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_polibase_persons_by_pin, (value, test)), PIH.DATA.EXTRACT.polibase_person)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.POLIBASE.create_not_found_error("идентификационным номером", value)
                 return result
 
             @staticmethod
-            def persons_by_card_registry_folder_name(value: str, test: bool = None) -> Result[list[PolibasePerson]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_polibase_persons_by_card_registry_folder_name, (value, test)), PolibasePerson)
+            def persons_by_card_registry_folder_name(value: str, test: bool | None = None) -> Result[list[PolibasePerson]]:
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_polibase_persons_by_card_registry_folder_name, (value, test)), PIH.DATA.EXTRACT.polibase_person)
 
             @staticmethod
-            def person_pin_list_with_old_format_barcode(test: bool = None) -> Result[list[int]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_polibase_person_pin_list_with_old_format_barcode, (test, )))
+            def person_pin_list_with_old_format_barcode(test: bool | None = None) -> Result[list[int]]:
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_polibase_person_pin_list_with_old_format_barcode, (test, )))
 
             @staticmethod
-            def persons_by_any(value: str, test: bool = None) -> Result[list[PolibasePerson]]:
+            def persons_by_any(value: str, test: bool | None = None) -> Result[list[PolibasePerson]]:
                 if PIH.CHECK.telephone_number(value) or PIH.CHECK.telephone_number_international(value):
                     return ResultTool.as_list(PIH.RESULT.POLIBASE.person_by_telephone_number(value, test))
                 if PIH.CHECK.POLIBASE.person_pin(value):
                     return ResultTool.as_list(PIH.RESULT.POLIBASE.person_by_pin(int(value), test))
                 if PIH.CHECK.POLIBASE.person_card_registry_folder_name(value):
                     return PIH.RESULT.POLIBASE.persons_by_card_registry_folder_name(value, test)
                 return ResultTool.as_list(PIH.RESULT.POLIBASE.persons_by_full_name(value))
 
         class USER:
 
             @staticmethod
-            def by_login(value: str, active: bool = None, cached: bool = None) -> Result[User]:
-                result: Result[User] = DataTool.to_result(RPC.call(ServiceCommands.get_user_by_login, (value, active, PIH.SETTINGS.USER.use_cache() if cached is None else cached)), User)
+            def by_login(value: str, active: bool | None = None, cached: bool | None = None) -> Result[User]:
+                result: Result[User] = DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_user_by_login, (value, active, cached)), User)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.USER.get_not_found_error("логином", active, value)
                 return result
 
             @staticmethod
-            def by_telephone_number(value: str, active: bool = None) -> Result[User]:
+            def by_telephone_number(value: str, active: bool | None = None) -> Result[User]:
                 result: Result[User] = DataTool.to_result(
-                    RPC.call(ServiceCommands.get_user_by_telephone_number, (value, active)), User, True)
+                    PIH.SERVICE.call_command(ServiceCommands.get_user_by_telephone_number, (value, active)), User, True)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.USER.get_not_found_error("номером телефона", active, value)
                 return result
 
             @staticmethod
             def by_internal_telephone_number(value: int) -> Result[User]:
                 workstation_list: list[Workstation] = PIH.RESULT.WORKSTATION.all().data
@@ -3136,30 +3923,30 @@
                     return PIH.RESULT.USER.by_login(workstation.samAccountName)
                 else:
                     raise PIH.ERROR.USER.get_not_found_error(
                         "внутренним номером телефона", True, str(value))
 
             @staticmethod
             def by_polibase_pin(value: int) -> Result[User]:
-                return PIH.RESULT.USER.by_name(PIH.RESULT.POLIBASE.person_by_pin(value).data.FullName)
+                return ResultTool.with_first_element(PIH.RESULT.USER.by_name(PIH.RESULT.POLIBASE.person_by_pin(value).data.FullName))
 
             @staticmethod
             def by_workstation_name(name: str) -> Result[User]:
                 name = name.lower()
-                user_workstation: Workstation = DataTool.to_result(RPC.call(
+                user_workstation: Workstation = DataTool.to_result(PIH.SERVICE.call_command(
                     ServiceCommands.get_user_by_workstation, name), Workstation, True).data
-                if user_workstation is None:
+                if DataTool.is_empty(user_workstation):
                     details: str = f"Компьютер с именем '{name}' не найден!"
                     raise NotFound(details)
-                if user_workstation.samAccountName is None:
+                if DataTool.is_empty(user_workstation.samAccountName):
                     raise NotFound(f"За компьютером {name} нет залогиненного пользователя", name)
                 return PIH.RESULT.USER.by_login(user_workstation.samAccountName)
 
             @staticmethod
-            def by_any(value: Any, active: bool = None) -> Result[list[User]]:
+            def by_any(value: Any, active: bool | None = None) -> Result[list[User]]:
                 def by_number(value: int) -> Result[list[User]]:
                     try:
                         return ResultTool.as_list(PIH.RESULT.USER.by_tab_number(value))
                     except NotFound:
                         try:
                             return ResultTool.as_list(PIH.RESULT.USER.by_login(PIH.RESULT.WORKSTATION.by_internal_telephone_number(value).data.samAccountName))
                         except:
@@ -3190,70 +3977,89 @@
                         return PIH.RESULT.USER.by_name(value, active)
                 elif isinstance(value, int):
                     return by_number(value)
                 raise PIH.ERROR.USER.get_not_found_error("поисковым значением", active, value)
 
             @staticmethod
             def by_job_position(value: AD.JobPisitions) -> Result[list[User]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_users_by_job_position, value.name), User)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_users_by_job_position, value.name), User)
 
             @staticmethod
             def by_group(value: AD.Groups) -> Result[list[User]]:
                 return PIH.RESULT.USER.by_group_name(value.name)
 
             @staticmethod
             def by_group_name(value: str) -> Result[list[User]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_users_by_group, value), User)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_users_by_group, value), User)
 
 
             @staticmethod
             def template_list() -> Result[list[User]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_template_users), User)
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_template_users), User)
 
             @staticmethod
-            def containers() -> Result[list[UserContainer]]:
-                return DataTool.to_result(RPC.call(
-                    ServiceCommands.get_containers), UserContainer)
+            def containers() -> Result[list[UserBase]]:
+                return DataTool.to_result(PIH.SERVICE.call_command(
+                    ServiceCommands.get_containers), UserBase)
 
             @staticmethod
-            def by_full_name(value: FullName, get_first: bool = False, active: bool = None) -> Result[list[User]]:
-                return DataTool.to_result(RPC.call(ServiceCommands.get_user_by_full_name, (value, active)), User, get_first)
+            def by_full_name(value: FullName, get_first: bool = False, active: bool | None = None) -> Result[list[User] | User]:
+                return DataTool.to_result(PIH.SERVICE.call_command(ServiceCommands.get_user_by_full_name, (value, active)), User, get_first)
 
             @staticmethod
-            def by_name(value: str, active: bool = None) -> Result[list[User]]:
+            def by_name(value: str, active: bool | None = None, cached: bool | None = None) -> Result[list[User]]:
                 result: Result[list[User]] = DataTool.to_result(
-                    RPC.call(ServiceCommands.get_users_by_name, (value, active)), User)
+                    PIH.SERVICE.call_command(ServiceCommands.get_users_by_name, (value, active, cached)), User)
                 if ResultTool.is_empty(result):
                     raise PIH.ERROR.USER.get_not_found_error("именем", active, value)
                 return result
 
             @staticmethod
-            def all(active: bool = None) -> Result[list[User]]:
+            def all(active: bool | None = None) -> Result[list[User]]:
                 return PIH.RESULT.USER.by_name(AD.SEARCH_ALL_PATTERN, active)
 
             @staticmethod
-            def list_with_telephone_number(active: bool = None) -> Result[list[User]]:
+            def list_with_telephone_number(active: bool | None = None) -> Result[list[User]]:
                 def user_with_telephone_number(user: User) -> bool:
                     return PIH.CHECK.telephone_number(user.telephoneNumber)
                 return ResultTool.filter(PIH.RESULT.USER.all(active), lambda user: user_with_telephone_number(user))
 
             @staticmethod
             def by_tab_number(value: str) -> Result[User]:
                 result: Result[Mark] = PIH.RESULT.MARK.by_tab_number(value)
                 if ResultTool.is_empty(result):
                     details: str = f"Карта доступа с номером {value} не найдена"
                     raise NotFound(details)
                 return PIH.RESULT.USER.by_mark(result.data)
 
             @staticmethod
             def by_mark(value: Mark) -> Result[User]:
-                return Result(FIELD_COLLECTION.AD.USER, DataTool.check(value, lambda: DataTool.get_first_item(PIH.RESULT.USER.by_full_name(FullNameTool.from_string(value.FullName)).data)))
+                return Result(FIELD_COLLECTION.AD.USER, DataTool.check(value, lambda: DataTool.get_first_item(PIH.RESULT.USER.by_full_name(FullNameTool.fullname_from_string(value.FullName)).data)))
 
     class CHECK:
 
+        class ACTIONS:
+
+            @staticmethod
+            def get(action_or_name: str | Actions) -> Actions | None:
+                _action: Actions | None = None if isinstance(action_or_name, str) else action_or_name
+                if DataTool.is_none(_action):
+                    for item in Actions:
+                        if item.name == action_or_name or item.value.name == action_or_name or item.value.alias == action_or_name:
+                            _action = item
+                            break
+                return _action
+
+
+        class EVENTS:
+
+            @staticmethod
+            def has(value: Events | None, parameters: tuple[Any] | None) -> bool:
+                return not ResultTool.is_empty(PIH.RESULT.EVENTS.get(value, parameters))
+
         class SETTINGS:
     
             @staticmethod
             def by_time(current: datetime, settings: SETTINGS) -> bool:
                 return DateTimeTool.is_equal_by_time(current, PIH.SETTINGS.to_datetime(settings))
 
         class INDICATION:
@@ -3261,19 +4067,40 @@
             @staticmethod
             def ct_notification_start_time(current: datetime) -> bool:
                 start_time_list: list[datetime] = PIH.SETTINGS.INDICATION.ct_notification_start_time()
                 for start_time in start_time_list:
                     if DateTimeTool.is_equal_by_time(current, start_time):
                         return True
                 return False
+            
+        class RECOGNIZE:
+
+            @staticmethod
+            def document_type_exists(file_path: str, value: DocumentTypes, log_level: int | None = None) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.document_type_exists, (file_path, value.name, log_level)))
+
+        class NOTES:
+
+            @staticmethod
+            def exists(name: str) -> bool:
+                return not DataTool.is_empty(DataTool.rpc_unrepresent(
+                    PIH.SERVICE.call_command(ServiceCommands.get_gkeep_item_id, (name, ))))
 
         class RESOURCE:
-        
+
+            @staticmethod
+            def accessibility_by_ping_with_port(address_or_ip: str, port:int, host: str | None = None, count: int | None = None, check_for_all: bool = True) -> bool:
+                return PIH.CHECK.RESOURCE.accessibility_by_ping(":".join((address_or_ip, str(port))), host, count, check_for_all)
+
             @staticmethod
-            def accessibility_by_ping(address_or_ip: str, host: str = None, count: int = None, check_for_all: bool = True) -> bool:
+            def accessibility_by_smb_port(address_or_ip: str, host: str | None = None, count: int | None = None, check_for_all: bool = True) -> bool:
+                return PIH.CHECK.RESOURCE.accessibility_by_ping_with_port(address_or_ip, WINDOWS.PORTS.SMB, host, count, check_for_all)
+            
+            @staticmethod
+            def accessibility_by_ping(address_or_ip: str, host: str | None = None, count: int | None = None, check_for_all: bool = True) -> bool:
                 count = count or 4
                 local_ping_commnad_list: list[str] = [PIH.PSTOOLS.get_executor_path(
                     CONST.PSTOOLS.PS_PING), CONST.PSTOOLS.ACCEPTEULA, "-4", "-n", str(count), address_or_ip]
                 pocess_result: CompletedProcess = A.PS.execute_command_list(local_ping_commnad_list if host is None else A.PS.create_command_list_for_psexec_command(local_ping_commnad_list, host, interactive=True), True, True)
                 if pocess_result.returncode == 0:
                     out: str = pocess_result.stdout
                     lost_marker: str = "Lost = "
@@ -3294,48 +4121,51 @@
                 else:
                     resource_status = PIH.RESULT.RESOURCES.get_resource_status(
                         resource_status_or_address)
                 return None if resource_status is None else resource_status.inaccessibility_counter < resource_status.inaccessibility_check_values[0]
                 
             @staticmethod
             def vpn_pacs_accessibility(count: int = 2) -> bool:
-                return PIH.PSTOOLS.ping(RESOURCE.DESCRIPTIONS.VPN_PACS_SPB.address, CONST.HOST.WS255.NAME, count)
+                return PIH.PSTOOLS.ping(RESOURCES.DESCRIPTIONS.VPN_PACS_SPB.address, CONST.HOST.WS255.NAME, count)
             
             @staticmethod
             def pacs_accessibility(count: int = 2) -> bool:
-                return PIH.CHECK.RESOURCE.accessibility_by_ping(RESOURCE.DESCRIPTIONS.PACS_SPB.address, CONST.HOST.WS255.NAME, count)
+                return PIH.CHECK.RESOURCE.accessibility_by_ping(RESOURCES.DESCRIPTIONS.PACS_SPB.address, CONST.HOST.WS255.NAME, count)
            
             @staticmethod
             def wappi_profile_accessibility(value: Any, cached: bool = False) -> bool:
                 return PIH.CHECK.RESOURCE.accessibility(PIH.RESULT.RESOURCES.get_resource_status(EnumTool.get_value(value, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value))) if cached else PIH.CHECK.MESSAGE.WHATSAPP.WAPPI.accessibility(value, False)
 
             @staticmethod
             def ws_accessibility(name: str) -> bool:
                 result: Result[Workstation] = PIH.RESULT.WORKSTATION.by_name(name)
                 return not ResultTool.is_empty(result) and result.data.accessable
             
             @staticmethod
             def polibase_accessibility(cached: bool = False) -> bool:
                 try:
                     if cached:
-                        return PIH.RESULT.RESOURCES.get_resource_status(RESOURCE.DESCRIPTIONS.POLIBASE).accessable
+                        return PIH.RESULT.RESOURCES.get_resource_status(RESOURCES.DESCRIPTIONS.POLIBASE).accessable
                     result_by_ping: bool = PIH.SERVICE.check_accessibility(ServiceRoles.POLIBASE)    
                     result_by_pin : bool = PIH.CHECK.POLIBASE.person_exists_by_pin(CONST.POLIBASE.PRERECORDING_PIN)
-                    print("POLIBASE", result_by_ping, result_by_pin)
                     return result_by_ping and result_by_pin
                 except NotFound:
-                    print("POLIBASE BY PIN")
                     pass
                 return False
 
         class EMAIL:
 
             @staticmethod
             def accessability(value: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.check_email_accessibility, value))
+                def internal_accessability(value: str, verification_method: EMAIL_VERIFICATION_METHODS = EMAIL_VERIFICATION_METHODS.DEFAULT) -> bool:
+                     return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.check_email_accessibility, (value, verification_method)))
+                if not internal_accessability(value, EMAIL_VERIFICATION_METHODS.DEFAULT):
+                    return internal_accessability(value, EMAIL_VERIFICATION_METHODS.ABSTRACT_API)   
+                return True
+               
 
         class FILE:
 
             @staticmethod
             def excel_file(path: str) -> bool:
                 return os.path.isfile(path) and PathTool.get_extension(path) in [FILE.EXTENSION.EXCEL_OLD, FILE.EXTENSION.EXCEL_NEW]
 
@@ -3352,15 +4182,15 @@
                     notify = False
                 else:
                     result = PIH.CHECK.USER.by_group(user, group)
                     if result:
                         session.add_allowed_group(group)
                 if notify:
                     PIH.LOG.it(
-                        f"Запрос на доступа к группе: {group.name} от пользователя {user.name} ({user.samAccountName}). Доступ {'разрешен' if result else 'отклонен'}.", LogLevels.NORMAL if result else LogLevels.ERROR)
+                        f"Запрос на доступа к группе: {group.name} от пользователя {user.name} ({user.samAccountName}). Доступ {'разрешен' if result else 'отклонен'}.", LogMessageFlags.NORMAL if result else LogMessageFlags.ERROR)
                 if not result and exit_on_access_denied:
                     session.exit(5, "Функционал недоступен...")
                 return result
 
             @staticmethod
             def admin(exit_on_access_denied: bool = False, session: SessionBase = None, notify_on_fail: bool = True, notify_on_success: bool = True) -> bool:
                 return PIH.CHECK.ACCESS.by_group(AD.Groups.Admin, exit_on_access_denied, session, notify_on_fail, notify_on_success)
@@ -3385,15 +4215,15 @@
 
             @staticmethod
             def by_group(user: User, group: AD.Groups) -> bool:
                 return not DataTool.is_empty(ResultTool.do_while(PIH.RESULT.USER.by_group(group), lambda check_user: check_user.samAccountName == user.samAccountName))
 
             @staticmethod
             def exists_by_login(value: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.check_user_exists_by_login, value))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.check_user_exists_by_login, value))
 
             @staticmethod
             def user(user: User) -> bool:
                 return PIH.CHECK.full_name(user.name)
 
             @staticmethod
             def active(user: User) -> bool:
@@ -3404,15 +4234,15 @@
                 return not ResultTool.is_empty(PIH.RESULT.USER.by_full_name(full_name))
 
             @staticmethod
             def search_attribute(value: str) -> bool:
                 return value in AD.SEARCH_ATTRIBUTES
 
             @staticmethod
-            def property(value: str | None, default_value: str = USER_PROPERTY.PASSWORD) -> str:
+            def property(value: str | None, default_value: str = USER_PROPERTIES.PASSWORD) -> str:
                 return value or default_value
 
             @staticmethod
             def accessibility() -> bool:
                 return PIH.SERVICE.check_accessibility(ServiceRoles.AD)
 
         class MESSAGE:
@@ -3424,15 +4254,15 @@
                     @staticmethod
                     def from_me(value: str) -> bool:
                         value = PIH.DATA.FORMAT.telephone_number(value)
                         return value in [PIH.DATA.TELEPHONE_NUMBER.it_administrator(), PIH.DATA.TELEPHONE_NUMBER.call_centre_administrator(), PIH.DATA.TELEPHONE_NUMBER.marketer()]
 
                     @staticmethod
                     def accessibility(profile: Any, cached: bool = True) -> bool:
-                        def internal_accessibility(profile: Any = None) -> bool:
+                        def internal_accessibility(profile: Any | None = None) -> bool:
                             profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                             url: str = f"{CONST.MESSAGE.WHATSAPP.WAPPI.URL_GET_STATUS}{profile}"
                             headers: dict = {
                                 "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION,
                                 "Content-Type": "application/json"
                             }
                             response_result: dict = None
@@ -3447,20 +4277,20 @@
                             return response_result["app_status"] == "open"
                         return PIH.CHECK.RESOURCE.wappi_profile_accessibility(profile, True) if cached else internal_accessibility(profile)
 
         class MARK:
 
             @staticmethod
             def free(tab_number: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.check_mark_free, tab_number))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.check_mark_free, tab_number))
 
             @staticmethod
             def exists_by_full_name(full_name: FullName) -> bool:
                 result: Result[list[Mark]] = PIH.RESULT.MARK.by_name(
-                    FullNameTool.to_string(full_name))
+                    FullNameTool.fullname_to_string(full_name))
                 return ResultTool.is_empty(result)
 
             @staticmethod
             def accessibility() -> bool:
                 return PIH.SERVICE.check_accessibility(ServiceRoles.MARK)
 
             @staticmethod
@@ -3473,29 +4303,29 @@
             def accessibility() -> bool:
                 return PIH.CHECK.ACCESS.by_group(AD.Groups.TimeTrackingReport)
 
         class INVENTORY:
 
             @staticmethod
             def is_report_file(file_path: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.check_inventory_report, file_path))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.check_inventory_report, file_path))
 
             @staticmethod
             def accessibility() -> bool:
                 return PIH.SERVICE.check_accessibility(ServiceRoles.DOCS) and PIH.CHECK.ACCESS.inventory()
 
         class POLIBASE:
 
             @staticmethod
             def accessibility() -> bool:
                 return PIH.SERVICE.check_accessibility(ServiceRoles.POLIBASE) and PIH.CHECK.ACCESS.polibase()
 
             @staticmethod
             def person_card_registry_folder_name(value: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.check_polibase_person_card_registry_folder_name, value))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.check_polibase_person_card_registry_folder_name, value))
 
             @staticmethod
             def person_exists_by_pin(pin: int) -> bool:
                 try:
                     return not ResultTool.is_empty(PIH.RESULT.POLIBASE.person_by_pin(pin))
                 except NotFound:
                     return False
@@ -3527,24 +4357,39 @@
         def login(value: str) -> bool:
             pattern: str = r"^[a-z]+[a-z_0-9]{"+str(CONST.NAME_POLICY.PART_ITEM_MIN_LENGTH - 1) + ",}"
             return re.fullmatch(pattern, value, re.IGNORECASE) is not None
 
         class WORKSTATION:
 
             @staticmethod
+            def accessibility(name: str) -> bool | None:
+                try:
+                    return PIH.RESULT.WORKSTATION.by_name(name).data.accessable
+                except NotFound as _:
+                    return None
+
+            @staticmethod
+            def windows_service_running(name: str, workstation_name: str) -> bool | None:
+                accessable: bool | None = PIH.CHECK.WORKSTATION.accessibility(workstation_name)
+                if DataTool.is_none(accessable):
+                    return None
+                return PIH.PSTOOLS.windows_service_running(name, workstation_name)
+
+            @staticmethod
             def name(value: str) -> bool:
                 value = PIH.DATA.FORMAT.string(value)
                 for prefix in AD.WORKSTATION_PREFIX_LIST:
                     if value.startswith(prefix):
                         return True
                 return False
 
             @staticmethod
             def exists(name: str) -> bool:
-                return not ResultTool.is_empty(ResultTool.filter(PIH.RESULT.WORKSTATION.all_description(), lambda workstation: name.lower() == workstation.name.lower()))
+                name = name.lower()
+                return not ResultTool.is_empty(ResultTool.filter(PIH.RESULT.WORKSTATION.all_description(), lambda workstation: name == workstation.name.lower()))
 
             @staticmethod
             def has_property(workstation: WorkstationDescription, property: AD.WSProperies) -> bool:
                 return BM.has(workstation.properties, property)
 
             @staticmethod
             def watchable(workstation: WorkstationDescription) -> bool:
@@ -3564,16 +4409,16 @@
 
         @staticmethod
         def telephone_number_international(value: str) -> bool:
             return PIH.CHECK.telephone_number(value, True)
 
         @staticmethod
         def email(value: str, check_accesability: bool = False) -> bool:
-            return re.fullmatch(r"([A-Za-z0-9]+[.-_])*[A-Za-z0-9]+@[A-Za-z0-9-]+(\.[A-Z|a-z]{2,})+", value) is not None and (not check_accesability or PIH.CHECK.EMAIL.accessability(value))
-
+            return not DataTool.is_empty(re.fullmatch(r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b", value))  and (not check_accesability or PIH.CHECK.EMAIL.accessability(value))
+        
         @staticmethod
         def name(value: str, use_space: bool = False) -> bool:
             pattern = r"[а-яА-ЯёЁ" + (" " if use_space else "") + \
                 "]{" + str(CONST.NAME_POLICY.PART_ITEM_MIN_LENGTH) + ",}$"
             return re.fullmatch(pattern, value) is not None
 
         @staticmethod
@@ -3589,325 +4434,77 @@
 
 
     class LOG:
 
         executor = ThreadPoolExecutor(max_workers=1)
 
         @staticmethod
-        def send_message(value: str, channel: LogChannels = LogChannels.DEFAULT, level: Any = LogLevels.DEFAULT) -> str:
-            level_value: int = None
-            level_list: list[LogLevels] = None
-            if isinstance(level, LogLevels):
-                level_list = [level]
-            if isinstance(level, int):
-                level_value = level
-            if level_value is None:
-                level_value = 0
-                for level_item in level_list:
-                    level_value = level_value | level_item.value
-
+        def send(value: str, channel: LogMessageChannels = LogMessageChannels.DEFAULT, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            level = level or LogMessageFlags.DEFAULT
             def internal_send_message(message: str, channel_name: str, level_value: int) -> None:
                 try:
-                    RPC.call(ServiceCommands.send_log_message,
+                    PIH.SERVICE.call_command(ServiceCommands.send_log_message,
                             (message, channel_name, level_value))
                 except Error as error:
                     PIH.output.error("Log send error")
             PIH.LOG.executor.submit(internal_send_message, value,
-                                        channel.name, level_value)
+                                        channel.name, DataTool.as_bitmask_value(level))
             return value
 
         @staticmethod
-        def send_command(value: LogCommands, parameters: Tuple = None) -> None:
-            message_commnad_description: LogCommandDescription = value.value
-            parameter_pattern_list: list = DataTool.as_list(
-                message_commnad_description.params)
-            parameters = parameters or ()
-            parameters_dict: dict = {}
-            if len(parameter_pattern_list) > len(parameters):
-                raise Exception(
-                    "Income parameter list length is less that parameter list length of command")
-            for index, parameter_pattern_item in enumerate(parameter_pattern_list):
-                parameter_pattern: ParamItem = parameter_pattern_item
-                parameters_dict[parameter_pattern.name] = parameters[index]
-
-            def internal_send_command(command_name: str, parameters: dict) -> None:
-                try:
-                    RPC.call(ServiceCommands.send_log_command,
-                            (command_name, parameters))
-                except Error as error:
-                    PIH.output.error("Log send error")
-            PIH.LOG.executor.submit(internal_send_command,
-                                        value.name, parameters_dict)
-
-        class COMMAND:
-
-            @staticmethod
-            def send(value: LogCommands, parameters: Tuple = None) -> None:
-                PIH.LOG.send_command(value, parameters)
-
-
-            @staticmethod
-            def computer_was_started(name: str) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.COMPUTER_WAS_STARTED, (name,))
-                
-            @staticmethod
-            def server_was_started(name: str) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.SERVER_WAS_STARTED, (name,))
-    
-            @staticmethod
-            def polibase_persons_with_old_format_barcode_was_detected(persons_pin: list[int]) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.POLIBASE_PERSONS_WITH_OLD_FORMAT_BARCODE_WAS_DETECTED, (len(persons_pin), persons_pin))
-
-            @staticmethod
-            def all_polibase_persons_barcode_with_old_format_was_created(persons_pin: list[int]) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.POLIBASE_ALL_PERSON_BARCODES_WITH_OLD_FORMAT_WAS_CREATED, (persons_pin,))
-
-            @staticmethod
-            def polibase_person_visit_was_registered(value: PolibasePersonVisitDS) -> None:
-                PIH.LOG.send_command(LogCommands.POLIBASE_PERSON_VISIT_WAS_REGISTERED, (
-                    value.FullName, "Предзапись" if value.pin == CONST.POLIBASE.PRERECORDING_PIN else value.pin, value))
-                
-            @staticmethod
-            def resource_accessible(resource: ResourceStatus, at_first_time: bool) -> None:
-                PIH.LOG.send_command(LogCommands.RESOURCE_ACCESSABLE, (resource.name, resource, at_first_time))
-
-            @staticmethod
-            def resource_inaccessible(resource: ResourceStatus, at_first_time: bool, reason: RESOURCE.INACCESSABLE_REASON | None = None) -> None:
-                reason_string: str = ""
-                reason_name: str | None = None
-                if not DataTool.is_empty(reason):
-                    reason_string = f"Причина: {reason.value}"
-                    reason_name =  reason.name
-                PIH.LOG.send_command(LogCommands.RESOURCE_INACCESSABLE, (resource.name, resource, at_first_time, reason_string, reason_name))
-
-            @staticmethod
-            def polibase_person_visit_notification_was_registered(visit: PolibasePersonVisitDS, notification: PolibasePersonVisitNotificationDS) -> None:
-                PIH.LOG.send_command(LogCommands.POLIBASE_PERSON_VISIT_NOTIFICATION_WAS_REGISTERED, (
-                    visit.FullName, "Предзапись" if visit.pin == CONST.POLIBASE.PRERECORDING_PIN else visit.pin, notification))
-
-            @staticmethod
-            def login() -> None:
-                login: str = PIH.session.get_login()
-                user: User = PIH.RESULT.USER.by_login(login).data
-                PIH.LOG.send_command(
-                    LogCommands.LOG_IN, (user.name, login, PIH.OS.host()))
-
-            @staticmethod
-            def whatsapp_message_received(message: WhatsAppMessage) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.WHATSAPP_MESSAGE_RECEIVED, (message,))
-
-            @staticmethod
-            def new_file_detected(path: str) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.NEW_FILE_DETECTED, (path,))
-                
-            @staticmethod
-            def new_polibase_scanned_document_detected(value: PolibaseScannedDocument):
-                PIH.LOG.send_command(LogCommands.NEW_POLIBASE_DOCUMENT_DETECTED, (value.file_path, value.pin, value.document_name))
-
-            @staticmethod
-            def start_session() -> None:
-                argv: list[str] = PIH.session.argv
-                argv_str: str = ""
-                if not DataTool.is_empty(argv):
-                    argv_str = " ".join(argv)
-                    argv_str = f"({argv_str})"
-                login: str = PIH.session.get_login()
-                user: User = PIH.RESULT.USER.by_login(login).data
-                PIH.LOG.send_command(LogCommands.SESSION_STARTED, (user.name, login,
-                                         f"{PIH.session.file_name} {argv_str}", f"{PIH.VERSION.local()}/{PIH.VERSION.remote()}", PIH.OS.host()))
-
-            @staticmethod
-            def backup_notify_about_robocopy_job_started(status: str) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.BACKUP_NOTIFY_ABOUT_ROBOCOPY_JOB_STARTED, (status, ))
-
-            @staticmethod
-            def backup_notify_about_robocopy_job_completed(status: str) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.BACKUP_NOTIFY_ABOUT_ROBOCOPY_JOB_COMPLETED, (status, ))
-
-            @staticmethod
-            def service_action(service_role_description: ServiceRoleDescription, log_command: LogCommands) -> None:
-                PIH.LOG.send_command(log_command, (service_role_description.name, service_role_description.description,
-                                         service_role_description.host, service_role_description.port, service_role_description.pid))
-
-            @staticmethod
-            def service_started(service_role_description: ServiceRoleDescription) -> None:
-                PIH.LOG.COMMAND.service_action(service_role_description, LogCommands.SERVICE_STARTED)
-            
-            @staticmethod
-            def service_starts(service_role_description: ServiceRoleDescription) -> None:
-                PIH.LOG.COMMAND.service_action(service_role_description, LogCommands.SERVICE_STARTS)
-
-            @staticmethod
-            def service_is_inaccessable_and_waiting_to_be_restarted(service_role_description: ServiceRoleDescription) -> None:
-                PIH.LOG.COMMAND.service_action(service_role_description, LogCommands.SERVICE_IS_INACCESIBLE_AND_WAITING_TO_BE_RESTARTED)
-
-            @staticmethod
-            def service_not_started(service_role_description: ServiceRoleDescription, error: str) -> None:
-                PIH.LOG.send_command(LogCommands.SERVICE_NOT_STARTED, (service_role_description.name, service_role_description.description,
-                                                                       service_role_description.host, service_role_description.port, error))
-
-            @staticmethod
-            def hr_notify_about_new_employee(login: User) -> None:
-                user: User = PIH.RESULT.USER.by_login(login).data
-                hr_user: User = ResultTool.get_first_element(
-                    PIH.RESULT.USER.by_job_position(AD.JobPisitions.HR))
-                PIH.LOG.send_command(LogCommands.HR_NOTIFY_ABOUT_NEW_EMPLOYEE, (FullNameTool.to_given_name(hr_user.name),
-                                                                                        user.name, user.mail))
-
-            @staticmethod
-            def it_notify_about_user_creation(login: str, password: str) -> None:
-                it_user_list: list[User] = PIH.RESULT.USER.by_job_position(
-                    AD.JobPisitions.IT).data
-                me_user_login: str = PIH.session.get_login()
-                it_user_list = list(
-                    filter(lambda user: user.samAccountName != me_user_login, it_user_list))
-                it_user: User = it_user_list[0]
-                user: User = PIH.RESULT.USER.by_login(login).data
-                PIH.LOG.send_command(LogCommands.IT_NOTIFY_ABOUT_CREATE_USER, (
-                    user.name, user.description, user.samAccountName, password, user.telephoneNumber, user.mail))
-                PIH.LOG.send_command(LogCommands.IT_TASK_AFTER_CREATE_NEW_USER, (FullNameTool.to_given_name(
-                    it_user.name), user.name, user.mail, password))
-
-            @staticmethod
-            def it_notify_about_mark_creation(temporary: bool, full_name: Any, tab_number: str = None) -> None:
-                name: str = FullNameTool.to_string(full_name) if isinstance(
-                    full_name, FullName) else full_name
-                mark: Mark = PIH.RESULT.MARK.by_name(name, True).data
-                telephone_number: str = PIH.DATA.FORMAT.telephone_number(
-                    mark.telephoneNumber)
-                if temporary:
-                    PIH.LOG.send_command(LogCommands.IT_NOTIFY_ABOUT_CREATE_TEMPORARY_MARK,
-                                             (name, tab_number, telephone_number))
-                else:
-                    PIH.LOG.send_command(LogCommands.IT_NOTIFY_ABOUT_CREATE_NEW_MARK, (
-                        name, telephone_number, mark.TabNumber, mark.GroupName))
-
-            @staticmethod
-            def it_notify_about_temporary_mark_return(mark: Mark, temporary_tab_number: int) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.IT_NOTIFY_ABOUT_TEMPORARY_MARK_RETURN, (mark.FullName, temporary_tab_number))
-
-            @staticmethod
-            def backup_notify_about_polibase_creation_db_dumb_start() -> None:
-                PIH.LOG.send_command(
-                    LogCommands.POLIBASE_CREATION_DB_DUMP_START)
-                
-            @staticmethod
-            def backup_notify_about_polibase_creation_db_dumb_complete() -> None:
-                PIH.LOG.send_command(
-                    LogCommands.POLIBASE_CREATION_DB_DUMP_COMPLETE)
-                
-            @staticmethod
-            def backup_notify_about_polibase_creation_archived_db_dumb_start() -> None:
-                PIH.LOG.send_command(
-                    LogCommands.POLIBASE_CREATION_ARCHIVED_DB_DUMP_START)
-                
-            @staticmethod
-            def backup_notify_about_polibase_creation_archived_db_dumb_complete() -> None:
-                PIH.LOG.send_command(
-                    LogCommands.POLIBASE_CREATION_ARCHIVED_DB_DUMP_COMPLETE)
-                
-            @staticmethod
-            def backup_notify_about_polibase_coping_archived_db_dumb_start(destination: str) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.POLIBASE_COPING_ARCHIVED_DB_DUMP_START, (destination,))
-
-            @staticmethod
-            def backup_notify_about_polibase_coping_archived_db_dumb_complete(destination: str) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.POLIBASE_COPING_ARCHIVED_DB_DUMP_COMPLETE, (destination,))
-                
-            @staticmethod
-            def backup_notify_about_polibase_coping_db_dumb_start(destination: str) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.POLIBASE_COPING_DB_DUMP_START, (destination,))
-
-            @staticmethod
-            def backup_notify_about_polibase_coping_db_dumb_complete(destination: str) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.POLIBASE_COPING_DB_DUMP_COMPLETE, (destination,))
-
-            @staticmethod
-            def it_notify_about_mark_return(mark: Mark) -> None:
-                PIH.LOG.send_command(
-                    LogCommands.IT_NOTIFY_ABOUT_MARK_RETURN, (mark.FullName, mark.TabNumber))
-
-            @staticmethod
-            def it_notify_about_create_new_mark(full_name: Any) -> None:
-                PIH.LOG.COMMAND.it_notify_about_mark_creation(
-                    False, full_name)
-
-            @staticmethod
-            def it_notify_about_create_temporary_mark(full_name: Any, tab_number: str) -> None:
-                PIH.LOG.COMMAND.it_notify_about_mark_creation(
-                    True, full_name, tab_number)
-
-            @staticmethod
-            def printer_report(name: str, location: str, report: str) -> bool:
-                return PIH.LOG.send_command(LogCommands.PRINTER_REPORT, (name, location, report))
-
-        @staticmethod
-        def debug_bot(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.DEBUG_BOT, level)
+        def debug_bot(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.DEBUG_BOT, level)
 
         @staticmethod
-        def debug(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.DEBUG, level)
+        def debug(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.DEBUG, level)
 
         @staticmethod
-        def services(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.SERVICE, level)
+        def services(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.SERVICES, level)
 
         @staticmethod
-        def resources(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.RESOURCES, level)
+        def resources(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.RESOURCES, level)
         
         @staticmethod
-        def printers(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.PRINTER, level)
+        def printers(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.PRINTER, level)
 
         @staticmethod
-        def services_bot(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.SERVICE_BOT, level)
+        def services_bot(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.SERVICE_BOT, level)
 
         @staticmethod
-        def backup(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.BACKUP, level)
+        def backup(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.BACKUP, level)
 
         @staticmethod
-        def notification(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.NOTIFICATION, level)
+        def polibase_notification(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.POLIBASE_NOTIFICATIONS, level)
 
         @staticmethod
-        def notification_bot(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.NOTIFICATION_BOT, level)
+        def polibase_notification_bot(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.POLIBASE_NOTIFICATIONS_BOT, level)
 
         @staticmethod
-        def it(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.IT, level)
+        def polibase_error_notification(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.POLIBASE_ERROR_NOTIFICATIONS, level)
 
         @staticmethod
-        def from_feedback_call_bot(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.POLIBASE_PERSON_FEEDBACK_CALL, level)
+        def polibase_error_notification_bot(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.POLIBASE_ERROR_NOTIFICATIONS_BOT, level)
 
         @staticmethod
-        def from_review_request_result(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.POLIBASE_PERSON_REVIEW_QUEST_RESULT, level)
+        def it(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.IT, level)
 
         @staticmethod
-        def it_bot(message: str, level: Any = LogLevels.DEFAULT) -> str:
-            return PIH.LOG.send_message(message, LogChannels.IT_BOT, level)
+        def it_bot(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
+            return PIH.LOG.send(message, LogMessageChannels.IT_BOT, level)
 
 
     class MESSAGE:
 
         class POLIBASE:
 
             @staticmethod
@@ -3926,24 +4523,24 @@
 
 
         class WORKSTATION:
               
             executor = ThreadPoolExecutor(max_workers=10)
 
             @staticmethod
-            def to_all_workstations(message: str, filter_group: AD.Groups = None, to_all_user_workstation_name_list: list[str] = None, session: Session = None, test: bool = True, timeout: int = 60) -> None:
+            def to_all_workstations(message: str, filter_group: AD.Groups | None = None, to_all_user_workstation_name_list: list[str] | None = None, session: Session = None, test: bool = True, timeout: int = 60) -> None:
                 session = session or PIH.session
                 filter_user_login_list: list[str] = None if filter_group is None else ResultTool.map(PIH.RESULT.USER.by_group(filter_group), lambda item: item.samAccountName.lower()).data
                 filter_user_login_list_is_empty: bool = DataTool.is_empty(filter_user_login_list)
                 to_all_user_workstation_name_list_is_empty: bool = DataTool.is_empty(
                     to_all_user_workstation_name_list)
                 def filter_function(workstation: Workstation) -> bool:
                     workstation_name: str = workstation.name.lower()
                     if test:
-                        return workstation_name == CONST.TEST.WS
+                        return workstation_name == CONST.TEST.WORKSTATION_MAME
                     return workstation.accessable and ((filter_user_login_list_is_empty or workstation.samAccountName in filter_user_login_list) or (to_all_user_workstation_name_list_is_empty or workstation_name in to_all_user_workstation_name_list))
                 def every_action(workstation: Workstation) -> None:
                     def internal_send_message(user_login: str | None, workstation_name: str, message: str) -> None:
                         if not DataTool.is_empty(to_all_user_workstation_name_list) and workstation_name in to_all_user_workstation_name_list:
                             if not test:
                                 PIH.MESSAGE.WORKSTATION.to_user_or_workstation(None, workstation_name, message, timeout)
                         else:
@@ -3951,71 +4548,59 @@
                                 if test:
                                     PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user_login, workstation_name, message, timeout)
                                 else:
                                     pass
                                 #dont send message - cause workstation is on but no one user is logged
                             else:
                                 if test:
-                                    if workstation_name == CONST.TEST.WS:
+                                    if workstation_name == CONST.TEST.WORKSTATION_MAME:
                                         PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user_login, workstation_name, message, timeout)
                                 else:
                                     PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user_login, workstation_name, message, timeout)
                     result_message: str = f"Сообщение от {session.user_given_name} ({A.D_F.description(session.get_user().description)}):"
                     result_message += f" День добрый, "
-                    user_data: dict = {"user" : None}
-                    def obtain_user_action() -> User:
-                        user: User = None
-                        try:
-                            user = A.R_U.by_login(workstation.samAccountName).data
-                            user_data["user"] = user
-                        except NotFound:
-                            pass
-                        return user
-                    if workstation.samAccountName:
-                        while_not_do(lambda: obtain_user_action() is not None)
-                    user: User | None = user_data["user"]
-                    result_message += "" if A.D_C.empty(workstation.samAccountName) else f"{FullNameTool.to_given_name(user)}, "
+                    user: User | None = None if DataTool.is_empty(workstation.samAccountName) else A.R_U.by_login(workstation.samAccountName, True, True).data
+                    result_message += DataTool.if_not_empty(user, f"{FullNameTool.to_given_name(user)}, ", "")
                     result_message += message
                     PIH.MESSAGE.WORKSTATION.executor.submit(
                         internal_send_message, workstation.samAccountName, workstation.name.lower(), result_message)
                 ResultTool.every(ResultTool.filter(PIH.RESULT.WORKSTATION.all(), filter_function), every_action)
 
             @staticmethod
-            def to_user(value: Any, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
+            def to_user(value: User | str, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
                 return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(value.samAccountName if isinstance(value, User) else value, None, message, timeout, method_type)
 
             @staticmethod
-            def to_workstation(value: Any, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
+            def to_workstation(value: WorkstationDescription | str, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
                 return PIH.MESSAGE.WORKSTATION.by_workstation_name(value.name if isinstance(value, WorkstationDescription) else value, message, timeout, method_type)
 
             @staticmethod
             def by_workstation_name(value: str, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
                 user: User = None
                 try:
                     user = PIH.RESULT.USER.by_workstation_name(value).data
-                except NotFound:
+                except NotFound as error:
                     pass
                 return PIH.MESSAGE.WORKSTATION.to_user_or_workstation(user.samAccountName if user is not None else None, value, message, timeout, method_type)
 
             @staticmethod
             def to_user_or_workstation(user_login: str, workstation_name: str, message: str, timeout: int = 60, method_type: WorkstationMessageMethodTypes = WorkstationMessageMethodTypes.REMOTE) -> bool:
-                if RPC.Service.role_description is not None and RPC.Service.role_description.name == ServiceRoles.WS.value.name:
-                    method_type = WorkstationMessageMethodTypes.LOCAL_PSTOOL_MSG
                 if method_type == WorkstationMessageMethodTypes.REMOTE:
-                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.send_message_to_user_or_workstation, (user_login, workstation_name, message, timeout)))
+                    return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.send_message_to_user_or_workstation, (user_login, workstation_name, message, timeout)))
                 def internal_send_by_login_and_workstation_name(login: str, workstation_name: str) -> None:
                     if method_type == WorkstationMessageMethodTypes.LOCAL_PSTOOL_MSG:
                         PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
                             [CONST.MSG.EXECUTOR, f"/time:{timeout}", login, message], workstation_name), False)
                     if method_type == WorkstationMessageMethodTypes.LOCAL_MSG:
                         PIH.PSTOOLS.execute_command_list(
                             [CONST.MSG.EXECUTOR, f"/time:{timeout}", login, f"/server:{workstation_name}", message], False)
                 if workstation_name is None:
-                    ResultTool.every(PIH.RESULT.WORKSTATION.by_login(
-                        user_login), lambda workstation: internal_send_by_login_and_workstation_name(user_login, workstation.name))
+                    result: Result[list[Workstation]] = PIH.RESULT.WORKSTATION.by_login(
+                        user_login)
+                    ResultTool.every(result, lambda workstation: internal_send_by_login_and_workstation_name(user_login, workstation.name))
                 else:
                     if user_login is None:
                         internal_send_by_login_and_workstation_name(
                             "*", workstation_name)
                     else:
                         internal_send_by_login_and_workstation_name(
                             user_login, workstation_name)
@@ -4033,15 +4618,15 @@
     
                     @staticmethod
                     def add(message: Message, recipient: str, sender: CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE, high_priority: bool = False) -> bool:
                         return PIH.MESSAGE.WHATSAPP.WAPPI.QUEUE.add_message(Message(message, recipient, sender.value), high_priority)
                     
                     @staticmethod
                     def add_message(message: Message, high_priority: bool = False) -> bool:
-                        return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.add_message_to_queue, (message, high_priority)))
+                        return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.add_message_to_queue, (message, high_priority)))
 
 
                 WAPPI_PROFILE_MAP: dict = None 
 
                 @staticmethod
                 def get_wappi_collection() -> dict:
                     WP = CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE
@@ -4066,15 +4651,15 @@
                     profile_id_collection = PIH.MESSAGE.WHATSAPP.WAPPI.get_wappi_collection()
                     for item in profile_id_collection:
                         if profile_id_collection[item] == telephone_number:
                             return item
                     return None
 
                 @staticmethod
-                def get_message_list(telephone_number: str, profile: Any = None) -> list[WhatsAppMessage]:
+                def get_message_list(telephone_number: str, profile: Any | None = None) -> list[WhatsAppMessage]:
                     profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                     url: str = f"{CONST.MESSAGE.WHATSAPP.WAPPI.URL_GET_MESSAGES}{profile}&chat_id={telephone_number}{CONST.MESSAGE.WHATSAPP.WAPPI.CONTACT_SUFFIX}"
                     headers: dict = {
                         "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION,
                         "Content-Type": "application/json"
                     }
                     result: list[WhatsAppMessage] = []
@@ -4088,83 +4673,81 @@
                         for message_item in response_result["messages"]:
                             if message_item["type"] == "chat":
                                 result.append(WhatsAppMessage(message_item["body"], message_item["fromMe"], str(message_item["from"]).split("@")[0], 
                                    str(message_item["to"]).split("@")[0], profile, message_item["time"]))
                     return result 
                 
                 @staticmethod
-                def send(telephone_number: str, message: Any, profile: Any = None) -> bool:
-                    #print(message)
+                def send(telephone_number: str, message: Any, profile: Any | None = None) -> bool:
                     profile = EnumTool.get_value(profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                     url: str = None
                     payload: dict = {"recipient": telephone_number}
                     if isinstance(message, str):
                         payload["body"] = message
                         url: str = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_MESSAGE
                     elif isinstance(message, (WhatsAppMessageListPayload, WhatsAppMessageButtonsPayload)):
-                        for item in message.__dataclass_fields__:
-                            item_value: Any = message.__getattribute__(item)
+                        for item_name in message.__dataclass_fields__:
+                            item_value: Any = message.__getattribute__(item_name)
                             if not DataTool.is_empty(item_value):
-                                payload[item] = item_value
+                                if item_name == "buttons":
+                                    payload[item_name] = list(map(lambda button: button.__dict__, item_value))
+                                else:
+                                    payload[item_name] = item_value
                         if isinstance(message, WhatsAppMessageListPayload):
                             url = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_LIST_MESSAGE
                         else:
                             url = CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_BUTTONS_MESSAGE
                     url += profile
                     headers: dict = {"accept": "application/json",
                                      "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION, "Content-Type": "application/json"}
                     try:
                         response: Response = requests.post(
                             url, data=json.dumps(payload), headers=headers)
                     except ConnectTimeout:
-                        #print("ConnectTimeout")
                         return False
                     if response.status_code == CONST.ERROR.WAPPI.PROFILE_NOT_PAID:
                         PIH.LOG.resources(
-                            "Аккаунт Wappi (сервис для отправики сообщений в WhatsApp) не оплачен", LogLevels.ERROR)
+                            "Аккаунт Wappi (сервис для отправики сообщений через WhatsApp) не оплачен", LogMessageFlags.ERROR)
                     status_code: int = response.status_code
-                    #print(status_code)
                     return status_code == 200
 
                 @staticmethod
-                def send_base64_file(url: str, telephone_number: str, caption: str, base64_content: str,  profile: Any = None) -> bool:
+                def send_base64_file(url: str, telephone_number: str, caption: str, file_name: str | None, base64_content: str,  profile: Any | None = None) -> bool:
                     profile = EnumTool.get_value(
                         profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                     payload: dict = {"recipient": telephone_number,
                                      "caption": caption,
                                      "b64_file": base64_content}
+                    if not DataTool.is_empty(file_name):
+                        payload["file_name"] = file_name   
                     headers: dict = {"accept": "application/json",
                                      "Authorization": CONST.MESSAGE.WHATSAPP.WAPPI.AUTHORIZATION, "Content-Type": "application/json"}
                     url = url + profile
                     try:
                         response: Response = requests.post(
                             url, data=json.dumps(payload), headers=headers)
                     except ConnectTimeout:
                         return False
                     if response.status_code == CONST.ERROR.WAPPI.PROFILE_NOT_PAID:
                         PIH.LOG.resources(
-                            "Аккаунт Wappi (сервис для отправики сообщений в WhatsApp) не оплачен", LogLevels.ERROR)
+                            "Аккаунт Wappi (сервис для отправики сообщений через WhatsApp) не оплачен", LogMessageFlags.ERROR)
                     return response.status_code == 200
 
                 @staticmethod
-                def send_video(telephone_number: str, caption: str, base64_content: str, profile: Any = None) -> bool:
-                    return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_VIDEO, telephone_number, caption, base64_content, profile)
+                def send_video(telephone_number: str, caption: str, base64_content: str, profile: Any | None = None) -> bool:
+                    return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_VIDEO, telephone_number, caption, None, base64_content, profile)
 
                 @staticmethod
-                def send_image(telephone_number: str, caption: str, base64_content: str, profile: Any = None) -> bool:
-                    return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_IMAGE, telephone_number, caption, base64_content, profile)
+                def send_image(telephone_number: str, caption: str, base64_content: str, profile: Any | None = None) -> bool:
+                    return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_IMAGE, telephone_number, caption, None, base64_content, profile)
 
                 @staticmethod
-                def send_document(telephone_number: str, caption: str, base64_content: str, profile: Any = None) -> bool:
-                    return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_DOCUMENT, telephone_number, caption, base64_content, profile)
+                def send_document(telephone_number: str, caption: str, file_name: str, base64_content: str, profile: Any | None = None) -> bool:
+                    return PIH.MESSAGE.WHATSAPP.WAPPI.send_base64_file(CONST.MESSAGE.WHATSAPP.WAPPI.URL_SEND_DOCUMENT, telephone_number, caption, file_name, base64_content, profile)
 
-            @staticmethod
-            def create_output(recipient: str) -> Output:
-                from MobileHelperCore.api import WappiOutput, WappiSession
-                return WappiOutput(WappiSession(recipient))
             
             @staticmethod
             def send_via_browser(telephone_number: str, message: str) -> bool:
                 pywhatkit_is_exists: bool = importlib.util.find_spec(
                     "pywhatkit") is not None
                 if not pywhatkit_is_exists:
                     PIH.output.green(
@@ -4175,15 +4758,15 @@
                 try:
                     import pywhatkit as pwk
                     pwk.sendwhatmsg_instantly(telephone_number, message)
                 except Exception as уrror:
                     PIH.output.error("Ошибка при отправке сообщения!")
 
             @staticmethod
-            def send(telephone_number: str, message: Any, via_wappi: bool = True, use_alternative: bool = True, wappi_profile: Any = None) -> bool:
+            def send(telephone_number: str, message: Any, via_wappi: bool = True, use_alternative: bool = True, wappi_profile: Any | None = None) -> bool:
                 wappi_profile = EnumTool.get_value(
                     wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                 result: bool = False
                 telephone_number = PIH.DATA.FORMAT.telephone_number(
                     telephone_number)
                 if via_wappi:
                     result = PIH.MESSAGE.WHATSAPP.WAPPI.send(
@@ -4191,63 +4774,105 @@
                 if result:
                     return result
                 if use_alternative or not via_wappi:
                     return PIH.MESSAGE.WHATSAPP.send_via_browser(telephone_number, message)
                 return False
 
             @staticmethod
-            def send_video(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any = None) -> bool:
+            def send_video(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any | None = None) -> bool:
                 wappi_profile = EnumTool.get_value(
                     wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                 telephone_number = PIH.DATA.FORMAT.telephone_number(telephone_number)
                 return PIH.MESSAGE.WHATSAPP.WAPPI.send_video(telephone_number, caption, base64_value, wappi_profile)
 
             @staticmethod
-            def send_image(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any = None) -> bool:
+            def send_image(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any | None = None) -> bool:
                 wappi_profile = EnumTool.get_value(
                     wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                 telephone_number = PIH.DATA.FORMAT.telephone_number(
                     telephone_number)
                 return PIH.MESSAGE.WHATSAPP.WAPPI.send_image(telephone_number, caption, base64_value, wappi_profile)
         
             @staticmethod
-            def send_document(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any = None) -> bool:
+            def send_document(telephone_number: str, caption: str, base64_value: str, wappi_profile: Any | None = None) -> bool:
                 wappi_profile = EnumTool.get_value(
                     wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value)
                 telephone_number = PIH.DATA.FORMAT.telephone_number(
                     telephone_number)
                 return PIH.MESSAGE.WHATSAPP.WAPPI.send_document(telephone_number, caption, base64_value, wappi_profile)
 
             @staticmethod
-            def send_to_user(user: User, message: Any, via_wappi: bool = True, use_alternative: bool = True, wappi_profile: Any = None) -> bool:
+            def send_to_user(user: User, message: Any, via_wappi: bool = True, use_alternative: bool = True, wappi_profile: Any | None = None) -> bool:
                 return PIH.MESSAGE.WHATSAPP.send(user.telephoneNumber, message, via_wappi, use_alternative, EnumTool.get_value(
                     wappi_profile, CONST.MESSAGE.WHATSAPP.WAPPI.PROFILE.DEFAULT.value))
 
         class DELAYED:
 
             @staticmethod
             def register(message: DelayedMessage) -> int:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.register_delayed_message, PIH.ACTION.MESSAGE.DELAYED.prepeare_message(message)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.register_delayed_message, PIH.ACTION.MESSAGE.DELAYED.prepeare_message(message)))
 
             @staticmethod
             def send(message: DelayedMessage, high_priority: bool = True) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.send_delayed_message, (PIH.ACTION.MESSAGE.DELAYED.prepeare_message(message), high_priority)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.send_delayed_message, (PIH.ACTION.MESSAGE.DELAYED.prepeare_message(message), high_priority)))
             
     
     class ACTION:
 
+        class ACTIONS:
+
+            @staticmethod
+            def done(action: Actions | str, user_login: str) -> bool | None:
+                user: User = A.R_U.by_login(user_login, True, True).data
+                _action: Actions | None = PIH.CHECK.ACTIONS.get(action)
+                if DataTool.is_none(_action):
+                    return None
+                PIH.EVENT.send(Events.ACTION_WAS_DONE, (_action.value.description, _action.name, user.name, user_login))
+                return True
+
+            @staticmethod
+            def have_to_be_done(action: Actions | str) -> bool | None:
+                _action: Actions | None = PIH.CHECK.ACTIONS.get(action)
+                if DataTool.is_none(_action):
+                    return None
+                PIH.EVENT.send(Events.ACTION_HAVE_TO_BE_DONE, (_action.name, _action.value.description))
+                return True
+
+        class EVENTS:
+    
+            @staticmethod
+            def register(value: Events, parameters: dict | None = None) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.register_event, (EventDS(value.name, parameters, DateTimeTool.now()), )))
+
+            @staticmethod
+            def update(value: Events, parameter_for_search: tuple[Any], parameters: tuple[Any]) -> bool:
+                return PIH.ACTION.EVENTS.remove(value, parameter_for_search) and PIH.ACTION.EVENTS.register(value, PIH.EVENT.BULDER.create_parameters_map(value, parameters))
+
+            @staticmethod
+            def remove(value: Events, parameters: tuple[Any]) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.remove_event, EventDS(value.name, PIH.EVENT.BULDER.create_parameters_map(value, parameters, check_for_parameters_count=False))))
+
+        class NOTES:
+        
+            @staticmethod
+            def create(name: str, note: Note) -> bool:
+                id: str | None = DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_note, (note, )))
+                if DataTool.is_empty(id):
+                    return False
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.add_gkeep_map_item, (name, id)))
+
         class QR_CODE:
 
             @staticmethod
             def titled(data: str, title, path: str, font_size: int | None = None) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_qr_code, (data, title, path, font_size)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_qr_code, (data, title, path, font_size)))
 
             @staticmethod
             def print(path: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.print_image, (path, )))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.print_image, (path, )))
 
             @staticmethod
             def for_mobile_helper_command(value: str, title: str, path: str, font_size: int | None = None) -> bool:
                 return PIH.ACTION.QR_CODE.titled(PIH.DATA.FORMAT.mobile_helper_qr_code_text(PIH.DATA.FORMAT.mobile_helper_command(value)), title, path, font_size)
             
             @staticmethod
             def for_polibase_person_card_registry_folder(name: str) -> bool:
@@ -4255,51 +4880,58 @@
                 return PIH.ACTION.QR_CODE.for_mobile_helper_command(" ".join(["card", "registry", name]), name, PIH.PATH.QR_CODE.polibase_person_card_registry_folder(name), 80)
 
         class INDICATION:
 
             class CT:
 
                 @staticmethod
-                def register(value: CTIndicationValue) -> bool:
-                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.register_ct_indications_value, (value), ))
+                def register(value: CTIndicationsValue, forced: bool = False) -> bool:
+                    return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.register_ct_indications_value, (value, forced)))
+
+            class CHILLER:
+                    
+                @staticmethod
+                def register(value: ChillerIndicationsValue, forced: bool = False) -> bool:
+                    data: dict = PIH.SERVICE.call_command(ServiceCommands.register_chiller_indications_value, (value, forced))
+                    return not DataTool.is_empty(data)
 
         class MOBILE_HELPER:
 
             @staticmethod
-            def send_message(name: str, telephone_number: str) -> None:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.send_mobile_helper_message, (name, telephone_number)))
+            def send_message(value: str, recipient: str | Enum) -> bool:    
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.send_mobile_helper_message, (value, recipient if isinstance(recipient, str) else EnumTool.get(recipient))))
 
         class BACKUP:
 
             @staticmethod
             def start_robocopy_job(name: str = None, source: str = None, destination: str = None, force: bool = False) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.robocopy_start_job, (name, source, destination, force)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.robocopy_start_job, (name, source, destination, force)))
 
             @staticmethod
             def start_robocopy_job_by_name(value: str, force: bool = False) -> bool:
                 return PIH.ACTION.BACKUP.start_robocopy_job(value, force=force)
 
         class DATA_STORAGE:
 
             @staticmethod
-            def value(value: object, name: str = None, section: str = None) -> bool:
+            def value(value: Any, name: str = None, section: str = None) -> bool:
                 try:
                     name = name or value.__getattribute__("name")
                 except AttributeError as error:
                     pass
                 else:
-                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_storage_value, (name, value, section)))
+                    return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_storage_value, (name, value, section)))
 
         class MESSAGE:
 
             class DELAYED:
 
                 @staticmethod
                 def update(value: DelayedMessageDS, search_critery: MessageSearchCritery) -> bool:
-                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.update_delayed_message, (value, search_critery)))
+                    return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.update_delayed_message, (value, search_critery)))
 
                 @staticmethod
                 def update_status(value: DelayedMessageDS, status: MessageStatuses) -> bool:
                     return PIH.ACTION.MESSAGE.DELAYED.update(DelayedMessageDS(status=status.value), MessageSearchCritery(id=value.id))
 
                 @staticmethod
                 def complete(value: DelayedMessageDS) -> bool:
@@ -4326,71 +4958,76 @@
                     return message
         
         class SETTINGS:
 
             @staticmethod
             def key(key: str, value: Any) -> bool:
                 return DataTool.rpc_unrepresent(
-                    RPC.call(ServiceCommands.set_settings_value, (key, value)))
+                    PIH.SERVICE.call_command(ServiceCommands.set_settings_value, (key, value)))
 
             @staticmethod
             def set(settings_item: SETTINGS, value: Any) -> bool:
                 return PIH.ACTION.SETTINGS.key(settings_item.value.key_name or settings_item.name, value)
 
             @staticmethod
             def set_default(settings_item: SETTINGS) -> bool:
                 return PIH.ACTION.SETTINGS.set(settings_item, settings_item.value.default_value)
 
         class USER:
 
             @staticmethod
+            def drop_user_cache() -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.drop_user_cache))
+
+
+            @staticmethod
             def create_from_template(container_dn: str,
                                      full_name: FullName, login: str, password: str, description: str, telephone: str, email: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_user_by_template, (container_dn, full_name, login, password, description, telephone, email)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_user_by_template, (container_dn, full_name, login, password, description, telephone, email)))
 
             @staticmethod
             def create_in_container(container_dn: str,
                                     full_name: FullName, login: str, password: str, description: str, telephone: str, email: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_user_in_container, (container_dn, full_name, login, password, description, telephone, email)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_user_in_container, (container_dn, full_name, login, password, description, telephone, email)))
 
             @staticmethod
             def set_telephone_number(user: User, telephone: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_user_telephone, (user.distinguishedName, telephone)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_user_telephone_number, (user.distinguishedName, telephone)))
 
             @staticmethod
             def set_password(user: User, password: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_user_password, (user.distinguishedName, password)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_user_password, (user.distinguishedName, password)))
 
             @staticmethod
-            def set_status(user: User, status: str, container: UserContainer) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_user_status, (user.distinguishedName, status, DataTool.check(container, lambda: container.distinguishedName))))
+            def set_status(user: User, status: str, container: UserBase) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_user_status, (user.distinguishedName, status, DataTool.check(container, lambda: container.distinguishedName))))
 
             @staticmethod
             def remove(user: User) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.remove_user, user.distinguishedName))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.remove_user, user.distinguishedName))
 
         class TIME_TRACKING:
 
             @staticmethod
-            def save_report(path: str, start_date: datetime, end_date: datetime, tab_number_list: list[str] = None, plain_format: bool = False) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.save_time_tracking_report, (path, DateTimeTool.start_date(start_date), DateTimeTool.end_date(end_date), tab_number_list, plain_format)))
+            def save_report(path: str, start_date: datetime, end_date: datetime, tab_number_list: list[str] | None = None, plain_format: bool = False) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.save_time_tracking_report, (path, DateTimeTool.start_date(start_date), DateTimeTool.end_date(end_date), tab_number_list, plain_format)))
 
         class INVENTORY:
 
             @staticmethod
             def create_barcodes(report_file_path: str, result_directory: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_barcodes_for_inventory, (report_file_path, result_directory)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_barcodes_for_inventory, (report_file_path, result_directory)))
 
             @staticmethod
             def save_report_item(report_file_path: str, item: InventoryReportItem) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.save_inventory_report_item, (report_file_path, item)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.save_inventory_report_item, (report_file_path, item)))
 
             @staticmethod
             def close_report(report_file_path: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.close_inventory_report, report_file_path))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.close_inventory_report, report_file_path))
 
         class PRINTER:
 
             @staticmethod
             def report() -> bool:
                 return not ResultTool.is_empty(PIH.RESULT.PRINTER.report())
 
@@ -4399,145 +5036,167 @@
                 return not ResultTool.is_empty(PIH.RESULT.PRINTER.status())
 
         class POLIBASE:
 
             executor: ThreadPoolExecutor = ThreadPoolExecutor(max_workers=10)
 
             @staticmethod
-            def program_close_for_all(notify: bool = True, notification_message: str | None = None, test: bool = True) -> None:
+            def client_program_close_for_all(notify: bool = True, notification_message: str | None = None, test: bool = True) -> None:
                 def close_action(workstation: Workstation) -> None:
                     PIH.ACTION.POLIBASE.client_program_close_for_workstation(workstation)
                 def filter_function(workstation: Workstation) -> bool:
-                    return workstation.name == CONST.TEST.WS if test else workstation.accessable 
+                    return workstation.name == CONST.TEST.WORKSTATION_MAME if test else workstation.accessable 
                 def every_action(workstation: Workstation) -> None:
                     PIH.ACTION.POLIBASE.executor.submit(close_action, workstation)
                 if notify:
                     PIH.MESSAGE.POLIBASE.notify_about_polibase_closing(notification_message, test)
                 ResultTool.every(ResultTool.filter(PIH.RESULT.WORKSTATION.all(), filter_function), every_action)
 
             @staticmethod
             def client_program_close_for_workstation(workstation: Workstation) -> bool:
                 return PIH.ACTION.WORKSTATION.kill_process(
                     CONST.POLIBASE.PROCESS_NAME, workstation.name)
 
             def restart(test: bool = True) -> None:
-                PIH.PSTOOLS.reboot(HOSTS.POLIBASE_TEST.NAME if test else HOSTS.POLIBASE.NAME)
+                PIH.PSTOOLS.ws_reboot(HOSTS.POLIBASE_TEST.NAME if test else HOSTS.POLIBASE.NAME)
 
             class NOTIFICATION:
 
                 @staticmethod
                 def register(value: PolibasePersonVisitNotificationDS) -> bool:
-                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.register_polibase_person_visit_notification, value))
+                    return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.register_polibase_person_visit_notification, value))
 
                 class CONFIRMATION:
 
                     @staticmethod
                     def update(recepient: str, sender: str, status: int) -> bool:
-                        return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.update_polibase_person_notification_confirmation, PolibasePersonNotificationConfirmation(recepient, sender, status)))
+                        return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.update_polibase_person_notification_confirmation, PolibasePersonNotificationConfirmation(recepient, sender, status)))
 
             class INFORMATION_QUEST:
 
                 @staticmethod
                 def register(person: PolibasePerson) -> bool:
-                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.register_polibase_person_information_quest, PolibasePersonInformationQuest(person.pin, person.FullName, person.telephoneNumber)))
+                    return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.register_polibase_person_information_quest, PolibasePersonInformationQuest(person.pin, person.FullName, person.telephoneNumber)))
                 
                 @staticmethod
-                def start(person: PolibasePerson) -> bool:
-                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.start_polibase_person_information_quest, (person.pin, )))
+                def start(person_or_pin: PolibasePerson | int) -> bool:
+                    return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.start_polibase_person_information_quest, (person_or_pin if isinstance(person_or_pin, int) else person_or_pin.pin, )))
 
                 @staticmethod
                 def update(value: PolibasePersonInformationQuest, search_critery: PolibasePersonInformationQuest) -> bool:
-                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.update_polibase_person_information_quest, (value, search_critery)))
+                    return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.update_polibase_person_information_quest, (value, search_critery)))
 
             @staticmethod
-            def create_barcode_for_person(pid: int, test: bool = None) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_barcode_for_polibase_person, (pid, test)))
+            def create_barcode(person: PolibasePerson, test: bool | None = None) -> bool:
+                return PIH.ACTION.POLIBASE.create_barcode_by_person_pin(person.pin, test)
+            
+            @staticmethod
+            def create_barcode_by_person_pin(value: int, test: bool | None = None) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_barcode_for_polibase_person, (value, test)))
 
             @staticmethod
-            def set_card_folder_for_person(name: str, pid: int, test: bool = None) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_polibase_person_card_folder_name, (name, pid, test)))
+            def set_card_folder_name(value: str, person_or_pin: PolibasePerson | int, test: bool | None = None) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_polibase_person_card_folder_name, (value, person_or_pin.pin if isinstance(person_or_pin, PolibasePerson) else person_or_pin, test)))
 
             @staticmethod
-            def set_email(value: str, pin: int, test: bool = None) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_polibase_person_email, (value, pin, test)))
+            def set_email(value: str, person: PolibasePerson, test: bool | None = None) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_polibase_person_email, (value, person.pin, test)))
+            
+            @staticmethod
+            def set_telephone_number(index: int, value: str, person: PolibasePerson, test: bool | None = None) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_polibase_person_telephone_number, (index, value, person.pin, test)))
 
             @staticmethod
-            def set_person_barcode_by_pin(barcode_file_name: str, pin: int, test: bool = None) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_polibase_person_barcode_by_pin, (barcode_file_name, pin, test)))
+            def set_person_barcode(value: str, person: PolibasePerson, test: bool | None = None) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_polibase_person_barcode_by_pin, (value, person.pin, test)))
 
             class DB:
 
                 @staticmethod
-                def backup(dump_file_name: str = None, test: bool = None) -> bool:
-                    return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_polibase_database_backup, (dump_file_name, test)))
+                def backup(dump_file_name: str = None, test: bool | None = None) -> bool:
+                    return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_polibase_database_backup, (dump_file_name, test)))
 
             class VISIT:
 
                 class DATA_STORAGE:
 
                     @staticmethod
                     def update(value: PolibasePersonVisitDS) -> bool:
-                        return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.update_polibase_person_visit_to_data_stogare, value))
+                        return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.update_polibase_person_visit_to_data_stogare, value))
 
         class MARK:
 
             @staticmethod
             def create(full_name: FullName, person_division_id: int,  tab_number: str, telephone: str = None) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_mark, (full_name, person_division_id, tab_number, telephone)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_mark, (full_name, person_division_id, tab_number, telephone)))
 
             @staticmethod
             def set_full_name_by_tab_number(full_name: FullName, tab_number: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_full_name_by_tab_number, (full_name, tab_number)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_full_name_by_tab_number, (full_name, tab_number)))
 
             @staticmethod
             def set_telephone_by_tab_number(telephone: str, tab_number: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.set_telephone_by_tab_number, (telephone, tab_number)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.set_telephone_by_tab_number, (telephone, tab_number)))
 
             @staticmethod
             def make_as_free_by_tab_number(tab_number: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.make_mark_as_free_by_tab_number, tab_number))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.make_mark_as_free_by_tab_number, tab_number))
 
             @staticmethod
             def make_as_temporary(temporary_mark: Mark, owner_mark: Mark) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.make_mark_as_temporary, (temporary_mark.TabNumber, owner_mark.TabNumber)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.make_mark_as_temporary, (temporary_mark.TabNumber, owner_mark.TabNumber)))
 
             @staticmethod
             def remove(mark: Mark) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.remove_mark_by_tab_number, mark.TabNumber))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.remove_mark_by_tab_number, mark.TabNumber))
 
         class DOCUMENTS:
 
             @staticmethod 
             def save_base64_as_image(path: str, content: str) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.save_base64_as_image, (path, content)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.save_base64_as_image, (path, content)))
 
             @staticmethod
             def create_for_user(path: str, full_name: FullName, tab_number: str, pc: LoginPasswordPair, polibase: LoginPasswordPair, email: LoginPasswordPair) -> bool:
                 locale.setlocale(locale.LC_ALL, 'ru_RU')
                 date_now = datetime.now().date()
                 date_now_string = f"{date_now.day} {calendar.month_name[date_now.month]} {date_now.year}"
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.create_user_document, (path, date_now_string, CONST.SITE_ADDRESS, CONST.SITE_PROTOCOL + CONST.SITE_ADDRESS, CONST.MAIL_ADDRESS, full_name, tab_number, pc, polibase, email)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.create_user_document, (path, date_now_string, CONST.SITE_ADDRESS, CONST.SITE_PROTOCOL + CONST.SITE_ADDRESS, CONST.EMAIL_ADDRESS, full_name, tab_number, pc, polibase, email)))
 
         class WORKSTATION:
     
             @staticmethod
             def reboot(host: str = None, force: bool = False) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.reboot, (host, force)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.reboot, (host, force)))
 
             @staticmethod
             def shutdown(host: str = None, force: bool = False) -> bool:
-                return DataTool.rpc_unrepresent(RPC.call(ServiceCommands.shutdown, (host, force)))
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.shutdown, (host, force)))
             
             @staticmethod
-            def kill_process(process_name: str, host: str) -> bool:
-                return PIH.PSTOOLS.kill_process(process_name, host)
-
+            def kill_process(name_or_pid: str | int, host: str, via_taskkill: bool = True) -> bool:
+                return DataTool.rpc_unrepresent(PIH.SERVICE.call_command(ServiceCommands.kill_process, (name_or_pid, host, via_taskkill)))
+            
+            @staticmethod
+            def kill_python_process(host: str, via_taskkill: bool = False) -> bool:
+                return PIH.ACTION.WORKSTATION.kill_process(A.CT.PYTHON.EXECUTOR, host, via_taskkill)   
+            
+            @staticmethod
+            def stop_windows_service(name: str, workstation_name: str) -> bool | None:
+                accessable: bool | None = PIH.CHECK.WORKSTATION.accessibility(workstation_name)
+                if DataTool.is_none(accessable):
+                    return None
+                return PIH.PSTOOLS.stop_windows_service(name, workstation_name)      
+            
             @staticmethod
-            def kill_process_via_windows(process_name: str, host: str) -> bool:
-                return PIH.PSTOOLS.kill_process_via_windows(process_name, host)
+            def start_windows_service(name: str, workstation_name: str) -> bool | None:
+                accessable: bool | None = PIH.CHECK.WORKSTATION.accessibility(workstation_name)
+                if DataTool.is_none(accessable):
+                    return None
+                return PIH.PSTOOLS.start_windows_service(name, workstation_name)      
 
 class ActionStack(list):
 
     def __init__(self, caption: str = "", *argv, input: InputBase = None, output: OutputBase = None):
         self.input = input or PIH.input
         self.output = output or PIH.output
         self.acion_value_list: list[ActionValue] = []
@@ -4588,47 +5247,56 @@
             for action_value in self.acion_value_list:
                 self.output.value(action_value.caption, action_value.value)
             if self.input.yes_no("Данные верны", True):
                 break
             else:
                 self.show_action_values()
 
-
 class A:
 
     root = PIH()
 
-    MH = root.MOBILE_HELPER
+    MIO = root.MIO
+
+    IW = root.INPUT_WAIT
 
     R = root.RESULT
     D = root.DATA
     D_TN = D.TELEPHONE_NUMBER
+    D_MR = D.MATERIALIZED_RESOURCES
     D_FL = D.FILTER
     D_E = D.EXTRACT
-    D_E_SPL = D_E.SERVICE_PARAMETER_LIST
+    D_E_E = D_E.EVENT
     D_M = D.MARK
     D_C = D.CHECK
     A = root.ACTION
     A_D = A.DOCUMENTS
     A_QR = A.QR_CODE
     A_I = A.INDICATION
     A_I_CT = A_I.CT
+    A_I_CH = A_I.CHILLER
     ME = root.MESSAGE
     ME_P = ME.POLIBASE
     A_WS = A.WORKSTATION
     R_ME = R.MESSAGE
     R_R = R.RESOURCES
+    R_RCG = R.RECOGNIZE
     R_SSH = R.SSH
     R_I = R.INDICATIONS
+    R_N = R.NOTES
+    R_E = R.EVENTS
     #
     A_ME = A.MESSAGE
+    A_ACT = A.ACTIONS
     A_TT = A.TIME_TRACKING
-    A_MH = A.MOBILE_HELPER
+    A_MIO = A.MOBILE_HELPER
     R_ME_D = R_ME.DELAYED
     A_ME_D = A_ME.DELAYED
+    A_N = A.NOTES
+    A_E = A.EVENTS
     
     #
     ME_WS = ME.WORKSTATION
     ME_P = ME.POLIBASE
     ME_WH = ME.WHATSAPP
     ME_D = ME.DELAYED
     ME_WH_W = ME_WH.WAPPI
@@ -4640,34 +5308,38 @@
     S_P = S.POLIBASE
     S_R = S.RESOURCE
     S_WS = S.WORKSTATION
     S_P_V = S_P.VISIT
     S_P_RN = S_P.REVIEW_NOTIFICATION
     #
     C = root.CHECK
+    C_ACT = C.ACTIONS
     C_R = C.RESOURCE
     C_I = C.INDICATION
     C_M = C.MARK
     C_TT = C.TIME_TRACKING
     C_A = C.ACCESS
     C_S = C.SETTINGS
     C_WS = C.WORKSTATION
     C_ME = C.MESSAGE
     C_ME_WH = C_ME.WHATSAPP
     C_ME_WH_W = C_ME_WH.WAPPI
+    C_N = C.NOTES
+    C_RCG = C.RECOGNIZE
     #
     A_M = A.MARK
     R_M = R.MARK
     R_U = R.USER
     R_TT = R.TIME_TRACKING
     A_U = A.USER
     C_U = C.USER
     D_F = D.FORMAT
     D_CO = D.CONVERT
     A_P = A.POLIBASE
+    C_E = C.EVENTS
     C_P = C.POLIBASE
     C_P_DB = C_P.DATABASE
     D_P = D.POLIBASE
     R_P = R.POLIBASE
     R_PR = R.PRINTER
     #
     A_P_V = A_P.VISIT
@@ -4694,40 +5366,62 @@
     SE = root.session
     A_DS = A.DATA_STORAGE
     R_DS = R.DATA_STORAGE
     V = root.VERSION
     OS = root.OS
     U = root.UPDATER
     PS = root.PSTOOLS
-    E = root.ERROR
-    EV = root.EVENT
+    ER = root.ERROR
+    E = root.EVENT
+    E_B = E.BULDER
     PTH = root.PATH
     PTH_U = PTH.USER
+    PTH_P = PTH.POLIBASE
     PTH_QR = PTH.QR_CODE
     PTH_FNT = PTH.FONTS
+    PTH_I = PTH.INDICATIONS
     L = root.LOG
-    L_C = L.COMMAND
 
     CT = CONST
+    CT_MR = MATERIALIZED_RESOURCES
+    CT_WINDOWS = WINDOWS
+    CT_SCN = SCAN
+    CT_EVM = EMAIL_VERIFICATION_METHODS
+    CT_D = DATA
+    CT_DT = DocumentTypes
+    CT_RBK = ROBOCOPY
+    CT_H = HOSTS
     CT_FNT = FONT
     CT_SR = ServiceRoles
     CT_SC = ServiceCommands
+    CT_SubT = SubscribtionTypes
     CT_F = FILE
-    CT_R = RESOURCE
+    CT_R = RESOURCES
     CT_R_D = CT_R.DESCRIPTIONS
-    CT_R_IR = CT_R.INACCESSABLE_REASON
+    CT_R_IR = CT_R.INACCESSABLE_REASONS
     CT_F_E = CT_F.EXTENSION
     CT_P = CT.POLIBASE
     CT_P_DD = CT_P.DOCUMENT_DESCRIPTIONS
+    CT_FC = FIELD_COLLECTION
     CT_S = SETTINGS
     CT_ME = CT.MESSAGE
     CT_ME_WH = CT_ME.WHATSAPP
     CT_ME_WH_W = CT_ME_WH.WAPPI
+    CT_L_ME_F = LogMessageFlags
+    CT_L_ME_CH = LogMessageChannels
     CT_V = CT.VISUAL
-    CT_LC = LogCommands
-    CT_MD = MEDICAl_DOCUMENT
+    CT_E = Events
+    CT_A = Actions
+    CT_MD = MEDICAL_DOCUMENT
     CT_MD_DT = CT_MD.DIRECTION_TYPES
     CT_DS = CT.DATA_STORAGE
     CT_FNC = FIELD_NAME_COLLECTION
     CT_FCA = FIELD_COLLECTION_ALIAS
-    CT_LL = LogLevels
-    CT_AD = AD
+    CT_UP = USER_PROPERTIES
+    CT_AD = AD
+    CT_AD_U = AD.USER
+    CT_I = INDICATIONS
+    C_P_DB = C_P.DATABASE
+    D_P = D.POLIBASE
+    R_P = R.POLIBASE
+    R_PR = R.PRINTER
+    #
```

### Comparing `pih-1.43/pih/rpcCommandCall_pb2.py` & `pih-1.45/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.43/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.45/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.43/pih/service_example.py` & `pih-1.45/pih/service_example.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import importlib.util
 import sys
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
 from pih import A
-from pih.const import ServiceRoles
+
+SR = A.CT_SR
+SC = A.CT_SC
 
 #version 1.0
 
-ROLE: ServiceRoles = ServiceRoles.DEVELOPER
-if A.U.update_for_service(ROLE, False, True, True):
+ROLE: SR = SR.DEVELOPER
+if A.U.update_for_service(ROLE):
 
     from typing import Any
-    from pih.const import ServiceCommands as SC
-    from pih.tools import EnumTool, ParameterList
+    from pih.tools import ParameterList
 
-    def handler_or_server_name(command_name: str, parameter_list: ParameterList, context) -> Any:
-        sc: SC = EnumTool.get(SC, command_name)       
+    def service_call_handler(sc: SC, parameter_list: ParameterList) -> Any:     
         return None
     
-
-    def service_started_handler() -> None:
-        pass
+    def service_starts_handler() -> None:
+        A.SRV_A.subscribe_on(SC.print_image)
        
-    A.SRV_A.serve(ROLE, handler_or_server_name, False, service_started_handler)
+    A.SRV_A.serve(ROLE, service_call_handler, service_starts_handler)
```

### Comparing `pih-1.43/pih/tools.py` & `pih-1.45/pih/tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,47 @@
+import enum
 from enum import Enum
 import ntpath
 from datetime import date, datetime, timedelta
 import importlib.util
 import pathlib
 import platform
 import re
 import string
 import random
 import json
 import os
+from os import walk
+from operator import itemgetter
 import subprocess
 import sys
 from typing import Any, Callable, Tuple, List
 import dataclasses
 import socket
 from typing import Any
+import inspect
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
-from pih.const import PASSWORD_GENERATION_ORDER, FIELD_COLLECTION_ALIAS
+from pih.const import PASSWORD_GENERATION_ORDER, FIELD_COLLECTION_ALIAS, CONST
 from pih.collection import R, T, FieldItem, FieldItemList, FullName, Result, User, PolibasePerson
 
 class EnumTool:
 
     @staticmethod
-    def get(cls: Enum, key: str, default_value: Any = None) -> Any:
+    def get(cls: Enum, key: str | None = None, default_value: Any | None = None, return_value: bool = True) -> Any | None:
+        if return_value and DataTool.is_empty(key):
+            return cls.value
         if key not in cls._member_map_:
             return default_value
         return cls._member_map_[key]
 
     @staticmethod
-    def get_by_value(cls: Enum, value: Any, default_value: str = None) -> Any:
+    def get_by_value(cls: Enum, value: Any, default_value: Any | None = None) -> Any | None:
         if isinstance(value, Enum):
             return value
         map: Any = cls._value2member_map_
         return default_value if value not in map else map[value]
     
     @staticmethod
     def get_by_value_or_key(cls: Enum, value: Any) -> Any:
@@ -46,43 +52,56 @@
         if value is not None and isinstance(value, Enum):
             return value.value
         return value or default_value
 
 class DataTool:
 
     @staticmethod
+    def as_bitmask_value(value: int | tuple[Enum] | Enum | list[Enum] | list[int]) -> int:
+        value_list: list[Enum | int] = None
+        if isinstance(value, (list, tuple)):
+            value_list = value
+        elif isinstance(value, (int, Enum)):
+            value_list = [value]
+        return BitMask.set(value_list)
+
+    @staticmethod
     def by_index(data: list | None, index: int, default_value: Any = None) -> Any:
         if data is None:
             return default_value
         if len(data) <= index:
             return default_value
         return data[index]
 
     @staticmethod
-    def represent(data: FieldItemList) -> str:
-        return json.dumps(data, cls=PIHEncoder)
+    def represent(data: dict, ensure_ascii: bool = True) -> str:
+        return json.dumps(data, cls=PIHEncoder, ensure_ascii=ensure_ascii)
 
     @staticmethod
-    def rpc_represent(data: dict) -> str:
-        return json.dumps(data, cls=PIHEncoder) if data is not None else ""
+    def rpc_represent(data: dict) -> str | None:
+        return json.dumps(data, cls=PIHEncoder) if data is not None else None
 
     @staticmethod
-    def rpc_unrepresent(value: str) -> dict:
-        return json.loads(value) if value is not None and value != "" else None
+    def rpc_unrepresent(value: str | None) -> dict | None:
+        return None if DataTool.is_empty(value) else json.loads(value) 
 
     @staticmethod
-    def to_result(result_string: str, class_type_holder: Any = None, first_data_item: bool = False) -> Result:
+    def to_result(result_string: str, class_type_holder: Any | Callable[[Any], Any] | None = None, first_data_item: bool = False) -> Result:
         result_object: dict = DataTool.rpc_unrepresent(result_string)
         if result_object is None:
             return Result(None, None)
         data: dict = result_object["data"]
         data = DataTool.get_first_item(data) if first_data_item else data
-        def obtain_data():
-            return (list(map(lambda item: DataTool.fill_data_from_source(class_type_holder(item) if callable(class_type_holder) else class_type_holder(), item), data)) if isinstance(data, list)
-                    and class_type_holder is not None else DataTool.fill_data_from_source(class_type_holder(data) if callable(class_type_holder) else class_type_holder(), data) if class_type_holder is not None else data) if data is not None else None
+        def fill_data_with(item: Any) -> Any:
+            if DataTool.is_empty(class_type_holder):
+                return item
+            return class_type_holder(item) if callable(class_type_holder) and not inspect.isclass(class_type_holder) else DataTool.fill_data_from_source(
+                class_type_holder() if inspect.isclass(class_type_holder) else class_type_holder, item)
+        def obtain_data() -> Any | None:
+            return list(map(fill_data_with, data)) if isinstance(data, list) else fill_data_with(data)
         if "fields_alias" in result_object:
             return Result(FieldItemList(EnumTool.get(FIELD_COLLECTION_ALIAS, result_object["fields_alias"]).value), obtain_data())
         else:
             fields = None if "fields" not in result_object else result_object["fields"]
         field_list: list[FieldItem] = None
         if fields is not None:
             field_list = []
@@ -96,20 +115,23 @@
         if isinstance(value, (list, Tuple)):
             return value
         if DataTool.is_empty(value):
             return [] 
         return [value]
 
     @staticmethod
-    def to_list(value: Any) -> list[Any]:
-        result: list[Any] = []
+    def to_list(value: dict | Enum, key_as_value: bool = False) -> list[Any]:
+        if isinstance(value, dict):
+            return [key if key_as_value else item for key, item in value.items()]
+        result: list[Any | str] = []
         for item in value:
-            result.append(item)
+            result.append(item.name if key_as_value else item.value)
         return result
 
+
     @staticmethod
     def triple_bool(value: bool, false_result: Any, true_result: Any, none_reult: Any) -> Any:
         if value is None:
             return none_reult
         return true_result if value else false_result
 
     @staticmethod
@@ -121,65 +143,99 @@
         return join_symbol.join(obj.__dict__.values())
 
     @staticmethod
     def to_data(obj: object) -> dict:
         return obj.__dict__
 
     @staticmethod
-    def fill_data_from_source(data: object, source: Any) -> object:
+    def fill_data_from_source(destination: object, source: Any, copy_by_index: bool = False, skip_not_none: bool = False) -> object | None:
         if dataclasses.is_dataclass(source):
             source = source.__dict__
-        if source is not None:
-            for item in data.__dataclass_fields__:
-                if item in source:
-                    data.__setattr__(item, source[item])
-        else:
+        if source is None:
             return None
-        return data
+        else:
+            if copy_by_index:
+                [setattr(destination, key.name, [source[key] for key in source][index])
+                 for index, key in enumerate(dataclasses.fields(destination))]
+            else:
+                for field in destination.__dataclass_fields__:
+                    if field in source:
+                        if not skip_not_none or DataTool.is_empty(destination.__getattribute__(field)):
+                            destination.__setattr__(field, source[field])
+        return destination
 
     @staticmethod
-    def fill_data_from_list_source(class_type, source: list) -> object:
-        return list(map(lambda item: DataTool.fill_data_from_source(class_type(), item), source))
+    def fill_data_from_list_source(class_type, source: list[Any] | dict[str, Any]) -> Any | None:
+        if source is None:
+            return None
+        return list(map(lambda item: DataTool.fill_data_from_source(class_type(), item), source if isinstance(source, list) else source.values()))
 
+    @staticmethod
     def fill_data_from_rpc_str(data: T, source: str) -> T:
         return DataTool.fill_data_from_source(data, DataTool.rpc_unrepresent(source))
 
     @staticmethod
-    def get_first_item(value: list[T] | T, default_value: Any = None) -> Any:
-        return DataTool.check(value is not None and len(value) > 0, lambda: value[0], default_value) if isinstance(value, list) else value or default_value
+    def get_first_item(value: list[T] | T, default_value: Any | None = None) -> T | Any | None:
+        return DataTool.check(not DataTool.is_empty(value), lambda: value[0], default_value) if isinstance(value, (list, tuple)) else value or default_value
+
+    @staticmethod
+    def check(check_value: bool, true_value: Callable[[None], Any | None] | Any, false_value: Callable[[None], Any | None] | Any | None = None) -> Any | None:
+        return (true_value() if callable(true_value) else true_value) if check_value else (false_value() if not DataTool.is_none(false_value) and callable(false_value) else false_value)
 
     @staticmethod
-    def check(check_value: bool, return_value: Callable, default_value: Any = None) -> Any:
-        return return_value() if check_value else default_value
+    def check_in(value: Any, arg_name: str, default_value:  Any | Callable[[None], Any | None] | None = None) -> Any | None:
+        return DataTool.check(arg_name in value, lambda: value[arg_name], default_value)
 
     @staticmethod
-    def not_none_check(check_value: Any, return_value: Callable, default_value: Any = None) -> Any:
-        return DataTool.check(check_value is not None, return_value, default_value() if default_value is not None and isinstance(default_value, Callable) else default_value)
+    def check_not_none(check_value: Any | list[Any] | None, true_value: Callable[[None], Any | None], false_value: Callable[[None], Any | None] | Any | None = None, check_all: bool = False) -> Any | None:
+        check: bool = False
+        if isinstance(check_value, list):
+            for item in check_value:
+                check = not DataTool.is_none(item)
+                if (not check_all and check) or (check_all and not check):
+                    break
+        else:
+            check = not DataTool.is_none(check_value)
+        return true_value() if check else false_value() if not DataTool.is_none(false_value) and callable(false_value) else false_value
 
     @staticmethod
-    def if_not_none(check_value: Any, return_value: Callable[[Any], Any], default_value: Any = None) -> Any:
-        return default_value if check_value is None else return_value(check_value)
+    def if_not_empty(check_value: Any | None, return_value: Callable[[Any], Any], default_value: Any | None = None) -> Any | None:
+        return default_value if DataTool.is_empty(check_value) else return_value(check_value)
 
     @staticmethod
-    def is_empty(value: Any) -> bool:
-        return value is None or (isinstance(value, (list, str, dict)) and len(value) == 0)
+    def is_empty(value: list | str | dict | tuple | Any | None) -> bool:
+        return DataTool.is_none(value) or (isinstance(value, (list, str, dict, tuple)) and len(value) == 0)
+    
+    @staticmethod
+    def is_not_none(value: Any | None) -> bool:
+        return not DataTool.is_none(value)
+    
+    @staticmethod
+    def is_none(value: Any | None) -> bool:
+        return value is None
 
 class ListTool:
 
     @staticmethod
     def not_empty_items(value: list[Any | None]) -> list[Any]:
         return list(filter(lambda item: not DataTool.is_empty(item), value))
     
     @staticmethod
     def not_less_length_items(value: list[Any | None], length: int) -> list[Any]:
         return list(filter(lambda item: not DataTool.is_empty(item) and len(item) >= length, value))
 
 class StringTool:
 
     @staticmethod
+    def contains(value1: str, value2: str) -> bool:
+        value1 = value1.lower()
+        value2 = value2.lower()
+        return (value2.find(value1) if len(value2) > len(value1) else value1.find(value2)) != -1
+
+    @staticmethod
     def split_with_not_empty_items(value: str, symbol: str = " ") -> list[str]:
         return ListTool.not_empty_items(value.split(symbol))
 
     @staticmethod
     def dequotes(value: str) -> tuple[list[str], list[str]]:
         quotes: list[str] = ["'", "\""]
         value_list: list[str] = list(
@@ -238,15 +294,23 @@
             return value[0].upper()
         return value[0].upper() + value[1:]
     
     @staticmethod
     def decapitalize(value: str) -> str:
         if DataTool.is_empty(value):
             return ""
-        return value[0].lower() + value[1:]
+        result: str = ""
+        for index, char in enumerate(value):
+            char_is_upper: bool = char.isupper()
+            if char == " " or char_is_upper:
+                char = char.lower() if char_is_upper else char
+                result += char
+                break 
+            result += char
+        return result + value[index + 1:] if index < len(value) else ""
 
     @staticmethod
     def from_russian_keyboard_layout(value: str) -> str:
         dictionary: dict[str, str] = {'Й': 'Q', 'Ц': 'W', 'У': 'E', 'К': 'R', 'Е': 'T',
                     'Н': 'Y', 'Г': 'U', 'Ш': 'I', 'Щ': 'O', 'З': 'P',
                     'Х': '{', 'Ъ': '}', 'Ф': 'A', 'Ы': 'S', 'В': 'D',
                     'А': 'F', 'П': 'G', 'Р': 'H', 'О': 'J', 'Л': 'K',
@@ -268,24 +332,32 @@
 class ParameterList:
 
     def __init__(self, list: Any):
         self.list = list if isinstance(
             list, List) or isinstance(self, Tuple) else [list]
         self.index = 0
 
-    def next(self, object: Any = None, default_value: Any = None) -> Any:
+    def next(self, object: Any | None = None, default_value: Any | None = None) -> Any | None:
         if self.index >= len(self.list):
             return default_value
-        value = self.list[self.index]
+        value: Any = self.list[self.index]
+        if value == "":
+            value = None
         self.index = self.index + 1
-        if object is not None:
-            value = DataTool.fill_data_from_source(object, value)
+        if not DataTool.is_empty(value) and not DataTool.is_empty(object):
+            if inspect.isclass(object) and issubclass(object, Enum):
+                value = EnumTool.get(object, value)
+            else:
+                value = DataTool.fill_data_from_source(object, value)
         return value
+    
+    def next_as_list(self, class_type) -> Any | None:
+        return DataTool.fill_data_from_list_source(class_type, self.next())
 
-    def get(self, index: int = 0, object: Any = None, default_value: Any = None) -> Any:
+    def get(self, index: int = 0, object: Any | None = None, default_value: Any | None = None) -> Any | None:
         temp_index: int = self.index
         self.index = index
         result: Any = self.next(object, default_value)
         self.index = temp_index
         return result
 
     def set(self, index: int, value: Any) -> None:
@@ -314,55 +386,62 @@
         return DateTimeTool.datetime_to_string(date, format) if date is not None else DateTimeTool.today_string(format)
 
     @staticmethod
     def today_string(format: str = None, subtract: int = 0) -> str:
         return DateTimeTool.datetime_to_string(DateTimeTool.today(subtract).date(), format)
 
     @staticmethod
-    def datetime_to_string(date: datetime, format: str = None) -> str:
+    def datetime_to_string(date: datetime | None, format: str | None = None) -> str | None:
         if date is None:
             return None
-        return date.isoformat() if format is None else date.strftime(format)
+        return DataTool.check_not_none(format, lambda: date.strftime(format), lambda: date.isoformat())
 
     @staticmethod
-    def date_to_string(date: datetime, format: str = None) -> str:
+    def date_to_string(date: datetime, format: str | None = None) -> str:
         return DateTimeTool.datetime_to_string(date.date(), format)
 
     @staticmethod
-    def to_date_string(date_string: str) -> str:
-        list : list[str] = date_string.split("T")
+    def to_date_string(isoformat_date_string: str) -> str:
+        list: list[str] = isoformat_date_string.split(CONST.DATETIME_SPLITTER)
         return list[0]
 
     @staticmethod
     def today(delta_days: int = 0) -> datetime:
         return datetime.today() + timedelta(days=delta_days)
 
     @staticmethod
-    def now() -> datetime:
-        return datetime.now()
+    def now(minute: int | None = None, second: int | None = None) -> datetime:
+        result: datetime = datetime.now()
+        if not DataTool.is_empty(minute):
+            result = result.replace(minute=minute)
+        if not DataTool.is_empty(second):
+            result = result.replace(second=second)
+        return result.replace(microsecond=0)
+    
+    @staticmethod
+    def now_to_string(format: str | None = None) -> str:
+        return DateTimeTool.datetime_to_string(DateTimeTool.now(), format)
 
     @staticmethod
-    def now_time_string(format: str = None, delta_minutes: int = 0) -> str:
+    def now_time_to_string(format: str = None, delta_minutes: int = 0) -> str:
         return DateTimeTool.datetime_to_string(DateTimeTool.now_time(delta_minutes), format)
 
     @staticmethod
     def now_time(delta_minutes: int = 0) -> datetime:
         return datetime.combine(date.today(), datetime.now().time()) + timedelta(minutes=delta_minutes)
 
     @staticmethod
-    def now_string(format: str) -> str:
-        return DateTimeTool.datetime_to_string(DateTimeTool.now(), format)
-
-    @staticmethod
-    def from_string(value: str, format: str = None) -> datetime:
-        return datetime.fromisoformat(value) if format is None else datetime.strptime(value, format)
+    def datetime_from_string(value: str | None, format: str | None = None) -> datetime | None:
+        if DataTool.is_empty(value):
+            return None
+        return DataTool.check_not_none(format, lambda: datetime.strptime(value, format), lambda: datetime.fromisoformat(value))
 
     @staticmethod
-    def is_equal_by_time(date: datetime, value: Any) -> bool:
-        if isinstance(value, Tuple):
+    def is_equal_by_time(date: datetime, value: tuple | list | datetime) -> bool:
+        if isinstance(value, (tuple, list)):
             return date.hour == value[0] and date.minute == value[1]
         if isinstance(value, datetime):
             return date.hour == value.hour and date.minute == value.minute
         return None
 
 class ResultTool:
 
@@ -373,18 +452,18 @@
             result["fields_alias"] = fields.name
         else:
             result["fields"] = fields
         return result
 
     @staticmethod
     def is_empty(result: Result | None) -> bool:
-        return result is None or DataTool.is_empty(result.data)
+        return DataTool.is_none(result) or DataTool.is_empty(result.data)
 
     @staticmethod
-    def get_first_element(result: Result[list[T] | T], default_value: Any | None = None) -> Any | T | None:
+    def get_first_element(result: Result[list[T] | T], default_value: Any | None = None) -> T | Any | None:
         return DataTool.get_first_item(result.data, default_value)
 
     @staticmethod
     def with_first_element(result: Result[T], default_value: Any = None) -> Result[T]:
         result.data = ResultTool.get_first_element(result, default_value)
         return result
 
@@ -432,17 +511,17 @@
             try:
                 result.data = list(filter(filter_function, result.data))
             except StopIteration:
                pass 
         return result
 
     @staticmethod
-    def sort(result: Result[list[T]], sort_function: Callable) -> Result[list[T]]:
+    def sort(result: Result[list[T]], sort_function: Callable, reserve: bool = False) -> Result[list[T]]:
         if sort_function is not None:
-            result.data.sort(key=sort_function)
+            result.data.sort(key=sort_function, reverse=reserve)
         return result
 
 
     @staticmethod
     def every(result: Result[list[T]], action_function: Callable[[T], None]) -> Result[list[T]]:
         for item in result.data:
             action_function(item)
@@ -465,47 +544,60 @@
 
 class TranslateTool:
 
     @staticmethod
     def ru_to_en(value: str) -> str:
         return value.translate(dict(zip(map(ord,  
         "йцукенгшщзхъфывапролджэячсмитьбю.ё"
-        'ЙЦУКЕНГШЩЗХЪФЫВАПРОЛДЖЭЯЧСМИТЬБЮ,Ё'),
+        "ЙЦУКЕНГШЩЗХЪФЫВАПРОЛДЖЭЯЧСМИТЬБЮ,Ё"),
         "qwertyuiop[]asdfghjkl;'zxcvbnm,./`"
         'QWERTYUIOP{}ASDFGHJKL:"ZXCVBNM<>?~')))
 
 class BitMask:
 
     @staticmethod
-    def set(value: int, bit: Any) -> int:
-        bits: list[int] = bit if isinstance(bit, list) else [bit]
+    def add(value: int, bit: int | tuple[Enum] | Enum | list[Enum] | list[int]) -> int:
+        bits: list[int | Enum] = bit if isinstance(bit, (list, tuple)) else [bit]
         for bit in bits:
-            value |= bit
+            if isinstance(bit, int):
+                value |= bit
+            elif isinstance(bit, Enum):
+                value |= bit.value
         return value
+    
+    @staticmethod
+    def set(bit: int | tuple[Enum] | Enum | list[Enum] | list[int]) -> int:
+        return BitMask.add(0, bit)
 
     @staticmethod
-    def has(value: int, bit: Any) -> bool:
+    def has(value: int, bit: int | tuple[Enum] | Enum | list[Enum] | list[int]) -> bool:
         if value is None:
             return False
-        bits: list[int] = bit if isinstance(bit, list) else [bit]
+        bits: list[int] = bit if isinstance(bit, (list, tuple)) else [bit]
         result: bool = False
         if len(bits) > 1:
             for bit in bits:
                 result = BitMask.has(value, bit)
                 if result:
                     break
         else:
             if isinstance(bit, int):
                 result = (value & bit) == bit
             elif isinstance(bit, Enum):
                 result = BitMask.has(value, bit.value)
         return result
+    
+    @staticmethod
+    def has_index(value: int, index: int) -> bool:
+        return BitMask.has(value, pow(2, index))
 
     @staticmethod
-    def unset(value: int, bit: int) -> int:
+    def remove(value: int, bit: int | Enum) -> int:
+        if isinstance(bit, Enum):
+            bit = bit.value
         if BitMask.has(value, bit):
             value ^= bit
         return value
 
 class ResultUnpack:
 
     @staticmethod
@@ -522,15 +614,25 @@
     def unpack_data(result: dict) -> Any:
         return result["data"]
 
    
 class PathTool:
 
     @staticmethod
-    def makedir_if_not_exists(path: str) -> bool:
+    def get_file_list(path: str, created_after: float | None = None) -> list[str]:
+        file_list = [(file_path, os.path.getctime(file_path))
+                     for file_path in [os.path.join(path, file_path) for file_path in [
+                         file_path for file_path in next(walk(path), (None, None, []))[2]]]]
+        if created_after is not None:
+            file_list = sorted(file_list, key=itemgetter(1), reverse=True)
+            return [file_item[0] for file_item in file_list if file_item[1] > created_after]
+        return [file_item[0] for file_item in file_list]
+
+    @staticmethod
+    def make_directory_if_not_exists(path: str) -> bool:
         try:
             is_exist = os.path.exists(path)
             if not is_exist:
                 os.makedirs(path)
                 return True
             return False
         except:
@@ -604,60 +706,65 @@
 class NetworkTool:
 
     @staticmethod
     def is_accessable(host_or_ip: str, packets: int = 1, timeout: int = 100):
         if platform.system().lower() == "windows":
             command = ["ping", "-4", "-n", str(packets), "-w", str(timeout), host_or_ip]
             result = subprocess.run(command, stdin=subprocess.DEVNULL, stdout=subprocess.PIPE,
-                                    stderr=subprocess.DEVNULL, creationflags=0x08000000)
-            out: str = str(result.stdout, "unicode_escape")
-            return result.returncode == 0 and (int(str(out.split(" = ")[-3:][2]).splitlines()[0]) < packets and out.count("(TTL)") < packets)
+                                    stderr=subprocess.DEVNULL, creationflags=0x08000000, encoding="unicode_escape")
+            out: str = result.stdout
+            return result.returncode == 0 and int(out.split(" = ")[-4].splitlines()[0].split(" ")[0]) < packets and out.count("(TTL)") < packets
+            #int(str(out.split(" = ")[-3:][2]).splitlines()[0].split(" ")[0]) < packets and out.count("(TTL)") < packets
         else:
             command = ["ping", "-c", str(packets), "-w", str(timeout), host_or_ip]
             result = subprocess.run(command, stdin=subprocess.DEVNULL, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
             return result.returncode == 0
 
     @staticmethod
     def next_free_port() -> int:
         with socket.socket() as soc:
-            soc.bind(('', 0))
+            soc.bind(("", 0))
             return soc.getsockname()[1]
         
         
 class FullNameTool:
 
     SPLIT_SYMBOL: str = " "
     FULL_NAME_LENGTH: int = 3
 
     @staticmethod
-    def to_string(full_name: FullName, join_symbol: str = SPLIT_SYMBOL) -> str:
+    def format(value: str) -> str:
+        return FullNameTool.fullname_to_string(FullNameTool.fullname_from_string(value))
+
+    @staticmethod
+    def fullname_to_string(full_name: FullName, join_symbol: str = SPLIT_SYMBOL) -> str:
         return DataTool.to_string(full_name, join_symbol)
 
     @staticmethod
-    def to_given_name(full_name_holder: Any, join_symbol: str = SPLIT_SYMBOL) -> str:
+    def to_given_name(full_name_holder: FullName | PolibasePerson | User | str, join_symbol: str = SPLIT_SYMBOL) -> str:
         if isinstance(full_name_holder, PolibasePerson):
             return FullNameTool.to_given_name(full_name_holder.FullName)
         if isinstance(full_name_holder, User):
             return FullNameTool.to_given_name(full_name_holder.name)
         if isinstance(full_name_holder, FullName):
             return join_symbol.join(ListTool.not_empty_items([full_name_holder.first_name, full_name_holder.middle_name]))
-        elif isinstance(full_name_holder, str):
+        if isinstance(full_name_holder, str):
             full_name_holder = full_name_holder.strip()
-            if FullNameTool.is_full_name(full_name_holder):
-                return FullNameTool.to_given_name(FullNameTool.from_string(full_name_holder, join_symbol))
+            if FullNameTool.is_fullname(full_name_holder):
+                return FullNameTool.to_given_name(FullNameTool.fullname_from_string(full_name_holder, join_symbol))
             else:
                 return full_name_holder
 
     @staticmethod
-    def from_string(value: str, split_symbol: str = SPLIT_SYMBOL) -> FullName:
+    def fullname_from_string(value: str, split_symbol: str = SPLIT_SYMBOL) -> FullName:
         full_name_string_list: list[str] = ListTool.not_empty_items(value.split(split_symbol))
         return FullName(full_name_string_list[0], full_name_string_list[1], full_name_string_list[2])
 
     @staticmethod
-    def is_full_name(value: str, split_symbol: str = SPLIT_SYMBOL) -> bool:
+    def is_fullname(value: str, split_symbol: str = SPLIT_SYMBOL) -> bool:
         return len(ListTool.not_empty_items(value.split(split_symbol))) >= FullNameTool.FULL_NAME_LENGTH
 
     @staticmethod
     def is_equal(fn_a: FullName, fn_b: FullName) -> bool:
         return fn_a.first_name == fn_b.first_name and fn_a.middle_name == fn_b.middle_name and fn_a.last_name == fn_b.last_name
 
     @staticmethod
```

### Comparing `pih-1.43/pih/widgets.py` & `pih-1.45/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.43/pih_setup.py` & `pih-1.45/pih_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,17 +48,14 @@
 
 #for polibase
     #cx_Oracle
 
 #for mobile helper
     #paramiko
 
-if PIH.VERSION.local() <= PIH.VERSION.remote():
-    raise Exception("PIH version is same as version from PyPi")
-
 #########################################################################################################
 """
 1. python pih_setup.py sdist --dist-dir pih_dist bdist_wheel --dist-dir pih_dist build --build-base pih_build
 2. twine upload --repository pypi pih_dist/*
 3. pip install pih -U
 """
 folder = "//pih/facade/pih_dist"
```

