# Comparing `tmp/fastapix_py-0.7.4-py3-none-any.whl.zip` & `tmp/fastapix_py-0.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 2470741 bytes, number of entries: 39
+Zip file size: 2470742 bytes, number of entries: 39
 -rw-r--r--  2.0 unx      638 b- defN 20-Feb-02 00:00 fastapix/__init__.py
 -rw-r--r--  2.0 unx      196 b- defN 20-Feb-02 00:00 fastapix/__main__.py
 -rw-r--r--  2.0 unx      425 b- defN 20-Feb-02 00:00 fastapix/exceptions.py
 -rw-r--r--  2.0 unx     2274 b- defN 20-Feb-02 00:00 fastapix/handlers.py
 -rw-r--r--  2.0 unx      224 b- defN 20-Feb-02 00:00 fastapix/innerclient.py
 -rw-r--r--  2.0 unx    15404 b- defN 20-Feb-02 00:00 fastapix/main.py
 -rw-r--r--  2.0 unx     2211 b- defN 20-Feb-02 00:00 fastapix/responses.py
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 fastapix/common/__init__.py
--rw-r--r--  2.0 unx    18853 b- defN 20-Feb-02 00:00 fastapix/common/pydantic.py
+-rw-r--r--  2.0 unx    18913 b- defN 20-Feb-02 00:00 fastapix/common/pydantic.py
 -rw-r--r--  2.0 unx     1430 b- defN 20-Feb-02 00:00 fastapix/common/serializer.py
 -rw-r--r--  2.0 unx      301 b- defN 20-Feb-02 00:00 fastapix/crud/__init__.py
 -rw-r--r--  2.0 unx     9912 b- defN 20-Feb-02 00:00 fastapix/crud/_models.py
 -rw-r--r--  2.0 unx     8081 b- defN 20-Feb-02 00:00 fastapix/crud/_router.py
 -rw-r--r--  2.0 unx     8358 b- defN 20-Feb-02 00:00 fastapix/crud/_selecter.py
 -rw-r--r--  2.0 unx     8827 b- defN 20-Feb-02 00:00 fastapix/crud/_sqlalchemy.py
 -rw-r--r--  2.0 unx    22334 b- defN 20-Feb-02 00:00 fastapix/crud/_sqlmodel.py
@@ -30,12 +30,12 @@
 -rw-r--r--  2.0 unx   260489 b- defN 20-Feb-02 00:00 fastapix/offline/static/openapi/swagger-ui.css.map
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 fastapix/sso/__init__.py
 -rw-r--r--  2.0 unx     3172 b- defN 20-Feb-02 00:00 fastapix/sso/_main.py
 -rw-r--r--  2.0 unx      156 b- defN 20-Feb-02 00:00 fastapix/sso/base/__init__.py
 -rw-r--r--  2.0 unx     1272 b- defN 20-Feb-02 00:00 fastapix/sso/base/_cas.py
 -rw-r--r--  2.0 unx      163 b- defN 20-Feb-02 00:00 fastapix/sso/plugin/__init__.py
 -rw-r--r--  2.0 unx     1957 b- defN 20-Feb-02 00:00 fastapix/sso/plugin/casdoor.py
-?rw-r--r--  2.0 unx     3899 b- defN 20-Feb-02 00:00 fastapix_py-0.7.4.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 fastapix_py-0.7.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11558 b- defN 20-Feb-02 00:00 fastapix_py-0.7.4.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     3379 b- defN 20-Feb-02 00:00 fastapix_py-0.7.4.dist-info/RECORD
-39 files, 8835751 bytes uncompressed, 2465347 bytes compressed:  72.1%
+?rw-r--r--  2.0 unx     3907 b- defN 20-Feb-02 00:00 fastapix_py-0.7.5.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 fastapix_py-0.7.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11558 b- defN 20-Feb-02 00:00 fastapix_py-0.7.5.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     3379 b- defN 20-Feb-02 00:00 fastapix_py-0.7.5.dist-info/RECORD
+39 files, 8835819 bytes uncompressed, 2465348 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -99,20 +99,20 @@
 
 Filename: fastapix/sso/plugin/__init__.py
 Comment: 
 
 Filename: fastapix/sso/plugin/casdoor.py
 Comment: 
 
