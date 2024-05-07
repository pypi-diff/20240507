# Comparing `tmp/mpflash-0.7.5.tar.gz` & `tmp/mpflash-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpflash-0.7.5.tar", max compression
+gzip compressed data, was "mpflash-0.7.6.tar", max compression
```

## Comparing `mpflash-0.7.5.tar` & `mpflash-0.7.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.7.5/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.7.5/mpflash/__init__.py
--rw-r--r--   0        0        0     9010 2024-05-03 13:05:36.158081 mpflash-0.7.5/mpflash/ask_input.py
--rw-r--r--   0        0        0     3642 2024-05-03 13:05:36.159263 mpflash-0.7.5/mpflash/cli_download.py
--rw-r--r--   0        0        0     5845 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/cli_flash.py
--rw-r--r--   0        0        0     1967 2024-04-29 18:55:09.407466 mpflash-0.7.5/mpflash/cli_group.py
--rw-r--r--   0        0        0     1024 2024-04-29 18:55:09.408806 mpflash-0.7.5/mpflash/cli_list.py
--rw-r--r--   0        0        0      656 2024-05-05 21:39:33.092998 mpflash-0.7.5/mpflash/cli_main.py
--rw-r--r--   0        0        0     1049 2024-04-29 18:55:09.409821 mpflash-0.7.5/mpflash/common.py
--rw-r--r--   0        0        0      419 2024-04-05 19:52:32.888852 mpflash-0.7.5/mpflash/config.py
--rw-r--r--   0        0        0    11120 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/download.py
--rw-r--r--   0        0        0     3803 2024-04-29 18:55:09.412110 mpflash-0.7.5/mpflash/downloaded.py
--rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.7.5/mpflash/errors.py
--rw-r--r--   0        0        0     2490 2024-04-29 18:55:09.414103 mpflash-0.7.5/mpflash/flash.py
--rw-r--r--   0        0        0     2314 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/flash_esp.py
--rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.7.5/mpflash/flash_stm32.py
--rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.7.5/mpflash/flash_stm32_cube.py
--rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.7.5/mpflash/flash_stm32_dfu.py
--rw-r--r--   0        0        0     2115 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/flash_uf2.py
--rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.7.5/mpflash/flash_uf2_boardid.py
--rw-r--r--   0        0        0     4319 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/flash_uf2_linux.py
--rw-r--r--   0        0        0     1093 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/flash_uf2_windows.py
--rw-r--r--   0        0        0     4713 2024-05-03 13:05:36.167441 mpflash-0.7.5/mpflash/list.py
--rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.7.5/mpflash/logger.py
--rw-r--r--   0        0        0     3621 2024-05-03 13:05:36.168458 mpflash-0.7.5/mpflash/mpboard_id/__init__.py
--rw-r--r--   0        0        0     2592 2024-05-05 21:35:23.329974 mpflash-0.7.5/mpflash/mpboard_id/board_id.py
--rw-r--r--   0        0        0    96983 2024-04-05 19:52:32.903789 mpflash-0.7.5/mpflash/mpboard_id/board_info.csv
--rw-r--r--   0        0        0   674442 2024-04-30 08:26:55.864409 mpflash-0.7.5/mpflash/mpboard_id/board_info.json
--rw-r--r--   0        0        0     7110 2024-05-05 21:00:42.554839 mpflash-0.7.5/mpflash/mpremoteboard/__init__.py
--rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.7.5/mpflash/mpremoteboard/mpy_fw_info.py
--rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.7.5/mpflash/mpremoteboard/runner.py
--rw-r--r--   0        0        0     5739 2024-04-29 18:55:09.422436 mpflash-0.7.5/mpflash/vendor/dfu.py
--rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.7.5/mpflash/vendor/pydfu.py
--rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.7.5/mpflash/vendor/readme.md
--rw-r--r--   0        0        0     3629 2024-05-05 21:35:22.350460 mpflash-0.7.5/mpflash/vendor/versions.py
--rw-r--r--   0        0        0     5297 2024-05-03 13:05:36.171762 mpflash-0.7.5/mpflash/worklist.py
--rw-r--r--   0        0        0     1648 2024-05-05 21:40:12.443828 mpflash-0.7.5/pyproject.toml
--rw-r--r--   0        0        0    13159 2024-04-29 21:19:09.956495 mpflash-0.7.5/README.md
--rw-r--r--   0        0        0    14633 1970-01-01 00:00:00.000000 mpflash-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.7.6/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.7.6/mpflash/__init__.py
+-rw-r--r--   0        0        0     9459 2024-05-06 20:44:27.103815 mpflash-0.7.6/mpflash/ask_input.py
+-rw-r--r--   0        0        0     3623 2024-05-06 20:03:34.319950 mpflash-0.7.6/mpflash/cli_download.py
+-rw-r--r--   0        0        0     6133 2024-05-06 20:14:08.358935 mpflash-0.7.6/mpflash/cli_flash.py
+-rw-r--r--   0        0        0     1967 2024-04-29 18:55:09.407466 mpflash-0.7.6/mpflash/cli_group.py
+-rw-r--r--   0        0        0     1024 2024-04-29 18:55:09.408806 mpflash-0.7.6/mpflash/cli_list.py
+-rw-r--r--   0        0        0      796 2024-05-06 21:28:04.732882 mpflash-0.7.6/mpflash/cli_main.py
+-rw-r--r--   0        0        0     1049 2024-04-29 18:55:09.409821 mpflash-0.7.6/mpflash/common.py
+-rw-r--r--   0        0        0      419 2024-04-05 19:52:32.888852 mpflash-0.7.6/mpflash/config.py
+-rw-r--r--   0        0        0    11120 2024-05-03 13:05:36.160916 mpflash-0.7.6/mpflash/download.py
+-rw-r--r--   0        0        0     3803 2024-04-29 18:55:09.412110 mpflash-0.7.6/mpflash/downloaded.py
+-rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.7.6/mpflash/errors.py
+-rw-r--r--   0        0        0     2490 2024-04-29 18:55:09.414103 mpflash-0.7.6/mpflash/flash.py
+-rw-r--r--   0        0        0     2314 2024-05-03 13:05:36.160916 mpflash-0.7.6/mpflash/flash_esp.py
+-rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.7.6/mpflash/flash_stm32.py
+-rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.7.6/mpflash/flash_stm32_cube.py
+-rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.7.6/mpflash/flash_stm32_dfu.py
+-rw-r--r--   0        0        0     2115 2024-05-03 13:05:36.160916 mpflash-0.7.6/mpflash/flash_uf2.py
+-rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.7.6/mpflash/flash_uf2_boardid.py
+-rw-r--r--   0        0        0     4319 2024-05-03 13:05:36.160916 mpflash-0.7.6/mpflash/flash_uf2_linux.py
+-rw-r--r--   0        0        0     1093 2024-05-03 13:05:36.160916 mpflash-0.7.6/mpflash/flash_uf2_windows.py
+-rw-r--r--   0        0        0     4713 2024-05-03 13:05:36.167441 mpflash-0.7.6/mpflash/list.py
+-rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.7.6/mpflash/logger.py
+-rw-r--r--   0        0        0     3621 2024-05-03 13:05:36.168458 mpflash-0.7.6/mpflash/mpboard_id/__init__.py
+-rw-r--r--   0        0        0     2592 2024-05-06 20:38:28.562420 mpflash-0.7.6/mpflash/mpboard_id/board_id.py
+-rw-r--r--   0        0        0    96983 2024-04-05 19:52:32.903789 mpflash-0.7.6/mpflash/mpboard_id/board_info.csv
+-rw-r--r--   0        0        0   674442 2024-04-30 08:26:55.864409 mpflash-0.7.6/mpflash/mpboard_id/board_info.json
+-rw-r--r--   0        0        0     7683 2024-05-06 21:22:30.569154 mpflash-0.7.6/mpflash/mpremoteboard/__init__.py
+-rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.7.6/mpflash/mpremoteboard/mpy_fw_info.py
+-rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.7.6/mpflash/mpremoteboard/runner.py
+-rw-r--r--   0        0        0     5739 2024-04-29 18:55:09.422436 mpflash-0.7.6/mpflash/vendor/dfu.py
+-rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.7.6/mpflash/vendor/pydfu.py
+-rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.7.6/mpflash/vendor/readme.md
+-rw-r--r--   0        0        0     3629 2024-05-06 20:38:28.565419 mpflash-0.7.6/mpflash/vendor/versions.py
+-rw-r--r--   0        0        0     5297 2024-05-03 13:05:36.171762 mpflash-0.7.6/mpflash/worklist.py
+-rw-r--r--   0        0        0     1648 2024-05-06 21:37:33.640498 mpflash-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0    13159 2024-04-29 21:19:09.956495 mpflash-0.7.6/README.md
+-rw-r--r--   0        0        0    14633 1970-01-01 00:00:00.000000 mpflash-0.7.6/PKG-INFO
```

### Comparing `mpflash-0.7.5/LICENSE` & `mpflash-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/ask_input.py` & `mpflash-0.7.6/mpflash/ask_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,59 +41,63 @@
 
 
 ParamType = Union[DownloadParams, FlashParams]
 
 
 def ask_missing_params(
     params: ParamType,
-    action: str = "download",
+    # action: str = "download",
 ) -> ParamType:
     """
     Asks the user for parameters that have not been supplied on the commandline and returns the updated params.
 
     Args:
         params (ParamType): The parameters to be updated.
         action (str, optional): The action to be performed. Defaults to "download".
 
     Returns:
         ParamType: The updated parameters.
     """
