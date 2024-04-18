# Comparing `tmp/avrotize-1.2.4.tar.gz` & `tmp/avrotize-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.2.4.tar` & `avrotize-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    25996 2024-04-12 11:17:55.511102 avrotize-1.2.4/README.md
--rw-r--r--   0        0        0     1673 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-04-12 11:18:01.903017 avrotize-1.2.4/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    15558 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotize.py
--rw-r--r--   0        0        0    36250 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    18518 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12102 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18104 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22185 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13086 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10151 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-04-12 11:17:55.511102 avrotize-1.2.4/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    12889 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    91408 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    15752 2024-04-12 11:17:55.515102 avrotize-1.2.4/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1019 2024-04-12 11:17:55.515102 avrotize-1.2.4/pyproject.toml
--rw-r--r--   0        0        0    26663 1970-01-01 00:00:00.000000 avrotize-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0    25996 2024-04-18 10:59:54.192486 avrotize-1.3.0/README.md
+-rw-r--r--   0        0        0     1673 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-04-18 10:59:59.036447 avrotize-1.3.0/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    15558 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotize.py
+-rw-r--r--   0        0        0    42917 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    18563 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12117 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18104 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22200 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13101 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10166 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    12889 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    95346 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-04-18 10:59:54.192486 avrotize-1.3.0/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    17371 2024-04-18 10:59:54.196486 avrotize-1.3.0/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1019 2024-04-18 10:59:54.196486 avrotize-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    26663 1970-01-01 00:00:00.000000 avrotize-1.3.0/PKG-INFO
```

### Comparing `avrotize-1.2.4/README.md` & `avrotize-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/__init__.py` & `avrotize-1.3.0/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/asn1toavro.py` & `avrotize-1.3.0/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/avrotize.py` & `avrotize-1.3.0/avrotize/avrotize.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/avrotocsharp.py` & `avrotize-1.3.0/avrotize/avrotocsharp.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,120 +15,173 @@
 
 INDENT = '    '
 CSPROJ_CONTENT = """
 <Project Sdk="Microsoft.NET.Sdk">
     <PropertyGroup>
         <TargetFramework>net8.0</TargetFramework>
         <Nullable>enable</Nullable>
+        <GenerateDocumentationFile>true</GenerateDocumentationFile>
     </PropertyGroup>
     <ItemGroup>
         <PackageReference Include="Apache.Avro" Version="1.11.3" />
         <PackageReference Include="Newtonsoft.Json" Version="13.0.3" />
         <PackageReference Include="System.Text.Json" Version="8.0.3" />
         <PackageReference Include="System.Memory.Data" Version="8.0.0" />
     </ItemGroup>
 </Project>     
 """
 
+PREAMBLE_TOBYTEARRAY = \
+"""
+var contentType = new System.Net.Mime.ContentType(contentTypeString);
+byte[]? result = null;
+"""
+
+
+EPILOGUE_TOBYTEARRAY_COMPRESSION = \
+"""
+if (result != null && contentType.MediaType.EndsWith("+gzip"))
+{
+    var stream = new System.IO.MemoryStream();
+    using (var gzip = new System.IO.Compression.GZipStream(stream, System.IO.Compression.CompressionMode.Compress))
+    {
+        gzip.Write(result, 0, result.Length);
+    }
+    result = stream.ToArray();
+}
+"""
+
+EPILOGUE_TOBYTEARRAY = \
+"""
+return ( result != null ) ? result : throw new System.NotSupportedException($"Unsupported media type {contentType.MediaType}");
+"""
+
 AVRO_TOBYTEARRAY = \
-    """
-if (contentType == "avro/binary")
+"""
+if (contentType.MediaType.StartsWith("avro/binary") || contentType.MediaType.StartsWith("application/vnd.apache.avro+avro"))
+{
+    var stream = new System.IO.MemoryStream();
+    var writer = new Avro.Specific.SpecificDatumWriter<{type_name}>({type_name}.AvroSchema);
+    writer.Write(this, new Avro.IO.BinaryEncoder(stream));
+    result = stream.ToArray();
+}
+else if (contentType.MediaType.StartsWith("avro/json") || contentType.MediaType.StartsWith("application/vnd.apache.avro+json"))
 {
     var stream = new System.IO.MemoryStream();
-    var encoder = new Avro.IO.BinaryEncoder(stream);
     var writer = new Avro.Specific.SpecificDatumWriter<{type_name}>({type_name}.AvroSchema);
-    writer.Write(this, encoder);
-    return stream.ToArray();
+    writer.Write(this, new Avro.IO.JsonEncoder({type_name}.AvroSchema, stream));
+    result = stream.ToArray();
 }
 """
 
 SYSTEM_TEXT_JSON_TOBYTEARRAY = \
-    """
-if (contentType == System.Net.Mime.MediaTypeNames.Application.Json)
+"""
+if (contentType.MediaType.StartsWith(System.Net.Mime.MediaTypeNames.Application.Json))
 {
-    return System.Text.Json.JsonSerializer.SerializeToUtf8Bytes(this);
+    result = System.Text.Json.JsonSerializer.SerializeToUtf8Bytes(this);
 }"""
 
 NEWTONSOFT_JSON_TOBYTEARRAY = \
-    """
-if (contentType == System.Net.Mime.MediaTypeNames.Application.Json)
+"""
+if (contentType.MediaType.StartsWith(System.Net.Mime.MediaTypeNames.Application.Json))
+{
+    result = System.Text.Encoding.GetEncoding(contentType.CharSet??"utf-8").GetBytes(Newtonsoft.Json.JsonConvert.SerializeObject(this));
+}
+"""
+
+PREAMBLE_FROMDATA = \
+"""
+var contentType = new System.Net.Mime.ContentType(contentTypeString);
+"""
+
+PREAMBLE_FROMDATA_COMPRESSION = \
+"""
+if ( contentType.MediaType.EndsWith("+gzip"))
 {
-    return System.Text.Encoding.UTF8.GetBytes(Newtonsoft.Json.JsonConvert.SerializeObject(this));
+    var stream = data switch
+    {
+        System.IO.Stream s => s, System.BinaryData bd => bd.ToStream(), byte[] bytes => new System.IO.MemoryStream(bytes),
+        _ => throw new NotSupportedException("Data is not of a supported type for gzip decompression")
+    };
+    using (var gzip = new System.IO.Compression.GZipStream(stream, System.IO.Compression.CompressionMode.Decompress))
+    {
+        data = new System.IO.MemoryStream();
+        gzip.CopyTo((System.IO.MemoryStream)data);
+    }
 }
 """
 
+EPILOGUE_FROMDATA = \
+"""
+throw new System.NotSupportedException($"Unsupported media type {contentType.MediaType}");
+"""
+
 SYSTEM_TEXT_JSON_FROMDATA = \
-    """
-if ( contentType == System.Net.Mime.MediaTypeNames.Application.Json)
+"""
+if ( contentType.MediaType.StartsWith(System.Net.Mime.MediaTypeNames.Application.Json))
 {
     if (data is System.Text.Json.JsonElement) 
     {
         return System.Text.Json.JsonSerializer.Deserialize<{type_name}>((System.Text.Json.JsonElement)data);
     }
     else if ( data is string)
     {
         return System.Text.Json.JsonSerializer.Deserialize<{type_name}>((string)data);
     }
     else if (data is System.BinaryData)
     {
         return ((System.BinaryData)data).ToObjectFromJson<{type_name}>();
     }
-    throw new NotSupportedException("Data is not of a supported type for JSON conversion to {type_name}");
 }
 """
 
 NEWTONSOFT_JSON_FROMDATA = \
-    """
-if ( contentType == System.Net.Mime.MediaTypeNames.Application.Json)
+"""
+if ( contentType.MediaType.StartsWith(System.Net.Mime.MediaTypeNames.Application.Json))
 {
     if (data is string)
     {
         return Newtonsoft.Json.JsonConvert.DeserializeObject<{type_name}>((string)data);
     }
     else if (data is System.BinaryData)
     {
         return ((System.BinaryData)data).ToObjectFromJson<{type_name}>();
     }
-    throw new NotSupportedException("Data is not of a supported type for JSON conversion to {type_name}");
 }
 """
 
 AVRO_FROMDATA = \
-    """
-if ( contentType.StartsWith("avro/") || contentType.StartsWith("application/avro") )
+"""
+if ( contentType.MediaType.StartsWith("avro/") || contentType.MediaType.StartsWith("application/vnd.apache.avro") )
 {
     var stream = data switch
     {
-        System.IO.Stream s => s,
-        System.BinaryData bd => bd.ToStream(),
-        byte[] bytes => new System.IO.MemoryStream(bytes),
+        System.IO.Stream s => s, System.BinaryData bd => bd.ToStream(), byte[] bytes => new System.IO.MemoryStream(bytes),
         _ => throw new NotSupportedException("Data is not of a supported type for conversion to Stream")
     };
-    if ( contentType == "avro/binary" || contentType == "application/avro+binary")
+    if (contentType.MediaType.StartsWith("avro/binary") || contentType.MediaType.StartsWith("application/vnd.apache.avro+avro"))
     {
-        var decoder = new Avro.IO.BinaryDecoder(stream);
         var reader = new Avro.Specific.SpecificDatumReader<{type_name}>({type_name}.AvroSchema, {type_name}.AvroSchema);
-        return reader.Read(new {type_name}(), decoder);
+        return reader.Read(new {type_name}(), new Avro.IO.BinaryDecoder(stream));
     }
-    if ( contentType == "avro/json" || contentType == "application/avro+json")
+    if ( contentType.MediaType.StartsWith("avro/json") || contentType.MediaType.StartsWith("application/avro+json"))
     {
-        var decoder = new Avro.IO.JsonDecoder({type_name}.AvroSchema, stream);
         var reader = new Avro.Specific.SpecificDatumReader<{type_name}>({type_name}.AvroSchema, {type_name}.AvroSchema);
-        return reader.Read(new {type_name}(), decoder);
+        return reader.Read(new {type_name}(), new Avro.IO.JsonDecoder({type_name}.AvroSchema, stream));
     }
-    throw new NotSupportedException("Unsupported Avro content type: " + contentType);
 }    
 """
 
 
 class AvroToCSharp:
     """ Converts Avro schema to C# classes """
 
     def __init__(self, base_namespace: str = '') -> None:
         self.base_namespace = base_namespace
+        self.schema_doc: JsonNode = None
         self.output_dir = os.getcwd()
         self.pascal_properties = False
         self.system_text_json_annotation = False
         self.newtonsoft_json_annotation = False
         self.avro_annotation = False
         self.generated_types: Dict[str,str] = {}
 
@@ -223,111 +276,125 @@
         elif avro_schema['type'] == 'enum':
             return self.generate_enum(avro_schema, parent_namespace, write_file)
         return ''
 
     def generate_class(self, avro_schema: Dict, parent_namespace: str, write_file: bool) -> str:
         """ Generates a Class """
         class_definition = ''
-        namespace = pascal(self.concat_namespace(
-            self.base_namespace, avro_schema.get('namespace', parent_namespace)))
-        if 'doc' in avro_schema:
-            class_definition += f"/// <summary>\n/// {avro_schema['doc']}\n/// </summary>\n"
+        avro_namespace = avro_schema.get('namespace', parent_namespace)
+        namespace = pascal(self.concat_namespace(self.base_namespace, avro_namespace))
         class_name = pascal(avro_schema['name'])
-        fields_str = [self.generate_property(
-            field, class_name, namespace) for field in avro_schema.get('fields', [])]
+        class_definition += f"/// <summary>\n/// { avro_schema.get('doc', class_name ) }\n/// </summary>\n"
+        fields_str = [self.generate_property(field, class_name, avro_namespace) for field in avro_schema.get('fields', [])]
         class_body = "\n".join(fields_str)
         class_definition += f"public partial class {class_name}"
         if self.avro_annotation:
             class_definition += " : global::Avro.Specific.ISpecificRecord"
         class_definition += "\n{\n"+class_body
         if self.avro_annotation:
             avro_schema_json = json.dumps(avro_schema)
             # wrap schema at 80 characters
             avro_schema_json = avro_schema_json.replace('"', '§')
             avro_schema_json = f"\"+\n{INDENT}\"".join(
                 [avro_schema_json[i:i+80] for i in range(0, len(avro_schema_json), 80)])
             avro_schema_json = avro_schema_json.replace('§', '\\"')
-            class_definition += f"\n\n{INDENT}public static global::Avro.Schema AvroSchema = global::Avro.Schema.Parse(\n{INDENT}\"{avro_schema_json}\");\n"
+            class_definition += f"\n\n{INDENT}/// <summary>\n{INDENT}/// Avro schema for this class\n{INDENT}/// </summary>"
+            class_definition += f"\n{INDENT}public static global::Avro.Schema AvroSchema = global::Avro.Schema.Parse(\n{INDENT}\"{avro_schema_json}\");\n"
             class_definition += f"\n{INDENT}Schema global::Avro.Specific.ISpecificRecord.Schema => AvroSchema;\n"
             get_method = f"{INDENT}object global::Avro.Specific.ISpecificRecord.Get(int fieldPos)\n" + \
                 INDENT+"{"+f"\n{INDENT*2}switch (fieldPos)\n{INDENT*2}" + "{"
             put_method = f"{INDENT}void global::Avro.Specific.ISpecificRecord.Put(int fieldPos, object fieldValue)\n" + \
                 INDENT+"{"+f"\n{INDENT*2}switch (fieldPos)\n{INDENT*2}"+"{"
             for pos, field in enumerate(avro_schema.get('fields', [])):
                 field_name = field['name']
                 if self.is_csharp_reserved_word(field_name):
                     field_name = f"@{field_name}"
-                field_type = self.convert_avro_type_to_csharp(class_name, field_name, field['type'], namespace)
+                field_type = self.convert_avro_type_to_csharp(class_name, field_name, field['type'], avro_namespace)
                 if self.pascal_properties:
                     field_name = pascal(field_name)
                 if field_name == class_name:
                     field_name += "_"
                 get_method += f"\n{INDENT*3}case {pos}: return this.{field_name};"
                 put_method += f"\n{INDENT*3}case {pos}: this.{field_name} = ({field_type})fieldValue; break;"
             get_method += f"\n{INDENT*3}default: throw new global::Avro.AvroRuntimeException($\"Bad index {{fieldPos}} in Get()\");"
             put_method += f"\n{INDENT*3}default: throw new global::Avro.AvroRuntimeException($\"Bad index {{fieldPos}} in Put()\");"
             get_method += "\n"+INDENT+INDENT+"}\n"+INDENT+"}"
             put_method += "\n"+INDENT+INDENT+"}\n"+INDENT+"}"
             class_definition += f"\n{get_method}\n{put_method}\n"
 
         # emit ToByteArray method
-        class_definition += f"\n\n{INDENT}public byte[] ToByteArray(string? contentType)\n{INDENT}{{"
+        class_definition += f"\n{INDENT}/// <summary>\n{INDENT}/// Converts the object to a byte array\n{INDENT}/// </summary>"
+        class_definition += f"\n{INDENT}/// <param name=\"contentTypeString\">The content type string of the desired encoding</param>"
+        class_definition += f"\n{INDENT}/// <returns>The encoded data</returns>"
+        class_definition += f"\n{INDENT}public byte[] ToByteArray(string contentTypeString)\n{INDENT}{{"
+        class_definition += f'\n{INDENT*2}'.join((PREAMBLE_TOBYTEARRAY).split("\n"))
         if self.avro_annotation:
             class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
                 AVRO_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
         if self.system_text_json_annotation:
             class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
                 SYSTEM_TEXT_JSON_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
         if self.newtonsoft_json_annotation:
             class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
                 NEWTONSOFT_JSON_TOBYTEARRAY.strip().replace("{type_name}", class_name).split("\n"))
-        class_definition += f"\n{INDENT*2}throw new System.NotImplementedException($\"Unsupported content type {{contentType}}\");\n{INDENT}}}"
+        if self.avro_annotation or self.system_text_json_annotation or self.newtonsoft_json_annotation:
+            class_definition += f"\n{INDENT*2}".join((EPILOGUE_TOBYTEARRAY_COMPRESSION).split("\n"))
+        class_definition += f"\n{INDENT*2}".join((EPILOGUE_TOBYTEARRAY).split("\n"))+f"\n{INDENT}}}"
 
         # emit FromData factory method
-        class_definition += f"\n\n{INDENT}public static {class_name} FromData(object? data, string contentType)\n{INDENT}{{"
+        class_definition += f"\n\n{INDENT}/// <summary>\n{INDENT}/// Creates an object from the data\n{INDENT}/// </summary>"
+        class_definition += f"\n{INDENT}/// <param name=\"data\">The input data to convert</param>"
+        class_definition += f"\n{INDENT}/// <param name=\"contentTypeString\">The content type string of the derired encoding</param>"
+        class_definition += f"\n{INDENT}/// <returns>The converted object</returns>"
+        class_definition += f"\n{INDENT}public static {class_name} FromData(object data, string contentTypeString)\n{INDENT}{{"
         class_definition += f'\n{INDENT*2}if ( data is {class_name}) return ({class_name})data;'
+        class_definition += f'\n{INDENT*2}'.join(((PREAMBLE_FROMDATA)).split("\n"))
+        if self.avro_annotation or self.system_text_json_annotation or self.newtonsoft_json_annotation:
+            class_definition += f'\n{INDENT*2}'.join(((PREAMBLE_FROMDATA_COMPRESSION)).split("\n"))
         if self.avro_annotation:
             class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
                 AVRO_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
         if self.system_text_json_annotation:
             class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
                 SYSTEM_TEXT_JSON_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
         if self.newtonsoft_json_annotation:
             class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
                 NEWTONSOFT_JSON_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
-        class_definition += f"\n{INDENT*2}throw new System.NotImplementedException($\"Unsupported content type {{contentType}}\");\n{INDENT}}}"
+        class_definition += f"\n{INDENT*2}".join((EPILOGUE_FROMDATA).split('\n'))+f"\n{INDENT}}}"
 
         # emit IsJsonMatch method for System.Text.Json
         if self.system_text_json_annotation:
-            class_definition += self.create_is_json_match_method(avro_schema, namespace, class_name)
+            class_definition += self.create_is_json_match_method(avro_schema, avro_namespace, class_name)
         class_definition += "\n"+"}"
 
         if write_file:
             self.write_to_file(namespace, class_name, class_definition)
         ref = 'global::'+self.concat_namespace(namespace, class_name)
         self.generated_types[ref] = "class"
         return ref
 
-    def create_is_json_match_method(self, avro_schema, namespace, class_name) -> str:
+    def create_is_json_match_method(self, avro_schema, parent_namespace, class_name) -> str:
         """ Generates the IsJsonMatch method for System.Text.Json """
         class_definition = ''
-        class_definition += f"\n\n{INDENT}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT}{{"
+        class_definition += f"\n\n{INDENT}/// <summary>\n{INDENT}/// Checks if the JSON element matches the schema\n{INDENT}/// </summary>"
+        class_definition += f"\n{INDENT}/// <param name=\"element\">The JSON element to check</param>"
+        class_definition += f"\n{INDENT}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT}{{"
         class_definition += f"\n{INDENT*2}return "
         field_count = 0
         for field in avro_schema.get('fields', []):
             if field_count > 0:
                 class_definition += f" && \n{INDENT*3}"
             field_count += 1
             field_name = field['name']
             if self.is_csharp_reserved_word(field_name):
                 field_name = f"@{field_name}"
             if field_name == class_name:
                 field_name += "_"
             field_type = self.convert_avro_type_to_csharp(
-                    class_name, field_name, field['type'], namespace)
+                    class_name, field_name, field['type'], parent_namespace)
             class_definition += self.get_is_json_match_clause(class_name, field_name, field_type)
         class_definition += f";\n{INDENT}}}"
         return class_definition
 
     def get_is_json_match_clause(self, class_name, field_name, field_type) -> str:
         """ Generates the IsJsonMatch clause for a field """
         class_definition = ''
