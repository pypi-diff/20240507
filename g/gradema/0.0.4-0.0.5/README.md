# Comparing `tmp/gradema-0.0.4.tar.gz` & `tmp/gradema-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradema-0.0.4.tar", max compression
+gzip compressed data, was "gradema-0.0.5.tar", max compression
```

## Comparing `gradema-0.0.4.tar` & `gradema-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1056 2024-03-21 22:01:48.859372 gradema-0.0.4/LICENSE
--rw-r--r--   0        0        0     2072 2024-04-29 22:14:51.217676 gradema-0.0.4/README.md
--rw-r--r--   0        0        0       76 2024-04-29 15:19:53.229011 gradema-0.0.4/gradema/__init__.py
--rw-r--r--   0        0        0      216 2024-04-29 15:40:40.187785 gradema-0.0.4/gradema/grader/__init__.py
--rw-r--r--   0        0        0     3572 2024-04-29 15:40:40.179785 gradema-0.0.4/gradema/grader/_grader.py
--rw-r--r--   0        0        0      952 2024-04-23 03:17:43.476074 gradema-0.0.4/gradema/grader/_reporter.py
--rw-r--r--   0        0        0      138 2024-04-28 23:22:30.124159 gradema-0.0.4/gradema/grader/console/__init__.py
--rw-r--r--   0        0        0    10414 2024-04-29 21:47:36.529334 gradema-0.0.4/gradema/grader/console/_console.py
--rw-r--r--   0        0        0     1207 2024-04-23 03:17:09.439666 gradema-0.0.4/gradema/grader/console/_indent.py
--rw-r--r--   0        0        0     2675 2024-04-29 01:36:25.808074 gradema-0.0.4/gradema/grader/console/_runner.py
--rw-r--r--   0        0        0      752 2024-04-27 03:22:41.296861 gradema-0.0.4/gradema/grader/console/_util.py
--rw-r--r--   0        0        0       81 2024-04-18 04:40:01.722764 gradema-0.0.4/gradema/section/__init__.py
--rw-r--r--   0        0        0     1806 2024-04-18 04:09:33.425423 gradema-0.0.4/gradema/section/_section.py
--rw-r--r--   0        0        0      889 2024-04-29 22:00:57.623296 gradema-0.0.4/gradema/test/__init__.py
--rw-r--r--   0        0        0      895 2024-04-28 23:17:24.376395 gradema-0.0.4/gradema/test/_command.py
--rw-r--r--   0        0        0      339 2024-04-29 15:39:17.702812 gradema-0.0.4/gradema/test/_dummy.py
--rw-r--r--   0        0        0     1442 2024-04-29 15:39:17.694812 gradema-0.0.4/gradema/test/_exists.py
--rw-r--r--   0        0        0     1792 2024-04-30 05:25:39.077336 gradema-0.0.4/gradema/test/_python.py
--rw-r--r--   0        0        0     5021 2024-04-26 21:13:22.593885 gradema-0.0.4/gradema/test/_reporter.py
--rw-r--r--   0        0        0     1558 2024-04-30 05:13:07.916008 gradema-0.0.4/gradema/test/_rust.py
--rw-r--r--   0        0        0     2492 2024-04-30 05:23:32.639766 gradema-0.0.4/gradema/test/_stdio.py
--rw-r--r--   0        0        0      511 2024-04-29 15:38:21.742151 gradema-0.0.4/gradema/test/_test.py
--rw-r--r--   0        0        0      126 2024-04-30 05:22:47.147201 gradema-0.0.4/gradema/test/argument.py
--rw-r--r--   0        0        0      603 2024-04-30 05:26:53.586261 gradema-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 gradema-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-03-21 22:01:48.859372 gradema-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1919 2024-05-05 19:22:46.166690 gradema-0.0.5/README.md
+-rw-r--r--   0        0        0       76 2024-04-29 15:19:53.229011 gradema-0.0.5/gradema/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-29 15:40:40.187785 gradema-0.0.5/gradema/grader/__init__.py
+-rw-r--r--   0        0        0     3572 2024-04-29 15:40:40.179785 gradema-0.0.5/gradema/grader/_grader.py
+-rw-r--r--   0        0        0      952 2024-04-23 03:17:43.476074 gradema-0.0.5/gradema/grader/_reporter.py
+-rw-r--r--   0        0        0      138 2024-04-28 23:22:30.124159 gradema-0.0.5/gradema/grader/console/__init__.py
+-rw-r--r--   0        0        0    11776 2024-05-05 19:55:39.691038 gradema-0.0.5/gradema/grader/console/_console.py
+-rw-r--r--   0        0        0     1207 2024-04-23 03:17:09.439666 gradema-0.0.5/gradema/grader/console/_indent.py
+-rw-r--r--   0        0        0     3074 2024-05-05 19:21:42.369911 gradema-0.0.5/gradema/grader/console/_runner.py
+-rw-r--r--   0        0        0      752 2024-04-27 03:22:41.296861 gradema-0.0.5/gradema/grader/console/_util.py
+-rw-r--r--   0        0        0       81 2024-04-18 04:40:01.722764 gradema-0.0.5/gradema/section/__init__.py
+-rw-r--r--   0        0        0     1806 2024-04-18 04:09:33.425423 gradema-0.0.5/gradema/section/_section.py
+-rw-r--r--   0        0        0     1053 2024-05-04 18:58:24.811647 gradema-0.0.5/gradema/test/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-28 23:17:24.376395 gradema-0.0.5/gradema/test/_command.py
+-rw-r--r--   0        0        0      339 2024-04-29 15:39:17.702812 gradema-0.0.5/gradema/test/_dummy.py
+-rw-r--r--   0        0        0     1442 2024-04-29 15:39:17.694812 gradema-0.0.5/gradema/test/_exists.py
+-rw-r--r--   0        0        0     4159 2024-05-05 23:17:52.897199 gradema-0.0.5/gradema/test/_python.py
+-rw-r--r--   0        0        0     7214 2024-05-05 20:01:17.638954 gradema-0.0.5/gradema/test/_reporter.py
+-rw-r--r--   0        0        0     2197 2024-05-04 04:51:27.181724 gradema-0.0.5/gradema/test/_rust.py
+-rw-r--r--   0        0        0     3620 2024-05-04 02:26:37.862521 gradema-0.0.5/gradema/test/_stdio.py
+-rw-r--r--   0        0        0      511 2024-04-29 15:38:21.742151 gradema-0.0.5/gradema/test/_test.py
+-rw-r--r--   0        0        0      256 2024-05-04 02:11:16.307576 gradema-0.0.5/gradema/test/argument.py
+-rw-r--r--   0        0        0      621 2024-05-07 17:57:25.466602 gradema-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2766 1970-01-01 00:00:00.000000 gradema-0.0.5/PKG-INFO
```

### Comparing `gradema-0.0.4/LICENSE` & `gradema-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gradema-0.0.4/README.md` & `gradema-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -51,13 +51,10 @@
 poetry run pytest tests
 ```
 
 
 # TODO
 
 * Use [py2cfg](https://pypi.org/project/py2cfg/) to produce control flow graphs
-* Use pytest instead of basic python3 and asserts
 * Text diff (not critical)
-* Arg tests and the OUTPUT_FILE interpolation thing
-* Think about where to put unit tests
-  * Rust - move tests inside src?
 * Do C++ example - lowest priority
+* Fuzzy diff support
```

