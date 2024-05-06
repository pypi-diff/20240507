# Comparing `tmp/rigging-0.2.2.tar.gz` & `tmp/rigging-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigging-0.2.2.tar", max compression
+gzip compressed data, was "rigging-1.0.0rc0.tar", max compression
```

## Comparing `rigging-0.2.2.tar` & `rigging-1.0.0rc0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-04-25 15:43:17.481841 rigging-0.2.2/LICENSE
--rw-r--r--   0        0        0     6803 2024-04-25 15:43:17.481841 rigging-0.2.2/README.md
--rw-r--r--   0        0        0     1842 2024-04-25 15:43:17.481841 rigging-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      536 2024-04-25 15:43:17.481841 rigging-0.2.2/rigging/__init__.py
--rw-r--r--   0        0        0    14218 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/chat.py
--rw-r--r--   0        0        0      457 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/error.py
--rw-r--r--   0        0        0     5068 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/generator.py
--rw-r--r--   0        0        0     1501 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/logging.py
--rw-r--r--   0        0        0     8077 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/message.py
--rw-r--r--   0        0        0     8682 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/model.py
--rw-r--r--   0        0        0     1090 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/prompt.py
--rw-r--r--   0        0        0        0 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/py.typed
--rw-r--r--   0        0        0     8455 2024-04-25 15:43:17.485841 rigging-0.2.2/rigging/tool.py
--rw-r--r--   0        0        0     7536 1970-01-01 00:00:00.000000 rigging-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-06 23:20:05.140907 rigging-1.0.0rc0/LICENSE
+-rw-r--r--   0        0        0     1477 2024-05-06 23:20:05.140907 rigging-1.0.0rc0/README.md
+-rw-r--r--   0        0        0     2146 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      684 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/__init__.py
+-rw-r--r--   0        0        0    39816 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/chat.py
+-rw-r--r--   0        0        0    21074 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/completion.py
+-rw-r--r--   0        0        0      865 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/error.py
+-rw-r--r--   0        0        0    19110 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/generator.py
+-rw-r--r--   0        0        0     2349 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/logging.py
+-rw-r--r--   0        0        0    13107 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/message.py
+-rw-r--r--   0        0        0    12573 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/model.py
+-rw-r--r--   0        0        0     3748 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/parsing.py
+-rw-r--r--   0        0        0     1090 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/prompt.py
+-rw-r--r--   0        0        0        0 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/py.typed
+-rw-r--r--   0        0        0    10210 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/tool.py
+-rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 rigging-1.0.0rc0/PKG-INFO
```

### Comparing `rigging-0.2.2/LICENSE` & `rigging-1.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `rigging-0.2.2/pyproject.toml` & `rigging-1.0.0rc0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 [tool.poetry]
 name = "rigging"
-version = "0.2.2"
+version = "1.0.0rc0"
 description = "LLM Interaction Framework"
 authors = ["Nick Landers <monoxgas@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/dreadnode/rigging"
 readme = "README.md"
+packages = [
+    {include = "rigging"}
+]
 
 [tool.poetry.dependencies]
 python = "<3.13,>=3.10"
 pydantic = "2.5.3"
 pydantic-xml = "2.7.0"
 loguru = "^0.7.2"
 litellm = "1.35.21"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.27.1"
 mypy = "^1.8.0"
 ruff = "^0.1.14"
 pytest = "^8.0.0"
 
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.6.0"
+mkdocs-material = {extras = ["imaging"], version = "^9.5.20"}
+mkdocstrings = "^0.25.0"
+mkdocstrings-python = "^1.10.0"
+mkdocs-section-index = "^0.3.9"
+pymdown-extensions = "^10.8.1"
+pygments = "^2.18.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::DeprecationWarning"]
```

