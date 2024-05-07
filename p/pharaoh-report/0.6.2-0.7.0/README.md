# Comparing `tmp/pharaoh_report-0.6.2.tar.gz` & `tmp/pharaoh_report-0.7.0.tar.gz`

## Comparing `pharaoh_report-0.6.2.tar` & `pharaoh_report-0.7.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/__main__.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/api.py
--rw-r--r--   0        0        0    12260 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/cli.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/errors.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/log.py
--rw-r--r--   0        0        0    45055 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/project.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/sphinx_app.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/version.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/__init__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/api.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/context.py
--rw-r--r--   0        0        0     9632 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/finder.py
--rw-r--r--   0        0        0    15749 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/generation.py
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/matlab_engine.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/resource.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/util.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/patches/.gitignore
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/patches/__init__.py
--rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/patches/_bokeh.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/patches/_holoviews.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/patches/_matplotlib.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/patches/_pandas.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/patches/_panel.py
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/patches/_plotly.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/assetlib/patches/bokeh_embed.html
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/api.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/contextvar.py
--rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/plugin_manager.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/spec.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/__init__.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/default_settings.yaml
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/plugin.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/asset_templates/datatable.rst.jinja2
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/asset_templates/error.rst.jinja2
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/asset_templates/iframe.rst.jinja2
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/asset_templates/image.rst.jinja2
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/asset_templates/include_wrapper.rst.jinja2
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/asset_templates/markdown.rst.jinja2
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/asset_templates/raw_html.rst.jinja2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/asset_templates/raw_rst.rst.jinja2
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/asset_templates/raw_txt.rst.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/empty/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/empty/default_context.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/empty/index.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/empty/asset_scripts/default_assets.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/__init__.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/conf.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/debug.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/index.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-archive.cmd
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-build.cmd
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-generate-assets.cmd
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh.cmd.jinja2
--rw-r--r--   0        0        0    12674 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/html_logo.png
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/sphinx_rtd_theme_overrides.css
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/css/override_datatables.css
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/footer.html
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/layout.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/user_templates/placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/first_level/__init__.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/first_level/find.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/first_level/render.py
--rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/first_level/scaffolder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/second_level/__init__.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/second_level/env_filters.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/second_level/env_globals.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/second_level/env_tests.py
--rw-r--r--   0        0        0    16536 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/second_level/template_env.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/second_level/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/second_level/sphinx_ext/__init__.py
--rw-r--r--   0        0        0    12635 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/second_level/sphinx_ext/asset_ext.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/second_level/sphinx_ext/asset_tmpl.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/templating/second_level/sphinx_ext/jinja_ext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/util/__init__.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/util/contextlib_chdir.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/util/json_encoder.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/util/mergedeep.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pharaoh/util/oc_resolvers.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/README.md
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 pharaoh_report-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/__main__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/api.py
+-rw-r--r--   0        0        0    12260 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/cli.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/errors.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/log.py
+-rw-r--r--   0        0        0    45028 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/project.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/sphinx_app.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/version.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/__init__.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/api.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/context.py
+-rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/finder.py
+-rw-r--r--   0        0        0    15818 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/generation.py
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/matlab_engine.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/resource.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/util.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/.gitignore
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/__init__.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_bokeh.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_holoviews.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_matplotlib.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_pandas.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_panel.py
+-rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/_plotly.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/assetlib/patches/bokeh_embed.html
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/api.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/contextvar.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/plugin_manager.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/spec.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/__init__.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/default_settings.yaml
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/plugin.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/datatable.rst.jinja2
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/error.rst.jinja2
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/iframe.rst.jinja2
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/image.rst.jinja2
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/include_wrapper.rst.jinja2
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/markdown.rst.jinja2
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/raw_html.rst.jinja2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/raw_rst.rst.jinja2
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/raw_txt.rst.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/empty/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/empty/default_context.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/empty/index.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/empty/asset_scripts/default_assets.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/conf.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/debug.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/index.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-archive.cmd
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-build.cmd
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh-generate-assets.cmd
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/pharaoh.cmd.jinja2
+-rw-r--r--   0        0        0    12674 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/html_logo.png
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/sphinx_rtd_theme_overrides.css
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/css/override_datatables.css
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/footer.html
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/layout.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/user_templates/placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/first_level/__init__.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/first_level/find.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/first_level/render.py
+-rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/first_level/scaffolder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/__init__.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/env_filters.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/env_globals.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/env_tests.py
+-rw-r--r--   0        0        0    16068 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/template_env.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/__init__.py
+-rw-r--r--   0        0        0    12647 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/asset_ext.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/asset_tmpl.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/jinja_ext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/util/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/util/contextlib_chdir.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/util/json_encoder.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/util/mergedeep.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pharaoh/util/oc_resolvers.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/README.md
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 pharaoh_report-0.7.0/PKG-INFO
```

### Comparing `pharaoh_report-0.6.2/pharaoh/cli.py` & `pharaoh_report-0.7.0/pharaoh/cli.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/log.py` & `pharaoh_report-0.7.0/pharaoh/log.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/project.py` & `pharaoh_report-0.7.0/pharaoh/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import copy
 import datetime
 import functools
 import logging
 import os
 import re
 import shutil
 import sys