@@ -394,22 +461,23 @@
         return class_definition
 
     def generate_enum(self, avro_schema: Dict, parent_namespace: str, write_file: bool) -> str:
         """ Generates an Enum """
         enum_definition = ''
         namespace = pascal(self.concat_namespace(
             self.base_namespace, avro_schema.get('namespace', parent_namespace)))
-        if 'doc' in avro_schema:
-            enum_definition += f"/// <summary>\n/// {avro_schema['doc']}\n/// </summary>\n"
         enum_name = pascal(avro_schema['name'])
+        enum_definition += "#pragma warning disable 1591\n\n"
+        enum_definition += f"/// <summary>\n/// {avro_schema.get('doc', enum_name )}\n/// </summary>\n"        
         symbols_str = [
             f"{INDENT}{symbol}" for symbol in avro_schema['symbols']]
         enum_body = ",\n".join(symbols_str)
         enum_definition += f"public enum {enum_name}\n{{\n{enum_body}\n}}"
         
+        
         if write_file:
             self.write_to_file(namespace, enum_name, enum_definition)
         ref = 'global::'+self.concat_namespace(namespace, enum_name)
         self.generated_types[ref] = "enum"
         return ref
 
     def generate_embedded_union_class_system_json_text(self, class_name: str, field_name: str, avro_type: List, parent_namespace: str, write_file: bool) -> str:
@@ -432,16 +500,20 @@
                 union_type_name = "Array" + pascal(match[0].rsplit('.', 1)[-1])
             elif union_type == "byte[]":
                 union_type_name = "bytes"
             else:
                 union_type_name = union_type.rsplit('.', 1)[-1]
             if self.is_csharp_reserved_word(union_type_name):
                 union_type_name = f"@{union_type_name}"
-            class_definition_ctors += f"{INDENT*2}public {union_class_name}({union_type}? {union_type_name})\n{INDENT*2}{{\n{INDENT*3}this.{union_type_name} = {union_type_name};\n{INDENT*2}}}\n"
-            class_definition_decls += f"{INDENT*2}public {union_type}? {union_type_name} {{ get; private set; }} = null;\n"            
+            class_definition_ctors += \
+                f"{INDENT*2}/// <summary>\n{INDENT*2}/// Constructor for {union_type_name} values\n{INDENT*2}/// </summary>\n" + \
+                f"{INDENT*2}public {union_class_name}({union_type}? {union_type_name})\n{INDENT*2}{{\n{INDENT*3}this.{union_type_name} = {union_type_name};\n{INDENT*2}}}\n"
+            class_definition_decls += \
+                f"{INDENT*2}/// <summary>\n{INDENT*2}/// Gets the {union_type_name} value\n{INDENT*2}/// </summary>\n" + \
+                f"{INDENT*2}public {union_type}? {union_type_name} {{ get; private set; }} = null;\n"            
             if is_dict:
                 class_definition_read += f"{INDENT*3}if (element.ValueKind == JsonValueKind.Object)\n{INDENT*3}{{\n" + \
                         f"{INDENT*4}var map = System.Text.Json.JsonSerializer.Deserialize<{union_type}>(element, options);\n" + \
                         f"{INDENT*4}if (map != null) {{ return new {union_class_name}(map); }} else {{ throw new NotSupportedException(); }};\n" + \
                         f"{INDENT*3}}}\n"
             elif is_list:
                 class_definition_read += f"{INDENT*3}if (element.ValueKind == JsonValueKind.Array)\n{INDENT*3}{{\n" + \
@@ -465,62 +537,99 @@
                 class_definition_read += f"{INDENT*3}if ({union_type}.IsJsonMatch(element))\n{INDENT*3}{{\n{INDENT*4}return new {union_class_name}({union_type}.FromData(element, System.Net.Mime.MediaTypeNames.Application.Json));\n{INDENT*3}}}\n"
             class_definition_write += f"{INDENT*3}{'else ' if i>0 else ''}if (value.{union_type_name} != null)\n{INDENT*3}{{\n{INDENT*4}System.Text.Json.JsonSerializer.Serialize(writer, value.{union_type_name}, options);\n{INDENT*3}}}\n"
             gij = self.get_is_json_match_clause_type("element", class_name, union_type)
             if gij:
                 list_is_json_match.append(gij)
 
         class_definition = \
+            f"/// <summary>\n/// {class_name}. Type union resolver. \n/// </summary>\n" + \
             f"public partial class {class_name}\n{{\n{INDENT}[System.Text.Json.Serialization.JsonConverter(typeof({union_class_name}))]\n{INDENT}public sealed class {union_class_name} : System.Text.Json.Serialization.JsonConverter<{union_class_name}>\n{INDENT}{{\n" + \
+            f"{INDENT*2}/// <summary>\n{INDENT*2}/// Default constructor\n{INDENT*2}/// </summary>\n" + \
             f"{INDENT*2}public {union_class_name}() {{ }}\n" + \
             class_definition_ctors + \
             class_definition_decls + \
-            f"\n{INDENT*2}public override {union_class_name}? Read(ref Utf8JsonReader reader, Type typeToConvert, JsonSerializerOptions options)\n{INDENT*2}{{\n{INDENT*3}var element = JsonElement.ParseValue(ref reader);\n" + \
+            f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Reads the JSON representation of the object.\n{INDENT*2}/// </summary>\n" + \
+            f"{INDENT*2}public override {union_class_name}? Read(ref Utf8JsonReader reader, Type typeToConvert, JsonSerializerOptions options)\n{INDENT*2}{{\n{INDENT*3}var element = JsonElement.ParseValue(ref reader);\n" + \
             class_definition_read + \
             f"{INDENT*3}throw new NotSupportedException(\"No record type matched the JSON data\");\n{INDENT*2}}}\n" + \
-            f"\n{INDENT*2}public override void Write(Utf8JsonWriter writer, {union_class_name} value, JsonSerializerOptions options)\n{INDENT*2}{{\n" + \
+            f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Writes the JSON representation of the object.\n{INDENT*2}/// </summary>\n" + \
+            f"{INDENT*2}public override void Write(Utf8JsonWriter writer, {union_class_name} value, JsonSerializerOptions options)\n{INDENT*2}{{\n" + \
             class_definition_write + \
             f"{INDENT*3}else\n{INDENT*3}{{\n{INDENT*4}throw new NotSupportedException(\"No record type is set in the union\");\n{INDENT*3}}}\n{INDENT*2}}}\n" + \
-            f"\n{INDENT*2}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT*2}{{" + \
+            f"\n{INDENT*2}/// <summary>\n{INDENT*2}/// Checks if the JSON element matches the schema\n{INDENT*2}/// </summary>\n" + \
+            f"{INDENT*2}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT*2}{{" + \
             f"\n{INDENT*3}return "+f"\n{INDENT*3} || ".join(list_is_json_match)+f";\n{INDENT*2}}}\n" + \
             f"{INDENT*1}}}\n}}\n"
 
         if write_file:
-            self.write_to_file(parent_namespace, class_name +"."+union_class_name, class_definition)
+            self.write_to_file(pascal(parent_namespace), class_name +"."+union_class_name, class_definition)
         self.generated_types[class_name+'.'+union_class_name] = "union" # it doesn't matter if the names clash, we just need to know whether it's a union
         return union_class_name
 
+    def find_type(self, kind: str, avro_schema: JsonNode, type_name: str, type_namespace: str, parent_namespace = '') -> JsonNode:
+        """ recursively find the type (kind 'record' or 'enum') in the schema """
+        if isinstance(avro_schema, list):
+            for s in avro_schema:
+                found = self.find_type(kind, s, type_name, type_namespace, parent_namespace)
+                if found:
+                    return found
+        elif isinstance(avro_schema, dict):
+            if avro_schema['type'] == kind and avro_schema['name'] == type_name and avro_schema.get('namespace', parent_namespace) == type_namespace:
+                return avro_schema
+            parent_namespace = avro_schema.get('namespace', parent_namespace)            
+            if 'fields' in avro_schema and isinstance(avro_schema['fields'], list):
+                for field in avro_schema['fields']:
+                    if isinstance(field,dict) and 'type' in field and isinstance(field['type'], dict):
+                        return self.find_type(kind, field['type'], type_name, type_namespace, parent_namespace)
+        return None
+
+    def is_enum_type(self, avro_type: Union[str, Dict, List]) -> bool:
+        """ Checks if a type is an enum """
+        if isinstance(avro_type, str):
+            schema = self.schema_doc
+            name = avro_type.split('.')[-1]
+            namespace = ".".join(avro_type.split('.')[:-1])
+            return self.find_type('enum', schema, name, namespace) is not None
+        elif isinstance(avro_type, list):
+            return False
+        elif isinstance(avro_type, dict):
+            return avro_type['type'] == 'enum'
+
     def generate_property(self, field: Dict, class_name: str, parent_namespace: str) -> str:
         """ Generates a property """
+        is_enum_type = self.is_enum_type(field['type'])
         field_type = self.convert_avro_type_to_csharp(
             class_name, field['name'], field['type'], parent_namespace)
+        field_default = field.get('const', field.get('default', None))
         annotation_name = field_name = field['name']
         if self.is_csharp_reserved_word(field_name):
             field_name = f"@{field_name}"
         if self.pascal_properties:
             field_name = pascal(field_name)
         if field_name == class_name:
             field_name += "_"
         prop = ''
-        if 'doc' in field:
-            prop += f"{INDENT}/// <summary>\n{INDENT}/// {field['doc']}\n{INDENT}/// </summary>\n"
+        prop += f"{INDENT}/// <summary>\n{INDENT}/// { field.get('doc', field_name) }\n{INDENT}/// </summary>\n"
         if self.system_text_json_annotation:
-            prop += f"{INDENT}[JsonPropertyName(\"{annotation_name}\")]\n"
+            prop += f"{INDENT}[System.Text.Json.Serialization.JsonPropertyName(\"{annotation_name}\")]\n"
+            if is_enum_type:
+                prop += f"{INDENT}[System.Text.Json.Serialization.JsonConverter(typeof(JsonStringEnumConverter))]\n"
             if field_type.endswith("Union") and not field_type.startswith("global::"):
                 prop += f"{INDENT}[System.Text.Json.Serialization.JsonConverter(typeof({field_type}))]\n"
         if self.newtonsoft_json_annotation:
-            prop += f"{INDENT}[JsonProperty(\"{annotation_name}\")]\n"
-        prop += f"{INDENT}public {field_type} {field_name} {{ get; set; }}"
+            prop += f"{INDENT}[Newtonsoft.Json.JsonProperty(\"{annotation_name}\")]\n"
+        prop += f"{INDENT}public {field_type} {field_name} {{ get; {'private ' if 'const' in field else ''}set; }}" + ((" = "+(f"\"{field_default}\"" if isinstance(field_default,str) else field_default) + ";") if field_default else "")
         return prop
 
     def write_to_file(self, namespace: str, name: str, definition: str):
         """ Writes the class or enum to a file """
         directory_path = os.path.join(
             self.output_dir, os.path.join(namespace.replace('.', os.sep)))
         if not os.path.exists(directory_path):
-            os.makedirs(directory_path)
+            os.makedirs(directory_path, exist_ok=True)
         file_path = os.path.join(directory_path, f"{name}.cs")
 
         with open(file_path, 'w', encoding='utf-8') as file:
             # Common using statements (add more as needed)
             file_content = "#pragma warning disable CS8618\n#pragma warning disable CS8603\n\nusing System;\nusing System.Collections.Generic;\n"
             if self.system_text_json_annotation:
                 file_content += "using System.Text.Json;\n"
@@ -536,15 +645,16 @@
             file_content += f"{indented_definition}\n}}"
             file.write(file_content)
 
     def convert_schema(self, schema: JsonNode, output_dir: str):
         """ Converts Avro schema to C# """
         if not isinstance(schema, list):
             schema = [schema]
-
+            
+        self.schema_doc = schema
         if not glob.glob(os.path.join(output_dir, '*.csproj')):
             csproj_file = os.path.join(
                 output_dir, f"{os.path.basename(output_dir)}.csproj")
             if not os.path.exists(csproj_file):
                 with open(csproj_file, 'w', encoding='utf-8') as file:
                     file.write(CSPROJ_CONTENT)
         self.output_dir = output_dir
```

### Comparing `avrotize-1.2.4/avrotize/avrotojava.py` & `avrotize-1.3.0/avrotize/avrotojava.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
                 property_def += f"{INDENT}public void set{field_name.capitalize()}As{flatten_type_name(union_type.type_name)}({union_type.type_name} {field_name}) {{ this.{field_name} = {field_name}; }}\n"
         return property_def
 
     def write_to_file(self, package: str, name: str, definition: str):
         """ Writes a Java class or enum to a file """
         directory_path = os.path.join(self.output_dir, package.replace('.', os.sep))
         if not os.path.exists(directory_path):
-            os.makedirs(directory_path)
+            os.makedirs(directory_path, exist_ok=True)
         file_path = os.path.join(directory_path, f"{name}.java")
 
         with open(file_path, 'w', encoding='utf-8') as file:
             if package:
                 file.write(f"package {package.replace('/', '.')};\n\n")
                 if "List<" in definition:
                     file.write("import java.util.List;\n")
@@ -323,23 +323,23 @@
             file.write(definition)
 
     def convert_schema(self, schema: JsonNode, output_dir: str):
         """Converts Avro schema to Java"""
         if not isinstance(schema, list):
             schema = [schema]
         if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
+            os.makedirs(output_dir, exist_ok=True)
         pom_path = os.path.join(output_dir, "pom.xml")
         if not os.path.exists(pom_path):
             with open(pom_path, 'w', encoding='utf-8') as file:
                 file.write(POM_CONTENT)
         output_dir = os.path.join(
             output_dir, "src/main/java".replace('/', os.sep))
         if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
+            os.makedirs(output_dir, exist_ok=True)
         self.output_dir = output_dir
         for avro_schema in (x for x in schema if isinstance(x, dict)):
             self.generate_class_or_enum(avro_schema, self.base_package)
 
     def convert(self, avro_schema_path: str, output_dir: str):
         """Converts Avro schema to Java"""
         with open(avro_schema_path, 'r', encoding='utf-8') as file:
```

### Comparing `avrotize-1.2.4/avrotize/avrotojs.py` & `avrotize-1.3.0/avrotize/avrotojs.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         self.write_to_file(namespace, enum_name, enum_definition)
         return f'{namespace}.{enum_name}'
 
     def write_to_file(self, namespace: str, name: str, content: str):
         """ Write TypeScript class to file """
         directory_path = os.path.join(self.output_dir, namespace.replace('.', os.sep))
         if not os.path.exists(directory_path):
-            os.makedirs(directory_path)
+            os.makedirs(directory_path, exist_ok=True)
         
         file_path = os.path.join(directory_path, f"{name}.js")
         with open(file_path, 'w', encoding='utf-8') as file:
             file.write(content)
 
     def convert_schema(self, schema: List|Dict, output_dir: str):
         """ Convert Avro schema to TypeScript classes """
```

### Comparing `avrotize-1.2.4/avrotize/avrotojsons.py` & `avrotize-1.3.0/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/avrotokusto.py` & `avrotize-1.3.0/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/avrotoparquet.py` & `avrotize-1.3.0/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/avrotoproto.py` & `avrotize-1.3.0/avrotize/avrotoproto.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
 
             #proto.imports.extend([f.package[len(proto.package)+1:] for f in proto_files.files if f.package.startswith(proto.package) and f.package != proto.package])
             proto.imports.extend([d for d in deps if d != proto.package])
             proto_file_path = os.path.join(proto_path, f"{proto.package}.proto")
             # create the directory for the proto file if it doesn't exist
             proto_dir = os.path.dirname(proto_file_path)
             if not os.path.exists(proto_dir):
-                os.makedirs(proto_dir)
+                os.makedirs(proto_dir, exist_ok=True)
             with open(proto_file_path, 'w') as proto_file:
                 # dump the ProtoFile structure in proto syntax
                 proto_str = f'syntax = "proto3";\n\n'
                 proto_str += f'package {proto.package};\n\n'
 
                 for import_package in proto.imports:
                     proto_str += f"import \"{import_package}.proto\";\n"
```

### Comparing `avrotize-1.2.4/avrotize/avrotopython.py` & `avrotize-1.3.0/avrotize/avrotopython.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         field_docstring = INDENT*2 + f"{field_name} ({field_type}): {field_doc}\n"
         return field_docstring
     
     def write_to_file(self, package:str, name: str, definition: str):
         """Writes a Python class to a file"""
         directory_path = os.path.join(self.output_dir, package.replace('.', '/').replace('/', os.sep).lower())
         if not os.path.exists(directory_path):
-            os.makedirs(directory_path)
+            os.makedirs(directory_path, exist_ok=True)
         
         # drop an __init.py__ file in all directories along the path above output_dir
         package_name = package
         while package_name:
             init_file_path = os.path.join(directory_path, '__init__.py')
             if not os.path.exists(init_file_path):
                 with open(init_file_path, 'w', encoding='utf-8') as file:
```

### Comparing `avrotize-1.2.4/avrotize/avrotots.py` & `avrotize-1.3.0/avrotize/avrotots.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         self.write_to_file(namespace, enum_name, enum_definition)
         return f'{namespace}.{enum_name}'
 
     def write_to_file(self, namespace: str, name: str, content: str):
         """ Write TypeScript class to file """
         directory_path = os.path.join(self.output_dir, namespace.replace('.', os.sep))
         if not os.path.exists(directory_path):
-            os.makedirs(directory_path)
+            os.makedirs(directory_path, exist_ok=True)
         
         file_path = os.path.join(directory_path, f"{name}.ts")
         with open(file_path, 'w', encoding='utf-8') as file:
             file.write(content)
 
     def convert_schema(self, schema: List|Dict, output_dir: str):
         """ Convert Avro schema to TypeScript classes """
```

### Comparing `avrotize-1.2.4/avrotize/avrototsql.py` & `avrotize-1.3.0/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/avrotoxsd.py` & `avrotize-1.3.0/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/common.py` & `avrotize-1.3.0/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/dependency_resolver.py` & `avrotize-1.3.0/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/generic/generic.avsc` & `avrotize-1.3.0/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/jsonstoavro.py` & `avrotize-1.3.0/avrotize/jsonstoavro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+""" JSON to Avro schema converter. """
+
+# pylint: disable=too-many-lines, line-too-long, too-many-branches, too-many-statements, too-many-locals, too-many-nested-blocks, too-many-arguments, too-many-instance-attributes, too-many-public-methods, too-many-boolean-expressions
+
 import json
 import os
+import copy
+import urllib
+from urllib.parse import ParseResult, urlparse, unquote
 from typing import Any, Dict, List, Tuple
 import jsonpointer
 from jsonpointer import JsonPointerException
 import requests
-import copy
 
-import urllib
 from avrotize.common import avro_name, avro_namespace, find_schema_node, generic_type, set_schema_node
 from avrotize.dependency_resolver import inline_dependencies_of, sort_messages_by_dependencies
-from urllib.parse import ParseResult, urlparse, unquote
 
+primitive_types = ['null', 'string', 'int',
+                   'long', 'float', 'double', 'boolean', 'bytes']
 
-primitive_types = ['null', 'string', 'int', 'long', 'float', 'double', 'boolean', 'bytes']
 
 class JsonToAvroConverter:
     """
     Converts JSON schema to Avro schema.
 
     Attributes:
     imported_types: A dictionary of imported type schemas.
@@ -30,15 +35,15 @@
     """
 
     def __init__(self) -> None:
         self.imported_types: Dict[Any, Any] = {}
         self.root_namespace = 'example.com'
         self.max_recursion_depth = 40
         self.types_with_unmerged_types: List[dict] = []