+    # if action flash,  single input
+    # if action download, multiple input
+    multi_select = isinstance(params, DownloadParams)
+    action = "download" if isinstance(params, DownloadParams) else "flash"
     if not config.interactive:
         # no interactivity allowed
         return params
     # import only when needed to reduce load time
     import inquirer
 
     questions = []
-    answers = {"action": action}
-    if isinstance(params, FlashParams):
+    answers = {"action": "download" if isinstance(params, DownloadParams) else "flash"}
+    if not multi_select:
         if not params.serial or "?" in params.serial:
-            ask_serialport(questions, action=action)
+            ask_serialport(questions)
         else:
             answers["serial"] = params.serial
 
     if not params.versions or "?" in params.versions:
-        ask_versions(questions, action=action)
+        ask_versions(questions, multi_select=multi_select, action=action)
     else:
         # versions is used to show only the boards for the selected versions
         answers["versions"] = params.versions  # type: ignore
 
     if not params.boards or "?" in params.boards:
-        ask_port_board(questions, action=action)
+        ask_port_board(questions, multi_select=multi_select, action=action)
     if questions:
         answers = inquirer.prompt(questions, answers=answers)
     if not answers:
         # input cancelled by user
         return []  # type: ignore
     # print(repr(answers))
     if isinstance(params, FlashParams) and "serial" in answers:
-        params.serial = answers["serial"]
+        params.serial = answers["serial"].split()[0]  # split to remove the description
     if "port" in answers:
         params.ports = [p for p in params.ports if p != "?"]  # remove the "?" if present
-        params.ports.extend(answers["port"])
+        params.ports.append(answers["port"])
     if "boards" in answers:
         params.boards = [b for b in params.boards if b != "?"]  # remove the "?" if present
         params.boards.extend(answers["boards"] if isinstance(answers["boards"], list) else [answers["boards"]])
     if "versions" in answers:
         params.versions = [v for v in params.versions if v != "?"]  # remove the "?" if present
         # make sure it is a list
         if isinstance(answers["versions"], (list, tuple)):
@@ -140,15 +144,15 @@
         # Get the values of the dictionary, which are the unique items from the original list
         some_boards = list(unique_dict.values())
     else:
         some_boards = [(f"No {answers['port']} boards found for version(s) {_versions}", "")]
     return some_boards
 
 
-def ask_port_board(questions: list, *, action: str):
+def ask_port_board(questions: list, *, multi_select: bool, action: str):
     """
     Asks the user for the port and board selection.
 
     Args:
         questions (list): The list of questions to be asked.
         action (str): The action to be performed.
 
@@ -156,15 +160,15 @@
         None
     """
     # import only when needed to reduce load time
     import inquirer
 
     # if action flash,  single input
     # if action download, multiple input
