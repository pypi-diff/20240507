# Comparing `tmp/contentctl-3.6.0.tar.gz` & `tmp/contentctl-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentctl-3.6.0.tar", max compression
+gzip compressed data, was "contentctl-4.0.1.tar", max compression
```

## Comparing `contentctl-3.6.0.tar` & `contentctl-4.0.1.tar`

### file list

```diff
@@ -1,175 +1,167 @@
--rw-r--r--   0        0        0    11344 2024-04-23 21:34:59.965770 contentctl-3.6.0/LICENSE.md
--rw-r--r--   0        0        0    17550 2024-04-23 21:34:59.969770 contentctl-3.6.0/README.md
--rw-r--r--   0        0        0       22 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/__init__.py
--rw-r--r--   0        0        0     1418 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/acs_deploy.py
--rw-r--r--   0        0        0     2999 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/apav_deploy.py
--rw-r--r--   0        0        0     6965 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/api_deploy.py
--rw-r--r--   0        0        0      704 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/convert.py
--rw-r--r--   0        0        0     5580 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/DataManipulation.py
--rw-r--r--   0        0        0     7257 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/DetectionTestingManager.py
--rw-r--r--   0        0        0    11155 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/GitService.py
--rw-r--r--   0        0        0     2259 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
--rw-r--r--   0        0        0    53389 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
--rw-r--r--   0        0        0     5327 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
--rw-r--r--   0        0        0      370 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
--rw-r--r--   0        0        0     3244 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/progress_bar.py
--rw-r--r--   0        0        0     7015 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingView.py
--rw-r--r--   0        0        0     2050 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
--rw-r--r--   0        0        0     1386 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
--rw-r--r--   0        0        0     4706 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
--rw-r--r--   0        0        0      857 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/doc_gen.py
--rw-r--r--   0        0        0     5273 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/generate.py
--rw-r--r--   0        0        0     3102 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/initialize.py
--rw-r--r--   0        0        0     9333 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/initialize_old.py
--rw-r--r--   0        0        0      992 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/new_content.py
--rw-r--r--   0        0        0    10193 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/release_notes.py
--rw-r--r--   0        0        0     1102 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/reporting.py
--rw-r--r--   0        0        0     3863 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/test.py
--rw-r--r--   0        0        0     2595 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/actions/validate.py
--rw-r--r--   0        0        0    31622 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/contentctl.py
--rw-r--r--   0        0        0     4392 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/enrichments/attack_enrichment.py
--rw-r--r--   0        0        0     3242 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/enrichments/cve_enrichment.py
--rw-r--r--   0        0        0     3418 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/enrichments/splunk_app_enrichment.py
--rw-r--r--   0        0        0     3032 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/helper/config_handler.py
--rw-r--r--   0        0        0     7238 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/helper/link_validator.py
--rw-r--r--   0        0        0        0 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/helper/logger.py
--rw-r--r--   0        0        0    15577 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/helper/utils.py
--rw-r--r--   0        0        0     5861 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/backend_splunk_ba.py
--rw-r--r--   0        0        0     2472 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/baseline_builder.py
--rw-r--r--   0        0        0     2270 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/basic_builder.py
--rw-r--r--   0        0        0    18813 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/detection_builder.py
--rw-r--r--   0        0        0    13161 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/director.py
--rw-r--r--   0        0        0     1244 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/investigation_builder.py
--rw-r--r--   0        0        0     4979 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/new_content_generator.py
--rw-r--r--   0        0        0     5610 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/new_content_questions.py
--rw-r--r--   0        0        0     2100 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/playbook_builder.py
--rw-r--r--   0        0        0    19512 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/sigma_converter.py
--rw-r--r--   0        0        0     7584 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/ssa_detection_builder.py
--rw-r--r--   0        0        0     4755 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/story_builder.py
--rw-r--r--   0        0        0     1385 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/input/yml_reader.py
--rw-r--r--   0        0        0    15307 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/abstract_security_content_objects/detection_abstract.py
--rw-r--r--   0        0        0     3015 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py
--rw-r--r--   0        0        0     7519 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/app.py
--rw-r--r--   0        0        0     1028 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/base_test.py
--rw-r--r--   0        0        0     4752 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/base_test_result.py
--rw-r--r--   0        0        0     1931 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/baseline.py
--rw-r--r--   0        0        0      711 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/baseline_tags.py
--rw-r--r--   0        0        0     6069 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/config.py
--rw-r--r--   0        0        0     3518 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/constants.py
--rw-r--r--   0        0        0    36903 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/correlation_search.py
--rw-r--r--   0        0        0      434 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/data_source.py
--rw-r--r--   0        0        0     1137 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment.py
--rw-r--r--   0        0        0      141 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_email.py
--rw-r--r--   0        0        0      164 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_notable.py
--rw-r--r--   0        0        0      201 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_phantom.py
--rw-r--r--   0        0        0      111 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_rba.py
--rw-r--r--   0        0        0      193 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_scheduling.py
--rw-r--r--   0        0        0      129 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/deployment_slack.py
--rw-r--r--   0        0        0      644 2024-04-23 21:34:59.969770 contentctl-3.6.0/contentctl/objects/detection.py
--rw-r--r--   0        0        0     6338 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/detection_tags.py
--rw-r--r--   0        0        0     2963 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/enums.py
--rw-r--r--   0        0        0     1285 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/integration_test.py
--rw-r--r--   0        0        0      429 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/integration_test_result.py
--rw-r--r--   0        0        0     2151 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/investigation.py
--rw-r--r--   0        0        0      191 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/investigation_tags.py
--rw-r--r--   0        0        0     2397 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/lookup.py
--rw-r--r--   0        0        0     3255 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/macro.py
--rw-r--r--   0        0        0      219 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/mitre_attack_enrichment.py
--rw-r--r--   0        0        0     1605 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/notable_action.py
--rw-r--r--   0        0        0     1288 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/observable.py
--rw-r--r--   0        0        0     1081 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/playbook.py
--rw-r--r--   0        0        0      315 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/playbook_tags.py
--rw-r--r--   0        0        0     6353 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/repo_config.py
--rw-r--r--   0        0        0     4288 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/risk_analysis_action.py
--rw-r--r--   0        0        0      904 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/risk_object.py
--rw-r--r--   0        0        0      325 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/security_content_object.py
--rw-r--r--   0        0        0     5806 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/ssa_detection.py
--rw-r--r--   0        0        0     5668 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/ssa_detection_tags.py
--rw-r--r--   0        0        0     1532 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/story.py
--rw-r--r--   0        0        0     1213 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/story_tags.py
--rw-r--r--   0        0        0    25020 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/test_config.py
--rw-r--r--   0        0        0     2600 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/test_group.py
--rw-r--r--   0        0        0      711 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/threat_object.py
--rw-r--r--   0        0        0     1412 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/unit_test.py
--rw-r--r--   0        0        0      606 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/unit_test_attack_data.py
--rw-r--r--   0        0        0      255 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/unit_test_baseline.py
--rw-r--r--   0        0        0      182 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/unit_test_old.py
--rw-r--r--   0        0        0     2874 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/objects/unit_test_result.py
--rw-r--r--   0        0        0     6174 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/api_json_output.py
--rw-r--r--   0        0        0     1701 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/attack_nav_output.py
--rw-r--r--   0        0        0     2130 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/attack_nav_writer.py
--rw-r--r--   0        0        0     5938 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/ba_yml_output.py
--rw-r--r--   0        0        0    24175 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/conf_output.py
--rw-r--r--   0        0        0     2960 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/conf_writer.py
--rw-r--r--   0        0        0      960 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/detection_writer.py
--rw-r--r--   0        0        0     3238 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/doc_md_output.py
--rw-r--r--   0        0        0     3935 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/finding_report_writer.py
--rw-r--r--   0        0        0     1089 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/jinja_writer.py
--rw-r--r--   0        0        0      209 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/json_writer.py
--rw-r--r--   0        0        0     2254 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/new_content_yml_output.py
--rw-r--r--   0        0        0     3084 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/svg_output.py
--rw-r--r--   0        0        0      745 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/analyticstories_detections.j2
--rw-r--r--   0        0        0      496 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/analyticstories_investigations.j2
--rw-r--r--   0        0        0      592 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/analyticstories_stories.j2
--rw-r--r--   0        0        0      717 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/app.conf.j2
--rw-r--r--   0        0        0     1047 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/app.manifest.j2
--rw-r--r--   0        0        0      181 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/collections.j2
--rw-r--r--   0        0        0       54 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/content-version.j2
--rw-r--r--   0        0        0      670 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/detection_count.j2
--rw-r--r--   0        0        0      671 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/detection_coverage.j2
--rw-r--r--   0        0        0     1002 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_detection_page.j2
--rw-r--r--   0        0        0     6586 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_detections.j2
--rw-r--r--   0        0        0     1471 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_navigation.j2
--rw-r--r--   0        0        0      203 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_navigation_pages.j2
--rw-r--r--   0        0        0     1681 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_playbooks.j2
--rw-r--r--   0        0        0      679 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_playbooks_page.j2
--rw-r--r--   0        0        0     1822 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_stories.j2
--rw-r--r--   0        0        0      874 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/doc_story_page.j2
--rw-r--r--   0        0        0      994 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/es_investigations_investigations.j2
--rw-r--r--   0        0        0      369 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/es_investigations_stories.j2
--rw-r--r--   0        0        0     1753 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/finding_report.j2
--rw-r--r--   0        0        0      177 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/header.j2
--rw-r--r--   0        0        0      424 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/macros.j2
--rw-r--r--   0        0        0      282 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/macros_detections.j2
--rw-r--r--   0        0        0      221 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/panel.j2
--rw-r--r--   0        0        0     1645 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/savedsearches_baselines.j2
--rw-r--r--   0        0        0     6288 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/savedsearches_detections.j2
--rw-r--r--   0        0        0     1180 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/savedsearches_investigations.j2
--rw-r--r--   0        0        0      897 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_story_detail.txt
--rw-r--r--   0        0        0     2538 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_summary.txt
--rw-r--r--   0        0        0     2432 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_usage_dashboard.txt
--rw-r--r--   0        0        0      467 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/README.md
--rw-r--r--   0        0        0      168 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/analytic_stories.conf
--rw-r--r--   0        0        0      685 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/app.conf
--rw-r--r--   0        0        0      319 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/commands.conf
--rw-r--r--   0        0        0       34 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/content-version.conf
--rw-r--r--   0        0        0      208 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/data/ui/nav/default.xml
--rw-r--r--   0        0        0     8635 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/data/ui/views/escu_summary.xml
--rw-r--r--   0        0        0      696 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/data/ui/views/feedback.xml
--rw-r--r--   0        0        0      156 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/distsearch.conf
--rw-r--r--   0        0        0     4257 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/usage_searches.conf
--rw-r--r--   0        0        0      168 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/default/use_case_library.conf
--rw-r--r--   0        0        0      423 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/metadata/default.meta
--rw-r--r--   0        0        0     3658 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIcon.png
--rw-r--r--   0        0        0     2656 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIconAlt.png
--rw-r--r--   0        0        0     7442 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIconAlt_2x.png
--rw-r--r--   0        0        0     3657 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png
--rw-r--r--   0        0        0     1416 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/transforms.j2
--rw-r--r--   0        0        0      925 2024-04-23 21:34:59.973770 contentctl-3.6.0/contentctl/output/templates/workflow_actions.j2
--rw-r--r--   0        0        0     2682 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/output/yml_output.py
--rw-r--r--   0        0        0      240 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/output/yml_writer.py
--rw-r--r--   0        0        0      133 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/README
--rw-r--r--   0        0        0     6390 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/app_default.yml
--rw-r--r--   0        0        0     9381 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/datamodels_cim.conf
--rw-r--r--   0        0        0      480 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/datamodels_custom.conf
--rw-r--r--   0        0        0      426 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/deployments/00_default_anomaly.yml
--rw-r--r--   0        0        0      342 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/deployments/00_default_baseline.yml
--rw-r--r--   0        0        0      528 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/deployments/00_default_correlation.yml
--rw-r--r--   0        0        0      336 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/deployments/00_default_hunting.yml
--rw-r--r--   0        0        0      556 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/deployments/00_default_ttp.yml
--rw-r--r--   0        0        0     3342 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml
--rw-r--r--   0        0        0      159 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/macros/security_content_ctime.yml
--rw-r--r--   0        0        0      162 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/macros/security_content_summariesonly.yml
--rw-r--r--   0        0        0     3095 2024-04-23 21:34:59.977770 contentctl-3.6.0/contentctl/templates/stories/cobalt_strike.yml
--rw-r--r--   0        0        0      815 2024-04-23 21:34:59.977770 contentctl-3.6.0/pyproject.toml
--rw-r--r--   0        0        0    18805 1970-01-01 00:00:00.000000 contentctl-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-05-07 02:00:52.753300 contentctl-4.0.1/LICENSE.md
+-rw-r--r--   0        0        0    18472 2024-05-07 02:00:52.753300 contentctl-4.0.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/__init__.py
+-rw-r--r--   0        0        0     1418 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/acs_deploy.py
+-rw-r--r--   0        0        0     2999 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/apav_deploy.py
+-rw-r--r--   0        0        0     6965 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/api_deploy.py
+-rw-r--r--   0        0        0     4765 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/build.py
+-rw-r--r--   0        0        0      704 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/convert.py
+-rw-r--r--   0        0        0     8818 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/DetectionTestingManager.py
+-rw-r--r--   0        0        0     8666 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/GitService.py
+-rw-r--r--   0        0        0     2259 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
+-rw-r--r--   0        0        0    53141 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
+-rw-r--r--   0        0        0     6846 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
+-rw-r--r--   0        0        0      370 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
+-rw-r--r--   0        0        0     3244 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/progress_bar.py
+-rw-r--r--   0        0        0     7013 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingView.py
+-rw-r--r--   0        0        0     2050 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
+-rw-r--r--   0        0        0     1123 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
+-rw-r--r--   0        0        0     4706 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
+-rw-r--r--   0        0        0      863 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/doc_gen.py
+-rw-r--r--   0        0        0     1749 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/initialize.py
+-rw-r--r--   0        0        0     9333 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/initialize_old.py
+-rw-r--r--   0        0        0    12628 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/inspect.py
+-rw-r--r--   0        0        0     5792 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/new_content.py
+-rw-r--r--   0        0        0    13115 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/release_notes.py
+-rw-r--r--   0        0        0     1583 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/reporting.py
+-rw-r--r--   0        0        0     4896 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/test.py
+-rw-r--r--   0        0        0     2363 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/validate.py
+-rw-r--r--   0        0        0    10083 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/contentctl.py
+-rw-r--r--   0        0        0     6732 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/enrichments/attack_enrichment.py
+-rw-r--r--   0        0        0     3934 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/enrichments/cve_enrichment.py
+-rw-r--r--   0        0        0     3418 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/enrichments/splunk_app_enrichment.py
+-rw-r--r--   0        0        0     7139 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/helper/link_validator.py
+-rw-r--r--   0        0        0        0 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/helper/logger.py
+-rw-r--r--   0        0        0    15659 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/helper/utils.py
+-rw-r--r--   0        0        0     5861 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/backend_splunk_ba.py
+-rw-r--r--   0        0        0    10716 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/director.py
+-rw-r--r--   0        0        0     5718 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/new_content_questions.py
+-rw-r--r--   0        0        0    19391 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/sigma_converter.py
+-rw-r--r--   0        0        0     8377 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/ssa_detection_builder.py
+-rw-r--r--   0        0        0     1475 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/yml_reader.py
+-rw-r--r--   0        0        0    30167 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/abstract_security_content_objects/detection_abstract.py
+-rw-r--r--   0        0        0     8065 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py
+-rw-r--r--   0        0        0     1335 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/alert_action.py
+-rw-r--r--   0        0        0     8979 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/atomic.py
+-rw-r--r--   0        0        0     1028 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/base_test.py
+-rw-r--r--   0        0        0     4752 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/base_test_result.py
+-rw-r--r--   0        0        0     2248 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/baseline.py
+-rw-r--r--   0        0        0     2978 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/baseline_tags.py
+-rw-r--r--   0        0        0    43708 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/config.py
+-rw-r--r--   0        0        0     3468 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/constants.py
+-rw-r--r--   0        0        0    36891 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/correlation_search.py
+-rw-r--r--   0        0        0      405 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/data_source.py
+-rw-r--r--   0        0        0     2651 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment.py
+-rw-r--r--   0        0        0      147 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_email.py
+-rw-r--r--   0        0        0      198 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_notable.py
+-rw-r--r--   0        0        0      207 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_phantom.py
+-rw-r--r--   0        0        0      125 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_rba.py
+-rw-r--r--   0        0        0      198 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_scheduling.py
+-rw-r--r--   0        0        0      135 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_slack.py
+-rw-r--r--   0        0        0      620 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/detection.py
+-rw-r--r--   0        0        0    10238 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/detection_tags.py
+-rw-r--r--   0        0        0    14030 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/enums.py
+-rw-r--r--   0        0        0     1273 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/integration_test.py
+-rw-r--r--   0        0        0      370 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/integration_test_result.py
+-rw-r--r--   0        0        0     2620 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/investigation.py
+-rw-r--r--   0        0        0     1280 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/investigation_tags.py
+-rw-r--r--   0        0        0     4556 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/lookup.py
+-rw-r--r--   0        0        0     2451 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/macro.py
+-rw-r--r--   0        0        0     1073 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/mitre_attack_enrichment.py
+-rw-r--r--   0        0        0     1605 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/notable_action.py
+-rw-r--r--   0        0        0     1156 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/observable.py
+-rw-r--r--   0        0        0     2469 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/playbook.py
+-rw-r--r--   0        0        0     1436 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/playbook_tags.py
+-rw-r--r--   0        0        0     4288 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/risk_analysis_action.py
+-rw-r--r--   0        0        0      904 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/risk_object.py
+-rw-r--r--   0        0        0      234 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/security_content_object.py
+-rw-r--r--   0        0        0     5873 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/ssa_detection.py
+-rw-r--r--   0        0        0     5224 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/ssa_detection_tags.py
+-rw-r--r--   0        0        0     4526 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/story.py
+-rw-r--r--   0        0        0     2169 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/story_tags.py
+-rw-r--r--   0        0        0     2600 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/test_group.py
+-rw-r--r--   0        0        0      711 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/threat_object.py
+-rw-r--r--   0        0        0     1655 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test.py
+-rw-r--r--   0        0        0      480 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test_attack_data.py
+-rw-r--r--   0        0        0      227 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test_baseline.py
+-rw-r--r--   0        0        0      199 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test_old.py
+-rw-r--r--   0        0        0     2940 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test_result.py
+-rw-r--r--   0        0        0      653 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test_ssa.py
+-rw-r--r--   0        0        0     9085 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/api_json_output.py
+-rw-r--r--   0        0        0     2304 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/attack_nav_output.py
+-rw-r--r--   0        0        0     2219 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/attack_nav_writer.py
+-rw-r--r--   0        0        0     5950 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/ba_yml_output.py
+-rw-r--r--   0        0        0    10147 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/conf_output.py
+-rw-r--r--   0        0        0     8280 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/conf_writer.py
+-rw-r--r--   0        0        0      960 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/detection_writer.py
+-rw-r--r--   0        0        0     3238 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/doc_md_output.py
+-rw-r--r--   0        0        0     3935 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/finding_report_writer.py
+-rw-r--r--   0        0        0     1119 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/jinja_writer.py
+-rw-r--r--   0        0        0     1007 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/json_writer.py
+-rw-r--r--   0        0        0     2321 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/new_content_yml_output.py
+-rw-r--r--   0        0        0     2751 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/svg_output.py
+-rw-r--r--   0        0        0      917 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/analyticstories_detections.j2
+-rw-r--r--   0        0        0      515 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/analyticstories_investigations.j2
+-rw-r--r--   0        0        0      668 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/analyticstories_stories.j2
+-rw-r--r--   0        0        0      737 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/app.conf.j2
+-rw-r--r--   0        0        0     1063 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/app.manifest.j2
+-rw-r--r--   0        0        0      181 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/collections.j2
+-rw-r--r--   0        0        0       54 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/content-version.j2
+-rw-r--r--   0        0        0      670 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/detection_count.j2
+-rw-r--r--   0        0        0      631 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/detection_coverage.j2
+-rw-r--r--   0        0        0     1012 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_detection_page.j2
+-rw-r--r--   0        0        0     6596 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_detections.j2
+-rw-r--r--   0        0        0     1471 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_navigation.j2
+-rw-r--r--   0        0        0      203 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_navigation_pages.j2
+-rw-r--r--   0        0        0     1681 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_playbooks.j2
+-rw-r--r--   0        0        0      679 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_playbooks_page.j2
+-rw-r--r--   0        0        0     1827 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_stories.j2
+-rw-r--r--   0        0        0      874 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_story_page.j2
+-rw-r--r--   0        0        0     1003 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/es_investigations_investigations.j2
+-rw-r--r--   0        0        0      388 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/es_investigations_stories.j2
+-rw-r--r--   0        0        0     1753 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/finding_report.j2
+-rw-r--r--   0        0        0      201 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/header.j2
+-rw-r--r--   0        0        0      390 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/macros.j2
+-rw-r--r--   0        0        0      221 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/panel.j2
+-rw-r--r--   0        0        0     1743 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/savedsearches_baselines.j2
+-rw-r--r--   0        0        0     6805 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/savedsearches_detections.j2
+-rw-r--r--   0        0        0     1259 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/output/templates/savedsearches_investigations.j2
+-rw-r--r--   0        0        0     1456 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/output/templates/transforms.j2
+-rw-r--r--   0        0        0      925 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/output/templates/workflow_actions.j2
+-rw-r--r--   0        0        0     2682 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/output/yml_output.py
+-rw-r--r--   0        0        0      271 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/output/yml_writer.py
+-rw-r--r--   0        0        0      133 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/README
+-rw-r--r--   0        0        0     6390 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_default.yml
+-rw-r--r--   0        0        0      897 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/README/essoc_story_detail.txt
+-rw-r--r--   0        0        0     2538 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/README/essoc_summary.txt
+-rw-r--r--   0        0        0     2432 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/README/essoc_usage_dashboard.txt
+-rw-r--r--   0        0        0      366 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/README.md
+-rw-r--r--   0        0        0      168 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/analytic_stories.conf
+-rw-r--r--   0        0        0      685 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/app.conf
+-rw-r--r--   0        0        0      319 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/commands.conf
+-rw-r--r--   0        0        0       34 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/content-version.conf
+-rw-r--r--   0        0        0      236 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/data/ui/nav/default.xml
+-rw-r--r--   0        0        0     8635 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/data/ui/views/escu_summary.xml
+-rw-r--r--   0        0        0      696 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/data/ui/views/feedback.xml
+-rw-r--r--   0        0        0      156 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/distsearch.conf
+-rw-r--r--   0        0        0     4257 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/usage_searches.conf
+-rw-r--r--   0        0        0      168 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/use_case_library.conf
+-rw-r--r--   0        0        0    66072 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/lookups/mitre_enrichment.csv
+-rw-r--r--   0        0        0      423 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/metadata/default.meta
+-rw-r--r--   0        0        0     3658 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/static/appIcon.png
+-rw-r--r--   0        0        0     2656 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/static/appIconAlt.png
+-rw-r--r--   0        0        0     7442 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/static/appIconAlt_2x.png
+-rw-r--r--   0        0        0     3657 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/static/appIcon_2x.png
+-rw-r--r--   0        0        0     9381 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/datamodels_cim.conf
+-rw-r--r--   0        0        0      480 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/datamodels_custom.conf
+-rw-r--r--   0        0        0      418 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_anomaly.yml
+-rw-r--r--   0        0        0      334 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_baseline.yml
+-rw-r--r--   0        0        0      519 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_correlation.yml
+-rw-r--r--   0        0        0      329 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_hunting.yml
+-rw-r--r--   0        0        0      548 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_ttp.yml
+-rw-r--r--   0        0        0     3323 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/detections/anomalous_usage_of_7zip.yml
+-rw-r--r--   0        0        0      159 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/macros/security_content_ctime.yml
+-rw-r--r--   0        0        0      162 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/macros/security_content_summariesonly.yml
+-rw-r--r--   0        0        0     3063 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/stories/cobalt_strike.yml
+-rw-r--r--   0        0        0      849 2024-05-07 02:00:52.761300 contentctl-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0    19705 1970-01-01 00:00:00.000000 contentctl-4.0.1/PKG-INFO
```

### Comparing `contentctl-3.6.0/LICENSE.md` & `contentctl-4.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/README.md` & `contentctl-4.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -174,15 +174,36 @@
 2. **new** - Creates new content (detection, story)
 3. **validate** - Validates written content
 4. **build** - Builds an application suitable for deployment on a search head using Slim, the Splunk Packaging Toolkit
 5. **deploy** - Deploy the security content pack to a Splunk Server
 6. **docs** - Create documentation as Markdown
 7. **reporting** - Create different reporting files such as a Mitre ATT&CK overlay
 