-        self.content_cache: Dict[str,str] = {}
+        self.content_cache: Dict[str, str] = {}
         self.utility_namespace = 'utility.vasters.com'
         self.split_top_level_records = False
         self.root_class_name = 'document'
 
     def is_empty_type(self, avro_type):
         """
         Check if the Avro type is an empty type.
@@ -55,18 +60,18 @@
             return all(self.is_empty_type(t) for t in avro_type)
         if isinstance(avro_type, dict):
             if not 'type' in avro_type:
                 return True
             if (avro_type['type'] == 'record' and (not 'fields' in avro_type or len(avro_type['fields']) == 0)) or \
                (avro_type['type'] == 'enum' and (not 'symbols' in avro_type or len(avro_type['symbols']) == 0)) or \
                (avro_type['type'] == 'array' and (not 'items' in avro_type or not avro_type['items'])) or \
-               (avro_type['type'] == 'map' and (not 'values' in avro_type or not avro_type['values'])):                
+               (avro_type['type'] == 'map' and (not 'values' in avro_type or not avro_type['values'])):
                 return True
         return False
-    
+
     def is_empty_json_type(self, json_type):
         """
         Check if the JSON type is an empty type.
 
         Parameters:
         json_type (any): The JSON type to check.
 
@@ -118,220 +123,236 @@
                     map_type = t
                     flat_list_1.append(t)
                 else:
                     map_type = self.merge_avro_schemas([map_type, t], [])
             elif not t in flat_list_1:
                 flat_list_1.append(t)
         return flat_list_1
-    
+
+    # pylint: disable=dangerous-default-value
     def merge_avro_schemas(self, schemas: list, avro_schemas: list, type_name: str | None = None, deps: List[str] = []) -> str | list | dict:
         """Merge multiple Avro type schemas into one."""
 
-        def split_merge(schema1, schema2, schema_list,offset):
+        def split_merge(schema1, schema2, schema_list, offset):
             """ return the continuing schema merges of incompatible schemas """
-            remaining_schemas = schema_list[offset + 1:] if len(schema_list) > offset else []
+            remaining_schemas = schema_list[offset +
+                                            1:] if len(schema_list) > offset else []
             if isinstance(schema2, dict) and 'dependencies' in schema2:
                 deps.extend(schema2['dependencies'])
                 del schema2['dependencies']
             if isinstance(schema1, dict) and 'dependencies' in schema1:
                 deps.extend(schema1['dependencies'])
                 del schema1['dependencies']
-            schema1_merged = self.merge_avro_schemas([schema2] + remaining_schemas, avro_schemas, type_name, deps)
-            schema2_merged = self.merge_avro_schemas([schema1] + remaining_schemas, avro_schemas, type_name, deps)
+            schema1_merged = self.merge_avro_schemas(
+                [schema2] + remaining_schemas, avro_schemas, type_name, deps)
+            schema2_merged = self.merge_avro_schemas(
+                [schema1] + remaining_schemas, avro_schemas, type_name, deps)
             if not self.is_empty_type(schema1_merged) and not self.is_empty_type(schema2_merged):
                 return self.flatten_union([schema1_merged, schema2_merged])
-            else:	
+            else:
                 if not self.is_empty_type(schema1_merged):
                     return schema1_merged
                 if not self.is_empty_type(schema2_merged):
                     return schema2_merged
                 # if both are empty, we'll return an empty record
                 return {'type': 'record', 'fields': []}
-        
+
         merged_schema: dict = {}
         if len(schemas) == 1:
             return schemas[0]
         if type_name:
             self.set_avro_type_value(merged_schema, 'name', type_name)
         for i, schema in enumerate(schemas):
             schema = copy.deepcopy(schema)
             if isinstance(schema, dict) and 'dependencies' in schema:
                 deps1: List[str] = merged_schema.get('dependencies', [])
                 deps1.extend(schema['dependencies'])
                 merged_schema['dependencies'] = deps1
             if (isinstance(schema, list) or isinstance(schema, dict)) and len(schema) == 0:
                 continue
             if isinstance(schema, str):
-                sch = next((s for s in avro_schemas if s.get('name') == schema), None)
+                sch = next(
+                    (s for s in avro_schemas if s.get('name') == schema), None)
                 if sch:
                     merged_schema.update(sch)
                 else:
                     merged_schema['type'] = schema
             elif isinstance(schema, list):
                 # the incoming schema is a list, so it's a union
-                if not 'type' in merged_schema:
+                if 'type' not in merged_schema:
                     merged_schema['type'] = schema
                 else:
                     if isinstance(merged_schema['type'], list):
-                        merged_schema['type'].extend(schema) 
+                        merged_schema['type'].extend(schema)
                     else:
                         if isinstance(merged_schema['type'], str):
                             if merged_schema['type'] == 'record' or merged_schema['type'] == 'enum' or merged_schema['type'] == 'fixed' \
                                or merged_schema['type'] == 'map' or merged_schema['type'] == 'array':
                                 return split_merge(merged_schema, schema, schemas, i)
                             else:
-                                merged_schema['type'] = [merged_schema['type']]    
+                                merged_schema['type'] = [merged_schema['type']]
                         else:
-                            merged_schema['type'].extend(schema)                                            
+                            merged_schema['type'].extend(schema)
             elif schema and ('type' not in schema or 'type' not in merged_schema):
                 merged_schema.update(schema)
             elif schema:
                 if 'type' in merged_schema and schema['type'] != merged_schema['type']:
-                    return split_merge(merged_schema, schema, schemas, i)           
+                    return split_merge(merged_schema, schema, schemas, i)
                 if not type_name:
-                    self.set_avro_type_value(merged_schema, 'name', avro_name(merged_schema.get('name', '') + schema.get('name', '')))
+                    self.set_avro_type_value(merged_schema, 'name', avro_name(
+                        merged_schema.get('name', '') + schema.get('name', '')))
                 if 'fields' in schema:
                     if 'fields' in merged_schema:
                         for field in schema['fields']:
                             if field not in merged_schema['fields']:
                                 merged_schema['fields'].append(field)
                             else:
-                                merged_schema_field = next(f for f in merged_schema['fields'] if f.get('name') == field.get('name'))
+                                merged_schema_field = next(
+                                    f for f in merged_schema['fields'] if f.get('name') == field.get('name'))
                                 if merged_schema_field['type'] != field['type']:
-                                    merged_schema_field['type'] = [field['type'],merged_schema_field['type']]
+                                    merged_schema_field['type'] = [
+                                        field['type'], merged_schema_field['type']]
                                 if 'doc' in field and 'doc' not in merged_schema_field:
                                     merged_schema_field['doc'] = field['doc']
                     else:
-                        merged_schema['fields'] = schema['fields']                                
+                        merged_schema['fields'] = schema['fields']
         if self.is_avro_complex_type(merged_schema) and 'namespace' in merged_schema:
             if merged_schema['type'] in ['array', 'map']:
                 del merged_schema['namespace']
         return merged_schema
 
     def merge_json_schemas(self, json_schemas: list[dict], intersect: bool = False) -> dict:
-            """
-            Merge multiple JSON schemas into one.
+        """
+        Merge multiple JSON schemas into one.
 
-            Args:
-                json_schemas (list[dict]): A list of JSON schemas to be merged.
-                intersect (bool, optional): If True, only keep the intersection of the required fields. Defaults to False.
-
-            Returns:
-                dict: The merged JSON schema.
-            """
-
-            def merge_structures(schema1: dict, schema2: dict) -> dict|list:
-                """ merge two JSON dicts recursively """
-                if 'type' in schema1 and 'type' in schema2 and schema1['type'] != schema2['type']:
-                    return [schema1, schema2]
-                schema1 = copy.deepcopy(schema1)
-                for key in schema2:
-                    if key not in schema1:
-                        schema1[key] = schema2[key]
-                    elif isinstance(schema1[key], dict) and isinstance(schema2[key], dict):
-                        schema1[key] = merge_structures(schema1[key], schema2[key])
-                    elif isinstance(schema1[key], list) and isinstance(schema2[key], list):
-                        schema1[key].extend(schema2[key])
-                    elif schema1[key] == schema2[key]:
-                        continue
-                    else:                    
-                        if isinstance(schema1[key], list):
-                            if schema2[key] not in schema1[key]:
-                                schema1[key].append(schema2[key])
-                        else:
-                            schema1[key] = [schema1[key], schema2[key]]
-                return schema1
+        Args:
+            json_schemas (list[dict]): A list of JSON schemas to be merged.
+            intersect (bool, optional): If True, only keep the intersection of the required fields. Defaults to False.
 
-            merged_type:dict = {}
+        Returns:
+            dict: The merged JSON schema.
+        """
 
-            for json_schema in json_schemas:
-                if 'type' not in json_schema or 'type' not in merged_type:
-                    for key in json_schema:
-                        if not key in merged_type:
-                            merged_type[key] = copy.deepcopy(json_schema[key])
-                        else:
-                            if key == 'required':
-                                merged_type[key] = list(set(merged_type[key]).union(set(json_schema[key])))
-                            if key == 'name' or key == 'title' or key == 'description':
-                                merged_type[key] = merged_type[key] + json_schema[key]
-                            elif isinstance(merged_type[key], dict):
-                                merged_type[key] = merge_structures(merged_type[key],copy.deepcopy(json_schema[key]))
-                            elif isinstance(merged_type[key], list) and isinstance(json_schema[key], list):
-                                for item in json_schema[key]:
-                                    if item not in merged_type[key]:
-                                        merged_type[key].append(item)
-                            else:
-                                if merged_type[key] == None:
-                                    merged_type[key] = json_schema[key]
-                                else:
-                                    merged_type[key] = [merged_type[key], copy.deepcopy(json_schema[key])]
+        def merge_structures(schema1: dict, schema2: dict) -> dict | list:
+            """ merge two JSON dicts recursively """
+            if 'type' in schema1 and 'type' in schema2 and schema1['type'] != schema2['type']:
+                return [schema1, schema2]
+            schema1 = copy.deepcopy(schema1)
+            for key in schema2:
+                if key not in schema1:
+                    schema1[key] = schema2[key]
+                elif isinstance(schema1[key], dict) and isinstance(schema2[key], dict):
+                    schema1[key] = merge_structures(schema1[key], schema2[key])
+                elif isinstance(schema1[key], list) and isinstance(schema2[key], list):
+                    schema1[key].extend(schema2[key])
+                elif schema1[key] == schema2[key]:
+                    continue
                 else:
-                    if 'type' in merged_type and json_schema['type'] != merged_type['type']:
-                        if isinstance(merged_type['type'], str):
-                            merged_type['type'] = [merged_type['type']]
-                        merged_type['type'].append(json_schema['type'])                    
-                    if 'required' in json_schema:
-                        if 'required' in merged_type:
-                            merged_type['required'] = list(set(merged_type['required']).union(set(json_schema['required'])))
-                        else:
-                            merged_type['required'] = json_schema['required']
-                    if 'name' in json_schema:
-                        if 'name' in merged_type:
-                            merged_type['name'] = merged_type.get('name','') + json_schema['name']
-                        else:
-                            merged_type['name'] = json_schema['name']
-                    if 'properties' in json_schema:
-                        if 'properties' in merged_type:
-                            for prop in json_schema['properties']:
-                                if prop in merged_type['properties']:
-                                    merged_type['properties'][prop] = merge_structures(merged_type['properties'][prop],copy.deepcopy(json_schema['properties'][prop]))
-                                else:
-                                    merged_type['properties'][prop] = json_schema['properties'][prop]
-                        else:
-                            merged_type['properties'] = json_schema['properties']
-                    if 'enum' in json_schema:
-                        if 'enum' in merged_type:
-                            merged_type['enum'] = list(set(merged_type['enum']).union(set(json_schema['enum'])))
-                        else:
-                            merged_type['enum'] = json_schema['enum']
-                    if 'format' in json_schema:
-                        if 'format' in merged_type:
-                            merged_type['format'] = merged_type['format'] + json_schema['format']
+                    if isinstance(schema1[key], list):
+                        if schema2[key] not in schema1[key]:
+                            schema1[key].append(schema2[key])
+                    else:
+                        schema1[key] = [schema1[key], schema2[key]]
+            return schema1
+
+        merged_type: dict = {}
+
+        for json_schema in json_schemas:
+            if 'type' not in json_schema or 'type' not in merged_type:
+                for key in json_schema:
+                    if not key in merged_type:
+                        merged_type[key] = copy.deepcopy(json_schema[key])
+                    else:
+                        if key == 'required':
+                            merged_type[key] = list(
+                                set(merged_type[key]).union(set(json_schema[key])))
+                        if key == 'name' or key == 'title' or key == 'description':
+                            merged_type[key] = merged_type[key] + \
+                                json_schema[key]
+                        elif isinstance(merged_type[key], dict):
+                            merged_type[key] = merge_structures(
+                                merged_type[key], copy.deepcopy(json_schema[key]))
+                        elif isinstance(merged_type[key], list) and isinstance(json_schema[key], list):
+                            for item in json_schema[key]:
+                                if item not in merged_type[key]:
+                                    merged_type[key].append(item)
                         else:
-                            merged_type['format'] = json_schema['format']
+                            if merged_type[key] is None:
+                                merged_type[key] = json_schema[key]
+                            else:
+                                merged_type[key] = [merged_type[key],
+                                                    copy.deepcopy(json_schema[key])]
+            else:
+                if 'type' in merged_type and json_schema['type'] != merged_type['type']:
+                    if isinstance(merged_type['type'], str):
+                        merged_type['type'] = [merged_type['type']]
+                    merged_type['type'].append(json_schema['type'])
+                if 'required' in json_schema:
+                    if 'required' in merged_type:
+                        merged_type['required'] = list(
+                            set(merged_type['required']).union(set(json_schema['required'])))
+                    else:
+                        merged_type['required'] = json_schema['required']
+                if 'name' in json_schema:
+                    if 'name' in merged_type:
+                        merged_type['name'] = merged_type.get(
+                            'name', '') + json_schema['name']
+                    else:
+                        merged_type['name'] = json_schema['name']
+                if 'properties' in json_schema:
+                    if 'properties' in merged_type:
+                        for prop in json_schema['properties']:
+                            if prop in merged_type['properties']:
+                                merged_type['properties'][prop] = merge_structures(
+                                    merged_type['properties'][prop], copy.deepcopy(json_schema['properties'][prop]))
+                            else:
+                                merged_type['properties'][prop] = json_schema['properties'][prop]
+                    else:
+                        merged_type['properties'] = json_schema['properties']
+                if 'enum' in json_schema:
+                    if 'enum' in merged_type:
+                        merged_type['enum'] = list(
+                            set(merged_type['enum']).union(set(json_schema['enum'])))
+                    else:
+                        merged_type['enum'] = json_schema['enum']
+                if 'format' in json_schema:
+                    if 'format' in merged_type:
+                        merged_type['format'] = merged_type['format'] + \
+                            json_schema['format']
+                    else:
+                        merged_type['format'] = json_schema['format']
 
-            if intersect:
-                # only keep the intersection of the required fields
-                if 'required' in merged_type:
-                    new_required = merged_type['required']
-                    for json_schema in json_schemas:
-                        new_required = list(set(new_required).intersection(set(json_schema.get('required',[]))))
-                    merged_type['required'] = new_required
+        if intersect:
+            # only keep the intersection of the required fields
+            if 'required' in merged_type:
+                new_required = merged_type['required']
+                for json_schema in json_schemas:
+                    new_required = list(set(new_required).intersection(
+                        set(json_schema.get('required', []))))
+                merged_type['required'] = new_required
 
-            return merged_type
-        
+        return merged_type
 
     def ensure_type(self, type: dict | str | list) -> dict | str | list:
         """
         Ensures that the given type is valid by adding a 'type' field if it is missing.
-        
+
         Args:
             type (dict | str | list): The type to ensure.
-            
+
         Returns:
             dict | str | list: The ensured type.
         """
         if isinstance(type, str) or isinstance(type, list) or 'type' in type:
             return type
-        
+
         type['type'] = generic_type()
         return type
 
-
-    def json_schema_primitive_to_avro_type(self, json_primitive: str | list, format: str | None, enum: list | None, record_name: str, field_name: str, namespace: str, dependencies: list) -> str | dict[str,Any] | list:
+    def json_schema_primitive_to_avro_type(self, json_primitive: str | list, format: str | None, enum: list | None, record_name: str, field_name: str, namespace: str, dependencies: list) -> str | dict[str, Any] | list:
         """
         Convert a JSON-schema primitive type to Avro primitive type.
 
         Args:
             json_primitive (str | list): The JSON-schema primitive type to be converted.
             format (str | None): The format of the JSON primitive type, if applicable.
             enum (list | None): The list of enum values, if applicable.
@@ -342,21 +363,24 @@
 
         Returns:
             str | dict[str,Any] | list: The converted Avro primitive type.
 
         """
         if isinstance(json_primitive, list):
             if enum:
-                json_primitive = 'string' 
+                json_primitive = 'string'
             else:
                 union = []
                 for item in json_primitive:
-                    enum2 = item.get('enum') if isinstance(item, dict) else None
-                    format2 = item.get('format') if isinstance(item, dict) else None
-                    avro_primitive = self.json_schema_primitive_to_avro_type(item, format2, enum2, record_name, field_name, self.compose_namespace(namespace, record_name, field_name), dependencies)
+                    enum2 = item.get('enum') if isinstance(
+                        item, dict) else None
+                    format2 = item.get('format') if isinstance(
+                        item, dict) else None
+                    avro_primitive = self.json_schema_primitive_to_avro_type(
+                        item, format2, enum2, record_name, field_name, self.compose_namespace(namespace, record_name, field_name), dependencies)
                     union.append(avro_primitive)
                 return union
 
         if json_primitive == 'string':
             avro_primitive = 'string'
         elif json_primitive == 'integer':
             avro_primitive = 'int'
@@ -374,21 +398,21 @@
         # if you've got { 'type': 'string', 'format': ['date-time', 'duration'] }, I'm sorry
         if format and isinstance(format, str):
             if format in ('date-time', 'date'):
                 avro_primitive = {'type': 'int', 'logicalType': 'date'}
             elif format in ('time'):
                 avro_primitive = {'type': 'int', 'logicalType': 'time-millis'}
             elif format in ('duration'):
-                avro_primitive = {'type': 'fixed', 'size': 12, 'logicalType': 'duration'}
+                avro_primitive = {'type': 'fixed',
+                                  'size': 12, 'logicalType': 'duration'}
             elif format in ('uuid'):
                 avro_primitive = {'type': 'string', 'logicalType': 'uuid'}
-        
+
         return avro_primitive
 
