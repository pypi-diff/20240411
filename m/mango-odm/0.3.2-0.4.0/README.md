# Comparing `tmp/mango_odm-0.3.2.tar.gz` & `tmp/mango_odm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango_odm-0.3.2.tar", last modified: Tue Aug  8 13:24:05 2023, max compression
+gzip compressed data, was "mango_odm-0.4.0.tar", last modified: Thu Apr 11 16:30:08 2024, max compression
```

## Comparing `mango_odm-0.3.2.tar` & `mango_odm-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-08-08 13:23:57.531989 mango_odm-0.3.2/LICENSE
--rw-r--r--   0        0        0     4815 2023-08-08 13:23:57.531989 mango_odm-0.3.2/README.md
--rw-r--r--   0        0        0      445 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/__init__.py
--rw-r--r--   0        0        0     4331 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/drive.py
--rw-r--r--   0        0        0     1110 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/encoder.py
--rw-r--r--   0        0        0     5639 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/expression.py
--rw-r--r--   0        0        0     3284 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/fields.py
--rw-r--r--   0        0        0     1665 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/index.py
--rw-r--r--   0        0        0     1040 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/meta.py
--rw-r--r--   0        0        0     9294 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/models.py
--rw-r--r--   0        0        0        0 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/py.typed
--rw-r--r--   0        0        0     6570 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/result.py
--rw-r--r--   0        0        0     2221 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/source.py
--rw-r--r--   0        0        0    16192 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/stage.py
--rw-r--r--   0        0        0     4405 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/utils.py
--rw-r--r--   0        0        0     2533 2023-08-08 13:24:05.240160 mango_odm-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     6047 1970-01-01 00:00:00.000000 mango_odm-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-11 16:30:05.457423 mango_odm-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4815 2024-04-11 16:30:05.457423 mango_odm-0.4.0/README.md
+-rw-r--r--   0        0        0      445 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/__init__.py
+-rw-r--r--   0        0        0     4275 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/drive.py
+-rw-r--r--   0        0        0     1110 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/encoder.py
+-rw-r--r--   0        0        0     5803 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/expression.py
+-rw-r--r--   0        0        0     5536 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/fields.py
+-rw-r--r--   0        0        0     1682 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/index.py
+-rw-r--r--   0        0        0      387 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/meta.py
+-rw-r--r--   0        0        0     9782 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/models.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/py.typed
+-rw-r--r--   0        0        0     6705 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/result.py
+-rw-r--r--   0        0        0     2238 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/source.py
+-rw-r--r--   0        0        0    16192 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/stage.py
+-rw-r--r--   0        0        0     4307 2024-04-11 16:30:05.457423 mango_odm-0.4.0/mango/utils.py
+-rw-r--r--   0        0        0     2109 2024-04-11 16:30:08.057419 mango_odm-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6074 1970-01-01 00:00:00.000000 mango_odm-0.4.0/PKG-INFO
```

### Comparing `mango_odm-0.3.2/LICENSE` & `mango_odm-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.2/README.md` & `mango_odm-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.2/mango/drive.py` & `mango_odm-0.4.0/mango/drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.db = db
         self.collections: dict[str, Collection] = {}
 
     def __getattr__(self, name: str) -> Collection:
         try:
             return self.collections[name]
         except KeyError:
-            collection: AsyncIOMotorCollection = self.db.get_collection(name)
+            collection = self.db.get_collection(name)
             self.collections[name] = Collection(collection)
             return self.collections[name]
 
     def __getitem__(self, name: str) -> Collection:
         return self.__getattr__(name)
 
     def __iter__(self) -> Iterator[Collection]:
@@ -82,15 +82,15 @@
         self.databases: dict[str, Database] = {}
         self.__class__._clients.add(self)
 
     def __getattr__(self, name: str) -> Database:
         try:
             return self.databases[name]
         except KeyError:
-            db: AsyncIOMotorDatabase = self.client.get_database(name)
+            db = self.client.get_database(name)
             self.databases[name] = Database(db)
             return self.databases[name]
 
     def __getitem__(self, name: str) -> Database:
         return self.__getattr__(name)
 
     def __iter__(self) -> Iterator[Database]:
