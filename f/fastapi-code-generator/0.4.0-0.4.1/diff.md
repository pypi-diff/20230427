# Comparing `tmp/fastapi_code_generator-0.4.0.tar.gz` & `tmp/fastapi_code_generator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_code_generator-0.4.0.tar", max compression
+gzip compressed data, was "fastapi_code_generator-0.4.1.tar", max compression
```

## Comparing `fastapi_code_generator-0.4.0.tar` & `fastapi_code_generator-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-01-17 16:26:24.586467 fastapi_code_generator-0.4.0/LICENSE
--rw-r--r--   0        0        0     9643 2023-01-17 16:26:24.586467 fastapi_code_generator-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-01-17 16:26:24.586467 fastapi_code_generator-0.4.0/fastapi_code_generator/__init__.py
--rw-r--r--   0        0        0     6020 2023-01-17 16:26:24.586467 fastapi_code_generator-0.4.0/fastapi_code_generator/__main__.py
--rw-r--r--   0        0        0    16521 2023-01-17 16:26:24.586467 fastapi_code_generator-0.4.0/fastapi_code_generator/parser.py
--rw-r--r--   0        0        0     1139 2023-01-17 16:26:24.586467 fastapi_code_generator-0.4.0/fastapi_code_generator/template/main.jinja2
--rw-r--r--   0        0        0      178 2023-01-17 16:26:24.586467 fastapi_code_generator-0.4.0/fastapi_code_generator/visitor.py
--rw-r--r--   0        0        0     1232 2023-01-17 16:26:24.586467 fastapi_code_generator-0.4.0/fastapi_code_generator/visitors/imports.py
--rw-r--r--   0        0        0      449 2023-01-17 16:26:24.586467 fastapi_code_generator-0.4.0/fastapi_code_generator/visitors/operations.py
--rw-r--r--   0        0        0     2199 2023-01-17 16:27:14.706616 fastapi_code_generator-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    11228 1970-01-01 00:00:00.000000 fastapi_code_generator-0.4.0/setup.py
--rw-r--r--   0        0        0    11107 1970-01-01 00:00:00.000000 fastapi_code_generator-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-02-15 15:28:41.828496 fastapi_code_generator-0.4.1/LICENSE
+-rw-r--r--   0        0        0     9643 2023-02-15 15:28:41.828496 fastapi_code_generator-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-02-15 15:28:41.828496 fastapi_code_generator-0.4.1/fastapi_code_generator/__init__.py
+-rw-r--r--   0        0        0     6276 2023-02-15 15:28:41.828496 fastapi_code_generator-0.4.1/fastapi_code_generator/__main__.py
+-rw-r--r--   0        0        0    17015 2023-02-15 15:28:41.828496 fastapi_code_generator-0.4.1/fastapi_code_generator/parser.py
+-rw-r--r--   0        0        0     1139 2023-02-15 15:28:41.828496 fastapi_code_generator-0.4.1/fastapi_code_generator/template/main.jinja2
+-rw-r--r--   0        0        0      178 2023-02-15 15:28:41.828496 fastapi_code_generator-0.4.1/fastapi_code_generator/visitor.py
+-rw-r--r--   0        0        0     1232 2023-02-15 15:28:41.828496 fastapi_code_generator-0.4.1/fastapi_code_generator/visitors/imports.py
+-rw-r--r--   0        0        0      449 2023-02-15 15:28:41.828496 fastapi_code_generator-0.4.1/fastapi_code_generator/visitors/operations.py
+-rw-r--r--   0        0        0     2199 2023-02-15 15:29:26.228226 fastapi_code_generator-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    11228 1970-01-01 00:00:00.000000 fastapi_code_generator-0.4.1/setup.py
+-rw-r--r--   0        0        0    11107 1970-01-01 00:00:00.000000 fastapi_code_generator-0.4.1/PKG-INFO
```

### Comparing `fastapi_code_generator-0.4.0/LICENSE` & `fastapi_code_generator-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_code_generator-0.4.0/README.md` & `fastapi_code_generator-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_code_generator-0.4.0/fastapi_code_generator/__main__.py` & `fastapi_code_generator-0.4.1/fastapi_code_generator/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     template_dir: Optional[Path] = typer.Option(None, "--template-dir", "-t"),
     enum_field_as_literal: Optional[LiteralType] = typer.Option(
         None, "--enum-field-as-literal"
     ),
     custom_visitors: Optional[List[Path]] = typer.Option(
         None, "--custom-visitor", "-c"
     ),