-    
     def fetch_content(self, url: str | ParseResult):
         """
         Fetches the content from the specified URL.
 
         Args:
             url (str or ParseResult): The URL to fetch the content from.
 
@@ -408,41 +432,36 @@
 
         if parsed_url.geturl() in self.content_cache:
             return self.content_cache[parsed_url.geturl()]
         scheme = parsed_url.scheme
 
         # Handle HTTP and HTTPS URLs
         if scheme in ['http', 'https']:
-            try:
-                response = requests.get(url if isinstance(url, str) else parsed_url.geturl())
-                response.raise_for_status()  # Raises an HTTPError if the response status code is 4XX/5XX
-                self.content_cache[parsed_url.geturl()] = response.text
-                return response.text
-            except requests.RequestException as e:
-                raise Exception(f'Error fetching {url}: {e}')
+            response = requests.get(url if isinstance(
+                url, str) else parsed_url.geturl(), timeout=30)
+            # Raises an HTTPError if the response status code is 4XX/5XX
+            response.raise_for_status()
+            self.content_cache[parsed_url.geturl()] = response.text
+            return response.text
 
         # Handle file URLs
         elif scheme == 'file':
             # Remove the leading 'file://' from the path for compatibility
             file_path = parsed_url.netloc
             if not file_path:
                 file_path = parsed_url.path
             # On Windows, a file URL might start with a '/' but it's not part of the actual path
             if os.name == 'nt' and file_path.startswith('/'):
                 file_path = file_path[1:]
-            try:
-               with open(file_path, 'r', encoding='utf-8') as file:
-                    text = file.read()
-                    self.content_cache[parsed_url.geturl()] = text
-                    return text
-            except Exception as e:
-                raise Exception(f'Error reading file at {file_path}: {e}')
-
+            with open(file_path, 'r', encoding='utf-8') as file:
+                text = file.read()
+                self.content_cache[parsed_url.geturl()] = text
+                return text
         else:
-            raise Exception(f'Unsupported URL scheme: {scheme}')
+            raise NotImplementedError(f'Unsupported URL scheme: {scheme}')
 
     def resolve_reference(self, json_type: dict, base_uri: str, json_doc: dict) -> Tuple[dict, dict]:
         """
         Resolve a JSON Pointer reference or a JSON $ref reference.
 
         Args:
             json_type (dict): The JSON type containing the reference.
@@ -467,45 +486,49 @@
                 file_uri = self.compose_uri(base_uri, url)
                 content = self.fetch_content(file_uri)
             if content:
                 try:
                     json_schema_doc = json_schema = json.loads(content)
                     # resolve the JSON Pointer reference, if any
                     if url.fragment:
-                        json_schema = jsonpointer.resolve_pointer(json_schema, url.fragment)
+                        json_schema = jsonpointer.resolve_pointer(
+                            json_schema, url.fragment)
                     return json_schema, json_schema_doc
                 except json.JSONDecodeError:
                     raise Exception(f'Error decoding JSON from {ref}')
-            
+
             if url.fragment:
                 json_pointer = unquote(url.fragment)
-                ref_schema = jsonpointer.resolve_pointer(json_doc, json_pointer)
+                ref_schema = jsonpointer.resolve_pointer(
+                    json_doc, json_pointer)
                 if ref_schema:
                     return ref_schema, json_doc
         except JsonPointerException as e:
-            raise Exception(f'Error resolving JSON Pointer reference for {base_uri}')
+            raise Exception(
+                f'Error resolving JSON Pointer reference for {base_uri}')
         return json_type, json_doc
 
     def compose_uri(self, base_uri, url):
         if isinstance(url, str):
             url = urlparse(url)
             if url.scheme:
                 return url.geturl()
         if not url.path and not url.netloc:
             return base_uri
         if base_uri.startswith('file'):
             parsed_file_uri = urlparse(base_uri)
-            dir = os.path.dirname(parsed_file_uri.netloc if parsed_file_uri.netloc else parsed_file_uri.path)
+            dir = os.path.dirname(
+                parsed_file_uri.netloc if parsed_file_uri.netloc else parsed_file_uri.path)
             filename = os.path.join(dir, url.path)
             file_uri = f'file://{filename}'
         else:
             # combine the base URI with the URL
             file_uri = urllib.parse.urljoin(base_uri, url.geturl())
-        return file_uri           
-    
+        return file_uri
+
     def get_field_type_name(self, field: dict) -> str:
         if isinstance(field['type'], str):
             return field['type']
         elif isinstance(field['type'], list):
             names = []
             for field_type in field['type']:
                 if isinstance(field_type, str):
@@ -514,34 +537,34 @@
                     names.append(self.get_field_type_name(field_type))
                 else:
                     names.append('union')
             return ', '.join(names)
         elif isinstance(field['type'], dict) and 'type' in field['type']:
             return field['type']['type']
         return 'union'
-            
 
-    def json_type_to_avro_type(self, json_type: str | dict, record_name: str, field_name: str, namespace : str, dependencies: list, json_schema: dict, base_uri: str, avro_schema: list, record_stack: list, recursion_depth = 1) -> dict | list | str:
+    def json_type_to_avro_type(self, json_type: str | dict, record_name: str, field_name: str, namespace: str, dependencies: list, json_schema: dict, base_uri: str, avro_schema: list, record_stack: list, recursion_depth=1) -> dict | list | str:
         """Convert a JSON type to Avro type."""
 
         try:
             if recursion_depth >= self.max_recursion_depth:
-                print(f'WARNING: Maximum recursion depth reached for {record_name} at field {field_name}')
+                print(
+                    f'WARNING: Maximum recursion depth reached for {record_name} at field {field_name}')
                 return generic_type()
-            
+
             avro_type: list | dict | str = {}
             local_name = avro_name(field_name if field_name else record_name)
             hasAnyOf = isinstance(json_type, dict) and 'anyOf' in json_type
 
             if isinstance(json_type, dict):
 
                 json_object_type = json_type.get('type')
                 if isinstance(json_object_type, list):
                     # if the 'type' is a list, we map it back to a string
-                    # if the list has only one item or if the list has two items 
+                    # if the list has only one item or if the list has two items
                     # and one of them is 'null'
                     # otherwise, we will construct and inject a oneOf type
                     # and split the type
                     if len(json_object_type) == 1:
                         json_object_type = json_object_type[0]
                     elif len(json_object_type) == 2 and 'null' in json_object_type:
                         if json_object_type[0] == 'null':
@@ -553,19 +576,19 @@
                         for option in json_object_type:
                             if not option == 'null':
                                 oneof.append({
                                     'type': option
                                 })
                         if len(oneof) > 0:
                             del json_type['type']
-                            json_type['oneOf'] = oneof                  
-                        
+                            json_type['oneOf'] = oneof
 
                 if 'if' in json_type or 'then' in json_type or 'else' in json_type or 'dependentSchemas' in json_type or 'dependentRequired' in json_type:
-                    print('WARNING: Conditional schema is not supported and will be ignored.')
+                    print(
+                        'WARNING: Conditional schema is not supported and will be ignored.')
                     if 'if' in json_type:
                         del json_type['if']
                     if 'then' in json_type:
                         del json_type['then']
                     if 'else' in json_type:
                         del json_type['else']
                     if 'dependentSchemas' in json_type:
@@ -576,27 +599,30 @@
                 base_type = json_type.copy()
                 if 'oneOf' in base_type:
                     del base_type['oneOf']
                 if 'anyOf' in base_type:
                     del base_type['anyOf']
                 if 'allOf' in base_type:
                     del base_type['allOf']
-                json_types = []            
+                json_types = []
 
                 if 'allOf' in json_type:
                     # if the json type is an allOf, we merge all types into one
                     # this may be lossy if aspects of the types overlap but differ
                     type_list = [copy.deepcopy(base_type)]
                     for allof_option in json_type['allOf']:
                         while isinstance(allof_option, dict) and '$ref' in allof_option:
-                            resolved_json_type, resolved_schema = self.resolve_reference(allof_option, base_uri, json_schema)
+                            resolved_json_type, resolved_schema = self.resolve_reference(
+                                allof_option, base_uri, json_schema)
                             del allof_option['$ref']
-                            allof_option = self.merge_json_schemas([allof_option, resolved_json_type])
+                            allof_option = self.merge_json_schemas(
+                                [allof_option, resolved_json_type])
                         type_list.append(copy.deepcopy(allof_option))
-                    merged_type = self.merge_json_schemas(type_list, intersect=False)
+                    merged_type = self.merge_json_schemas(
+                        type_list, intersect=False)
                     json_types.append(merged_type)
 
                 if 'oneOf' in json_type:
                     # if the json type is a oneOf, we create a type union of all types
                     if len(json_types) == 0:
                         type_to_process = copy.deepcopy(base_type)
                     else:
@@ -605,96 +631,113 @@
                     oneof = json_type['oneOf']
                     if len(json_types) == 0:
                         for oneof_option in oneof:
                             if isinstance(oneof_option, dict) and 'type' in oneof_option and 'type' in type_to_process and not type_to_process.get('type') == oneof_option.get('type'):
                                 # we can't merge these due to conflicting types, so we pass the option-type on as-is
                                 json_types.append(oneof_option)
                             else:
-                                json_types.append(self.merge_json_schemas([type_to_process, oneof_option], intersect=True))  
+                                json_types.append(self.merge_json_schemas(
+                                    [type_to_process, oneof_option], intersect=True))
                     else:
                         new_json_types = []
                         for oneof_option in oneof:
                             for json_type_option in json_types:
-                                json_type_option = self.merge_json_schemas([json_type_option, oneof_option], intersect=True)
+                                json_type_option = self.merge_json_schemas(
+                                    [json_type_option, oneof_option], intersect=True)
                                 new_json_types.append(json_type_option)
                         json_types = new_json_types
-                
+
                 if 'anyOf' in json_type:
-                    types_to_process = json_types.copy() if len(json_types) > 0 else [copy.deepcopy(base_type)]
+                    types_to_process = json_types.copy() if len(json_types) > 0 else [
+                        copy.deepcopy(base_type)]
                     json_types = []
                     for type_to_process in types_to_process:
                         type_list = [copy.deepcopy(type_to_process)]
-                        # anyOf is a list of types where any number from 1 to all 
+                        # anyOf is a list of types where any number from 1 to all
                         # may match the data. Trouble with anyOf is that it doesn't
                         # really have a semantic interpretation in the context of Avro.
                         for anyof_option in json_type['anyOf']:
                             if isinstance(anyof_option, dict) and '$ref' in anyof_option:
                                 # if we have a ref, we can't merge into the base type, so we pass it on as-is.
                                 # into the JSON type list
                                 json_types.append(copy.deepcopy(anyof_option))
                             else:
                                 type_list.append(copy.deepcopy(anyof_option))
-                        merged_type = self.merge_json_schemas(type_list, intersect=False)
+                        merged_type = self.merge_json_schemas(
+                            type_list, intersect=False)
                         json_types.append(merged_type)
 
                 if len(json_types) > 0:
                     if len(json_types) == 1:
-                        avro_type = self.json_type_to_avro_type(json_types[0], record_name, field_name, namespace, dependencies, json_schema, base_uri, avro_schema, record_stack, recursion_depth + 1)
+                        avro_type = self.json_type_to_avro_type(
+                            json_types[0], record_name, field_name, namespace, dependencies, json_schema, base_uri, avro_schema, record_stack, recursion_depth + 1)
                         if isinstance(avro_type, dict) and self.is_empty_type(avro_type) and not 'allOf' in json_type:
                             avro_type['type'] = generic_type()
-                        avro_type = self.post_check_avro_type(dependencies, avro_type)
+                        avro_type = self.post_check_avro_type(
+                            dependencies, avro_type)
                         return avro_type
                     else:
-                        try:    
-                            record_stack.append(field_name if field_name else record_name)
+                        try:
+                            record_stack.append(
+                                field_name if field_name else record_name)
                             subtypes = []
                             count = 1
                             type_deps: List[str] = []
-                            for json_type_option in json_types:                                
+                            for json_type_option in json_types:
                                 if isinstance(json_type_option, dict) and '$ref' in json_type_option:
                                     ref = json_type_option['$ref']
                                     if ref in self.imported_types:
                                         avro_subtype = self.imported_types[ref]
                                         subtypes.append(avro_subtype)
                                         type_deps.append(avro_subtype)
                                         continue
 
                                 subtype_deps: List[str] = []
-                                sub_field_name = avro_name(local_name + '_' + str(count)) if not isinstance(json_type_option, dict) or not '$ref' in json_type_option else None
-                                avro_subtype = self.json_type_to_avro_type(json_type_option, record_name, sub_field_name, namespace, subtype_deps, json_schema, base_uri, avro_schema, record_stack, recursion_depth + 1)
+                                sub_field_name = avro_name(local_name + '_' + str(count)) if not isinstance(
+                                    json_type_option, dict) or not '$ref' in json_type_option else None
+                                avro_subtype = self.json_type_to_avro_type(
+                                    json_type_option, record_name, sub_field_name, namespace, subtype_deps, json_schema, base_uri, avro_schema, record_stack, recursion_depth + 1)
                                 if not avro_subtype:
                                     continue
                                 if isinstance(avro_subtype, dict) and 'name' in avro_subtype and 'type' in avro_subtype and (avro_subtype['type'] == 'record' or avro_subtype['type'] == 'enum'):
                                     # we have a standalone record or enum so we need to add it to the schema at the top-level
                                     # and reference it as a dependency from the parent type if it's not already been added.
-                                    existing_type = next((t for t in avro_schema if t.get('name') == avro_subtype['name'] and t.get('namespace') == avro_subtype.get('namespace') ), None)
+                                    existing_type = next((t for t in avro_schema if t.get('name') == avro_subtype['name'] and t.get(
+                                        'namespace') == avro_subtype.get('namespace')), None)
                                     if not existing_type:
                                         if subtype_deps:
                                             if not 'dependencies' in avro_subtype:
                                                 avro_subtype['dependencies'] = subtype_deps
                                             else:
-                                                avro_subtype['dependencies'].extend(subtype_deps)                                    
+                                                avro_subtype['dependencies'].extend(
+                                                    subtype_deps)
                                         if self.is_empty_type(avro_subtype):
-                                            print(f'WARN: Standalone type {avro_subtype["name"]} is empty')
+                                            print(
+                                                f'WARN: Standalone type {avro_subtype["name"]} is empty')
                                         if avro_subtype['type'] != 'enum' and avro_subtype['type'] != 'record' and avro_subtype['type'] != 'fixed':
-                                            raise ValueError(f'WARN: Standalone type {avro_subtype["name"]} is not a record or enum or fixed type')
+                                            raise ValueError(
+                                                f'WARN: Standalone type {avro_subtype["name"]} is not a record or enum or fixed type')
                                         avro_schema.append(avro_subtype)
-                                    full_name = self.get_qualified_name(avro_subtype)
+                                    full_name = self.get_qualified_name(
+                                        avro_subtype)
                                     subtype_deps = [full_name]
                                     avro_subtype = full_name
                                 if isinstance(avro_subtype, dict) and 'dependencies' in avro_subtype:
-                                    subtype_deps.extend(avro_subtype['dependencies'])
+                                    subtype_deps.extend(
+                                        avro_subtype['dependencies'])
                                     del avro_subtype['dependencies']
                                 if len(subtype_deps) > 0:
                                     type_deps.extend(subtype_deps)
                                 if not self.is_empty_type(avro_subtype):
                                     if isinstance(avro_subtype, list):
-                                        subtypes.extend(copy.deepcopy(avro_subtype))
+                                        subtypes.extend(
+                                            copy.deepcopy(avro_subtype))
                                     else:
-                                        subtypes.append(copy.deepcopy(avro_subtype))
+                                        subtypes.append(
+                                            copy.deepcopy(avro_subtype))
                                 count += 1
                             if len(type_deps) > 0:
                                 dependencies.extend(type_deps)
                             if len(subtypes) == 1:
                                 return self.post_check_avro_type(dependencies, subtypes[0])
                         finally:
                             record_stack.pop()
@@ -702,20 +745,20 @@
                         if hasAnyOf:
                             # if all subtypes are strings, they are either primitive types or type references
                             # which means there's nothing to merge, so we'll return the list of types
                             if all([isinstance(st, str) for st in subtypes]):
                                 return self.post_check_avro_type(dependencies, subtypes)
 
                             # we now has a list of types that may match the data, but this would be
-                            # an Avro union which is mutually exclusive. We will merge this list 
+                            # an Avro union which is mutually exclusive. We will merge this list
                             # into a record type in postprocessing when all types are available
                             if not isinstance(avro_type, dict):
                                 avro_type = {}
                             avro_type['unmerged_types'] = subtypes
-                            avro_type['type'] = 'record'                 
+                            avro_type['type'] = 'record'
                             avro_type['name'] = avro_name(local_name)
                             avro_type['namespace'] = namespace
                             avro_type['fields'] = []
                             if 'description' in json_type:
                                 avro_type['doc'] = json_type['description']
                             json_type = {}
                         else:
@@ -724,401 +767,455 @@
                 if 'properties' in json_type and not 'type' in json_type:
                     json_type['type'] = 'object'
 
                 if 'description' in json_type and isinstance(avro_type, dict):
                     avro_type['doc'] = json_type['description']
 
                 if 'title' in json_type and isinstance(avro_type, dict):
-                    self.set_avro_type_value(avro_type, 'name', avro_name(json_type['title']))
+                    self.set_avro_type_value(
+                        avro_type, 'name', avro_name(json_type['title']))
 
                 # first, pull in any referenced definitions and merge with this schema
                 if '$ref' in json_type:
                     # the $ref can indeed be a list as a result from a prior allOf/anyOf merge
-                    # if that is so, we will copy the type and process each $ref separately 
+                    # if that is so, we will copy the type and process each $ref separately
                     # and return the result as a list of types
                     if isinstance(json_type['$ref'], list):
                         types = []
                         for ref in json_type['$ref']:
                             json_type_copy = copy.deepcopy(json_type)
                             json_type_copy['$ref'] = ref
-                            types.append(self.json_type_to_avro_type(json_type_copy, record_name, field_name, namespace, dependencies, json_schema, base_uri, avro_schema, record_stack, recursion_depth + 1))
+                            types.append(self.json_type_to_avro_type(json_type_copy, record_name, field_name, namespace,
+                                         dependencies, json_schema, base_uri, avro_schema, record_stack, recursion_depth + 1))
                         return self.post_check_avro_type(dependencies, types)
 
                     ref = json_type['$ref']
                     if ref in self.imported_types:
                         # reference was already resolved, so we can resolve the reference simply by returning the type
                         type_ref = copy.deepcopy(self.imported_types[ref])
                         if isinstance(type_ref, str):
                             dependencies.append(type_ref)
                         return self.post_check_avro_type(dependencies, type_ref)
                     else:
-                        new_base_uri = self.compose_uri(base_uri, json_type['$ref'])
-                        resolved_json_type, resolved_schema = self.resolve_reference(json_type, base_uri, json_schema)
-                        if self.is_empty_json_type(json_type): 
-                            # it's a standalone reference, so will import the type into the schema 
+                        new_base_uri = self.compose_uri(
+                            base_uri, json_type['$ref'])
+                        resolved_json_type, resolved_schema = self.resolve_reference(
+                            json_type, base_uri, json_schema)
+                        if self.is_empty_json_type(json_type):
+                            # it's a standalone reference, so will import the type into the schema
                             # and reference it like it was in the same file
                             type_name = record_name
                             type_namespace = namespace
                             parsed_ref = urlparse(ref)
                             if parsed_ref.fragment:
-                                type_name = avro_name(parsed_ref.fragment.split('/')[-1])
-                                sub_namespace = self.compose_namespace(*parsed_ref.fragment.split('/')[2:-1])
-                                type_namespace = self.compose_namespace(self.root_namespace, sub_namespace)
-                            
+                                type_name = avro_name(
+                                    parsed_ref.fragment.split('/')[-1])
+                                sub_namespace = self.compose_namespace(
+                                    *parsed_ref.fragment.split('/')[2:-1])
+                                type_namespace = self.compose_namespace(
+                                    self.root_namespace, sub_namespace)
+
                             # registering in imported_types ahead of resolving to prevent circular references.
                             # we only cache the type if it's forseeable that it is usable as a standalone type
                             # which means that it must be either a record or an enum or a fixed type when converted
                             # to Avro. That means we look for the presence of 'type', 'properties', 'allOf', 'anyOf',
                             # and 'enum' in the resolved type.
