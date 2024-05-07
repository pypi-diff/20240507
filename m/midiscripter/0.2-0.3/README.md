# Comparing `tmp/midiscripter-0.2.tar.gz` & `tmp/midiscripter-0.3.tar.gz`

## Comparing `midiscripter-0.2.tar` & `midiscripter-0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/base/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/base/msg_base.py
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/base/port_base.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/base/shared.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/cli/__init__.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/cli/starters.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/file_event/__init__.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/file_event/file_event_msg.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/file_event/file_event_port.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/__init__.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/app.py
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/log_widget.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/main_window.py
--rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/menu_bar.py
--rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/ports_widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/gui_widgets/__init__.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/gui_widgets/button.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/gui_widgets/gui_msg.py
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/gui_widgets/gui_widget_base.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/gui_widgets/layout.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/gui_widgets/list.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/gui_widgets/mixins.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/gui/gui_widgets/text.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/keyboard/__init__.py
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/keyboard/keyboard_msg.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/keyboard/keyboard_port.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/logger/__init__.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/logger/console_sink.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/logger/html_sink.py
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/logger/log.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/metronome/__init__.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/metronome/metronome_port.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/midi/__init__.py
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/midi/midi_msg.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/midi/midi_note_data.py
--rw-r--r--   0        0        0     6776 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/midi/midi_port.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/midi/midi_ports_update.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/osc/__init__.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/osc/osc_msg.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/osc/osc_port.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/osc/osc_query_maker.py
--rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/resources/icon.ico
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 midiscripter-0.2/midiscripter/resources/icon.svg
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 midiscripter-0.2/LICENSE
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 midiscripter-0.2/README.md
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 midiscripter-0.2/pyproject.toml
--rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 midiscripter-0.2/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/base/__init__.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/base/msg_base.py
+-rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/base/port_base.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/base/shared.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/cli/__init__.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/cli/starters.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/file_event/__init__.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/file_event/file_event_msg.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/file_event/file_event_port.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/__init__.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/app.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/log_widget.py
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/main_window.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/menu_bar.py
+-rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/ports_widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/__init__.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/button.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/gui_msg.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/gui_widget_base.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/layout.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/list.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/mixins.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/gui/gui_widgets/text.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/keyboard/__init__.py
+-rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/keyboard/keyboard_msg.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/keyboard/keyboard_port.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/logger/__init__.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/logger/console_sink.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/logger/html_sink.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/logger/log.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/metronome/__init__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/metronome/metronome_port.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/midi/__init__.py
+-rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/midi/midi_msg.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/midi/midi_note_data.py
+-rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/midi/midi_port.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/midi/midi_ports_update.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/osc/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/osc/osc_msg.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/osc/osc_port.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/osc/osc_query_maker.py
+-rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/resources/icon.ico
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 midiscripter-0.3/midiscripter/resources/icon.svg
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 midiscripter-0.3/LICENSE
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 midiscripter-0.3/README.md
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 midiscripter-0.3/pyproject.toml
+-rw-r--r--   0        0        0    14416 2020-02-02 00:00:00.000000 midiscripter-0.3/PKG-INFO
```

### Comparing `midiscripter-0.2/midiscripter/base/msg_base.py` & `midiscripter-0.3/midiscripter/base/msg_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import enum
-from typing import Optional
 from collections.abc import Container
 
 import midiscripter.base.shared
 from midiscripter.base.port_base import Input
 
 
 class AttrEnum(enum.StrEnum):
```

### Comparing `midiscripter-0.2/midiscripter/base/port_base.py` & `midiscripter-0.3/midiscripter/base/port_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import collections
 import contextlib
 import copy
 import traceback
-from typing import TYPE_CHECKING, TypeVar
 from collections.abc import Callable, Hashable
+from typing import TYPE_CHECKING, TypeVar
 
 import midiscripter.base.shared
 from midiscripter.logger import log
 
 if TYPE_CHECKING:
     from midiscripter.base.msg_base import Msg
 
 
 @contextlib.contextmanager
-def _all_opened():
+def _all_opened() -> None:
     for port in _PortRegistryMeta.instance_registry.values():
         port._open()
 
     for call in midiscripter.base.shared.run_after_ports_open_subscribed_calls:
 
-        def __call_runner():
+        def __call_runner() -> None:
             try:
                 log('Running {call}', call=call)  # noqa: B023
                 call()  # noqa: B023
             except Exception as exc:
                 log.red(''.join(traceback.format_exception(exc)))
 
         midiscripter.base.shared.thread_executor.submit(__call_runner)
@@ -225,25 +225,29 @@
 
     def send(self, msg: 'Msg') -> None:
         """Send message using the output port.
 
         Args:
             msg: Message to send.
         """
-        with self._check_and_log_sent_message(msg):
-            raise NotImplementedError
+        if not self._validate_msg_send(msg):
+            return
+
+        raise NotImplementedError
 
-    @contextlib.contextmanager
-    def _check_and_log_sent_message(self, msg: 'Msg'):
+        # noinspection PyUnreachableCode
+        self._log_msg_sent(msg)
+
+    def _validate_msg_send(self, msg: 'Msg') -> bool:
         if not self.is_enabled:
             log.red("Can't send message {msg}. {output} is disabled!", msg=msg, output=self)
-            return
-
-        yield
+            return False
+        return True
 
+    def _log_msg_sent(self, msg: 'Msg') -> None:
         if msg.source:
             log(
                 '{output} sent message {msg} received {age_ms} ms ago',
                 output=self,
                 msg=msg,
                 age_ms=msg._age_ms,
             )
```

### Comparing `midiscripter-0.2/midiscripter/cli/starters.py` & `midiscripter-0.3/midiscripter/cli/starters.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     """Starts the script without logging. The fastest way to run the script."""
     log.is_enabled = False
     _run_cli_loop()
 
 
 def _run_cli_loop() -> NoReturn:
     """Opens the ports and loops until broken by user."""
+    if not midiscripter.base.shared.script_path:
+        raise RuntimeError('Starter can only be called from a script')
+
     midiscripter.base.shared._raise_current_process_cpu_priority()
     with midiscripter.base.port_base._all_opened():
         while True:
             try:
                 time.sleep(1)
             except (KeyboardInterrupt, SystemExit):
                 break
```

### Comparing `midiscripter-0.2/midiscripter/file_event/file_event_msg.py` & `midiscripter-0.3/midiscripter/file_event/file_event_msg.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pathlib
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING
 
 import midiscripter.base.msg_base
 
 if TYPE_CHECKING:
+    from collections.abc import Container
     from midiscripter.file_event.file_event_port import FileEventIn
 
 
 class FileEventType(midiscripter.base.msg_base.AttrEnum):
     # Names are hardcoded, equal watchdog's event types
     MOVED = 'MOVED'
     DELETED = 'DELETED'
@@ -22,28 +23,33 @@
 
     type: FileEventType
     """File event type"""
 
     path: pathlib.Path
     """File path of event"""
 
-    source: Optional['FileEventIn']
+    source: 'None | FileEventIn'
 
     def __init__(
         self,
         type: FileEventType | str,
         path: pathlib.Path,
         *,
-        source: Optional['FileEventIn'] = None,
+        source: 'None | FileEventIn' = None,
     ):
         """
         Args:
             type: File event type
             path: File path
-            source (FileEventIn): The [`FileEventIn`][midiscripter.FileEventIn] instance that generated the message
+            source (FileEventIn): The [`FileEventIn`][midiscripter.FileEventIn]
+                                  instance that generated the message
         """
         super().__init__(type, source)
         self.type = type
         self.path = path
 
-    def matches(self, type=None, path=None):
+    def matches(
+        self,
+        type: 'None | Container[FileEventType] | FileEventType | str' = None,
+        path: 'None | Container[pathlib.Path] | pathlib.Path' = None,
+    ) -> bool:
         return super().matches(type, path)
```

### Comparing `midiscripter-0.2/midiscripter/file_event/file_event_port.py` & `midiscripter-0.3/midiscripter/file_event/file_event_port.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pathlib
-from typing import Union
 
 import watchdog.events
 import watchdog.observers
 
 import midiscripter.base.port_base
 import midiscripter.file_event
 import midiscripter.logger
```

### Comparing `midiscripter-0.2/midiscripter/gui/app.py` & `midiscripter-0.3/midiscripter/gui/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,31 +21,35 @@
 
     RESTART_DELAY = 2
     widgets_to_add = []
 
     def __init__(self):
         super().__init__()
         self.setOrganizationName('MIDI Scripter')
-        self.setApplicationName(pathlib.Path(midiscripter.base.shared.script_path).name)
+        if midiscripter.base.shared.script_path:
+            self.setApplicationName(pathlib.Path(midiscripter.base.shared.script_path).name)
+
         icon_path = pathlib.Path(midiscripter.__file__).parent / 'resources' / 'icon.ico'
         self.setWindowIcon(QIcon(str(icon_path)))
 
         self.__time_until_restart_sec = self.RESTART_DELAY
         self.request_restart.connect(self, self.restart)
         self.aboutToQuit.connect(self.__cleanup)
 
-    def prepare_main_window(self, minimized_to_tray: bool = False):
+    def prepare_main_window(self, minimized_to_tray: bool = False) -> None:
         self.main_window = midiscripter.gui.main_window.MainWindow(self.widgets_to_add)
 
         if not minimized_to_tray:
             self.main_window.show_from_tray()
         else:
             self.main_window.close()
 
-    def restart_at_file_change(self, msg: 'midiscripter.file_event.file_change_msg.FileEventMsg'):
+    def restart_at_file_change(
+        self, msg: 'midiscripter.file_event.file_change_msg.FileEventMsg'
+    ) -> None:
         if msg.type not in (
             midiscripter.file_event.file_event_msg.FileEventType.CREATED,
             midiscripter.file_event.file_event_msg.FileEventType.MODIFIED,
         ):
             return
 
         self.__time_until_restart_sec = self.RESTART_DELAY
@@ -53,46 +57,49 @@
 
         while self.__time_until_restart_sec > 0:
             time.sleep(sleep_step_sec)
             self.__time_until_restart_sec -= sleep_step_sec
 
         self.request_restart.emit()
 
-    def restart(self):
+    def restart(self) -> NoReturn:
         if pathlib.Path(midiscripter.base.shared.script_path).is_file():
             # These settings saved only for restart
             self.processEvents()  # update win status to get correct status
-            QSettings().setValue('restart win minimized', int(self.main_window.isMinimized()))
-            QSettings().setValue('restart closed to tray', int(not self.main_window.isVisible()))
+            QSettings().setValue('restart win minimized', self.main_window.isMinimized())
+            QSettings().setValue('restart closed to tray', not self.main_window.isVisible())
             self.exit(1467)
 
-    def __cleanup(self):
+    def __cleanup(self) -> None:
         self.main_window.close()
         self.main_window.tray.hide()
 
 
 # Creating app at import to allow QWidget instance init in other modules
 app_instance = ScripterGUI()
 
 
-def add_qwidget(qwidget: QWidget):
+def add_qwidget(qwidget: QWidget) -> None:
     """Add custom pyside6 QWidget to the GUI"""
     if qwidget not in midiscripter.gui.app.ScripterGUI.widgets_to_add:
         midiscripter.gui.app.ScripterGUI.widgets_to_add.append(qwidget)
 
 
-def remove_qwidget(qwidget: QWidget):
+def remove_qwidget(qwidget: QWidget) -> None:
     """Remove custom pyside6 QWidget to the GUI"""
     try:
         midiscripter.gui.app.ScripterGUI.widgets_to_add.remove(qwidget)
     except ValueError:
         pass
 
 
 def start_gui() -> NoReturn:
+    if not midiscripter.base.shared.script_path:
+        raise RuntimeError('Starter can only be called from a script')
+
     """Starts the script and runs GUI. Logging goes to GUI Log widget."""
     midiscripter.base.shared._raise_current_process_cpu_priority()
 
     sigint_exit_code = {'Windows': -1073741510, 'Linux': 130, 'Darwin': 2}[platform.system()]
     signal.signal(signal.SIGINT, lambda *_: app_instance.exit(sigint_exit_code))
 
     signal_checker_dummy_timer = QTimer()  # runs python code from Qt to allow the signal to trigger
```

### Comparing `midiscripter-0.2/midiscripter/gui/log_widget.py` & `midiscripter-0.3/midiscripter/gui/log_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from PySide6.QtCore import *
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
 import midiscripter.logger.html_sink
 from midiscripter.logger import log
 
@@ -45,25 +43,25 @@
         self.setMaximumBlockCount(log.BUFFER_SIZE)
         self.setMouseTracking(True)
 
         self.append_html_entry.connect(self.__add_entry)
         log._sink = midiscripter.logger.html_sink.HtmlSink(self.append_html_entry.emit)
 
     @Slot(str)
-    def set_filter(self, filter_text: str):
+    def set_filter(self, filter_text: str) -> None:
         self.__filter_words = filter_text.split()
         self.__apply_filter()
 
-    def __apply_filter(self, to_last_n_blocks: int = 0):
+    def __apply_filter(self, to_last_n_blocks: int = 0) -> None:
         self.__hide_lines_not_matching_filter(to_last_n_blocks)
         if not to_last_n_blocks:
             self.__clear_highlighting()
         self.__highlight_filter_matches(to_last_n_blocks)
 
