# Comparing `tmp/pih-auto-0.19.tar.gz` & `tmp/pih-auto-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-auto-0.19.tar", last modified: Wed Apr 10 01:31:28 2024, max compression
+gzip compressed data, was "pih-auto-0.20.tar", last modified: Thu Apr 18 05:26:05 2024, max compression
```

## Comparing `pih-auto-0.19.tar` & `pih-auto-0.20.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:31:28.443618 pih-auto-0.19/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:31:27.990510 pih-auto-0.19/AutomationService/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-auto-0.19/AutomationService/__init__.py
--rw-rw-rw-   0        0        0      152 2024-02-14 02:13:48.000000 pih-auto-0.19/AutomationService/__main__.py
--rw-rw-rw-   0        0        0      559 2024-04-09 23:52:18.000000 pih-auto-0.19/AutomationService/const.py
--rw-rw-rw-   0        0        0    14806 2024-04-09 22:56:43.000000 pih-auto-0.19/AutomationService/service.py
--rw-rw-rw-   0        0        0      295 2024-04-10 01:31:28.396758 pih-auto-0.19/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:31:28.365482 pih-auto-0.19/pih_auto.egg-info/
--rw-rw-rw-   0        0        0      295 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-10 01:31:27.000000 pih-auto-0.19/pih_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:31:28.459228 pih-auto-0.19/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 05:26:05.845057 pih-auto-0.20/
+drwxrwxrwx   0        0        0        0 2024-04-18 05:26:05.433960 pih-auto-0.20/AutomationService/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-auto-0.20/AutomationService/__init__.py
+-rw-rw-rw-   0        0        0      152 2024-02-14 02:13:48.000000 pih-auto-0.20/AutomationService/__main__.py
+-rw-rw-rw-   0        0        0      559 2024-04-18 05:21:39.000000 pih-auto-0.20/AutomationService/const.py
+-rw-rw-rw-   0        0        0    19242 2024-04-18 05:21:31.000000 pih-auto-0.20/AutomationService/service.py
+-rw-rw-rw-   0        0        0      295 2024-04-18 05:26:05.812589 pih-auto-0.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 05:26:05.780310 pih-auto-0.20/pih_auto.egg-info/
+-rw-rw-rw-   0        0        0      295 2024-04-18 05:26:04.000000 pih-auto-0.20/pih_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-04-18 05:26:05.000000 pih-auto-0.20/pih_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:26:05.000000 pih-auto-0.20/pih_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-18 05:26:05.000000 pih-auto-0.20/pih_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-04-18 05:26:05.000000 pih-auto-0.20/pih_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-18 05:26:05.000000 pih-auto-0.20/pih_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 05:26:05.860745 pih-auto-0.20/setup.cfg
```

### Comparing `pih-auto-0.19/AutomationService/const.py` & `pih-auto-0.20/AutomationService/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "Automation"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.19"
+VERSION: str = "0.20"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Automation service",
     host=HOST.NAME,
     use_standalone=True,
     standalone_name="auto",
```

### Comparing `pih-auto-0.19/AutomationService/service.py` & `pih-auto-0.20/AutomationService/service.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,312 +4,406 @@
 from collections import defaultdict
 
 import ipih
 
 from pih.tools import *
 from pih.consts import *
 from pih.collections import *
-from pih import A, PIHThread, serve
 from AutomationService.const import *
 from pih.consts.errors import NotFound
-from MobileHelperService.client import Client as MIO
-from MobileHelperService.const import COMMAND_KEYWORDS
-from MobileHelperService.api import MobileOutput, mio_command
+from pih import A, PIHThread, serve, subscribe_on
+
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
 
 def start(as_standalone: bool = False) -> None:
-    from pih.tools import ParameterList
-    from datetime import datetime
-    from pih.collections import (
-        User,
-        ActionWasDone,
-        NewMailMessage,
-        PolibasePerson,
-        ResourceStatus,
-        EmailInformation,
-        ChillerIndicationsValueContainer,
-    )
-    from pih.collections.service import SubscribtionResult
-
-    class DH:
-        resource_problem_status_map: dict[str, ProblemState] = defaultdict(ProblemState)
-        hr_user: str | None = None
-
-    def get_resource_status_address(resource_status: ResourceStatus) -> str:
-        resource_status_address: str = resource_status.address # type: ignore
-        address_list: list[str] = [
-            A.CT_R_D.VPN_PACS_SPB.address,
-            A.CT_R_D.PACS_SPB.address,
-        ] # type: ignore
-        if resource_status.address in address_list:
-            resource_status_address = address_list[0]
-        return resource_status_address
-
-    def get_problem_state(resource_status: ResourceStatus) -> ProblemState:
-        return DH.resource_problem_status_map[
-            get_resource_status_address(resource_status)
-        ]
-
-    def set_problem_state(resource_status: ResourceStatus, value: ProblemState) -> None:
-        DH.resource_problem_status_map[get_resource_status_address(resource_status)] = (
-            value
+
+    if A.U.for_service(SD, as_standalone=as_standalone):
+
+        from pih.collections import (
+            User,
+            ActionWasDone,
+            NewMailMessage,
+            PolibasePerson,
+            ResourceStatus,
+            EmailInformation,
+            ChillerIndicationsValueContainer,
         )
+        from MobileHelperService.client import Client as MIO
+        from pih.collections.service import SubscribtionResult
+        from MobileHelperService.api import MobileOutput, mio_command
+        from MobileHelperService.const import COMMAND_KEYWORDS, FLAG_KEYWORDS
 
-    def service_call_handler(
-        sc: SC,
-        pl: ParameterList,
-        subscribtion_result: SubscribtionResult | None,
-    ) -> Any:
-        if sc == SC.heart_beat:
-            current_datetime: datetime = A.D_Ex.parameter_list(pl).get()
-            PIHThread(
-                lambda: A.R_F.execute(
-                    "@on_heart_beat", {"current_datetime": current_datetime}
-                )
-            )
-            return
-        if sc == SC.register_chiller_indications_value:
-            result: dict[str, Any] | None = subscribtion_result.result
-            if ne(result):
-                if A.C_IND.chiller_on():
-                    indications_value_container: ChillerIndicationsValueContainer = (
-                        A.D.fill_data_from_source(
-                            ChillerIndicationsValueContainer(), result
-                        )
-                    )  # type: ignore
-                    shutil.copy(
-                        A.PTH_IND.CHILLER_DATA_IMAGE_LAST_RESULT,
-                        A.PTH_IND.CHILLER_DATA_IMAGE_RESULT(
-                            A.PTH.replace_prohibited_symbols_from_path_with_symbol(
-                                A.D_F.datetime(indications_value_container.timestamp)
+        from datetime import datetime
+
+        class tools:
+
+            class send:
+
+                @staticmethod
+                def ct_indications() -> None:
+                    indications_value_container: CTIndicationsValueContainer | None = (
+                        one(A.R_IND.last_ct_value_containers(True))
+                    )
+
+                    if ne(indications_value_container):
+                        MIO.create_output(A.CT_ME_WH.GROUP.CT_INDICATIONS).write_result(
+                            Result(
+                                A.CT_FC.INDICATIONS.CT_VALUE,
+                                CTIndicationsValue(
+                                    indications_value_container.temperature,
+                                    indications_value_container.humidity,
+                                ),
                             ),
-                            indications_value_container.temperature,
-                            indications_value_container.indicators,
+                            title="Показания в помещение КТ:",
+                        )
+
+                @staticmethod
+                def all_indications() -> None:
+                    A.A_MIO.send_command_to(
+                        js(
+                            (
+                                "indications",
+                                FLAG_KEYWORDS.ALL_SYMBOL,
+                                FLAG_KEYWORDS.SILENCE,
+                            )
                         ),
+                        A.CT_ME_WH.GROUP.CONTROL_SERVICE_INDICATIONS,
                     )
-            return
-        if sc == SC.send_event:
-            if subscribtion_result.result:
-                event: A.CT_E | None = None
-                event_parameters: list[Any] | None = None
-                event, event_parameters = A.D_Ex_E.with_parameters(pl)
+
+        class DH:
+            resource_problem_status_map: dict[str, ProblemState] = defaultdict(
+                ProblemState
+            )
+            hr_user: str | None = None
+
+        def get_resource_status_address(resource_status: ResourceStatus) -> str:
+            resource_status_address: str = resource_status.address  # type: ignore
+            address_list: list[str] = [
+                A.CT_R_D.VPN_PACS_SPB.address,
+                A.CT_R_D.PACS_SPB.address,
+            ]  # type: ignore
+            if resource_status.address in address_list:
+                resource_status_address = address_list[0]
+            return resource_status_address
+
+        def get_problem_state(resource_status: ResourceStatus) -> ProblemState:
+            return DH.resource_problem_status_map[
+                get_resource_status_address(resource_status)
+            ]
+
+        def set_problem_state(
+            resource_status: ResourceStatus, value: ProblemState
+        ) -> None:
+            DH.resource_problem_status_map[
+                get_resource_status_address(resource_status)
+            ] = value
+
+        def service_call_handler(
+            sc: SC,
+            pl: ParameterList,
+            subscribtion_result: SubscribtionResult | None,
+        ) -> Any:
+            if sc == SC.heart_beat:
+                current_datetime: datetime = A.D_Ex.parameter_list(pl).get()
                 PIHThread(
-                    lambda event_and_parameters: A.R_F.execute(
-                        "@on_event", event_and_parameters
-                    ),
-                    args=({"event": event, "event_parameters": event_parameters, "pl" : pl},),
+                    lambda: A.R_F.execute(
+                        "@on_heart_beat",
+                        {
+                            "current_datetime": current_datetime,
+                            "pl": pl,
+                            "tools": tools,
+                        },
+                    )
                 )
-                if event in [A.CT_E.RESOURCE_ACCESSABLE, A.CT_E.RESOURCE_INACCESSABLE]:
-                    resource_status: ResourceStatus = A.D.fill_data_from_source(
-                        ResourceStatus(), event_parameters[1]
+                return
+            if sc == SC.register_chiller_indications_value:
+                result: dict[str, Any] | None = subscribtion_result.result
+                if ne(result):
+                    if A.C_IND.chiller_on():
+                        indications_value_container: (
+                            ChillerIndicationsValueContainer
+                        ) = A.D.fill_data_from_source(
+                            ChillerIndicationsValueContainer(), result
+                        )  # type: ignore
+                        shutil.copy(
+                            A.PTH_IND.CHILLER_DATA_IMAGE_LAST_RESULT,
+                            A.PTH_IND.CHILLER_DATA_IMAGE_RESULT(
+                                A.PTH.replace_prohibited_symbols_from_path_with_symbol(
+                                    A.D_F.datetime(
+                                        indications_value_container.timestamp
+                                    )
+                                ),
+                                indications_value_container.temperature,
+                                indications_value_container.indicators,
+                            ),
+                        )
+                return
+            if sc == SC.send_event:
+                if subscribtion_result.result:
+                    event: A.CT_E | None = None
+                    event_parameters: list[Any] | None = None
+                    event, event_parameters = A.D_Ex_E.with_parameters(pl)
+                    PIHThread(
+                        lambda event_and_parameters: A.R_F.execute(
+                            "@on_event", event_and_parameters
+                        ),
+                        args=(
+                            {
+                                "event": event,
+                                "event_parameters": event_parameters,
+                                "pl": pl,
+                                "tools": tools,
+                            },
+                        ),
                     )
-                    if event == A.CT_E.RESOURCE_ACCESSABLE:
-                        set_problem_state(resource_status, ProblemState.FIXED)
-                    else:
-                        reason_value: str | None = event_parameters[4]
-                        reason: A.CT_R_IR | None = (
-                            None
-                            if e(reason_value)
-                            else A.D.get(
-                                A.CT_R_IR, event_parameters[4], return_value=False
-                            )
+                    if event in [
+                        A.CT_E.RESOURCE_ACCESSABLE,
+                        A.CT_E.RESOURCE_INACCESSABLE,
+                    ]:
+                        resource_status: ResourceStatus = A.D.fill_data_from_source(
+                            ResourceStatus(), event_parameters[1]
                         )
-                        if (
-                            get_problem_state(resource_status)
-                            == ProblemState.WAIT_FOR_FIX_RESULT
-                        ):
-                            set_problem_state(resource_status, ProblemState.NOT_FIXED)
-                        if get_problem_state(resource_status) != ProblemState.AT_FIX:
-                            resource_status_address: str = get_resource_status_address(
-                                resource_status
+                        if event == A.CT_E.RESOURCE_ACCESSABLE:
+                            set_problem_state(resource_status, ProblemState.FIXED)
+                        else:
+                            reason_value: str | None = event_parameters[4]
+                            reason: A.CT_R_IR | None = (
+                                None
+                                if e(reason_value)
+                                else A.D.get(
+                                    A.CT_R_IR, event_parameters[4], return_value=False
+                                )
                             )
-                            if resource_status_address in [
-                                A.CT_ADDR.SITE_ADDRESS,
-                                A.CT_ADDR.EMAIL_SERVER_ADDRESS,
-                                A.CT_ADDR.API_SITE_ADDRESS,
-                            ]:
-                                if reason == A.CT_R_IR.CERTIFICATE_ERROR:
+                            if (
+                                get_problem_state(resource_status)
+                                == ProblemState.WAIT_FOR_FIX_RESULT
+                            ):
+                                set_problem_state(
+                                    resource_status, ProblemState.NOT_FIXED
+                                )
+                            if (
+                                get_problem_state(resource_status)
+                                != ProblemState.AT_FIX
+                            ):
+                                resource_status_address: str = (
+                                    get_resource_status_address(resource_status)
+                                )
+                                if resource_status_address in [
+                                    A.CT_ADDR.SITE_ADDRESS,
+                                    A.CT_ADDR.EMAIL_SERVER_ADDRESS,
+                                    A.CT_ADDR.API_SITE_ADDRESS,
+                                ]:
+                                    if reason == A.CT_R_IR.CERTIFICATE_ERROR:
+                                        set_problem_state(
+                                            resource_status, ProblemState.AT_FIX
+                                        )
+                                        for command in [
+                                            "certbot renew",
+                                            "service postfix restart",
+                                            "service nginx restart",
+                                            "service dovecot restart",
+                                        ]:
+                                            A.R_SSH.execute(
+                                                command, resource_status.address
+                                            )
+                                if (
+                                    resource_status_address
+                                    == A.CT_R_D.VPN_PACS_SPB.address
+                                ):
+                                    openVPN_folder: str = r"C:\Program Files\OpenVPN"
                                     set_problem_state(
                                         resource_status, ProblemState.AT_FIX
                                     )
-                                    for command in [
-                                        "certbot renew",
-                                        "service postfix restart",
-                                        "service nginx restart",
-                                        "service dovecot restart",
-                                    ]:
-                                        A.R_SSH.execute(
-                                            command, resource_status.address
-                                        )
-                            if resource_status_address == A.CT_R_D.VPN_PACS_SPB.address:
-                                openVPN_folder: str = r"C:\Program Files\OpenVPN"
-                                set_problem_state(resource_status, ProblemState.AT_FIX)
-                                A.EXC.kill_process("openvpn", A.CT.HOST.WS255.NAME)
-                                A.EXC.execute(
-                                    A.EXC.create_command_for_psexec(
-                                        (
-                                            A.PTH.join(
-                                                openVPN_folder, "bin", "openvpn"
-                                            ),
-                                            "--config",
-                                            A.PTH.join(
-                                                openVPN_folder, "config", "cmrt.ovpn"
-                                            ),
-                                            "--auth-user-pass",
-                                            A.PTH.join(
-                                                openVPN_folder, "config", "auth.txt"
+                                    A.EXC.kill_process("openvpn", A.CT.HOST.WS255.NAME)
+                                    A.EXC.execute(
+                                        A.EXC.create_command_for_psexec(
+                                            (
+                                                A.PTH.join(
+                                                    openVPN_folder, "bin", "openvpn"
+                                                ),
+                                                "--config",
+                                                A.PTH.join(
+                                                    openVPN_folder,
+                                                    "config",
+                                                    "cmrt.ovpn",
+                                                ),
+                                                "--auth-user-pass",
+                                                A.PTH.join(
+                                                    openVPN_folder, "config", "auth.txt"
+                                                ),
                                             ),
+                                            A.CT.HOST.WS255.NAME,
                                         ),
-                                        A.CT.HOST.WS255.NAME,
-                                    ),
-                                    True,
-                                )
-                            set_problem_state(
-                                resource_status, ProblemState.WAIT_FOR_FIX_RESULT
-                            )
-                    return
-                if event == A.CT_E.NEW_EMAIL_MESSAGE_WAS_RECEIVED:
-                    mail_message: NewMailMessage = A.D_Ex.new_mail_message(
-                        event_parameters[3]
-                    )
-                    if n(DH.hr_user):
-                        DH.hr_user = one(A.R_U.by_job_position(A.CT_AD.JobPositions.HR))
-                    if mail_message.from_ in [DH.hr_user.mail, A.CT.TEST.EMAIL_ADDRESS]:
-                        subject: str = mail_message.subject.lower()
-                        if (
-                            subject.find("т/у") != -1
-                            or subject.find("трудоустройство") != -1
-                        ):
-                            recipient: str = A.D.get(A.CT_ME_WH.GROUP.PIH_CLI)
-                            mobile_output: MobileOutput = MIO.create_output(recipient)
-                            mobile_output.write_line(
-                                j(
-                                    (
-                                        "Получено новое сообщение об трудоустройстве от ",
-                                        b("Отдела кадров"),
-                                        " (",
-                                        DH.hr_user.name,
-                                        ")",
+                                        True,
                                     )
+                                set_problem_state(
+                                    resource_status, ProblemState.WAIT_FOR_FIX_RESULT
                                 )
+                        return
+                    if event == A.CT_E.NEW_EMAIL_MESSAGE_WAS_RECEIVED:
+                        mail_message: NewMailMessage = A.D_Ex.new_mail_message(
+                            event_parameters[3]
+                        )
+                        if n(DH.hr_user):
+                            DH.hr_user = one(
+                                A.R_U.by_job_position(A.CT_AD.JobPositions.HR)
                             )
-                            with mobile_output.make_separated_lines():
-                                for line in A.D.not_empty_items(
-                                    mail_message.text.splitlines()
-                                ):
-                                    text_list: list[str] = line.split(":")
-                                    has_separator: bool = len(text_list) > 1
-                                    title: str = (
-                                        text_list[0].strip() if has_separator else line
-                                    )
-                                    text: str | None = (
-                                        text_list[1].strip() if has_separator else None
-                                    )
-                                    mobile_output.write_line(b(title))
-                                    if ne(text):
-                                        mobile_output.write_line(text)
-                            A.A_MIO.send_command_to(
-                                js(
-                                    (
-                                        mio_command(COMMAND_KEYWORDS.CREATE),
-                                        mio_command(COMMAND_KEYWORDS.USER),
+                        if mail_message.from_ in [
+                            DH.hr_user.mail,
+                            A.CT.TEST.EMAIL_ADDRESS,
+                        ]:
+                            subject: str = mail_message.subject.lower()
+                            if (
+                                subject.find("т/у") != -1
+                                or subject.find("трудоустройство") != -1
+                            ):
+                                recipient: str = A.D.get(A.CT_ME_WH.GROUP.PIH_CLI)
+                                mobile_output: MobileOutput = MIO.create_output(
+                                    recipient
+                                )
+                                mobile_output.write_line(
+                                    j(
+                                        (
+                                            "Получено новое сообщение об трудоустройстве от ",
+                                            b("Отдела кадров"),
+                                            " (",
+                                            DH.hr_user.name,
+                                            ")",
+                                        )
                                     )
-                                ),
-                                recipient,
-                                recipient,
-                            )
-                    return
-                if event in (A.CT_E.EMPLOYEE_CHECKED_IN, A.CT_E.EMPLOYEE_CHECKED_OUT):
-                    checked_in: bool = event == A.CT_E.EMPLOYEE_CHECKED_IN
-                    user: User | None = None
-                    try:
-                        name: str = event_parameters[0]
-                        user = one(A.D_U.by_name(name))
-                    except NotFound as _:
-                        pass
-                    if nn(user):
-                        PIHThread(
-                            lambda: A.R_F.execute(
-                                "@on_employee_checked_event",
-                                {"user": user, "checked_in": checked_in},
+                                )
+                                with mobile_output.make_separated_lines():
+                                    for line in A.D.not_empty_items(
+                                        mail_message.text.splitlines()
+                                    ):
+                                        text_list: list[str] = line.split(":")
+                                        has_separator: bool = len(text_list) > 1
+                                        title: str = (
+                                            text_list[0].strip()
+                                            if has_separator
+                                            else line
+                                        )
+                                        text: str | None = (
+                                            text_list[1].strip()
+                                            if has_separator
+                                            else None
+                                        )
+                                        mobile_output.write_line(b(title))
+                                        if ne(text):
+                                            mobile_output.write_line(text)
+                                A.A_MIO.send_command_to(
+                                    js(
+                                        (
+                                            mio_command(COMMAND_KEYWORDS.CREATE),
+                                            mio_command(COMMAND_KEYWORDS.USER),
+                                        )
+                                    ),
+                                    recipient,
+                                    recipient,
+                                )
+                        return
+                    if event in (
+                        A.CT_E.EMPLOYEE_CHECKED_IN,
+                        A.CT_E.EMPLOYEE_CHECKED_OUT,
+                    ):
+                        checked_in: bool = event == A.CT_E.EMPLOYEE_CHECKED_IN
+                        user: User | None = None
+                        try:
+                            name: str = event_parameters[0]
+                            user = one(A.D_U.by_name(name))
+                        except NotFound as _:
+                            pass
+                        if nn(user):
+                            PIHThread(
+                                lambda: A.R_F.execute(
+                                    "@on_employee_checked_event",
+                                    {"user": user, "checked_in": checked_in},
+                                )
                             )
+                        return
+
+                    if event == A.E_B.chiller_temperature_alert_was_fired():
+                        send_message_to_control_service(
+                            j(
+                                (
+                                    "ВНИМАНИЕ: превышена температруа чиллера (",
+                                    A.S.get(A.CT_S.CHILLER_ALERT_TEMPERATURE),
+                                    A.CT_V.TEMPERATURE_SYMBOL,
+                                    ")",
+                                )
+                            ),
+                            True,
+                        )
+                        return
+                    if event == A.E_B.polibase_person_email_was_added():
+                        email_information: EmailInformation = A.D.fill_data_from_source(
+                            EmailInformation(),
+                            A.E.get_parameter(event, event_parameters),
+                        )
+                        polibase_person: PolibasePerson = A.R_P.person_by_pin(
+                            email_information.person_pin
+                        ).data
+                        params: dict[str, str | None] = {
+                            "format": "json",
+                            "api_key": "65ddrin3zh791hxarbkwe4fmah5p44hkg4cjwsuy",
+                            "list_ids": "407",
+                            "fields[email]": polibase_person.email,
+                            "fields[Name]": polibase_person.FullName,
+                            "tags": "Polibase",
+                        }
+                        requests.get(
+                            "https://api.unisender.com/ru/api/subscribe",
+                            verify=False,
+                            params=params,
                         )
-                    return
 
-                if event == A.E_B.chiller_temperature_alert_was_fired():
-                    send_message_to_control_service(
-                        j(
-                            (
-                                "ВНИМАНИЕ: превышена температруа чиллера (",
-                                A.S.get(A.CT_S.CHILLER_ALERT_TEMPERATURE),
-                                A.CT_V.TEMPERATURE_SYMBOL,
-                                ")",
+                    if event == A.E_B.action_was_done():
+                        action_data: ActionWasDone = A.D_Ex_E.action(event_parameters)
+                        action: A.CT_ACT = action_data.action
+                        PIHThread(
+                            lambda: print(
+                                A.R_F.execute(
+                                    "@on_action",
+                                    {
+                                        "action": action,
+                                        "action_data": action_data,
+                                        "pl": pl,
+                                    },
+                                    stdout_redirect=True,
+                                )
                             )
-                        ),
-                        True,
-                    )
-                    return
-                if event == A.E_B.polibase_person_email_was_added():
-                    email_information: EmailInformation = A.D.fill_data_from_source(
-                        EmailInformation(),
-                        A.E.get_parameter(event, event_parameters),
-                    )
-                    polibase_person: PolibasePerson = A.R_P.person_by_pin(
-                        email_information.person_pin
-                    ).data
-                    params: dict[str, str | None] = {
-                        "format": "json",
-                        "api_key": "65ddrin3zh791hxarbkwe4fmah5p44hkg4cjwsuy",
-                        "list_ids": "407",
-                        "fields[email]": polibase_person.email,
-                        "fields[Name]": polibase_person.FullName,
-                        "tags": "Polibase",
-                    }
-                    requests.get(
-                        "https://api.unisender.com/ru/api/subscribe",
-                        verify=False,
-                        params=params,
-                    )
+                        )
+                        return
+            return True
 
-                if event == A.E_B.action_was_done():
-                    action_data: ActionWasDone = A.D_Ex_E.action(event_parameters)
-                    action: A.CT_ACT = action_data.action
-                    PIHThread(
-                        lambda: print(A.R_F.execute(
-                            "@on_action",
-                            {"action": action, "action_data": action_data, "pl" : pl},
-                            stdout_redirect = True
-                        ))
-                    )
-                    return
-        return True
+        def send_message_to_control_service(
+            value: str, on_workstation: bool = False
+        ) -> None:
+            if on_workstation:
+                A.ME_WS.by_login(A.CT_AD_U.CONTROL_SERVICE, value, 60 * 60 * 24)
+            MIO.create_output(A.CT_ME_WH.GROUP.CONTROL_SERVICE_INDICATIONS).write_line(
+                value
+            )
+            MIO.create_output(A.D_TN.by_login(A.CT_AD_U.CONTROL_SERVICE)).write_line(
+                value
+            )
 
-    def send_message_to_control_service(
-        value: str, on_workstation: bool = False
-    ) -> None:
-        if on_workstation:
-            A.ME_WS.by_login(A.CT_AD_U.CONTROL_SERVICE, value, 60 * 60 * 24)
-        MIO.create_output(A.CT_ME_WH.GROUP.CONTROL_SERVICE_INDICATIONS).write_line(
-            value
+        def service_starts_handler() -> None:
+            subscribe_on(SC.heart_beat)
+            subscribe_on(SC.send_event)
+            subscribe_on(SC.register_chiller_indications_value)
+
+        serve(
+            SD,
+            service_call_handler,
+            service_starts_handler,
+            isolate=ISOLATED,
+            as_standalone=as_standalone,
         )
-        MIO.create_output(A.D_TN.by_login(A.CT_AD_U.CONTROL_SERVICE)).write_line(value)
-
-    def service_starts_handler() -> None:
-        A.SRV_A.subscribe_on(SC.heart_beat)
-        A.SRV_A.subscribe_on(SC.send_event)
-        A.SRV_A.subscribe_on(SC.register_chiller_indications_value)
-
-    serve(
-        SD,
-        service_call_handler,
-        service_starts_handler,
-        isolate=ISOLATED,
-        as_standalone=as_standalone,
-    )
 
 
 if __name__ == "__main__":
     start()
```