+    disable_timestamp: bool = typer.Option(False, "--disable-timestamp"),
 ) -> None:
     input_name: str = input_file.name
     input_text: str = input_file.read()
     if model_file:
         model_path = Path(model_file).with_suffix('.py')
     else:
         model_path = MODEL_PATH
@@ -57,22 +58,24 @@
         return generate_code(
             input_name,
             input_text,
             output_dir,
             template_dir,
             model_path,
             enum_field_as_literal,
+            disable_timestamp=disable_timestamp,
         )
     return generate_code(
         input_name,
         input_text,
         output_dir,
         template_dir,
         model_path,
         custom_visitors=custom_visitors,
+        disable_timestamp=disable_timestamp,
     )
 
 
 def _get_most_of_reference(data_type: DataType) -> Optional[Reference]:
     if data_type.reference:
         return data_type.reference
     for data_type in data_type.data_types:
@@ -86,14 +89,15 @@
     input_name: str,
     input_text: str,
     output_dir: Path,
     template_dir: Optional[Path],
     model_path: Optional[Path] = None,
     enum_field_as_literal: Optional[str] = None,
     custom_visitors: Optional[List[Path]] = [],
+    disable_timestamp: bool = False,
 ) -> None:
     if not model_path:
         model_path = MODEL_PATH
     if not output_dir.exists():
         output_dir.mkdir(parents=True)
     if not template_dir:
         template_dir = BUILTIN_TEMPLATE_DIR
@@ -144,28 +148,29 @@
         template = environment.get_template(str(relative_path))
         result = template.render(template_vars)
         results[relative_path] = code_formatter.format_code(result)
 
     timestamp = datetime.now(timezone.utc).replace(microsecond=0).isoformat()
     header = f"""\
 # generated by fastapi-codegen:
-#   filename:  {Path(input_name).name}
-#   timestamp: {timestamp}"""
+#   filename:  {Path(input_name).name}"""
+    if not disable_timestamp:
+        header += f"\n#   timestamp: {timestamp}"
 
     for path, code in results.items():
         with output_dir.joinpath(path.with_suffix(".py")).open("wt") as file:
             print(header, file=file)
             print("", file=file)
             print(code.rstrip(), file=file)
 
     header = f'''\
 # generated by fastapi-codegen:
 #   filename:  {{filename}}'''
-    #     if not disable_timestamp:
-    header += f'\n#   timestamp: {timestamp}'
+    if not disable_timestamp:
+        header += f'\n#   timestamp: {timestamp}'
 
     for path, body_and_filename in modules.items():
         body, filename = body_and_filename
         if path is None:
             file = None
         else:
             if not path.parent.exists():
```

### Comparing `fastapi_code_generator-0.4.0/fastapi_code_generator/parser.py` & `fastapi_code_generator-0.4.1/fastapi_code_generator/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,14 +374,25 @@
                             type_hint='Request',  # type: ignore
                             required=True,
                         )
                     )
                     self.imports_for_fastapi.append(
                         Import.from_full_path('starlette.requests.Request')
                     )