-    def __hide_lines_not_matching_filter(self, last_n_blocks: int = 0):
+    def __hide_lines_not_matching_filter(self, last_n_blocks: int = 0) -> None:
         document = self.document()
 
         start_from = 0 if not last_n_blocks else document.blockCount() - last_n_blocks
 
         for line_n in range(start_from, document.blockCount()):
             block = document.findBlockByNumber(line_n)
 
@@ -77,23 +75,23 @@
             ):
                 block.setVisible(False)
             else:
                 block.setVisible(True)
 
         self.setDocument(document)
 
-    def __clear_highlighting(self):
+    def __clear_highlighting(self) -> None:
         text_format = QTextCharFormat()
         text_format.setBackground(QBrush(Qt.NoBrush))
 
         cursor = self.textCursor()
         cursor.select(QTextCursor.SelectionType.Document)
         cursor.mergeCharFormat(text_format)
 
-    def __highlight_filter_matches(self, last_n_blocks: int = 0):
+    def __highlight_filter_matches(self, last_n_blocks: int = 0) -> None:
         if not self.__filter_words:
             return
 
         cursor = self.textCursor()
 
         text_format = QTextCharFormat()
         text_format.setBackground(QBrush(QColor('yellow')))
@@ -116,39 +114,39 @@
                     QTextCursor.MoveOperation.NextCharacter,
                     QTextCursor.MoveMode.KeepAnchor,
                     match.capturedLength(),
                 )
                 cursor.mergeCharFormat(text_format)
 
     @Slot(list)
-    def __add_entry(self, log_entries: list[str]):
+    def __add_entry(self, log_entries: list[str]) -> None:
         [self.appendHtml(f'<div>{entry}</div>') for entry in log_entries]
         self.verticalScrollBar().setValue(self.verticalScrollBar().maximum())
 
         if self.__filter_words:
             self.__apply_filter(len(log_entries))
 
-    def showEvent(self, event: QShowEvent):
+    def showEvent(self, event: QShowEvent) -> None:
         log.flushing_is_enabled = True
         log._flush()
         super().showEvent(event)
 
-    def hideEvent(self, event: QHideEvent):
+    def hideEvent(self, event: QHideEvent) -> None:
         log.flushing_is_enabled = False
         super().hideEvent(event)
 
-    def mouseMoveEvent(self, event: QMouseEvent):
+    def mouseMoveEvent(self, event: QMouseEvent) -> None:
         self.__anchor_text = self.anchorAt(event.pos())
         if self.__anchor_text:
             self.viewport().setCursor(Qt.PointingHandCursor)
         else:
             self.viewport().setCursor(Qt.IBeamCursor)
         super().mouseMoveEvent(event)
 
-    def mouseReleaseEvent(self, event: QMouseEvent):
+    def mouseReleaseEvent(self, event: QMouseEvent) -> None:
         if event.button() == Qt.LeftButton and self.__anchor_text:
             QGuiApplication.clipboard().setText(self.__anchor_text)
             QToolTip().showText(
                 event.globalPosition().toPoint(),
                 f'Copied {self.__anchor_text}',
                 self,
                 msecShowTime=2000,
```

### Comparing `midiscripter-0.2/midiscripter/gui/main_window.py` & `midiscripter-0.3/midiscripter/gui/main_window.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import midiscripter.base.shared
 import midiscripter.gui.log_widget
 import midiscripter.gui.menu_bar
 import midiscripter.gui.ports_widget
 
 
 class TrayIcon(QSystemTrayIcon):
-    def __init__(self, icon, parent: 'MainWindow' = None):
+    def __init__(self, icon: QIcon, parent: 'MainWindow' = None):
         super().__init__(icon, parent)
         self.setToolTip(QApplication.instance().applicationName())
         self.activated.connect(self.__activated)
 
         menu = QMenu(parent)
         menu.setDefaultAction(menu.addAction('Open GUI', parent.showNormal))
         self.restart_act = menu.addAction('Restart script', QApplication.instance().restart)
         menu.addAction('Quit', QApplication.instance().exit)
         self.setContextMenu(menu)
 
-    def __activated(self, reason: QSystemTrayIcon.ActivationReason):
+    def __activated(self, reason: QSystemTrayIcon.ActivationReason) -> None:
         if reason == QSystemTrayIcon.ActivationReason.Trigger:
             if self.parent().isVisible():
                 self.parent().close()
             else:
                 self.parent().show_from_tray()
 
         if reason == QSystemTrayIcon.ActivationReason.MiddleClick:
@@ -54,68 +54,68 @@
 
         self.menu_bar = midiscripter.gui.menu_bar.MenuBar(self)
         self.setMenuBar(self.menu_bar)
 
         self.tray = TrayIcon(self.windowIcon(), self)
         self.tray.show()
 
-    def add_widget_as_dock(self, widget: QWidget):
+    def add_widget_as_dock(self, widget: QWidget) -> None:
         dock = QDockWidget(self)
         dock.setObjectName(widget.objectName())
         dock.setWindowTitle(widget.objectName())
         dock.setWidget(widget)
 
         self.addDockWidget(Qt.DockWidgetArea.TopDockWidgetArea, dock)
         self.dock_widgets.append(dock)
 
-    def set_dock_titles_visibility(self, are_hidden: bool):
+    def set_dock_titles_visibility(self, are_hidden: bool) -> None:
         # Can't make full lock with setFixedSize due to AdaptiveTextSizeWidgets
         # that has "Ignore" size policy and always restore at maximum size after that
         for dock in self.dock_widgets:
             if are_hidden:
                 dock.setTitleBarWidget(QWidget())
             else:
                 dock.setTitleBarWidget(None)
 
-    def show_from_tray(self):
+    def show_from_tray(self) -> None:
         self.setWindowState(self.windowState() & ~Qt.WindowMinimized | Qt.WindowActive)
         self.resize(QSettings().value('win size', QSize(800, 500)))
         self.move(QSettings().value('win position', self.__get_screen_center()))
         self.restoreState(QSettings().value('win state'))
 
-        if QSettings().value('restart win minimized', False):
+        if QSettings().value('restart win minimized', False, type=bool):
             self.showMinimized()
             # 'win minimized' set by restart request, cleared for the next normal start
-            QSettings().setValue('restart win minimized', 0)
-        elif QSettings().value('win maximized', False):
+            QSettings().setValue('restart win minimized', False)
+        elif QSettings().value('win maximized', False, type=bool):
             self.showMaximized()
         else:
             self.show()
 
         # Somewhere in window preparation the window size changes, second resize makes it stick.
         self.resize(QSettings().value('win size', QSize(800, 500)))
         self.move(QSettings().value('win position', self.__get_screen_center()))
 
         # 'win visible' set by restart request, cleared for the next normal start
-        if QSettings().value('restart closed to tray', False):
-            QSettings().setValue('restart closed to tray', 0)
+        if QSettings().value('restart closed to tray', False, type=bool):
+            QSettings().setValue('restart closed to tray', False)
             self.close()
 
-    def closeEvent(self, event: QCloseEvent):
+    def closeEvent(self, event: QCloseEvent) -> None:
         event.ignore()
         QSettings().setValue('win state', self.saveState())
-        QSettings().setValue('win maximized', int(self.isMaximized()))
+        QSettings().setValue('win maximized', self.isMaximized())
 
         if not self.isMaximized():
             QSettings().setValue('win size', self.size())
             QSettings().setValue('win position', self.pos())
 
         self.hide()
 
-    def set_always_on_top(self, state: bool):
+    def set_always_on_top(self, state: bool) -> None:
         if state:
             self.setWindowFlags(self.__always_on_top_flags)
         else:
             self.setWindowFlags(self.__normal_flags)
         self.show()
 
     def __get_screen_center(self) -> QPoint:
```

### Comparing `midiscripter-0.2/midiscripter/gui/menu_bar.py` & `midiscripter-0.3/midiscripter/gui/menu_bar.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import pathlib
-import platform
-import sys
-from typing import TYPE_CHECKING, Optional
-from collections.abc import Callable
+from typing import TYPE_CHECKING
 
-import win32com.client
 from PySide6.QtCore import *
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
 import midiscripter.base.shared
 import midiscripter.file_event
 import midiscripter.gui.main_window
 import midiscripter.midi.midi_ports_update
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
+    from base.msg_base import Msg
+
 
 class SavedCheckedStateAction(QAction):
     def __init__(
         self,
         name: str,
-        func_for_state: Callable | None = None,
+        func_for_state: 'Callable | None' = None,
         *,
-        checked_func: Callable | None = None,
-        unchecked_func: Callable | None = None,
+        checked_func: 'Callable | None' = None,
+        unchecked_func: 'Callable | None' = None,
         default_state: bool = False,
-        key_shortcut: QKeySequence | None = None,
+        key_shortcut: 'QKeySequence | None' = None,
     ):
         super().__init__(name)
         self.__func_for_state = func_for_state
         self.__checked_func = checked_func
         self.__unchecked_func = unchecked_func
         self.__default_state = default_state
         self.__setting_name = f'action {name}'
@@ -36,21 +36,21 @@
         if key_shortcut:
             self.setShortcut(key_shortcut)
 
         self.setCheckable(True)
         # replaces force _state_changed that causes widgets toggled by action to pop up
         self.setChecked(default_state)
         self.toggled.connect(self.__state_changed)
-        self.setChecked(QSettings().value(self.__setting_name, int(default_state)))
+        self.setChecked(bool(self))
 
     def __bool__(self):
-        return bool(QSettings().value(self.__setting_name, int(self.__default_state)))
+        return bool(QSettings().value(self.__setting_name, self.__default_state, type=bool))
 
-    def __state_changed(self, state: bool):
-        QSettings().setValue(self.__setting_name, int(state))
+    def __state_changed(self, state: bool) -> None:
+        QSettings().setValue(self.__setting_name, state)
 
         if self.__func_for_state:
             self.__func_for_state(state)
 
         if state is True and self.__checked_func:
             self.__checked_func()
         if state is False and self.__unchecked_func:
@@ -72,24 +72,19 @@
         script_menu.addAction('Run another', self._run_another_script)
         script_menu.addAction('&Restart', QApplication.instance().restart, QKeySequence('Ctrl+R'))
         script_menu.addAction('&Quit', QApplication.instance().exit, QKeySequence('Ctrl+Q'))
 
         # Options
         options_menu = self.addMenu('Options')
 
-        if platform.system() == 'Windows':
-            shortcut_name = (
-                f'{self.autostart_shortcut_prefix}'
-                f'{pathlib.Path(midiscripter.base.shared.script_path).stem}.lnk'
-            )
-            self.__autostart_script_path = self.autostart_path / shortcut_name
-            toggle_autostart = options_menu.addAction('Run at start up')
-            toggle_autostart.setCheckable(True)
-            toggle_autostart.setChecked(self.__autostart_script_path.is_file())
-            toggle_autostart.toggled.connect(self.__set_autostart)
+        self.autostart = midiscripter.base.shared.AutostartManager()
+        toggle_autostart = options_menu.addAction('Run at start up')
+        toggle_autostart.setCheckable(True)
+        toggle_autostart.setChecked(self.autostart._check_if_enabled())
+        toggle_autostart.toggled.connect(self.__set_autostart)
 
         self.always_on_top = SavedCheckedStateAction(
             'Window always on top',
             main_window.set_always_on_top,
             key_shortcut=QKeySequence('Ctrl+Space'),
         )
         options_menu.insertAction(QAction(), self.always_on_top)
@@ -127,80 +122,61 @@
             lambda: QDesktopServices.openUrl(QUrl('https://github.com/Maboroshy/midi-scripter')),
         )
         script_menu.addAction(
             'Documentation',
             lambda: QDesktopServices.openUrl(QUrl('https://maboroshy.github.io/midi-scripter')),
         )
 
-    def _run_another_script(self):
+    def _run_another_script(self) -> None:
         file_path_str = QFileDialog.getOpenFileName(
             self,
             'Select python script',
             str(pathlib.Path(midiscripter.base.shared.script_path).parent),
             'Python script (*.py)',
         )[0]
         if file_path_str:
             midiscripter.base.shared.script_path = file_path_str
             QApplication.instance().restart()
 
     @Slot(bool)
     def __set_autostart(self, state: bool) -> None:
-        other_autostart_shortcuts = []
-        for path in self.autostart_path.iterdir():
-            if (
-                path.name.startswith(self.autostart_shortcut_prefix)
-                and path.is_file()
-                and path != self.__autostart_script_path.resolve()
-            ):
-                other_autostart_shortcuts.append(path)  # noqa: PERF401
-
-        if other_autostart_shortcuts:
+        if self.autostart._check_if_other_scripts_present():
             remove_other_dialog = QMessageBox()
             remove_other_dialog.setText(
                 'There are other scripts with enabled autostart. Disable them?'
             )
             remove_other_dialog.setStandardButtons(
                 QMessageBox.Yes | QMessageBox.No | QMessageBox.Cancel
             )
             remove_other_dialog_pressed_button = remove_other_dialog.exec()
 
             if remove_other_dialog_pressed_button == QMessageBox.Cancel:
                 return
             elif remove_other_dialog_pressed_button == QMessageBox.Yes:
-                for shortcut_path in other_autostart_shortcuts:
-                    shortcut_path.unlink()
+                self.autostart._disable_others()
 
         if state:
-            shell = win32com.client.Dispatch('WScript.Shell')
-            shortcut = shell.CreateShortCut(str(self.__autostart_script_path.resolve()))
-            shortcut.Targetpath = str(pathlib.Path(sys.executable).parent / 'pythonw.exe')
-            shortcut.WorkingDirectory = str(
-                pathlib.Path(midiscripter.base.shared.script_path).parent.resolve()
-            )
-            shortcut.Arguments = (
-                f'"{pathlib.Path(midiscripter.base.shared.script_path).resolve()}" "--tray"'
-            )
-            shortcut.save()
+            self.autostart._enable()
         else:
-            self.__autostart_script_path.resolve().unlink(True)
+            self.autostart._disable()
 
-    def __set_watching_script_file(self, new_status: bool):
+    def __set_watching_script_file(self, new_status: bool) -> None:
         if new_status:
             self.file_watcher_port = midiscripter.file_event.FileEventIn(
                 midiscripter.base.shared.script_path
             )
             self.file_watcher_port.subscribe(QApplication.instance().restart_at_file_change)
             self.file_watcher_port._open()
         else:
             self.file_watcher_port.is_enabled = False
 
-    def __set_watching_midi_ports(self, new_status: bool):
+    def __set_watching_midi_ports(self, new_status: bool) -> None:
         if new_status:
             self.midi_port_watcher_port = midiscripter.midi.midi_ports_update.MidiPortsChangedIn()
 
             @self.midi_port_watcher_port.subscribe
-            def restart_on_midi_port_change(_):
+            def restart_on_midi_port_change(_: 'Msg') -> None:
                 QApplication.instance().request_restart.emit()
 
             self.midi_port_watcher_port._open()
         else:
             self.midi_port_watcher_port.is_enabled = False
```

### Comparing `midiscripter-0.2/midiscripter/gui/ports_widget.py` & `midiscripter-0.3/midiscripter/gui/ports_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 from collections.abc import Callable
 
 from PySide6.QtCore import *
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
 import midiscripter.logger.html_sink
@@ -13,107 +14,130 @@
 class PortsWidget(QTreeWidget):
     PORT_CLASS_ROLE = 100
     PORT_UID_ROLE = 101
     PORT_REPR_ROLE = 103
     CALLBACK_FUNCTION_ROLE = 104
     PASSTHROUGH_OUT_PORT_ROLE = 105
 
+    VIRTUAL_PORT_PREFIX = '[v]'
+
     def __init__(self):
         super().__init__()
         self.setObjectName('Ports')
         self.setHeaderHidden(True)
         self.setMinimumWidth(200)
         self.setMinimumHeight(200)
         self.setMouseTracking(True)
         self.itemEntered.connect(self.__update_item_tooltip)
         self.__populate()
 
-    def __add_top_level_item(self, item_text: str):
+    def __add_top_level_item(self, item_text: str) -> None:
         bold_font = self.font()
         bold_font.setBold(True)
 
         top_item = QTreeWidgetItem(self, (item_text,))
         top_item.setData(0, Qt.ItemDataRole.FontRole, bold_font)
         top_item.setExpanded(True)
 
         return top_item
 
-    def __populate(self):
+    def __populate(self) -> None:
         """Populates the widget with items"""
         self.clear()
-        self.__add_midi_inputs()
-        self.__add_midi_outputs()
+        self.__add_midi_port_class(
+            'MIDI Inputs', MidiIn, midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input], True
+        )
+        self.__add_midi_port_class(
+            'MIDI Outputs', MidiOut, midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output], False
+        )
         self.__add_ports_if_declared('OSC Inputs', midiscripter.OscIn)
         self.__add_ports_if_declared('OSC Outputs', midiscripter.OscOut)
         self.__add_keyboard_in()
         self.__add_ports_if_declared('Keyboard Output', midiscripter.KeyOut)
         self.__add_ports_if_declared('Metronome', midiscripter.MetronomeIn)
         self.__add_ports_if_declared('File Event Watcher', midiscripter.FileEventIn)
         self.__add_ports_if_declared('MIDI Port Changes Watcher', midiscripter.MidiPortsChangedIn)
 
         self.itemChanged.connect(self.__item_state_changed)
         self.itemSelectionChanged.connect(self.__item_selected)
 
-    def __add_midi_inputs(self):
-        if not MidiIn._available_names:
+    def __add_midi_port_class(
+        self,
+        title: str,
+        port_class: type[MidiIn | MidiOut],
+        item_color: QColor,
+        add_attached: bool,
+    ) -> None:
+        if not port_class._available_names:
             return
 
-        inputs_top = self.__add_top_level_item('MIDI Inputs')
+        top_item = self.__add_top_level_item(title)
 
-        for input_port_name in MidiIn._available_names:
-            port_key = (MidiIn.__name__, input_port_name)
-            port_instance = MidiIn.instance_registry.get(port_key, None)
-            input_item = QTreeWidgetItem(inputs_top, (input_port_name,))
+        virtual_port_names = [
+            port._uid
+            for port in port_class.instance_registry.values()
+            if isinstance(port, port_class) and port._is_virtual
+        ]
+
+        for port_name in itertools.chain(port_class._available_names, virtual_port_names):
+            port_key = (port_class.__name__, port_name)
+            port_instance = port_class.instance_registry.get(port_key, None)
+
+            port_item_name = (
+                f'{self.VIRTUAL_PORT_PREFIX} {port_name}'
+                if port_instance and port_instance._is_virtual
+                else port_name
+            )
+            port_item = QTreeWidgetItem(top_item, (port_item_name,))
 
             if not port_instance:
-                input_item.setCheckState(0, Qt.CheckState.Unchecked)
+                port_item.setCheckState(0, Qt.CheckState.Unchecked)
             elif port_instance.is_enabled:
-                input_item.setCheckState(0, Qt.CheckState.Checked)
+                port_item.setCheckState(0, Qt.CheckState.Checked)
             else:
-                input_item.setCheckState(0, Qt.CheckState.Unchecked)
-                input_item.setData(
+                port_item.setCheckState(0, Qt.CheckState.Unchecked)
+                port_item.setData(
                     0, Qt.ItemDataRole.BackgroundRole, QBrush(QColor().fromRgb(255, 0, 0, 20))
                 )
 
-            input_item.setData(0, self.PORT_CLASS_ROLE, MidiIn)
-            input_item.setData(0, self.PORT_UID_ROLE, input_port_name)
+            port_item.setData(0, self.PORT_CLASS_ROLE, port_class)
+            port_item.setData(0, self.PORT_UID_ROLE, port_name)
 
-            port_repr = f"{MidiIn.__name__}('{input_port_name}')"
-            input_item.setData(0, self.PORT_REPR_ROLE, port_repr)
-
-            input_item.setData(
-                0,
-                Qt.ItemDataRole.ForegroundRole,
-                QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]),
-            )
+            port_repr = f"{port_class.__name__}('{port_name}')"
+            port_item.setData(0, self.PORT_REPR_ROLE, port_repr)
+            port_item.setData(0, Qt.ItemDataRole.ForegroundRole, QBrush(item_color))
 
-            if port_instance:
+            if add_attached and port_instance:
                 for passthrough_out_port in port_instance.attached_passthrough_outs:
-                    sub_item = QTreeWidgetItem(input_item, (passthrough_out_port._uid,))
+                    sub_item = QTreeWidgetItem(port_item, (passthrough_out_port._uid,))
                     sub_item.setCheckState(0, Qt.CheckState.Checked)
 
                     sub_item.setData(
                         0,
                         Qt.ItemDataRole.ForegroundRole,
                         QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]),
                     )
                     sub_item.setData(0, self.PORT_CLASS_ROLE, MidiIn)
-                    sub_item.setData(0, self.PORT_UID_ROLE, input_port_name)
+                    sub_item.setData(0, self.PORT_UID_ROLE, port_name)
                     sub_item.setData(0, self.PASSTHROUGH_OUT_PORT_ROLE, passthrough_out_port)
                     sub_item.setData(0, self.PORT_REPR_ROLE, passthrough_out_port.__repr__())
 
-                self.__add_inputs_subscribed_calls(input_item)
+                self.__add_inputs_subscribed_calls(port_item)
 
-        for port_instance in MidiIn.instance_registry.values():
-            if isinstance(port_instance, MidiIn) and not port_instance._is_available:
-                absent_input_item = QTreeWidgetItem(inputs_top, (str(port_instance),))
+        for port_instance in port_class.instance_registry.values():
+            if (
+                isinstance(port_instance, port_class)
+                and not port_instance._is_available
+                and port_instance._uid not in virtual_port_names
+            ):
+                absent_input_item = QTreeWidgetItem(top_item, (str(port_instance),))
                 absent_input_item.setCheckState(0, Qt.CheckState.Unchecked)
                 absent_input_item.setDisabled(True)
 
-    def __add_inputs_subscribed_calls(self, input_item: QTreeWidgetItem):
+    def __add_inputs_subscribed_calls(self, input_item: QTreeWidgetItem) -> None:
         port_class = input_item.data(0, self.PORT_CLASS_ROLE)
         port_name = input_item.data(0, self.PORT_UID_ROLE)
 
         port_instance = port_class(port_name) if port_name else port_class()
 
         for callback_function in port_instance.subscribed_calls:
             sub_item = QTreeWidgetItem(input_item, (callback_function.__name__,))
@@ -124,54 +148,15 @@
                 Qt.ItemDataRole.ForegroundRole,
                 QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Callable]),
             )
             sub_item.setData(0, self.PORT_CLASS_ROLE, MidiIn)
             sub_item.setData(0, self.PORT_UID_ROLE, port_name)
             sub_item.setData(0, self.CALLBACK_FUNCTION_ROLE, callback_function)
 
-    def __add_midi_outputs(self):
-        if not MidiOut._available_names:
-            return
-
-        outputs_top = self.__add_top_level_item('MIDI Outputs')
-
-        for output_port_name in MidiOut._available_names:
-            port_key = (MidiOut.__name__, output_port_name)
-            port_instance = MidiOut.instance_registry.get(port_key, None)
-            output_item = QTreeWidgetItem(outputs_top, (output_port_name,))
-
-            if not port_instance:
-                output_item.setCheckState(0, Qt.CheckState.Unchecked)
-            elif port_instance.is_enabled:
-                output_item.setCheckState(0, Qt.CheckState.Checked)
-            else:
-                output_item.setCheckState(0, Qt.CheckState.Unchecked)
-                output_item.setData(
-                    0, Qt.ItemDataRole.BackgroundRole, QBrush(QColor().fromRgb(255, 0, 0, 20))
-                )
-
-            output_item.setData(0, self.PORT_CLASS_ROLE, MidiOut)
-            output_item.setData(0, self.PORT_UID_ROLE, output_port_name)
-
-            port_repr = f"{MidiOut.__name__}('{output_port_name}')"
-            output_item.setData(0, self.PORT_REPR_ROLE, port_repr)
-
-            output_item.setData(
-                0,
-                Qt.ItemDataRole.ForegroundRole,
-                QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]),
-            )
-
-        for port_instance in MidiOut.instance_registry.values():
-            if isinstance(port_instance, MidiOut) and not port_instance._is_available:
-                absent_output_item = QTreeWidgetItem(outputs_top, (port_instance._uid,))
-                absent_output_item.setCheckState(0, Qt.CheckState.Unchecked)
-                absent_output_item.setDisabled(True)
-
-    def __add_ports_if_declared(self, title: str, port_type: type):
+    def __add_ports_if_declared(self, title: str, port_type: type[Input | Output]) -> None:
         port_instances_to_add = []
         for port_key, port_instance in port_type.instance_registry.items():
             if port_key[0] is port_type.__name__:
                 port_instances_to_add.append(port_instance)
 
         if not port_instances_to_add:
             return
@@ -189,20 +174,20 @@
                 port_item.setData(0, self.PORT_UID_ROLE, None)
             else:
                 port_item.setData(0, self.PORT_UID_ROLE, port._uid)
 
             if issubclass(port_type, Input):
                 item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]
                 self.__add_inputs_subscribed_calls(port_item)
-            elif issubclass(port_type, Output):
+            else:
                 item_color = midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Output]
 
             port_item.setData(0, Qt.ItemDataRole.ForegroundRole, QBrush(item_color))
 
-    def __add_keyboard_in(self):
+    def __add_keyboard_in(self) -> None:
         port_top = self.__add_top_level_item('Keyboard Input')
         port_item = QTreeWidgetItem(port_top, ('Keyboard Input',))
         if (
             midiscripter.KeyIn.__name__,
             midiscripter.KeyIn._force_uid,
         ) in midiscripter.KeyIn.instance_registry:
             port_item.setCheckState(0, Qt.CheckState.Checked)
@@ -214,15 +199,15 @@
         port_item.setData(0, self.PORT_REPR_ROLE, f'{midiscripter.KeyIn.__name__}()')
         port_item.setData(
             0,
             Qt.ItemDataRole.ForegroundRole,
             QBrush(midiscripter.logger.html_sink.HtmlSink.COLOR_MAP[Input]),
         )
 
-    def __item_selected(self):
+    def __item_selected(self) -> None:
         """Sends selected item text to the clipboard and shows a "copied" tooltip"""
         if not self.selectedItems():
             return
 
         selected_item: QTreeWidgetItem = self.selectedItems()[0]
         port_repr = selected_item.data(0, self.PORT_REPR_ROLE)
         if port_repr:
@@ -231,16 +216,17 @@
                 200,
                 lambda: QToolTip().showText(
                     self.cursor().pos(), f'Copied {port_repr}', self, msecShowTime=2000
                 ),
             )  # Don't hide on mouse button release
         selected_item.setSelected(False)
 