@@ -559,15 +558,15 @@
         """
         found = []
         for comp in self.iter_components():
             if not expression:
                 found.append(comp)
                 continue
             try:
-                result = eval(expression, {}, copy.deepcopy(comp))
+                result = eval(expression, {}, comp)
             except Exception:
                 result = False
             if result:
                 found.append(comp)
         return found
 
     def get_resource(self, alias: str, component: str) -> resource.Resource:
```

### Comparing `pharaoh_report-0.6.2/pharaoh/sphinx_app.py` & `pharaoh_report-0.7.0/pharaoh/sphinx_app.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/api.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa: F401,F403
 """
 This module contains API functions related to asset generation.
 When asset scripts are accessing those API functions, the functions can access the project information by themselves.
 """
+
 # Don't remove unused imports. They may be unused here but maybe in user code!
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from pharaoh.assetlib.context import metadata_context
 from pharaoh.assetlib.generation import register_asset, register_templating_context
```

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/context.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/context.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/finder.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,33 +84,45 @@
 
         if Path(self.assetfile).is_dir():
             shutil.copytree(self.assetfile, target_dir / self.assetfile.name)
             return target_dir / self.assetfile.name
 
         raise NotImplementedError
 
-    def read_json(self):
+    def read_json(self) -> dict:
+        """
+        Reads the file using a JSON parser.
+        """
         if self.assetfile.suffix.lower() != ".json":
             msg = "Can only read .json files!"
             raise Exception(msg)
         return json.loads(self.assetfile.read_text("utf-8"))
 
-    def read_yaml(self):
+    def read_yaml(self) -> dict:
+        """
+        Reads the file using a YAML parser.
+        """
         import yaml
 
-        if self.assetfile.suffix.lower() != ".yaml":
-            msg = "Can only read .yaml files!"
+        if self.assetfile.suffix.lower() not in (".yaml", ".yml"):
+            msg = "Can only read .yaml/.yml files!"
             raise Exception(msg)
         with open(self.assetfile, encoding="utf-8") as fp:
-            return yaml.load(fp, yaml.Loader)
+            return yaml.safe_load(fp)
 
-    def read_text(self, encoding: str = "utf-8"):
+    def read_text(self, encoding: str = "utf-8") -> str:
+        """
+        Reads the file as text
+        """
         return self.assetfile.read_text(encoding)
 
-    def read_bytes(self):
+    def read_bytes(self) -> bytes:
+        """
+        Reads the file as bytes
+        """
         return self.assetfile.read_bytes()
 
 
 class AssetFinder:
     def __init__(self, lookup_path: Path):
         """
         A class for discovering and searching generated assets.
@@ -167,15 +179,15 @@
             return []
 
         code = compile(condition, "<string>", "eval")
         found = []
 
         for asset in self.iter_assets(components):
             try:
-                result = eval(code, {}, asset.context.copy())
+                result = eval(code, {}, asset.context)
             except Exception:
                 result = False
             if result:
                 found.append(asset)
 
         def sort_key(asset):
             try:
```

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/generation.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,22 +52,25 @@
         script_path = asset_src.relative_to(project_root).as_posix()
     except ValueError:
         script_path = asset_src.as_posix()
 
     if asset_src.suffix.lower() == ".py":
         script_ignore_pattern = proj.get_setting("asset_gen.script_ignore_pattern")
 
-        with patches.patch_3rd_party_libraries(), context_stack.new_context(
-            context_name="generate_assets",
-            asset={
-                "script_name": asset_src.name,
-                "script_path": asset_src,
-                "index": 0,
-                "component_name": component_name,
-            },
+        with (
+            patches.patch_3rd_party_libraries(),
+            context_stack.new_context(
+                context_name="generate_assets",
+                asset={
+                    "script_name": asset_src.name,
+                    "script_path": asset_src,
+                    "index": 0,
+                    "component_name": component_name,
+                },
+            ),
         ):
             code = asset_src.read_text(encoding="utf-8")
 
             first_line = code.split("\n", maxsplit=1)[0].strip()
             if re.fullmatch(script_ignore_pattern, asset_src.name) or re.fullmatch(
                 r"^# *pharaoh?: *ignore *", first_line, re.IGNORECASE
             ):
```

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/matlab_engine.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/matlab_engine.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/resource.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/resource.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/util.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/util.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/patches/__init__.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/patches/_bokeh.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_bokeh.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/patches/_holoviews.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_holoviews.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/patches/_matplotlib.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_matplotlib.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/patches/_pandas.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_pandas.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/patches/_panel.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_panel.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/patches/_plotly.py` & `pharaoh_report-0.7.0/pharaoh/assetlib/patches/_plotly.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/assetlib/patches/bokeh_embed.html` & `pharaoh_report-0.7.0/pharaoh/assetlib/patches/bokeh_embed.html`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/contextvar.py` & `pharaoh_report-0.7.0/pharaoh/plugins/contextvar.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/plugin_manager.py` & `pharaoh_report-0.7.0/pharaoh/plugins/plugin_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,15 @@
         self.pm = pluggy.PluginManager("pharaoh")
 
         def before(hook_name, hook_impls, kwargs):
             ...
             # log.debug(f"Plugins: Executing hook {hook_name!r} from plugins " +
             #           ", ".join([impl.plugin_name for impl in hook_impls]))
 
-        def after(outcome, hook_name, hook_impls, kwargs):
-            ...
+        def after(outcome, hook_name, hook_impls, kwargs): ...
 
         self.pm.add_hookcall_monitoring(before=before, after=after)
         self.pm.add_hookspecs(spec)
         self.reload_plugins()
 
     def reload_plugins(self):
         for name, plugin in self.pm.list_name_plugin():
```

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/spec.py` & `pharaoh_report-0.7.0/pharaoh/plugins/spec.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/template.py` & `pharaoh_report-0.7.0/pharaoh/plugins/template.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/default_settings.yaml` & `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/plugin.py` & `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/asset_templates/datatable.rst.jinja2` & `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/asset_templates/datatable.rst.jinja2`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/conf.py` & `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Configuration file for the Sphinx documentation builder.
 
 This file only contains a selection of the most common options. For a full
 list see the documentation:
 https://www.sphinx-doc.org/en/master/usage/configuration.html
 """
+
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any, Callable
 
 from pharaoh.api import PharaohProject
```

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/html_logo.png` & `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/html_logo.png`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/sphinx_rtd_theme_overrides.css` & `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/sphinx_rtd_theme_overrides.css`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/css/override_datatables.css` & `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_static/css/override_datatables.css`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/layout.html` & `pharaoh_report-0.7.0/pharaoh/plugins/core_plugin/level_1/pharaoh_sphinx_project/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/templating/first_level/find.py` & `pharaoh_report-0.7.0/pharaoh/templating/first_level/find.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/templating/first_level/render.py` & `pharaoh_report-0.7.0/pharaoh/templating/first_level/render.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/templating/first_level/scaffolder.py` & `pharaoh_report-0.7.0/pharaoh/templating/first_level/scaffolder.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/templating/second_level/env_filters.py` & `pharaoh_report-0.7.0/pharaoh/templating/second_level/env_filters.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/templating/second_level/env_globals.py` & `pharaoh_report-0.7.0/pharaoh/templating/second_level/env_globals.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/templating/second_level/template_env.py` & `pharaoh_report-0.7.0/pharaoh/templating/second_level/template_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import copy
 import functools
 import os
 import pprint
 import shutil
 import uuid
 from functools import partial
 from pathlib import Path
@@ -198,17 +197,15 @@
         source[0] = rendered  # source item 0 must be modified in place
 
     def sphinx_include_read_hook(self, app: PharaohSphinx, relative_path, parent_docname, content):
         file = Path(self.sphinx_app.srcdir) / relative_path
         rendered, _ = self.render_file(file)
         content[0] = rendered
 
-    def render_file(self, docname: Path | str, additional_context: dict | None = None) -> tuple[str, Path]:
-        context = {}
-
+    def render_file(self, docname: Path | str) -> tuple[str, Path]:
         project: pharaoh.project.PharaohProject = self.sphinx_app.pharaoh_proj
 
         if isinstance(docname, str):
             template_file = Path(self.sphinx_app.env.doc2path(docname))
         elif isinstance(docname, Path):
             template_file = docname
         else:
@@ -222,54 +219,51 @@
                 parts = template_file.relative_to(components_dir).parts
                 component_name = "" if len(parts) < 2 else parts[0]
             except ValueError:
                 component_name = ""
 
             # Context Creation
             log.debug(f"Discovering additional templating context for component {component_name!r}...")
-            context = copy.deepcopy(self.default_context)
-            context["project"]["component_name"] = component_name
-            for key, ctx in self.read_local_context_files(context, template_file.parent).items():
+            self.default_context["project"]["component_name"] = component_name
+            self.default_context["local"] = {}
+
+            for key, ctx in self.read_local_context_files(self.default_context, template_file.parent).items():
                 log.debug(f"... discovered local context {key!r}")
-                if key in context["local"]:
+                if key in self.default_context["local"]:
                     log.warning(f"Overwriting existing local context namespace {key!r}!")
-                context["local"][key] = ctx
+                self.default_context["local"][key] = ctx
 
             for key, ctx in self.read_asset_context_files(component=component_name):
                 log.debug(f"... discovered asset context {key!r}")
-                if key in context["local"]:
+                if key in self.default_context["local"]:
                     log.warning(f"Overwriting existing local context namespace {key!r}!")
-                context["local"][key] = ctx
-
-            # additional_context only has data if this function is called by the global function "render_template"
-            for key, val in (additional_context or {}).items():
-                if key in context:
-                    log.warning(f"Overwriting existing context key {key}!")
-                context[key] = val
+                self.default_context["local"][key] = ctx
 
             render_globals = {
                 "search_assets": functools.partial(project.asset_finder.search_assets, components=[component_name]),
                 "asset_rel_path_from_project": partial(asset_rel_path_from_project, project),
                 "asset_rel_path_from_build": partial(asset_rel_path_from_build, self.sphinx_app, template_file),
             }
 
             with chdir(template_file.parent):
                 template = self.select_template([template_file.name], parent=str(template_file.parent))
-                rendered = template.render({"ctx": context}, **render_globals)
+                rendered = template.render({"ctx": self.default_context}, **render_globals)
 
             rendered_file = template_file.parent / (template_file.name + ".rendered")
             rendered_file.write_text(rendered)
             return rendered, rendered_file
         except Exception:
             log.error(
                 f"Error in PharaohTemplateEnv.sphinx_source_read_hook while trying to render template "
-                f"{template_file} with context {pprint.pformat(context)}!",
+                f"{template_file} with context {pprint.pformat(self.default_context)}!",
                 exc_info=True,
             )
             raise
+        finally:
+            self.default_context["local"] = {}
 
     def join_path(self, template: str, parent: str) -> str:
         """
         Join a template with the parent. By default, all the lookups are
         relative to the loader root so this method returns the `template`
         parameter unchanged, but if the paths should be relative to the
         parent template, this function can be used to calculate the real
@@ -307,17 +301,14 @@
         for file in basepath.glob("*_context.py"):
             f = Path(file)
             key = f.name.rsplit("_", 1)[0]
             if f in self.local_context_file_cache:
                 module = self.local_context_file_cache[f]
             else:
                 module = module_from_file(f)
-                eval_ctx = copy.deepcopy(base_context)
-                eval_ctx["local"] = local_context  # Pass in previously read context to allow more powerful scripts
-                module.__dict__["base_ctx"] = eval_ctx
                 run_module(module, f.read_text(encoding="utf-8"))
                 self.local_context_file_cache[f] = module
             result_ctx: dict = module.__dict__
             if not ("context" in result_ctx and isinstance(result_ctx["context"], dict)):
                 msg = (
                     "No dict-typed variable named 'context' was defined by the script!\n"
                     "Example of valid script content: context={}"
```