@@ -116,15 +116,15 @@
         try:
             client = next(iter(cls._clients))
         except StopIteration:
             client = cls()
 
         if isinstance(db, Database):
             return db
-        return client[db] if isinstance(db, str) else client.default_database
+        return client[db] if db else client.default_database
 
     @property
     def default_database(self) -> Database:
         """默认为首次调用的数据库, 如果不存在, 则创建 test 数据库"""
         try:
             return next(iter(self.databases.values()))
         except StopIteration:
@@ -136,9 +136,9 @@
         return self.client.HOST
 
     @property
     def port(self) -> int:
         return self.client.PORT
 
     @property
-    def address(self) -> tuple[str, int]:
+    def address(self) -> tuple[str, int] | None:
         return self.client.address
```

### Comparing `mango_odm-0.3.2/mango/encoder.py` & `mango_odm-0.4.0/mango/encoder.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.2/mango/expression.py` & `mango_odm-0.4.0/mango/expression.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import TYPE_CHECKING, Any
 
-from pydantic.fields import ModelField
+from pydantic._internal import _repr
 from typing_extensions import Self
 
 from mango.fields import FieldInfo
 
 if TYPE_CHECKING:  # pragma: no cover
     from mango.models import Document
 
@@ -39,23 +39,24 @@
 
     def __str__(self) -> str:
         return f"${self.name.lower()}"
 
 
 class ExpressionField:
     def __init__(
-        self, field: ModelField, parents: list[tuple[str, "Document"]]
+        self, name: str, field: FieldInfo, parents: list[tuple[str, "Document"]]
     ) -> None:
-        self.field = field
-        self.parents = parents
+        self.__name = name
+        self.__field = field
+        self.__parents = parents
 
-    def __eq__(self, other: Any) -> "Expression":
+    def __eq__(self, other: object) -> "Expression":
         return OPR(self).eq(other)
 
-    def __ne__(self, other: Any) -> "Expression":
+    def __ne__(self, other: object) -> "Expression":
         return OPR(self).ne(other)
 
     def __lt__(self, other: Any) -> "Expression":
         return OPR(self).lt(other)
 
     def __le__(self, other: Any) -> "Expression":
         return OPR(self).lte(other)
@@ -66,46 +67,47 @@
     def __ge__(self, other: Any) -> "Expression":
         return OPR(self).gte(other)
 
     def __hash__(self) -> int:
         return super().__hash__()
 
     def __repr__(self) -> str:
-        return f"ExpressionField(name={self!s}, type={self.field._type_display()})"
+        annotation = _repr.PlainRepr(_repr.display_as_type(self.__field.annotation))
+        return f"ExpressionField(name={self!s}, type={annotation})"
 
     def __str__(self) -> str:
-        names = [p[0] for p in self.parents]
-        if isinstance(finfo := self.field.field_info, FieldInfo) and finfo.primary_key:
+        names = [p[0] for p in self.__parents]
+        if isinstance(self.__field, FieldInfo) and self.__field.primary_key:
             names.append("_id")
         else:
-            names.append(self.field.name)
+            names.append(self.__name)
         return ".".join(names)
 
     def __getattr__(self, name: str) -> Any:
         """内嵌查询反向查找分配父级"""
-        attr = getattr(self.field.outer_type_, name)
-        if isinstance(attr, self.__class__):
-            new_parent = (self.field.name, self.field.outer_type_)
-            if new_parent not in attr.parents:
-                attr.parents.append(new_parent)
-            if new_parents := list(set(self.parents) - set(attr.parents)):
-                attr.parents = new_parents + attr.parents
+        attr = object.__getattribute__(self.__field.annotation, name)
+        if isinstance(attr, self.__class__) and self.__field.annotation:
+            new_parent = (self.__name, self.__field.annotation)
+            if new_parent not in attr.__parents:
+                attr.__parents.append(new_parent)
+            if new_parents := list(set(self.__parents) - set(attr.__parents)):
+                attr.__parents = new_parents + attr.__parents
         return attr
 
 
 @dataclass
 class Expression:
     key: ExpressionField | None
     operator: Operators
     value: Any
 
-    def __or__(self, other: Self) -> Self:
+    def __or__(self, other: Self) -> "Expression":
         return OPR.or_(self, other)
 