-    def __item_state_changed(self, item: QTreeWidgetItem, _):
-        """Enabled or disables the MIDI port / passthrough out / call according to the checked state change"""
+    def __item_state_changed(self, item: QTreeWidgetItem, _: int) -> None:
+        """Enabled or disables the MIDI port / passthrough out / call according to the checked
+        state change"""
         new_checked_state = item.checkState(0) == Qt.CheckState.Checked
 
         port_class = item.data(0, self.PORT_CLASS_ROLE)
         port_name = item.data(0, self.PORT_UID_ROLE)
 
         callback_function = item.data(0, self.CALLBACK_FUNCTION_ROLE)
         passthrough_out_port: MidiOut = item.data(0, self.PASSTHROUGH_OUT_PORT_ROLE)
@@ -259,22 +245,24 @@
             else:
                 port_instance.attached_passthrough_outs.remove(passthrough_out_port)
 
         else:
             if new_checked_state:
                 if not port_instance.is_enabled:
                     port_instance._open()
-                    port_instance.is_enabled = True
-                    log('Enabled {port}', port=port_instance)
 
-                if not port_instance.is_enabled:
-                    item.setData(
-                        0, Qt.ItemDataRole.BackgroundRole, QBrush(QColor().fromRgb(255, 0, 0, 20))
-                    )
-                    log.red("Can't enable {port}", port=port_instance)
+                    if port_instance.is_enabled:
+                        log('Enabled {port}', port=port_instance)
+                    else:
+                        item.setData(
+                            0,
+                            Qt.ItemDataRole.BackgroundRole,
+                            QBrush(QColor().fromRgb(255, 0, 0, 20)),
+                        )
+                        log.red("Can't enable {port}", port=port_instance)
                 else:
                     item.setData(
                         0,
                         Qt.ItemDataRole.BackgroundRole,
                         QBrush(QColor(Qt.GlobalColor.transparent)),
                     )
 
@@ -284,15 +272,15 @@
 
             self.blockSignals(True)
             item.setCheckState(
                 0, (Qt.CheckState.Unchecked, Qt.CheckState.Checked)[port_instance.is_enabled]
             )
             self.blockSignals(False)
 
-    def __update_item_tooltip(self, item: QTreeWidgetItem):
+    def __update_item_tooltip(self, item: QTreeWidgetItem) -> None:
         """Updates items tooltip on hover"""
         call_function = item.data(0, self.CALLBACK_FUNCTION_ROLE)
         if call_function:
             port_class = item.data(0, self.PORT_CLASS_ROLE)
             call_statistics = list(port_class._call_statistics[call_function])
 
             if not call_statistics:
```

### Comparing `midiscripter-0.2/midiscripter/gui/gui_widgets/button.py` & `midiscripter-0.3/midiscripter/gui/gui_widgets/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Optional, Union
 from collections.abc import Sequence
 
 from PySide6.QtWidgets import *
 
 from .gui_widget_base import GuiWidget
 from .mixins import AdaptiveTextSizeMixin, WrappedQWidgetMixin
 
@@ -109,15 +108,15 @@
             self.qt_button_group.addButton(qt_button, index)
 
             self.wrapped_qt_buttons_map[index] = qt_button
             self.wrapped_qt_buttons_map[text] = qt_button
 
         self.qt_button_group.idReleased.connect(self.selection_changed_signal)
 
-    def set_selection(self, selection: int | str):
+    def set_selection(self, selection: int | str) -> None:
         try:
             self.wrapped_qt_buttons_map[selection].click()
         except KeyError:
             pass
 
     def get_selected_item_index(self) -> int | None:
         return self.qt_button_group.checkedId()
@@ -130,15 +129,15 @@
 class GuiButtonSelectorH(GuiWidget):
     """Button group to select value, horizontal layout."""
 
     _qt_widget_class = ButtonGroupWidgetHorizontal
 
     def __init__(
         self,
-        content: Sequence[str],
+        content: tuple[str, ...],
         title: str | None = None,
         color: str | tuple[int, int, int] | None = None,
         *,
         select: int | str | None = None,
     ):
         """
         Args:
@@ -157,15 +156,15 @@
 class GuiButtonSelectorV(GuiWidget):
     """Button group to select value, vertical layout."""
 
     _qt_widget_class = ButtonGroupWidgetVertical
 
     def __init__(
         self,
-        content: Sequence[str],
+        content: tuple[str, ...],
         title: str | None = None,
         color: str | tuple[int, int, int] | None = None,
         *,
         select: int | str | None = None,
     ):
         """
         Args:
```

### Comparing `midiscripter-0.2/midiscripter/gui/gui_widgets/gui_msg.py` & `midiscripter-0.3/midiscripter/gui/gui_widgets/gui_msg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import TYPE_CHECKING, Optional, Union
-from collections.abc import Sequence
+from typing import TYPE_CHECKING
 
 import midiscripter.base.msg_base
 
 if TYPE_CHECKING:
+    from collections.abc import Sequence, Container
     from midiscripter.gui.gui_widgets.gui_widget_base import GuiWidget
 
 
 class GuiEventType(midiscripter.base.msg_base.AttrEnum):
     """GUI event type enumerator to use as [`GuiEventMsg`][midiscripter.GuiEventMsg] `type` attribute."""
 
     TRIGGERED = 'TRIGGERED'
@@ -20,36 +20,41 @@
 
 class GuiEventMsg(midiscripter.base.msg_base.Msg):
     """GUI interaction message produced by GUI widget port."""
 
     type: GuiEventType
     """GUI event type."""
 
-    data: str | int | bool | Sequence | None
+    data: 'str | int | bool | Sequence | None'
     """New value set by event.
     
     Data meaning for event types:  
     TRIGGERED - None.  
     CONTENT_SET - New content.  
     COLOR_SET - New text color.  
     TOGGLED - New toggle state.  
     SELECTED - Selected item text.  
     VALUE_CHANGED - New value.
     """
 
-    source: Optional['GuiWidget']
+    source: 'None | GuiWidget'
 
     __match_args__: tuple[str] = ('type', 'data')
 
     def __init__(
         self,
         type: GuiEventType,
-        data: str | int | bool | Sequence | None = None,
+        data: 'str | int | bool | Sequence | None' = None,
         *,
-        source: Optional['GuiWidget'] = None,
+        source: 'None | GuiWidget' = None,
     ):
         super().__init__(source)
         self.type = type
         self.data = data
 
-    def matches(self, type=None, data=None) -> bool:
+    def matches(
+        self,
+        type: 'None | Container[GuiEventType] | GuiEventType' = None,
+        data: 'None | Container[str | int | bool | Sequence | None] | \
+                       str | int | bool | Sequence | None' = None,
+    ) -> bool:
         return super().matches(type, data)
```

### Comparing `midiscripter-0.2/midiscripter/gui/gui_widgets/gui_widget_base.py` & `midiscripter-0.3/midiscripter/gui/gui_widgets/gui_widget_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import TYPE_CHECKING, Optional, Union
+import types
+from typing import TYPE_CHECKING
 from collections.abc import Sequence
 
 from PySide6.QtWidgets import *
 
 import midiscripter.base.msg_base
 import midiscripter.base.port_base
 import midiscripter.gui.app
@@ -16,15 +17,15 @@
 class GuiWidget(midiscripter.base.port_base.Input):
     """GUI windows widget which also acts like an input port."""
 
     _qt_widget_class: type[QWidget, 'WrappedQWidgetMixin']
 
     def __init__(
         self,
-        content: str | Sequence[str],
+        content: str | tuple[str, ...],
         title: str | None = None,
         color: str | tuple[int, int, int] | None = None,
         *,
         value: str | None = None,
         select: int | str | None = None,
         toggle_state: bool | None = None,
     ):
@@ -33,14 +34,17 @@
             content: Widget's text or text for its items
             title: Widget's title, `None` for same as content
             color: Preset text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple
             value: Preset value
             select: Preset item text / index to select
             toggle_state: Preset toggle state
         """
+        if isinstance(content, types.GeneratorType):
+            content = tuple(content)
+
         self.title = title or str(content)
         """Widget's title."""
         super().__init__(self.title)
 
         self.qt_widget = self._qt_widget_class()  # workaround for mkdocstrings issue #607
 
         self.qt_widget: QWidget
@@ -87,33 +91,33 @@
         self.qt_widget.toggle_state_changed_signal.connect(
             lambda: self._send_input_msg_to_calls(
                 GuiEventMsg(GuiEventType.TOGGLED, self.qt_widget.get_toggle_state())
             )
         )
 
     @property
-    def content(self):
+    def content(self) -> str | tuple[str, ...]:
         """Widget's text or text for its items."""
         return self.qt_widget.get_content()
 
     @content.setter
-    def content(self, new_content: str | Sequence[str]):
+    def content(self, new_content: str | tuple[str, ...]) -> None:
         self.qt_widget.set_content_signal.emit(new_content)
         self.qt_widget.content_changed_signal.emit()
 
     @property
     def value(self) -> str | None:
         """Widget's value / selected item text."""
         try:
             return self.qt_widget.get_value()
         except NotImplementedError:
             return None
 
     @value.setter
-    def value(self, new_value):
+    def value(self, new_value: str | None) -> None:
         self.qt_widget.set_value_signal.emit(new_value)
         self.qt_widget.value_changed_signal.emit()
 
     @property
     def selected_item_text(self) -> str | None:
         """Widget's currently selected item's text."""
         try:
@@ -125,15 +129,15 @@
     def selected_item_index(self) -> int | None:
         """Widget's currently selected item's index"""
         try:
             return self.qt_widget.get_selected_item_index()
         except NotImplementedError:
             return None
 
-    def select(self, selection: int | str):
+    def select(self, selection: int | str) -> None:
         """Select widget's item
 
         Args:
             selection: Index or text of item to select
         """
         self.qt_widget.set_selection_signal.emit(selection)
         self.qt_widget.selection_changed_signal.emit()
@@ -143,25 +147,25 @@
         """Toggle state."""
         try:
             return self.qt_widget.get_toggle_state()
         except NotImplementedError:
             return None
 
     @toggle_state.setter
-    def toggle_state(self, new_state: bool):
+    def toggle_state(self, new_state: bool) -> None:
         self.qt_widget.set_toggle_state_signal.emit(new_state)
         self.qt_widget.toggle_state_changed_signal.emit()
 
     @property
     def color(self) -> str | tuple[int, int, int] | None:
         """Text color as [color name](https://www.w3.org/TR/SVG11/types.html#ColorKeywords) or RGB tuple"""
         return self.qt_widget.get_color()
 
     @color.setter
-    def color(self, new_color_value: str | tuple[int, int, int]):
+    def color(self, new_color_value: str | tuple[int, int, int]) -> None:
         self.qt_widget.set_color_signal.emit(new_color_value)
         self._send_input_msg_to_calls(
             GuiEventMsg(GuiEventType.COLOR_SET, new_color_value, source=self)
         )
 
     @property
     def is_visible(self) -> bool:
```

### Comparing `midiscripter-0.2/midiscripter/gui/gui_widgets/layout.py` & `midiscripter-0.3/midiscripter/gui/gui_widgets/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
             'gui_widget_base.GuiWidget | GuiWidgetLayout | '
             'Sequence[gui_widget_base.GuiWidget | GuiWidgetLayout]'
         ],
     ):
         """
         Args:
             rows: A tuple of items to put in a row.
-            Items can be widgets, layouts or tuples of widgets or layouts.
-            If item is a tuple it's a column of items inside the tuple.
+                  Items can be widgets, layouts or tuples of widgets or layouts.
+                  If item is a tuple it's a column of items inside the tuple.
 
         Warning:
             Calls can't be subscribed to `GuiWidgetLayout`.
             Pre-declare widgets to subscribed calls to them.
 
         Example:
             ```
```

### Comparing `midiscripter-0.2/midiscripter/gui/gui_widgets/list.py` & `midiscripter-0.3/midiscripter/gui/gui_widgets/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Optional, Union
 from collections.abc import Sequence
 
 from PySide6.QtWidgets import *
 
 from .gui_widget_base import GuiWidget
 from .mixins import WrappedQWidgetMixin
 
@@ -17,22 +16,22 @@
         font = self.font()
         font.setPointSize(self.FONT_SIZE)
         self.setFont(font)
 
         self.__content = None
         self.currentRowChanged.connect(self.selection_changed_signal)
 
-    def get_content(self):
+    def get_content(self) -> tuple[str]:
         return self.__content
 
-    def set_content(self, list_items: Sequence[str]):
+    def set_content(self, list_items: tuple[str]) -> None:
         self.__content = list_items
         self.addItems(self.__content)
 
-    def set_selection(self, selection: int | str):
+    def set_selection(self, selection: int | str) -> None:
         if isinstance(selection, int):
             self.setCurrentRow(selection)
         else:
             try:
                 self.setCurrentRow(self.__content.index(selection))
             except ValueError:
                 pass
@@ -47,15 +46,15 @@
 class GuiListSelector(GuiWidget):
     """List of text items to select value."""
 
     _qt_widget_class = ListSelectorWidget
 
     def __init__(
         self,
-        content: Sequence[str],
+        content: tuple[str, ...],
         title: str | None = None,
         color: str | tuple[int, int, int] | None = None,
         *,
         select: int | str | None = None,
     ):
         """
         Args:
```

### Comparing `midiscripter-0.2/midiscripter/gui/gui_widgets/mixins.py` & `midiscripter-0.3/midiscripter/gui/gui_widgets/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Optional, Union
 from collections.abc import Sequence
 
 from PySide6.QtCore import *
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
 