+                elif media_type == 'application/octet-stream':
+                    arguments.append(
+                        Argument(
+                            name='file',  # type: ignore
+                            type_hint='UploadFile',  # type: ignore
+                            required=True,
+                        )
+                    )
+                    self.imports_for_fastapi.append(
+                        Import.from_full_path("fastapi.UploadFile")
+                    )
         self._temporary_operation['_request'] = arguments[0] if arguments else None
 
     def parse_responses(
         self,
         name: str,
         responses: Dict[str, Union[ResponseObject, ReferenceObject]],
         path: List[str],
```

### Comparing `fastapi_code_generator-0.4.0/fastapi_code_generator/template/main.jinja2` & `fastapi_code_generator-0.4.1/fastapi_code_generator/template/main.jinja2`

 * *Files identical despite different names*

### Comparing `fastapi_code_generator-0.4.0/fastapi_code_generator/visitors/imports.py` & `fastapi_code_generator-0.4.1/fastapi_code_generator/visitors/imports.py`

 * *Files identical despite different names*

### Comparing `fastapi_code_generator-0.4.0/pyproject.toml` & `fastapi_code_generator-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-code-generator"
-version = "0.4.0"
+version = "0.4.1"
 description = ""
 authors = ["Koudai Aono <koxudaxi@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/koxudaxi/fastapi-code-generator"
 repository = "https://github.com/koxudaxi/fastapi-code-generator"
 
@@ -26,15 +26,15 @@
 
 [tool.poetry.scripts]
 fastapi-codegen = "fastapi_code_generator.__main__:app"
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
 typer = {extras = ["all"], version = ">=0.2.1,<0.7.0"}
-datamodel-code-generator =  {extras = ["http"], version = "0.16.0"}
+datamodel-code-generator =  {extras = ["http"], version = "0.16.1"}
 stringcase = "^1.2.0"
 PySnooper = ">=0.4.1,<1.2.0"
 jinja2 = ">=2.11.2,<4.0.0"
 pydantic = "^1.5.1"
 typed-ast = [
     {version = ">=1.5.0", python = ">=3.9.8"},
     {version = ">=1.4.2", python = "<3.9.8"},
```

### Comparing `fastapi_code_generator-0.4.0/setup.py` & `fastapi_code_generator-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 ['fastapi_code_generator', 'fastapi_code_generator.visitors']
 
 package_data = \
 {'': ['*'], 'fastapi_code_generator': ['template/*']}
 
 install_requires = \
 ['PySnooper>=0.4.1,<1.2.0',
- 'datamodel-code-generator[http]==0.16.0',
+ 'datamodel-code-generator[http]==0.16.1',
  'jinja2>=2.11.2,<4.0.0',
  'pydantic>=1.5.1,<2.0.0',
  'stringcase>=1.2.0,<2.0.0',
  'typer[all]>=0.2.1,<0.7.0']
 
 extras_require = \
 {':python_full_version < "3.9.8"': ['typed-ast>=1.4.2'],
  ':python_full_version >= "3.9.8"': ['typed-ast>=1.5.0']}
 
 entry_points = \
 {'console_scripts': ['fastapi-codegen = fastapi_code_generator.__main__:app']}
 
 setup_kwargs = {
     'name': 'fastapi-code-generator',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': '',
     'long_description': '# fastapi-code-generator\n\nThis code generator creates a FastAPI app from an openapi file.\n\n[![PyPI version](https://badge.fury.io/py/fastapi-code-generator.svg)](https://pypi.python.org/pypi/fastapi-code-generator)\n[![Downloads](https://pepy.tech/badge/fastapi-code-generator/month)](https://pepy.tech/project/fastapi-code-generator)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-code-generator)](https://pypi.python.org/pypi/fastapi-code-generator)\n[![codecov](https://codecov.io/gh/koxudaxi/fastapi-code-generator/branch/master/graph/badge.svg)](https://codecov.io/gh/koxudaxi/fastapi-code-generator)\n![license](https://img.shields.io/github/license/koxudaxi/fastapi-code-generator.svg)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\n## This project is in experimental phase.\n\nfastapi-code-generator uses [datamodel-code-generator](https://github.com/koxudaxi/datamodel-code-generator) to generate pydantic models\n\n## Help\nSee [documentation](https://koxudaxi.github.io/fastapi-code-generator) for more details.\n\n\n## Installation\n\nTo install `fastapi-code-generator`:\n```sh\n$ pip install fastapi-code-generator\n```\n\n## Usage\n\nThe `fastapi-code-generator` command:\n```\nUsage: fastapi-codegen [OPTIONS]\n\nOptions:\n  -i, --input FILENAME     [required]\n  -o, --output PATH        [required]\n  -t, --template-dir PATH\n  -m, --model-file         Specify generated model file path + name, if not default to models.py\n  -c, --custom-visitors    PATH - A custom visitor that adds variables to the template.\n  --install-completion     Install completion for the current shell.\n  --show-completion        Show completion for the current shell, to copy it\n                           or customize the installation.\n\n  --help                   Show this message and exit.\n```\n\n## Example\n### OpenAPI\n```sh\n$ fastapi-codegen --input api.yaml --output app\n```\n\n<details>\n<summary>api.yaml</summary>\n<pre>\n<code>\nopenapi: "3.0.0"\ninfo:\n  version: 1.0.0\n  title: Swagger Petstore\n  license:\n    name: MIT\nservers:\n  - url: http://petstore.swagger.io/v1\npaths:\n  /pets:\n    get:\n      summary: List all pets\n      operationId: listPets\n      tags:\n        - pets\n      parameters:\n        - name: limit\n          in: query\n          description: How many items to return at one time (max 100)\n          required: false\n          schema:\n            type: integer\n            format: int32\n      responses:\n        \'200\':\n          description: A paged array of pets\n          headers:\n            x-next:\n              description: A link to the next page of responses\n              schema:\n                type: string\n          content:\n            application/json:\n              schema:\n                $ref: "#/components/schemas/Pets"\n        default:\n          description: unexpected error\n          content:\n            application/json:\n              schema:\n                $ref: "#/components/schemas/Error"\n                x-amazon-apigateway-integration:\n                  uri:\n                    Fn::Sub: arn:aws:apigateway:${AWS::Region}:lambda:path/2015-03-31/functions/${PythonVersionFunction.Arn}/invocations\n                  passthroughBehavior: when_no_templates\n                  httpMethod: POST\n                  type: aws_proxy\n    post:\n      summary: Create a pet\n      operationId: createPets\n      tags:\n        - pets\n      responses:\n        \'201\':\n          description: Null response\n        default:\n          description: unexpected error\n          content:\n            application/json:\n              schema:\n                $ref: "#/components/schemas/Error"\n                x-amazon-apigateway-integration:\n                  uri:\n                    Fn::Sub: arn:aws:apigateway:${AWS::Region}:lambda:path/2015-03-31/functions/${PythonVersionFunction.Arn}/invocations\n                  passthroughBehavior: when_no_templates\n                  httpMethod: POST\n                  type: aws_proxy\n  /pets/{petId}:\n    get:\n      summary: Info for a specific pet\n      operationId: showPetById\n      tags:\n        - pets\n      parameters:\n        - name: petId\n          in: path\n          required: true\n          description: The id of the pet to retrieve\n          schema:\n            type: string\n      responses:\n        \'200\':\n          description: Expected response to a valid request\n          content:\n            application/json:\n              schema:\n                $ref: "#/components/schemas/Pets"\n        default:\n          description: unexpected error\n          content:\n            application/json:\n              schema:\n                $ref: "#/components/schemas/Error"\n    x-amazon-apigateway-integration:\n      uri:\n        Fn::Sub: arn:aws:apigateway:${AWS::Region}:lambda:path/2015-03-31/functions/${PythonVersionFunction.Arn}/invocations\n      passthroughBehavior: when_no_templates\n      httpMethod: POST\n      type: aws_proxy\ncomponents:\n  schemas:\n    Pet:\n      required:\n        - id\n        - name\n      properties:\n        id:\n          type: integer\n          format: int64\n        name:\n          type: string\n        tag:\n          type: string\n    Pets:\n      type: array\n      description: list of pet\n      items:\n        $ref: "#/components/schemas/Pet"\n    Error:\n      required:\n        - code\n        - message\n      properties:\n        code:\n          type: integer\n          format: int32\n        message:\n          type: string\n</code>\n</pre>\n</details>\n\n\n`app/main.py`:\n```python\n# generated by fastapi-codegen:\n#   filename:  api.yaml\n#   timestamp: 2020-06-14T10:45:22+00:00\n\nfrom __future__ import annotations\n\nfrom typing import Optional\n\nfrom fastapi import FastAPI, Query\n\nfrom .models import Pets\n\napp = FastAPI(version="1.0.0", title="Swagger Petstore", license="{\'name\': \'MIT\'}",)\n\n\n@app.get(\'/pets\', response_model=Pets)\ndef list_pets(limit: Optional[int] = None) -> Pets:\n    """\n    List all pets\n    """\n    pass\n\n\n@app.post(\'/pets\', response_model=None)\ndef create_pets() -> None:\n    """\n    Create a pet\n    """\n    pass\n\n\n@app.get(\'/pets/{pet_id}\', response_model=Pets)\ndef show_pet_by_id(pet_id: str = Query(..., alias=\'petId\')) -> Pets:\n    """\n    Info for a specific pet\n    """\n    pass\n\n```\n\n`app/models.py`:\n```python\n# generated by datamodel-codegen:\n#   filename:  api.yaml\n#   timestamp: 2020-06-14T10:45:22+00:00\n\nfrom typing import List, Optional\n\nfrom pydantic import BaseModel, Field\n\n\nclass Pet(BaseModel):\n    id: int\n    name: str\n    tag: Optional[str] = None\n\n\nclass Pets(BaseModel):\n    __root__: List[Pet] = Field(..., description=\'list of pet\')\n\n\nclass Error(BaseModel):\n    code: int\n    message: str\n```\n\n## Custom Template\nIf you want to generate custom `*.py` files then you can give a custom template directory to fastapi-code-generator with `-t` or `--template-dir` options of the command.\n\nfastapi-code-generator will search for [jinja2](https://jinja.palletsprojects.com/) template files in given template directory, for example `some_jinja_templates/list_pets.py`.\n\n```bash\nfastapi-code-generator --template-dir some_jinja_templates --output app --input api.yaml\n```\n\nThese files will be rendered and written to the output directory. Also, the generated file names will be created with the template name and extension of `*.py`, for example `app/list_pets.py` will be a separate file generated from the jinja template alongside the default `app/main.py`\n\n### Variables\nYou can use the following variables in the jinja2 templates\n\n- `imports`  all imports statements\n- `info`  all info statements\n- `operations` `operations` is list of `operation`\n  - `operation.type` HTTP METHOD\n  - `operation.path` Path\n  - `operation.snake_case_path` Snake-cased Path\n  - `operation.response` response object\n  - `operation.function_name` function name is created `operationId` or `METHOD` + `Path` \n  - `operation.snake_case_arguments` Snake-cased function arguments\n  - `operation.security` [Security](https://swagger.io/docs/specification/authentication/)\n  - `operation.summary` a summary\n  - `operation.tags` [Tags](https://swagger.io/docs/specification/grouping-operations-with-tags/)\n\n### default template \n`main.jinja2`\n```jinja2\nfrom __future__ import annotations\n\nfrom fastapi import FastAPI\n\n{{imports}}\n\napp = FastAPI(\n    {% if info %}\n    {% for key,value in info.items() %}\n    {{ key }} = "{{ value }}",\n    {% endfor %}\n    {% endif %}\n    )\n\n\n{% for operation in operations %}\n@app.{{operation.type}}(\'{{operation.snake_case_path}}\', response_model={{operation.response}})\ndef {{operation.function_name}}({{operation.snake_case_arguments}}) -> {{operation.response}}:\n    {%- if operation.summary %}\n    """\n    {{ operation.summary }}\n    """\n    {%- endif %}\n    pass\n{% endfor %}\n\n```\n\n## Custom Visitors\n\nCustom visitors allow you to pass custom variables to your custom templates.\n\nE.g.\n\n### custom template\n`custom-template.jinja2`\n```jinja2\n#{ % custom_header %}\nfrom __future__ import annotations\n\nfrom fastapi import FastAPI\n\n...\n```\n\n### custom visitor\n`custom-visitor.py`\n```python\nfrom typing import Dict, Optional\n\nfrom fastapi_code_generator.parser import OpenAPIParser\nfrom fastapi_code_generator.visitor import Visitor\n\n\ndef custom_visitor(parser: OpenAPIParser, model_path: Path) -> Dict[str, object]:\n    return {\'custom_header\': \'My header\'}\n\n\nvisit: Visitor = custom_visitor\n```\n\n## PyPi \n\n[https://pypi.org/project/fastapi-code-generator](https://pypi.org/project/fastapi-code-generator)\n\n## License\n\nfastapi-code-generator is released under the MIT License. http://www.opensource.org/licenses/mit-license\n\n',
     'author': 'Koudai Aono',
     'author_email': 'koxudaxi@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/koxudaxi/fastapi-code-generator',
```

### Comparing `fastapi_code_generator-0.4.0/PKG-INFO` & `fastapi_code_generator-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-code-generator
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Home-page: https://github.com/koxudaxi/fastapi-code-generator
 License: MIT
 Author: Koudai Aono
 Author-email: koxudaxi@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: PySnooper (>=0.4.1,<1.2.0)
-Requires-Dist: datamodel-code-generator[http] (==0.16.0)
+Requires-Dist: datamodel-code-generator[http] (==0.16.1)
 Requires-Dist: jinja2 (>=2.11.2,<4.0.0)
 Requires-Dist: pydantic (>=1.5.1,<2.0.0)
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Requires-Dist: typed-ast (>=1.4.2) ; python_full_version < "3.9.8"
 Requires-Dist: typed-ast (>=1.5.0) ; python_full_version >= "3.9.8"
 Requires-Dist: typer[all] (>=0.2.1,<0.7.0)
 Project-URL: Repository, https://github.com/koxudaxi/fastapi-code-generator
```

