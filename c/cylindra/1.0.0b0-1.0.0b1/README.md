# Comparing `tmp/cylindra-1.0.0b0.tar.gz` & `tmp/cylindra-1.0.0b1.tar.gz`

## Comparing `cylindra-1.0.0b0.tar` & `cylindra-1.0.0b1.tar`

### file list

```diff
@@ -1,224 +1,225 @@
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 cylindra-1.0.0b0/Cargo.toml
--rw-r--r--   0     1001      127     2783 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     1132 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/.github/workflows/docs.yml
--rw-r--r--   0     1001      127     1589 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/.github/workflows/test.yml
--rw-r--r--   0     1001      127     1991 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/.gitignore
--rw-r--r--   0     1001      127      502 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1517 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/LICENSE
--rw-r--r--   0     1001      127     2735 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/README.md
--rw-r--r--   0     1001      127     1045 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/__init__.py
--rw-r--r--   0     1001      127     1085 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/__main__.py
--rw-r--r--   0     1001      127     8242 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_config.py
--rw-r--r--   0     1001      127     5180 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_cylindra_ext.pyi
--rw-r--r--   0     1001      127      390 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_dask.py
--rw-r--r--   0     1001      127      276 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_data/BtubAB.json
--rw-r--r--   0     1001      127      282 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_data/TMV.json
--rw-r--r--   0     1001      127      277 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_data/actin.json
--rw-r--r--   0     1001      127      283 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_data/eukaryotic_MT.json
--rw-r--r--   0     1001      127      288 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_napari/__init__.py
--rw-r--r--   0     1001      127     7413 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_napari/_layer_controls.py
--rw-r--r--   0     1001      127    16169 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_napari/_layers.py
--rw-r--r--   0     1001      127     5967 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_previews.py
--rw-r--r--   0     1001      127     6756 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/_shared_doc.py
--rw-r--r--   0     1001      127      813 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/__init__.py
--rw-r--r--   0     1001      127     2715 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/_base.py
--rw-r--r--   0     1001      127     3249 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/average.py
--rw-r--r--   0     1001      127     5555 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/config.py
--rw-r--r--   0     1001      127     5455 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/find.py
--rw-r--r--   0     1001      127     3170 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/new.py
--rw-r--r--   0     1001      127     1468 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/none.py
--rw-r--r--   0     1001      127     2869 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/open.py
--rw-r--r--   0     1001      127     5886 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/preview.py
--rw-r--r--   0     1001      127     1842 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/run.py
--rw-r--r--   0     1001      127     2582 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cli/workflow.py
--rw-r--r--   0     1001      127      580 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/__init__.py
--rw-r--r--   0     1001      127     1894 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/_base.py
--rw-r--r--   0     1001      127     8182 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/_cylinder_params.py
--rw-r--r--   0     1001      127     8355 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/_ftprops.py
--rw-r--r--   0     1001      127     7230 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/_peak.py
--rw-r--r--   0     1001      127    16282 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/cylindric.py
--rw-r--r--   0     1001      127    28246 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/landscape.py
--rw-r--r--   0     1001      127     5181 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/picker.py
--rw-r--r--   0     1001      127     5931 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/seam_search.py
--rw-r--r--   0     1001      127      231 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/spline/__init__.py
--rw-r--r--   0     1001      127     6377 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/spline/_config.py
--rw-r--r--   0     1001      127     8360 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/spline/_cyl_spline.py
--rw-r--r--   0     1001      127     7817 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/spline/_props.py
--rw-r--r--   0     1001      127    39295 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/spline/_spline_base.py
--rw-r--r--   0     1001      127      810 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/spline/_types.py
--rw-r--r--   0     1001      127      163 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/tomogram/__init__.py
--rw-r--r--   0     1001      127    51468 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/tomogram/_cyl_tomo.py
--rw-r--r--   0     1001      127     5500 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/tomogram/_spline_list.py
--rw-r--r--   0     1001      127     2614 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/tomogram/_straighten.py
--rw-r--r--   0     1001      127    13212 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/tomogram/_tomo_base.py
--rw-r--r--   0     1001      127     3541 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/components/visualize.py
--rw-r--r--   0     1001      127     6255 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/const.py
--rw-r--r--   0     1001      127     7319 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/core.py
--rw-r--r--   0     1001      127     7437 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cylfilters.py
--rw-r--r--   0     1001      127    16394 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cylmeasure.py
--rw-r--r--   0     1001      127     2473 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/cyltransform.py
--rw-r--r--   0     1001      127      219 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/ext/__init__.py
--rw-r--r--   0     1001      127     1386 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/ext/_utils.py
--rw-r--r--   0     1001      127      159 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/ext/imod/__init__.py
--rw-r--r--   0     1001      127     4057 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/ext/imod/cmd.py
--rw-r--r--   0     1001      127    12506 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/ext/imod/menu.py
--rw-r--r--   0     1001      127       66 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/ext/relion/__init__.py
--rw-r--r--   0     1001      127     8277 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/ext/relion/menu.py
--rw-r--r--   0     1001      127      397 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/project/__init__.py
--rw-r--r--   0     1001      127     6119 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/project/_base.py
--rw-r--r--   0     1001      127     4975 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/project/_batch.py
--rw-r--r--   0     1001      127      790 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/project/_json.py
--rw-r--r--   0     1001      127     4719 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/project/_layer_info.py
--rw-r--r--   0     1001      127    23310 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/project/_sequence.py
--rw-r--r--   0     1001      127    20162 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/project/_single.py
--rw-r--r--   0     1001      127     1272 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/project/_utils.py
--rw-r--r--   0     1001      127     7390 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/project/_widgets.py
--rw-r--r--   0     1001      127     1519 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/types.py
--rw-r--r--   0     1001      127      155 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/utils/__init__.py
--rw-r--r--   0     1001      127      366 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/utils/_color.py
--rw-r--r--   0     1001      127     2878 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/utils/_correlation.py
--rw-r--r--   0     1001      127     9936 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/utils/_misc.py
--rw-r--r--   0     1001      127    11214 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widget_utils.py
--rw-r--r--   0     1001      127     1036 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/__init__.py
--rw-r--r--   0     1001      127     9318 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/_accessors.py
--rw-r--r--   0     1001      127     5906 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/_annealing.py
--rw-r--r--   0     1001      127     2273 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/_annotated.py
--rw-r--r--   0     1001      127     5371 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/_main_utils.py
--rw-r--r--   0     1001      127     4009 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/_process_template.py
--rw-r--r--   0     1001      127     2742 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/_progress_desc.py
--rw-r--r--   0     1001      127     4833 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/_reserved_layers.py
--rw-r--r--   0     1001      127    18057 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/_ui_init.py
--rw-r--r--   0     1001      127    25893 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/_widget_ext.py
--rw-r--r--   0     1001      127      154 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/batch/__init__.py
--rw-r--r--   0     1001      127     2291 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/batch/_loaderlist.py
--rw-r--r--   0     1001      127    16297 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/batch/_sequence.py
--rw-r--r--   0     1001      127     3601 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/batch/_utils.py
--rw-r--r--   0     1001      127     8830 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/batch/main.py
--rw-r--r--   0     1001      127      859 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/batch/menus.py
--rw-r--r--   0     1001      127    23188 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/batch/sta.py
--rw-r--r--   0     1001      127      510 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/icons/grip.svg
--rw-r--r--   0     1001      127   111878 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/main.py
--rw-r--r--   0     1001      127    80535 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/sta.py
--rw-r--r--   0     1001      127      226 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/style.qss
--rw-r--r--   0     1001      127     1542 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/__init__.py
--rw-r--r--   0     1001      127      291 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/_child_widget.py
--rw-r--r--   0     1001      127     6630 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/file_iter.py
--rw-r--r--   0     1001      127    10046 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/function_menu.py
--rw-r--r--   0     1001      127     6872 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/image_processor.py
--rw-r--r--   0     1001      127     9318 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/measure.py
--rw-r--r--   0     1001      127    44223 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/menus.py
--rw-r--r--   0     1001      127     6611 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/misc.py
--rw-r--r--   0     1001      127     1869 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/pca.py
--rw-r--r--   0     1001      127     8982 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/properties.py
--rw-r--r--   0     1001      127     6455 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/runner.py
--rw-r--r--   0     1001      127    37183 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/simulator.py
--rw-r--r--   0     1001      127    16958 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/slicer.py
--rw-r--r--   0     1001      127     6115 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/spline_clipper.py
--rw-r--r--   0     1001      127    12792 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/spline_control.py
--rw-r--r--   0     1001      127    10434 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/spline_fitter.py
--rw-r--r--   0     1001      127     3585 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/cylindra/widgets/subwidgets/toolbar.py
--rw-r--r--   0     1001      127     7412 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/alignment/conventional.md
--rw-r--r--   0     1001      127     1344 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/alignment/index.md
--rw-r--r--   0     1001      127     2168 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/alignment/landscape.md
--rw-r--r--   0     1001      127     1940 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/alignment/rma.md
--rw-r--r--   0     1001      127     1571 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/alignment/viterbi.md
--rw-r--r--   0     1001      127      641 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/components.md
--rw-r--r--   0     1001      127      115 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/core.md
--rw-r--r--   0     1001      127      127 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/cylfilters.md
--rw-r--r--   0     1001      127      127 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/cylmeasure.md
--rw-r--r--   0     1001      127      302 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/ext.md
--rw-r--r--   0     1001      127       73 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/index.md
--rw-r--r--   0     1001      127      121 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/project.md
--rw-r--r--   0     1001      127      453 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/widgets/batch.md
--rw-r--r--   0     1001      127      169 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/widgets/main.md
--rw-r--r--   0     1001      127      221 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/widgets/sta.md
--rw-r--r--   0     1001      127      223 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/api/widgets/subwidgets.md
--rw-r--r--   0     1001      127     5676 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/basics.md
--rw-r--r--   0     1001      127      343 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/batch/average.md
--rw-r--r--   0     1001      127     2553 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/batch/collect_projects.md
--rw-r--r--   0     1001      127     3492 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/batch/construct.md
--rw-r--r--   0     1001      127      223 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/batch/index.md
--rw-r--r--   0     1001      127     1016 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/cli.md
--rw-r--r--   0     1001      127     2366 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/extern/imod.md
--rw-r--r--   0     1001      127      241 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/extern/index.md
--rw-r--r--   0     1001      127     1705 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/extern/relion.md
--rw-r--r--   0     1001      127     6913 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/fit_splines.md
--rw-r--r--   0     1001      127   276476 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/images/average_tubulin.png
--rw-r--r--   0     1001      127  1910217 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/images/draw_splines.gif
--rw-r--r--   0     1001      127  2869509 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/images/generate_molecules.gif
--rw-r--r--   0     1001      127    65566 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/images/lattice_params.png
--rw-r--r--   0     1001      127     2447 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/index.md
--rw-r--r--   0     1001      127     1844 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/installation.md
--rw-r--r--   0     1001      127    13432 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/lattice_params.md
--rw-r--r--   0     1001      127     2212 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/molecules/expressions.md
--rw-r--r--   0     1001      127     3122 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/molecules/features.md
--rw-r--r--   0     1001      127     1744 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/molecules/filter_molecules.md
--rw-r--r--   0     1001      127     2684 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/molecules/headers.md
--rw-r--r--   0     1001      127      467 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/molecules/index.md
--rw-r--r--   0     1001      127     9053 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/molecules/spline_to_molecules.md
--rw-r--r--   0     1001      127     2452 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/molecules/split_and_combine.md
--rw-r--r--   0     1001      127     1733 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/molecules/transform.md
--rw-r--r--   0     1001      127     7627 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/open_image.md
--rw-r--r--   0     1001      127      622 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/process_images.md
--rw-r--r--   0     1001      127     3071 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/project_io.md
--rw-r--r--   0     1001      127      903 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/scripts/_dynamic_doc.py
--rw-r--r--   0     1001      127     5510 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/scripts/_screenshots.py
--rw-r--r--   0     1001      127     2889 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/seam_search.md
--rw-r--r--   0     1001      127     6243 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/simulate.md
--rw-r--r--   0     1001      127     1954 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/spline/clip.md
--rw-r--r--   0     1001      127     3891 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/spline/config.md
--rw-r--r--   0     1001      127      300 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/spline/index.md
--rw-r--r--   0     1001      127     3864 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/docs/workflows.md
--rw-r--r--   0     1001      127     3216 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/mkdocs.yml
--rw-r--r--   0     1001      127   845316 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/resources/fig.png
--rw-r--r--   0     1001      127     3278 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/scripts/annealing_demo.py
--rw-r--r--   0     1001      127     3080 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/scripts/calibrate_nsr.py
--rw-r--r--   0     1001      127     2344 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/scripts/generate_images.py
--rw-r--r--   0     1001      127     3275 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/scripts/rma_demo.py
--rw-r--r--   0     1001      127     4586 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/scripts/rma_fluctuation.py
--rw-r--r--   0     1001      127     8297 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/scripts/simulate_alignments.py
--rw-r--r--   0     1001      127    12675 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/scripts/simulate_cft.py
--rw-r--r--   0     1001      127     4063 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/scripts/simulate_supertwist.py
--rw-r--r--   0     1001      127      803 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/scripts/tip_recognition_demo.py
--rw-r--r--   0     1001      127     4215 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/alleviate.rs
--rw-r--r--   0     1001      127    11874 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/annealing/core.rs
--rw-r--r--   0     1001      127    20263 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/annealing/graph.rs
--rw-r--r--   0     1001      127      129 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/annealing/mod.rs
--rw-r--r--   0     1001      127     5940 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/annealing/potential.rs
--rw-r--r--   0     1001      127     4193 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/annealing/random.rs
--rw-r--r--   0     1001      127     1650 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/annealing/reservoir.rs
--rw-r--r--   0     1001      127     2237 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/array.rs
--rw-r--r--   0     1001      127     1999 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/coordinates/coordinate_system.rs
--rw-r--r--   0     1001      127      133 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/coordinates/mod.rs
--rw-r--r--   0     1001      127     7366 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/coordinates/vector.rs
--rw-r--r--   0     1001      127     6994 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/cylindric.rs
--rw-r--r--   0     1001      127      449 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/exceptions.rs
--rw-r--r--   0     1001      127    15711 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/filters.rs
--rw-r--r--   0     1001      127     1054 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/lib.rs
--rw-r--r--   0     1001      127    10848 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/regionprops.rs
--rw-r--r--   0     1001      127     6358 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/viterbi/constraint.rs
--rw-r--r--   0     1001      127    17258 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/viterbi/core.rs
--rw-r--r--   0     1001      127       68 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/src/viterbi/mod.rs
--rw-r--r--   0     1001      127   703618 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/13pf_MT.tif
--rw-r--r--   0     1001      127   510466 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/14pf_MT.tif
--rw-r--r--   0     1001      127      241 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/__init__.py
--rw-r--r--   0     1001      127      159 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/_const.py
--rw-r--r--   0     1001      127    33024 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/beta-tubulin.mrc
--rw-r--r--   0     1001      127     1079 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/conftest.py
--rw-r--r--   0     1001      127     6455 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_algorithms.py
--rw-r--r--   0     1001      127     1109 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_custom_widgets.py
--rw-r--r--   0     1001      127     2113 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_cylfilters.py
--rw-r--r--   0     1001      127     3084 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_cylindric_model.py
--rw-r--r--   0     1001      127    57671 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_gui_0.py
--rw-r--r--   0     1001      127     5305 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_gui_1_batch.py
--rw-r--r--   0     1001      127     2946 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_gui_2_extensions.py
--rw-r--r--   0     1001      127      322 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_io.py
--rw-r--r--   0     1001      127     1654 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_projects.py
--rw-r--r--   0     1001      127     3220 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_regionprops.py
--rw-r--r--   0     1001      127     8057 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_splines.py
--rw-r--r--   0     1001      127     5057 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_utils.py
--rw-r--r--   0     1001      127     3966 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/test_viterbi.py
--rw-r--r--   0     1001      127     2002 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/tests/utils.py
--rw-r--r--   0     1001      127    12720 2024-05-01 09:07:18.000000 cylindra-1.0.0b0/Cargo.lock
--rw-r--r--   0     1001      127     3891 2024-05-01 09:07:15.000000 cylindra-1.0.0b0/pyproject.toml
--rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 cylindra-1.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 cylindra-1.0.0b1/Cargo.toml
+-rw-r--r--   0     1001      127     2783 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     1110 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/.github/workflows/docs.yml
+-rw-r--r--   0     1001      127     1589 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     1991 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/.gitignore
+-rw-r--r--   0     1001      127      502 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1517 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/LICENSE
+-rw-r--r--   0     1001      127     3255 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/README.md
+-rw-r--r--   0     1001      127     1045 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/__init__.py
+-rw-r--r--   0     1001      127     1085 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/__main__.py
+-rw-r--r--   0     1001      127     8242 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_config.py
+-rw-r--r--   0     1001      127     5180 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_cylindra_ext.pyi
+-rw-r--r--   0     1001      127      390 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_dask.py
+-rw-r--r--   0     1001      127      276 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_data/BtubAB.json
+-rw-r--r--   0     1001      127      282 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_data/TMV.json
+-rw-r--r--   0     1001      127      277 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_data/actin.json
+-rw-r--r--   0     1001      127      283 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_data/eukaryotic_MT.json
+-rw-r--r--   0     1001      127      288 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_napari/__init__.py
+-rw-r--r--   0     1001      127     7413 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_napari/_layer_controls.py
+-rw-r--r--   0     1001      127    16169 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_napari/_layers.py
+-rw-r--r--   0     1001      127     5967 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_previews.py
+-rw-r--r--   0     1001      127     6756 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/_shared_doc.py
+-rw-r--r--   0     1001      127      813 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/__init__.py
+-rw-r--r--   0     1001      127     2715 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/_base.py
+-rw-r--r--   0     1001      127     3249 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/average.py
+-rw-r--r--   0     1001      127     5555 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/config.py
+-rw-r--r--   0     1001      127     5455 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/find.py
+-rw-r--r--   0     1001      127     3170 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/new.py
+-rw-r--r--   0     1001      127     1468 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/none.py
+-rw-r--r--   0     1001      127     2869 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/open.py
+-rw-r--r--   0     1001      127     5886 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/preview.py
+-rw-r--r--   0     1001      127     1842 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/run.py
+-rw-r--r--   0     1001      127     2582 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cli/workflow.py
+-rw-r--r--   0     1001      127      580 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/__init__.py
+-rw-r--r--   0     1001      127     1894 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/_base.py
+-rw-r--r--   0     1001      127     8182 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/_cylinder_params.py
+-rw-r--r--   0     1001      127     8355 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/_ftprops.py
+-rw-r--r--   0     1001      127     7230 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/_peak.py
+-rw-r--r--   0     1001      127    16282 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/cylindric.py
+-rw-r--r--   0     1001      127    28246 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/landscape.py
+-rw-r--r--   0     1001      127     5181 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/picker.py
+-rw-r--r--   0     1001      127     5931 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/seam_search.py
+-rw-r--r--   0     1001      127      231 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/spline/__init__.py
+-rw-r--r--   0     1001      127     6377 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/spline/_config.py
+-rw-r--r--   0     1001      127     8360 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/spline/_cyl_spline.py
+-rw-r--r--   0     1001      127     7817 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/spline/_props.py
+-rw-r--r--   0     1001      127    36534 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/spline/_spline_base.py
+-rw-r--r--   0     1001      127      810 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/spline/_types.py
+-rw-r--r--   0     1001      127      163 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/tomogram/__init__.py
+-rw-r--r--   0     1001      127    51203 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/tomogram/_cyl_tomo.py
+-rw-r--r--   0     1001      127     5588 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/tomogram/_spline_list.py
+-rw-r--r--   0     1001      127     2614 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/tomogram/_straighten.py
+-rw-r--r--   0     1001      127    13212 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/tomogram/_tomo_base.py
+-rw-r--r--   0     1001      127     3541 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/components/visualize.py
+-rw-r--r--   0     1001      127     6255 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/const.py
+-rw-r--r--   0     1001      127     7891 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/core.py
+-rw-r--r--   0     1001      127     7437 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cylfilters.py
+-rw-r--r--   0     1001      127    16394 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cylmeasure.py
+-rw-r--r--   0     1001      127     2473 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/cyltransform.py
+-rw-r--r--   0     1001      127      219 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/ext/__init__.py
+-rw-r--r--   0     1001      127     1386 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/ext/_utils.py
+-rw-r--r--   0     1001      127      159 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/ext/imod/__init__.py
+-rw-r--r--   0     1001      127     4057 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/ext/imod/cmd.py
+-rw-r--r--   0     1001      127    12506 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/ext/imod/menu.py
+-rw-r--r--   0     1001      127       66 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/ext/relion/__init__.py
+-rw-r--r--   0     1001      127     8277 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/ext/relion/menu.py
+-rw-r--r--   0     1001      127      251 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/napari.yaml
+-rw-r--r--   0     1001      127      397 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/project/__init__.py
+-rw-r--r--   0     1001      127     6198 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/project/_base.py
+-rw-r--r--   0     1001      127     5021 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/project/_batch.py
+-rw-r--r--   0     1001      127      790 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/project/_json.py
+-rw-r--r--   0     1001      127     4763 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/project/_layer_info.py
+-rw-r--r--   0     1001      127    23310 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/project/_sequence.py
+-rw-r--r--   0     1001      127    20162 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/project/_single.py
+-rw-r--r--   0     1001      127     1272 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/project/_utils.py
+-rw-r--r--   0     1001      127     7390 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/project/_widgets.py
+-rw-r--r--   0     1001      127     1519 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/types.py
+-rw-r--r--   0     1001      127      155 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/utils/__init__.py
+-rw-r--r--   0     1001      127      366 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/utils/_color.py
+-rw-r--r--   0     1001      127     2878 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/utils/_correlation.py
+-rw-r--r--   0     1001      127     9936 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/utils/_misc.py
+-rw-r--r--   0     1001      127    10465 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widget_utils.py
+-rw-r--r--   0     1001      127     1172 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/__init__.py
+-rw-r--r--   0     1001      127     9318 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/_accessors.py
+-rw-r--r--   0     1001      127     5906 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/_annealing.py
+-rw-r--r--   0     1001      127     2273 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/_annotated.py
+-rw-r--r--   0     1001      127     5371 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/_main_utils.py
+-rw-r--r--   0     1001      127     4009 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/_process_template.py
+-rw-r--r--   0     1001      127     2742 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/_progress_desc.py
+-rw-r--r--   0     1001      127     4833 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/_reserved_layers.py
+-rw-r--r--   0     1001      127    17875 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/_ui_init.py
+-rw-r--r--   0     1001      127    25893 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/_widget_ext.py
+-rw-r--r--   0     1001      127      154 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/batch/__init__.py
+-rw-r--r--   0     1001      127     2291 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/batch/_loaderlist.py
+-rw-r--r--   0     1001      127    16297 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/batch/_sequence.py
+-rw-r--r--   0     1001      127     3601 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/batch/_utils.py
+-rw-r--r--   0     1001      127     8830 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/batch/main.py
+-rw-r--r--   0     1001      127      859 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/batch/menus.py
+-rw-r--r--   0     1001      127    23188 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/batch/sta.py
+-rw-r--r--   0     1001      127      510 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/icons/grip.svg
+-rw-r--r--   0     1001      127   111869 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/main.py
+-rw-r--r--   0     1001      127    80756 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/sta.py
+-rw-r--r--   0     1001      127      226 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/style.qss
+-rw-r--r--   0     1001      127     1542 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/__init__.py
+-rw-r--r--   0     1001      127      291 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/_child_widget.py
+-rw-r--r--   0     1001      127     6630 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/file_iter.py
+-rw-r--r--   0     1001      127    10046 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/function_menu.py
+-rw-r--r--   0     1001      127     6872 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/image_processor.py
+-rw-r--r--   0     1001      127     9318 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/measure.py
+-rw-r--r--   0     1001      127    44223 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/menus.py
+-rw-r--r--   0     1001      127     6611 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/misc.py
+-rw-r--r--   0     1001      127     1869 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/pca.py
+-rw-r--r--   0     1001      127     8982 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/properties.py
+-rw-r--r--   0     1001      127     6455 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/runner.py
+-rw-r--r--   0     1001      127    39651 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/simulator.py
+-rw-r--r--   0     1001      127    16958 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/slicer.py
+-rw-r--r--   0     1001      127     6115 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/spline_clipper.py
+-rw-r--r--   0     1001      127    12792 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/spline_control.py
+-rw-r--r--   0     1001      127    10434 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/spline_fitter.py
+-rw-r--r--   0     1001      127     3585 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/cylindra/widgets/subwidgets/toolbar.py
+-rw-r--r--   0     1001      127     7412 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/alignment/conventional.md
+-rw-r--r--   0     1001      127     1344 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/alignment/index.md
+-rw-r--r--   0     1001      127     2168 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/alignment/landscape.md
+-rw-r--r--   0     1001      127     1940 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/alignment/rma.md
+-rw-r--r--   0     1001      127     1571 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/alignment/viterbi.md
+-rw-r--r--   0     1001      127      641 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/components.md
+-rw-r--r--   0     1001      127      115 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/core.md
+-rw-r--r--   0     1001      127      127 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/cylfilters.md
+-rw-r--r--   0     1001      127      127 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/cylmeasure.md
+-rw-r--r--   0     1001      127      302 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/ext.md
+-rw-r--r--   0     1001      127       73 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/index.md
+-rw-r--r--   0     1001      127      121 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/project.md
+-rw-r--r--   0     1001      127      453 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/widgets/batch.md
+-rw-r--r--   0     1001      127      169 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/widgets/main.md
+-rw-r--r--   0     1001      127      221 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/widgets/sta.md
+-rw-r--r--   0     1001      127      223 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/api/widgets/subwidgets.md
+-rw-r--r--   0     1001      127     5676 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/basics.md
+-rw-r--r--   0     1001      127      343 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/batch/average.md
+-rw-r--r--   0     1001      127     2553 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/batch/collect_projects.md
+-rw-r--r--   0     1001      127     3492 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/batch/construct.md
+-rw-r--r--   0     1001      127      223 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/batch/index.md
+-rw-r--r--   0     1001      127     1016 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/cli.md
+-rw-r--r--   0     1001      127     2366 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/extern/imod.md
+-rw-r--r--   0     1001      127      241 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/extern/index.md
+-rw-r--r--   0     1001      127     1705 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/extern/relion.md
+-rw-r--r--   0     1001      127     6913 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/fit_splines.md
+-rw-r--r--   0     1001      127   276476 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/images/average_tubulin.png
+-rw-r--r--   0     1001      127  1910217 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/images/draw_splines.gif
+-rw-r--r--   0     1001      127  2869509 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/images/generate_molecules.gif
+-rw-r--r--   0     1001      127    65566 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/images/lattice_params.png
+-rw-r--r--   0     1001      127     2685 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/index.md
+-rw-r--r--   0     1001      127     1844 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/installation.md
+-rw-r--r--   0     1001      127    13432 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/lattice_params.md
+-rw-r--r--   0     1001      127     2212 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/molecules/expressions.md
+-rw-r--r--   0     1001      127     3122 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/molecules/features.md
+-rw-r--r--   0     1001      127     1744 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/molecules/filter_molecules.md
+-rw-r--r--   0     1001      127     2684 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/molecules/headers.md
+-rw-r--r--   0     1001      127      467 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/molecules/index.md
+-rw-r--r--   0     1001      127     9053 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/molecules/spline_to_molecules.md
+-rw-r--r--   0     1001      127     2452 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/molecules/split_and_combine.md
+-rw-r--r--   0     1001      127     1733 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/molecules/transform.md
+-rw-r--r--   0     1001      127     7632 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/open_image.md
+-rw-r--r--   0     1001      127      622 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/process_images.md
+-rw-r--r--   0     1001      127     3071 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/project_io.md
+-rw-r--r--   0     1001      127      903 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/scripts/_dynamic_doc.py
+-rw-r--r--   0     1001      127     5510 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/scripts/_screenshots.py
+-rw-r--r--   0     1001      127     2889 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/seam_search.md
+-rw-r--r--   0     1001      127     6509 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/simulate.md
+-rw-r--r--   0     1001      127     1954 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/spline/clip.md
+-rw-r--r--   0     1001      127     3891 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/spline/config.md
+-rw-r--r--   0     1001      127      300 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/spline/index.md
+-rw-r--r--   0     1001      127     3864 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/docs/workflows.md
+-rw-r--r--   0     1001      127     3216 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/mkdocs.yml
+-rw-r--r--   0     1001      127   845316 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/resources/fig.png
+-rw-r--r--   0     1001      127     3278 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/scripts/annealing_demo.py
+-rw-r--r--   0     1001      127     3080 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/scripts/calibrate_nsr.py
+-rw-r--r--   0     1001      127     2344 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/scripts/generate_images.py
+-rw-r--r--   0     1001      127     3275 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/scripts/rma_demo.py
+-rw-r--r--   0     1001      127     4586 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/scripts/rma_fluctuation.py
+-rw-r--r--   0     1001      127     8297 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/scripts/simulate_alignments.py
+-rw-r--r--   0     1001      127    12675 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/scripts/simulate_cft.py
+-rw-r--r--   0     1001      127     4063 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/scripts/simulate_supertwist.py
+-rw-r--r--   0     1001      127      803 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/scripts/tip_recognition_demo.py
+-rw-r--r--   0     1001      127     4215 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/alleviate.rs
+-rw-r--r--   0     1001      127    11874 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/annealing/core.rs
+-rw-r--r--   0     1001      127    20263 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/annealing/graph.rs
+-rw-r--r--   0     1001      127      129 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/annealing/mod.rs
+-rw-r--r--   0     1001      127     5940 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/annealing/potential.rs
+-rw-r--r--   0     1001      127     4193 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/annealing/random.rs
+-rw-r--r--   0     1001      127     1650 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/annealing/reservoir.rs
+-rw-r--r--   0     1001      127     2237 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/array.rs
+-rw-r--r--   0     1001      127     1999 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/coordinates/coordinate_system.rs
+-rw-r--r--   0     1001      127      133 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/coordinates/mod.rs
+-rw-r--r--   0     1001      127     7366 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/coordinates/vector.rs
+-rw-r--r--   0     1001      127     6994 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/cylindric.rs
+-rw-r--r--   0     1001      127      449 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/exceptions.rs
+-rw-r--r--   0     1001      127    15711 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/filters.rs
+-rw-r--r--   0     1001      127     1054 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/lib.rs
+-rw-r--r--   0     1001      127    10848 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/regionprops.rs
+-rw-r--r--   0     1001      127     6358 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/viterbi/constraint.rs
+-rw-r--r--   0     1001      127    17258 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/viterbi/core.rs
+-rw-r--r--   0     1001      127       68 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/src/viterbi/mod.rs
+-rw-r--r--   0     1001      127   703618 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/13pf_MT.tif
+-rw-r--r--   0     1001      127   510466 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/14pf_MT.tif
+-rw-r--r--   0     1001      127      241 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/__init__.py
+-rw-r--r--   0     1001      127      159 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/_const.py
+-rw-r--r--   0     1001      127    33024 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/beta-tubulin.mrc
+-rw-r--r--   0     1001      127     1079 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/conftest.py
+-rw-r--r--   0     1001      127     7439 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_algorithms.py
+-rw-r--r--   0     1001      127     1109 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_custom_widgets.py
+-rw-r--r--   0     1001      127     2113 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_cylfilters.py
+-rw-r--r--   0     1001      127     3084 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_cylindric_model.py
+-rw-r--r--   0     1001      127    59766 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_gui_0.py
+-rw-r--r--   0     1001      127     5305 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_gui_1_batch.py
+-rw-r--r--   0     1001      127     2946 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_gui_2_extensions.py
+-rw-r--r--   0     1001      127      322 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_io.py
+-rw-r--r--   0     1001      127     1654 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_projects.py
+-rw-r--r--   0     1001      127     3220 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_regionprops.py
+-rw-r--r--   0     1001      127     8057 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_splines.py
+-rw-r--r--   0     1001      127     5524 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_utils.py
+-rw-r--r--   0     1001      127     3966 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/test_viterbi.py
+-rw-r--r--   0     1001      127     2002 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/tests/utils.py
+-rw-r--r--   0     1001      127    12708 2024-05-07 14:35:27.000000 cylindra-1.0.0b1/Cargo.lock
+-rw-r--r--   0     1001      127     3994 2024-05-07 14:35:23.000000 cylindra-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     6096 1970-01-01 00:00:00.000000 cylindra-1.0.0b1/PKG-INFO
```