@@ -29,42 +28,42 @@
         self.set_selection_signal.connect(self.set_selection)
         self.set_toggle_state_signal.connect(self.set_toggle_state)
         self.set_color_signal.connect(self.set_color)
 
     def get_content(self) -> str | Sequence[str]:
         raise NotImplementedError
 
-    def set_content(self, new_content: str | Sequence[str]):
+    def set_content(self, new_content: str | Sequence[str]) -> None:
         raise NotImplementedError
 
     def get_value(self) -> str | None:
         raise NotImplementedError
 
-    def set_value(self, new_value: str | int | bool):
+    def set_value(self, new_value: str | int | bool) -> None:
         raise NotImplementedError
 
     def get_selected_item_index(self) -> int | None:
         raise NotImplementedError
 
     def get_selected_item_text(self) -> str | None:
         raise NotImplementedError
 
-    def set_selection(self, selection: int | str):
+    def set_selection(self, selection: int | str) -> None:
         raise NotImplementedError
 
     def get_toggle_state(self) -> bool | None:
         raise NotImplementedError
 
-    def set_toggle_state(self, new_state: bool):
+    def set_toggle_state(self, new_state: bool) -> None:
         raise NotImplementedError
 
     def get_color(self) -> str | None:
         return self.__color
 
-    def set_color(self, new_color_value: str | tuple[int, int, int]):
+    def set_color(self, new_color_value: str | tuple[int, int, int]) -> None:
         if isinstance(new_color_value, str):
             color = QColor(new_color_value)
         else:
             color = QColor(*new_color_value)
 
         palette = self.palette()
         palette.setColor(QPalette.ColorGroup.Active, QPalette.ColorRole.ButtonText, color)
@@ -87,19 +86,19 @@
         if (
             text_rect.height() > self.__longest_text_rect_size.height()
             or text_rect.width() > self.__longest_text_rect_size.width()
         ):
             self.__make_text_size_fit_widget_size()
             self.__longest_text_rect_size = text_rect
 
-    def resizeEvent(self, event):
+    def resizeEvent(self, event: QResizeEvent) -> None:
         super().resizeEvent(event)
         self.__make_text_size_fit_widget_size()
 
-    def __make_text_size_fit_widget_size(self):
+    def __make_text_size_fit_widget_size(self) -> None:
         if not self.text():
             return
 
         font = self.font()
         content_rect = self.contentsRect()
 
         font_size = 0
```

### Comparing `midiscripter-0.2/midiscripter/gui/gui_widgets/text.py` & `midiscripter-0.3/midiscripter/gui/gui_widgets/text.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional, Union
-
 from PySide6.QtCore import *
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
 from .gui_widget_base import GuiWidget
 from .mixins import AdaptiveTextSizeMixin, WrappedQWidgetMixin
 
@@ -17,15 +15,15 @@
 
         self.get_content = self.text
         self.set_content = self.setText
 
     def get_toggle_state(self) -> bool:
         return self.isEnabled()
 
-    def set_toggle_state(self, new_state: bool):
+    def set_toggle_state(self, new_state: bool) -> None:
         self.setEnabled(new_state)
 
 
 class GuiText(GuiWidget):
     """Text widget. Goes grey on toggle off.
 
     Tip:
```

### Comparing `midiscripter-0.2/midiscripter/keyboard/keyboard_msg.py` & `midiscripter-0.3/midiscripter/keyboard/keyboard_msg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING
 from collections.abc import Iterable
 
 import pynput.keyboard
 
 import midiscripter.base.msg_base
 
 if TYPE_CHECKING:
+    from collections.abc import Container
     from midiscripter.keyboard.keyboard_port import KeyIn
 
 
 MODIFIER_KEYS = {
     pynput.keyboard.Key.alt,
     pynput.keyboard.Key.cmd,
     pynput.keyboard.Key.ctrl,
@@ -44,22 +45,22 @@
 
     type: KeyEventType
     """Keyboard event type"""
 
     keycodes: list[pynput.keyboard.Key]
     """Keycodes in the order they were pressed. Use when press order matters."""
 
-    source: Optional['KeyIn']
+    source: 'None | KeyIn'
 
     def __init__(
         self,
         type: KeyEventType,
         shortcut_or_keycodes: str | Iterable[pynput.keyboard.Key],
         *,
-        source: Optional['KeyIn'] = None,
+        source: 'None | KeyIn' = None,
     ):
         """
         Args:
             type: Keyboard event type
             shortcut_or_keycodes: keyboard shortcut description or event key codes
             source (KeyIn): The [`KeyIn`][midiscripter.KeyIn] instance that generated the message
 
@@ -100,18 +101,22 @@
 
             self.__cached_keycodes = self.keycodes
             self.__shortcut_cache = shortcut
 
         return self.__shortcut_cache
 
     @shortcut.setter
-    def shortcut(self, shortcut: str):
+    def shortcut(self, shortcut: str) -> None:
         self.keycodes = []
         for key in shortcut.split('+'):
             if len(key) == 1:
                 key = pynput.keyboard.KeyCode.from_char(key)
             else:
                 key = getattr(pynput.keyboard.Key, key)
             self.keycodes.append(key)
 
-    def matches(self, type=None, shortcut=None):
+    def matches(
+        self,
+        type: 'None | Container[KeyEventType] | KeyEventType' = None,
+        shortcut: 'None | Container[str] | str' = None,
+    ) -> bool:
         return super().matches(type, shortcut)
```

### Comparing `midiscripter-0.2/midiscripter/keyboard/keyboard_port.py` & `midiscripter-0.3/midiscripter/keyboard/keyboard_port.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 
     def __init__(self):
         """ """  # to override Input docstring
         super().__init__(self._force_uid)
         self.__pynput_listener = None
         self.pressed_keys = []
 
-    def __on_press(self, key: pynput.keyboard.Key):
+    def __on_press(self, key: pynput.keyboard.Key) -> None:
         if not self.is_enabled:
             return
 
         if type(key) is pynput.keyboard.KeyCode:
             key = self.__pynput_listener.canonical(key)
 
         if key not in self.pressed_keys:
             self.pressed_keys.append(key)
 
         msg = KeyMsg(KeyEventType.KEY_PRESS, self.pressed_keys.copy(), source=self)
         self._send_input_msg_to_calls(msg)
 
-    def __on_release(self, key: pynput.keyboard.Key):
+    def __on_release(self, key: pynput.keyboard.Key) -> None:
         if not self.is_enabled:
             return
 
         if type(key) is pynput.keyboard.KeyCode:
             key = self.__pynput_listener.canonical(key)
 
         try:
@@ -45,49 +45,52 @@
             self.pressed_keys.remove(key)
 
             msg = KeyMsg(KeyEventType.KEY_RELEASE, pressed_keys_for_msg, source=self)
             self._send_input_msg_to_calls(msg)
         except ValueError:
             pass
 
-    def _open(self):
+    def _open(self) -> None:
         if self.__pynput_listener:
+            self.is_enabled = True
             return
 
         self.__pynput_listener = pynput.keyboard.Listener(self.__on_press, self.__on_release)
         self.__pynput_listener.start()
         self.__pynput_listener.wait()
         self.is_enabled = True
         log('Started keyboard input listener')
 
-    def _close(self):
+    def _close(self) -> None:
         self.__pynput_listener.stop()
         self.is_enabled = False
         log('Stopped keyboard input listener')
 
 
 class KeyOut(midiscripter.base.port_base.Output):
     """Keyboard output port. Sends [`KeyMsg`][midiscripter.KeyMsg] objects."""
 
     _force_uid = 'Keyboard Output'
 
     def __init__(self):
         super().__init__(self._force_uid)
         self.__pynput_controller = pynput.keyboard.Controller()
 
-    def send(self, msg: KeyMsg):
+    def send(self, msg: KeyMsg) -> None:
         """Send the keyboard input.
 
         Args:
             msg: object to send
         """
+        if not self._validate_msg_send(msg):
+            return
+
         # Log messages sent before actual sending, so receive messages for sent keys
         # won't be displayed before the message
-        with self._check_and_log_sent_message(msg):
-            pass
+        self._log_msg_sent(msg)
 
         if msg.type is KeyEventType.KEY_PRESS:
             for keycode in msg.keycodes:
                 self.__pynput_controller.press(keycode)
 
         elif msg.type is KeyEventType.KEY_RELEASE:
             for keycode in msg.keycodes:
@@ -95,9 +98,9 @@
 
         elif msg.type is KeyEventType.KEY_TAP:
             for keycode in msg.keycodes:
                 self.__pynput_controller.press(keycode)
             for keycode in reversed(msg.keycodes):
                 self.__pynput_controller.release(keycode)
 
-    def type_in(self, string_to_type: str):
+    def type_in(self, string_to_type: str) -> None:
         self.__pynput_controller.type(string_to_type)
```

### Comparing `midiscripter-0.2/midiscripter/logger/console_sink.py` & `midiscripter-0.3/midiscripter/logger/console_sink.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.2/midiscripter/logger/html_sink.py` & `midiscripter-0.3/midiscripter/logger/html_sink.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.2/midiscripter/logger/log.py` & `midiscripter-0.3/midiscripter/logger/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import collections
 import threading
 import time
-from typing import TYPE_CHECKING, Union
-from collections.abc import Callable
+from typing import TYPE_CHECKING
 
 import midiscripter.base.shared
 
 if TYPE_CHECKING:
+    from collections.abc import Callable
     from midiscripter.logger.console_sink import ConsoleSink
     from midiscripter.logger.html_sink import HtmlSink
 
 
 class Log:
     """Prints log messages to GUI Log widget or console.
     Can print messages in different text colors and highlight object representations.
@@ -36,15 +36,15 @@
         self.__sink = None
         self.is_enabled = True
 
         self.__buffer = collections.deque(maxlen=self.BUFFER_SIZE)
         self.__start_buffer_flush_thread()
         self.__wait_counter = 0
 
-    def __call__(self, text, **kwargs):
+    def __call__(self, text: str, **kwargs):
         """Print log message.
 
         Args:
             text: Log entry to print. Use `.format` style string to insert kwargs.
             **kwargs: Optional variables to `.format` text with.
                       Passed [inputs][midiscripter.base.port_base.Input],
                       [outputs][midiscripter.base.port_base.Output],
@@ -61,37 +61,37 @@
         milisec_part = after_dot[:3]
         microsec_part = after_dot[3:]
         kwargs['_ctime_str'] = f'{time_string}.{milisec_part},{microsec_part}'
 
         self.__buffer.append((str(text), kwargs))
 
     @property
-    def _sink(self):
+    def _sink(self) -> 'Callable':
         """A callable that receives a list of log strings to print them for user.
         Set by starter. Can be altered to customize the logger."""
         return self.__sink
 
     @_sink.setter
-    def _sink(self, sink_obj: Union['HtmlSink', 'ConsoleSink', Callable[[list[str]], None]]):
+    def _sink(self, sink_obj: 'HtmlSink | ConsoleSink | Callable[[list[str]], None]') -> None:
         self.__sink = sink_obj
         self._flush()
         self.__start_buffer_flush_thread()
 
-    def __start_buffer_flush_thread(self):
+    def __start_buffer_flush_thread(self) -> None:
         threading.Thread(target=self._buffer_flush_worker, daemon=True).start()
 
-    def _buffer_flush_worker(self):
+    def _buffer_flush_worker(self) -> None:
         """Thread worker loop that flushes buffered messages"""
         while self._sink:
             time.sleep(self.FLUSH_DELAY)
             self.__wait_counter += self.FLUSH_DELAY
             if self.__buffer:
                 self._flush()
 
-    def _flush(self):
+    def _flush(self) -> None:
         """Sends buffered messages to sink"""
         output_entries = []
 
         if self.__wait_counter > self.ADD_SPACER_THRESHOLD_SEC:
             output_entries.append(('', {}))
         self.__wait_counter = 0
 
@@ -99,30 +99,30 @@
             output_entries.append(self.__buffer.popleft())  # for thread safety
 
         try:
             self._sink(output_entries)
         except (TypeError, RuntimeError):  # ignore Qt error on widget destruction at app exit
             pass
 
-    def red(self, text: str, **kwargs):
+    def red(self, text: str, **kwargs) -> None:
         """Print red log message."""
         self(text, _color='red', **kwargs)
 
-    def blue(self, text: str, **kwargs):
+    def blue(self, text: str, **kwargs) -> None:
         """Print blue log message."""
         self(text, _color='blue', **kwargs)
 
-    def cyan(self, text: str, **kwargs):
+    def cyan(self, text: str, **kwargs) -> None:
         """Print cyan log message."""
         self(text, _color='cyan', **kwargs)
 
-    def magenta(self, text: str, **kwargs):
+    def magenta(self, text: str, **kwargs) -> None:
         """Print magenta log message."""
         self(text, _color='magenta', **kwargs)
 
-    def green(self, text: str, **kwargs):
+    def green(self, text: str, **kwargs) -> None:
         """Print green log message."""
         self(text, _color='green', **kwargs)
 
-    def yellow(self, text: str, **kwargs):
+    def yellow(self, text: str, **kwargs) -> None:
         """Print yellow log message."""
         self(text, _color='yellow', **kwargs)
```

### Comparing `midiscripter-0.2/midiscripter/metronome/metronome_port.py` & `midiscripter-0.3/midiscripter/metronome/metronome_port.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import time
-from typing import Union
 
 import midiscripter.base.port_base
 import midiscripter.base.shared
 from midiscripter.base.msg_base import Msg
 from midiscripter.base.port_base import Output
 from midiscripter.logger import log
 
