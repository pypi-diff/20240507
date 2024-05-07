# Comparing `tmp/quickmq-1.0.1.tar.gz` & `tmp/quickmq-1.0.2.tar.gz`

## Comparing `quickmq-1.0.1.tar` & `quickmq-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,23 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quickmq-1.0.1/CONTRIBUTING
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 quickmq-1.0.1/requirements-dev.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 quickmq-1.0.1/requirements.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 quickmq-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 quickmq-1.0.1/docs/reqs-and-specs.md
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 quickmq-1.0.1/src/ssec_amqp/__about__.py
--rw-r--r--   0        0        0    10736 2020-02-02 00:00:00.000000 quickmq-1.0.1/src/ssec_amqp/__init__.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 quickmq-1.0.1/src/ssec_amqp/_defs.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 quickmq-1.0.1/src/ssec_amqp/_utils.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 quickmq-1.0.1/src/ssec_amqp/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quickmq-1.0.1/tests/test_api.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 quickmq-1.0.1/tests/test_client.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 quickmq-1.0.1/tests/test_exchange.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 quickmq-1.0.1/tests/test_utils.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 quickmq-1.0.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quickmq-1.0.1/README.md
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 quickmq-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 quickmq-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 quickmq-1.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 quickmq-1.0.2/CHANGELOG
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quickmq-1.0.2/CONTRIBUTING
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quickmq-1.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 quickmq-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 quickmq-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 quickmq-1.0.2/docs/reqs-and-specs.md
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 quickmq-1.0.2/src/ssec_amqp/__about__.py
+-rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 quickmq-1.0.2/src/ssec_amqp/__init__.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 quickmq-1.0.2/src/ssec_amqp/_defs.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 quickmq-1.0.2/src/ssec_amqp/_utils.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 quickmq-1.0.2/src/ssec_amqp/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quickmq-1.0.2/src/ssec_amqp/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quickmq-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 quickmq-1.0.2/tests/test_api.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 quickmq-1.0.2/tests/test_client.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 quickmq-1.0.2/tests/test_exchange.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 quickmq-1.0.2/tests/test_utils.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 quickmq-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 quickmq-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 quickmq-1.0.2/README.md
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 quickmq-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 quickmq-1.0.2/PKG-INFO
```

### Comparing `quickmq-1.0.1/docs/reqs-and-specs.md` & `quickmq-1.0.2/docs/reqs-and-specs.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 6. Handles lack of data for arbitrary amount of time, resumes without failure.
 7. Is able to handle SSEC AMQP message/topic definitions.
 8. Installable through pip.
 9. Handles switching server DNS aliases.
 
 ## Use Cases & User Stories
 
-As a user of the library, I want to be able to publish messages to a RabbitMQ exchange on remote servers.
-As a user of the library, I want to be able to publish messages to multiple servers at once.
-As a user of the library, I want to install the library from the python package index using pip.
-As a user of the library, I want to import it into my python program.
-As a user of the library at the SSEC, I want the library to support the SSEC's AMQP message/topic standards.
-As a user of the library, I want connection drops, server restarts, and DNS changes to not affect my code.
-As a user of the library, I want to be able to see the status of published messages to each server.
-As a user of the library, I want to be able to tune the verbosity of the logs of the library.
-As a developer of quickq, I don't want log messages to stdout/files, instead pass them to calling script.
-As a user of the library, I want to know when a connection is established successfully.
-As a user of the library, I want to know when connections to servers are reconnecting.
+- As a user of the library, I want to be able to publish messages to a RabbitMQ exchange on remote servers.
+- As a user of the library, I want to be able to publish messages to multiple servers at once.
+- As a user of the library, I want to install the library from the python package index using pip.
+- As a user of the library, I want to import it into my python program.
+- As a user of the library at the SSEC, I want the library to support the SSEC's AMQP message/topic standards.
+- As a user of the library, I want connection drops, server restarts, and DNS changes to not affect my code.
+- As a user of the library, I want to be able to see the status of published messages to each server.
+- As a user of the library, I want to be able to tune the verbosity of the logs of the library.
+- As a developer of quickq, I don't want log messages to stdout/files, instead pass them to calling script.
+- As a user of the library, I want to know when a connection is established successfully.
+- As a user of the library, I want to know when connections to servers are reconnecting.
 
 ## Security Requirements
 
 1. Don't expose passwords in logs or stacktraces.
 
 ## System Requirements