### Comparing `cylindra-1.0.0b0/.github/workflows/CI.yml` & `cylindra-1.0.0b1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/.github/workflows/test.yml` & `cylindra-1.0.0b1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/.gitignore` & `cylindra-1.0.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/LICENSE` & `cylindra-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/README.md` & `cylindra-1.0.0b1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [![BSD 3-Clause License](https://img.shields.io/pypi/l/cylindra.svg?color=green)](https://github.com/hanjinliu/cylindra/blob/main/LICENSE)
 [![Python package index download statistics](https://img.shields.io/pypi/dm/cylindra.svg)](https://pypistats.org/packages/cylindra)
 [![PyPI version](https://badge.fury.io/py/cylindra.svg)](https://badge.fury.io/py/cylindra)
+[![codecov](https://codecov.io/gh/hanjinliu/cylindra/graph/badge.svg?token=X1F259JYT5)](https://codecov.io/gh/hanjinliu/cylindra)
+
+![](https://github.com/hanjinliu/cylindra/blob/main/resources/fig.png)
 
 # cylindra
 
 `cylindra` is a GUI-integrated cryo-ET image analysis tool for cylindric periodic
 structures such as microtubules.
 
-![](resources/fig.png)
-
-## Documentation
-
-COMING SOON
+### [&rarr; Documentation](https://hanjinliu.github.io/cylindra/)
 
 ## Installation
 
 - Use `pip`
 
 ```shell
 pip install cylindra -U
@@ -78,19 +77,23 @@
   recommended.
 - **Images should be loaded from SSD**. Raw image stacks are loaded lazily in most of
   the processes. Loading from HDD will slow down many analyses as well.
 
 ## Issues
 
 If you encountered any bugs or have any requests, feel free to
-[report an issue](https://github.com/hanjinliu/cylindra/issues).
+[report an issue](https://github.com/hanjinliu/cylindra/issues/new).
 (We'll appreciate if you find some methods are over-fitted to microtubules and do not
 work well on other cylindric structures)
 
 For better reproducibility, please copy your environments from `Others > cylindra info`
 and the recorded macro from `Others > Macro > Show macro`.
 
 ## Citation
 
-If you find `cylindra` useful in your work, please consider citing our paper.
+If you find `cylindra` useful in your work, please consider citing [our paper](https://www.biorxiv.org/content/10.1101/2024.04.30.591984v1).
 
-COMING SOON
+```
+Heterogeneous local structures of the microtubule lattice revealed by cryo-ET and non-averaging analysis
+Hanjin Liu, Hiroshi Yamaguchi, Masahide Kikkawa, Tomohiro Shima
+bioRxiv 2024.04.30.591984; doi: https://doi.org/10.1101/2024.04.30.591984
+```
```

### Comparing `cylindra-1.0.0b0/cylindra/__init__.py` & `cylindra-1.0.0b1/cylindra/__init__.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/__main__.py` & `cylindra-1.0.0b1/cylindra/__main__.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/_config.py` & `cylindra-1.0.0b1/cylindra/_config.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/_cylindra_ext.pyi` & `cylindra-1.0.0b1/cylindra/_cylindra_ext.pyi`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/_napari/_layer_controls.py` & `cylindra-1.0.0b1/cylindra/_napari/_layer_controls.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/_napari/_layers.py` & `cylindra-1.0.0b1/cylindra/_napari/_layers.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/_previews.py` & `cylindra-1.0.0b1/cylindra/_previews.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/_shared_doc.py` & `cylindra-1.0.0b1/cylindra/_shared_doc.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/__init__.py` & `cylindra-1.0.0b1/cylindra/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/_base.py` & `cylindra-1.0.0b1/cylindra/cli/_base.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/average.py` & `cylindra-1.0.0b1/cylindra/cli/average.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/config.py` & `cylindra-1.0.0b1/cylindra/cli/config.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/find.py` & `cylindra-1.0.0b1/cylindra/cli/find.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/new.py` & `cylindra-1.0.0b1/cylindra/cli/new.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/none.py` & `cylindra-1.0.0b1/cylindra/cli/none.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/open.py` & `cylindra-1.0.0b1/cylindra/cli/open.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/preview.py` & `cylindra-1.0.0b1/cylindra/cli/preview.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/run.py` & `cylindra-1.0.0b1/cylindra/cli/run.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cli/workflow.py` & `cylindra-1.0.0b1/cylindra/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/__init__.py` & `cylindra-1.0.0b1/cylindra/components/__init__.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/_base.py` & `cylindra-1.0.0b1/cylindra/components/_base.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/_cylinder_params.py` & `cylindra-1.0.0b1/cylindra/components/_cylinder_params.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/_ftprops.py` & `cylindra-1.0.0b1/cylindra/components/_ftprops.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/_peak.py` & `cylindra-1.0.0b1/cylindra/components/_peak.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/cylindric.py` & `cylindra-1.0.0b1/cylindra/components/cylindric.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/landscape.py` & `cylindra-1.0.0b1/cylindra/components/landscape.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/picker.py` & `cylindra-1.0.0b1/cylindra/components/picker.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/seam_search.py` & `cylindra-1.0.0b1/cylindra/components/seam_search.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/spline/_config.py` & `cylindra-1.0.0b1/cylindra/components/spline/_config.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/spline/_cyl_spline.py` & `cylindra-1.0.0b1/cylindra/components/spline/_cyl_spline.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/spline/_props.py` & `cylindra-1.0.0b1/cylindra/components/spline/_props.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/spline/_spline_base.py` & `cylindra-1.0.0b1/cylindra/components/spline/_spline_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from scipy.interpolate import splev, splprep, splrep
 from scipy.spatial.transform import Rotation
 
 from cylindra.components._base import BaseComponent
 from cylindra.components.spline._config import SplineConfig
 from cylindra.components.spline._props import SplineProps
 from cylindra.components.spline._types import SplineFitResult, SplineInfo, TCKType
-from cylindra.const import ExtrapolationMode, Mode, nm
+from cylindra.const import ExtrapolationMode, nm
 from cylindra.cyltransform import polar_coords_2d
 from cylindra.utils import ceilint, interval_divmod, roundint
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike, NDArray
     from typing_extensions import Self
 
@@ -716,82 +716,14 @@
         self._tck = (t, c, k)
         self._u = np.asarray(d["u"])
         self.props._window_size = d.get("localprops_window_size", {})
         if cfg := d.get("config", None):
             self._config = SplineConfig.from_dict(cfg)
         return self
 
-    def affine_matrix(
-        self,
-        positions: Sequence[float] = None,
-        center: Sequence[float] = None,
-        *,
-        inverse: bool = False,
-    ) -> NDArray[np.float32]:
-        """
-        Calculate list of Affine transformation matrix along spline, which correspond to
-        the orientation of spline curve.
-
-        Parameters
-        ----------
-        positions : array-like, (N,)
-            Positions. Between 0 and 1.
-        center : array-like, optional
-            If not provided, rotation will be executed around the origin. If an array is provided,
-            it will be considered as the coordinates of rotation center. This is useful for
-            rotating images.
-        inverse : bool, default False
-            If True, rotation matrix will be inversed.
-
-        Returns
-        -------
-        np.ndarray (N, 4, 4)
-            3D array of matrices, where the first dimension corresponds to each point.
-        """
-        if positions is None:
-            positions = self.anchors
-        ds = self.map(positions, der=1)
-
-        if ds.ndim == 1:
-            ds = ds[np.newaxis]
-        rot = axes_to_rotator(None, ds)
-        if inverse:
-            rot = rot.inv()
-        out = np.zeros((len(rot), 4, 4), dtype=np.float32)
-        out[:, :3, :3] = rot.as_matrix()
-        out[:, 3, 3] = 1.0
-
-        if center is not None:
-            dz, dy, dx = center
-            # center to corner
-            translation_0 = np.array(
-                [
-                    [1.0, 0.0, 0.0, dz],
-                    [0.0, 1.0, 0.0, dy],
-                    [0.0, 0.0, 1.0, dx],
-                    [0.0, 0.0, 0.0, 1.0],
-                ],
-                dtype=np.float32,
-            )
-            # corner to center
-            translation_1 = np.array(
-                [
-                    [1.0, 0.0, 0.0, -dz],
-                    [0.0, 1.0, 0.0, -dy],
-                    [0.0, 0.0, 1.0, -dx],
-                    [0.0, 0.0, 0.0, 1.0],
-                ],
-                dtype=np.float32,
-            )
-
-            out = translation_0 @ out @ translation_1
-        if np.isscalar(positions):
-            out = out[0]
-        return out
-
     def get_rotator(
         self,
         positions: Sequence[float] | None = None,
         inverse: bool = False,
     ) -> Rotation:
         """
         Calculate list of Affine transformation matrix along spline, which correspond to
@@ -1093,35 +1025,14 @@
         # world coordinates of the projection point of coords onto the spline
         u = self.y_to_position(coords[:, 1])
         ycoords = self.map(u)
         zvec = world_coords - ycoords
         yvec = self.map(u, der=1)
         return Molecules.from_axes(pos=world_coords, z=zvec, y=yvec)
 
-    def slice_along(
-        self,
-        array: NDArray[np.float32],
-        s_range: tuple[float, float] = (0.0, 1.0),
-        order: int = 3,
-        mode: str = Mode.constant,
-        cval: float = 0.0,
-    ) -> NDArray[np.float32]:
-        """Slice input array along the spline."""
-        from scipy import ndimage as ndi
-
-        _, coords = self._get_y_ax_coords(s_range)
-        return ndi.map_coordinates(
-            array,
-            coords.T,
-            order=order,
-            mode=mode,
-            cval=cval,
-            prefilter=order > 1,
-        )
-
     def _get_coords(
         self,
         map_func: Callable[[tuple], NDArray[np.float32]],
         map_params: tuple,
         s_range: tuple[float, float],
         scale: nm,
     ):
```

### Comparing `cylindra-1.0.0b0/cylindra/components/spline/_types.py` & `cylindra-1.0.0b1/cylindra/components/spline/_types.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/tomogram/_cyl_tomo.py` & `cylindra-1.0.0b1/cylindra/components/tomogram/_cyl_tomo.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,28 +133,19 @@
     return _func
 
 
 class FitResult:
     def __init__(self, residual: NDArray[np.float64]):
         self.residual = residual
 
-    def __repr__(self) -> str:
-        cname = self.__class__.__name__
-        return f"{cname}(rmsd={self.rmsd:.3f} nm, max={self.max:.3f} nm)"
-
     @property
     def rmsd(self) -> float:
         """Root mean square deviation."""
         return np.sqrt(np.sum(self.residual**2) / self.residual.shape[0])
 
-    @property
-    def max(self) -> float:
-        """Maximum deviation."""
-        return np.abs(self.residual).max()
-
 
 class CylTomogram(Tomogram):
     """Tomogram with cylindrical splines."""
 
     def __init__(self):
         super().__init__()
         self._splines = SplineList()
```

### Comparing `cylindra-1.0.0b0/cylindra/components/tomogram/_spline_list.py` & `cylindra-1.0.0b1/cylindra/components/tomogram/_spline_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,24 +72,23 @@
     def count(self) -> int:
         """Number of splines in the list."""
         return len(self)
 
     def filter(self, predicate: pl.Expr) -> SplineList:
         """Filter the list by its global properties."""
 
-        def fn(spl):
-            return spl.props.glob.select(predicate)[0]
-
-        return SplineList(filter(fn, self._list))
+        df = pl.concat([spl.props.glob for spl in self])
+        indices = np.where(df.select(predicate).to_series().to_numpy())[0]
+        return SplineList([self._list[i] for i in indices])
 
     def sort(self, by: pl.Expr | str) -> SplineList:
         """Sort the list by its global properties."""
 
-        def fn(spl):
-            return spl.props.glob.select(by)[0]
+        def fn(spl: CylSpline):
+            return spl.props.glob.select(by).to_series()[0]
 
         return SplineList(sorted(self._list, key=fn))
 
     def iter(self) -> Iterator[CylSpline]:
         """Iterate over splines."""
         return iter(self)
```

### Comparing `cylindra-1.0.0b0/cylindra/components/tomogram/_straighten.py` & `cylindra-1.0.0b1/cylindra/components/tomogram/_straighten.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/tomogram/_tomo_base.py` & `cylindra-1.0.0b1/cylindra/components/tomogram/_tomo_base.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/components/visualize.py` & `cylindra-1.0.0b1/cylindra/components/visualize.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/const.py` & `cylindra-1.0.0b1/cylindra/const.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/core.py` & `cylindra-1.0.0b1/cylindra/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 def start(
     project_file: str | None = None,
     viewer: napari.Viewer | None = None,
     *,
     log_level: int | str = "INFO",
     headless: bool = False,
+    add_main_widget: bool = True,
+    run: bool = True,
 ) -> CylindraMainWidget:
     """
     Start napari viewer and dock cylindra widget as a dock widget.
 
     Parameters
     ----------
     project_file : path-like, optional
@@ -79,18 +81,19 @@
         else:
             raise ValueError(f"Invalid log level: {log_level}")
     logger.setLevel(log_level)
 
     # set polars display options
     pl.Config().set_tbl_width_chars(120)
 
-    dock = viewer.window.add_dock_widget(
-        ui, area="right", allowed_areas=["right"], name="cylindra"
-    )
-    dock.setMinimumHeight(300)
+    if add_main_widget:
+        dock = viewer.window.add_dock_widget(
+            ui, area="right", allowed_areas=["right"], name="cylindra"
+        )
+        dock.setMinimumHeight(300)
     viewer.window.add_dock_widget(logger.widget, name="Log")
     ui.macro.options.syntax_highlight = False
 
     if project_file is not None:
         ui.load_project(project_file)
     _CURRENT_INSTANCE = ui
 
@@ -115,29 +118,47 @@
         def _on_destroy():
             viewer.layers.events.removing.disconnect()
             viewer.layers.events.removed.disconnect()
 
         # napari-console disables calltips by default. It's better to enable it.
         viewer.window._qt_viewer.console.enable_calltips = True
 
-    ui.show()
-    try:  # Just in case
-        # avoid accidentally closing/hiding the dock widget
-        dock.title.close_button.disconnect()
-        dock.title.hide_button.disconnect()
-    except Exception:  # pragma: no cover
-        print("Failed to disconnect the close/hide button of the dock widget.")
+    ui.show(run=run)
+    if add_main_widget:
+        try:  # Just in case
+            # avoid accidentally closing/hiding the dock widget
+            dock.title.close_button.disconnect()
+            dock.title.hide_button.disconnect()
+        except Exception:  # pragma: no cover
+            print("Failed to disconnect the close/hide button of the dock widget.")
 
     # Programmatically run `%matplotlib inline` magic
     ipy = get_ipython()
     ipy.run_line_magic("matplotlib", "inline")
 
     return ui
 
 
+def start_as_plugin(run: bool = True):
+    """Start Cylindra as a napari plugin"""
+    import napari
+    from magicclass import logging
+
+    ui = start(
+        viewer=napari.current_viewer(),
+        add_main_widget=False,
+        run=run,
+    )
+    # float logger widget
+    logger = logging.getLogger("cylindra")
+    logger.widget.native.parentWidget().setFloating(True)
+    logger.widget.height = 160
+    return ui
+
+
 # fmt: off
 @overload
 def instance(create: Literal[False] = False) -> CylindraMainWidget | None: ...
 @overload
 def instance(create: Literal[True]) -> CylindraMainWidget: ...
 # fmt: on
```

### Comparing `cylindra-1.0.0b0/cylindra/cylfilters.py` & `cylindra-1.0.0b1/cylindra/cylfilters.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cylmeasure.py` & `cylindra-1.0.0b1/cylindra/cylmeasure.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/cyltransform.py` & `cylindra-1.0.0b1/cylindra/cyltransform.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/ext/_utils.py` & `cylindra-1.0.0b1/cylindra/ext/_utils.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/ext/imod/cmd.py` & `cylindra-1.0.0b1/cylindra/ext/imod/cmd.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/ext/imod/menu.py` & `cylindra-1.0.0b1/cylindra/ext/imod/menu.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/ext/relion/menu.py` & `cylindra-1.0.0b1/cylindra/ext/relion/menu.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/project/_base.py` & `cylindra-1.0.0b1/cylindra/project/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import io
 import json
 from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from pydantic_compat import BaseModel
 from typing_extensions import Self
 
 from cylindra.project._json import project_json_encoder
 from cylindra.project._utils import get_project_file
 
+if TYPE_CHECKING:
+    from pydantic import BaseModel
+else:
+    from pydantic_compat import BaseModel
+
 PathLike = Path | str | bytes
 
 
 class BaseProject(BaseModel):
     """The basic project class."""
 
     datetime: str
```

### Comparing `cylindra-1.0.0b0/cylindra/project/_batch.py` & `cylindra-1.0.0b1/cylindra/project/_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import macrokit as mk
-from pydantic_compat import BaseModel
 
 from cylindra._config import get_config
 from cylindra.const import MoleculesHeader as Mole
 from cylindra.const import get_versions, nm
 from cylindra.project._base import BaseProject, PathLike, resolve_path
 from cylindra.project._utils import as_main_function
 
 if TYPE_CHECKING:
+    from pydantic import BaseModel
+
     from cylindra.widgets.batch import CylindraBatchWidget
+else:
+    from pydantic_compat import BaseModel
 
 
 class ImageInfo(BaseModel):
     """Model that describe how to load an image."""
 
     id: int
     image: PathLike
```

### Comparing `cylindra-1.0.0b0/cylindra/project/_json.py` & `cylindra-1.0.0b1/cylindra/project/_json.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/project/_layer_info.py` & `cylindra-1.0.0b1/cylindra/project/_layer_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import warnings
 from abc import abstractmethod
 from pathlib import Path
 from typing import TYPE_CHECKING
 
-from pydantic_compat import BaseModel
-
 if TYPE_CHECKING:
     from napari.layers import Layer
+    from pydantic import BaseModel
 
     from cylindra._napari import LandscapeSurface, MoleculesLayer
     from cylindra.widgets.main import CylindraMainWidget
+else:
+    from pydantic_compat import BaseModel
 
 
 class LayerInfo(BaseModel):
     @classmethod
     @abstractmethod
     def from_layer(cls, gui: "CylindraMainWidget", layer: "Layer") -> "LayerInfo":
         """Convert layer to info."""
```

### Comparing `cylindra-1.0.0b0/cylindra/project/_sequence.py` & `cylindra-1.0.0b1/cylindra/project/_sequence.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/project/_single.py` & `cylindra-1.0.0b1/cylindra/project/_single.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/project/_utils.py` & `cylindra-1.0.0b1/cylindra/project/_utils.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/project/_widgets.py` & `cylindra-1.0.0b1/cylindra/project/_widgets.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/types.py` & `cylindra-1.0.0b1/cylindra/types.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/utils/_correlation.py` & `cylindra-1.0.0b1/cylindra/utils/_correlation.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/utils/_misc.py` & `cylindra-1.0.0b1/cylindra/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widget_utils.py` & `cylindra-1.0.0b1/cylindra/widget_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,65 +62,37 @@
     {
         "widget_type": EvalLineEdit,
         "namespace": POLARS_NAMESPACE,
         "validator": _validate_expr_or_scalar,
     },
 ]
 
-_FLOAT_NAMESPACE = {"__builtins__": {}, "inf": float("inf"), "nan": float("nan")}
-
-
-def _validate_float(x):
-    if isinstance(x, str):
-        x = eval(x, _FLOAT_NAMESPACE)
-    if not isinstance(x, (int, float, np.number)):
-        raise TypeError(f"Invalid type: {type(x)}")
-    return x
-
-
-FloatInfNan = Annotated[
-    float,
-    {
-        "widget_type": EvalLineEdit,
-        "namespace": _FLOAT_NAMESPACE,
-        "validator": _validate_float,
-    },
-]
-
 
 def _unwrap_rust_expr(expr: mk.Symbol | mk.Expr) -> mk.Symbol | mk.Expr:
     """The str of pl.Expr use brackets for binary expressions."""
     if not isinstance(expr, mk.Expr):
         return expr
     if expr.head is mk.Head.list and len(expr.args) == 1:
         return _unwrap_rust_expr(expr.args[0])
     return mk.Expr(expr.head, [_unwrap_rust_expr(a) for a in expr.args])
 
 
-def _replace_utf8(string: str) -> str:
-    ptn = re.compile(r"Utf8\(.?+\)")
-    m0 = ptn.search(string)
-    if m0 is None:
-        return string
-    sl_0 = slice(None, m0.start())
-    sl_mid = slice(m0.start() + 5, m0.end() - 1)
-    sl_1 = slice(m0.end(), None)
-    return string[sl_0] + '"' + string[sl_mid] + '"' + string[sl_1]
-
-
 def _replace_dyn(string: str, fmt: str) -> str:
     _float_or_int = r"[-+]?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)?"
     return re.sub(rf"\(dyn {fmt}: ({_float_or_int})\)", r"\1", string)
 
 
+def _replace_string(string: str) -> str:
+    return re.sub(r"String\(([^)]+)\)", r"'\1'", string)
+
+
 def _polars_expr_to_str(expr: pl.Expr) -> str:
     expr_str = str(expr).replace(".when(", "when(").replace(".strict_cast(", ".cast(")
-    if "Utf8" in expr_str:
-        # Utf8(xxx) -> "xxx"
-        expr_str = _replace_utf8(expr_str)
+    if "String(" in expr_str:
+        expr_str = _replace_string(expr_str)
     if "dyn int:" in expr_str:
         expr_str = _replace_dyn(expr_str, "int")
     if "dyn float:" in expr_str:
         expr_str = _replace_dyn(expr_str, "float")
     if "[" in expr_str:
         # converting binary expression to str will add brackets so remove them
         # e.g. [col("a") == (3)] -> col("a") == (3)
@@ -129,15 +101,15 @@
         if (
             out.head is mk.Head.binop
             and expr_str.startswith("(")
             and expr_str.endswith(")")
         ):
             expr_str = expr_str[1:-1]
     try:
-        ns = dict(**POLARS_NAMESPACE, true=True, false=False, String=str)
+        ns = dict(**POLARS_NAMESPACE)
         ExprStr(expr_str, ns).eval()
     except Exception:
         raise ValueError(
             f"Expression {expr_str!r} cannot be safely parsed. Please use "
             "str as the input."
         ) from None
     return expr_str
```

### Comparing `cylindra-1.0.0b0/cylindra/widgets/__init__.py` & `cylindra-1.0.0b1/cylindra/widgets/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import sys
 
 
 def dont_use_native_menu_bar():  # pragma: no cover
     # cylindra has menu bars in sub widgets.
     from qtpy.QtCore import QCoreApplication, Qt
 
+    if QCoreApplication.instance() is not None:
+        return None
     QCoreApplication.setAttribute(Qt.ApplicationAttribute.AA_DontUseNativeMenuBar)
     return None
 
 
 def init_opengl_and_dpi():
     from qtpy import QT6
     from qtpy.QtCore import QCoreApplication, Qt
 
+    if QCoreApplication.instance() is not None:
+        return None
     # Docking vispy widget in napari viewer requires this.
     QCoreApplication.setAttribute(Qt.ApplicationAttribute.AA_ShareOpenGLContexts)
     # High DPI support for High-DPI devices such as Surface Pro. Only for Qt<6.
     if not QT6:
         QCoreApplication.setAttribute(Qt.ApplicationAttribute.AA_UseHighDpiPixmaps)
     return None
```

### Comparing `cylindra-1.0.0b0/cylindra/widgets/_accessors.py` & `cylindra-1.0.0b1/cylindra/widgets/_accessors.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/_annealing.py` & `cylindra-1.0.0b1/cylindra/widgets/_annealing.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/_annotated.py` & `cylindra-1.0.0b1/cylindra/widgets/_annotated.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/_main_utils.py` & `cylindra-1.0.0b1/cylindra/widgets/_main_utils.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/_process_template.py` & `cylindra-1.0.0b1/cylindra/widgets/_process_template.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/_progress_desc.py` & `cylindra-1.0.0b1/cylindra/widgets/_progress_desc.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/_reserved_layers.py` & `cylindra-1.0.0b1/cylindra/widgets/_reserved_layers.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/_ui_init.py` & `cylindra-1.0.0b1/cylindra/widgets/_ui_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,17 @@
 from magicclass.widgets import ConsoleTextEdit
 from magicgui.widgets import FunctionGui, Label, PushButton
 from napari.utils.colormaps import label_colormap
 
 from cylindra import _config, utils, widget_utils
 from cylindra._napari import MoleculesLayer
 from cylindra._previews import view_tables
-from cylindra.const import (
-    PREVIEW_LAYER_NAME,
-)
-from cylindra.const import (
-    MoleculesHeader as Mole,
-)
-from cylindra.const import (
-    PropertyNames as H,
-)
+from cylindra.const import PREVIEW_LAYER_NAME
+from cylindra.const import MoleculesHeader as Mole
+from cylindra.const import PropertyNames as H
 from cylindra.core import ACTIVE_WIDGETS
 from cylindra.project import CylindraProject
 from cylindra.widgets._main_utils import (
     degrees_to_rotator,
     normalize_offsets,
     normalize_radius,
 )
@@ -110,19 +104,15 @@
     interval = spl.props.glob.select(interv_expr).to_series()[0]
     out = tomo.map_pf_line(
         i=spline,
         interval=interval,
         offsets=normalize_offsets(offsets, spl),
         orientation=orientation,
     )
-    if PREVIEW_LAYER_NAME in viewer.layers:
-        layer: MoleculesLayer = viewer.layers[PREVIEW_LAYER_NAME]
-        layer.molecules = out
-    else:
-        layer = self.add_molecules(out, name=PREVIEW_LAYER_NAME)
+    layer = _update_existing_layer(self, out)
     layer.face_color = "crimson"
     is_active = yield
     if not is_active and layer in viewer.layers:
         viewer.layers.remove(layer)
 
 
 @impl_preview(CylindraMainWidget.map_monomers_with_extensions, auto_call=True)
@@ -142,21 +132,17 @@
         coords=coords,
         orientation=orientation,
         offsets=normalize_offsets(offsets, spl),
         radius=normalize_radius(radius, spl),
     )
     viewer = self.parent_viewer
 
-    if PREVIEW_LAYER_NAME in viewer.layers:
-        layer: MoleculesLayer = viewer.layers[PREVIEW_LAYER_NAME]
-        layer.molecules = out
-    else:
-        layer = self.add_molecules(out, name=PREVIEW_LAYER_NAME)
-        layer.view_ndim = 2
-        layer.text = {"string": "{pf-id}"}
+    layer = _update_existing_layer(self, out)
+    layer.view_ndim = 2
+    layer.text = {"string": "{pf-id}"}
     layer.face_color = "crimson"
     is_active = yield
     if not is_active and layer in viewer.layers:
         viewer.layers.remove(layer)
 
 
 @impl_preview(CylindraMainWidget.split_molecules, auto_call=True)
@@ -207,20 +193,16 @@
         if internal:
             out = mole.translate_internal(translation)
         else:
             out = mole.translate(translation)
         all_mole.append(out)
     out = Molecules.concat(all_mole, concat_features=False)
     viewer = self.parent_viewer
-    if PREVIEW_LAYER_NAME in viewer.layers:
-        layer: Layer = viewer.layers[PREVIEW_LAYER_NAME]
-        layer.data = out.pos
-    else:
-        layer = self.add_molecules(out, name=PREVIEW_LAYER_NAME)
-        layer.face_color = "crimson"
+    layer = _update_existing_layer(self, out)
+    layer.face_color = "crimson"
     is_active = False
     is_active = yield
     if not is_active and layer in viewer.layers:
         viewer.layers.remove(layer)
 
 
 @impl_preview(CylindraMainWidget.rotate_molecules, auto_call=True)
@@ -544,7 +526,17 @@
         layer.face_color = fc
         layer.edge_color = ec
         layer.face_colormap = fcmap
         layer.edge_colormap = ecmap
         layer.face_contrast_limits = fclim
         layer.edge_contrast_limits = eclim
         layer._colormap_info = info
+
+
+def _update_existing_layer(self: CylindraMainWidget, out: Molecules) -> MoleculesLayer:
+    viewer = self.parent_viewer
+    if PREVIEW_LAYER_NAME in viewer.layers:
+        layer: MoleculesLayer = viewer.layers[PREVIEW_LAYER_NAME]
+        layer.molecules = out
+    else:
+        layer = self.add_molecules(out, name=PREVIEW_LAYER_NAME)
+    return layer
```

### Comparing `cylindra-1.0.0b0/cylindra/widgets/_widget_ext.py` & `cylindra-1.0.0b1/cylindra/widgets/_widget_ext.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/batch/_loaderlist.py` & `cylindra-1.0.0b1/cylindra/widgets/batch/_loaderlist.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/batch/_sequence.py` & `cylindra-1.0.0b1/cylindra/widgets/batch/_sequence.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/batch/_utils.py` & `cylindra-1.0.0b1/cylindra/widgets/batch/_utils.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/batch/main.py` & `cylindra-1.0.0b1/cylindra/widgets/batch/main.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/batch/menus.py` & `cylindra-1.0.0b1/cylindra/widgets/batch/menus.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/batch/sta.py` & `cylindra-1.0.0b1/cylindra/widgets/batch/sta.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/main.py` & `cylindra-1.0.0b1/cylindra/widgets/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,17 +34,15 @@
     PREVIEW_LAYER_NAME,
     FileFilter,
     ImageFilter,
     Ori,
     SplineColor,
     nm,
 )
-from cylindra.const import (
-    MoleculesHeader as Mole,
-)
+from cylindra.const import MoleculesHeader as Mole
 from cylindra.const import PropertyNames as H
 from cylindra.project import CylindraProject, extract
 from cylindra.widget_utils import (
     PolarsExprStr,
     PolarsExprStrOrScalar,
     add_molecules,
     capitalize,
```

### Comparing `cylindra-1.0.0b0/cylindra/widgets/sta.py` & `cylindra-1.0.0b1/cylindra/widgets/sta.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import TYPE_CHECKING, Annotated, Any, Callable, Iterable, Literal
 
 import impy as ip
 import napari
 import numpy as np
 import polars as pl
 from acryo import Molecules, SubtomogramLoader, alignment, pipe
+from acryo._utils import SubvolumeOutOfBoundError
 from magicclass import (
     MagicTemplate,
     abstractapi,
     do_not_record,
     field,
     impl_preview,
     magicclass,
@@ -1798,20 +1799,25 @@
         mole: Molecules,
         range_long: tuple[float, float],
         angle_max: float,
         min_score: float,
         npf: int | None = None,
         **kwargs,
     ):
-        score_hist_0 = []
+        score_hist_0 = list[float]()
         score_hist_1 = list[float]()
         next_mole, cur_fixed = _prep_next_molecules(mole)
         aligned_molecules = list[Molecules]()
         while True:
-            landscape = self._construct_landscape(molecules=next_mole, **kwargs)
+            try:
+                landscape = self._construct_landscape(molecules=next_mole, **kwargs)
+            except SubvolumeOutOfBoundError:
+                if score_hist_0:
+                    score_hist_0.pop()
+                break
             if len(score_hist_0) == 0:
                 score_hist_0.append(-landscape.energies[(0, *landscape.offset)])
             aligned_mole = landscape.run_viterbi_fixed_start(
                 cur_fixed,
                 range_long=range_long,
                 angle_max=angle_max,
             )
```

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/__init__.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/file_iter.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/file_iter.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/function_menu.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/function_menu.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/image_processor.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/image_processor.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/measure.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/measure.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/menus.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/menus.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/misc.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/misc.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/pca.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/pca.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/properties.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/properties.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/runner.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/runner.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/simulator.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 from cylindra.const import PropertyNames as H
 from cylindra.utils import ceilint, roundint
 from cylindra.widget_utils import POLARS_NAMESPACE, capitalize
 from cylindra.widgets._annotated import MoleculesLayerType, _as_layer_name, assert_layer
 from cylindra.widgets.subwidgets._child_widget import ChildWidget
 
 if TYPE_CHECKING:
+    import napari
     from napari.layers import Layer
 
 _TiltRange = Annotated[
     tuple[float, float],
     {
         "label": "Tilt range (deg)",
         "widget_type": "FloatRangeSlider",
@@ -159,14 +160,15 @@
 
     @magicmenu(name="Simulate")
     class SimulateMenu(ChildWidget):
         simulate_tomogram = abstractapi()
         simulate_tomogram_from_tilt_series = abstractapi()
         simulate_tomogram_and_open = abstractapi()
         simulate_tilt_series = abstractapi()
+        simulate_projection = abstractapi()
 
     @magictoolbar
     class SimulatorTools(ChildWidget):
         add_component = abstractapi()
         sep0 = field(Separator)
         generate_molecules = abstractapi()
         expand = abstractapi()
@@ -367,15 +369,16 @@
             Radius of the cylinder.
         """
         # NOTE: these parameters are hard-coded for microtubule for now.
         main = self._get_main()
         spl = main.splines[spline]
         model = self._prep_model(spl, spacing, twist, start, npf, radius, offsets)
         mole = model.to_molecules(spl)
-        layer = main.add_molecules(mole, name=f"Mole(Sim)-{spline}", source=spl)
+        name = _make_simulated_mole_name(main.parent_viewer)
+        layer = main.add_molecules(mole, name=name, source=spl)
         _set_simulation_model(layer, model)
         if update_glob:
             cparams = spl.cylinder_params(
                 spacing=spacing, twist=twist, start=start, npf=npf, radius=radius
             )
             spl.update_glob_by_cylinder_params(cparams)
 
@@ -473,16 +476,16 @@
         main = self._get_main()
         degrees = np.linspace(*tilt_range, n_tilt)
         sino = self._prep_radon(components, degrees, order=interpolation)
 
         yield _on_radon_finished.with_args(sino, degrees)
 
         rng = ip.random.default_rng(seed)
+        imax = sino.max()
         for i, nsr_val in enumerate(nsr):
-            imax = sino.max()
             sino_noise = sino + rng.normal(
                 scale=imax * nsr_val, size=sino.shape, axes=sino.axes
             )
             rec = sino_noise.iradon(
                 degrees,
                 central_axis="y",
                 height=main.tomogram.image.shape[0],
@@ -670,14 +673,59 @@
         scale = sino.scale.x
         save_path = save_dir / "image.mrc"
         sino.set_axes("zyx").set_scale(zyx=scale, unit="nm").imsave(save_path)
         _Logger.print(f"Tilt series saved at {save_path}.")
         self._get_main().save_project(save_dir / PROJECT_NAME, molecules_ext=".parquet")
         return None
 
+    @set_design(text=capitalize, location=SimulateMenu)
+    @dask_thread_worker.with_progress(desc="Simulating 2D projections...")
+    def simulate_projection(
+        self,
+        components: Annotated[Any, {"bind": _get_components}],
+        save_dir: Annotated[Path.Save, {"label": "Save at"}],
+        nsr: _NSRatios = [1.5],
+        interpolation: Annotated[int, {"choices": INTERPOLATION_CHOICES}] = 3,
+        seed: Optional[Annotated[int, {"min": 0, "max": 1e8}]] = None,
+    ):  # fmt: skip
+        """
+        Simulate a projection without tilt (cryo-EM-like image).
+
+        Parameters
+        ----------
+        components : list of (str, Path)
+            List of tuples of layer name and path to the template image.
+        save_dir : Path
+            Path to the directory where the images will be saved.
+        nsr : list of float
+            Noise-to-signal ratio. It is defined by N/S, where S is the maximum
+            value of the true monomer density and N is the standard deviation of
+            the Gaussian noise. Duplicate values are allowed, which is useful
+            for simulation of multiple images with the same noise level.
+        interpolation : int
+            Interpolation method used during the simulation.
+        seed : int, optional
+            Random seed used for the Gaussian noise.
+        """
+        save_dir = _norm_save_dir(save_dir)
+        _assert_not_empty(components)
+        proj = self._prep_radon(components, np.zeros(1), order=interpolation)[0]
+        proj = proj.set_axes("yx").set_scale(yx=proj.scale.x, unit="nm")
+        yield _on_iradon_finished.with_args(proj, "Projection (noise-free)")
+        rng = ip.random.default_rng(seed)
+        imax = proj.max()
+        for i, nsr_val in enumerate(nsr):
+            proj_noise = proj + rng.normal(
+                scale=imax * nsr_val, size=proj.shape, axes=proj.axes
+            )
+            proj_noise.imsave(save_dir / f"image-{i}.tif")
+        _Logger.print(f"Projections saved at {save_dir}.")
+        self._get_main().save_project(save_dir / PROJECT_NAME, molecules_ext=".parquet")
+        return None
+
     @set_design(icon="iconoir:expand-lines", location=SimulatorTools)
     def expand(
         self,
         layer: _ModeledMoleculesLayer,
         by: Annotated[float, {"min": -100, "max": 100}] = 0.0,
         yrange: Annotated[tuple[int, int], {"widget_type": RangeSlider}] = (0, 1),
         arange: Annotated[tuple[int, int], {"widget_type": RangeSlider}] = (0, 1),
@@ -1031,7 +1079,16 @@
         .to_numpy()
     )
     layer.selected_data = np.where(if_select)[0]
     layer.refresh()
     yield
     layer.data = layer.molecules.pos
     layer.selected_data = {}
+
+
+def _make_simulated_mole_name(viewer: "napari.Viewer"):
+    num = 0
+    name = "Mole(Sim)"
+    existing_names = {layer.name for layer in viewer.layers}
+    while f"{name}-{num}" in existing_names:
+        num += 1
+    return f"{name}-{num}"
```

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/slicer.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/slicer.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/spline_clipper.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/spline_clipper.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/spline_control.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/spline_control.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/spline_fitter.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/spline_fitter.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/cylindra/widgets/subwidgets/toolbar.py` & `cylindra-1.0.0b1/cylindra/widgets/subwidgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/alignment/conventional.md` & `cylindra-1.0.0b1/docs/alignment/conventional.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/alignment/index.md` & `cylindra-1.0.0b1/docs/alignment/index.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/alignment/landscape.md` & `cylindra-1.0.0b1/docs/alignment/landscape.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/alignment/rma.md` & `cylindra-1.0.0b1/docs/alignment/rma.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/alignment/viterbi.md` & `cylindra-1.0.0b1/docs/alignment/viterbi.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/api/components.md` & `cylindra-1.0.0b1/docs/api/components.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/basics.md` & `cylindra-1.0.0b1/docs/basics.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/batch/collect_projects.md` & `cylindra-1.0.0b1/docs/batch/collect_projects.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/batch/construct.md` & `cylindra-1.0.0b1/docs/batch/construct.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/cli.md` & `cylindra-1.0.0b1/docs/cli.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/extern/imod.md` & `cylindra-1.0.0b1/docs/extern/imod.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/extern/relion.md` & `cylindra-1.0.0b1/docs/extern/relion.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/fit_splines.md` & `cylindra-1.0.0b1/docs/fit_splines.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/images/average_tubulin.png` & `cylindra-1.0.0b1/docs/images/average_tubulin.png`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/images/draw_splines.gif` & `cylindra-1.0.0b1/docs/images/draw_splines.gif`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/images/generate_molecules.gif` & `cylindra-1.0.0b1/docs/images/generate_molecules.gif`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/images/lattice_params.png` & `cylindra-1.0.0b1/docs/images/lattice_params.png`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/index.md` & `cylindra-1.0.0b1/docs/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -56,9 +56,11 @@
       data analysis.
 
 ### Reference
 
 If you find `cylindra` useful in your work, please consider citing our paper.
 
 ```
-TODO
+Heterogeneous local structures of the microtubule lattice revealed by cryo-ET and non-averaging analysis
+Hanjin Liu, Hiroshi Yamaguchi, Masahide Kikkawa, Tomohiro Shima
+bioRxiv 2024.04.30.591984; doi: https://doi.org/10.1101/2024.04.30.591984
 ```
```

### Comparing `cylindra-1.0.0b0/docs/installation.md` & `cylindra-1.0.0b1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/lattice_params.md` & `cylindra-1.0.0b1/docs/lattice_params.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/molecules/expressions.md` & `cylindra-1.0.0b1/docs/molecules/expressions.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/molecules/features.md` & `cylindra-1.0.0b1/docs/molecules/features.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/molecules/filter_molecules.md` & `cylindra-1.0.0b1/docs/molecules/filter_molecules.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/molecules/headers.md` & `cylindra-1.0.0b1/docs/molecules/headers.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/molecules/spline_to_molecules.md` & `cylindra-1.0.0b1/docs/molecules/spline_to_molecules.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/molecules/split_and_combine.md` & `cylindra-1.0.0b1/docs/molecules/split_and_combine.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/molecules/transform.md` & `cylindra-1.0.0b1/docs/molecules/transform.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/open_image.md` & `cylindra-1.0.0b1/docs/open_image.md`

 * *Files 0% similar despite different names*

```diff
@@ -55,19 +55,19 @@
 
 In this dialog, you can configure how to open the image. Note that the image opened in
 the viewer is **NOT the original image**. `cylindra` uses a binned and optionally
 filtered image for visualization.
 
 !!! danger "Important: Use dark background images"
 
-   Most of the methods require dark-background images, while most of the raw images of
-   electron microscopy are light-background. You have to manually prepare an inverted
-   image file, or check the "Invert intensity" option in the open-image dialog. The
-   loaded image can also be inverted from the menu (see
-   [Invert Images](#invert-images)).
+    Most of the methods require dark-background images, while most of the raw images of
+    electron microscopy are light-background. You have to manually prepare an inverted
+    image file, or check the "Invert intensity" option in the open-image dialog. The
+    loaded image can also be inverted from the menu (see
+    [Invert Images](#invert-images)).
 
 1. Click "Select file" to select the image file to open. tiff and mrc files are
    supported.
 2. Set the appropriate pixel scale. You can click "Scan header" to automatically detect
    the pixel scale.
 3. Set the tilt range and the tilt axis used for calculating missing wedges.
 4. Set the bin sizes used during your analysis. For example, setting to `[2, 4]` will
```

### Comparing `cylindra-1.0.0b0/docs/process_images.md` & `cylindra-1.0.0b1/docs/process_images.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/project_io.md` & `cylindra-1.0.0b1/docs/project_io.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/scripts/_dynamic_doc.py` & `cylindra-1.0.0b1/docs/scripts/_dynamic_doc.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/scripts/_screenshots.py` & `cylindra-1.0.0b1/docs/scripts/_screenshots.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/seam_search.md` & `cylindra-1.0.0b1/docs/seam_search.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/simulate.md` & `cylindra-1.0.0b1/docs/simulate.md`

 * *Files 2% similar despite different names*

```diff
@@ -136,7 +136,13 @@
 :material-arrow-right-thin-circle-outline: GUI: `Simulator widget > Simulate > Simulate tilt series`
 
 ### 4. Simulate tomogram from a tilt series
 
 :material-arrow-right-thin-circle-outline: API: [`simulate_tomogram_from_tilt_series`][cylindra.widgets.subwidgets.Simulator.simulate_tomogram_from_tilt_series]
 
 :material-arrow-right-thin-circle-outline: GUI: `Simulator widget > Simulate > Simulate tomogram from tilt series`
+
+### 5. Simulate a 2D projection
+
+:material-arrow-right-thin-circle-outline: API: [`simulate_projection`][cylindra.widgets.subwidgets.Simulator.simulate_projection]
+
+:material-arrow-right-thin-circle-outline: GUI: `Simulator widget > Simulate > Simulate projection`
```

### Comparing `cylindra-1.0.0b0/docs/spline/clip.md` & `cylindra-1.0.0b1/docs/spline/clip.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/spline/config.md` & `cylindra-1.0.0b1/docs/spline/config.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/docs/workflows.md` & `cylindra-1.0.0b1/docs/workflows.md`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/mkdocs.yml` & `cylindra-1.0.0b1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/resources/fig.png` & `cylindra-1.0.0b1/resources/fig.png`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/scripts/annealing_demo.py` & `cylindra-1.0.0b1/scripts/annealing_demo.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/scripts/calibrate_nsr.py` & `cylindra-1.0.0b1/scripts/calibrate_nsr.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/scripts/generate_images.py` & `cylindra-1.0.0b1/scripts/generate_images.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/scripts/rma_demo.py` & `cylindra-1.0.0b1/scripts/rma_demo.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/scripts/rma_fluctuation.py` & `cylindra-1.0.0b1/scripts/rma_fluctuation.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/scripts/simulate_alignments.py` & `cylindra-1.0.0b1/scripts/simulate_alignments.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/scripts/simulate_cft.py` & `cylindra-1.0.0b1/scripts/simulate_cft.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/scripts/simulate_supertwist.py` & `cylindra-1.0.0b1/scripts/simulate_supertwist.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/scripts/tip_recognition_demo.py` & `cylindra-1.0.0b1/scripts/tip_recognition_demo.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/alleviate.rs` & `cylindra-1.0.0b1/src/alleviate.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/annealing/core.rs` & `cylindra-1.0.0b1/src/annealing/core.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/annealing/graph.rs` & `cylindra-1.0.0b1/src/annealing/graph.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/annealing/potential.rs` & `cylindra-1.0.0b1/src/annealing/potential.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/annealing/random.rs` & `cylindra-1.0.0b1/src/annealing/random.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/annealing/reservoir.rs` & `cylindra-1.0.0b1/src/annealing/reservoir.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/array.rs` & `cylindra-1.0.0b1/src/array.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/coordinates/coordinate_system.rs` & `cylindra-1.0.0b1/src/coordinates/coordinate_system.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/coordinates/vector.rs` & `cylindra-1.0.0b1/src/coordinates/vector.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/cylindric.rs` & `cylindra-1.0.0b1/src/cylindric.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/filters.rs` & `cylindra-1.0.0b1/src/filters.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/lib.rs` & `cylindra-1.0.0b1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/regionprops.rs` & `cylindra-1.0.0b1/src/regionprops.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/viterbi/constraint.rs` & `cylindra-1.0.0b1/src/viterbi/constraint.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/src/viterbi/core.rs` & `cylindra-1.0.0b1/src/viterbi/core.rs`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/13pf_MT.tif` & `cylindra-1.0.0b1/tests/13pf_MT.tif`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/14pf_MT.tif` & `cylindra-1.0.0b1/tests/14pf_MT.tif`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/beta-tubulin.mrc` & `cylindra-1.0.0b1/tests/beta-tubulin.mrc`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/conftest.py` & `cylindra-1.0.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/test_algorithms.py` & `cylindra-1.0.0b1/tests/test_algorithms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
+import polars as pl
 import pytest
 from numpy.testing import assert_allclose
 
-from cylindra.components import CylTomogram
+from cylindra.components import CylSpline, CylTomogram
 from cylindra.const import PropertyNames as H
 from cylindra.project._base import MissingWedge
 
 from ._const import TEST_DIR
 
 coords_13pf = [[18.97, 190.0, 28.99], [18.97, 107.8, 51.48], [18.97, 35.2, 79.90]]
 coords_14pf = [[21.97, 123.1, 32.98], [21.97, 83.3, 40.5], [21.97, 17.6, 64.96]]
@@ -25,14 +26,16 @@
     # the length of spline is ~80 nm
     tomo.add_spline(coords=coords)
     tomo.fit()
     tomo.refine()
     tomo.make_anchors(n=3)
     assert tomo.splines.collect_localprops() is None
     assert tomo.splines.collect_globalprops() is None
+    tomo.measure_radius(positions="auto")
+    tomo.measure_radius(positions=[0.2, 0.8])
     tomo.measure_radius()
     assert tomo.splines.collect_localprops() is None
     assert H.radius in tomo.splines.collect_globalprops(allow_none=False).columns
 
     tomo.make_anchors(interval=30)
     assert tomo.splines.collect_localprops() is None
     assert H.radius in tomo.splines.collect_globalprops(allow_none=False).columns
@@ -70,15 +73,15 @@
     assert cp.spacing == pytest.approx(spl.props.get_glob(H.spacing), abs=1e-6)
     assert cp.twist == pytest.approx(spl.props.get_glob(H.twist), abs=1e-6)
     assert cp.skew == pytest.approx(spl.props.get_glob(H.skew), abs=1e-6)
     assert cp.rise_angle == pytest.approx(spl.props.get_glob(H.rise), abs=1e-6)
 
     tomo.local_radii()
     tomo.local_cft_params(radius="local")
-    tomo.local_cft_params(radius=10.2)
+    tomo.local_cft_params(radius=10.2, update_glob=True)
 
     repr(tomo.splines[0].props)
     tomo.splines[0].props[H.spacing]
     tomo.splines[0].props.select([H.spacing])
     tomo.splines[0].props.update_glob({H.spacing: 4.0})
     tomo.splines[0].props.drop_glob(H.spacing)
     tomo.splines[0].props.drop_loc(H.spacing)
@@ -171,7 +174,26 @@
     tomo = CylTomogram.imread(path, binsize=[1], tilt=tilt, compute=False)
     tilt0 = tomo.tilt
     wedge_model = MissingWedge.parse(tomo.tilt)
     tomo = CylTomogram.imread(
         path, binsize=[1], tilt=wedge_model.as_param(), compute=False
     )
     assert tilt0 == tomo.tilt
+
+
+def test_spline_list():
+    path = TEST_DIR / "13pf_MT.tif"
+    tomo = CylTomogram.imread(path, binsize=[1], compute=False)
+    tomo.add_spline(coords=[[18.97, 190.0, 28.99], [18.97, 107.8, 51.48]])
+    tomo.add_spline(coords=[[18.97, 190.0, 28.99], [18.97, 107.8, 51.48]])
+    tomo.add_spline(coords=[[18.97, 190.0, 28.99], [18.97, 187.8, 30.00]])
+    for spl in tomo.splines.iter():
+        assert isinstance(spl, CylSpline)
+        spl.props.update_glob(length=spl.length())
+    for _, spl in tomo.splines.enumerate():
+        spl.make_anchors(n=3)
+    splines_filt = tomo.splines.filter(pl.col("length") > 60)
+    assert len(splines_filt) == 2
+    assert len(tomo.splines.sort(pl.col("length"))) == 3
+    for coords in tomo.splines.iter_anchor_coords():
+        assert isinstance(coords, np.ndarray)
+    tomo.splines.remove(tomo.splines[1])
```

### Comparing `cylindra-1.0.0b0/tests/test_custom_widgets.py` & `cylindra-1.0.0b1/tests/test_custom_widgets.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/test_cylfilters.py` & `cylindra-1.0.0b1/tests/test_cylfilters.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/test_cylindric_model.py` & `cylindra-1.0.0b1/tests/test_cylindric_model.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/test_gui_0.py` & `cylindra-1.0.0b1/tests/test_gui_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from cylindra import _config, cylmeasure, view_project
 from cylindra._config import get_config
 from cylindra.const import (
     MoleculesHeader as Mole,
 )
 from cylindra.const import PropertyNames as H
 from cylindra.widgets import CylindraMainWidget
-from cylindra.widgets.sta import MaskChoice
+from cylindra.widgets.sta import MaskChoice, TemplateChoice
 
 from ._const import PROJECT_DIR_13PF, PROJECT_DIR_14PF, TEST_DIR
 from .utils import ExceptionGroup, pytest_group
 
 coords_13pf = [[18.97, 190.0, 28.99], [18.97, 107.8, 51.48]]
 coords_14pf = [[21.97, 123.1, 32.98], [21.97, 83.3, 40.5]]
 coords = {13: coords_13pf, 14: coords_14pf}
@@ -67,14 +67,21 @@
 
 def test_tooltip(ui: CylindraMainWidget):
     mcls_testing.check_tooltip(ui)
     mcls_testing.check_tooltip(ui.sta)
     mcls_testing.check_tooltip(ui.simulator)
 
 
+def test_plugin(make_napari_viewer):
+    from cylindra.core import start_as_plugin
+
+    make_napari_viewer()
+    start_as_plugin(run=False)
+
+
 @pytest.mark.parametrize(
     "save_path,npf", [(PROJECT_DIR_13PF, 13), (PROJECT_DIR_14PF, 14)]
 )
 def test_io(ui: CylindraMainWidget, save_path: Path, npf: int):
     path = TEST_DIR / f"{npf}pf_MT.tif"
     ui.open_image(path=path, scale=1.052, tilt_range=(-60, 60), bin_size=[1])
     ui.add_multiscale(2)
@@ -164,14 +171,17 @@
     ui.SplineControl.pos = 1
     ui.SplineControl.footer.highlight_subvolume = False
 
     ui.load_project(PROJECT_DIR_14PF, filter=None, read_image=False)
     ui.mole_layers.get("Mole-0")
     ui.mole_layers.get("Mole-100", None)
     list(ui.mole_layers.iter())
+    ui.mole_layers.first()
+    ui.mole_layers.count()
+    assert "Mole-0" in ui.mole_layers
 
 
 def test_picking_splines(ui: CylindraMainWidget):
     path = TEST_DIR / "13pf_MT.tif"
     ui.open_image(path=path, scale=1.052, tilt_range=(-60, 60), bin_size=[1, 2])
     ui._reserved_layers.work.add(coords_13pf[0])
     ui._reserved_layers.work.add(coords_13pf[1])
@@ -204,14 +214,22 @@
     assert ui._reserved_layers.prof.features["spline-id"].values[-1] == 0.0
     ui.Toolbar.redo()
     ui.Toolbar.redo()
     assert ui._reserved_layers.prof.features["spline-id"].values[0] == 0.0
     assert ui._reserved_layers.prof.features["spline-id"].values[-1] == 0.0
 
 
+def test_serialize(ui: CylindraMainWidget):
+    from magicclass.serialize import deserialize, serialize
+
+    ui.load_project(PROJECT_DIR_13PF, filter=None)
+    d = serialize(ui)
+    deserialize(ui, d)
+
+
 def test_workflow_with_many_input(ui: CylindraMainWidget):
     ui.load_project(PROJECT_DIR_14PF, filter=None)
     exc_group = ExceptionGroup()
     with exc_group.merging():
         ui._runner.run([0], max_shift=-1)  # no fit
     with exc_group.merging():
         ui._runner.run([0], n_refine=0)  # no refine
@@ -519,14 +537,18 @@
     tester.click_preview()
     tester = mcls_testing.FunctionGuiTester(ui.sta.seam_search_manually)
     tester.click_preview()
     ui.binarize_feature(ui.mole_layers["Mole-0"], "nth", threshold=3)
     tester = mcls_testing.FunctionGuiTester(ui.label_feature_clusters)
     tester.click_preview()
 
+    # two preview layers
+    mcls_testing.FunctionGuiTester(ui.translate_molecules).click_preview()
+    mcls_testing.FunctionGuiTester(ui.map_along_pf).click_preview()
+
 
 def test_sub_widgets(ui: CylindraMainWidget):
     ui.load_project(PROJECT_DIR_13PF, filter=None)
     ui.ImageMenu.open_slicer()
     with thread_worker.blocking_mode():
         ui.spline_slicer.refresh_widget_state()
         ui.spline_slicer.show_what = "CFT"
@@ -658,14 +680,15 @@
     ui.sta.calculate_correlation(
         layers=["Mole-0-ALN1"],
         template_path=template_path,
         column_prefix="score",
     )
     ui.sta.get_subtomograms("Mole-0", shape=(5, 5, 5), bin_size=bin_size, order=1)
     assert "score_0" in ui.mole_layers["Mole-0-ALN1"].features
+    ui.sta.params.template_choice = TemplateChoice.from_files
 
 
 def test_seam_search(ui: CylindraMainWidget):
     ui.load_project(PROJECT_DIR_13PF, filter=None)
     ui.filter_molecules(
         ui.parent_viewer.layers["Mole-0"], predicate="pl.col('nth') < 5"
     )
@@ -706,14 +729,23 @@
                 size=12.0,
                 interpolation=1,
                 bin_size=binsize,
             )
     exc_group.raise_exceptions()
 
 
+def test_extend_filament(ui: CylindraMainWidget):
+    ui.load_project(PROJECT_DIR_13PF, filter=None)
+    ui.sta.extend_filaments(
+        "Mole-1",
+        TEST_DIR / "beta-tubulin.mrc",
+        min_score=0.8,
+    )
+
+
 def test_clip_spline(ui: CylindraMainWidget):
     path = TEST_DIR / "13pf_MT.tif"
     ui.open_image(path=path, scale=1.052, tilt_range=(-60, 60), bin_size=2)
     ui.register_path(coords=coords_13pf)
     length_old = ui.tomogram.splines[0].length()
     ui.clip_spline(0, (10, 5))
     length_new = ui.tomogram.splines[0].length()
@@ -801,14 +833,18 @@
         ui.simulator.twist,
         ui.simulator.dilate,
         ui.simulator.displace,
     ]:
         tester = mcls_testing.FunctionGuiTester(method)
         tester.click_preview()
         tester.click_preview()
+
+    ui.simulator.add_component(layer, TEST_DIR / "beta-tubulin.mrc")
+    comp = list(ui.simulator.component_list._iter_components())[0]
+    comp.remove_me()
     ui.simulator.close()
 
 
 @pytest_group("simulate", maxfail=1)
 def test_simulate_tomogram(ui: CylindraMainWidget):
     ui.simulator.create_image_with_straight_line(25, (40, 42, 42), scale=0.5)
     ui.simulator.generate_molecules(
@@ -848,14 +884,19 @@
         ui.simulator.simulate_tilt_series(
             components=[(ui.mole_layers.last().name, TEST_DIR / "beta-tubulin.mrc")],
             save_dir=dirpath,
             tilt_range=(-60.0, 60.0),
             n_tilt=11,
             interpolation=1,
         )
+        ui.simulator.simulate_projection(
+            components=[(ui.mole_layers.last().name, TEST_DIR / "beta-tubulin.mrc")],
+            save_dir=Path(dirpath) / "projection_test",
+            nsr=[0.1, 1.5],
+        )
         ui.simulator.simulate_tomogram_from_tilt_series(Path(dirpath) / "image.mrc")
     ui.simulator.close()
 
 
 def test_project_viewer():
     pviewer = view_project(PROJECT_DIR_14PF)
     # TODO: fails due to delayed returned callback
@@ -1396,17 +1437,18 @@
     ui.sta.run_viterbi_on_landscape(
         layer_land,
         range_long=("-0.1", "+0.1"),
         angle_max=10,
     )
     # click preview
     tester = mcls_testing.FunctionGuiTester(ui.sta.run_annealing_on_landscape)
+    tester.gui  # noqa: B018
     tester.click_preview()
     ui.sta.run_annealing_on_landscape(
-        layer_land,
+        layer_land.name,
         range_long=("-0.1", "+0.1"),
         range_lat=("-0.1", "+0.1"),
         angle_max=20,
         random_seeds=[0, 1],
     )
     with tempfile.TemporaryDirectory() as dirpath:
         dirpath = Path(dirpath)
@@ -1455,14 +1497,29 @@
     ui.OthersMenu.open_logger()
     loader = ui.FileMenu.open_image_loader()
     loader.path = TEST_DIR / "13pf_MT.tif"
     loader.scan_header()
     loader.preview_image().close()
     ui.FileMenu.view_project(PROJECT_DIR_13PF / "project.json")
 
+    loader.tilt_model.value = None
+    assert loader.tilt_model.value is None
+    loader.tilt_model.value = {"kind": "x", "range": (-50, 60)}
+    assert loader.tilt_model.value == {"kind": "x", "range": (-50, 60)}
+    loader.tilt_model.value = {"kind": "y", "range": (-50, 60)}
+    assert loader.tilt_model.value == {"kind": "y", "range": (-50, 60)}
+    loader.tilt_model.value = {"kind": "dual", "xrange": (-50, 60), "yrange": (-50, 60)}
+    assert loader.tilt_model.value == {
+        "kind": "dual",
+        "xrange": (-50, 60),
+        "yrange": (-50, 60),
+    }
+    loader.tilt_model.value = (-60, 60)
+    assert loader.tilt_model.value == {"kind": "y", "range": (-60, 60)}
+
 
 def test_image_processor(ui: CylindraMainWidget):
     input_path = TEST_DIR / "13pf_MT.tif"
     ui.FileMenu.open_image_processor()
     ui.image_processor.input_image = input_path
     with tempfile.TemporaryDirectory() as dirpath:
         output_path = Path(dirpath) / "output.tif"
@@ -1509,7 +1566,9 @@
         name0 = _config.get_stash_list()[0]
         ui.FileMenu.Stash.load_stash_project(name0, filter=None)
         ui.FileMenu.Stash.pop_stash_project(name0, filter=None)
         ui.FileMenu.Stash.stash_project()
         name1 = _config.get_stash_list()[0]
         ui.FileMenu.Stash.delete_stash_project(name1)
         ui.FileMenu.Stash.clear_stash_projects()
+    ui.OthersMenu.configure_dask(num_workers=2)
+    ui.OthersMenu.configure_dask(num_workers=None)
```

### Comparing `cylindra-1.0.0b0/tests/test_gui_1_batch.py` & `cylindra-1.0.0b1/tests/test_gui_1_batch.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/test_gui_2_extensions.py` & `cylindra-1.0.0b1/tests/test_gui_2_extensions.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/test_projects.py` & `cylindra-1.0.0b1/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/test_regionprops.py` & `cylindra-1.0.0b1/tests/test_regionprops.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/test_splines.py` & `cylindra-1.0.0b1/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/test_utils.py` & `cylindra-1.0.0b1/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import impy as ip
 import numpy as np
+import polars as pl
 import pytest
 from numpy.testing import assert_allclose
 
-from cylindra import utils
+from cylindra import utils, widget_utils
 from cylindra.components.seam_search import BooleanSeamSearcher
 
 
 def test_ints():
     assert utils.roundint(1.0) == 1
     assert utils.roundint(2.0) == 2
     assert utils.roundint(1.47) == 1
@@ -163,7 +164,18 @@
         (np.array([[1, 0, 0, 0], [0, 1, 1, 1], [1, 0, 0, 0], [0, 1, 1, 1]]).ravel(), 1),
         (np.array([[1, 0, 1, 0], [0, 0, 0, 1], [1, 1, 1, 0], [1, 0, 0, 1]]).ravel(), 3),
     ],
 )
 def test_infer_seam(label, expected: int):
     searcher = BooleanSeamSearcher(npf=4)
     assert searcher.search(label).seam_pos == expected
+
+
+def test_rust_expressions():
+    assert widget_utils._polars_expr_to_str(pl.col("a") == 3) == "col('a') == 3"
+    assert widget_utils._polars_expr_to_str(pl.col("f") == -4.2) == "col('f') == (-4.2)"
+    assert widget_utils._polars_expr_to_str(pl.col("b") == "ts") == "col('b') == 'ts'"
+
+
+def test_validate():
+    widget_utils._validate_expr_or_scalar(pl.col("a") == 3)
+    widget_utils._validate_expr_or_scalar('pl.col("a") == 3')
```

### Comparing `cylindra-1.0.0b0/tests/test_viterbi.py` & `cylindra-1.0.0b1/tests/test_viterbi.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/tests/utils.py` & `cylindra-1.0.0b1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cylindra-1.0.0b0/Cargo.lock` & `cylindra-1.0.0b1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
@@ -18,28 +18,28 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cylindra_ext"
-version = "1.0.0-beta.0"
+version = "1.0.0-beta.1"
 dependencies = [
  "mt19937",
  "num",
  "numpy",
  "pyo3",
  "rand",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -123,19 +123,18 @@
  "num-iter",
  "num-rational",
  "num-traits",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
 version = "0.4.5"
@@ -152,17 +151,17 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
+checksum = "1429034a0490724d0075ebb2bc9e875d6503c3cf69e235a8941aa757d83ef5bf"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
@@ -175,17 +174,17 @@
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
 version = "0.20.0"
@@ -240,17 +239,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -384,17 +383,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `cylindra-1.0.0b0/pyproject.toml` & `cylindra-1.0.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Framework :: napari",
 ]
 license = { file = "LICENSE" }
 dynamic = ["version"]
 dependencies = [
     "impy-array>=2.4.1",
     "acryo>=0.4.7",
     "macro-kit>=0.4.6",
@@ -80,14 +81,17 @@
     "mkdocstrings-python>=1.7.5",
     "maturin>=1.5.0,<2.0.0",
 ]
 
 [project.scripts]
 cylindra = "cylindra.__main__:main"
 
+[project.entry-points."napari.manifest"]
+cylindra = "cylindra:napari.yaml"
+
 [tool.maturin]
 include = ["**/*.pyi", "*.pyi", "**/*.svg", "**/*.yaml", "**/*.qss", "**/*.json"]
 features = ["pyo3/extension-module"]
 module-name = "cylindra._cylindra_ext"
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `cylindra-1.0.0b0/PKG-INFO` & `cylindra-1.0.0b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.3
 Name: cylindra
-Version: 1.0.0b0
+Version: 1.0.0b1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Framework :: napari
 Requires-Dist: impy-array >=2.4.1
 Requires-Dist: acryo >=0.4.7
 Requires-Dist: macro-kit >=0.4.6
 Requires-Dist: magicgui >=0.8.1
 Requires-Dist: magic-class >=0.7.10
 Requires-Dist: psygnal >=0.9.1
 Requires-Dist: superqt[iconify] >=0.6.1
@@ -65,25 +66,24 @@
 Author-email: liuha@med.kobe-u.ac.jp
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 [![BSD 3-Clause License](https://img.shields.io/pypi/l/cylindra.svg?color=green)](https://github.com/hanjinliu/cylindra/blob/main/LICENSE)
 [![Python package index download statistics](https://img.shields.io/pypi/dm/cylindra.svg)](https://pypistats.org/packages/cylindra)
 [![PyPI version](https://badge.fury.io/py/cylindra.svg)](https://badge.fury.io/py/cylindra)
+[![codecov](https://codecov.io/gh/hanjinliu/cylindra/graph/badge.svg?token=X1F259JYT5)](https://codecov.io/gh/hanjinliu/cylindra)
+
+![](https://github.com/hanjinliu/cylindra/blob/main/resources/fig.png)
 
 # cylindra
 
 `cylindra` is a GUI-integrated cryo-ET image analysis tool for cylindric periodic
 structures such as microtubules.
 
-![](resources/fig.png)
-
-## Documentation
-
-COMING SOON
+### [&rarr; Documentation](https://hanjinliu.github.io/cylindra/)
 
 ## Installation
 
 - Use `pip`
 
 ```shell
 pip install cylindra -U
@@ -146,20 +146,24 @@
   recommended.
 - **Images should be loaded from SSD**. Raw image stacks are loaded lazily in most of
   the processes. Loading from HDD will slow down many analyses as well.
 
 ## Issues
 
 If you encountered any bugs or have any requests, feel free to
-[report an issue](https://github.com/hanjinliu/cylindra/issues).
+[report an issue](https://github.com/hanjinliu/cylindra/issues/new).
 (We'll appreciate if you find some methods are over-fitted to microtubules and do not
 work well on other cylindric structures)
 
 For better reproducibility, please copy your environments from `Others > cylindra info`
 and the recorded macro from `Others > Macro > Show macro`.
 
 ## Citation
 
-If you find `cylindra` useful in your work, please consider citing our paper.
+If you find `cylindra` useful in your work, please consider citing [our paper](https://www.biorxiv.org/content/10.1101/2024.04.30.591984v1).
 
-COMING SOON
+```
+Heterogeneous local structures of the microtubule lattice revealed by cryo-ET and non-averaging analysis
+Hanjin Liu, Hiroshi Yamaguchi, Masahide Kikkawa, Tomohiro Shima
+bioRxiv 2024.04.30.591984; doi: https://doi.org/10.1101/2024.04.30.591984
+```
```

