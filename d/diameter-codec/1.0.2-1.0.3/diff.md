# Comparing `tmp/diameter-codec-1.0.2.tar.gz` & `tmp/diameter-codec-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diameter-codec-1.0.2.tar", last modified: Wed Jan 11 06:59:19 2023, max compression
+gzip compressed data, was "diameter-codec-1.0.3.tar", last modified: Thu Apr 27 08:19:49 2023, max compression
```

## Comparing `diameter-codec-1.0.2.tar` & `diameter-codec-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 kpopovic  (1000) kpopovic  (1000)        0 2023-01-11 06:59:19.348708 diameter-codec-1.0.2/
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     3166 2023-01-11 06:59:19.348708 diameter-codec-1.0.2/PKG-INFO
-drwxrwxr-x   0 kpopovic  (1000) kpopovic  (1000)        0 2023-01-11 06:59:19.344708 diameter-codec-1.0.2/codec/
-drwxrwxr-x   0 kpopovic  (1000) kpopovic  (1000)        0 2023-01-11 06:59:19.344708 diameter-codec-1.0.2/codec/diameter/
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)        0 2022-11-02 15:50:26.000000 diameter-codec-1.0.2/codec/diameter/__init__.py
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     7807 2023-01-07 00:37:10.000000 diameter-codec-1.0.2/codec/diameter/_avp_decoder.py
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     9754 2023-01-09 09:33:13.000000 diameter-codec-1.0.2/codec/diameter/_avp_encoder.py
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     5106 2023-01-10 15:31:04.000000 diameter-codec-1.0.2/codec/diameter/_diam_tools.py
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     6510 2023-01-10 15:31:04.000000 diameter-codec-1.0.2/codec/diameter/diameter.py
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     7941 2023-01-10 15:01:34.000000 diameter-codec-1.0.2/codec/diameter/dictionary.py
-drwxrwxr-x   0 kpopovic  (1000) kpopovic  (1000)        0 2023-01-11 06:59:19.348708 diameter-codec-1.0.2/diameter_codec.egg-info/
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     3166 2023-01-11 06:59:19.000000 diameter-codec-1.0.2/diameter_codec.egg-info/PKG-INFO
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)      415 2023-01-11 06:59:19.000000 diameter-codec-1.0.2/diameter_codec.egg-info/SOURCES.txt
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)        1 2023-01-11 06:59:19.000000 diameter-codec-1.0.2/diameter_codec.egg-info/dependency_links.txt
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)        1 2023-01-11 06:59:19.000000 diameter-codec-1.0.2/diameter_codec.egg-info/namespace_packages.txt
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)        6 2023-01-11 06:59:19.000000 diameter-codec-1.0.2/diameter_codec.egg-info/top_level.txt
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)        1 2023-01-11 06:59:19.000000 diameter-codec-1.0.2/diameter_codec.egg-info/zip-safe
--rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)       38 2023-01-11 06:59:19.348708 diameter-codec-1.0.2/setup.cfg
--rwxr-xr-x   0 kpopovic  (1000) kpopovic  (1000)     4264 2023-01-11 06:59:18.000000 diameter-codec-1.0.2/setup.py
+drwxrwxr-x   0 kpopovic  (1000) kpopovic  (1000)        0 2023-04-27 08:19:49.444176 diameter-codec-1.0.3/
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     3166 2023-04-27 08:19:49.444176 diameter-codec-1.0.3/PKG-INFO
+drwxrwxr-x   0 kpopovic  (1000) kpopovic  (1000)        0 2023-04-27 08:19:49.444176 diameter-codec-1.0.3/codec/
+drwxrwxr-x   0 kpopovic  (1000) kpopovic  (1000)        0 2023-04-27 08:19:49.444176 diameter-codec-1.0.3/codec/diameter/
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)        0 2022-11-02 15:50:26.000000 diameter-codec-1.0.3/codec/diameter/__init__.py
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     7688 2023-04-27 08:07:07.000000 diameter-codec-1.0.3/codec/diameter/_avp_decoder.py
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)    10222 2023-04-27 08:07:07.000000 diameter-codec-1.0.3/codec/diameter/_avp_encoder.py
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     5106 2023-01-10 15:31:04.000000 diameter-codec-1.0.3/codec/diameter/_diam_tools.py
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     6510 2023-01-10 15:31:04.000000 diameter-codec-1.0.3/codec/diameter/diameter.py
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     9161 2023-04-27 08:07:07.000000 diameter-codec-1.0.3/codec/diameter/dictionary.py
+drwxrwxr-x   0 kpopovic  (1000) kpopovic  (1000)        0 2023-04-27 08:19:49.444176 diameter-codec-1.0.3/diameter_codec.egg-info/
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)     3166 2023-04-27 08:19:49.000000 diameter-codec-1.0.3/diameter_codec.egg-info/PKG-INFO
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)      415 2023-04-27 08:19:49.000000 diameter-codec-1.0.3/diameter_codec.egg-info/SOURCES.txt
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)        1 2023-04-27 08:19:49.000000 diameter-codec-1.0.3/diameter_codec.egg-info/dependency_links.txt
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)        1 2023-04-27 08:19:49.000000 diameter-codec-1.0.3/diameter_codec.egg-info/namespace_packages.txt
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)        6 2023-04-27 08:19:49.000000 diameter-codec-1.0.3/diameter_codec.egg-info/top_level.txt
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)        1 2023-04-27 08:19:49.000000 diameter-codec-1.0.3/diameter_codec.egg-info/zip-safe
+-rw-rw-r--   0 kpopovic  (1000) kpopovic  (1000)       38 2023-04-27 08:19:49.444176 diameter-codec-1.0.3/setup.cfg
+-rwxr-xr-x   0 kpopovic  (1000) kpopovic  (1000)     4264 2023-04-27 08:19:48.000000 diameter-codec-1.0.3/setup.py
```

### Comparing `diameter-codec-1.0.2/PKG-INFO` & `diameter-codec-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diameter-codec
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://gitlab.com/3gpp-toolbox/diameter-codec
 Author: Kresimir Popovic
 Author-email: kresimir.popovic@gmail.com
 Maintainer: 
 Maintainer-email: 
 License: European Union Public Licence 1.2 (EUPL 1.2)
 Keywords: diameter codec rfc6733