-    def __and__(self, other: Self) -> Self:
+    def __and__(self, other: Self) -> "Expression":
         return OPR.and_(self, other)
 
     def __repr__(self) -> str:
         return f"Expression({self.struct()})"
 
     def struct(self) -> dict[str, Any]:
         """转换为 MongoDB 查询结构"""
@@ -164,21 +166,21 @@
     @classmethod
     def and_(cls, *expressions: Expression | bool) -> Expression:
         merge = cls._merge(Operators.AND, expressions)
         return Expression(None, *merge)
 
     @classmethod
     def nor(cls, *expressions: Expression | bool) -> Expression:
-        """既不……也不……"""
+        """既不也不"""
         merge = cls._merge(Operators.NOR, expressions)
         return Expression(None, *merge)
 
     @classmethod
     def _merge(
-        cls, operator: Operators, expressions: tuple[Expression | bool]
+        cls, operator: Operators, expressions: tuple[Expression | bool, ...]
     ) -> tuple[Operators, list[Expression]]:
         merge_expr: list[Expression] = []
         for expression in expressions:
             if not isinstance(expression, Expression):
                 raise TypeError("必须是有效的表达式")
 
             if expression.operator is operator:
```

### Comparing `mango_odm-0.3.2/mango/index.py` & `mango_odm-0.4.0/mango/index.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ASC = pymongo.ASCENDING
     """升序排序"""
     DESC = pymongo.DESCENDING
     """降序排序"""
 
 
 @unique
-class Attr(str, IndexEnum):
+class Attr(str, IndexEnum):  # noqa: SLOT000
     GEO2D = pymongo.GEO2D
     """二维地理空间索引"""
     GEOSPHERE = pymongo.GEOSPHERE
     """球型地理空间索引"""
     HASHED = pymongo.HASHED
     """散列索引"""
     TEXT = pymongo.TEXT
```

### Comparing `mango_odm-0.3.2/mango/models.py` & `mango_odm-0.4.0/mango/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import contextlib
 from collections.abc import Mapping, MutableMapping, Sequence
 from functools import reduce
 from typing import TYPE_CHECKING, Any, ClassVar
 
 import bson
 from bson import ObjectId
-from pydantic import BaseModel
-from pydantic.main import ModelMetaclass
+from pydantic import BaseModel, ConfigDict
+from pydantic._internal._model_construction import ModelMetaclass
 from typing_extensions import Self, dataclass_transform
 
 from mango.encoder import Encoder
 from mango.expression import Expression, ExpressionField, Operators
 from mango.fields import Field, FieldInfo, ObjectIdField
-from mango.meta import MetaConfig, inherit_meta
+from mango.meta import MetaConfig
 from mango.result import AggregateResult, FindMapping, FindResult
 from mango.source import Mango
 from mango.stage import Pipeline
 from mango.utils import add_fields, all_check, validate_fields
 
 if TYPE_CHECKING:
     from bson.codec_options import CodecOptions
-    from pydantic.fields import ModelField
     from pymongo.results import DeleteResult, UpdateResult
 
     from mango.drive import Collection, Database
 
 operators = tuple(str(i) for i in Operators)
 
 
@@ -40,16 +39,26 @@
         return False
 
     # 存在 id 字段但未定义主键，且其被继承
     return not any(getattr(base, "id", None) for base in bases)
 
 
 def set_default_pk(model: type["Document"]) -> None:
-    value = Field(default_factory=ObjectId, allow_mutation=False, init=False)
-    add_fields(model, id=(ObjectIdField, value))
+    add_fields(
+        model,
+        id=(
+            ObjectIdField,
+            {
+                "default_factory": ObjectId,
+                "primary_key": True,
+                "frozen": True,
+                "init": False,
+            },
+        ),
+    )
     model.__primary_key__ = "id"
 
 
 def flat_filter(data: Mapping[str, Any]) -> dict[str, Any]:
     flatted = {}
     for key, value in data.items():
         if key.startswith(operators):
@@ -62,69 +71,92 @@
                 if isinstance(value, dict) and operator in value:
                     flatted[key] = value[operator]
     return flatted
 
 
 def merge_map(data: MutableMapping[Any, Any], into: Mapping[Any, Any]) -> None:
     for k, v in into.items():
