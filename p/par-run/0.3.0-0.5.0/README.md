# Comparing `tmp/par_run-0.3.0.tar.gz` & `tmp/par_run-0.5.0.tar.gz`

## Comparing `par_run-0.3.0.tar` & `par_run-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,25 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.3.0/.python-version
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 par_run-0.3.0/commands.ini
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 par_run-0.3.0/requirements-dev.lock
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 par_run-0.3.0/requirements.lock
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/coverage_html.js
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/d_417a353b6036f046___init___py.html
--rw-r--r--   0        0        0   109310 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/d_417a353b6036f046_cli_py.html
--rw-r--r--   0        0        0   146586 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/d_417a353b6036f046_executor_py.html
--rw-r--r--   0        0        0    46396 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/d_417a353b6036f046_web_cli_py.html
--rw-r--r--   0        0        0    23112 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/d_417a353b6036f046_web_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/favicon_32.png
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/keybd_open.png
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/status.json
--rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 par_run-0.3.0/.reports/html/style.css
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 par_run-0.3.0/.vscode/launch.json
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/__init__.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/conftest.py
--rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/test_cli.py
--rw-r--r--   0        0        0    13957 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/test_executor.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/test_main.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 par_run-0.3.0/py_tests/test_web.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/__init__.py
--rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/cli.py
--rw-r--r--   0        0        0    16427 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/executor.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/web.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/static/css/style.css
--rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/static/js/app.js
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.3.0/src/par_run/templates/index.html
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.3.0/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.3.0/LICENSE
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 par_run-0.3.0/README.md
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 par_run-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 par_run-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 par_run-0.5.0/.git
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 par_run-0.5.0/.python-version
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 par_run-0.5.0/commands.toml
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 par_run-0.5.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 par_run-0.5.0/requirements.lock
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 par_run-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 par_run-0.5.0/.vscode/launch.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 par_run-0.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 par_run-0.5.0/py_tests/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 par_run-0.5.0/py_tests/conftest.py
+-rw-r--r--   0        0        0    20245 2020-02-02 00:00:00.000000 par_run-0.5.0/py_tests/test_cli.py
+-rw-r--r--   0        0        0    21682 2020-02-02 00:00:00.000000 par_run-0.5.0/py_tests/test_executor.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 par_run-0.5.0/py_tests/test_web.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 par_run-0.5.0/src/par_run/__init__.py
+-rw-r--r--   0        0        0    13539 2020-02-02 00:00:00.000000 par_run-0.5.0/src/par_run/cli.py
+-rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 par_run-0.5.0/src/par_run/executor.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 par_run-0.5.0/src/par_run/web.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 par_run-0.5.0/src/par_run/static/css/style.css
+-rw-r--r--   0        0        0     8623 2020-02-02 00:00:00.000000 par_run-0.5.0/src/par_run/static/js/app.js
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 par_run-0.5.0/src/par_run/templates/index.html
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 par_run-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 par_run-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 par_run-0.5.0/README.md
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 par_run-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 par_run-0.5.0/PKG-INFO
```

### Comparing `par_run-0.3.0/requirements-dev.lock` & `par_run-0.5.0/requirements-dev.lock`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 #   with-sources: false
 
 -e file:.
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
     # via httpx
+    # via par-run
     # via starlette
     # via watchfiles
 asttokens==2.4.1
     # via stack-data
+attrs==23.2.0
+    # via outcome
+    # via trio
 backports-tarfile==1.0.0
     # via jaraco-context
 bump-my-version==0.20.0
 certifi==2024.2.2
     # via httpcore
     # via httpx
     # via requests
@@ -36,18 +40,22 @@
     # via pytest-cov
 cryptography==42.0.5
     # via secretstorage
 decorator==5.1.1
     # via ipython
 docutils==0.21.1
     # via readme-renderer
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via anyio
     # via ipython
+    # via par-run
     # via pytest
+    # via trio
+execnet==2.1.1
+    # via pytest-xdist
 executing==2.0.1
     # via stack-data
 fastapi==0.110.1
     # via par-run
 h11==0.14.0
     # via httpcore
     # via uvicorn
@@ -56,14 +64,15 @@
 httptools==0.6.1
     # via uvicorn
 httpx==0.27.0
 idna==3.7
     # via anyio
     # via httpx
     # via requests
+    # via trio
 importlib-metadata==7.1.0
     # via keyring
     # via twine
 iniconfig==2.0.0
     # via pytest
 ipython==8.18.1
 jaraco-classes==3.4.0
@@ -93,14 +102,16 @@
     # via jaraco-classes
     # via jaraco-functools
 mypy==1.9.0
 mypy-extensions==1.0.0
     # via mypy
 nh3==0.2.17
     # via readme-renderer
+outcome==1.3.0.post0
+    # via trio
 packaging==24.0
     # via pytest
 parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 pkginfo==1.10.0
@@ -130,24 +141,24 @@
 pydantic-settings==2.2.1
     # via bump-my-version
 pygments==2.17.2
     # via ipython
     # via readme-renderer
     # via rich
 pytest==8.1.1
-    # via pytest-asyncio
     # via pytest-benchmark
     # via pytest-cov
     # via pytest-mock
     # via pytest-random-order
-pytest-asyncio==0.23.6
+    # via pytest-xdist
 pytest-benchmark==4.0.0
 pytest-cov==5.0.0
 pytest-mock==3.14.0
 pytest-random-order==1.1.1
+pytest-xdist==3.5.0
 python-dotenv==1.0.1
     # via pydantic-settings
     # via uvicorn
 pyyaml==6.0.1
     # via uvicorn
 questionary==1.10.0
     # via bump-my-version
@@ -174,32 +185,38 @@
 shellingham==1.5.4
     # via typer
 six==1.16.0
     # via asttokens
 sniffio==1.3.1
     # via anyio
     # via httpx
+    # via trio
+sortedcontainers==2.4.0
+    # via trio
 stack-data==0.6.3
     # via ipython
 starlette==0.37.2
     # via fastapi
 tomli==2.0.1
     # via coverage
     # via mypy
     # via pytest
 tomlkit==0.12.4
     # via bump-my-version
     # via par-run
 traitlets==5.14.2
     # via ipython
     # via matplotlib-inline
+trio==0.25.0
+    # via anyio
 twine==5.0.0
 typer==0.12.3
     # via par-run
 types-psutil==5.9.5.20240316
+types-requests==2.31.0.20240406
 types-toml==0.10.8.20240310
 typing-extensions==4.11.0
     # via anyio
     # via fastapi
     # via ipython
     # via mypy
     # via pydantic
@@ -207,14 +224,15 @@
     # via rich-click
     # via starlette
     # via typer
     # via uvicorn
 urllib3==2.2.1
     # via requests
     # via twine
+    # via types-requests
 uvicorn==0.29.0
     # via par-run
 uvloop==0.19.0
     # via uvicorn
 watchfiles==0.21.0
     # via uvicorn
 wcwidth==0.2.13
```

### Comparing `par_run-0.3.0/requirements.lock` & `par_run-0.5.0/requirements.lock`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 #   all-features: true
 #   with-sources: false
 
 -e file:.
 annotated-types==0.6.0
     # via pydantic
 anyio==4.3.0
+    # via par-run
     # via starlette
     # via watchfiles
 click==8.1.7
     # via typer
     # via uvicorn
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via anyio
+    # via par-run
 fastapi==0.110.1
     # via par-run
 h11==0.14.0
     # via uvicorn
 httptools==0.6.1
     # via uvicorn
 idna==3.7
