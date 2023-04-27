# Comparing `tmp/fw_meta-3.2.0-py3-none-any.whl.zip` & `tmp/fw_meta-3.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13751 bytes, number of entries: 9
+Zip file size: 14167 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 fw_meta/__init__.py
 -rw-r--r--  2.0 unx      631 b- defN 80-Jan-01 00:00 fw_meta/aliases.py
 -rw-r--r--  2.0 unx     7728 b- defN 80-Jan-01 00:00 fw_meta/exports.py
--rw-r--r--  2.0 unx    18540 b- defN 80-Jan-01 00:00 fw_meta/imports.py
+-rw-r--r--  2.0 unx    20152 b- defN 80-Jan-01 00:00 fw_meta/imports.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_meta/py.typed
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_meta-3.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    10028 b- defN 80-Jan-01 00:00 fw_meta-3.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_meta-3.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      665 b- defN 16-Jan-01 00:00 fw_meta-3.2.0.dist-info/RECORD
-9 files, 39144 bytes uncompressed, 12623 bytes compressed:  67.8%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_meta-3.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10028 b- defN 80-Jan-01 00:00 fw_meta-3.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_meta-3.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      665 b- defN 16-Jan-01 00:00 fw_meta-3.3.0.dist-info/RECORD
+9 files, 40756 bytes uncompressed, 13039 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: fw_meta/imports.py
 Comment: 
 
 Filename: fw_meta/py.typed
 Comment: 
 
-Filename: fw_meta-3.2.0.dist-info/LICENSE
+Filename: fw_meta-3.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: fw_meta-3.2.0.dist-info/METADATA
+Filename: fw_meta-3.3.0.dist-info/METADATA
 Comment: 
 
-Filename: fw_meta-3.2.0.dist-info/WHEEL
+Filename: fw_meta-3.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: fw_meta-3.2.0.dist-info/RECORD
+Filename: fw_meta-3.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_meta/imports.py