-        k = str(k)
+        k = str(k)  # noqa: PLW2901
         if isinstance(data.get(k), dict) and isinstance(v, dict | EmbeddedDocument):
-            merge_map(data[k], v if isinstance(v, dict) else v.dict())
+            merge_map(data[k], v if isinstance(v, dict) else v.model_dump())
         else:
             data[k] = v
 
 
+config_keys = set(MetaConfig.__annotations__.keys())
+
+
+def merge_config(
+    bases: tuple[type[Any], ...], attrs: dict[str, Any], kwargs: dict[str, Any]
+) -> MetaConfig:
+    config = MetaConfig()
+
+    for base in bases:
+        if cfg := getattr(base, "meta_config", None):
+            config.update(cfg.copy())
+
+    config.update(attrs.get("meta_config", MetaConfig()))
+
+    for k in list(kwargs.keys()):
+        if k in config_keys:
+            config[k] = kwargs.pop(k)
+        if k == "db":
+            config["database"] = kwargs.pop(k)
+
+    return config
+
+
 @dataclass_transform(kw_only_default=True, field_specifiers=(Field, FieldInfo))
 class MetaDocument(ModelMetaclass):
     def __new__(
         cls,
         cname: str,
         bases: tuple[type[Any], ...],
         attrs: dict[str, Any],
         **kwargs: Any,
     ) -> Any:
-        meta = MetaConfig
+        # 跳过基类
+        if bases == (BaseModel,):
+            return super().__new__(cls, cname, bases, attrs, **kwargs)
 
-        for base in reversed(bases):
-            if base != BaseModel and issubclass(base, Document):
-                meta = inherit_meta(base.__meta__, MetaConfig)
-
-        kwargs.setdefault("database", kwargs.pop("db", None))
-
-        allowed_meta_kwargs = {
-            key
-            for key in dir(meta)
-            if not (key.startswith("__") and key.endswith("__"))
-        }
-        meta_kwargs = {
-            key: kwargs.pop(key) for key in kwargs.keys() & allowed_meta_kwargs
-        }
+        # 合并配置
+        attrs["meta_config"] = merge_config(bases, attrs, kwargs)
 
-        attrs["__meta__"] = inherit_meta(attrs.get("Meta"), meta, **meta_kwargs)
-        attrs["__encoder__"] = Encoder.create(attrs["__meta__"].bson_encoders)
+        # 创建编码器
+        attrs["__encoder__"] = Encoder.create(attrs["meta_config"].get("bson_encoders"))
 
         scls = super().__new__(cls, cname, bases, attrs, **kwargs)
 
-        # 由于此处代码使用了 setattr，导致子类重写父类的字段时会引发错误，暂无解决办法
-        # NameError: Field name "xxx" shadows a BaseModel attribute;
-        # use a different field name with "alias='xxx'".
-        for fname, field in scls.__fields__.items():
-            setattr(scls, fname, ExpressionField(field, []))
-            if isinstance(finfo := field.field_info, FieldInfo) and finfo.primary_key:
-                pk = finfo.alias or fname
-                if getattr(scls, "__primary_key__", pk) != pk:
-                    raise ValueError("文档的主键应唯一")
-                finfo.allow_mutation = False
-                scls.__primary_key__ = pk
-
-        if not hasattr(scls, "__primary_key__") and is_need_default_pk(
-            bases, attrs.get("__annotations__")
-        ):
+        # 设置模型字段
+        annotations = attrs.get("__annotations__", {})
+        for fname in annotations:
+            field = scls.model_fields[fname]
+            setattr(scls, fname, ExpressionField(fname, field, []))
+
+        # 检查主键是否唯一
+        pk_fields = {
+            fname: field
+            for fname, field in scls.model_fields.items()
+            if isinstance(field, FieldInfo) and field.primary_key
+        }
+        if len(pk_fields) > 1:
+            raise ValueError(
+                f"文档的主键应唯一, 当前有主键字段: {', '.join(pk_fields.keys())}"
+            )
+
+        # 设置显式主键
+        if len(pk_fields) == 1:
+            pk_name, pk_filed = next(iter(pk_fields.items()))
+            scls.__primary_key__ = pk_filed.alias or pk_name
+
+        # 设置默认主键
+        if not pk_fields and is_need_default_pk(bases, annotations):
             set_default_pk(scls)
 