### Comparing `gradema-0.0.4/gradema/grader/_grader.py` & `gradema-0.0.5/gradema/grader/_grader.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.4/gradema/grader/_reporter.py` & `gradema-0.0.5/gradema/grader/_reporter.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.4/gradema/grader/console/_console.py` & `gradema-0.0.5/gradema/grader/console/_console.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import difflib
 import io
 import shlex
 import shutil
 import subprocess
 import traceback
 from pathlib import Path
-from typing import TextIO, Optional
+from typing import TextIO, Optional, Sequence, Mapping
 
 from rich import markup
 from rich.console import Console
 from rich.prompt import Prompt
 
 from gradema.grader import GraderReporter
 from gradema.grader.console._util import indentation, arrow, header, indent_text
@@ -21,17 +21,16 @@
     CommandData,
     Test,
     TestResult,
     FractionalTestResult,
     PercentTestResult,
     StdioCommandData,
 )
+from gradema.test.argument import Argument, ResolvedArgumentInfo, OutputFile
 
-
-BACKSLASH = markup.escape("\\")
 TEST_DIRECTORY = Path("build/test")
 
 
 def has_vim_installed() -> bool:
     return shutil.which("vim") is not None
 
 
@@ -67,23 +66,23 @@
         ],
         stdin=subprocess.DEVNULL,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
     )
 
 