```

### Comparing `par_run-0.3.0/.vscode/launch.json` & `par_run-0.5.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `par_run-0.3.0/py_tests/test_cli.py` & `par_run-0.5.0/py_tests/test_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,129 @@
 import itertools
+from collections import OrderedDict
+from pathlib import Path
 
 import psutil
 import pytest
+from pytest_mock import MockerFixture
 from typer.testing import CliRunner
 
 from par_run.cli import (
     CLICommandCBOnComp,
+    CLICommandCBOnRecv,
+    add_command_row,
+    add_table_break,
+    build_results_tbl,
     clean_up,
     cli_app,
+    command_status_to_emoji,
+    fmt_group_name,
     get_process_port,
     get_web_server_status,
     list_uvicorn_processes,
     start_web_server,
     stop_web_server,
 )
 from par_run.executor import Command, CommandGroup, CommandStatus
 
 runner = CliRunner()
 
 
 @pytest.fixture()
-def mock_command_group():
+def mock_command_group() -> CommandGroup:
     command1 = Command(name="cmd1", cmd="echo 'Hello, World!'")
     command2 = Command(name="cmd2", cmd="echo 'Goodbye, World!'")
-    commands = {"cmd1": command1, "cmd2": command2}
+    commands = OrderedDict()
+    commands[command1.name] = command1
+    commands[command2.name] = command2
     return CommandGroup(name="group1", cmds=commands)
 
 
 @pytest.fixture()
-def mock_command_group_part_fail():
+def mock_command_group_part_fail() -> CommandGroup:
     command1 = Command(name="cmd1", cmd="echo 'Hello, World!'")
     command2 = Command(name="cmd2", cmd="exit 1")
-    commands = {"cmd1": command1, "cmd2": command2}
+    commands = OrderedDict()
+    commands[command1.name] = command1
+    commands[command2.name] = command2
     return CommandGroup(name="group1", cmds=commands)
 
 
-def test_run(mocker, mock_command_group):
+def test_run(mocker: MockerFixture, mock_command_group: CommandGroup) -> None:
     mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run", "--show"])
     assert result.exit_code == 0
 
 
-def test_CLICommandCB_on_start(mocker):
+@pytest.mark.anyio
+async def test_CLICommandCB_on_start(mocker: MockerFixture) -> None:
     mock_rich_print = mocker.patch("par_run.cli.rich.print")
     cb = CLICommandCBOnComp()
     command = Command(name="cmd1", cmd="echo 'Hello'")
-    cb.on_start(command)
+    await cb.on_start(command)
     mock_rich_print.assert_called_once()
 
 
-def test_CLICommandCB_on_recv(mocker):
+@pytest.mark.anyio
+async def test_CLICommandCB_on_recv(mocker: MockerFixture) -> None:
     mock_rich_print = mocker.patch("par_run.cli.rich.print")
     cb = CLICommandCBOnComp()
     command = Command(name="cmd1", cmd="echo 'Hello'")
-    cb.on_recv(command, "Hello, World!")
+    await cb.on_recv(command, "Hello, World!")
     mock_rich_print.assert_called_once_with("Hello, World!")
 
 
+@pytest.mark.anyio
 @pytest.mark.parametrize("status", [CommandStatus.SUCCESS, CommandStatus.FAILURE])
-def test_CLICommandCB_on_term(mocker, status):
+async def test_CLICommandCB_on_term(mocker: MockerFixture, status: CommandStatus) -> None:
     mock_rich_print = mocker.patch("par_run.cli.rich.print")
     cb = CLICommandCBOnComp()
     command = Command(name="cmd1", cmd="echo 'Hello'")
     command.status = status
-    cb.on_term(command, 0)
+    await cb.on_term(command, 0)
     assert mock_rich_print.called
 
 
-def test_clean_up(mocker, tmp_path):
+def test_clean_up(mocker: MockerFixture, tmp_path: Path) -> None:
     pid_file = tmp_path / ".par-run.uvicorn.pid"
     pid_file.write_text("1234")
     mocker.patch("par_run.cli.PID_FILE", str(pid_file))
     clean_up()
     assert not pid_file.exists()
 
 
 @pytest.mark.parametrize("command", ["start", "stop", "restart", "status"])
-def test_web(mocker, command):
+def test_web(mocker: MockerFixture, command: str) -> None:
     mocker.patch("par_run.cli.start_web_server")
     mocker.patch("par_run.cli.stop_web_server")
     mocker.patch("par_run.cli.get_web_server_status")
     result = runner.invoke(cli_app, ["web", command])
     assert result.exit_code == 0
 
 
-def test_web_fail(mocker):
+def test_web_fail(mocker: MockerFixture) -> None:
     mocker.patch("par_run.cli.start_web_server")
     mocker.patch("par_run.cli.stop_web_server")
     mocker.patch("par_run.cli.get_web_server_status")
     result = runner.invoke(cli_app, ["web", "NOT_A_CMD"])
     assert result.exit_code != 0
 
 
-def test_start_web_server(mocker, tmp_path):
+def test_start_web_server(mocker: MockerFixture, tmp_path: Path) -> None:
     mocker.patch("par_run.cli.subprocess.Popen")
     mocker.patch("par_run.cli.os.path.isfile", return_value=False)
     mocker.patch("par_run.cli.time.time_ns", side_effect=[0, 3 * 10**9 + 1])  # Simulate 3 seconds passing
     pid_file = tmp_path / ".par-run.uvicorn.pid"
     mocker.patch("par_run.cli.PID_FILE", str(pid_file))
     start_web_server(8000)
     assert pid_file.exists()
 
 
-def test_start_web_server_running(mocker, tmp_path):
+def test_start_web_server_running(mocker: MockerFixture, tmp_path: Path) -> None:
     # Setup: Mock subprocess.Popen to simulate the server process
     mock_process = mocker.MagicMock()
     mocker.patch("par_run.cli.subprocess.Popen", return_value=mock_process)
     mock_process.pid = 12345  # Example PID for the server process
 
     # Setup: Mock os.path.isfile to simulate the PID file does not exist initially
     mocker.patch("par_run.cli.os.path.isfile", return_value=False)
@@ -137,24 +153,31 @@
     # Verify: Check that the server is detected as running on the correct port
     mock_echo.assert_any_call("UVicorn server is running on port 8000 in 2000.00 ms.")
 
     # Cleanup: Ensure PID file is created
     assert pid_file.exists()
 
 
-def test_stop_web_server(mocker, tmp_path):
+def test_stop_web_server(mocker: MockerFixture, tmp_path: Path) -> None:
     pid_file = tmp_path / ".par-run.uvicorn.pid"
     pid_file.write_text("1234")
     mocker.patch("par_run.cli.PID_FILE", str(pid_file))
     mocker.patch("par_run.cli.os.kill")
     stop_web_server()
     assert not pid_file.exists()
 
 
-def test_get_web_server_status(mocker, tmp_path):
+def test_stop_web_server_no_pid_file(mocker: MockerFixture, tmp_path: Path) -> None:
+    pid_file = tmp_path / ".par-run.uvicorn.pid"
+    mocker.patch("par_run.cli.PID_FILE", str(pid_file))
+    mocker.patch("par_run.cli.os.kill")
+    stop_web_server()
+
+
+def test_get_web_server_status(mocker: MockerFixture, tmp_path: Path) -> None:
     pid_file = tmp_path / ".par-run.uvicorn.pid"
     mocker.patch("par_run.cli.PID_FILE", str(pid_file))
     mocker.patch("par_run.cli.typer.echo")
     # Test with no PID file
     get_web_server_status()
     pid_file.write_text("1234")
     # Test with PID file but no process
@@ -162,126 +185,142 @@
     get_web_server_status()
     # Test with PID file and process
     mocker.patch("par_run.cli.psutil.pid_exists", return_value=True)
     mocker.patch("par_run.cli.get_process_port", return_value=8000)
     get_web_server_status()
 
 
-def test_run_with_specific_groups(mocker, mock_command_group):
+def test_run_with_on_recv(mocker: MockerFixture, mock_command_group: CommandGroup) -> None:
+    read_mock = mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
+    mocker.patch("par_run.cli.rich.print")
+    result = runner.invoke(cli_app, ["run", "--style", "recv"])
+    assert result.exit_code == 0
+    read_mock.assert_called_once()
+
+
+def test_run_with_on_comp(mocker: MockerFixture, mock_command_group: CommandGroup) -> None:
+    read_mock = mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
+    mocker.patch("par_run.cli.rich.print")
+    result = runner.invoke(cli_app, ["run", "--style", "comp"])
+    assert result.exit_code == 0
+    read_mock.assert_called_once()
+
+
+def test_run_with_specific_groups(mocker: MockerFixture, mock_command_group: CommandGroup) -> None:
     read_mock = mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run", "--groups", "group1"])
     assert result.exit_code == 0
     read_mock.assert_called_once()
 
 
-def test_run_with_fails(mocker, mock_command_group_part_fail):
+def test_run_with_fails(mocker: MockerFixture, mock_command_group_part_fail: CommandGroup) -> None:
     read_mock = mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group_part_fail])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run"])
     assert result.exit_code != 0
     read_mock.assert_called_once()
 
 
-def test_run_with_specific_cmds(mocker, mock_command_group):
+def test_run_with_specific_cmds(mocker: MockerFixture, mock_command_group: CommandGroup) -> None:
     mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run", "--cmds", "cmd1"])
     assert result.exit_code == 0
     # Add additional assertions to check if the command was filtered correctly
 
 
-def test_run_with_nonexistent_group(mocker, mock_command_group):
+def test_run_with_nonexistent_group(mocker: MockerFixture, mock_command_group: CommandGroup) -> None:
     mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run", "--groups", "nonexistent"])
     assert result.exit_code == 0
     # Add assertion to ensure no commands are run and appropriate message is displayed
 
 
-def test_run_with_nonexistent_cmd(mocker, mock_command_group):
+def test_run_with_nonexistent_cmd(mocker: MockerFixture, mock_command_group: CommandGroup) -> None:
     mocker.patch("par_run.cli.read_commands_toml", return_value=[mock_command_group])
     mocker.patch("par_run.cli.rich.print")
     result = runner.invoke(cli_app, ["run", "--cmds", "nonexistent"])
     assert result.exit_code == 0
     # Add assertion to ensure no commands are run and appropriate message is displayed
 
 
-def test_start_web_server_already_running(mocker, tmp_path):
+def test_start_web_server_already_running(mocker: MockerFixture, tmp_path: Path) -> None:
     pid_file = tmp_path / ".par-run.uvicorn.pid"
     pid_file.write_text("1234")
     mocker.patch("par_run.cli.PID_FILE", str(pid_file))
     mocker.patch("par_run.cli.typer.echo")
     with pytest.raises(SystemExit):
         start_web_server(8000)
 
 
-def test_get_web_server_status_running(mocker, tmp_path):
+def test_get_web_server_status_running(mocker: MockerFixture, tmp_path: Path) -> None:
     pid_file = tmp_path / ".par-run.uvicorn.pid"
     pid_file.write_text("1234")
     mocker.patch("par_run.cli.PID_FILE", str(pid_file))
     mocker.patch("par_run.cli.psutil.pid_exists", return_value=True)
     mocker.patch("par_run.cli.get_process_port", return_value=8000)
     mocker.patch("par_run.cli.typer.echo")
     get_web_server_status()
     # Add assertion to check the status message for a running server
 
 
-def test_get_web_server_status_not_running_pid_file_exists(mocker, tmp_path):
+def test_get_web_server_status_not_running_pid_file_exists(mocker: MockerFixture, tmp_path: Path) -> None:
     pid_file = tmp_path / ".par-run.uvicorn.pid"
     pid_file.write_text("1234")
     mocker.patch("par_run.cli.PID_FILE", str(pid_file))
     mocker.patch("par_run.cli.psutil.pid_exists", return_value=False)
     mocker.patch("par_run.cli.typer.echo")
     get_web_server_status()
     # Add assertion to check the status message and cleanup action when the server is not running but PID file exists
 
 
-def test_start_web_server_failure_to_start(mocker, tmp_path):
+def test_start_web_server_failure_to_start(mocker: MockerFixture, tmp_path: Path) -> None:
     mocker.patch("par_run.cli.subprocess.Popen", side_effect=Exception("Failed to start"))
     pid_file = tmp_path / ".par-run.uvicorn.pid"
     mocker.patch("par_run.cli.PID_FILE", str(pid_file))
     mocker.patch("par_run.cli.typer.echo")
     with pytest.raises(Exception, match="Failed to start"):
         start_web_server(8000)
 
 
-def test_stop_web_server_failure(mocker, tmp_path):
+def test_stop_web_server_failure(mocker: MockerFixture, tmp_path: Path) -> None:
     pid_file = tmp_path / ".par-run.uvicorn.pid"
     pid_file.write_text("1234")
     mocker.patch("par_run.cli.PID_FILE", str(pid_file))
     mocker.patch("par_run.cli.os.kill", side_effect=Exception("Failed to kill"))
     mocker.patch("par_run.cli.typer.echo")
     with pytest.raises(Exception, match="Failed to kill"):
         stop_web_server()
 
 
-def test_get_process_port(mocker):
+def test_get_process_port(mocker: MockerFixture) -> None:
     # Mock psutil.Process and its connections method
     mock_process = mocker.patch("par_run.cli.psutil.Process")
     mock_conn = mocker.MagicMock()
     run_port = 8000
     mock_conn.laddr.port = run_port
     mock_process.return_value.connections.return_value = [mock_conn]
 
     example_pid = 1234
     port = get_process_port(example_pid)
     assert port == run_port
 
 
-def test_get_process_port_no_connections(mocker):
+def test_get_process_port_no_connections(mocker: MockerFixture) -> None:
     # Mock psutil.Process to return no connections
     mock_process = mocker.patch("par_run.cli.psutil.Process")
     mock_process.return_value.connections.return_value = []
 
     port = get_process_port(1234)  # Example PID
     assert port is None
 
 
-def test_list_uvicorn_processes(mocker):
+def test_list_uvicorn_processes(mocker: MockerFixture) -> None:
     # Mock psutil.process_iter to yield mock processes
     mock_process_iter = mocker.patch("par_run.cli.psutil.process_iter")
     mock_process_uvicorn = mocker.MagicMock()
     mock_process_uvicorn.name.return_value = "uvicorn"
     mock_process_uvicorn.pid = 1234
     mock_process_other = mocker.MagicMock()
     mock_process_other.name.return_value = "other_process"
@@ -292,30 +331,30 @@
     list_uvicorn_processes()
 
     # Directly assert the calls made to typer.echo
     mock_echo.assert_any_call("Other UVicorn processes:")
     mock_echo.assert_any_call("PID: 1234, Name: uvicorn")
 
 
-def test_list_no_uvicorn_processes(mocker):
+def test_list_no_uvicorn_processes(mocker: MockerFixture) -> None:
     # Mock psutil.process_iter to yield no UVicorn processes
     mock_process_iter = mocker.patch("par_run.cli.psutil.process_iter")
     mock_process_other = mocker.MagicMock()
     mock_process_other.name.return_value = "other_process"
     mock_process_iter.return_value = [mock_process_other]
 
     mock_echo = mocker.patch("par_run.cli.typer.echo")
 
     list_uvicorn_processes()
 
     # Directly assert the calls made to typer.echo
     mock_echo.assert_any_call("No other UVicorn processes found.")
 
 
-def test_list_uvicorn_processes_with_exceptions(mocker):
+def test_list_uvicorn_processes_with_exceptions(mocker: MockerFixture) -> None:
     # Mock psutil.process_iter to yield processes that raise exceptions
     mock_process_iter = mocker.patch("par_run.cli.psutil.process_iter")
 
     # Create mock processes that raise the exceptions when name() is called
     mock_process_no_such_process = mocker.MagicMock()
     mock_process_no_such_process.name.side_effect = psutil.NoSuchProcess(pid=123)
 
@@ -339,15 +378,15 @@
     # Since all processes raise exceptions, the output should indicate no UVicorn processes found
     mock_echo.assert_any_call("No other UVicorn processes found.")
 
     # Optionally, assert that the exceptions were caught and did not cause the function to fail
     # This can be inferred from the fact that the function executed to completion and made the expected call to mock_echo
 
 
-def test_get_web_server_status_running_no_port(mocker, tmp_path):
+def test_get_web_server_status_running_no_port(mocker: MockerFixture, tmp_path: Path) -> None:
     # Setup: Create a temporary PID file with a mock PID
     pid_file = tmp_path / ".par-run.uvicorn.pid"
     pid_file.write_text("1234")  # Example PID
     mocker.patch("par_run.cli.PID_FILE", str(pid_file))
 
     # Mock psutil.pid_exists to return True, indicating the process exists
     mocker.patch("par_run.cli.psutil.pid_exists", return_value=True)
@@ -359,7 +398,129 @@
     mock_echo = mocker.patch("par_run.cli.typer.echo")
 
     # Execute: Call the function to test
     get_web_server_status()
 
     # Verify: Check that the appropriate message is output when the port cannot be determined
     mock_echo.assert_any_call("UVicorn server is running with pid=1234, couldn't determine port.")
+
+
+def test_web_command_enum() -> None:
+    from par_run.cli import WebCommand
+
+    for cmd in WebCommand:
+        assert isinstance(cmd.value, str)
+        assert str(cmd) == cmd.value
+
+
+@pytest.mark.anyio
+async def test_command_cb_comp_success(mocker: MockerFixture) -> None:
+    mocker.patch("par_run.cli.rich.print")
+    cb = CLICommandCBOnComp()
+    command = Command(name="cmd1", cmd="echo 'Hello'")
+    await cb.on_start(command)
+    await cb.on_recv(command, "Hello, World!")
+    command.status = CommandStatus.SUCCESS
+    await cb.on_term(command, 0)
+
+
+@pytest.mark.anyio
+async def test_command_cb_comp_fail(mocker: MockerFixture) -> None:
+    mocker.patch("par_run.cli.rich.print")
+    cb = CLICommandCBOnComp()
+    command = Command(name="cmd1", cmd="echo 'Hello'")
+    await cb.on_start(command)
+    await cb.on_recv(command, "Hello, World!")
+    command.status = CommandStatus.FAILURE
+    await cb.on_term(command, 1)
+
+
+@pytest.mark.anyio
+async def test_command_cb_recv_success(mocker: MockerFixture) -> None:
+    mocker.patch("par_run.cli.rich.print")
+    cb = CLICommandCBOnRecv()
+    command = Command(name="cmd1", cmd="echo 'Hello'")
+    await cb.on_start(command)
+    await cb.on_recv(command, "Hello, World!")
+    command.status = CommandStatus.SUCCESS
+    await cb.on_term(command, 0)
+
+
+@pytest.mark.anyio
+async def test_command_cb_recv_fail(mocker: MockerFixture) -> None:
+    mocker.patch("par_run.cli.rich.print")
+    cb = CLICommandCBOnRecv()
+    command = Command(name="cmd1", cmd="echo 'Hello'")
+    await cb.on_start(command)
+    await cb.on_recv(command, "Hello, World!")
+    command.status = CommandStatus.FAILURE
+    await cb.on_term(command, 1)
+
+
+def test_results_table() -> None:
+    tbl = build_results_tbl()
+    cols = ["Group", "Name", "Command", "Status", "Elapsed"]
+    assert tbl is not None
+    assert len(tbl.columns) == len(cols)
+    tbl_cols = [col.header for col in tbl.columns]
+    assert all([col in tbl_cols for col in cols])
+    command = Command(name="cmd1", cmd="echo 'Hello'")
+    add_command_row(tbl, command, "group1")
+    add_table_break(tbl)
+    add_command_row(tbl, command, "group2")
+    add_table_break(tbl)
+    add_command_row(tbl, command, "group3")
+
+
+def test_fmt_group_name() -> None:
+    cmd_name = "group1"
+    cmd_grp = CommandGroup(name=cmd_name, cmds=OrderedDict())
+    cmd_grp.status = CommandStatus.SUCCESS
+    fmt_res = fmt_group_name(cmd_grp)
+    assert cmd_name in fmt_res
+    assert "[green]" in fmt_res
+
+    cmd_grp = CommandGroup(name=cmd_name, cmds=OrderedDict())
+    cmd_grp.status = CommandStatus.FAILURE
+    fmt_res = fmt_group_name(cmd_grp)
+    assert cmd_name in fmt_res
+    assert "[red]" in fmt_res
+
+    cmd_grp = CommandGroup(name=cmd_name, cmds=OrderedDict())
+    cmd_grp.status = CommandStatus.NOT_STARTED
+    fmt_res = fmt_group_name(cmd_grp)
+    assert cmd_name in fmt_res
+    assert "[yellow]" in fmt_res
+
+
+def test_add_command_row_colours() -> None:
+    command = Command(name="cmd1", cmd="echo 'Hello'")
+    command.status = CommandStatus.SUCCESS
+    emoji, row_style = command_status_to_emoji(command)
+    assert emoji
+    assert "green" in row_style
+
+    command.status = CommandStatus.FAILURE
+    emoji, row_style = command_status_to_emoji(command)
+    assert emoji
+    assert "red" in row_style
+
+    command.status = CommandStatus.NOT_STARTED
+    emoji, row_style = command_status_to_emoji(command)
+    assert emoji
+    assert "red" in row_style
+
+    command.status = CommandStatus.RUNNING
+    emoji, row_style = command_status_to_emoji(command)
+    assert emoji
+    assert "red" in row_style
+
+    command.status = CommandStatus.TIMEOUT
+    emoji, row_style = command_status_to_emoji(command)
+    assert emoji
+    assert "orange1" in row_style
+
+
+def test_cli_app() -> None:
+    with pytest.raises(SystemExit):
+        app = cli_app(["--help"])
+        assert app
```

