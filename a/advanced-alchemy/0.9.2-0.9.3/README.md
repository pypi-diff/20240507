# Comparing `tmp/advanced_alchemy-0.9.2.tar.gz` & `tmp/advanced_alchemy-0.9.3.tar.gz`

## Comparing `advanced_alchemy-0.9.2.tar` & `advanced_alchemy-0.9.3.tar`

### file list

```diff
@@ -1,198 +1,198 @@
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.sourcery.yaml
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/Makefile
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/codecov.yml
--rw-r--r--   0        0        0   350525 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/pdm.lock
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/sonar-project.properties
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.github/dependabot.yaml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.github/workflows/docs-preview.yml
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.github/workflows/pr-title.yml
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/__init__.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/__metadata__.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/_listeners.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/_serialization.py
--rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/base.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/exceptions.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/filters.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/operations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/__init__.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/commands.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/asyncio/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/asyncio/alembic.ini.mako
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/asyncio/env.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/asyncio/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/sync/__init__.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/sync/alembic.ini.mako
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/sync/env.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/sync/script.py.mako
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/config/__init__.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/config/asyncio.py
--rw-r--r--   0        0        0    10651 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/config/common.py
--rw-r--r--   0        0        0    11108 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/config/engine.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/config/sync.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/__init__.py
--rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/sanic.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/starlette.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/__init__.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/_utils.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/alembic.py
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/cli.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/dto.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/__init__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/_slots_base.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/serialization.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/__init__.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/plugin.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/config/__init__.py
--rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/config/common.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/config/engine.py
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/config/sync.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/mixins/__init__.py
--rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/mixins/unique.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/repository/__init__.py
--rw-r--r--   0        0        0    64625 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/repository/_async.py
--rw-r--r--   0        0        0    63981 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/repository/_sync.py
--rw-r--r--   0        0        0    10853 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/repository/_util.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/repository/typing.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/repository/memory/__init__.py
--rw-r--r--   0        0        0    19775 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/repository/memory/_async.py
--rw-r--r--   0        0        0    19591 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/repository/memory/_sync.py
--rw-r--r--   0        0        0    11955 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/repository/memory/base.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/service/__init__.py
--rw-r--r--   0        0        0    29109 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/service/_async.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/service/_converters.py
--rw-r--r--   0        0        0    28761 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/service/_sync.py
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/service/_util.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/service/pagination.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/service/typing.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/types/__init__.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/types/datetime.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/types/encrypted_string.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/types/guid.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/types/identity.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/types/json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/utils/__init__.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/utils/dataclass.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/utils/deprecation.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/utils/fixtures.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/advanced_alchemy/utils/text.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/Makefile
--rw-r--r--   0        0        0    86654 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/changelog.rst
--rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/conf.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/contribution-guide.rst
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/fix_missing_references.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/getting-started.rst
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/index.rst
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/releases.rst
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/_static/css/style.css
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/_static/css/versioning.js
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/_static/css/versions.json
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/base.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/exceptions.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/filters.rst
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/index.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/operations.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/repository.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/service.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/types.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/utils.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/alembic/commands.rst
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/alembic/index.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/alembic/templates/asyncio/alembic-ini.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/alembic/templates/asyncio/env.rst
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/alembic/templates/asyncio/index.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/alembic/templates/asyncio/script-py.rst
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/alembic/templates/sync/alembic-ini.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/alembic/templates/sync/env.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/alembic/templates/sync/index.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/alembic/templates/sync/script-py.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/config/asyncio.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/config/common.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/config/engine.rst
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/config/index.rst
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/config/sync.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/config/types.rst
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/index.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/sanic.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/starlette.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/alembic.rst
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/cli.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/dto.rst
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/index.rst
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/plugins/index.rst
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/plugins/serialization.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/plugins/init/plugin.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/plugins/init/config/asyncio.rst
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/plugins/init/config/common.rst
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/plugins/init/config/engine.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/plugins/init/config/sync.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/extensions/litestar/plugins/init/config/types.rst
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/mixins/index.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/reference/mixins/unique.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/usage/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/docs/usage/placeholder.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/examples/__init__.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/examples/fastapi.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/examples/flask.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/examples/sanic.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/examples/standalone.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/examples/standalone_json.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/examples/us_state_lookup.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/examples/litestar/__init__.py
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/examples/litestar/litestar_repo_only.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/examples/litestar/litestar_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/docker-compose.yml
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/docker_service_fixtures.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/helpers.py
--rw-r--r--   0        0        0    15780 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/models_bigint.py
--rw-r--r--   0        0        0    15438 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/models_uuid.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/integration/__init__.py
--rw-r--r--   0        0        0    16718 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/integration/conftest.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/integration/helpers.py
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/integration/test_alembic_commands.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/integration/test_lambda_stmt.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/integration/test_oracledb_json.py
--rw-r--r--   0        0        0    95759 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/integration/test_repository.py
--rw-r--r--   0        0        0     7278 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/integration/test_sqlquery_service.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/integration/test_unique_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/__init__.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_exceptions.py
--rw-r--r--   0        0        0    31969 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/__init__.py
--rw-r--r--   0        0        0     8694 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_sanic.py
--rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_starlette.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/__init__.py
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/conftest.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_context.py
--rw-r--r--   0        0        0    21775 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_dto.py
--rw-r--r--   0        0        0    21538 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_dto_integration.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_litestar_re_exports.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_serialization_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_init_plugin/__init__.py
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_init_plugin/test_asyncio.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_init_plugin/test_common.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_init_plugin/test_engine.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_init_plugin/test_sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_utils/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tests/unit/test_utils/test_text.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tools/build_docs.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/tools/convert_docs.sh
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/LICENSE
--rw-r--r--   0        0        0    19716 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/README.md
--rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    21919 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.sourcery.yaml
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/Makefile
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/codecov.yml
+-rw-r--r--   0        0        0   350525 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/pdm.lock
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/sonar-project.properties
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.github/dependabot.yaml
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.github/workflows/docs-preview.yml
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.github/workflows/pr-title.yml
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/__init__.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/__metadata__.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/_listeners.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/_serialization.py
+-rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/base.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/exceptions.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/filters.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/operations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/__init__.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/commands.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/asyncio/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/asyncio/alembic.ini.mako
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/asyncio/env.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/asyncio/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/sync/__init__.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/sync/alembic.ini.mako
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/sync/env.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/sync/script.py.mako
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/config/__init__.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/config/asyncio.py
+-rw-r--r--   0        0        0    10651 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/config/common.py
+-rw-r--r--   0        0        0    11108 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/config/engine.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/config/sync.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/__init__.py
+-rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/sanic.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/starlette.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/__init__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/_utils.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/alembic.py
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/cli.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/dto.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/_slots_base.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/serialization.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/__init__.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/plugin.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/config/common.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/config/engine.py
+-rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/config/sync.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/mixins/unique.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/repository/__init__.py
+-rw-r--r--   0        0        0    64625 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/repository/_async.py
+-rw-r--r--   0        0        0    63981 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/repository/_sync.py
+-rw-r--r--   0        0        0    10853 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/repository/_util.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/repository/typing.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/repository/memory/__init__.py
+-rw-r--r--   0        0        0    19775 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/repository/memory/_async.py
+-rw-r--r--   0        0        0    19591 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/repository/memory/_sync.py
+-rw-r--r--   0        0        0    11955 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/repository/memory/base.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/service/__init__.py
+-rw-r--r--   0        0        0    29109 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/service/_async.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/service/_converters.py
+-rw-r--r--   0        0        0    28761 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/service/_sync.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/service/_util.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/service/pagination.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/service/typing.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/types/__init__.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/types/datetime.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/types/encrypted_string.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/types/guid.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/types/identity.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/types/json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/utils/__init__.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/utils/dataclass.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/utils/deprecation.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/utils/fixtures.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/advanced_alchemy/utils/text.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/Makefile
+-rw-r--r--   0        0        0    86654 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/changelog.rst
+-rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/conf.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/contribution-guide.rst
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/fix_missing_references.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/getting-started.rst
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/index.rst
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/releases.rst
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/_static/css/style.css
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/_static/css/versioning.js
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/_static/css/versions.json
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/base.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/exceptions.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/filters.rst
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/index.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/operations.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/repository.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/service.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/types.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/utils.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/alembic/commands.rst
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/alembic/index.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/alembic/templates/asyncio/alembic-ini.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/alembic/templates/asyncio/env.rst
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/alembic/templates/asyncio/index.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/alembic/templates/asyncio/script-py.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/alembic/templates/sync/alembic-ini.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/alembic/templates/sync/env.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/alembic/templates/sync/index.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/alembic/templates/sync/script-py.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/config/asyncio.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/config/common.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/config/engine.rst
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/config/index.rst
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/config/sync.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/config/types.rst
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/index.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/sanic.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/starlette.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/alembic.rst
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/cli.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/dto.rst
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/index.rst
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/plugins/index.rst
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/plugins/serialization.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/plugins/init/plugin.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/plugins/init/config/asyncio.rst
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/plugins/init/config/common.rst
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/plugins/init/config/engine.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/plugins/init/config/sync.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/extensions/litestar/plugins/init/config/types.rst
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/mixins/index.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/reference/mixins/unique.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/usage/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/docs/usage/placeholder.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/examples/__init__.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/examples/fastapi.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/examples/flask.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/examples/sanic.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/examples/standalone.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/examples/standalone_json.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/examples/us_state_lookup.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/examples/litestar/__init__.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/examples/litestar/litestar_repo_only.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/examples/litestar/litestar_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/docker-compose.yml
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/docker_service_fixtures.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/helpers.py
+-rw-r--r--   0        0        0    15780 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/models_bigint.py
+-rw-r--r--   0        0        0    15438 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/models_uuid.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/integration/__init__.py
+-rw-r--r--   0        0        0    16718 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/integration/conftest.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/integration/helpers.py
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/integration/test_alembic_commands.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/integration/test_lambda_stmt.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/integration/test_oracledb_json.py
+-rw-r--r--   0        0        0    95759 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/integration/test_repository.py
+-rw-r--r--   0        0        0     7278 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/integration/test_sqlquery_service.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/integration/test_unique_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_exceptions.py
+-rw-r--r--   0        0        0    31969 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/__init__.py
+-rw-r--r--   0        0        0     8694 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_sanic.py
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_starlette.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/__init__.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/conftest.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_context.py
+-rw-r--r--   0        0        0    21775 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_dto.py
+-rw-r--r--   0        0        0    21538 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_dto_integration.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_litestar_re_exports.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_serialization_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_init_plugin/__init__.py
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_asyncio.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_common.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_engine.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_utils/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tests/unit/test_utils/test_text.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tools/build_docs.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/tools/convert_docs.sh
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/LICENSE
+-rw-r--r--   0        0        0    19716 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/README.md
+-rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    21919 2020-02-02 00:00:00.000000 advanced_alchemy-0.9.3/PKG-INFO
```

