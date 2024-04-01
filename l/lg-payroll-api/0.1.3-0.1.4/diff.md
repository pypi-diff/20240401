# Comparing `tmp/lg_payroll_api-0.1.3.tar.gz` & `tmp/lg_payroll_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lg_payroll_api-0.1.3.tar", max compression
+gzip compressed data, was "lg_payroll_api-0.1.4.tar", max compression
```

## Comparing `lg_payroll_api-0.1.3.tar` & `lg_payroll_api-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1078 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/LICENSE
--rw-r--r--   0        0        0     1953 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/README.md
--rw-r--r--   0        0        0     1286 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/__init__.py
--rw-r--r--   0        0        0      134 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/helpers/__init__.py
--rw-r--r--   0        0        0     4891 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/helpers/api_results.py
--rw-r--r--   0        0        0     1781 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/helpers/authentication.py
--rw-r--r--   0        0        0     1364 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/helpers/base_client.py
--rw-r--r--   0        0        0      353 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/scripts/__init__.py
--rw-r--r--   0        0        0     1947 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/scripts/company.py
--rw-r--r--   0        0        0     3495 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/scripts/cost_center.py
--rw-r--r--   0        0        0     3595 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/scripts/employee.py
--rw-r--r--   0        0        0     7371 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/scripts/employment_contract.py
--rw-r--r--   0        0        0     6171 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/scripts/organizational_unit.py
--rw-r--r--   0        0        0        0 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/utils/__init__.py
--rw-r--r--   0        0        0      766 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/utils/aux_functions.py
--rw-r--r--   0        0        0      852 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/utils/aux_types.py
--rw-r--r--   0        0        0      687 2024-03-26 12:54:38.540177 lg_payroll_api-0.1.3/lg_payroll_api/utils/lg_exceptions.py
--rw-r--r--   0        0        0      633 2024-03-26 12:54:38.544177 lg_payroll_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 lg_payroll_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1953 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/README.md
+-rw-r--r--   0        0        0     1286 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/__init__.py
+-rw-r--r--   0        0        0      134 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/helpers/__init__.py
+-rw-r--r--   0        0        0     4891 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/helpers/api_results.py
+-rw-r--r--   0        0        0     1781 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/helpers/authentication.py
+-rw-r--r--   0        0        0     1364 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/helpers/base_client.py
+-rw-r--r--   0        0        0      353 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/scripts/__init__.py
+-rw-r--r--   0        0        0     1947 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/scripts/company.py
+-rw-r--r--   0        0        0     3495 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/scripts/cost_center.py
+-rw-r--r--   0        0        0     3595 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/scripts/employee.py
+-rw-r--r--   0        0        0     8472 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/scripts/employment_contract.py
+-rw-r--r--   0        0        0     6171 2024-04-01 20:14:04.516716 lg_payroll_api-0.1.4/lg_payroll_api/scripts/organizational_unit.py
+-rw-r--r--   0        0        0        0 2024-04-01 20:14:04.520716 lg_payroll_api-0.1.4/lg_payroll_api/utils/__init__.py
+-rw-r--r--   0        0        0      766 2024-04-01 20:14:04.520716 lg_payroll_api-0.1.4/lg_payroll_api/utils/aux_functions.py
+-rw-r--r--   0        0        0     1048 2024-04-01 20:14:04.520716 lg_payroll_api-0.1.4/lg_payroll_api/utils/aux_types.py
+-rw-r--r--   0        0        0      687 2024-04-01 20:14:04.520716 lg_payroll_api-0.1.4/lg_payroll_api/utils/lg_exceptions.py
+-rw-r--r--   0        0        0      633 2024-04-01 20:14:04.520716 lg_payroll_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 lg_payroll_api-0.1.4/PKG-INFO
```

### Comparing `lg_payroll_api-0.1.3/LICENSE` & `lg_payroll_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/README.md` & `lg_payroll_api-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/__init__.py` & `lg_payroll_api-0.1.4/lg_payroll_api/__init__.py`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/helpers/api_results.py` & `lg_payroll_api-0.1.4/lg_payroll_api/helpers/api_results.py`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/helpers/authentication.py` & `lg_payroll_api-0.1.4/lg_payroll_api/helpers/authentication.py`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/helpers/base_client.py` & `lg_payroll_api-0.1.4/lg_payroll_api/helpers/base_client.py`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/scripts/company.py` & `lg_payroll_api-0.1.4/lg_payroll_api/scripts/company.py`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/scripts/cost_center.py` & `lg_payroll_api-0.1.4/lg_payroll_api/scripts/cost_center.py`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/scripts/employee.py` & `lg_payroll_api-0.1.4/lg_payroll_api/scripts/employee.py`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/scripts/employment_contract.py` & `lg_payroll_api-0.1.4/lg_payroll_api/scripts/employment_contract.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from datetime import date
+from typing import Any, Literal
 
 from zeep.helpers import serialize_object
 
 from lg_payroll_api.helpers.api_results import (
     LgApiExecutionReturn,
     LgApiPaginationReturn,
     LgApiReturn,
 )
 from lg_payroll_api.helpers.base_client import BaseLgServiceClient, LgAuthentication
 from lg_payroll_api.utils.aux_types import (
     SITUATIONS,
     EnumTipoDeDadosModificados,
     EnumTipoDeOperacaoContratoLog,
+    EnumCampoDeBuscaDoContratoDeTrabalho,
 )
 
 
 class LgApiEmploymentContract(BaseLgServiceClient):
     def __init__(self, lg_auth: LgAuthentication):
         super().__init__(lg_auth=lg_auth, wsdl_service="v2/ServicoDeContratoDeTrabalho")
 
@@ -32,14 +34,44 @@
                 self.send_request(
                     service_client=self.wsdl_client.service.Consultar,
                     body=body,
                 )
             )
         )
 
+    def consult_list(
+        self,
+        company_code: int,
+        search_field: EnumCampoDeBuscaDoContratoDeTrabalho = None,
+        search_value: str = None,
+        employee_type: Literal["Funcionário", "Autônomo"] = None,
+    ) -> LgApiReturn:
+        if (
+            search_field == None and not search_value == None
+            or search_value == None and not search_field == None
+        ):
+            raise ValueError("If search field is defined, you need to define a search value or vice versa.")
+
+        body = {
+            "Empresa": {
+                "FiltroComCodigoNumerico": {"Codigo": company_code}
+            },
+            "CampoDeBusca": search_field,
+            "TipoDoColaborador": employee_type,
+            "TermoDeBusca": search_value,
+        }
+        return LgApiReturn(
+            **serialize_object(
+                self.send_request(
+                    service_client=self.wsdl_client.service.ConsultarLista,
+                    body=body,
+                )
+            )
+        )
+
     def list_on_demand(
         self,
         companies: list[int] = None,
         offices: list[tuple[int, int]] = None,
         employee_status: list[SITUATIONS] = None,
         current_page: int = None,
     ) -> LgApiPaginationReturn:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/scripts/organizational_unit.py` & `lg_payroll_api-0.1.4/lg_payroll_api/scripts/organizational_unit.py`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/utils/aux_functions.py` & `lg_payroll_api-0.1.4/lg_payroll_api/utils/aux_functions.py`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/utils/aux_types.py` & `lg_payroll_api-0.1.4/lg_payroll_api/utils/aux_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,7 +37,19 @@
     NENHUM = 0
     OBJETO_SEM_ALTERACAO = 1
     CADASTRO = 2
     ATUALIZACAO = 3
     EXCLUSAO = 4
     CADASTRO_EM_LOTE = 5
     VALIDACAO = 6
+
+
+class EnumCampoDeBuscaDoContratoDeTrabalho(int, Enum):
+    MATRICULA = 0
+    ID_PESSOA = 1
+    CPF = 2
+    IDENTIDADE = 3
+    RIC = 4
+    CTPS = 5
+    PIS = 6
+    TITULO_ELEITOR = 7
+    CNH = 8
```

### Comparing `lg_payroll_api-0.1.3/lg_payroll_api/utils/lg_exceptions.py` & `lg_payroll_api-0.1.4/lg_payroll_api/utils/lg_exceptions.py`

 * *Files identical despite different names*

### Comparing `lg_payroll_api-0.1.3/pyproject.toml` & `lg_payroll_api-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lg-payroll-api"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["stone_people_analytics <systems-techpeople@stone.com.br>"]
 maintainers = [
     "diogo56 <diogo.amorim2001@gmail.com>",
     "guilherme_lsilva <manager.guilherme.silva@gmail.com>",
     "root-who <joaopaulo_gonzaga@outlook.com>",
 ]
```

### Comparing `lg_payroll_api-0.1.3/PKG-INFO` & `lg_payroll_api-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lg-payroll-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Home-page: https://github.com/people-analytics-tech/lg-payroll-api
 License: MIT
 Author: stone_people_analytics
 Author-email: systems-techpeople@stone.com.br
 Maintainer: diogo56
 Maintainer-email: diogo.amorim2001@gmail.com
```

