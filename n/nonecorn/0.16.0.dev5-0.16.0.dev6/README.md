# Comparing `tmp/nonecorn-0.16.0.dev5.tar.gz` & `tmp/nonecorn-0.16.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonecorn-0.16.0.dev5.tar", last modified: Thu May  2 10:01:50 2024, max compression
+gzip compressed data, was "nonecorn-0.16.0.dev6.tar", last modified: Tue May  7 11:13:12 2024, max compression
```

## Comparing `nonecorn-0.16.0.dev5.tar` & `nonecorn-0.16.0.dev6.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.319561 nonecorn-0.16.0.dev5/
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.218535 nonecorn-0.16.0.dev5/.github/
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.233539 nonecorn-0.16.0.dev5/.github/workflows/
--rw-rw-rw-   0        0        0     3183 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/.github/workflows/ci.yml
--rw-rw-rw-   0        0        0      847 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev5/.github/workflows/publish.yml
--rw-rw-rw-   0        0        0      200 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev5/.gitignore
--rw-rw-rw-   0        0        0      215 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev5/.readthedocs.yaml
--rw-rw-rw-   0        0        0    21466 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev5/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1072 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/LICENSE
--rw-rw-rw-   0        0        0       30 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev5/MANIFEST.in
--rw-rw-rw-   0        0        0     4929 2024-05-02 10:01:50.319561 nonecorn-0.16.0.dev5/PKG-INFO
--rw-rw-rw-   0        0        0     3796 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev5/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.236540 nonecorn-0.16.0.dev5/artwork/
--rw-rw-rw-   0        0        0      560 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/artwork/LICENSE
--rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/artwork/logo.png
--rw-rw-rw-   0        0        0    19020 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/artwork/logo.svg
--rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/artwork/logo_small.png
--rw-rw-rw-   0        0        0     5947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/artwork/logo_small.svg
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.219536 nonecorn-0.16.0.dev5/compliance/
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.238540 nonecorn-0.16.0.dev5/compliance/autobahn/
--rw-rw-rw-   0        0        0      279 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/compliance/autobahn/fuzzingclient.json
--rw-rw-rw-   0        0        0      782 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev5/compliance/autobahn/server.py
--rw-rw-rw-   0        0        0      262 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev5/compliance/autobahn/summarise.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.240541 nonecorn-0.16.0.dev5/compliance/h2spec/
--rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/compliance/h2spec/cert.pem
--rw-rw-rw-   0        0        0     3324 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/compliance/h2spec/key.pem
--rw-rw-rw-   0        0        0      899 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev5/compliance/h2spec/server.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.243541 nonecorn-0.16.0.dev5/docs/
--rw-rw-rw-   0        0        0      630 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.245542 nonecorn-0.16.0.dev5/docs/_static/
--rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/_static/logo.png
--rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/_static/logo_small.png
--rw-rw-rw-   0        0        0     5624 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev5/docs/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.250677 nonecorn-0.16.0.dev5/docs/discussion/
--rw-rw-rw-   0        0        0      728 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/discussion/backpressure.rst
--rw-rw-rw-   0        0        0     2116 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/discussion/closing.rst
--rw-rw-rw-   0        0        0      331 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/discussion/design_choices.rst
--rw-rw-rw-   0        0        0     7278 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev5/docs/discussion/dos_mitigations.rst
--rw-rw-rw-   0        0        0     1335 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev5/docs/discussion/flow.rst
--rw-rw-rw-   0        0        0     1479 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/discussion/http2.rst
--rw-rw-rw-   0        0        0      201 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev5/docs/discussion/index.rst
--rw-rw-rw-   0        0        0      705 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/discussion/workers.rst
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.258547 nonecorn-0.16.0.dev5/docs/how_to_guides/
--rw-rw-rw-   0        0        0     3444 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/api_usage.rst
--rw-rw-rw-   0        0        0     1322 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/binds.rst
--rw-rw-rw-   0        0        0    12293 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/configuring.rst
--rw-rw-rw-   0        0        0     1396 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/dispatch_apps.rst
--rw-rw-rw-   0        0        0     1947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/http_https_redirect.rst
--rw-rw-rw-   0        0        0      270 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/index.rst
--rw-rw-rw-   0        0        0     2741 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/logging.rst
--rw-rw-rw-   0        0        0     1347 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/proxy_fix.rst
--rw-rw-rw-   0        0        0      534 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/server_names.rst
--rw-rw-rw-   0        0        0     1274 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/statsd.rst
--rw-rw-rw-   0        0        0     1211 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev5/docs/how_to_guides/wsgi_apps.rst
--rw-rw-rw-   0        0        0     1204 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/index.rst
--rwxrwxrwx   0        0        0      807 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/make.bat
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.259547 nonecorn-0.16.0.dev5/docs/reference/
--rw-rw-rw-   0        0        0      112 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/reference/api.rst
--rw-rw-rw-   0        0        0       80 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/reference/index.rst
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.262548 nonecorn-0.16.0.dev5/docs/tutorials/
--rw-rw-rw-   0        0        0      122 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/tutorials/index.rst
--rw-rw-rw-   0        0        0      231 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev5/docs/tutorials/installation.rst
--rw-rw-rw-   0        0        0      859 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/tutorials/quickstart.rst
--rw-rw-rw-   0        0        0      606 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/docs/tutorials/usage.rst
--rw-rw-rw-   0        0        0     3127 2024-05-02 10:01:27.000000 nonecorn-0.16.0.dev5/pyproject.toml
--rw-rw-rw-   0        0        0      910 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev5/readme_zh.markdown
--rw-rw-rw-   0        0        0      156 2024-05-02 10:01:50.320562 nonecorn-0.16.0.dev5/setup.cfg
--rw-rw-rw-   0        0        0     2242 2024-05-02 10:01:27.000000 nonecorn-0.16.0.dev5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.222536 nonecorn-0.16.0.dev5/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.270550 nonecorn-0.16.0.dev5/src/hypercorn/
--rw-rw-rw-   0        0        0       91 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/src/hypercorn/__init__.py
--rw-rw-rw-   0        0        0    11280 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev5/src/hypercorn/__main__.py
--rw-rw-rw-   0        0        0     5675 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/src/hypercorn/app_wrappers.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.276551 nonecorn-0.16.0.dev5/src/hypercorn/asyncio/
--rw-rw-rw-   0        0        0     1490 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev5/src/hypercorn/asyncio/__init__.py
--rw-rw-rw-   0        0        0     4069 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev5/src/hypercorn/asyncio/lifespan.py
--rw-rw-rw-   0        0        0     8240 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev5/src/hypercorn/asyncio/run.py
--rw-rw-rw-   0        0        0      795 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev5/src/hypercorn/asyncio/statsd.py
--rw-rw-rw-   0        0        0     2305 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev5/src/hypercorn/asyncio/task_group.py
--rw-rw-rw-   0        0        0     6455 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev5/src/hypercorn/asyncio/tcp_server.py
--rw-rw-rw-   0        0        0     3228 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev5/src/hypercorn/asyncio/udp_server.py
--rw-rw-rw-   0        0        0     1223 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev5/src/hypercorn/asyncio/worker_context.py
--rw-rw-rw-   0        0        0    14242 2024-05-02 08:29:18.000000 nonecorn-0.16.0.dev5/src/hypercorn/config.py
--rw-rw-rw-   0        0        0      557 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev5/src/hypercorn/events.py
--rw-rw-rw-   0        0        0     7587 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev5/src/hypercorn/logging.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.279552 nonecorn-0.16.0.dev5/src/hypercorn/middleware/
--rw-rw-rw-   0        0        0      415 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev5/src/hypercorn/middleware/__init__.py
--rw-rw-rw-   0        0        0     4414 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/src/hypercorn/middleware/dispatcher.py
--rw-rw-rw-   0        0        0     2686 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/src/hypercorn/middleware/http_to_https.py
--rw-rw-rw-   0        0        0     2772 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev5/src/hypercorn/middleware/proxy_fix.py
--rw-rw-rw-   0        0        0     1538 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/src/hypercorn/middleware/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.285553 nonecorn-0.16.0.dev5/src/hypercorn/protocol/
--rw-rw-rw-   0        0        0     3235 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev5/src/hypercorn/protocol/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev5/src/hypercorn/protocol/events.py
--rw-rw-rw-   0        0        0    13933 2024-01-15 10:30:30.000000 nonecorn-0.16.0.dev5/src/hypercorn/protocol/h11.py
--rw-rw-rw-   0        0        0    17133 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev5/src/hypercorn/protocol/h2.py
--rw-rw-rw-   0        0        0     6125 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev5/src/hypercorn/protocol/h3.py
--rw-rw-rw-   0        0        0    14834 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/src/hypercorn/protocol/http_stream.py
--rw-rw-rw-   0        0        0     5346 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev5/src/hypercorn/protocol/quic.py
--rw-rw-rw-   0        0        0    19463 2024-01-15 10:31:48.000000 nonecorn-0.16.0.dev5/src/hypercorn/protocol/ws_stream.py
--rw-rw-rw-   0        0        0        8 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/src/hypercorn/py.typed
--rw-rw-rw-   0        0        0     4993 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev5/src/hypercorn/run.py
--rw-rw-rw-   0        0        0     3927 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/src/hypercorn/statsd.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.291555 nonecorn-0.16.0.dev5/src/hypercorn/trio/
--rw-rw-rw-   0        0        0     1611 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev5/src/hypercorn/trio/__init__.py
--rw-rw-rw-   0        0        0     3728 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev5/src/hypercorn/trio/lifespan.py
--rw-rw-rw-   0        0        0     5209 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev5/src/hypercorn/trio/run.py
--rw-rw-rw-   0        0        0      509 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/src/hypercorn/trio/statsd.py
--rw-rw-rw-   0        0        0     2503 2023-07-08 16:37:15.000000 nonecorn-0.16.0.dev5/src/hypercorn/trio/task_group.py
--rw-rw-rw-   0        0        0     5373 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev5/src/hypercorn/trio/tcp_server.py
--rw-rw-rw-   0        0        0     1783 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev5/src/hypercorn/trio/udp_server.py
--rw-rw-rw-   0        0        0     1211 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev5/src/hypercorn/trio/worker_context.py
--rw-rw-rw-   0        0        0     8258 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev5/src/hypercorn/typing.py
--rw-rw-rw-   0        0        0     9646 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev5/src/hypercorn/utils.py
--rw-rw-rw-   0        0        0    14133 2024-05-02 09:54:46.000000 nonecorn-0.16.0.dev5/src/hypercorn/workers.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.295556 nonecorn-0.16.0.dev5/src/nonecorn.egg-info/
--rw-rw-rw-   0        0        0     4929 2024-05-02 10:01:49.000000 nonecorn-0.16.0.dev5/src/nonecorn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3694 2024-05-02 10:01:50.000000 nonecorn-0.16.0.dev5/src/nonecorn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 10:01:49.000000 nonecorn-0.16.0.dev5/src/nonecorn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-02 10:01:49.000000 nonecorn-0.16.0.dev5/src/nonecorn.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      273 2024-05-02 10:01:49.000000 nonecorn-0.16.0.dev5/src/nonecorn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-02 10:01:49.000000 nonecorn-0.16.0.dev5/src/nonecorn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.301557 nonecorn-0.16.0.dev5/tests/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.305558 nonecorn-0.16.0.dev5/tests/assets/
--rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/assets/cert.pem
--rw-rw-rw-   0        0        0      147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/assets/config.py
--rw-rw-rw-   0        0        0       81 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/assets/config.toml
--rw-rw-rw-   0        0        0      217 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/assets/config_ssl.py
--rw-rw-rw-   0        0        0     3320 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/assets/key.pem
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.310559 nonecorn-0.16.0.dev5/tests/asyncio/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/asyncio/__init__.py
--rw-rw-rw-   0        0        0     1705 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/asyncio/helpers.py
--rw-rw-rw-   0        0        0     4075 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/tests/asyncio/test_keep_alive.py
--rw-rw-rw-   0        0        0     2654 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/tests/asyncio/test_lifespan.py
--rw-rw-rw-   0        0        0     8765 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/tests/asyncio/test_sanity.py
--rw-rw-rw-   0        0        0     1571 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/tests/asyncio/test_task_group.py
--rw-rw-rw-   0        0        0     1680 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/tests/asyncio/test_tcp_server.py
--rw-rw-rw-   0        0        0      897 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/conftest.py
--rw-rw-rw-   0        0        0     4396 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev5/tests/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.313560 nonecorn-0.16.0.dev5/tests/middleware/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/middleware/__init__.py
--rw-rw-rw-   0        0        0     3309 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev5/tests/middleware/test_dispatcher.py
--rw-rw-rw-   0        0        0     4886 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/middleware/test_http_to_https.py
--rw-rw-rw-   0        0        0     2175 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev5/tests/middleware/test_proxy_fix.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.316561 nonecorn-0.16.0.dev5/tests/protocol/
--rw-rw-rw-   0        0        0    15278 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/tests/protocol/test_h11.py
--rw-rw-rw-   0        0        0     3612 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/tests/protocol/test_h2.py
--rw-rw-rw-   0        0        0    10000 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev5/tests/protocol/test_http_stream.py
--rw-rw-rw-   0        0        0    17493 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/tests/protocol/test_ws_stream.py
--rw-rw-rw-   0        0        0     2983 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/test___main__.py
--rw-rw-rw-   0        0        0     6111 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev5/tests/test_app_wrappers.py
--rw-rw-rw-   0        0        0     5687 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/tests/test_config.py
--rw-rw-rw-   0        0        0     4147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/test_logging.py
--rw-rw-rw-   0        0        0     2223 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:01:50.318561 nonecorn-0.16.0.dev5/tests/trio/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev5/tests/trio/__init__.py
--rw-rw-rw-   0        0        0     3980 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev5/tests/trio/test_keep_alive.py
--rw-rw-rw-   0        0        0     1661 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev5/tests/trio/test_lifespan.py
--rw-rw-rw-   0        0        0     8241 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev5/tests/trio/test_sanity.py
--rw-rw-rw-   0        0        0     1245 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev5/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.823251 nonecorn-0.16.0.dev6/
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.713225 nonecorn-0.16.0.dev6/.github/
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.729229 nonecorn-0.16.0.dev6/.github/workflows/
+-rw-rw-rw-   0        0        0     3183 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/.github/workflows/ci.yml
+-rw-rw-rw-   0        0        0      847 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/.github/workflows/publish.yml
+-rw-rw-rw-   0        0        0      200 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev6/.gitignore
+-rw-rw-rw-   0        0        0      215 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev6/.readthedocs.yaml
+-rw-rw-rw-   0        0        0    21466 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1072 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4929 2024-05-07 11:13:12.824252 nonecorn-0.16.0.dev6/PKG-INFO
+-rw-rw-rw-   0        0        0     3796 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev6/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.733230 nonecorn-0.16.0.dev6/artwork/
+-rw-rw-rw-   0        0        0      560 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/artwork/LICENSE
+-rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/artwork/logo.png
+-rw-rw-rw-   0        0        0    19020 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/artwork/logo.svg
+-rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/artwork/logo_small.png
+-rw-rw-rw-   0        0        0     5947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/artwork/logo_small.svg
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.714226 nonecorn-0.16.0.dev6/compliance/
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.735231 nonecorn-0.16.0.dev6/compliance/autobahn/
+-rw-rw-rw-   0        0        0      279 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/compliance/autobahn/fuzzingclient.json
+-rw-rw-rw-   0        0        0      782 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/compliance/autobahn/server.py
+-rw-rw-rw-   0        0        0      262 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/compliance/autobahn/summarise.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.738231 nonecorn-0.16.0.dev6/compliance/h2spec/
+-rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/compliance/h2spec/cert.pem
+-rw-rw-rw-   0        0        0     3324 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/compliance/h2spec/key.pem
+-rw-rw-rw-   0        0        0      899 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/compliance/h2spec/server.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.741232 nonecorn-0.16.0.dev6/docs/
+-rw-rw-rw-   0        0        0      630 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.743232 nonecorn-0.16.0.dev6/docs/_static/
+-rw-rw-rw-   0        0        0    22901 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/_static/logo.png
+-rw-rw-rw-   0        0        0     7610 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/_static/logo_small.png
+-rw-rw-rw-   0        0        0     5624 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/docs/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.749234 nonecorn-0.16.0.dev6/docs/discussion/
+-rw-rw-rw-   0        0        0      728 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/discussion/backpressure.rst
+-rw-rw-rw-   0        0        0     2116 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/discussion/closing.rst
+-rw-rw-rw-   0        0        0      331 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/discussion/design_choices.rst
+-rw-rw-rw-   0        0        0     7278 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev6/docs/discussion/dos_mitigations.rst
+-rw-rw-rw-   0        0        0     1335 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/docs/discussion/flow.rst
+-rw-rw-rw-   0        0        0     1479 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/discussion/http2.rst
+-rw-rw-rw-   0        0        0      201 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/docs/discussion/index.rst
+-rw-rw-rw-   0        0        0      705 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/discussion/workers.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.757236 nonecorn-0.16.0.dev6/docs/how_to_guides/
+-rw-rw-rw-   0        0        0     3444 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/api_usage.rst
+-rw-rw-rw-   0        0        0     1322 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/binds.rst
+-rw-rw-rw-   0        0        0    12293 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/configuring.rst
+-rw-rw-rw-   0        0        0     1396 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/dispatch_apps.rst
+-rw-rw-rw-   0        0        0     1947 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/http_https_redirect.rst
+-rw-rw-rw-   0        0        0      270 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/index.rst
+-rw-rw-rw-   0        0        0     2741 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/logging.rst
+-rw-rw-rw-   0        0        0     1347 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/proxy_fix.rst
+-rw-rw-rw-   0        0        0      534 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/server_names.rst
+-rw-rw-rw-   0        0        0     1274 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/statsd.rst
+-rw-rw-rw-   0        0        0     1211 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev6/docs/how_to_guides/wsgi_apps.rst
+-rw-rw-rw-   0        0        0     1204 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/index.rst
+-rwxrwxrwx   0        0        0      807 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/make.bat
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.759236 nonecorn-0.16.0.dev6/docs/reference/
+-rw-rw-rw-   0        0        0      112 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/reference/api.rst
+-rw-rw-rw-   0        0        0       80 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/reference/index.rst
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.762237 nonecorn-0.16.0.dev6/docs/tutorials/
+-rw-rw-rw-   0        0        0      122 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/tutorials/index.rst
+-rw-rw-rw-   0        0        0      231 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev6/docs/tutorials/installation.rst
+-rw-rw-rw-   0        0        0      859 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/tutorials/quickstart.rst
+-rw-rw-rw-   0        0        0      606 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/docs/tutorials/usage.rst
+-rw-rw-rw-   0        0        0     3127 2024-05-07 11:12:57.000000 nonecorn-0.16.0.dev6/pyproject.toml
+-rw-rw-rw-   0        0        0      910 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/readme_zh.markdown
+-rw-rw-rw-   0        0        0      156 2024-05-07 11:13:12.824252 nonecorn-0.16.0.dev6/setup.cfg
+-rw-rw-rw-   0        0        0     2242 2024-05-07 11:12:32.000000 nonecorn-0.16.0.dev6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.717226 nonecorn-0.16.0.dev6/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.771239 nonecorn-0.16.0.dev6/src/hypercorn/
+-rw-rw-rw-   0        0        0       91 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/src/hypercorn/__init__.py
+-rw-rw-rw-   0        0        0    11280 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/src/hypercorn/__main__.py
+-rw-rw-rw-   0        0        0     5675 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/src/hypercorn/app_wrappers.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.777241 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/
+-rw-rw-rw-   0        0        0     1490 2023-12-03 11:38:47.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     4069 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/lifespan.py
+-rw-rw-rw-   0        0        0     8240 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/run.py
+-rw-rw-rw-   0        0        0      795 2023-03-10 03:15:15.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/statsd.py
+-rw-rw-rw-   0        0        0     2305 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/task_group.py
+-rw-rw-rw-   0        0        0     6455 2023-12-27 11:54:20.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/tcp_server.py
+-rw-rw-rw-   0        0        0     3228 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/udp_server.py
+-rw-rw-rw-   0        0        0     1223 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/src/hypercorn/asyncio/worker_context.py
+-rw-rw-rw-   0        0        0    14318 2024-05-07 11:10:54.000000 nonecorn-0.16.0.dev6/src/hypercorn/config.py
+-rw-rw-rw-   0        0        0      557 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/events.py
+-rw-rw-rw-   0        0        0     7587 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/src/hypercorn/logging.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.780241 nonecorn-0.16.0.dev6/src/hypercorn/middleware/
+-rw-rw-rw-   0        0        0      415 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev6/src/hypercorn/middleware/__init__.py
+-rw-rw-rw-   0        0        0     4414 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/src/hypercorn/middleware/dispatcher.py
+-rw-rw-rw-   0        0        0     2686 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/src/hypercorn/middleware/http_to_https.py
+-rw-rw-rw-   0        0        0     2772 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev6/src/hypercorn/middleware/proxy_fix.py
+-rw-rw-rw-   0        0        0     1538 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/src/hypercorn/middleware/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.786243 nonecorn-0.16.0.dev6/src/hypercorn/protocol/
+-rw-rw-rw-   0        0        0     3235 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-12-03 11:38:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/events.py
+-rw-rw-rw-   0        0        0    13933 2024-01-15 10:30:30.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/h11.py
+-rw-rw-rw-   0        0        0    17133 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/h2.py
+-rw-rw-rw-   0        0        0     6125 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/h3.py
+-rw-rw-rw-   0        0        0    14834 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/http_stream.py
+-rw-rw-rw-   0        0        0     5346 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/quic.py
+-rw-rw-rw-   0        0        0    19463 2024-01-15 10:31:48.000000 nonecorn-0.16.0.dev6/src/hypercorn/protocol/ws_stream.py
+-rw-rw-rw-   0        0        0        8 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/src/hypercorn/py.typed
+-rw-rw-rw-   0        0        0     4993 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/src/hypercorn/run.py
+-rw-rw-rw-   0        0        0     3985 2024-05-07 11:10:54.000000 nonecorn-0.16.0.dev6/src/hypercorn/statsd.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.794245 nonecorn-0.16.0.dev6/src/hypercorn/trio/
+-rw-rw-rw-   0        0        0     1611 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/__init__.py
+-rw-rw-rw-   0        0        0     3728 2024-05-02 07:37:34.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/lifespan.py
+-rw-rw-rw-   0        0        0     5209 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/run.py
+-rw-rw-rw-   0        0        0      509 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/statsd.py
+-rw-rw-rw-   0        0        0     2503 2023-07-08 16:37:15.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/task_group.py
+-rw-rw-rw-   0        0        0     5373 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/tcp_server.py
+-rw-rw-rw-   0        0        0     1783 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/udp_server.py
+-rw-rw-rw-   0        0        0     1211 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/src/hypercorn/trio/worker_context.py
+-rw-rw-rw-   0        0        0     8258 2024-05-02 07:37:37.000000 nonecorn-0.16.0.dev6/src/hypercorn/typing.py
+-rw-rw-rw-   0        0        0     9646 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/src/hypercorn/utils.py
+-rw-rw-rw-   0        0        0    14215 2024-05-07 11:05:55.000000 nonecorn-0.16.0.dev6/src/hypercorn/workers.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.799246 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/
+-rw-rw-rw-   0        0        0     4929 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3694 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      273 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-07 11:13:12.000000 nonecorn-0.16.0.dev6/src/nonecorn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.806247 nonecorn-0.16.0.dev6/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.809248 nonecorn-0.16.0.dev6/tests/assets/
+-rw-rw-rw-   0        0        0     1678 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/assets/cert.pem
+-rw-rw-rw-   0        0        0      147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/assets/config.py
+-rw-rw-rw-   0        0        0       81 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/assets/config.toml
+-rw-rw-rw-   0        0        0      217 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/assets/config_ssl.py
+-rw-rw-rw-   0        0        0     3320 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/assets/key.pem
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.814249 nonecorn-0.16.0.dev6/tests/asyncio/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     1705 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/asyncio/helpers.py
+-rw-rw-rw-   0        0        0     4075 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/asyncio/test_keep_alive.py
+-rw-rw-rw-   0        0        0     2654 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/asyncio/test_lifespan.py
+-rw-rw-rw-   0        0        0     8765 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/asyncio/test_sanity.py
+-rw-rw-rw-   0        0        0     1571 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/asyncio/test_task_group.py
+-rw-rw-rw-   0        0        0     1680 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/asyncio/test_tcp_server.py
+-rw-rw-rw-   0        0        0      897 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/conftest.py
+-rw-rw-rw-   0        0        0     4396 2023-07-08 14:46:18.000000 nonecorn-0.16.0.dev6/tests/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.817250 nonecorn-0.16.0.dev6/tests/middleware/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/middleware/__init__.py
+-rw-rw-rw-   0        0        0     3309 2023-12-27 10:48:15.000000 nonecorn-0.16.0.dev6/tests/middleware/test_dispatcher.py
+-rw-rw-rw-   0        0        0     4886 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/middleware/test_http_to_https.py
+-rw-rw-rw-   0        0        0     2175 2024-01-05 11:44:30.000000 nonecorn-0.16.0.dev6/tests/middleware/test_proxy_fix.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.820251 nonecorn-0.16.0.dev6/tests/protocol/
+-rw-rw-rw-   0        0        0    15278 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/protocol/test_h11.py
+-rw-rw-rw-   0        0        0     3612 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/protocol/test_h2.py
+-rw-rw-rw-   0        0        0    10742 2024-05-07 11:10:54.000000 nonecorn-0.16.0.dev6/tests/protocol/test_http_stream.py
+-rw-rw-rw-   0        0        0    17493 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/protocol/test_ws_stream.py
+-rw-rw-rw-   0        0        0     2983 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/test___main__.py
+-rw-rw-rw-   0        0        0     6111 2023-12-29 15:43:11.000000 nonecorn-0.16.0.dev6/tests/test_app_wrappers.py
+-rw-rw-rw-   0        0        0     5687 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/test_config.py
+-rw-rw-rw-   0        0        0     4147 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/test_logging.py
+-rw-rw-rw-   0        0        0     2223 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 11:13:12.823251 nonecorn-0.16.0.dev6/tests/trio/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:15:16.000000 nonecorn-0.16.0.dev6/tests/trio/__init__.py
+-rw-rw-rw-   0        0        0     3980 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/tests/trio/test_keep_alive.py
+-rw-rw-rw-   0        0        0     1661 2024-04-21 06:24:22.000000 nonecorn-0.16.0.dev6/tests/trio/test_lifespan.py
+-rw-rw-rw-   0        0        0     8241 2024-01-03 05:14:38.000000 nonecorn-0.16.0.dev6/tests/trio/test_sanity.py
+-rw-rw-rw-   0        0        0     1245 2023-10-30 11:48:33.000000 nonecorn-0.16.0.dev6/tox.ini
```

### Comparing `nonecorn-0.16.0.dev5/.github/workflows/ci.yml` & `nonecorn-0.16.0.dev6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/.github/workflows/publish.yml` & `nonecorn-0.16.0.dev6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/CHANGELOG.rst` & `nonecorn-0.16.0.dev6/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/LICENSE` & `nonecorn-0.16.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/PKG-INFO` & `nonecorn-0.16.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonecorn
-Version: 0.16.0.dev5
+Version: 0.16.0.dev6
 Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
 Home-page: https://gitlab.com/pgjones/hypercorn/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nonecorn-0.16.0.dev5/README.rst` & `nonecorn-0.16.0.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/artwork/LICENSE` & `nonecorn-0.16.0.dev6/artwork/LICENSE`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/artwork/logo.png` & `nonecorn-0.16.0.dev6/artwork/logo.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/artwork/logo.svg` & `nonecorn-0.16.0.dev6/artwork/logo.svg`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/artwork/logo_small.png` & `nonecorn-0.16.0.dev6/artwork/logo_small.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/artwork/logo_small.svg` & `nonecorn-0.16.0.dev6/artwork/logo_small.svg`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/compliance/autobahn/server.py` & `nonecorn-0.16.0.dev6/compliance/autobahn/server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/compliance/h2spec/cert.pem` & `nonecorn-0.16.0.dev6/compliance/h2spec/cert.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/compliance/h2spec/key.pem` & `nonecorn-0.16.0.dev6/compliance/h2spec/key.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/compliance/h2spec/server.py` & `nonecorn-0.16.0.dev6/compliance/h2spec/server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/Makefile` & `nonecorn-0.16.0.dev6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/_static/logo.png` & `nonecorn-0.16.0.dev6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/_static/logo_small.png` & `nonecorn-0.16.0.dev6/docs/_static/logo_small.png`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/conf.py` & `nonecorn-0.16.0.dev6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/discussion/backpressure.rst` & `nonecorn-0.16.0.dev6/docs/discussion/backpressure.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/discussion/closing.rst` & `nonecorn-0.16.0.dev6/docs/discussion/closing.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/discussion/dos_mitigations.rst` & `nonecorn-0.16.0.dev6/docs/discussion/dos_mitigations.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/discussion/flow.rst` & `nonecorn-0.16.0.dev6/docs/discussion/flow.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/discussion/http2.rst` & `nonecorn-0.16.0.dev6/docs/discussion/http2.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/discussion/workers.rst` & `nonecorn-0.16.0.dev6/docs/discussion/workers.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/how_to_guides/api_usage.rst` & `nonecorn-0.16.0.dev6/docs/how_to_guides/api_usage.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/how_to_guides/binds.rst` & `nonecorn-0.16.0.dev6/docs/how_to_guides/binds.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/how_to_guides/configuring.rst` & `nonecorn-0.16.0.dev6/docs/how_to_guides/configuring.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/how_to_guides/dispatch_apps.rst` & `nonecorn-0.16.0.dev6/docs/how_to_guides/dispatch_apps.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/how_to_guides/http_https_redirect.rst` & `nonecorn-0.16.0.dev6/docs/how_to_guides/http_https_redirect.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/how_to_guides/logging.rst` & `nonecorn-0.16.0.dev6/docs/how_to_guides/logging.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/how_to_guides/proxy_fix.rst` & `nonecorn-0.16.0.dev6/docs/how_to_guides/proxy_fix.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/how_to_guides/server_names.rst` & `nonecorn-0.16.0.dev6/docs/how_to_guides/server_names.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/how_to_guides/statsd.rst` & `nonecorn-0.16.0.dev6/docs/how_to_guides/statsd.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/how_to_guides/wsgi_apps.rst` & `nonecorn-0.16.0.dev6/docs/how_to_guides/wsgi_apps.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/index.rst` & `nonecorn-0.16.0.dev6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/make.bat` & `nonecorn-0.16.0.dev6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/tutorials/quickstart.rst` & `nonecorn-0.16.0.dev6/docs/tutorials/quickstart.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/docs/tutorials/usage.rst` & `nonecorn-0.16.0.dev6/docs/tutorials/usage.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/pyproject.toml` & `nonecorn-0.16.0.dev6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonecorn"