+        # 注册模型
         Mango.register_model(scls)
 
         return scls
 
 
 @dataclass_transform(kw_only_default=True, field_specifiers=(Field, FieldInfo))
 class MetaEmbeddedDocument(ModelMetaclass):
@@ -132,40 +164,39 @@
         cls,
         name: str,
         bases: tuple[type[Any], ...],
         attrs: dict[str, Any],
         **kwargs: Any,
     ) -> Any:
         scls = super().__new__(cls, name, bases, attrs, **kwargs)
-        for fname, field in scls.__fields__.items():
-            setattr(scls, fname, ExpressionField(field, []))
-            if isinstance(finfo := field.field_info, FieldInfo) and finfo.primary_key:
+        for fname, field in scls.model_fields.items():
+            setattr(scls, fname, ExpressionField(fname, field, []))
+            if isinstance(field, FieldInfo) and field.primary_key:
                 raise ValueError("内嵌文档不可设置主键")
         return scls
 
 
 class Document(BaseModel, metaclass=MetaDocument):
     if TYPE_CHECKING:  # pragma: no cover
         id: ClassVar[ObjectId]
-        __fields__: ClassVar[dict[str, ModelField]]
-        __meta__: ClassVar[type[MetaConfig]]
+        model_fields: ClassVar[dict[str, FieldInfo]]
         __encoder__: ClassVar[CodecOptions]
         __collection__: ClassVar[Collection]
         __primary_key__: ClassVar[str]
 
         def __init_subclass__(
             cls,
             *,
             name: str | None = None,
             db: Database | str | None = None,
             **kwargs: Any,
-        ) -> None:
-            ...
+        ) -> None: ...
 
-    Meta = MetaConfig
+    meta_config: ClassVar[MetaConfig] = MetaConfig()
+    model_config = ConfigDict(validate_assignment=True)
 
     @property
     def pk(self) -> Any:
         """主键值"""
         return getattr(self, self.__primary_key__)
 
     async def insert(self) -> Self:
@@ -196,28 +227,30 @@
     async def delete(self) -> bool:
         """删除文档"""
         result: DeleteResult = await self.__collection__.delete_one({"_id": self.pk})
         return bool(result.deleted_count)
 
     def doc(self, **kwargs: Any) -> dict[str, Any]:
         """转换为 MongoDB 文档"""
-        kwargs["by_alias"] = self.__meta__.by_alias
-        data = self.dict(**kwargs)
+        if by_alias := self.meta_config.get("by_alias"):
+            kwargs.setdefault("by_alias", by_alias)
+        data = self.model_dump(**kwargs)
         pk = self.__primary_key__
         exclude = kwargs.get("exclude")
         if not (exclude and pk in exclude):
             data["_id"] = data.pop(pk)
         return bson.decode(bson.encode(data, codec_options=self.__encoder__))
 
     @classmethod
-    def from_doc(cls, document: dict[str, Any]) -> Self:
+    def from_doc(cls, document: Mapping[str, Any]) -> Self:
         """从文档构建模型实例"""
+        doc = dict(document)
         with contextlib.suppress(KeyError):
-            document[cls.__primary_key__] = document.pop("_id")
-        return cls(**document)
+            doc[cls.__primary_key__] = doc.pop("_id")
+        return cls(**doc)
 
     @classmethod
     async def save_all(cls, *documents: Self) -> None:
         """保存全部文档"""
         await cls.__collection__.insert_many(doc.doc() for doc in documents)
 
     @classmethod
@@ -255,14 +288,10 @@
             return model
         default = defaults.doc() if isinstance(defaults, Document) else defaults or {}
         data = flat_filter(result.filter)
         merge_map(data, default)
         model = cls.from_doc(data)
         return await model.save()
 
-    class Config:
-        validate_assignment = True
-
 
 class EmbeddedDocument(BaseModel, metaclass=MetaEmbeddedDocument):
-    class Config:
-        validate_assignment = True
+    model_config = ConfigDict(validate_assignment=True)
```

### Comparing `mango_odm-0.3.2/mango/result.py` & `mango_odm-0.4.0/mango/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class FindOptions(BaseModel):
     limit: int = 0
     skip: int = 0
     sort: list[SortType] = []
 
     def kwdict(self, *exclude: str) -> dict[str, Any]:
-        return self.dict(exclude=set(exclude), exclude_defaults=True)
+        return self.model_dump(exclude=set(exclude), exclude_defaults=True)
 
 
 class FindResult(Generic[T_Model]):
     def __init__(
         self,
         model: type[T_Model],
         *filter: FindMapping | Expression,
@@ -64,41 +64,41 @@
 
     @property
     def filter(self) -> dict[str, Any]:
         """查询过滤条件"""
         compiled: dict[str, Any] = {}
         for condition in self._filter:
             if isinstance(condition, Mapping):
-                condition = dict(condition)
+                condition = dict(condition)  # noqa: PLW2901
             elif isinstance(condition, Expression):
-                condition = condition.struct()
+                condition = condition.struct()  # noqa: PLW2901
             else:
                 raise TypeError("查询过滤条件不正确, 应为映射或表达式")
             compiled |= self._compile(condition)
         return compiled
 
     def _compile(
         self,
         source: Mapping[KeyField, Any] | Mapping[str, Any],
     ) -> dict[str, Any]:
         compiled: dict[str, Any] = {}
 
         for key, value in source.items():
-            key = str(key)
+            key = str(key)  # noqa: PLW2901
             if isinstance(value, Expression):
                 compiled[key] = value.struct()
             elif isinstance(value, Mapping):
                 compiled[key] = self._compile(value)
             elif is_sequence(value):
                 compiled[key] = []
                 for i in value:
                     if isinstance(i, Expression):
-                        i = i.struct()
+                        i = i.struct()  # noqa: PLW2901
                     if isinstance(i, Mapping):
-                        i = self._compile(i)
+                        i = self._compile(i)  # noqa: PLW2901
                     compiled[key].append(i)
             else:
                 compiled[key] = value
 
         return compiled
 
     def limit(self, limit: int = 0) -> "FindResult[T_Model]":
@@ -121,15 +121,17 @@
                 key, direction = order
             else:
                 key = order
 
             try:
                 key, direction = str(key), Order(direction)
             except ValueError as e:
-                raise TypeError("键应为字符串或字段, 排序方向应为 Order 枚举成员") from e
+                raise TypeError(
+                    "键应为字符串或字段, 排序方向应为 Order 枚举成员"
+                ) from e
             else:
                 self.options.sort.append((key, direction))
 
         return self
 
     def asc(self, *keys: Any) -> "FindResult[T_Model]":
         """升序排列"""
@@ -174,17 +176,17 @@
         await self.collection.update_many(self.filter, {"$set": values})
 
 
 class AggregateResult:
     def __init__(self, cursor: AsyncIOMotorLatentCommandCursor) -> None:
         self.cursor = cursor
 
-    def __await__(self) -> Generator[None, None, list[dict[str, Any]]]:
+    def __await__(self) -> Generator[None, None, list[Mapping[str, Any]]]:
         """
         `await` : 等待时，将返回聚合管道的结果文档列表
         """
         return (yield from self.cursor.to_list(length=None).__await__())
 
-    async def __aiter__(self) -> AsyncGenerator[dict[str, Any], None]:
+    async def __aiter__(self) -> AsyncGenerator[Mapping[str, Any], None]:
         """`async for`: 异步迭代聚合管道的结果文档"""
         async for document in self.cursor:  # type: ignore
             yield document
```

### Comparing `mango_odm-0.3.2/mango/source.py` & `mango_odm-0.4.0/mango/source.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     from mango.models import Document
 
 
 async def init_model(model: type["Document"], *, revise_index: bool = False) -> None:
     """初始化文档模型"""
-    meta = model.__meta__
-    db = Client.get_database(meta.database)
-    model.__collection__ = db[meta.name or to_snake_case(model.__name__)]
+    meta = model.meta_config
+    db = Client.get_database(meta.get("database"))
+    model.__collection__ = db[meta.get("name") or to_snake_case(model.__name__)]
     await init_index(model, revise_index=revise_index)
 
 
 async def init_index(model: type["Document"], *, revise_index: bool = False) -> None:
     """初始化文档索引"""
     required = ["_id_"]
     if indexes := list(get_indexes(model)):
```

### Comparing `mango_odm-0.3.2/mango/stage.py` & `mango_odm-0.4.0/mango/stage.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.2/mango/utils.py` & `mango_odm-0.4.0/mango/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import re
 from collections.abc import Callable, Generator, Iterable, Sequence
 from types import UnionType
 from typing import TYPE_CHECKING, Any
 
 import pydantic
-from pydantic.fields import ModelField
 
 from mango.fields import FieldInfo
 from mango.index import Index, IndexType
 
 if TYPE_CHECKING:  # pragma: no cover
+    from pydantic import BaseModel
+
     from mango.models import Document
 
 
 def to_snake_case(string: str) -> str:
     """将字符串转换为蛇形命名法"""
     tmp = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", string)
     return re.sub("([a-z0-9])([A-Z])", r"\1_\2", tmp).lower()
@@ -58,37 +59,34 @@
     return isinstance(iter_obj, Sequence) and not isinstance(iter_obj, bytes | str)
 
 
 def validate_fields(
     model: type["Document"], input_data: dict[str, Any]
 ) -> dict[str, Any]:
     """验证模型的指定字段"""
-    if miss := set(input_data) - set(model.__fields__):
+    if miss := set(input_data) - set(model.model_fields):
         raise ValueError(f"这些字段在 {model.__name__} 中不存在: {miss}")
 
     fields = {
-        k: (v.outer_type_, v.field_info)
-        for k, v in model.__fields__.items()
+        k: (v.annotation, v.get_default())
+        for k, v in model.model_fields.items()
         if k in input_data
     }
-    new_model = pydantic.create_model(model.__name__, **fields)
-    values, _, validation_error = pydantic.validate_model(new_model, input_data)
-
-    if validation_error:
-        raise validation_error
+    new_model: "BaseModel" = pydantic.create_model(model.__name__, **fields)  # type: ignore
+    new_model.model_validate(input_data)
 
-    return values
+    return input_data
 
 
 def add_fields(model: type["Document"], **field_definitions: Any) -> None:
     """动态添加字段
 
     来源见: https://github.com/pydantic/pydantic/issues/1937
     """
-    new_fields: dict[str, ModelField] = {}
+    new_fields: dict[str, FieldInfo] = {}
     new_annotations: dict[str, type | None] = {}
 
     for f_name, f_def in field_definitions.items():
         if isinstance(f_def, tuple):
             try:
                 f_annotation, f_value = f_def
             except ValueError as e:
@@ -96,44 +94,41 @@
                     "field definitions should either be a tuple of (<type>, <default>) "
                     "or just a default value, unfortunately this means tuples as "
                     "default values are not allowed"
                 ) from e
         else:
             f_annotation, f_value = None, f_def
 
