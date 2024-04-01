# Comparing `tmp/dialog2rasa-0.1.5.tar.gz` & `tmp/dialog2rasa-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog2rasa-0.1.5.tar", max compression
+gzip compressed data, was "dialog2rasa-0.1.6.tar", max compression
```

## Comparing `dialog2rasa-0.1.5.tar` & `dialog2rasa-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11347 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/LICENSE
--rw-r--r--   0        0        0     1835 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/README.md
--rw-r--r--   0        0        0      433 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/__init__.py
--rw-r--r--   0        0        0      619 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/cli.py
--rw-r--r--   0        0        0        0 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/converters/__init__.py
--rw-r--r--   0        0        0      884 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/converters/base.py
--rw-r--r--   0        0        0     1640 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/converters/core.py
--rw-r--r--   0        0        0     4765 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/converters/entity.py
--rw-r--r--   0        0        0     1958 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/converters/intent.py
--rw-r--r--   0        0        0      483 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/converters/manager.py
--rw-r--r--   0        0        0     2021 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/converters/utterance.py
--rw-r--r--   0        0        0        0 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/utils/__init__.py
--rw-r--r--   0        0        0     1118 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/utils/general.py
--rw-r--r--   0        0        0     1158 2024-03-29 19:48:22.825015 dialog2rasa-0.1.5/src/dialog2rasa/utils/io.py
--rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 dialog2rasa-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1750 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/README.md
+-rw-r--r--   0        0        0      433 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/__init__.py
+-rw-r--r--   0        0        0     1025 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/cli.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/converters/__init__.py
+-rw-r--r--   0        0        0     1011 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/converters/base.py
+-rw-r--r--   0        0        0     1606 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/converters/core.py
+-rw-r--r--   0        0        0     4624 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/converters/entity.py
+-rw-r--r--   0        0        0     2039 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/converters/intent.py
+-rw-r--r--   0        0        0      483 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/converters/manager.py
+-rw-r--r--   0        0        0     2124 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/converters/utterance.py
+-rw-r--r--   0        0        0        0 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/utils/__init__.py
+-rw-r--r--   0        0        0     1118 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/utils/general.py
+-rw-r--r--   0        0        0     1161 2024-03-29 22:50:56.875956 dialog2rasa-0.1.6/src/dialog2rasa/utils/io.py
+-rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 dialog2rasa-0.1.6/PKG-INFO
```

### Comparing `dialog2rasa-0.1.5/LICENSE` & `dialog2rasa-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dialog2rasa-0.1.5/README.md` & `dialog2rasa-0.1.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 # Dialog2Rasa Converter
 
-Transform your Dialogflow agents into Rasa format, suitable for Rasa version 3 and above. This CLI tool streamlines the migration process from Dialogflow to Rasa, ensuring a smoother transition for developers aiming to leverage Rasa's capabilities. It converts the Dialogflow export into Rasa YAML format.
+Easily convert Dialogflow agents to Rasa format for Rasa version 3+. This tool automates the migration to Rasa, converting Dialogflow exports into Rasa YAML format.
 
 ## Installation
 
-To install `dialog2rasa`, simply run:
+Install `dialog2rasa` with:
 
 ```bash
 pip install dialog2rasa
 ```
 