```

### Comparing `diameter-codec-1.0.2/codec/diameter/_avp_decoder.py` & `diameter-codec-1.0.3/codec/diameter/_avp_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,35 +120,41 @@
         :param application_id: application id
         :return: Avp object
         """
         code: int = int.from_bytes(avp_header[:4], "big")
         flags: int = int.from_bytes(avp_header[4:5], "big")
         length: int = int.from_bytes(avp_header[5:8], "big")
         data: bytes = b''
-        decode_data: any = None
+        decode_data: any
         #   ----------------------------------------------------
 
         if flags >= 128:
             vendor_id: int = int.from_bytes(avp_header[8:12], "big")
             if vendor_id > 0:
                 data = avp_header[12: length]
         else:
             data = avp_header[8: length]
 
         avp_dict: AvpDict = self.dictionary_layout.find_avp_by_code(application_id, code)
         if avp_dict is None:
             logging.warning(f"DECODER: application_id={application_id}, avp code={code} in diameter dictionary not "
                             f"found!")
-            return None
+            return Avp(f"{application_id}-{code}", data.hex())
 
         if len(data) == 0:
             logging.warning(f"DECODER: application_id={application_id}, {avp_dict.name}(code={code}) has no data!")
             return Avp(avp_dict.name, None)
 
-        if avp_dict.type.lower() == "unsigned32":
+        if avp_dict.has_enums():
+            value = struct.unpack(">I", data)
+            decode_data = avp_dict.find_enum_text_by_value(int(value[0]))
+            if not decode_data:
+                logging.warning(f"DECODER: application_id={application_id}, {avp_dict.name}(code={code}) has unknown "
+                                f"enumerated value='{value}'")
+        elif avp_dict.type.lower() == "unsigned32":
             decode_data = struct.unpack(">I", data)[0]
         elif avp_dict.type.lower() == "unsigned64":
             decode_data = struct.unpack(">Q", data)[0]
         elif avp_dict.type.lower() == "integer32":
             decode_data = struct.unpack(">i", data)[0]
         elif avp_dict.type.lower() == "integer64":
             decode_data = struct.unpack(">q", data)[0]
@@ -170,21 +176,11 @@
             secs_between_1900_and_1970: int = (70 * 365 + 17) * 86400
             timestamp = struct.unpack(">I", data)[0]
             decode_data = timestamp - secs_between_1900_and_1970
         elif avp_dict.type.lower() == "diameteruri":
             decode_data = urlparse(data.decode("utf-8")).geturl()
         elif avp_dict.type.lower() == "ipfilterrule":
             decode_data = data.decode("utf-8")
-        elif avp_dict.type.lower() == "enumerated":
-            value = struct.unpack(">i", data)
-            for enum_value, enum_text in avp_dict.enums.items():
-                if int(enum_value) == int(value[0]):  # e.g value=(6, )
-                    decode_data = enum_text
-                    break
-
-            if not decode_data:
-                logging.warning(f"DECODER: application_id={application_id}, {avp_dict.name}(code={code}) has unknown "
-                                f"enumerated value='{value}'")
         else:
             decode_data = data.decode("utf-8")
 
         return Avp(avp_dict.name, decode_data)
```

### Comparing `diameter-codec-1.0.2/codec/diameter/_avp_encoder.py` & `diameter-codec-1.0.3/codec/diameter/_avp_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         if isinstance(data, (IPv4Address, IPv6Address)):
             encoded_data = data.packed
         elif isinstance(data, (str, bytes)) and _DiamTools.is_ip_v4_address(data):
             encoded_data = IPv4Address(data).packed
         elif isinstance(data, (str, bytes)) and _DiamTools.is_ip_v6_address(data):
             encoded_data = IPv6Address(data).packed
-        elif avp_dict.content_type.lower() == "binary" and isinstance(data, str):   # hex-string expected
+        elif avp_dict.content_type.lower() == "binary" and isinstance(data, str):  # hex-string expected
             encoded_data = bytes.fromhex(data.replace("0x", "", 1))
         elif isinstance(data, str):
             struct_format = f"!{len(data)}s"
             encoded_data = struct.pack(struct_format, data.encode("utf-8"))
         elif isinstance(data, int):
             encoded_data = bytes.fromhex(hex(data).replace("0x", "", 1))
         elif isinstance(data, bytes):
@@ -128,15 +128,32 @@
         bytes_1_flags: bytes
         bytes_4_vendor_id: bytes
         bytes_3_length: bytes
         bytes_data: bytes = b''
         avp_buffer: bytes = b''
         avp_length: int
 
-        if avp_dict.type.lower() == "unsigned32" and isinstance(avp.data, int):
+        if avp_dict.has_enums() and isinstance(avp.data, (str, int)):
+            if isinstance(avp.data, str):
+                enum_value = avp_dict.find_enum_value_by_text(avp.data.strip(), -1)
+                if enum_value > -1:
+                    bytes_data = struct.pack(">I", enum_value)
+                else:
+                    raise ValueError(
+                        f"ENCODER: application_id={application_id}, {avp_dict.name}(code={avp_dict.code}) has unknown "
+                        f"enumerated text={avp.data}")
+            elif isinstance(avp.data, int):
+                enum_text = avp_dict.find_enum_text_by_value(avp.data, "")
+                if len(enum_text) != 0:
+                    bytes_data = struct.pack(">I", avp.data)
+                else:
+                    raise ValueError(
+                        f"ENCODER: application_id={application_id}, {avp_dict.name}(code={avp_dict.code}) has unknown "
+                        f"enumerated value={avp.data}")
+        elif avp_dict.type.lower() == "unsigned32" and isinstance(avp.data, int):
             bytes_data = struct.pack(">I", int(avp.data))
         elif avp_dict.type.lower() == "unsigned64" and isinstance(avp.data, int):
             bytes_data = struct.pack(">Q", avp.data)
         elif avp_dict.type.lower() == "integer32" and isinstance(avp.data, int):
             bytes_data = struct.pack(">i", avp.data)
         elif avp_dict.type.lower() == "integer64" and isinstance(avp.data, int):
             bytes_data = struct.pack(">q", avp.data)
@@ -160,28 +177,17 @@
             bytes_data = struct.pack(">I", timestamp)
         elif avp_dict.type.lower() == "diameteruri" and isinstance(avp.data, ParseResult):
             bytes_data = avp.data.geturl().encode("utf-8")
         elif avp_dict.type.lower() == "diameteruri" and isinstance(avp.data, str):
             bytes_data = urlparse(str(avp.data)).geturl().encode("utf-8")
         elif avp_dict.type.lower() == "ipfilterrule" and isinstance(avp.data, str):
             bytes_data = str(avp.data).encode("utf-8")
-        elif avp_dict.type.lower() == "enumerated" and isinstance(avp.data, str):
-            for enum_value, enum_text in avp_dict.enums.items():
-                if enum_text.strip() == avp.data.strip():
-                    bytes_data = struct.pack(">i", enum_value)
-                    break
-
-            if not bytes_data:
-                logging.warning(f"ENCODER: application_id={application_id}, {avp_dict.name}(code={avp_dict.code}) has "
-                                f"unknown enumerated text={avp.data}")
-
         elif avp.data:  # unknown type, do best effort to encode
             logging.warning(f"ENCODER: application_id={application_id}, {avp_dict.name}(code={avp_dict.code}) has "
                             f"unknown data type={avp_dict.type}")
-
             bytes_data = str(avp.data).encode("utf-8")
         else:
             logging.warning(f"ENCODER: application_id={application_id}, {avp_dict.name}(code={avp_dict.code}) has no "
                             f"data!")
 
         has_vendor_id: bool = avp_dict.vendor_id > 0
         bytes_1_flags = _DiamTools.modify_flags_bit(bytes([0]), 7, has_vendor_id)
```

### Comparing `diameter-codec-1.0.2/codec/diameter/_diam_tools.py` & `diameter-codec-1.0.3/codec/diameter/_diam_tools.py`

 * *Files identical despite different names*

### Comparing `diameter-codec-1.0.2/codec/diameter/diameter.py` & `diameter-codec-1.0.3/codec/diameter/diameter.py`

 * *Files identical despite different names*

### Comparing `diameter-codec-1.0.2/codec/diameter/dictionary.py` & `diameter-codec-1.0.3/codec/diameter/dictionary.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,48 @@
     type: str
     content_type: str
     vendor_id: int
     vendor_flag: bool
     mandatory_flag: bool
     enums: dict
 
+    def has_enums(self) -> bool:
+        """
+        Checks is enum dict contains enumerated items
+        @return:
+        """
+        return self.enums is not None \
+            and (self.type.lower() == "enumerated" or self.content_type.lower() == "enumerated")
+
+    def find_enum_text_by_value(self, value: int, def_val: str = None) -> Optional[str]:
+        """
+        Functions gets from dictionary enum text based on enum value.
+        @param value: enum value
+        @param def_val: to return if value is not found
+        @return: enum text or None
+        """
+        if not self.has_enums():
+            return def_val
+        return self.enums.get(value, def_val)
+
+    def find_enum_value_by_text(self, text: str, def_text: int = None) -> Optional[int]:
+        """
+        Functions gets from dictionary enum value based on enum text.
+        @param text: enum text
+        @param def_text: to return if text is not found
+        @return: enum value or None
+        """
+        if not self.has_enums():
+            return def_text
+        for enum_value, enum_text in self.enums.items():
+            if enum_text.strip() == text.strip():
+                return int(enum_value)
+
+        return def_text
+
 
 class DictionaryLayout(ABC):
     """ ABC DictionaryLayout """
     __dictionary: ElementTree
 
     @abstractmethod
     def __init__(self, path: str):
@@ -62,14 +96,15 @@
         :param application_id: application id
         :param avp_code: avp code
         """
 
 
 class DefaultDictionaryLayout(DictionaryLayout):
     """ DefaultDictionaryLayout """