+        if not isinstance(f_value, dict):
+            f_value = {"default": f_value}
+
         if f_annotation:
             new_annotations[f_name] = f_annotation
 
-        new_fields[f_name] = ModelField.infer(
-            name=f_name,
-            value=f_value,
-            annotation=f_annotation,
-            class_validators=None,
-            config=model.__config__,
-        )
+        new_fields[f_name] = FieldInfo(annotation=f_annotation, **f_value)
 
-    model.__fields__.update(new_fields)
+    model.model_fields.update(new_fields)
     model.__annotations__.update(new_annotations)
+    model.model_rebuild(force=True)
 
 
 def get_indexes(model: type["Document"]) -> Generator[Index, None, None]:
     """获取模型中定义的索引, 包括字段与元配置"""
-    for name, field in model.__fields__.items():
-        finfo = field.field_info
-        if isinstance(finfo, FieldInfo):
-            if index := finfo.index:
+    for name, field in model.model_fields.items():
+        if isinstance(field, FieldInfo):
+            if index := field.index:
                 if index is True:
                     yield Index(name)
                 elif isinstance(index, IndexType):
                     yield Index((name, index))
                 else:
                     yield index
-            elif (expire := finfo.expire) is not None:
+            elif (expire := field.expire) is not None:
                 yield Index(name, expireAfterSeconds=expire)
 
-    for index in model.__meta__.indexes:
+    for index in model.meta_config.get("indexes", []):
         if isinstance(index, str):
             yield Index(index)
         elif isinstance(index, Sequence):
             yield Index(*index)
         else:
             yield index