-version = "0.16.0dev5"
+version = "0.16.0dev6"
 description = "A ASGI Server based on Hyper libraries and inspired by Gunicorn"
 authors = ["pgjones <philip.graham.jones@googlemail.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `nonecorn-0.16.0.dev5/readme_zh.markdown` & `nonecorn-0.16.0.dev6/readme_zh.markdown`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/setup.py` & `nonecorn-0.16.0.dev6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "pytest-cov",
     "pytest-trio",
     "trio",
 ]
 
 setup(
     name="nonecorn",
-    version="0.16.0dev5",
+    version="0.16.0dev6",
     python_requires=">=3.7",
     description="A ASGI Server forked from hypercorn with more extra feature beyond ASGI",
     long_description=long_description,
     url="https://gitlab.com/pgjones/hypercorn/",
     author="P G Jones",
     author_email="philip.graham.jones@googlemail.com",
     license="MIT",
```

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/__main__.py` & `nonecorn-0.16.0.dev6/src/hypercorn/__main__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/app_wrappers.py` & `nonecorn-0.16.0.dev6/src/hypercorn/app_wrappers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/asyncio/__init__.py` & `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/asyncio/lifespan.py` & `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/asyncio/run.py` & `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/asyncio/statsd.py` & `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/statsd.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/asyncio/task_group.py` & `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/task_group.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/asyncio/tcp_server.py` & `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/tcp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/asyncio/udp_server.py` & `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/udp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/asyncio/worker_context.py` & `nonecorn-0.16.0.dev6/src/hypercorn/asyncio/worker_context.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/config.py` & `nonecorn-0.16.0.dev6/src/hypercorn/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,15 @@
                 bind = bind.replace("[", "").replace("]", "")
                 try:
                     value = bind.rsplit(":", 1)
                     host, port = value[0], int(value[1])
                 except (ValueError, IndexError):
                     host, port = bind, 8000
                 sock = socket.socket(socket.AF_INET6 if ":" in host else socket.AF_INET, type_)
+                sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
                 if self.workers > 1:
                     try:
                         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
                     except AttributeError:
                         pass
                 binding = (host, port)
```

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/events.py` & `nonecorn-0.16.0.dev6/src/hypercorn/events.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/logging.py` & `nonecorn-0.16.0.dev6/src/hypercorn/logging.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/middleware/dispatcher.py` & `nonecorn-0.16.0.dev6/src/hypercorn/middleware/dispatcher.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/middleware/http_to_https.py` & `nonecorn-0.16.0.dev6/src/hypercorn/middleware/http_to_https.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/middleware/proxy_fix.py` & `nonecorn-0.16.0.dev6/src/hypercorn/middleware/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/middleware/wsgi.py` & `nonecorn-0.16.0.dev6/src/hypercorn/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/protocol/__init__.py` & `nonecorn-0.16.0.dev6/src/hypercorn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/protocol/events.py` & `nonecorn-0.16.0.dev6/src/hypercorn/protocol/events.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/protocol/h11.py` & `nonecorn-0.16.0.dev6/src/hypercorn/protocol/h11.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/protocol/h2.py` & `nonecorn-0.16.0.dev6/src/hypercorn/protocol/h2.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/protocol/h3.py` & `nonecorn-0.16.0.dev6/src/hypercorn/protocol/h3.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/protocol/http_stream.py` & `nonecorn-0.16.0.dev6/src/hypercorn/protocol/http_stream.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/protocol/quic.py` & `nonecorn-0.16.0.dev6/src/hypercorn/protocol/quic.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/protocol/ws_stream.py` & `nonecorn-0.16.0.dev6/src/hypercorn/protocol/ws_stream.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/run.py` & `nonecorn-0.16.0.dev6/src/hypercorn/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/statsd.py` & `nonecorn-0.16.0.dev6/src/hypercorn/statsd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, TYPE_CHECKING
+from typing import Any, Optional, TYPE_CHECKING
 
 from .logging import Logger
 
 if TYPE_CHECKING:
     from .config import Config
     from .typing import ResponseSummary, WWWScope
 
@@ -63,20 +63,21 @@
 
             if message:
                 await super().log(level, message, *args, **kwargs)
         except Exception:
             await super().warning("Failed to log to statsd", exc_info=True)
 
     async def access(
-        self, request: "WWWScope", response: "ResponseSummary", request_time: float
+        self, request: "WWWScope", response: Optional["ResponseSummary"], request_time: float
     ) -> None:
         await super().access(request, response, request_time)
         await self.histogram("hypercorn.request.duration", request_time * 1_000)
         await self.increment("hypercorn.requests", 1)
-        await self.increment(f"hypercorn.request.status.{response['status']}", 1)
+        if response is not None:
+            await self.increment(f"hypercorn.request.status.{response['status']}", 1)
 
     async def gauge(self, name: str, value: int) -> None:
         await self._send(f"{self.prefix}{name}:{value}|g")
 
     async def increment(self, name: str, value: int, sampling_rate: float = 1.0) -> None:
         await self._send(f"{self.prefix}{name}:{value}|c|@{sampling_rate}")
```

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/trio/__init__.py` & `nonecorn-0.16.0.dev6/src/hypercorn/trio/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/trio/lifespan.py` & `nonecorn-0.16.0.dev6/src/hypercorn/trio/lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/trio/run.py` & `nonecorn-0.16.0.dev6/src/hypercorn/trio/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/trio/task_group.py` & `nonecorn-0.16.0.dev6/src/hypercorn/trio/task_group.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/trio/tcp_server.py` & `nonecorn-0.16.0.dev6/src/hypercorn/trio/tcp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/trio/udp_server.py` & `nonecorn-0.16.0.dev6/src/hypercorn/trio/udp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/trio/worker_context.py` & `nonecorn-0.16.0.dev6/src/hypercorn/trio/worker_context.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/typing.py` & `nonecorn-0.16.0.dev6/src/hypercorn/typing.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/utils.py` & `nonecorn-0.16.0.dev6/src/hypercorn/utils.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/src/hypercorn/workers.py` & `nonecorn-0.16.0.dev6/src/hypercorn/workers.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
             "h11_pass_raw_headers": getattr(self.cfg, "h11_pass_raw_headers", None),
             "h2_max_concurrent_streams": getattr(self.cfg, "h2_max_concurrent_streams", None),
             "h2_max_header_list_size": getattr(self.cfg, "h2_max_header_list_size", None),
             "h2_max_inbound_frame_size": getattr(self.cfg, "h2_max_inbound_frame_size", None),
             "include_date_header": getattr(self.cfg, "include_date_header", None),
             "include_server_header": getattr(self.cfg, "include_server_header", None),
             "max_app_queue_size": getattr(self.cfg, "max_app_queue_size", None),
-            "max_requests": getattr(self.cfg, "max_requests", None),
+            "max_requests": self.cfg.max_requests or None,
             "max_requests_jitter": getattr(self.cfg, "max_requests_jitter", None),
             "pid_path": getattr(self.cfg, "pidfile", None),
             "root_path": getattr(self.cfg, "root_path", None),
             "server_names": getattr(self.cfg, "server_names", None),
             "shutdown_timeout": getattr(self.cfg, "shutdown_timeout", None),
             "ssl_handshake_timeout": getattr(self.cfg, "ssl_handshake_timeout", None),
             "startup_timeout": getattr(self.cfg, "startup_timeout", None),
@@ -379,15 +379,18 @@
         # Copy from uvicorn
         loop = asyncio.get_running_loop()
         loop.add_signal_handler(signal.SIGQUIT, self.handle_exit, signal.SIGQUIT, None)
 
     async def _asyncio_serve(self):
         self._install_sigquit_handler()
         await asyncio.wait(
-            [asyncio_serve(self.wsgi, self.config), self.asyncio_callback_notify()],
+            [
+                asyncio.create_task(asyncio_serve(self.wsgi, self.config)),
+                asyncio.create_task(self.asyncio_callback_notify()),
+            ],
             return_when=asyncio.FIRST_COMPLETED,
         )
 
     async def _trio_serve(self):
         import trio
 
         from hypercorn.trio import serve as trio_serve
```

### Comparing `nonecorn-0.16.0.dev5/src/nonecorn.egg-info/PKG-INFO` & `nonecorn-0.16.0.dev6/src/nonecorn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonecorn
-Version: 0.16.0.dev5
+Version: 0.16.0.dev6
 Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
 Home-page: https://gitlab.com/pgjones/hypercorn/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nonecorn-0.16.0.dev5/src/nonecorn.egg-info/SOURCES.txt` & `nonecorn-0.16.0.dev6/src/nonecorn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/assets/cert.pem` & `nonecorn-0.16.0.dev6/tests/assets/cert.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/assets/key.pem` & `nonecorn-0.16.0.dev6/tests/assets/key.pem`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/asyncio/helpers.py` & `nonecorn-0.16.0.dev6/tests/asyncio/helpers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/asyncio/test_keep_alive.py` & `nonecorn-0.16.0.dev6/tests/asyncio/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/asyncio/test_lifespan.py` & `nonecorn-0.16.0.dev6/tests/asyncio/test_lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/asyncio/test_sanity.py` & `nonecorn-0.16.0.dev6/tests/asyncio/test_sanity.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/asyncio/test_task_group.py` & `nonecorn-0.16.0.dev6/tests/asyncio/test_task_group.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/asyncio/test_tcp_server.py` & `nonecorn-0.16.0.dev6/tests/asyncio/test_tcp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/conftest.py` & `nonecorn-0.16.0.dev6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/helpers.py` & `nonecorn-0.16.0.dev6/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/middleware/test_dispatcher.py` & `nonecorn-0.16.0.dev6/tests/middleware/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/middleware/test_http_to_https.py` & `nonecorn-0.16.0.dev6/tests/middleware/test_http_to_https.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/middleware/test_proxy_fix.py` & `nonecorn-0.16.0.dev6/tests/middleware/test_proxy_fix.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/protocol/test_h11.py` & `nonecorn-0.16.0.dev6/tests/protocol/test_h11.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/protocol/test_h2.py` & `nonecorn-0.16.0.dev6/tests/protocol/test_h2.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/protocol/test_http_stream.py` & `nonecorn-0.16.0.dev6/tests/protocol/test_http_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import Any, cast
 from unittest.mock import call
 
 import pytest
 import pytest_asyncio
 
+from hypercorn.asyncio.statsd import StatsdLogger
 from hypercorn.asyncio.worker_context import WorkerContext
 from hypercorn.config import Config
 from hypercorn.logging import Logger
 from hypercorn.protocol.events import (
     Body,
     EndBody,
     InformationalResponse,
@@ -294,7 +295,25 @@
 @pytest.mark.asyncio
 async def test_closed_app_send_noop(stream: HTTPStream) -> None:
     stream.closed = True
     await stream.app_send(
         cast(HTTPResponseStartEvent, {"type": "http.response.start", "status": 200, "headers": []})
     )
     stream.send.assert_not_called()  # type: ignore
+
+
+@pytest.mark.asyncio
+async def test_abnormal_close_logging() -> None:
+    config = Config()
+    config.accesslog = "-"
+    config.statsd_host = "localhost:9125"
+    # This exercises an issue where `HTTPStream` at one point called the statsd logger
+    # with `response=None` when the statsd logger failed to handle it.
+    config.set_statsd_logger_class(StatsdLogger)
+    stream = HTTPStream(
+        AsyncMock(), config, WorkerContext(None), AsyncMock(), False, None, None, AsyncMock(), 1
+    )
+
+    await stream.handle(
+        Request(stream_id=1, http_version="2", headers=[], raw_path=b"/?a=b", method="GET")
+    )
+    await stream.handle(StreamClosed(stream_id=1))
```

### Comparing `nonecorn-0.16.0.dev5/tests/protocol/test_ws_stream.py` & `nonecorn-0.16.0.dev6/tests/protocol/test_ws_stream.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/test___main__.py` & `nonecorn-0.16.0.dev6/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/test_app_wrappers.py` & `nonecorn-0.16.0.dev6/tests/test_app_wrappers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/test_config.py` & `nonecorn-0.16.0.dev6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/test_logging.py` & `nonecorn-0.16.0.dev6/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/test_utils.py` & `nonecorn-0.16.0.dev6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/trio/test_keep_alive.py` & `nonecorn-0.16.0.dev6/tests/trio/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/trio/test_lifespan.py` & `nonecorn-0.16.0.dev6/tests/trio/test_lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tests/trio/test_sanity.py` & `nonecorn-0.16.0.dev6/tests/trio/test_sanity.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.16.0.dev5/tox.ini` & `nonecorn-0.16.0.dev6/tox.ini`

 * *Files identical despite different names*

