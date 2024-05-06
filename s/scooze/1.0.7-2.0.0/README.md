# Comparing `tmp/scooze-1.0.7.tar.gz` & `tmp/scooze-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scooze-1.0.7.tar", max compression
+gzip compressed data, was "scooze-2.0.0.tar", max compression
```

## Comparing `scooze-1.0.7.tar` & `scooze-2.0.0.tar`

### file list

```diff
@@ -1,47 +1,43 @@
--rw-r--r--   0        0        0     1191 2024-04-03 21:52:55.892997 scooze-1.0.7/LICENSE
--rw-r--r--   0        0        0     2990 2024-04-03 21:52:55.892997 scooze-1.0.7/README.md
--rw-r--r--   0        0        0     2565 2024-04-03 21:52:55.892997 scooze-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 21:52:55.892997 scooze-1.0.7/src/scooze/__init__.py
--rw-r--r--   0        0        0       46 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/README.md
--rw-r--r--   0        0        0    18295 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/__init__.py
--rw-r--r--   0        0        0     3020 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/bulkdata.py
--rw-r--r--   0        0        0     5375 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/card.py
--rw-r--r--   0        0        0      354 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/deck.py
--rw-r--r--   0        0        0      993 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/utils.py
--rw-r--r--   0        0        0     3166 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/bulkdata.py
--rw-r--r--   0        0        0    29964 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/card.py
--rw-r--r--   0        0        0    14218 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/cardparts.py
--rw-r--r--   0        0        0    16435 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/catalogs.py
--rw-r--r--   0        0        0      482 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/config.py
--rw-r--r--   0        0        0        0 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/__init__.py
--rw-r--r--   0        0        0     1502 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/cli.py
--rw-r--r--   0        0        0     1738 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/delete.py
--rw-r--r--   0        0        0     1910 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/load/cards.py
--rw-r--r--   0        0        0     2420 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/load/decks.py
--rw-r--r--   0        0        0      319 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/run.py
--rw-r--r--   0        0        0     1446 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/setup/docker.py
--rw-r--r--   0        0        0      371 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/setup/local.py
--rw-r--r--   0        0        0      545 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/teardown/docker.py
--rw-r--r--   0        0        0      410 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/teardown/local.py
--rw-r--r--   0        0        0     6337 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/database/core.py
--rw-r--r--   0        0        0     4522 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/database/deck.py
--rw-r--r--   0        0        0      593 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/database/mongo.py
--rw-r--r--   0        0        0    15016 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/deck.py
--rw-r--r--   0        0        0     4601 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/deckpart.py
--rw-r--r--   0        0        0      681 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/enum.py
--rw-r--r--   0        0        0       44 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/errors.py
--rw-r--r--   0        0        0     1302 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/main.py
--rw-r--r--   0        0        0        0 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/models/__init__.py
--rw-r--r--   0        0        0    22935 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/models/card.py
--rw-r--r--   0        0        0    10971 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/models/cardparts.py
--rw-r--r--   0        0        0     4311 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/models/deck.py
--rw-r--r--   0        0        0     2737 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/models/utils.py
--rw-r--r--   0        0        0      592 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/mongo.py
--rw-r--r--   0        0        0        0 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/routers/__init__.py
--rw-r--r--   0        0        0     5527 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/routers/card.py
--rw-r--r--   0        0        0     3656 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/routers/cards.py
--rw-r--r--   0        0        0     3134 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/routers/deck.py
--rw-r--r--   0        0        0     2847 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/routers/decks.py
--rw-r--r--   0        0        0      281 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/static/index.html
--rw-r--r--   0        0        0    14609 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/utils.py
--rw-r--r--   0        0        0     4071 1970-01-01 00:00:00.000000 scooze-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1191 2024-05-06 22:45:58.706376 scooze-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2971 2024-05-06 22:45:58.706376 scooze-2.0.0/README.md
+-rw-r--r--   0        0        0     1769 2024-05-06 22:45:58.710376 scooze-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1747 2024-05-06 22:45:58.710376 scooze-2.0.0/src/scooze/__init__.py
+-rw-r--r--   0        0        0       46 2024-05-06 22:45:58.710376 scooze-2.0.0/src/scooze/api/README.md
+-rw-r--r--   0        0        0    17856 2024-05-06 22:45:58.710376 scooze-2.0.0/src/scooze/api/__init__.py
+-rw-r--r--   0        0        0     2623 2024-05-06 22:45:58.710376 scooze-2.0.0/src/scooze/api/bulkdata.py
+-rw-r--r--   0        0        0     5069 2024-05-06 22:45:58.710376 scooze-2.0.0/src/scooze/api/card.py
+-rw-r--r--   0        0        0      320 2024-05-06 22:45:58.710376 scooze-2.0.0/src/scooze/api/deck.py
+-rw-r--r--   0        0        0      993 2024-05-06 22:45:58.710376 scooze-2.0.0/src/scooze/api/utils.py
+-rw-r--r--   0        0        0     3127 2024-05-06 22:45:58.710376 scooze-2.0.0/src/scooze/bulkdata.py
+-rw-r--r--   0        0        0    23138 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/card.py
+-rw-r--r--   0        0        0     3373 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/cardlist.py
+-rw-r--r--   0        0        0    12089 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/cardparts.py
+-rw-r--r--   0        0        0    16749 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/catalogs.py
+-rw-r--r--   0        0        0     1141 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/config.py
+-rw-r--r--   0        0        0     1283 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/configs/logging_config.json
+-rw-r--r--   0        0        0       81 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/console/__init__.py
+-rw-r--r--   0        0        0     1411 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/console/cli.py
+-rw-r--r--   0        0        0     1729 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/console/commands/delete.py
+-rw-r--r--   0        0        0     3661 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/console/commands/load/cards.py
+-rw-r--r--   0        0        0     2501 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/console/commands/load/decks.py
+-rw-r--r--   0        0        0      514 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/console/commands/run.py
+-rw-r--r--   0        0        0     1645 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/console/commands/save/cards.py
+-rw-r--r--   0        0        0    17004 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/deck.py
+-rw-r--r--   0        0        0      872 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/enums.py
+-rw-r--r--   0        0        0       74 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/errors.py
+-rw-r--r--   0        0        0     1128 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/logger.py
+-rw-r--r--   0        0        0     1318 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/main.py
+-rw-r--r--   0        0        0      467 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/models/__init__.py
+-rw-r--r--   0        0        0    23423 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/models/card.py
+-rw-r--r--   0        0        0    10971 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/models/cardparts.py
+-rw-r--r--   0        0        0     4765 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/models/deck.py
+-rw-r--r--   0        0        0     2686 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/models/utils.py
+-rw-r--r--   0        0        0      592 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/mongo.py
+-rw-r--r--   0        0        0        0 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/routers/__init__.py
+-rw-r--r--   0        0        0     5741 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/routers/card.py
+-rw-r--r--   0        0        0     3742 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/routers/cards.py
+-rw-r--r--   0        0        0     4909 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/routers/deck.py
+-rw-r--r--   0        0        0     3721 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/routers/decks.py
+-rw-r--r--   0        0        0      405 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/static/index.html
+-rw-r--r--   0        0        0    17198 2024-05-06 22:45:58.714376 scooze-2.0.0/src/scooze/utils.py
+-rw-r--r--   0        0        0     4037 1970-01-01 00:00:00.000000 scooze-2.0.0/PKG-INFO
```

### Comparing `scooze-1.0.7/LICENSE` & `scooze-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scooze-1.0.7/README.md` & `scooze-2.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # scooze
 