-Filename: fastapix_py-0.7.4.dist-info/METADATA
+Filename: fastapix_py-0.7.5.dist-info/METADATA
 Comment: 
 
-Filename: fastapix_py-0.7.4.dist-info/WHEEL
+Filename: fastapix_py-0.7.5.dist-info/WHEEL
 Comment: 
 
-Filename: fastapix_py-0.7.4.dist-info/licenses/LICENSE
+Filename: fastapix_py-0.7.5.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: fastapix_py-0.7.4.dist-info/RECORD
+Filename: fastapix_py-0.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapix/__init__.py

```diff
@@ -1,13 +1,13 @@
 # !/usr/bin/env Python3
 # -*- coding: utf-8 -*-
 # @Author   : zhangzhanqi
 # @FILE     : __init__.py
 # @Time     : 2023/11/16 16:37
-__version__ = "0.7.4"
+__version__ = "0.7.5"
 
 
 from fastapi import FastAPI
 
 from .main import run, main
```

## fastapix/common/pydantic.py

```diff
@@ -17,15 +17,14 @@
 UnionType = getattr(types, "UnionType", Union)
 NoneType = type(None)
 _TSQLModel = TypeVar("_TSQLModel", bound="SQLModel")
 
 PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
 
 if PYDANTIC_V2:
-    from pydantic.fields import AliasChoices, AliasPath
     from pydantic._internal._fields import PydanticMetadata  # noqa: F401
     from pydantic.v1.datetime_parse import parse_date, parse_datetime  # noqa: F401
     from pydantic_settings import BaseSettings  # noqa: F401
 
     GenericModel = BaseModel
     from pydantic import model_validator  # noqa: F401
     from pydantic.v1.typing import is_literal_type, is_none_type, is_union  # noqa: F401
@@ -103,23 +102,23 @@
         return fields
 
 
     def model_config(model: Type[BaseModel]) -> Union[type, Dict[str, Any]]:
         return model.model_config  # noqa: F401
 
 
-    def marge_model_config(config: Union[ConfigDict, BaseConfig], update: Dict[str, Any]) -> Union[type, Dict[str, Any]]:
+    def marge_model_config(config: Union[ConfigDict, BaseConfig], update: Dict[str, Any]) -> Union[
+        type, Dict[str, Any]]:
         if config is None:
             config = AllowExtraModelMixin.model_config
         if isinstance(config, BaseConfig):
             return {**config.__dict__, **update}
         return {**config, **update}  # noqa: F401
 
 
-
     def model_config_attr(model: Type[BaseModel], name: str, default: Any = None) -> Any:
         return model.model_config.get(name, default)  # noqa: F401
 
 
     def model_dump(model: BaseModel, *args, **kwargs) -> Dict[str, Any]:
         return model.model_dump(*args, **kwargs)  # noqa: F401
 
@@ -147,14 +146,15 @@
                 type_ = bases[0] if bases[0] is not NoneType else bases[1]
                 return _get_origin(type_)
             return origin
 
         origin = _get_origin(type_)
         return origin
 
+
     def is_field_noneable(field: ModelField) -> bool:
         field_info = field.field_info
         if getattr(field_info, "nullable", Undefined) is not Undefined:
             return field_info.nullable  # type: ignore
         origin = get_origin(field_info.annotation)
         if origin is not None and (origin is UnionType or origin is Union):
             args = get_args(field_info.annotation)
@@ -164,73 +164,75 @@
             if field_info.default is Undefined:
                 return False
             if field_info.annotation is None or field_info.annotation is NoneType:  # type: ignore[comparison-overlap]
                 return True
             return False
         return False
 
+
     def sqlmodel_table_construct(
-        *,
-        self_instance: _TSQLModel,
-        values: Dict[str, Any],
-        _fields_set: Union[Set[str], None] = None,
+            *,
+            self_instance: _TSQLModel,
+            values: Dict[str, Any],
+            _fields_set: Union[Set[str], None] = None,
     ) -> _TSQLModel:
         # Copy from SQLModel's _compat.sqlmodel_table_construct Ref:
         # https://github.com/tiangolo/sqlmodel/blob/0c7def88b5d9652bf9288738e2e9276d9dd24b5f/sqlmodel/_compat.py#L210
         cls = type(self_instance)
         old_dict = self_instance.__dict__.copy()
 
         fields_values: Dict[str, Any] = {}
         defaults: Dict[
             str, Any
         ] = {}  # keeping this separate from `fields_values` helps us compute `_fields_set`
         # SQLModel override BaseModel, value BaseModel.validate
         errs = []
         for name, field in model_fields(cls).items():
-            if field.alias and field.alias in values:
-                _v = values.get(field.alias)
+            field_alias = field.field_info.alias or field.field_info.validation_alias
+            if field_alias and field_alias in values:
+                _v = values.get(field_alias)
                 fields_values[name], err = field.validate(_v)
                 if err:
                     if getattr(field.field_info, "primary_key", None) and err[0].get('input') is None:
                         # 主键默认None, 将自动生成主键值
                         continue
                     for e in err:
                         if e['loc']:
                             e['loc'] = [f"{name}.{loc}" for loc in e['loc']]
                         else:
-                            e['loc'] = e['loc'] or (field.field_info.title or name,)
+                            e['loc'] = e['loc'] or (name,)
                     errs.extend(err)
             elif name in values:
                 _v = values.get(name)
                 fields_values[name], err = field.validate(_v)
                 if err:
-                    if getattr(field.field_info, "primary_key", None) and err[0].get('input') is None:
+                    if getattr(field.field_info, "primary_key", None) is True and err[0].get('input') is None:
                         # 主键默认None, 将自动生成主键值
                         continue
                     for e in err:
                         if e['loc']:
                             e['loc'] = [f"{name}.{loc}" for loc in e['loc']]
                         else:
                             e['loc'] = (name,)
                     errs.extend(err)
             elif not field.required:
                 _v = field.get_default()
                 defaults[name], err = field.validate(_v)
                 if err:
-                    if getattr(field.field_info, "primary_key", None) and err[0].get('input') is None:
+                    if getattr(field.field_info, "primary_key", None) is True and err[0].get('input') is None:
                         # 主键默认None, 将自动生成主键值
                         continue
                     for e in err:
                         if e['loc']:
                             e['loc'] = [f"{name}.{loc}" for loc in e['loc']]
                         else:
                             e['loc'] = (name,)
                     errs.extend(err)
             elif field.required:
-                if getattr(field.field_info, "primary_key", None):
+                if getattr(field.field_info, "primary_key", None) is True:
                     # 主键默认None, 将自动生成主键值
                     continue
                 errs.extend([InitErrorDetails(type='missing', loc=(name,), input=values)])
         if errs:
             raise ValidationError.from_exception_data(
                 title=self_instance.__class__.__name__,
                 line_errors=[InitErrorDetails(**err) for err in errs],
@@ -256,14 +258,15 @@
             object.__setattr__(self_instance, "__pydantic_private__", None)
         for key in self_instance.__sqlmodel_relationships__:
             value = values.get(key, Undefined)
             if value is not Undefined:
                 setattr(self_instance, key, value)
         return self_instance
 
+
     def sqlmodel_init(*, self: "SQLModel", data: Dict[str, Any]) -> None:
         # Copy sqlmodel._compat
         old_dict = self.__dict__.copy()
         if not is_table_model_class(self.__class__):
             self.__pydantic_validator__.validate_python(
                 data,
                 self_instance=self,
@@ -379,19 +382,20 @@
         if isinstance(field.type_, type) and field.shape == SHAPE_SINGLETON:
             return field.type_
         elif isinstance(field.type_, type) and field.shape in (SHAPE_LIST, SHAPE_SET, SHAPE_TUPLE, SHAPE_SEQUENCE):
             return list
         elif isinstance(field.type_, type) and field.shape in (SHAPE_DICT, SHAPE_DEFAULTDICT):
             return dict
 
+
     def is_field_noneable(field: ModelField) -> bool:
         if not field.required:  # type: ignore[attr-defined]
             # Taken from [Pydantic](https://github.com/samuelcolvin/pydantic/blob/v1.8.2/pydantic/fields.py#L946-L947)
             return field.allow_none and (  # type: ignore[attr-defined]
-                field.shape != SHAPE_SINGLETON or not field.sub_fields  # type: ignore[attr-defined]
+                    field.shape != SHAPE_SINGLETON or not field.sub_fields  # type: ignore[attr-defined]
             )
         return field.allow_none  # type: ignore[no-any-return, attr-defined]
 
 
     def sqlmodel_init(*, self: "SQLModel", data: Dict[str, Any]) -> None:
         # Copy sqlmodel._compat
         values, fields_set, validation_error = validate_model(self.__class__, data)
```