```

### Comparing `quickmq-1.0.1/src/ssec_amqp/__init__.py` & `quickmq-1.0.2/src/ssec_amqp/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,309 +1,342 @@
-import json
-from enum import Enum
-import logging
-from typing import Dict, List, Optional
-
-import amqp
-from amqp.exceptions import MessageNacked
-
-from ._utils import RetryInterval, catch_amqp_errors, NOTYET
-from ._defs import (
-    AMQP_EXCHANGE_ID_FORMAT,
-    DEFAULT_EXCHANGE,
-    DEFAULT_PASS,
-    DEFAULT_PORT,
-    DEFAULT_USER,
-    DEFAULT_VHOST,
-    DEFAULT_RECONNECT_WINDOW,
-)
-
-LOG = logging.getLogger("ssec_amqp")
-
-
-class DeliveryStatus(Enum):
-    """Enum for status of messages being delivered"""
-
-    # Message was acknowledged by the server.
-    DELIVERED = "delivered"
-    # Message was dropped due to reconnection.
-    DROPPED = "dropped"
-    # Message was rejected by the server.
-    REJECTED = "rejected"
-
-
-class AmqpExchange:
-    """Abstraction of an exchange on a AMQP server."""
-
-    def __init__(
-        self,
-        host: str,
-        user: Optional[str] = None,
-        password: Optional[str] = None,
-        exchange: Optional[str] = None,
-        vhost: Optional[str] = None,
-        port: Optional[int] = None,
-    ) -> None:
-        """Initialize the AmqpExchange.
-
-        Args:
-            host (str): where the exchange is
-            user (str): user to connect with
-            password (str): password to connect with
-            exchange (Optional[str], optional): name of the exchange. Defaults to None.
-            vhost (Optional[str], optional): vhost of the exchange. Defaults to None.
-            port (Optional[int], optional): port to connect with. Defaults to None.
-        """
-        self.host = host
-        self.user = user or DEFAULT_USER
-        self.vhost = vhost or DEFAULT_VHOST
-        self.port = port or DEFAULT_PORT
-        self.exchange = exchange or DEFAULT_EXCHANGE
-        self.__password = password or DEFAULT_PASS
-
-        self.__conn = None
-        self.__chan = None
-        self.__chan_id = None
-
-    @property
-    def connected(self) -> bool:
-        return self.__conn is not None and self.__conn.connected
-
-    @property
-    def id(self) -> str:
-        return str(self)
-
-    @catch_amqp_errors
-    def connect(self) -> None:
-        """Connects the object to the AMQP exchange using the parameters supplied in constructor."""
-        if self.connected:
-            self.refresh()
-            return
-
-        self.__conn = amqp.Connection(
-            f"{self.host}:{self.port}",
-            userid=self.user,
-            password=self.__password,
-            confirm_publish=True,
-        )
-        self.__conn.connect()
-        self.__chan = self.__conn.channel(channel_id=self.__chan_id)
-        self.__chan_id = self.__chan.channel_id
-
-    @catch_amqp_errors
-    def produce(self, content_dict, route_key: Optional[str] = None) -> bool:
-        """Produce a message to the exchange
-
-        Args:
-            content_dict (JSON): The body of the message to produce.
-            key (Optional[str], optional): key to send with. Defaults to None.
-
-        Raises:
-            RuntimeError: If the AmqpExchange is not connected.
-            ConnectionError: If there is a problem with the connection when publishing.
-
-        Returns:
-            bool: Was the message delivered?
-        """
-        self.refresh()
-        content_json = json.dumps(content_dict)
-        route_key = route_key or ""
-        try:
-            self.__chan.basic_publish(
-                msg=amqp.Message(
-                    body=content_json,
-                    content_type="application/json",
-                    content_encoding="utf-8",
-                ),
-                exchange=self.exchange,
-                routing_key=route_key,
-            )
-            return True
-        except MessageNacked:
-            LOG.debug(f"{self} message was not delivered!")
-            return False
-        finally:
-            if self.__conn.connected and self.__chan is None or not self.__chan.is_open:
-                self.__chan = self.__conn.channel(channel_id=self.__chan_id)
-
-    @catch_amqp_errors
-    def refresh(self) -> None:
-        """Refresh the AMQP connection, assure that it is still connected."""
-        if self.__conn is None:
-            raise RuntimeError(
-                f"Must call connect() before performing this action on{self!r}!"
-            )
-        try:
-            self.__conn.heartbeat_tick()
-        except amqp.ConnectionForced:
-            self.connect()  # Try again on heartbeat misses
-
-    def close(self) -> None:
-        """Closes the connection to the AMQP exchange."""
-        if self.__conn is None:
-            return
-        self.__conn.collect()
-
-    def __hash__(self) -> int:
-        return hash(self.id)
-
-    def __repr__(self) -> str:
-        return AMQP_EXCHANGE_ID_FORMAT.format(
-            user=self.user,
-            host=self.host,
-            port=self.port,
-            vhost=self.vhost,
-            exchange=self.exchange,
-        )
-
-    def __eq__(self, __value: object) -> bool:
-        if not isinstance(__value, self.__class__):
-            return False
-        return (
-            __value.host == self.host
-            and __value.exchange == self.exchange
-            and __value.user == self.user
-            and __value.port == self.port
-            and __value.vhost == self.vhost
-        )
-
-
-# TODO: What to do when exchange disconnects?
-class AmqpClient:
-    """Client that manages multiple AmqpExchanges at once."""
-
-    def __init__(self, reconnect_window: Optional[float] = None) -> None:
-        """Initialize a AmqpClient.
-
-        Args:
-            reconnect_window (Optional[float], optional): How long an AmqpExchange
-            has to reconnect before an error is raised. Negative for infinite time.
-            Defaults to -1.
-        """
-        self.reconnect_window = reconnect_window or DEFAULT_RECONNECT_WINDOW
-
-        self._connected_pool: List[AmqpExchange] = []
-        self._reconnect_pool: Dict[AmqpExchange, RetryInterval] = {}
-
-    @property
-    def connections(self) -> Dict[str, str]:
-        self._refresh_pools()
-        d = {exch.id: "connected" for exch in self._connected_pool}
-        d.update({exch.id: "reconnecting" for exch in self._reconnect_pool})
-        return d
-
-    def connect(self, exchange: AmqpExchange) -> None:
-        """Connect this AmqpClient to an AmqpExchange
-
-        Args:
-            exchange (AmqpExchange): The AmqpExchange to connect to.
-
-        Raises:
-            ConnectionError: If it cannot connect to the exchange.
-        """
-        self._refresh_pools()  # Could raise a timeout error!
-        LOG.debug(f"Attempting to connect to {exchange}")
-
-        if exchange in self._connected_pool:
-            LOG.debug(f"Already connected to {exchange}, skipping...")
-            return
-
-        if exchange in self._reconnect_pool or not exchange.connected:
-            exchange.connect()
-
-        LOG.debug(f"Successfully connected to {exchange}")
-        self._to_connected(exchange)
-
-    def publish(
-        self, message, route_key: Optional[str] = None
-    ) -> Dict[str, DeliveryStatus]:
-        """Publish an AMQP message to all exchanges connected to this client.
-
-        Args:
-            message (JSONable): A JSON-able message to publish
-            route_key (Optional[str], optional): the route key to publish with. Defaults to None.
-
-        Returns:
-            Dict[str, DeliveryStatus]: The status of the publish to all exchanges connected to this client.
-        """
-        status = {}
-        self._refresh_pools()
-        for exchange in self._connected_pool:
-            try:
-                routable = exchange.produce(message, route_key)
-            except ConnectionError:
-                self._to_reconnect(exchange)
-            else:
-                status[exchange.id] = (
-                    DeliveryStatus.DELIVERED if routable else DeliveryStatus.REJECTED
-                )
-
-        # Set status as dropped for all reconnecting exchanges
-        status.update(
-            {exchange.id: DeliveryStatus.DROPPED for exchange in self._reconnect_pool}
-        )
-        return status
-
-    def disconnect(self, exchange: Optional[AmqpExchange] = None) -> None:
-        """Disconnect this AmqpClient from one or all exchanges.
-
-        Args:
-            exchange (Optional[AmqpExchange], optional): A specific exchange to disconnect from.
-            If none, disconnect from all exchanges. Defaults to None.
-        """
-        if exchange is not None:
-            exchange.close()
-            self._reconnect_pool.pop(exchange, None)
-            try:
-                self._connected_pool.remove(exchange)
-            except ValueError:
-                pass
-            return
-
-        for exchange in self._connected_pool:
-            exchange.close()
-        for exchange in self._reconnect_pool:
-            exchange.close()
-        self._reconnect_pool.clear()
-        self._connected_pool.clear()
-
-    def _to_reconnect(self, exchange: AmqpExchange) -> None:
-        """Move an exchange to reconnecting pool.
-
-        Args:
-            exchange (AmqpExchange): AmqpExchange to move.
-        """
-        if exchange in self._connected_pool:
-            self._connected_pool.remove(exchange)
-        LOG.info(f"Moving {exchange!r} to reconnect dict")
-        self._reconnect_pool[exchange] = RetryInterval(
-            exchange.connect,
-            self.reconnect_window,
-            (ConnectionError,),
-        )
-
-    def _to_connected(self, exchange: AmqpExchange) -> None:
-        """Move an exchange to connected pool.
-
-        Args:
-            exchange (AmqpExchange): AmqpExchange to move.
-        """
-        if exchange in self._reconnect_pool:
-            del self._reconnect_pool[exchange]
-        LOG.info(f"Moving {exchange!r} to connected list")
-        self._connected_pool.append(exchange)
-
-    def _refresh_pools(self) -> None:
-        """Refresh this client's pools. Checks if exchanges can reconnect."""
-        LOG.debug("Refreshing reconnect pool")
-        for exchange, reconnect in self._reconnect_pool.copy().items():
-            if reconnect() is NOTYET:
-                LOG.debug(f"{exchange} not yet ready to reconnect")
-            else:
-                LOG.debug(f"Moving {exchange!r} to be connected")
-                self._to_connected(exchange)
-        for exchange in self._connected_pool:
-            try:
-                exchange.refresh()
-            except ConnectionError:
-                LOG.debug(f"{exchange} is not connected!")
-                self._to_reconnect(exchange)
+import json
+import logging
+from contextlib import suppress
+from typing import Dict, Optional
+
+import amqp
+from amqp.exceptions import MessageNacked
+from strenum import StrEnum
+
+from ssec_amqp._defs import (
+    AMQP_EXCHANGE_ID_FORMAT,
+    DEFAULT_EXCHANGE,
+    DEFAULT_PASS,
+    DEFAULT_PORT,
+    DEFAULT_RECONNECT_WINDOW,
+    DEFAULT_USER,
+    DEFAULT_VHOST,
+    DEFUALT_ROUTE_KEY,
+    AMQPConnectionError,
+    StateError,
+)
+from ssec_amqp._utils import NOTYET, RetryInterval, catch_amqp_errors
+
+LOG = logging.getLogger("ssec_amqp")
+
+
+__all__ = [
+    "AmqpExchange",
+    "AmqpClient",
+    "DeliveryStatus",
+    "ConnectionStatus",
+]
+
+
+class DeliveryStatus(StrEnum):
+    """Enum for status of messages being delivered"""
+
+    # Message was acknowledged by the server.
+    DELIVERED = "DELIVERED"
+    # Message was dropped due to reconnection.
+    DROPPED = "DROPPED"
+    # Message was rejected by the server.
+    REJECTED = "REJECTED"
+
+
+class ConnectionStatus(StrEnum):
+    """Enum for status of exchange's connection"""
+
+    # Exchange is connected to the server
+    CONNECTED = "CONNECTED"
+
+    # Exchange is reconnecting to the server
+    RECONNECTING = "RECONNECTING"
+
+    # Exchange is disconnected from the server
+    DISCONNECTED = "DISCONNECTED"
+
+
+class AmqpExchange:
+    """Abstraction of an exchange on a AMQP server."""
+
+    def __init__(
+        self,
+        host: str,
+        user: Optional[str] = None,
+        password: Optional[str] = None,
+        exchange: Optional[str] = None,
+        vhost: Optional[str] = None,
+        port: Optional[int] = None,
+    ) -> None:
+        """Initialize the AmqpExchange.
+
+        Args:
+            host (str): where the exchange is
+            user (str): user to connect with
+            password (str): password to connect with
+            exchange (Optional[str], optional): name of the exchange. Defaults to None.
+            vhost (Optional[str], optional): vhost of the exchange. Defaults to None.
+            port (Optional[int], optional): port to connect with. Defaults to None.
+        """
+        self.host = host
+        self.user = user or DEFAULT_USER
+        self.vhost = vhost or DEFAULT_VHOST
+        self.port = port or DEFAULT_PORT
+        self.exchange = exchange or DEFAULT_EXCHANGE
+        self.__password = password or DEFAULT_PASS
+
+        # Ignore types for amqp module, as it is untyped itself.
+        self.__conn = amqp.Connection(
+            f"{self.host}:{self.port}",
+            userid=self.user,
+            password=self.__password,
+            confirm_publish=True,
+        )
+        self.__chan = None  # type: ignore
+        self.__chan_id = None
+
+    @property
+    def connected(self) -> bool:
+        status = self.__conn.connected
+        if status is None:
+            return False
+        return status
+
+    @property
+    def identifier(self) -> str:
+        return str(self)
+
+    def _channel_open(self) -> bool:
+        if not self.connected:
+            return False
+        return self.__chan is not None and self.__chan.is_open
+
+    @catch_amqp_errors
+    def connect(self) -> None:
+        """Connects the object to the AMQP exchange using the parameters supplied in constructor."""
+        if self.connected:
+            return
+
+        self.__conn.connect()  # type: ignore [attr-defined]
+        self.__chan = self.__conn.channel(channel_id=self.__chan_id)  # type: ignore [attr-defined]
+        self.__chan_id = self.__chan.channel_id  # type: ignore [attr-defined]
+
+    @catch_amqp_errors
+    def produce(self, content_dict, route_key: Optional[str] = None) -> bool:
+        """Produce a message to the exchange
+
+        Args:
+            content_dict (JSON): The body of the message to produce.
+            key (Optional[str], optional): key to send with. Defaults to None.
+
+        Raises:
+            AmqpConnectionError: If there is a problem with the connection when publishing.
+
+        Returns:
+            bool: Was the message delivered?
+        """
+        self.refresh()
+        content_json = json.dumps(content_dict)
+        route_key = route_key or DEFUALT_ROUTE_KEY
+        try:
+            self.__chan.basic_publish(  # type: ignore [attr-defined]
+                msg=amqp.Message(
+                    body=content_json,
+                    content_type="application/json",
+                    content_encoding="utf-8",
+                ),
+                exchange=self.exchange,
+                routing_key=route_key,
+            )
+        except MessageNacked:
+            LOG.debug("%s - message was not delivered!", str(self))
+            return False
+        else:
+            return True
+        finally:
+            if not self._channel_open():  # type: ignore [attr-defined]
+                self.__chan = self.__conn.channel(channel_id=self.__chan_id)  # type: ignore [attr-defined]
+
+    @catch_amqp_errors
+    def refresh(self) -> None:
+        """Refresh the AMQP connection, assure that it is still connected.
+
+        Raises:
+            StateError: If the exchange is not connected.
+        """
+        if self.__conn.connected is None:
+            raise StateError(action="refresh", state_info="call connect()")
+        try:
+            self.__conn.heartbeat_tick()
+        except amqp.ConnectionForced:
+            self.connect()  # Try again on heartbeat misses
+
+    def close(self) -> None:
+        """Closes the connection to the AMQP exchange."""
+        self.__conn.collect()
+
+    def __hash__(self) -> int:
+        return hash(self.identifier)
+
+    def __repr__(self) -> str:
+        return AMQP_EXCHANGE_ID_FORMAT.format(
+            user=self.user,
+            host=self.host,
+            port=self.port,
+            vhost=self.vhost,
+            exchange=self.exchange,
+        )
+
+    def __eq__(self, __value: object) -> bool:
+        if not isinstance(__value, self.__class__):
+            return False
+        return (
+            __value.host == self.host
+            and __value.exchange == self.exchange
+            and __value.user == self.user
+            and __value.port == self.port
+            and __value.vhost == self.vhost
+        )
+
+
+# TODO: What to do when exchange disconnects?
+class AmqpClient:
+    """Client that manages multiple AmqpExchanges at once."""
+
+    def __init__(self, reconnect_window: Optional[float] = None) -> None:
+        """Initialize a AmqpClient.
+
+        Args:
+            reconnect_window (Optional[float], optional): How long an AmqpExchange
+            has to reconnect before an error is raised. Negative for infinite time.
+            Defaults to -1.
+        """
+        self.reconnect_window = reconnect_window or DEFAULT_RECONNECT_WINDOW
+
+        self._connected_pool: list[AmqpExchange] = []
+        self._reconnect_pool: dict[AmqpExchange, RetryInterval] = {}
+
+    @property
+    def connections(self) -> Dict[str, str]:
+        self.refresh_pools()
+        d = {exch.identifier: ConnectionStatus.CONNECTED for exch in self._connected_pool}
+        d.update({exch.identifier: ConnectionStatus.RECONNECTING for exch in self._reconnect_pool})
+        return d
+
+    def connect(self, exchange: AmqpExchange) -> None:
+        """Connect this AmqpClient to an AmqpExchange
+
+        Args:
+            exchange (AmqpExchange): The AmqpExchange to connect to.
+
+        Raises:
+            ConnectionError: If it cannot connect to the exchange.
+        """
+        LOG.debug("Attempting to connect to %s", str(exchange))
+
+        if exchange in self._connected_pool:
+            LOG.debug("Already connected to %s, skipping...", str(exchange))
+            return
+
+        if exchange.connected:
+            exchange.refresh()
+            self._to_connected(exchange)
+            return
+
+        try:
+            exchange.connect()
+        except AMQPConnectionError:
+            self._to_reconnect(exchange)
+            LOG.info("Initial connection to %s failed, reconnecting", str(exchange))
+        else:
+            self._to_connected(exchange)
+            LOG.debug("Successfully connected to %s", str(exchange))
+
+        self.refresh_pools()  # Could raise a timeout error!
+
+    def publish(self, message, route_key: Optional[str] = None) -> Dict[str, str]:
+        """Publish an AMQP message to all exchanges connected to this client.
+
+        Args:
+            message (JSONable): A JSON-able message to publish
+            route_key (Optional[str], optional): the route key to publish with. Defaults to None.
+
+        Returns:
+            Dict[str, DeliveryStatus]: The status of the publish to all exchanges connected to this client.
+        """
+        status = {}
+        self.refresh_pools()
+        for exchange in self._connected_pool:
+            try:
+                routable = exchange.produce(message, route_key)
+            except AMQPConnectionError:
+                self._to_reconnect(exchange)
+            else:
+                status[exchange.identifier] = DeliveryStatus.DELIVERED if routable else DeliveryStatus.REJECTED
+
+        # Set status as dropped for all reconnecting exchanges
+        status.update({exchange.identifier: DeliveryStatus.DROPPED for exchange in self._reconnect_pool})
+        return status
+
+    def disconnect(self, exchange: Optional[AmqpExchange] = None) -> None:
+        """Disconnect this AmqpClient from one or all exchanges.
+
+        Args:
+            exchange (Optional[AmqpExchange], optional): A specific exchange to disconnect from.
+            If none, disconnect from all exchanges. Defaults to None.
+        """
+        if exchange is not None:
+            exchange.close()
+            self._reconnect_pool.pop(exchange, None)
+            with suppress(ValueError):
+                self._connected_pool.remove(exchange)
+            return
+
+        for exchange in self._connected_pool:
+            exchange.close()
+        for exchange in self._reconnect_pool:
+            exchange.close()
+        self._reconnect_pool.clear()
+        self._connected_pool.clear()
+
+    def _to_reconnect(self, exchange: AmqpExchange) -> None:
+        """Move an exchange to reconnecting pool.
+
+        Args:
+            exchange (AmqpExchange): AmqpExchange to move.
+        """
+        if exchange in self._connected_pool:
+            self._connected_pool.remove(exchange)
+        LOG.info("Moving %s to reconnect dict", str(exchange))
+        self._reconnect_pool[exchange] = RetryInterval(
+            exchange.connect,
+            self.reconnect_window,
+            (AMQPConnectionError,),
+        )
+
+    def _to_connected(self, exchange: AmqpExchange) -> None:
+        """Move an exchange to connected pool.
+
+        Args:
+            exchange (AmqpExchange): AmqpExchange to move.
+        """
+        if exchange in self._reconnect_pool:
+            del self._reconnect_pool[exchange]
+        LOG.info("Moving %s to connected list", str(exchange))
+        self._connected_pool.append(exchange)
+
+    def refresh_pools(self) -> None:
+        """Refresh this client's pools. Checks if exchanges can reconnect."""
+        LOG.debug("Refreshing reconnect pool")
+        for exchange, reconnect in self._reconnect_pool.copy().items():
+            if reconnect() is NOTYET:
+                LOG.debug("%s not yet ready to reconnect", str(exchange))
+            else:
+                LOG.debug("Moving %s to be connected", str(exchange))
+                self._to_connected(exchange)
+        for exchange in self._connected_pool:
+            try:
+                exchange.refresh()
+            except AMQPConnectionError:
+                LOG.debug("%s is not connected!", str(exchange))
+                self._to_reconnect(exchange)
```

### Comparing `quickmq-1.0.1/src/ssec_amqp/_utils.py` & `quickmq-1.0.2/src/ssec_amqp/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,47 +5,46 @@
 Internal utility classes/functions.
 """
 
 import time
 
 from amqp import Connection
 
+from ssec_amqp._defs import AMQPConnectionError, RetryTimeoutError
 
-class NotYet(object):
-    """Sentinal class for when a retry is not yet ready"""
 
-    pass
+class NotYet:
+    """Sentinal class for when a retry is not yet ready"""
 
 
 # Sentinal to use for RetryInterval
 NOTYET = NotYet()
 
 
 class RetryInterval:
     def __init__(self, action, total_interval: float, errors=(Exception)) -> None:
         self._init_time = time.time()
 
         self.action = action
         self.errors = errors
+        self.total_interval = total_interval
 
         if total_interval < 0:
             self._max_time = float("inf")
         else:
             self._max_time = self._init_time + total_interval
 
     def __call__(self) -> NotYet:
         cur_time = time.time()
 
         try:
             return self.action()
         except self.errors as e:
             if cur_time >= self._max_time:
-                raise TimeoutError(
-                    f"Action {self.action!r} could not complete on time!"
-                ) from e
+                raise RetryTimeoutError(self.total_interval) from e
             return NOTYET
 
 
 def catch_amqp_errors(func):
     """Utility decorator to catch all of Pika's AMQPConnectionError and
     raise them as built-in ConnectionError
 