-    inquirer_ux = inquirer.Checkbox if action == "download" else inquirer.List
+    inquirer_ux = inquirer.Checkbox if multi_select else inquirer.List
     questions.extend(
         (
             inquirer.List(
                 "port",
                 message="Which port do you want to {action} " + "to {serial} ?" if action == "flash" else "?",
                 choices=get_known_ports(),
                 autocomplete=True,
@@ -179,30 +183,30 @@
                 choices=filter_matching_boards,
                 validate=lambda _, x: True if x else "Please select at least one board",  # type: ignore
             ),
         )
     )
 
 
-def ask_versions(questions: list, *, action: str):
+def ask_versions(questions: list, *, multi_select: bool, action: str):
     """
     Asks the user for the version selection.
 
     Args:
         questions (list): The list of questions to be asked.
         action (str): The action to be performed.
 
     Returns:
         None
     """
     # import only when needed to reduce load time
     import inquirer
     import inquirer.errors
 
-    input_ux = inquirer.Checkbox if action == "download" else inquirer.List
+    input_ux = inquirer.Checkbox if multi_select else inquirer.List
     mp_versions: List[str] = micropython_versions()
     mp_versions = [v for v in mp_versions if "preview" not in v]
 
     # remove the versions for which there are no known boards in the board_info.json
     # todo: this may be a little slow
     mp_versions = [v for v in mp_versions if get_known_boards_for_port("stm32", [v])]
 
@@ -222,38 +226,38 @@
             # inquirer.List(
             "versions",
             message="Which version(s) do you want to {action} " + ("to {serial} ?" if action == "flash" else "?"),
             # Hints would be nice , but needs a hint for each and every option
             # hints=["Use space to select multiple options"],
             choices=mp_versions,
             autocomplete=True,
-            validate=at_least_one_validation,
+            validate=at_least_one_validation,  # type: ignore
         )
     )
 
 
-def ask_serialport(questions: list, *, action: str):
+def ask_serialport(questions: list, *, multi_select: bool = False, bluetooth: bool = False):
     """
     Asks the user for the serial port selection.
 
     Args:
         questions (list): The list of questions to be asked.
         action (str): The action to be performed.
 
     Returns:
         None
     """
     # import only when needed to reduce load time
     import inquirer
 
-    serialports = MPRemoteBoard.connected_boards()
+    comports = MPRemoteBoard.connected_boards(bluetooth=bluetooth, description=True)
     questions.append(
         inquirer.List(
             "serial",
             message="Which serial port do you want to {action} ?",
-            choices=serialports,
+            choices=comports,
             other=True,
             validate=lambda _, x: True if x else "Please select or enter a serial port",  # type: ignore
         )
     )
 
     return questions
```

### Comparing `mpflash-0.7.5/mpflash/cli_download.py` & `mpflash-0.7.6/mpflash/cli_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                         params.ports.append(board_["port"])
                     except MPFlashError as e:
                         log.error(f"{e}")
     else:
         # no boards specified - detect connected ports and boards
         params.ports, params.boards = connected_ports_boards()
 