## Comparing `fastapix_py-0.7.4.dist-info/METADATA` & `fastapix_py-0.7.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fastapix-py
-Version: 0.7.4
+Version: 0.7.5
 Summary: A FastAPI plugin that quickly builds CRUD-API based on SQLAlchemy
 Project-URL: Homepage, https://gitee.com/kaiqione/fastapix
 Project-URL: Repository, https://gitee.com/kaiqione/fastapix
 Project-URL: Source, https://gitee.com/kaiqione/fastapix
 Author-email: zhangzhanqi <zzq120203@163.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: fastapi
 Requires-Dist: loguru
 Requires-Dist: pydantic[email]
 Requires-Dist: sqlalchemy-database
-Requires-Dist: sqlmodel
+Requires-Dist: sqlmodel>=0.0.14
 Requires-Dist: uvicorn[standard]
 Provides-Extra: casdoor
 Requires-Dist: aiohttp; extra == 'casdoor'
 Requires-Dist: casdoor; extra == 'casdoor'
 Requires-Dist: cryptography; extra == 'casdoor'
 Requires-Dist: itsdangerous; extra == 'casdoor'
 Requires-Dist: pyjwt; extra == 'casdoor'
```

## Comparing `fastapix_py-0.7.4.dist-info/licenses/LICENSE` & `fastapix_py-0.7.5.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapix_py-0.7.4.dist-info/RECORD` & `fastapix_py-0.7.5.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-fastapix/__init__.py,sha256=k-2gwfOlmXZvPT6CIO2phIrl3UgAhpxVXhRuYov0Fus,638
+fastapix/__init__.py,sha256=fO5GzOLTz8sLVY7VdObdJQ7w99fMMOUqtlTHeHhE57o,638
 fastapix/__main__.py,sha256=qgNubHbROxqYWp6jEgD-uhczpvt7d8MEpEA1VPr0UVw,196
 fastapix/exceptions.py,sha256=nVVh2-gWqzcHrNGfyU_lHN-EG2MHv3dfPbmIZwAiiHM,425
 fastapix/handlers.py,sha256=2lRjy0JZZAqTN37yntOgTOh_JvTWeNlRXDyh4dPMZgk,2274
 fastapix/innerclient.py,sha256=39hdDGWP1C7KKbYZ-6X4RIeRBJCsDBctoLHbBvLF4Kc,224
 fastapix/main.py,sha256=JUgonmAqrOjeqHtXRuNQm20anb04nbmUEqcVpD1IXh0,15404
 fastapix/responses.py,sha256=lFun2Mn8UQXAqJeaKyaya9OMX9TN0pI78fPPWnMTQ6k,2211
 fastapix/common/__init__.py,sha256=3PwrW-AbN6xjeONyF0W-qtQt4Zi-qx4g_Xeb4TGCCR8,134