@@ -24,49 +23,49 @@
         except ValueError:
             self.bpm = bpm
 
         self.msg_to_send = msg_to_send
         self.msg_to_send.source = self
 
         self.attached_passthrough_outs: list[Output] = []
-        """[`Output`][midiscripter.Output] ports attached 
+        """[`Output`][midiscripter.base.port_base.Output] ports attached 
            as pass-through ports to send metronome messages"""
 
     @property
     def bpm(self) -> float:
         """Message sending interval in beats per minute."""
         return 60 / self.__interval_sec
 
     @bpm.setter
-    def bpm(self, bpm: float):
+    def bpm(self, bpm: float) -> None:
         self.__interval_sec = 60 / bpm
 
-    def passthrough_out(self, output: Output):
+    def passthrough_out(self, output: Output) -> None:
         """Attach output port as a pass-through port to send metronome messages.
         The output port should be compatible to send messages.
 
         Args:
-            output: [`Output`][midiscripter.Output] port to use for pass-through
+            output: [`Output`][midiscripter.base.port_base.Output] port to use for pass-through
         """
         if output not in self.attached_passthrough_outs:
             self.attached_passthrough_outs.append(output)
             log('{input} input will pass through {output}', input=self, output=output)
 
-    def _open(self):
+    def _open(self) -> None:
         self.is_enabled = True
         midiscripter.base.shared.thread_executor.submit(self.__send_clicks_worker)
         log(f'Started metronome at {self.bpm} bpm')
 
-    def __send_clicks_worker(self):
+    def __send_clicks_worker(self) -> None:
         while self.is_enabled:
             time.sleep(self.__interval_sec)
             self.msg_to_send.ctime = midiscripter.base.shared.precise_epoch_time()
 
             for output in self.attached_passthrough_outs:
                 output.send(self.msg_to_send)
 
             self._send_input_msg_to_calls(self.msg_to_send)
 
         log(f'Stopped metronome at {self.bpm} bpm')
 
-    def _close(self):
+    def _close(self) -> None:
         self.is_enabled = False
```

### Comparing `midiscripter-0.2/midiscripter/midi/midi_msg.py` & `midiscripter-0.3/midiscripter/midi/midi_msg.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING
 from collections.abc import Sequence
 
 import rtmidi.midiconstants
 
 import midiscripter.base.msg_base
 
 if TYPE_CHECKING:
+    from collections.abc import Container
     from midiscripter.midi.midi_port import MidiIn
 
 
 class MidiType(midiscripter.base.msg_base.AttrEnum):
     """MIDI message type enumerator to use as [`MidiMsg`][midiscripter.MidiMsg] `type` attribute."""
 
     NOTE_ON = 'NOTE_ON'
@@ -37,23 +38,30 @@
     __match_args__: tuple[str] = ('type', 'channel', 'data1', 'data2')
 
     type: MidiType
     channel: int | tuple[int] | tuple[int, int, int]
     data1: int | tuple[int, int]
     data2: int | tuple[int, ...]
     combined_data: int | tuple[int, ...]
-    source: Optional['MidiIn']
+    source: 'None | MidiIn'
 
     def __new__(cls, *args, **kwargs):
         if args and isinstance(args[0], tuple) or not args and 'combined_data' in kwargs:
             return SysexMsg.__new__(SysexMsg, *args, **kwargs)
         else:
             return ChannelMsg.__new__(ChannelMsg, *args, **kwargs)
 
-    def matches(self, type=None, channel=None, data1=None, data2=None) -> bool:
+    def matches(
+        self,
+        type: 'None | Container[MidiType] | MidiType' = None,
+        channel: 'None | Container[ int | tuple[int] | tuple[int, int, int] ] | \
+                 int | tuple[int] | tuple[int, int, int]' = None,
+        data1: 'None | Container[int | tuple[int, int]] | int | tuple[int, int]' = None,
+        data2: 'None | Container[int | tuple[int, ...]] | int | tuple[int, ...]' = None,
+    ) -> bool:
         return super().matches(type, channel, data1, data2)
 
 
 class ChannelMsg(MidiMsg):
     """Channel voice/mode MIDI message. The most common MIDI message."""
 
     type: MidiType
@@ -76,22 +84,22 @@
     def __init__(
         self,
         type: MidiType = MidiType.CONTROL_CHANGE,
         channel: int = 1,
         data1: int = 0,
         data2: int = 127,
         *,
-        source: Optional['MidiIn'] = None,
+        source: 'None | MidiIn' = None,
     ):
         """
         Args:
             type: MIDI message type.
             channel: MIDI message channel
             data1: First data byte: note, control, program or aftertouch value
-            depending on MIDI message type
+                   depending on MIDI message type
             data2: Second data byte: velocity, value depending on MIDI message type
             source (MidiIn): The [`MidiIn`][midiscripter.MidiIn] instance that generated the message
         """
         super().__init__(type, source)
         self.channel = channel
         self.data1 = data1
         self.data2 = data2
@@ -99,38 +107,38 @@
     @property
     def combined_data(self) -> int | tuple[int, ...]:
         """Both data bytes combined to 14-bit number:
         pitch value for pitch bend MIDI message (0-16383)."""
         return self.data1 | (self.data2 << 7)
 
     @combined_data.setter
-    def combined_data(self, combined_data_value: int | Sequence[int]):
+    def combined_data(self, combined_data_value: int | Sequence[int]) -> None:
         self.data1 = combined_data_value & 0x7F
         self.data2 = combined_data_value >> 7
 
 
 class SysexMsg(MidiMsg):
     """System exclusive MIDI message"""
 
     type = MidiType.SYSEX
     """MIDI message type."""
 
-    channel: tuple[int] | tuple[int, int, int]
+    channel: tuple[int, ...]
     """Manufacturer ID (protocol)."""
 
-    data1: tuple[int, int]
+    data1: tuple[int, ...]
     """Sub ID (model, device, command, etc.)."""
 
     data2: tuple[int, ...]
     """Message data."""
 
     def __new__(cls, *args, **kwargs):
         return object.__new__(SysexMsg)
 
-    def __init__(self, combined_data: tuple[int, ...], *, source: Optional['MidiIn'] = None):
+    def __init__(self, combined_data: tuple[int, ...], *, source: 'None | MidiIn' = None):
         """
         Args:
             combined_data: Whole sysex message including opening (`240`) and closing (`247`) bytes
             source (MidiIn): The [`MidiIn`][midiscripter.MidiIn] instance that generated the message
         """
         midiscripter.base.msg_base.Msg.__init__(self, MidiType.SYSEX, source)
         self.combined_data = combined_data
@@ -152,31 +160,37 @@
             *self.channel,
             *self.data1,
             *self.data2,
             rtmidi.midiconstants.END_OF_EXCLUSIVE,
         )
 
     @combined_data.setter
-    def combined_data(self, combined_data: Sequence[int]):
+    def combined_data(self, combined_data: Sequence[int]) -> None:
         if (
             combined_data[0] != rtmidi.midiconstants.SYSTEM_EXCLUSIVE
             or combined_data[-1] != rtmidi.midiconstants.END_OF_EXCLUSIVE
         ):
             raise AttributeError(
                 'Sysex message should start with 240 (0xF0) and end with 247 (0xF7)'
             )
 
-        # combined_data[0] is sysex status byte
-        sub_id_start_index = 4 if combined_data[1] == 0 else 2
-        data_start_index = sub_id_start_index + 2
-        manufacturer = tuple(combined_data[1:sub_id_start_index])
+        payload_data = combined_data[1:-1]  # without opening and closing bytes
+
+        if payload_data[0] == 0:  # 3 int manufacturer
+            channel_len = 3
+        elif payload_data[0] in (126, 127):  # universal
+            channel_len = 2
+        else:  # 1 int manufacturer
+            channel_len = 1
+
+        sub_id_len = 2
 
-        if len(combined_data) < data_start_index + 1:  # +1 for closing 247 byte
+        minimal_valid_msg_len = 1 + channel_len + sub_id_len + 1
+        if len(combined_data) < minimal_valid_msg_len:
             raise AttributeError(
-                f'Sysex message for manufacturer {manufacturer} '
-                f'should be at least {data_start_index + 1} ints '
-                f'starting with 240 and ending with 247'
+                f'This sysex message should be at least {minimal_valid_msg_len} ints '
+                f'starting with 240 and ending with 247, it has only {len(combined_data)}'
             )
 
-        self.channel = manufacturer
-        self.data1 = tuple(combined_data[sub_id_start_index:data_start_index])
-        self.data2 = tuple(combined_data[data_start_index:-1])  # sysex end byte excluded
+        self.channel = tuple(payload_data[0:channel_len])
+        self.data1 = tuple(payload_data[channel_len : channel_len + sub_id_len])
+        self.data2 = tuple(payload_data[channel_len + sub_id_len :])
```

### Comparing `midiscripter-0.2/midiscripter/midi/midi_note_data.py` & `midiscripter-0.3/midiscripter/midi/midi_note_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-from typing import Union
 
 _NOTE_NAMES = {
     'Cb': -1,
     'C': 0,
     'C#': 1,
     'Db': 1,
     'D': 2,
```

### Comparing `midiscripter-0.2/midiscripter/midi/midi_port.py` & `midiscripter-0.3/midiscripter/midi/midi_port.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import TYPE_CHECKING, Optional, Union
+import platform
 from collections.abc import Callable
+from typing import TYPE_CHECKING
 
 import rtmidi
 import rtmidi.midiconstants
 
 import midiscripter.base.port_base
 from midiscripter.logger import log
 from midiscripter.midi.midi_msg import MidiType
 
 if TYPE_CHECKING:
     from midiscripter.midi.midi_msg import MidiMsg
 
-
 BYTE_TO_TYPE_MAP = {
     rtmidi.midiconstants.NOTE_ON: MidiType.NOTE_ON,
     rtmidi.midiconstants.NOTE_OFF: MidiType.NOTE_OFF,
     rtmidi.midiconstants.PITCH_BEND: MidiType.PITCH_BEND,
     rtmidi.midiconstants.PROGRAM_CHANGE: MidiType.PROGRAM_CHANGE,
     rtmidi.midiconstants.CONTROLLER_CHANGE: MidiType.CONTROL_CHANGE,
     rtmidi.midiconstants.POLY_PRESSURE: MidiType.POLYTOUCH,
@@ -31,103 +31,125 @@
     MidiType.POLYTOUCH: 3,
     MidiType.PITCH_BEND: 3,
     MidiType.AFTERTOUCH: 2,
     MidiType.PROGRAM_CHANGE: 2,
 }
 
 
+def _get_available_midi_port_names(
+    rtmidi_port_class: type[rtmidi.MidiIn | rtmidi.MidiOut],
+) -> list[str]:
+    raw_port_names = rtmidi_port_class().get_ports()
+    persistent_port_names = [port_name[: port_name.rfind(' ')] for port_name in raw_port_names]
+
+    if platform.system() == 'Windows':
+        return persistent_port_names
+    else:
+        port_names_without_prefixes = [
+            port_name[port_name.find(':') + 1 :] for port_name in persistent_port_names
+        ]
+        return port_names_without_prefixes
+
+
 class _MidiPortMixin(midiscripter.base.port_base.Port):
     # Attrs provided by the class that inherits from MidiPortMixin
     is_enabled: bool
     _available_names: list[str]
+    _is_virtual = False
 
     # noinspection PyMissingConstructor
     def __init__(self, port_name: str, input_callback: Callable | None = None):
         self.__port_name = port_name
 
         if input_callback:
-            self.__rtmidi_port = rtmidi.MidiIn()
-            self.__rtmidi_port.ignore_types(sysex=False)
-            self.__rtmidi_port.set_callback(input_callback)
+            self._rtmidi_port = rtmidi.MidiIn()
+            self._rtmidi_port.ignore_types(sysex=False)
+            self._rtmidi_port.set_callback(input_callback)
         else:
-            self.__rtmidi_port = rtmidi.MidiOut()
+            self._rtmidi_port = rtmidi.MidiOut()
 
     @property
     def _is_available(self) -> bool:
         """Port is available and can be opened."""
         return self.__port_name in self._available_names
 
-    def _open(self):
-        if self.__rtmidi_port.is_port_open():
+    def _open(self) -> None:
+        if self._rtmidi_port.is_port_open():
+            self.is_enabled = True
             return
 
         try:
             port_index = self._available_names.index(self.__port_name)
-            self.__rtmidi_port.open_port(port_index)
+            self._rtmidi_port.open_port(port_index)
             self.is_enabled = True
             log('Opened {port}', port=self)
         except ValueError:
-            log.red("Can't find port {port}. Check the port name.", port=self)
+            if platform.system() == 'Windows':
+                log.red("Can't find port {port}. Check the port name.", port=self)
+            else:
+                self._rtmidi_port.open_virtual_port(self.__port_name)
+                self._is_virtual = True
+                self.is_enabled = True
+                log('Created and opened virtual port {port}', port=self)
         except Exception:
             log.red('Failed to open {port}', port=self)
 
-    def _close(self):
-        if not self.__rtmidi_port.is_port_open():
+    def _close(self) -> None:
+        if not self._rtmidi_port.is_port_open():
             return
 
         try:
-            self.__rtmidi_port.close_port()
-            self.__rtmidi_port.delete()
+            self._rtmidi_port.close_port()
+            self._rtmidi_port.delete()
             self.is_enabled = False
             log('Closed {port}', port=self)
         except Exception:
             log.red('Failed to close {port}', port=self)
 
 
 class MidiIn(_MidiPortMixin, midiscripter.base.port_base.Input):
     """MIDI input port. Produces [`MidiMsg`][midiscripter.MidiMsg] objects."""
 
-    _available_names: list[str] = [
-        port_name[: port_name.rfind(' ')] for port_name in rtmidi.MidiIn().get_ports()
-    ]
+    _available_names: list[str] = _get_available_midi_port_names(rtmidi.MidiIn)
 
     def __init__(self, port_name: str):
         """
         Args:
             port_name: MIDI input port name
         """
         _MidiPortMixin.__init__(self, port_name, self.__callback)
         midiscripter.base.port_base.Input.__init__(self, port_name)
 
         self.attached_passthrough_outs: list['MidiOut'] = []
-        """[`MidiOut`][midiscripter.MidiOut] ports attached as pass-through ports 
+        """[`MidiOut`][midiscripter.MidiOut] ports attached as pass-through ports
         which will send all incoming messages as soon as they arrive before sending them to calls"""
 