-    params = ask_missing_params(params, action="download")
+    params = ask_missing_params(params)
     if not params:  # Cancelled by user
         return 2
     params.versions = [clean_version(v, drop_v=True) for v in params.versions]
     assert isinstance(params, DownloadParams)
 
     try:
         download(
```

### Comparing `mpflash-0.7.5/mpflash/cli_flash.py` & `mpflash-0.7.6/mpflash/cli_flash.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,22 @@
     if kwargs["board"] is None:
         kwargs["boards"] = []
         kwargs.pop("board")
     else:
         kwargs["boards"] = [kwargs.pop("board")]
 
     params = FlashParams(**kwargs)
+
+    # make it simple for the user to flash one board
+    # by asking for the serial port if not specified
+    if params.boards == ["?"] and params.serial == "auto":
+        params.serial = "?"
+
+    # Detect connected boards if not specified,
+    # and ask for input if boards cannot be detected
     if not params.boards or params.boards == []:
         # nothing specified - detect connected boards
         params.ports, params.boards = connected_ports_boards()
         if params.boards == []:
             # No MicroPython boards detected, but it could be unflashed or not in bootloader mode
             # Ask for serial port and board_id to flash
             params.serial = "?"
@@ -121,15 +129,15 @@
                         log.info(f"Resolved board description: {info['board']}")
                         params.boards.remove(board_id)
                         params.boards.append(info["board"])
                 except Exception as e:
                     log.warning(f"unable to resolve board description: {e}")
 
     # Ask for missing input if needed
-    params = ask_missing_params(params, action="flash")
+    params = ask_missing_params(params)
     if not params:  # Cancelled by user
         return 2
     # TODO: Just in time Download of firmware
 
     assert isinstance(params, FlashParams)
 
     if len(params.versions) > 1:
```

### Comparing `mpflash-0.7.5/mpflash/cli_group.py` & `mpflash-0.7.6/mpflash/cli_group.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/cli_list.py` & `mpflash-0.7.6/mpflash/cli_list.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/cli_main.py` & `mpflash-0.7.6/mpflash/cli_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """mpflash is a CLI to download and flash MicroPython firmware to various boards."""
 
 # import rich_click as click
 
 import click
+from loguru import logger as log
 
 from .cli_download import cli_download
 from .cli_flash import cli_flash_board
 from .cli_group import cli
 from .cli_list import cli_list_mcus
 
 
@@ -15,13 +16,16 @@
     cli.add_command(cli_list_mcus)
     cli.add_command(cli_download)
     # cli(auto_envvar_prefix="MPFLASH")
     try:
         result = cli(standalone_mode=False)
         exit(result)
     except AttributeError as e:
-        print(f"Error: {e}")
+        log.error(f"Error: {e}")
         exit(-1)
+    except click.exceptions.ClickException as e:
+        log.error(f"Error: {e}")
+        exit(-2)
 
 
 if __name__ == "__main__":
     mpflash()
```

### Comparing `mpflash-0.7.5/mpflash/common.py` & `mpflash-0.7.6/mpflash/common.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/download.py` & `mpflash-0.7.6/mpflash/download.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/downloaded.py` & `mpflash-0.7.6/mpflash/downloaded.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/flash.py` & `mpflash-0.7.6/mpflash/flash.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/flash_esp.py` & `mpflash-0.7.6/mpflash/flash_esp.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/flash_stm32.py` & `mpflash-0.7.6/mpflash/flash_stm32.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/flash_stm32_cube.py` & `mpflash-0.7.6/mpflash/flash_stm32_cube.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/flash_stm32_dfu.py` & `mpflash-0.7.6/mpflash/flash_stm32_dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/flash_uf2.py` & `mpflash-0.7.6/mpflash/flash_uf2.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/flash_uf2_linux.py` & `mpflash-0.7.6/mpflash/flash_uf2_linux.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/flash_uf2_windows.py` & `mpflash-0.7.6/mpflash/flash_uf2_windows.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/list.py` & `mpflash-0.7.6/mpflash/list.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/logger.py` & `mpflash-0.7.6/mpflash/logger.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/mpboard_id/__init__.py` & `mpflash-0.7.6/mpflash/mpboard_id/__init__.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/mpboard_id/board_id.py` & `mpflash-0.7.6/mpflash/mpboard_id/board_id.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/mpboard_id/board_info.csv` & `mpflash-0.7.6/mpflash/mpboard_id/board_info.csv`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/mpboard_id/board_info.json` & `mpflash-0.7.6/mpflash/mpboard_id/board_info.json`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/mpremoteboard/__init__.py` & `mpflash-0.7.6/mpflash/mpremoteboard/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
         Returns:
         - str: The string representation of the object.
         """
         return f"MPRemoteBoard({self.serialport}, {self.family} {self.port}, {self.board}, {self.version})"
 
     @staticmethod
-    def connected_boards(bluetooth: bool = False) -> List[str]:
+    def connected_boards(bluetooth: bool = False, description: bool = False) -> List[str]:
         # TODO: rename to connected_comports
         """
         Get a list of connected comports.
 
         Parameters:
         - bluetooth (bool): Whether to include Bluetooth ports. Default is False.
 
@@ -77,16 +77,27 @@
         """
         comports = serial.tools.list_ports.comports()
 
         if not bluetooth:
             # filter out bluetooth ports
             comports = [p for p in comports if "bluetooth" not in p.description.lower()]
             comports = [p for p in comports if "BTHENUM" not in p.hwid]
-
-        return sorted([p.device for p in comports])
+        if description:
+            output = [
+                f"{p.device} {(p.manufacturer + ' ') if p.manufacturer and not p.description.startswith(p.manufacturer) else ''}{p.description}"
+                for p in comports
+            ]
+        else:
+            output = [p.device for p in comports]
+
+        if sys.platform == "win32":
+            # Windows sort of comports by number - but fallback to device name
+            return sorted(output, key=lambda x: int(x.split()[0][3:]) if x.split()[0][3:].isdigit() else x)
+        # sort by device name
+        return sorted(output)
 
     @retry(stop=stop_after_attempt(RETRIES), wait=wait_fixed(1), reraise=True)  # type: ignore ## retry_error_cls=ConnectionError,
     def get_mcu_info(self, timeout: int = 2):
         """
         Get MCU information from the connected board.
 
         Parameters:
```

### Comparing `mpflash-0.7.5/mpflash/mpremoteboard/mpy_fw_info.py` & `mpflash-0.7.6/mpflash/mpremoteboard/mpy_fw_info.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/mpremoteboard/runner.py` & `mpflash-0.7.6/mpflash/mpremoteboard/runner.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/vendor/dfu.py` & `mpflash-0.7.6/mpflash/vendor/dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/vendor/pydfu.py` & `mpflash-0.7.6/mpflash/vendor/pydfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/vendor/versions.py` & `mpflash-0.7.6/mpflash/vendor/versions.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/mpflash/worklist.py` & `mpflash-0.7.6/mpflash/worklist.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/pyproject.toml` & `mpflash-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpflash"
-version = "0.7.5"
+version = "0.7.6"
 description = "Flash and download tool for MicroPython firmwares"
 authors = ["Jos Verlinde <jos_verlinde@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["MicroPython", "firmware", "flash", "download", "UF2", "esptool"]
 homepage = "https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md"
 repository = "https://github.com/Josverl/micropython-stubber"
```

### Comparing `mpflash-0.7.5/README.md` & `mpflash-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.5/PKG-INFO` & `mpflash-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpflash
-Version: 0.7.5
+Version: 0.7.6
 Summary: Flash and download tool for MicroPython firmwares
 Home-page: https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md
 License: MIT
 Keywords: MicroPython,firmware,flash,download,UF2,esptool
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8.1,<4.0
```