-fastapix/common/pydantic.py,sha256=b7TjqrS8xqnZAD_oClJzhVTmwXsyjR6ywfH2F4ok19g,18853
+fastapix/common/pydantic.py,sha256=00IZvlymMW5y-7xnoL-g9aBbDw9_p63-DsQjzu8pl1U,18913
 fastapix/common/serializer.py,sha256=ob2IVcbcsiG558lIcz-s2vjcpNgCxMxwLWyD9aagTm0,1430
 fastapix/crud/__init__.py,sha256=kCq6wsUBEC_Q4QZjw29T56eQiIUcp4sqa6rZDaOk7Wg,301
 fastapix/crud/_models.py,sha256=PvC--OTxLR7QdYwhI0j_n3iuGNjp4-gN6C26mf-xXTA,9912
 fastapix/crud/_router.py,sha256=O1MBjLprTUlZWsQZ35lVMwKMR8_WFhwuGT2G2IGB-hY,8081
 fastapix/crud/_selecter.py,sha256=INmU2JrYyvSZsitRD-LOLrtVUsyZs3OalLPWOujeMLA,8358
 fastapix/crud/_sqlalchemy.py,sha256=tyAmcen3P2sl1Gv_6Tif1uGJvgigBjrorCGfM4Qi7U0,8827
 fastapix/crud/_sqlmodel.py,sha256=GiVn5aBVfqgI9csRkXyT8YPw37JBO_njzuqi8V2lzMM,22334