-def html_diff(left_path: Path, right_path: Path, html_output_path: Path) -> None:
+def html_diff(goal_path: Path, actual_output_path: Path, html_output_path: Path) -> None:
     # TODO remember that file.readlines() LOADS THE ENTIRE FILE INTO MEMORY
     #   We might not care about that right now, but this could be a problem later with huge files
-    with left_path.open("r") as left, right_path.open("r") as right:
+    with goal_path.open("r") as left, actual_output_path.open("r") as right:
         diff = difflib.HtmlDiff().make_file(
             left.readlines(),
             right.readlines(),
-            str(left_path),
-            str(right_path),
+            f"Goal: {goal_path}",
+            f"Your output: {actual_output_path}",
         )
         with html_output_path.open("w") as f_out:
             f_out.write(diff)
 
 
 @dataclasses.dataclass
 class ConsoleTestReporter(TestReporter):
@@ -96,36 +95,54 @@
         indent = indentation(self.reporter.depth)
         buffer = io.StringIO()
         traceback.print_exception(exception, file=buffer)
         indented_text = indent_text(self.reporter.depth, buffer.getvalue())
         # make end="" because the exception text should have a trailing newline
         self.reporter.console.print(f"{indent}Unexpected exception:\n{indented_text}", highlight=False, end="")
 
-    def report_command(self, command: list[str]) -> CommandData:
+    def __get_output_file(self, test_identifier: str) -> Path:
+        directory = TEST_DIRECTORY / "stdio/outputs"
+        directory.mkdir(parents=True, exist_ok=True)
+        return directory / f"{test_identifier}.txt"
+
+    def resolve_command(self, command: Sequence[Argument], test_identifier: str) -> tuple[Sequence[str], Mapping[tuple[int, Argument], ResolvedArgumentInfo]]:
+        resolved_command = []
+        argument_info_dictionary: dict[tuple[int, Argument], ResolvedArgumentInfo] = dict()
+        # NOTE: We have to specify the type of argument_info_dictionary because the key is not covariant: https://github.com/python/typing/pull/273
+        for i, argument in enumerate(command):
+            if isinstance(argument, OutputFile):
+                output_file = self.__get_output_file(test_identifier)
+                resolved_command.append(str(output_file))
+                argument_info_dictionary[(i, argument)] = output_file
+            else:  # argument should be a str. If you get errors here, someone messed with the definition of Argument and you need to implement more cases
+                resolved_command.append(argument)
+
+        return resolved_command, argument_info_dictionary
+
+    def report_command(self, command: Sequence[str]) -> CommandData:
         indent = indentation(self.reporter.depth)
         self.reporter.console.print(f"{indent}Running command: [magenta]{markup.escape(shlex.join(command))}[/magenta]")
         return CommandData(self.reporter.stdout, self.reporter.stderr)
 