-                            if resolved_json_type and (('type' in resolved_json_type and resolved_json_type['type'] == 'object') or 'properties' in resolved_json_type or 'enum' in resolved_json_type or \
-                                                    'allOf' in resolved_json_type or 'anyOf' in resolved_json_type):
-                                self.imported_types[ref] = self.compose_namespace(type_namespace, type_name)
+                            if resolved_json_type and (('type' in resolved_json_type and resolved_json_type['type'] == 'object') or 'properties' in resolved_json_type or 'enum' in resolved_json_type or
+                                                       'allOf' in resolved_json_type or 'anyOf' in resolved_json_type):
+                                self.imported_types[ref] = self.compose_namespace(
+                                    type_namespace, type_name)
                             # resolve type
                             deps: List[str] = []
-                            resolved_avro_type: dict | list | str | None = self.json_type_to_avro_type(resolved_json_type, type_name, '', type_namespace, deps, resolved_schema, new_base_uri, avro_schema, [], recursion_depth + 1)
+                            resolved_avro_type: dict | list | str | None = self.json_type_to_avro_type(
+                                resolved_json_type, type_name, '', type_namespace, deps, resolved_schema, new_base_uri, avro_schema, [], recursion_depth + 1)
                             if isinstance(resolved_avro_type, str):
                                 dependencies.extend(deps)
                                 return self.post_check_avro_type(dependencies, resolved_avro_type)
                             if isinstance(resolved_avro_type, list) or (not isinstance(resolved_avro_type, dict) or (not resolved_avro_type.get('type') == 'record' and not resolved_avro_type.get('type') == 'enum')):
                                 if isinstance(resolved_avro_type, dict) and not 'type' in resolved_avro_type:
                                     if isinstance(avro_type, dict):
-                                        # the resolved type didn't have a type and avro_type is a dict, 
+                                        # the resolved type didn't have a type and avro_type is a dict,
                                         # so we assume it's a mixin into the type we found
                                         avro_type.update(resolved_avro_type)
                                         resolved_avro_type = None
                                     else:
-                                        # no 'type' definition for this field and we can't mix into the avro type, 
+                                        # no 'type' definition for this field and we can't mix into the avro type,
                                         # so we fallback to a generic type
-                                        print(f"WARNING: no 'type' definition for {ref} in record {record_name}: {json.dumps(resolved_avro_type)}")
+                                        print(
+                                            f"WARNING: no 'type' definition for {ref} in record {record_name}: {json.dumps(resolved_avro_type)}")
                                         resolved_avro_type = generic_type()
-                                elif isinstance(avro_type,str) and resolved_avro_type:
+                                elif isinstance(avro_type, str) and resolved_avro_type:
                                     # this is a plain type reference
                                     avro_type = resolved_avro_type
                                     self.imported_types[ref] = avro_type
-                                    resolved_avro_type = None                        
+                                    resolved_avro_type = None
                                 if resolved_avro_type:
                                     # this is not a record type that can stand on its own,
-                                    # so we remove the cached type entry 
+                                    # so we remove the cached type entry
                                     # and pass it on as an inline type
                                     dependencies.extend(deps)
                                     if ref in self.imported_types:
                                         del self.imported_types[ref]
-                                    avro_type = self.merge_avro_schemas([avro_type, resolved_avro_type], avro_schema, local_name)
+                                    avro_type = self.merge_avro_schemas(
+                                        [avro_type, resolved_avro_type], avro_schema, local_name)
                                     if isinstance(avro_type, dict) and 'name' in avro_type and not self.is_standalone_avro_type(avro_type):
-                                        del avro_type['name']                                        
+                                        del avro_type['name']
                                         return self.post_check_avro_type(dependencies, avro_type)
                             else:
                                 avro_type = resolved_avro_type
-                                self.imported_types[ref] = copy.deepcopy(avro_type)
+                                self.imported_types[ref] = copy.deepcopy(
+                                    avro_type)
 
                             if len(deps) > 0:
                                 if isinstance(avro_type, dict):
                                     avro_type['dependencies'] = deps
                                 else:
                                     dependencies.extend(deps)
-                            
+
                             if self.is_standalone_avro_type(avro_type):
                                 self.register_type(avro_schema, avro_type)
                                 full_name = self.get_qualified_name(avro_type)
                                 if ref in self.imported_types:
                                     # update the import reference to the resolved type if it's cached
                                     self.imported_types[ref] = full_name
                                 dependencies.append(full_name)
-                                avro_type = full_name                    
+                                avro_type = full_name
                         else:
                             del json_type['$ref']
                             # it's a reference within a definition, so we will turn this into an inline type
                             if isinstance(resolved_json_type, dict) and 'type' in resolved_json_type and json_type.get('type') and not json_type['type'] == resolved_json_type['type']:
                                 # the types conflict, so we can't merge them
-                                type1 = self.json_type_to_avro_type(json_type, record_name, field_name, namespace, dependencies, resolved_schema, new_base_uri, avro_schema, record_stack, recursion_depth + 1)
-                                type2 = self.json_type_to_avro_type(resolved_json_type, record_name, field_name, namespace, dependencies, resolved_schema, new_base_uri, avro_schema, record_stack, recursion_depth + 1)
+                                type1 = self.json_type_to_avro_type(
+                                    json_type, record_name, field_name, namespace, dependencies, resolved_schema, new_base_uri, avro_schema, record_stack, recursion_depth + 1)
+                                type2 = self.json_type_to_avro_type(resolved_json_type, record_name, field_name, namespace,
+                                                                    dependencies, resolved_schema, new_base_uri, avro_schema, record_stack, recursion_depth + 1)
                                 # if either of the types are empty, use just the other one
                                 if not self.is_empty_type(type1) and not self.is_empty_type(type2):
                                     return self.flatten_union([type1, type2])
                                 if not self.is_empty_type(type1):
                                     avro_type = type1
                                     if isinstance(avro_type, list):
                                         return self.post_check_avro_type(dependencies, avro_type)
                                 if not self.is_empty_type(type2):
-                                    avro_type = type2   
+                                    avro_type = type2
                                     if isinstance(avro_type, list):
                                         return self.post_check_avro_type(dependencies, avro_type)
                                 json_type = {}
                             else:
-                                json_type = self.merge_json_schemas([json_type, resolved_json_type])
-                                avro_type = self.json_type_to_avro_type(json_type, record_name, field_name, namespace, dependencies, resolved_schema, new_base_uri, avro_schema, record_stack, recursion_depth + 1)
+                                json_type = self.merge_json_schemas(
+                                    [json_type, resolved_json_type])
+                                avro_type = self.json_type_to_avro_type(
+                                    json_type, record_name, field_name, namespace, dependencies, resolved_schema, new_base_uri, avro_schema, record_stack, recursion_depth + 1)
                                 json_type = {}
                             if ref in self.imported_types:
                                 # update the import reference to the resolved type if it's cached
                                 if isinstance(avro_type, dict) and 'name' in avro_type:
                                     self.imported_types[ref] = avro_type['name']
                                 else:
                                     self.imported_types[ref] = avro_type
-                            
+
                 # if 'const' is present, make this an enum
                 if 'const' in json_type:
-                    const_list = json_type['const'] if isinstance(json_type['const'], list) else [json_type['const']]
-                    avro_type = self.merge_avro_schemas([avro_type, self.create_enum_type(local_name, namespace, const_list)], avro_schema, local_name)
+                    const_list = json_type['const'] if isinstance(
+                        json_type['const'], list) else [json_type['const']]
+                    avro_type = self.merge_avro_schemas([avro_type, self.create_enum_type(
+                        local_name, namespace, const_list)], avro_schema, local_name)
                 if json_object_type or 'enum' in json_type:
                     if json_object_type == 'array':
                         if isinstance(json_type, dict) and 'items' in json_type:
                             deps = []
-                            item_type = self.json_type_to_avro_type(json_type['items'], record_name, field_name, namespace, deps, json_schema, base_uri, avro_schema, record_stack, recursion_depth + 1)
+                            item_type = self.json_type_to_avro_type(
+                                json_type['items'], record_name, field_name, namespace, deps, json_schema, base_uri, avro_schema, record_stack, recursion_depth + 1)
                             if self.is_standalone_avro_type(item_type):
                                 if isinstance(item_type, dict) and len(deps) > 0:
                                     item_type['dependencies'] = deps
                                 self.register_type(avro_schema, item_type)
-                                dependencies.append(self.get_qualified_name(item_type))
+                                dependencies.append(
+                                    self.get_qualified_name(item_type))
                             else:
                                 dependencies.extend(deps)
                                 if isinstance(item_type, dict) and not 'type' in item_type:
                                     item_type = generic_type()
                                 elif isinstance(item_type, str) and not item_type in primitive_types:
                                     dependencies.append(item_type)
                                 else:  # not a standalone type, but has a type definition, so we unwind that here
-                                    item_type = self.post_check_avro_type(dependencies, item_type)
-                            avro_type = self.merge_avro_schemas([avro_type, self.create_array_type(item_type)], avro_schema, '')
+                                    item_type = self.post_check_avro_type(
+                                        dependencies, item_type)
+                            avro_type = self.merge_avro_schemas(
+                                [avro_type, self.create_array_type(item_type)], avro_schema, '')
                         else:
-                            avro_type = self.merge_avro_schemas([avro_type, self.create_array_type(generic_type())], avro_schema, '')
+                            avro_type = self.merge_avro_schemas(
+                                [avro_type, self.create_array_type(generic_type())], avro_schema, '')
                     elif json_object_type and (json_object_type == 'object' or 'object' in json_object_type):
-                        avro_record_type = self.json_schema_object_to_avro_record(local_name, json_type, namespace, json_schema, base_uri, avro_schema, record_stack)
+                        avro_record_type = self.json_schema_object_to_avro_record(
+                            local_name, json_type, namespace, json_schema, base_uri, avro_schema, record_stack)
                         if isinstance(avro_record_type, list):
                             for record_entry in avro_record_type:
-                                self.lift_dependencies_from_type(record_entry, dependencies)
-                        avro_type = self.merge_avro_schemas([avro_type, avro_record_type], avro_schema, avro_type.get('name', local_name) if isinstance(avro_type,dict) else local_name)
-                        self.lift_dependencies_from_type(avro_type, dependencies)
+                                self.lift_dependencies_from_type(
+                                    record_entry, dependencies)
+                        avro_type = self.merge_avro_schemas([avro_type, avro_record_type], avro_schema, avro_type.get(
+                            'name', local_name) if isinstance(avro_type, dict) else local_name)
+                        self.lift_dependencies_from_type(
+                            avro_type, dependencies)
                     elif 'enum' in json_type and (not 'type' in json_type or json_type['type'] == "string"):
                         # we skip all enums that are not of implicit or explicit type 'string'
-                        enum = [avro_name(e) for e in json_type['enum'] if isinstance(e, str) and e != '']
-                        if len(enum) > 0: 
+                        enum = [avro_name(e) for e in json_type['enum'] if isinstance(
+                            e, str) and e != '']
+                        if len(enum) > 0:
                             # if the enum ends up empty (only non-strings in the enum), we will skip it
                             enum = list(set(enum))
                             if len(enum) > 0:
-                                avro_type = self.create_enum_type(local_name, self.compose_namespace(namespace, record_name + '_types'), enum)
+                                avro_type = self.create_enum_type(local_name, self.compose_namespace(
+                                    namespace, record_name + '_types'), enum)
                     else:
-                        avro_type = self.json_schema_primitive_to_avro_type(json_object_type, json_type.get('format'), json_type.get('enum'), record_name, field_name, namespace, dependencies)    
+                        avro_type = self.json_schema_primitive_to_avro_type(json_object_type, json_type.get(
+                            'format'), json_type.get('enum'), record_name, field_name, namespace, dependencies)
             else:
                 if isinstance(json_type, dict):
-                    avro_type = self.merge_avro_schemas([avro_type,self.json_schema_primitive_to_avro_type(json_type, json_type.get('format'), json_type.get('enum'), record_name, field_name, namespace, dependencies)], avro_schema, avro_type.get('name', local_name) if isinstance(avro_type,dict) else local_name)
+                    avro_type = self.merge_avro_schemas([avro_type, self.json_schema_primitive_to_avro_type(json_type, json_type.get('format'), json_type.get(
+                        'enum'), record_name, field_name, namespace, dependencies)], avro_schema, avro_type.get('name', local_name) if isinstance(avro_type, dict) else local_name)
                 else:
-                    avro_type = self.merge_avro_schemas([avro_type,self.json_schema_primitive_to_avro_type(json_type, None, None, record_name, field_name, namespace, dependencies)], avro_schema, avro_type.get('name', local_name) if isinstance(avro_type,dict) else local_name)
-            
+                    avro_type = self.merge_avro_schemas([avro_type, self.json_schema_primitive_to_avro_type(
+                        json_type, None, None, record_name, field_name, namespace, dependencies)], avro_schema, avro_type.get('name', local_name) if isinstance(avro_type, dict) else local_name)
+
             if isinstance(avro_type, dict) and 'name' in avro_type and 'type' in avro_type and not (avro_type['type'] in ['array', 'map']):
                 if not 'namespace' in avro_type:
                     avro_type['namespace'] = namespace
-                existing_type = next((t for t in avro_schema if t.get('name') == avro_type['name'] and t.get('namespace') == avro_type.get('namespace') ), None)
+                existing_type = next((t for t in avro_schema if t.get(
+                    'name') == avro_type['name'] and t.get('namespace') == avro_type.get('namespace')), None)
                 if existing_type:
                     existing_type_name = self.get_qualified_name(existing_type)
                     if not existing_type_name in dependencies:
                         dependencies.append(existing_type_name)
                     return existing_type_name
                 self.set_avro_type_value(avro_type, 'name', local_name)
-            
+
             # post-check on the avro type: if the type is a dict, and the 'type' is not
             # a record, enum, fixed, array, or map, we will just return the basic type
             # and push its dependencies up the stack
             avro_type = self.post_check_avro_type(dependencies, avro_type)
-                        
+
             if isinstance(avro_type, dict) and 'unmerged_types' in avro_type:
                 self.types_with_unmerged_types.append(avro_type)
-                
+
             return avro_type
         except RecursionError as e:
-            print(f"Recursion error while processing {namespace}:{record_name}:{field_name} with recursion depth {recursion_depth}")
+            print(
+                f"Recursion error while processing {namespace}:{record_name}:{field_name} with recursion depth {recursion_depth}")
             raise e
 
     def post_check_avro_type(self, dependencies, avro_type):
+        """Post-check the Avro type and push dependencies up the stack."""
         if isinstance(avro_type, dict) and 'type' in avro_type and (isinstance(avro_type, list) or not avro_type['type'] in ['array', 'map', 'record', 'enum', 'fixed']):
             if 'dependencies' in avro_type:
                 dependencies.extend(avro_type['dependencies'])
             avro_type = avro_type['type']
         return avro_type
 
     def register_type(self, avro_schema, avro_type) -> bool:
-        existing_type = next((t for t in avro_schema if t.get('name') == avro_type['name'] and t.get('namespace') == avro_type.get('namespace') ), None)
+        """Register a type in the Avro schema."""
+        existing_type = next((t for t in avro_schema if t.get(
+            'name') == avro_type['name'] and t.get('namespace') == avro_type.get('namespace')), None)
         if not existing_type:
             if self.is_empty_type(avro_type) and not 'unmerged_types' in avro_type:
                 print(f'WARN: Standalone type {avro_type["name"]} is empty')
             if self.is_standalone_avro_type(avro_type):
                 avro_schema.append(avro_type)
                 return True
             else:
                 return False
         else:
             return True
-    
+
     def has_composition_keywords(self, json_object: dict) -> bool:
-            """Check if the JSON object has any of the combining keywords: allOf, oneOf, anyOf."""
-            return isinstance(json_object, dict) and ('allOf' in json_object or 'oneOf' in json_object or 'anyOf' in json_object)
-    
+        """Check if the JSON object has any of the combining keywords: allOf, oneOf, anyOf."""
+        return isinstance(json_object, dict) and ('allOf' in json_object or 'oneOf' in json_object or 'anyOf' in json_object)
+
     def has_enum_keyword(self, json_object: dict) -> bool:
         """Check if the JSON object is an enum."""
         return isinstance(json_object, dict) and 'enum' in json_object
-    
+
     def is_array_object(self, json_object: dict) -> bool:
+        """Check if the JSON object is an array object."""
         return isinstance(json_object, dict) and 'type' in json_object and json_object['type'] == 'array'
-    
+
     def is_standalone_avro_type(self, avro_type: dict | list | str) -> bool:
+        """Check if the Avro type is a standalone type."""
         return isinstance(avro_type, dict) and 'type' in avro_type and (avro_type['type'] in ['record', 'enum', 'fixed'])
-    
+
     def is_avro_complex_type(self, avro_type: dict) -> bool:
-        return 'type' in avro_type and avro_type['type'] in ['record', 'enum', 'fixed', 'array', 'map'] 
+        """Check if the Avro type is a complex type."""
+        return 'type' in avro_type and avro_type['type'] in ['record', 'enum', 'fixed', 'array', 'map']
 
     def set_avro_type_value(self, avro_type: dict | list | str, name: str, value: dict | list | str):
+        """Set a value in an Avro type."""
         if isinstance(avro_type, dict):
             if name == 'namespace' or name == 'name':
                 if 'type' in avro_type:
                     if not (avro_type['type'] in ['record', 'enum', 'fixed']):
                         return
             avro_type[name] = value
-    
+
     def create_avro_record(self, name: str, namespace: str, fields: list) -> dict:
         """Create an Avro record type."""
         return {
-            'type': 'record', 
+            'type': 'record',
             'name': avro_name(name),
             'namespace': namespace,
             'fields': fields
         }
-    
+
     def create_wrapper_record(self, wrapper_name: str, wrapper_namespace: str, wrapper_field: str, dependencies: list, avro_type: list | str | dict) -> dict:
         """Create a union wrapper type in Avro."""
         rec = self.create_avro_record(wrapper_name, wrapper_namespace, [
-                    {
-                        'name': wrapper_field,
-                        'type': avro_type
-                    }
-                ])
+            {
+                'name': wrapper_field,
+                'type': avro_type
+            }
+        ])
         if len(dependencies) > 0:
             rec['dependencies'] = dependencies
-        return rec    
+        return rec
 
     def create_enum_type(self, name: str, namespace: str, symbols: list) -> dict:
         """Create an Avro enum type."""
         # the symbol list may have been merged by composition to we flatten it to have a unique list
         symbols = self.flatten_union(symbols)
         return {
-            'type': 'enum', 
-            'name': name, 
+            'type': 'enum',
+            'name': name,
             'namespace': namespace,
             'symbols': [avro_name(s) for s in symbols]
-        }        
-    
+        }
+
     def create_array_type(self, items: list | dict | str) -> dict:
         """Create an Avro array type."""
         return {
             'type': 'array',
             'items': items
         }
-    
+
     def create_map_type(self, values: list | dict | str) -> dict:
         """Create an Avro map type."""
         return {
             'type': 'map',
             'values': values
         }
-    
+
     def nullable(self, avro_type: list | dict | str) -> list | dict | str:
         """Wrap a type in a union with null."""
         if isinstance(avro_type, list):
             cp = avro_type.copy()
             cp.insert(0, 'null')
             return cp
         return ['null', avro_type]
-    
+
     def merge_description_into_doc(self, source_json: dict, target_avro: dict | list | str):
         """Merge a description in JSON into Avro doc."""
         if isinstance(source_json, dict) and 'description' in source_json and isinstance(target_avro, dict):