@@ -29,11 +29,11 @@
 fastapix/offline/static/openapi/swagger-ui.css.map,sha256=GgsE41JXzVK1xNz-Wsi-VK-8axxLKhIK2_L2d1BGPRo,260489
 fastapix/sso/__init__.py,sha256=vpy4EQeIvvq2NkHDLjMFDUgMxbv__9XZPw762hHGglM,134
 fastapix/sso/_main.py,sha256=tW1b76g1TC2-_EAyxzC1q8ZJUmh2aAZxNunhCcruMI8,3172
 fastapix/sso/base/__init__.py,sha256=XAXJPawH9f9ZkE3ZQEkqEKdbGwITzASCbMNkSIgPO54,156
 fastapix/sso/base/_cas.py,sha256=Qs5wIfNnFRsDoRRfnaQTcoiDzpZrnWn-gPFbxb6IHBo,1272
 fastapix/sso/plugin/__init__.py,sha256=0dhq1dhGYhSjKZBOxlLJooGY-A4g8RvRpI3Un2PoQKk,163
 fastapix/sso/plugin/casdoor.py,sha256=9s8brFUuUekPGbGOposOT2dZj0TC361H3xwSFbG2F6Y,1957
-fastapix_py-0.7.4.dist-info/METADATA,sha256=V7Xq-f7Ea0qZJzMaH2th4PoJgPdXa9sfgOwyYYUPkD4,3899
-fastapix_py-0.7.4.dist-info/WHEEL,sha256=mRYSEL3Ih6g5a_CVMIcwiF__0Ae4_gLYh01YFNwiq1k,87
-fastapix_py-0.7.4.dist-info/licenses/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-fastapix_py-0.7.4.dist-info/RECORD,,
+fastapix_py-0.7.5.dist-info/METADATA,sha256=GFt-57rbg1EXTDgmAW2tbVD7YnM61h073RdIvth2ymY,3907
+fastapix_py-0.7.5.dist-info/WHEEL,sha256=mRYSEL3Ih6g5a_CVMIcwiF__0Ae4_gLYh01YFNwiq1k,87
+fastapix_py-0.7.5.dist-info/licenses/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+fastapix_py-0.7.5.dist-info/RECORD,,
```

