# Comparing `tmp/target_mssql-0.1.2.tar.gz` & `tmp/target_mssql-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_mssql-0.1.2.tar", max compression
+gzip compressed data, was "target_mssql-0.2.1.tar", max compression
```

## Comparing `target_mssql-0.1.2.tar` & `target_mssql-0.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11357 2023-04-24 06:53:50.732862 target_mssql-0.1.2/LICENSE
--rw-r--r--   0        0        0      850 2023-04-24 06:53:50.732862 target_mssql-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/__init__.py
--rw-r--r--   0        0        0    14800 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/connector.py
--rw-r--r--   0        0        0    11284 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/sinks.py
--rw-r--r--   0        0        0     1507 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/target.py
--rw-r--r--   0        0        0       35 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/__init__.py
--rw-r--r--   0        0        0      667 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/array_data.singer
--rw-r--r--   0        0        0      426 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/camelcase.singer
--rw-r--r--   0        0        0     1861 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/camelcase_complex_schema.singer
--rw-r--r--   0        0        0      516 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/column_comments.singer
--rw-r--r--   0        0        0     1227 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/disappearing_columns.singer
--rw-r--r--   0        0        0      721 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/duplicate_records.singer
--rw-r--r--   0        0        0     4319 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/encoded_strings.singer
--rw-r--r--   0        0        0      445 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/insert_merge_part1.singer
--rw-r--r--   0        0        0      433 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/insert_merge_part2.singer
--rw-r--r--   0        0        0      103 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/invalid_schema.singer
--rw-r--r--   0        0        0      362 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/large_int.singer
--rw-r--r--   0        0        0      440 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/long_string.singer
--rw-r--r--   0        0        0      607 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/missing_value.singer
--rw-r--r--   0        0        0     2128 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/multiple_state_messages.singer
--rw-r--r--   0        0        0      449 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/no_primary_keys.singer
--rw-r--r--   0        0        0      610 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/no_primary_keys_append.singer
--rw-r--r--   0        0        0      392 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/null_key.singer
--rw-r--r--   0        0        0      640 2023-04-24 06:53:50.732862 target_mssql-0.1.2/target_mssql/tests/data_files/optional_attributes.singer
--rw-r--r--   0        0        0      378 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/record_before_schema.singer
--rw-r--r--   0        0        0      287 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/record_missing_key_property.singer
--rw-r--r--   0        0        0      313 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/record_missing_required_property.singer
--rw-r--r--   0        0        0      838 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/schema_no_properties.singer
--rw-r--r--   0        0        0     1814 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/schema_updates.singer
--rw-r--r--   0        0        0     1333 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/simple_continents.singer
--rw-r--r--   0        0        0     5549 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/simple_countries.singer
--rw-r--r--   0        0        0      427 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/simple_stream.singer
--rw-r--r--   0        0        0      559 2023-04-24 06:53:50.736870 target_mssql-0.1.2/target_mssql/tests/data_files/special_chars_in_attributes.singer
--rw-r--r--   0        0        0  1859439 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/data_files/tap_aapl.singer
--rw-r--r--   0        0        0    97655 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/data_files/tap_countries.singer
--rw-r--r--   0        0        0      480 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/data_files/target_schema.singer
--rw-r--r--   0        0        0     1991 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/data_files/user_location_data.singer
--rw-r--r--   0        0        0     2322 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/data_files/user_location_upsert_data.singer
--rw-r--r--   0        0        0       15 2023-04-24 06:53:50.740877 target_mssql-0.1.2/target_mssql/tests/samples/__init__.py
--rw-r--r--   0        0        0   763998 2023-04-24 06:53:50.744885 target_mssql-0.1.2/target_mssql/tests/samples/aapl/AAPL.json
--rw-r--r--   0        0        0       26 2023-04-24 06:53:50.744885 target_mssql-0.1.2/target_mssql/tests/samples/aapl/__init__.py
--rw-r--r--   0        0        0      129 2023-04-24 06:53:50.744885 target_mssql-0.1.2/target_mssql/tests/samples/aapl/__main__.py
--rw-r--r--   0        0        0      654 2023-04-24 06:53:50.744885 target_mssql-0.1.2/target_mssql/tests/samples/aapl/aapl.py
--rw-r--r--   0        0        0  1492450 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/samples/aapl/fundamentals.json
--rw-r--r--   0        0        0       28 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/__init__.py
--rw-r--r--   0        0        0     2215 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/countries_streams.py
--rw-r--r--   0        0        0      812 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/countries_tap.py
--rw-r--r--   0        0        0      146 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/schemas/continents.json
--rw-r--r--   0        0        0     7860 2023-04-24 06:53:50.748893 target_mssql-0.1.2/target_mssql/tests/test_core.py
--rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 target_mssql-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 06:18:22.823335 target_mssql-0.2.1/LICENSE
+-rw-r--r--   0        0        0      850 2023-04-27 06:18:22.823335 target_mssql-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-27 06:18:22.823335 target_mssql-0.2.1/target_mssql/__init__.py
+-rw-r--r--   0        0        0    14962 2023-04-27 06:18:22.823335 target_mssql-0.2.1/target_mssql/connector.py
+-rw-r--r--   0        0        0    11293 2023-04-27 06:18:22.823335 target_mssql-0.2.1/target_mssql/sinks.py
+-rw-r--r--   0        0        0     1726 2023-04-27 06:18:22.823335 target_mssql-0.2.1/target_mssql/target.py
+-rw-r--r--   0        0        0       35 2023-04-27 06:18:22.823335 target_mssql-0.2.1/target_mssql/tests/__init__.py
+-rw-r--r--   0        0        0      668 2023-04-27 06:18:22.823335 target_mssql-0.2.1/target_mssql/tests/data_files/array_data.singer
+-rw-r--r--   0        0        0      426 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/camelcase.singer
+-rw-r--r--   0        0        0     1862 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/camelcase_complex_schema.singer
+-rw-r--r--   0        0        0      516 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/column_comments.singer
+-rw-r--r--   0        0        0     1227 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/disappearing_columns.singer
+-rw-r--r--   0        0        0      722 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/duplicate_records.singer
+-rw-r--r--   0        0        0     4320 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/encoded_strings.singer
+-rw-r--r--   0        0        0      445 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/insert_merge_part1.singer
+-rw-r--r--   0        0        0      434 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/insert_merge_part2.singer
+-rw-r--r--   0        0        0      104 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/invalid_schema.singer
+-rw-r--r--   0        0        0      362 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/large_int.singer
+-rw-r--r--   0        0        0      440 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/long_string.singer
+-rw-r--r--   0        0        0      607 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/missing_value.singer
+-rw-r--r--   0        0        0     2129 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/multiple_state_messages.singer
+-rw-r--r--   0        0        0      450 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/no_primary_keys.singer
+-rw-r--r--   0        0        0      611 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/no_primary_keys_append.singer
+-rw-r--r--   0        0        0      392 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/null_key.singer
+-rw-r--r--   0        0        0      641 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/optional_attributes.singer
+-rw-r--r--   0        0        0      378 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/record_before_schema.singer
+-rw-r--r--   0        0        0      288 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/record_missing_key_property.singer
+-rw-r--r--   0        0        0      314 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/record_missing_required_property.singer
+-rw-r--r--   0        0        0      839 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/schema_no_properties.singer
+-rw-r--r--   0        0        0     1815 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/schema_updates.singer
+-rw-r--r--   0        0        0     1334 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/simple_continents.singer
+-rw-r--r--   0        0        0     5549 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/simple_countries.singer
+-rw-r--r--   0        0        0      427 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/simple_stream.singer
+-rw-r--r--   0        0        0      560 2023-04-27 06:18:22.827335 target_mssql-0.2.1/target_mssql/tests/data_files/special_chars_in_attributes.singer
+-rw-r--r--   0        0        0  1859439 2023-04-27 06:18:22.831335 target_mssql-0.2.1/target_mssql/tests/data_files/tap_aapl.singer
+-rw-r--r--   0        0        0    97655 2023-04-27 06:18:22.831335 target_mssql-0.2.1/target_mssql/tests/data_files/tap_countries.singer
+-rw-r--r--   0        0        0      481 2023-04-27 06:18:22.831335 target_mssql-0.2.1/target_mssql/tests/data_files/target_schema.singer
+-rw-r--r--   0        0        0     1992 2023-04-27 06:18:22.831335 target_mssql-0.2.1/target_mssql/tests/data_files/user_location_data.singer
+-rw-r--r--   0        0        0     2323 2023-04-27 06:18:22.831335 target_mssql-0.2.1/target_mssql/tests/data_files/user_location_upsert_data.singer
+-rw-r--r--   0        0        0       15 2023-04-27 06:18:22.831335 target_mssql-0.2.1/target_mssql/tests/samples/__init__.py
+-rw-r--r--   0        0        0   763999 2023-04-27 06:18:22.835336 target_mssql-0.2.1/target_mssql/tests/samples/aapl/AAPL.json
+-rw-r--r--   0        0        0       26 2023-04-27 06:18:22.835336 target_mssql-0.2.1/target_mssql/tests/samples/aapl/__init__.py
+-rw-r--r--   0        0        0      129 2023-04-27 06:18:22.835336 target_mssql-0.2.1/target_mssql/tests/samples/aapl/__main__.py
+-rw-r--r--   0        0        0      654 2023-04-27 06:18:22.835336 target_mssql-0.2.1/target_mssql/tests/samples/aapl/aapl.py
+-rw-r--r--   0        0        0  1492450 2023-04-27 06:18:22.839336 target_mssql-0.2.1/target_mssql/tests/samples/aapl/fundamentals.json
+-rw-r--r--   0        0        0       28 2023-04-27 06:18:22.839336 target_mssql-0.2.1/target_mssql/tests/samples/sample_tap_countries/__init__.py
+-rw-r--r--   0        0        0     2215 2023-04-27 06:18:22.839336 target_mssql-0.2.1/target_mssql/tests/samples/sample_tap_countries/countries_streams.py
+-rw-r--r--   0        0        0      812 2023-04-27 06:18:22.839336 target_mssql-0.2.1/target_mssql/tests/samples/sample_tap_countries/countries_tap.py
+-rw-r--r--   0        0        0      147 2023-04-27 06:18:22.839336 target_mssql-0.2.1/target_mssql/tests/samples/sample_tap_countries/schemas/continents.json
+-rw-r--r--   0        0        0     8179 2023-04-27 06:18:22.839336 target_mssql-0.2.1/target_mssql/tests/test_core.py
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 target_mssql-0.2.1/PKG-INFO
```

### Comparing `target_mssql-0.1.2/LICENSE` & `target_mssql-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/pyproject.toml` & `target_mssql-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-mssql"
-version = "0.1.2"
+version = "0.2.1"
 description = "`target-mssql` is a Singer target for mssql, built with the Meltano SDK for Singer Targets."
 authors = ["Henning Holgersen"]
 keywords = [
     "ELT",
     "mssql",
 ]
 license = "Apache 2.0"