### Comparing `advanced_alchemy-0.9.2/.pre-commit-config.yaml` & `advanced_alchemy-0.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/.sourcery.yaml` & `advanced_alchemy-0.9.3/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/CONTRIBUTING.rst` & `advanced_alchemy-0.9.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/Makefile` & `advanced_alchemy-0.9.3/Makefile`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/pdm.lock` & `advanced_alchemy-0.9.3/pdm.lock`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/sonar-project.properties` & `advanced_alchemy-0.9.3/sonar-project.properties`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 sonar.tests=tests
 sonar.coverage.exclusions=\
   **/__init__.py, \
   examples/*.py, \
   tests/*.py, \
   tests/**/*.py, \
   advanced_alchemy/service/_converters.py, \
+  advanced_alchemy/service/_util.py, \
   advanced_alchemy/alembic/templates/asyncio/env.py, \
   advanced_alchemy/alembic/templates/sync/env.py, \
   tests/integration/conftest.py, \
   advanced_alchemy/service/_sync.py, \
   advanced_alchemy/service/_async.py, \
   advanced_alchemy/service/pagination.py, \
   advanced_alchemy/extensions/litestar/plugins/init/config/asyncio.py, \
```

### Comparing `advanced_alchemy-0.9.2/.github/workflows/cd.yml` & `advanced_alchemy-0.9.3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/.github/workflows/ci.yml` & `advanced_alchemy-0.9.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/.github/workflows/codeql.yml` & `advanced_alchemy-0.9.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/.github/workflows/docs-preview.yml` & `advanced_alchemy-0.9.3/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/.github/workflows/docs.yml` & `advanced_alchemy-0.9.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/.github/workflows/publish.yml` & `advanced_alchemy-0.9.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/.github/workflows/test.yml` & `advanced_alchemy-0.9.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/_listeners.py` & `advanced_alchemy-0.9.3/advanced_alchemy/_listeners.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/_serialization.py` & `advanced_alchemy-0.9.3/advanced_alchemy/_serialization.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/base.py` & `advanced_alchemy-0.9.3/advanced_alchemy/base.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/exceptions.py` & `advanced_alchemy-0.9.3/advanced_alchemy/exceptions.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/filters.py` & `advanced_alchemy-0.9.3/advanced_alchemy/filters.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/operations.py` & `advanced_alchemy-0.9.3/advanced_alchemy/operations.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/alembic/commands.py` & `advanced_alchemy-0.9.3/advanced_alchemy/alembic/commands.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/asyncio/alembic.ini.mako` & `advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/asyncio/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/asyncio/env.py` & `advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/asyncio/env.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/asyncio/script.py.mako` & `advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/asyncio/script.py.mako`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/sync/alembic.ini.mako` & `advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/sync/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/sync/env.py` & `advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/sync/env.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/alembic/templates/sync/script.py.mako` & `advanced_alchemy-0.9.3/advanced_alchemy/alembic/templates/sync/script.py.mako`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/config/__init__.py` & `advanced_alchemy-0.9.3/advanced_alchemy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/config/asyncio.py` & `advanced_alchemy-0.9.3/advanced_alchemy/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/config/common.py` & `advanced_alchemy-0.9.3/advanced_alchemy/config/common.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/config/engine.py` & `advanced_alchemy-0.9.3/advanced_alchemy/config/engine.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/config/sync.py` & `advanced_alchemy-0.9.3/advanced_alchemy/config/sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/config/types.py` & `advanced_alchemy-0.9.3/advanced_alchemy/config/types.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/sanic.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/sanic.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/starlette.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/starlette.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/__init__.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/_utils.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/_utils.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/alembic.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/alembic.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/cli.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/cli.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/dto.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/dto.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/__init__.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/serialization.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/serialization.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/plugin.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/plugin.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/config/asyncio.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/config/engine.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/config/engine.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/extensions/litestar/plugins/init/config/sync.py` & `advanced_alchemy-0.9.3/advanced_alchemy/extensions/litestar/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/mixins/unique.py` & `advanced_alchemy-0.9.3/advanced_alchemy/mixins/unique.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/repository/__init__.py` & `advanced_alchemy-0.9.3/advanced_alchemy/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/repository/_async.py` & `advanced_alchemy-0.9.3/advanced_alchemy/repository/_async.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/repository/_sync.py` & `advanced_alchemy-0.9.3/advanced_alchemy/repository/_sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/repository/_util.py` & `advanced_alchemy-0.9.3/advanced_alchemy/repository/_util.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/repository/typing.py` & `advanced_alchemy-0.9.3/advanced_alchemy/repository/typing.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/repository/memory/_async.py` & `advanced_alchemy-0.9.3/advanced_alchemy/repository/memory/_async.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/repository/memory/_sync.py` & `advanced_alchemy-0.9.3/advanced_alchemy/repository/memory/_sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/repository/memory/base.py` & `advanced_alchemy-0.9.3/advanced_alchemy/repository/memory/base.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/service/__init__.py` & `advanced_alchemy-0.9.3/advanced_alchemy/service/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/service/_async.py` & `advanced_alchemy-0.9.3/advanced_alchemy/service/_async.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/service/_converters.py` & `advanced_alchemy-0.9.3/advanced_alchemy/service/_converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 from uuid import UUID
 
 from advanced_alchemy.filters import FilterTypes, LimitOffset
 from advanced_alchemy.repository.typing import ModelT
 from advanced_alchemy.service.pagination import OffsetPagination
 
 if TYPE_CHECKING:
-    from sqlalchemy import ColumnElement, RowMapping
-    from sqlalchemy.orm import DeclarativeBase
+    from sqlalchemy import ColumnElement
 
-    from advanced_alchemy.service.typing import FilterTypeT, ModelDTOT
+    from advanced_alchemy.service.typing import FilterTypeT, ModelDTOT, RowMappingT
 
 try:
     from msgspec import Struct, convert
 except ImportError:  # pragma: nocover
 
     class Struct:  # type: ignore[no-redef]
         """Placeholder Implementation"""
@@ -96,25 +95,25 @@
     return next(
         (cast("FilterTypeT | None", filter_) for filter_ in filters if isinstance(filter_, filter_type)),
         None,
     )
 
 
 def to_schema(
-    data: ModelT | Sequence[ModelT] | Sequence[RowMapping] | RowMapping,
+    data: ModelT | Sequence[ModelT] | Sequence[RowMappingT] | RowMappingT,
     total: int | None = None,
     filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
-    schema_type: type[ModelT | ModelDTOT | DeclarativeBase] | None = None,
+    schema_type: type[ModelT | ModelDTOT | RowMappingT] | None = None,
 ) -> (
     ModelT
     | OffsetPagination[ModelT]
     | ModelDTOT
     | OffsetPagination[ModelDTOT]
-    | RowMapping
-    | OffsetPagination[RowMapping]
+    | RowMappingT
+    | OffsetPagination[RowMappingT]
 ):
     if schema_type is not None and issubclass(schema_type, Struct):
         if not isinstance(data, Sequence):
             return convert(  # type: ignore  # noqa: PGH003
                 obj=data,
                 type=schema_type,
                 from_attributes=True,
```

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/service/_sync.py` & `advanced_alchemy-0.9.3/advanced_alchemy/service/_sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/service/_util.py` & `advanced_alchemy-0.9.3/advanced_alchemy/service/_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,90 +12,123 @@
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from sqlalchemy import RowMapping
     from sqlalchemy.sql import ColumnElement
 
+    from advanced_alchemy.base import ModelProtocol
     from advanced_alchemy.filters import FilterTypes
     from advanced_alchemy.repository.typing import ModelT
     from advanced_alchemy.service.pagination import OffsetPagination
-    from advanced_alchemy.service.typing import ModelDTOT
+    from advanced_alchemy.service.typing import ModelDTOT, RowMappingT
 
 
 class ResultConverter:
     """Simple mixin to help convert to a paginated response model the results set is a list."""
 
     @overload
     def to_schema(
         self,
+        data: RowMappingT,
+        total: int | None = None,
+        filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
+    ) -> RowMappingT: ...
+
+    @overload
+    def to_schema(
+        self,
+        data: Sequence[RowMappingT],
+        total: int | None = None,
+        filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
+    ) -> OffsetPagination[RowMappingT]: ...
+
+    @overload
+    def to_schema(
+        self,
         data: RowMapping,
         total: int | None = None,
         filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
         schema_type: type[ModelDTOT] | None = None,
-    ) -> RowMapping: ...
+    ) -> ModelDTOT: ...
 
     @overload
     def to_schema(
         self,
         data: Sequence[RowMapping],
         total: int | None = None,
         filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
         schema_type: type[ModelDTOT] | None = None,
-    ) -> OffsetPagination[RowMapping]: ...
+    ) -> OffsetPagination[ModelDTOT]: ...
 
     @overload
     def to_schema(
         self,
         data: ModelT,
         total: int | None = None,
         filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
-        schema_type: type[ModelT] | None = None,
     ) -> ModelT: ...
 
     @overload
     def to_schema(
         self,
         data: Sequence[ModelT],
         total: int | None = None,
         filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
-        schema_type: type[ModelT] | None = None,
     ) -> OffsetPagination[ModelT]: ...
 
     @overload
     def to_schema(
         self,
         data: ModelT,
         total: int | None = None,
         filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
-        schema_type: type[ModelDTOT] = ...,
+        schema_type: type[ModelT] = ...,
+    ) -> ModelT: ...
+
+    @overload
+    def to_schema(
+        self,
+        data: Sequence[ModelT],
+        total: int | None = None,
+        filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
+        schema_type: type[ModelT] = ...,
+    ) -> OffsetPagination[ModelT]: ...
+
+    @overload
+    def to_schema(
+        self,
+        data: ModelProtocol,
+        total: int | None = None,
+        filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
+        schema_type: type[ModelDTOT] | None = None,
     ) -> ModelDTOT: ...
 
     @overload
     def to_schema(
         self,
-        data: Sequence[ModelT] | Sequence[RowMapping],
+        data: Sequence[ModelT],
         total: int | None = None,
         filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
-        schema_type: type[ModelDTOT] = ...,
+        schema_type: type[ModelDTOT] | None = None,
     ) -> OffsetPagination[ModelDTOT]: ...
 
     def to_schema(
         self,
-        data: ModelT | Sequence[ModelT] | Sequence[RowMapping] | RowMapping,
+        data: ModelT | Sequence[ModelT] | Sequence[RowMappingT] | RowMappingT,
         total: int | None = None,
         filters: Sequence[FilterTypes | ColumnElement[bool]] | Sequence[FilterTypes] = EMPTY_FILTER,
         schema_type: type[ModelDTOT | ModelT] | None = None,
     ) -> (
         ModelT
         | OffsetPagination[ModelT]
         | ModelDTOT
         | OffsetPagination[ModelDTOT]
         | RowMapping
-        | OffsetPagination[RowMapping]
+        | OffsetPagination[RowMappingT]
     ):
         """Convert the object to a response schema.  When `schema_type` is None, the model is returned with no conversion.
 
         Args:
             data: The return from one of the service calls.
             total: the total number of rows in the data
             schema_type: Collection route filters.
```

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/service/pagination.py` & `advanced_alchemy-0.9.3/advanced_alchemy/service/pagination.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/service/typing.py` & `advanced_alchemy-0.9.3/advanced_alchemy/service/typing.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 should be a SQLAlchemy model.
 """
 
 from __future__ import annotations
 
 from typing import Any, TypeVar
 
+from sqlalchemy import RowMapping  # noqa: TCH002
 from typing_extensions import TypeAlias
 
 from advanced_alchemy.filters import FilterTypes
 from advanced_alchemy.repository.typing import ModelT  # noqa: TCH001
 
 try:
     from msgspec import Struct
@@ -29,7 +30,8 @@
         """Placeholder Implementation"""
 
 
 ModelDictT: TypeAlias = "dict[str, Any] | ModelT"
 ModelDictListT: TypeAlias = "list[ModelT | dict[str, Any]] | list[dict[str, Any]]"
 FilterTypeT = TypeVar("FilterTypeT", bound=FilterTypes)
 ModelDTOT = TypeVar("ModelDTOT", bound="Struct | BaseModel")
+RowMappingT = TypeVar("RowMappingT", bound="RowMapping")
```

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/types/__init__.py` & `advanced_alchemy-0.9.3/advanced_alchemy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/types/datetime.py` & `advanced_alchemy-0.9.3/advanced_alchemy/types/datetime.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/types/encrypted_string.py` & `advanced_alchemy-0.9.3/advanced_alchemy/types/encrypted_string.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/types/guid.py` & `advanced_alchemy-0.9.3/advanced_alchemy/types/guid.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/types/json.py` & `advanced_alchemy-0.9.3/advanced_alchemy/types/json.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/utils/dataclass.py` & `advanced_alchemy-0.9.3/advanced_alchemy/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/utils/deprecation.py` & `advanced_alchemy-0.9.3/advanced_alchemy/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/utils/fixtures.py` & `advanced_alchemy-0.9.3/advanced_alchemy/utils/fixtures.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/advanced_alchemy/utils/text.py` & `advanced_alchemy-0.9.3/advanced_alchemy/utils/text.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/docs/Makefile` & `advanced_alchemy-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/docs/changelog.rst` & `advanced_alchemy-0.9.3/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/docs/conf.py` & `advanced_alchemy-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/docs/fix_missing_references.py` & `advanced_alchemy-0.9.3/docs/fix_missing_references.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/docs/getting-started.rst` & `advanced_alchemy-0.9.3/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/docs/index.rst` & `advanced_alchemy-0.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/docs/releases.rst` & `advanced_alchemy-0.9.3/docs/releases.rst`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/docs/_static/css/style.css` & `advanced_alchemy-0.9.3/docs/_static/css/style.css`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/docs/_static/css/versioning.js` & `advanced_alchemy-0.9.3/docs/_static/css/versioning.js`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/docs/reference/index.rst` & `advanced_alchemy-0.9.3/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/examples/fastapi.py` & `advanced_alchemy-0.9.3/examples/fastapi.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/examples/flask.py` & `advanced_alchemy-0.9.3/examples/flask.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/examples/sanic.py` & `advanced_alchemy-0.9.3/examples/sanic.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/examples/standalone.py` & `advanced_alchemy-0.9.3/examples/standalone.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/examples/standalone_json.py` & `advanced_alchemy-0.9.3/examples/standalone_json.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/examples/us_state_lookup.json` & `advanced_alchemy-0.9.3/examples/us_state_lookup.json`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/examples/litestar/litestar_repo_only.py` & `advanced_alchemy-0.9.3/examples/litestar/litestar_repo_only.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/examples/litestar/litestar_service.py` & `advanced_alchemy-0.9.3/examples/litestar/litestar_service.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/docker-compose.yml` & `advanced_alchemy-0.9.3/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/docker_service_fixtures.py` & `advanced_alchemy-0.9.3/tests/docker_service_fixtures.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/helpers.py` & `advanced_alchemy-0.9.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/models_bigint.py` & `advanced_alchemy-0.9.3/tests/models_bigint.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/models_uuid.py` & `advanced_alchemy-0.9.3/tests/models_uuid.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/integration/conftest.py` & `advanced_alchemy-0.9.3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/integration/helpers.py` & `advanced_alchemy-0.9.3/tests/integration/helpers.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/integration/test_alembic_commands.py` & `advanced_alchemy-0.9.3/tests/integration/test_alembic_commands.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/integration/test_lambda_stmt.py` & `advanced_alchemy-0.9.3/tests/integration/test_lambda_stmt.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/integration/test_oracledb_json.py` & `advanced_alchemy-0.9.3/tests/integration/test_oracledb_json.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/integration/test_repository.py` & `advanced_alchemy-0.9.3/tests/integration/test_repository.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/integration/test_sqlquery_service.py` & `advanced_alchemy-0.9.3/tests/integration/test_sqlquery_service.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/integration/test_unique_mixin.py` & `advanced_alchemy-0.9.3/tests/integration/test_unique_mixin.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_repository.py` & `advanced_alchemy-0.9.3/tests/unit/test_repository.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_extensions/test_sanic.py` & `advanced_alchemy-0.9.3/tests/unit/test_extensions/test_sanic.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_extensions/test_starlette.py` & `advanced_alchemy-0.9.3/tests/unit/test_extensions/test_starlette.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/conftest.py` & `advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/conftest.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_context.py` & `advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_context.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_dto.py` & `advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_dto.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_dto_integration.py` & `advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_dto_integration.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_serialization_plugin.py` & `advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_serialization_plugin.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_init_plugin/test_asyncio.py` & `advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_init_plugin/test_common.py` & `advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_common.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tests/unit/test_extensions/test_litestar/test_init_plugin/test_sync.py` & `advanced_alchemy-0.9.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/tools/build_docs.py` & `advanced_alchemy-0.9.3/tools/build_docs.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/.gitignore` & `advanced_alchemy-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/LICENSE` & `advanced_alchemy-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/README.md` & `advanced_alchemy-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.9.2/pyproject.toml` & `advanced_alchemy-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
   { name = "Peter Schutt", email = "peter@litestar.dev" },
   { name = "Visakh Unnikrishnan", email = "guacs@litestar.dev" },
   { name = "Alc", email = "alc@litestar.dev" },
 ]
 name = "advanced_alchemy"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.9.2"
+version = "0.9.3"
 
 [project.urls]
 Changelog = "https://docs.advanced-alchemy.litestar.dev/latest/changelog"
 Discord = "https://discord.gg/litestar"
 Documentation = "https://docs.advanced-alchemy.litestar.dev/latest/"
 Funding = "https://github.com/sponsors/litestar-org"
 Homepage = "https://docs.advanced-alchemy.litestar.dev/latest/"
```

### Comparing `advanced_alchemy-0.9.2/PKG-INFO` & `advanced_alchemy-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: advanced_alchemy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Ready-to-go SQLAlchemy concoctions.
 Project-URL: Changelog, https://docs.advanced-alchemy.litestar.dev/latest/changelog
 Project-URL: Discord, https://discord.gg/litestar
 Project-URL: Documentation, https://docs.advanced-alchemy.litestar.dev/latest/
 Project-URL: Funding, https://github.com/sponsors/litestar-org
 Project-URL: Homepage, https://docs.advanced-alchemy.litestar.dev/latest/
 Project-URL: Issue, https://github.com/litestar-org/advanced-alchemy/issues/
```