-For more information and details about the package, you can visit the PyPI page at: <https://pypi.org/project/dialog2rasa/>.
+For more details, visit [PyPI](https://pypi.org/project/dialog2rasa/).
 
 ## Usage
 
-After installation, convert your Dialogflow export to Rasa format using the command:
+Unzip your Dialogflow export first. Then, convert it to Rasa format with:
 
 ```sh
-dialog2rasa -p path/to/extracted/dialogflow/export
+dialog2rasa -p path/to/extracted/dialogflow/export -l language_code
 ```
 
+### Command Details
+
+- `-p PATH`: Path to the Dialogflow export’s extracted folder.
+- `-l LANGUAGE`: Language code (e.g., 'en' for English), defaults to 'de' (German).
+
+The conversion output is saved in `/output/[LANGUAGE_CODE]` within the Dialogflow agent’s directory, with `[LANGUAGE_CODE]` being the actual language code used.
+
 ## Features and Limitations
 
-- Converts Dialogflow intents, entities, and utterances to Rasa-compatible YAML format.
+- **Features**: Converts intents, entities, and utterances to Rasa YAML.
 - **Limitations**:
-  - **Compound Entities**: Does not handle compound entities directly. Instead, creates pseudo YAML files with a `__compound__` prefix.
-  - **Synonym Entities**: Groups single synonym entities within a lookup table. Entities with multiple synonyms are handled accordingly.
-  - **Output Naming**: The output NLU data is named after the agent, facilitating integration into larger projects (assuming `nlu` as a directory).
+  - Does not support compound entities directly; creates pseudo-yaml `__compound_` with prefix as workaround.
+  - Groups entities with a single synonym in a lookup table; handles entities multiple synonyms also as synonyms in Rasa.
+  - Names output NLU data after the agent for easy project integration.
+
+> Note: See `test/mockup-agent` and its reference output [here](./tests/mockup-agent) to understand these limitations.
 
 ## Contributing
 
-Feedback and contributions are welcome as we work towards making this tool more robust and versatile. For bugs, feature requests, or contributions, please open an issue or pull request.
+Your feedback and contributions are appreciated to enhance this tool. Report bugs or suggest features via issues or pull requests.
 
 ### Testing
 
-This project includes automated unit tests when distributed as a PyPi package (triggered by Github actions workflow). Please be sure to test your code and extend the tests with `pytest` before submitting a pull request. This will ensure reliability and functionality of the package.
+The package includes automated tests. Contribute by writing tests with `pytest` for your code changes to maintain functionality and reliability.
 
 ## License
 
-This project is licensed under the Apache 2.0 License.
+Licensed under the Apache 2.0 License.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dialog2rasa-0.1.5/src/dialog2rasa/converters/base.py` & `dialog2rasa-0.1.6/src/dialog2rasa/converters/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from abc import abstractmethod
+from pathlib import Path
+from typing import Optional
 
 
 class BaseConverter:
     """
     Base converter to simplify initialization. Main function are:
     1) Manipulate the strings from Dialogflow export files and;
     2) Export the output files following the RASA YAML-format.
     """
 
-    def __init__(self, agent_dir, agent_name, languages, output_file=None, sub_dir=""):
+    def __init__(
+        self,
+        agent_dir: Path,
+        agent_name: str,
+        language: str,
+        output_file: Optional[str] = None,
+        sub_dir: str = "",
+    ) -> None:
         self.agent_dir = agent_dir
         self.agent_name = agent_name
-        self.languages = languages
-        self.base_output_path = agent_dir / "output"
+        self.language = language
+        self.output_dir = agent_dir / "output" / self.language
         self.nlu_folder_path = (
-            self.base_output_path / "data" / "nlu"
-            if sub_dir == "nlu"
-            else self.base_output_path
+            self.output_dir / "data" / "nlu" if sub_dir == "nlu" else self.output_dir
         )
         self.output_file = output_file if output_file else f"{self.agent_name}.yml"
         self.output_path = self.nlu_folder_path / self.output_file
 
     @abstractmethod
     def convert(self) -> None: ...
```

### Comparing `dialog2rasa-0.1.5/src/dialog2rasa/converters/core.py` & `dialog2rasa-0.1.6/src/dialog2rasa/converters/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from pathlib import Path
+from typing import Optional
 
 from dialog2rasa.converters.base import BaseConverter
 from dialog2rasa.converters.manager import get_converter
-from dialog2rasa.utils.io import reset_directory
 from dialog2rasa.utils.general import logger
+from dialog2rasa.utils.io import reset_directory
 
 
-class DialogflowToRasaConverter:
+class DialogflowToRasaConverter(BaseConverter):
     """Converts Dialogflow agent files (.zip export) to Rasa format."""
 
-    def __init__(self, agent_dir: str, languages=("de",)) -> None:
+    def __init__(
+        self,
+        agent_dir: Path,
+        language: str,
+        output_file: Optional[str] = None,
+    ) -> None:
+        agent_name = agent_dir.name.replace("Agent-", "").replace("-", "_").lower()
+        super().__init__(agent_dir, agent_name, language, output_file, "nlu")
         """Initializes converter settings."""
-        self.agent_dir = Path(agent_dir)
-        self.languages = languages
-        self.agent_name = (
-            self.agent_dir.name.replace("Agent-", "").replace("-", "_").lower()
-        )
-        self.output_dir = self.agent_dir / "output"
-        self.lookup_path = self.output_dir / "data" / "nlu" / "lookup"
 
-    def _initialize_converters(self):
+    def _initialize_converters(self) -> None:
         """Initializes all required converters."""
         converter_types = ["intent", "utterance", "entity"]
         self.converters: dict[str, BaseConverter] = {}
         for converter_type in converter_types:
             self.converters[converter_type] = get_converter(
-                converter_type, self.agent_dir, self.agent_name, self.languages
+                converter_type, self.agent_dir, self.agent_name, self.language
             )
 
     def convert_all(self) -> None:
         """Converts all Dialogflow files to Rasa format."""
         logger.info("Starting conversion...")
         reset_directory(self.output_dir, "data/nlu/lookup")
```

### Comparing `dialog2rasa-0.1.5/src/dialog2rasa/converters/entity.py` & `dialog2rasa-0.1.6/src/dialog2rasa/converters/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,24 @@
+from pathlib import Path
+from typing import Optional
+
 from dialog2rasa.converters.base import BaseConverter
 from dialog2rasa.utils.general import camel_to_snake, logger
 from dialog2rasa.utils.io import read_json_file, write_dict_files
 
 
 class EntityConverter(BaseConverter):
-    def __init__(self, agent_dir, agent_name, languages, output_file=None):
-        super().__init__(agent_dir, agent_name, languages, output_file, "nlu")
+    def __init__(
+        self,
+        agent_dir: Path,
+        agent_name: str,
+        language: str,
+        output_file: Optional[str] = None,
+    ) -> None:
+        super().__init__(agent_dir, agent_name, language, output_file, "nlu")
         self.lookup_path = self.nlu_folder_path / "lookup"
         self.entities_path = self.agent_dir / "entities"
 
     def convert(self) -> None:
         """Processes and converts Dialogflow entities to Rasa format."""
         entity_contents = self._handle_entities()
         for entity_dict in entity_contents:
@@ -17,80 +26,77 @@
         logger.info(
             f"The entity files have been created in dir '{self.nlu_folder_path}'."
         )
 
     def _handle_entities(self) -> tuple:
         synonym_content, lookup_content, compound_content = {}, {}, {}
 
-        for lang in self.languages:
-            for entity_file in self.entities_path.glob(f"*_entries_{lang}.json"):
-                entity_name = camel_to_snake(entity_file.stem).replace(
-                    f"_entries_{lang}", ""
-                )
-                entries = read_json_file(entity_file)
-
-                for entry in entries:
-                    if any("@" in syn for syn in entry["synonyms"]):
-                        # @ refers to compound entities in dialogflow
-                        compound_file_path = (
-                            self.nlu_folder_path / f"__compound__{entity_name}.yml"
-                        )
-                        if compound_file_path not in compound_content:
-                            compound_content[compound_file_path] = (
-                                self._init_compound_file_content(entity_name)
-                            )
-                            logger.warning(
-                                "Manual adaptation needed for compound "
-                                f"entity '{entity_name}' in Rasa. "
-                                f"See file: '__compound__{entity_name}.yml'."
-                            )
-                        self._update_content(
-                            compound_content,
-                            compound_file_path,
-                            self._handle_compounds(entry),
-                        )
-
-                    elif len(entry["synonyms"]) > 1:
-                        # multiple synonyms are considered also synonyms in RASA
-                        synonyms_file_path = (
-                            self.nlu_folder_path / f"{self.agent_name}.yml"
-                        )
-                        self._update_content(
-                            synonym_content,
-                            synonyms_file_path,
-                            self._handle_synonyms(entry),
+        for entity_file in self.entities_path.glob(f"*_entries_{self.language}.json"):
+            entity_name = camel_to_snake(entity_file.stem).replace(
+                f"_entries_{self.language}", ""
+            )
+            entries = read_json_file(entity_file)
+
+            for entry in entries:
+                if any("@" in syn for syn in entry["synonyms"]):
+                    # @ refers to compound entities in dialogflow
+                    compound_file_path = (
+                        self.nlu_folder_path / f"__compound__{entity_name}.yml"
+                    )
+                    if compound_file_path not in compound_content:
+                        compound_content[compound_file_path] = (
+                            self._init_compound_file_content()
                         )
-
-                    else:
-                        # single synonyms are accumulated in lookup tables
-                        lookup_file_path = self.lookup_path / f"{entity_name}.txt"
-                        self._update_content(
-                            lookup_content,
-                            lookup_file_path,
-                            self._handle_lookup(entry, entity_name),
+                        logger.warning(
+                            "Manual adaptation needed for compound "
+                            f"entity '{entity_name}' in Rasa. "
+                            f"See file: '__compound__{entity_name}.yml'."
                         )
+                    self._update_content(
+                        compound_content,
+                        compound_file_path,
+                        self._handle_compounds(entry),
+                    )
+
+                elif len(entry["synonyms"]) > 1:
+                    # multiple synonyms are considered also synonyms in RASA
+                    synonyms_file_path = self.nlu_folder_path / f"{self.agent_name}.yml"
+                    self._update_content(
+                        synonym_content,
+                        synonyms_file_path,
+                        self._handle_synonyms(entry),
+                    )
+
+                else:
+                    # single synonyms are accumulated in lookup tables
+                    lookup_file_path = self.lookup_path / f"{entity_name}.txt"
+                    self._update_content(
+                        lookup_content,
+                        lookup_file_path,
+                        self._handle_lookup(entry),
+                    )
 
         return synonym_content, lookup_content, compound_content
 
-    def _update_content(self, content_dict, file_path, new_content):
+    def _update_content(self, content_dict: dict, file_path: Path, new_content: str):
         if file_path not in content_dict:
             content_dict[file_path] = ""
         content_dict[file_path] += new_content
 
     def _handle_synonyms(self, entry: dict) -> str:
         """Returns Rasa format string for Dialogflow synonyms."""
         synonym = entry["value"]
         examples = "\n".join(f"    - {syn}" for syn in entry["synonyms"])
         return f"- synonym: {synonym}\n  examples: |\n{examples}\n\n"
 
-    def _handle_lookup(self, entry: dict, entity_name: str) -> str:
+    def _handle_lookup(self, entry: dict) -> str:
         """Returns Rasa format string for Dialogflow lookup tables."""
         return "\n".join(entry["synonyms"]) + "\n"
 
-    def _init_compound_file_content(self, entity_name: str) -> str:
+    def _init_compound_file_content(self) -> str:
         """Returns the initial content for a new compound entity file."""
         header_content = "# Compound entity: Manual adaptation needed for Rasa\n"
         header_content += 'version: "3.1"\n\nnlu:\n'
         return header_content
 
     def _handle_compounds(self, entry: dict) -> str:
         """
```

### Comparing `dialog2rasa-0.1.5/src/dialog2rasa/converters/intent.py` & `dialog2rasa-0.1.6/src/dialog2rasa/converters/intent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,44 @@
+from pathlib import Path
+from typing import Optional
+
 from dialog2rasa.converters.base import BaseConverter
 from dialog2rasa.utils.general import camel_to_snake, logger
 from dialog2rasa.utils.io import read_json_file, write_to_file
 
 
 class IntentConverter(BaseConverter):
-    def __init__(self, agent_dir, agent_name, languages, output_file=None):
-        super().__init__(agent_dir, agent_name, languages, output_file, "nlu")
+    def __init__(
+        self,
+        agent_dir: Path,
+        agent_name: str,
+        language: str,
+        output_file: Optional[str] = None,
+    ) -> None:
+        super().__init__(agent_dir, agent_name, language, output_file, "nlu")
         self.intents_path = agent_dir / "intents"
 
     def convert(self) -> None:
         """Converts Dialogflow intents to Rasa NLU format."""
         converted_intents = self._handle_intents()
         write_to_file(self.output_path, converted_intents)
         logger.info(f"The file '{self.output_path}' has been created.")
 
     def _handle_intents(self) -> str:
         """Handles conversion of individual Dialogflow intents."""
         converted_intents = 'version: "3.1"\n\nnlu:\n'
-        for lang in self.languages:
-            intent_file_stem = f"_usersays_{lang}"
+        intent_file_stem = f"_usersays_{self.language}"
 
-            for file in sorted(self.intents_path.glob(f"*{intent_file_stem}.json")):
-                intent_name = camel_to_snake(file.stem.split(intent_file_stem)[0])
-                data = read_json_file(file)
-                examples = self._handle_examples(data)
-                converted_intents += (
-                    f"  - intent: {intent_name}\n    examples: |\n{examples}\n"
-                )
+        for file in sorted(self.intents_path.glob(f"*{intent_file_stem}.json")):
+            intent_name = camel_to_snake(file.stem.split(intent_file_stem)[0])
+            data = read_json_file(file)
+            examples = self._handle_examples(data)
+            converted_intents += (
+                f"  - intent: {intent_name}\n    examples: |\n{examples}\n"
+            )
 
         return converted_intents
 
     def _handle_examples(self, data: dict) -> str:
         """Handles conversion of Dialogflow examples to Rasa format."""
         examples = ""
         for d in data:
```

### Comparing `dialog2rasa-0.1.5/src/dialog2rasa/converters/utterance.py` & `dialog2rasa-0.1.6/src/dialog2rasa/converters/utterance.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,49 @@
+from pathlib import Path
+from typing import Optional
+
 from dialog2rasa.converters.base import BaseConverter
-from dialog2rasa.utils.io import read_json_file, write_to_file
 from dialog2rasa.utils.general import camel_to_snake, logger
+from dialog2rasa.utils.io import read_json_file, write_to_file
 
 
 class UtteranceConverter(BaseConverter):
-    def __init__(self, agent_dir, agent_name, languages, output_file="domain.yml"):
-        super().__init__(agent_dir, agent_name, languages, output_file)
+    def __init__(
+        self,
+        agent_dir: Path,
+        agent_name: str,
+        language: str,
+        output_file: Optional[str] = "domain.yml",
+    ) -> None:
+        super().__init__(agent_dir, agent_name, language, output_file)
 
     def convert(self) -> None:
         """Converts Dialogflow utterances to Rasa domain format."""
         responses_folder_path = self.agent_dir / "intents"
         converted_responses = self._handle_responses(responses_folder_path)
         write_to_file(self.output_path, converted_responses)
         logger.info(f"The file '{self.output_path}' has been created.")
 
-    def _handle_responses(self, responses_folder_path) -> str:
+    def _handle_responses(self, responses_folder_path: Path) -> str:
         """Handles conversion of Dialogflow responses to Rasa format."""
         converted_responses = "responses:\n"
         for file in sorted(responses_folder_path.iterdir()):
-            if not any(
-                file.name.endswith(f"usersays_{lang}.json") for lang in self.languages
-            ):
+            if not file.name.endswith(f"usersays_{self.language}.json"):
                 intent_name = camel_to_snake(file.stem)
                 data = read_json_file(file)
                 for response in data.get("responses", []):
                     converted_responses += self._handle_utter_message(
                         intent_name, response
                     )
         return converted_responses
 
-    def _handle_utter_message(self, intent_name, response) -> str:
+    def _handle_utter_message(self, intent_name: str, response: dict) -> str:
         """Handles conversion of individual Dialogflow utter messages."""
         converted_utter = ""
         for message in response.get("messages", []):
-            if message.get("lang") in self.languages:
+            if message.get("lang") == self.language:
                 if "speech" in message:
                     converted_utter += f"  utter_{intent_name}:\n"
                     for s in message["speech"]:
                         converted_utter += f'    - text: "{s}"\n'
                     converted_utter += "\n"
         return converted_utter
```

### Comparing `dialog2rasa-0.1.5/src/dialog2rasa/utils/general.py` & `dialog2rasa-0.1.6/src/dialog2rasa/utils/general.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
-from logging import INFO, Logger, StreamHandler
 import re
+from logging import INFO, Logger, StreamHandler
 
 
 def setup_logger() -> Logger:
     """Sets up the logger configuration."""
     # Format string including level, module, and function name
     format_str = "%(levelname)s - %(module)s - %(funcName)s - %(message)s"
```

### Comparing `dialog2rasa-0.1.5/src/dialog2rasa/utils/io.py` & `dialog2rasa-0.1.6/src/dialog2rasa/utils/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import shutil
 from pathlib import Path
+
 from dialog2rasa.utils.general import logger
 
 
 def reset_directory(dir_path: Path, deepest_subdir: str) -> None:
     """
     Deletes all files and folders in the specified directory recursively,
     then creates the specified deepest subdirectory.
@@ -12,21 +13,21 @@
     if dir_path.exists():
         logger.info(f"Clearing all contents from '{dir_path}'...")
         shutil.rmtree(dir_path)
         logger.info("Output directory cleared.")
     (dir_path / deepest_subdir).mkdir(parents=True, exist_ok=True)
 
 
-def read_json_file(file_path: str) -> dict:
+def read_json_file(file_path: Path) -> dict:
     """Reads and returns JSON data from a file."""
     with Path(file_path).open("r", encoding="utf-8") as file:
         return json.load(file)
 
 
-def write_to_file(file_path: str, content: str, mode: str = "w") -> None:
+def write_to_file(file_path: Path, content: str, mode: str = "w") -> None:
     """Writes given content to a file."""
     with Path(file_path).open(mode, encoding="utf-8") as file:
         file.write(content)
 
 
 def write_dict_files(content_dict: dict) -> None:
     """Writes given content to corresponding files."""
```

### Comparing `dialog2rasa-0.1.5/PKG-INFO` & `dialog2rasa-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 Metadata-Version: 2.1
 Name: dialog2rasa
-Version: 0.1.5
+Version: 0.1.6
 Summary: Dialogflow to Rasa > 3.0 agent converter.
 License: Apache 2.0
 Author: Murilo Bellatini
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Description-Content-Type: text/markdown
 
 # Dialog2Rasa Converter
 
-Transform your Dialogflow agents into Rasa format, suitable for Rasa version 3 and above. This CLI tool streamlines the migration process from Dialogflow to Rasa, ensuring a smoother transition for developers aiming to leverage Rasa's capabilities. It converts the Dialogflow export into Rasa YAML format.
+Easily convert Dialogflow agents to Rasa format for Rasa version 3+. This tool automates the migration to Rasa, converting Dialogflow exports into Rasa YAML format.
 
 ## Installation
 
-To install `dialog2rasa`, simply run:
+Install `dialog2rasa` with:
 
 ```bash
 pip install dialog2rasa
 ```
 
-For more information and details about the package, you can visit the PyPI page at: <https://pypi.org/project/dialog2rasa/>.
+For more details, visit [PyPI](https://pypi.org/project/dialog2rasa/).
 
 ## Usage
 
-After installation, convert your Dialogflow export to Rasa format using the command:
+Unzip your Dialogflow export first. Then, convert it to Rasa format with:
 
 ```sh
-dialog2rasa -p path/to/extracted/dialogflow/export
+dialog2rasa -p path/to/extracted/dialogflow/export -l language_code
 ```
 
+### Command Details
+
+- `-p PATH`: Path to the Dialogflow export’s extracted folder.
+- `-l LANGUAGE`: Language code (e.g., 'en' for English), defaults to 'de' (German).
+
+The conversion output is saved in `/output/[LANGUAGE_CODE]` within the Dialogflow agent’s directory, with `[LANGUAGE_CODE]` being the actual language code used.
+
 ## Features and Limitations
 
-- Converts Dialogflow intents, entities, and utterances to Rasa-compatible YAML format.
+- **Features**: Converts intents, entities, and utterances to Rasa YAML.
 - **Limitations**:
-  - **Compound Entities**: Does not handle compound entities directly. Instead, creates pseudo YAML files with a `__compound__` prefix.
-  - **Synonym Entities**: Groups single synonym entities within a lookup table. Entities with multiple synonyms are handled accordingly.
-  - **Output Naming**: The output NLU data is named after the agent, facilitating integration into larger projects (assuming `nlu` as a directory).
+  - Does not support compound entities directly; creates pseudo-yaml `__compound_` with prefix as workaround.
+  - Groups entities with a single synonym in a lookup table; handles entities multiple synonyms also as synonyms in Rasa.
+  - Names output NLU data after the agent for easy project integration.
+
+> Note: See `test/mockup-agent` and its reference output [here](./tests/mockup-agent) to understand these limitations.
 
 ## Contributing
 
-Feedback and contributions are welcome as we work towards making this tool more robust and versatile. For bugs, feature requests, or contributions, please open an issue or pull request.
+Your feedback and contributions are appreciated to enhance this tool. Report bugs or suggest features via issues or pull requests.
 
 ### Testing
 
-This project includes automated unit tests when distributed as a PyPi package (triggered by Github actions workflow). Please be sure to test your code and extend the tests with `pytest` before submitting a pull request. This will ensure reliability and functionality of the package.
+The package includes automated tests. Contribute by writing tests with `pytest` for your code changes to maintain functionality and reliability.
 
 ## License
 
-This project is licensed under the Apache 2.0 License.
+Licensed under the Apache 2.0 License.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