```

### Comparing `target_mssql-0.1.2/target_mssql/connector.py` & `target_mssql-0.2.1/target_mssql/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,16 +353,20 @@
 
             return cast(
                 sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR(maxlength)
             )
 
         if self._jsonschema_type_check(jsonschema_type, ("integer",)):
             return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.BIGINT())
+
         if self._jsonschema_type_check(jsonschema_type, ("number",)):
-            return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.NUMERIC(22, 16))
+            if self.config.get("prefer_float_over_numeric", False):
+                return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.FLOAT())
+            return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.NUMERIC(38, 16))
+
         if self._jsonschema_type_check(jsonschema_type, ("boolean",)):
             return cast(sqlalchemy.types.TypeEngine, mssql.VARCHAR(1))
 
         if self._jsonschema_type_check(jsonschema_type, ("object",)):
             return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR())
 
         if self._jsonschema_type_check(jsonschema_type, ("array",)):
@@ -384,10 +388,10 @@
         droptable = f"DROP TABLE IF EXISTS {tmp_full_table_name}"
         self.connection.execute(droptable)
 
         ddl = f"""
             SELECT TOP 0 *
             into {tmp_full_table_name}
             FROM {full_table_name}
-        """
+        """  # nosec
 
         self.connection.execute(ddl)
```

### Comparing `target_mssql-0.1.2/target_mssql/sinks.py` & `target_mssql-0.2.1/target_mssql/sinks.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
             ON {join_condition}
             WHEN MATCHED THEN
                 UPDATE SET
                     { update_stmt }
             WHEN NOT MATCHED THEN
                 INSERT ({", ".join(schema["properties"].keys())})
                 VALUES ({", ".join([f"temp.{key}" for key in schema["properties"].keys()])});
-        """
+        """  # nosec
 
         with self.connection.begin():
             self.connection.execute(merge_sql)
 
     def parse_full_table_name(
         self, full_table_name: str
     ) -> tuple[str | None, str | None, str]:
```

### Comparing `target_mssql-0.1.2/target_mssql/target.py` & `target_mssql-0.2.1/target_mssql/target.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,20 @@
             "default_target_schema",
             th.StringType,
             description="Default target schema to write to",
         ),
         th.Property(
             "table_prefix", th.StringType, description="Prefix to add to table name"
         ),
+        th.Property(
+            "prefer_float_over_numeric",
+            th.BooleanType,
+            description="Use float data type for numbers (otherwise number type is used)",
+            default=False,
+        ),
     ).to_dict()
 
     default_sink_class = mssqlSink
 
 
 if __name__ == "__main__":
     Targetmssql.cli()
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/array_data.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/array_data.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 {"type": "SCHEMA", "stream": "test_carts", "key_properties": ["id"], "schema": {"required": ["id"], "type": "object", "properties": {"id": {"type": "integer"}, "fruits": {"type": "array","items": {"type": "string"}}}}}
 {"type": "RECORD", "stream": "test_carts", "record": {"id": 1, "fruits": [ "apple", "orange", "pear" ]}}
 {"type": "RECORD", "stream": "test_carts", "record": {"id": 2, "fruits": [ "banana", "apple" ]}}
 {"type": "RECORD", "stream": "test_carts", "record": {"id": 3, "fruits": [ "pear" ]}}
 {"type": "RECORD", "stream": "test_carts", "record": {"id": 4, "fruits": [ "orange", "banana", "apple", "pear" ]}}
-{"type": "STATE", "value": {"test_carts": 4}}
+{"type": "STATE", "value": {"test_carts": 4}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/camelcase_complex_schema.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/camelcase_complex_schema.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,2 +1,2 @@
 {"type": "SCHEMA", "stream": "ForecastingTypeToCategory", "schema": {"properties": {"Id": {"type": "string"}, "IsDeleted": {"type": ["null", "boolean"]}, "CreatedDate": {"anyOf": [{"type": "string", "format": "date-time"}, {"type": ["string", "null"]}]}, "CreatedById": {"type": ["null", "string"]}, "LastModifiedDate": {"anyOf": [{"type": "string", "format": "date-time"}, {"type": ["string", "null"]}]}, "LastModifiedById": {"type": ["null", "string"]}, "SystemModstamp": {"anyOf": [{"type": "string", "format": "date-time"}, {"type": ["string", "null"]}]}, "ForecastingTypeId": {"type": ["null", "string"]}, "ForecastingItemCategory": {"type": ["null", "string"]}, "DisplayPosition": {"type": ["null", "integer"]}, "IsAdjustable": {"type": ["null", "boolean"]}, "IsOwnerAdjustable": {"type": ["null", "boolean"]}}, "type": "object", "additionalProperties": false}, "key_properties": ["Id"]}
-{"type": "SCHEMA", "stream": "ForecastingTypeToCategory", "schema": {"properties": {"Id": {"type": "string"}, "IsDeleted": {"type": ["null", "boolean"]}, "CreatedDate": {"anyOf": [{"type": "string", "format": "date-time"}, {"type": ["string", "null"]}]}, "CreatedById": {"type": ["null", "string"]}, "LastModifiedDate": {"anyOf": [{"type": "string", "format": "date-time"}, {"type": ["string", "null"]}]}, "LastModifiedById": {"type": ["null", "string"]}, "SystemModstamp": {"anyOf": [{"type": "string", "format": "date-time"}, {"type": ["string", "null"]}]}, "ForecastingTypeId": {"type": ["null", "string"]}, "ForecastingItemCategory": {"type": ["null", "string"]}, "DisplayPosition": {"type": ["null", "integer"]}, "IsAdjustable": {"type": ["null", "boolean"]}, "IsOwnerAdjustable": {"type": ["null", "boolean"]}, "age": {"type": "integer"}, "NewCamelCasedAttribute": {"type": "string"}}, "type": "object", "additionalProperties": false}, "key_properties": ["Id"]}
+{"type": "SCHEMA", "stream": "ForecastingTypeToCategory", "schema": {"properties": {"Id": {"type": "string"}, "IsDeleted": {"type": ["null", "boolean"]}, "CreatedDate": {"anyOf": [{"type": "string", "format": "date-time"}, {"type": ["string", "null"]}]}, "CreatedById": {"type": ["null", "string"]}, "LastModifiedDate": {"anyOf": [{"type": "string", "format": "date-time"}, {"type": ["string", "null"]}]}, "LastModifiedById": {"type": ["null", "string"]}, "SystemModstamp": {"anyOf": [{"type": "string", "format": "date-time"}, {"type": ["string", "null"]}]}, "ForecastingTypeId": {"type": ["null", "string"]}, "ForecastingItemCategory": {"type": ["null", "string"]}, "DisplayPosition": {"type": ["null", "integer"]}, "IsAdjustable": {"type": ["null", "boolean"]}, "IsOwnerAdjustable": {"type": ["null", "boolean"]}, "age": {"type": "integer"}, "NewCamelCasedAttribute": {"type": "string"}}, "type": "object", "additionalProperties": false}, "key_properties": ["Id"]}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/column_comments.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/column_comments.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/disappearing_columns.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/disappearing_columns.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/duplicate_records.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/duplicate_records.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 {"type": "SCHEMA", "stream": "test_duplicate_records", "key_properties": ["id"], "schema": {"required": ["id", "metric"], "type": "object", "properties": {"id": {"type": "integer"}, "metric": {"type": "integer"}}}}
 {"type": "RECORD", "stream": "test_duplicate_records", "record": {"id": 1, "metric": 1}}
 {"type": "RECORD", "stream": "test_duplicate_records", "record": {"id": 2, "metric": 2}}
 {"type": "RECORD", "stream": "test_duplicate_records", "record": {"id": 1, "metric": 10}}
 {"type": "RECORD", "stream": "test_duplicate_records", "record": {"id": 2, "metric": 20}}
 {"type": "RECORD", "stream": "test_duplicate_records", "record": {"id": 1, "metric": 100}}
-{"type": "STATE", "value": {"test_duplicate_records": 2}}
+{"type": "STATE", "value": {"test_duplicate_records": 2}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/encoded_strings.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/encoded_strings.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 {"type": "SCHEMA", "stream": "test_strings_in_arrays", "key_properties": ["id"], "schema": {"required": ["id"], "type": "object", "properties": {"id": {"type": "integer"}, "strings": {"type": "array", "items": {"type": "string"}}}}}
 {"type": "RECORD", "stream": "test_strings_in_arrays", "record": {"id": 1, "strings": ["simple string", "απλή συμβολοσειρά", "简单的字串"]}}
 {"type": "RECORD", "stream": "test_strings_in_arrays", "record": {"id": 2, "strings": ["chaîne simple", "quoted \"string\""]}}
 {"type": "RECORD", "stream": "test_strings_in_arrays", "record": {"id": 3, "strings": ["various \" \\ \/ \n escape sequences"]}}
 {"type": "RECORD", "stream": "test_strings_in_arrays", "record": {"id": 4, "strings": ["\u006D", "\u0101", "\u0199"]}}
 {"type": "RECORD", "stream": "test_strings_in_arrays", "record": {"id": 5, "strings": ["aaa", "Double quoting: \\u0000 \\u0041 \\u0001"]}}
 {"type": "RECORD", "stream": "test_strings_in_arrays", "record": {"id": 6, "strings": ["bbb", "Control Characters in string: \u0000 \u0041 \u0001"]}}
-{"type": "STATE", "value": {"test_strings": 11, "test_strings_in_objects": 11, "test_strings_in_arrays": 6}}
+{"type": "STATE", "value": {"test_strings": 11, "test_strings_in_objects": 11, "test_strings_in_arrays": 6}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/missing_value.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/missing_value.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/multiple_state_messages.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/multiple_state_messages.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 {"type": "RECORD", "stream": "test_multiple_state_messages_a", "record": {"id": 5, "metric": 500}}
 {"type": "RECORD", "stream": "test_multiple_state_messages_b", "record": {"id": 3, "metric": 330}}
 {"type": "STATE", "value": {"test_multiple_state_messages_a": 5, "test_multiple_state_messages_b": 3}}
 {"type": "RECORD", "stream": "test_multiple_state_messages_b", "record": {"id": 4, "metric": 440}}
 {"type": "RECORD", "stream": "test_multiple_state_messages_b", "record": {"id": 5, "metric": 550}}
 {"type": "RECORD", "stream": "test_multiple_state_messages_b", "record": {"id": 6, "metric": 660}}
 {"type": "STATE", "value": {"test_multiple_state_messages_a": 5, "test_multiple_state_messages_b": 6}}
-{"type": "RECORD", "stream": "test_multiple_state_messages_a", "record": {"id": 6, "metric": 600}}
+{"type": "RECORD", "stream": "test_multiple_state_messages_a", "record": {"id": 6, "metric": 600}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/no_primary_keys_append.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/no_primary_keys_append.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 {"type": "SCHEMA", "stream": "test_no_pk", "key_properties": [], "schema": { "type": "object", "properties": {"id": {"type": "integer"}, "metric": {"type": "integer"}}}}
 {"type": "RECORD", "stream": "test_no_pk", "record": {"id": 1, "metric": 101}}
 {"type": "RECORD", "stream": "test_no_pk", "record": {"id": 2, "metric": 202}}
 {"type": "RECORD", "stream": "test_no_pk", "record": {"id": 3, "metric": 303}}
 {"type": "RECORD", "stream": "test_no_pk", "record": {"id": 4, "metric": 404}}
 {"type": "RECORD", "stream": "test_no_pk", "record": {"id": 5, "metric": 505}}
-{"type": "STATE", "value": {"test_no_pk": 5}}
+{"type": "STATE", "value": {"test_no_pk": 5}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/optional_attributes.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/optional_attributes.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 {"type": "SCHEMA", "stream": "test_optional_attributes", "key_properties": ["id"], "schema": {"required": ["id"], "type": "object", "properties": {"id": {"type": "integer"}, "optional": {"type": "string"}}}}
 {"type": "RECORD", "stream": "test_optional_attributes", "record": {"id": 1, "optional": "This is optional"}}
 {"type": "RECORD", "stream": "test_optional_attributes", "record": {"id": 2}}
 {"type": "RECORD", "stream": "test_optional_attributes", "record": {"id": 3, "optional": "Also optional"}}
 {"type": "RECORD", "stream": "test_optional_attributes", "record": {"id": 4}}
-{"type": "STATE", "value": {"test_optional_attributes": 4}}
+{"type": "STATE", "value": {"test_optional_attributes": 4}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/schema_no_properties.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/schema_no_properties.singer`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 {"type": "SCHEMA", "stream": "test_object_schema_with_properties", "key_properties": [], "schema": {"type": "object", "properties": { "object_store": {"type": "object", "properties": {"id": {"type": "integer"}, "metric": {"type": "integer"}}}}}}
 {"type": "RECORD", "stream": "test_object_schema_with_properties", "record": {"object_store": {"id": 1, "metric": 187}}}
 {"type": "RECORD", "stream": "test_object_schema_with_properties", "record": {"object_store": {"id": 2, "metric": 203}}}
 {"type": "SCHEMA", "stream": "test_object_schema_no_properties", "key_properties": [], "schema": {"type": "object"}}
 {"type": "RECORD", "stream": "test_object_schema_no_properties", "record": {"object_store": {"id": 1, "metric": 1}}}
-{"type": "RECORD", "stream": "test_object_schema_no_properties", "record": {"object_store": {"id": 2, "metric": 2}}}
+{"type": "RECORD", "stream": "test_object_schema_no_properties", "record": {"object_store": {"id": 2, "metric": 2}}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/schema_updates.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/schema_updates.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 {"type": "RECORD", "stream": "test_schema_updates", "record": {"id": 2, "a1": 102, "a2": "string2", "a3": true}}
 {"type": "SCHEMA", "stream": "test_schema_updates", "key_properties": ["id"], "schema": {"type": "object", "properties": {"id": {"type": "integer"}, "a1": {"type": "number"}, "a2": {"type": "string"}, "a3": {"type": "boolean"}, "a5": {"type": "string", "maxLength": 64}}}}
 {"type": "RECORD", "stream": "test_schema_updates", "record": {"id": 3, "a1": 103, "a2": "string3", "a3": false, "a5": "banana"}}
 {"type": "RECORD", "stream": "test_schema_updates", "record": {"id": 4, "a1": 104, "a2": "string4", "a3": true, "a5": "orange"}}
 {"type": "SCHEMA", "stream": "test_schema_updates", "key_properties": ["id"], "schema": {"type": "object", "properties": {"id": {"type": "integer"}, "a1": {"type": "number"}, "a2": {"type": "string"}, "a3": {"type": "boolean"}, "a5": {"type": "string", "maxLength": 164}, "a6": {"type": "integer"}}}}
 {"type": "RECORD", "stream": "test_schema_updates", "record": {"id": 5, "a1": 105, "a2": "string5", "a3": false, "a5": "apple", "a6": 985}}
 {"type": "RECORD", "stream": "test_schema_updates", "record": {"id": 6, "a1": 106, "a2": "string6", "a3": true, "a5": "banana", "a6": 341}}
-{"type": "STATE", "value": {"test_schema_updates": 6}}
+{"type": "STATE", "value": {"test_schema_updates": 6}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/simple_continents.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/simple_continents.singer`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 {"type": "STATE", "value": {"bookmarks": {"nocontinents": {"starting_replication_value": null}}}}
 {"type": "RECORD", "stream": "nocontinents", "record": {"code": "AN", "name": "Antarctica"}, "time_extracted": "2022-07-17T20:43:18.860817Z"}
 {"type": "RECORD", "stream": "nocontinents", "record": {"code": "AS", "name": "Asia"}, "time_extracted": "2022-07-17T20:43:18.860857Z"}
 {"type": "RECORD", "stream": "nocontinents", "record": {"code": "EU", "name": "Europe"}, "time_extracted": "2022-07-17T20:43:18.860890Z"}
 {"type": "RECORD", "stream": "nocontinents", "record": {"code": "NA", "name": "North America"}, "time_extracted": "2022-07-17T20:43:18.860922Z"}
 {"type": "RECORD", "stream": "nocontinents", "record": {"code": "OC", "name": "Oceania"}, "time_extracted": "2022-07-17T20:43:18.860952Z"}
 {"type": "RECORD", "stream": "nocontinents", "record": {"code": "SA", "name": "South America"}, "time_extracted": "2022-07-17T20:43:18.860983Z"}
-{"type": "STATE", "value": {"bookmarks": {"nocontinents": {}}}}
+{"type": "STATE", "value": {"bookmarks": {"nocontinents": {}}}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/simple_countries.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/simple_countries.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/special_chars_in_attributes.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/special_chars_in_attributes.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,2 +1,2 @@
 {"type": "SCHEMA", "stream": "test:SpecialChars!in?attributes", "schema": {"type": "object", "properties": {"_id": {"type": "string"}, "d": {"type": "object", "properties": {"env": {"type": "string"}, "agent__type": {"type": "string"}, "agent__os__version": {"type": "string"}}}}}, "key_properties": ["_id"]}
-{"type": "RECORD", "stream": "test:SpecialChars!in?attributes", "record": {"_id": "a2e98886", "d": {"env": "prod", "agent__type": "desktop", "agent__os__version": "10.13.1"}}, "version": 1541199424491, "time_extracted": "2018-11-02T22:57:04.841020Z"}
+{"type": "RECORD", "stream": "test:SpecialChars!in?attributes", "record": {"_id": "a2e98886", "d": {"env": "prod", "agent__type": "desktop", "agent__os__version": "10.13.1"}}, "version": 1541199424491, "time_extracted": "2018-11-02T22:57:04.841020Z"}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/tap_aapl.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/tap_aapl.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/tap_countries.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/tap_countries.singer`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/user_location_data.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/user_location_data.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 {"type": "RECORD", "stream": "test_locations", "record": {"id": 1, "name": "Philadelphia"}}
 {"type": "RECORD", "stream": "test_locations", "record": {"id": 2, "name": "NY"}}
 {"type": "RECORD", "stream": "test_locations", "record": {"id": 3, "name": "SF"}}
 {"type": "SCHEMA", "stream": "test_user_in_location", "key_properties": ["id"], "schema": {"required": ["id", "user_id", "location_id"], "type": "object", "properties": {"id": {"type": "integer"}, "user_id": {"type": "integer"}, "location_id": {"type": "integer"}, "info": {"type": "object", "properties": {"weather": {"type": "string"}, "mood": {"type": "string"}}}}}}
 {"type": "RECORD", "stream": "test_user_in_location", "record": {"id": 1, "user_id": 1, "location_id": 1, "info": {"weather": "rainy", "mood": "sad"}}}
 {"type": "RECORD", "stream": "test_user_in_location", "record": {"id": 2, "user_id": 1, "location_id": 2, "info": {"weather": "sunny", "mood": "satisfied"}}}
 {"type": "RECORD", "stream": "test_user_in_location", "record": {"id": 3, "user_id": 1, "location_id": 3, "info": {"weather": "sunny", "mood": "happy"}}}
-{"type": "STATE", "value": {"test_users": 5, "test_locations": 3, "test_user_in_location": 3}}
+{"type": "STATE", "value": {"test_users": 5, "test_locations": 3, "test_user_in_location": 3}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/data_files/user_location_upsert_data.singer` & `target_mssql-0.2.1/target_mssql/tests/data_files/user_location_upsert_data.singer`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 {"type": "RECORD", "stream": "test_locations", "record": {"id": 6, "name": "Colorado"}}
 {"type": "RECORD", "stream": "test_locations", "record": {"id": 8, "name": "Boston"}}
 {"type": "SCHEMA", "stream": "test_user_in_location", "key_properties": ["id"], "schema": {"required": ["id", "user_id", "location_id"], "type": "object", "properties": {"id": {"type": "integer"}, "user_id": {"type": "integer"}, "location_id": {"type": "integer"}, "info": {"type": "object", "properties": {"weather": {"type": "string"}, "mood": {"type": "string"}}}}}}
 {"type": "RECORD", "stream": "test_user_in_location", "record": {"id": 1, "user_id": 1, "location_id": 4, "info": {"weather": "rainy", "mood": "sad"}}}
 {"type": "RECORD", "stream": "test_user_in_location", "record": {"id": 2, "user_id": 2, "location_id": 3, "info": {"weather": "sunny", "mood": "satisfied"}}}
 {"type": "RECORD", "stream": "test_user_in_location", "record": {"id": 6, "user_id": 3, "location_id": 2, "info": {"weather": "sunny", "mood": "happy"}}}
 {"type": "RECORD", "stream": "test_user_in_location", "record": {"id": 14, "user_id": 4, "location_id": 1, "info": {"weather": "cloudy", "mood": "ok"}}}
-{"type": "STATE", "value": {"test_users": 13, "test_locations": 8, "test_user_in_location": 14}}
+{"type": "STATE", "value": {"test_users": 13, "test_locations": 8, "test_user_in_location": 14}}
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/samples/aapl/AAPL.json` & `target_mssql-0.2.1/target_mssql/tests/samples/aapl/AAPL.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -47743,8 +47743,8 @@
 000ba7e0: 3a6e 756c 6c2c 226e 6574 496e 636f 6d65  :null,"netIncome
 000ba7f0: 4672 6f6d 436f 6e74 696e 7569 6e67 4f70  FromContinuingOp
 000ba800: 7322 3a6e 756c 6c2c 226e 6574 496e 636f  s":null,"netInco
 000ba810: 6d65 4170 706c 6963 6162 6c65 546f 436f  meApplicableToCo
 000ba820: 6d6d 6f6e 5368 6172 6573 223a 6e75 6c6c  mmonShares":null
 000ba830: 2c22 7072 6566 6572 7265 6453 746f 636b  ,"preferredStock
 000ba840: 416e 644f 7468 6572 4164 6a75 7374 6d65  AndOtherAdjustme
-000ba850: 6e74 7322 3a6e 756c 6c7d 7d7d 7d7d       nts":null}}}}}
+000ba850: 6e74 7322 3a6e 756c 6c7d 7d7d 7d7d 0a    nts":null}}}}}.
```

### Comparing `target_mssql-0.1.2/target_mssql/tests/samples/aapl/aapl.py` & `target_mssql-0.2.1/target_mssql/tests/samples/aapl/aapl.py`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/target_mssql/tests/samples/aapl/fundamentals.json` & `target_mssql-0.2.1/target_mssql/tests/samples/aapl/fundamentals.json`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/countries_streams.py` & `target_mssql-0.2.1/target_mssql/tests/samples/sample_tap_countries/countries_streams.py`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/target_mssql/tests/samples/sample_tap_countries/countries_tap.py` & `target_mssql-0.2.1/target_mssql/tests/samples/sample_tap_countries/countries_tap.py`

 * *Files identical despite different names*

### Comparing `target_mssql-0.1.2/target_mssql/tests/test_core.py` & `target_mssql-0.2.1/target_mssql/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,25 @@
     with pytest.raises(Exception) as e_info:
         file_name = "schema_no_properties.singer"
         singer_file_to_target(file_name, mssql_target)
 
 
 # TODO test that data is correct
 def test_schema_updates(mssql_target):
+    base_config = {
+        "schema": "dbo",
+        "username": "sa",
+        "password": "P@55w0rd",
+        "host": "localhost",
+        "port": "1433",
+        "database": "master",
+        "table_prefix": "prfx_",
+        "prefer_float_over_numeric": True,
+    }
+    mssql_target = Targetmssql(config=base_config)
     file_name = "schema_updates.singer"
     singer_file_to_target(file_name, mssql_target)
 
 
 # TODO test that data is correct
 def test_multiple_state_messages(mssql_target):
     file_name = "multiple_state_messages.singer"
```

### Comparing `target_mssql-0.1.2/PKG-INFO` & `target_mssql-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-mssql
-Version: 0.1.2
+Version: 0.2.1
 Summary: `target-mssql` is a Singer target for mssql, built with the Meltano SDK for Singer Targets.
 License: Apache 2.0
 Keywords: ELT,mssql
 Author: Henning Holgersen
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