-    def passthrough_out(self, midi_output: 'MidiOut'):
-        """Attach [`MidiOut`][midiscripter.MidiOut] as a pass-through port to send all incoming messages
-        as soon as they arrive, before sending them to calls. This can greatly reduce latency.
+    def passthrough_out(self, midi_output: 'MidiOut') -> None:
+        """Attach [`MidiOut`][midiscripter.MidiOut] as a pass-through port
+        to send all incoming messages as soon as they arrive,
+        before sending them to calls. This can greatly reduce latency.
 
         Args:
             midi_output: [`MidiOut`][midiscripter.MidiOut] port to use for pass-through
         """
         if midi_output not in self.attached_passthrough_outs:
             self.attached_passthrough_outs.append(midi_output)
             log('{input} input will pass through {output}', input=self, output=midi_output)
 
-    def __callback(self, rt_midi_input: tuple[tuple[hex, ...], float], _):
+    def __callback(self, rt_midi_input: tuple[tuple[hex, ...], float], _: list) -> None:
         if not self.is_enabled:
             return
 
         rt_midi_data, _ = rt_midi_input
         [output._passthrough_send(rt_midi_data) for output in self.attached_passthrough_outs]
         self._send_input_msg_to_calls(self.__convert_to_msg(rt_midi_data))
 
     def __convert_to_msg(
         self, rt_midi_data: tuple[hex, ...]
-    ) -> Union['midiscripter.midi.midi_msg.ChannelMsg', 'midiscripter.midi.midi_msg.SysexMsg']:
+    ) -> 'midiscripter.midi.midi_msg.ChannelMsg | midiscripter.midi.midi_msg.SysexMsg':
         if (
             rt_midi_data[0] == rtmidi.midiconstants.SYSTEM_EXCLUSIVE
             and rt_midi_data[-1] == rtmidi.midiconstants.END_OF_EXCLUSIVE
         ):
             return midiscripter.midi.midi_msg.SysexMsg(rt_midi_data, source=self)
 
         elif rt_midi_data[0] < rtmidi.midiconstants.SYSTEM_EXCLUSIVE:
@@ -141,17 +163,15 @@
         else:
             log.red(f'Unsupported MIDI msg type byte: {rt_midi_data[0]}')
 
 
 class MidiOut(_MidiPortMixin, midiscripter.base.port_base.Output):
     """MIDI output port. Sends [`MidiMsg`][midiscripter.MidiMsg] objects."""
 
-    _available_names: list[str] = [
-        port_name[: port_name.rfind(' ')] for port_name in rtmidi.MidiOut().get_ports()
-    ]
+    _available_names: list[str] = _get_available_midi_port_names(rtmidi.MidiOut)
 
     def __init__(self, port_name: str):
         """
         Args:
             port_name: MIDI output port name
         """
         _MidiPortMixin.__init__(self, port_name)
@@ -159,25 +179,33 @@
 
     def send(self, msg: 'MidiMsg') -> None:
         """Send the MIDI message.
 
         Args:
             msg: object to send
         """
-        with self._check_and_log_sent_message(msg):
-            if msg.type == MidiType.SYSEX:
-                rt_midi_output = msg.combined_data
-            else:
-                status_byte = (TYPE_TO_BYTE_MAP[msg.type] & 0xF0) | (msg.channel - 1 & 0xF)
-                msg_raw_data = status_byte, msg.data1, msg.data2
-                rt_midi_output = [msg_raw_data][: TYPE_TO_DATA_BYTES_COUNT[msg.type]]
+        if not self._validate_msg_send(msg):
+            return
+
+        if msg.type == MidiType.SYSEX:
+            rt_midi_output = msg.combined_data
+        else:
+            status_byte = (TYPE_TO_BYTE_MAP[msg.type] & 0xF0) | (msg.channel - 1 & 0xF)
+            msg_raw_data = status_byte, msg.data1, msg.data2
+            rt_midi_output = msg_raw_data[: TYPE_TO_DATA_BYTES_COUNT[msg.type]]
+
+        try:
+            self._rtmidi_port.send_message(rt_midi_output)
+        except Exception:
+            # For _rtmidi.SystemError: MidiOutWinMM::sendMessage: error sending MIDI message
+            log.red(f'Failed to send message: {msg}')
+            return
 
-            self.__rtmidi_port.send_message(rt_midi_output)
+        self._log_msg_sent(msg)
 
-    def _passthrough_send(self, rt_midi_data: tuple[hex, hex, hex]):
+    def _passthrough_send(self, rt_midi_data: tuple[hex, hex, hex]) -> None:
         if self.is_enabled:
             try:
-                self.__rtmidi_port.send_message(rt_midi_data)
-            except (
-                Exception
-            ):  # _rtmidi.SystemError: MidiOutWinMM::sendMessage: error sending MIDI message.
+                self._rtmidi_port.send_message(rt_midi_data)
+            except Exception:
+                # For _rtmidi.SystemError: MidiOutWinMM::sendMessage: error sending MIDI message
                 log.red(f'Failed to send message data: {rt_midi_data}')
```

### Comparing `midiscripter-0.2/midiscripter/midi/midi_ports_update.py` & `midiscripter-0.3/midiscripter/midi/midi_ports_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self.is_enabled = True
         midiscripter.base.shared.thread_executor.submit(self.__updater_worker)
         midiscripter.logger.log('Started MIDI ports change watcher')
 
     def _close(self) -> None:
         self.is_enabled = False
 
-    def __updater_worker(self):
+    def __updater_worker(self) -> None:
         while self.is_enabled:
             time.sleep(self.REFRESH_RATE_SEC)
 
             current_inputs = self.__dummy_midi_input.get_ports()
             current_outputs = self.__dummy_midi_output.get_ports()
 
             if (
```

### Comparing `midiscripter-0.2/midiscripter/osc/osc_port.py` & `midiscripter-0.3/midiscripter/osc/osc_port.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Union
-
 import pythonosc.osc_server
 import pythonosc.udp_client
 
 import midiscripter.base.port_base
 import midiscripter.base.shared
 import midiscripter.osc.osc_msg
 from midiscripter.logger import log
@@ -38,38 +36,39 @@
         Args:
             listener_ip_port: 'ip:port' or local port to listen for incoming OSC messages
         """
         super().__init__(listener_ip_port)
         self.listener_ip_address, self.listener_port = _parse_ip_port(listener_ip_port)
         self.__dispatcher = None
 
-    def __osc_server_msg_handler(self, address: str, *data):
+    def __osc_server_msg_handler(self, address: str, *data) -> None:
         if not self.is_enabled:
             return
 
         if len(data) == 1:
             data = data[0]
         input_msg = OscMsg(address, data, source=self)
         self._send_input_msg_to_calls(input_msg)
 
-    def _open(self):
+    def _open(self) -> None:
         if self.__dispatcher:
+            self.is_enabled = True
             return
 
         self.__dispatcher = pythonosc.osc_server.Dispatcher()
         self.__dispatcher.set_default_handler(self.__osc_server_msg_handler)
         self._osc_server = pythonosc.osc_server.BlockingOSCUDPServer(
             (self.listener_ip_address, self.listener_port), self.__dispatcher
         )
 
         midiscripter.base.shared.thread_executor.submit(self._osc_server.serve_forever)
         self.is_enabled = True
         log('Opened {input}', input=self)
 
-    def _close(self):
+    def _close(self) -> None:
         self._osc_server.shutdown()
         self.is_enabled = False
         log('Stopped {input}', input=self)
 
 
 class OscOut(midiscripter.base.port_base.Output):
     """Open Sound Control output port. Sends [`OscMsg`][midiscripter.OscMsg] objects."""