```diff
@@ -343,14 +343,15 @@
 
 
 def validate_import_template_field(field: str) -> str:
     """Return canonic import field name if !prefixed, otherwise value as-is."""
     if field.startswith("!"):
         field, _ = validate_import_field(field[1:])
         return f"!{field}"
+    # TODO validate that only path/dir/name[/ext? /type?] is used if not parsed
     return field
 
 
 class ImportTemplate(Template):
     """Import template for formatting data or !metadata fields."""
 
     def __init__(self, template: str) -> None:
@@ -445,14 +446,25 @@
     exclude: t.Optional[t.List[str]] = Field(
         title=(
             "Exclude filters - if given, "
             "exclude files matching any of the exclude filters"
         ),
         example=["path=~meta.json"],
     )
+    type: t.Optional[str] = Field(
+        title=(
+            "Data type to import matching files as - if given, "
+            "allows extracting additional metadata for known types"
+        ),
+        example="dicom",
+    )
+    group_by: t.Optional[str] = Field(
+        title="Group and process files together based on shared property", example="dir"
+    )
+    zip: t.Optional[bool] = Field(title="Import multiple grouped files zipped together")
     mappings: Mappings = Field(
         title="Metadata mapping patterns",
         example=[
             ("path", "{sub}/{ses}/{acq}/{file}"),
             ("path", "{file.info.original_path}"),
         ],
     )
@@ -466,70 +478,94 @@
     )
 
     @property
     def meta_fields(self) -> t.Set[str]:
         """Return metadata fields that are present in the rule."""
         return self.extractor.fields
 
-    @root_validator(skip_on_failure=True)
+    @root_validator(pre=True, skip_on_failure=True)
     @classmethod
     def validate_rule(cls, values: dict) -> dict:
         """Validate the filters and the mappings given the level constraint."""
         level = ImportLevel(values.setdefault("level", "acquisition"))
         # sanity check that level is acquisition for know
         assert level == ImportLevel.acquisition, f"Unsupported import level {level}"
         # validate filters
         filt = ImportFilter(
             include=values.get("include"),
             exclude=values.get("exclude"),
         )
         values["include"] = [str(i) for i in filt.include]
         values["exclude"] = [str(e) for e in filt.exclude]
+        # validate type/group_by/zip
+        if values.get("type") == "dicom":
+            values.setdefault("group_by", "dir")
+            values.setdefault("zip", True)
+        if group_by := values.get("group_by"):
+            ImportTemplate(group_by)
+        if values.get("zip"):
+            assert group_by, "Zipping is only allowed when using group_by"
         # validate patterns
         extractor = MetaExtractor(
             mappings=values.get("mappings"),
             defaults=values.get("defaults"),
             overrides=values.get("overrides"),
         )
         values["mappings"] = [(str(t), str(p)) for t, p in extractor.mappings]
         values["defaults"] = extractor.defaults
         values["overrides"] = extractor.overrides
         assert values["mappings"], "At least one pattern is required"
         return values
 
     _filter: ImportFilter = PrivateAttr(None)
+    _group_tpl: ImportTemplate = PrivateAttr(None)
     _extractor: MetaExtractor = PrivateAttr(None)
 
     @property
     def filter(self) -> ImportFilter:
         """Return initialized import filter instance."""
         if not self._filter:
             self._filter = ImportFilter(include=self.include, exclude=self.exclude)
         return self._filter
 
     @property
+    def group_tpl(self) -> t.Optional[ImportTemplate]:
+        """Return initialized group_by template instance."""
+        if not self._group_tpl and self.group_by:
+            self._group_tpl = ImportTemplate(self.group_by)
+        return self._group_tpl
+
+    @property
     def extractor(self) -> MetaExtractor:
         """Return initialized meta extractor instance."""
         if not self._extractor:
             self._extractor = MetaExtractor(
                 mappings=self.mappings,
                 defaults=self.defaults,
                 overrides=self.overrides,
             )
         return self._extractor
 
     def match(self, value) -> bool:
-        """Return True if the values passes the include/exclude filters."""
+        """Return True if the value passes the include/exclude filters."""
         return self.filter.match(value)
 
+    def group(self, value) -> t.Optional[str]:
+        """Return the value's group based on the group_by template."""
+        return self.group_tpl.format(value) if self.group_tpl else None
+
     def extract(self, value: dict) -> t.Optional[MetaData]:
-        """Extract metadata."""
+        """Return extracted metadata if the value matches the filters."""
         if not self.match(value):
             return None  # pragma: no cover
-        return self.extractor.extract(value)
+        meta = self.extractor.extract(value)
+        if self.type:
+            meta.setdefault("file.type", self.type)
+        # TODO consider suffixing [.type].zip to file.name here
+        return meta
 
 
 # HELPERS
 
 
 def parse_metadata_mappings(mappings: Mappings) -> t.Iterable[t.Tuple[str, str]]:
     """Parse and yield metadata mappings as a tuple."""
```

## Comparing `fw_meta-3.2.0.dist-info/LICENSE` & `fw_meta-3.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_meta-3.2.0.dist-info/METADATA` & `fw_meta-3.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-meta
-Version: 3.2.0
+Version: 3.3.0
 Summary: Flywheel metadata extraction.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-meta
 License: MIT
 Keywords: Flywheel,DICOM,metadata,extract
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

## Comparing `fw_meta-3.2.0.dist-info/RECORD` & `fw_meta-3.3.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 fw_meta/__init__.py,sha256=WrDqzdSjEJ5mc0JE3p4Cqbkhi8LI33lWdzB5PBsII18,386
 fw_meta/aliases.py,sha256=rBa60kdqLAAi0WJ9e1nmOPdiqm--bm3OtGXRbe-Aboc,631
 fw_meta/exports.py,sha256=GoVR3XIt7_K481ntlx3PVKtxGm1ycCPCb4QzkI6FQwk,7728
-fw_meta/imports.py,sha256=nv0dISDxoRF4mTe8I-y1DnF3xWcm3FFhFGGGPg04Uqk,18540
+fw_meta/imports.py,sha256=3XoK8qahPBinqwZOBNpIsw6wnOfE-NGrZvNlSJH4wgM,20152
 fw_meta/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fw_meta-3.2.0.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
-fw_meta-3.2.0.dist-info/METADATA,sha256=LFjhztspIqEaPb22Hq6SQLRs86V9oY12lIbREGvBhbw,10028
-fw_meta-3.2.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fw_meta-3.2.0.dist-info/RECORD,,
+fw_meta-3.3.0.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
+fw_meta-3.3.0.dist-info/METADATA,sha256=wa9kZhy2Tlfatj6yLBB3aOfKgdpfRiaonYKfc8wUyWE,10028
+fw_meta-3.3.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fw_meta-3.3.0.dist-info/RECORD,,
```