+
     def __init__(self, path: str):
         """
         Constructor.
         :param path: path to file
         """
         super().__init__(path)
         self._ns = {'xmlns': self.__find_namespace(super().get_dictionary())}
```

### Comparing `diameter-codec-1.0.2/diameter_codec.egg-info/PKG-INFO` & `diameter-codec-1.0.3/diameter_codec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diameter-codec
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://gitlab.com/3gpp-toolbox/diameter-codec
 Author: Kresimir Popovic
 Author-email: kresimir.popovic@gmail.com
 Maintainer: 
 Maintainer-email: 
 License: European Union Public Licence 1.2 (EUPL 1.2)
 Keywords: diameter codec rfc6733
```

### Comparing `diameter-codec-1.0.2/setup.py` & `diameter-codec-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'diameter-codec',
-        version = '1.0.2',
+        version = '1.0.3',
         description = '',
         long_description = '# Diameter codec - encoder & decoder  \n- codec is based on RFC https://datatracker.ietf.org/doc/html/rfc6733  \n- no third party py libs dependencies  \n- very simple and straightforward to use  \n- python support: >= 3.6  \n  \n### How to setup dev env  \n- apt install python3.6   \n- apt install python3.6-venv  \n- source venv/bin/activate  \n- pip install -r requirements.txt\n- pylint src/main/python/codec/diameter/ --ignored-classes=_socketobject *.py\n  \n### How to build project  \n- pyb -v\n- pyb -Q\n\n### How to upload project to test.pypi with twine\n-   python -m twine upload --repository-url https://test.pypi.org/legacy/ target/dist/diameter-codec-<x.y.z>/dist/*\n\n### How to upload project to pypi with twine (production)\n-   python -m twine upload target/dist/diameter-codec-<x.y.z>/dist/*\n\n### How to push git tag\n- git push origin v<x.y.z>\n\n### How to encode and decode Capabilities-Exchange message\n\timport os  \n\timport typing    \n\tfrom codec.diameter.diameter import DiameterHeader, Diameter, Avp  \n\tfrom codec.diameter.dictionary import DictionaryLayout, DefaultDictionaryLayout\t\n\tcer_request: typing.Tuple = (  \n      Avp("Product-Name", "hello"),  \n      Avp("Origin-Realm", "zte.com.cn"),  \n      Avp("Origin-Host", "dmtsrv001.zte.com.cn"),  \n      Avp("Host-IP-Address", "192.168.0.1"),  \n      Avp("Vendor-Id", 10415),  \n      Avp("Product-Name", "dummy-product"),  \n      Avp("Inband-Security-Id", 1),  \n      Avp("Vendor-Specific-Application-Id", (  \n         Avp("Vendor-Id", 10415),  \n         Avp("Acct-Application-Id", 1),  \n         Avp("Auth-Application-Id", 1),  \n      )),  \n      Avp("Vendor-Specific-Application-Id", (  \n         Avp("Auth-Application-Id", 2),  \n         Avp("Acct-Application-Id", 2),  \n         Avp("Vendor-Id", 10415),  \n      )),  \n    )\n    header: DiameterHeader = DiameterHeader(application_id=0, command_code=257, avp_set=cer_request)\n    xml_dict_path: str = <path to diameter xml file>  \n\tdictionary_layout: DictionaryLayout = DefaultDictionaryLayout(xml_dict_path)  \n\tdiameter: Diameter = Diameter(dictionary_layout)\n    encoded_header: bytes = self.diameter.encode(header) #\tsend to TCP server     \n    decoded_header: DiameterHeader = diameter.decode(encoded_header) # decoded on TCP server',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'Development Status :: 4 - Beta',
             'Environment :: Console',
             'Intended Audience :: Developers',
```