@@ -53,10 +52,10 @@
         func (Callable): Function to decorate
     """
 
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Connection.recoverable_connection_errors as e:
-            raise ConnectionError("AMQP Connection Error") from e
+            raise AMQPConnectionError from e
 
     return wrapper
```

### Comparing `quickmq-1.0.1/tests/test_utils.py` & `quickmq-1.0.2/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from typing import Any, Optional
-import pytest
+from __future__ import annotations
 
-from pika.exceptions import AMQPConnectionError
+from typing import Any
 
-from ssec_amqp._utils import catch_amqp_errors
+import pytest
+from amqp.exceptions import RecoverableConnectionError
+from ssec_amqp._utils import AMQPConnectionError, catch_amqp_errors
 
 
-def mock_function(
-    to_return: Optional[Any] = None, to_raise: Optional[Exception] = None
-):
+def mock_function(to_return: Any | None = None, to_raise: Exception | None = None):
     if to_return is not None:
         return to_return
     if to_raise is not None:
         raise to_raise
     return None
 
 
 def test_catch_amqp_errors_no_error():
     rv = 5
     assert catch_amqp_errors(mock_function)(to_return=rv) == rv
 
 
 def test_catch_amqp_errors_amqp_error():
-    with pytest.raises(ConnectionError):
-        catch_amqp_errors(mock_function)(to_raise=AMQPConnectionError)
+    with pytest.raises(AMQPConnectionError):
+        catch_amqp_errors(mock_function)(to_raise=RecoverableConnectionError)
 
 
 def test_catch_amqp_errors_diff_error():
     err = TypeError
     with pytest.raises(err):
         catch_amqp_errors(mock_function)(to_raise=err)
```

### Comparing `quickmq-1.0.1/.gitignore` & `quickmq-1.0.2/.gitignore`

 * *Files identical despite different names*