+# Shell tab-complete
 
+Leveraging the tab completion featureset of the CLI library we're using, you can generate tab completions for `contentctl` automatically, for zsh, bash, and tcsh. For additional details, you can view the docs for the library [here.](https://brentyi.github.io/tyro/tab_completion/) 
+
+### Zsh
+If you already have a location for your ZSH tab completions, you only need to run the generation line and can skip the folder creation, configuring the rest to fit with your shell config.
+
+```zsh
+mkdir -p ~/.zfunc
+contentctl --tyro-write-completion zsh ~/.zfunc/_contentctl
+echo "fpath+=~/.zfunc" >> ~/.zshrc
+echo "autoload -Uz compinit && compinit" >> ~/.zshrc
+source ~/.zshrc
+```
+
+### Bash
+
+```bash
+completion_dir=${BASH_COMPLETION_USER_DIR:-${XDG_DATA_HOME:-$HOME/.local/share}/bash-completion}/completions/
+mkdir -p $completion_dir
+contentctl --tyro-write-completion bash ${completion_dir}/_contentctl
+```
 
 # Acronyms
 | Acronym | Meaning| Description | 
 | --------------------- | ------------------------------------------------------- | ---- |
 | SOC | Security Operation Center | Description of a SoC | 
 | DaC | Detection as Code | A systematic approach applying DevOps priciples to Detection Engineering. DaC enables Continuous Integration and Continuous Delivery of Detectionsa via automated validation, testing, and deployment |
 | CICD | Continuous Integration/Continuous Delivery | A modern DevOps practice that encourages users to make small, frequent changes which are automatically tested and deployed. This contrasts with legacy approaches that emphasize large changes which may be manually tested an infrequently deployed. |
```

### Comparing `contentctl-3.6.0/contentctl/actions/acs_deploy.py` & `contentctl-4.0.1/contentctl/actions/acs_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/actions/apav_deploy.py` & `contentctl-4.0.1/contentctl/actions/apav_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/actions/api_deploy.py` & `contentctl-4.0.1/contentctl/actions/api_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/actions/convert.py` & `contentctl-4.0.1/contentctl/actions/convert.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/actions/detection_testing/DetectionTestingManager.py` & `contentctl-4.0.1/contentctl/actions/detection_testing/DetectionTestingManager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,39 @@
-from contentctl.objects.test_config import TestConfig
-from contentctl.actions.detection_testing.infrastructures.DetectionTestingInfrastructure import (
-    DetectionTestingInfrastructure,
-)
-from contentctl.actions.detection_testing.infrastructures.DetectionTestingInfrastructureContainer import (
-    DetectionTestingInfrastructureContainer,
-)
-from contentctl.actions.detection_testing.infrastructures.DetectionTestingInfrastructureServer import (
-    DetectionTestingInfrastructureServer,
-)
-
-from contentctl.objects.app import App
-import pathlib
-import os
-from contentctl.helper.utils import Utils
+from typing import List,Union
+from contentctl.objects.config import test, test_servers, Container,Infrastructure
+from contentctl.actions.detection_testing.infrastructures.DetectionTestingInfrastructure import DetectionTestingInfrastructure
+from contentctl.actions.detection_testing.infrastructures.DetectionTestingInfrastructureContainer import DetectionTestingInfrastructureContainer
+from contentctl.actions.detection_testing.infrastructures.DetectionTestingInfrastructureServer import DetectionTestingInfrastructureServer
 from urllib.parse import urlparse
-import time
 from copy import deepcopy
 from contentctl.objects.enums import DetectionTestingTargetInfrastructure
 import signal
 import datetime
-
 # from queue import Queue
-
-CONTAINER_APP_PATH = pathlib.Path("apps")
-
 from dataclasses import dataclass
-
 # import threading
 import ctypes
 from contentctl.actions.detection_testing.infrastructures.DetectionTestingInfrastructure import (
     DetectionTestingInfrastructure,
     DetectionTestingManagerOutputDto,
 )
 from contentctl.actions.detection_testing.views.DetectionTestingView import (
     DetectionTestingView,
 )
-
 from contentctl.objects.enums import PostTestBehavior
-
 from pydantic import BaseModel, Field
-from contentctl.input.director import DirectorOutputDto
 from contentctl.objects.detection import Detection
-
-
 import concurrent.futures
-
-import tqdm
+import docker
 
 
 @dataclass(frozen=False)
 class DetectionTestingManagerInputDto:
-    config: TestConfig
-    testContent: DirectorOutputDto
+    config: Union[test,test_servers]
+    detections: List[Detection]
     views: list[DetectionTestingView]
 
 
 class DetectionTestingManager(BaseModel):
     input_dto: DetectionTestingManagerInputDto
     output_dto: DetectionTestingManagerOutputDto
     detectionTestingInfrastructureObjects: list[DetectionTestingInfrastructure] = []
@@ -63,15 +41,15 @@
     def setup(self):
         # Some views, such as the Web View, will require some initial setup.
         # for view in self.input_dto.views:
         #    view.setup()
 
         # for content in self.input_dto.testContent.detections:
         #    self.pending_queue.put(content)