-    def report_stdio_command(self, command: list[str], test_identifier: str, input_file: Optional[Path]) -> StdioCommandData:
+    def report_stdio_command(self, command: Sequence[str], test_identifier: str, input_file: Optional[Path], stdout_as_output: bool) -> StdioCommandData:
         indent = indentation(self.reporter.depth)
         indent_plus = indentation(self.reporter.depth + 1)
-        directory = TEST_DIRECTORY / "stdio/outputs"
-        directory.mkdir(parents=True, exist_ok=True)
-        output_file = directory / f"{test_identifier}.txt"
+        output_file = self.__get_output_file(test_identifier)
         self.reporter.console.print(f"{indent}Command to be run: [magenta]{markup.escape(shlex.join(command))}[/magenta]")
-        self.reporter.console.print(f"{indent}Command to be run including I/O redirection:")
-        self.reporter.console.print(
-            f"{indent}[magenta]{markup.escape(shlex.join(command))} {BACKSLASH}[/magenta]"
-            + (f"\n{indent_plus}[magenta]< {markup.escape(shlex.quote(str(input_file)))} {BACKSLASH}[/magenta]" if input_file is not None else "")
-            + f"\n{indent_plus}[magenta]> {markup.escape(shlex.quote(str(output_file)))}[/magenta]"
-        )
+        if input_file is not None or stdout_as_output:
+            self.reporter.console.print(f"{indent}Command to be run including I/O redirection:")
+            self.reporter.console.print(
+                f"{indent}[magenta]{markup.escape(shlex.join(command))}[/magenta]"
+                + (f" \\\n{indent_plus}[magenta]< {markup.escape(shlex.quote(str(input_file)))}[/magenta]" if input_file is not None else "")
+                + (f" \\\n{indent_plus}[magenta]> {markup.escape(shlex.quote(str(output_file)))}[/magenta]" if stdout_as_output else "")
+            )
 
-        return StdioCommandData(output_file, self.reporter.stderr)
+        return StdioCommandData(output_file, self.reporter.stdout, self.reporter.stderr)
 
-    def maybe_launch_debugger(self, command: list[str]) -> None:
+    def maybe_launch_debugger(self, command: Sequence[str]) -> None:
         indent = indentation(self.reporter.depth)
         if self.reporter.debug_mode:
             self.reporter.console.print(f"{indent}This test did not complete successfully. We are going to launch the debugger now.")
             self.reporter.console.print(f"{indent}Debug command: [magenta]{markup.escape(shlex.join(command))}[/magenta]")
             launch_debugger = True
             while True:
                 response = Prompt.ask(
```

### Comparing `gradema-0.0.4/gradema/grader/console/_indent.py` & `gradema-0.0.5/gradema/grader/console/_indent.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.4/gradema/grader/console/_runner.py` & `gradema-0.0.5/gradema/grader/console/_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 import sys
+from pathlib import Path
 
 from rich.console import Console
 from rich.text import Text
 
 from ._console import ConsoleGraderReporter
 from gradema.section import Section
 from gradema.grader import grade_section
 
 
+RESULTS_PATH = Path("results.txt")
+
+
+def save_score(points: int) -> None:
+    # It is necessary to remove results.txt before writing to it because if a student wrote to results.txt and changed its permissions, we couldn't write to it
+    RESULTS_PATH.unlink(missing_ok=True)
+    with RESULTS_PATH.open("w") as file:
+        print(points, file=file)
+
+
 def welcome(console: Console) -> None:
     console.print("Welcome to Gradema!")
     console.print("This script will grandma you through completing this programming assignment")
     console.line()
     console.print(f"    [magenta]Magenta[/magenta] is bash/shell commands.")
     console.print(f"    [green]Green[/green] is used to indicate a pass.")
     console.print(f"    [red]Red[/red] is used to indicate a fail.")
@@ -56,14 +67,15 @@
         sys.stdout,
         sys.stderr,
         interactive=interactive,
         debug_mode=debug_mode,
         depth=0,
     )
     points = grade_section(reporter, section.points, section)
