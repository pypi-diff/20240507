# Comparing `tmp/strledger-0.6.2.tar.gz` & `tmp/strledger-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strledger-0.6.2.tar", max compression
+gzip compressed data, was "strledger-0.7.0.tar", max compression
```

## Comparing `strledger-0.6.2.tar` & `strledger-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-23 09:34:52.502126 strledger-0.6.2/LICENSE
--rw-r--r--   0        0        0     1188 2024-04-23 12:41:53.731085 strledger-0.6.2/README.md
--rw-r--r--   0        0        0     1375 2024-04-30 09:08:33.374138 strledger-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      120 2024-04-30 09:08:37.476327 strledger-0.6.2/strledger/__init__.py
--rw-r--r--   0        0        0    10249 2024-04-30 09:08:11.685426 strledger-0.6.2/strledger/cli.py
--rw-r--r--   0        0        0     7066 2024-04-23 09:34:52.505980 strledger-0.6.2/strledger/core.py
--rw-r--r--   0        0        0        0 2024-04-23 09:34:52.506030 strledger-0.6.2/strledger/py.typed
--rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 strledger-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 09:34:52.502126 strledger-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1176 2024-05-07 09:21:50.097703 strledger-0.7.0/README.md
+-rw-r--r--   0        0        0     1405 2024-05-07 09:21:50.098181 strledger-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-07 09:21:50.098639 strledger-0.7.0/strledger/__init__.py
+-rw-r--r--   0        0        0    10505 2024-05-07 09:21:50.099037 strledger-0.7.0/strledger/cli.py
+-rw-r--r--   0        0        0     7836 2024-05-07 09:21:50.099451 strledger-0.7.0/strledger/core.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:34:52.506030 strledger-0.7.0/strledger/py.typed
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 strledger-0.7.0/PKG-INFO
```

### Comparing `strledger-0.6.2/LICENSE` & `strledger-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strledger-0.6.2/README.md` & `strledger-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   --help         Show this message and exit.
 
 Commands:
   app-info      Get Stellar app info.
   get-address   Get Stellar public address.
   sign-auth     Sign a base64-encoded soroban authorization...
   sign-tx       Sign a base64-encoded transaction envelope.
-  sign-tx-hash  Sign a hex encoded transaction hash.
+  sign-tx-hash  Sign a hex encoded hash.
   version       Get strledger version info.
 ```
 
 ## Library Usage
 
 ```python
 from strledger import get_default_client