-            target_avro['doc'] = target_avro['doc'] + ", " + source_json['description'] if 'doc' in target_avro else source_json['description']
-        
-    
-    def merge_dependencies_into_parent(self, dependencies:list , child_type: dict | list | str, parent_type: dict | list | str):
+            target_avro['doc'] = target_avro['doc'] + ", " + \
+                source_json['description'] if 'doc' in target_avro else source_json['description']
+
+    def merge_dependencies_into_parent(self, dependencies: list, child_type: dict | list | str, parent_type: dict | list | str):
+        """Merge dependencies from a child type into a parent type."""
         self.lift_dependencies_from_type(child_type, dependencies)
         if len(dependencies) > 0 and isinstance(parent_type, dict):
             if 'dependencies' in parent_type:
                 dependencies.extend(parent_type['dependencies'])
             else:
                 parent_type['dependencies'] = dependencies
-    
+
     def lift_dependencies_from_type(self, child_type: dict | list | str, dependencies: list):
         """Lift all dependencies from a type and return a new type with the dependencies lifted."""
         if isinstance(child_type, dict):
             if 'dependencies' in child_type:
                 dependencies.extend(child_type['dependencies'])
                 del child_type['dependencies']
-        
+
     def compose_namespace(self, *names) -> str:
+        """Compose a namespace from a list of names."""
         return '.'.join([avro_namespace(n) for n in names if n])
-    
+
     def get_qualified_name(self, avro_type):
-        return self.compose_namespace(avro_type.get('namespace',''), avro_type.get('name', ''))
-        
+        """Get the qualified name of an Avro type."""
+        return self.compose_namespace(avro_type.get('namespace', ''), avro_type.get('name', ''))
+
     def json_schema_object_to_avro_record(self, name: str, json_object: dict, namespace: str, json_schema: dict, base_uri: str, avro_schema: list, record_stack: list) -> dict | list | str | None:
         """Convert a JSON schema object declaration to an Avro record."""
         dependencies: List[str] = []
         avro_type: list | dict | str = {}
-        
+
         # handle top-level allOf, anyOf, oneOf
         if self.has_composition_keywords(json_object):
             # we will merge allOf, oneOf, anyOf into a union record type
-            type = self.json_type_to_avro_type(json_object, name, '', namespace, dependencies, json_schema, base_uri, avro_schema, record_stack)
+            type = self.json_type_to_avro_type(
+                json_object, name, '', namespace, dependencies, json_schema, base_uri, avro_schema, record_stack)
             if isinstance(type, str):
                 # we are skipping references and primitives
                 return None
             if isinstance(type, list):
                 # we should have a union type
-                avro_type = self.create_wrapper_record(name+"_union", self.utility_namespace, 'options', [], type)
+                avro_type = self.create_wrapper_record(
+                    name+"_union", self.utility_namespace, 'options', [], type)
             elif isinstance(type, dict) and 'type' in type and type['type'] != 'record':
                 # merge the type into a record type if it's not a record type
-                print(f'INFO: Standalone type {name} is being wrapped in a record')
-                avro_type = self.create_wrapper_record(avro_name(type.get('name',name)+'_wrapper'), self.utility_namespace, 'value', type.get('dependencies', []), type)
+                print(
+                    f'INFO: Standalone type {name} is being wrapped in a record')
+                avro_type = self.create_wrapper_record(avro_name(type.get(
+                    'name', name)+'_wrapper'), self.utility_namespace, 'value', type.get('dependencies', []), type)
             else:
                 avro_type = type
-            # add external dependencies to the record    
+            # add external dependencies to the record
             self.merge_dependencies_into_parent(dependencies, type, avro_type)
             self.merge_description_into_doc(json_object, avro_type)
             # return the union type
-            return avro_type    
-        
+            return avro_type
+
         if self.has_enum_keyword(json_object):
             # this is an enum
-            avro_enum = self.create_enum_type(avro_name(name), namespace, json_object['enum'])
+            avro_enum = self.create_enum_type(
+                avro_name(name), namespace, json_object['enum'])
             self.merge_description_into_doc(json_object, avro_enum)
             return avro_enum
-        
+
         if self.is_array_object(json_object):
             # this is an array, which can't be standalone in Avro, so we will wraps it into a record
             # and include the type as an inline
-            print(f'WARN: Standalone array type {name} will be wrapped in a record')
-            deps: List[str] =[]
-            array_type = self.json_type_to_avro_type(json_object, name, avro_name(name), namespace, deps, json_schema, base_uri, avro_schema, record_stack)
-            avro_array = self.create_wrapper_record(avro_name(name+'_wrapper'), self.utility_namespace, 'items', [], array_type)
+            print(
+                f'WARN: Standalone array type {name} will be wrapped in a record')
+            deps: List[str] = []
+            array_type = self.json_type_to_avro_type(json_object, name, avro_name(
+                name), namespace, deps, json_schema, base_uri, avro_schema, record_stack)
+            avro_array = self.create_wrapper_record(
+                avro_name(name+'_wrapper'), self.utility_namespace, 'items', [], array_type)
             self.merge_description_into_doc(json_object, avro_array)
             self.merge_dependencies_into_parent(deps, array_type, avro_array)
-            return avro_array       
-        
-        
+            return avro_array
+
         # at this point, we have to assume that we have a JSON schema object
         title = json_object.get('title')
         record_name = avro_name(name if name else title if title else None)
-        if record_name == None:
-            raise ValueError(f"Cannot determine record name for json_object {json_object}")
+        if record_name is None:
+            raise ValueError(
+                f"Cannot determine record name for json_object {json_object}")
         if len(record_stack) > 0:
             # if we have a record stack, we need to add the current name to
             # the namespace since nested types are disambiguated by their namespace
-            namespace = self.compose_namespace(namespace, record_stack[-1] + "_types")
+            namespace = self.compose_namespace(
+                namespace, record_stack[-1] + "_types")
         # at this point we have a record type
         avro_record = self.create_avro_record(record_name, namespace, [])
-        # we need to prevent circular dependencies, so we will maintain a stack of the in-progress 
+        # we need to prevent circular dependencies, so we will maintain a stack of the in-progress
         # records and will resolve the cycle as we go. if this record is already in the stack, we will
         # just return a reference to a record that contains this record
         if record_name in record_stack:
-            # to break the cycle, we will use a containment type that references 
+            # to break the cycle, we will use a containment type that references
             # the record that is being defined
-            print(f'WARN: Circular dependency found for record {record_name}. Creating {record_name}_ref.')
+            print(
+                f'WARN: Circular dependency found for record {record_name}. Creating {record_name}_ref.')
             ref_name = avro_name(record_name + '_ref')
             return self.create_wrapper_record(ref_name, namespace, record_name, [], self.compose_namespace(namespace, record_name))
         try:
             # enter the record stack scope for this record
             record_stack.append(record_name)
             # collect the required fields so we can make those fields non-null
             required_fields = json_object.get('required', [])
@@ -1130,400 +1227,459 @@
                     if isinstance(json_field_types, bool):
                         # for "propertyname": true, we skip. schema bug.
                         continue
                     if not isinstance(json_field_types, list):
                         json_field_types = [json_field_types]
                     field_type_list = []
                     field_ref_type_list = []
+                    const = None
+                    default = None
+                    description = None
                     for json_field_type in json_field_types:
                         # skip fields with an bad or empty type
                         if not isinstance(json_field_type, dict):
                             continue
                         field_name = avro_name(field_name)
+                        # last const wins if there are multiple
+                        const = json_field_type.get('const', const)
+                        # last default wins if there are multiple
+                        default_value = json_field_type.get('default')
+                        if default_value and not isinstance(default_value, dict) and not isinstance(default_value, list):
+                            default = default_value
+                        # get the description from the field type
+                        description = json_field_type.get('description', description)
                         # convert the JSON-type field to an Avro-type field
-                        avro_field_ref_type = avro_field_type = self.ensure_type(self.json_type_to_avro_type(json_field_type, record_name, field_name, namespace, dependencies, json_schema, base_uri, avro_schema, record_stack))
+                        avro_field_ref_type = avro_field_type = self.ensure_type(self.json_type_to_avro_type(
+                            json_field_type, record_name, field_name, namespace, dependencies, json_schema, base_uri, avro_schema, record_stack))
                         if isinstance(avro_field_type, list):
-                            avro_field_type = self.flatten_union(avro_field_type)
+                            avro_field_type = self.flatten_union(
+                                avro_field_type)
                             avro_field_ref_type = avro_field_type
                         elif isinstance(avro_field_type, dict):
-                            self.lift_dependencies_from_type(avro_field_type, dependencies)
+                            self.lift_dependencies_from_type(
+                                avro_field_type, dependencies)
                             # if the first call gave us a global type that got added to the schema, this call will give us a reference
                             if self.is_standalone_avro_type(avro_field_type):
-                                avro_field_ref_type = self.get_qualified_name(avro_field_type)                        
+                                avro_field_ref_type = self.get_qualified_name(
+                                    avro_field_type)
                         if avro_field_type is None:
                             # None type is a problem
-                            raise ValueError(f"avro_field_type is None for field {field_name}")                    
-                        if isinstance(avro_field_type,dict) and 'type' in avro_field_type and not self.is_avro_complex_type(avro_field_type):
+                            raise ValueError(
+                                f"avro_field_type is None for field {field_name}")
+                        if isinstance(avro_field_type, dict) and 'type' in avro_field_type and not self.is_avro_complex_type(avro_field_type):
                             # if the field type is a basic type, inline it
-                            avro_field_type = avro_field_type['type']                                       
+                            avro_field_type = avro_field_type['type']
                         field_type_list.append(avro_field_type)
-                        field_ref_type_list.append(avro_field_ref_type)            
-                    
-                    effective_field_type = field_type_list[0] if len(field_type_list) == 1 else field_type_list
-                    effective_field_ref_type = field_ref_type_list[0] if len(field_ref_type_list) == 1 else field_ref_type_list                        
+                        field_ref_type_list.append(avro_field_ref_type)
+
+                    effective_field_type = field_type_list[0] if len(
+                        field_type_list) == 1 else field_type_list
+                    effective_field_ref_type = field_ref_type_list[0] if len(
+                        field_ref_type_list) == 1 else field_ref_type_list
                     avro_field = {
-                        'name': avro_name(field_name), 
-                        'type': self.nullable(effective_field_type) if not field_name in required_fields and not 'null' in effective_field_type else effective_field_type
+                        'name': avro_name(field_name),
+                        'type': self.nullable(effective_field_type) if not field_name in required_fields and 'null' not in effective_field_type else effective_field_type
                     }
-                    self.merge_description_into_doc(json_field_type, avro_field)
+                    if const:
+                        avro_field['const'] = const
+                    if default:
+                        avro_field['default'] = default
+                    if description:
+                        avro_field['doc'] = description
                     field_type_list.append(avro_field_type)
                     avro_field_ref = {
-                        'name': avro_name(field_name), 
-                        'type': self.nullable(effective_field_ref_type) if not field_name in required_fields and not 'null' in effective_field_ref_type else effective_field_ref_type
+                        'name': avro_name(field_name),
+                        'type': self.nullable(effective_field_ref_type) if not field_name in required_fields and 'null' not in effective_field_ref_type else effective_field_ref_type
                     }
-                    self.merge_description_into_doc(json_field_type, avro_field_ref)
+                    if description:
+                        avro_field_ref['doc'] = description
                     field_ref_type_list.append(avro_field_ref)
                     # add the field to the record
                     avro_record['fields'].append(avro_field)
                     field_refs.append(avro_field_ref)
             elif not 'additionalProperties' in json_object and not 'patternProperties' in json_object:
                 if 'type' in json_object and (json_object['type'] == 'object' or 'object' in json_object['type']) and \
-                    not 'allOf' in json_object and not 'oneOf' in json_object and not 'anyOf' in json_object:
+                        not 'allOf' in json_object and not 'oneOf' in json_object and not 'anyOf' in json_object:
                     # we don't have any fields, but we have an object type, so we create a map
                     avro_record = self.create_map_type(generic_type())
                 elif 'type' in json_object and (json_object['type'] == 'array' or 'array' in json_object['type']) and \
-                    not 'allOf' in json_object and not 'oneOf' in json_object and not 'anyOf' in json_object:
+                        not 'allOf' in json_object and not 'oneOf' in json_object and not 'anyOf' in json_object:
                     # we don't have any fields, but we have an array type, so we create a record with an 'items' field
                     avro_record = self.create_array_type(
-                        self.json_type_to_avro_type(json_object['items'], record_name, 'values', namespace, dependencies, json_schema, base_uri, avro_schema, record_stack) 
-                            if 'items' in json_object 
-                                else generic_type())
+                        self.json_type_to_avro_type(
+                            json_object['items'], record_name, 'values', namespace, dependencies, json_schema, base_uri, avro_schema, record_stack)
+                        if 'items' in json_object
+                        else generic_type())
                 else:
                     return json_object['type'] if 'type' in json_object else generic_type()
 
-            extension_types = []            
+            extension_types = []
             prop_docs = ''
             if 'patternProperties' in json_object and isinstance(json_object['patternProperties'], dict) and len(json_object['patternProperties']) > 0:
                 # pattern properties are represented as a record with field names that are the patterns
                 pattern_props = json_object['patternProperties']
                 for pattern_name, props in pattern_props.items():
                     deps = []
-                    prop_type = self.ensure_type(self.json_type_to_avro_type(props, record_name, pattern_name, namespace, deps, json_schema, base_uri, avro_schema, record_stack))
+                    prop_type = self.ensure_type(self.json_type_to_avro_type(
+                        props, record_name, pattern_name, namespace, deps, json_schema, base_uri, avro_schema, record_stack))
                     if self.is_standalone_avro_type(prop_type):
                         self.lift_dependencies_from_type(prop_type, deps)
-                        self.set_avro_type_value(prop_type, 'namespace', namespace)
+                        self.set_avro_type_value(
+                            prop_type, 'namespace', namespace)
                         self.register_type(avro_schema, prop_type)
                         prop_type_ref = self.get_qualified_name(prop_type)
                         dependencies.append(prop_type_ref)
                     else:
                         dependencies.extend(deps)
                         if isinstance(prop_type, str) and not prop_type in primitive_types:
                             dependencies.append(prop_type)
                     if self.is_empty_type(prop_type):
                         prop_type = generic_type()
                     prop_docs += f"Name pattern '{pattern_name}': [{self.get_field_type_name({'type':prop_type})}]. "
-                    extension_types.append(prop_type)            
-            
+                    extension_types.append(prop_type)
+
             if 'additionalProperties' in json_object and isinstance(json_object['additionalProperties'], bool):
                 if True == json_object['additionalProperties']:
                     prop_type = generic_type()
                     extension_types.append(prop_type)
             elif 'additionalProperties' in json_object and isinstance(json_object['additionalProperties'], dict) and len(json_object['additionalProperties']) > 0:
                 # additional properties are represented as a map of string to the type of the value
                 additional_props = json_object['additionalProperties']
                 deps = []
-                values_type = self.json_type_to_avro_type(additional_props, record_name, record_name + '_extensions', namespace, dependencies, json_schema, base_uri, avro_schema, record_stack)
+                values_type = self.json_type_to_avro_type(
+                    additional_props, record_name, record_name + '_extensions', namespace, dependencies, json_schema, base_uri, avro_schema, record_stack)
                 if self.is_standalone_avro_type(values_type):
                     self.lift_dependencies_from_type(values_type, deps)
-                    self.set_avro_type_value(values_type, 'namespace', namespace)
+                    self.set_avro_type_value(
+                        values_type, 'namespace', namespace)
                     self.register_type(avro_schema, values_type)
                     values_type_ref = self.get_qualified_name(values_type)
                     dependencies.append(values_type_ref)
                 else:
                     dependencies.extend(deps)
                     if isinstance(values_type, str) and not values_type in primitive_types:
                         dependencies.append(values_type)
                 if self.is_empty_type(values_type):
                     values_type = generic_type()
-                prop_docs += f"Extra properties: [{self.get_field_type_name({'type':values_type})}]. "	
+                prop_docs += f"Extra properties: [{self.get_field_type_name({'type':values_type})}]. "
                 extension_types.append(values_type)
             self.merge_description_into_doc(json_object, avro_record)
 
             avro_alternate_record = None
             if extension_types:
                 # Since Avro Schema does not allow fields with dynamic names
-                # to appear alongside regular fields, we will union the types of all properties with the 
+                # to appear alongside regular fields, we will union the types of all properties with the
                 # type of the additionalProperties and document this in the record's description
                 json_field_types = [field['type'] for field in field_refs]
-                field_type_names = [[field['name'], self.get_field_type_name(field)] for field in field_refs]
-                field_type_name_list: str = ', '.join([f"'{field[0]}': [{field[1]}]" for field in field_type_names])
+                field_type_names = [
+                    [field['name'], self.get_field_type_name(field)] for field in field_refs]
+                field_type_name_list: str = ', '.join(
+                    [f"'{field[0]}': [{field[1]}]" for field in field_type_names])
                 json_field_types.extend(extension_types)
                 json_field_types = self.flatten_union(json_field_types)
                 if len(json_field_types) == 1:
                     json_field_types = json_field_types[0]
                 doc = f"Alternate map: {field_type_name_list}. " if field_type_names else ''
                 doc += prop_docs
                 avro_alternate_record = self.create_map_type(json_field_types)
-                dependencies.append(self.compose_namespace(namespace,record_name))
+                dependencies.append(
+                    self.compose_namespace(namespace, record_name))
                 avro_record['doc'] = doc if not 'doc' in avro_record else avro_record['doc'] + ', ' + doc
-            
+
             if len(dependencies) > 0:
                 # dedupe the list
-                dependencies = list(set(dependencies))    
-                avro_record['dependencies'] = dependencies        
+                dependencies = list(set(dependencies))
+                avro_record['dependencies'] = dependencies
         finally:
             record_stack.pop()
         if avro_alternate_record:
             if self.is_empty_type(avro_record):
-                # there's no substantive content in the record, 
-                # so we will just return the alternate record, which 
+                # there's no substantive content in the record,
+                # so we will just return the alternate record, which
                 # is a plain map
                 return avro_alternate_record
             return [avro_record, avro_alternate_record]
         return avro_record
 
     def postprocess_schema(self, avro_schema: list) -> None:
         """ Post-process the Avro Schema for cases wheer we need a second pass """
-        if len(self.types_with_unmerged_types)>0:
-            types_with_unmerged_types = copy.deepcopy(self.types_with_unmerged_types)
+        if len(self.types_with_unmerged_types) > 0:
+            types_with_unmerged_types = copy.deepcopy(
+                self.types_with_unmerged_types)
             self.types_with_unmerged_types = []
             for ref_type in types_with_unmerged_types:
                 # find ref_type anywhere in the avro_schema graph, matching
-                # on name and namespace. 
-                find_fn = lambda t: 'name' in t and t['name'] == ref_type['name'] and 'namespace' in t and t['namespace'] == ref_type['namespace']
+                # on name and namespace.
+                def find_fn(
+                    t): return 'name' in t and t['name'] == ref_type['name'] and 'namespace' in t and t['namespace'] == ref_type['namespace']
                 type = find_schema_node(find_fn, avro_schema)
                 if not type:
-                    raise ValueError(f"Couldn't find type {ref_type['namespace']}.{ref_type['name']} in the Avro Schema.")
+                    raise ValueError(
+                        f"Couldn't find type {ref_type['namespace']}.{ref_type['name']} in the Avro Schema.")
                 # resolve the unmerged types
                 local_name = type.get('name')
                 if not isinstance(type, dict):
                     continue
                 unmerged_types = type.get('unmerged_types', [])
                 if len(unmerged_types) == 0:
                     if 'unmerged_types' in type:
                         del type['unmerged_types']
                     continue
                 base_type = copy.deepcopy(type)
                 if 'unmerged_types' in base_type:
                     del base_type['unmerged_types']
                 mergeable_types = [base_type]
                 deps: List[str] = []
-                self.lift_dependencies_from_type(type, deps)   
+                self.lift_dependencies_from_type(type, deps)
                 for item in unmerged_types:
-                    if isinstance(item,str):
-                        found_avro_type = next((t for t in avro_schema if self.get_qualified_name(t) == item ), None)
+                    if isinstance(item, str):
+                        found_avro_type = next(
+                            (t for t in avro_schema if self.get_qualified_name(t) == item), None)
                         if not found_avro_type:
                             continue
-                    elif isinstance(item,dict):
+                    elif isinstance(item, dict):
                         found_avro_type = item
                         self.lift_dependencies_from_type(found_avro_type, deps)
-                    if isinstance(found_avro_type,dict):
+                    if isinstance(found_avro_type, dict):
                         candidate = found_avro_type
                         if 'unmerged_types' in candidate:
                             del candidate['unmerged_types']
                         mergeable_types.append(candidate)
-                merge_result = self.merge_avro_schemas(mergeable_types, avro_schema, local_name, deps)
-                if isinstance(merge_result,dict):
+                merge_result = self.merge_avro_schemas(
+                    mergeable_types, avro_schema, local_name, deps)
+                if isinstance(merge_result, dict):
                     merge_result['dependencies'] = deps
                     if 'unmerged_types' in merge_result:
                         del merge_result['unmerged_types']
                 if isinstance(merge_result, list):
                     # unmerged field containers have fields.
-                    self.set_avro_type_value(type, 'name', type['name'] + '_item')
-                    self.set_avro_type_value(type, 'fields', [{'name': 'value', 'type': merge_result }])
+                    self.set_avro_type_value(
+                        type, 'name', type['name'] + '_item')
+                    self.set_avro_type_value(
+                        type, 'fields', [{'name': 'value', 'type': merge_result}])
                     merge_result = copy.deepcopy(type)
                 set_schema_node(find_fn, merge_result, avro_schema)
-    
+
     def process_definition_list(self, json_schema, namespace, base_uri, avro_schema, record_stack, schema_name, json_schema_list):
         """Process a schema definition list."""
         for sub_schema_name, schema in json_schema_list.items():
             if not isinstance(schema, dict) and not isinstance(schema, list):
                 # skip items that are not schema definitions or lists
                 continue
             if 'type' in schema or 'allOf' in schema or 'oneOf' in schema or 'anyOf' in schema or 'properties' in schema or 'enum' in schema or '$ref' in schema or 'additionalProperties' in schema or 'patternProperties' in schema:
                 # this is a schema definition
-                self.process_definition(json_schema, namespace, base_uri, avro_schema, record_stack, sub_schema_name, schema)
+                self.process_definition(
+                    json_schema, namespace, base_uri, avro_schema, record_stack, sub_schema_name, schema)
                 continue
             # it's a schema definition list
-            self.process_definition_list(json_schema, namespace, base_uri, avro_schema, record_stack, schema_name, schema)
+            self.process_definition_list(
+                json_schema, namespace, base_uri, avro_schema, record_stack, schema_name, schema)
 
     def process_definition(self, json_schema, namespace, base_uri, avro_schema, record_stack, schema_name, schema, is_root: bool = False) -> Tuple[str, str] | None:
         """ Process a schema definition. """
         avro_schema_item = None
-        avro_schema_item_list = self.json_schema_object_to_avro_record(schema_name, schema, namespace, json_schema, base_uri, avro_schema, record_stack)
+        avro_schema_item_list = self.json_schema_object_to_avro_record(
+            schema_name, schema, namespace, json_schema, base_uri, avro_schema, record_stack)
         if not isinstance(avro_schema_item_list, list) and not isinstance(avro_schema_item_list, dict):
             # skip if the record couldn't be resolved
             return None
         # the call above usually returns a single record, but we pretend it's normally a list to handle allOf/anyOf/oneOf cases
         if isinstance(avro_schema_item_list, list) and is_root and len(avro_schema_item_list) > 1:
             # if we have multiple root-level records, we will wrap them all in a single record
-            root_avro_schema_item = self.create_wrapper_record(schema_name+'_wrapper', namespace, 'root', [], avro_schema_item_list)
+            root_avro_schema_item = self.create_wrapper_record(
+                schema_name+'_wrapper', namespace, 'root', [], avro_schema_item_list)
             for avro_schema_item in avro_schema_item_list:
-                self.merge_dependencies_into_parent([], avro_schema_item, root_avro_schema_item)
+                self.merge_dependencies_into_parent(
+                    [], avro_schema_item, root_avro_schema_item)
             self.register_type(avro_schema, root_avro_schema_item)
             return root_avro_schema_item['namespace'], root_avro_schema_item['name']
         elif not isinstance(avro_schema_item_list, list):
             # is not a list, so we'll wrap it in a list
             avro_schema_item_list = [avro_schema_item_list]
         for avro_schema_item in avro_schema_item_list:
             # add the item to the schema if it's not already there
             if isinstance(avro_schema_item, str):
                 continue
-            if isinstance(avro_schema_item,dict) and not 'name' in avro_schema_item:
+            if isinstance(avro_schema_item, dict) and not 'name' in avro_schema_item:
                 avro_schema_item['name'] = avro_name(schema_name)
-            existing_type = next((t for t in avro_schema if t.get('name') == avro_schema_item['name'] and t.get('namespace') == avro_schema_item.get('namespace') ), None)
+            existing_type = next((t for t in avro_schema if t.get('name') == avro_schema_item['name'] and t.get(
+                'namespace') == avro_schema_item.get('namespace')), None)
             if not existing_type:
                 if (not self.is_empty_type(avro_schema_item) or 'unmerged_types' in avro_schema_item) and \
-                    self.is_standalone_avro_type(avro_schema_item):
+                        self.is_standalone_avro_type(avro_schema_item):
                     # we only register record/enum as type. the other defs are mix-ins
-                    self.register_type(avro_schema, avro_schema_item)              
+                    self.register_type(avro_schema, avro_schema_item)
                     return avro_schema_item['namespace'], avro_schema_item['name']
                 elif is_root:
                     # at the root, we will wrap the type in a record to make it top-level
-                    deps: List [str] = []
-                    self.lift_dependencies_from_type(avro_schema_item, deps)                    
-                    avro_schema_wrapper = self.create_wrapper_record(schema_name, avro_schema_item.get('namespace',namespace), avro_schema_item['name'], deps, avro_schema_item)
+                    deps: List[str] = []
+                    self.lift_dependencies_from_type(avro_schema_item, deps)
+                    avro_schema_wrapper = self.create_wrapper_record(schema_name, avro_schema_item.get(
+                        'namespace', namespace), avro_schema_item['name'], deps, avro_schema_item)
                     if len(deps) > 0:
                         avro_schema_wrapper['dependencies'] = deps
                     avro_schema_item = avro_schema_wrapper
                     self.register_type(avro_schema, avro_schema_item)
                     return avro_schema_item['namespace'], avro_schema_item['name']
         return None
-        
 
     def id_to_avro_namespace(self, id: str) -> str:
         """Convert a XSD namespace to Avro Namespace."""
         parsed_url = urlparse(id)
-        # strip the file extension 
+        # strip the file extension
         path = parsed_url.path.rsplit('.')[0]
         path_segments = path.strip('/').replace('-', '_').split('/')
         reversed_path_segments = reversed(path_segments)
         namespace_suffix = self.compose_namespace(*reversed_path_segments)
         if parsed_url.hostname:
-            namespace_prefix = self.compose_namespace(*reversed(parsed_url.hostname.split('.')))
+            namespace_prefix = self.compose_namespace(
+                *reversed(parsed_url.hostname.split('.')))
         namespace = self.compose_namespace(namespace_prefix, namespace_suffix)
         return namespace
-    
 
     def jsons_to_avro(self, json_schema: dict | list, namespace: str, base_uri: str) -> list | dict | str:
         """Convert a JSON-schema to an Avro-schema."""
         avro_schema: List[dict] = []
         record_stack: List[str] = []
 
         parsed_url = urlparse(base_uri)
         schema_name = self.root_class_name
 
         if isinstance(json_schema, dict) and ('definitions' in json_schema or '$defs' in json_schema):
             # this is a swagger file or has a 'definitions' block
-            json_schema_defs = json_schema.get('definitions', json_schema.get('$defs', []))
+            json_schema_defs = json_schema.get(
+                'definitions', json_schema.get('$defs', []))
             for def_schema_name, schema in json_schema_defs.items():
                 if 'type' in schema or 'allOf' in schema or 'oneOf' in schema or 'anyOf' in schema or 'properties' in schema or 'enum' in schema or '$ref' in schema or 'additionalProperties' in schema or 'patternProperties' in schema:
                     # this is a schema definition
-                    self.process_definition(json_schema, namespace, base_uri, avro_schema, record_stack, def_schema_name, schema)
+                    self.process_definition(
+                        json_schema, namespace, base_uri, avro_schema, record_stack, def_schema_name, schema)
                 else:
                     # it's a schema definition list
-                    self.process_definition_list(json_schema, namespace, base_uri, avro_schema, record_stack, schema_name, schema.copy())
+                    self.process_definition_list(
+                        json_schema, namespace, base_uri, avro_schema, record_stack, schema_name, schema.copy())
         elif isinstance(json_schema, list):
             # this is a schema definition list
-            self.process_definition_list(json_schema, namespace, base_uri, avro_schema, record_stack, schema_name, json_schema)
+            self.process_definition_list(
+                json_schema, namespace, base_uri, avro_schema, record_stack, schema_name, json_schema)
 
         root_namespace = None
         root_name = None
         if isinstance(json_schema, dict) and 'type' in json_schema or 'allOf' in json_schema or 'oneOf' in json_schema or 'anyOf' in json_schema or 'properties' in json_schema:
             # this is a schema definition
             if isinstance(json_schema, dict) and '$ref' in json_schema:
-                #if there is a $ref at the root level, resolve the reference and merge it with the current schema
+                # if there is a $ref at the root level, resolve the reference and merge it with the current schema
                 ref = json_schema['$ref']
                 if ref:
-                    ref_schema, json_doc = self.resolve_reference(json_schema, base_uri, json_schema)
-                    json_schema = self.merge_json_schemas([json_schema, ref_schema], intersect=False)
-            root_info = self.process_definition(json_schema, namespace, base_uri, avro_schema, record_stack, schema_name, json_schema, is_root=True)
+                    ref_schema, json_doc = self.resolve_reference(
+                        json_schema, base_uri, json_schema)
+                    json_schema = self.merge_json_schemas(
+                        [json_schema, ref_schema], intersect=False)
+            root_info = self.process_definition(
+                json_schema, namespace, base_uri, avro_schema, record_stack, schema_name, json_schema, is_root=True)
             if root_info:
                 root_namespace, root_name = root_info
-        
+
         # postprocessing pass
         self.postprocess_schema(avro_schema)
 
-        if isinstance(avro_schema,list) and len(avro_schema) > 1 and self.split_top_level_records:
+        if isinstance(avro_schema, list) and len(avro_schema) > 1 and self.split_top_level_records:
             new_avro_schema = []
             for item in avro_schema:
                 if isinstance(item, dict) and 'type' in item and item['type'] == 'record':
                     # we need to make a copy since the inlining operation shuffles types
                     schema_copy = copy.deepcopy(avro_schema)
                     # find the item with the same name and namespace in the copy
-                    found_item = next((t for t in schema_copy if t.get('name') == item['name'] and t.get('namespace') == item.get('namespace') ), None)
+                    found_item = next((t for t in schema_copy if t.get(
+                        'name') == item['name'] and t.get('namespace') == item.get('namespace')), None)
                     if found_item:
                         # inline all dependencies of the item
                         inline_dependencies_of(schema_copy, found_item)
                         new_avro_schema.append(found_item)
             avro_schema = new_avro_schema
         else:
             # sort the records by their dependencies
             if root_name and root_namespace and not ('definitions' in json_schema or '$defs' in json_schema):
                 # inline all dependencies if this is a doc with only a root level definition
-                root = find_schema_node(lambda t: 'name' in t and t['name'] == root_name and 'namespace' in t and t['namespace'] == root_namespace, avro_schema)
+                root = find_schema_node(
+                    lambda t: 'name' in t and t['name'] == root_name and 'namespace' in t and t['namespace'] == root_namespace, avro_schema)
                 inline_dependencies_of(avro_schema, root)
                 return root
             else:
-                avro_schema = sort_messages_by_dependencies(avro_schema)       
-        
+                avro_schema = sort_messages_by_dependencies(avro_schema)
+
             if parsed_url.fragment and isinstance(json_schema, dict):
                 # if the fragment is present in the URL, it's a reference to a schema definition
                 # so we will resolve that reference and return a type
                 self.imported_types.clear()
                 fragment_schema: List[dict] = []
                 json_pointer = parsed_url.fragment
                 schema_name = parsed_url.fragment.split('/')[-1]
                 schema = jsonpointer.resolve_pointer(json_schema, json_pointer)
-                avro_schema_item = self.json_schema_object_to_avro_record(schema_name, schema, namespace, json_schema, base_uri, fragment_schema, record_stack)
+                avro_schema_item = self.json_schema_object_to_avro_record(
+                    schema_name, schema, namespace, json_schema, base_uri, fragment_schema, record_stack)
                 if avro_schema_item:
                     # we roll all the types into this record as the top level type
                     inline_dependencies_of(avro_schema, avro_schema_item)
                     return avro_schema_item
-        
-        return avro_schema
 
+        return avro_schema
 
     def convert_jsons_to_avro(self, json_schema_file_path: str, avro_schema_path: str, namespace: str | None = None, utility_namespace: str | None = None) -> list | dict | str:
         """Convert JSON schema file to Avro schema file."""
         # turn the file path into a file URI if it's not a URI already
         parsed_url = urlparse(json_schema_file_path)
         if not parsed_url.hostname and not parsed_url.scheme == 'file':
             json_schema_file_path = 'file://' + json_schema_file_path
             parsed_url = urlparse(json_schema_file_path)
         content = self.fetch_content(parsed_url.geturl())
         json_schema = json.loads(content)
 
         if not namespace:
-            namespace = parsed_url.geturl().replace('\\','/').replace('-','_').split('/')[-1].split('.')[0]
-            # get the $id if present 
+            namespace = parsed_url.geturl().replace('\\', '/').replace('-',
+                                                                       '_').split('/')[-1].split('.')[0]
+            # get the $id if present
             if '$id' in json_schema:
                 namespace = self.id_to_avro_namespace(json_schema['$id'])
         self.root_namespace = namespace
         if utility_namespace:
             self.utility_namespace = utility_namespace
         else:
             self.utility_namespace = self.root_namespace + '.utility'
-        
+
         # drop the file name from the parsed URL to get the base URI
-        avro_schema = self.jsons_to_avro(json_schema, namespace, parsed_url.geturl())
+        avro_schema = self.jsons_to_avro(
+            json_schema, namespace, parsed_url.geturl())
         if len(avro_schema) == 1:
             avro_schema = avro_schema[0]
 
         # create the directory for the Avro schema file if it doesn't exist
-        dir = os.path.dirname(avro_schema_path) if not self.split_top_level_records else avro_schema_path
+        dir = os.path.dirname(
+            avro_schema_path) if not self.split_top_level_records else avro_schema_path
         if dir != '' and not os.path.exists(dir):
             os.makedirs(dir, exist_ok=True)
         if self.split_top_level_records:
             # if we are splitting top level records, we will create a file for each record
             for item in avro_schema:
                 if isinstance(item, dict) and 'type' in item and item['type'] == 'record':
-                    schema_file_path = os.path.join(dir, item['name'] + '.avsc')
+                    schema_file_path = os.path.join(
+                        dir, item['name'] + '.avsc')
                     with open(schema_file_path, 'w') as avro_file:
                         json.dump(item, avro_file, indent=4)
         else:
             with open(avro_schema_path, 'w') as avro_file:
                 json.dump(avro_schema, avro_file, indent=4)
         return avro_schema
-    
 
-def convert_jsons_to_avro(json_schema_file_path: str, avro_schema_path: str, namespace: str = '', utility_namespace = '', root_class_name = '', split_top_level_records = False) -> list | dict | str:
+
+def convert_jsons_to_avro(json_schema_file_path: str, avro_schema_path: str, namespace: str = '', utility_namespace='', root_class_name='', split_top_level_records=False) -> list | dict | str:
     """Convert JSON schema file to Avro schema file."""
     try:
         converter = JsonToAvroConverter()
         converter.split_top_level_records = split_top_level_records
         if root_class_name:
             converter.root_class_name = root_class_name
         return converter.convert_jsons_to_avro(json_schema_file_path, avro_schema_path, namespace, utility_namespace)
     except Exception as e:
-        print(f'Error converting JSON {json_schema_file_path} to Avro: {e.args[0]}')
-        return []
+        print(
+            f'Error converting JSON {json_schema_file_path} to Avro: {e.args[0]}')
+        return []
```

### Comparing `avrotize-1.2.4/avrotize/kconnect.json` & `avrotize-1.3.0/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/kstructtoavro.py` & `avrotize-1.3.0/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/proto2parser.py` & `avrotize-1.3.0/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/proto3parser.py` & `avrotize-1.3.0/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/prototoavro.py` & `avrotize-1.3.0/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/prototypes/any.avsc` & `avrotize-1.3.0/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/prototypes/api.avsc` & `avrotize-1.3.0/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/prototypes/duration.avsc` & `avrotize-1.3.0/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/prototypes/field_mask.avsc` & `avrotize-1.3.0/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/prototypes/struct.avsc` & `avrotize-1.3.0/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/prototypes/timestamp.avsc` & `avrotize-1.3.0/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/prototypes/type.avsc` & `avrotize-1.3.0/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/prototypes/wrappers.avsc` & `avrotize-1.3.0/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/avrotize/xsdtoavro.py` & `avrotize-1.3.0/avrotize/xsdtoavro.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,76 @@
+# pylint: disable=line-too-long, consider-iterating-dictionary, too-many-locals, too-many-branches
+
+"""Converts XSD to Avro schema."""
+
 import re
 from typing import Dict, List, Tuple
 import xml.etree.ElementTree as ET
 import json
-import re
 from urllib.parse import urlparse
-from avrotize.common import avro_name, avro_namespace, generic_type
+from avrotize.common import avro_namespace, generic_type
 
 from avrotize.dependency_resolver import inline_dependencies_of, sort_messages_by_dependencies
 
-xsd_namespace = 'http://www.w3.org/2001/XMLSchema'
+XSD_NAMESPACE = 'http://www.w3.org/2001/XMLSchema'
+
 
 class XSDToAvro:
+    """ Convert XSD to Avro schema."""
 
     def __init__(self) -> None:
-        self.simple_type_map: Dict[str,str | dict] = {}
+        """ Initialize the class. """
+        self.simple_type_map: Dict[str, str | dict] = {}
         self.avro_namespace = ''
 
     def xsd_targetnamespace_to_avro_namespace(self, targetnamespace: str) -> str:
         """Convert a XSD namespace to Avro Namespace."""
         parsed_url = urlparse(targetnamespace)
         if parsed_url.scheme == 'urn':
-            path_segments = parsed_url.path.strip(':').replace('.','-').split(':')
+            path_segments = parsed_url.path.strip(
+                ':').replace('.', '-').split(':')
             # join all path segments that start with a number with the previous one
             new_path_segments: List[str] = []
             n = len(path_segments)
             for i in range(n):
                 if path_segments[i][0].isdigit():
                     if i == 0:
                         new_path_segments.append('_'+path_segments[i])
                     else:
                         new_path_segments[-1] = f"{new_path_segments[-1]}-{path_segments[i]}"
                 else:
                     new_path_segments.append(path_segments[i])
             path_segments = new_path_segments