+    save_score(points)
     passing = points >= 70
     console.line()
     console.print("=" * console.width, style="green" if passing else "red")
     console.print(f"Your total grade is:\n{points}")
     console.line()
     if points == 100:
         console.print("It's perfect! Congratulations!", style="green")
```

### Comparing `gradema-0.0.4/gradema/grader/console/_util.py` & `gradema-0.0.5/gradema/grader/console/_util.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.4/gradema/section/_section.py` & `gradema-0.0.5/gradema/section/_section.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.4/gradema/test/__init__.py` & `gradema-0.0.5/gradema/test/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from ._reporter import TestReporter, CommandData, StdioCommandData
 from ._test import Test, FractionalTestResult, PercentTestResult, TestResult
 from ._python import (
     create_python_test,
+    create_python_pytest,
     create_python_format_check,
     create_python_format_check_from_path,
     create_python_type_check,
     create_python_stdio_test,
-    create_python_arg_test,
+    create_python_traditional_stdio_test,
+    create_python_traditional_arg_test,
 )
 from ._dummy import dummy_test
 from ._exists import create_file_exists_test
 from ._rust import RustProgram
 
 __all__ = [
     "TestReporter",
     "CommandData",
     "StdioCommandData",
     "Test",
     "FractionalTestResult",
     "PercentTestResult",
     "TestResult",
     "create_python_test",
+    "create_python_pytest",
     "create_python_stdio_test",
+    "create_python_traditional_stdio_test",
     "create_python_format_check",
     "create_python_format_check_from_path",
     "create_python_type_check",
     "dummy_test",
     "create_file_exists_test",
     "RustProgram",
-    "create_python_arg_test",
+    "create_python_traditional_arg_test",
 ]
```

### Comparing `gradema-0.0.4/gradema/test/_command.py` & `gradema-0.0.5/gradema/test/_command.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.4/gradema/test/_exists.py` & `gradema-0.0.5/gradema/test/_exists.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.4/pyproject.toml` & `gradema-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gradema"
-version = "0.0.4"
+version = "0.0.5"
 description = "The utility you need to easily configure auto-grading"
 authors = ["Lavender Shannon <jdsfz4@mst.edu>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://gradema.readthedocs.io"
 repository = "https://git.mst.edu/gradema/gradema"
@@ -12,14 +12,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 rich = "13.7.1"
 pudb = "^2024.1"
 mypy = "^1.10.0"
 editorconfig = "^0.12.4"
 python-magic = "^0.4.27"
+py2cfg = "^0.7.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "8.1.1"
 black = "^24.4.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `gradema-0.0.4/PKG-INFO` & `gradema-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: gradema
-Version: 0.0.4
+Version: 0.0.5
 Summary: The utility you need to easily configure auto-grading
 Home-page: https://gradema.readthedocs.io
 License: MIT
 Author: Lavender Shannon
 Author-email: jdsfz4@mst.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: editorconfig (>=0.12.4,<0.13.0)
 Requires-Dist: mypy (>=1.10.0,<2.0.0)
 Requires-Dist: pudb (>=2024.1,<2025.0)
+Requires-Dist: py2cfg (>=0.7.3,<0.8.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: rich (==13.7.1)
 Project-URL: Repository, https://git.mst.edu/gradema/gradema
 Description-Content-Type: text/markdown
 
 # Gradema
 
@@ -73,14 +74,11 @@
 poetry run pytest tests
 ```
 
 
 # TODO
 
 * Use [py2cfg](https://pypi.org/project/py2cfg/) to produce control flow graphs
-* Use pytest instead of basic python3 and asserts
 * Text diff (not critical)
-* Arg tests and the OUTPUT_FILE interpolation thing
-* Think about where to put unit tests
-  * Rust - move tests inside src?
 * Do C++ example - lowest priority
+* Fuzzy diff support
```