```

### Comparing `strledger-0.6.2/pyproject.toml` & `strledger-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "strledger"
-version = "0.6.2"
+version = "0.7.0"
 description = "Sign Stellar Transaction with Ledger on the command line."
 authors = ["overcat <4catcode@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
-homepage = "https://github.com/overcat/strledger"
-repository = "https://github.com/overcat/strledger"
-documentation = "https://github.com/overcat/strledger"
+homepage = "https://github.com/lightsail-network/strledger"
+repository = "https://github.com/lightsail-network/strledger"
+documentation = "https://github.com/lightsail-network/strledger"
 keywords = ["stellar", "ledger"]
 include = ["strledger/py.typed", "LICENSE"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
```

### Comparing `strledger-0.6.2/strledger/cli.py` & `strledger-0.7.0/strledger/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -136,111 +136,108 @@
         echo_error(
             "Failed to parse XDR.\n"
             "Make sure to pass a valid base64-encoded transaction envelope.\n"
             "You can check whether the data you submitted is valid "
             "through XDR Viewer - https://laboratory.stellar.org/#xdr-viewer"
         )
         sys.exit(1)
+
     tx_hash = te.hash_hex()
     echo_normal(f"Network Passphrase: {network_passphrase}")
     echo_normal(f"Transaction Hash: {tx_hash}")
-    echo_normal("Please confirm this transaction on Ledger.")
+    echo_normal("Please confirm the transaction on Ledger.")
 
-    if hash_signing:
-        try:
-            signature = client.sign_transaction_hash(tx_hash, keypair_index)
-        except CommException as e:
-            if e.sw == SW.TX_HASH_SIGNING_MODE_NOT_ENABLED:
-                echo_error(
-                    "Hash signing is not enabled on this device.\n"
-                    "Please enable it on the device and try again."
-                )
-            elif e.sw == SW.DENY:
-                echo_error("The request to sign the transaction hash was denied.")
-                sys.exit(1)
-            else:
-                raise e
-        keypair = client.get_keypair(keypair_index=keypair_index)
-        decorated_signature = DecoratedSignature(keypair.signature_hint(), signature)
-        te.signatures.append(decorated_signature)
-    else:
-        try:
+    try:
+        if hash_signing:
+            signature = client.sign_hash(tx_hash, keypair_index)
+            keypair = client.get_keypair(keypair_index=keypair_index)
+            decorated_signature = DecoratedSignature(
+                keypair.signature_hint(), signature
+            )
+            te.signatures.append(decorated_signature)
+        else:
             assert isinstance(te, (TransactionEnvelope, FeeBumpTransactionEnvelope))
             client.sign_transaction(
                 transaction_envelope=te, keypair_index=keypair_index
             )
-        except CommException as e:
-            if e.sw == SW.DENY:
-                echo_error("The request to sign the transaction was denied.")
-            elif e.sw == SW.UNKNOWN_OP:
-                echo_error("The transaction contains unsupported operation(s).")
-            elif e.sw == SW.UNKNOWN_ENVELOPE_TYPE:
-                echo_error(
-                    "The transaction contains unsupported transaction envelope type."
-                )
-            else:
-                echo_error(f"Unknown exception, you can the problem here: {__issue__}")
-                raise
-            sys.exit(1)
+    except CommException as e:
+        if hash_signing and e.sw == SW.TX_HASH_SIGNING_MODE_NOT_ENABLED:
+            echo_error(
+                "Hash signing is not enabled on this device.\n"
+                "Please enable it on the device and try again."
+            )
+        elif e.sw == SW.DENY:
+            echo_error("The request to sign the transaction was denied.")
+        elif e.sw == SW.SW_REQUEST_DATA_TOO_LARGE:
+            echo_error(
+                "The request data is too large, please try to sign a smaller transaction, or sign the hash only."
+            )
+        else:
+            echo_error(
+                f"Unknown exception, you can report the problem here: {__issue__}"
+            )
+            raise
+        sys.exit(1)
 
     echo_success("Signed successfully.")
     echo_success("Base64-encoded signed transaction envelope:")
     echo_success(te.to_xdr())
+
     if submit:
         echo_normal("Submitting to the network...")
         server = Server(horizon_url)
         try:
             server.submit_transaction(te)
         except BaseRequestError as e:
-            echo_error("submit failed, error info:")
+            echo_error("Submit failed, error info:")
             echo_error(e)
             sys.exit(1)
 
-        echo_success(f"Successfully submitted.")
+        echo_success("Successfully submitted.")
         if network_passphrase == Network.PUBLIC_NETWORK_PASSPHRASE:
             url = f"https://stellar.expert/explorer/public/tx/{tx_hash}"
         elif network_passphrase == Network.TESTNET_NETWORK_PASSPHRASE:
             url = f"https://stellar.expert/explorer/testnet/tx/{tx_hash}"
         else:
             url = urljoin(horizon_url, f"/transactions/{tx_hash}")
         echo_success(f"Stellar Explorer: {url}")
 
 
-@cli.command(name="sign-tx-hash")
+@cli.command(name="sign-hash")
 @click.option(
     "-i",
     "--keypair-index",
     type=int,
     required=False,
     help="Keypair Index.",
     default=DEFAULT_KEYPAIR_INDEX,
     show_default=True,
 )
-@click.argument("transaction_hash")
+@click.argument("hash")
 @click.pass_obj
-def sign_transaction_hash(
+def sign_hash(
     get_client: Callable[[], StrLedger],
-    transaction_hash: str,
+    hash: str,
     keypair_index: int,
 ):
-    """Sign a hex encoded transaction hash."""
+    """Sign a hex encoded hash."""
     client = get_client()
     try:
-        signature = client.sign_transaction_hash(transaction_hash, keypair_index)
+        signature = client.sign_hash(hash, keypair_index)
     except CommException as e:
         if e.sw == SW.TX_HASH_SIGNING_MODE_NOT_ENABLED:
             echo_error(
                 "Hash signing is not enabled on this device.\n"
                 "Please enable it on the device and try again."
             )
         elif e.sw == SW.DENY:
             echo_error("The request to sign the transaction hash was denied.")
-            sys.exit(1)
         else:
             raise e
+        sys.exit(1)
     signature_base64 = base64.b64encode(signature).decode()
     echo_success(signature_base64)
 
 
 @cli.command(name="get-address")
 @click.option(
     "-i",
@@ -275,53 +272,73 @@
     "--keypair-index",
     type=int,
     required=False,
     help="Keypair Index.",
     default=DEFAULT_KEYPAIR_INDEX,
     show_default=True,
 )
+@click.option(
+    "-a",
+    "--hash-signing",
+    is_flag=True,
+    help="Only send the hash to the device for signing.",
+)
 @click.argument("soroban_authorization")
 @click.pass_obj
 def sign_soroban_authorization(
     get_client: Callable[[], StrLedger],
     keypair_index: int,
+    hash_signing: bool,
     soroban_authorization: str,
 ):
     """Sign a base64-encoded soroban authorization (HashIDPreimage)."""
     client = get_client()
     try:
         auth = HashIDPreimage.from_xdr(soroban_authorization)
     except Exception:
         echo_error(
             "Failed to parse XDR.\n"
             "Make sure to pass a valid base64-encoded soroban authorization."
         )
         sys.exit(1)
 
-    echo_normal(f"HashIDPreimage Hash: {sha256(auth.to_xdr_bytes()).hex()}")
-    echo_normal("Please confirm this transaction on Ledger.")
+    preimage_hash = sha256(auth.to_xdr_bytes()).hex()
+    echo_normal(f"HashIDPreimage Hash: {preimage_hash}")
+    echo_normal("Please confirm the Soroban authorization on Ledger.")
 
-    signature = None
     try:
-        signature = client.sign_soroban_authorization(auth, keypair_index=keypair_index)
-        echo_success("Signed successfully.")
-        echo_success("Base64-encoded signature:")
-        echo_success(base64.b64encode(signature).decode())
+        if hash_signing:
+            signature = client.sign_hash(preimage_hash, keypair_index)
+        else:
+            signature = client.sign_soroban_authorization(
+                auth, keypair_index=keypair_index
+            )
     except CommException as e:
-        if e.sw == SW.DENY:
-            echo_error("The request to sign the soroban auth was denied.")
-        elif e.sw == SW.UNKNOWN_ENVELOPE_TYPE:
+        if hash_signing and e.sw == SW.TX_HASH_SIGNING_MODE_NOT_ENABLED:
             echo_error(
-                "The transaction contains unsupported transaction envelope type."
+                "Hash signing is not enabled on this device.\n"
+                "Please enable it on the device and try again."
+            )
+        elif e.sw == SW.DENY:
+            echo_error("The request to sign the Soroban authorization was denied.")
+        elif e.sw == SW.SW_REQUEST_DATA_TOO_LARGE:
+            echo_error(
+                "The request data is too large, please try to sign a Soroban authorization, or sign the hash only."
             )
         else:
-            echo_error(f"Unknown exception, you can the problem here: {__issue__}")
+            echo_error(
+                f"Unknown exception, you can report the problem here: {__issue__}"
+            )
             raise
         sys.exit(1)
 
+    echo_success("Signed successfully.")
+    echo_success("Base64-encoded signature:")
+    echo_success(base64.b64encode(signature).decode())
+
 
 @cli.command(name="version")
 def version() -> None:
     """Get strledger version info."""
     echo_success(f"StrLedger Version: {strledger_version}")
     echo_success(f"Ledger Wallet Version: {ledger_wallet_version}")
     echo_success(f"Stellar SDK Version: {stellar_sdk_version}")
```

### Comparing `strledger-0.6.2/strledger/core.py` & `strledger-0.7.0/strledger/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import binascii
+import dataclasses
 from enum import IntEnum
 from typing import Optional, Union
 
 from ledgerwallet.client import LedgerClient
 from ledgerwallet.params import Bip32Path
 from ledgerwallet.transport import enumerate_devices
 from stellar_sdk import (
@@ -25,121 +26,126 @@
     "StrLedger",
 ]
 
 DEFAULT_KEYPAIR_INDEX = 0
 
 
 class Ins(IntEnum):
+    """Instruction enum for APDU commands."""
+
     GET_PK = 0x02
     SIGN_TX = 0x04
     GET_CONF = 0x06
-    SIGN_TX_HASH = 0x08
+    SIGN_HASH = 0x08
     SIGN_SOROBAN_AUTHORIZATION = 0x0A
 
 
 class P1(IntEnum):
+    """P1 parameter enum for APDU commands."""
+
     NONE = 0x00
     FIRST_APDU = 0x00
     MORE_APDU = 0x80
 
 
 class P2(IntEnum):
+    """P2 parameter enum for APDU commands."""
+
     NON_CONFIRM = 0x00
     CONFIRM = 0x01
     LAST_APDU = 0x00
     MORE_APDU = 0x80
 
 
 class SW(IntEnum):
-    # Status word for fail of transaction formatting.
-    TX_FORMATTING_FAIL = 0x6125
+    """Status Words enum for APDU responses.
+
+    See https://github.com/lightsail-network/app-stellar/blob/develop/docs/COMMANDS.md#status-words
+    """
+
     # Status word for denied by user.
     DENY = 0x6985
-    # Status word for either wrong Lc or minimum APDU lenght is incorrect.
-    WRONG_DATA_LENGTH = 0x6A87
-    # Status word for incorrect P1 or P2.
-    WRONG_P1P2 = 0x6B00
-    # Unknown stellar operation
-    UNKNOWN_OP = 0x6C24
-    # Unknown stellar operation
-    UNKNOWN_ENVELOPE_TYPE = 0x6C25
     # Status word for hash signing model not enabled.
     TX_HASH_SIGNING_MODE_NOT_ENABLED = 0x6C66
-    # Status word for unknown command with this INS.
-    INS_NOT_SUPPORTED = 0x6D00
-    # Status word for instruction class is different than CLA.
-    CLA_NOT_SUPPORTED = 0x6E00
-    # Status word for wrong response length (buffer too small or too big).
-    WRONG_RESPONSE_LENGTH = 0xB000
-    # Status word for fail to display address.
-    DISPLAY_ADDRESS_FAIL = 0xB002
-    # Status word for fail to display transaction hash.
-    DISPLAY_TRANSACTION_HASH_FAIL = 0xB003
-    # Status word for wrong transaction length.
-    WRONG_TX_LENGTH = 0xB004
-    # Status word for fail of transaction parsing.
-    TX_PARSING_FAIL = 0xB005
-    # Status word for fail of transaction hash.
-    TX_HASH_FAIL = 0xB006
-    # Status word for bad state.
-    BAD_STATE = 0xB007
-    # Status word for signature fail.
-    SIGNATURE_FAIL = 0xB008
-    # Status word for fail to check swap params
-    SWAP_CHECKING_FAIL = 0xB009
+    # Status word for data too large.
+    SW_REQUEST_DATA_TOO_LARGE = 0x6C67
     # Status word for success.
     OK = 0x9000
 
 
 class DeviceNotFoundException(Exception):
+    """Exception raised when no Ledger device is found."""
+
     pass
 
 
 def get_default_client() -> "StrLedger":
+    """Get the default Ledger client.
+
+    Returns:
+        StrLedger: The default Ledger client instance.
+
+    Raises:
+        DeviceNotFoundException: If no Ledger device is found.
+    """
     devices = enumerate_devices()
     if len(devices) == 0:
         raise DeviceNotFoundException
     client = LedgerClient(devices[0])
     return StrLedger(client)
 
 
+@dataclasses.dataclass
 class AppInfo:
-    def __init__(self, version: str, hash_signing_enabled: bool) -> None:
-        self.version = version
-        self.hash_signing_enabled = hash_signing_enabled
-
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, self.__class__):
-            return NotImplemented
-        return (
-            self.version == other.version
-            and self.hash_signing_enabled == other.hash_signing_enabled
-        )
+    """App configuration information."""
 
-    def __str__(self) -> str:
-        return f"AppConfiguration(version='{self.version}', hash_signing_enabled={self.hash_signing_enabled})"
+    version: str
+    """The version of the app."""
+    hash_signing_enabled: bool
+    """Whether hash signing is enabled."""
 
 
 class StrLedger:
+    """Stellar Ledger client class."""
+
     def __init__(self, client: LedgerClient) -> None:
+        """Initialize the Stellar Ledger client.
+
+        Args:
+            client (LedgerClient): The Ledger client instance.
+        """
         self.client = client
 
     def get_app_info(self) -> AppInfo:
+        """Get the app configuration information.
+
+        Returns:
+            AppInfo: The app configuration information.
+        """
         data = self.client.apdu_exchange(
             ins=Ins.GET_CONF, p1=P1.FIRST_APDU, p2=P2.LAST_APDU
         )
         hash_signing_enabled = bool(data[0])
         version = f"{data[1]}.{data[2]}.{data[3]}"
         return AppInfo(version=version, hash_signing_enabled=hash_signing_enabled)
 
     def get_keypair(
         self,
         keypair_index: int = DEFAULT_KEYPAIR_INDEX,
         confirm_on_device: bool = False,
     ) -> Keypair:
+        """Get the public key for the specified keypair index.
+
+        Args:
+            keypair_index (int): The keypair index (default is 0).
+            confirm_on_device (bool): Whether to confirm the action on the device (default is False).
+
+        Returns:
+            Keypair: The keypair instance.
+        """
         path = Bip32Path.build(f"44'/148'/{keypair_index}'")
         data = self.client.apdu_exchange(
             ins=Ins.GET_PK,
             data=path,
             p1=P1.NONE,
             p2=P2.CONFIRM if confirm_on_device else P2.NON_CONFIRM,
         )
@@ -147,44 +153,71 @@
         return keypair
 
     def sign_transaction(
         self,
         transaction_envelope: Union[TransactionEnvelope, FeeBumpTransactionEnvelope],
         keypair_index: int = DEFAULT_KEYPAIR_INDEX,
     ) -> None:
+        """Sign a transaction envelope.
+
+        Args:
+            transaction_envelope (Union[TransactionEnvelope, FeeBumpTransactionEnvelope]): The transaction envelope to sign.
+            keypair_index (int): The keypair index (default is 0).
+        """
         sign_data = transaction_envelope.signature_base()
         keypair = self.get_keypair(keypair_index=keypair_index)
 
         path = Bip32Path.build(f"44'/148'/{keypair_index}'")
         payload = path + sign_data
         signature = self._send_payload(Ins.SIGN_TX, payload)
         assert isinstance(signature, bytes)
         decorated_signature = DecoratedSignature(keypair.signature_hint(), signature)
         transaction_envelope.signatures.append(decorated_signature)
 
-    def sign_transaction_hash(
+    def sign_hash(
         self,
         transaction_hash: Union[str, bytes],
         keypair_index: int = DEFAULT_KEYPAIR_INDEX,
     ) -> bytes:
+        """Sign a transaction hash.
+
+        Args:
+            transaction_hash (Union[str, bytes]): The transaction hash to sign.
+            keypair_index (int): The keypair index (default is 0).
+
+        Returns:
+            bytes: The signature.
+        """
         if isinstance(transaction_hash, str):
             transaction_hash = binascii.unhexlify(transaction_hash)
         path = Bip32Path.build(f"44'/148'/{keypair_index}'")
         payload = path + transaction_hash
 
         data = self.client.apdu_exchange(
-            ins=Ins.SIGN_TX_HASH, data=payload, p1=P1.FIRST_APDU, p2=P2.LAST_APDU
+            ins=Ins.SIGN_HASH, data=payload, p1=P1.FIRST_APDU, p2=P2.LAST_APDU
         )
         return data
 
     def sign_soroban_authorization(
         self,
         soroban_authorization: Union[str, bytes, HashIDPreimage],
         keypair_index: int = DEFAULT_KEYPAIR_INDEX,
     ) -> bytes:
+        """Sign a Soroban authorization.
+
+        Args:
+            soroban_authorization (Union[str, bytes, HashIDPreimage]): The Soroban authorization to sign.
+            keypair_index (int): The keypair index (default is 0).
+
+        Returns:
+            bytes: The signature.
+
+        Raises:
+            ValueError: If the Soroban authorization type is invalid.
+        """
         if isinstance(soroban_authorization, str):
             soroban_authorization = HashIDPreimage.from_xdr(soroban_authorization)
         if isinstance(soroban_authorization, bytes):
             soroban_authorization = HashIDPreimage.from_xdr_bytes(soroban_authorization)
 
         if (
             soroban_authorization.type
@@ -196,14 +229,23 @@
         path = Bip32Path.build(f"44'/148'/{keypair_index}'")
         payload = path + soroban_authorization.to_xdr_bytes()
         signature = self._send_payload(Ins.SIGN_SOROBAN_AUTHORIZATION, payload)
         assert isinstance(signature, bytes)
         return signature
 
     def _send_payload(self, ins: Ins, payload) -> Optional[Union[int, bytes]]:
+        """Send a payload to the Ledger device.
+
+        Args:
+            ins (Ins): The instruction for the APDU command.
+            payload: The payload to send.
+
+        Returns:
+            Optional[Union[int, bytes]]: The response from the Ledger device.
+        """
         chunk_size = 255
         first = True
         while payload:
             if first:
                 p1 = P1.FIRST_APDU
                 first = False
             else:
```

### Comparing `strledger-0.6.2/PKG-INFO` & `strledger-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: strledger
-Version: 0.6.2
+Version: 0.7.0
 Summary: Sign Stellar Transaction with Ledger on the command line.
-Home-page: https://github.com/overcat/strledger
+Home-page: https://github.com/lightsail-network/strledger
 License: MIT
 Keywords: stellar,ledger
 Author: overcat
 Author-email: 4catcode@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -23,16 +23,16 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Typing :: Typed
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: ledgerwallet (>=0.4.0,<0.5.0)
 Requires-Dist: stellar-sdk (>=9,<10)
 Project-URL: Bug Tracker, https://github.com/lightsail-network/strledger/issues
-Project-URL: Documentation, https://github.com/overcat/strledger
-Project-URL: Repository, https://github.com/overcat/strledger
+Project-URL: Documentation, https://github.com/lightsail-network/strledger
+Project-URL: Repository, https://github.com/lightsail-network/strledger
 Description-Content-Type: text/markdown
 
 # strledger - Sign Stellar Transaction with Ledger on the command line.
 
 ![example](https://github.com/lightsail-network/strledger/blob/main/img/example.png)
 
 ## Installation
@@ -54,15 +54,15 @@
   --help         Show this message and exit.
 
 Commands:
   app-info      Get Stellar app info.
   get-address   Get Stellar public address.
   sign-auth     Sign a base64-encoded soroban authorization...
   sign-tx       Sign a base64-encoded transaction envelope.
-  sign-tx-hash  Sign a hex encoded transaction hash.
+  sign-tx-hash  Sign a hex encoded hash.
   version       Get strledger version info.
 ```
 
 ## Library Usage
 
 ```python
 from strledger import get_default_client
```