### Comparing `pharaoh_report-0.6.2/pharaoh/templating/second_level/util.py` & `pharaoh_report-0.7.0/pharaoh/templating/second_level/util.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/templating/second_level/sphinx_ext/asset_ext.py` & `pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/asset_ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,16 @@
     if not arg or not arg.strip():
         # no argument given, assume used as a flag
         return True
     if arg.strip().lower() in ("no", "0", "false"):
         return False
     if arg.strip().lower() in ("yes", "1", "true"):
         return True
-    raise ValueError('"%s" unknown boolean' % arg)
+    msg = f'"{arg}" unknown boolean'
+    raise ValueError(msg)
 
 
 # -------------------------------------
 # Directive
 # -------------------------------------
 class PharaohAssetDirective(Directive):
     """The ``.. pharaoh-asset::`` directive."""
```

### Comparing `pharaoh_report-0.6.2/pharaoh/templating/second_level/sphinx_ext/asset_tmpl.py` & `pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/asset_tmpl.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/templating/second_level/sphinx_ext/jinja_ext.py` & `pharaoh_report-0.7.0/pharaoh/templating/second_level/sphinx_ext/jinja_ext.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/util/contextlib_chdir.py` & `pharaoh_report-0.7.0/pharaoh/util/contextlib_chdir.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Backport of contextlib.chdir stdlib class added in Python3.11.
 """
+
 from __future__ import annotations
 
 import os
 from contextlib import AbstractContextManager
 from pathlib import Path
```

### Comparing `pharaoh_report-0.6.2/pharaoh/util/json_encoder.py` & `pharaoh_report-0.7.0/pharaoh/util/json_encoder.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/util/mergedeep.py` & `pharaoh_report-0.7.0/pharaoh/util/mergedeep.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pharaoh/util/oc_resolvers.py` & `pharaoh_report-0.7.0/pharaoh/util/oc_resolvers.py`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/LICENSE.txt` & `pharaoh_report-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/README.md` & `pharaoh_report-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pharaoh_report-0.6.2/pyproject.toml` & `pharaoh_report-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 license = { text = "MIT" }
 keywords = [
     "reporting",
     "sphinx",
     "jinja",
     "templating",
 ]
-requires-python = ">=3.9.2, <3.13"
+requires-python = ">=3.9.2"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX",
   "Programming Language :: Python :: 3 :: Only",
@@ -44,30 +44,29 @@
 urls.Tracker = "https://github.com/Infineon/pharaoh-dev/issues"
 
 dependencies = [
     "attrs",
     "click", # CLI
     "omegaconf", # yaml R/W
     "natsort", # sorting paths naturally
-    "pyyaml==5.3.1",  # https://github.com/yaml/pyyaml/issues/724
+    "pyyaml!=5.3.0",
     "pluggy",
     "nbconvert", # used to programmatically execute asset notebooks",
     "mistletoe", # Markdown to HTML
     # Sphinx, theme & extensions
     "sphinx >=7.2.5, <8.0",
     "sphinxcontrib-jquery",
     "sphinx-design",
     "sphinx-rtd-theme",
     #    "sphinx-toolbox",
     #    "sphinx-data-viewer",
     # Jinja & extensions
     "jinja2",
     "jinja2-git",
     "jinja2-ansible-filters",
-    "numpy<2.0", # transitive dependency only # todo: remove this requirement once compatibility with 2.x is tested
     "wrapt",
 ]
 
 [project.optional-dependencies]
 bokeh = [
     "bokeh>=3.0.0,<3.3.0; python_version>='3.9'",
     "bokeh>=3.1.0,<3.3.0; python_version>='3.11'",
@@ -160,17 +159,24 @@
     "def __repr__",
     "def __str__",
     "if self.debug:",
     "if settings.DEBUG",
     "raise AssertionError",
 ]
 
+
 [tool.ruff]
-src = ["src", "tests"]
-preview = false
+# https://docs.astral.sh/ruff/settings
+target-version = "py39"
+line-length = 120
+fix = false  # Allow autofix for all enabled rules (when `--fix`) is provided.
+show-fixes = true
+unsafe-fixes = true
+
+[tool.ruff.lint]
 select = [
     "E",  # pycodestyle errors
     "F",  # pyflakes
     "I",   # isort
     "UP",  # pyupgrade
     "B",  # bugbear
     "C4",  # flake8-comprehensions
@@ -184,42 +190,33 @@
     "SIM",  # flake8-simplify
     "TID252",  # flake8-tidy-imports -> convert relative-imports (makes absolufiy-imports hook redundant)
     "TCH",  # flake8-type-checking
     "PLE",  # Pylint - errors
     "PLW",  # Pylint - warnings
     "PLC",  # Pylint - conventions
     "RUF",  # Ruff-specific rules
-
-    # Enable those later maybe when there's time to fix those errors
-    # "BLE",  # flake8-blind-except
-    # "PTH",  # flake8-use-pathlib
-    # "NPY",  # NumPy-specific rules
 ]
 ignore = [
     "PLW2901",  # Pylint - warnings: redefined-loop-name
     "E501", # https://docs.astral.sh/ruff/faq/#is-the-ruff-linter-compatible-with-black
 ]
 exclude = []
-fix = true  # Allow autofix for all enabled rules (when `--fix`) is provided.
-unsafe-fixes = true
-show-fixes = true
-line-length = 120  # Same as Black.
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-isort = {known-first-party = ["pharaoh", "tests"], required-imports = ["from __future__ import annotations"]}
+[tool.ruff.lint.isort]
+known-first-party = ["pharaoh", "test"]
+required-imports = ["from __future__ import annotations"]
 
-
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "api.py" = ["F401"]
 
-
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 # Whether to ban all relative imports ("all"),
 # or only those imports that extend into the parent module or beyond ("parents").
 ban-relative-imports = "parents"
 
 
 [tool.mypy]
 python_version = "3.11"
```

### Comparing `pharaoh_report-0.6.2/PKG-INFO` & `pharaoh_report-0.7.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pharaoh-report
-Version: 0.6.2
+Version: 0.7.0
 Summary: Pharaoh is a Sphinx-based Python framework for generating reports in various formats by combining the power of configurable Jinja templates and Python scripts for asset generation.
 Project-URL: Documentation, https://infineon.github.io/pharaoh-dev/
 Project-URL: Homepage, https://infineon.github.io/pharaoh-dev/
 Project-URL: Release Notes, https://infineon.github.io/pharaoh-dev/changelog.html
 Project-URL: Source, https://github.com/Infineon/pharaoh-dev
 Project-URL: Tracker, https://github.com/Infineon/pharaoh-dev/issues
 Author: Johannes Loibl
@@ -19,49 +19,70 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: <3.13,>=3.9.2
+Requires-Python: >=3.9.2
 Requires-Dist: attrs
 Requires-Dist: click
 Requires-Dist: jinja2
 Requires-Dist: jinja2-ansible-filters
 Requires-Dist: jinja2-git
 Requires-Dist: mistletoe
 Requires-Dist: natsort
 Requires-Dist: nbconvert
-Requires-Dist: numpy<2.0
 Requires-Dist: omegaconf
 Requires-Dist: pluggy
-Requires-Dist: pyyaml==5.3.1
+Requires-Dist: pyyaml!=5.3.0
 Requires-Dist: sphinx-design
 Requires-Dist: sphinx-rtd-theme
 Requires-Dist: sphinx<8.0,>=7.2.5
 Requires-Dist: sphinxcontrib-jquery
 Requires-Dist: wrapt
 Provides-Extra: all-plotting
-Requires-Dist: pharaoh-report[bokeh,holoviews,jupyter,matplotlib,pandas,plotly]; extra == 'all-plotting'
+Requires-Dist: bokeh<3.3.0,>=3.0.0; (python_version >= '3.9') and extra == 'all-plotting'
+Requires-Dist: bokeh<3.3.0,>=3.1.0; (python_version >= '3.11') and extra == 'all-plotting'
+Requires-Dist: holoviews; extra == 'all-plotting'
+Requires-Dist: holoviews>=1.16; (python_version >= '3.11') and extra == 'all-plotting'
+Requires-Dist: jupyter; extra == 'all-plotting'
+Requires-Dist: jupyter-contrib-nbextensions; extra == 'all-plotting'
+Requires-Dist: kaleido; (platform_system == 'Linux') and extra == 'all-plotting'
+Requires-Dist: kaleido==0.1.0.post1; (platform_system == 'Windows') and extra == 'all-plotting'
+Requires-Dist: matplotlib; extra == 'all-plotting'
+Requires-Dist: pandas>=1.5; extra == 'all-plotting'
+Requires-Dist: plotly; extra == 'all-plotting'
+Requires-Dist: selenium>=4.11; extra == 'all-plotting'
 Provides-Extra: bokeh
 Requires-Dist: bokeh<3.3.0,>=3.0.0; (python_version >= '3.9') and extra == 'bokeh'
 Requires-Dist: bokeh<3.3.0,>=3.1.0; (python_version >= '3.11') and extra == 'bokeh'
 Requires-Dist: selenium>=4.11; extra == 'bokeh'
 Provides-Extra: dev
+Requires-Dist: bokeh<3.3.0,>=3.0.0; (python_version >= '3.9') and extra == 'dev'
+Requires-Dist: bokeh<3.3.0,>=3.1.0; (python_version >= '3.11') and extra == 'dev'
 Requires-Dist: diff-cover>=7.7; extra == 'dev'
 Requires-Dist: gitpython; extra == 'dev'
-Requires-Dist: pharaoh-report[all-plotting]; extra == 'dev'
+Requires-Dist: holoviews; extra == 'dev'
+Requires-Dist: holoviews>=1.16; (python_version >= '3.11') and extra == 'dev'
+Requires-Dist: jupyter; extra == 'dev'
+Requires-Dist: jupyter-contrib-nbextensions; extra == 'dev'
+Requires-Dist: kaleido; (platform_system == 'Linux') and extra == 'dev'
+Requires-Dist: kaleido==0.1.0.post1; (platform_system == 'Windows') and extra == 'dev'
+Requires-Dist: matplotlib; extra == 'dev'
+Requires-Dist: pandas>=1.5; extra == 'dev'
+Requires-Dist: plotly; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-mock; extra == 'dev'
 Requires-Dist: pytest-randomly; extra == 'dev'
 Requires-Dist: pytest-sugar; extra == 'dev'
 Requires-Dist: pytest-timeout; extra == 'dev'
 Requires-Dist: pytest-xdist; extra == 'dev'
+Requires-Dist: selenium>=4.11; extra == 'dev'
 Requires-Dist: setuptools-scm; extra == 'dev'
 Requires-Dist: tox; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: numpy<2.0; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Requires-Dist: sphinx-jinja; extra == 'docs'
```