-        else:   
+        else:
             path_segments = parsed_url.path.strip('/').split('/')
             path_segments = list(reversed(path_segments))
         namespace_prefix = '.'.join(path_segments)
         if parsed_url.hostname:
             namespace_suffix = parsed_url.hostname
             namespace = f"{namespace_prefix}.{namespace_suffix}"
         else:
             namespace = namespace_prefix
         return avro_namespace(namespace)
 
     def xsd_to_avro_type(self, xsd_type: str, namespaces: dict):
         """Convert a XSD type to an Avro type."""
         if xsd_type in self.simple_type_map:
             return self.simple_type_map[xsd_type]
-        
+
         # split the type on the first colon
         if ':' not in xsd_type:
-            type = xsd_type
+            type_name = xsd_type
             prefix = ''
         else:
-            prefix, type = xsd_type.split(':', 1)
-            if not type:
-                type = prefix
+            prefix, type_name = xsd_type.split(':', 1)
+            if not type_name:
+                type_name = prefix
                 prefix = ''
         # find the namespace for the prefix
-        ns = namespaces.get(xsd_namespace, '')
+        ns = namespaces.get(XSD_NAMESPACE, '')
         if ns == prefix:
             base_type_map = {
                 'string': 'string',
                 'int': 'int',
                 'integer': 'int',
                 'long': 'long',
                 'short': 'int',
@@ -104,66 +111,73 @@
                 'IDREF': 'string',
                 'IDREFS': 'string',
                 'NMTOKEN': 'string',
                 'NMTOKENS': 'string',
                 'QName': 'string',
                 'NOTATION': 'string'
             }
-            return base_type_map.get(type, self.avro_namespace+'.'+type)
+            return base_type_map.get(type_name, self.avro_namespace+'.'+type_name)
         else:
-            return self.avro_namespace+'.'+type
-
-
+            return self.avro_namespace+'.'+type_name
 
-    def process_element(self, element: ET.Element, namespaces: dict, avro_schema: list, dependencies: list):
+    def process_element(self, element: ET.Element, namespaces: dict, dependencies: list):
+        """Process an element in the XSD schema."""
         name = element.get('name')
-        type = element.get('type','')
-        avro_type = self.xsd_to_avro_type(type, namespaces)  
-        if not type.startswith(f'{namespaces[xsd_namespace]}:') and type not in self.simple_type_map.keys():           
-            dependencies.append(avro_type if isinstance(avro_type, str) else avro_type.get('namespace')+'.'+avro_type.get('name'))
+        type_value = element.get('type', '')
+        avro_type = self.xsd_to_avro_type(type_value, namespaces)
+        if not type_value.startswith(f'{namespaces[XSD_NAMESPACE]}:') and type_value not in self.simple_type_map.keys():
+            dependencies.append(avro_type if isinstance(
+                avro_type, str) else avro_type.get('namespace')+'.'+avro_type.get('name'))
             dependencies = list(set(dependencies))
-        
-        maxOccurs = element.get('maxOccurs')
-        if maxOccurs is not None and maxOccurs != '1':
-            avro_type = {'type' : 'array', 'items': avro_type}
-        minOccurs = element.get('minOccurs')
-        if minOccurs is not None and minOccurs == '0':
-            avro_type = ['null', avro_type]    
-        return {'name': name, 'type': avro_type}  
 
+        max_occurs = element.get('maxOccurs')
+        if max_occurs is not None and max_occurs != '1':
+            avro_type = {'type': 'array', 'items': avro_type}
+        min_occurs = element.get('minOccurs')
+        if min_occurs is not None and min_occurs == '0':
+            avro_type = ['null', avro_type]
+        return {'name': name, 'type': avro_type}
 
-    def process_complex_type(self, complex_type: ET.Element, namespaces: dict, avro_schema: list) -> dict | str:
+    def process_complex_type(self, complex_type: ET.Element, namespaces: dict) -> dict | str:
+        """ Process a complex type in the XSD schema."""
         dependencies: List[str] = []
-        avro_type: dict  = {
-            'type': 'record', 
+        avro_type: dict = {
+            'type': 'record',
             'name': complex_type.attrib.get('name'),
             'namespace': self.avro_namespace,
             'fields': []
-            }
+        }
         avro_doc = ''
-        annotation = complex_type.find(f'{{{xsd_namespace}}}annotation', namespaces)
+        annotation = complex_type.find(
+            f'{{{XSD_NAMESPACE}}}annotation', namespaces)
         if annotation is not None:
-            documentation = annotation.find(f'{{{xsd_namespace}}}documentation', namespaces)
+            documentation = annotation.find(
+                f'{{{XSD_NAMESPACE}}}documentation', namespaces)
             if documentation is not None and documentation.text is not None:
                 avro_doc = documentation.text.strip()
                 avro_type['doc'] = avro_doc
         fields = []
-        for sequence in complex_type.findall(f'{{{xsd_namespace}}}sequence', namespaces):
-            for el in sequence.findall(f'{{{xsd_namespace}}}element', namespaces):
-                fields.append(self.process_element(el, namespaces, avro_schema, dependencies))
-            if sequence.findall(f'{{{xsd_namespace}}}any', namespaces):
-                fields.append({ "name": "any", "type": generic_type() })
-        for all in complex_type.findall(f'{{{xsd_namespace}}}all', namespaces):
-            for el in all.findall(f'{{{xsd_namespace}}}element', namespaces):
-                fields.append(self.process_element(el, namespaces, avro_schema, dependencies))
-        for choice in complex_type.findall(f'{{{xsd_namespace}}}choice', namespaces):
+        for sequence in complex_type.findall(f'{{{XSD_NAMESPACE}}}sequence', namespaces):
+            for el in sequence.findall(f'{{{XSD_NAMESPACE}}}element', namespaces):
+                field = self.process_element(el, namespaces, dependencies)
+                field['xmlkind'] = 'element'
+                fields.append(field)
+            if sequence.findall(f'{{{XSD_NAMESPACE}}}any', namespaces):
+                fields.append({"name": "any", "xmlkind": "any", "type": generic_type()})
+        for all_types in complex_type.findall(f'{{{XSD_NAMESPACE}}}all', namespaces):
+            for el in all_types.findall(f'{{{XSD_NAMESPACE}}}element', namespaces):
+                field = self.process_element(el, namespaces, dependencies)
+                field['xmlkind'] = 'element'
+                fields.append(field)
+        for choice in complex_type.findall(f'{{{XSD_NAMESPACE}}}choice', namespaces):
             choices: list = []
-            for el in choice.findall(f'{{{xsd_namespace}}}element', namespaces):
-                deps: List [str] = []
-                choice_field = self.process_element(el, namespaces, avro_schema, deps)
+            for el in choice.findall(f'{{{XSD_NAMESPACE}}}element', namespaces):
+                deps: List[str] = []
+                choice_field = self.process_element(el, namespaces, deps)
+                choice_field['xmlkind'] = 'element'
                 choice_record = {
                     'type': 'record',
                     'name': f'{complex_type.attrib.get("name")}_{choice_field["name"]}',
                     'fields': [choice_field],
                     'namespace': self.avro_namespace
                 }
                 if avro_doc:
@@ -172,150 +186,191 @@
                 dependencies.extend(deps)
                 dependencies = list(set(dependencies))
             choices_field = {
                 'name': f'{complex_type.attrib.get("name")}',
                 'type': choices
             }
             fields.append(choices_field)
-        for attribute in complex_type.findall(f'.{{{xsd_namespace}}}attribute', namespaces):
-            fields.append(self.process_element(attribute, namespaces, avro_schema, dependencies))
-        for el in complex_type.findall(f'{{{xsd_namespace}}}simpleContent', namespaces):
-            simple_content = el.find(f'{{{xsd_namespace}}}extension', namespaces)
+        for attribute in complex_type.findall(f'.{{{XSD_NAMESPACE}}}attribute', namespaces):
+            field = self.process_element(attribute, namespaces, dependencies)
+            field['xmlkind'] = 'attribute'
+            fields.append(field)
+        for el in complex_type.findall(f'{{{XSD_NAMESPACE}}}simpleContent', namespaces):
+            simple_content = el.find(
+                f'{{{XSD_NAMESPACE}}}extension', namespaces)
             if simple_content is not None:
-                baseType = simple_content.attrib.get('base')
-                if baseType:
-                    fields.append({"name": "value", "type": self.xsd_to_avro_type(baseType, namespaces)})
-                    for se in simple_content.findall(f'{{{xsd_namespace}}}attribute', namespaces):
-                        fields.append(self.process_element(se, namespaces, avro_schema, dependencies))
+                base_type = simple_content.attrib.get('base')
+                if base_type:
+                    fields.append(
+                        {"name": "value", "type": self.xsd_to_avro_type(base_type, namespaces)})
+                    for se in simple_content.findall(f'{{{XSD_NAMESPACE}}}attribute', namespaces):
+                        field = self.process_element(se, namespaces, dependencies)
+                        field['xmlkind'] = 'attribute'
+                        fields.append(field)
                 else:
                     raise ValueError("No base found in simpleContent")
 
         avro_type['fields'] = fields
         if dependencies:
             avro_type['dependencies'] = dependencies
         return avro_type
 
-    def process_simple_type(self, simple_type: ET.Element, namespaces: dict, avro_schema: list) -> Tuple[bool, dict | str]:
+    def process_simple_type(self, simple_type: ET.Element, namespaces: dict) -> Tuple[bool, dict | str]:
+        """ Process a simple type in the XSD schema. """
         type_name = simple_type.attrib.get('name')
         if not type_name:
             raise ValueError("SimpleType must have a name")
         avro_doc = ''
-        annotation = simple_type.find(f'{{{xsd_namespace}}}annotation', namespaces)
+        annotation = simple_type.find(
+            f'{{{XSD_NAMESPACE}}}annotation', namespaces)
         if annotation is not None:
-            documentation = annotation.find(f'{{{xsd_namespace}}}documentation', namespaces)
+            documentation = annotation.find(
+                f'{{{XSD_NAMESPACE}}}documentation', namespaces)
             if documentation is not None and documentation.text is not None:
                 avro_doc = documentation.text.strip()
-        
-        for restriction in simple_type.findall(f'{{{xsd_namespace}}}restriction', namespaces):
-            baseType = restriction.get('base')
-            enums: List[str] = [el.attrib.get('value','Empty') for el in restriction.findall(f'{{{xsd_namespace}}}enumeration', namespaces)]
+
+        for restriction in simple_type.findall(f'{{{XSD_NAMESPACE}}}restriction', namespaces):
+            base_type = restriction.get('base')
+            enums: List[str] = [el.attrib.get('value', 'Empty') for el in restriction.findall(
+                f'{{{XSD_NAMESPACE}}}enumeration', namespaces)]
             # if any of the enum entries start with a digit, we need to prefix the entry with _
             if enums:
-                for i,enum in enumerate(enums):
+                for i, enum in enumerate(enums):
                     if enums[i][0].isdigit():
                         enums[i] = '_'+enum
                 enum_type = {
-                    'type': 'enum', 
-                    'name': simple_type.attrib.get('name'), 
+                    'type': 'enum',
+                    'name': simple_type.attrib.get('name'),
                     'namespace': self.avro_namespace,
                     'symbols': enums
-                    }
+                }
                 if avro_doc:
                     enum_type['doc'] = avro_doc
                 return True, enum_type
-            elif baseType:
+            elif base_type:
                 # if the baseType is a decimal, get the precision and scale sub-element value attributes to set the logicalType
-                if baseType == namespaces [xsd_namespace]+':'+'decimal':
-                    precision = restriction.find(f'{{{xsd_namespace}}}totalDigits', namespaces)
-                    scale = restriction.find(f'{{{xsd_namespace}}}fractionDigits', namespaces)
-                    logicalType = {
-                        'type': 'bytes', 
-                        'logicalType': 'decimal', 
-                        'precision': int(precision.attrib.get('value', 32)) if isinstance(precision, ET.Element) else 32, 
+                if base_type == namespaces[XSD_NAMESPACE]+':'+'decimal':
+                    precision = restriction.find(
+                        f'{{{XSD_NAMESPACE}}}totalDigits', namespaces)
+                    scale = restriction.find(
+                        f'{{{XSD_NAMESPACE}}}fractionDigits', namespaces)
+                    logical_type = {
+                        'type': 'bytes',
+                        'logicalType': 'decimal',
+                        'precision': int(precision.attrib.get('value', 32)) if isinstance(precision, ET.Element) else 32,
                         'scale': int(scale.attrib.get('value', 6)) if isinstance(scale, ET.Element) else 6,
-                        }
+                    }
                     if avro_doc:
-                        logicalType['doc'] = avro_doc
-                    self.simple_type_map[type_name] = logicalType
-                    return False, logicalType                    
+                        logical_type['doc'] = avro_doc
+                    self.simple_type_map[type_name] = logical_type
+                    return False, logical_type
                 else:
-                    self.simple_type_map[type_name] = self.xsd_to_avro_type(baseType, namespaces)
+                    self.simple_type_map[type_name] = self.xsd_to_avro_type(
+                        base_type, namespaces)
                     return False, self.simple_type_map[type_name]
         raise ValueError("No content found in simple type")
 
-    def process_top_level_element(self, element: ET.Element, namespaces: dict, avro_schema: list):
+    def process_top_level_element(self, element: ET.Element, namespaces: dict):
+        """ Process a top level element in the XSD schema. """
         dependencies: List[str] = []
         avro_type: dict = {
-            'type': 'record', 
-            'name': 'Root', 
+            'type': 'record',
+            'name': 'Root',
             'namespace': self.avro_namespace,
             'fields': []
-            }
-        annotation = element.find(f'{{{xsd_namespace}}}annotation', namespaces)
+        }
+        annotation = element.find(f'{{{XSD_NAMESPACE}}}annotation', namespaces)
         if annotation is not None:
-            documentation = annotation.find(f'{{{xsd_namespace}}}documentation', namespaces)
+            documentation = annotation.find(
+                f'{{{XSD_NAMESPACE}}}documentation', namespaces)
             if documentation is not None and documentation.text is not None:
                 avro_type['doc'] = documentation.text.strip()
-        
+
         if 'type' in element.attrib:
-            avro_type['fields'].append(self.process_element(element, namespaces, avro_schema, dependencies))
+            field = self.process_element(element, namespaces, dependencies)
+            field['xmlkind'] = 'attribute'
+            avro_type['fields'].append(field)
             if dependencies:
                 avro_type['dependencies'] = dependencies
             return avro_type
         else:
-            complex_type = element.find(f'{{{xsd_namespace}}}complexType', namespaces)
+            complex_type = element.find(
+                f'{{{XSD_NAMESPACE}}}complexType', namespaces)
             if complex_type is None:
-                raise ValueError('top level element must have a type or be complexType')
-            complex_type.set('name', element.get('name',''))
-            avro_complex_type = self.process_complex_type(complex_type, namespaces, avro_schema)
+                raise ValueError(
+                    'top level element must have a type or be complexType')
+            complex_type.set('name', element.get('name', ''))
+            avro_complex_type = self.process_complex_type(
+                complex_type, namespaces)
             return avro_complex_type
 
     def extract_xml_namespaces(self, xml_str: str):
+        """ Extract XML namespaces from an XML string."""
         # This regex finds all xmlns:prefix="uri" declarations
         pattern = re.compile(r'xmlns:([\w]+)="([^"]+)"')
-        namespaces = {m.group(2): m.group(1) for m in pattern.finditer(xml_str)}
+        namespaces = {m.group(2): m.group(1)
+                      for m in pattern.finditer(xml_str)}
         return namespaces
 
-    def xsd_to_avro(self, xsd_path: str):
+    def xsd_to_avro(self, xsd_path: str, code_namespace: str | None = None):
+        """ Convert XSD to Avro schema. """
         # load the XSD file into a string
-        with open(xsd_path, 'r') as f:
+        with open(xsd_path, 'r', encoding='utf-8') as f:
             xsd = f.read()
 
         namespaces = self.extract_xml_namespaces(xsd)
         root = ET.fromstring(xsd)
-        targetNamespace = root.get('targetNamespace')
-        if targetNamespace is None:
+        target_namespace = root.get('targetNamespace')
+        if target_namespace is None:
             raise ValueError('targetNamespace not found')
-        self.avro_namespace = self.xsd_targetnamespace_to_avro_namespace(targetNamespace)
-        ET.register_namespace(namespaces[xsd_namespace], xsd_namespace) 
-        avro_schema: List[dict|list|str] = []
-        
-        for simple_type in root.findall(f'{{{xsd_namespace}}}simpleType', namespaces):
-            add_to_schema, simple_type_type = self.process_simple_type(simple_type, namespaces, avro_schema)
+        if not code_namespace:
+            self.avro_namespace = self.xsd_targetnamespace_to_avro_namespace(target_namespace)
+        else:
+            self.avro_namespace = code_namespace
+        ET.register_namespace(namespaces[XSD_NAMESPACE], XSD_NAMESPACE)
+        avro_schema: List[dict | list | str] = []
+
+        for simple_type in root.findall(f'{{{XSD_NAMESPACE}}}simpleType', namespaces):
+            add_to_schema, simple_type_type = self.process_simple_type(
+                simple_type, namespaces)
             # we only want to append simple types if they are not resolved to one of the base types
             if add_to_schema:
                 avro_schema.append(simple_type_type)
-        for complex_type in root.findall(f'{{{xsd_namespace}}}complexType', namespaces):
-            avro_schema.append(self.process_complex_type(complex_type, namespaces, avro_schema))    
+        for complex_type in root.findall(f'{{{XSD_NAMESPACE}}}complexType', namespaces):
+            avro_schema.append(self.process_complex_type(
+                complex_type, namespaces))
 
-        top_level_elements = root.findall(f'{{{xsd_namespace}}}element', namespaces)
+        top_level_elements = root.findall(
+            f'{{{XSD_NAMESPACE}}}element', namespaces)
         if len(top_level_elements) == 1:
-             record = self.process_top_level_element(top_level_elements[0], namespaces, avro_schema)
-             inline_dependencies_of(avro_schema, record)
-             return record
+            record = self.process_top_level_element(
+                top_level_elements[0], namespaces)
+            inline_dependencies_of(avro_schema, record)
+            return record
         for element in top_level_elements:
-            avro_schema.append(self.process_top_level_element(element, namespaces, avro_schema))    
-        
+            avro_schema.append(self.process_top_level_element(
+                element, namespaces))
+
         avro_schema = sort_messages_by_dependencies(avro_schema)
         if len(avro_schema) == 1:
             return avro_schema[0]
         else:
             return avro_schema
 
     def convert_xsd_to_avro(self, xsd_path: str, avro_path: str, namespace: str | None = None):
-        avro_schema = self.xsd_to_avro(xsd_path)
-        with open(avro_path, 'w') as f:
+        """Convert XSD to Avro schema and write to a file."""
+        avro_schema = self.xsd_to_avro(xsd_path, code_namespace=namespace)
+        with open(avro_path, 'w', encoding='utf-8') as f:
             json.dump(avro_schema, f, indent=4)
 
+
 def convert_xsd_to_avro(xsd_path: str, avro_path: str, namespace: str | None = None):
+    """ 
+    Convert XSD to Avro schema and write to a file. 
+    
+    Params:
+    xsd_path: str - Path to the XSD file.
+    avro_path: str - Path to the Avro file.
+    namespace: str | None - Namespace of the Avro schema.    
+    """
     xsd_to_avro = XSDToAvro()
-    xsd_to_avro.convert_xsd_to_avro(xsd_path, avro_path, namespace)
+    xsd_to_avro.convert_xsd_to_avro(xsd_path, avro_path, namespace)
```

### Comparing `avrotize-1.2.4/pyproject.toml` & `avrotize-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.4/PKG-INFO` & `avrotize-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.2.4
+Version: 1.3.0
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