@@ -80,16 +79,20 @@
             target_ip_port: 'ip:port' or local port to send output OSC messages to
         """
         super().__init__(target_ip_port)
         target_ip_address, target_port = _parse_ip_port(target_ip_port)
         self._osc_client = pythonosc.udp_client.SimpleUDPClient(target_ip_address, target_port)
         self.is_enabled = True
 
-    def send(self, msg: OscMsg):
+    def send(self, msg: OscMsg) -> None:
         """Send the OSC message
 
         Args:
             msg: object to send
         """
-        with self._check_and_log_sent_message(msg):
-            data = list(msg.data) if isinstance(msg.data, tuple) else msg.data
-            self._osc_client.send_message(msg.address, data)
+        if not self._validate_msg_send(msg):
+            return
+
+        data = list(msg.data) if isinstance(msg.data, tuple) else msg.data
+        self._osc_client.send_message(msg.address, data)
+
+        self._log_msg_sent(msg)
```

### Comparing `midiscripter-0.2/midiscripter/osc/osc_query_maker.py` & `midiscripter-0.3/midiscripter/osc/osc_query_maker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import queue
-from typing import Union
 
 from midiscripter.logger import log
 from midiscripter.osc.osc_msg import OscMsg
 from midiscripter.osc.osc_port import OscIn, OscOut
 
 
 class OscQueryMaker:
```

### Comparing `midiscripter-0.2/midiscripter/resources/icon.ico` & `midiscripter-0.3/midiscripter/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `midiscripter-0.2/midiscripter/resources/icon.svg` & `midiscripter-0.3/midiscripter/resources/icon.svg`

 * *Files identical despite different names*

### Comparing `midiscripter-0.2/LICENSE` & `midiscripter-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `midiscripter-0.2/README.md` & `midiscripter-0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,103 @@
 # MIDI Scripter
 
-MIDI Scripter is a framework for scripting MIDI, keyboard and Open Sound Control (OSC) input and output with a few lines of Python code.
+MIDI Scripter is a framework for scripting MIDI, keyboard and Open Sound
+Control (OSC) input and output with only a few lines of Python code.
 
-MIDI Scripter is intended for digital audio workstation (DAW) controls scripting but can also be used for general input conversion and automation. It fits where controller mappings are not enough but rewriting DAW controller integration is too much. 
+MIDI Scripter listens to selected input ports and feed incoming messages to
+subscribed callables (functions, methods, etc.). These callables or any
+other Python code can send modified or brand-new messages with
+output ports. MIDI Scripter can act as a proxy to filter and transform and
+convert the input.
+
+MIDI Scripter included customizable GUI that provides messages logging,
+"ready to paste" port and message declarations and one line of code widgets for
+monitoring / controlling scripts.
 
 An octave transposer with GUI controls in 10 lines of code:
 
 ``` python
-from midiscripter import *  # safe * import with no bloat
+from midiscripter import *
 
-midi_keyboard = MidiIn('Port name')  # GUI will provide you with port names
-proxy_output = MidiOut('loopMIDI Port') # using loopMIDI virtual port for output
+midi_keyboard = MidiIn('MIDI Keyboard')  # GUI will provide you with port names
+proxy_output = MidiOut('To DAW')  # using virtual port for output
 
-# GUI control in a single line, many widget available, custom widgets supported
+# GUI control in a single line
 octave_selector = GuiButtonSelectorH(('-2', '-1', '0', '+1', '+2'), select='0')
 
 @midi_keyboard.subscribe  # decorated function will receive port's messages
 def transpose(msg: MidiMsg) -> None:
 	if msg.type == MidiType.NOTE_ON or msg.type == MidiType.NOTE_OFF:  # filter
 		msg.data1 += 12 * int(octave_selector.selected_item_text)  # modify
 		proxy_output.send(msg)  # route
 
 if __name__ == '__main__':  # combine multiple scripts by importing them
 	start_gui()  # opens helpful customizable GUI
 ```
 
-![Screenshot](https://github.com/Maboroshy/midi-scripter/blob/master/examples/octave_transposer/screenshot.png?raw=true)
+![Screenshot after some widget arrangement](https://github.com/Maboroshy/midi-scripter/blob/master/examples/octave_transposer/screenshot.png?raw=true)
 
-[Scripting guide and API documentation available](https://maboroshy.github.io/midi-scripter)
+[You can find more examples here.](https://github.com/Maboroshy/midi-scripter/tree/master/examples)
 
-Easy tasks for MIDI Scripter:  
-1. Filter, modify and route MIDI, OSC and keyboard messages in any way.  
-2. Map MIDI, OSC and keyboard to each other.  
-3. Map any Python code to input message.  
-4. Make extra "shift" keys to multiply MIDI controls.  
-5. Organize mappings into sets / scenes with GUI controls.  
-6. Make an extra overlay mappings on top of MIDI controller's default DAW integration by using proxy.  
-
-Complex tasks for MIDI Scripter:
-1. Create and map complex macros involving multiple hardware or virtual MIDI controllers.
-2. Make custom sequencer or MIDI input generator.
-3. Make music education ot trainer GUI application based on MIDI input.
+[Scripting guide and API documentation available.](https://maboroshy.github.io/midi-scripter)
 
-Currently MIDI Scripter is at "beta" development stage. It's fully functional but needs some more testing. It targets only Windows for now but Linux and macOS support will follow.
+Currently MIDI Scripter is at "beta" development stage. It's fully
+functional but needs more user feedback. It works on Windows and Linx and
+should work on macOS.
+
+## What it can do
+
+For writing Python code:
+
+- Prepare MIDI, OSC and keyboard inputs and outputs with a single line,
+  without boilerplate code.
+- Feed input messages to functions or any callables by "decorating" them.
+- Work with common message objects instead of raw data different for each port
+  type.
+- Send MIDI, OSC and keyboard output messages.
+- Create GUI widgets with one line and arrange them with mouse on your script's
+  dashboard.
+
+For live performance setups:
+
+- Make extra layers to multiply MIDI controls.
+- Organize mappings into sets / scenes with GUI dashboard.
+- Make an extra overlay mappings on top of MIDI controller's DAW integration by
+  using proxies.
+- Create and map complex macros.
+
+For MIDI related apps:
+
+- Make custom sequencers or MIDI output generators.
+- Make basic music training GUI applications based on MIDI input.
+
+For software control and automation:
+
+- Use MIDI controllers or keyboard shortcuts to run any Python code.
+- Use keyboard macros to control apps.
 
 ## Installation
-1. [Python 3.11+](https://www.python.org/downloads/) with "Add python.exe to PATH" option.
-2. [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) for virtual MIDI output ports on Windows.
-3. `pip install midiscripter` in console.
 
-## Setup
-Run loopMIDI and add virtual ports you want to send MIDI messages. You can enable its autostart option.
+1. Install [Python 3.11+](https://www.python.org/downloads/) including pip.
+2. Run `pip install midiscripter`.
 
-Enable virtual MIDI output ports as MIDI inputs in DAW. 
+Extra steps for Windows:
+
+1. Enable `Add python .exe to PATH` option in Python installer.
+2. Install [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html)
+   and set required virtual MIDI ports inside it.
 
 ## Quick Start
-1. Paste [script template](examples/script_template.py) to Python IDE or plain text editor. IDE is greatly recommended.
-2. Run unchanged template script from IDE or by `python .\script_template.py` to open GUI for more info on available ports and their input.
-3. Turn on the ports' checkboxes to enable them and watch the log for input messages.
-4. Click on port names and messages to copy their declarations to the clipboard. Paste the declarations to your script.
-5. Write the functions you need. Subscribe them to messages with `@input_port.subscribe` decorator. Use `log('messages')` for debugging. Use `output_port.send(msg)` to send modified or created messages from a function.
-6. Restart the script from GUI.
+
+1. Paste [script template](examples/script_template.py) to Python IDE or plain
+   text editor. IDE is greatly recommended.
+2. Run unaltered template script from IDE or by `python` command to open GUI for
+   more info on available ports and their input.
+3. Turn on available ports' checkboxes to enable them, and watch the log for
+   input messages.
+4. Click on port names and messages to copy their declarations to the clipboard.
+   Paste the declarations to your script.
+5. Write the functions you need. Subscribe them to input messages with
+   `@input_port.subscribe` decorator. Use `log('messages')` for debugging.
+   Use `output_port.send(msg)` to send modified or created messages from a
+   function.
+6. Restart the script from GUI to check how in works.
```

### Comparing `midiscripter-0.2/pyproject.toml` & `midiscripter-0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'midiscripter'
-version = '0.2'
+version = '0.3'
 description = 'Framework for scripting MIDI, keyboard and Open Sound Control input and output'
 readme = 'README.md'
 requires-python = '>=3.11'
 license = {file = "LICENSE"}
 keywords = ['MIDI', 'OSC', 'script', 'automation', 'input']
 authors = [{name = 'Maboroshy'}]
 classifiers = [
   'Development Status :: 4 - Beta',
-  'Programming Language :: Python',
   'Programming Language :: Python :: 3.11',
   'Programming Language :: Python :: 3.12',
-  'Programming Language :: Python :: Implementation :: CPython',
   'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
-  'Operating System :: Microsoft :: Windows',
   'Topic :: Multimedia :: Sound/Audio',
   'Topic :: Multimedia :: Sound/Audio :: MIDI',
   'Topic :: Software Development :: Libraries :: Python Modules',
 ]
 dependencies = [
   'colorama ~=0.4',  # BSD
   'python-rtmidi ~=1.5',  # MIT
@@ -30,14 +27,15 @@
   'pynput ~=1.7',  # LGPL
   'watchdog ~=4.0',  # Apache
   'PySide6_Essentials >6.4, <6.7',  # LGPL Got broken Signal.connect on 6.7
   'pywin32; platform_system == "Windows"',  # BSD
 ]
 
 [project.optional-dependencies]
+dev = ['ruff']
 doc = [
   'mkdocs-material',
   'mkdocstrings',
   'griffe-inherited-docstrings',
 ]
 
 [tool.hatch.build.targets.sdist]
@@ -51,12 +49,13 @@
 Issues = 'https://github.com/Maboroshy/midi-scripter/issues'
 Source = 'https://github.com/Maboroshy/midi-scripter'
 
 [tool.ruff]
 line-length = 100
 
 [tool.ruff.lint]
-select = ['B', 'C', 'E', 'F', 'PERF', 'TCH', 'SIM', 'UP']
+select = ['B', 'C', 'E', 'F', 'PERF', 'TCH', 'SIM', 'UP', 'ANN001',
+  'ANN201', 'ANN202', ]
 ignore = ['E501', 'F401', 'F405', 'F403', 'SIM105']
 
 [tool.ruff.format]
 quote-style = 'single'
```

### Comparing `midiscripter-0.2/PKG-INFO` & `midiscripter-0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: midiscripter
-Version: 0.2
+Version: 0.3
 Summary: Framework for scripting MIDI, keyboard and Open Sound Control input and output
 Project-URL: Documentation, https://maboroshy.github.io/midi-scripter
 Project-URL: Issues, https://github.com/Maboroshy/midi-scripter/issues
 Project-URL: Source, https://github.com/Maboroshy/midi-scripter
 Author: Maboroshy
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -171,92 +171,131 @@
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 License-File: LICENSE
 Keywords: MIDI,OSC,automation,input,script
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Requires-Dist: colorama~=0.4
 Requires-Dist: pynput~=1.7
 Requires-Dist: pyside6-essentials<6.7,>6.4
 Requires-Dist: python-osc~=1.7
 Requires-Dist: python-rtmidi~=1.5
 Requires-Dist: pywin32; platform_system == 'Windows'
 Requires-Dist: watchdog~=4.0
+Provides-Extra: dev
+Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: griffe-inherited-docstrings; extra == 'doc'
 Requires-Dist: mkdocs-material; extra == 'doc'
 Requires-Dist: mkdocstrings; extra == 'doc'
 Description-Content-Type: text/markdown
 
 # MIDI Scripter
 
-MIDI Scripter is a framework for scripting MIDI, keyboard and Open Sound Control (OSC) input and output with a few lines of Python code.
+MIDI Scripter is a framework for scripting MIDI, keyboard and Open Sound
+Control (OSC) input and output with only a few lines of Python code.
 
-MIDI Scripter is intended for digital audio workstation (DAW) controls scripting but can also be used for general input conversion and automation. It fits where controller mappings are not enough but rewriting DAW controller integration is too much. 
+MIDI Scripter listens to selected input ports and feed incoming messages to
+subscribed callables (functions, methods, etc.). These callables or any
+other Python code can send modified or brand-new messages with
+output ports. MIDI Scripter can act as a proxy to filter and transform and
+convert the input.
+
+MIDI Scripter included customizable GUI that provides messages logging,
+"ready to paste" port and message declarations and one line of code widgets for
+monitoring / controlling scripts.
 
 An octave transposer with GUI controls in 10 lines of code:
 
 ``` python
-from midiscripter import *  # safe * import with no bloat
+from midiscripter import *
 
-midi_keyboard = MidiIn('Port name')  # GUI will provide you with port names
-proxy_output = MidiOut('loopMIDI Port') # using loopMIDI virtual port for output
+midi_keyboard = MidiIn('MIDI Keyboard')  # GUI will provide you with port names
+proxy_output = MidiOut('To DAW')  # using virtual port for output
 
-# GUI control in a single line, many widget available, custom widgets supported
+# GUI control in a single line
 octave_selector = GuiButtonSelectorH(('-2', '-1', '0', '+1', '+2'), select='0')
 
 @midi_keyboard.subscribe  # decorated function will receive port's messages
 def transpose(msg: MidiMsg) -> None:
 	if msg.type == MidiType.NOTE_ON or msg.type == MidiType.NOTE_OFF:  # filter
 		msg.data1 += 12 * int(octave_selector.selected_item_text)  # modify
 		proxy_output.send(msg)  # route
 
 if __name__ == '__main__':  # combine multiple scripts by importing them
 	start_gui()  # opens helpful customizable GUI
 ```
 
-![Screenshot](https://github.com/Maboroshy/midi-scripter/blob/master/examples/octave_transposer/screenshot.png?raw=true)
+![Screenshot after some widget arrangement](https://github.com/Maboroshy/midi-scripter/blob/master/examples/octave_transposer/screenshot.png?raw=true)
 
-[Scripting guide and API documentation available](https://maboroshy.github.io/midi-scripter)
+[You can find more examples here.](https://github.com/Maboroshy/midi-scripter/tree/master/examples)
 
-Easy tasks for MIDI Scripter:  
-1. Filter, modify and route MIDI, OSC and keyboard messages in any way.  
-2. Map MIDI, OSC and keyboard to each other.  
-3. Map any Python code to input message.  
-4. Make extra "shift" keys to multiply MIDI controls.  
-5. Organize mappings into sets / scenes with GUI controls.  
-6. Make an extra overlay mappings on top of MIDI controller's default DAW integration by using proxy.  
-
-Complex tasks for MIDI Scripter:
-1. Create and map complex macros involving multiple hardware or virtual MIDI controllers.
-2. Make custom sequencer or MIDI input generator.
-3. Make music education ot trainer GUI application based on MIDI input.
+[Scripting guide and API documentation available.](https://maboroshy.github.io/midi-scripter)
 
-Currently MIDI Scripter is at "beta" development stage. It's fully functional but needs some more testing. It targets only Windows for now but Linux and macOS support will follow.
+Currently MIDI Scripter is at "beta" development stage. It's fully
+functional but needs more user feedback. It works on Windows and Linx and
+should work on macOS.
+
+## What it can do
+
+For writing Python code:
+
+- Prepare MIDI, OSC and keyboard inputs and outputs with a single line,
+  without boilerplate code.
+- Feed input messages to functions or any callables by "decorating" them.
+- Work with common message objects instead of raw data different for each port
+  type.
+- Send MIDI, OSC and keyboard output messages.
+- Create GUI widgets with one line and arrange them with mouse on your script's
+  dashboard.
+
+For live performance setups:
+
+- Make extra layers to multiply MIDI controls.
+- Organize mappings into sets / scenes with GUI dashboard.
+- Make an extra overlay mappings on top of MIDI controller's DAW integration by
+  using proxies.
+- Create and map complex macros.
+
+For MIDI related apps:
+
+- Make custom sequencers or MIDI output generators.
+- Make basic music training GUI applications based on MIDI input.
+
+For software control and automation:
+
+- Use MIDI controllers or keyboard shortcuts to run any Python code.
+- Use keyboard macros to control apps.
 
 ## Installation
-1. [Python 3.11+](https://www.python.org/downloads/) with "Add python.exe to PATH" option.
-2. [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) for virtual MIDI output ports on Windows.
-3. `pip install midiscripter` in console.
 
-## Setup
-Run loopMIDI and add virtual ports you want to send MIDI messages. You can enable its autostart option.
+1. Install [Python 3.11+](https://www.python.org/downloads/) including pip.
+2. Run `pip install midiscripter`.
 
-Enable virtual MIDI output ports as MIDI inputs in DAW. 
+Extra steps for Windows:
+
+1. Enable `Add python .exe to PATH` option in Python installer.
+2. Install [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html)
+   and set required virtual MIDI ports inside it.
 
 ## Quick Start
-1. Paste [script template](examples/script_template.py) to Python IDE or plain text editor. IDE is greatly recommended.
-2. Run unchanged template script from IDE or by `python .\script_template.py` to open GUI for more info on available ports and their input.
-3. Turn on the ports' checkboxes to enable them and watch the log for input messages.
-4. Click on port names and messages to copy their declarations to the clipboard. Paste the declarations to your script.
-5. Write the functions you need. Subscribe them to messages with `@input_port.subscribe` decorator. Use `log('messages')` for debugging. Use `output_port.send(msg)` to send modified or created messages from a function.
-6. Restart the script from GUI.
+
+1. Paste [script template](examples/script_template.py) to Python IDE or plain
+   text editor. IDE is greatly recommended.
+2. Run unaltered template script from IDE or by `python` command to open GUI for
+   more info on available ports and their input.
+3. Turn on available ports' checkboxes to enable them, and watch the log for
+   input messages.
+4. Click on port names and messages to copy their declarations to the clipboard.
+   Paste the declarations to your script.
+5. Write the functions you need. Subscribe them to input messages with
+   `@input_port.subscribe` decorator. Use `log('messages')` for debugging.
+   Use `output_port.send(msg)` to send modified or created messages from a
+   function.
+6. Restart the script from GUI to check how in works.
```