### Comparing `rigging-0.2.2/rigging/logging.py` & `rigging-1.0.0rc0/rigging/logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+We use loguru for logging. This module provides a function to configure the logging settings.
+
+To enable rigging logging, call `logger.enable("rigging")` after importing the module.
+"""
+
 import pathlib
 import sys
 import typing as t
 
 from loguru import logger
 
 g_configured: bool = False
@@ -11,14 +17,28 @@
 
 
 def configure_logging(
     log_level: str,
     log_file: pathlib.Path | None = None,
     log_file_level: LogLevelLiteral = "debug",
 ) -> None:
+    """
+    Configures the loguru settings for the rigging module.
+
+    This is optional, and calling `logger.enable("rigging")` will enable the logging
+    and you can control the formatting and log levels using the loguru API.
+
+    Args:
+        log_level: The desired log level. Valid values are 'TRACE', 'DEBUG', 'INFO',
+            'SUCCESS', 'WARNING', 'ERROR', and 'CRITICAL'.
+        log_file: The path to the log file. If None, logging
+            will only be done to the console.
+        log_file_level: The log level for the log file. Valid values
+            are 'TRACE', 'DEBUG', 'INFO', 'SUCCESS', 'WARNING', 'ERROR', and 'CRITICAL'.
+    """
     global g_configured
 
     if g_configured:
         return
 
     logger.enable("rigging")
```

### Comparing `rigging-0.2.2/rigging/model.py` & `rigging-1.0.0rc0/rigging/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+"""
+Models are the core datatypes for structured parsing.
+"""
+
 import re
 import typing as t
 from xml.etree import ElementTree as ET
 
 from pydantic import ValidationError, field_validator
 from pydantic.alias_generators import to_snake
 from pydantic_xml import BaseXmlModel
 from pydantic_xml import attr as attr
 from pydantic_xml import element as element
 from pydantic_xml import wrapped as wrapped
 from pydantic_xml.element import SearchMode  # type: ignore [attr-defined]
-from pydantic_xml.typedefs import NsMap
+from pydantic_xml.typedefs import EntityLocation, NsMap
 
 from rigging.error import MissingModelError
 
 #
 # Core XML serializable models for messages
 #
 
@@ -23,14 +27,33 @@
 # It's strictness for parsing XML and expecting all interior
 # content to be escaped. We should probably just write something
 # custom for our use case that supports JSON, YAML, and XML
 
 BASIC_TYPES = [int, str, float, bool]
 
 
+def escape_xml(xml_string: str) -> str:
+    prepared = re.sub(r"&(?!(?:amp|lt|gt|apos|quot);)", "&amp;", xml_string)
+
+    return prepared
+
+
+def unescape_xml(xml_string: str) -> str:
+    # We only expect to use this in our "simple"
+    # models, but I'd like a better long-term solution
+
+    unescaped = re.sub(r"&amp;", "&", xml_string)
+    unescaped = re.sub(r"&lt;", "<", unescaped)
+    unescaped = re.sub(r"&gt;", ">", unescaped)
+    unescaped = re.sub(r"&apos;", "'", unescaped)
+    unescaped = re.sub(r"&quot;", '"', unescaped)
+
+    return unescaped
+
+
 class XmlTagDescriptor:
     def __get__(self, _: t.Any, owner: t.Any) -> str:
         return to_snake(next(iter(owner.mro())).__name__).replace("_", "-")
 
 
 class Model(BaseXmlModel):
     def __init_subclass__(
@@ -50,67 +73,124 @@
         # Some models appear to do better if the separator is a dash
         # instead of a underscore, and users are free to override
         # as needed.
         super().__init_subclass__(tag, ns, nsmap, ns_attrs, skip_empty, search_mode, **kwargs)
         cls.__xml_tag__ = XmlTagDescriptor()  # type: ignore [assignment]
 
     # to_xml() doesn't prettify normally, and extended
-    # requirements like lxml seemed like poor form
+    # requirements like lxml seemed like poor form for
+    # just this feature
     def to_pretty_xml(self) -> str:
+        """
+        Converts the model to a pretty XML string with indents and newlines.
+
+        Returns:
+            The pretty XML representation of the model.
+        """
         tree = self.to_xml_tree()
         ET.indent(tree, "   ")
         pretty_encoded_xml = ET.tostring(tree).decode()
 
-        # TODO: I didn't note why this edge case is here, but it makes
-        # me nervous - should investigate and remove if possible
         if self.__class__.is_simple():
-            return pretty_encoded_xml.replace("&lt;", "<").replace("&gt;", ">")
+            return unescape_xml(pretty_encoded_xml)
         else:
             return pretty_encoded_xml
 
     # XML parsing gets weird when the interior text contains tags like <br>.
     # Essentially it assumes all the text is valid XML first, then parses.
     # So we'll handle easy cases here and mark the model as "simple"
     # if it only contains a single basic field. It makes our parsing
     # much more consistent and is likely the most popular model type.
+    #
+    # TODO: lxml with the recover option is likely a better approach
     @classmethod
     def is_simple(cls) -> bool:
+        """
+        Check if the model is "simple", meaning it has a single field with a basic datatype.
+
+        Until we refactor our XML parsing, this helps make the parsing more consistent for models
+        which can support it.
+
+        Returns:
+            True if the model is simple, False otherwise.
+        """
         field_values = list(cls.model_fields.values())
         return len(field_values) == 1 and field_values[0].annotation in BASIC_TYPES
 
     @classmethod
     def xml_start_tag(cls) -> str:
+        """Helper method which wrapped the class tag in XML braces."""
         return f"<{cls.__xml_tag__}>"
 
     @classmethod
     def xml_end_tag(cls) -> str:
+        """Helper method which wrapped the class tag in XML braces with a leading slash."""
         return f"</{cls.__xml_tag__}>"
 
     @classmethod
     def xml_tags(cls) -> str:
+        """Helper method which returns the full XML tags for the class."""
         return cls.xml_start_tag() + cls.xml_end_tag()
 
     # This can be overridden to provide a more complex example
     # to a model when it's required.
     @classmethod
     def xml_example(cls) -> str:
+        """
+        Returns an example XML representation of the given class.
+
+        Models should typically override this method to provide a more complex example.
+
+        By default, this method just returns the XML tags for the class.
+
+        Returns:
+            A string containing the XML representation of the class.
+        """
         return cls.xml_tags()
 
+    @classmethod
+    def ensure_valid(cls) -> None:
+        # Do a sanity check for models with a single
+        # attr field, which our parsing currently doesn't support
+        #
+        # TODO: Add support for <thing attr="value" /> style models
+
+        if len(cls.model_fields) == 1:
+            field_info = next(iter(cls.model_fields.values()))
+            if hasattr(field_info, "location") and field_info.location == EntityLocation.ATTRIBUTE:
+                raise ValueError(f"Model '{cls.__name__}' has a single attr() field which is not supported")
+
     # Attempt to extract this object from an arbitrary string
     # which may contain other XML elements or text, returns
     # the object and the string from which is was parsed.
     #
     # The potential complexities here are many, models might
     # return partial tags, multiple copies of our tags, or
     # nested tags inside others. We try to do our best to
     # parse for all the edge cases -> see the note above
     # about migrating from pydantic-xml
 
     @classmethod
     def from_text(cls, content: str) -> list[tuple[ModelT, slice]]:
+        """
+        The core parsing method which attempts to extract and parse as many
+        valid instances of a model from semi-structured text.
+
+        Args:
+            content: The text content to parse.
+
+        Returns:
+            A list of tuples containing the extracted models and their corresponding slices.
+
+        Raises:
+            MissingModelError: If the specified model tags are not found in the message.
+            ValidationError: If an error occurs while parsing the content.
+        """
+        cls.ensure_valid()
+
         pattern = r"(<([\w-]+).*?>((.*?)</\2>))"
         matches = [m for m in re.finditer(pattern, content, flags=re.DOTALL) if m.group(2) == cls.__xml_tag__]
 
         if not matches:
             raise MissingModelError(f"Failed to find '{cls.xml_tags()}' in message")
 
         # Sort matches_with_tag based on the length of the interior text,
@@ -125,38 +205,58 @@
 
             # The model might trip up regex by including partial tags
             # in passing before actually using them. We'll continually try
             # to parse the inner text until we can't extract our model anymore.
             #
             # Example: "Sure I'll use <answer> tags: <answer>hello</answer>"
             #
+            # TODO: The opposite could be true, and we could greedily parse
+            # backwards if we get failures. This is a simple solution for now.
+
             inner_match: re.Match[str] | None = match
             while inner_match is not None:
                 inner_matches = re.finditer(pattern, inner_with_end_tag, flags=re.DOTALL)
                 inner_match = next((m for m in inner_matches if m.group(2) == cls.__xml_tag__), None)
                 if inner_match is not None:
                     full_text, _, inner_with_end_tag, inner = inner_match.groups()
 
             try:
-                model = cls(**{next(iter(cls.model_fields)): inner}) if cls.is_simple() else cls.from_xml(full_text)
+                model = (
+                    cls(**{next(iter(cls.model_fields)): inner})
+                    if cls.is_simple()
+                    else cls.from_xml(escape_xml(full_text))
+                )
                 extracted.append((model, slice(match.start(), match.end())))  # type: ignore [arg-type]
             except Exception as e:
                 exceptions.append(e)
                 continue
 
         # TODO: This is poor form atm, but the exception stacking
         # and final error should involve some careful thought
 
         if not extracted:
             raise exceptions[0]
 
         return extracted
 
     @classmethod
-    def one_from_text(cls, content: str, fail_on_many: bool = False) -> tuple[ModelT, slice]:
+    def one_from_text(cls, content: str, *, fail_on_many: bool = False) -> tuple[ModelT, slice]:
+        """
+        Finds and returns a single match from the given text content.
+
+        Args:
+            content: The text content to search for matches.
+            fail_on_many: If True, raises a ValidationError if multiple matches are found.
+
+        Returns:
+            A tuple containing the matched model and the slice indicating the match location.
+
+        Raises:
+            ValidationError: If multiple matches are found and fail_on_many is True.
+        """
         matches = cls.from_text(content)  # type: ignore [var-annotated]
         if fail_on_many and len(matches) > 1:
             raise ValidationError("Multiple matches found with 'fail_on_many=True'")
         return max(matches, key=lambda x: x[1].stop - x[1].start)
 
 
 #
@@ -182,46 +282,61 @@
     content: str
 
 
 # Common structured helpers
 
 
 class Thinking(Model):
+    """Quick model for thinking messages."""
+
     content: str
 
 
 class Question(Model):
+    """Quick model for questions."""
+
     content: str
 
 
 class Answer(Model):
+    """Quick model for answers."""
+
     content: str
 
 
 class QuestionAnswer(Model):
-    question: Question
-    answer: Answer
+    """Quick model for question-answer pairs."""
+
+    question: Question = element()
+    """The question"""
+    answer: Answer = element()
+    """The answer"""
 
 
 class Description(Model):
+    """Quick model for descriptions."""
+
     content: str
 
 
 class Instructions(Model):
+    """Quick model for instructions."""
+
     content: str
 
 
 class DelimitedAnswer(Model):
     "Mixed support delimited answer (- | / ,) selected based on most-matches"
 
     content: str
     _delimiters: t.ClassVar[list[str]] = [",", "-", "/", "|"]
 
     @property
     def items(self) -> list[str]:
+        """Parsed items from the content."""
         split_sizes: dict[str, int] = {}
         for delimiter in self._delimiters:
             split_sizes[delimiter] = len(self.content.split(delimiter))
         delimiter = max(split_sizes, key=split_sizes.get)  # type: ignore [arg-type]
         split = [i.strip(" \"'\t\r\n") for i in self.content.split(delimiter)]
         return [s for s in split if s]
 
@@ -244,14 +359,15 @@
     _delimiters = ["\n"]
 
 
 class YesNoAnswer(Model):
     "Yes/No answer answer with coercion"
 
     boolean: bool
+    """The boolean value of the answer."""
 
     @field_validator("boolean", mode="before")
     def parse_str_to_bool(cls, v: t.Any) -> t.Any:
         if isinstance(v, str):
             if v.strip().lower().startswith("yes"):
                 return True
             elif v.strip().lower().startswith("no"):
```

### Comparing `rigging-0.2.2/rigging/prompt.py` & `rigging-1.0.0rc0/rigging/prompt.py`

 * *Files identical despite different names*

### Comparing `rigging-0.2.2/rigging/tool.py` & `rigging-1.0.0rc0/rigging/tool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-import abc
+"""
+This module defines handles tool interaction with rigging generation.
+"""
+
 import inspect
 import typing as t
 
 from pydantic import Field, computed_field, model_validator
 from pydantic_xml import attr, element, wrapped
 
 from rigging.model import Model
@@ -53,14 +56,15 @@
 
     # This can be used in prompts to teach the model
     # the particular XML structure we're looking for
     #
     # TODO: We should consider building a base model
     # interface for both simple tags (<thing></thing>)
     # and full examples will filled in template vars
+
     @classmethod
     def xml_example(cls) -> str:
         return cls(
             calls=[
                 ToolCall(
                     tool="$TOOL_A",
                     function="$FUNCTION_A",
@@ -120,27 +124,64 @@
 
 
 #
 # 4 - Base class for implementing tools
 #
 
 
-class Tool(abc.ABC):
-    # TODO: I don't love having these defined as property getters,
-    # I would prefer to have them as class attributes, but I'm not
-    # sure how we can hint/enforce that to derived classes
-    @property
-    @abc.abstractmethod
-    def name(self) -> str:
-        ...
-
-    @property
-    @abc.abstractmethod
-    def description(self) -> str:
-        ...
+class Tool:
+    """
+    Base class for implementing tools in the Rigging system.
+
+    You should subclass this to define your own tools:
+
+    ```python
+    def Hammer(Tool):
+        name = "Hammer"
+        description = "A tool for hitting things."
+
+        def hit(self, target: Annotated[str, "Target of the hit") -> str:
+            return f"Hit {target} with a hammer."
+
+    chat = generator.chat(...).using(Hammer()).run()
+    ```
+
+    Note:
+        The `name` and `description` attributes are required and can be defined
+        as class attributes or properties. If you define them as properties,
+        you must also define a getter for them.
+
+    Note:
+        All functions on the tool must have type hints for their parameters and
+        use the `Annotated` type hint to provide a description for each parameter.
+    """
+
+    name: str
+    """Name of the tool"""
+    description: str
+    """Description of the tool"""
+
+    def __init_subclass__(cls, *, name: str | None = None, description: str | None = None, **kwargs: t.Any) -> None:
+        super().__init_subclass__(**kwargs)
+        if name is not None:
+            cls.name = name
+        if description is not None:
+            cls.description = description
+
+        # Ensure name and description are defined
+        if not (hasattr(cls, "name") or hasattr(cls, "name_property")):
+            raise TypeError(f"{cls.__name__} must define 'name' attribute or 'name' property.")
+        if not (hasattr(cls, "description") or hasattr(cls, "description_property")):
+            raise TypeError(f"{cls.__name__} must define 'description' attribute or 'description' property.")
+
+        # Check that they aren't empty or unset
+        if not getattr(cls, "name", None):
+            raise ValueError(f"{cls.__name__}.name must not be empty.")
+        if not getattr(cls, "description", None):
+            raise ValueError(f"{cls.__name__}.description must not be empty.")
 
     # TODO: We could alternatively use the get_description()
     # object and check against that (or even cast into it first)
     #
     # NOTE: We assume some sanity checks have already been performed
     def _execute(self, call: ToolCall) -> str:
         tool_description = self.get_description()
@@ -166,27 +207,29 @@
         result = function(**arguments)
 
         # Cast back to string for simplicity despite us likely
         # having more complex types underneath (we want them castable to str)
         return str(result)
 
     def execute(self, call: ToolCall) -> ToolResult:
+        """Executes a function call on the tool."""
         try:
             content = self._execute(call)
             return ToolResult(tool=call.tool, function=call.function, error=False, content=content)
         except Exception as e:
             return ToolResult(tool=call.tool, function=call.function, error=True, content=str(e))
 
     __call__ = execute
 
     # Lots of sanity checks and validation, but we essentially
     # want to use the class def, functions, params, etc. and
     # build a ToolDescription object that can be serialized
     # and passed to a model
     def get_description(self) -> ToolDescription:
+        """Creates a full description of the tool for use in prompting"""
         functions: list[ToolFunction] = []
         for method_name, method in inspect.getmembers(self.__class__, predicate=inspect.isfunction):
             if not method.__qualname__.startswith(self.__class__.__name__):
                 continue
 
             if method_name.startswith("_"):
                 continue
```