-[![CI](https://img.shields.io/github/actions/workflow/status/arcavios/scooze/pytest.yml?branch=dev&logo=github&label=CI)](https://github.com/arcavios/scooze/actions?query=event%3Apush+branch%3Adev+workflow%3Apytest)
+[![CI](https://img.shields.io/github/actions/workflow/status/arcavios/scooze/ci.yml?branch=dev&logo=github&label=CI)](https://github.com/arcavios/scooze/actions?query=event%3Apush+branch%3Adev+workflow%3A%22Continuous+Integration%22)
 [![pypi](https://img.shields.io/pypi/v/scooze.svg)](https://pypi.python.org/pypi/scooze)
 [![versions](https://img.shields.io/pypi/pyversions/scooze.svg)](https://github.com/arcavios/scooze)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/arcavios/scooze/blob/dev/LICENSE)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
 
-A flexible data layer for applications working with Magic: the Gathering cards, decks, and tournaments.
+A flexible data layer for applications working with Magic: the Gathering cards and decks.
 
 ## Features
 
-📊 Robust data models for representing Magic: the Gathering cards, decks, and tournaments
+📊 Robust data models for representing Magic: the Gathering cards and decks
 
 - Cards - follows the Scryfall standard
 - Decks - main deck/sideboard/command zone, format legality, average words, and more
-- Tournaments - coming soon!
 
 🎛️ CLI to manage a local database of [Scryfall](https://scryfall.com/docs/api/bulk-data) data
 
 🐍 Python and REST APIs for interacting with the scooze database
 
 ## Help
 
-See our [documentation](https://scooze.readthedocs.io/en/latest) for more information.
+The source code can be found [here](https://github.com/arcavios/scooze).
+
+See our [documentation](https://scooze.readthedocs.io/en/stable/) for more information.
 
 ## Installation
 
-Install using `pip install scooze`. For more installation options, see the [Install](https://scooze.readthedocs.io/en/latest/installation) section in the documentation.
+Install using `pip install scooze`. For more installation options, see the [Install](https://scooze.readthedocs.io/en/stable/installation) section in the documentation.
 
 ## A Simple Example
 
 ``` python
-from scooze.card import Card
-from scooze.deck import Deck, InThe
-from scooze.catalogs import Format
+from scooze import Card, Deck, Format, InThe
 
 deck = Deck()
 card1 = Card("Python")
 card2 = Card("Anaconda")
 swamp = Card("Swamp")
 
 deck.add_card(card1, 25)
@@ -54,19 +53,19 @@
 15 Swamp
 
 Sideboard:
 100 Anaconda
 """
 ```
 
-See [Setup](https://scooze.readthedocs.io/en/latest/setup/) and our [API Documentation](https://scooze.readthedocs.io/en/latest/dataclasses/card/) for more details.
+See [Setup](https://scooze.readthedocs.io/en/stable/setup/) and our [API Documentation](https://scooze.readthedocs.io/en/stable/dataclasses/card/) for more details.
 
 ## Contributing
 
-For guidance on setting up a development environment and how to make a contribution to scooze, see [Contributing to scooze](https://scooze.readthedocs.io/en/latest/contributing).
+For guidance on setting up a development environment and how to make a contribution to scooze, see [Contributing to scooze](https://scooze.readthedocs.io/en/stable/contributing).
 
 ## Report a Bug
 
 If you find a bug 🐛 please open a [bug report](https://github.com/arcavios/scooze/issues/new?assignees=&labels=bug&template=bug_report.md&title=). If you have an idea for an improvement or new feature 🚀 please open a [feature request](https://github.com/arcavios/scooze/issues/new?assignees=&labels=enhancement&template=feature_request.md&title=).
 
 If you find a security vulnerability, please follow the instructions [here](https://github.com/arcavios/scooze/security/policy).
```

### Comparing `scooze-1.0.7/src/scooze/api/__init__.py` & `scooze-2.0.0/src/scooze/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from functools import cache
 from typing import Any
 
 import scooze.api.bulkdata as bulkdata_api
 import scooze.api.card as card_api
 from beanie import PydanticObjectId, init_beanie
 from scooze.api.utils import _check_for_safe_context, _safe_cache
-from scooze.card import CardT, FullCard
+from scooze.card import Card
 from scooze.catalogs import ScryfallBulkFile
 from scooze.config import CONFIG
 from scooze.models.card import CardModel
 from scooze.mongo import db, mongo_close, mongo_connect
 
 
 class ScoozeApi(AbstractContextManager):
@@ -24,16 +24,15 @@
             green_cards = s.get_cards_by("colors", [Color.GREEN])
             woe_cards = s.get_cards_by_set("woe")
             black_lotus = s.get_card_by_scryfall_id("b0faa7f2-b547-42c4-a810-839da50dadfe")
             print(black_lotus.total_words())
         ```
     """
 
-    def __init__(self, card_class: type[CardT] = FullCard):
-        self.card_class = card_class
+    def __init__(self):
         self.safe_context = False
 
     def __enter__(self):
         self.safe_context = True
         asyncio.get_event_loop().run_until_complete(mongo_connect())
         asyncio.get_event_loop().run_until_complete(
             init_beanie(database=db.client[CONFIG.mongo_db], document_models=[CardModel])
@@ -44,15 +43,15 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         asyncio.get_event_loop().run_until_complete(mongo_close())
 
     # region Card endpoints
 
     @_safe_cache
     @_check_for_safe_context
-    def get_card_by(self, property_name: str, value: Any) -> CardT:
+    def get_card_by(self, property_name: str, value: Any) -> Card:
         """
         Search the database for the first card that matches the given criteria.
 
         Args:
             property_name: The property to check.
             value: The value to match on.
 
@@ -60,26 +59,26 @@
             The first matching card, or None if none were found.
 
         Raises:
             RuntimeError: If used outside a `with` context.
         """
 
         return asyncio.get_event_loop().run_until_complete(
-            card_api.get_card_by(property_name=property_name, value=value, card_class=self.card_class)
+            card_api.get_card_by(property_name=property_name, value=value)
         )
 
     @_check_for_safe_context
     def get_cards_by(
         self,
         property_name: str,
         values: list[Any],
         paginated: bool = False,
         page: int = 1,
         page_size: int = 10,
-    ) -> list[CardT]:
+    ) -> list[Card]:
         """
         Search the database for cards matching the given criteria, with options for
         pagination.
 
         Args:
             property_name: The property to check.
             values: A list of values to match on.
@@ -95,26 +94,25 @@
             RuntimeError: If used outside a `with` context.
         """
 
         return asyncio.get_event_loop().run_until_complete(
             card_api.get_cards_by(
                 property_name=property_name,
                 values=values,
-                card_class=self.card_class,
                 paginated=paginated,
                 page=page,
                 page_size=page_size,
             )
         )
 
     # region Convenience methods for single-card lookup
 
     @cache
     @_check_for_safe_context
-    def get_card_by_name(self, name: str) -> CardT:
+    def get_card_by_name(self, name: str) -> Card:
         """
         Search the database for a card with the given name.
 
         Args:
             name: The card name to search for.
 
         Returns:
@@ -124,21 +122,20 @@
             RuntimeError: If used outside a `with` context.
         """
 
         return asyncio.get_event_loop().run_until_complete(
             card_api.get_card_by(
                 property_name="name",
                 value=name,
-                card_class=self.card_class,
             )
         )
 
     @cache
     @_check_for_safe_context
-    def get_card_by_oracle_id(self, oracle_id: str) -> CardT:
+    def get_card_by_oracle_id(self, oracle_id: str) -> Card:
         """
         Search the database for a card with the given Oracle ID.
 
         Args:
             oracle_id: The card [Oracle ID](https://scryfall.com/docs/api/cards) to search for.
 
         Returns:
@@ -148,21 +145,20 @@
             RuntimeError: If used outside a `with` context.
         """
 
         return asyncio.get_event_loop().run_until_complete(
             card_api.get_card_by(
                 property_name="oracle_id",
                 value=oracle_id,
-                card_class=self.card_class,
             )
         )
 
     @cache
     @_check_for_safe_context
-    def get_card_by_scryfall_id(self, scryfall_id: str) -> CardT:
+    def get_card_by_scryfall_id(self, scryfall_id: str) -> Card:
         """
         Search the database for a card with the given Scryfall ID.
 
         Args:
             scryfall_id: The card [Scryfall ID](https://scryfall.com/docs/api/cards) to search for.
 
         Returns:
@@ -172,24 +168,23 @@
             RuntimeError: If used outside a `with` context.
         """
 
         return asyncio.get_event_loop().run_until_complete(
             card_api.get_card_by(
                 property_name="scryfall_id",
                 value=scryfall_id,
-                card_class=self.card_class,
             )
         )
 
     # endregion
 
     # region Convenience methods for multiple card lookup
 
     @_check_for_safe_context
-    def get_cards_by_set(self, set_code: str) -> list[CardT]:
+    def get_cards_by_set(self, set_code: str) -> list[Card]:
         """
          Search the database for all cards in the given set.
          Expects the 3-letter [set code](https://en.wikipedia.org/wiki/List_of_Magic:_The_Gathering_sets)
          for a set (e.g. "CMD")
 
          Args:
              set_code: The set code to search for.
@@ -201,38 +196,37 @@
              RuntimeError: If used outside a `with` context.
         """
 
         return asyncio.get_event_loop().run_until_complete(
             card_api.get_cards_by(
                 property_name="set",
                 values=[set_code],
-                card_class=self.card_class,
             )
         )
 
     @_check_for_safe_context
-    def get_cards_all(self) -> list[CardT]:
+    def get_cards_all(self) -> list[Card]:
         """
         Get all cards from the database. WARNING: may be extremely large.
 
         Returns:
             A list of all cards in the database.
 
         Raises:
             RuntimeError: If used outside a `with` context.
         """
 
-        return asyncio.get_event_loop().run_until_complete(card_api.get_cards_all(self.card_class))
+        return asyncio.get_event_loop().run_until_complete(card_api.get_cards_all())
 
     # TODO(#146): add function get_cards_by_format (format, legality)
 
     # endregion
 
     @_check_for_safe_context
-    def add_card(self, card: CardT) -> PydanticObjectId:
+    def add_card(self, card: Card) -> PydanticObjectId:
         """
         Add a card to the database.
 
         Args:
             card: The card to insert.
 
         Returns:
@@ -241,15 +235,15 @@
         Raises:
             RuntimeError: If used outside a `with` context.
         """
 
         return asyncio.get_event_loop().run_until_complete(card_api.add_card(card=card))
 
     @_check_for_safe_context
-    def add_cards(self, cards: list[CardT]) -> list[PydanticObjectId]:
+    def add_cards(self, cards: list[Card]) -> list[PydanticObjectId]:
         """
         Add a list of cards to the database.
 
         Args:
             cards: The list of card to insert.
 
         Returns:
@@ -299,33 +293,33 @@
     # TODO(#145): add deck endpoints to python api
 
     # endregion
 
     # region Bulk data I/O
 
     @_check_for_safe_context
-    def load_card_file(self, file_type: ScryfallBulkFile, bulk_file_dir: str):
+    def load_card_file(self, file_type: ScryfallBulkFile, bulk_file_dir: str, show_progress: bool = True) -> int:
         """
         Loads the desired file from the given directory into a local database.
-        Attempts to download it from Scryfall if it isn't found.
 
         Args:
             file_type: The type of [ScryfallBulkFile](https://scryfall.com/docs/api/bulk-data)
                 to insert into the database.
             bulk_file_dir: The path to the folder containing the ScryfallBulkFile.
+            show_progress: Flag to log progress while loading a file.
+
+        Returns:
+            The total number of cards loaded into the database.
 
         Raises:
             RuntimeError: If used outside a `with` context.
         """
 
         return asyncio.get_event_loop().run_until_complete(
-            bulkdata_api.load_card_file(
-                file_type=file_type,
-                bulk_file_dir=bulk_file_dir,
-            )
+            bulkdata_api.load_card_file(file_type=file_type, bulk_file_dir=bulk_file_dir, show_progress=show_progress)
         )
 
     # endregion
 
 
 class AsyncScoozeApi(AbstractAsyncContextManager):
     """
@@ -339,16 +333,15 @@
             green_cards = await s.get_cards_by("colors", [Color.GREEN])
             woe_cards = await s.get_cards_by_set("woe")
             black_lotus = await s.get_card_by_scryfall_id("b0faa7f2-b547-42c4-a810-839da50dadfe")
             print(black_lotus.total_words())
         ```
     """
 
-    def __init__(self, card_class: type[CardT] = FullCard):
-        self.card_class = card_class
+    def __init__(self):
         self.safe_context = False
 
     async def __aenter__(self):
         self.safe_context = True
         await mongo_connect()
         await init_beanie(database=db.client[CONFIG.mongo_db], document_models=[CardModel])
 
@@ -357,40 +350,40 @@
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await mongo_close()
 
     # region Card endpoints
 
     @_safe_cache
     @_check_for_safe_context
-    async def get_card_by(self, property_name: str, value: Any) -> CardT:
+    async def get_card_by(self, property_name: str, value: Any) -> Card:
         """
         Search the database for the first card that matches the given criteria.
 
         Args:
             property_name: The property to check.
             value: The value to match on.
 
         Returns:
             The first matching card, or None if none were found.
 
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
-        return await card_api.get_card_by(property_name=property_name, value=value, card_class=self.card_class)
+        return await card_api.get_card_by(property_name=property_name, value=value)
 
     @_check_for_safe_context
     async def get_cards_by(
         self,
         property_name: str,
         values: list[Any],
         paginated: bool = False,
         page: int = 1,
         page_size: int = 10,
-    ) -> list[CardT]:
+    ) -> list[Card]:
         """
         Search the database for cards matching the given criteria, with options for
         pagination.
 
         Args:
             property_name: The property to check.
             values: A list of values to match on.
@@ -405,25 +398,24 @@
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
         return await card_api.get_cards_by(
             property_name=property_name,
             values=values,
-            card_class=self.card_class,
             paginated=paginated,
             page=page,
             page_size=page_size,
         )
 
     # region Convenience methods for single-card lookup
 
     @cache
     @_check_for_safe_context
-    async def get_card_by_name(self, name: str) -> CardT:
+    async def get_card_by_name(self, name: str) -> Card:
         """
         Search the database for a card with the given name.
 
         Args:
             name: The card name to search for.
 
         Returns:
@@ -432,20 +424,19 @@
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
         return await card_api.get_card_by(
             property_name="name",
             value=name,
-            card_class=self.card_class,
         )
 
     @cache
     @_check_for_safe_context
-    async def get_card_by_oracle_id(self, oracle_id: str) -> CardT:
+    async def get_card_by_oracle_id(self, oracle_id: str) -> Card:
         """
         Search the database for a card with the given Oracle ID.
 
         Args:
             oracle_id: The card [Oracle ID](https://scryfall.com/docs/api/cards) to search for.
 
         Returns:
@@ -454,20 +445,19 @@
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
         return await card_api.get_card_by(
             property_name="oracle_id",
             value=oracle_id,
-            card_class=self.card_class,
         )
 
     @cache
     @_check_for_safe_context
-    async def get_card_by_scryfall_id(self, scryfall_id: str) -> CardT:
+    async def get_card_by_scryfall_id(self, scryfall_id: str) -> Card:
         """
         Search the database for a card with the given Scryfall ID.
 
         Args:
             scryfall_id: The card [Scryfall ID](https://scryfall.com/docs/api/cards) to search for.
 
         Returns:
@@ -476,23 +466,22 @@
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
         return await card_api.get_card_by(
             property_name="scryfall_id",
             value=scryfall_id,
-            card_class=self.card_class,
         )
 
     # endregion
 
     # region Convenience methods for multiple card lookup
 
     @_check_for_safe_context
-    async def get_cards_by_set(self, set_code: str) -> list[CardT]:
+    async def get_cards_by_set(self, set_code: str) -> list[Card]:
         """
         Search the database for all cards in the given set.
         Expects the 3-letter [set code](https://en.wikipedia.org/wiki/List_of_Magic:_The_Gathering_sets)
         for a set (e.g. "CMD")
 
         Args:
             set_code: The set code to search for.
@@ -503,37 +492,36 @@
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
         return await card_api.get_cards_by(
             property_name="set",
             values=[set_code],
-            card_class=self.card_class,
         )
 
     @_check_for_safe_context
-    async def get_cards_all(self) -> list[CardT]:
+    async def get_cards_all(self) -> list[Card]:
         """
         Get all cards from the database. WARNING: may be extremely large.
 
         Returns:
             A list of all cards in the database.
 
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
-        return await card_api.get_cards_all(self.card_class)
+        return await card_api.get_cards_all()
 
     # TODO(#146): add function get_cards_by_format (format, legality)
 
     # endregion
 
     @_check_for_safe_context
-    async def add_card(self, card: CardT) -> PydanticObjectId:
+    async def add_card(self, card: Card) -> PydanticObjectId:
         """
         Add a card to the database.
 
         Args:
             card: The card to insert.
 
         Returns:
@@ -542,15 +530,15 @@
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
         return await card_api.add_card(card=card)
 
     @_check_for_safe_context
-    async def add_cards(self, cards: list[CardT]) -> list[PydanticObjectId]:
+    async def add_cards(self, cards: list[Card]) -> list[PydanticObjectId]:
         """
         Add a list of cards to the database.
 
         Args:
             cards: The list of card to insert.
 
         Returns:
@@ -600,27 +588,29 @@
     # TODO(#145): add deck endpoints to python api
 
     # endregion
 
     # region Bulk data I/O
 
     @_check_for_safe_context
-    async def load_card_file(self, file_type: ScryfallBulkFile, bulk_file_dir: str):
+    async def load_card_file(self, file_type: ScryfallBulkFile, bulk_file_dir: str, show_progress: bool = True) -> int:
         """
         Loads the desired file from the given directory into a local database.
-        Attempts to download it from Scryfall if it isn't found.
 
         Args:
             file_type: The type of [ScryfallBulkFile](https://scryfall.com/docs/api/bulk-data)
                 to insert into the database.
             bulk_file_dir: The path to the folder containing the ScryfallBulkFile.
+            show_progress: Flag to log progress while loading a file.
+
+        Returns:
+            The total number of cards loaded into the database.
 
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
         return await bulkdata_api.load_card_file(
-            file_type=file_type,
-            bulk_file_dir=bulk_file_dir,
+            file_type=file_type, bulk_file_dir=bulk_file_dir, show_progress=show_progress
         )
 
     # endregion
```

### Comparing `scooze-1.0.7/src/scooze/api/bulkdata.py` & `scooze-2.0.0/src/scooze/api/bulkdata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,59 @@
+from pathlib import Path
+
 import ijson
 from pydantic_core import ValidationError
-from scooze.bulkdata import download_bulk_data_file_by_type
 from scooze.catalogs import ScryfallBulkFile
+from scooze.console import logger as cli_logger
 from scooze.models.card import CardModel, CardModelData
 
 
-async def load_card_file(file_type: ScryfallBulkFile, bulk_file_dir: str) -> None:
+async def load_card_file(file_type: ScryfallBulkFile, bulk_file_dir: str, show_progress: bool = True) -> int:
     """
     Loads the desired file from the given directory into a local Mongo
-    database. Attempts to download it from Scryfall if it isn't found.
+    database.
 
     Args:
         file_type: The type of [ScryfallBulkFile](https://scryfall.com/docs/api/bulk-data)
         to insert into the database.
         bulk_file_dir: The path to the folder containing the ScryfallBulkFile.
+        show_progress: Flag to log progress while loading a file.
+
+    Returns:
+        The total number of cards loaded into the database.
     """
 
-    file_path = f"{bulk_file_dir}/{file_type}.json"
-    try:
-        print(f"Loading {file_type} file into the database...")
-        with open(file_path, "rb") as cards_file:
-            batch_size = 5000
-            current_batch_count = 0
-            results_count = 0
-            current_batch: list[CardModel] = []
-            card_jsons = ijson.items(cards_file, "item")
-
-            async def load_batch(batch: list[CardModel]) -> int:
-                batch_results = await CardModel.insert_many(batch)
-                if batch_results is not None:
-                    return len(batch_results.inserted_ids)
-                return 0
-
-            for card_json in card_jsons:
-                if (validated_card := _try_validate_card(card_json)) is not None:
-                    current_batch.append(validated_card)
-                    current_batch_count += 1
-                    if current_batch_count >= batch_size:
-                        results_count += await load_batch(current_batch)
-                        current_batch = []
-                        current_batch_count = 0
+    file_path = Path(bulk_file_dir) / f"{file_type}.json"
+    batch_size = 5000
+    current_batch_count = 0
+    results_count = 0
+    current_batch: list[CardModel] = []
+
+    with file_path.open(mode="rb") as cards_file:
+        card_jsons = ijson.items(cards_file, "item")
+
+        async def load_batch(batch: list[CardModel]) -> int:
+            batch_results = await CardModel.insert_many(batch)
+            if batch_results is not None:
+                return len(batch_results.inserted_ids)
+            return 0
+
+        for card_json in card_jsons:
+            if (validated_card := _try_validate_card(card_json)) is not None:
+                current_batch.append(validated_card)
+                current_batch_count += 1
+                if current_batch_count >= batch_size:
+                    results_count += await load_batch(current_batch)
+                    current_batch = []
+                    current_batch_count = 0
+                    if show_progress:
                         print(f"Finished processing {results_count} cards...", end="\r")
-            results_count += await load_batch(current_batch)
-
-            print(f"Loaded {results_count} cards to the database.")
+        results_count += await load_batch(current_batch)
 
-    except FileNotFoundError:
-        print(file_path)
-        download_now = input(f"{file_type} file not found; would you like to download it now? [y/N] ") in "yY"
-        if not download_now:
-            print("No cards loaded into database.")
-            return
-        download_bulk_data_file_by_type(file_type, bulk_file_dir)
-        await load_card_file(file_type, bulk_file_dir)
+    return results_count
 
 
 def _try_validate_card(card_json: dict) -> CardModel | None:
     """
     Attempt to convert a single card's JSON to a model for DB import, and
     report validation errors that arise in conversion.
 
@@ -65,13 +62,15 @@
 
     Returns:
         A validated model, or None if validation failed.
     """
 
     try:
         card = CardModelData.model_validate(card_json)
-        return CardModel.model_validate(card.model_dump(mode="json", by_alias=True))
+        return CardModel.model_validate(card.model_dump())
 
     except ValidationError as e:
-        print(f"Card with name {card_json['name']} not added due to validation error: \n{e}")
+        cli_logger.exception(
+            f"{card_json['name']} not loaded due to validation error.", exc_info=e, extra={"card": card_json}
+        )
 
         return
```

### Comparing `scooze-1.0.7/src/scooze/api/card.py` & `scooze-2.0.0/src/scooze/api/card.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,114 @@
 from typing import Any
 
 from beanie import PydanticObjectId
-from scooze.card import CardT, FullCard
+from scooze.card import Card
 from scooze.errors import BulkAddError
+from scooze.logger import logger
 from scooze.models.card import CardModel, CardModelData
-from scooze.utils import scooze_logger, to_lower_camel
-
-logger = scooze_logger()
+from scooze.utils import to_lower_camel
 
 
 def _normalize_for_ids(property_name: str, value, is_many: bool = False) -> tuple[str, Any | list[Any]]:
     match property_name:
         case "_id" | "id" | "scooze_id":
             prop_name = "_id"
             val = [PydanticObjectId(v) for v in value] if is_many else PydanticObjectId(value)
             return prop_name, val
         case _:
             return to_lower_camel(property_name), value
 
 
-async def get_card_by(property_name: str, value, card_class: CardT = FullCard) -> CardT:
+async def get_card_by(property_name: str, value: Any) -> Card:
     """
     Search the database for the first card that matches the given criteria.
 
     Args:
         property_name: The property to check.
         value: The value to match on.
-        card_class: The type of card to return.
 
     Returns:
         The first matching card, or None if none were found.
     """
 
     prop_name, val = _normalize_for_ids(property_name, value)
     card_model = await CardModel.find_one({prop_name: val})
 
     if card_model is not None:
-        return card_class.from_model(card_model)
+        return Card.from_model(card_model)
 
 
 async def get_cards_by(
     property_name: str,
     values: list[Any],
-    card_class: CardT = FullCard,
     paginated: bool = False,
     page: int = 1,
     page_size: int = 10,
-) -> list[CardT]:
+) -> list[Card]:
     """
     Search the database for cards matching the given criteria, with options for
     pagination.
 
     Args:
         property_name: The property to check.
         values: A list of values to match on.
-        card_class: The type of card object to return.
         paginated: Whether to paginate the results.
         page: The page to look at, if paginated.
         page_size: The size of each page, if paginated.
 
     Returns:
         A list of cards matching the search criteria, or empty list if none
         were found.
     """
 
     prop_name, vals = _normalize_for_ids(property_name, values)
     skip = (page - 1) * page_size if paginated else 0
     limit = page_size if paginated else None
     card_models = await CardModel.find({"$or": [{prop_name: v} for v in vals]}, skip=skip, limit=limit).to_list()
 
-    return [card_class.from_model(m) for m in card_models]
+    return [Card.from_model(m) for m in card_models]
 
 
-async def get_cards_all(card_class: CardT = FullCard) -> list[CardT]:
+async def get_cards_all() -> list[Card]:
     """
     Get all cards from the database. WARNING: may be extremely large.
 
     Returns:
         A list of all cards in the database.
     """
 
     card_models = await CardModel.find_all().to_list()
 
-    return [card_class.from_model(m) for m in card_models]
+    return [Card.from_model(m) for m in card_models]
 
 
-async def add_card(card: CardT) -> PydanticObjectId:
+async def add_card(card: Card) -> PydanticObjectId:
     """
     Add a card to the database.
 
     Assign the resulting database ID to the given Card.
 
     Args:
         card: The card to insert.
 
     Returns:
         The ID of the inserted card, or None if it was unable.
     """
 
     try:
         card_data = CardModelData.model_validate(card.__dict__)
-        card_model = CardModel.model_validate(card_data.model_dump(mode="json", by_alias=True))
+        card_model = CardModel.model_validate(card_data.model_dump())
         await card_model.create()
         card.scooze_id = card_model.id
         return card_model.id
     except Exception as e:
         logger.exception("Failed to add card.", extra={"card": card}, exc_info=e)
 
 
-async def add_cards(cards: list[CardT]) -> list[PydanticObjectId]:
+async def add_cards(cards: list[Card]) -> list[PydanticObjectId]:
     """
     Add a list of cards to the database.
 
     Assign the resulting database IDs to the given Cards.
 
     Args:
         cards: The list of cards to insert.
@@ -125,17 +121,15 @@
     """
 
     if not cards:
         return []
 
     try:
         card_models = [CardModelData.model_validate(card.__dict__) for card in cards]
-        cards_to_insert = [
-            CardModel.model_validate(card_model.model_dump(mode="json", by_alias=True)) for card_model in card_models
-        ]
+        cards_to_insert = [CardModel.model_validate(card_model.model_dump()) for card_model in card_models]
         insert_result = await CardModel.insert_many(cards_to_insert)
         card_ids = insert_result.inserted_ids
 
         if len(card_ids) != len(cards):
             # TODO(#202): Perform card lookups to get the ids of the cards that were successfully added.
             raise Exception()
         else:
```

### Comparing `scooze-1.0.7/src/scooze/api/utils.py` & `scooze-2.0.0/src/scooze/api/utils.py`

 * *Files identical despite different names*

### Comparing `scooze-1.0.7/src/scooze/bulkdata.py` & `scooze-2.0.0/src/scooze/bulkdata.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,58 @@
-import os
-from urllib.error import (  # TODO(#153): This allows for autolinking to the HTTPError documentation, but it's bloat, right?
-    HTTPError,
-)
+from pathlib import Path
+from urllib.error import HTTPError  # import HTTPError for linking in docs
 
 import requests
 from scooze.catalogs import ScryfallBulkFile
-from scooze.utils import DEFAULT_BULK_FILE_DIR
+from scooze.config import CONFIG
 
 SCRYFALL_BULK_INFO_ENDPOINT = "https://api.scryfall.com/bulk-data"
 
 
 def download_bulk_data_file(
     uri: str,
     bulk_file_type: ScryfallBulkFile | None = None,
-    bulk_file_dir: str = DEFAULT_BULK_FILE_DIR,
+    bulk_file_dir: Path = CONFIG.bulk_file_dir,
 ) -> None:
     """
     Download a single bulk data file from Scryfall.
 
     Args:
         uri: Location of bulk data file (generally found from bulk info
             endpoint).
         bulk_file_type: Type of bulk file, used to set filename.
-        bulk_file_dir: Directory to save bulk files. Defaults to `./data/bulk` if
-            not specified.
+        bulk_file_dir: Directory to save bulk files. Defaults to
+            `~/.scooze/data/bulk` if not specified.
 
     Raises:
         HTTPError: If request for bulk file not successful.
     """
 
     # TODO(#74): flag for check vs existing file; don't overwrite with same file or older version
     with requests.get(uri, stream=True) as r:
         r.raise_for_status()
-        os.makedirs(bulk_file_dir, exist_ok=True)
-        file_name = f"{bulk_file_dir}/{bulk_file_type}.json"
-        with open(file_name, "wb") as f:
+        bulk_file_dir.mkdir(parents=True, exist_ok=True)
+        file = bulk_file_dir / f"{bulk_file_type}.json"
+        with file.open(mode="wb") as f:
             for chunk in r.iter_content(chunk_size=None):
                 f.write(chunk)
 
 
 def download_bulk_data_file_by_type(
     bulk_file_type: ScryfallBulkFile | None = None,
-    bulk_file_dir: str = DEFAULT_BULK_FILE_DIR,
+    bulk_file_dir: str = CONFIG.bulk_file_dir,
 ) -> None:
     """
-    Get a bulk data file from Scryfall, specified by file type (from among ScryfallBulkFile).
+    Get a bulk data file from Scryfall, specified by file type
+    (from among ScryfallBulkFile).
 
     Args:
         bulk_file_type: Type of bulk file, used to set filename.
-        bulk_file_dir: Directory to save bulk files. Defaults to `./data/bulk` if
-            not specified.
+        bulk_file_dir: Directory to save bulk files. Defaults to
+            `~/.scooze/data/bulk` if not specified.
 
     Raises:
         HTTPError: If request for bulk file not successful.
     """
 
     # get URI from Scryfall bulk endpoint
 
@@ -63,22 +62,22 @@
     bulk_files = {t["type"]: t["download_uri"] for t in bulk_metadata}
     if bulk_file_type not in bulk_files:
         return
     download_bulk_data_file(bulk_files[bulk_file_type], bulk_file_type, bulk_file_dir)
 
 
 def download_all_bulk_data_files(
-    bulk_file_dir: str = DEFAULT_BULK_FILE_DIR,
+    bulk_file_dir: str = CONFIG.bulk_file_dir,
 ) -> None:
     """
     Download all supported Scryfall bulk data files to local filesystem.
 
     Args:
-        bulk_file_dir: Directory to save bulk files. Defaults to `./data/bulk` if
-            not specified.
+        bulk_file_dir: Directory to save bulk files. Defaults to
+            `~/.scooze/data/bulk` if not specified.
 
     Raises:
         HTTPError: If request for bulk file not successful.
     """
 
     with requests.get(SCRYFALL_BULK_INFO_ENDPOINT) as bulk_metadata_request:
         bulk_metadata_request.raise_for_status()
```

### Comparing `scooze-1.0.7/src/scooze/card.py` & `scooze-2.0.0/src/scooze/card.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,280 +1,50 @@
 import json
 import re
+from collections import Counter
 from datetime import date
-from typing import Iterable, Mapping, Self, TypeVar
+from typing import Iterable, Mapping, Self
 
 from beanie import PydanticObjectId
 from scooze.cardparts import (
     CardFace,
     CardPartsNormalizer,
-    FullCardFace,
     ImageUris,
     Preview,
     Prices,
     PurchaseUris,
     RelatedCard,
     RelatedUris,
 )
 from scooze.catalogs import (
     BorderColor,
     Color,
+    CostSymbol,
     Finish,
     Format,
     Frame,
     FrameEffect,
     Game,
     ImageStatus,
     Language,
     Layout,
     Legality,
     Rarity,
     SecurityStamp,
     SetType,
 )
+from scooze.logger import logger
 from scooze.models.card import CardModel
-from scooze.utils import FloatableT, HashableObject, scooze_logger
+from scooze.utils import FloatableT, HashableObject, parse_symbols
 
-logger = scooze_logger()
-
-## Generic Types
-CardFaceT = TypeVar("CardFaceT", bound=CardFace)  # generic CardFace type
+# TODO(#309): Add functionality to Card to get only the values for an "OracleCard"
 
 
 class Card(HashableObject):
     """
-    A basic Card object with minimal fields. Contains all information you might
-    use to sort a decklist.
-
-    Attributes:
-        name (str | None): This card's name.
-        scooze_id (PydanticObjectId | None): A unique identifier for a document
-            in a scooze database.
-        cmc (float | None): This card's mana value/converted mana cost.
-        color_identity (frozenset[Color] | None): This card's color identity,
-            for Commander variant deckbuilding.
-        colors (frozenset[Color] | None): This card's colors.
-        legalities (frozendict[Format, Legality] | None): Formats and the
-            legality status of this card in them.
-        mana_cost (str | None): Mana cost, as string of mana symbols.
-            (e.g. "{1}{W}{U}{B}{R}{G}")
-        power (str | None): Power of this card, if applicable.
-        toughness (str | None): Toughness of this card, if applicable.
-        type_line (str | None): This card's type line. (e.g. "Creature — Ooze")
-    """
-
-    def __init__(
-        self,
-        name: str | None = None,
-        cmc: FloatableT | None = None,
-        color_identity: Iterable[Color] | None = None,
-        colors: Iterable[Color] | None = None,
-        legalities: Mapping[Format, Legality] | None = None,
-        mana_cost: str | None = None,
-        power: str | None = None,
-        toughness: str | None = None,
-        type_line: str | None = None,
-        # kwargs
-        **kwargs,
-    ):
-        self.scooze_id = CardNormalizer.to_id(id_like=kwargs.get("id"))
-
-        self.name = name
-        self.cmc = CardNormalizer.to_float(cmc)
-        self.color_identity = CardNormalizer.to_frozenset(color_identity, convert_to_enum=Color)
-        self.colors = CardNormalizer.to_frozenset(colors, convert_to_enum=Color)
-        self.legalities = CardNormalizer.to_frozendict(
-            legalities, convert_key_to_enum=Format, convert_value_to_enum=Legality
-        )
-        self.mana_cost = mana_cost
-        self.power = power
-        self.toughness = toughness
-        self.type_line = type_line
-
-        if kwargs:
-            logger.debug("kwargs found", extra=kwargs)
-
-    def __str__(self):
-        return self.name
-
-    @classmethod
-    def from_json(cls, data: dict | str) -> Self:
-        """
-        Create a new Card with the given JSON.
-
-        Args:
-            data: Some JSON to create a scooze Card from.
-        """
-        if isinstance(data, dict):
-            return cls(**data)
-        elif isinstance(data, str):
-            return cls(**json.loads(data))
-
-    @classmethod
-    def from_model(cls, model: CardModel) -> Self:
-        """
-        Create a new Card with the given `CardModel`.
-
-        Args:
-            model: A CardModel to create a scooze Card from.
-        """
-        return cls(**model.model_dump())
-
-
-class OracleCard(Card):
-    """
-    A Card object containing all information about a unique card in Magic.
-    All information in this class is print-agnostic.
-
-    Attributes:
-        name (str | None): This card's name.
-        scooze_id (PydanticObjectId | None): A unique identifier for a document
-            in a scooze database.
-        card_faces (tuple[CardFaceT] | None): All component CardFaces of this
-            card, for multifaced cards.
-        cmc (float | None): This card's mana value/converted mana cost.
-        color_identity (frozenset[Color] | None): This card's color identity,
-            for Commander variant deckbuilding.
-        color_indicator (frozenset[Color] | None): The colors in this card's
-            color indicator, if it has one.
-        colors (frozenset[Color] | None): This card's colors.
-        edhrec_rank (int | None): This card's rank/popularity on EDHREC, if
-            applicable.
-        hand_modifier (str | None): This card's Vanguard hand size modifier, if
-            applicable.
-        keywords (frozenset[str] | None): Keywords and keyword actions this
-            card uses.
-        legalities (frozendict[Format, Legality] | None): Formats and the
-            legality status of this card in them.
-        life_modifier (str | None): This card's Vanguard life modifier value,
-            if applicable.
-        loyalty (str | None): This card's starting planeswalker loyalty, if
-            applicable.
-        mana_cost (str | None): Mana cost, as string of mana symbols.
-            (e.g. "{1}{W}{U}{B}{R}{G}")
-        oracle_id (str | None): A UUID for this card's oracle identity; shared
-            across prints of the same card but not same-named objects with
-            different gameplay properties.
-        oracle_text (str | None): This card's oracle text, if any.
-        penny_rank (int | None): This card's rank/popularity on Penny Dreadful.
-        power (str | None): Power of this card, if applicable.
-        prints_search_uri (str | None): A link to begin paginating through all
-            prints of this card in Scryfall's API.
-        produced_mana (frozenset[Color] | None): Which colors of mana this card
-            can produce.
-        reserved (bool | None): Whether this card is on the Reserved List.
-        rulings_uri (str | None): A link to rulings for this card in Scryfall's
-            API.
-        toughness (str | None): Toughness of this card, if applicable.
-        type_line (str | None): This card's type line. (e.g. "Creature — Ooze")
-    """
-
-    def __init__(
-        self,
-        name: str | None = None,
-        card_faces: Iterable[CardFace] | None = None,
-        cmc: FloatableT | None = None,
-        color_identity: Iterable[Color] | None = None,
-        color_indicator: Iterable[Color] | None = None,
-        colors: Iterable[Color] | None = None,
-        edhrec_rank: int | None = None,
-        hand_modifier: str | None = None,
-        keywords: Iterable[str] = None,
-        legalities: Mapping[Format, Legality] = None,
-        life_modifier: str | None = None,
-        loyalty: str | None = None,
-        mana_cost: str | None = None,
-        oracle_id: str | None = None,
-        oracle_text: str | None = None,
-        penny_rank: int | None = None,
-        power: str | None = None,
-        prints_search_uri: str | None = None,
-        produced_mana: Iterable[Color] | None = None,
-        reserved: bool | None = None,
-        rulings_uri: str | None = None,
-        toughness: str | None = None,
-        type_line: str | None = None,
-        # kwargs
-        **kwargs,
-    ):
-        super().__init__(
-            name=name,
-            cmc=cmc,
-            color_identity=color_identity,
-            colors=colors,
-            legalities=legalities,
-            mana_cost=mana_cost,
-            power=power,
-            toughness=toughness,
-            type_line=type_line,
-            **kwargs,
-        )
-        self.scooze_id = CardNormalizer.to_id(id_like=kwargs.get("id"))
-
-        self.card_faces = CardNormalizer.to_card_faces(card_faces, card_face_class=CardFace)
-        self.color_indicator = CardNormalizer.to_frozenset(color_indicator, convert_to_enum=Color)
-        self.edhrec_rank = edhrec_rank
-        self.hand_modifier = hand_modifier
-        self.keywords = CardNormalizer.to_frozenset(keywords)
-        self.life_modifier = life_modifier
-        self.loyalty = loyalty
-        self.oracle_id = oracle_id
-        self.oracle_text = oracle_text
-        self.penny_rank = penny_rank
-        self.prints_search_uri = prints_search_uri
-        self.produced_mana = CardNormalizer.to_frozenset(produced_mana, convert_to_enum=Color)
-        self.reserved = reserved
-        self.rulings_uri = rulings_uri
-
-    @classmethod
-    def oracle_text_without_reminder(cls, oracle_text: str) -> str:
-        """
-        Provide the given oracle text with reminder text removed.
-
-        Note:
-            This is a class method because cards with two unique faces won't
-            know which face you'd want. Instead you simply pass the text from
-            which you want to trim reminder text.
-
-        Args:
-            oracle_text: The oracle text of a card.
-        """
-
-        pattern_reminder = r" ?\([^()]+\) ?"  # text between parens ()
-        return re.sub(pattern_reminder, "", oracle_text)
-
-    def is_double_sided(self) -> bool:
-        """
-        Determine if this is a double-sided card.
-        """
-
-        return self.card_faces is not None
-
-    def total_words(self) -> int:
-        """
-        The number of words in this card's oracle text (excludes reminder text).
-        """
-
-        pattern_words = r"([a-zA-Z0-9+/{}']+)"  # words on a card
-
-        # MDFC
-        if self.is_double_sided():
-            return sum(
-                [
-                    len(re.findall(pattern_words, OracleCard.oracle_text_without_reminder(face.oracle_text)))
-                    for face in self.card_faces
-                ]
-            )
-        # Non-MDFC
-        else:
-            return len(re.findall(pattern_words, OracleCard.oracle_text_without_reminder(self.oracle_text)))
-
-
-class FullCard(OracleCard):
-    """
     A Card object that supports all fields available from Scryfall's JSON data.
     Represents a specific printing of a card.
 
     Attributes:
         name (str | None): This card's name.
         scooze_id (PydanticObjectId | None): A unique identifier for a document
             in a scooze database.
@@ -302,15 +72,15 @@
         rulings_uri (str | None): A link to rulings for this card in Scryfall's
             API.
         scryfall_uri (str | None): A link to the Scryfall page for this card.
         uri (str | None): A link to this card in Scryfall's API.
 
         all_parts (tuple[RelatedCard] | None): RelatedCards for tokens/meld
             pairs/other associated parts to this card, if applicable.
-        card_faces (tuple[CardFaceT] | None): All component CardFaces of this
+        card_faces (tuple[CardFace] | None): All component CardFaces of this
             card, for multifaced cards.
         cmc (float | None): This card's mana value/converted mana cost.
         color_identity (frozenset[Color] | None): This card's color identity,
             for Commander variant deckbuilding.
         color_indicator (frozenset[Color] | None): The colors in this card's
             color indicator, if it has one.
         colors (frozenset[Color] | None): This card's colors.
@@ -436,15 +206,15 @@
         oracle_id: str | None = None,
         prints_search_uri: str | None = None,
         rulings_uri: str | None = None,
         scryfall_uri: str | None = None,
         uri: str | None = None,
         # Gameplay Fields
         all_parts: Iterable[RelatedCard] | None = None,
-        card_faces: Iterable[FullCardFace] | None = None,
+        card_faces: Iterable[CardFace] | None = None,
         cmc: FloatableT | None = None,
         color_identity: Iterable[Color] | None = None,
         color_indicator: Iterable[Color] | None = None,
         colors: Iterable[Color] | None = None,
         edhrec_rank: int | None = None,
         hand_modifier: str | None = None,
         keywords: Iterable[str] | None = None,
@@ -506,42 +276,51 @@
         textless: bool | None = None,
         variation: bool | None = None,
         variation_of: str | None = None,
         watermark: str | None = None,
         # kwargs
         **kwargs,
     ):
-        super().__init__(
-            name=name,
-            card_faces=None,  # will be overridden with FullCardFaces
-            cmc=0,  # will be overridden with reversible card logic
-            color_identity=color_identity,
-            color_indicator=color_indicator,
-            colors=colors,
-            edhrec_rank=edhrec_rank,
-            hand_modifier=hand_modifier,
-            keywords=keywords,
-            legalities=legalities,
-            life_modifier=life_modifier,
-            loyalty=loyalty,
-            mana_cost=mana_cost,
-            oracle_id=oracle_id,
-            oracle_text=oracle_text,
-            penny_rank=penny_rank,
-            power=power,
-            prints_search_uri=prints_search_uri,
-            produced_mana=produced_mana,
-            reserved=reserved,
-            rulings_uri=rulings_uri,
-            toughness=toughness,
-            type_line=type_line,
-            **kwargs,
-        )
         self.scooze_id = CardNormalizer.to_id(id_like=kwargs.get("id"))
 
+        if kwargs:
+            logger.debug("kwargs found", extra=kwargs)
+
+        # region Basic Fields
+
+        self.name = name
+        self.cmc = CardNormalizer.to_float(cmc)
+        self.color_identity = CardNormalizer.to_frozenset(color_identity, convert_to_enum=Color)
+        self.colors = CardNormalizer.to_frozenset(colors, convert_to_enum=Color)
+        self.legalities = CardNormalizer.to_frozendict(
+            legalities, convert_key_to_enum=Format, convert_value_to_enum=Legality
+        )
+        self.mana_cost = mana_cost
+        self.power = power
+        self.toughness = toughness
+        self.type_line = type_line
+
+        # Oracle Fields
+        self.card_faces = CardNormalizer.to_card_faces(card_faces)
+        self.color_indicator = CardNormalizer.to_frozenset(color_indicator, convert_to_enum=Color)
+        self.edhrec_rank = edhrec_rank
+        self.hand_modifier = hand_modifier
+        self.keywords = CardNormalizer.to_frozenset(keywords)
+        self.life_modifier = life_modifier
+        self.loyalty = loyalty
+        self.oracle_id = oracle_id
+        self.oracle_text = oracle_text
+        self.penny_rank = penny_rank
+        self.prints_search_uri = prints_search_uri
+        self.produced_mana = CardNormalizer.to_frozenset(produced_mana, convert_to_enum=Color)
+        self.reserved = reserved
+        self.rulings_uri = rulings_uri
+
+        # endregion
+
         # region Core Fields
 
         self.arena_id = arena_id
         self.scryfall_id = scryfall_id if scryfall_id else kwargs.get("id")
         self.lang = CardNormalizer.to_enum(Language, lang)
         self.mtgo_id = mtgo_id
         self.mtgo_foil_id = mtgo_foil_id
@@ -553,16 +332,17 @@
         self.uri = uri
 
         # endregion
 
         # region Gameplay Fields
 
         self.all_parts = CardNormalizer.to_all_parts(all_parts)
-        self.card_faces = CardNormalizer.to_card_faces(card_faces, card_face_class=FullCardFace)
-        # Reversible cards currently have the same oracle card on both sides; will need to change this if this changes.
+        self.card_faces = CardNormalizer.to_card_faces(card_faces)
+        # NOTE: Reversible cards currently have the same oracle card on both sides;
+        # will need to change this if this changes.
         if layout == Layout.REVERSIBLE_CARD:
             self.cmc = CardNormalizer.to_float(self.card_faces[0].cmc)
         else:
             self.cmc = CardNormalizer.to_float(cmc)
         self.oversized = oversized
 
         # endregion
@@ -614,22 +394,97 @@
         self.textless = textless
         self.variation = variation
         self.variation_of = variation_of
         self.watermark = watermark
 
         # endregion
 
+    def __str__(self):
+        return self.name
+
+    @classmethod
+    def from_json(cls, data: dict | str) -> Self:
+        """
+        Create a new Card with the given JSON.
+
+        Args:
+            data: Some JSON to create a scooze Card from.
+        """
+
+        if isinstance(data, dict):
+            return cls(**data)
+        elif isinstance(data, str):
+            return cls(**json.loads(data))
+
+    @classmethod
+    def from_model(cls, model: CardModel) -> Self:
+        """
+        Create a new Card with the given `CardModel`.
+
+        Args:
+            model: A CardModel to create a scooze Card from.
+        """
+
+        return cls(**model.model_dump())
+
+    @classmethod
+    def oracle_text_without_reminder(cls, oracle_text: str) -> str:
+        """
+        Provide the given oracle text with reminder text removed.
+
+        Note:
+            This is a class method because cards with two unique faces won't
+            know which face you'd want. Instead you simply pass the text from
+            which you want to trim reminder text.
+
+        Args:
+            oracle_text: The oracle text of a card.
+        """
+
+        pattern_reminder = r" ?\([^()]+\) ?"  # text between parens ()
+        return re.sub(pattern_reminder, "", oracle_text)
+
+    def is_double_sided(self) -> bool:
+        """
+        Determine if this is a double-sided card.
+        """
+
+        return self.card_faces is not None
+
+    def mana_symbols(self) -> Counter[CostSymbol]:
+        """
+        A mapping of CostSymbols to how many times those symbols appear in this card's mana cost.
+        """
+
+        return parse_symbols(self.mana_cost)
+
     def total_words(self) -> int:
         """
-        The number of words in this card's oracle text (excludes reminder
-        text).
+        The number of words in this card's oracle text
+        (excludes reminder text).
         """
 
+        pattern_words = r"([a-zA-Z0-9+/{}']+)"  # words on a card
+
+        word_count: int
+
+        # MDFC
+        if self.is_double_sided():
+            word_count = sum(
+                [
+                    len(re.findall(pattern_words, Card.oracle_text_without_reminder(face.oracle_text)))
+                    for face in self.card_faces
+                ]
+            )
+        # Non-MDFC
+        else:
+            word_count = len(re.findall(pattern_words, Card.oracle_text_without_reminder(self.oracle_text)))
+
         # Don't double count reversible card text
-        return int(super().total_words() / (2 if self.layout is Layout.REVERSIBLE_CARD else 1))
+        return int(word_count / (2 if self.layout is Layout.REVERSIBLE_CARD else 1))
 
 
 class CardNormalizer(CardPartsNormalizer):
     """
     A simple class to use when normalizing non-serializable data from JSON.
 
     Usage:
@@ -652,34 +507,30 @@
             return all_parts
         elif all(isinstance(part, dict) for part in all_parts):
             return tuple(RelatedCard(**part) for part in all_parts)
 
     @classmethod
     def to_card_faces(
         cls,
-        card_faces: Iterable[CardFaceT] | Iterable[dict] | None,
-        card_face_class: type[CardFaceT] = CardFace,
-    ) -> tuple[CardFaceT] | None:
+        card_faces: Iterable[CardFace] | Iterable[dict] | None,
+    ) -> tuple[CardFace] | None:
         """
         Normalize card_faces from JSON.
 
         Args:
-            card_faces: A Iterable[F] or Iterable[JSON] to normalize. F is of
-                type CardFace or FullCardFace.
-            card_face_class: A CardFace class to create an instance of.
-                (one of CardFace or FullCardFace)
+            card_faces: An Iterable[CardFace] to normalize.
 
         Returns:
-            A tuple[F] where F is of type CardFace or FullCardFace.
+            A tuple[CardFace].
         """
 
-        if card_faces is None or all(isinstance(card_face, card_face_class) for card_face in card_faces):
+        if card_faces is None:
             return card_faces
         elif all(isinstance(card_face, dict) for card_face in card_faces):
-            return tuple(card_face_class.from_json(card_face) for card_face in card_faces)
+            return tuple(CardFace.from_json(card_face) for card_face in card_faces)
 
     @classmethod
     def to_id(cls, id_like: PydanticObjectId | str | None) -> PydanticObjectId | None:
         """
         Normalize ID from JSON.
 
         Args:
@@ -723,13 +574,7 @@
             An instance of Prices.
         """
 
         if prices is None or isinstance(prices, Prices):
             return prices
         elif isinstance(prices, dict):
             return Prices(**prices)
-
-
-CardT = TypeVar("CardT", bound=Card)
-"""
-A TypeVar for representing Generic Card types.
-"""
```

### Comparing `scooze-1.0.7/src/scooze/cardparts.py` & `scooze-2.0.0/src/scooze/cardparts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 from datetime import date
 from typing import Iterable, Mapping, Self
 
 from scooze.catalogs import Color, Component, Layout
-from scooze.utils import FloatableT, HashableObject, JsonNormalizer, scooze_logger
-
-logger = scooze_logger()
+from scooze.logger import logger
+from scooze.utils import FloatableT, HashableObject, JsonNormalizer
 
 
 class ImageUris(HashableObject):
     """
     URIs of images associated with this object on [Scryfall](https://scryfall.com/docs/api/images).
 
     Attributes:
@@ -44,77 +43,15 @@
 
         if kwargs:
             logger.debug("kwargs found", extra=kwargs)
 
 
 class CardFace(HashableObject):
     """
-    An object for a single face of a multi-faced OracleCard. Contains only
-    fields that are consistent between card prints.
-    Multi-faced cards include MDFCs, split cards, aftermath, etc;
-    see [here](https://scryfall.com/docs/api/cards#card-face-objects)
-
-    Attributes:
-        name (str | None): Name of this face.
-        cmc (float | None): Mana value of this face.
-        color_indicator (frozenset[Color] | None): Color indicator on this
-            face, if any.
-        colors (frozenset[Color] | None): Colors of this face.
-        loyalty (str | None): Starting planeswalker loyalty of this face, if
-            any.
-        mana_cost (str | None): Mana cost of this face.
-        oracle_id (str | None): Oracle ID of this face, for reversible cards.
-        oracle_text (str | None): Oracle text of this face, if any.
-        power (str | None): Power of this face, if any.
-        toughness (str | None): Toughness of this face, if any.
-        type_line (str | None): Type line of this face, if any.
-    """
-
-    def __init__(
-        self,
-        name: str | None = None,
-        cmc: FloatableT | None = None,
-        color_indicator: Iterable[Color] | None = None,
-        colors: Iterable[Color] | None = None,
-        loyalty: str | None = None,
-        mana_cost: str | None = None,
-        oracle_id: str | None = None,
-        oracle_text: str | None = None,
-        power: str | None = None,
-        toughness: str | None = None,
-        type_line: str | None = None,
-        # kwargs
-        **kwargs,
-    ):
-        self.name = name
-        self.cmc = CardPartsNormalizer.to_float(cmc)
-        self.color_indicator = CardPartsNormalizer.to_frozenset(color_indicator)
-        self.colors = CardPartsNormalizer.to_frozenset(colors)
-        self.loyalty = loyalty
-        self.mana_cost = mana_cost
-        self.oracle_id = oracle_id
-        self.oracle_text = oracle_text
-        self.power = power
-        self.toughness = toughness
-        self.type_line = type_line
-
-        if kwargs:
-            logger.debug("kwargs found", extra=kwargs)
-
-    @classmethod
-    def from_json(cls, data: dict | str) -> Self:
-        if isinstance(data, dict):
-            return cls(**data)
-        elif isinstance(data, str):
-            return cls(**json.loads(data))
-
-
-class FullCardFace(CardFace):
-    """
-    An object for a single face of a multi-faced FullCard.
+    An object for a single face of a multi-faced Card.
     Multi-faced cards include MDFCs, split cards, aftermath, etc;
     see [here](https://scryfall.com/docs/api/cards#card-face-objects)
 
     Attributes:
         name (str | None): Name of this face.
         artist (str | None): Illustrator for art on this face.
         artist_id (str | None): Scryfall ID for the artist of this face.
@@ -167,14 +104,17 @@
         printed_type_line: str | None = None,
         toughness: str | None = None,
         type_line: str | None = None,
         watermark: str | None = None,
         # kwargs
         **kwargs,
     ):
+        if kwargs:
+            logger.debug("kwargs found", extra=kwargs)
+
         self.name = name
         self.artist = artist
         self.artist_id = artist_id
         self.cmc = CardPartsNormalizer.to_float(cmc)
         self.color_indicator = CardPartsNormalizer.to_frozenset(color_indicator, convert_to_enum=Color)
         self.colors = CardPartsNormalizer.to_frozenset(colors, convert_to_enum=Color)
         self.flavor_text = flavor_text
@@ -189,14 +129,44 @@
         self.printed_name = printed_name
         self.printed_text = printed_text
         self.printed_type_line = printed_type_line
         self.toughness = toughness
         self.type_line = type_line
         self.watermark = watermark
 
+    @classmethod
+    def from_json(cls, data: dict | str) -> Self:
+        if isinstance(data, dict):
+            return cls(**data)
+        elif isinstance(data, str):
+            return cls(**json.loads(data))
+
+
+class Preview(HashableObject):
+    """
+    An object for information about where and when a card was previewed.
+
+    Attributes:
+        previewed_at (date | None): Date/time of preview being shown or added to Scryfall.
+        source (str | None): Name of preview source.
+        source_uri (str | None): Location of preview source.
+    """
+
+    def __init__(
+        self,
+        previewed_at: date | None = None,
+        source: str | None = None,
+        source_uri: str | None = None,
+        # kwargs
+        **kwargs,
+    ):
+        self.previewed_at = CardPartsNormalizer.to_date(previewed_at)
+        self.source = source
+        self.source_uri = source_uri
+
         if kwargs:
             logger.debug("kwargs found", extra=kwargs)
 
 
 class Prices(HashableObject):
     """
     An object for all price data associated with a Card object.
@@ -228,40 +198,14 @@
         self.eur_foil = CardPartsNormalizer.to_float(eur_foil)
         self.tix = CardPartsNormalizer.to_float(tix)
 
         if kwargs:
             logger.debug("kwargs found", extra=kwargs)
 
 
-class Preview(HashableObject):
-    """
-    An object for information about where and when a card was previewed.
-
-    Attributes:
-        previewed_at (date | None): Date/time of preview being shown or added to Scryfall.
-        source (str | None): Name of preview source.
-        source_uri (str | None): Location of preview source.
-    """
-
-    def __init__(
-        self,
-        previewed_at: date | None = None,
-        source: str | None = None,
-        source_uri: str | None = None,
-        # kwargs
-        **kwargs,
-    ):
-        self.previewed_at = CardPartsNormalizer.to_date(previewed_at)
-        self.source = source
-        self.source_uri = source_uri
-
-        if kwargs:
-            logger.debug("kwargs found", extra=kwargs)
-
-
 class PurchaseUris(HashableObject):
     """
     URIs to this card's listings on major marketplaces.
 
     Attributes:
         tcgplayer (str | None): Link to buy this card on the TCGplayer marketplace.
         cardmarket (str | None): Link to buy this card on the Cardmarket marketplace.
```

### Comparing `scooze-1.0.7/src/scooze/catalogs.py` & `scooze-2.0.0/src/scooze/catalogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 from enum import StrEnum, auto
 from functools import cache
 from typing import FrozenSet
 
-from scooze.enum import ExtendedEnum
+from scooze.enums import ExtendedEnum
+
+__all__ = (
+    "BorderColor",
+    "Color",
+    "Component",
+    "Finish",
+    "Format",
+    "Frame",
+    "FrameEffect",
+    "Game",
+    "ImageStatus",
+    "Language",
+    "Layout",
+    "Legality",
+    "Rarity",
+    "ScryfallBulkFile",
+    "SecurityStamp",
+    "SetType",
+    "CostSymbol",
+)
 
 # region Card Enums
 
 
 class BorderColor(ExtendedEnum, StrEnum):
     """
     A color that borders of Magic cards can be.
@@ -117,14 +137,15 @@
     LEGENDARY = auto()
     LESSON = auto()
     MIRACLE = auto()
     NYXTOUCHED = auto()
     SHATTEREDGLASS = auto()
     SHOWCASE = auto()
     SNOW = auto()
+    SPREE = auto()
     TEXTLESS = auto()
     TOMBSTONE = auto()
 
     # Double-faced card marks
     COMPASSLANDDFC = auto()
     CONVERTDFC = auto()
     FANDFC = auto()
@@ -302,14 +323,15 @@
     TOKEN = auto()
     TREASURE_CHEST = auto()
     VANGUARD = auto()
 
 
 # endregion
 
+
 # region Symbology
 
 
 class CostSymbol(ExtendedEnum, StrEnum):
     """
     A symbol that can show up in mana cost or oracle text of Magic cards.
     """
```

### Comparing `scooze-1.0.7/src/scooze/console/cli.py` & `scooze-2.0.0/src/scooze/console/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,23 +12,19 @@
 
     from cleo.commands.command import Command
 
 # Accepted scooze CLI commands
 COMMANDS = [
     "delete",
     "run",
+    # Save commands
+    "save cards",
     # Load commands
     "load cards",
     "load decks",
-    # Setup commands
-    "setup docker",
-    "setup local",
-    # Teardown commands
-    "teardown docker",
-    "teardown local",
 ]
 
 
 def load_scooze_command(name: str) -> Callable[[], Command]:
     def _scooze_command_factory() -> Command:
         cli_words = name.split(" ")
         module = import_module("scooze.console.commands." + ".".join(cli_words))
```

### Comparing `scooze-1.0.7/src/scooze/console/commands/delete.py` & `scooze-2.0.0/src/scooze/console/commands/delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import scooze.database.deck as deck_db
 from cleo.commands.command import Command
 from cleo.helpers import argument
 from scooze.api import ScoozeApi
-from scooze.database.core import DbCollection
+from scooze.enums import DbCollection
 
 ACCEPTED_DELETE_ARGS = {
     "all",
     "cards",
     "decks",
 }
 
@@ -36,21 +35,19 @@
                 to_delete.append(DbCollection.DECKS)
 
         if len(to_delete) == 0:
             extra_args = " ".join(delete_args - ACCEPTED_DELETE_ARGS)
             self.line(f"No valid collections were given. Ignored the following: <fg=cyan>{extra_args}</>")
 
         for collection in to_delete:
-            delete_collection(collection)
+            self.delete_collection(collection)
 
-
-def delete_collection(coll: DbCollection):
-    clean = input(f"Delete existing {coll}? [y/N] ") in "yY"
-    if clean:
-        print(f"Deleting all {coll} from your local database...")
-        match coll:
-            case DbCollection.CARDS:
-                with ScoozeApi() as s:
-                    s.delete_cards_all()
-            case DbCollection.DECKS:
-                # TODO(#145): Use the ScoozeApi for this
-                deck_db.delete_decks_all()
+    def delete_collection(self, coll: DbCollection):
+        if self.confirm(f"Delete existing {coll}?"):
+            self.line(f"Deleting all {coll} from your local database...")
+            match coll:
+                case DbCollection.CARDS:
+                    with ScoozeApi() as s:
+                        s.delete_cards_all()
+                case DbCollection.DECKS:
+                    # TODO(#145): Use the ScoozeApi for this
+                    self.line("Can't delete decks yet.")
```

### Comparing `scooze-1.0.7/src/scooze/console/commands/load/cards.py` & `scooze-2.0.0/src/scooze/console/commands/save/cards.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 from cleo.commands.command import Command
 from cleo.helpers import option
-from scooze.api import ScoozeApi
+from scooze.bulkdata import download_bulk_data_file_by_type
 from scooze.catalogs import ScryfallBulkFile
-from scooze.utils import DEFAULT_BULK_FILE_DIR
+from scooze.config import CONFIG
 
 
-class LoadCardsCommand(Command):
-    name = "load cards"
-    description = "Load sets of cards into the database."
+class SaveCardsCommand(Command):
+    name = "save cards"
+    description = "Save sets of cards to a local directory."
 
     options = [
         option("all", description="Every print of all cards and game objects in all languages."),
         option("artwork", description="Includes each unique illustration once."),
         option("oracle", description="One version of each card ever printed."),
         option("prints", description="Every print of each card ever printed, in English where available."),
         option("test", description="The Power 9, for testing purposes."),
         option(
             "bulk-data-dir",
-            description="Directory to store bulk files, used with load cards.",
-            default=DEFAULT_BULK_FILE_DIR,
+            description="Directory to store bulk files.",
+            default=CONFIG.bulk_file_dir,
             value_required=True,
             flag=False,
         ),
     ]
 
     def handle(self):
-        to_load: list[ScryfallBulkFile] = []
-        load_all = self.option("all")
-        load_test = self.option("test") and not load_all
+        to_save: list[ScryfallBulkFile] = []
 
         if self.option("all"):
-            to_load.append(ScryfallBulkFile.ALL)
+            to_save.append(ScryfallBulkFile.ALL)
         else:
             if self.option("oracle"):
-                to_load.append(ScryfallBulkFile.ORACLE)
+                to_save.append(ScryfallBulkFile.ORACLE)
             if self.option("artwork"):
-                to_load.append(ScryfallBulkFile.ARTWORK)
+                to_save.append(ScryfallBulkFile.ARTWORK)
             if self.option("prints"):
-                to_load.append(ScryfallBulkFile.DEFAULT)
+                to_save.append(ScryfallBulkFile.DEFAULT)
 
-        if len(to_load) == 0 and not load_test:
-            self.line("No files were selected to load.")
-
-        with ScoozeApi() as s:
-            for bulk_file in to_load:
-                s.load_card_file(bulk_file, self.option("bulk-data-dir"))
-            if load_test:
-                s.load_card_file(ScryfallBulkFile.DEFAULT, "./data/test")
+        for bulk_file in to_save:
+            self.line(f"Downloading {bulk_file} from Scryfall...")
+            download_bulk_data_file_by_type(bulk_file, self.option("bulk-data-dir"))
```

### Comparing `scooze-1.0.7/src/scooze/console/commands/load/decks.py` & `scooze-2.0.0/src/scooze/console/commands/load/decks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-import asyncio
 import json
 import os
+from pathlib import Path
 
 import ijson
-import scooze.database.deck as deck_db
 from cleo.commands.command import Command
 from cleo.helpers import option
-from scooze.models.deck import DeckModelIn
-from scooze.utils import DEFAULT_DECKS_DIR
+from scooze.config import CONFIG
+from scooze.models.deck import DeckModel
 
 
 class LoadDecksCommand(Command):
     name = "load decks"
     description = "Load sets of decks into the database."
 
     options = [
         option("all", description="All decks in the decks directory."),
         option("test", description="A set of Pioneer decks for testing purposes."),
         option(
             "decks-dir",
             description="Directory to store deck files, used with load decks.",
-            default=DEFAULT_DECKS_DIR,
+            default=CONFIG.decks_dir,
             value_required=True,
             flag=False,
         ),
     ]
 
     def handle(self):
         # TODO(#145): Use ScoozeApi to load decks via API
@@ -38,32 +37,34 @@
 
 # TODO(#145): Can remove this once the command uses ScoozeApi
 def load_all_decks(decks_dir: str):
     files = os.listdir(decks_dir)
     try:
         for file_path in files:
             with open(file_path, "r", encoding="utf8") as deck_file:
-                print(f"Inserting {file_path.split('/')[-1]} file into the database...")
+                # print(f"Inserting {file_path.split('/')[-1]} file into the database...")
                 decks = [
-                    DeckModelIn.model_validate(deck_json)
+                    DeckModel.model_validate(deck_json)
                     for deck_json in ijson.items(
                         deck_file,
                         "item",
                     )
                 ]
-                asyncio.run(deck_db.add_decks(decks))
+                # asyncio.run(deck_db.add_decks(decks))
+        print("This doesn't actually do anything yet.")
     except OSError as e:
         print(f"Encountered an error while trying to load {file_path.split('/')[-1]}")
         raise e
 
 
 # TODO(#145): Can remove this once the command uses ScoozeApi
 def load_test_decks():
     try:
-        with open("./data/test/pioneer_decks.jsonl") as decks_file:
-            print("Inserting test decks into the database...")
+        with Path("./data/test/pioneer_decks.jsonl").open() as decks_file:
+            # print("Inserting test decks into the database...")
             json_list = list(decks_file)
-            decks = [DeckModelIn.model_validate(json.loads(deck_json)) for deck_json in json_list]
-            asyncio.run(deck_db.add_decks(decks))  # TODO(#7): this need async for now, replace with Python API
+            decks = [DeckModel.model_validate(json.loads(deck_json)) for deck_json in json_list]
+            # asyncio.run(deck_db.add_decks(decks))  # TODO(#7): this need async for now, replace with Python API
+        print("This doesn't actually do anything yet.")
     except OSError as e:
         print("Encountered an error while trying to load test decks")
         raise e
```

### Comparing `scooze-1.0.7/src/scooze/database/mongo.py` & `scooze-2.0.0/src/scooze/mongo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from motor.motor_asyncio import AsyncIOMotorClient
-
-MONGO_URI = "mongodb://127.0.0.1:27017"
+from scooze.config import CONFIG
 
 
 class Database:
     """
     A simple database object to house the Motor client.
 
     Attributes:
@@ -18,15 +17,15 @@
 
 
 async def mongo_connect():
     """
     Connect to the database client to MongoDB.
     """
 
-    db.client = AsyncIOMotorClient(MONGO_URI)
+    db.client = AsyncIOMotorClient(CONFIG.mongo_dsn)
 
 
 async def mongo_close():
     """
     Close the database client's MongoDB connection.
     """
```

### Comparing `scooze-1.0.7/src/scooze/deck.py` & `scooze-2.0.0/src/scooze/deck.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from collections import Counter
 from enum import StrEnum, auto
 from sys import maxsize
-from typing import Generic, Self
+from typing import Self
 
 import scooze.utils as utils
-from scooze.card import CardT
-from scooze.catalogs import Format, Legality
-from scooze.deckpart import DeckDiff, DeckPart
-from scooze.enum import ExtendedEnum
-from scooze.utils import ComparableObject
+from scooze.card import Card
+from scooze.cardlist import CardList
+from scooze.catalogs import CostSymbol, Format, Legality
+from scooze.enums import ExtendedEnum
+from scooze.logger import logger
+from scooze.utils import ComparableObject, DictDiff
 
-logger = utils.scooze_logger()
-
-# region Deck Enums
+# region Deck Helpers
 
 
 class InThe(ExtendedEnum, StrEnum):
     """
     The location of a Card in a Deck.
     """
 
@@ -32,67 +31,125 @@
     A method of formatting a decklist for external systems.
     """
 
     ARENA = auto()
     MTGO = auto()
 
 
+class DeckDiff(ComparableObject):
+    """
+    A class to represent a diff between two decks.
+
+    Attributes:
+        main (DictDiff): The diff between the main decks of two Decks.
+        side (DictDiff): The diff between the sideboards of two Decks.
+        cmdr (DictDiff): The diff between the command zones of two Decks.
+        attractions (DictDiff): The diff between the attractions of the two Decks.
+        stickers (DictDiff): The diff between the stickers of the two Decks.
+    """
+
+    def __init__(
+        self,
+        main: DictDiff,
+        side: DictDiff = None,
+        cmdr: DictDiff = None,
+        attractions: DictDiff = None,
+        stickers: DictDiff = None,
+    ):
+        self.main = main
+        self.side = side or DictDiff(contents={})
+        self.cmdr = cmdr or DictDiff(contents={})
+        self.attractions = attractions or DictDiff(contents={})
+        self.stickers = stickers or DictDiff(contents={})
+
+    def __str__(self):
+        if self.total() > 0:
+            main_diff = str(self.main)
+            side_diff = str(self.side)
+            cmdr_diff = str(self.cmdr)
+            attractions_diff = str(self.stickers)
+            stickers_diff = str(self.stickers)
+
+            diff = f"Main Diff:\n{main_diff}"
+            if not self.side.is_empty():
+                diff += f"\nSide Diff:\n{side_diff}"
+            if not self.cmdr.is_empty():
+                diff += f"\nCmdr Diff:\n{cmdr_diff}"
+            if not self.attractions.is_empty():
+                diff += f"\nAttractions Diff:\n{attractions_diff}"
+            if not self.stickers.is_empty():
+                diff += f"\nStickers{stickers_diff}"
+
+            return diff
+
+        return ""
+
+    def total(self) -> int:
+        """
+        The number of cards in this DeckDiff.
+        """
+
+        return sum(map(len, (self.main, self.side, self.cmdr, self.attractions, self.stickers)))
+
+
 # endregion
 
 
-class Deck(ComparableObject, Generic[CardT]):
+class Deck(ComparableObject):
     """
     A class to represent a deck of Magic: the Gathering cards.
 
     Attributes:
         archetype (str | None): The archetype of this Deck.
         format (Format): The format legality of the cards in this Deck.
-        main (DeckPart[CardT]): The main deck. Typically 60 cards minimum.
-        side (DeckPart[CardT]): The sideboard. Typically 15 cards maximum.
-        cmdr (DeckPart[CardT]): The command zone. Typically 1 or 2 cards in Commander formats.
-        attractions (DeckPart[CardT]): The attraction deck.
-        stickers (DeckPart[CardT]): The sticker deck.
-        companion (CardT | None): This deck's companion (if applicable).
+        main (CardList): The main deck. Typically 60 cards minimum.
+        side (CardList): The sideboard. Typically 15 cards maximum.
+        cmdr (CardList): The command zone. Typically 1 or 2 cards in Commander formats.
+        attractions (CardList): The attraction deck.
+        stickers (CardList): The sticker deck.
+        companion (Card | None): This deck's companion (if applicable).
     """
 
     def __init__(
         self,
         archetype: str | None = None,
         format: Format = Format.NONE,
-        main: DeckPart[CardT] | None = None,
-        side: DeckPart[CardT] | None = None,
-        cmdr: DeckPart[CardT] | None = None,
-        attractions: DeckPart[CardT] | None = None,
-        stickers: DeckPart[CardT] | None = None,
-        companion: CardT | None = None,
+        main: CardList | None = None,
+        side: CardList | None = None,
+        cmdr: CardList | None = None,
+        attractions: CardList | None = None,
+        stickers: CardList | None = None,
+        companion: Card | None = None,
     ):
         self.archetype = archetype
         self.format = format
 
-        self.main = main if main is not None else DeckPart()
-        self.side = side if side is not None else DeckPart()
-        self.cmdr = cmdr if cmdr is not None else DeckPart()
-        self.attractions = attractions if attractions is not None else DeckPart()
-        self.stickers = stickers if stickers is not None else DeckPart()
+        self.main = main if main is not None else CardList()
+        self.side = side if side is not None else CardList()
+        self.cmdr = cmdr if cmdr is not None else CardList()
+        self.attractions = attractions if attractions is not None else CardList()
+        self.stickers = stickers if stickers is not None else CardList()
 
         self.companion = companion
 
     @property
-    def cards(self) -> Counter[CardT]:
+    def cards(self) -> Counter[Card]:
         """
         Get this Deck as a collection of cards.
         """
+
         return self.main.cards + self.side.cards + self.cmdr.cards + self.attractions.cards + self.stickers.cards
 
     def __str__(self):
         decklist = self.export()
         return f"""Archetype: {self.archetype}\n""" f"""Format: {self.format}\n""" f"""Decklist:\n{decklist}\n"""
 
+    # region Deck statistics
+
     # TODO(#112): Add type filters.
-    # TODO(#113): Reversible cards do not have a top-level cmc. Assign one?
     def average_cmc(self) -> float:
         """
         The average mana value of cards in this Deck.
         """
 
         total_cards = self.total_cards()
 
@@ -109,14 +166,48 @@
 
         total_cards = self.total_cards()
 
         if total_cards > 0:
             return self.total_words() / self.total_cards()
         return 0
 
+    def total_cards(self) -> int:
+        """
+        The number of cards in this Deck.
+        """
+
+        return (
+            self.main.total() + self.side.total() + self.cmdr.total() + self.attractions.total() + self.stickers.total()
+        )
+
+    def total_cmc(self) -> float:
+        """
+        The total mana value of cards in this Deck.
+        """
+
+        return sum([c.cmc * q for c, q in self.cards.items()])
+
+    def count_pips(self) -> Counter[CostSymbol]:
+        """
+        A mapping of Colors to how many times they appear as mana symbols in
+        costs of cards in this Deck.
+        """
+
+        return sum([part.count_pips() for part in [self.main, self.side, self.cmdr]], Counter())
+
+    def total_words(self) -> int:
+        """
+        The number of words across all oracle text on all cards in this Deck
+        (excludes reminder text).
+        """
+
+        return sum([c.total_words() * q for c, q in self.cards.items()])
+
+    # endregion
+
     def diff(self, other: Self) -> DeckDiff:
         """
         Generate a diff between this Deck and another.
 
         Args:
             other: The other Deck.
 
@@ -274,43 +365,17 @@
             if self.attractions.total() > len(self.attractions.cards):
                 return False
             if self.stickers.total() > len(self.stickers.cards):
                 return False
 
         return True
 
-    def total_cards(self) -> int:
-        """
-        The number of cards in this Deck.
-        """
-
-        return (
-            self.main.total() + self.side.total() + self.cmdr.total() + self.attractions.total() + self.stickers.total()
-        )
-
-    def total_cmc(self) -> float:
-        """
-        The total mana value of cards in this Deck.
-        """
-
-        # TODO(#113): Reversible cards do not have a top-level cmc. Assign one?
-
-        return sum([c.cmc * q for c, q in self.cards.items()])
-
-    def total_words(self) -> int:
-        """
-        The number of words across all oracle text on all cards in this Deck
-        (excludes reminder text).
-        """
-
-        return sum([c.total_words() * q for c, q in self.cards.items()])
-
     # region Mutating Methods
 
-    def add_card(self, card: CardT, quantity: int = 1, in_the: InThe = InThe.MAIN) -> None:
+    def add_card(self, card: Card, quantity: int = 1, in_the: InThe = InThe.MAIN) -> None:
         """
         Add a given quantity of a given card to this Deck.
 
         Args:
             card: The card to add.
             quantity: The number of copies of the card to be added.
             in_the: Where to add the card (main, side, etc.)
@@ -327,15 +392,15 @@
                 self.attractions.add_card(card=card, quantity=quantity)
             case InThe.STICKERS:
                 self.stickers.add_card(card=card, quantity=quantity)
             case _:
                 logger.info("Failed to add card.", extra={"card": card})
                 logger.warning(f'in_the "{in_the}" not found. Must be one of {InThe.list()}')
 
-    def add_cards(self, cards: Counter[CardT], in_the: InThe = InThe.MAIN) -> None:
+    def add_cards(self, cards: Counter[Card], in_the: InThe = InThe.MAIN) -> None:
         """
         Add the given cards to this Deck.
 
         Args:
             cards: The cards to add.
             in_the: Where to add the cards (main, side, etc.)
         """
@@ -348,15 +413,15 @@
             case InThe.CMDR:
                 self.cmdr.add_cards(cards)
             case InThe.ATTRACTIONS:
                 self.attractions.add_cards(cards)
             case InThe.STICKERS:
                 self.stickers.add_cards(cards)
 
-    def remove_card(self, card: CardT, quantity: int = maxsize, in_the: InThe = InThe.MAIN) -> None:
+    def remove_card(self, card: Card, quantity: int = maxsize, in_the: InThe = InThe.MAIN) -> None:
         """
         Remove a given quantity of a given card from this Deck. If quantity is
         not provided, removes all copies.
 
         Args:
             card: The card to remove.
             quantity: The number of copies of the card to be removed.
@@ -375,15 +440,15 @@
                 self.attractions.remove_card(card=card, quantity=quantity)
             case InThe.STICKERS:
                 self.stickers.remove_card(card=card, quantity=quantity)
             case _:
                 logger.info("Failed to remove card.", extra={"card": card})
                 logger.warning(f'in_the "{in_the}" not found. Must be one of {InThe.list()}')
 
-    def remove_cards(self, cards: Counter[CardT], in_the: InThe = InThe.MAIN) -> None:
+    def remove_cards(self, cards: Counter[Card], in_the: InThe = InThe.MAIN) -> None:
         """
         Remove the given cards from this Deck.
 
         Args:
             cards: The cards to remove.
             in_the: Where to remove the cards from (main, side, etc.)
         """
```

### Comparing `scooze-1.0.7/src/scooze/enum.py` & `scooze-2.0.0/src/scooze/enums.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enum import Enum, EnumMeta
+from enum import Enum, EnumMeta, StrEnum
 
 # region Enum Extensions
 
 
 class CaseInsensitiveEnumMeta(EnumMeta):
     """
     An extension of the classic Python EnumMeta to support case-insensitive
@@ -26,7 +26,22 @@
         """
         Get a list of this Enum's field names.
         """
         return list(map(lambda c: c.value, cls))
 
 
 # endregion
+
+
+# region Database Enums
+
+
+class DbCollection(ExtendedEnum, StrEnum):
+    """
+    Collections in the scooze database.
+    """
+
+    CARDS = "cards"
+    DECKS = "decks"
+
+
+# endregion
```

### Comparing `scooze-1.0.7/src/scooze/main.py` & `scooze-2.0.0/src/scooze/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from contextlib import asynccontextmanager
+from pathlib import Path
 
 from beanie import init_beanie
 from fastapi import FastAPI
 from fastapi.staticfiles import StaticFiles
 from scooze.config import CONFIG
 from scooze.models.card import CardModel
 from scooze.mongo import db, mongo_close, mongo_connect
@@ -25,22 +26,23 @@
 
     # Mongo teardown
     await mongo_close()
 
 
 app = FastAPI(
     title="scooze",
-    summary="REST API for interacting with MongoDB for Magic: the Gathering tournaments, decklists, and cards.",
+    summary="REST API for interacting with Magic: the Gathering cards and decks.",
     lifespan=lifespan,
+    version=CONFIG.version,
 )
 
 
 # Router inclusion
 app.include_router(CardRouter)
 app.include_router(CardsRouter)
 app.include_router(DeckRouter)
 app.include_router(DecksRouter)
 
 # Mount index.html
 app_dir = os.path.dirname(__file__)
-static_dir = os.path.join(app_dir, "static/")
+static_dir = Path(app_dir) / "static/"
 app.mount("/", StaticFiles(directory=static_dir, html=True), name="static")
```

### Comparing `scooze-1.0.7/src/scooze/models/card.py` & `scooze-2.0.0/src/scooze/models/card.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from datetime import date
-from typing import Any
+from typing import Any, Callable
 
-from pydantic import AliasChoices, ConfigDict, Field, field_serializer, field_validator
+from pydantic import (
+    AliasChoices,
+    ConfigDict,
+    Field,
+    ValidationInfo,
+    field_serializer,
+    field_validator,
+)
 from scooze.cardparts import (
     CardFace,
-    FullCardFace,
     ImageUris,
     Preview,
     Prices,
     PurchaseUris,
     RelatedCard,
     RelatedUris,
 )
@@ -24,31 +30,32 @@
     Language,
     Layout,
     Legality,
     Rarity,
     SecurityStamp,
     SetType,
 )
-from scooze.database.core import DbCollection
+from scooze.enums import DbCollection
+from scooze.logger import logger
 from scooze.models.cardparts import (
     CardFaceModel,
     ImageUrisModel,
     PreviewModel,
     PricesModel,
     PurchaseUrisModel,
     RelatedCardModel,
     RelatedUrisModel,
 )
 from scooze.models.utils import ScoozeBaseModel, ScoozeDocument
-from scooze.utils import DATE_FORMAT
+from scooze.utils import encode_date
 
 
 class CardModelData(ScoozeBaseModel):
     """
-    A Card object that supports all fields available from Scryfall's JSON data.
+    A data model that supports all fields available from Scryfall's JSON data.
     Represents a specific printing of a card.
 
     Attributes:
         arena_id: This card's Arena ID, if applicable.
         scryfall_id: Scryfall's unique ID for this card.
         lang: The language code for this print;
             see [here](https://scryfall.com/docs/api/languages)
@@ -506,93 +513,102 @@
 
     # endregion
 
     # region Validators
 
     @field_validator("all_parts", mode="before")
     @classmethod
-    def all_parts_validator(cls, vals):
+    def _validate_all_parts(cls, vals):
         if vals is not None and all(isinstance(v, RelatedCard) for v in vals):
             vals = [RelatedCardModel.model_validate(v.__dict__) for v in vals]
         return vals
 
     @field_validator("card_faces", mode="before")
     @classmethod
-    def card_faces_validator(cls, vals):
-        if vals is not None and all(isinstance(v, CardFace | FullCardFace) for v in vals):
+    def _validate_card_faces(cls, vals):
+        if vals is not None and all(isinstance(v, CardFace) for v in vals):
             vals = [CardFaceModel.model_validate(v.__dict__) for v in vals]
         return vals
 
     @field_validator("image_uris", mode="before")
     @classmethod
-    def image_uris_validator(cls, v):
+    def _validate_image_uris(cls, v):
         if isinstance(v, ImageUris):
             v = ImageUrisModel.model_validate(v.__dict__)
         return v
 
     @field_validator("preview", mode="before")
     @classmethod
-    def preview_validator(cls, v):
+    def _validate_preview(cls, v):
         if isinstance(v, Preview):
             v = PreviewModel.model_validate(v.__dict__)
         return v
 
     @field_validator("prices", mode="before")
     @classmethod
-    def prices_validator(cls, v):
+    def _validate_prices(cls, v):
         if isinstance(v, Prices):
             v = PricesModel.model_validate(v.__dict__)
         return v
 
     @field_validator("purchase_uris", mode="before")
     @classmethod
-    def purchase_uris_validator(cls, v):
+    def _validate_purchase_uris(cls, v):
         if isinstance(v, PurchaseUris):
             v = PurchaseUrisModel.model_validate(v.__dict__)
         return v
 
     @field_validator("related_uris", mode="before")
     @classmethod
-    def related_uris_validator(cls, v):
+    def _validate_related_uris(cls, v):
         if isinstance(v, RelatedUris):
             v = RelatedUrisModel.model_validate(v.__dict__)
         return v
 
+    @field_validator("produced_mana", mode="wrap")
+    def _validate_produced_mana(cls, val: Any | None, next_: Callable[[Any], Any], ctx: ValidationInfo) -> Any:
+        """
+        Skip validation for exceptional cards.
+        """
+
+        # Sole Performer has `produced_mana = ["T"]`, so we won't validate it.
+        if ctx.data.get("name") == "Sole Performer":
+            logger.info("Skipping field validation for 'produced_mana' for Sole Performer.")
+            return None
+
+        return next_(val)
+
     # endregion
 
     # region Serializers
 
     @field_serializer("released_at")
-    def serialize_date(self, dt_field: date):
+    def _serialize_date(self, dt_field: date):
         return super().serialize_date(dt_field=dt_field)
 
     @field_serializer(
         "attraction_lights",
         "color_identity",
         "color_indicator",
         "colors",
         "finishes",
         "frame_effects",
         "games",
         "keywords",
         "produced_mana",
         "promo_types",
     )
-    def serialize_set(self, set_field: set[Any]):
+    def _serialize_set(self, set_field: set[Any]):
         return super().serialize_set(set_field=set_field)
 
     # endregion
 
     # TODO(#46): add Card field validators
 
 
-def encode_date(dt: date):
-    return dt.strftime(format=DATE_FORMAT)
-
-
 class CardModel(ScoozeDocument, CardModelData):
     """
     A database representation of a scooze Card.
     """
 
     model_config = ConfigDict(
         json_schema_extra={
```

### Comparing `scooze-1.0.7/src/scooze/models/cardparts.py` & `scooze-2.0.0/src/scooze/models/cardparts.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -173,14 +173,42 @@
         if isinstance(v, ImageUris):
             v = ImageUrisModel.model_validate(v.__dict__)
         return v
 
     # endregion
 
 
+class PreviewModel(ScoozeBaseModel):
+    """
+    A model for information about where and when a card was previewed.
+
+    Attributes:
+        previewed_at: Date/time of preview being shown or added to Scryfall.
+        source: Name of preview source.
+        source_uri: Location of preview source.
+    """
+
+    previewed_at: date | None = Field(
+        default=None,
+        description="Date/time of preview being shown or added to Scryfall.",
+    )
+    source: str | None = Field(
+        default=None,
+        description="Name of preview source.",
+    )
+    source_uri: str | None = Field(
+        default=None,
+        description="Location of preview source.",
+    )
+
+    @field_serializer("previewed_at")
+    def serialize_date(self, dt_field: date):
+        return super().serialize_date(dt_field=dt_field)
+
+
 class PricesModel(ScoozeBaseModel):
     """
     A model for all price data associated with a `CardModel`.
 
     Attributes:
         usd: Price in US dollars, from TCGplayer.
         usd_foil: Foil price in US dollars, from TCGplayer.
@@ -212,42 +240,14 @@
     )
     tix: float | None = Field(
         default=None,
         description="Price in MTGO tix, from Cardhoarder.",
     )
 
 
-class PreviewModel(ScoozeBaseModel):
-    """
-    A model for information about where and when a card was previewed.
-
-    Attributes:
-        previewed_at: Date/time of preview being shown or added to Scryfall.
-        source: Name of preview source.
-        source_uri: Location of preview source.
-    """
-
-    previewed_at: date | None = Field(
-        default=None,
-        description="Date/time of preview being shown or added to Scryfall.",
-    )
-    source: str | None = Field(
-        default=None,
-        description="Name of preview source.",
-    )
-    source_uri: str | None = Field(
-        default=None,
-        description="Location of preview source.",
-    )
-
-    @field_serializer("previewed_at")
-    def serialize_date(self, dt_field: date):
-        return super().serialize_date(dt_field=dt_field)
-
-
 class PurchaseUrisModel(ScoozeBaseModel):
     """
     URIs to this card's listings on major marketplaces.
 
     Attributes:
         tcgplayer: Link to buy this card on the TCGplayer marketplace.
         cardmarket: Link to buy this card on the Cardmarket marketplace.
```

### Comparing `scooze-1.0.7/src/scooze/models/deck.py` & `scooze-2.0.0/src/scooze/models/deck.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,58 @@
 from collections import Counter
 from datetime import date
 
-from pydantic import Field, model_validator
+from pydantic import ConfigDict, Field, field_serializer, model_validator
 from scooze.catalogs import Format
-from scooze.models.utils import ObjectIdT, ScoozeBaseModel
-from scooze.utils import cmdr_size, main_size, side_size
+from scooze.enums import DbCollection
+from scooze.models.utils import ObjectIdT, ScoozeBaseModel, ScoozeDocument
+from scooze.utils import cmdr_size, encode_date, main_size, side_size
 
 
-class DeckModel(ScoozeBaseModel):
+class DeckModelData(ScoozeBaseModel):
     """
-    A model to represent a deck of Magic: the Gathering cards.
+    A data model to represent a deck of Magic: the Gathering cards.
 
     Attributes:
         archetype: The archetype of this DeckModel.
         format: The format legality of the cards in this DeckModel.
         date_played: The date this DeckModel was played.
         main: The main deck. Typically 60 cards minimum.
         side: The sideboard. Typically 15 cards maximum.
         cmdr: The command zone. Typically 1 or 2 cards in Commander formats.
+        TODO(#273): Add attraction and sticker decks to Deck model.
     """
 
-    model_config = ScoozeBaseModel.model_config.copy()
-    model_config["json_schema_extra"] = {
-        "examples": [
-            {
-                "archetype": "scooze Deck Example",
-                "format": "Limited",
-                "main": {
-                    "6502bf99532dd43b31e6055a": 4,  # TODO(#6): replace with Python scooze id
-                    "6502bf77bffae3b433093dcb": 4,  # TODO(#6): replace with Scavenging Ooze scooze id
-                },
-                "side": {
-                    "6502bfe2e0e370d002c87ceb": 1,  # TODO(#6): replace with Keruga scooze id
-                },
-            },
-        ]
-    }
-
     archetype: str = Field(
         default="",
         description="The archetype of this Deck.",
     )
     format: Format = Field(
         default=Format.NONE,
         description="The format of the tournament where this Deck was played.",
     )
     date_played: date = Field(
         default=None,
         description="The date this Deck was played.",
     )
     main: Counter[ObjectIdT] = Field(
-        default=Counter(),
+        default=Counter[ObjectIdT](),
         description="The main deck. Typically 60 cards minimum.",
     )
     side: Counter[ObjectIdT] = Field(
-        default=Counter(),
+        default=Counter[ObjectIdT](),
         description="The sideboard. Typically 15 cards maximum.",
     )
     cmdr: Counter[ObjectIdT] = Field(
-        default=Counter(),
+        default=Counter[ObjectIdT](),
         description="The command zone. Typically 1 or 2 cards in Commander formats.",
     )
 
+    # TODO(#273): Add attraction and sticker decks to Deck model.
+
     # region Validators
 
     # TODO(#49): add validation for fields
 
     @model_validator(mode="after")
     def validate_main(self):
         m_min, m_max = main_size(self.format)
@@ -103,30 +90,49 @@
             )
         elif self.cmdr.total() > c_max:
             raise ValueError(
                 f"Too many cards in command zone. Provided command zone has {self.cmdr.total()} cards. Expected at most {c_max}."
             )
         return self
 
+    # TODO(#273): Add attraction and sticker deck validators.
+
     # endregion
 
+    # region Serializers
 
-class DeckModelIn(DeckModel):
-    """
-    A Deck model to be passed to the database.
-    """
+    @field_serializer("date_played")
+    def serialize_date(self, dt_field: date):
+        return super().serialize_date(dt_field=dt_field)
 
-    pass
+    # endregion
 
 
-class DeckModelOut(DeckModel):
+class DeckModel(ScoozeDocument, DeckModelData):
     """
-    A Deck model to be retrieved from the database.
-
-    Attributes:
-        id: A UUID for this deck in the database.
+    Database representation of a scooze Deck.
     """
 
-    id: ObjectIdT = Field(
-        default=None,
-        alias="_id",
+    model_config = ConfigDict(
+        json_schema_extra={
+            "examples": [
+                {
+                    "archetype": "Example Deck",
+                    "format": "Limited",
+                    "main": {
+                        "6502bf99532dd43b31e6055a": 4,  # TODO(#6): replace with Python scooze id
+                        "6502bf77bffae3b433093dcb": 4,  # TODO(#6): replace with Scavenging Ooze scooze id
+                    },
+                    "side": {
+                        "6502bfe2e0e370d002c87ceb": 1,  # TODO(#6): replace with Keruga scooze id
+                    },
+                },
+            ]
+        }
     )
+
+    class Settings:
+        name = DbCollection.DECKS
+        validate_on_save = True
+        bson_encoders = {
+            date: encode_date,
+        }
```

### Comparing `scooze-1.0.7/src/scooze/models/utils.py` & `scooze-2.0.0/src/scooze/models/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,14 @@
 from beanie import Document, PydanticObjectId
 from bson import ObjectId as BsonObjectId
 from pydantic import BaseModel, ConfigDict, Field, GetJsonSchemaHandler
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import CoreSchema, core_schema
 from scooze.utils import DATE_FORMAT, to_lower_camel
 
-# region Private Utility Functions
-
-
-# endregion
-
-
 # region Public Utility Classes
 
 
 class ScoozeDocument(Document):
     """
     A simple base Beanie Document class to support models in scooze.
```

### Comparing `scooze-1.0.7/src/scooze/routers/card.py` & `scooze-2.0.0/src/scooze/routers/card.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from http import HTTPStatus
+
 from beanie import PydanticObjectId
 from bson.errors import InvalidId
 from fastapi import APIRouter, Depends
 from fastapi.exceptions import HTTPException
 from fastapi.responses import JSONResponse
 from scooze.models.card import CardModel, CardModelData
 
 router = APIRouter(
     prefix="/card",
     tags=["card"],
-    responses={404: {"description": "Card Not Found"}},
+    responses={HTTPStatus.NOT_FOUND: {"description": "Card Not Found"}},
 )
 
 
 def _validate_card_id(card_id: str) -> PydanticObjectId:
     """
     Helper to validate incoming strings as card IDs
 
@@ -25,15 +27,15 @@
     Raises:
         HTTPException: 422 - String was not a valid id.
     """
 
     try:
         return PydanticObjectId(card_id)
     except InvalidId:
-        raise HTTPException(status_code=422, detail="Must give a valid ID.")
+        raise HTTPException(status_code=HTTPStatus.UNPROCESSABLE_ENTITY, detail="Must give a valid ID.")
 
 
 @router.get("/", summary="Get a card at random")
 async def card_root() -> CardModel:
     """
     Get a random card from the database.
 
@@ -42,16 +44,16 @@
 
     Raises:
         HTTPException: 404 - No cards found in the database.
     """
 
     cards = await CardModel.aggregate([{"$sample": {"size": 1}}], projection_model=CardModel).to_list()
 
-    if cards is None or len(cards) == 0:
-        raise HTTPException(status_code=404, detail="No cards found in the database.")
+    if cards is None or not cards:
+        raise HTTPException(status_code=HTTPStatus.NOT_FOUND, detail="No cards found in the database.")
 
     return cards[0]
 
 
 # Create
 
 
@@ -72,15 +74,15 @@
 
     try:
         # NOTE: would like to add the dupe protection back in
         card = CardModel.model_validate(card_data.model_dump())
 
         return await card.create()
     except Exception as e:
-        raise HTTPException(status_code=400, detail=f"Failed to create a new card. Error: {e}")
+        raise HTTPException(status_code=HTTPStatus.BAD_REQUEST, detail=f"Failed to create a new card. Error: {e}")
 
 
 # Read
 
 
 @router.get("/id/{card_id}", summary="Get a card by ID")
 async def get_card_by_id(card_id: PydanticObjectId = Depends(_validate_card_id)) -> CardModel:
@@ -97,15 +99,15 @@
         HTTPException: 404 - Card wasn't found.
         HTTPException: 422 - Bad ID given.
     """
 
     card = await CardModel.get(card_id)
 
     if card is None:
-        raise HTTPException(status_code=404, detail=f"Card with ID {card_id} not found.")
+        raise HTTPException(status_code=HTTPStatus.NOT_FOUND, detail=f"Card with ID {card_id} not found.")
 
     return card
 
 
 @router.get("/name/{card_name}", summary="Get a card by name")
 async def get_card_by_name(card_name: str) -> CardModel:
     """
@@ -122,15 +124,15 @@
     Raises:
         HTTPException: 404 - Card wasn't found.
     """
 
     card = await CardModel.find_one({"name": card_name})
 
     if card is None:
-        raise HTTPException(status_code=404, detail=f"Card with name '{card_name}' not found.")
+        raise HTTPException(status_code=HTTPStatus.NOT_FOUND, detail=f"Card with name '{card_name}' not found.")
 
     return card
 
 
 # Update
 
 
@@ -151,27 +153,27 @@
 
     Raises:
         HTTPException: 404 - Card wasn't found, pre-update.
         HTTPException: 404 - Card wasn't found, post-update.
         HTTPException: 422 - Bad ID given.
     """
 
-    field_updates = {k: v for k, v in card_req.dict().items() if v is not None}
+    field_updates = {k: v for k, v in card_req.model_dump().items() if v is not None}
     card = await CardModel.get(card_id)
 
     if card is None:
-        raise HTTPException(status_code=404, detail=f"Card with ID {card_id} not found.")
+        raise HTTPException(status_code=HTTPStatus.NOT_FOUND, detail=f"Card with ID {card_id} not found.")
 
     # NOTE: This could be slightly less verbose by chaining a la CardModel.get().update() but
     # the typing gets weird from things on Beanie's end so I broke it up like this
     _ = await card.set(field_updates)
     updated_card = await CardModel.get(card_id)
 
     if updated_card is None:
-        raise HTTPException(status_code=404, detail=f"Card with ID {card_id} not found post-update.")
+        raise HTTPException(status_code=HTTPStatus.NOT_FOUND, detail=f"Card with ID {card_id} not found post-update.")
 
     return updated_card
 
 
 # Delete
 
 
@@ -191,15 +193,15 @@
         HTTPException: 404 - Card wasn't found.
         HTTPException: 422 - Bad ID given.
     """
 
     card_to_delete = await CardModel.get(card_id)
 
     if card_to_delete is None:
-        raise HTTPException(status_code=404, detail=f"Card with ID {card_id} not found.")
+        raise HTTPException(status_code=HTTPStatus.NOT_FOUND, detail=f"Card with ID {card_id} not found.")
 
     delete_result = await card_to_delete.delete()
 
     if delete_result is None:
-        raise HTTPException(status_code=400, detail=f"Card with ID {card_id} not deleted.")
+        raise HTTPException(status_code=HTTPStatus.BAD_REQUEST, detail=f"Card with ID {card_id} not deleted.")
 
     return JSONResponse(f"Card with ID {card_id} deleted.")
```

### Comparing `scooze-1.0.7/src/scooze/routers/cards.py` & `scooze-2.0.0/src/scooze/routers/cards.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,42 @@
+from http import HTTPStatus
 from typing import Any
 
 from beanie import PydanticObjectId
 from fastapi import APIRouter, HTTPException
 from fastapi.responses import JSONResponse
 from scooze.models.card import CardModel, CardModelData
 from scooze.utils import to_lower_camel
 
 router = APIRouter(
     prefix="/cards",
     tags=["cards"],
-    responses={404: {"description": "Cards Not Found"}},
+    responses={HTTPStatus.NOT_FOUND: {"description": "Cards Not Found"}},
 )
 
 
 @router.get("/", summary="Get cards at random")
 async def cards_root(limit: int = 3) -> list[CardModel]:
     """
-    Get a random card from the database.
+    Get random cards from the database.
 
     Args:
         limit: The maximum number of cards to get.
 
     Returns:
         Random cards from the database.
 
     Raises:
         HTTPException: 404 - No cards found in the database.
     """
 
     cards = await CardModel.aggregate([{"$sample": {"size": limit}}], projection_model=CardModel).to_list()
 
-    if cards is None or len(cards) == 0:
-        raise HTTPException(status_code=404, detail="No cards found in the database.")
+    if cards is None or not cards:
+        raise HTTPException(status_code=HTTPStatus.NOT_FOUND, detail="No cards found in the database.")
 
     return cards
 
 
 # Create
 
 
@@ -51,19 +52,19 @@
         A message stating how many cards were created.
 
     Raises:
         HTTPException: 400 - Create failed, passes along the error message.
     """
 
     try:
-        cards_to_insert = [CardModel.model_validate(card.model_dump(mode="json", by_alias=True)) for card in cards]
+        cards_to_insert = [CardModel.model_validate(card.model_dump()) for card in cards]
         insert_result = await CardModel.insert_many(cards_to_insert)
         return JSONResponse(f"Created {len(insert_result.inserted_ids)} card(s).")
     except Exception as e:
-        raise HTTPException(status_code=400, detail=f"Failed to create new cards. Error: {e}")
+        raise HTTPException(status_code=HTTPStatus.BAD_REQUEST, detail=f"Failed to create new cards. Error: {e}")
 
 
 # Read
 
 
 @router.post("/by", summary="Get cards by property")
 async def get_cards_by(
@@ -74,40 +75,40 @@
     page_size: int = 10,
 ) -> list[CardModel]:
     """
     Get cards where the given property matches any of the given values.
 
     Args:
         property_name: The property to check against.
-        values: Matching values for the given property
-        paginated: Return paginated results if True, or all matches if False
+        values: Matching values for the given property.
+        paginated: Return paginated results if True, or all matches if False.
         page: The page to return matches from.
         page_size: The number of results per page.
 
     Returns:
         A list of cards matching the search criteria.
 
     Raises:
         HTTPException: 404 - Cards weren't found.
     """
 
     match property_name:
         case "_id" | "id":
             prop_name = "_id"
-            vals = [PydanticObjectId(v) for v in values]  # Normalize Mongo ids
+            vals = [PydanticObjectId(v) for v in values]  # Normalize Mongo IDs
         case _:
             prop_name = to_lower_camel(property_name)
             vals = values
 
     skip = (page - 1) * page_size if paginated else 0
     limit = page_size if paginated else None
     cards = await CardModel.find({"$or": [{prop_name: v} for v in vals]}, skip=skip, limit=limit).to_list()
 
     if len(cards) == 0:
-        raise HTTPException(status_code=404, detail="Cards not found.")
+        raise HTTPException(status_code=HTTPStatus.NOT_FOUND, detail="Cards not found.")
 
     return cards
 
 
 # Delete
 
 
@@ -122,10 +123,10 @@
     Raises:
         HTTPException: 400 - Cards weren't deleted.
     """
 
     delete_result = await CardModel.delete_all()
 
     if delete_result is None:
-        raise HTTPException(status_code=400, detail="Cards weren't deleted.")
+        raise HTTPException(status_code=HTTPStatus.BAD_REQUEST, detail="Cards weren't deleted.")
 
     return JSONResponse(f"Deleted {delete_result.deleted_count} card(s).")
```

### Comparing `scooze-1.0.7/src/scooze/utils.py` & `scooze-2.0.0/src/scooze/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,149 @@
+import datetime as dt
+import json
 import logging
 import re
 from collections import Counter
 from datetime import date, datetime
-from enum import Enum, EnumMeta
+from logging.handlers import RotatingFileHandler
 from sys import maxsize
 from typing import Any, Hashable, Iterable, Mapping, Self, Type, TypeVar
 
 from frozendict import frozendict
 from pydantic.alias_generators import to_camel
 from scooze.catalogs import CostSymbol, Format
-from scooze.enum import ExtendedEnum
-
-DEFAULT_BULK_FILE_DIR = "./data/bulk"
-DEFAULT_DECKS_DIR = "./data/decks"
+from scooze.config import CONFIG
+from scooze.enums import ExtendedEnum
 
 ## Generic Types
 T = TypeVar("T")  # generic type
 V = TypeVar("V")  # generic value type
 E = TypeVar("E", bound=ExtendedEnum)  # generic Enum type
 N = TypeVar("N", bound=ExtendedEnum)  # generic Enum (for mapping values) type
 FloatableT = TypeVar("FloatableT", float, int, str)  # type that can normalize to float
 
-
 ## String formatting
 DATE_FORMAT = "%Y-%m-%d"
 
+# region Logging Utils
 
-def to_lower_camel(string: str) -> str:
-    if len(string.split("_")) == 1:
-        return string
-
-    return to_camel(string)
+# NOTE: LogRecord objects. Subject to change; see https://docs.python.org/3/library/logging.html#logrecord-objects
+LOG_RECORD_BUILTIN_ATTRS = {
+    "args",
+    "asctime",
+    "created",
+    "exc_info",
+    "exc_text",
+    "filename",
+    "funcName",
+    "levelname",
+    "levelno",
+    "lineno",
+    "module",
+    "msecs",
+    "message",
+    "msg",
+    "name",
+    "pathname",
+    "process",
+    "processName",
+    "relativeCreated",
+    "stack_info",
+    "thread",
+    "threadName",
+    "taskName",
+}
+
+
+class ScoozeRotatingFileHandler(RotatingFileHandler):
+    """
+    Simple RotatingFileHandler that writes to the home directory.
+    """
+
+    def __init__(
+        self,
+        filename: str,
+        mode: str = "a",
+        maxBytes: int = 0,
+        backupCount: int = 0,
+        encoding: str | None = None,
+        delay: bool = False,
+        errors: str | None = None,
+    ):
+        path = CONFIG.logs_dir
+        path.mkdir(parents=True, exist_ok=True)
+        super(ScoozeRotatingFileHandler, self).__init__(
+            filename=path / filename,
+            mode=mode,
+            maxBytes=maxBytes,
+            backupCount=backupCount,
+            encoding=encoding,
+            delay=delay,
+            errors=errors,
+        )
 
 
-def scooze_logger() -> logging.Logger:
+class JsonLoggingFormatter(logging.Formatter):
     """
-    Helper function to get the scooze logger.
-
-    Use the default logging functionality here without any filters, formatters,
-    or handlers, so users can make informed decisions about their own logging.
+    Simple logging Formatter to generate json lines output.
     """
 
-    return logging.getLogger("scooze")
+    def __init__(self, *, fmt_keys: dict[str, str] | None = None):
+        super().__init__()
+        self.fmt_keys = fmt_keys if fmt_keys is not None else {}
+
+    # TODO(py3.12): Python 3.12 typing has an override wrapper
+    # @override
+    def format(self, record: logging.LogRecord) -> str:
+        message = self._prepare_log_dict(record)
+        return json.dumps(message, default=str)
+
+    def _prepare_log_dict(self, record: logging.LogRecord):
+        always_fields = {
+            "message": record.getMessage(),
+            "timestamp": dt.datetime.fromtimestamp(record.created, tz=dt.timezone.utc).isoformat(),
+        }
+
+        if record.exc_info is not None:
+            always_fields["exc_info"] = self.formatException(record.exc_info)
+
+        if record.stack_info is not None:
+            always_fields["stack_info"] = self.formatStack(record.stack_info)
+
+        # fmt: off
+        # disable black formatter
+        message = {
+            key: msg_val
+            if (msg_val := always_fields.pop(val, None)) is not None
+            else getattr(record, val)
+            for key, val in self.fmt_keys.items()
+        }
+        # fmt: on
+        message.update(always_fields)
+
+        # Handle extras
+        for key, val in record.__dict__.items():
+            if key not in LOG_RECORD_BUILTIN_ATTRS:
+                message[key] = val
+
+        return message
+
+
+# endregion
+
+
+def encode_date(dt: date) -> str:
+    return dt.strftime(format=DATE_FORMAT)
+
+
+def to_lower_camel(string: str) -> str:
+    if len(string.split("_")) == 1:
+        return string
+
+    return to_camel(string)
 
 
 # region Deck Format Helpers
 
 
 def max_relentless_quantity(name: str) -> int:
     """
@@ -341,17 +439,39 @@
 
         case Format.LIMITED | Format.NONE | _:
             return 0, maxsize
 
 
 # endregion
 
+# region Symbology utils
+
+
+def parse_symbols(cost: str) -> Counter[CostSymbol]:
+    """
+    Parse a string containing one or more cost symbols, in standard oracle text form (e.g. "{4}{G}").
+
+    Args:
+        cost: String representing a mana cost, or rules text that may have one or more symbols.
+
+    Returns:
+        A mapping of cost symbols to the number of times they appear in that string.
+    """
+
+    # find all symbols of form {W}, {W/P}, etc
+    symbols = [CostSymbol(s) for s in re.findall(r"{([^}]+)}", cost)]
+    return Counter[CostSymbol](symbols)
+
+
+# endregion
+
 
 # region Helper Classes
 
+
 # region Base Classes
 
 
 class ComparableObject:
     """
     A simple base class to support comparable objects.
     """
@@ -558,28 +678,7 @@
         return self.contents == {}
 
 
 # endregion
 
 
 # endregion
-
-# region Symbology utils
-
-
-def parse_symbols(cost: str) -> Counter[CostSymbol]:
-    """
-    Parse a string containing one or more cost symbols, in standard oracle text form (e.g. "{4}{G}").
-
-    Args:
-        cost: String representing a mana cost, or rules text that may have one or more symbols.
-
-    Returns:
-        A mapping of cost symbols to the number of times they appear in that string.
-    """
-
-    # find all symbols of form {W}, {W/P}, etc
-    symbols = [CostSymbol(s) for s in re.findall("{([^}]+)}", cost)]
-    return Counter(symbols)
-
-
-# endregion
```

### Comparing `scooze-1.0.7/PKG-INFO` & `scooze-2.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,68 @@
 Metadata-Version: 2.1
 Name: scooze
-Version: 1.0.7
-Summary: A flexible data layer for applications working with Magic: the Gathering cards, decks, and tournaments.
+Version: 2.0.0
+Summary: A flexible data layer for applications working with Magic: the Gathering cards and decks.
 Author: Alexander Gimmi
 Author-email: iambroadband@gmail.com
 Requires-Python: >=3.11,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beanie (>=1.23.0,<2.0.0)
 Requires-Dist: cleo (>=2.0.1,<3.0.0)
-Requires-Dist: docker (>=6.1.3,<7.0.0)
 Requires-Dist: fastapi (>=0.100.0,<1.0.0)
 Requires-Dist: frozendict (>=2.3.8,<3.0.0)
 Requires-Dist: ijson (>=3.2.3,<4.0.0)
 Requires-Dist: motor (>=3.2.0,<4.0.0)
-Requires-Dist: pydantic (>=2.0.0,<3.0.0)
+Requires-Dist: pydantic (>=2.0.0)
 Requires-Dist: pydantic-settings (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: setuptools (>=68.2.2,<69.0.0)
 Requires-Dist: uvicorn[standard] (>=0.23.1,<0.24.0)
 Project-URL: documentation, https://scooze.readthedocs.io
 Project-URL: homepage, https://github.com/arcavios/scooze
 Project-URL: repository, https://github.com/arcavios/scooze
 Description-Content-Type: text/markdown
 
 # scooze
 
-[![CI](https://img.shields.io/github/actions/workflow/status/arcavios/scooze/pytest.yml?branch=dev&logo=github&label=CI)](https://github.com/arcavios/scooze/actions?query=event%3Apush+branch%3Adev+workflow%3Apytest)
+[![CI](https://img.shields.io/github/actions/workflow/status/arcavios/scooze/ci.yml?branch=dev&logo=github&label=CI)](https://github.com/arcavios/scooze/actions?query=event%3Apush+branch%3Adev+workflow%3A%22Continuous+Integration%22)
 [![pypi](https://img.shields.io/pypi/v/scooze.svg)](https://pypi.python.org/pypi/scooze)
 [![versions](https://img.shields.io/pypi/pyversions/scooze.svg)](https://github.com/arcavios/scooze)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://github.com/arcavios/scooze/blob/dev/LICENSE)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
 
-A flexible data layer for applications working with Magic: the Gathering cards, decks, and tournaments.
+A flexible data layer for applications working with Magic: the Gathering cards and decks.
 
 ## Features
 
-📊 Robust data models for representing Magic: the Gathering cards, decks, and tournaments
+📊 Robust data models for representing Magic: the Gathering cards and decks
 
 - Cards - follows the Scryfall standard
 - Decks - main deck/sideboard/command zone, format legality, average words, and more
-- Tournaments - coming soon!
 
 🎛️ CLI to manage a local database of [Scryfall](https://scryfall.com/docs/api/bulk-data) data
 
 🐍 Python and REST APIs for interacting with the scooze database
 
 ## Help
 
-See our [documentation](https://scooze.readthedocs.io/en/latest) for more information.
+The source code can be found [here](https://github.com/arcavios/scooze).
+
+See our [documentation](https://scooze.readthedocs.io/en/stable/) for more information.
 
 ## Installation
 
-Install using `pip install scooze`. For more installation options, see the [Install](https://scooze.readthedocs.io/en/latest/installation) section in the documentation.
+Install using `pip install scooze`. For more installation options, see the [Install](https://scooze.readthedocs.io/en/stable/installation) section in the documentation.
 
 ## A Simple Example
 
 ``` python
-from scooze.card import Card
-from scooze.deck import Deck, InThe
-from scooze.catalogs import Format
+from scooze import Card, Deck, Format, InThe
 
 deck = Deck()
 card1 = Card("Python")
 card2 = Card("Anaconda")
 swamp = Card("Swamp")
 
 deck.add_card(card1, 25)
@@ -80,19 +79,19 @@
 15 Swamp
 
 Sideboard:
 100 Anaconda
 """
 ```
 
-See [Setup](https://scooze.readthedocs.io/en/latest/setup/) and our [API Documentation](https://scooze.readthedocs.io/en/latest/dataclasses/card/) for more details.
+See [Setup](https://scooze.readthedocs.io/en/stable/setup/) and our [API Documentation](https://scooze.readthedocs.io/en/stable/dataclasses/card/) for more details.
 
 ## Contributing
 
-For guidance on setting up a development environment and how to make a contribution to scooze, see [Contributing to scooze](https://scooze.readthedocs.io/en/latest/contributing).
+For guidance on setting up a development environment and how to make a contribution to scooze, see [Contributing to scooze](https://scooze.readthedocs.io/en/stable/contributing).
 
 ## Report a Bug
 
 If you find a bug 🐛 please open a [bug report](https://github.com/arcavios/scooze/issues/new?assignees=&labels=bug&template=bug_report.md&title=). If you have an idea for an improvement or new feature 🚀 please open a [feature request](https://github.com/arcavios/scooze/issues/new?assignees=&labels=enhancement&template=feature_request.md&title=).
 
 If you find a security vulnerability, please follow the instructions [here](https://github.com/arcavios/scooze/security/policy).
```