-        self.output_dto.inputQueue = self.input_dto.testContent.detections
+        self.output_dto.inputQueue = self.input_dto.detections
         self.create_DetectionTestingInfrastructureObjects()
 
     def execute(self) -> DetectionTestingManagerOutputDto:
         def sigint_handler(signum, frame):
             print("SIGINT (Ctrl-C Received.  Shutting down test...)")
             self.output_dto.terminate = True
             if self.input_dto.config.post_test_behavior in [
@@ -83,21 +61,21 @@
                 print("*******************************")
                 print(
                     "If testing is paused and you are debugging a detection, you MUST hit CTRL-D at the prompt to complete shutdown."
                 )
                 print("*******************************")
 
         signal.signal(signal.SIGINT, sigint_handler)
-
+        
         with concurrent.futures.ThreadPoolExecutor(
-            max_workers=len(self.input_dto.config.infrastructure_config.infrastructures),
+            max_workers=len(self.input_dto.config.test_instances),
         ) as instance_pool, concurrent.futures.ThreadPoolExecutor(
             max_workers=len(self.input_dto.views)
         ) as view_runner, concurrent.futures.ThreadPoolExecutor(
-            max_workers=len(self.input_dto.config.infrastructure_config.infrastructures),
+            max_workers=len(self.input_dto.config.test_instances),
         ) as view_shutdowner:
 
             # Start all the views
             future_views = {
                 view_runner.submit(view.setup): view for view in self.input_dto.views
             }
             # Configure all the instances
@@ -147,39 +125,60 @@
                     result = future.result()
                 except Exception as e:
                     print(f"Error running container: {str(e)}")
 
         return self.output_dto
 
     def create_DetectionTestingInfrastructureObjects(self):
-        import sys
+        #Make sure that, if we need to, we pull the appropriate container
+        for infrastructure in self.input_dto.config.test_instances:
+            if (isinstance(self.input_dto.config, test) and isinstance(infrastructure, Container)):
+                try:
+                    client = docker.from_env()
+                except Exception as e:
+                    raise Exception("Unable to connect to docker.  Are you sure that docker is running on this host?")
+                try:
+                    
+                    parts = self.input_dto.config.container_settings.full_image_path.split(':')
+                    if len(parts) != 2:
+                        raise Exception(f"Expected to find a name:tag in {self.input_dto.config.container_settings.full_image_path}, "
+                                        f"but instead found {parts}. Note that this path MUST include the tag, which is separated by ':'")
+                    
+                    print(
+                        f"Getting the latest version of the container image [{self.input_dto.config.container_settings.full_image_path}]...",
+                        end="",
+                        flush=True,
+                    )
+                    client.images.pull(parts[0], tag=parts[1], platform="linux/amd64")
+                    print("done!")
+                    break
+                except Exception as e:
+                    raise Exception(f"Failed to pull docker container image [{self.input_dto.config.container_settings.full_image_path}]: {str(e)}")
 
-        for infrastructure in self.input_dto.config.infrastructure_config.infrastructures:
+        already_staged_container_files = False
+        for infrastructure in self.input_dto.config.test_instances:
 
-            if (
-                self.input_dto.config.infrastructure_config.infrastructure_type
-                == DetectionTestingTargetInfrastructure.container
-            ):
+            if (isinstance(self.input_dto.config, test) and isinstance(infrastructure, Container)):
+                # Stage the files in the apps dir so that they can be passed directly to
+                # subsequent containers. Do this here, instead of inside each container, to
+                # avoid duplicate downloads/moves/copies
+                if not already_staged_container_files:
+                    self.input_dto.config.getContainerEnvironmentString(stage_file=True)
+                    already_staged_container_files = True
 
                 self.detectionTestingInfrastructureObjects.append(
                     DetectionTestingInfrastructureContainer(
                         global_config=self.input_dto.config, infrastructure=infrastructure, sync_obj=self.output_dto
                     )
                 )
 
-            elif (
-                self.input_dto.config.infrastructure_config.infrastructure_type
-                == DetectionTestingTargetInfrastructure.server
-            ):
-
+            elif (isinstance(self.input_dto.config, test_servers) and isinstance(infrastructure, Infrastructure)):
                 self.detectionTestingInfrastructureObjects.append(
                     DetectionTestingInfrastructureServer(
                         global_config=self.input_dto.config, infrastructure=infrastructure, sync_obj=self.output_dto
                     )
                 )
 
             else:
 
-                print(
-                    f"Unsupported target infrastructure '{self.input_dto.config.infrastructure_config.infrastructure_type}'"
-                )
-                sys.exit(1)
+                raise Exception(f"Unsupported target infrastructure '{infrastructure}' and config type {self.input_dto.config}")
+
```

### Comparing `contentctl-3.6.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py` & `contentctl-4.0.1/contentctl/actions/detection_testing/generate_detection_coverage_badge.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py` & `contentctl-4.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,43 +6,40 @@
 import json
 import datetime
 import tqdm                                                                                         # type: ignore
 import pathlib
 from tempfile import TemporaryDirectory, mktemp
 from ssl import SSLEOFError, SSLZeroReturnError
 from sys import stdout
-from dataclasses import dataclass
+#from dataclasses import dataclass
 from shutil import copyfile
 from typing import Union, Optional
 
-from pydantic import BaseModel, PrivateAttr, Field
+from pydantic import BaseModel, PrivateAttr, Field, dataclasses
 import requests                                                                                     # type: ignore
 import splunklib.client as client                                                                   # type: ignore
 from splunklib.binding import HTTPError                                                             # type: ignore
 from splunklib.results import JSONResultsReader, Message                                            # type: ignore
 import splunklib.results
 from urllib3 import disable_warnings
 import urllib.parse
 
+from contentctl.objects.config import test_common, Infrastructure
 from contentctl.objects.enums import PostTestBehavior, AnalyticsType
 from contentctl.objects.detection import Detection
 from contentctl.objects.base_test import BaseTest
 from contentctl.objects.unit_test import UnitTest
 from contentctl.objects.integration_test import IntegrationTest
 from contentctl.objects.unit_test_attack_data import UnitTestAttackData
 from contentctl.objects.unit_test_result import UnitTestResult
 from contentctl.objects.integration_test_result import IntegrationTestResult
-from contentctl.objects.test_config import TestConfig, Infrastructure
 from contentctl.objects.test_group import TestGroup
 from contentctl.objects.base_test_result import TestResultStatus
 from contentctl.objects.correlation_search import CorrelationSearch, PbarData
 from contentctl.helper.utils import Utils
-from contentctl.actions.detection_testing.DataManipulation import (
-    DataManipulation,
-)
 from contentctl.actions.detection_testing.progress_bar import (
     format_pbar_string,
     TestReportingType,
     FinalTestingStates,
     TestingStates
 )
 
@@ -62,30 +59,30 @@
     start_time: float
 
 
 class ContainerStoppedException(Exception):
     pass
 
 
-@dataclass(frozen=False)
-class DetectionTestingManagerOutputDto:
+@dataclasses.dataclass(frozen=False)
+class DetectionTestingManagerOutputDto():
     inputQueue: list[Detection] = Field(default_factory=list)
     outputQueue: list[Detection] = Field(default_factory=list)
     skippedQueue: list[Detection] = Field(default_factory=list)
     currentTestingQueue: dict[str, Union[Detection, None]] = Field(default_factory=dict)
     start_time: Union[datetime.datetime, None] = None
     replay_index: str = "CONTENTCTL_TESTING_INDEX"
     replay_host: str = "CONTENTCTL_HOST"
     timeout_seconds: int = 60
     terminate: bool = False
 
 
 class DetectionTestingInfrastructure(BaseModel, abc.ABC):
     # thread: threading.Thread = threading.Thread()
-    global_config: TestConfig
+    global_config: test_common
     infrastructure: Infrastructure
     sync_obj: DetectionTestingManagerOutputDto
     hec_token: str = ""
     hec_channel: str = ""
     _conn: client.Service = PrivateAttr()
     pbar: tqdm.tqdm = None
     start_time: float = None
@@ -235,14 +232,15 @@
                 pass
             except ConnectionResetError:
                 pass
             except Exception as e:
                 self.pbar.write(
                     f"Error getting API connection (not quitting) '{type(e).__name__}': {str(e)}"
                 )
+                print("wow")
                 # self.pbar.write(
                 #     f"Unhandled exception getting connection to splunk server: {str(e)}"
                 # )
                 # self.sync_obj.terminate = True
 
             for _ in range(sleep_seconds):
                 self.format_pbar_string(
@@ -393,15 +391,15 @@
                 #    f"No more detections to test, shutting down {self.get_name()}"
                 # )
                 self.finish()
                 return
             try:
                 self.test_detection(detection)
             except ContainerStoppedException:
-                self.pbar.write(f"Stopped container [{self.get_name()}]")
+                self.pbar.write(f"Warning - container was stopped when trying to execute detection [{self.get_name()}]")
                 self.finish()
                 return
             except Exception as e:
                 self.pbar.write(f"Error testing detection: {type(e).__name__}: {str(e)}")
                 raise e
             finally:
                 self.sync_obj.outputQueue.append(detection)
@@ -1192,22 +1190,20 @@
         attack_data_file: UnitTestAttackData,
         tmp_dir: str,
         test_group: TestGroup,
         test_group_start_time: float,
     ):
         tempfile = mktemp(dir=tmp_dir)
 
-        if not (
-            attack_data_file.data.startswith("https://")
-            or attack_data_file.data.startswith("http://")
-        ):
-            if pathlib.Path(attack_data_file.data).is_file():
+        if not (str(attack_data_file.data).startswith("http://") or 
+                str(attack_data_file.data).startswith("https://")) :
+            if pathlib.Path(str(attack_data_file.data)).is_file():
                 self.format_pbar_string(TestReportingType.GROUP, test_group.name, "Copying Data", test_group_start_time)
                 try:
-                    copyfile(attack_data_file.data, tempfile)
+                    copyfile(str(attack_data_file.data), tempfile)
                 except Exception as e:
                     raise Exception(
                         f"Error copying local Attack Data File for [{test_group.name}] - [{attack_data_file.data}]: "
                         f"{str(e)}"
                     )
             else:
                 raise Exception(
@@ -1225,29 +1221,23 @@
                     TestReportingType.GROUP,
                     test_group.name,
                     TestingStates.DOWNLOADING.value,
                     test_group_start_time
                 )
 
                 Utils.download_file_from_http(
-                    attack_data_file.data, tempfile, self.pbar, overwrite_file=True
+                    str(attack_data_file.data), tempfile, self.pbar, overwrite_file=True
                 )
             except Exception as e:
                 raise (
                     Exception(
                         f"Could not download attack data file [{attack_data_file.data}]:{str(e)}"
                     )
                 )
 
-        # Update timestamps before replay
-        if attack_data_file.update_timestamp:
-            data_manipulation = DataManipulation()
-            data_manipulation.manipulate_timestamp(
-                tempfile, attack_data_file.sourcetype, attack_data_file.source
-            )
 
         # Upload the data
         self.format_pbar_string(
             TestReportingType.GROUP,
             test_group.name,
             TestingStates.REPLAYING.value,
             test_group_start_time
@@ -1362,13 +1352,13 @@
             except Exception as e:
                 raise (Exception(f"There was an exception in the post: {str(e)}"))
 
     def status(self):
         pass
 
     def finish(self):
-        self.pbar.bar_format = f"Stopped container [{self.get_name()}]"
+        self.pbar.bar_format = f"Finished running tests on instance: [{self.get_name()}]"
         self.pbar.update()
         self.pbar.close()
 
     def check_health(self):
         pass
```

### Comparing `contentctl-3.6.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py` & `contentctl-4.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from contentctl.actions.detection_testing.infrastructures.DetectionTestingInfrastructure import (
     DetectionTestingInfrastructure,
 )
+from contentctl.objects.config import test
 import docker.models.resource
 import docker.models.containers
 import docker
 import docker.types
-from contentctl.objects.test_config import (
-    CONTAINER_APP_DIR,
-    LOCAL_APP_DIR,
-)
 
 
 class DetectionTestingInfrastructureContainer(DetectionTestingInfrastructure):
+    global_config: test
     container: docker.models.resource.Model = None
 
     def start(self):
-        if self.global_config.infrastructure_config.persist_and_reuse_container:
+        if self.global_config.container_settings.leave_running:
             # If we are configured to use the persistent container, then check and see if it's already
             # running. If so, just use it without additional configuration.
             try:
                 self.container = self.get_docker_client().containers.get(self.get_name())
                 return
             except Exception:
                 #We did not find the container running, we will set it up
@@ -72,64 +70,92 @@
             "8000/tcp": self.infrastructure.web_ui_port,
             "8088/tcp": self.infrastructure.hec_port,
             "8089/tcp": self.infrastructure.api_port,
         }
 
         mounts = [
             docker.types.Mount(
-                source=str(LOCAL_APP_DIR.absolute()),
-                target=str(CONTAINER_APP_DIR.absolute()),
+                source=str(self.global_config.getLocalAppDir()),
+                target=str(self.global_config.getContainerAppDir()),
                 type="bind",
                 read_only=True,
             )
         ]
 
         environment = {}
         environment["SPLUNK_START_ARGS"] = "--accept-license"
         environment["SPLUNK_PASSWORD"] = self.infrastructure.splunk_app_password
-        environment["SPLUNK_APPS_URL"] = ",".join(
-            p.environment_path for p in self.global_config.apps 
-        )
+        # Files have already been staged by the time that we call this. Files must only be staged
+        # once, not staged by every container
+        environment["SPLUNK_APPS_URL"] = self.global_config.getContainerEnvironmentString(stage_file=False)
         if (
-            self.global_config.splunkbase_password is not None
-            and self.global_config.splunkbase_username is not None
+            self.global_config.splunk_api_username is not None
+            and self.global_config.splunk_api_password is not None
         ):
-            environment["SPLUNKBASE_USERNAME"] = self.global_config.splunkbase_username
-            environment["SPLUNKBASE_PASSWORD"] = self.global_config.splunkbase_password
-
+            environment["SPLUNKBASE_USERNAME"] = self.global_config.splunk_api_username
+            environment["SPLUNKBASE_PASSWORD"] = self.global_config.splunk_api_password
+        
+
+
+        def emit_docker_run_equivalent():
+            environment_string = " ".join([f'-e "{k}={environment.get(k)}"' for k in environment.keys()])
+            print(f"\n\ndocker run -d "\
+                  f"-p {self.infrastructure.web_ui_port}:8000 "
+                  f"-p {self.infrastructure.hec_port}:8088 "
+                  f"-p {self.infrastructure.api_port}:8089 "
+                  f"{environment_string} "            
+                  f" --name {self.get_name()} "
+                  f"--platform linux/amd64 "
+                  f"{self.global_config.container_settings.full_image_path}\n\n")
+        #emit_docker_run_equivalent()
+        
         container = self.get_docker_client().containers.create(
-            self.global_config.infrastructure_config.full_image_path,
+            self.global_config.container_settings.full_image_path,
             ports=ports_dict,
             environment=environment,
             name=self.get_name(),
             mounts=mounts,
             detach=True,
             platform="linux/amd64"
         )
+        
+        if self.global_config.enterpriseSecurityInApps():
+            #ES sets up https, so make sure it is included in the link
+            address = f"https://{self.infrastructure.instance_address}:{self.infrastructure.web_ui_port}"
+        else:
+            address = f"http://{self.infrastructure.instance_address}:{self.infrastructure.web_ui_port}"
+        print(f"\nStarted container with the following information:\n"
+              f"\tname    : [{self.get_name()}]\n"
+              f"\taddress : [{address}]\n"
+              f"\tusername: [{self.infrastructure.splunk_app_username}]\n"
+              f"\tpassword: [{self.infrastructure.splunk_app_password}]\n"
+              )
 
         return container
 
     def removeContainer(self, removeVolumes: bool = True, forceRemove: bool = True):
         try:
             container: docker.models.containers.Container = (
                 self.get_docker_client().containers.get(self.get_name())
             )
         except Exception as e:
             # Container does not exist, no need to try and remove it
             return
         try:
             # If the user wants to persist the container (or use a previously configured container), then DO NOT remove it.
             # Emit the following message, which they will see on initial setup and teardown at the end of the test. 
-            if self.global_config.infrastructure_config.persist_and_reuse_container:
+            if self.global_config.container_settings.leave_running:
                 print(f"\nContainer [{self.get_name()}] has NOT been terminated because 'contentctl_test.yml ---> infrastructure_config ---> persist_and_reuse_container = True'")
                 print(f"To remove it, please manually run the following at the command line: `docker container rm -fv {self.get_name()}`\n")
                 return
             # container was found, so now we try to remove it
             # v also removes volumes linked to the container
             container.remove(v=removeVolumes, force=forceRemove)
+            print(f"container [{self.get_name()}] successfully removed")
+
             # remove it even if it is running. remove volumes as well
             # No need to print that the container has been removed, it is expected behavior
 
         except Exception as e:
             raise (
                 Exception(
                     f"Could not remove Docker Container [{self.get_name()}]: {str(e)}"
```

### Comparing `contentctl-3.6.0/contentctl/actions/detection_testing/progress_bar.py` & `contentctl-4.0.1/contentctl/actions/detection_testing/progress_bar.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingView.py` & `contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingView.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import abc
 import datetime
 
 from pydantic import BaseModel
 
-from contentctl.objects.test_config import TestConfig
+from contentctl.objects.config import test_common
+
 from contentctl.actions.detection_testing.infrastructures.DetectionTestingInfrastructure import (
     DetectionTestingManagerOutputDto,
 )
 from contentctl.helper.utils import Utils
 from contentctl.objects.enums import DetectionStatus
 
 
 class DetectionTestingView(BaseModel, abc.ABC):
-    config: TestConfig
+    config: test_common
     sync_obj: DetectionTestingManagerOutputDto
 
     interval: float = 10
     next_update: float = 0
 
     def setup(self):
         pass
```

### Comparing `contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py` & `contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py` & `contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/actions/doc_gen.py` & `contentctl-4.0.1/contentctl/actions/doc_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 @dataclass(frozen=True)
 class DocGenInputDto:
     director_input_dto: DirectorInputDto
 
 class DocGen:
 
     def execute(self, input_dto: DocGenInputDto) -> None:
-        director_output_dto = DirectorOutputDto([],[],[],[],[],[],[],[])
+        director_output_dto = DirectorOutputDto([],[],[],[],[],[],[],[],[],[])
         director = Director(director_output_dto)
         director.execute(input_dto.director_input_dto)
 
         doc_md_output = DocMdOutput()
         doc_md_output.writeObjects(
             [director_output_dto.stories, director_output_dto.detections, director_output_dto.playbooks], 
             os.path.join(input_dto.director_input_dto.input_path, "docs")
```

### Comparing `contentctl-3.6.0/contentctl/actions/generate.py` & `contentctl-4.0.1/contentctl/actions/build.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,89 @@
 import sys
 import shutil
 import os
 
 from dataclasses import dataclass
 
 from contentctl.objects.enums import SecurityContentProduct, SecurityContentType
-from contentctl.input.director import Director, DirectorInputDto, DirectorOutputDto
+from contentctl.input.director import Director, DirectorOutputDto
 from contentctl.output.conf_output import ConfOutput
+from contentctl.output.conf_writer import ConfWriter
 from contentctl.output.ba_yml_output import BAYmlOutput
 from contentctl.output.api_json_output import ApiJsonOutput
 import pathlib
 import json
 import datetime
 from typing import Union
 
+from contentctl.objects.config import build
+
 @dataclass(frozen=True)
-class GenerateInputDto:
-    director_input_dto: DirectorInputDto
-    splunk_api_username: Union[str,None] = None
-    splunk_api_password: Union[str,None] = None
-    #For most cloud stacks, the stack_type argument has been deprecated for appinspect.
-    #Still, we will pass it in case there are users of very old stacks.
-    stack_type: str = "victoria"
-
-class Generate:
-
-    def execute(self, input_dto: GenerateInputDto) -> DirectorOutputDto:
-        director_output_dto = DirectorOutputDto([],[],[],[],[],[],[],[],[])
-        director = Director(director_output_dto)
-        director.execute(input_dto.director_input_dto)
-
-        if input_dto.director_input_dto.product == SecurityContentProduct.SPLUNK_APP:
-            if (input_dto.splunk_api_username is None) ^ (input_dto.splunk_api_password is None):
-                # Exclusive OR above finds when ONE of these is defined but the other is not
-                if input_dto.splunk_api_password:
-                    raise Exception("splunk_api_password was provided, but splunk_api_username was not. Please provide both or neither")
-                else:
-                    raise Exception("splunk_api_username was provided, but splunk_api_password was not. Please provide both or neither")                
+class BuildInputDto:
+    director_output_dto: DirectorOutputDto
+    config:build
+
+
+class Build:
 
 
-            
-            
-            conf_output = ConfOutput(input_dto.director_input_dto.input_path, input_dto.director_input_dto.config)
-            conf_output.writeHeaders()
-            conf_output.writeObjects(director_output_dto.detections, SecurityContentType.detections)
-            conf_output.writeObjects(director_output_dto.stories, SecurityContentType.stories)
-            conf_output.writeObjects(director_output_dto.baselines, SecurityContentType.baselines)
-            conf_output.writeObjects(director_output_dto.investigations, SecurityContentType.investigations)
-            conf_output.writeObjects(director_output_dto.lookups, SecurityContentType.lookups)
-            conf_output.writeObjects(director_output_dto.macros, SecurityContentType.macros)
-            conf_output.writeAppConf()
-            conf_output.packageApp()
 
-            #conf_output.inspectAppCLI()
-            if input_dto.splunk_api_username and input_dto.splunk_api_password:
-                _ = conf_output.inspectAppAPI(input_dto.splunk_api_username, input_dto.splunk_api_password, input_dto.stack_type)
+    def execute(self, input_dto: BuildInputDto) -> DirectorOutputDto:
+        if input_dto.config.build_app:    
+            updated_conf_files:set[pathlib.Path] = set()
+            conf_output = ConfOutput(input_dto.config)
+            updated_conf_files.update(conf_output.writeHeaders())
+            updated_conf_files.update(conf_output.writeObjects(input_dto.director_output_dto.detections, SecurityContentType.detections))
+            updated_conf_files.update(conf_output.writeObjects(input_dto.director_output_dto.stories, SecurityContentType.stories))
+            updated_conf_files.update(conf_output.writeObjects(input_dto.director_output_dto.baselines, SecurityContentType.baselines))
+            updated_conf_files.update(conf_output.writeObjects(input_dto.director_output_dto.investigations, SecurityContentType.investigations))
+            updated_conf_files.update(conf_output.writeObjects(input_dto.director_output_dto.lookups, SecurityContentType.lookups))
+            updated_conf_files.update(conf_output.writeObjects(input_dto.director_output_dto.macros, SecurityContentType.macros))
+            updated_conf_files.update(conf_output.writeAppConf())
+            
+            #Ensure that the conf file we just generated/update is syntactically valid
+            for conf_file in updated_conf_files:
+                ConfWriter.validateConfFile(conf_file) 
                 
-            print(f'Generate of security content successful to {conf_output.output_path}')
-            return director_output_dto
+            conf_output.packageApp()
 
-        elif input_dto.director_input_dto.product == SecurityContentProduct.SSA:
-            output_path = os.path.join(input_dto.director_input_dto.input_path, input_dto.director_input_dto.config.build_ssa.path_root)
-            shutil.rmtree(output_path + '/srs/', ignore_errors=True)
-            shutil.rmtree(output_path + '/complex/', ignore_errors=True)
-            os.makedirs(output_path + '/complex/')
-            os.makedirs(output_path + '/srs/')     
-            ba_yml_output = BAYmlOutput()
-            ba_yml_output.writeObjects(director_output_dto.ssa_detections, output_path)
+            print(f"Build of '{input_dto.config.app.title}' APP successful to {input_dto.config.getPackageFilePath()}")
+        
 
-        elif input_dto.director_input_dto.product == SecurityContentProduct.API:
-            output_path = os.path.join(input_dto.director_input_dto.input_path, input_dto.director_input_dto.config.build_api.path_root)
-            shutil.rmtree(output_path, ignore_errors=True)
-            os.makedirs(output_path)
+        if input_dto.config.build_api:    
+            shutil.rmtree(input_dto.config.getAPIPath(), ignore_errors=True)
+            input_dto.config.getAPIPath().mkdir(parents=True)
             api_json_output = ApiJsonOutput()
-            api_json_output.writeObjects(director_output_dto.detections, output_path, SecurityContentType.detections)
-            api_json_output.writeObjects(director_output_dto.stories, output_path, SecurityContentType.stories)
-            api_json_output.writeObjects(director_output_dto.baselines, output_path, SecurityContentType.baselines)
-            api_json_output.writeObjects(director_output_dto.investigations, output_path, SecurityContentType.investigations)
-            api_json_output.writeObjects(director_output_dto.lookups, output_path, SecurityContentType.lookups)
-            api_json_output.writeObjects(director_output_dto.macros, output_path, SecurityContentType.macros)
-            api_json_output.writeObjects(director_output_dto.deployments, output_path, SecurityContentType.deployments)
- 
+            for output_objects, output_type in [(input_dto.director_output_dto.detections, SecurityContentType.detections),
+                                                (input_dto.director_output_dto.stories, SecurityContentType.stories),
+                                                (input_dto.director_output_dto.baselines, SecurityContentType.baselines),
+                                                (input_dto.director_output_dto.investigations, SecurityContentType.investigations),
+                                                (input_dto.director_output_dto.lookups, SecurityContentType.lookups),
+                                                (input_dto.director_output_dto.macros, SecurityContentType.macros),
+                                                (input_dto.director_output_dto.deployments, SecurityContentType.deployments)]:
+                api_json_output.writeObjects(output_objects, input_dto.config.getAPIPath(), input_dto.config.app.label, output_type )
+            
+           
+            
             #create version file for sse api
-            version_file = pathlib.Path(output_path)/"version.json"
-            utc_time = datetime.datetime.utcnow().replace(microsecond=0).isoformat()
-            version_dict = {"version":{"name":f"v{input_dto.director_input_dto.config.build.version}","published_at": f"{utc_time}Z"  }}
+            version_file = input_dto.config.getAPIPath()/"version.json"
+            utc_time = datetime.datetime.now(datetime.timezone.utc).replace(microsecond=0,tzinfo=None).isoformat()
+            version_dict = {"version":{"name":f"v{input_dto.config.app.version}","published_at": f"{utc_time}Z"  }}
             with open(version_file,"w") as version_f:
                 json.dump(version_dict,version_f)
+            
+            print(f"Build of '{input_dto.config.app.title}' API successful to {input_dto.config.getAPIPath()}")
+
+        if input_dto.config.build_ssa:
+            
+            srs_path = input_dto.config.getSSAPath() / 'srs'
+            complex_path = input_dto.config.getSSAPath() / 'complex'
+            shutil.rmtree(srs_path, ignore_errors=True)
+            shutil.rmtree(complex_path, ignore_errors=True)
+            srs_path.mkdir(parents=True)
+            complex_path.mkdir(parents=True)
+            ba_yml_output = BAYmlOutput()
+            ba_yml_output.writeObjects(input_dto.director_output_dto.ssa_detections, str(input_dto.config.getSSAPath()))
+
+            print(f"Build of 'SSA' successful to {input_dto.config.getSSAPath()}")
                 
-        return director_output_dto
+        return input_dto.director_output_dto
```

### Comparing `contentctl-3.6.0/contentctl/actions/initialize_old.py` & `contentctl-4.0.1/contentctl/actions/initialize_old.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/enrichments/attack_enrichment.py` & `contentctl-4.0.1/contentctl/enrichments/attack_enrichment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,111 @@
 
+from __future__ import annotations
 import csv
 import os
 from posixpath import split
 from typing import Optional
 import sys
 from attackcti import attack_client
 import logging
+from pydantic import BaseModel, Field
+from dataclasses import field
+from typing import Union,Annotated
+from contentctl.objects.mitre_attack_enrichment import MitreAttackEnrichment
+from contentctl.objects.config import validate
 logging.getLogger('taxii2client').setLevel(logging.CRITICAL)
 
 
-class AttackEnrichment():
-
-    @classmethod
-    def get_attack_lookup(self, input_path: str, store_csv = False, force_cached_or_offline: bool = False, skip_enrichment:bool = False) -> dict:
+class AttackEnrichment(BaseModel):
+    data: dict[str, MitreAttackEnrichment] = field(default_factory=dict)
+    use_enrichment:bool = True
+    
+    @staticmethod
+    def getAttackEnrichment(config:validate)->AttackEnrichment:
+        enrichment = AttackEnrichment(use_enrichment=config.enrichments)
+        _ = enrichment.get_attack_lookup(str(config.path))
+        return enrichment
+    
+    def getEnrichmentByMitreID(self, mitre_id:Annotated[str, Field(pattern="^T\d{4}(.\d{3})?$")])->Union[MitreAttackEnrichment,None]:
+        if not self.use_enrichment:
+            return None
+        
+        enrichment = self.data.get(mitre_id, None)
+        if enrichment is not None:
+            return enrichment
+        else:
+            raise ValueError(f"Error, Unable to find Mitre Enrichment for MitreID {mitre_id}")
+        
+
+    def addMitreID(self, technique:dict, tactics:list[str], groups:list[str])->None:
+        
+        technique_id = technique['technique_id']
+        technique_obj = technique['technique']
+        tactics.sort()
+        groups.sort()
+
+        if technique_id in self.data:
+            raise ValueError(f"Error, trying to redefine MITRE ID '{technique_id}'")
+        
+        self.data[technique_id] = MitreAttackEnrichment(mitre_attack_id=technique_id, 
+                                                        mitre_attack_technique=technique_obj, 
+                                                        mitre_attack_tactics=tactics, 
+                                                        mitre_attack_groups=groups)
+
+    
+    def get_attack_lookup(self, input_path: str, store_csv: bool = False, force_cached_or_offline: bool = False, skip_enrichment:bool = False) -> dict:
+        if self.use_enrichment is False:
+            return {}
         print("Getting MITRE Attack Enrichment Data. This may take some time...")
         attack_lookup = dict()
-        file_path = os.path.join(input_path, "lookups", "mitre_enrichment.csv")
+        file_path = os.path.join(input_path, "app_template", "lookups", "mitre_enrichment.csv")
 
         if skip_enrichment is True:
             print("Skipping enrichment")
             return attack_lookup
         try:
 
             if force_cached_or_offline is True:
                 raise(Exception("WARNING - Using cached MITRE Attack Enrichment.  Attack Enrichment may be out of date. Only use this setting for offline environments and development purposes."))
             print(f"\r{'Client'.rjust(23)}: [{0:3.0f}%]...", end="", flush=True)
             lift = attack_client()
             print(f"\r{'Client'.rjust(23)}: [{100:3.0f}%]...Done!", end="\n", flush=True)
             
-            print(f"\r{'Enterprise'.rjust(23)}: [{0.0:3.0f}%]...", end="", flush=True)
-            all_enterprise = lift.get_enterprise(stix_format=False)
-            print(f"\r{'Enterprise'.rjust(23)}: [{100:3.0f}%]...Done!", end="\n", flush=True)
+            print(f"\r{'Techniques'.rjust(23)}: [{0.0:3.0f}%]...", end="", flush=True)
+            all_enterprise_techniques = lift.get_enterprise_techniques(stix_format=False)
+            
+            print(f"\r{'Techniques'.rjust(23)}: [{100:3.0f}%]...Done!", end="\n", flush=True)
             
             print(f"\r{'Relationships'.rjust(23)}: [{0.0:3.0f}%]...", end="", flush=True)
-            enterprise_relationships = lift.get_enterprise_relationships()
+            enterprise_relationships = lift.get_enterprise_relationships(stix_format=False)
             print(f"\r{'Relationships'.rjust(23)}: [{100:3.0f}%]...Done!", end="\n", flush=True)
             
             print(f"\r{'Groups'.rjust(23)}: [{0:3.0f}%]...", end="", flush=True)
-            enterprise_groups = lift.get_enterprise_groups()
+            enterprise_groups = lift.get_enterprise_groups(stix_format=False)
             print(f"\r{'Groups'.rjust(23)}: [{100:3.0f}%]...Done!", end="\n", flush=True)
             
-            for index, technique in enumerate(all_enterprise['techniques']):
-                progress_percent = ((index+1)/len(all_enterprise['techniques'])) * 100
+            
+            for index, technique in enumerate(all_enterprise_techniques):
+                progress_percent = ((index+1)/len(all_enterprise_techniques)) * 100
                 if (sys.stdout.isatty() and sys.stdin.isatty() and sys.stderr.isatty()):
                     print(f"\r\t{'MITRE Technique Progress'.rjust(23)}: [{progress_percent:3.0f}%]...", end="", flush=True)
                 apt_groups = []
                 for relationship in enterprise_relationships:
-                    if (relationship['target_ref'] == technique['id']) and relationship['source_ref'].startswith('intrusion-set'):
+                    if (relationship['target_object'] == technique['id']) and relationship['source_object'].startswith('intrusion-set'):
                         for group in enterprise_groups:
-                            if relationship['source_ref'] == group['id']:
-                                apt_groups.append(group['name'])
+                            if relationship['source_object'] == group['id']:
+                                apt_groups.append(group['group'])
 
                 tactics = []
                 if ('tactic' in technique):
                     for tactic in technique['tactic']:
                         tactics.append(tactic.replace('-',' ').title())
 
-                if not ('revoked' in technique):
-                    attack_lookup[technique['technique_id']] = {'technique': technique['technique'], 'tactics': tactics, 'groups': apt_groups}
+                self.addMitreID(technique, tactics, apt_groups)
+                attack_lookup[technique['technique_id']] = {'technique': technique['technique'], 'tactics': tactics, 'groups': apt_groups}
 
             if store_csv:
                 f = open(file_path, 'w')
                 writer = csv.writer(f)
                 writer.writerow(['mitre_id', 'technique', 'tactics' ,'groups'])
                 for key in attack_lookup.keys():
                     if len(attack_lookup[key]['groups']) == 0:
@@ -75,17 +119,23 @@
                         '|'.join(attack_lookup[key]['tactics']),
                         groups
                     ])
                 
                 f.close()
 
         except Exception as err:
-            print('Warning: ' + str(err))
-            print('Use local copy lookups/mitre_enrichment.csv')
-            dict_from_csv = {}
+            print(f'\nError: {str(err)}')
+            print('Use local copy app_template/lookups/mitre_enrichment.csv')
             with open(file_path, mode='r') as inp:
                 reader = csv.reader(inp)
                 attack_lookup = {rows[0]:{'technique': rows[1], 'tactics': rows[2].split('|'), 'groups': rows[3].split('|')} for rows in reader}
             attack_lookup.pop('mitre_id')
+            for key in attack_lookup.keys():
+                technique_input = {'technique_id': key , 'technique': attack_lookup[key]['technique'] }
+                tactics_input = attack_lookup[key]['tactics']
+                groups_input = attack_lookup[key]['groups']
+                self.addMitreID(technique=technique_input, tactics=tactics_input, groups=groups_input)
+            
+                
 
         print("Done!")
         return attack_lookup
```

### Comparing `contentctl-3.6.0/contentctl/enrichments/cve_enrichment.py` & `contentctl-4.0.1/contentctl/enrichments/cve_enrichment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-
+from __future__ import annotations
 from pycvesearch import CVESearch
 import functools
 import os
 import shelve
 import time
-import sys
+from typing import Annotated
+from pydantic import BaseModel,Field,ConfigDict
+
+from decimal import Decimal
 CVESSEARCH_API_URL = 'https://cve.circl.lu'
 
 CVE_CACHE_FILENAME = "lookups/CVE_CACHE.db"
 
 NON_PERSISTENT_CACHE = {}
 
 
-
+''''''
 @functools.cache
 def cvesearch_helper(url:str, cve_id:str, force_cached_or_offline:bool=False, max_api_attempts:int=3, retry_sleep_seconds:int=5):
     if max_api_attempts < 1:
             raise(Exception(f"The minimum number of CVESearch API attempts is 1.  You have passed {max_api_attempts}"))
 
     if force_cached_or_offline:
         if not os.path.exists(CVE_CACHE_FILENAME):
@@ -59,27 +62,39 @@
     #The initial CVESearch call takes some time.
     #We cache it to avoid making this call each time we need to do a lookup
     cve = CVESearch(CVESSEARCH_API_URL)
     return cve
 
 
 
-class CveEnrichment():
 
+class CveEnrichmentObj(BaseModel):
+    id:Annotated[str, "^CVE-[1|2][0-9]{3}-[0-9]+$"]
+    cvss:Annotated[Decimal, Field(ge=.1, le=10, decimal_places=1)]
+    summary:str
+
+
+    @staticmethod
+    def buildEnrichmentOnFailure(id:Annotated[str, "^CVE-[1|2][0-9]{3}-[0-9]+$"], errorMessage:str)->CveEnrichmentObj:
+        message = f"{errorMessage}. Default CVSS of 5.0 used"
+        print(message)
+        return CveEnrichmentObj(id=id, cvss=Decimal(5.0), summary=message)
+
+class CveEnrichment():
     @classmethod
-    def enrich_cve(self, cve_id: str, force_cached_or_offline: bool = False) -> dict:
+    def enrich_cve(cls, cve_id: str, force_cached_or_offline: bool = False, treat_failures_as_warnings:bool=True) -> CveEnrichmentObj:
         cve_enriched = dict()
         try:
             
             result = cvesearch_helper(CVESSEARCH_API_URL, cve_id, force_cached_or_offline)
             cve_enriched['id'] = cve_id
             cve_enriched['cvss'] = result['cvss']
             cve_enriched['summary'] = result['summary']
-        except TypeError as TypeErr:
-            # there was a error calling the circl api lets just empty the object
-            print("WARNING, issue enriching {0}, with error: {1}".format(cve_id, str(TypeErr)))
-            cve_enriched = dict()
-            
         except Exception as e:
-            print("WARNING - {0}".format(str(e)))
-    
-        return cve_enriched
+            message = f"issue enriching {cve_id}, with error: {str(e)}"
+            if treat_failures_as_warnings: 
+                return CveEnrichmentObj.buildEnrichmentOnFailure(id = cve_id, errorMessage=f"WARNING, {message}")
+            else:
+                raise ValueError(f"ERROR, {message}")
+        
+        return CveEnrichmentObj.model_validate(cve_enriched)
+
```

### Comparing `contentctl-3.6.0/contentctl/enrichments/splunk_app_enrichment.py` & `contentctl-4.0.1/contentctl/enrichments/splunk_app_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/helper/link_validator.py` & `contentctl-4.0.1/contentctl/helper/link_validator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-import re
-from tracemalloc import start
-from unittest.mock import DEFAULT
-from pydantic import BaseModel, validator, root_validator,Field
-from typing import Union, Callable
+from pydantic import BaseModel, model_validator
+from typing import Union, Callable, Any
 import requests
 import urllib3, urllib3.exceptions
 import time
 import abc
 
 import os
 import shelve
 
 DEFAULT_USER_AGENT_STRING = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.4951.41 Safari/537.36"
 ALLOWED_HTTP_CODES = [200]
 class LinkStats(BaseModel):
+
     #Static Values
     method: Callable = requests.get
     allowed_http_codes: list[int] = ALLOWED_HTTP_CODES 
     access_count: int = 1 #when constructor is called, it has been accessed once!
     timeout_seconds: int = 15
     allow_redirects: bool = True
     headers: dict = {"User-Agent": DEFAULT_USER_AGENT_STRING}
@@ -38,56 +36,56 @@
     
     
     def is_link_valid(self, referencing_file:str)->bool:
         self.access_count += 1
         self.referencing_files.add(referencing_file)
         return self.valid
     
-    @root_validator
-    def check_reference(cls, values):
+    @model_validator(mode="before")
+    def check_reference(cls, data:Any)->Any:
         start_time = time.time()
         #Get out all the fields names to make them easier to reference
-        method = values['method']
-        reference = values['reference']
-        timeout_seconds = values['timeout_seconds']
-        headers = values['headers']
-        allow_redirects = values['allow_redirects']
-        verify_ssl = values['verify_ssl']
-        allowed_http_codes = values['allowed_http_codes']
+        method = data['method']
+        reference = data['reference']
+        timeout_seconds = data['timeout_seconds']
+        headers = data['headers']
+        allow_redirects = data['allow_redirects']
+        verify_ssl = data['verify_ssl']
+        allowed_http_codes = data['allowed_http_codes']
         if not (reference.startswith("http://") or reference.startswith("https://")):
             raise(ValueError(f"Reference {reference} does not begin with http(s). Only http(s) references are supported"))
         
         try:
             get = method(reference, timeout=timeout_seconds, 
                             headers = headers, 
                             allow_redirects=allow_redirects, verify=verify_ssl)
             resolution_time = time.time() - start_time
-            values['status_code'] = get.status_code
-            values['resolution_time'] = resolution_time
+            data['status_code'] = get.status_code
+            data['resolution_time'] = resolution_time
             if reference != get.url:
-                values['redirect'] = get.url
+                data['redirect'] = get.url
             else:
-                values['redirect'] = None #None is also already the default
+                data['redirect'] = None #None is also already the default
 
             #Returns the updated values and sets them for the object
             if get.status_code in allowed_http_codes:
-                values['valid'] = True
+                data['valid'] = True
             else:
                 #print(f"Unacceptable HTTP Status Code {get.status_code} received for {reference}")
-                values['valid'] = False
-            return values    
+                data['valid'] = False
+            return data    
 
         except Exception as e:
             resolution_time = time.time() - start_time
             #print(f"Reference {reference} was not reachable after {resolution_time:.2f} seconds")
-            values['status_code'] = 0
-            values['valid'] = False
-            values['redirect'] = None
-            values['resolution_time'] = resolution_time
-            return values
+            data['status_code'] = 0
+            data['valid'] = False
+            data['redirect'] = None
+            data['resolution_time'] = resolution_time
+            return data
 
 
 class LinkValidator(abc.ABC):
     cache: Union[dict[str,LinkStats], shelve.Shelf] = {}
     uncached_checks: int = 0
     total_checks: int = 0
     #cache: dict[str,LinkStats] = {}
```

### Comparing `contentctl-3.6.0/contentctl/helper/utils.py` & `contentctl-4.0.1/contentctl/helper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 import git
 import shutil
 import requests
 import random
 import string
 from timeit import default_timer
 import pathlib
-import datetime
+
 from typing import Union, Tuple
-from pydantic import ValidationError
 import tqdm
-from contentctl.objects.security_content_object import SecurityContentObject
 from math import ceil
 
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from contentctl.objects.security_content_object import SecurityContentObject
+from contentctl.objects.security_content_object import SecurityContentObject
+
+
 TOTAL_BYTES = 0
 ALWAYS_PULL = True
 
 
 class Utils:
     @staticmethod
     def get_all_yml_files_from_directory(path: str) -> list[pathlib.Path]:
```

### Comparing `contentctl-3.6.0/contentctl/input/backend_splunk_ba.py` & `contentctl-4.0.1/contentctl/input/backend_splunk_ba.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/input/director.py` & `contentctl-4.0.1/contentctl/input/director.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,295 +1,233 @@
 import os
 import sys
-import pathlib
-from dataclasses import dataclass
+from typing import Union
+from dataclasses import dataclass, field
 from pydantic import ValidationError
-
-
-
+from uuid import UUID
+from contentctl.input.yml_reader import YmlReader
+    
+    
+    
 from contentctl.objects.detection import Detection
 from contentctl.objects.story import Story
+
+from contentctl.objects.enums import SecurityContentProduct
 from contentctl.objects.baseline import Baseline
 from contentctl.objects.investigation import Investigation
 from contentctl.objects.playbook import Playbook
 from contentctl.objects.deployment import Deployment
 from contentctl.objects.macro import Macro
 from contentctl.objects.lookup import Lookup
 from contentctl.objects.ssa_detection import SSADetection
+from contentctl.objects.atomic import AtomicTest
+from contentctl.objects.security_content_object import SecurityContentObject
 
-from contentctl.input.basic_builder import BasicBuilder
-from contentctl.input.detection_builder import DetectionBuilder
-from contentctl.input.ssa_detection_builder import SSADetectionBuilder
-from contentctl.input.playbook_builder import PlaybookBuilder
-from contentctl.input.baseline_builder import BaselineBuilder
-from contentctl.input.investigation_builder import InvestigationBuilder
-from contentctl.input.story_builder import StoryBuilder
-from contentctl.objects.enums import SecurityContentType
-from contentctl.objects.enums import SecurityContentProduct
-from contentctl.objects.enums import DetectionStatus 
-from contentctl.helper.utils import Utils
 from contentctl.enrichments.attack_enrichment import AttackEnrichment
-from contentctl.objects.config import Config
+from contentctl.enrichments.cve_enrichment import CveEnrichment
 
-from contentctl.objects.config import Config
+from contentctl.objects.config import validate
 
 
 
-@dataclass(frozen=True)
-class DirectorInputDto:
-    input_path: pathlib.Path
-    product: SecurityContentProduct
-    config: Config
-
-
 @dataclass()
 class DirectorOutputDto:
+     # Atomic Tests are first because parsing them 
+     # is far quicker than attack_enrichment
+     atomic_tests: Union[list[AtomicTest],None]
+     attack_enrichment: AttackEnrichment
      detections: list[Detection]
      stories: list[Story]
      baselines: list[Baseline]
      investigations: list[Investigation]
      playbooks: list[Playbook]
      macros: list[Macro]
      lookups: list[Lookup]
      deployments: list[Deployment]
      ssa_detections: list[SSADetection]
+     #cve_enrichment: CveEnrichment
+
+     name_to_content_map: dict[str, SecurityContentObject] = field(default_factory=dict)
+     uuid_to_content_map: dict[UUID, SecurityContentObject] = field(default_factory=dict)
+     
+
+
+
+
+from contentctl.input.ssa_detection_builder import SSADetectionBuilder
+from contentctl.objects.enums import SecurityContentType
+
+from contentctl.objects.enums import DetectionStatus 
+from contentctl.helper.utils import Utils
+
+
+
+
+
+
+     
 
 
 class Director():
-    input_dto: DirectorInputDto
+    input_dto: validate
     output_dto: DirectorOutputDto
-    basic_builder: BasicBuilder
-    playbook_builder: PlaybookBuilder
-    baseline_builder: BaselineBuilder
-    investigation_builder: InvestigationBuilder
-    story_builder: StoryBuilder
-    detection_builder: DetectionBuilder
     ssa_detection_builder: SSADetectionBuilder
-    attack_enrichment: dict
-    config: Config
+    
 
 
     def __init__(self, output_dto: DirectorOutputDto) -> None:
         self.output_dto = output_dto
-        self.attack_enrichment = dict()
-
-
-    def execute(self, input_dto: DirectorInputDto) -> None:
-        self.input_dto = input_dto
+        self.ssa_detection_builder = SSADetectionBuilder()
+    
+    def addContentToDictMappings(self, content:SecurityContentObject):
+         content_name = content.name
+         if isinstance(content,SSADetection):
+            # Since SSA detections may have the same name as ESCU detection,
+            # for this function we prepend 'SSA ' to the name.
+            content_name = f"SSA {content_name}"               
+         if content_name in self.output_dto.name_to_content_map:
+            raise ValueError(f"Duplicate name '{content_name}' with paths:\n"
+                             f" - {content.file_path}\n"
+                             f" - {self.output_dto.name_to_content_map[content_name].file_path}")
+         elif content.id in self.output_dto.uuid_to_content_map:
+            raise ValueError(f"Duplicate id '{content.id}' with paths:\n"
+                    f" - {content.file_path}\n"
+                    f" - {self.output_dto.name_to_content_map[content_name].file_path}")
+         
+         self.output_dto.name_to_content_map[content_name] = content 
+         self.output_dto.uuid_to_content_map[content.id] = content 
+    
         
-        if self.input_dto.config.enrichments.attack_enrichment:
-            self.attack_enrichment = AttackEnrichment.get_attack_lookup(self.input_dto.input_path)
+    
+    def execute(self, input_dto: validate) -> None:
+        self.input_dto = input_dto
+
         
-        self.basic_builder = BasicBuilder()
-        self.playbook_builder = PlaybookBuilder(self.input_dto.input_path)
-        self.baseline_builder = BaselineBuilder()
-        self.investigation_builder = InvestigationBuilder()
-        self.story_builder = StoryBuilder()
-        self.detection_builder = DetectionBuilder()
-        self.ssa_detection_builder = SSADetectionBuilder()
-        if self.input_dto.product == SecurityContentProduct.SPLUNK_APP or self.input_dto.product == SecurityContentProduct.API:
-            self.createSecurityContent(SecurityContentType.deployments)
-            self.createSecurityContent(SecurityContentType.lookups)
-            self.createSecurityContent(SecurityContentType.macros)
-            self.createSecurityContent(SecurityContentType.baselines)
-            self.createSecurityContent(SecurityContentType.investigations)
-            self.createSecurityContent(SecurityContentType.playbooks)
-            self.createSecurityContent(SecurityContentType.detections)
-            self.createSecurityContent(SecurityContentType.stories)
-        elif self.input_dto.product == SecurityContentProduct.SSA:
-            self.createSecurityContent(SecurityContentType.ssa_detections)
+        self.createSecurityContent(SecurityContentType.deployments)
+        self.createSecurityContent(SecurityContentType.lookups)
+        self.createSecurityContent(SecurityContentType.macros)
+        self.createSecurityContent(SecurityContentType.stories)
+        self.createSecurityContent(SecurityContentType.baselines)
+        self.createSecurityContent(SecurityContentType.investigations)
+        self.createSecurityContent(SecurityContentType.playbooks)
+        self.createSecurityContent(SecurityContentType.detections)
+
+
+        self.createSecurityContent(SecurityContentType.ssa_detections)
         
 
-    def createSecurityContent(self, type: SecurityContentType) -> None:
-        if type == SecurityContentType.ssa_detections:
-            files = Utils.get_all_yml_files_from_directory(os.path.join(self.input_dto.input_path, 'ssa_detections'))
-        elif type == SecurityContentType.unit_tests:
-            files = Utils.get_all_yml_files_from_directory(os.path.join(self.input_dto.input_path, 'tests'))
+    def createSecurityContent(self, contentType: SecurityContentType) -> None:
+        if contentType == SecurityContentType.ssa_detections:
+            files = Utils.get_all_yml_files_from_directory(os.path.join(self.input_dto.path, 'ssa_detections'))
+            security_content_files = [f for f in files if f.name.startswith('ssa___')]
+            
+        elif contentType in [SecurityContentType.deployments, 
+                             SecurityContentType.lookups, 
+                             SecurityContentType.macros, 
+                             SecurityContentType.stories,
+                             SecurityContentType.baselines,
+                             SecurityContentType.investigations,
+                             SecurityContentType.playbooks,
+                             SecurityContentType.detections]:
+            files = Utils.get_all_yml_files_from_directory(os.path.join(self.input_dto.path, str(contentType.name)))
+            security_content_files = [f for f in files if not f.name.startswith('ssa___')]
         else:
-            files = Utils.get_all_yml_files_from_directory(os.path.join(self.input_dto.input_path, str(type.name)))
+             raise(Exception(f"Cannot createSecurityContent for unknown product."))
 
         validation_errors = []
                 
         already_ran = False
         progress_percent = 0
-
-        if self.input_dto.product == SecurityContentProduct.SPLUNK_APP or self.input_dto.product == SecurityContentProduct.API:
-            security_content_files = [f for f in files if not f.name.startswith('ssa___')]
-        elif self.input_dto.product == SecurityContentProduct.SSA:
-            security_content_files = [f for f in files if f.name.startswith('ssa___')]
-        else:
-            raise(Exception(f"Cannot createSecurityContent for unknown product '{self.input_dto.product}'"))
-
         
         for index,file in enumerate(security_content_files):
             progress_percent = ((index+1)/len(security_content_files)) * 100
             try:
-                type_string = type.name.upper()
-                if type == SecurityContentType.lookups:
-                        self.constructLookup(self.basic_builder, file)
-                        lookup = self.basic_builder.getObject()
+                type_string = contentType.name.upper()
+                modelDict = YmlReader.load_file(file)
+
+                if contentType == SecurityContentType.lookups:
+                        lookup = Lookup.model_validate(modelDict,context={"output_dto":self.output_dto, "config":self.input_dto})
                         self.output_dto.lookups.append(lookup)
+                        self.addContentToDictMappings(lookup)
                 
-                elif type == SecurityContentType.macros:
-                        self.constructMacro(self.basic_builder, file)
-                        macro = self.basic_builder.getObject()
+                elif contentType == SecurityContentType.macros:
+                        macro = Macro.model_validate(modelDict,context={"output_dto":self.output_dto})
                         self.output_dto.macros.append(macro)
+                        self.addContentToDictMappings(macro)
                 
-                elif type == SecurityContentType.deployments:
-                        self.constructDeployment(self.basic_builder, file)
-                        deployment = self.basic_builder.getObject()
+                elif contentType == SecurityContentType.deployments:
+                        deployment = Deployment.model_validate(modelDict,context={"output_dto":self.output_dto})
                         self.output_dto.deployments.append(deployment)
+                        self.addContentToDictMappings(deployment)
                 
-                elif type == SecurityContentType.playbooks:
-                        self.constructPlaybook(self.playbook_builder, file)
-                        playbook = self.playbook_builder.getObject()
-                        self.output_dto.playbooks.append(playbook)                    
+                elif contentType == SecurityContentType.playbooks:
+                        playbook = Playbook.model_validate(modelDict,context={"output_dto":self.output_dto})
+                        self.output_dto.playbooks.append(playbook)  
+                        self.addContentToDictMappings(playbook)                  
                 
-                elif type == SecurityContentType.baselines:
-                        self.constructBaseline(self.baseline_builder, file)
-                        baseline = self.baseline_builder.getObject()
+                elif contentType == SecurityContentType.baselines:
+                        baseline = Baseline.model_validate(modelDict,context={"output_dto":self.output_dto})
                         self.output_dto.baselines.append(baseline)
+                        self.addContentToDictMappings(baseline)
                 
-                elif type == SecurityContentType.investigations:
-                        self.constructInvestigation(self.investigation_builder, file)
-                        investigation = self.investigation_builder.getObject()
+                elif contentType == SecurityContentType.investigations:
+                        investigation = Investigation.model_validate(modelDict,context={"output_dto":self.output_dto})
                         self.output_dto.investigations.append(investigation)
+                        self.addContentToDictMappings(investigation)
 
-                elif type == SecurityContentType.stories:
-                        self.constructStory(self.story_builder, file)
-                        story = self.story_builder.getObject()
+                elif contentType == SecurityContentType.stories:
+                        story = Story.model_validate(modelDict,context={"output_dto":self.output_dto})
                         self.output_dto.stories.append(story)
+                        self.addContentToDictMappings(story)
             
-                elif type == SecurityContentType.detections:
-                        self.constructDetection(self.detection_builder, file)
-                        detection = self.detection_builder.getObject()
+                elif contentType == SecurityContentType.detections:
+                        detection = Detection.model_validate(modelDict,context={"output_dto":self.output_dto})
                         self.output_dto.detections.append(detection)
+                        self.addContentToDictMappings(detection)
 
-                elif type == SecurityContentType.ssa_detections:
-                        self.constructSSADetection(self.ssa_detection_builder, file)
-                        detection = self.ssa_detection_builder.getObject()
-                        if detection.status in  [DetectionStatus.production.value, DetectionStatus.validation.value]:
-                            self.output_dto.ssa_detections.append(detection)
+                elif contentType == SecurityContentType.ssa_detections:
+                        self.constructSSADetection(self.ssa_detection_builder, self.output_dto,str(file))
+                        ssa_detection = self.ssa_detection_builder.getObject()
+                        if ssa_detection.status in [DetectionStatus.production.value, DetectionStatus.validation.value]:
+                            self.output_dto.ssa_detections.append(ssa_detection)
+                            self.addContentToDictMappings(ssa_detection)
 
                 else:
-                        raise Exception(f"Unsupported type: [{type}]")
+                        raise Exception(f"Unsupported type: [{contentType}]")
                 
                 if (sys.stdout.isatty() and sys.stdin.isatty() and sys.stderr.isatty()) or not already_ran:
                         already_ran = True
                         print(f"\r{f'{type_string} Progress'.rjust(23)}: [{progress_percent:3.0f}%]...", end="", flush=True)
             
             except (ValidationError, ValueError) as e:
-                relative_path = file.absolute().relative_to(self.input_dto.input_path.absolute())
+                relative_path = file.absolute().relative_to(self.input_dto.path.absolute())
                 validation_errors.append((relative_path,e))
+                
 
-        print(f"\r{f'{type.name.upper()} Progress'.rjust(23)}: [{progress_percent:3.0f}%]...", end="", flush=True)
+        print(f"\r{f'{contentType.name.upper()} Progress'.rjust(23)}: [{progress_percent:3.0f}%]...", end="", flush=True)
         print("Done!")
 
         if len(validation_errors) > 0:
-            errors_string = '\n\n'.join([f"{e_tuple[0]}\n{str(e_tuple[1])}" for e_tuple in validation_errors])
+            errors_string = '\n\n'.join([f"File: {e_tuple[0]}\nError: {str(e_tuple[1])}" for e_tuple in validation_errors])
+            #print(f"The following {len(validation_errors)} error(s) were found during validation:\n\n{errors_string}\n\nVALIDATION FAILED")
+            # We quit after validation a single type/group of content because it can cause significant cascading errors in subsequent
+            # types of content (since they may import or otherwise use it)
             raise Exception(f"The following {len(validation_errors)} error(s) were found during validation:\n\n{errors_string}\n\nVALIDATION FAILED")
 
 
-    def constructDetection(self, builder: DetectionBuilder, file_path: str) -> None:
-        builder.reset()
-        builder.setObject(file_path)
-        builder.addDeployment(self.output_dto.deployments)
-        builder.addMitreAttackEnrichment(self.attack_enrichment)
-        builder.addKillChainPhase()
-        builder.addCIS()
-        builder.addNist()
-        builder.addDatamodel()
-        builder.addRBA()
-        builder.addProvidingTechnologies()
-        builder.addNesFields()
-        builder.addAnnotations()
-        builder.addMappings()
-        builder.addBaseline(self.output_dto.baselines)
-        builder.addPlaybook(self.output_dto.playbooks)
-        builder.addMacros(self.output_dto.macros)
-        builder.addLookups(self.output_dto.lookups)
-
-        if self.input_dto.config.enrichments.attack_enrichment:
-            builder.addMitreAttackEnrichment(self.attack_enrichment)
-
-        if self.input_dto.config.enrichments.cve_enrichment:
-            builder.addCve()
-
-        if self.input_dto.config.enrichments.splunk_app_enrichment:
-            builder.addSplunkApp()
-
-        # Skip all integration tests if configured to do so
-        # TODO: is there a better way to handle this? The `test` portion of the config is not defined for validate
-        if (self.input_dto.config.test is not None) and (not self.input_dto.config.test.enable_integration_testing):
-            builder.skipIntegrationTests()
-        
-        if builder.security_content_obj is not None and \
-           builder.security_content_obj.tags is not None and \
-           isinstance(builder.security_content_obj.tags.manual_test,str):
-            # Set all tests, both Unit AND Integration, to manual_test.  Note that integration test messages
-            # will intentionally overwrite the justification in the skipIntegrationTests call above. 
-            builder.skipAllTests(builder.security_content_obj.tags.manual_test)
-
+    
+    
 
-    def constructSSADetection(self, builder: DetectionBuilder, file_path: str) -> None:
+    def constructSSADetection(self, builder: SSADetectionBuilder, directorOutput:DirectorOutputDto, file_path: str) -> None:
         builder.reset()
-        builder.setObject(file_path)
-        builder.addMitreAttackEnrichment(self.attack_enrichment)
+        builder.setObject(file_path,self.output_dto)
+        builder.addMitreAttackEnrichmentNew(directorOutput.attack_enrichment)
         builder.addKillChainPhase()
         builder.addCIS()
         builder.addNist()
         builder.addAnnotations()
         builder.addMappings()
         builder.addUnitTest()
         builder.addRBA()
 
 
-    def constructStory(self, builder: StoryBuilder, file_path: str) -> None:
-        builder.reset()
-        builder.setObject(file_path)
-        builder.addDetections(self.output_dto.detections, self.input_dto.config)
-        builder.addInvestigations(self.output_dto.investigations)
-        builder.addBaselines(self.output_dto.baselines)
-        builder.addAuthorCompanyName()
-
-
-    def constructBaseline(self, builder: BaselineBuilder, file_path: str) -> None:
-        builder.reset()
-        builder.setObject(file_path)
-        builder.addDeployment(self.output_dto.deployments)
-
-
-    def constructDeployment(self, builder: BasicBuilder, file_path: str) -> None:
-        builder.reset()
-        builder.setObject(file_path, SecurityContentType.deployments)
-
-
-    def constructLookup(self, builder: BasicBuilder, file_path: str) -> None:
-        builder.reset()
-        builder.setObject(file_path, SecurityContentType.lookups)
-
-
-    def constructMacro(self, builder: BasicBuilder, file_path: str) -> None:
-        builder.reset()
-        builder.setObject(file_path, SecurityContentType.macros)
-
-
-    def constructPlaybook(self, builder: PlaybookBuilder, file_path: str) -> None:
-        builder.reset()
-        builder.setObject(file_path)
-        builder.addDetections()
-
-
-    def constructTest(self, builder: BasicBuilder, file_path: str) -> None:
-        builder.reset()
-        builder.setObject(file_path, SecurityContentType.unit_tests)
-
-
-    def constructInvestigation(self, builder: InvestigationBuilder, file_path: str) -> None:
-        builder.reset()
-        builder.setObject(file_path)
-        builder.addInputs()
-        builder.addLowercaseName()
-
-    def constructObjects(self, builder: BasicBuilder, file_path: str) -> None:
-        builder.reset()
-        builder.setObject(file_path)
+
```

### Comparing `contentctl-3.6.0/contentctl/input/sigma_converter.py` & `contentctl-4.0.1/contentctl/input/sigma_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,14 @@
 
         if len(errors) > 0:
             errors_string = '\n\t'.join(errors)
             raise Exception(f"The following errors were encountered during conversion:\n\t{errors_string}")
 
     def read_detection(self, detection_path : str) -> Detection:
         yml_dict = YmlReader.load_file(detection_path)
-        yml_dict["tags"]["name"] = yml_dict["name"]
         
         #SSA Detections are ALLOWED to have names longer than 67 characters,
         #unlike Splunk App Detections.  Because we still want to use the 
         #Detection Object (and its validations), we will arbitrarily 
         #truncate the name of a detection if it is too long so that
         #it passes validation, then updated the name after the object
         #is constructed.  Because we do not have Pydantic configured
@@ -230,15 +229,15 @@
         # for ESCU Content and NOT for BA Content. Instead of filtering OUT
         # IntegrationTest, we will ONLY include UnitTest. This supports the introduction
         # of additional ESCU Test Types in the future.
         detection.tests = list(filter(lambda t: isinstance(t, UnitTest), detection.tests))
 
         detection.name = name
 
-        detection.source = os.path.split(os.path.dirname(detection_path))[-1]  
+          
         return detection 
 
 
     def load_data_source(self, input_path: str, data_source_name: str) -> DataSource:
         data_sources = list()
         files = Utils.get_all_yml_files_from_directory(os.path.join(input_path, 'data_sources'))
         for file in files:
```

### Comparing `contentctl-3.6.0/contentctl/input/ssa_detection_builder.py` & `contentctl-4.0.1/contentctl/input/ssa_detection_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import sys
 import re
 import os
 
 from pydantic import ValidationError
-
+from typing import List
 from contentctl.input.yml_reader import YmlReader
 from contentctl.objects.detection import Detection
 from contentctl.objects.security_content_object import SecurityContentObject
 from contentctl.objects.macro import Macro
 from contentctl.objects.mitre_attack_enrichment import MitreAttackEnrichment
 from contentctl.enrichments.cve_enrichment import CveEnrichment
 from contentctl.enrichments.splunk_app_enrichment import SplunkAppEnrichment
 from contentctl.objects.ssa_detection import SSADetection
-from contentctl.objects.constants import ATTACK_TACTICS_KILLCHAIN_MAPPING
-
+from contentctl.objects.constants import *
+from contentctl.input.director import DirectorOutputDto
+from contentctl.enrichments.attack_enrichment import AttackEnrichment
 
 class SSADetectionBuilder():
     security_content_obj : SSADetection
 
 
-    def setObject(self, path: str) -> None:
+    def setObject(self, path: str,
+                  output_dto:DirectorOutputDto ) -> None:
         yml_dict = YmlReader.load_file(path)
-        yml_dict["tags"]["name"] = yml_dict["name"]
+        #self.security_content_obj = SSADetection.model_validate(yml_dict, context={"output_dto":output_dto})     
         self.security_content_obj = SSADetection.parse_obj(yml_dict)
-        self.security_content_obj.source = os.path.split(os.path.dirname(self.security_content_obj.file_path))[-1]      
-
+        self.security_content_obj.source = os.path.split(os.path.dirname(self.security_content_obj.file_path))[-1]
 
     def addProvidingTechnologies(self) -> None:
         if self.security_content_obj:
             if 'Endpoint' in str(self.security_content_obj.search):
                 self.security_content_obj.providing_technologies = ["Sysmon", "Microsoft Windows","Carbon Black Response","CrowdStrike Falcon", "Symantec Endpoint Protection"]
             if "`cloudtrail`" in str(self.security_content_obj.search):
                 self.security_content_obj.providing_technologies = ["Amazon Web Services - Cloudtrail"]
@@ -86,14 +87,22 @@
                                 mitre_attack_tactics = sorted(attack_enrichment[mitre_attack_id]["tactics"]), 
                                 mitre_attack_groups = sorted(attack_enrichment[mitre_attack_id]["groups"])
                             )
                             self.security_content_obj.tags.mitre_attack_enrichments.append(mitre_attack_enrichment)
                         else:
                             #print("mitre_attack_id " + mitre_attack_id + " doesn't exist for detecction " + self.security_content_obj.name)
                             raise ValueError("mitre_attack_id " + mitre_attack_id + " doesn't exist for detection " + self.security_content_obj.name)
+    def addMitreAttackEnrichmentNew(self, attack_enrichment: AttackEnrichment) -> None:
+        if self.security_content_obj and self.security_content_obj.tags.mitre_attack_id:
+            self.security_content_obj.tags.mitre_attack_enrichments = []
+            for mitre_attack_id in self.security_content_obj.tags.mitre_attack_id:
+                enrichment_obj = attack_enrichment.getEnrichmentByMitreID(mitre_attack_id)
+                if enrichment_obj is not None:
+                    self.security_content_obj.tags.mitre_attack_enrichments.append(enrichment_obj)
+
 
 
     def addCIS(self) -> None:
         if self.security_content_obj:
             if self.security_content_obj.tags.security_domain == "network":
                 self.security_content_obj.tags.cis20 = ["CIS 13"]
             else:
```

### Comparing `contentctl-3.6.0/contentctl/input/story_builder.py` & `contentctl-4.0.1/contentctl/objects/story.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,106 +1,147 @@
+from __future__ import annotations
+from typing import TYPE_CHECKING,List
+from contentctl.objects.story_tags import StoryTags
+from pydantic import Field, model_serializer,computed_field, model_validator
 import re
-import sys
-import pathlib
-from pydantic import ValidationError
-
-from contentctl.objects.story import Story
-from contentctl.objects.enums import SecurityContentType
-from contentctl.objects.config import Config
-from contentctl.input.yml_reader import YmlReader
-
-
-class StoryBuilder():
-    story: Story
-
-    def setObject(self, path: pathlib.Path) -> None:
-        yml_dict = YmlReader.load_file(path)
-        yml_dict["tags"]["name"] = yml_dict["name"]
-
-        try:
-            self.story = Story.parse_obj(yml_dict)
-        except ValidationError as e:
-            print('Validation Error for file ' + str(path))
-            print(e)
-            sys.exit(1)
-
-    def reset(self) -> None:
-        self.story = None
-
-    def getObject(self) -> Story:
-        return self.story
-
-    def addDetections(self, detections: list, config: Config) -> None:
-        matched_detection_names = []
-        matched_detections = []
-        mitre_attack_enrichments = []
-        mitre_attack_tactics = set()
-        datamodels = set()
-        kill_chain_phases = set()
-
-        for detection in detections:
-            if detection:
-                for detection_analytic_story in detection.tags.analytic_story:
-                    if detection_analytic_story == self.story.name:
-                        matched_detection_names.append(str(f'{config.build.prefix} - ' + detection.name + ' - Rule'))
-                        mitre_attack_enrichments_list = []
-                        if (detection.tags.mitre_attack_enrichments):
-                            for attack in detection.tags.mitre_attack_enrichments:
-                                mitre_attack_enrichments_list.append({"mitre_attack_technique": attack.mitre_attack_technique})
-                        tags_obj = {"mitre_attack_enrichments": mitre_attack_enrichments_list}
-                        matched_detections.append({
-                            "name": detection.name,
-                            "source": detection.source,
-                            "type": detection.type,
-                            "tags": tags_obj
-                        })
-                        datamodels.update(detection.datamodel)
-                        if detection.tags.kill_chain_phases:
-                            kill_chain_phases.update(detection.tags.kill_chain_phases)
-
-                        if detection.tags.mitre_attack_enrichments:
-                            for attack_enrichment in detection.tags.mitre_attack_enrichments:
-                                mitre_attack_tactics.update(attack_enrichment.mitre_attack_tactics)
-                                if attack_enrichment.mitre_attack_id not in [attack.mitre_attack_id for attack in mitre_attack_enrichments]:
-                                    mitre_attack_enrichments.append(attack_enrichment)
-
-        self.story.detection_names = matched_detection_names
-        self.story.detections = matched_detections
-        self.story.tags.datamodels = sorted(list(datamodels))
-        self.story.tags.kill_chain_phases = sorted(list(kill_chain_phases))
-        self.story.tags.mitre_attack_enrichments = mitre_attack_enrichments
-        self.story.tags.mitre_attack_tactics = sorted(list(mitre_attack_tactics))
-
-
-    def addBaselines(self, baselines: list) -> None:
-        matched_baseline_names = []
-        for baseline in baselines:
-            for baseline_analytic_story in  baseline.tags.analytic_story:
-                if baseline_analytic_story == self.story.name:
-                    matched_baseline_names.append(str(f'ESCU - ' + baseline.name))
-
-        self.story.baseline_names = matched_baseline_names
-
-    def addInvestigations(self, investigations: list) -> None:
-        matched_investigation_names = []
-        matched_investigations = []
-        for investigation in investigations:
-            for investigation_analytic_story in  investigation.tags.analytic_story:
-                if investigation_analytic_story == self.story.name:
-                    matched_investigation_names.append(str(f'ESCU - ' + investigation.name + ' - Response Task'))
-                    matched_investigations.append(investigation)
+if TYPE_CHECKING:
+    from contentctl.objects.detection import Detection
+    from contentctl.objects.investigation import Investigation
+    from contentctl.objects.baseline import Baseline
+    
+
+from contentctl.objects.security_content_object import SecurityContentObject
 
-        self.story.investigation_names = matched_investigation_names
-        self.story.investigations = matched_investigations
 
-    def addAuthorCompanyName(self) -> None:
-        match_author = re.search(r'^([^,]+)', self.story.author)
+
+
+
+#from contentctl.objects.investigation import Investigation
+
+
+
+class Story(SecurityContentObject):
+    narrative: str = Field(...)
+    tags: StoryTags = Field(...)
+
+    # enrichments
+    #detection_names: List[str] = []
+    #investigation_names: List[str] = []
+    #baseline_names: List[str] = []
+
+    # These are updated when detection and investigation objects are created.
+    # Specifically in the model_post_init functions
+    detections:List[Detection] = []
+    investigations: List[Investigation] = []
+    baselines: List[Baseline] = []
+
+
+    def storyAndInvestigationNamesWithApp(self, app_name:str)->List[str]:
+        return [f"{app_name} - {name} - Rule" for name in self.detection_names] + \
+               [f"{app_name} - {name} - Response Task" for name in self.investigation_names]
+        
+    @model_serializer
+    def serialize_model(self):
+        #Call serializer for parent
+        super_fields = super().serialize_model()
+        
+        #All fields custom to this model
+        model= {
+            "narrative": self.narrative,
+            "tags": self.tags.model_dump(),
+            "detection_names": self.detection_names,
+            "investigation_names": self.investigation_names,
+            "baseline_names": self.baseline_names,
+            "author_company": self.author_company,
+            "author_name":self.author_name
+        }
+        detections = []
+        for detection in self.detections:
+            new_detection = {
+                "name":detection.name,
+                "source":detection.source,
+                "type":detection.type
+            }
+            if self.tags.mitre_attack_enrichments is not None:
+                new_detection['tags'] = {"mitre_attack_enrichments": [{"mitre_attack_technique":  enrichment.mitre_attack_technique} for enrichment in detection.tags.mitre_attack_enrichments]}
+            detections.append(new_detection)
+
+        model['detections'] = detections
+        #Combine fields from this model with fields from parent
+        super_fields.update(model)
+        
+        #return the model
+        return super_fields
+
+    @model_validator(mode="after")
+    def setTagsFields(self):
+        
+        enrichments = []
+        for detection in self.detections:
+            enrichments.extend(detection.tags.mitre_attack_enrichments)
+        self.tags.mitre_attack_enrichments = list(set(enrichments))
+
+    
+        tactics = []
+        for enrichment in self.tags.mitre_attack_enrichments:
+            tactics.extend(enrichment.mitre_attack_tactics)
+        self.tags.mitre_attack_tactics = set(tactics)
+
+    
+    
+        datamodels = []
+        for detection in self.detections:
+            datamodels.extend(detection.datamodel)
+        self.tags.datamodels = set(datamodels)
+
+    
+    
+        kill_chain_phases = []
+        for detection in self.detections:
+            kill_chain_phases.extend(detection.tags.kill_chain_phases)
+        self.tags.kill_chain_phases = set(kill_chain_phases)
+
+        return self
+
+
+    @computed_field
+    @property
+    def author_name(self)->str:
+        match_author = re.search(r'^([^,]+)', self.author)
         if match_author is None:
-            self.story.author_name = 'no'
+            return 'no'
         else:
-            self.story.author_name = match_author.group(1)
+            return match_author.group(1)
 
-        match_company = re.search(r',\s?(.*)$', self.story.author)
+    @computed_field
+    @property
+    def author_company(self)->str:
+        match_company = re.search(r',\s?(.*)$', self.author)
         if match_company is None:
-            self.story.author_company = 'no'
+            return 'no'
         else:
-            self.story.author_company = match_company.group(1)
+            return match_company.group(1)
+
+    @computed_field
+    @property
+    def author_email(self)->str:
+        return "-"
+
+    @computed_field
+    @property
+    def detection_names(self)->List[str]:
+        return [detection.name for detection in self.detections]
+    
+    @computed_field
+    @property
+    def investigation_names(self)->List[str]:
+        return [investigation.name for investigation in self.investigations]
+
+    @computed_field
+    @property
+    def baseline_names(self)->List[str]:        
+        return [baseline.name for baseline in self.baselines]
+    
+   
+    
+    
+
```

### Comparing `contentctl-3.6.0/contentctl/input/yml_reader.py` & `contentctl-4.0.1/contentctl/input/yml_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Dict
+from typing import Dict, Any
 
 import yaml
 
 
 import sys
 import pathlib
 
 class YmlReader():
 
     @staticmethod
-    def load_file(file_path: pathlib.Path, add_fields=True, STRICT_YML_CHECKING=False) -> Dict:
+    def load_file(file_path: pathlib.Path, add_fields=True, STRICT_YML_CHECKING=False) -> Dict[str,Any]:
         try:
             file_handler = open(file_path, 'r', encoding="utf-8")
             
             # The following code can help diagnose issues with duplicate keys or 
             # poorly-formatted but still "compliant" YML.  This code should be
             # enabled manually for debugging purposes. As such, strictyaml 
             # library is intentionally excluded from the contentctl requirements
@@ -23,15 +23,16 @@
                 try:
                     strictyaml.dirty_load(file_handler.read(), allow_flow_style = True)
                     file_handler.seek(0)
                 except Exception as e:
                     print(f"Error loading YML file {file_path}: {str(e)}")
                     sys.exit(1)
             try:
-                yml_obj = list(yaml.safe_load_all(file_handler))[0]
+                #yml_obj = list(yaml.safe_load_all(file_handler))[0]
+                yml_obj = yaml.load(file_handler, Loader=yaml.CSafeLoader)
             except yaml.YAMLError as exc:
                 print(exc)
                 sys.exit(1)
 
         except OSError as exc:
             print(exc)
             sys.exit(1)
```

### Comparing `contentctl-3.6.0/contentctl/objects/base_test.py` & `contentctl-4.0.1/contentctl/objects/base_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/objects/base_test_result.py` & `contentctl-4.0.1/contentctl/objects/base_test_result.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/objects/constants.py` & `contentctl-4.0.1/contentctl/objects/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     "Privilege Escalation": "Exploitation",
     "Defense Evasion": "Exploitation",
     "Credential Access": "Exploitation",
     "Discovery": "Exploitation",
     "Lateral Movement": "Exploitation",
     "Collection": "Exploitation",
     "Command And Control": "Command and Control",
-    "Command And Control": "Command and Control",
     "Exfiltration": "Actions on Objectives",
     "Impact": "Actions on Objectives"
 }
 
 SES_CONTEXT_MAPPING = {
     "Unknown": 0,
     "Source:Endpoint": 10,
```

### Comparing `contentctl-3.6.0/contentctl/objects/correlation_search.py` & `contentctl-4.0.1/contentctl/objects/correlation_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
     ## All remaining fields can be derived from other fields or have intentional defaults that      # noqa: E266
     ## should not be changed (validators should prevent instantiating some of these fields directly # noqa: E266
     ## to prevent undefined behavior)                                                               # noqa: E266
 
     # The logger to use (logs all go to a null pipe unless ENABLE_LOGGING is set to True, so as not
     # to conflict w/ tqdm)
-    logger: logging.Logger = Field(default_factory=get_logger, const=True)
+    logger: logging.Logger = Field(default_factory=get_logger)
 
     # The search name (e.g. "ESCU - Windows Modify Registry EnableLinkedConnections - Rule")
     name: Optional[str] = None
 
     # The path to the saved search on the Splunk instance
     splunk_path: Optional[str] = None
```

### Comparing `contentctl-3.6.0/contentctl/objects/deployment.py` & `contentctl-4.0.1/contentctl/objects/alert_action.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,40 @@
+from __future__ import annotations
+from pydantic import BaseModel, model_serializer
+from typing import Optional
 
-import uuid
-import string
-
-from pydantic import BaseModel, validator, ValidationError
-from datetime import datetime
-
-from contentctl.objects.security_content_object import SecurityContentObject
-from contentctl.objects.deployment_scheduling import DeploymentScheduling
 from contentctl.objects.deployment_email import DeploymentEmail
 from contentctl.objects.deployment_notable import DeploymentNotable
 from contentctl.objects.deployment_rba import DeploymentRBA
 from contentctl.objects.deployment_slack import DeploymentSlack
 from contentctl.objects.deployment_phantom import DeploymentPhantom
-from contentctl.objects.enums import SecurityContentType
-class Deployment(SecurityContentObject):
-    name: str = "PLACEHOLDER_NAME"
-    #id: str = None
-    #date: str = None
-    #author: str = None
-    #description: str = None
-    #contentType: SecurityContentType = SecurityContentType.deployments
-    scheduling: DeploymentScheduling = None
-    email: DeploymentEmail = None
-    notable: DeploymentNotable = None
-    rba: DeploymentRBA = None
-    slack: DeploymentSlack = None
-    phantom: DeploymentPhantom = None
-    tags: dict = None
-    
+
+class AlertAction(BaseModel):
+    email: Optional[DeploymentEmail] = None
+    notable: Optional[DeploymentNotable] = None
+    rba: Optional[DeploymentRBA] = DeploymentRBA()
+    slack: Optional[DeploymentSlack] = None
+    phantom: Optional[DeploymentPhantom] = None
+
+    
+    @model_serializer
+    def serialize_model(self):
+        #Call serializer for parent
+        model = {}
+
+        if self.email is not None:
+            raise Exception("Email not implemented")
+
+        if self.notable is not None:
+            model['notable'] = self.notable
+
+        if self.rba is not None and self.rba.enabled:
+            model['rba'] = {'enabled': "true"}
+
+        if self.slack is not None:
+            raise Exception("Slack not implemented")
+        
+        if self.phantom is not None:
+            raise Exception("Phantom not implemented")
+        
+        #return the model
+        return model
```

### Comparing `contentctl-3.6.0/contentctl/objects/detection.py` & `contentctl-4.0.1/contentctl/objects/detection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-from typing import Union
-from pydantic import validator
-
+from __future__ import annotations
 from contentctl.objects.abstract_security_content_objects.detection_abstract import Detection_Abstract
 
-
-
 class Detection(Detection_Abstract):
     # Customization to the Detection Class go here.
     # You may add fields and/or validations
 
     # You may also experiment with removing fields
     # and/or validations,  or chagning validation(s).
     # Please be aware that many defaults field(s)
```

### Comparing `contentctl-3.6.0/contentctl/objects/detection_tags.py` & `contentctl-4.0.1/contentctl/objects/ssa_detection_tags.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+from __future__ import annotations
 import re
+from typing import List
+from pydantic import BaseModel, validator, ValidationError, model_validator, Field
 
-from pydantic import BaseModel, validator, ValidationError, root_validator
 from contentctl.objects.mitre_attack_enrichment import MitreAttackEnrichment
 from contentctl.objects.constants import *
-from contentctl.objects.observable import Observable
+from contentctl.objects.enums import SecurityContentProductName
 
-class DetectionTags(BaseModel):
+class SSADetectionTags(BaseModel):
     # detection spec
-    name: str
+    #name: str
     analytic_story: list
     asset_type: str
     automated_detection_testing: str = None
     cis20: list = None
-    confidence: str
+    confidence: int
     impact: int
     kill_chain_phases: list = None
+    message: str
     mitre_attack_id: list = None
     nist: list = None
-    observable: list[Observable] = []
-    message: str
-    product: list
+    observable: list
+    product: List[SecurityContentProductName] = Field(...,min_length=1)
     required_fields: list
     risk_score: int
     security_domain: str
     risk_severity: str = None
     cve: list = None
     supported_tas: list = None
     atomic_guid: list = None
@@ -36,15 +38,17 @@
     confidence_id: int = None
     impact_id: int = None
     context_ids: list = None
     risk_level_id: int = None
     risk_level: str = None
     observable_str: str = None
     evidence_str: str = None
-    kill_chain_phases_id: list = None
+    analytics_story_str: str = None
+    kill_chain_phases_id:dict = None
+    kill_chain_phases_str:str = None
     research_site_url: str = None
     event_schema: str = None
     mappings: list = None
     annotations: dict = None
 
 
     @validator('cis20')
@@ -71,90 +75,64 @@
                 raise ValueError(f"NIST Category '{value}' is not a valid category")
         return v
 
     @validator('confidence')
     def tags_confidence(cls, v, values):
         v = int(v)
         if not (v > 0 and v <= 100):
-             raise ValueError('confidence score is out of range 1-100: ' + values["name"])
+             raise ValueError('confidence score is out of range 1-100.' )
         else:
             return v
 
-    @validator('context_ids')
-    def tags_context(cls, v, values):
-        context_list = SES_CONTEXT_MAPPING.keys()
-        for value in v:
-            if value not in context_list:
-                raise ValueError('context value not valid for ' + values["name"] + '. valid options are ' + str(context_list) )
-        return v
 
     @validator('impact')
     def tags_impact(cls, v, values):
         if not (v > 0 and v <= 100):
-             raise ValueError('impact score is out of range 1-100: ' + values["name"])
+             raise ValueError('impact score is out of range 1-100.')
         else:
             return v
 
     @validator('kill_chain_phases')
     def tags_kill_chain_phases(cls, v, values):
         valid_kill_chain_phases = SES_KILL_CHAIN_MAPPINGS.keys()
         for value in v:
             if value not in valid_kill_chain_phases:
-                raise ValueError('kill chain phase not valid for ' + values["name"] + '. valid options are ' + str(valid_kill_chain_phases))
+                raise ValueError('kill chain phase not valid. Valid options are ' + str(valid_kill_chain_phases))
         return v
 
     @validator('mitre_attack_id')
     def tags_mitre_attack_id(cls, v, values):
         pattern = 'T[0-9]{4}'
         for value in v:
             if not re.match(pattern, value):
-                raise ValueError('Mitre Attack ID are not following the pattern Txxxx: ' + values["name"])
+                raise ValueError('Mitre Attack ID are not following the pattern Txxxx:' )
         return v
 
-    @validator('product')
-    def tags_product(cls, v, values):
-        valid_products = [
-            "Splunk Enterprise", "Splunk Enterprise Security", "Splunk Cloud",
-            "Splunk Security Analytics for AWS", "Splunk Behavioral Analytics"
-        ]
 
-        for value in v:
-            if value not in valid_products:
-                raise ValueError('product is not valid for ' + values['name'] + '. valid products are ' + str(valid_products))
-        return v
 
     @validator('risk_score')
     def tags_calculate_risk_score(cls, v, values):
         calculated_risk_score = round(values['impact'] * values['confidence'] / 100)
         if calculated_risk_score != int(v):
             raise ValueError(f"Risk Score must be calculated as round(confidence * impact / 100)"
                              f"\n  Expected risk_score={calculated_risk_score}, found risk_score={int(v)}: {values['name']}")
         return v
-    
-    # The following validator is temporarily disabled pending further discussions
-    # @validator('message')
-    # def validate_message(cls,v,values):
-        
-    #     observables:list[Observable] = values.get("observable",[])
-    #     observable_names = set([o.name for o in observables])
-    #     #find all of the observables used in the message by name
-    #     name_match_regex = r"\$([^\s.]*)\$"
-        
-    #     message_observables = set()
 
-    #     #Make sure that all observable names in 
-    #     for match in re.findall(name_match_regex, v):
-    #         #Remove
-    #         match_without_dollars = match.replace("$", "")
-    #         message_observables.add(match_without_dollars)
-        
 
-    #     missing_observables = message_observables - observable_names
-    #     unused_observables = observable_names - message_observables
-    #     if len(missing_observables) > 0:
-    #         raise ValueError(f"The following observables are referenced in the message, but were not declared as observables: {missing_observables}")
+    @model_validator(mode="after")
+    def tags_observable(self):
+        valid_roles = SES_OBSERVABLE_ROLE_MAPPING.keys()
+        valid_types = SES_OBSERVABLE_TYPE_MAPPING.keys()
         
-    #     if len(unused_observables) > 0:
-    #         raise ValueError(f"The following observables were declared, but are not referenced in the message: {unused_observables}")        
-    #     return v
-
-    
+        for value in self.observable:
+            if value['type'] in valid_types:
+                if 'Splunk Behavioral Analytics' in self.product:
+                    continue
+
+                if 'role' not in value:
+                    raise ValueError('Observable role is missing')
+                for role in value['role']:
+                    if role not in valid_roles:
+                        raise ValueError(f'Observable role ' + role + ' not valid. Valid options are {str(valid_roles)}')
+            else:
+                raise ValueError(f'Observable type ' + value['type'] + ' not valid. Valid options are {str(valid_types)}')
+        return self
```

### Comparing `contentctl-3.6.0/contentctl/objects/integration_test.py` & `contentctl-4.0.1/contentctl/objects/integration_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class IntegrationTest(BaseTest):
     """
     An integration test for a detection against ES
     """
     # The test type (integration)
-    test_type: TestType = Field(TestType.INTEGRATION, const=True)
+    test_type: TestType = Field(TestType.INTEGRATION)
 
     # The test result
     result: Union[None, IntegrationTestResult] = None
 
     @classmethod
     def derive_from_unit_test(cls, unit_test: UnitTest) -> "IntegrationTest":
         """
```

### Comparing `contentctl-3.6.0/contentctl/objects/macro.py` & `contentctl-4.0.1/contentctl/objects/macro.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,64 @@
 # Used so that we can have a staticmethod that takes the class 
 # type Macro as an argument
 from __future__ import annotations
+from typing import TYPE_CHECKING, List
 import re
-from pydantic import BaseModel, validator, ValidationError
-
+from pydantic import Field, model_serializer
+if TYPE_CHECKING:
+    from contentctl.input.director import DirectorOutputDto
 from contentctl.objects.security_content_object import SecurityContentObject
-from contentctl.objects.enums import SecurityContentType
-from typing import Tuple
+
 
 
 MACROS_TO_IGNORE = set(["_filter", "drop_dm_object_name"])
 #Should all of the following be included as well?
 MACROS_TO_IGNORE.add("get_asset" )
 MACROS_TO_IGNORE.add("get_risk_severity")
 MACROS_TO_IGNORE.add("cim_corporate_web_domain_search")
 MACROS_TO_IGNORE.add("prohibited_processes")
 
 
-class Macro(BaseModel):
-    #contentType: SecurityContentType = SecurityContentType.macros
-    name: str
-    definition: str
-    description: str
-    arguments: list = None
-    file_path: str = None
-
-    # Macro can have different punctuatuation in it,
-    # so redefine the name validator. For now, jsut
-    # allow any characters in the macro
-    @validator('name',check_fields=False)
-    def name_invalid_chars(cls, v):
-        return v
-
-
-    # Allow long names for macros
-    @validator('name',check_fields=False)
-    def name_max_length(cls, v):
-        #if len(v) > 67:
-        #    raise ValueError('name is longer then 67 chars: ' + v)
-        return v
+class Macro(SecurityContentObject):
+    definition: str = Field(..., min_length=1)
+    arguments: List[str] = Field([])
+    
+    
+
 
+    @model_serializer
+    def serialize_model(self):
+        #Call serializer for parent
+        super_fields = super().serialize_model()
+
+        #All fields custom to this model
+        model= {
+            "definition": self.definition,
+            "description": self.description,
+        }
+        
+        #return the model
+        model.update(super_fields)
+        
+        return model
     
     @staticmethod
-    def get_macros(text_field:str, all_macros: list[Macro], ignore_macros:set[str]=MACROS_TO_IGNORE)->Tuple[list[Macro], set[str]]:
+
+    def get_macros(text_field:str, director:DirectorOutputDto , ignore_macros:set[str]=MACROS_TO_IGNORE)->list[Macro]:
         #Remove any comments, allowing there to be macros (which have a single backtick) inside those comments
         #If a comment ENDS in a macro, for example ```this is a comment with a macro `macro_here````
         #then there is a small edge case where the regex below does not work properly.  If that is 
         #the case, we edit the search slightly to insert a space
         text_field = re.sub(r"\`\`\`\`", r"` ```", text_field)
         text_field = re.sub(r"\`\`\`.*?\`\`\`", " ", text_field)
         
+
         macros_to_get = re.findall(r'`([^\s]+)`', text_field)
         #If macros take arguments, stop at the first argument.  We just want the name of the macro
         macros_to_get = set([macro[:macro.find('(')] if macro.find('(') != -1 else macro for macro in macros_to_get])
         
         macros_to_ignore = set([macro for macro in macros_to_get if any(to_ignore in macro for to_ignore in ignore_macros)])
         #remove the ones that we will ignore
         macros_to_get -= macros_to_ignore
-        found_macros, missing_macros = SecurityContentObject.get_objects_by_name(macros_to_get, all_macros)
-        return found_macros, missing_macros
-
-        # found_macros = [macro for macro in all_macros if macro.name in macros_to_get]
-        
-        # missing_macros = macros_to_get - set([macro.name for macro in found_macros])
-        # missing_macros_after_ignored_macros = set()
-        # for macro in missing_macros:
-        #     found = False
-        #     for ignore in ignore_macros:
-        #         if ignore in macro:
-        #             found=True
-        #             break
-        #     if found is False:
-        #         missing_macros_after_ignored_macros.add(macro)
-
-        #return found_macros, missing_macros_after_ignored_macros
+        return Macro.mapNamesToSecurityContentObjects(list(macros_to_get), director)
         
-
-
-
+
```

### Comparing `contentctl-3.6.0/contentctl/objects/notable_action.py` & `contentctl-4.0.1/contentctl/objects/notable_action.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/objects/observable.py` & `contentctl-4.0.1/contentctl/objects/observable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-import abc
-import string
-import uuid
-from typing import Literal
-from datetime import datetime
-from pydantic import BaseModel, validator, ValidationError
-from contentctl.objects.enums import SecurityContentType
+from __future__ import annotations
+from pydantic import BaseModel, validator
+
 from contentctl.objects.constants import *
 
 
 
 class Observable(BaseModel):
     name: str
     type: str
```

### Comparing `contentctl-3.6.0/contentctl/objects/risk_analysis_action.py` & `contentctl-4.0.1/contentctl/objects/risk_analysis_action.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/objects/risk_object.py` & `contentctl-4.0.1/contentctl/objects/risk_object.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/objects/ssa_detection.py` & `contentctl-4.0.1/contentctl/objects/ssa_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import uuid
 import string
 import requests
 import time
 from pydantic import BaseModel, validator, root_validator
 from dataclasses import dataclass
 from datetime import datetime
@@ -10,16 +11,16 @@
 
 from contentctl.objects.abstract_security_content_objects.detection_abstract import Detection_Abstract
 from contentctl.objects.enums import AnalyticsType
 from contentctl.objects.enums import DataModel
 from contentctl.objects.enums import DetectionStatus
 from contentctl.objects.deployment import Deployment
 from contentctl.objects.ssa_detection_tags import SSADetectionTags
-from contentctl.objects.config import ConfigDetectionConfiguration
-from contentctl.objects.unit_test import UnitTest
+from contentctl.objects.unit_test_ssa import UnitTestSSA
+from contentctl.objects.unit_test_old import UnitTestOld
 from contentctl.objects.macro import Macro
 from contentctl.objects.lookup import Lookup
 from contentctl.objects.baseline import Baseline
 from contentctl.objects.playbook import Playbook
 from contentctl.helper.link_validator import LinkValidator
 from contentctl.objects.enums import SecurityContentType
 
@@ -36,35 +37,36 @@
     description: str
     data_source: list[str]
     search: Union[str, dict]
     how_to_implement: str
     known_false_positives: str
     references: list
     tags: SSADetectionTags
-    tests: list[UnitTest] = None
+    tests: list[UnitTestSSA] = None
 
     # enrichments
     annotations: dict = None
     risk: list = None
     mappings: dict = None
     file_path: str = None
     source: str = None
-    test: Union[UnitTest, dict] = None
+    test: Union[UnitTestSSA, dict, UnitTestOld] = None
     runtime: str = None
     internalVersion: int = None
 
     # @validator('name')v
     # def name_max_length(cls, v, values):
     #     if len(v) > 67:
     #         raise ValueError('name is longer then 67 chars: ' + v)
     #     return v
 
     class Config:
         use_enum_values = True
 
+    '''
     @validator("name")
     def name_invalid_chars(cls, v):
         invalidChars = set(string.punctuation.replace("-", ""))
         if any(char in invalidChars for char in v):
             raise ValueError("invalid chars used in name: " + v)
         return v
 
@@ -146,7 +148,9 @@
     @validator("tests")
     def tests_validate(cls, v, values):
         if (values.get("status","") in [DetectionStatus.production.value, DetectionStatus.validation.value]) and not v:
             raise ValueError(
                 "At least one test is required for a production or validation detection: " + values["name"]
             )
         return v
+
+    '''
```

### Comparing `contentctl-3.6.0/contentctl/objects/test_group.py` & `contentctl-4.0.1/contentctl/objects/test_group.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/objects/threat_object.py` & `contentctl-4.0.1/contentctl/objects/threat_object.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/objects/unit_test.py` & `contentctl-4.0.1/contentctl/objects/unit_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-
+from __future__ import annotations
+from pydantic import Field
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from contentctl.objects.unit_test_attack_data import UnitTestAttackData
+    from contentctl.objects.unit_test_result import UnitTestResult
 
 from typing import Union
 
 from pydantic import Field
 
 # from contentctl.objects.security_content_object import SecurityContentObject
 # from contentctl.objects.enums import SecurityContentType
@@ -16,15 +21,15 @@
 class UnitTest(BaseTest):
     """
     A unit test for a detection
     """
     # contentType: SecurityContentType = SecurityContentType.unit_tests
 
     # The test type (unit)
-    test_type: TestType = Field(TestType.UNIT, const=True)
+    test_type: TestType = Field(TestType.UNIT)
 
     # The condition to check if the search was successful
     pass_condition: Union[str, None] = None
 
     # Baselines to be run before a unit test
     baselines: list[UnitTestBaseline] = []
```

### Comparing `contentctl-3.6.0/contentctl/objects/unit_test_result.py` & `contentctl-4.0.1/contentctl/objects/unit_test_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import Union
+from __future__ import annotations
 
+from typing import Union,TYPE_CHECKING
 from splunklib.data import Record
-
-from contentctl.objects.test_config import Infrastructure
 from contentctl.objects.base_test_result import BaseTestResult, TestResultStatus
 
+if TYPE_CHECKING:
+    from contentctl.objects.config import Infrastructure
+
 FORCE_TEST_FAILURE_FOR_MISSING_OBSERVABLE = False
 
 NO_SID = "Testing Failed, NO Search ID"
 SID_TEMPLATE = "{server}:{web_port}/en-US/app/search/search?sid={sid}"
 
 
 class UnitTestResult(BaseTestResult):
```

### Comparing `contentctl-3.6.0/contentctl/output/attack_nav_output.py` & `contentctl-4.0.1/contentctl/output/attack_nav_output.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 import os
+from typing import List,Union
+import pathlib
 
-
-from contentctl.objects.enums import SecurityContentType
+from contentctl.objects.detection import Detection
 from contentctl.output.attack_nav_writer import AttackNavWriter
 
 
 class AttackNavOutput():
 
-    def writeObjects(self, objects: list, output_path: str, type: SecurityContentType = None) -> None:
-        techniques = dict()
+    def writeObjects(self, detections: List[Detection], output_path: pathlib.Path) -> None:
+        techniques:dict[str,dict[str,Union[List[str],int]]] = {}
+        for detection in detections:
+            for tactic in detection.tags.mitre_attack_id:
+                if tactic not in techniques:
+                    techniques[tactic] = {'score':0,'file_paths':[]}
+                
+                detection_url = f"https://github.com/splunk/security_content/blob/develop/detections/{detection.source}/{detection.file_path.name}"
+                techniques[tactic]['score'] += 1
+                techniques[tactic]['file_paths'].append(detection_url)
+                
+        '''
         for detection in objects:
             if detection.tags.mitre_attack_enrichments:
                 for mitre_attack_enrichment in detection.tags.mitre_attack_enrichments:
                     if not mitre_attack_enrichment.mitre_attack_id in techniques:
                         techniques[mitre_attack_enrichment.mitre_attack_id] = {
                                 'score': 1,
-                                'file_paths': ['https://github.com/splunk/security_content/blob/develop/detections/' + detection.source + '/' + self.convertNameToFileName(detection.name)]
+                                'file_paths': ['https://github.com/splunk/security_content/blob/develop/detections/' + detection.getSource() + '/' + self.convertNameToFileName(detection.name)]
                             }
                     else:
                         techniques[mitre_attack_enrichment.mitre_attack_id]['score'] = techniques[mitre_attack_enrichment.mitre_attack_id]['score'] + 1
-                        techniques[mitre_attack_enrichment.mitre_attack_id]['file_paths'].append('https://github.com/splunk/security_content/blob/develop/detections/' + detection.source + '/' + self.convertNameToFileName(detection.name))
-
-        AttackNavWriter.writeAttackNavFile(techniques, os.path.join(output_path, 'coverage.json'))
-
+                        techniques[mitre_attack_enrichment.mitre_attack_id]['file_paths'].append('https://github.com/splunk/security_content/blob/develop/detections/' + detection.getSource() + '/' + self.convertNameToFileName(detection.name))
+        '''
+        AttackNavWriter.writeAttackNavFile(techniques, output_path / 'coverage.json')
+        
 
     def convertNameToFileName(self, name: str):
         file_name = name \
             .replace(' ', '_') \
             .replace('-','_') \
             .replace('.','_') \
             .replace('/','_') \
```

### Comparing `contentctl-3.6.0/contentctl/output/attack_nav_writer.py` & `contentctl-4.0.1/contentctl/output/attack_nav_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 import json
-
-
+from typing import Union, List
+import pathlib
 VERSION = "4.3"
 NAME = "Detection Coverage"
 DESCRIPTION = "security_content detection coverage"
 DOMAIN = "mitre-enterprise"
 
 
 class AttackNavWriter():
 
     @staticmethod
-    def writeAttackNavFile(mitre_techniques : dict, output_path : str) -> None:
+    def writeAttackNavFile(mitre_techniques : dict[str,dict[str,Union[List[str],int]]], output_path : pathlib.Path) -> None:
         max_count = 0
         for technique_id in mitre_techniques.keys():
             if mitre_techniques[technique_id]['score'] > max_count:
                 max_count = mitre_techniques[technique_id]['score']
         
         layer_json = {
             "version": VERSION,
```

### Comparing `contentctl-3.6.0/contentctl/output/ba_yml_output.py` & `contentctl-4.0.1/contentctl/output/ba_yml_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             file_path = object['file_path']
             object.pop('file_path')
             object.pop('deprecated')
             object.pop('experimental') 
             YmlWriter.writeYmlFile(file_path, object)
 
 
-    def writeObjects(self, objects: list, output_path: str, type: SecurityContentType = None) -> None:
+    def writeObjects(self, objects: list, output_path: str, contentType: SecurityContentType = None) -> None:
         for obj in objects: 
             file_name = "ssa___" + self.convertNameToFileName(obj.name, obj.tags)
             if self.isComplexBARule(obj.search):
                 file_path = os.path.join(output_path, 'complex', file_name)
             else:
                 file_path = os.path.join(output_path, 'srs', file_name)
 
@@ -42,16 +42,17 @@
             if obj.test:
                 test_dict = {
                     "name": obj.name + " Unit Test",
                     "tests": [obj.test.dict()]
                 }
                 test_dict["tests"][0]["name"] = obj.name
                 for count in range(len(test_dict["tests"][0]["attack_data"])):
-                    a = urlparse(test_dict["tests"][0]["attack_data"][count]["data"])
+                    a = urlparse(str(test_dict["tests"][0]["attack_data"][count]["data"]))
                     test_dict["tests"][0]["attack_data"][count]["file_name"] = os.path.basename(a.path)
+
                 test = UnitTestOld.parse_obj(test_dict)
 
                 obj.test = test
 
             # create annotations object
             obj.tags.annotations = {
                 "analytic_story": obj.tags.analytic_story,
@@ -146,8 +147,7 @@
             file_name = file_name + '.yml'
         return file_name
 
 
     def isComplexBARule(self, search):
         return re.findall("stats|first_time_event|adaptive_threshold", search)
 
-
```

### Comparing `contentctl-3.6.0/contentctl/output/detection_writer.py` & `contentctl-4.0.1/contentctl/output/detection_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/doc_md_output.py` & `contentctl-4.0.1/contentctl/output/doc_md_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/finding_report_writer.py` & `contentctl-4.0.1/contentctl/output/finding_report_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/jinja_writer.py` & `contentctl-4.0.1/contentctl/output/jinja_writer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-
+from typing import Any
 from jinja2 import Environment, FileSystemLoader
 
 
 class JinjaWriter:
 
     @staticmethod
     def writeObjectsList(template_name : str, output_path : str, objects : list) -> None:
@@ -16,15 +16,15 @@
         output = template.render(objects=objects)
         with open(output_path, 'w') as f:
             output = output.encode('ascii', 'ignore').decode('ascii')
             f.write(output)
 
 
     @staticmethod
-    def writeObject(template_name : str, output_path : str, object : dict) -> None:
+    def writeObject(template_name : str, output_path : str, object: dict[str,Any]) -> None:
 
         j2_env = Environment(
             loader=FileSystemLoader(os.path.join(os.path.dirname(__file__), 'templates')), 
             trim_blocks=False)
 
         template = j2_env.get_template(template_name)
         output = template.render(object=object)
```

### Comparing `contentctl-3.6.0/contentctl/output/new_content_yml_output.py` & `contentctl-4.0.1/contentctl/output/new_content_yml_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import os
 import pathlib
 from contentctl.objects.enums import SecurityContentType
 from contentctl.output.yml_writer import YmlWriter
-
-
+import pathlib
+from contentctl.objects.config import NewContentType
 class NewContentYmlOutput():
-    output_path: str
+    output_path: pathlib.Path
     
-    def __init__(self, output_path:str):
+    def __init__(self, output_path:pathlib.Path):
         self.output_path = output_path
     
     
-    def writeObjectNewContent(self, object: dict, subdirectory_name: str, type: SecurityContentType) -> None:
-        if type == SecurityContentType.detections:
+    def writeObjectNewContent(self, object: dict, subdirectory_name: str, type: NewContentType) -> None:
+        if type == NewContentType.detection:
+
             file_path = os.path.join(self.output_path, 'detections', subdirectory_name, self.convertNameToFileName(object['name'], object['tags']['product']))
             output_folder = pathlib.Path(self.output_path)/'detections'/subdirectory_name
             #make sure the output folder exists for this detection
             output_folder.mkdir(exist_ok=True)
 
             YmlWriter.writeYmlFile(file_path, object)
             print("Successfully created detection " + file_path)
         
-        elif type == SecurityContentType.stories:
+        elif type == NewContentType.story:
             file_path = os.path.join(self.output_path, 'stories', self.convertNameToFileName(object['name'], object['tags']['product']))
             YmlWriter.writeYmlFile(file_path, object)
             print("Successfully created story " + file_path)        
         
         else:
             raise(Exception(f"Object Must be Story or Detection, but is not: {object}"))
```

### Comparing `contentctl-3.6.0/contentctl/output/svg_output.py` & `contentctl-4.0.1/contentctl/output/svg_output.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import os
 import pathlib
+from typing import List, Any
 
 from contentctl.objects.enums import SecurityContentType
 from contentctl.output.jinja_writer import JinjaWriter
-from contentctl.objects.config import Config
 from contentctl.objects.enums import DetectionStatus
+from contentctl.objects.detection import Detection
 class SvgOutput():
 
-    def get_badge_dict(self, name:str, total_detections:list, these_detections:list):
-        obj = dict()
+    
+    def get_badge_dict(self, name:str, total_detections:List[Detection], these_detections:List[Detection])->dict[str,Any]:
+        obj:dict[str,Any] = {}
         obj['name'] = name
+
         if name == "Production":
             obj['color'] = "Green"
         elif name == "Detections":
             obj['color'] = "Green"
         elif name == "Experimental":
             obj['color'] = "Yellow"
         elif name == "Deprecated":
@@ -22,44 +25,31 @@
         obj['count'] = len(total_detections)
         if obj['count'] == 0:
             obj['coverage'] = "NaN"
         else:
             obj['coverage'] = len(these_detections) / obj['count']
             obj['coverage'] = "{:.0%}".format(obj['coverage'])
         return obj
-
-    def writeObjects(self, objects: list, path: str, type: SecurityContentType = None) -> None:
+    
+    def writeObjects(self, detections: List[Detection], output_path: pathlib.Path, type: SecurityContentType = None) -> None:
         
-        detections_tmp = objects    
-
-        output_path = pathlib.Path(path)
-
-        production_detections = []
-        deprecated_detections = []
-        experimental_detections = []
-        obj = dict()
         
-        for detection in detections_tmp:
-            if detection.status == DetectionStatus.production.value:
-                production_detections.append(detection)
-            if detection.status == DetectionStatus.deprecated.value:
-                deprecated_detections.append(detection)
-            elif detection.status == DetectionStatus.experimental.value:
-                experimental_detections.append(detection)
 
+        total_dict:dict[str,Any] = self.get_badge_dict("Detections", detections, detections)
+        production_dict:dict[str,Any] = self.get_badge_dict("% Production", detections, [detection for detection in detections if detection.status == DetectionStatus.production.value])
+        #deprecated_dict = self.get_badge_dict("Deprecated", detections, [detection for detection in detections if detection.status == DetectionStatus.deprecated])
+        #experimental_dict = self.get_badge_dict("Experimental", detections, [detection for detection in detections if detection.status == DetectionStatus.experimental])
         
-        total_detections = production_detections + deprecated_detections + experimental_detections
-        total_dict = self.get_badge_dict("Detections", total_detections, production_detections)
-        production_dict = self.get_badge_dict("Production", total_detections, production_detections)
-        deprecated_dict = self.get_badge_dict("Deprecated", total_detections, deprecated_detections)
-        experimental_dict = self.get_badge_dict("Experimental", total_detections, experimental_detections)
         
 
-        JinjaWriter.writeObject('detection_count.j2', os.path.join(output_path, 'detection_count.svg'), total_dict)
+
+        #Total number of detections
+        JinjaWriter.writeObject('detection_count.j2', output_path /'detection_count.svg', total_dict)
         #JinjaWriter.writeObject('detection_count.j2', os.path.join(output_path, 'production_count.svg'), production_dict)
         #JinjaWriter.writeObject('detection_count.j2', os.path.join(output_path, 'deprecated_count.svg'), deprecated_dict)
         #JinjaWriter.writeObject('detection_count.j2', os.path.join(output_path, 'experimental_count.svg'), experimental_dict)
 
-        JinjaWriter.writeObject('detection_coverage.j2', os.path.join(output_path, 'detection_coverage.svg'), total_dict)
+        #Percentage of detections that are production
+        JinjaWriter.writeObject('detection_coverage.j2', output_path/'detection_coverage.svg', production_dict)
         #JinjaWriter.writeObject('detection_coverage.j2', os.path.join(output_path, 'detection_coverage.svg'), deprecated_dict)
         #JinjaWriter.writeObject('detection_coverage.j2', os.path.join(output_path, 'detection_coverage.svg'), experimental_dict)
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/analyticstories_detections.j2` & `contentctl-4.0.1/contentctl/output/templates/analyticstories_detections.j2`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 
 ### DETECTIONS ###
 
 {% for detection in objects %}
 {% if (detection.type == 'TTP' or detection.type == 'Anomaly' or detection.type == 'Hunting' or detection.type == 'Correlation') %}
 [savedsearch://{{APP_NAME}} - {{ detection.name }} - Rule]
 type = detection
-asset_type = {{ detection.tags.asset_type }}
+asset_type = {{ detection.tags.asset_type.value }}
 confidence = medium
-explanation = {{ detection.description }}
+explanation = {{ detection.description | escapeNewlines() }}
 {% if detection.how_to_implement is defined %}
-how_to_implement = {{ detection.how_to_implement }}
+how_to_implement = {{ detection.how_to_implement | escapeNewlines() }}
 {% else %}
 how_to_implement = none
 {% endif %}
 annotations = {{ detection.mappings | tojson }}
-known_false_positives = {{ detection.known_false_positives }}
+known_false_positives = {{ detection.known_false_positives | escapeNewlines() }}
+{% if detection.providing_technologies | length > 0  %}
 providing_technologies = {{ detection.providing_technologies | tojson }}
+{% else %}
+providing_technologies = null
+{% endif %}
 
 {% endif %}
 {% endfor %}
 ### END DETECTIONS ###
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/analyticstories_stories.j2` & `contentctl-4.0.1/contentctl/output/templates/analyticstories_stories.j2`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 
 ### STORIES ###
 
 {% for story in objects %}
 [analytic_story://{{ story.name }}]
-category = {{ story.tags.category[0].value }}
+category = {{ story.tags.getCategory_conf() }}
 last_updated = {{ story.date }}
 version = {{ story.version }}
-references = {{ story.references | tojson }}
-maintainers = [{"company": "{{ story.author_company }}", "email": "-", "name": "{{ story.author_name }}"}]
+references = {{ story.getReferencesListForJson() | tojson }}
+maintainers = [{"company": "{{ story.author_company }}", "email": "{{ story.author_email }}", "name": "{{ story.author_name }}"}]
 spec_version = 3
-searches = {{ (story.detection_names + story.investigation_names) | tojson }}
-description = {{ story.description }}
+searches = {{ story.storyAndInvestigationNamesWithApp(APP_NAME) | tojson }}
+description = {{ story.description | escapeNewlines() }}
 {% if story.narrative is defined %}
-narrative = {{ story.narrative }}
+narrative = {{ story.narrative | escapeNewlines() }}
 {% endif %}
 
 {% endfor %}
 ### END STORIES ###
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/app.conf.j2` & `contentctl-4.0.1/contentctl/output/templates/app.conf.j2`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 reload.postprocess = simple
 reload.content-version = simple
 reload.es_investigations = simple
 
 [launcher]
 author = {{ objects[0].author_company }}
 version = {{ objects[0].version }} 
-description = {{ objects[0].description }}
+description = {{ objects[0].description | escapeNewlines() }}
 
 [ui]
 is_visible = true
 label = {{ objects[0].title }}
 
 [package]
-id = {{ objects[0].name }}
+id = {{ objects[0].appid }}
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/app.manifest.j2` & `contentctl-4.0.1/contentctl/output/templates/app.manifest.j2`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'info'": "{'id': {'name': '{{ objects[0].appid }}'}, 'releaseDate': '{{ currentDate }}'}"}*

```diff
@@ -14,28 +14,28 @@
             "developmentStatus": null,
             "intendedAudience": null
         },
         "commonInformationModels": null,
         "description": "{{ objects[0].description }}",
         "id": {
             "group": null,
-            "name": "{{ objects[0].name }}",
+            "name": "{{ objects[0].appid }}",
             "version": "{{ objects[0].version }}"
         },
         "license": {
             "name": null,
             "text": null,
             "uri": null
         },
         "privacyPolicy": {
             "name": null,
             "text": null,
             "uri": null
         },
-        "releaseDate": null,
+        "releaseDate": "{{ currentDate }}",
         "releaseNotes": {
             "name": null,
             "text": "./README.md",
             "uri": null
         },
         "title": "{{ objects[0].title }}"
     },
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/detection_count.j2` & `contentctl-4.0.1/contentctl/output/templates/detection_count.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/detection_coverage.j2` & `contentctl-4.0.1/contentctl/output/templates/detection_coverage.j2`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 223f 3e0a 3c73 7667 2078 6d6c 6e73  .0"?>.<svg xmlns
 00000020: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
 00000030: 6f72 672f 3230 3030 2f73 7667 2220 7769  org/2000/svg" wi
-00000040: 6474 683d 2231 3030 2220 6865 6967 6874  dth="100" height
+00000040: 6474 683d 2231 3330 2220 6865 6967 6874  dth="130" height
 00000050: 3d22 3230 223e 0a3c 6c69 6e65 6172 4772  ="20">.<linearGr
 00000060: 6164 6965 6e74 2069 643d 2261 2220 7832  adient id="a" x2
 00000070: 3d22 3022 2079 323d 2231 3030 2522 3e0a  ="0" y2="100%">.
 00000080: 2020 3c73 746f 7020 6f66 6673 6574 3d22    <stop offset="
 00000090: 3022 2073 746f 702d 636f 6c6f 723d 2223  0" stop-color="#
 000000a0: 6262 6222 2073 746f 702d 6f70 6163 6974  bbb" stop-opacit
 000000b0: 793d 222e 3122 2f3e 0a20 203c 7374 6f70  y=".1"/>.  <stop
 000000c0: 206f 6666 7365 743d 2232 2220 7374 6f70   offset="2" stop
 000000d0: 2d6f 7061 6369 7479 3d22 2e31 222f 3e0a  -opacity=".1"/>.
 000000e0: 3c2f 6c69 6e65 6172 4772 6164 6965 6e74  </linearGradient
 000000f0: 3e0a 0a3c 7265 6374 2072 783d 2233 2220  >..<rect rx="3" 
-00000100: 7769 6474 683d 2236 3022 2068 6569 6768  width="60" heigh
+00000100: 7769 6474 683d 2239 3022 2068 6569 6768  width="90" heigh
 00000110: 743d 2232 3022 2066 696c 6c3d 2223 3535  t="20" fill="#55
 00000120: 3522 2f3e 203c 212d 2d20 436f 6d6d 656e  5"/> <!-- Commen
 00000130: 7420 2d2d 3e0a 3c72 6563 7420 7278 3d22  t -->.<rect rx="
-00000140: 3322 2078 3d22 3630 2220 7769 6474 683d  3" x="60" width=
+00000140: 3322 2078 3d22 3930 2220 7769 6474 683d  3" x="90" width=
 00000150: 2234 3022 2068 6569 6768 743d 2232 3022  "40" height="20"
 00000160: 2066 696c 6c3d 2223 3463 3122 2f3e 0a0a   fill="#4c1"/>..
-00000170: 3c70 6174 6820 6669 6c6c 3d22 2334 6331  <path fill="#4c1
-00000180: 2220 643d 224d 3538 2030 6834 7632 3068  " d="M58 0h4v20h
-00000190: 2d34 7a22 2f3e 0a0a 3c72 6563 7420 7278  -4z"/>..<rect rx
-000001a0: 3d22 3322 2077 6964 7468 3d22 3130 3022  ="3" width="100"
-000001b0: 2068 6569 6768 743d 2232 3022 2066 696c   height="20" fil
-000001c0: 6c3d 2275 726c 2823 6129 222f 3e0a 3c67  l="url(#a)"/>.<g
-000001d0: 2066 696c 6c3d 2223 6666 6622 2074 6578   fill="#fff" tex
-000001e0: 742d 616e 6368 6f72 3d22 6d69 6464 6c65  t-anchor="middle
-000001f0: 2220 666f 6e74 2d66 616d 696c 793d 2244  " font-family="D
-00000200: 656a 6156 7520 5361 6e73 2c56 6572 6461  ejaVu Sans,Verda
-00000210: 6e61 2c47 656e 6576 612c 7361 6e73 2d73  na,Geneva,sans-s
-00000220: 6572 6966 2220 666f 6e74 2d73 697a 653d  erif" font-size=
-00000230: 2231 3122 3e0a 2020 2020 3c74 6578 7420  "11">.    <text 
-00000240: 783d 2233 3022 2079 3d22 3134 223e 636f  x="30" y="14">co
-00000250: 7665 7261 6765 3c2f 7465 7874 3e0a 2020  verage</text>.  
-00000260: 2020 3c74 6578 7420 783d 2238 3022 2079    <text x="80" y
-00000270: 3d22 3134 223e 7b7b 206f 626a 6563 742e  ="14">{{ object.
-00000280: 636f 7665 7261 6765 207d 7d3c 2f74 6578  coverage }}</tex
-00000290: 743e 0a3c 2f67 3e0a 3c2f 7376 673e 0a    t>.</g>.</svg>.
+00000170: 3c72 6563 7420 7278 3d22 3322 2077 6964  <rect rx="3" wid
+00000180: 7468 3d22 3130 3022 2068 6569 6768 743d  th="100" height=
+00000190: 2232 3022 2066 696c 6c3d 2275 726c 2823  "20" fill="url(#
+000001a0: 6129 222f 3e0a 3c67 2066 696c 6c3d 2223  a)"/>.<g fill="#
+000001b0: 6666 6622 2074 6578 742d 616e 6368 6f72  fff" text-anchor
+000001c0: 3d22 6c65 6674 2220 666f 6e74 2d66 616d  ="left" font-fam
+000001d0: 696c 793d 2244 656a 6156 7520 5361 6e73  ily="DejaVu Sans
+000001e0: 2c56 6572 6461 6e61 2c47 656e 6576 612c  ,Verdana,Geneva,
+000001f0: 7361 6e73 2d73 6572 6966 2220 666f 6e74  sans-serif" font
+00000200: 2d73 697a 653d 2231 3122 3e0a 2020 2020  -size="11">.    
+00000210: 3c74 6578 7420 783d 2235 2220 793d 2231  <text x="5" y="1
+00000220: 3422 3e25 2050 726f 6475 6374 696f 6e3c  4">% Production<
+00000230: 2f74 6578 743e 0a20 2020 203c 7465 7874  /text>.    <text
+00000240: 2078 3d22 3130 3022 2079 3d22 3134 223e   x="100" y="14">
+00000250: 7b7b 6f62 6a65 6374 2e63 6f76 6572 6167  {{object.coverag
+00000260: 657d 7d3c 2f74 6578 743e 0a3c 2f67 3e0a  e}}</text>.</g>.
+00000270: 3c2f 7376 673e 0a                        </svg>.
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/doc_detection_page.j2` & `contentctl-4.0.1/contentctl/output/templates/doc_detection_page.j2`

 * *Files 24% similar despite different names*

```diff
@@ -8,12 +8,12 @@
   nav: "detections"
 ---
 
 | Name           | Technique       | Type            |
 | -------------- | --------------- | --------------- |
 {%- for detection in objects -%}
 {% if detection.tags.mitre_attack_enrichments %}
-| [{{ detection.name }}](/{{ detection.source }}/{{ detection.name | lower | replace(' ', '_') }}/) | {% for attack in detection.tags.mitre_attack_enrichments -%} [{{ attack.mitre_attack_technique }}](/tags/#{{ attack.mitre_attack_technique | lower | replace(" ", "-") }}){% if not loop.last -%}, {% endif -%}{%- endfor %} | [{{ detection.type }}](https://github.com/splunk/security_content/wiki/Detection-Analytic-Types) |
+| [{{ detection.name }}](/{{ detection.getSource() }}/{{ detection.name | lower | replace(' ', '_') }}/) | {% for attack in detection.tags.mitre_attack_enrichments -%} [{{ attack.mitre_attack_technique }}](/tags/#{{ attack.mitre_attack_technique | lower | replace(" ", "-") }}){% if not loop.last -%}, {% endif -%}{%- endfor %} | [{{ detection.type }}](https://github.com/splunk/security_content/wiki/Detection-Analytic-Types) |
 {%- else %}
-| [{{ detection.name }}](/{{ detection.source }}/{{ detection.name | lower | replace(' ', '_') }}/) | None | [{{ detection.type }}](https://github.com/splunk/security_content/wiki/Detection-Analytic-Types) |
+| [{{ detection.name }}](/{{ detection.getSource() }}/{{ detection.name | lower | replace(' ', '_') }}/) | None | [{{ detection.type }}](https://github.com/splunk/security_content/wiki/Detection-Analytic-Types) |
 {%- endif -%}
 {%- endfor -%}
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/doc_detections.j2` & `contentctl-4.0.1/contentctl/output/templates/doc_detections.j2`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 title: "{{object.name}}"
 excerpt: "{% if object.tags.mitre_attack_enrichments %}{% for attack in object.tags.mitre_attack_enrichments -%}
 {{ attack.mitre_attack_technique }}
 {% if not loop.last -%}, {% endif -%}
 {% endfor %}{% endif -%}"
 categories:
-  - {{object.source|capitalize}}
+  - {{object.getSource()|capitalize}}
 last_modified_at: {{object.date}}
 toc: true
 toc_label: ""
 tags:
 {%- if object.tags.mitre_attack_enrichments %}
 {%- for attack in object.tags.mitre_attack_enrichments %}
   - {{ attack.mitre_attack_technique }}
@@ -203,8 +203,8 @@
 
 {% if object.tags.dataset %}
 {% for dataset in object.tags.dataset -%}
 * [{{dataset}}]({{ dataset }})
 {% endfor %}
 {% endif %}
 
-[*source*](https://github.com/splunk/security_content/tree/develop/detections/{% if object.experimental is sameas true -%}experimental/{%- endif -%}{{object.source}}/{{ object.name | lower | replace (" ", "_") | replace("-", "_") }}.yml) \| *version*: **{{object.version}}**
+[*source*](https://github.com/splunk/security_content/tree/develop/detections/{% if object.experimental is sameas true -%}experimental/{%- endif -%}{{object.getSource()}}/{{ object.name | lower | replace (" ", "_") | replace("-", "_") }}.yml) \| *version*: **{{object.version}}**
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/doc_navigation.j2` & `contentctl-4.0.1/contentctl/output/templates/doc_navigation.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/doc_playbooks.j2` & `contentctl-4.0.1/contentctl/output/templates/doc_playbooks.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/doc_playbooks_page.j2` & `contentctl-4.0.1/contentctl/output/templates/doc_playbooks_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/doc_stories.j2` & `contentctl-4.0.1/contentctl/output/templates/doc_stories.j2`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 #### Detections
 
 | Name        | Technique   | Type         |
 | ----------- | ----------- |--------------|
 {%- if object.detections %}
 {%- for detection in object.detections %}
-| [{{ detection.name }}](/{{ detection.source }}/{{ detection.name | lower | replace(' ', '_') }}/) | {% if detection.tags.mitre_attack_enrichments %}{% for attack in detection.tags.mitre_attack_enrichments -%}[{{ attack.mitre_attack_technique }}](/tags/#{{ attack.mitre_attack_technique | lower | replace(" ", "-") }}){% if not loop.last %}, {% endif %}{%- endfor %}{% else %}None{%- endif -%} | {{ detection.type }} |
+| [{{ detection.name }}](/{{ detection.getSource() }}/{{ detection.name | lower | replace(' ', '_') }}/) | {% if detection.tags.mitre_attack_enrichments %}{% for attack in detection.tags.mitre_attack_enrichments -%}[{{ attack.mitre_attack_technique }}](/tags/#{{ attack.mitre_attack_technique | lower | replace(" ", "-") }}){% if not loop.last %}, {% endif %}{%- endfor %}{% else %}None{%- endif -%} | {{ detection.type }} |
 {%- endfor %}
 {%- endif %}
 
 #### Reference
 {% if object.references %}
 {% for reference in object.references -%}
 * [{{ reference }}]({{ reference }})
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/doc_story_page.j2` & `contentctl-4.0.1/contentctl/output/templates/doc_story_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/es_investigations_investigations.j2` & `contentctl-4.0.1/contentctl/output/templates/es_investigations_investigations.j2`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 
 {% for response_task in objects %}
 [panel://workbench_panel_{{ response_task.lowercase_name }}___response_task]
 label = {{ response_task.name }}
-description = {{ response_task.description }}
+description = {{ response_task.description | escapeNewlines() }}
 disabled = 0
 tokens = {\
 {% for token in response_task.inputs %}
 {% if token == 'user' %}
-    "user": {\
-      "valuePrefix": "\"",\
-      "valueSuffix": "\"",\
-      "delimiter": " OR {{ token }}=",\
-      "valueType": "primitive",\
-      "value": "identity",\
-      "default": "null"\
-    }{% elif token == 'dest'%}
+  "user": {\
+    "valuePrefix": "\"",\
+    "valueSuffix": "\"",\
+    "delimiter": " OR {{ token }}=",\
+    "valueType": "primitive",\
+    "value": "identity",\
+    "default": "null"\
+    }\{% elif token == 'dest'%}
     "dest": {\
       "valuePrefix": "\"",\
       "valueSuffix": "\"",\
       "delimiter": " OR {{ token }}=",\
       "valueType": "primitive",\
       "value": "asset",\
       "default": "null"\
-    }{% else %}
+    }\{% else %}
     "{{ token }}": {\
       "valuePrefix": "\"",\
       "valueSuffix": "\"",\
       "delimiter": " OR {{ token }}=",\
       "valueType": "primitive",\
       "value": "file",\
       "default": "null"\
-    }{% endif %}{{ "," if not loop.last }}\
+    }\{% endif %}{{ "," if not loop.last }}
 {% endfor %}
-}\
+  }\
 
 
 {% endfor %}
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/finding_report.j2` & `contentctl-4.0.1/contentctl/output/templates/finding_report.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/savedsearches_baselines.j2` & `contentctl-4.0.1/contentctl/output/templates/savedsearches_baselines.j2`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 {% for detection in objects %}
 {% if (detection.type == 'Baseline') %}
 [{{APP_NAME}} - {{ detection.name }}]
 action.escu = 0
 action.escu.enabled = 1
 action.escu.search_type = support
 action.escu.full_search_name = {{APP_NAME}} - {{ detection.name }}
-description = {{ detection.description }}
+description = {{ detection.description | escapeNewlines() }}
 action.escu.creation_date = {{ detection.date }}
 action.escu.modification_date = {{ detection.date }}
 {% if detection.tags.analytic_story is defined %}
-action.escu.analytic_story = {{ detection.tags.analytic_story | tojson }}
+action.escu.analytic_story = {{ objectListToNameList(detection.tags.analytic_story) | tojson }}
 {% else %}
 action.escu.analytic_story = []
 {% endif %}
 action.escu.data_models = {{ detection.datamodel | tojson }}
 cron_schedule = {{ detection.deployment.scheduling.cron_schedule }}
 enableSched = 1
 dispatch.earliest_time = {{ detection.deployment.scheduling.earliest_time }}
@@ -26,24 +26,24 @@
 schedule_window = {{ detection.deployment.scheduling.schedule_window }}
 {% endif %}
 {% if detection.providing_technologies is defined %}
 action.escu.providing_technologies = {{ detection.providing_technologies | tojson }}
 {% else %}
 action.escu.providing_technologies = []
 {% endif %}
-action.escu.eli5 = {{ detection.description }}
+action.escu.eli5 = {{ detection.description | escapeNewlines() }}
 {% if detection.how_to_implement is defined %}
-action.escu.how_to_implement = {{ detection.how_to_implement }}
+action.escu.how_to_implement = {{ detection.how_to_implement | escapeNewlines() }}
 {% else %}
 action.escu.how_to_implement = none
 {% endif %}
 {% if detection.disabled is defined %}
 disabled = false
 {% else %}
 disabled = true
 {% endif %}
 is_visible = false
-search = {{ detection.search }}
+search = {{ detection.search | escapeNewlines() }}
 
 {% endif %}
 {% endfor %}
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/savedsearches_detections.j2` & `contentctl-4.0.1/contentctl/output/templates/savedsearches_detections.j2`

 * *Files 6% similar despite different names*

```diff
@@ -2,51 +2,54 @@
 
 {% for detection in objects %}
 {% if (detection.type == 'TTP' or detection.type == 'Anomaly' or detection.type == 'Hunting' or detection.type == 'Correlation') %}
 [{{APP_NAME}} - {{ detection.name }} - Rule]
 action.escu = 0
 action.escu.enabled = 1
 {% if detection.status == "deprecated" %}
-description = **WARNING**, this detection has been marked **DEPRECATED** by the Splunk Threat Research Team. This means that it will no longer be maintained or supported. If you have any questions feel free to email us at: research@splunk.com. {{ detection.description }}
+description = **WARNING**, this detection has been marked **DEPRECATED** by the Splunk Threat Research Team. This means that it will no longer be maintained or supported. If you have any questions feel free to email us at: research@splunk.com. {{ detection.description | escapeNewlines() }} 
 {% elif detection.status == "experimental" %}
-description = **WARNING**, this detection is marked **EXPERIMENTAL** by the Splunk Threat Research Team. This means that the detection has been manually tested but we do not have the associated attack data to perform automated testing or cannot share this attack dataset due to its sensitive nature. If you have any questions feel free to email us at: research@splunk.com. {{ detection.description }} 
+description = **WARNING**, this detection is marked **EXPERIMENTAL** by the Splunk Threat Research Team. This means that the detection has been manually tested but we do not have the associated attack data to perform automated testing or cannot share this attack dataset due to its sensitive nature. If you have any questions feel free to email us at: research@splunk.com. {{ detection.description | escapeNewlines() }} 
 {% else %}
-description = {{ detection.description }}
+description = {{ detection.description | escapeNewlines() }}
 {% endif %}
 action.escu.mappings = {{ detection.mappings | tojson }}
 action.escu.data_models = {{ detection.datamodel | tojson }}
-action.escu.eli5 = {{ detection.description }}
-{% if detection.how_to_implement is defined %}
-action.escu.how_to_implement = {{ detection.how_to_implement }}
+action.escu.eli5 = {{ detection.description | escapeNewlines() }}
+{% if detection.how_to_implement %}
+action.escu.how_to_implement = {{ detection.how_to_implement | escapeNewlines() }}
 {% else %}
 action.escu.how_to_implement = none
 {% endif %}
-{% if detection.known_false_positives is defined %}
-action.escu.known_false_positives = {{ detection.known_false_positives }}
+{% if detection.known_false_positives %}
+action.escu.known_false_positives = {{ detection.known_false_positives | escapeNewlines() }}
 {% else %}
 action.escu.known_false_positives = None
 {% endif %}
 action.escu.creation_date = {{ detection.date }}
 action.escu.modification_date = {{ detection.date }}
 action.escu.confidence = high
 action.escu.full_search_name = {{APP_NAME}} - {{ detection.name }} - Rule
 action.escu.search_type = detection
 {% if detection.tags.product is defined %}
 action.escu.product = {{ detection.tags.product | tojson }}
 {% endif %}
-{% if detection.providing_technologies is defined %}
+{% if detection.tags.atomic_guid %}
+action.escu.atomic_red_team_guids = {{ detection.tags.getAtomicGuidStringArray() | tojson }}
+{% endif %}
+{% if detection.providing_technologies | length > 0  %}
 action.escu.providing_technologies = {{ detection.providing_technologies | tojson }}
 {% else %}
-action.escu.providing_technologies = []
+action.escu.providing_technologies = null
 {% endif %}
-{% if detection.tags.analytic_story is defined %}
-action.escu.analytic_story = {{ detection.tags.analytic_story | tojson }}
-{% if detection.deployment.rba.enabled is defined %}
+{% if detection.tags.analytic_story %}
+action.escu.analytic_story = {{ objectListToNameList(detection.tags.analytic_story) | tojson }}
+{% if detection.deployment.alert_action.rba.enabled%}
 action.risk = 1
-action.risk.param._risk_message = {{ detection.tags.message }}
+action.risk.param._risk_message = {{ detection.tags.message | escapeNewlines() }}
 action.risk.param._risk = {{ detection.risk | tojson }}
 action.risk.param._risk_score = 0
 action.risk.param.verbose = 0
 {% endif %}
 {% else %}
 action.escu.analytic_story = []
 {% endif %}
@@ -65,42 +68,42 @@
 {% endif %}
 action.correlationsearch.annotations = {{ detection.annotations | tojson }}
 action.correlationsearch.metadata = {{ detection.getMetadata() | tojson }}
 {% if detection.deployment.scheduling.schedule_window is defined %}
 schedule_window = {{ detection.deployment.scheduling.schedule_window }}
 {% endif %}
 {% if detection.deployment is defined %}
-{% if detection.deployment.notable.rule_title is defined %}
+{% if detection.deployment.alert_action.notable %}
 action.notable = 1
-{% if detection.nes_fields is defined %}
+{% if detection.nes_fields %}
 action.notable.param.nes_fields = {{ detection.nes_fields }}
 {% endif %}
-action.notable.param.rule_description = {{ detection.deployment.notable.rule_description | custom_jinja2_enrichment_filter(detection) }}
-action.notable.param.rule_title = {% if detection.type | lower == "correlation" %}RBA: {{ detection.deployment.notable.rule_title | custom_jinja2_enrichment_filter(detection) }}{% else %}{{ detection.deployment.notable.rule_title | custom_jinja2_enrichment_filter(detection) }}{% endif +%}
-action.notable.param.security_domain = {{ detection.tags.security_domain }}
+action.notable.param.rule_description = {{ detection.deployment.alert_action.notable.rule_description | custom_jinja2_enrichment_filter(detection) | escapeNewlines()}}
+action.notable.param.rule_title = {% if detection.type | lower == "correlation" %}RBA: {{ detection.deployment.alert_action.notable.rule_title | custom_jinja2_enrichment_filter(detection) }}{% else %}{{ detection.deployment.alert_action.notable.rule_title | custom_jinja2_enrichment_filter(detection) }}{% endif +%}
+action.notable.param.security_domain = {{ detection.tags.security_domain.value }}
 action.notable.param.severity = high
 {% endif %}
-{% if detection.deployment.email.to is defined %}
-action.email.subject.alert = {{ detection.deployment.email.subject | custom_jinja2_enrichment_filter(detection) }}
-action.email.to = {{ detection.deployment.email.to }}
-action.email.message.alert = {{ detection.deployment.email.message | custom_jinja2_enrichment_filter(detection) }}
+{% if detection.deployment.alert_action.email %}
+action.email.subject.alert = {{ detection.deployment.alert_action.email.subject | custom_jinja2_enrichment_filter(detection) | escapeNewlines() }}
+action.email.to = {{ detection.deployment.alert_action.email.to }}
+action.email.message.alert = {{ detection.deployment.alert_action.email.message | custom_jinja2_enrichment_filter(detection) | escapeNewlines() }}
 action.email.useNSSubject = 1
 {% endif %}
-{% if detection.deployment.slack.channel is defined %}
+{% if detection.deployment.alert_action.slack %}
 action.slack = 1
-action.slack.param.channel = {{ detection.deployment.slack.channel | custom_jinja2_enrichment_filter(detection) }}
-action.slack.param.message = {{ detection.deployment.slack.message | custom_jinja2_enrichment_filter(detection) }}
+action.slack.param.channel = {{ detection.deployment.alert_action.slack.channel | custom_jinja2_enrichment_filter(detection) | escapeNewlines() }}
+action.slack.param.message = {{ detection.deployment.alert_action.slack.message | custom_jinja2_enrichment_filter(detection) | escapeNewlines() }}
 {% endif %}
-{% if detection.deployment.phantom.phantom_server is defined %}
+{% if detection.deployment.alert_action.phantom%}
 action.sendtophantom = 1
-action.sendtophantom.param._cam_workers = {{ detection.deployment.phantom.cam_workers | custom_jinja2_enrichment_filter(detection) }}
-action.sendtophantom.param.label = {{ detection.deployment.phantom.label | custom_jinja2_enrichment_filter(detection) }}
-action.sendtophantom.param.phantom_server = {{ detection.deployment.phantom.phantom_server | custom_jinja2_enrichment_filter(detection) }}
-action.sendtophantom.param.sensitivity = {{ detection.deployment.phantom.sensitivity | custom_jinja2_enrichment_filter(detection) }}
-action.sendtophantom.param.severity = {{ detection.deployment.phantom.severity | custom_jinja2_enrichment_filter(detection) }}
+action.sendtophantom.param._cam_workers = {{ detection.deployment.alert_action.phantom.cam_workers | custom_jinja2_enrichment_filter(detection) }}
+action.sendtophantom.param.label = {{ detection.deployment.alert_action.phantom.label | custom_jinja2_enrichment_filter(detection) }}
+action.sendtophantom.param.phantom_server = {{ detection.deployment.alert_action.phantom.phantom_server | custom_jinja2_enrichment_filter(detection) }}
+action.sendtophantom.param.sensitivity = {{ detection.deployment.alert_action.phantom.sensitivity | custom_jinja2_enrichment_filter(detection) }}
+action.sendtophantom.param.severity = {{ detection.deployment.alert_action.phantom.severity | custom_jinja2_enrichment_filter(detection) }}
 {% endif %}
 {% endif %}
 alert.digest_mode = 1
 {% if detection.enabled_by_default %}
 disabled = false
 {% else %}
 disabled = true
@@ -108,12 +111,12 @@
 enableSched = 1
 allow_skew = 100%
 counttype = number of events
 relation = greater than
 quantity = 0
 realtime_schedule = 0
 is_visible = false
-search = {{ detection.search }}
+search = {{ detection.search | escapeNewlines() }}
 
 {% endif %}
 {% endfor %}
 ### END {{ APP_NAME }} DETECTIONS ###
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/savedsearches_investigations.j2` & `contentctl-4.0.1/contentctl/output/templates/savedsearches_investigations.j2`

 * *Files 8% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 {% if (detection.type == 'Investigation') %}
 {% if detection.search is defined %}
 [{{APP_NAME}} - {{ detection.name }} - Response Task]
 action.escu = 0
 action.escu.enabled = 1
 action.escu.search_type = investigative
 action.escu.full_search_name = {{APP_NAME}} - {{ detection.name }} - Response Task
-description = {{ detection.description }}
+description = {{ detection.description | escapeNewlines() }}
 action.escu.creation_date = {{ detection.date }}
 action.escu.modification_date = {{ detection.date }}
 {% if detection.tags.analytic_story is defined %}
-action.escu.analytic_story = {{ detection.tags.analytic_story | tojson }}
+action.escu.analytic_story = {{ objectListToNameList(detection.tags.analytic_story) | tojson }}
 {% else %}
 action.escu.analytic_story = []
 {% endif %}
 action.escu.earliest_time_offset = 3600
 action.escu.latest_time_offset = 86400
 action.escu.providing_technologies = []
 action.escu.data_models = {{ detection.datamodel | tojson }}
-action.escu.eli5 = {{ detection.description }}
+action.escu.eli5 = {{ detection.description | escapeNewlines() }}
 action.escu.how_to_implement = none
 action.escu.known_false_positives = None at this time
 disabled = true
 schedule_window = auto
 is_visible = false
-search = {{ detection.search }}
+search = {{ detection.search | escapeNewlines() }}
 
 {% endif %}
 {% endif %}
 {% endfor %}
 
 
 ### END {{ APP_NAME }} RESPONSE TASKS ###
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_story_detail.txt` & `contentctl-4.0.1/contentctl/templates/app_template/README/essoc_story_detail.txt`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_summary.txt` & `contentctl-4.0.1/contentctl/templates/app_template/README/essoc_summary.txt`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/README/essoc_usage_dashboard.txt` & `contentctl-4.0.1/contentctl/templates/app_template/README/essoc_usage_dashboard.txt`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/default/app.conf` & `contentctl-4.0.1/contentctl/templates/app_template/default/app.conf`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/default/data/ui/views/escu_summary.xml` & `contentctl-4.0.1/contentctl/templates/app_template/default/data/ui/views/escu_summary.xml`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/default/data/ui/views/feedback.xml` & `contentctl-4.0.1/contentctl/templates/app_template/default/data/ui/views/feedback.xml`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/default/usage_searches.conf` & `contentctl-4.0.1/contentctl/templates/app_template/default/usage_searches.conf`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIcon.png` & `contentctl-4.0.1/contentctl/templates/app_template/static/appIcon.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIconAlt.png` & `contentctl-4.0.1/contentctl/templates/app_template/static/appIconAlt.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIconAlt_2x.png` & `contentctl-4.0.1/contentctl/templates/app_template/static/appIconAlt_2x.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/splunk_app/static/appIcon_2x.png` & `contentctl-4.0.1/contentctl/templates/app_template/static/appIcon_2x.png`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/templates/transforms.j2` & `contentctl-4.0.1/contentctl/output/templates/transforms.j2`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 {% for lookup in objects %}
 [{{ lookup.name }}]
 {% if lookup.filename is defined and lookup.filename != None %}
-filename = {{ lookup.filename  }}
+filename = {{ lookup.filename.name  }}
 {% else %}
 collection = {{ lookup.collection }}
 external_type = kvstore
 {% endif %}
 {% if lookup.default_match is defined and lookup.default_match != None  %}
-default_match = {{ lookup.default_match }}
+default_match = {{ lookup.default_match | lower }}
 {% endif %}
 {% if lookup.case_sensitive_match is defined and lookup.case_sensitive_match != None %}
-case_sensitive_match = {{ lookup.case_sensitive_match }}
+case_sensitive_match = {{ lookup.case_sensitive_match | lower }}
 {% endif %}
 {% if lookup.description is defined and lookup.description != None %}
-# description = {{ lookup.description }}
+# description = {{ lookup.description | escapeNewlines() }}
 {% endif %}
 {% if lookup.match_type is defined and lookup.match_type != None %}
 match_type = {{ lookup.match_type }}
 {% endif %}
 {% if lookup.max_matches is defined and lookup.max_matches != None %}
 max_matches = {{ lookup.max_matches }}
 {% endif %}
```

### Comparing `contentctl-3.6.0/contentctl/output/templates/workflow_actions.j2` & `contentctl-4.0.1/contentctl/output/templates/workflow_actions.j2`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/output/yml_output.py` & `contentctl-4.0.1/contentctl/output/yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/templates/app_default.yml` & `contentctl-4.0.1/contentctl/templates/app_default.yml`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/templates/datamodels_cim.conf` & `contentctl-4.0.1/contentctl/templates/datamodels_cim.conf`

 * *Files identical despite different names*

### Comparing `contentctl-3.6.0/contentctl/templates/deployments/00_default_correlation.yml` & `contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_correlation.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 name: ESCU Default Configuration Correlation
 id: 36ba498c-46e8-4b62-8bde-67e984a40fb4
 date: '2021-12-21'
 author: Patrick Bareiss
+type: Correlation
 description: This configuration file applies to all detections of type Correlation.
   These correlations will generate Notable Events.
 scheduling:
   cron_schedule: 0 * * * *
   earliest_time: -70m@m
   latest_time: -10m@m
   schedule_window: auto
 alert_action:
   notable:
     rule_description: '%description%'
     rule_title: '%name%'
     nes_fields: 
     - user
     - dest
-tags:
-  type: 'Correlation'
+
```

### Comparing `contentctl-3.6.0/contentctl/templates/deployments/00_default_ttp.yml` & `contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_ttp.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 name: ESCU Default Configuration TTP
 id: b81cd059-a3e8-4c03-96ca-e168c50ff70b
 date: '2021-12-21'
 author: Patrick Bareiss
+type: TTP
 description: This configuration file applies to all detections of type TTP.
   These detections will use Risk Based Alerting and generate Notable Events.
 scheduling:
   cron_schedule: 0 * * * *
   earliest_time: -70m@m
   latest_time: -10m@m
   schedule_window: auto
@@ -14,9 +15,7 @@
     rule_description: '%description%'
     rule_title: '%name%'
     nes_fields: 
     - user 
     - dest
   rba:
     enabled: 'true'
-tags:
-  type: TTP
```

### Comparing `contentctl-3.6.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml` & `contentctl-4.0.1/contentctl/templates/detections/anomalous_usage_of_7zip.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 references:
 - https://attack.mitre.org/techniques/T1560/001/
 - https://www.microsoft.com/security/blog/2021/01/20/deep-dive-into-the-solorigate-second-stage-activation-from-sunburst-to-teardrop-and-raindrop/
 - https://thedfirreport.com/2021/01/31/bazar-no-ryuk/
 tags:
   analytic_story:
   - Cobalt Strike
-  - NOBELIUM Group
   asset_type: Endpoint
   confidence: 80
   impact: 80
   message: An instance of $parent_process_name$ spawning $process_name$ was identified
     on endpoint $dest$ by user $user$. This behavior is indicative of suspicious loading
     of 7zip.
   mitre_attack_id:
```

### Comparing `contentctl-3.6.0/contentctl/templates/stories/cobalt_strike.yml` & `contentctl-4.0.1/contentctl/templates/stories/cobalt_strike.yml`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 - https://www.infocyte.com/blog/2020/09/02/cobalt-strike-the-new-favorite-among-thieves/
 - https://bluescreenofjeff.com/2017-01-24-how-to-write-malleable-c2-profiles-for-cobalt-strike/
 - https://blog.talosintelligence.com/2020/09/coverage-strikes-back-cobalt-strike-paper.html
 - https://www.fireeye.com/blog/threat-research/2020/12/unauthorized-access-of-fireeye-red-team-tools.html
 - https://github.com/MichaelKoczwara/Awesome-CobaltStrike-Defence
 - https://github.com/zer0yu/Awesome-CobaltStrike
 tags:
-  analytic_story: Cobalt Strike
   category:
   - Adversary Tactics
   product:
   - Splunk Enterprise
   - Splunk Enterprise Security
   - Splunk Cloud
   usecase: Advanced Threat Detection
```

### Comparing `contentctl-3.6.0/pyproject.toml` & `contentctl-4.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [tool.poetry]
 name = "contentctl"
-version = "3.6.0"
+version = "4.0.1"
 description = "Splunk Content Control Tool"
 authors = ["STRT <research@splunk.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 contentctl = 'contentctl.contentctl:main'
 
 [tool.poetry.dependencies]
-python = "^3.9"
-pydantic = "^1.10.11"
-PyYAML = "^6.0"
-requests = "^2.28.1"
+python = "^3.11"
+pydantic = "^2.5.1"
+PyYAML = "^6.0.1"
+requests = "^2.31.0"
 pycvesearch = "^1.2"
 xmltodict = "^0.13.0"
 attackcti = "^0.3.7"
 Jinja2 = "^3.1.2"
-questionary = "^1.10.0"
-gitpython = "^3.1.29"
-docker = "^6.0.1"
-splunk-sdk = "^1.7.2"
-validators = "^0.20.0"
+questionary = "^2.0.1"
+docker = "^6.1.3"
+splunk-sdk = "^2.0.1"
+validators = "^0.22.0"
 semantic-version = "^2.10.0"
-bottle = "^0.12.23"
-tqdm = "^4.65.0"
+bottle = "^0.12.25"
+tqdm = "^4.66.1"
 #splunk-appinspect = "^2.36.0"
-pysigma = "^0.10.5"
+pysigma = "^0.10.8"
 pysigma-backend-splunk = "^1.0.3"
-
+pygit2 = "^1.14.1"
+tyro = "^0.8.3"
+gitpython = "^3.1.43"
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `contentctl-3.6.0/PKG-INFO` & `contentctl-4.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: contentctl
-Version: 3.6.0
+Version: 4.0.1
 Summary: Splunk Content Control Tool
 License: Apache 2.0
 Author: STRT
 Author-email: research@splunk.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: attackcti (>=0.3.7,<0.4.0)
-Requires-Dist: bottle (>=0.12.23,<0.13.0)
-Requires-Dist: docker (>=6.0.1,<7.0.0)
-Requires-Dist: gitpython (>=3.1.29,<4.0.0)
+Requires-Dist: bottle (>=0.12.25,<0.13.0)
+Requires-Dist: docker (>=6.1.3,<7.0.0)
+Requires-Dist: gitpython (>=3.1.43,<4.0.0)
 Requires-Dist: pycvesearch (>=1.2,<2.0)
-Requires-Dist: pydantic (>=1.10.11,<2.0.0)
-Requires-Dist: pysigma (>=0.10.5,<0.11.0)
+Requires-Dist: pydantic (>=2.5.1,<3.0.0)
+Requires-Dist: pygit2 (>=1.14.1,<2.0.0)
+Requires-Dist: pysigma (>=0.10.8,<0.11.0)
 Requires-Dist: pysigma-backend-splunk (>=1.0.3,<2.0.0)
-Requires-Dist: questionary (>=1.10.0,<2.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: questionary (>=2.0.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
-Requires-Dist: splunk-sdk (>=1.7.2,<2.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: validators (>=0.20.0,<0.21.0)
+Requires-Dist: splunk-sdk (>=2.0.1,<3.0.0)
+Requires-Dist: tqdm (>=4.66.1,<5.0.0)
+Requires-Dist: tyro (>=0.8.3,<0.9.0)
+Requires-Dist: validators (>=0.22.0,<0.23.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 
 # contentctl
 <p align="center">
 <img src="docs/contentctl_logo_white.png" title="In case you're wondering, it's a capybara" alt="contentctl logo" width="250" height="250"></p>
@@ -207,15 +207,36 @@
 2. **new** - Creates new content (detection, story)
 3. **validate** - Validates written content
 4. **build** - Builds an application suitable for deployment on a search head using Slim, the Splunk Packaging Toolkit
 5. **deploy** - Deploy the security content pack to a Splunk Server
 6. **docs** - Create documentation as Markdown
 7. **reporting** - Create different reporting files such as a Mitre ATT&CK overlay
 
+# Shell tab-complete
 
+Leveraging the tab completion featureset of the CLI library we're using, you can generate tab completions for `contentctl` automatically, for zsh, bash, and tcsh. For additional details, you can view the docs for the library [here.](https://brentyi.github.io/tyro/tab_completion/) 
+
+### Zsh
+If you already have a location for your ZSH tab completions, you only need to run the generation line and can skip the folder creation, configuring the rest to fit with your shell config.
+
+```zsh
+mkdir -p ~/.zfunc
+contentctl --tyro-write-completion zsh ~/.zfunc/_contentctl
+echo "fpath+=~/.zfunc" >> ~/.zshrc
+echo "autoload -Uz compinit && compinit" >> ~/.zshrc
+source ~/.zshrc
+```
+
+### Bash
+
+```bash
+completion_dir=${BASH_COMPLETION_USER_DIR:-${XDG_DATA_HOME:-$HOME/.local/share}/bash-completion}/completions/
+mkdir -p $completion_dir
+contentctl --tyro-write-completion bash ${completion_dir}/_contentctl
+```
 
 # Acronyms
 | Acronym | Meaning| Description | 
 | --------------------- | ------------------------------------------------------- | ---- |
 | SOC | Security Operation Center | Description of a SoC | 
 | DaC | Detection as Code | A systematic approach applying DevOps priciples to Detection Engineering. DaC enables Continuous Integration and Continuous Delivery of Detectionsa via automated validation, testing, and deployment |
 | CICD | Continuous Integration/Continuous Delivery | A modern DevOps practice that encourages users to make small, frequent changes which are automatically tested and deployed. This contrasts with legacy approaches that emphasize large changes which may be manually tested an infrequently deployed. |
```