### Comparing `par_run-0.3.0/src/par_run/cli.py` & `par_run-0.5.0/src/par_run/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """CLI for running commands in parallel"""
 
 import contextlib
 import enum
 from collections import OrderedDict
 from pathlib import Path
-from typing import Annotated, Optional
+from typing import Annotated, Any, Optional
 
+import anyio
 import rich
 import typer
 
 from .executor import Command, CommandGroup, CommandStatus, ProcessingStrategy, read_commands_toml
 
 PID_FILE = ".par-run.uvicorn.pid"
 
 cli_app = typer.Typer()
 
 
 # Web only functions
-def clean_up():
+def clean_up() -> None:
     """Clean up by removing the PID file."""
     Path(PID_FILE).unlink()
     typer.echo("Cleaned up PID file.")
 
 
-def start_web_server(port: int):
+def start_web_server(port: int) -> None:
     """Start the web server"""
     if Path(PID_FILE).is_file():
         typer.echo("UVicorn server is already running.")
         sys.exit(1)
     with Path(PID_FILE).open("w", encoding="utf-8") as pid_file:
         typer.echo(f"Starting UVicorn server on port {port}...")
         uvicorn_command = [
@@ -45,23 +46,24 @@
         wait_time = 3 * 10**9  # 3 seconds
         start_time = time.time_ns()
 
         while time.time_ns() - start_time < wait_time:
             test_port = get_process_port(process.pid)
             if port == test_port:
                 typer.echo(f"UVicorn server is running on port {port} in {(time.time_ns() - start_time)/10**6:.2f} ms.")
+                typer.echo(f"Server running at http://localhost:{port}/")
                 break
             time.sleep(0.1)  # Poll every 0.1 seconds
 
         else:
             typer.echo(f"UVicorn server did not respond within {wait_time} seconds.")
             typer.echo("run 'par-run web status' to check the status.")
 
 
-def stop_web_server():
+def stop_web_server() -> None:
     """Stop the UVicorn server by reading its PID from the PID file and sending a termination signal."""
     if not Path(PID_FILE).is_file():
         typer.echo("UVicorn server is not running.")
         return
 
     with Path(PID_FILE).open() as pid_file:
         pid = int(pid_file.read().strip())
@@ -77,15 +79,15 @@
     connections = process.connections()
     if connections:
         port = connections[0].laddr.port
         return port
     return None
 
 
-def list_uvicorn_processes():
+def list_uvicorn_processes() -> None:
     """Check for other UVicorn processes and list them"""
     uvicorn_processes = []
     with contextlib.suppress(psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
         for process in psutil.process_iter():
             process_name = process.name()
             if "uvicorn" in process_name.lower():
                 uvicorn_processes.append(process)
@@ -94,15 +96,15 @@
         typer.echo("Other UVicorn processes:")
         for process in uvicorn_processes:
             typer.echo(f"PID: {process.pid}, Name: {process.name()}")
     else:
         typer.echo("No other UVicorn processes found.")
 
 
-def get_web_server_status():
+def get_web_server_status() -> None:
     """Get the status of the UVicorn server by reading its PID from the PID file."""
     if not Path(PID_FILE).is_file():
         typer.echo("No pid file found. Server likely not running.")
         list_uvicorn_processes()
         return
 
     with Path(PID_FILE).open() as pid_file:
@@ -122,41 +124,52 @@
     """Web command enumeration."""
 
     START = "start"
     STOP = "stop"
     RESTART = "restart"
     STATUS = "status"
 
-    def __str__(self):
+    def __str__(self) -> str:
+        return self.value
+
+
+class AsyncBackend(enum.Enum):
+    """Async backend enumeration."""
+
+    TRIO = "trio"
+    ASYNCIO = "asyncio"
+    ASYNCIO_NATIVE = "asyncio-native"
+
+    def __str__(self) -> str:
         return self.value
 
 
 class CLICommandCBOnComp:
-    def on_start(self, cmd: Command):
-        rich.print(f"[blue bold]Completed command {cmd.name}[/]")
+    async def on_start(self, cmd: Command) -> None:
+        rich.print(f"[blue bold]{cmd.name}: Started[/]")
 
-    def on_recv(self, _: Command, output: str):
+    async def on_recv(self, _: Command, output: str) -> None:
         rich.print(output)
 
-    def on_term(self, cmd: Command, exit_code: int):
+    async def on_term(self, cmd: Command, exit_code: int) -> None:
         """Callback function for when a command receives output"""
         if cmd.status == CommandStatus.SUCCESS:
-            rich.print(f"[green bold]Command {cmd.name} finished[/]")
+            rich.print(f"[green bold]{cmd.name}: Finished[/]")
         elif cmd.status == CommandStatus.FAILURE:
-            rich.print(f"[red bold]Command {cmd.name} failed, {exit_code=:}[/]")
+            rich.print(f"[red bold]{cmd.name}: Failed, {exit_code=:}[/]")
 
 
 class CLICommandCBOnRecv:
-    def on_start(self, cmd: Command):
+    async def on_start(self, cmd: Command) -> None:
         rich.print(f"[blue bold]{cmd.name}: Started[/]")
 
-    def on_recv(self, cmd: Command, output: str):
+    async def on_recv(self, cmd: Command, output: str) -> None:
         rich.print(f"{cmd.name}: {output}")
 
-    def on_term(self, cmd: Command, exit_code: int):
+    async def on_term(self, cmd: Command, exit_code: int) -> None:
         """Callback function for when a command receives output"""
         if cmd.status == CommandStatus.SUCCESS:
             rich.print(f"[green bold]{cmd.name}: Finished[/]")
         elif cmd.status == CommandStatus.FAILURE:
             rich.print(f"[red bold]{cmd.name}: Failed, {exit_code=:}[/]")
 
 
@@ -176,20 +189,18 @@
     minutes = (int(seconds) % 3600) // 60
     seconds = seconds % 60  # Keeping the fractional part of seconds
 
     # Return formatted string with seconds rounded to 2 d.p.
     return f"{hours:02}:{minutes:02}:{seconds:06.3f}"
 
 
-def show_commands(groups: list[CommandGroup]):
+def show_commands(groups: list[CommandGroup]) -> None:
     for grp in groups:
         rich.print(f"[blue bold]Group: {grp.name}[/]")
-        rich.print(
-            f"Params: cont_on_fail={grp.cont_on_fail}, serial={grp.serial}, timeout={grp.timeout}, retries={grp.retries}"
-        )
+        rich.print(f"Params: cont_on_fail={grp.cont_on_fail}, serial={grp.serial}, timeout={grp.timeout}")
         for cmd in grp.cmds.values():
             rich.print(f"[green bold]{cmd.name}[/]: {cmd.cmd}")
 
 
 def filter_groups(
     group_list: list[CommandGroup], filter_groups: Optional[str], filter_cmds: Optional[str]
 ) -> list[CommandGroup]:
@@ -225,80 +236,94 @@
     res_tbl.add_column("Name", style="bold blue", width=name_w, no_wrap=True)
     res_tbl.add_column("Command", style="bold blue", width=cmd_w, no_wrap=True)
     res_tbl.add_column("Status", style="bold blue", width=status_w, no_wrap=True)
     res_tbl.add_column("Elapsed", style="bold blue", width=elap_w, no_wrap=True)
     return res_tbl
 
 
-def add_command_row(tbl: rich.table.Table, cmd: Command, group_name: str) -> rich.table.Table:
-    elap_str = format_elapsed_time(cmd.elapsed) if cmd.elapsed else "XX:XX:XX.xxx"
-
+def command_status_to_emoji(cmd: Command) -> tuple[str, str]:
     if cmd.status == CommandStatus.SUCCESS:
-        cmd_status = "✅"
-        row_style = "green"
+        return ("✅", "green")
     elif cmd.status == CommandStatus.FAILURE:
-        cmd_status = "❌"
-        row_style = "red"
+        return ("❌", "red")
+    elif cmd.status == CommandStatus.TIMEOUT:
+        return ("⏰", "orange1")
     else:
-        cmd_status = "⏳"
-        row_style = "yellow"
+        return ("🚫", "red")
+
 
-    tbl.add_row(group_name, cmd.name, cmd.cmd, cmd_status, elap_str, style=row_style)
+def add_command_row(tbl: rich.table.Table, cmd: Command, group_name: str) -> rich.table.Table:
+    elap_str = format_elapsed_time(cmd.elapsed) if cmd.elapsed else "XX:XX:XX.xxx"
+    emoji, row_style = command_status_to_emoji(cmd)
+    tbl.add_row(group_name, cmd.name, cmd.cmd, emoji, elap_str, style=row_style)
     return tbl
 
 
 def fmt_group_name(cmd_group: CommandGroup) -> str:
     if cmd_group.status == CommandStatus.SUCCESS:
         return f"[green]{cmd_group.name}[/]"
     elif cmd_group.status == CommandStatus.FAILURE:
         return f"[red]{cmd_group.name}[/]"
     else:
         return f"[yellow]{cmd_group.name}[/]"
 
 
-style_default = typer.Option(help="Processing strategy", default="comp")
+style_default = typer.Option(help="Processing strategy, for serial commands this is always --recv", default="comp")
 show_default = typer.Option(help="Show available groups and commands", default=False)
 pyproj_default = typer.Option(help="The default toml file to use", default=Path("pyproject.toml"))
 groups_default = typer.Option(help="Run a specific group of commands, comma spearated", default=None)
 cmds_default = typer.Option(help="Run specific commands, comma separated", default=None)
+backend_default = typer.Option(help="The backend to use", default="trio")
+
+backend_options: dict[AsyncBackend, Any] = {
+    AsyncBackend.TRIO: {"backend": "trio", "backend_options": {}},
+    AsyncBackend.ASYNCIO: {"backend": "asyncio", "backend_options": {"use_uvloop": True}},
+    AsyncBackend.ASYNCIO_NATIVE: {"backend": "asyncio", "backend_options": {"use_uvloop": False}},
+}
 
 
 @cli_app.command()
-def run(
+def run(  # noqa: PLR0913
     style: Annotated[ProcessingStrategy, typer.Option] = style_default,
     show: Annotated[bool, typer.Option] = show_default,
     file: Annotated[Path, typer.Option] = pyproj_default,
     groups: Annotated[Optional[str], typer.Option] = groups_default,
     cmds: Annotated[Optional[str], typer.Option] = cmds_default,
-):
+    backend: Annotated[AsyncBackend, typer.Option] = backend_default,
+) -> None:
     """Run commands in parallel"""
     # Overall exit code, need to track all command exit codes to update this
     exit_code = 0
     st_all = time.perf_counter()
 
+    actual_backend = backend_options[backend]["backend"]
+    actual_backend_opts = backend_options[backend]["backend_options"]
+
     master_groups = read_commands_toml(file)
     if show:
         return show_commands(master_groups)
 
     master_groups = filter_groups(master_groups, groups, cmds)
 
     if not master_groups:
         rich.print("[blue]No groups or commands found.[/]")
         raise typer.Exit(0)
 
     for grp in master_groups:
+        # Run the async function with Trio's event loop
         if style == ProcessingStrategy.ON_COMP:
-            exit_code = grp.run(style, CLICommandCBOnComp())
+            anyio.run(grp.run, style, CLICommandCBOnComp(), backend=actual_backend, backend_options=actual_backend_opts)
         elif style == ProcessingStrategy.ON_RECV:
-            exit_code = grp.run(style, CLICommandCBOnRecv())
+            anyio.run(grp.run, style, CLICommandCBOnRecv(), backend=actual_backend, backend_options=actual_backend_opts)
         else:
-            raise typer.BadParameter("Invalid processing strategy")
-        if exit_code != 0 and not grp.cont_on_fail:
-            break
-
+            raise typer.BadParameter("Invalid processing strategy")  # pragma: no cover
+        if grp.status != CommandStatus.SUCCESS:
+            exit_code = 1
+            if not grp.cont_on_fail:
+                break
     # Summarise the results
     console = rich.console.Console()
     res_tbl = build_results_tbl()
 
     for grp_ix, grp in enumerate(master_groups):
         for ix, cmd in enumerate(grp.cmds.values()):
             if grp_ix > 0 and ix == 0:
@@ -333,27 +358,24 @@
     command_default = typer.Argument(..., help="command to control/interract with the web server")
     port_default = typer.Option(8001, help="Port to run the web server")
 
     @cli_app.command()
     def web(
         command: WebCommand = command_default,
         port: int = port_default,
-    ):
+    ) -> None:
         """Run the web server"""
         if command == WebCommand.START:
             start_web_server(port)
         elif command == WebCommand.STOP:
             stop_web_server()
         elif command == WebCommand.RESTART:
             stop_web_server()
             start_web_server(port)
         elif command == WebCommand.STATUS:
             get_web_server_status()
         else:
-            typer.echo(f"Not a valid command '{command}'", err=True)
-            raise typer.Abort()
+            typer.echo(f"Not a valid command '{command}'", err=True)  # pragma: no cover
+            raise typer.Abort()  # pragma: no cover
 
 except ImportError:  # pragma: no cover
     pass  # pragma: no cover
-
-if __name__ == "__main__":
-    cli_app()
```

### Comparing `par_run-0.3.0/src/par_run/executor.py` & `par_run-0.5.0/src/par_run/executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 """Todo"""
 
-import asyncio
-import configparser
 import enum
-import multiprocessing as mp
 import os
-import queue
 import subprocess
 import time
 from collections import OrderedDict
-from concurrent.futures import Future, ProcessPoolExecutor
+from collections.abc import AsyncIterable
 from pathlib import Path
-from queue import Queue
-from typing import Any, Optional, Protocol, TypeVar, Union
+from typing import Any, Optional, Protocol, Union, cast
 
+import anyio
+import anyio.to_thread
 import tomlkit
 from pydantic import BaseModel, ConfigDict, Field
 
-# Type alias for a generic future.
-GenFuture = Union[Future, asyncio.Future]
-
-ContextT = TypeVar("ContextT")
+internal_error_ret_code = 999
 
 
 class ProcessingStrategy(enum.Enum):
     """Enum for processing strategies."""
 
     ON_COMP = "comp"
     ON_RECV = "recv"
@@ -33,18 +27,20 @@
 class CommandStatus(enum.Enum):
     """Enum for command status."""
 
     NOT_STARTED = "Not Started"
     RUNNING = "Running"
     SUCCESS = "Success"
     FAILURE = "Failure"
+    TIMEOUT = "Timeout"
+    CANCELLED = "Cancelled"
 
     def completed(self) -> bool:
         """Return True if the command has completed."""
-        return self in [CommandStatus.SUCCESS, CommandStatus.FAILURE]
+        return self in [CommandStatus.SUCCESS, CommandStatus.FAILURE, CommandStatus.TIMEOUT, CommandStatus.CANCELLED]
 
 
 class Command(BaseModel):
     """Holder for a command and its name."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
@@ -52,15 +48,14 @@
     cmd: str
     passenv: Optional[list[str]] = Field(default=None)
     setenv: Optional[dict[str, str]] = Field(default=None)
     status: CommandStatus = CommandStatus.NOT_STARTED
     unflushed: list[str] = Field(default=[], exclude=True)
     num_non_empty_lines: int = Field(default=0, exclude=True)
     ret_code: Optional[int] = Field(default=None, exclude=True)
-    fut: Optional[GenFuture] = Field(default=None, exclude=True)
     start_time: Optional[float] = Field(default=None, exclude=True)
     elapsed: Optional[float] = Field(default=None, exclude=True)
 
     def incr_line_count(self, line: str) -> None:
         """Increment the non-empty line count."""
         if line.strip():
             self.num_non_empty_lines += 1
@@ -69,286 +64,164 @@
         """Append a line to the output and increment the non-empty line count."""
         self.unflushed.append(line)
 
     def clear_unflushed(self) -> None:
         """Clear the unflushed output."""
         self.unflushed.clear()
 
-    def set_ret_code(self, ret_code: int):
+    def set_ret_code(self, ret_code: int) -> None:
         """Set the return code and status of the command."""
         if self.start_time:
             self.elapsed = time.perf_counter() - self.start_time
         self.ret_code = ret_code
-        if self.fut:
-            self.fut.cancel()
-            self.fut = None
         if ret_code == 0:
             self.status = CommandStatus.SUCCESS
         else:
             self.status = CommandStatus.FAILURE
 
-    def set_running(self):
+    def set_timeout(self) -> None:
+        """Set the command status to timeout."""
+        self.status = CommandStatus.TIMEOUT
+        if self.start_time:
+            self.elapsed = time.perf_counter() - self.start_time
+        self.ret_code = internal_error_ret_code
+
+    def set_running(self) -> None:
         """Set the command status to running."""
         self.start_time = time.perf_counter()
         self.status = CommandStatus.RUNNING
 
-
-class CommandCB(Protocol):
-    def on_start(self, cmd: Command) -> None: ...
-    def on_recv(self, cmd: Command, output: str) -> None: ...
-    def on_term(self, cmd: Command, exit_code: int) -> None: ...
+    def set_cancelled(self) -> None:
+        """Set the command status to cancelled."""
+        self.status = CommandStatus.CANCELLED
+        self.ret_code = internal_error_ret_code
 
 
-class CommandAsyncCB(Protocol):
+class CommandCB(Protocol):
     async def on_start(self, cmd: Command) -> None: ...
     async def on_recv(self, cmd: Command, output: str) -> None: ...
     async def on_term(self, cmd: Command, exit_code: int) -> None: ...
 
 
-class QRetriever:
-    def __init__(self, q: Queue, timeout: int, retries: int):
-        self.q = q
-        self.timeout = timeout
-        self.retries = retries
-
-    def get(self):
-        retry_count = 0
-        while True:
-            try:
-                return self.q.get(block=True, timeout=self.timeout)
-            except queue.Empty:  # noqa: PERF203
-                if retry_count < self.retries:
-                    retry_count += 1
-                    continue
-                else:
-                    raise TimeoutError("Timeout waiting for command output") from None
-
-    def __str__(self) -> str:
-        return f"QRetriever(timeout={self.timeout}, retries={self.retries})"
-
-
 class CommandGroup(BaseModel):
     """Holder for a group of commands."""
 
     name: str
     desc: Optional[str] = None
     cmds: OrderedDict[str, Command] = Field(default_factory=OrderedDict)
     timeout: int = Field(default=30)
-    retries: int = Field(default=3)
     cont_on_fail: bool = Field(default=False)
     serial: bool = Field(default=False)
     status: CommandStatus = CommandStatus.NOT_STARTED
 
-    def update_status(self, cmds: OrderedDict[str, Command]):
+    def update_status(self, cmds: OrderedDict[str, Command]) -> None:
         """Update the status of the command group."""
         if all(cmd.status == CommandStatus.SUCCESS for cmd in cmds.values()):
             self.status = CommandStatus.SUCCESS
         else:
             self.status = CommandStatus.FAILURE
 
-    async def run_async(
-        self,
-        strategy: ProcessingStrategy,
-        callbacks: CommandAsyncCB,
-    ):
-        q = mp.Manager().Queue()
-        pool = ProcessPoolExecutor()
-        futs = [
-            asyncio.get_event_loop().run_in_executor(pool, run_command, cmd.name, cmd.cmd, cmd.setenv, q)
-            for _, cmd in self.cmds.items()
-        ]
-
-        for (_, cmd), fut in zip(self.cmds.items(), futs):
-            cmd.fut = fut
-            cmd.set_running()
-
-        return await self._process_q_async(q, strategy, callbacks)
-
-    def run(self, strategy: ProcessingStrategy, callbacks: CommandCB):
-        q = mp.Manager().Queue()
-        pool = ProcessPoolExecutor()
-        cmd_series = [OrderedDict([(k, v)]) for k, v in self.cmds.items()] if self.serial else [self.cmds]
-        group_exit_code = 0
-
-        for cmd_entries in cmd_series:
-            futs = [pool.submit(run_command, cmd.name, cmd.cmd, cmd.setenv, q) for cmd in cmd_entries.values()]
-            for cmd, fut in zip(cmd_entries.values(), futs):
-                cmd.fut = fut
+    async def run_serial(self, callbacks: CommandCB) -> None:
+        try:
+            for ix in range(len(self.cmds.values())):
+                cmd = list(self.cmds.values())[ix]
                 cmd.set_running()
-            exit_code = self._process_q(cmd_entries, q, strategy, callbacks)
-            if exit_code != 0:
-                group_exit_code = 1
-                if not self.cont_on_fail:
+                async with anyio.create_task_group() as nursery:
+                    nursery.start_soon(self._run_command, cmd, ProcessingStrategy.ON_RECV, callbacks)
+                if cmd.status != CommandStatus.SUCCESS and not self.cont_on_fail:
+                    # Cancel all remaining cmds
+                    for jx in range(ix + 1, len(self.cmds.values())):
+                        cmd = list(self.cmds.values())[jx]
+                        cmd.set_cancelled()
+                    self.update_status(self.cmds)
                     break
-        return group_exit_code
-
-    def _process_q(  # noqa: PLR0912
-        self,
-        cmds: OrderedDict[str, Command],
-        q: Queue,
-        strategy: ProcessingStrategy,
-        callbacks: CommandCB,
-    ) -> int:
-        grp_exit_code = 0
+        except Exception as _:
+            self.status = CommandStatus.FAILURE
+        else:
+            self.update_status(self.cmds)
 
-        if strategy == ProcessingStrategy.ON_RECV:
-            for cmd in cmds.values():
-                callbacks.on_start(cmd)
+    async def run_parallel(self, strategy: ProcessingStrategy, callbacks: CommandCB) -> None:
+        try:
+            async with anyio.create_task_group() as nursery:
+                for cmd in self.cmds.values():
+                    nursery.start_soon(self._run_command, cmd, strategy, callbacks)
+                    cmd.set_running()
+        except Exception as _:
+            self.status = CommandStatus.FAILURE
+        else:
+            self.update_status(self.cmds)
 
-        q_ret = QRetriever(q, self.timeout, self.retries)
-        while True:
-            q_result = q_ret.get()
-
-            # Can only get here with a valid message from the Q
-            cmd_name = q_result[0]
-            exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else None
-            output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str) else None
-            if exit_code is None and output_line is None:
-                raise ValueError("Invalid Q message")  # pragma: no cover
-
-            cmd = self.cmds[cmd_name]
-            if strategy == ProcessingStrategy.ON_RECV:
-                if output_line is not None:
-                    cmd.incr_line_count(output_line)
-                    callbacks.on_recv(cmd, output_line)
-                elif exit_code is not None:
-                    cmd.set_ret_code(exit_code)
-                    callbacks.on_term(cmd, exit_code)
-                    if exit_code != 0:
-                        grp_exit_code = 1
-                else:
-                    raise ValueError("Invalid Q message")  # pragma: no cover
-
-            if strategy == ProcessingStrategy.ON_COMP:
-                if output_line is not None:
-                    cmd.incr_line_count(output_line)
-                    cmd.append_unflushed(output_line)
-                elif exit_code is not None:
-                    callbacks.on_start(cmd)
-                    for line in cmd.unflushed:
-                        callbacks.on_recv(cmd, line)
-                    cmd.clear_unflushed()
-                    callbacks.on_term(cmd, exit_code)
-                    cmd.set_ret_code(exit_code)
-                    if exit_code != 0:
-                        grp_exit_code = 1
-                else:
-                    raise ValueError("Invalid Q message")  # pragma: no cover
-
-            if all(cmd.status.completed() for cmd in cmds.values()):
-                self.update_status(cmds)
-                break
-        return grp_exit_code
-
-    async def _process_q_async(  # noqa: PLR0912
-        self,
-        q: Queue,
-        strategy: ProcessingStrategy,
-        callbacks: CommandAsyncCB,
-    ) -> int:
-        grp_exit_code = 0
+    async def run(self, strategy: ProcessingStrategy, callbacks: CommandCB) -> None:
+        if self.serial:
+            await self.run_serial(callbacks)
+        else:
+            await self.run_parallel(strategy, callbacks)
 
+    async def _proces_stdxx_line(
+        self, cmd: Command, line: str, strategy: ProcessingStrategy, callbacks: CommandCB
+    ) -> None:
         if strategy == ProcessingStrategy.ON_RECV:
-            for cmd in self.cmds.values():
-                await callbacks.on_start(cmd)
-
-        q_ret = QRetriever(q, self.timeout, self.retries)
-        while True:
-            await asyncio.sleep(0)
-            q_result = q_ret.get()
-
-            # Can only get here with a valid message from the Q
-            cmd_name = q_result[0]
-            exit_code: Optional[int] = q_result[1] if isinstance(q_result[1], int) else None
-            output_line: Optional[str] = q_result[1] if isinstance(q_result[1], str) else None
-            if exit_code is None and output_line is None:
-                raise ValueError("Invalid Q message")  # pragma: no cover
-
-            cmd = self.cmds[cmd_name]
-            if strategy == ProcessingStrategy.ON_RECV:
-                if output_line is not None:
-                    cmd.incr_line_count(output_line)
-                    await callbacks.on_recv(cmd, output_line)
-                elif exit_code is not None:
-                    cmd.set_ret_code(exit_code)
-                    await callbacks.on_term(cmd, exit_code)
-                    if exit_code != 0:
-                        grp_exit_code = 1
-                else:
-                    raise ValueError("Invalid Q message")  # pragma: no cover
-
-            if strategy == ProcessingStrategy.ON_COMP:
-                if output_line is not None:
-                    cmd.incr_line_count(output_line)
-                    cmd.append_unflushed(output_line)
-                elif exit_code is not None:
-                    await callbacks.on_start(cmd)
-                    for line in cmd.unflushed:
-                        await callbacks.on_recv(cmd, line)
-                    cmd.clear_unflushed()
-                    await callbacks.on_term(cmd, exit_code)
-                    cmd.set_ret_code(exit_code)
-                    if exit_code != 0:
-                        grp_exit_code = 1
-                else:
-                    raise ValueError("Invalid Q message")  # pragma: no cover
-
-            if all(cmd.status.completed() for _, cmd in self.cmds.items()):
-                break
-        return grp_exit_code
-
-
-def read_commands_ini(filename: Union[str, Path]) -> list[CommandGroup]:
-    """Read a commands.ini file and return a list of CommandGroup objects.
-
-    Args:
-    ----
-        filename (Union[str, Path]): The filename of the commands.ini file.
-
-    Returns:
-    -------
-        list[CommandGroup]: A list of CommandGroup objects.
-
-    """
-    config = configparser.ConfigParser()
-    config.read(filename)
-
-    command_groups = []
-    for section in config.sections():
-        if section.startswith("group."):
-            group_name = section.replace("group.", "")
-            commands = OrderedDict()
-            for name, cmd in config.items(section):
-                clean_name = name.strip()
-                commands[clean_name] = Command(name=clean_name, cmd=cmd.strip())
-            command_group = CommandGroup(name=group_name, cmds=commands)
-            command_groups.append(command_group)
-
-    return command_groups
-
-
-def write_commands_ini(filename: Union[str, Path], command_groups: list[CommandGroup]):
-    """Write a list of CommandGroup objects to a commands.ini file.
-
-    Args:
-    ----
-        filename (Union[str, Path]): The filename of the commands.ini file.
-        command_groups (list[CommandGroup]): A list of CommandGroup objects.
-
-    """
-    config = configparser.ConfigParser()
-
-    for group in command_groups:
-        section_name = f"group.{group.name}"
-        config[section_name] = {}
-        for command in group.cmds.values():
-            config[section_name][command.name] = command.cmd
-
-    with Path(filename).open("w", encoding="utf-8") as configfile:
-        config.write(configfile)
+            await callbacks.on_recv(cmd, line)
+        elif strategy == ProcessingStrategy.ON_COMP:
+            cmd.append_unflushed(line)
+        cmd.incr_line_count(line)
+
+    async def _process_stdxxx(
+        self, cmd: Command, strategy: ProcessingStrategy, stream: AsyncIterable[bytes], callbacks: CommandCB
+    ) -> None:
+        await callbacks.on_start(cmd)
+
+        incomplete_line = ""
+
+        async for chunk in stream:
+            # Decode the bytes to a string
+            decoded_chunk = chunk.decode("utf-8")
+            # Combine the remainder of the last chunk with the new chunk
+            lines = (incomplete_line + decoded_chunk).split("\n")
+
+            # The last line might be incomplete; hold it back
+            incomplete_line = lines.pop() if lines[-1] else ""
+
+            for line in lines:
+                await self._proces_stdxx_line(cmd, line, strategy, callbacks)
+
+        if incomplete_line:
+            await self._proces_stdxx_line(cmd, incomplete_line, strategy, callbacks)  # pragma: no cover
+
+        if strategy == ProcessingStrategy.ON_COMP:
+            for _ix, line in enumerate(cmd.unflushed):
+                await callbacks.on_recv(cmd, line)
+            cmd.clear_unflushed()
+
+    async def _run_command(self, cmd: Command, strategy: ProcessingStrategy, callbacks: CommandCB) -> int:
+        env = os.environ.copy()
+        if cmd.setenv:
+            env.update(cmd.setenv)
+
+        # Running the command asynchronously and capturing the output
+        try:
+            with anyio.fail_after(self.timeout):
+                async with (
+                    await anyio.open_process(
+                        command=cmd.cmd, env=env, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
+                    ) as process,
+                    anyio.create_task_group() as tg,
+                ):
+                    if process.stdout:
+                        tg.start_soon(self._process_stdxxx, cmd, strategy, process.stdout, callbacks)
+                    await process.wait()
+        except TimeoutError:
+            cmd.set_timeout()
+            await callbacks.on_term(cmd, internal_error_ret_code)
+            return internal_error_ret_code
+        else:
+            exit_code = cast(int, process.returncode)
+            cmd.set_ret_code(exit_code)
+            await callbacks.on_term(cmd, exit_code)
+            return exit_code
 
 
 def _validate_mandatory_keys(data: tomlkit.items.Table, keys: list[str], context: str) -> tuple[Any, ...]:
     """Validate that the mandatory keys are present in the data.
 
     Args:
     ----
@@ -361,15 +234,15 @@
         val = data.get(key, None)
         if not val:
             raise ValueError(f"{key} is mandatory, not found in {context}")
         vals.append(val)
     return tuple(vals)
 
 
-def _get_optional_keys(data: tomlkit.items.Table, keys: list[str], default=None) -> tuple[Optional[Any], ...]:
+def _get_optional_keys(data: tomlkit.items.Table, keys: list[str], default: Any = None) -> tuple[Optional[Any], ...]:  # noqa: ANN001, ANN401
     """Get Optional keys or default.
 
     Args:
     ----
         data (tomlkit.items.Table): The data to use as source
         keys (list[str]): The optional keys.
 
@@ -389,83 +262,50 @@
     -------
         list[CommandGroup]: A list of CommandGroup objects.
 
     """
     with Path(filename).open(encoding="utf-8") as toml_file:
         toml_data = tomlkit.parse(toml_file.read())
 
-    cmd_groups_data = toml_data.get("tool", {}).get("par-run", {})
+    if (isinstance(filename, Path) and filename.name == "pyproject.toml") or (
+        isinstance(filename, str) and filename == "pyproject.toml"
+    ):
+        cmd_groups_data = toml_data.get("tool", {}).get("par-run", {})
+    else:
+        cmd_groups_data = toml_data.get("par-run", None)
+
     if not cmd_groups_data:
-        raise ValueError("No par-run data found in toml file")
+        raise ValueError(f"No par-run data found in toml file {filename}")
     _ = cmd_groups_data.get("description", None)
 
     command_groups = []
     for group_data in cmd_groups_data.get("groups", []):
         (group_name,) = _validate_mandatory_keys(group_data, ["name"], "top level par-run group")
-        group_desc, group_timeout, group_retries = _get_optional_keys(
+        group_desc, group_timeout = _get_optional_keys(
             group_data,
-            ["desc", "timeout", "retries"],
+            ["desc", "timeout"],
             default=None,
         )
         (group_cont_on_fail, group_serial) = _get_optional_keys(group_data, ["cont_on_fail", "serial"], default=False)
 
         if not group_timeout:
             group_timeout = 30
-        if not group_retries:
-            group_retries = 3
         group_cont_on_fail = bool(group_cont_on_fail and group_cont_on_fail is True)
         group_serial = bool(group_serial and group_serial is True)
 
         commands = OrderedDict()
         for cmd_data in group_data.get("commands", []):
             name, exec = _validate_mandatory_keys(cmd_data, ["name", "exec"], f"command group {group_name}")
             setenv, passenv = _get_optional_keys(cmd_data, ["setenv", "passenv"], default=None)
 
             commands[name] = Command(name=name, cmd=exec, setenv=setenv, passenv=passenv)
         command_group = CommandGroup(
             name=group_name,
             desc=group_desc,
             cmds=commands,
             timeout=group_timeout,
-            retries=group_retries,
             cont_on_fail=group_cont_on_fail,
             serial=group_serial,
         )
         command_groups.append(command_group)
 
     return command_groups
-
-
-def run_command(name: str, command: str, setenv: Optional[dict[str, str]], q: Queue) -> None:
-    """Run a command and put the output into a queue. The output is a tuple of the command
-    name and the output line. The final output is a tuple of the command name and a dictionary
-    with the return code.
-
-    Args:
-    ----
-        name (Command): Command to run.
-        q (Queue): Queue to put the output into.
-
-    """
-    new_env = None
-    if setenv:
-        new_env = os.environ.copy()
-        new_env.update(setenv)
-
-    with subprocess.Popen(
-        command,
-        shell=True,
-        env=new_env,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.STDOUT,
-        text=True,
-    ) as process:
-        if process.stdout:
-            for line in iter(process.stdout.readline, ""):
-                q.put((name, line.strip()))
-            process.stdout.close()
-            process.wait()
-            ret_code = process.returncode
-            if ret_code is not None:
-                q.put((name, int(ret_code)))
-            else:
-                raise ValueError("Process has no return code")  # pragma: no cover
```

### Comparing `par_run-0.3.0/src/par_run/web.py` & `par_run-0.5.0/src/par_run/web.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 """Web UI Module"""
 
 from pathlib import Path
 
 import rich
-from fastapi import Body, FastAPI, Request, WebSocket
+from fastapi import FastAPI, Request, WebSocket
+from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 
-from .executor import Command, ProcessingStrategy, read_commands_ini, write_commands_ini
+from .executor import Command, CommandGroup, CommandStatus, ProcessingStrategy, read_commands_toml
 
 BASE_PATH = Path(__file__).resolve().parent
 
 ws_app = FastAPI()
 ws_app.mount("/static", StaticFiles(directory=str(BASE_PATH / "static")), name="static")
 templates = Jinja2Templates(directory=str(BASE_PATH / "templates"))
 
 
 @ws_app.get("/")
-async def ws_main(request: Request):
+async def ws_main(request: Request) -> HTMLResponse:
     """Get the main page."""
     return templates.TemplateResponse("index.html", {"request": request})
 
 
 @ws_app.get("/get-commands-config")
-async def get_commands_config():
+async def get_commands_config() -> list[CommandGroup]:
     """Get the commands configuration."""
-    return read_commands_ini("commands.ini")
-
-
-@ws_app.post("/update-commands-config")
-async def update_commands_config(updated_config=Body(...)):  # noqa: B008
-    """Update the commands configuration."""
-    write_commands_ini("commands.ini", updated_config)
-    return {"message": "Configuration updated successfully"}
+    return read_commands_toml("commands.toml")
 
 
 class WebCommandCB:
     """Websocket command callbacks."""
 
-    def __init__(self, ws: WebSocket):
+    def __init__(self, ws: WebSocket) -> None:
         self.ws = ws
 
-    async def on_start(self, cmd: Command):
+    async def on_start(self, cmd: Command) -> None:
         rich.print(f"[blue bold]Started command {cmd.name}[/]")
 
-    async def on_recv(self, cmd: Command, output: str):
+    async def on_recv(self, cmd: Command, output: str) -> None:
         await self.ws.send_json({"commandName": cmd.name, "output": output})
 
-    async def on_term(self, cmd: Command, exit_code: int):
+    async def on_term(self, cmd: Command, exit_code: int) -> None:
+        if cmd.status == CommandStatus.SUCCESS:
+            rich.print(f"[green bold]Command {cmd.name} finished[/]")
+        elif cmd.status == CommandStatus.FAILURE:
+            rich.print(f"[red bold]Command {cmd.name} failed, {exit_code=:}[/]")
         await self.ws.send_json({"commandName": cmd.name, "output": {"ret_code": exit_code}})
 
 
 @ws_app.websocket_route("/ws")
-async def websocket_endpoint(websocket: WebSocket):
+async def websocket_endpoint(websocket: WebSocket) -> None:
     """Websocket endpoint to run commands."""
     rich.print("Websocket connection")
-    master_groups = read_commands_ini("commands.ini")
+    master_groups = read_commands_toml("commands.toml")
     await websocket.accept()
+    rich.print("Websocket accepted")
     cb = WebCommandCB(websocket)
-    exit_code = 0
+    rich.print("Websocket command cb created")
     for grp in master_groups:
-        exit_code = exit_code or await grp.run_async(ProcessingStrategy.ON_RECV, cb)
+        await grp.run(ProcessingStrategy.ON_RECV, cb)
+        if grp.status != CommandStatus.SUCCESS and not grp.cont_on_fail:
+            break
```

### Comparing `par_run-0.3.0/src/par_run/static/css/style.css` & `par_run-0.5.0/src/par_run/static/css/style.css`

 * *Files identical despite different names*

### Comparing `par_run-0.3.0/src/par_run/static/js/app.js` & `par_run-0.5.0/src/par_run/static/js/app.js`

 * *Files identical despite different names*

### Comparing `par_run-0.3.0/src/par_run/templates/index.html` & `par_run-0.5.0/src/par_run/templates/index.html`

 * *Files identical despite different names*

### Comparing `par_run-0.3.0/.gitignore` & `par_run-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `par_run-0.3.0/LICENSE` & `par_run-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `par_run-0.3.0/README.md` & `par_run-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `par_run-0.3.0/pyproject.toml` & `par_run-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "par-run"
-version = "0.3.0"
+version = "0.5.0"
 description = "Parallel command runner"
 license = "MIT"
 authors = [
     { name = "Naz Quadri", email = "naz.quadri@gmail.com" }
 ]
 classifiers = [
     'Development Status :: 4 - Beta',
@@ -18,14 +18,16 @@
     'Programming Language :: Python :: 3.12',
 ]
 dependencies = [
     "pydantic>=2.0.0",
     "tomlkit>=0.12.4",
     "typer>=0.9.0",
     "rich>=13.0.0",
+    "exceptiongroup>=1.2.1",
+    "anyio[trio]>=4.3.0",
 ]
 readme = "README.md"
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://github.com/nazq/par-run"
 Documentation = "https://github.com/nazq/par-run"
@@ -35,55 +37,62 @@
 
 [project.optional-dependencies]
 web = [
     "fastapi>=0.100.0",
     "uvicorn[standard]>=0.29.0",
     "jinja2>=3.0.0",
     "psutil>=5.9.0",
+    # "hypercorn[trio]",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "bump-my-version>=0.19.3",
     "httpx>=0.27.0",
     "ipython>=8.18.1",
     "mypy>=1.9.0",
     "pytest>=8.1.1",
-    "pytest-asyncio>=0.23.6",
     "pytest-benchmark>=4.0.0",
     "pytest-cov>=5.0.0",
     "pytest-mock>=3.14.0",
     "pytest-random-order>=1.1.1",
+    "pytest-xdist>=3.5.0",
     "ruff>=0.3.4",
     "twine>=5.0.0",
     "types-toml>=0.10.8.20240310",
     "types-psutil>=5.9.5.20240316",
+    "types-requests>=2.31.0.20240406",
 ]
 
 [project.scripts]
 "par-run" = "par_run.cli:cli_app"
 
+[tool.mypy]
+ignore_missing_imports = true
+show_error_codes = true
+strict = true
+disallow_untyped_defs = true
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = [
     "src/par_run",
     "static",
     "templates",
 ]
 
 [tool.bumpversion]
-current_version = "0.3.0"
+current_version = "0.5.0"
 commit = true
 tag = true
 tag_name = "{new_version}"
 tag_message = "Version {new_version}"
 message = "Bump version: {current_version} → {new_version}"
 allow_dirty = true
 parse = """(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"""
@@ -111,41 +120,42 @@
     'F',
     'PTH',
     'PIE',
     'TID',
     'ERA',
     'ARG',
     'PL',
-    #'ANN',
+    'ANN',
     'SIM',
     'PERF',
     'T20',
 ]
-extend-ignore = ["S101", "FA100"]
+extend-ignore = ["S101", "FA100", "ANN101"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["par_run"]
 
 
 [tool.pytest.ini_options]
-addopts = "--cov src --cov-report html:.reports/html --cov-report term --random-order -p no:warnings -v"
+#addopts = "--cov src --cov-report html:.reports/html --cov-report term --random-order -p no:warnings -v -n auto"
+addopts = "--cov src --cov-report html:.reports/html --cov-report term -p no:warnings -v"
 minversion = "8.0"
 pythonpath = ["src", "py_tests"]
 testpaths = "py_tests"
 pythonfiles = "test_*.py"
+trio_mode = true
 
 
 [tool.par-run]
 desc = "par-run from pyproject.toml"
 
 [[tool.par-run.groups]]
 name = "Formatting"
 desc = "Code formatting commands."
 timeout = 5
-retries = 3 
 cont_on_fail = true # default is false
 serial = false # default is false
 
   [[tool.par-run.groups.commands]]
   name = "ruff_fmt"
   exec = "ruff format src py_tests"
   # Define an empty extras using standard table notation, or simply omit it if it's always empty
@@ -155,16 +165,15 @@
   exec = "ruff check --fix src py_tests"
   # Define an empty extras using standard table notation, or simply omit it if it's always empty
 
 
 [[tool.par-run.groups]]
 name = "Quality"
 desc = "Code Quality Tools. No code mutation"
-timeout = 5
-retries = 3
+timeout = 30
 cont_on_fail = true # default is false
 
   [[tool.par-run.groups.commands]]
   name = "ruff_lint"
   exec = "ruff check src py_tests"
   # extras omitted as it's empty
 
@@ -173,43 +182,7 @@
   exec = "mypy src"
   setenv = {NODE_ENV = "production", ENABLE_LOGS = "true"}
 
   [[tool.par-run.groups.commands]]
   name = "pytest"
   exec = "pytest py_tests"
   setenv = {NODE_ENV = "production", ENABLE_LOGS = "true"}
-
-
-[[tool.par-run.groups]]
-name = "ENV"
-desc = "Code Quality Tools. No code mutation"
-timeout = 5
-retries = 3
-cont_on_fail = true # default is false
-
-
-  [[tool.par-run.groups.commands]]
-  name = "full_env"
-  exec = "env"
-  setenv = {MY_VAR = "production", ENABLE_LOGS = "true"}
-
-  [[tool.par-run.groups.commands]]
-  name = "my_var"
-  exec = "echo \"MY_VAR=$MY_VAR\", \"ENABLE_LOGS=$ENABLE_LOGS\""
-  setenv = {MY_VAR = "production", ENABLE_LOGS = "true"}
-
-
-[[tool.par-run.groups]]
-name = "Serial"
-desc = "Must run serially"
-timeout = 5
-retries = 3
-cont_on_fail = true # default is false
-serial = true
-
-  [[tool.par-run.groups.commands]]
-  name = "sleep then create file"
-  exec = "sleep 2 && touch /tmp/test.pr"
-
-  [[tool.par-run.groups.commands]]
-  name = "try delete file"
-  exec = "rm /tmp/test.pr"
```

### Comparing `par_run-0.3.0/PKG-INFO` & `par_run-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: par-run
-Version: 0.3.0
+Version: 0.5.0
 Summary: Parallel command runner
 Project-URL: Homepage, https://github.com/nazq/par-run
 Project-URL: Documentation, https://github.com/nazq/par-run
 Project-URL: Repository, https://github.com/nazq/par-run
 Project-URL: Issues, https://github.com/nazq/par-run/issues
 Project-URL: Changelog, https://github.com/nazq/par-run
 Author-email: Naz Quadri <naz.quadri@gmail.com>
@@ -16,14 +16,16 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
+Requires-Dist: anyio[trio]>=4.3.0
+Requires-Dist: exceptiongroup>=1.2.1
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: rich>=13.0.0
 Requires-Dist: tomlkit>=0.12.4
 Requires-Dist: typer>=0.9.0
 Provides-Extra: web
 Requires-Dist: fastapi>=0.100.0; extra == 'web'
 Requires-Dist: jinja2>=3.0.0; extra == 'web'
```