```

### Comparing `mango_odm-0.3.2/pyproject.toml` & `mango_odm-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mango-odm"
-version = "0.3.2"
+version = "0.4.0"
 description = "🥭 Async MongoDB ODM with type hints in Python"
 authors = [
     { name = "Akirami", email = "akiramiaya@outlook.com" },
 ]
 requires-python = ">=3.10,<4.0"
 readme = "README.md"
 keywords = [
@@ -33,100 +33,53 @@
     "Topic :: Software Development",
     "Topic :: Software Development :: Object Brokering",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 dependencies = [
-    "motor>=3.2.0",
-    "pydantic>=1.10.12,<2.0.0",
+    "motor>=3.3.2",
+    "pydantic>=2.6.1",
+    "motor-types>=1.0.0b4",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/A-kirami/mango"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black>=23.7.0",
-    "ruff>=0.0.280",
-    "pre-commit>=3.3.3",
+    "ruff>=0.3.4",
+    "pre-commit>=3.6.0",
 ]
 test = [
-    "pytest>=7.4.0",
+    "pytest>=7.4.4",
     "pytest-cov>=4.1.0",
-    "pytest-sugar>=0.9.7",
+    "pytest-sugar>=1.0.0",
     "allure-pytest>=2.13.2",
-    "pytest-asyncio>=0.21.1",
-    "hypothesis>=6.82.0",
-    "Faker>=19.2.0",
+    "pytest-asyncio>=0.23.4",
+    "hypothesis>=6.98.9",
+    "Faker>=23.2.1",
 ]
 
 [tool.pdm.scripts]
+lint = "ruff check"
+"lint:fix" = "ruff check --fix"
+format = "ruff format"
 post_install = "pre-commit install"
 
-[tool.black]
-target-version = [
-    "py310",
-]
-
-[tool.ruff]
-select = [
-    "F",
-    "E",
-    "W",
-    "UP",
-    "ANN",
-    "S",
-    "B",
-    "C4",
-    "ISC",
-    "INP",
-    "T20",
-    "PT",
-    "Q",
-    "RSE",
-    "RET",
-    "SIM",
-    "TID",
-    "TCH",
-    "ARG",
-    "PTH",
-    "ERA",
-    "PL",
-    "TRY",
-    "RUF",
-]
-ignore = [
-    "E402",
-    "E501",
-    "B008",
-    "B009",
-    "B010",
-    "ANN002",
-    "ANN003",
-    "ANN101",
-    "ANN102",
-    "ANN401",
-    "ERA001",
-    "PLC0414",
-    "PLR0913",
-    "PLW2901",
-    "TRY003",
-    "RUF001",
-    "RUF002",
-    "RUF003",
-]
-unfixable = [
-    "F401",
-    "F841",
-    "ERA001",
-]
+[tool.pyright]
+pythonVersion = "3.10"
+pythonPlatform = "All"
+typeCheckingMode = "basic"
+
+[tool.pyright.defineConstant]
+PYDANTIC_V2 = true
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 addopts = "--cov=mango --cov-report=html --cov-report=xml --junit-xml=results.xml --cov-report=term-missing --alluredir=allure_report --clean-alluredir"
 
 [build-system]
 requires = [
```

### Comparing `mango_odm-0.3.2/PKG-INFO` & `mango_odm-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-odm
-Version: 0.3.2
+Version: 0.4.0
 Summary: 🥭 Async MongoDB ODM with type hints in Python
 Keywords: mongo mongodb async asyncio odm types pydantic motor
 Author-Email: Akirami <akiramiaya@outlook.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -20,16 +20,17 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/A-kirami/mango
 Requires-Python: <4.0,>=3.10
-Requires-Dist: motor>=3.2.0
-Requires-Dist: pydantic<2.0.0,>=1.10.12
+Requires-Dist: motor>=3.3.2
+Requires-Dist: pydantic>=2.6.1
+Requires-Dist: motor-types>=1.0.0b4
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a name="readme-top"></a>
     <a href="https://github.com/A-kirami/mango">
         <img width="140px" src="https://raw.githubusercontent.com/A-kirami/mango/main/assets/mango-logo.svg" align="center" alt="Mango" />
     </a>
```

